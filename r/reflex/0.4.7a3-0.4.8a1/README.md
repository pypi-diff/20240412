# Comparing `tmp/reflex-0.4.7a3.tar.gz` & `tmp/reflex-0.4.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.4.7a3.tar", max compression
+gzip compressed data, was "reflex-0.4.8a1.tar", max compression
```

## Comparing `reflex-0.4.7a3.tar` & `reflex-0.4.8a1.tar`

### file list

```diff
@@ -1,508 +1,510 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.4.7a3/LICENSE
--rw-r--r--   0        0        0     9568 2024-04-04 21:37:03.943217 reflex-0.4.7a3/README.md
--rw-r--r--   0        0        0     2922 2024-04-09 01:49:54.817202 reflex-0.4.7a3/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-11-07 19:58:07.469572 reflex-0.4.7a3/reflex/.templates/apps/blank/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-11-07 19:58:07.469657 reflex-0.4.7a3/reflex/.templates/apps/blank/code/__init__.py
--rw-r--r--   0        0        0      861 2024-04-05 00:24:11.496563 reflex-0.4.7a3/reflex/.templates/apps/blank/code/blank.py
--rw-r--r--   0        0        0       32 2023-11-07 19:58:07.469933 reflex-0.4.7a3/reflex/.templates/apps/demo/.gitignore
--rw-r--r--   0        0        0     4286 2023-11-07 19:58:07.470079 reflex-0.4.7a3/reflex/.templates/apps/demo/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-07 19:58:07.470183 reflex-0.4.7a3/reflex/.templates/apps/demo/assets/github.svg
--rw-r--r--   0        0        0     1899 2023-11-07 19:58:07.470263 reflex-0.4.7a3/reflex/.templates/apps/demo/assets/icon.svg
--rw-r--r--   0        0        0     5403 2023-11-07 19:58:07.470351 reflex-0.4.7a3/reflex/.templates/apps/demo/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-07 19:58:07.470441 reflex-0.4.7a3/reflex/.templates/apps/demo/assets/paneleft.svg
--rw-r--r--   0        0        0       32 2023-11-07 19:58:07.470556 reflex-0.4.7a3/reflex/.templates/apps/demo/code/__init__.py
--rw-r--r--   0        0        0     2928 2024-04-02 19:14:34.394285 reflex-0.4.7a3/reflex/.templates/apps/demo/code/demo.py
--rw-r--r--   0        0        0      194 2023-11-07 19:58:07.470763 reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/__init__.py
--rw-r--r--   0        0        0      706 2024-04-02 19:14:34.394398 reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/chatapp.py
--rw-r--r--   0        0        0    10910 2024-04-02 19:14:34.394812 reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/datatable.py
--rw-r--r--   0        0        0     8383 2024-04-02 19:14:34.395299 reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/forms.py
--rw-r--r--   0        0        0     8519 2024-04-02 19:14:34.395551 reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/graphing.py
--rw-r--r--   0        0        0     1822 2024-04-02 19:14:34.395723 reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/home.py
--rw-r--r--   0        0        0     4722 2024-04-02 19:14:34.395853 reflex-0.4.7a3/reflex/.templates/apps/demo/code/sidebar.py
--rw-r--r--   0        0        0      510 2023-11-07 19:58:07.471657 reflex-0.4.7a3/reflex/.templates/apps/demo/code/state.py
--rw-r--r--   0        0        0      912 2023-11-07 19:58:07.471802 reflex-0.4.7a3/reflex/.templates/apps/demo/code/states/form_state.py
--rw-r--r--   0        0        0     1189 2023-11-07 19:58:07.471905 reflex-0.4.7a3/reflex/.templates/apps/demo/code/states/pie_state.py
--rw-r--r--   0        0        0     1486 2024-04-02 19:14:34.395963 reflex-0.4.7a3/reflex/.templates/apps/demo/code/styles.py
--rw-r--r--   0        0        0        0 2023-11-07 19:58:07.472085 reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/__init__.py
--rw-r--r--   0        0        0      120 2023-11-07 19:58:07.472204 reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/__init__.py
--rw-r--r--   0        0        0     3584 2024-04-02 19:14:34.396085 reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/chat.py
--rw-r--r--   0        0        0      680 2023-11-07 19:58:07.472372 reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
--rw-r--r--   0        0        0     1829 2024-04-02 19:14:34.396198 reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/modal.py
--rw-r--r--   0        0        0     2251 2024-04-02 19:14:34.396306 reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/navbar.py
--rw-r--r--   0        0        0     1735 2024-04-02 19:14:34.396392 reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/sidebar.py
--rw-r--r--   0        0        0     4001 2023-11-07 19:58:07.472705 reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/state.py
--rw-r--r--   0        0        0     2281 2024-04-02 19:14:34.396499 reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/styles.py
--rw-r--r--   0        0        0       74 2023-09-18 23:00:36.695709 reflex-0.4.7a3/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      127 2024-04-02 19:14:34.400175 reflex-0.4.7a3/reflex/.templates/jinja/custom_components/README.md.jinja2
--rw-r--r--   0        0        0       32 2024-04-02 19:14:34.401028 reflex-0.4.7a3/reflex/.templates/jinja/custom_components/__init__.py.jinja2
--rw-r--r--   0        0        0      826 2024-04-02 19:14:34.401442 reflex-0.4.7a3/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
--rw-r--r--   0        0        0      614 2024-04-04 21:37:03.945011 reflex-0.4.7a3/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
--rw-r--r--   0        0        0     2403 2024-04-04 21:37:03.945109 reflex-0.4.7a3/reflex/.templates/jinja/custom_components/src.py.jinja2
--rw-r--r--   0        0        0      548 2023-09-25 02:29:12.548714 reflex-0.4.7a3/reflex/.templates/jinja/web/package.json.jinja2
--rw-r--r--   0        0        0      930 2024-04-02 19:14:34.402842 reflex-0.4.7a3/reflex/.templates/jinja/web/pages/_app.js.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.4.7a3/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      400 2024-02-13 04:39:14.427011 reflex-0.4.7a3/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0       86 2023-09-25 02:29:12.549046 reflex-0.4.7a3/reflex/.templates/jinja/web/pages/component.js.jinja2
--rw-r--r--   0        0        0      882 2023-12-04 22:31:51.571558 reflex-0.4.7a3/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0      343 2024-04-04 21:37:03.945229 reflex-0.4.7a3/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0      388 2024-04-04 21:37:03.945317 reflex-0.4.7a3/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
--rw-r--r--   0        0        0      101 2023-12-04 22:31:51.572637 reflex-0.4.7a3/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
--rw-r--r--   0        0        0     3883 2024-02-10 02:26:35.013845 reflex-0.4.7a3/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      141 2023-09-18 23:00:36.695917 reflex-0.4.7a3/reflex/.templates/jinja/web/styles/styles.css.jinja2
--rw-r--r--   0        0        0      436 2024-02-10 02:26:35.013954 reflex-0.4.7a3/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0     3790 2024-04-02 19:14:34.404054 reflex-0.4.7a3/reflex/.templates/jinja/web/utils/context.js.jinja2
--rw-r--r--   0        0        0       37 2023-10-20 19:16:08.667797 reflex-0.4.7a3/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.4.7a3/reflex/.templates/web/.gitignore
--rw-r--r--   0        0        0      595 2023-10-20 19:16:08.667942 reflex-0.4.7a3/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
--rw-r--r--   0        0        0      645 2024-04-02 19:14:34.404228 reflex-0.4.7a3/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
--rw-r--r--   0        0        0       97 2023-09-18 23:00:36.696123 reflex-0.4.7a3/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0      118 2023-11-14 20:34:38.772076 reflex-0.4.7a3/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.4.7a3/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.4.7a3/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     1254 2023-09-06 00:16:27.465104 reflex-0.4.7a3/reflex/.templates/web/utils/client_side_routing.js
--rw-r--r--   0        0        0     1622 2024-02-10 02:26:35.014073 reflex-0.4.7a3/reflex/.templates/web/utils/helpers/dataeditor.js
--rw-r--r--   0        0        0     1152 2023-11-14 20:34:38.772264 reflex-0.4.7a3/reflex/.templates/web/utils/helpers/range.js
--rw-r--r--   0        0        0    21688 2024-04-04 22:32:02.761656 reflex-0.4.7a3/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     5723 2024-04-04 21:37:03.945600 reflex-0.4.7a3/reflex/__init__.py
--rw-r--r--   0        0        0     7649 2024-04-09 00:51:00.940379 reflex-0.4.7a3/reflex/__init__.pyi
--rw-r--r--   0        0        0      108 2023-08-10 23:30:03.955150 reflex-0.4.7a3/reflex/__main__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.4.7a3/reflex/admin.py
--rw-r--r--   0        0        0    44562 2024-04-04 21:37:03.945930 reflex-0.4.7a3/reflex/app.py
--rw-r--r--   0        0        0     5010 2024-04-04 21:37:03.946046 reflex-0.4.7a3/reflex/app.pyi
--rw-r--r--   0        0        0     1152 2024-04-02 19:14:34.406758 reflex-0.4.7a3/reflex/app_module_for_backend.py
--rw-r--r--   0        0        0     4250 2024-04-02 19:14:34.407224 reflex-0.4.7a3/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.4.7a3/reflex/compiler/__init__.py
--rw-r--r--   0        0        0    17037 2024-04-04 21:37:03.946194 reflex-0.4.7a3/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     4344 2024-04-02 19:14:34.407873 reflex-0.4.7a3/reflex/compiler/templates.py
--rw-r--r--   0        0        0    14022 2024-04-06 01:57:36.880131 reflex-0.4.7a3/reflex/compiler/utils.py
--rw-r--r--   0        0        0      530 2024-04-02 19:14:34.408438 reflex-0.4.7a3/reflex/components/__init__.py
--rw-r--r--   0        0        0      325 2024-02-10 02:26:35.019008 reflex-0.4.7a3/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      573 2024-02-10 02:26:35.019123 reflex-0.4.7a3/reflex/components/base/app_wrap.py
--rw-r--r--   0        0        0     2890 2024-04-02 19:14:34.408568 reflex-0.4.7a3/reflex/components/base/app_wrap.pyi
--rw-r--r--   0        0        0     1234 2024-04-02 19:14:34.408691 reflex-0.4.7a3/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-12-21 01:07:08.388770 reflex-0.4.7a3/reflex/components/base/body.py
--rw-r--r--   0        0        0     3277 2024-04-02 19:14:34.408849 reflex-0.4.7a3/reflex/components/base/body.pyi
--rw-r--r--   0        0        0      583 2024-04-02 19:14:34.409155 reflex-0.4.7a3/reflex/components/base/document.py
--rw-r--r--   0        0        0    14587 2024-04-02 19:14:34.409362 reflex-0.4.7a3/reflex/components/base/document.pyi
--rw-r--r--   0        0        0      312 2024-02-10 02:26:35.020357 reflex-0.4.7a3/reflex/components/base/fragment.py
--rw-r--r--   0        0        0     3289 2024-04-02 19:14:34.409517 reflex-0.4.7a3/reflex/components/base/fragment.pyi
--rw-r--r--   0        0        0      297 2023-12-21 01:07:08.390493 reflex-0.4.7a3/reflex/components/base/head.py
--rw-r--r--   0        0        0     6073 2024-04-02 19:14:34.409716 reflex-0.4.7a3/reflex/components/base/head.pyi
--rw-r--r--   0        0        0      929 2023-12-21 01:07:08.390801 reflex-0.4.7a3/reflex/components/base/link.py
--rw-r--r--   0        0        0     7132 2024-04-02 19:14:34.410033 reflex-0.4.7a3/reflex/components/base/link.pyi
--rw-r--r--   0        0        0     1438 2023-12-21 01:07:08.390993 reflex-0.4.7a3/reflex/components/base/meta.py
--rw-r--r--   0        0        0    13088 2024-04-02 19:14:34.410197 reflex-0.4.7a3/reflex/components/base/meta.pyi
--rw-r--r--   0        0        0     2298 2023-12-21 01:07:08.391208 reflex-0.4.7a3/reflex/components/base/script.py
--rw-r--r--   0        0        0     4500 2024-04-02 19:14:34.410334 reflex-0.4.7a3/reflex/components/base/script.pyi
--rw-r--r--   0        0        0     6378 2024-04-02 19:14:34.410492 reflex-0.4.7a3/reflex/components/chakra/__init__.py
--rw-r--r--   0        0        0     5242 2024-02-16 18:55:54.269834 reflex-0.4.7a3/reflex/components/chakra/base.py
--rw-r--r--   0        0        0    11059 2024-04-02 19:14:34.410632 reflex-0.4.7a3/reflex/components/chakra/base.pyi
--rw-r--r--   0        0        0      459 2024-04-02 19:14:34.410790 reflex-0.4.7a3/reflex/components/chakra/datadisplay/__init__.py
--rw-r--r--   0        0        0      352 2024-02-10 02:26:35.022081 reflex-0.4.7a3/reflex/components/chakra/datadisplay/badge.py
--rw-r--r--   0        0        0     3725 2024-04-02 19:14:34.410909 reflex-0.4.7a3/reflex/components/chakra/datadisplay/badge.pyi
--rw-r--r--   0        0        0      174 2024-04-02 19:14:34.411078 reflex-0.4.7a3/reflex/components/chakra/datadisplay/code.py
--rw-r--r--   0        0        0     3300 2024-04-02 19:14:34.411266 reflex-0.4.7a3/reflex/components/chakra/datadisplay/code.pyi
--rw-r--r--   0        0        0      657 2024-02-10 02:26:35.022721 reflex-0.4.7a3/reflex/components/chakra/datadisplay/divider.py
--rw-r--r--   0        0        0     4005 2024-04-02 19:14:34.411393 reflex-0.4.7a3/reflex/components/chakra/datadisplay/divider.pyi
--rw-r--r--   0        0        0      180 2024-02-10 02:26:35.022864 reflex-0.4.7a3/reflex/components/chakra/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     3322 2024-04-02 19:14:34.411517 reflex-0.4.7a3/reflex/components/chakra/datadisplay/keyboard_key.pyi
--rw-r--r--   0        0        0     1505 2024-02-10 02:26:35.022985 reflex-0.4.7a3/reflex/components/chakra/datadisplay/list.py
--rw-r--r--   0        0        0    13065 2024-04-02 19:14:34.411638 reflex-0.4.7a3/reflex/components/chakra/datadisplay/list.pyi
--rw-r--r--   0        0        0     2149 2024-02-10 02:26:35.023113 reflex-0.4.7a3/reflex/components/chakra/datadisplay/stat.py
--rw-r--r--   0        0        0    17816 2024-04-02 19:14:34.411771 reflex-0.4.7a3/reflex/components/chakra/datadisplay/stat.pyi
--rw-r--r--   0        0        0     9122 2024-02-10 02:26:35.023268 reflex-0.4.7a3/reflex/components/chakra/datadisplay/table.py
--rw-r--r--   0        0        0    27536 2024-04-02 19:14:34.411949 reflex-0.4.7a3/reflex/components/chakra/datadisplay/table.pyi
--rw-r--r--   0        0        0     2294 2024-02-10 02:26:35.023510 reflex-0.4.7a3/reflex/components/chakra/datadisplay/tag.py
--rw-r--r--   0        0        0    16018 2024-04-02 19:14:34.412089 reflex-0.4.7a3/reflex/components/chakra/datadisplay/tag.pyi
--rw-r--r--   0        0        0      384 2024-02-10 02:26:35.023677 reflex-0.4.7a3/reflex/components/chakra/disclosure/__init__.py
--rw-r--r--   0        0        0     3509 2024-02-10 02:26:35.023748 reflex-0.4.7a3/reflex/components/chakra/disclosure/accordion.py
--rw-r--r--   0        0        0    16087 2024-04-02 19:14:34.412252 reflex-0.4.7a3/reflex/components/chakra/disclosure/accordion.pyi
--rw-r--r--   0        0        0     3295 2024-02-10 02:26:35.024084 reflex-0.4.7a3/reflex/components/chakra/disclosure/tabs.py
--rw-r--r--   0        0        0    18809 2024-04-02 19:14:34.412388 reflex-0.4.7a3/reflex/components/chakra/disclosure/tabs.pyi
--rw-r--r--   0        0        0     1732 2024-02-10 02:26:35.024232 reflex-0.4.7a3/reflex/components/chakra/disclosure/transition.py
--rw-r--r--   0        0        0    20429 2024-04-02 19:14:34.412530 reflex-0.4.7a3/reflex/components/chakra/disclosure/transition.pyi
--rw-r--r--   0        0        0      278 2024-02-10 02:26:35.024533 reflex-0.4.7a3/reflex/components/chakra/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0     3329 2024-04-02 19:14:34.412660 reflex-0.4.7a3/reflex/components/chakra/disclosure/visuallyhidden.pyi
--rw-r--r--   0        0        0      313 2024-02-10 02:26:35.024661 reflex-0.4.7a3/reflex/components/chakra/feedback/__init__.py
--rw-r--r--   0        0        0     1623 2024-02-10 02:26:35.024723 reflex-0.4.7a3/reflex/components/chakra/feedback/alert.py
--rw-r--r--   0        0        0    12594 2024-04-02 19:14:34.412793 reflex-0.4.7a3/reflex/components/chakra/feedback/alert.pyi
--rw-r--r--   0        0        0     2006 2024-02-10 02:26:35.024858 reflex-0.4.7a3/reflex/components/chakra/feedback/circularprogress.py
--rw-r--r--   0        0        0     7708 2024-04-02 19:14:34.412916 reflex-0.4.7a3/reflex/components/chakra/feedback/circularprogress.pyi
--rw-r--r--   0        0        0      871 2024-02-10 02:26:35.024988 reflex-0.4.7a3/reflex/components/chakra/feedback/progress.py
--rw-r--r--   0        0        0     4349 2024-04-02 19:14:34.413051 reflex-0.4.7a3/reflex/components/chakra/feedback/progress.pyi
--rw-r--r--   0        0        0     1776 2024-02-10 02:26:35.025096 reflex-0.4.7a3/reflex/components/chakra/feedback/skeleton.py
--rw-r--r--   0        0        0    10903 2024-04-02 19:14:34.413182 reflex-0.4.7a3/reflex/components/chakra/feedback/skeleton.pyi
--rw-r--r--   0        0        0      704 2024-02-10 02:26:35.025211 reflex-0.4.7a3/reflex/components/chakra/feedback/spinner.py
--rw-r--r--   0        0        0     4178 2024-04-02 19:14:34.413298 reflex-0.4.7a3/reflex/components/chakra/feedback/spinner.pyi
--rw-r--r--   0        0        0     1453 2024-04-02 19:14:34.413424 reflex-0.4.7a3/reflex/components/chakra/forms/__init__.py
--rw-r--r--   0        0        0     2395 2024-02-10 02:26:35.025415 reflex-0.4.7a3/reflex/components/chakra/forms/button.py
--rw-r--r--   0        0        0    10687 2024-04-02 19:14:34.413528 reflex-0.4.7a3/reflex/components/chakra/forms/button.pyi
--rw-r--r--   0        0        0     2764 2024-02-10 02:26:35.025535 reflex-0.4.7a3/reflex/components/chakra/forms/checkbox.py
--rw-r--r--   0        0        0    10443 2024-04-02 19:14:34.413633 reflex-0.4.7a3/reflex/components/chakra/forms/checkbox.pyi
--rw-r--r--   0        0        0     2860 2024-04-02 19:14:34.413744 reflex-0.4.7a3/reflex/components/chakra/forms/colormodeswitch.py
--rw-r--r--   0        0        0    18530 2024-04-02 19:14:34.413852 reflex-0.4.7a3/reflex/components/chakra/forms/colormodeswitch.pyi
--rw-r--r--   0        0        0      246 2024-02-10 02:26:35.025773 reflex-0.4.7a3/reflex/components/chakra/forms/date_picker.py
--rw-r--r--   0        0        0     5841 2024-04-02 19:14:34.413954 reflex-0.4.7a3/reflex/components/chakra/forms/date_picker.pyi
--rw-r--r--   0        0        0      280 2024-02-10 02:26:35.025877 reflex-0.4.7a3/reflex/components/chakra/forms/date_time_picker.py
--rw-r--r--   0        0        0     5854 2024-04-02 19:14:34.414051 reflex-0.4.7a3/reflex/components/chakra/forms/date_time_picker.pyi
--rw-r--r--   0        0        0     2110 2024-02-10 02:26:35.025987 reflex-0.4.7a3/reflex/components/chakra/forms/editable.py
--rw-r--r--   0        0        0    13623 2024-04-02 19:14:34.414156 reflex-0.4.7a3/reflex/components/chakra/forms/editable.pyi
--rw-r--r--   0        0        0      246 2024-02-10 02:26:35.026103 reflex-0.4.7a3/reflex/components/chakra/forms/email.py
--rw-r--r--   0        0        0     5825 2024-04-02 19:14:34.414250 reflex-0.4.7a3/reflex/components/chakra/forms/email.pyi
--rw-r--r--   0        0        0     2579 2024-04-02 19:14:34.414562 reflex-0.4.7a3/reflex/components/chakra/forms/form.py
--rw-r--r--   0        0        0    20832 2024-04-02 19:14:34.414743 reflex-0.4.7a3/reflex/components/chakra/forms/form.pyi
--rw-r--r--   0        0        0      935 2024-02-10 02:26:35.026649 reflex-0.4.7a3/reflex/components/chakra/forms/iconbutton.py
--rw-r--r--   0        0        0     4739 2024-04-02 19:14:34.414896 reflex-0.4.7a3/reflex/components/chakra/forms/iconbutton.pyi
--rw-r--r--   0        0        0     4312 2024-04-02 19:14:34.415230 reflex-0.4.7a3/reflex/components/chakra/forms/input.py
--rw-r--r--   0        0        0    21869 2024-04-02 19:14:34.415375 reflex-0.4.7a3/reflex/components/chakra/forms/input.pyi
--rw-r--r--   0        0        0    12940 2024-02-10 02:26:35.027180 reflex-0.4.7a3/reflex/components/chakra/forms/multiselect.py
--rw-r--r--   0        0        0     4334 2024-02-10 02:26:35.027253 reflex-0.4.7a3/reflex/components/chakra/forms/numberinput.py
--rw-r--r--   0        0        0    18377 2024-04-02 19:14:34.415512 reflex-0.4.7a3/reflex/components/chakra/forms/numberinput.pyi
--rw-r--r--   0        0        0      256 2024-02-10 02:26:35.027395 reflex-0.4.7a3/reflex/components/chakra/forms/password.py
--rw-r--r--   0        0        0     5834 2024-04-02 19:14:34.415639 reflex-0.4.7a3/reflex/components/chakra/forms/password.pyi
--rw-r--r--   0        0        0     6507 2024-04-04 21:37:03.946495 reflex-0.4.7a3/reflex/components/chakra/forms/pininput.py
--rw-r--r--   0        0        0     9432 2024-04-02 19:14:34.415764 reflex-0.4.7a3/reflex/components/chakra/forms/pininput.pyi
--rw-r--r--   0        0        0     3176 2024-02-10 02:26:35.027681 reflex-0.4.7a3/reflex/components/chakra/forms/radio.py
--rw-r--r--   0        0        0     8414 2024-04-02 19:14:34.415876 reflex-0.4.7a3/reflex/components/chakra/forms/radio.pyi
--rw-r--r--   0        0        0     4547 2024-02-10 02:26:35.027836 reflex-0.4.7a3/reflex/components/chakra/forms/rangeslider.py
--rw-r--r--   0        0        0    14156 2024-04-02 19:14:34.415997 reflex-0.4.7a3/reflex/components/chakra/forms/rangeslider.pyi
--rw-r--r--   0        0        0     3624 2024-02-10 02:26:35.027969 reflex-0.4.7a3/reflex/components/chakra/forms/select.py
--rw-r--r--   0        0        0     8868 2024-04-02 19:14:34.416109 reflex-0.4.7a3/reflex/components/chakra/forms/select.pyi
--rw-r--r--   0        0        0     3532 2024-02-10 02:26:35.028089 reflex-0.4.7a3/reflex/components/chakra/forms/slider.py
--rw-r--r--   0        0        0    17745 2024-04-02 19:14:34.416245 reflex-0.4.7a3/reflex/components/chakra/forms/slider.pyi
--rw-r--r--   0        0        0     1838 2024-02-10 02:26:35.028236 reflex-0.4.7a3/reflex/components/chakra/forms/switch.py
--rw-r--r--   0        0        0     6602 2024-04-02 19:14:34.416373 reflex-0.4.7a3/reflex/components/chakra/forms/switch.pyi
--rw-r--r--   0        0        0     2474 2024-02-16 18:55:54.270329 reflex-0.4.7a3/reflex/components/chakra/forms/textarea.py
--rw-r--r--   0        0        0     5419 2024-04-02 19:14:34.416480 reflex-0.4.7a3/reflex/components/chakra/forms/textarea.pyi
--rw-r--r--   0        0        0      246 2024-02-10 02:26:35.028621 reflex-0.4.7a3/reflex/components/chakra/forms/time_picker.py
--rw-r--r--   0        0        0     5841 2024-04-02 19:14:34.416578 reflex-0.4.7a3/reflex/components/chakra/forms/time_picker.pyi
--rw-r--r--   0        0        0      487 2024-04-02 19:14:34.416715 reflex-0.4.7a3/reflex/components/chakra/layout/__init__.py
--rw-r--r--   0        0        0      315 2024-02-10 02:26:35.028815 reflex-0.4.7a3/reflex/components/chakra/layout/aspect_ratio.py
--rw-r--r--   0        0        0     3450 2024-04-02 19:14:34.416820 reflex-0.4.7a3/reflex/components/chakra/layout/aspect_ratio.pyi
--rw-r--r--   0        0        0      755 2024-02-10 02:26:35.028940 reflex-0.4.7a3/reflex/components/chakra/layout/box.py
--rw-r--r--   0        0        0     3733 2024-04-02 19:14:34.416924 reflex-0.4.7a3/reflex/components/chakra/layout/box.pyi
--rw-r--r--   0        0        0     2967 2024-02-10 02:26:35.029073 reflex-0.4.7a3/reflex/components/chakra/layout/card.py
--rw-r--r--   0        0        0    14063 2024-04-02 19:14:34.417040 reflex-0.4.7a3/reflex/components/chakra/layout/card.pyi
--rw-r--r--   0        0        0      389 2024-02-10 02:26:35.029302 reflex-0.4.7a3/reflex/components/chakra/layout/center.py
--rw-r--r--   0        0        0     8905 2024-04-02 19:14:34.417147 reflex-0.4.7a3/reflex/components/chakra/layout/center.pyi
--rw-r--r--   0        0        0      354 2024-02-10 02:26:35.029446 reflex-0.4.7a3/reflex/components/chakra/layout/container.py
--rw-r--r--   0        0        0     3502 2024-04-02 19:14:34.417255 reflex-0.4.7a3/reflex/components/chakra/layout/container.pyi
--rw-r--r--   0        0        0      715 2024-02-10 02:26:35.029582 reflex-0.4.7a3/reflex/components/chakra/layout/flex.py
--rw-r--r--   0        0        0     4209 2024-04-02 19:14:34.417357 reflex-0.4.7a3/reflex/components/chakra/layout/flex.pyi
--rw-r--r--   0        0        0     4318 2024-02-10 02:26:35.029717 reflex-0.4.7a3/reflex/components/chakra/layout/grid.py
--rw-r--r--   0        0        0    14066 2024-04-02 19:14:34.417480 reflex-0.4.7a3/reflex/components/chakra/layout/grid.pyi
--rw-r--r--   0        0        0      179 2024-02-10 02:26:35.029946 reflex-0.4.7a3/reflex/components/chakra/layout/spacer.py
--rw-r--r--   0        0        0     3301 2024-04-02 19:14:34.417588 reflex-0.4.7a3/reflex/components/chakra/layout/spacer.pyi
--rw-r--r--   0        0        0     1077 2024-02-10 02:26:35.030045 reflex-0.4.7a3/reflex/components/chakra/layout/stack.py
--rw-r--r--   0        0        0    12432 2024-04-02 19:14:34.417697 reflex-0.4.7a3/reflex/components/chakra/layout/stack.pyi
--rw-r--r--   0        0        0     1463 2024-02-10 02:26:35.030152 reflex-0.4.7a3/reflex/components/chakra/layout/wrap.py
--rw-r--r--   0        0        0     7014 2024-04-02 19:14:34.417807 reflex-0.4.7a3/reflex/components/chakra/layout/wrap.pyi
--rw-r--r--   0        0        0      190 2024-02-10 02:26:35.030265 reflex-0.4.7a3/reflex/components/chakra/media/__init__.py
--rw-r--r--   0        0        0     1668 2024-02-10 02:26:35.030317 reflex-0.4.7a3/reflex/components/chakra/media/avatar.py
--rw-r--r--   0        0        0    10658 2024-04-02 19:14:34.417938 reflex-0.4.7a3/reflex/components/chakra/media/avatar.pyi
--rw-r--r--   0        0        0     2461 2024-02-10 02:26:35.030430 reflex-0.4.7a3/reflex/components/chakra/media/icon.py
--rw-r--r--   0        0        0     6342 2024-04-02 19:14:34.418161 reflex-0.4.7a3/reflex/components/chakra/media/icon.pyi
--rw-r--r--   0        0        0     2400 2024-02-10 02:26:35.030535 reflex-0.4.7a3/reflex/components/chakra/media/image.py
--rw-r--r--   0        0        0     5423 2024-04-02 19:14:34.418332 reflex-0.4.7a3/reflex/components/chakra/media/image.pyi
--rw-r--r--   0        0        0      419 2024-02-10 02:26:35.030653 reflex-0.4.7a3/reflex/components/chakra/navigation/__init__.py
--rw-r--r--   0        0        0     2925 2024-02-10 02:26:35.030704 reflex-0.4.7a3/reflex/components/chakra/navigation/breadcrumb.py
--rw-r--r--   0        0        0    13646 2024-04-02 19:14:34.418567 reflex-0.4.7a3/reflex/components/chakra/navigation/breadcrumb.pyi
--rw-r--r--   0        0        0     1475 2024-02-10 02:26:35.030830 reflex-0.4.7a3/reflex/components/chakra/navigation/link.py
--rw-r--r--   0        0        0     3999 2024-04-02 19:14:34.418745 reflex-0.4.7a3/reflex/components/chakra/navigation/link.pyi
--rw-r--r--   0        0        0      521 2024-02-10 02:26:35.031182 reflex-0.4.7a3/reflex/components/chakra/navigation/linkoverlay.py
--rw-r--r--   0        0        0     6375 2024-04-02 19:14:34.418852 reflex-0.4.7a3/reflex/components/chakra/navigation/linkoverlay.pyi
--rw-r--r--   0        0        0     2935 2024-02-10 02:26:35.031313 reflex-0.4.7a3/reflex/components/chakra/navigation/stepper.py
--rw-r--r--   0        0        0    28490 2024-04-02 19:14:34.418987 reflex-0.4.7a3/reflex/components/chakra/navigation/stepper.pyi
--rw-r--r--   0        0        0      850 2024-02-10 02:26:35.031514 reflex-0.4.7a3/reflex/components/chakra/overlay/__init__.py
--rw-r--r--   0        0        0     5200 2024-02-10 02:26:35.031625 reflex-0.4.7a3/reflex/components/chakra/overlay/alertdialog.py
--rw-r--r--   0        0        0    24411 2024-04-02 19:14:34.419146 reflex-0.4.7a3/reflex/components/chakra/overlay/alertdialog.pyi
--rw-r--r--   0        0        0     5186 2024-02-10 02:26:35.031772 reflex-0.4.7a3/reflex/components/chakra/overlay/drawer.py
--rw-r--r--   0        0        0    25832 2024-04-02 19:14:34.419276 reflex-0.4.7a3/reflex/components/chakra/overlay/drawer.pyi
--rw-r--r--   0        0        0     6974 2024-02-10 02:26:35.031928 reflex-0.4.7a3/reflex/components/chakra/overlay/menu.py
--rw-r--r--   0        0        0    29108 2024-04-02 19:14:34.419396 reflex-0.4.7a3/reflex/components/chakra/overlay/menu.pyi
--rw-r--r--   0        0        0     5270 2024-02-10 02:26:35.032050 reflex-0.4.7a3/reflex/components/chakra/overlay/modal.py
--rw-r--r--   0        0        0    23975 2024-04-02 19:14:34.419505 reflex-0.4.7a3/reflex/components/chakra/overlay/modal.pyi
--rw-r--r--   0        0        0     5967 2024-02-10 02:26:35.032202 reflex-0.4.7a3/reflex/components/chakra/overlay/popover.py
--rw-r--r--   0        0        0    30461 2024-04-02 19:14:34.419633 reflex-0.4.7a3/reflex/components/chakra/overlay/popover.pyi
--rw-r--r--   0        0        0     2127 2024-02-10 02:26:35.032416 reflex-0.4.7a3/reflex/components/chakra/overlay/tooltip.py
--rw-r--r--   0        0        0     6131 2024-04-02 19:14:34.419766 reflex-0.4.7a3/reflex/components/chakra/overlay/tooltip.pyi
--rw-r--r--   0        0        0      271 2024-02-10 02:26:35.032550 reflex-0.4.7a3/reflex/components/chakra/typography/__init__.py
--rw-r--r--   0        0        0      379 2024-02-10 02:26:35.032612 reflex-0.4.7a3/reflex/components/chakra/typography/heading.py
--rw-r--r--   0        0        0     3777 2024-04-02 19:14:34.419870 reflex-0.4.7a3/reflex/components/chakra/typography/heading.pyi
--rw-r--r--   0        0        0      671 2024-02-10 02:26:35.032741 reflex-0.4.7a3/reflex/components/chakra/typography/highlight.py
--rw-r--r--   0        0        0     3716 2024-04-02 19:14:34.419964 reflex-0.4.7a3/reflex/components/chakra/typography/highlight.pyi
--rw-r--r--   0        0        0      328 2024-02-10 02:26:35.032862 reflex-0.4.7a3/reflex/components/chakra/typography/span.py
--rw-r--r--   0        0        0     3443 2024-04-02 19:14:34.420093 reflex-0.4.7a3/reflex/components/chakra/typography/span.pyi
--rw-r--r--   0        0        0      472 2024-02-10 02:26:35.033013 reflex-0.4.7a3/reflex/components/chakra/typography/text.py
--rw-r--r--   0        0        0     3667 2024-04-02 19:14:34.420216 reflex-0.4.7a3/reflex/components/chakra/typography/text.pyi
--rw-r--r--   0        0        0    64790 2024-04-04 21:37:03.946766 reflex-0.4.7a3/reflex/components/component.py
--rw-r--r--   0        0        0      844 2024-04-02 19:14:34.421147 reflex-0.4.7a3/reflex/components/core/__init__.py
--rw-r--r--   0        0        0     5943 2024-04-04 21:37:03.946911 reflex-0.4.7a3/reflex/components/core/banner.py
--rw-r--r--   0        0        0    17164 2024-04-02 19:14:34.421397 reflex-0.4.7a3/reflex/components/core/banner.pyi
--rw-r--r--   0        0        0     1873 2024-02-10 02:26:35.034230 reflex-0.4.7a3/reflex/components/core/client_side_routing.py
--rw-r--r--   0        0        0     6406 2024-04-02 19:14:34.421550 reflex-0.4.7a3/reflex/components/core/client_side_routing.pyi
--rw-r--r--   0        0        0      590 2024-04-02 19:14:34.421679 reflex-0.4.7a3/reflex/components/core/colors.py
--rw-r--r--   0        0        0     6291 2024-04-08 21:11:25.547238 reflex-0.4.7a3/reflex/components/core/cond.py
--rw-r--r--   0        0        0     4642 2024-04-02 19:14:34.422253 reflex-0.4.7a3/reflex/components/core/debounce.py
--rw-r--r--   0        0        0     4149 2024-04-02 19:14:34.422370 reflex-0.4.7a3/reflex/components/core/debounce.pyi
--rw-r--r--   0        0        0     4031 2024-04-02 18:24:25.099624 reflex-0.4.7a3/reflex/components/core/foreach.py
--rw-r--r--   0        0        0     1033 2024-04-02 19:14:34.422562 reflex-0.4.7a3/reflex/components/core/html.py
--rw-r--r--   0        0        0     6616 2024-04-02 19:14:34.422669 reflex-0.4.7a3/reflex/components/core/html.pyi
--rw-r--r--   0        0        0       30 2024-02-10 02:26:35.035636 reflex-0.4.7a3/reflex/components/core/layout/__init__.py
--rw-r--r--   0        0        0     9989 2024-04-02 19:14:34.422836 reflex-0.4.7a3/reflex/components/core/match.py
--rw-r--r--   0        0        0     1907 2024-04-02 19:14:34.427781 reflex-0.4.7a3/reflex/components/core/responsive.py
--rw-r--r--   0        0        0     9000 2024-04-04 21:37:03.947039 reflex-0.4.7a3/reflex/components/core/upload.py
--rw-r--r--   0        0        0     8667 2024-04-02 19:14:34.429377 reflex-0.4.7a3/reflex/components/core/upload.pyi
--rw-r--r--   0        0        0      357 2024-04-04 21:37:03.947140 reflex-0.4.7a3/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0    11227 2024-04-02 19:14:34.430271 reflex-0.4.7a3/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0    31107 2024-04-02 19:14:34.430442 reflex-0.4.7a3/reflex/components/datadisplay/code.pyi
--rw-r--r--   0        0        0    12632 2024-02-10 02:26:35.036910 reflex-0.4.7a3/reflex/components/datadisplay/dataeditor.py
--rw-r--r--   0        0        0    10485 2024-04-02 19:14:34.430603 reflex-0.4.7a3/reflex/components/datadisplay/dataeditor.pyi
--rw-r--r--   0        0        0     2562 2024-04-04 21:37:03.947200 reflex-0.4.7a3/reflex/components/datadisplay/logo.py
--rw-r--r--   0        0        0       73 2024-02-07 01:47:48.949909 reflex-0.4.7a3/reflex/components/el/__init__.py
--rw-r--r--   0        0        0      113 2023-12-21 01:07:08.429460 reflex-0.4.7a3/reflex/components/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-12-21 01:07:08.429529 reflex-0.4.7a3/reflex/components/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-12-21 01:07:08.429622 reflex-0.4.7a3/reflex/components/el/constants/react.py
--rw-r--r--   0        0        0     1713 2023-12-21 01:07:08.429682 reflex-0.4.7a3/reflex/components/el/constants/reflex.py
--rw-r--r--   0        0        0      494 2023-12-21 01:07:08.429898 reflex-0.4.7a3/reflex/components/el/element.py
--rw-r--r--   0        0        0     3284 2024-04-02 19:14:34.430869 reflex-0.4.7a3/reflex/components/el/element.pyi
--rw-r--r--   0        0        0     3529 2024-04-02 19:14:34.432601 reflex-0.4.7a3/reflex/components/el/elements/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-02 19:14:34.432772 reflex-0.4.7a3/reflex/components/el/elements/base.py
--rw-r--r--   0        0        0     6411 2024-04-02 19:14:34.432874 reflex-0.4.7a3/reflex/components/el/elements/base.pyi
--rw-r--r--   0        0        0    20102 2024-04-04 21:37:03.947356 reflex-0.4.7a3/reflex/components/el/elements/forms.py
--rw-r--r--   0        0        0   100476 2024-04-04 21:37:03.947614 reflex-0.4.7a3/reflex/components/el/elements/forms.pyi
--rw-r--r--   0        0        0     3610 2024-02-10 02:26:35.038470 reflex-0.4.7a3/reflex/components/el/elements/inline.py
--rw-r--r--   0        0        0   166595 2024-04-02 19:14:34.433892 reflex-0.4.7a3/reflex/components/el/elements/inline.pyi
--rw-r--r--   0        0        0     7929 2024-04-02 19:14:34.434037 reflex-0.4.7a3/reflex/components/el/elements/media.py
--rw-r--r--   0        0        0    94561 2024-04-02 19:14:34.434188 reflex-0.4.7a3/reflex/components/el/elements/media.pyi
--rw-r--r--   0        0        0     1337 2023-12-21 01:07:08.433098 reflex-0.4.7a3/reflex/components/el/elements/metadata.py
--rw-r--r--   0        0        0    28386 2024-04-02 19:14:34.434330 reflex-0.4.7a3/reflex/components/el/elements/metadata.pyi
--rw-r--r--   0        0        0     1569 2023-12-21 01:07:08.433349 reflex-0.4.7a3/reflex/components/el/elements/other.py
--rw-r--r--   0        0        0    42530 2024-04-02 19:14:34.434559 reflex-0.4.7a3/reflex/components/el/elements/other.pyi
--rw-r--r--   0        0        0     1406 2024-04-02 19:14:34.434672 reflex-0.4.7a3/reflex/components/el/elements/scripts.py
--rw-r--r--   0        0        0    19828 2024-04-02 19:14:34.434788 reflex-0.4.7a3/reflex/components/el/elements/scripts.pyi
--rw-r--r--   0        0        0     1535 2024-04-02 19:14:34.434940 reflex-0.4.7a3/reflex/components/el/elements/sectioning.py
--rw-r--r--   0        0        0    88307 2024-04-02 19:14:34.435104 reflex-0.4.7a3/reflex/components/el/elements/sectioning.pyi
--rw-r--r--   0        0        0     2767 2024-04-02 19:14:34.435250 reflex-0.4.7a3/reflex/components/el/elements/tables.py
--rw-r--r--   0        0        0    62559 2024-04-02 19:14:34.435538 reflex-0.4.7a3/reflex/components/el/elements/tables.pyi
--rw-r--r--   0        0        0     2432 2024-04-02 19:14:34.436021 reflex-0.4.7a3/reflex/components/el/elements/typography.py
--rw-r--r--   0        0        0    90180 2024-04-02 19:14:34.436215 reflex-0.4.7a3/reflex/components/el/elements/typography.pyi
--rw-r--r--   0        0        0       88 2024-02-10 02:26:35.040149 reflex-0.4.7a3/reflex/components/gridjs/__init__.py
--rw-r--r--   0        0        0     4300 2024-02-10 02:26:35.040226 reflex-0.4.7a3/reflex/components/gridjs/datatable.py
--rw-r--r--   0        0        0     7124 2024-04-02 19:14:34.436409 reflex-0.4.7a3/reflex/components/gridjs/datatable.pyi
--rw-r--r--   0        0        0      501 2024-02-10 02:26:35.040431 reflex-0.4.7a3/reflex/components/literals.py
--rw-r--r--   0        0        0       73 2024-02-10 02:26:35.040887 reflex-0.4.7a3/reflex/components/lucide/__init__.py
--rw-r--r--   0        0        0    34237 2024-04-04 21:37:03.947839 reflex-0.4.7a3/reflex/components/lucide/icon.py
--rw-r--r--   0        0        0    38020 2024-04-04 21:37:03.948033 reflex-0.4.7a3/reflex/components/lucide/icon.pyi
--rw-r--r--   0        0        0       87 2024-02-10 02:26:35.041813 reflex-0.4.7a3/reflex/components/markdown/__init__.py
--rw-r--r--   0        0        0    11448 2024-04-04 21:37:03.948197 reflex-0.4.7a3/reflex/components/markdown/markdown.py
--rw-r--r--   0        0        0     5278 2024-04-04 21:37:03.948324 reflex-0.4.7a3/reflex/components/markdown/markdown.pyi
--rw-r--r--   0        0        0       44 2024-02-10 02:26:35.042167 reflex-0.4.7a3/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      102 2024-02-10 02:26:35.042266 reflex-0.4.7a3/reflex/components/media/icon.py
--rw-r--r--   0        0        0       79 2024-02-10 02:26:35.042315 reflex-0.4.7a3/reflex/components/moment/__init__.py
--rw-r--r--   0        0        0     3925 2024-02-10 02:26:35.042375 reflex-0.4.7a3/reflex/components/moment/moment.py
--rw-r--r--   0        0        0     6870 2024-04-02 19:14:34.438557 reflex-0.4.7a3/reflex/components/moment/moment.pyi
--rw-r--r--   0        0        0      239 2024-02-10 02:26:35.042504 reflex-0.4.7a3/reflex/components/next/__init__.py
--rw-r--r--   0        0        0      189 2024-02-10 02:26:35.042549 reflex-0.4.7a3/reflex/components/next/base.py
--rw-r--r--   0        0        0     3304 2024-04-02 19:14:34.438775 reflex-0.4.7a3/reflex/components/next/base.pyi
--rw-r--r--   0        0        0     3831 2024-02-10 02:26:35.042660 reflex-0.4.7a3/reflex/components/next/image.py
--rw-r--r--   0        0        0     5795 2024-04-02 19:14:34.438919 reflex-0.4.7a3/reflex/components/next/image.pyi
--rw-r--r--   0        0        0      503 2024-02-10 02:26:35.042780 reflex-0.4.7a3/reflex/components/next/link.py
--rw-r--r--   0        0        0     3532 2024-04-02 19:14:34.439026 reflex-0.4.7a3/reflex/components/next/link.pyi
--rw-r--r--   0        0        0      730 2024-02-10 02:26:35.042905 reflex-0.4.7a3/reflex/components/next/video.py
--rw-r--r--   0        0        0     3429 2024-04-02 19:14:34.439128 reflex-0.4.7a3/reflex/components/next/video.pyi
--rw-r--r--   0        0        0       77 2024-02-10 02:26:35.043030 reflex-0.4.7a3/reflex/components/plotly/__init__.py
--rw-r--r--   0        0        0      964 2024-04-02 19:14:34.439545 reflex-0.4.7a3/reflex/components/plotly/plotly.py
--rw-r--r--   0        0        0     7007 2024-04-02 19:14:34.439682 reflex-0.4.7a3/reflex/components/plotly/plotly.pyi
--rw-r--r--   0        0        0      112 2024-04-02 19:14:34.440146 reflex-0.4.7a3/reflex/components/radix/__init__.py
--rw-r--r--   0        0        0      214 2024-04-02 19:14:34.440350 reflex-0.4.7a3/reflex/components/radix/primitives/__init__.py
--rw-r--r--   0        0        0    21406 2024-04-02 19:14:34.440707 reflex-0.4.7a3/reflex/components/radix/primitives/accordion.py
--rw-r--r--   0        0        0    26956 2024-04-02 19:14:34.440903 reflex-0.4.7a3/reflex/components/radix/primitives/accordion.pyi
--rw-r--r--   0        0        0      869 2024-02-10 02:26:35.044768 reflex-0.4.7a3/reflex/components/radix/primitives/base.py
--rw-r--r--   0        0        0     6620 2024-04-02 19:14:34.441366 reflex-0.4.7a3/reflex/components/radix/primitives/base.pyi
--rw-r--r--   0        0        0     8660 2024-04-02 19:14:34.442162 reflex-0.4.7a3/reflex/components/radix/primitives/drawer.py
--rw-r--r--   0        0        0    34981 2024-04-02 19:14:34.442473 reflex-0.4.7a3/reflex/components/radix/primitives/drawer.pyi
--rw-r--r--   0        0        0     4760 2024-04-02 19:14:34.442846 reflex-0.4.7a3/reflex/components/radix/primitives/form.py
--rw-r--r--   0        0        0    48365 2024-04-02 19:14:34.443076 reflex-0.4.7a3/reflex/components/radix/primitives/form.pyi
--rw-r--r--   0        0        0     3996 2024-04-02 19:14:34.443510 reflex-0.4.7a3/reflex/components/radix/primitives/progress.py
--rw-r--r--   0        0        0    22997 2024-04-02 19:14:34.444066 reflex-0.4.7a3/reflex/components/radix/primitives/progress.pyi
--rw-r--r--   0        0        0     5004 2024-04-02 19:14:34.444533 reflex-0.4.7a3/reflex/components/radix/primitives/slider.py
--rw-r--r--   0        0        0    17052 2024-04-02 19:14:34.444665 reflex-0.4.7a3/reflex/components/radix/primitives/slider.pyi
--rw-r--r--   0        0        0      292 2024-04-02 19:14:34.444811 reflex-0.4.7a3/reflex/components/radix/themes/__init__.py
--rw-r--r--   0        0        0     8097 2024-04-02 19:14:34.445088 reflex-0.4.7a3/reflex/components/radix/themes/base.py
--rw-r--r--   0        0        0    24216 2024-04-02 19:14:34.445340 reflex-0.4.7a3/reflex/components/radix/themes/base.pyi
--rw-r--r--   0        0        0     3007 2024-04-02 19:14:34.445446 reflex-0.4.7a3/reflex/components/radix/themes/color_mode.py
--rw-r--r--   0        0        0    21283 2024-04-02 19:14:34.445570 reflex-0.4.7a3/reflex/components/radix/themes/color_mode.pyi
--rw-r--r--   0        0        0     1776 2024-04-02 19:14:34.445724 reflex-0.4.7a3/reflex/components/radix/themes/components/__init__.py
--rw-r--r--   0        0        0     3267 2024-04-02 19:14:34.446644 reflex-0.4.7a3/reflex/components/radix/themes/components/alert_dialog.py
--rw-r--r--   0        0        0    24434 2024-04-02 19:14:34.446757 reflex-0.4.7a3/reflex/components/radix/themes/components/alert_dialog.pyi
--rw-r--r--   0        0        0    40237 2024-04-02 19:14:34.447529 reflex-0.4.7a3/reflex/components/radix/themes/components/alertdialog.pyi
--rw-r--r--   0        0        0      400 2024-04-02 19:14:34.447703 reflex-0.4.7a3/reflex/components/radix/themes/components/aspect_ratio.py
--rw-r--r--   0        0        0     3640 2024-04-02 19:14:34.447802 reflex-0.4.7a3/reflex/components/radix/themes/components/aspect_ratio.pyi
--rw-r--r--   0        0        0     5724 2024-04-02 19:14:34.448082 reflex-0.4.7a3/reflex/components/radix/themes/components/aspectratio.pyi
--rw-r--r--   0        0        0      989 2024-04-02 19:14:34.448493 reflex-0.4.7a3/reflex/components/radix/themes/components/avatar.py
--rw-r--r--   0        0        0     6562 2024-04-02 19:14:34.448953 reflex-0.4.7a3/reflex/components/radix/themes/components/avatar.pyi
--rw-r--r--   0        0        0      815 2024-04-02 19:14:34.449058 reflex-0.4.7a3/reflex/components/radix/themes/components/badge.py
--rw-r--r--   0        0        0     9315 2024-04-02 19:14:34.449155 reflex-0.4.7a3/reflex/components/radix/themes/components/badge.pyi
--rw-r--r--   0        0        0     1084 2024-04-02 19:14:34.449285 reflex-0.4.7a3/reflex/components/radix/themes/components/button.py
--rw-r--r--   0        0        0    11758 2024-04-02 19:14:34.449372 reflex-0.4.7a3/reflex/components/radix/themes/components/button.pyi
--rw-r--r--   0        0        0     2378 2024-04-02 19:14:34.449904 reflex-0.4.7a3/reflex/components/radix/themes/components/callout.py
--rw-r--r--   0        0        0    38710 2024-04-02 19:14:34.450185 reflex-0.4.7a3/reflex/components/radix/themes/components/callout.pyi
--rw-r--r--   0        0        0      659 2024-04-02 19:14:34.450330 reflex-0.4.7a3/reflex/components/radix/themes/components/card.py
--rw-r--r--   0        0        0     7200 2024-04-02 19:14:34.450427 reflex-0.4.7a3/reflex/components/radix/themes/components/card.pyi
--rw-r--r--   0        0        0     4679 2024-04-02 19:14:34.451369 reflex-0.4.7a3/reflex/components/radix/themes/components/checkbox.py
--rw-r--r--   0        0        0    20877 2024-04-02 19:14:34.451567 reflex-0.4.7a3/reflex/components/radix/themes/components/checkbox.pyi
--rw-r--r--   0        0        0     5049 2024-04-02 19:14:34.451786 reflex-0.4.7a3/reflex/components/radix/themes/components/context_menu.py
--rw-r--r--   0        0        0    31192 2024-04-02 19:14:34.451890 reflex-0.4.7a3/reflex/components/radix/themes/components/context_menu.pyi
--rw-r--r--   0        0        0    44130 2024-04-02 19:14:34.452056 reflex-0.4.7a3/reflex/components/radix/themes/components/contextmenu.pyi
--rw-r--r--   0        0        0     2600 2024-04-02 19:14:34.452261 reflex-0.4.7a3/reflex/components/radix/themes/components/dialog.py
--rw-r--r--   0        0        0    24895 2024-04-02 19:14:34.452419 reflex-0.4.7a3/reflex/components/radix/themes/components/dialog.pyi
--rw-r--r--   0        0        0    11256 2024-04-02 19:14:34.452696 reflex-0.4.7a3/reflex/components/radix/themes/components/dropdown_menu.py
--rw-r--r--   0        0        0    37901 2024-04-02 19:14:34.452840 reflex-0.4.7a3/reflex/components/radix/themes/components/dropdown_menu.pyi
--rw-r--r--   0        0        0    52185 2024-04-02 19:14:34.453086 reflex-0.4.7a3/reflex/components/radix/themes/components/dropdownmenu.pyi
--rw-r--r--   0        0        0     2405 2024-04-02 19:14:34.453445 reflex-0.4.7a3/reflex/components/radix/themes/components/hover_card.py
--rw-r--r--   0        0        0    17744 2024-04-02 19:14:34.453581 reflex-0.4.7a3/reflex/components/radix/themes/components/hover_card.pyi
--rw-r--r--   0        0        0    26453 2024-04-02 19:14:34.453788 reflex-0.4.7a3/reflex/components/radix/themes/components/hovercard.pyi
--rw-r--r--   0        0        0     2789 2024-04-02 19:14:34.454202 reflex-0.4.7a3/reflex/components/radix/themes/components/icon_button.py
--rw-r--r--   0        0        0    11916 2024-04-02 19:14:34.454271 reflex-0.4.7a3/reflex/components/radix/themes/components/icon_button.pyi
--rw-r--r--   0        0        0    12021 2024-04-02 19:14:34.454397 reflex-0.4.7a3/reflex/components/radix/themes/components/iconbutton.pyi
--rw-r--r--   0        0        0     1015 2024-04-02 19:14:34.454891 reflex-0.4.7a3/reflex/components/radix/themes/components/inset.py
--rw-r--r--   0        0        0     7889 2024-04-02 19:14:34.455045 reflex-0.4.7a3/reflex/components/radix/themes/components/inset.pyi
--rw-r--r--   0        0        0     3177 2024-04-02 19:14:34.455306 reflex-0.4.7a3/reflex/components/radix/themes/components/popover.py
--rw-r--r--   0        0        0    17404 2024-04-02 19:14:34.455466 reflex-0.4.7a3/reflex/components/radix/themes/components/popover.pyi
--rw-r--r--   0        0        0     6253 2024-04-02 19:14:34.455911 reflex-0.4.7a3/reflex/components/radix/themes/components/radio_group.py
--rw-r--r--   0        0        0    24106 2024-04-02 19:14:34.456002 reflex-0.4.7a3/reflex/components/radix/themes/components/radio_group.pyi
--rw-r--r--   0        0        0    26222 2024-04-02 19:14:34.457988 reflex-0.4.7a3/reflex/components/radix/themes/components/radiogroup.pyi
--rw-r--r--   0        0        0      920 2024-04-02 19:14:34.458077 reflex-0.4.7a3/reflex/components/radix/themes/components/scroll_area.py
--rw-r--r--   0        0        0     4427 2024-04-02 19:14:34.458156 reflex-0.4.7a3/reflex/components/radix/themes/components/scroll_area.pyi
--rw-r--r--   0        0        0     6513 2024-04-02 19:14:34.458390 reflex-0.4.7a3/reflex/components/radix/themes/components/scrollarea.pyi
--rw-r--r--   0        0        0     8028 2024-04-04 21:37:03.948474 reflex-0.4.7a3/reflex/components/radix/themes/components/select.py
--rw-r--r--   0        0        0    45123 2024-04-02 19:14:34.459754 reflex-0.4.7a3/reflex/components/radix/themes/components/select.pyi
--rw-r--r--   0        0        0      868 2024-04-02 19:14:34.459929 reflex-0.4.7a3/reflex/components/radix/themes/components/separator.py
--rw-r--r--   0        0        0     6078 2024-04-02 19:14:34.460031 reflex-0.4.7a3/reflex/components/radix/themes/components/separator.pyi
--rw-r--r--   0        0        0     3234 2024-04-02 19:14:34.460186 reflex-0.4.7a3/reflex/components/radix/themes/components/slider.py
--rw-r--r--   0        0        0     8162 2024-04-02 19:14:34.460283 reflex-0.4.7a3/reflex/components/radix/themes/components/slider.pyi
--rw-r--r--   0        0        0     1976 2024-04-02 19:14:34.460390 reflex-0.4.7a3/reflex/components/radix/themes/components/switch.py
--rw-r--r--   0        0        0     7404 2024-04-02 19:14:34.460484 reflex-0.4.7a3/reflex/components/radix/themes/components/switch.pyi
--rw-r--r--   0        0        0     3111 2024-04-02 19:14:34.460743 reflex-0.4.7a3/reflex/components/radix/themes/components/table.py
--rw-r--r--   0        0        0    47387 2024-04-02 19:14:34.460872 reflex-0.4.7a3/reflex/components/radix/themes/components/table.pyi
--rw-r--r--   0        0        0     2213 2024-04-02 19:14:34.463534 reflex-0.4.7a3/reflex/components/radix/themes/components/tabs.py
--rw-r--r--   0        0        0    17321 2024-04-02 19:14:34.463662 reflex-0.4.7a3/reflex/components/radix/themes/components/tabs.pyi
--rw-r--r--   0        0        0     3233 2024-04-02 19:14:34.463765 reflex-0.4.7a3/reflex/components/radix/themes/components/text_area.py
--rw-r--r--   0        0        0    11711 2024-04-02 19:14:34.463961 reflex-0.4.7a3/reflex/components/radix/themes/components/text_area.pyi
--rw-r--r--   0        0        0     5106 2024-04-02 19:14:34.464711 reflex-0.4.7a3/reflex/components/radix/themes/components/text_field.py
--rw-r--r--   0        0        0    43043 2024-04-02 19:14:34.464805 reflex-0.4.7a3/reflex/components/radix/themes/components/text_field.pyi
--rw-r--r--   0        0        0    43365 2024-04-02 19:14:34.464956 reflex-0.4.7a3/reflex/components/radix/themes/components/textfield.pyi
--rw-r--r--   0        0        0     4465 2024-04-02 19:14:34.465166 reflex-0.4.7a3/reflex/components/radix/themes/components/tooltip.py
--rw-r--r--   0        0        0     8092 2024-04-02 19:14:34.465305 reflex-0.4.7a3/reflex/components/radix/themes/components/tooltip.pyi
--rw-r--r--   0        0        0      811 2024-04-02 19:14:34.465647 reflex-0.4.7a3/reflex/components/radix/themes/layout/__init__.py
--rw-r--r--   0        0        0     1201 2024-04-02 19:14:34.465990 reflex-0.4.7a3/reflex/components/radix/themes/layout/base.py
--rw-r--r--   0        0        0     7643 2024-04-02 19:14:34.466154 reflex-0.4.7a3/reflex/components/radix/themes/layout/base.pyi
--rw-r--r--   0        0        0      281 2024-02-10 02:26:35.060028 reflex-0.4.7a3/reflex/components/radix/themes/layout/box.py
--rw-r--r--   0        0        0     6462 2024-04-02 19:14:34.466266 reflex-0.4.7a3/reflex/components/radix/themes/layout/box.pyi
--rw-r--r--   0        0        0      422 2024-04-02 19:14:34.466627 reflex-0.4.7a3/reflex/components/radix/themes/layout/center.py
--rw-r--r--   0        0        0     8245 2024-04-02 19:14:34.466794 reflex-0.4.7a3/reflex/components/radix/themes/layout/center.pyi
--rw-r--r--   0        0        0      552 2024-02-10 02:26:35.060445 reflex-0.4.7a3/reflex/components/radix/themes/layout/container.py
--rw-r--r--   0        0        0     6779 2024-04-02 19:14:34.466930 reflex-0.4.7a3/reflex/components/radix/themes/layout/container.pyi
--rw-r--r--   0        0        0     1374 2024-04-02 19:14:34.467197 reflex-0.4.7a3/reflex/components/radix/themes/layout/flex.py
--rw-r--r--   0        0        0     8501 2024-04-02 19:14:34.467710 reflex-0.4.7a3/reflex/components/radix/themes/layout/flex.pyi
--rw-r--r--   0        0        0     1498 2024-04-02 19:14:34.468616 reflex-0.4.7a3/reflex/components/radix/themes/layout/grid.py
--rw-r--r--   0        0        0     8907 2024-04-02 19:14:34.468790 reflex-0.4.7a3/reflex/components/radix/themes/layout/grid.pyi
--rw-r--r--   0        0        0     4889 2024-04-02 19:14:34.469076 reflex-0.4.7a3/reflex/components/radix/themes/layout/list.py
--rw-r--r--   0        0        0    29367 2024-04-02 19:14:34.469203 reflex-0.4.7a3/reflex/components/radix/themes/layout/list.pyi
--rw-r--r--   0        0        0      458 2024-02-10 02:26:35.060937 reflex-0.4.7a3/reflex/components/radix/themes/layout/section.py
--rw-r--r--   0        0        0     6758 2024-04-02 19:14:34.469367 reflex-0.4.7a3/reflex/components/radix/themes/layout/section.pyi
--rw-r--r--   0        0        0      412 2024-04-02 19:14:34.469593 reflex-0.4.7a3/reflex/components/radix/themes/layout/spacer.py
--rw-r--r--   0        0        0     8245 2024-04-02 19:14:34.469727 reflex-0.4.7a3/reflex/components/radix/themes/layout/spacer.pyi
--rw-r--r--   0        0        0     1270 2024-04-02 19:14:34.469849 reflex-0.4.7a3/reflex/components/radix/themes/layout/stack.py
--rw-r--r--   0        0        0    22132 2024-04-02 19:14:34.470027 reflex-0.4.7a3/reflex/components/radix/themes/layout/stack.pyi
--rw-r--r--   0        0        0      343 2024-04-02 19:14:34.470193 reflex-0.4.7a3/reflex/components/radix/themes/typography/__init__.py
--rw-r--r--   0        0        0      408 2024-02-10 02:26:35.061693 reflex-0.4.7a3/reflex/components/radix/themes/typography/base.py
--rw-r--r--   0        0        0      799 2024-02-10 02:26:35.061822 reflex-0.4.7a3/reflex/components/radix/themes/typography/blockquote.py
--rw-r--r--   0        0        0     9316 2024-04-02 19:14:34.470311 reflex-0.4.7a3/reflex/components/radix/themes/typography/blockquote.pyi
--rw-r--r--   0        0        0      909 2024-02-10 02:26:35.062001 reflex-0.4.7a3/reflex/components/radix/themes/typography/code.py
--rw-r--r--   0        0        0     9513 2024-04-02 19:14:34.470410 reflex-0.4.7a3/reflex/components/radix/themes/typography/code.pyi
--rw-r--r--   0        0        0     8547 2024-04-02 19:14:34.470588 reflex-0.4.7a3/reflex/components/radix/themes/typography/em.pyi
--rw-r--r--   0        0        0     1324 2024-02-10 02:26:35.062444 reflex-0.4.7a3/reflex/components/radix/themes/typography/heading.py
--rw-r--r--   0        0        0    10106 2024-04-02 19:14:34.470692 reflex-0.4.7a3/reflex/components/radix/themes/typography/heading.pyi
--rw-r--r--   0        0        0     8872 2024-04-02 19:14:34.470802 reflex-0.4.7a3/reflex/components/radix/themes/typography/kbd.pyi
--rw-r--r--   0        0        0     3154 2024-04-02 19:14:34.471091 reflex-0.4.7a3/reflex/components/radix/themes/typography/link.py
--rw-r--r--   0        0        0    12063 2024-04-02 19:14:34.471230 reflex-0.4.7a3/reflex/components/radix/themes/typography/link.pyi
--rw-r--r--   0        0        0     8701 2024-04-02 19:14:34.471467 reflex-0.4.7a3/reflex/components/radix/themes/typography/quote.pyi
--rw-r--r--   0        0        0     8563 2024-04-02 19:14:34.471621 reflex-0.4.7a3/reflex/components/radix/themes/typography/strong.pyi
--rw-r--r--   0        0        0     2604 2024-04-02 19:14:34.472005 reflex-0.4.7a3/reflex/components/radix/themes/typography/text.py
--rw-r--r--   0        0        0    57238 2024-04-02 19:14:34.472171 reflex-0.4.7a3/reflex/components/radix/themes/typography/text.pyi
--rw-r--r--   0        0        0      144 2024-02-10 02:26:35.063629 reflex-0.4.7a3/reflex/components/react_player/__init__.py
--rw-r--r--   0        0        0      185 2024-02-10 02:26:35.063689 reflex-0.4.7a3/reflex/components/react_player/audio.py
--rw-r--r--   0        0        0     4398 2024-04-02 19:14:34.472284 reflex-0.4.7a3/reflex/components/react_player/audio.pyi
--rw-r--r--   0        0        0     1087 2024-02-10 02:26:35.063804 reflex-0.4.7a3/reflex/components/react_player/react_player.py
--rw-r--r--   0        0        0     4425 2024-04-02 19:14:34.472391 reflex-0.4.7a3/reflex/components/react_player/react_player.pyi
--rw-r--r--   0        0        0      185 2024-02-10 02:26:35.063907 reflex-0.4.7a3/reflex/components/react_player/video.py
--rw-r--r--   0        0        0     4398 2024-04-02 19:14:34.472479 reflex-0.4.7a3/reflex/components/react_player/video.pyi
--rw-r--r--   0        0        0     2373 2024-02-10 02:26:35.064033 reflex-0.4.7a3/reflex/components/recharts/__init__.py
--rw-r--r--   0        0        0    19595 2024-02-10 02:26:35.064126 reflex-0.4.7a3/reflex/components/recharts/cartesian.py
--rw-r--r--   0        0        0    85500 2024-04-02 19:14:34.472660 reflex-0.4.7a3/reflex/components/recharts/cartesian.pyi
--rw-r--r--   0        0        0    18493 2024-02-10 02:26:35.064337 reflex-0.4.7a3/reflex/components/recharts/charts.py
--rw-r--r--   0        0        0    48757 2024-04-02 19:14:34.472846 reflex-0.4.7a3/reflex/components/recharts/charts.pyi
--rw-r--r--   0        0        0     5624 2024-02-10 02:26:35.064489 reflex-0.4.7a3/reflex/components/recharts/general.py
--rw-r--r--   0        0        0    23071 2024-04-02 19:14:34.472964 reflex-0.4.7a3/reflex/components/recharts/general.pyi
--rw-r--r--   0        0        0    10410 2024-02-10 02:26:35.064657 reflex-0.4.7a3/reflex/components/recharts/polar.py
--rw-r--r--   0        0        0    24752 2024-04-02 19:14:34.473068 reflex-0.4.7a3/reflex/components/recharts/polar.pyi
--rw-r--r--   0        0        0     2870 2024-02-10 02:26:35.064789 reflex-0.4.7a3/reflex/components/recharts/recharts.py
--rw-r--r--   0        0        0     8606 2024-04-02 19:14:34.473190 reflex-0.4.7a3/reflex/components/recharts/recharts.pyi
--rw-r--r--   0        0        0      109 2024-02-10 02:26:35.064909 reflex-0.4.7a3/reflex/components/suneditor/__init__.py
--rw-r--r--   0        0        0     7360 2024-02-10 02:26:35.064985 reflex-0.4.7a3/reflex/components/suneditor/editor.py
--rw-r--r--   0        0        0    10330 2024-04-02 19:14:34.473324 reflex-0.4.7a3/reflex/components/suneditor/editor.pyi
--rw-r--r--   0        0        0      152 2024-02-10 02:26:35.065200 reflex-0.4.7a3/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-12-21 01:07:08.463011 reflex-0.4.7a3/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3620 2024-02-10 02:26:35.065323 reflex-0.4.7a3/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0      387 2024-02-10 02:26:35.065376 reflex-0.4.7a3/reflex/components/tags/match_tag.py
--rw-r--r--   0        0        0     2778 2024-04-02 19:14:34.473664 reflex-0.4.7a3/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-12-21 01:07:08.463394 reflex-0.4.7a3/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0    11082 2024-04-04 21:37:03.948613 reflex-0.4.7a3/reflex/config.py
--rw-r--r--   0        0        0     3318 2024-04-04 21:37:03.948873 reflex-0.4.7a3/reflex/config.pyi
--rw-r--r--   0        0        0     2036 2024-04-02 19:14:34.474441 reflex-0.4.7a3/reflex/constants/__init__.py
--rw-r--r--   0        0        0     5640 2024-04-04 22:32:02.761988 reflex-0.4.7a3/reflex/constants/base.py
--rw-r--r--   0        0        0     2980 2024-04-04 22:32:02.762262 reflex-0.4.7a3/reflex/constants/base.pyi
--rw-r--r--   0        0        0     1599 2024-04-02 19:14:34.474865 reflex-0.4.7a3/reflex/constants/colors.py
--rw-r--r--   0        0        0     4137 2024-04-04 21:37:03.949234 reflex-0.4.7a3/reflex/constants/compiler.py
--rw-r--r--   0        0        0     1331 2024-02-10 02:26:35.066956 reflex-0.4.7a3/reflex/constants/config.py
--rw-r--r--   0        0        0     1268 2024-04-02 19:14:34.475565 reflex-0.4.7a3/reflex/constants/custom_components.py
--rw-r--r--   0        0        0     2668 2024-02-10 02:26:35.067613 reflex-0.4.7a3/reflex/constants/event.py
--rw-r--r--   0        0        0     3177 2024-04-02 19:14:34.475856 reflex-0.4.7a3/reflex/constants/installer.py
--rw-r--r--   0        0        0     1940 2024-04-02 19:14:34.476122 reflex-0.4.7a3/reflex/constants/route.py
--rw-r--r--   0        0        0      636 2024-02-10 02:26:35.067842 reflex-0.4.7a3/reflex/constants/style.py
--rw-r--r--   0        0        0       36 2024-04-02 19:14:34.476236 reflex-0.4.7a3/reflex/custom_components/__init__.py
--rw-r--r--   0        0        0    31705 2024-04-09 01:49:49.020352 reflex-0.4.7a3/reflex/custom_components/custom_components.py
--rw-r--r--   0        0        0    26634 2024-04-05 22:42:13.970118 reflex-0.4.7a3/reflex/event.py
--rw-r--r--   0        0        0      287 2024-04-04 21:37:03.949637 reflex-0.4.7a3/reflex/experimental/__init__.py
--rw-r--r--   0        0        0     1647 2024-04-04 21:37:03.949706 reflex-0.4.7a3/reflex/experimental/hooks.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.4.7a3/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1484 2024-04-02 19:14:34.477238 reflex-0.4.7a3/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1169 2023-12-04 22:31:51.618237 reflex-0.4.7a3/reflex/middleware/middleware.py
--rw-r--r--   0        0        0    13091 2024-04-06 01:57:36.880449 reflex-0.4.7a3/reflex/model.py
--rw-r--r--   0        0        0     1921 2024-04-04 21:37:03.949824 reflex-0.4.7a3/reflex/page.py
--rw-r--r--   0        0        0    17871 2024-04-04 22:32:02.763178 reflex-0.4.7a3/reflex/reflex.py
--rw-r--r--   0        0        0     2908 2024-04-02 19:14:34.478054 reflex-0.4.7a3/reflex/route.py
--rw-r--r--   0        0        0   105642 2024-04-02 19:14:34.478448 reflex-0.4.7a3/reflex/state.py
--rw-r--r--   0        0        0     8834 2024-04-04 21:37:03.950185 reflex-0.4.7a3/reflex/style.py
--rw-r--r--   0        0        0    29808 2024-04-04 22:32:02.763768 reflex-0.4.7a3/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-11-07 19:58:07.486037 reflex-0.4.7a3/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8573 2024-02-10 02:26:35.070031 reflex-0.4.7a3/reflex/utils/build.py
--rw-r--r--   0        0        0     5018 2024-04-04 22:32:02.764358 reflex-0.4.7a3/reflex/utils/console.py
--rw-r--r--   0        0        0      504 2024-02-10 02:26:35.070129 reflex-0.4.7a3/reflex/utils/exceptions.py
--rw-r--r--   0        0        0     9969 2024-04-04 21:37:03.950843 reflex-0.4.7a3/reflex/utils/exec.py
--rw-r--r--   0        0        0     2357 2024-04-04 21:37:03.951057 reflex-0.4.7a3/reflex/utils/export.py
--rw-r--r--   0        0        0    22648 2024-04-02 19:14:34.479804 reflex-0.4.7a3/reflex/utils/format.py
--rw-r--r--   0        0        0     1919 2023-12-04 22:31:51.620673 reflex-0.4.7a3/reflex/utils/imports.py
--rw-r--r--   0        0        0     4737 2024-02-10 02:26:35.070893 reflex-0.4.7a3/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    45757 2024-04-05 22:41:26.508584 reflex-0.4.7a3/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     8481 2024-04-04 21:37:03.951498 reflex-0.4.7a3/reflex/utils/processes.py
--rw-r--r--   0        0        0    27674 2024-04-02 19:14:34.480893 reflex-0.4.7a3/reflex/utils/pyi_generator.py
--rw-r--r--   0        0        0     8538 2024-04-08 18:50:32.983082 reflex-0.4.7a3/reflex/utils/serializers.py
--rw-r--r--   0        0        0     4013 2024-04-04 21:37:03.951599 reflex-0.4.7a3/reflex/utils/telemetry.py
--rw-r--r--   0        0        0    13677 2024-04-08 23:20:53.686606 reflex-0.4.7a3/reflex/utils/types.py
--rw-r--r--   0        0        0     2609 2023-11-21 01:55:15.773146 reflex-0.4.7a3/reflex/utils/watch.py
--rw-r--r--   0        0        0    67152 2024-04-04 21:37:03.951876 reflex-0.4.7a3/reflex/vars.py
--rw-r--r--   0        0        0     5583 2024-04-04 21:37:03.951997 reflex-0.4.7a3/reflex/vars.pyi
--rw-r--r--   0        0        0    11815 1970-01-01 00:00:00.000000 reflex-0.4.7a3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.4.8a1/LICENSE
+-rw-r--r--   0        0        0     9568 2024-04-05 17:14:14.456384 reflex-0.4.8a1/README.md
+-rw-r--r--   0        0        0     2922 2024-04-12 01:14:24.524384 reflex-0.4.8a1/pyproject.toml
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.4.8a1/reflex/.templates/apps/blank/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.4.8a1/reflex/.templates/apps/blank/code/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-05 17:14:14.457193 reflex-0.4.8a1/reflex/.templates/apps/blank/code/blank.py
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.4.8a1/reflex/.templates/apps/demo/.gitignore
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/github.svg
+-rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/icon.svg
+-rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/paneleft.svg
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.4.8a1/reflex/.templates/apps/demo/code/__init__.py
+-rw-r--r--   0        0        0     2928 2024-02-17 20:02:02.399454 reflex-0.4.8a1/reflex/.templates/apps/demo/code/demo.py
+-rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/__init__.py
+-rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/chatapp.py
+-rw-r--r--   0        0        0    10910 2024-03-20 23:54:55.829615 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/datatable.py
+-rw-r--r--   0        0        0     8383 2024-03-20 23:54:55.830163 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/forms.py
+-rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/graphing.py
+-rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/home.py
+-rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.4.8a1/reflex/.templates/apps/demo/code/sidebar.py
+-rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.4.8a1/reflex/.templates/apps/demo/code/state.py
+-rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/form_state.py
+-rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/pie_state.py
+-rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.4.8a1/reflex/.templates/apps/demo/code/styles.py
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/__init__.py
+-rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/__init__.py
+-rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/chat.py
+-rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
+-rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/modal.py
+-rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/navbar.py
+-rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py
+-rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/state.py
+-rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/styles.py
+-rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.4.8a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/README.md.jinja2
+-rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/__init__.py.jinja2
+-rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
+-rw-r--r--   0        0        0      614 2024-04-04 14:57:26.374812 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
+-rw-r--r--   0        0        0     2403 2024-04-05 17:14:14.457446 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/src.py.jinja2
+-rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.4.8a1/reflex/.templates/jinja/web/package.json.jinja2
+-rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/_app.js.jinja2
+-rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/component.js.jinja2
+-rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0      388 2024-04-05 17:14:14.457553 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
+-rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
+-rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.4.8a1/reflex/.templates/jinja/web/styles/styles.css.jinja2
+-rw-r--r--   0        0        0      436 2024-02-06 00:51:31.970725 reflex-0.4.8a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.4.8a1/reflex/.templates/jinja/web/utils/context.js.jinja2
+-rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.4.8a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.4.8a1/reflex/.templates/web/.gitignore
+-rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.4.8a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
+-rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.4.8a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
+-rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.4.8a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.4.8a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.4.8a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.4.8a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.4.8a1/reflex/.templates/web/utils/client_side_routing.js
+-rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.4.8a1/reflex/.templates/web/utils/helpers/dataeditor.js
+-rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.4.8a1/reflex/.templates/web/utils/helpers/range.js
+-rw-r--r--   0        0        0    21909 2024-04-12 01:14:12.255596 reflex-0.4.8a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     5723 2024-04-05 17:14:14.458168 reflex-0.4.8a1/reflex/__init__.py
+-rw-r--r--   0        0        0     7649 2024-04-06 01:20:11.620853 reflex-0.4.8a1/reflex/__init__.pyi
+-rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.4.8a1/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.4.8a1/reflex/admin.py
+-rw-r--r--   0        0        0    45016 2024-04-12 01:14:12.255992 reflex-0.4.8a1/reflex/app.py
+-rw-r--r--   0        0        0     5010 2024-04-04 14:57:26.376271 reflex-0.4.8a1/reflex/app.pyi
+-rw-r--r--   0        0        0     1152 2024-03-20 23:54:55.837204 reflex-0.4.8a1/reflex/app_module_for_backend.py
+-rw-r--r--   0        0        0     4250 2024-04-04 14:57:26.376408 reflex-0.4.8a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.4.8a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0    17037 2024-04-05 17:14:14.458702 reflex-0.4.8a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.4.8a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0    14024 2024-04-12 01:14:12.256301 reflex-0.4.8a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0      530 2024-02-17 20:02:02.404048 reflex-0.4.8a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.4.8a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.4.8a1/reflex/components/base/app_wrap.py
+-rw-r--r--   0        0        0     2890 2024-04-04 14:57:26.376832 reflex-0.4.8a1/reflex/components/base/app_wrap.pyi
+-rw-r--r--   0        0        0     1234 2024-04-04 14:57:26.376921 reflex-0.4.8a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.4.8a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0     3206 2024-04-12 01:14:12.256423 reflex-0.4.8a1/reflex/components/base/body.pyi
+-rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.4.8a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0    14232 2024-04-12 01:14:12.256750 reflex-0.4.8a1/reflex/components/base/document.pyi
+-rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.4.8a1/reflex/components/base/fragment.py
+-rw-r--r--   0        0        0     3218 2024-04-12 01:14:12.256848 reflex-0.4.8a1/reflex/components/base/fragment.pyi
+-rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.4.8a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0     6002 2024-04-12 01:14:12.257050 reflex-0.4.8a1/reflex/components/base/head.pyi
+-rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.4.8a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     6990 2024-04-12 01:14:12.257244 reflex-0.4.8a1/reflex/components/base/link.pyi
+-rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.4.8a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    12804 2024-04-12 01:14:12.257347 reflex-0.4.8a1/reflex/components/base/meta.pyi
+-rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.4.8a1/reflex/components/base/script.py
+-rw-r--r--   0        0        0     4500 2024-04-04 14:57:26.377962 reflex-0.4.8a1/reflex/components/base/script.pyi
+-rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.4.8a1/reflex/components/chakra/__init__.py
+-rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.4.8a1/reflex/components/chakra/base.py
+-rw-r--r--   0        0        0    10917 2024-04-12 01:14:12.257771 reflex-0.4.8a1/reflex/components/chakra/base.pyi
+-rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.4.8a1/reflex/components/chakra/datadisplay/__init__.py
+-rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.4.8a1/reflex/components/chakra/datadisplay/badge.py
+-rw-r--r--   0        0        0     3654 2024-04-12 01:14:12.257918 reflex-0.4.8a1/reflex/components/chakra/datadisplay/badge.pyi
+-rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.4.8a1/reflex/components/chakra/datadisplay/code.py
+-rw-r--r--   0        0        0     3229 2024-04-12 01:14:12.258034 reflex-0.4.8a1/reflex/components/chakra/datadisplay/code.pyi
+-rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.py
+-rw-r--r--   0        0        0     3934 2024-04-12 01:14:12.258149 reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.pyi
+-rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.4.8a1/reflex/components/chakra/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     3251 2024-04-12 01:14:12.258264 reflex-0.4.8a1/reflex/components/chakra/datadisplay/keyboard_key.pyi
+-rw-r--r--   0        0        0     1505 2024-02-07 21:48:43.272557 reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.py
+-rw-r--r--   0        0        0    12994 2024-04-12 01:14:12.258377 reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.pyi
+-rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.py
+-rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.258509 reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.pyi
+-rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.py
+-rw-r--r--   0        0        0    27252 2024-04-12 01:14:12.258649 reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.pyi
+-rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.py
+-rw-r--r--   0        0        0    15734 2024-04-12 01:14:12.258803 reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.pyi
+-rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.4.8a1/reflex/components/chakra/disclosure/__init__.py
+-rw-r--r--   0        0        0     3509 2024-02-07 21:48:43.274196 reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.py
+-rw-r--r--   0        0        0    15803 2024-04-12 01:14:12.258961 reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.pyi
+-rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.py
+-rw-r--r--   0        0        0    18525 2024-04-12 01:14:12.259114 reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.pyi
+-rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.py
+-rw-r--r--   0        0        0    20003 2024-04-12 01:14:12.259285 reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.pyi
+-rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.4.8a1/reflex/components/chakra/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0     3258 2024-04-12 01:14:12.259424 reflex-0.4.8a1/reflex/components/chakra/disclosure/visuallyhidden.pyi
+-rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.4.8a1/reflex/components/chakra/feedback/__init__.py
+-rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.4.8a1/reflex/components/chakra/feedback/alert.py
+-rw-r--r--   0        0        0    12381 2024-04-12 01:14:12.259528 reflex-0.4.8a1/reflex/components/chakra/feedback/alert.pyi
+-rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.py
+-rw-r--r--   0        0        0     7637 2024-04-12 01:14:12.259726 reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.pyi
+-rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.4.8a1/reflex/components/chakra/feedback/progress.py
+-rw-r--r--   0        0        0     4278 2024-04-12 01:14:12.259930 reflex-0.4.8a1/reflex/components/chakra/feedback/progress.pyi
+-rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.py
+-rw-r--r--   0        0        0    10690 2024-04-12 01:14:12.260187 reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.pyi
+-rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.py
+-rw-r--r--   0        0        0     4107 2024-04-12 01:14:12.260440 reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.pyi
+-rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.4.8a1/reflex/components/chakra/forms/__init__.py
+-rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.4.8a1/reflex/components/chakra/forms/button.py
+-rw-r--r--   0        0        0    10545 2024-04-12 01:14:12.260613 reflex-0.4.8a1/reflex/components/chakra/forms/button.pyi
+-rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.py
+-rw-r--r--   0        0        0    10301 2024-04-12 01:14:12.260767 reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.pyi
+-rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.py
+-rw-r--r--   0        0        0    18459 2024-04-12 01:14:12.260906 reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.4.8a1/reflex/components/chakra/forms/date_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.380782 reflex-0.4.8a1/reflex/components/chakra/forms/date_picker.pyi
+-rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.4.8a1/reflex/components/chakra/forms/date_time_picker.py
+-rw-r--r--   0        0        0     5854 2024-04-04 14:57:26.380893 reflex-0.4.8a1/reflex/components/chakra/forms/date_time_picker.pyi
+-rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.4.8a1/reflex/components/chakra/forms/editable.py
+-rw-r--r--   0        0        0    13339 2024-04-12 01:14:12.261047 reflex-0.4.8a1/reflex/components/chakra/forms/editable.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.4.8a1/reflex/components/chakra/forms/email.py
+-rw-r--r--   0        0        0     5825 2024-04-04 14:57:26.381120 reflex-0.4.8a1/reflex/components/chakra/forms/email.pyi
+-rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.4.8a1/reflex/components/chakra/forms/form.py
+-rw-r--r--   0        0        0    20619 2024-04-12 01:14:12.261180 reflex-0.4.8a1/reflex/components/chakra/forms/form.pyi
+-rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.py
+-rw-r--r--   0        0        0     4668 2024-04-12 01:14:12.261417 reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.pyi
+-rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.4.8a1/reflex/components/chakra/forms/input.py
+-rw-r--r--   0        0        0    21514 2024-04-12 01:14:12.261540 reflex-0.4.8a1/reflex/components/chakra/forms/input.pyi
+-rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.4.8a1/reflex/components/chakra/forms/multiselect.py
+-rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.py
+-rw-r--r--   0        0        0    18093 2024-04-12 01:14:12.261730 reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.pyi
+-rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.4.8a1/reflex/components/chakra/forms/password.py
+-rw-r--r--   0        0        0     5834 2024-04-04 14:57:26.381709 reflex-0.4.8a1/reflex/components/chakra/forms/password.pyi
+-rw-r--r--   0        0        0     6503 2024-04-12 01:14:12.262063 reflex-0.4.8a1/reflex/components/chakra/forms/pininput.py
+-rw-r--r--   0        0        0     9357 2024-04-12 01:14:12.262316 reflex-0.4.8a1/reflex/components/chakra/forms/pininput.pyi
+-rw-r--r--   0        0        0     3172 2024-04-12 01:14:12.263122 reflex-0.4.8a1/reflex/components/chakra/forms/radio.py
+-rw-r--r--   0        0        0     8410 2024-04-12 01:14:12.263294 reflex-0.4.8a1/reflex/components/chakra/forms/radio.pyi
+-rw-r--r--   0        0        0     4543 2024-04-12 01:14:12.263746 reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.py
+-rw-r--r--   0        0        0    13939 2024-04-12 01:14:12.263866 reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.pyi
+-rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.4.8a1/reflex/components/chakra/forms/select.py
+-rw-r--r--   0        0        0     8868 2024-04-04 14:57:26.382156 reflex-0.4.8a1/reflex/components/chakra/forms/select.pyi
+-rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.4.8a1/reflex/components/chakra/forms/slider.py
+-rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.263981 reflex-0.4.8a1/reflex/components/chakra/forms/slider.pyi
+-rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.4.8a1/reflex/components/chakra/forms/switch.py
+-rw-r--r--   0        0        0     6531 2024-04-12 01:14:12.264203 reflex-0.4.8a1/reflex/components/chakra/forms/switch.pyi
+-rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.4.8a1/reflex/components/chakra/forms/textarea.py
+-rw-r--r--   0        0        0     5419 2024-04-04 14:57:26.382551 reflex-0.4.8a1/reflex/components/chakra/forms/textarea.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.4.8a1/reflex/components/chakra/forms/time_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.382659 reflex-0.4.8a1/reflex/components/chakra/forms/time_picker.pyi
+-rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.4.8a1/reflex/components/chakra/layout/__init__.py
+-rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.4.8a1/reflex/components/chakra/layout/aspect_ratio.py
+-rw-r--r--   0        0        0     3379 2024-04-12 01:14:12.264318 reflex-0.4.8a1/reflex/components/chakra/layout/aspect_ratio.pyi
+-rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.4.8a1/reflex/components/chakra/layout/box.py
+-rw-r--r--   0        0        0     3662 2024-04-12 01:14:12.264413 reflex-0.4.8a1/reflex/components/chakra/layout/box.pyi
+-rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.4.8a1/reflex/components/chakra/layout/card.py
+-rw-r--r--   0        0        0    13850 2024-04-12 01:14:12.264513 reflex-0.4.8a1/reflex/components/chakra/layout/card.pyi
+-rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.4.8a1/reflex/components/chakra/layout/center.py
+-rw-r--r--   0        0        0     8692 2024-04-12 01:14:12.264634 reflex-0.4.8a1/reflex/components/chakra/layout/center.pyi
+-rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.4.8a1/reflex/components/chakra/layout/container.py
+-rw-r--r--   0        0        0     3431 2024-04-12 01:14:12.264741 reflex-0.4.8a1/reflex/components/chakra/layout/container.pyi
+-rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.4.8a1/reflex/components/chakra/layout/flex.py
+-rw-r--r--   0        0        0     4138 2024-04-12 01:14:12.264933 reflex-0.4.8a1/reflex/components/chakra/layout/flex.pyi
+-rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.4.8a1/reflex/components/chakra/layout/grid.py
+-rw-r--r--   0        0        0    13853 2024-04-12 01:14:12.265035 reflex-0.4.8a1/reflex/components/chakra/layout/grid.pyi
+-rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.4.8a1/reflex/components/chakra/layout/spacer.py
+-rw-r--r--   0        0        0     3230 2024-04-12 01:14:12.265136 reflex-0.4.8a1/reflex/components/chakra/layout/spacer.pyi
+-rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.4.8a1/reflex/components/chakra/layout/stack.py
+-rw-r--r--   0        0        0    12219 2024-04-12 01:14:12.265267 reflex-0.4.8a1/reflex/components/chakra/layout/stack.pyi
+-rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.4.8a1/reflex/components/chakra/layout/wrap.py
+-rw-r--r--   0        0        0     6943 2024-04-12 01:14:12.265632 reflex-0.4.8a1/reflex/components/chakra/layout/wrap.pyi
+-rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.4.8a1/reflex/components/chakra/media/__init__.py
+-rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.4.8a1/reflex/components/chakra/media/avatar.py
+-rw-r--r--   0        0        0    10445 2024-04-12 01:14:12.265841 reflex-0.4.8a1/reflex/components/chakra/media/avatar.pyi
+-rw-r--r--   0        0        0     2461 2024-02-06 00:51:31.985395 reflex-0.4.8a1/reflex/components/chakra/media/icon.py
+-rw-r--r--   0        0        0     6271 2024-04-12 01:14:12.266058 reflex-0.4.8a1/reflex/components/chakra/media/icon.pyi
+-rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.4.8a1/reflex/components/chakra/media/image.py
+-rw-r--r--   0        0        0     5423 2024-04-04 14:57:26.384173 reflex-0.4.8a1/reflex/components/chakra/media/image.pyi
+-rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.4.8a1/reflex/components/chakra/navigation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.py
+-rw-r--r--   0        0        0    13575 2024-04-12 01:14:12.266197 reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.pyi
+-rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.4.8a1/reflex/components/chakra/navigation/link.py
+-rw-r--r--   0        0        0     3999 2024-04-04 14:57:26.384405 reflex-0.4.8a1/reflex/components/chakra/navigation/link.pyi
+-rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.py
+-rw-r--r--   0        0        0     6233 2024-04-12 01:14:12.266398 reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.pyi
+-rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.py
+-rw-r--r--   0        0        0    27922 2024-04-12 01:14:12.266521 reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.pyi
+-rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.4.8a1/reflex/components/chakra/overlay/__init__.py
+-rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.py
+-rw-r--r--   0        0        0    23985 2024-04-12 01:14:12.266681 reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.pyi
+-rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.py
+-rw-r--r--   0        0        0    25406 2024-04-12 01:14:12.266827 reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.pyi
+-rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.4.8a1/reflex/components/chakra/overlay/menu.py
+-rw-r--r--   0        0        0    28682 2024-04-12 01:14:12.266967 reflex-0.4.8a1/reflex/components/chakra/overlay/menu.pyi
+-rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.4.8a1/reflex/components/chakra/overlay/modal.py
+-rw-r--r--   0        0        0    23549 2024-04-12 01:14:12.267114 reflex-0.4.8a1/reflex/components/chakra/overlay/modal.pyi
+-rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.4.8a1/reflex/components/chakra/overlay/popover.py
+-rw-r--r--   0        0        0    29893 2024-04-12 01:14:12.267256 reflex-0.4.8a1/reflex/components/chakra/overlay/popover.pyi
+-rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.py
+-rw-r--r--   0        0        0     6060 2024-04-12 01:14:12.267494 reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.pyi
+-rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.4.8a1/reflex/components/chakra/typography/__init__.py
+-rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.4.8a1/reflex/components/chakra/typography/heading.py
+-rw-r--r--   0        0        0     3706 2024-04-12 01:14:12.267618 reflex-0.4.8a1/reflex/components/chakra/typography/heading.pyi
+-rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.4.8a1/reflex/components/chakra/typography/highlight.py
+-rw-r--r--   0        0        0     3645 2024-04-12 01:14:12.267722 reflex-0.4.8a1/reflex/components/chakra/typography/highlight.pyi
+-rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.4.8a1/reflex/components/chakra/typography/span.py
+-rw-r--r--   0        0        0     3372 2024-04-12 01:14:12.267821 reflex-0.4.8a1/reflex/components/chakra/typography/span.pyi
+-rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.4.8a1/reflex/components/chakra/typography/text.py
+-rw-r--r--   0        0        0     3596 2024-04-12 01:14:12.267927 reflex-0.4.8a1/reflex/components/chakra/typography/text.pyi
+-rw-r--r--   0        0        0    66011 2024-04-12 01:14:12.268153 reflex-0.4.8a1/reflex/components/component.py
+-rw-r--r--   0        0        0      844 2024-03-20 23:54:55.841256 reflex-0.4.8a1/reflex/components/core/__init__.py
+-rw-r--r--   0        0        0     5943 2024-04-04 14:57:26.386161 reflex-0.4.8a1/reflex/components/core/banner.py
+-rw-r--r--   0        0        0    17164 2024-04-04 14:57:26.386284 reflex-0.4.8a1/reflex/components/core/banner.pyi
+-rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.4.8a1/reflex/components/core/client_side_routing.py
+-rw-r--r--   0        0        0     6264 2024-04-12 01:14:12.268957 reflex-0.4.8a1/reflex/components/core/client_side_routing.pyi
+-rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.4.8a1/reflex/components/core/colors.py
+-rw-r--r--   0        0        0     6291 2024-04-04 14:19:59.331531 reflex-0.4.8a1/reflex/components/core/cond.py
+-rw-r--r--   0        0        0     4642 2024-03-20 23:54:55.842359 reflex-0.4.8a1/reflex/components/core/debounce.py
+-rw-r--r--   0        0        0     4149 2024-04-04 14:57:26.386549 reflex-0.4.8a1/reflex/components/core/debounce.pyi
+-rw-r--r--   0        0        0     4031 2024-02-06 00:51:31.992601 reflex-0.4.8a1/reflex/components/core/foreach.py
+-rw-r--r--   0        0        0     1033 2024-02-17 20:02:02.418184 reflex-0.4.8a1/reflex/components/core/html.py
+-rw-r--r--   0        0        0     6616 2024-04-04 14:57:26.386705 reflex-0.4.8a1/reflex/components/core/html.pyi
+-rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.4.8a1/reflex/components/core/layout/__init__.py
+-rw-r--r--   0        0        0     9989 2024-02-17 20:02:02.418463 reflex-0.4.8a1/reflex/components/core/match.py
+-rw-r--r--   0        0        0     1907 2024-04-04 14:19:59.331992 reflex-0.4.8a1/reflex/components/core/responsive.py
+-rw-r--r--   0        0        0     9035 2024-04-12 01:14:12.269123 reflex-0.4.8a1/reflex/components/core/upload.py
+-rw-r--r--   0        0        0     8596 2024-04-12 01:14:12.269265 reflex-0.4.8a1/reflex/components/core/upload.pyi
+-rw-r--r--   0        0        0      357 2024-04-05 17:14:14.460655 reflex-0.4.8a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0    11227 2024-04-04 14:19:59.332304 reflex-0.4.8a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0    31107 2024-04-04 14:57:26.387164 reflex-0.4.8a1/reflex/components/datadisplay/code.pyi
+-rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.py
+-rw-r--r--   0        0        0    10485 2024-04-04 14:57:26.387318 reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.pyi
+-rw-r--r--   0        0        0     2562 2024-04-05 17:14:14.460754 reflex-0.4.8a1/reflex/components/datadisplay/logo.py
+-rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.4.8a1/reflex/components/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.4.8a1/reflex/components/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.4.8a1/reflex/components/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.4.8a1/reflex/components/el/constants/react.py
+-rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.4.8a1/reflex/components/el/constants/reflex.py
+-rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.4.8a1/reflex/components/el/element.py
+-rw-r--r--   0        0        0     3213 2024-04-12 01:14:12.269384 reflex-0.4.8a1/reflex/components/el/element.pyi
+-rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.4.8a1/reflex/components/el/elements/__init__.py
+-rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.4.8a1/reflex/components/el/elements/base.py
+-rw-r--r--   0        0        0     6340 2024-04-12 01:14:12.269589 reflex-0.4.8a1/reflex/components/el/elements/base.pyi
+-rw-r--r--   0        0        0    20102 2024-04-05 17:14:14.460921 reflex-0.4.8a1/reflex/components/el/elements/forms.py
+-rw-r--r--   0        0        0    99553 2024-04-12 01:14:12.269801 reflex-0.4.8a1/reflex/components/el/elements/forms.pyi
+-rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.4.8a1/reflex/components/el/elements/inline.py
+-rw-r--r--   0        0        0   164607 2024-04-12 01:14:12.270476 reflex-0.4.8a1/reflex/components/el/elements/inline.pyi
+-rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.4.8a1/reflex/components/el/elements/media.py
+-rw-r--r--   0        0        0    93567 2024-04-12 01:14:12.270712 reflex-0.4.8a1/reflex/components/el/elements/media.pyi
+-rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.4.8a1/reflex/components/el/elements/metadata.py
+-rw-r--r--   0        0        0    28031 2024-04-12 01:14:12.270995 reflex-0.4.8a1/reflex/components/el/elements/metadata.pyi
+-rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.4.8a1/reflex/components/el/elements/other.py
+-rw-r--r--   0        0        0    42033 2024-04-12 01:14:12.271158 reflex-0.4.8a1/reflex/components/el/elements/other.pyi
+-rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.4.8a1/reflex/components/el/elements/scripts.py
+-rw-r--r--   0        0        0    19615 2024-04-12 01:14:12.271357 reflex-0.4.8a1/reflex/components/el/elements/scripts.pyi
+-rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.4.8a1/reflex/components/el/elements/sectioning.py
+-rw-r--r--   0        0        0    87242 2024-04-12 01:14:12.271561 reflex-0.4.8a1/reflex/components/el/elements/sectioning.pyi
+-rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.4.8a1/reflex/components/el/elements/tables.py
+-rw-r--r--   0        0        0    61849 2024-04-12 01:14:12.271965 reflex-0.4.8a1/reflex/components/el/elements/tables.pyi
+-rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.4.8a1/reflex/components/el/elements/typography.py
+-rw-r--r--   0        0        0    89115 2024-04-12 01:14:12.272183 reflex-0.4.8a1/reflex/components/el/elements/typography.pyi
+-rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.4.8a1/reflex/components/gridjs/__init__.py
+-rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.4.8a1/reflex/components/gridjs/datatable.py
+-rw-r--r--   0        0        0     7053 2024-04-12 01:14:12.272607 reflex-0.4.8a1/reflex/components/gridjs/datatable.pyi
+-rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.4.8a1/reflex/components/literals.py
+-rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.4.8a1/reflex/components/lucide/__init__.py
+-rw-r--r--   0        0        0    34237 2024-04-04 14:57:26.389624 reflex-0.4.8a1/reflex/components/lucide/icon.py
+-rw-r--r--   0        0        0    37949 2024-04-12 01:14:12.272820 reflex-0.4.8a1/reflex/components/lucide/icon.pyi
+-rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.4.8a1/reflex/components/markdown/__init__.py
+-rw-r--r--   0        0        0    11448 2024-04-05 17:14:14.461428 reflex-0.4.8a1/reflex/components/markdown/markdown.py
+-rw-r--r--   0        0        0     5278 2024-04-05 17:14:14.461583 reflex-0.4.8a1/reflex/components/markdown/markdown.pyi
+-rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.4.8a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.4.8a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.4.8a1/reflex/components/moment/__init__.py
+-rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.4.8a1/reflex/components/moment/moment.py
+-rw-r--r--   0        0        0     6870 2024-04-04 14:57:26.390245 reflex-0.4.8a1/reflex/components/moment/moment.pyi
+-rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.4.8a1/reflex/components/next/__init__.py
+-rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.4.8a1/reflex/components/next/base.py
+-rw-r--r--   0        0        0     3233 2024-04-12 01:14:12.273046 reflex-0.4.8a1/reflex/components/next/base.pyi
+-rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.4.8a1/reflex/components/next/image.py
+-rw-r--r--   0        0        0     5795 2024-04-04 14:57:26.390489 reflex-0.4.8a1/reflex/components/next/image.pyi
+-rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.4.8a1/reflex/components/next/link.py
+-rw-r--r--   0        0        0     3461 2024-04-12 01:14:12.273179 reflex-0.4.8a1/reflex/components/next/link.pyi
+-rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.4.8a1/reflex/components/next/video.py
+-rw-r--r--   0        0        0     3429 2024-04-04 14:57:26.390675 reflex-0.4.8a1/reflex/components/next/video.pyi
+-rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.4.8a1/reflex/components/plotly/__init__.py
+-rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.4.8a1/reflex/components/plotly/plotly.py
+-rw-r--r--   0        0        0     6865 2024-04-12 01:14:12.273411 reflex-0.4.8a1/reflex/components/plotly/plotly.pyi
+-rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.4.8a1/reflex/components/radix/__init__.py
+-rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.4.8a1/reflex/components/radix/primitives/__init__.py
+-rw-r--r--   0        0        0    21406 2024-03-20 23:54:55.846431 reflex-0.4.8a1/reflex/components/radix/primitives/accordion.py
+-rw-r--r--   0        0        0    26885 2024-04-12 01:14:12.273564 reflex-0.4.8a1/reflex/components/radix/primitives/accordion.pyi
+-rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.4.8a1/reflex/components/radix/primitives/base.py
+-rw-r--r--   0        0        0     6478 2024-04-12 01:14:12.273957 reflex-0.4.8a1/reflex/components/radix/primitives/base.pyi
+-rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.4.8a1/reflex/components/radix/primitives/drawer.py
+-rw-r--r--   0        0        0    34484 2024-04-12 01:14:12.274125 reflex-0.4.8a1/reflex/components/radix/primitives/drawer.pyi
+-rw-r--r--   0        0        0     4760 2024-03-20 23:54:55.847327 reflex-0.4.8a1/reflex/components/radix/primitives/form.py
+-rw-r--r--   0        0        0    47939 2024-04-12 01:14:12.274318 reflex-0.4.8a1/reflex/components/radix/primitives/form.pyi
+-rw-r--r--   0        0        0     3996 2024-03-20 23:54:55.847641 reflex-0.4.8a1/reflex/components/radix/primitives/progress.py
+-rw-r--r--   0        0        0    22784 2024-04-12 01:14:12.274470 reflex-0.4.8a1/reflex/components/radix/primitives/progress.pyi
+-rw-r--r--   0        0        0     5004 2024-03-20 23:54:55.848258 reflex-0.4.8a1/reflex/components/radix/primitives/slider.py
+-rw-r--r--   0        0        0    16697 2024-04-12 01:14:12.275306 reflex-0.4.8a1/reflex/components/radix/primitives/slider.pyi
+-rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.4.8a1/reflex/components/radix/themes/__init__.py
+-rw-r--r--   0        0        0     8097 2024-03-20 23:54:55.848920 reflex-0.4.8a1/reflex/components/radix/themes/base.py
+-rw-r--r--   0        0        0    24074 2024-04-12 01:14:12.275479 reflex-0.4.8a1/reflex/components/radix/themes/base.pyi
+-rw-r--r--   0        0        0     3007 2024-03-20 23:54:55.849383 reflex-0.4.8a1/reflex/components/radix/themes/color_mode.py
+-rw-r--r--   0        0        0    21283 2024-04-04 14:57:26.391843 reflex-0.4.8a1/reflex/components/radix/themes/color_mode.pyi
+-rw-r--r--   0        0        0     1776 2024-02-17 20:02:02.427848 reflex-0.4.8a1/reflex/components/radix/themes/components/__init__.py
+-rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.py
+-rw-r--r--   0        0        0    24434 2024-04-04 14:57:26.391969 reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.pyi
+-rw-r--r--   0        0        0    40237 2024-02-17 20:02:02.428774 reflex-0.4.8a1/reflex/components/radix/themes/components/alertdialog.pyi
+-rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.4.8a1/reflex/components/radix/themes/components/aspect_ratio.py
+-rw-r--r--   0        0        0     3640 2024-04-04 14:57:26.392096 reflex-0.4.8a1/reflex/components/radix/themes/components/aspect_ratio.pyi
+-rw-r--r--   0        0        0     5724 2024-02-17 20:02:02.429087 reflex-0.4.8a1/reflex/components/radix/themes/components/aspectratio.pyi
+-rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.py
+-rw-r--r--   0        0        0     6562 2024-04-04 14:57:26.392242 reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.pyi
+-rw-r--r--   0        0        0      815 2024-02-17 20:02:02.429580 reflex-0.4.8a1/reflex/components/radix/themes/components/badge.py
+-rw-r--r--   0        0        0     9315 2024-04-04 14:57:26.392362 reflex-0.4.8a1/reflex/components/radix/themes/components/badge.pyi
+-rw-r--r--   0        0        0     1084 2024-02-17 20:02:02.429875 reflex-0.4.8a1/reflex/components/radix/themes/components/button.py
+-rw-r--r--   0        0        0    11758 2024-04-04 14:57:26.392476 reflex-0.4.8a1/reflex/components/radix/themes/components/button.pyi
+-rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.4.8a1/reflex/components/radix/themes/components/callout.py
+-rw-r--r--   0        0        0    38710 2024-04-04 14:57:26.392589 reflex-0.4.8a1/reflex/components/radix/themes/components/callout.pyi
+-rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.4.8a1/reflex/components/radix/themes/components/card.py
+-rw-r--r--   0        0        0     7200 2024-04-04 14:57:26.392715 reflex-0.4.8a1/reflex/components/radix/themes/components/card.pyi
+-rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.py
+-rw-r--r--   0        0        0    20877 2024-04-04 14:57:26.392804 reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.pyi
+-rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.py
+-rw-r--r--   0        0        0    31192 2024-04-04 14:57:26.392918 reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.pyi
+-rw-r--r--   0        0        0    44130 2024-02-17 20:02:02.432309 reflex-0.4.8a1/reflex/components/radix/themes/components/contextmenu.pyi
+-rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.py
+-rw-r--r--   0        0        0    24895 2024-04-04 14:57:26.393065 reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.pyi
+-rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.py
+-rw-r--r--   0        0        0    37901 2024-04-04 14:57:26.393223 reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.pyi
+-rw-r--r--   0        0        0    52185 2024-02-17 20:02:02.435613 reflex-0.4.8a1/reflex/components/radix/themes/components/dropdownmenu.pyi
+-rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.py
+-rw-r--r--   0        0        0    17744 2024-04-04 14:57:26.393356 reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.pyi
+-rw-r--r--   0        0        0    26453 2024-02-17 20:02:02.436260 reflex-0.4.8a1/reflex/components/radix/themes/components/hovercard.pyi
+-rw-r--r--   0        0        0     2789 2024-03-20 23:54:55.853758 reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.py
+-rw-r--r--   0        0        0    11916 2024-04-04 14:57:26.393481 reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.pyi
+-rw-r--r--   0        0        0    12021 2024-02-17 20:02:02.436631 reflex-0.4.8a1/reflex/components/radix/themes/components/iconbutton.pyi
+-rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.4.8a1/reflex/components/radix/themes/components/inset.py
+-rw-r--r--   0        0        0     7889 2024-04-04 14:57:26.393614 reflex-0.4.8a1/reflex/components/radix/themes/components/inset.pyi
+-rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.4.8a1/reflex/components/radix/themes/components/popover.py
+-rw-r--r--   0        0        0    17404 2024-04-04 14:57:26.393725 reflex-0.4.8a1/reflex/components/radix/themes/components/popover.pyi
+-rw-r--r--   0        0        0     6253 2024-03-20 23:54:55.854319 reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.py
+-rw-r--r--   0        0        0    24106 2024-04-04 14:57:26.393848 reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.pyi
+-rw-r--r--   0        0        0    26222 2024-03-20 23:54:55.854920 reflex-0.4.8a1/reflex/components/radix/themes/components/radiogroup.pyi
+-rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.py
+-rw-r--r--   0        0        0     4427 2024-04-04 14:57:26.393997 reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.pyi
+-rw-r--r--   0        0        0     6513 2024-02-17 20:02:02.439025 reflex-0.4.8a1/reflex/components/radix/themes/components/scrollarea.pyi
+-rw-r--r--   0        0        0     8028 2024-04-05 17:14:14.462095 reflex-0.4.8a1/reflex/components/radix/themes/components/select.py
+-rw-r--r--   0        0        0    45123 2024-04-04 14:57:26.394155 reflex-0.4.8a1/reflex/components/radix/themes/components/select.pyi
+-rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.4.8a1/reflex/components/radix/themes/components/separator.py
+-rw-r--r--   0        0        0     6078 2024-04-04 14:57:26.394306 reflex-0.4.8a1/reflex/components/radix/themes/components/separator.pyi
+-rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.4.8a1/reflex/components/radix/themes/components/slider.py
+-rw-r--r--   0        0        0     8162 2024-04-04 14:57:26.394440 reflex-0.4.8a1/reflex/components/radix/themes/components/slider.pyi
+-rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.4.8a1/reflex/components/radix/themes/components/switch.py
+-rw-r--r--   0        0        0     7404 2024-04-04 14:57:26.394593 reflex-0.4.8a1/reflex/components/radix/themes/components/switch.pyi
+-rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.4.8a1/reflex/components/radix/themes/components/table.py
+-rw-r--r--   0        0        0    47387 2024-04-04 14:57:26.394744 reflex-0.4.8a1/reflex/components/radix/themes/components/table.pyi
+-rw-r--r--   0        0        0     2213 2024-03-20 23:54:55.858062 reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.py
+-rw-r--r--   0        0        0    17321 2024-04-04 14:57:26.394873 reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.pyi
+-rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.py
+-rw-r--r--   0        0        0    11711 2024-04-04 14:57:26.395020 reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.pyi
+-rw-r--r--   0        0        0     5106 2024-03-20 23:54:55.858542 reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.py
+-rw-r--r--   0        0        0    43043 2024-04-04 14:57:26.395140 reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.pyi
+-rw-r--r--   0        0        0    43365 2024-02-17 20:02:02.442188 reflex-0.4.8a1/reflex/components/radix/themes/components/textfield.pyi
+-rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.py
+-rw-r--r--   0        0        0     8092 2024-04-04 14:57:26.395307 reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.pyi
+-rw-r--r--   0        0        0      811 2024-04-04 14:19:59.340548 reflex-0.4.8a1/reflex/components/radix/themes/layout/__init__.py
+-rw-r--r--   0        0        0     1201 2024-03-20 23:54:55.859150 reflex-0.4.8a1/reflex/components/radix/themes/layout/base.py
+-rw-r--r--   0        0        0     7643 2024-04-04 14:57:26.395455 reflex-0.4.8a1/reflex/components/radix/themes/layout/base.pyi
+-rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.4.8a1/reflex/components/radix/themes/layout/box.py
+-rw-r--r--   0        0        0     6462 2024-04-04 14:57:26.395640 reflex-0.4.8a1/reflex/components/radix/themes/layout/box.pyi
+-rw-r--r--   0        0        0      422 2024-03-20 23:54:55.859399 reflex-0.4.8a1/reflex/components/radix/themes/layout/center.py
+-rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.395883 reflex-0.4.8a1/reflex/components/radix/themes/layout/center.pyi
+-rw-r--r--   0        0        0      552 2024-02-07 21:48:43.319123 reflex-0.4.8a1/reflex/components/radix/themes/layout/container.py
+-rw-r--r--   0        0        0     6779 2024-04-04 14:57:26.396069 reflex-0.4.8a1/reflex/components/radix/themes/layout/container.pyi
+-rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.py
+-rw-r--r--   0        0        0     8501 2024-04-04 14:57:26.396231 reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.pyi
+-rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.py
+-rw-r--r--   0        0        0     8907 2024-04-04 14:57:26.396387 reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.pyi
+-rw-r--r--   0        0        0     4889 2024-04-04 14:19:59.341578 reflex-0.4.8a1/reflex/components/radix/themes/layout/list.py
+-rw-r--r--   0        0        0    29367 2024-04-04 14:57:26.396553 reflex-0.4.8a1/reflex/components/radix/themes/layout/list.pyi
+-rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.4.8a1/reflex/components/radix/themes/layout/section.py
+-rw-r--r--   0        0        0     6758 2024-04-04 14:57:26.396712 reflex-0.4.8a1/reflex/components/radix/themes/layout/section.pyi
+-rw-r--r--   0        0        0      412 2024-03-20 23:54:55.861110 reflex-0.4.8a1/reflex/components/radix/themes/layout/spacer.py
+-rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.396834 reflex-0.4.8a1/reflex/components/radix/themes/layout/spacer.pyi
+-rw-r--r--   0        0        0     1270 2024-03-20 23:54:55.861618 reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.py
+-rw-r--r--   0        0        0    22132 2024-04-04 14:57:26.396967 reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.pyi
+-rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.4.8a1/reflex/components/radix/themes/typography/__init__.py
+-rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.4.8a1/reflex/components/radix/themes/typography/base.py
+-rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.py
+-rw-r--r--   0        0        0     9316 2024-04-04 14:57:26.397104 reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.pyi
+-rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.4.8a1/reflex/components/radix/themes/typography/code.py
+-rw-r--r--   0        0        0     9513 2024-04-04 14:57:26.397215 reflex-0.4.8a1/reflex/components/radix/themes/typography/code.pyi
+-rw-r--r--   0        0        0     8547 2024-02-17 20:02:02.446585 reflex-0.4.8a1/reflex/components/radix/themes/typography/em.pyi
+-rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.py
+-rw-r--r--   0        0        0    10106 2024-04-04 14:57:26.397327 reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.pyi
+-rw-r--r--   0        0        0     8872 2024-02-17 20:02:02.446866 reflex-0.4.8a1/reflex/components/radix/themes/typography/kbd.pyi
+-rw-r--r--   0        0        0     3154 2024-03-20 23:54:55.862398 reflex-0.4.8a1/reflex/components/radix/themes/typography/link.py
+-rw-r--r--   0        0        0    12063 2024-04-04 14:57:26.397447 reflex-0.4.8a1/reflex/components/radix/themes/typography/link.pyi
+-rw-r--r--   0        0        0     8701 2024-02-17 20:02:02.447165 reflex-0.4.8a1/reflex/components/radix/themes/typography/quote.pyi
+-rw-r--r--   0        0        0     8563 2024-02-17 20:02:02.447296 reflex-0.4.8a1/reflex/components/radix/themes/typography/strong.pyi
+-rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.4.8a1/reflex/components/radix/themes/typography/text.py
+-rw-r--r--   0        0        0    57238 2024-04-04 14:57:26.397579 reflex-0.4.8a1/reflex/components/radix/themes/typography/text.pyi
+-rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.4.8a1/reflex/components/react_player/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.4.8a1/reflex/components/react_player/audio.py
+-rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.275710 reflex-0.4.8a1/reflex/components/react_player/audio.pyi
+-rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.4.8a1/reflex/components/react_player/react_player.py
+-rw-r--r--   0        0        0     4354 2024-04-12 01:14:12.275922 reflex-0.4.8a1/reflex/components/react_player/react_player.pyi
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.4.8a1/reflex/components/react_player/video.py
+-rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.276135 reflex-0.4.8a1/reflex/components/react_player/video.pyi
+-rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.4.8a1/reflex/components/recharts/__init__.py
+-rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.4.8a1/reflex/components/recharts/cartesian.py
+-rw-r--r--   0        0        0    84151 2024-04-12 01:14:12.276362 reflex-0.4.8a1/reflex/components/recharts/cartesian.pyi
+-rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.4.8a1/reflex/components/recharts/charts.py
+-rw-r--r--   0        0        0    48757 2024-04-04 14:57:26.398259 reflex-0.4.8a1/reflex/components/recharts/charts.pyi
+-rw-r--r--   0        0        0     5624 2024-02-06 00:51:32.028409 reflex-0.4.8a1/reflex/components/recharts/general.py
+-rw-r--r--   0        0        0    22787 2024-04-12 01:14:12.276538 reflex-0.4.8a1/reflex/components/recharts/general.pyi
+-rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.4.8a1/reflex/components/recharts/polar.py
+-rw-r--r--   0        0        0    24326 2024-04-12 01:14:12.276828 reflex-0.4.8a1/reflex/components/recharts/polar.pyi
+-rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.4.8a1/reflex/components/recharts/recharts.py
+-rw-r--r--   0        0        0     8535 2024-04-12 01:14:12.277140 reflex-0.4.8a1/reflex/components/recharts/recharts.pyi
+-rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.4.8a1/reflex/components/suneditor/__init__.py
+-rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.4.8a1/reflex/components/suneditor/editor.py
+-rw-r--r--   0        0        0    10330 2024-04-04 14:57:26.398718 reflex-0.4.8a1/reflex/components/suneditor/editor.pyi
+-rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.4.8a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.4.8a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3620 2024-02-06 00:51:32.029458 reflex-0.4.8a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.4.8a1/reflex/components/tags/match_tag.py
+-rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.4.8a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.4.8a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0    11082 2024-04-05 17:14:06.328847 reflex-0.4.8a1/reflex/config.py
+-rw-r--r--   0        0        0     3318 2024-04-05 17:14:06.329003 reflex-0.4.8a1/reflex/config.pyi
+-rw-r--r--   0        0        0     2128 2024-04-12 01:14:12.277275 reflex-0.4.8a1/reflex/constants/__init__.py
+-rw-r--r--   0        0        0     5833 2024-04-12 01:14:12.277500 reflex-0.4.8a1/reflex/constants/base.py
+-rw-r--r--   0        0        0     2980 2024-04-05 17:14:14.462329 reflex-0.4.8a1/reflex/constants/base.pyi
+-rw-r--r--   0        0        0     1599 2024-03-20 23:54:55.865089 reflex-0.4.8a1/reflex/constants/colors.py
+-rw-r--r--   0        0        0     4207 2024-04-12 01:14:12.277724 reflex-0.4.8a1/reflex/constants/compiler.py
+-rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.4.8a1/reflex/constants/config.py
+-rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.4.8a1/reflex/constants/custom_components.py
+-rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.4.8a1/reflex/constants/event.py
+-rw-r--r--   0        0        0     3223 2024-04-12 01:14:12.277858 reflex-0.4.8a1/reflex/constants/installer.py
+-rw-r--r--   0        0        0     1940 2024-03-20 23:54:55.865486 reflex-0.4.8a1/reflex/constants/route.py
+-rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.4.8a1/reflex/constants/style.py
+-rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.4.8a1/reflex/custom_components/__init__.py
+-rw-r--r--   0        0        0    31705 2024-04-11 18:27:43.382941 reflex-0.4.8a1/reflex/custom_components/custom_components.py
+-rw-r--r--   0        0        0    26537 2024-04-12 01:14:12.278011 reflex-0.4.8a1/reflex/event.py
+-rw-r--r--   0        0        0      369 2024-04-12 01:14:12.278154 reflex-0.4.8a1/reflex/experimental/__init__.py
+-rw-r--r--   0        0        0     1647 2024-04-05 17:14:14.462793 reflex-0.4.8a1/reflex/experimental/hooks.py
+-rw-r--r--   0        0        0      281 2024-04-12 01:14:12.278217 reflex-0.4.8a1/reflex/experimental/misc.py
+-rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.4.8a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.4.8a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.4.8a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0    13116 2024-04-12 01:14:12.278614 reflex-0.4.8a1/reflex/model.py
+-rw-r--r--   0        0        0     1921 2024-04-05 17:14:14.463098 reflex-0.4.8a1/reflex/page.py
+-rw-r--r--   0        0        0    17828 2024-04-12 01:14:12.279090 reflex-0.4.8a1/reflex/reflex.py
+-rw-r--r--   0        0        0     2908 2024-03-20 23:54:55.866329 reflex-0.4.8a1/reflex/route.py
+-rw-r--r--   0        0        0   105642 2024-04-04 14:57:26.399697 reflex-0.4.8a1/reflex/state.py
+-rw-r--r--   0        0        0     8834 2024-04-04 14:57:26.399846 reflex-0.4.8a1/reflex/style.py
+-rw-r--r--   0        0        0    29808 2024-04-05 17:14:14.463602 reflex-0.4.8a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.4.8a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.4.8a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1255 2024-04-12 01:14:12.279414 reflex-0.4.8a1/reflex/utils/compat.py
+-rw-r--r--   0        0        0     5168 2024-04-12 01:14:12.279640 reflex-0.4.8a1/reflex/utils/console.py
+-rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.4.8a1/reflex/utils/exceptions.py
+-rw-r--r--   0        0        0     9969 2024-04-05 17:14:14.463946 reflex-0.4.8a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0     2270 2024-04-12 01:14:12.279905 reflex-0.4.8a1/reflex/utils/export.py
+-rw-r--r--   0        0        0    22648 2024-03-20 23:54:55.867980 reflex-0.4.8a1/reflex/utils/format.py
+-rw-r--r--   0        0        0     2277 2024-04-12 01:14:12.280013 reflex-0.4.8a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.4.8a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    46993 2024-04-12 01:14:12.280227 reflex-0.4.8a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0    10050 2024-04-12 01:14:12.280420 reflex-0.4.8a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0    27674 2024-04-04 14:57:26.400476 reflex-0.4.8a1/reflex/utils/pyi_generator.py
+-rw-r--r--   0        0        0     8771 2024-04-11 18:27:43.383699 reflex-0.4.8a1/reflex/utils/serializers.py
+-rw-r--r--   0        0        0     4013 2024-04-04 14:57:26.400591 reflex-0.4.8a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0    13679 2024-04-12 01:14:12.280735 reflex-0.4.8a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.4.8a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    67152 2024-04-04 14:57:26.400899 reflex-0.4.8a1/reflex/vars.py
+-rw-r--r--   0        0        0     5583 2024-04-04 14:57:26.401034 reflex-0.4.8a1/reflex/vars.pyi
+-rw-r--r--   0        0        0    11764 1970-01-01 00:00:00.000000 reflex-0.4.8a1/PKG-INFO
```

### Comparing `reflex-0.4.7a3/LICENSE` & `reflex-0.4.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/README.md` & `reflex-0.4.8a1/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/pyproject.toml` & `reflex-0.4.8a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.4.7a3"
+version = "0.4.8a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
     "Masen Furer <masen@reflex.dev>",
     "Elijah Ahianyo <elijah@reflex.dev>",
```

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/blank/assets/favicon.ico` & `reflex-0.4.8a1/reflex/.templates/apps/blank/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/blank/code/blank.py` & `reflex-0.4.8a1/reflex/.templates/apps/blank/code/blank.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/assets/favicon.ico` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/assets/github.svg` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/assets/icon.svg` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/assets/logo.svg` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/assets/paneleft.svg` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/demo.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/demo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/chatapp.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/chatapp.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/datatable.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/forms.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/graphing.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/graphing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/pages/home.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/home.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/sidebar.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/states/form_state.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/form_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/states/pie_state.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/pie_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/styles.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/chat.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/chat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/loading_icon.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/modal.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/navbar.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/navbar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/components/sidebar.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/state.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/apps/demo/code/webui/styles.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/jinja/custom_components/demo_app.py.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/jinja/custom_components/src.py.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/custom_components/src.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/jinja/web/package.json.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/package.json.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/jinja/web/pages/_app.js.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/pages/_app.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/jinja/web/pages/custom_component.js.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/jinja/web/utils/context.js.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/utils/context.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js` & `reflex-0.4.8a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js` & `reflex-0.4.8a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/web/utils/client_side_routing.js` & `reflex-0.4.8a1/reflex/.templates/web/utils/client_side_routing.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/web/utils/helpers/dataeditor.js` & `reflex-0.4.8a1/reflex/.templates/web/utils/helpers/dataeditor.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/web/utils/helpers/range.js` & `reflex-0.4.8a1/reflex/.templates/web/utils/helpers/range.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/.templates/web/utils/state.js` & `reflex-0.4.8a1/reflex/.templates/web/utils/state.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -252,15 +252,21 @@
  * @param event The current event.
  * @param socket The socket object to send the response event(s) on.
  *
  * @returns Whether the event was sent.
  */
 export const applyRestEvent = async (event, socket) => {
     let eventSent = false;
-    if (event.handler == "uploadFiles") {
+    if (event.handler === "uploadFiles") {
+
+        if (event.payload.files === undefined || event.payload.files.length === 0) {
+            // Submit the event over the websocket to trigger the event handler.
+            return await applyEvent(Event(event.name), socket)
+        }
+
         // Start upload, but do not wait for it, which would block other events.
         uploadFiles(
             event.name,
             event.payload.files,
             event.payload.upload_id,
             event.payload.on_upload_progress,
             socket
```

### Comparing `reflex-0.4.7a3/reflex/__init__.py` & `reflex-0.4.8a1/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/__init__.pyi` & `reflex-0.4.8a1/reflex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/app.py` & `reflex-0.4.8a1/reflex/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -725,17 +725,20 @@
 
         This can move back into `compile_` when py39 support is dropped.
         """
         # Add the @rx.page decorated pages to collect on_load events.
         for render, kwargs in DECORATED_PAGES:
             self.add_page(render, **kwargs)
 
-    def compile_(self):
+    def compile_(self, export: bool = False):
         """Compile the app and output it to the pages folder.
 
+        Args:
+            export: Whether to compile the app for export.
+
         Raises:
             RuntimeError: When any page uses state, but no rx.State subclass is defined.
         """
         # Render a default 404 page if the user didn't supply one
         if constants.Page404.SLUG not in self.pages:
             self.add_custom_404_page()
 
@@ -933,14 +936,25 @@
 
         progress.advance(task)
         progress.stop()
 
         # Install frontend packages.
         self.get_frontend_packages(all_imports)
 
+        # Setup the next.config.js
+        transpile_packages = [
+            package
+            for package, import_vars in all_imports.items()
+            if any(import_var.transpile for import_var in import_vars)
+        ]
+        prerequisites.update_next_config(
+            export=export,
+            transpile_packages=transpile_packages,
+        )
+
         for output_path, code in compile_results:
             compiler_utils.write_page(output_path, code)
 
     @contextlib.asynccontextmanager
     async def modify_state(self, token: str) -> AsyncIterator[BaseState]:
         """Modify the state out of band.
```

### Comparing `reflex-0.4.7a3/reflex/app.pyi` & `reflex-0.4.8a1/reflex/app.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/app_module_for_backend.py` & `reflex-0.4.8a1/reflex/app_module_for_backend.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/base.py` & `reflex-0.4.8a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/compiler/compiler.py` & `reflex-0.4.8a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/compiler/templates.py` & `reflex-0.4.8a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/compiler/utils.py` & `reflex-0.4.8a1/reflex/compiler/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from urllib.parse import urlparse
 
 try:
     # TODO The type checking guard can be removed once
     # reflex-hosting-cli tools are compatible with pydantic v2
 
     if not TYPE_CHECKING:
-        import pydantic.v1.fields as ModelField
+        from pydantic.v1.fields import ModelField
     else:
         raise ModuleNotFoundError
 except ModuleNotFoundError:
     from pydantic.fields import ModelField
 
 from reflex import constants
 from reflex.components.base import (
```

### Comparing `reflex-0.4.7a3/reflex/components/__init__.py` & `reflex-0.4.8a1/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/base/app_wrap.py` & `reflex-0.4.8a1/reflex/components/base/app_wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/base/app_wrap.pyi` & `reflex-0.4.8a1/reflex/components/base/app_wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/base/bare.py` & `reflex-0.4.8a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/base/body.pyi` & `reflex-0.4.8a1/reflex/components/next/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-"""Stub file for reflex/components/base/body.py"""
+"""Stub file for reflex/components/next/base.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from reflex.components.component import Component
 
-class Body(Component):
+class NextComponent(Component):
+    ...
+
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -63,27 +65,24 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Body":
+    ) -> "NextComponent":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/base/document.py` & `reflex-0.4.8a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/base/document.pyi` & `reflex-0.4.8a1/reflex/components/base/document.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Html(NextDocumentLib):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -159,17 +156,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DocumentHead(NextDocumentLib):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -238,17 +232,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Main(NextDocumentLib):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -317,17 +308,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class NextScript(NextDocumentLib):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -396,12 +384,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/base/fragment.pyi` & `reflex-0.4.8a1/reflex/components/base/fragment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -78,12 +78,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/base/head.pyi` & `reflex-0.4.8a1/reflex/components/base/head.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Head(NextHeadLib, MemoizationLeaf):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.4.7a3/reflex/components/base/link.py` & `reflex-0.4.8a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/base/link.pyi` & `reflex-0.4.8a1/reflex/components/base/link.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ScriptTag(Component):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -176,12 +173,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/base/meta.py` & `reflex-0.4.8a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/base/meta.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/card.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-"""Stub file for reflex/components/base/meta.py"""
+"""Stub file for reflex/components/chakra/layout/card.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional
-from reflex.components.base.bare import Bare
+from reflex.components.chakra import (
+    ChakraComponent,
+    LiteralCardVariant,
+    LiteralColorScheme,
+    LiteralTagSize,
+)
 from reflex.components.component import Component
+from reflex.vars import Var
 
-class Title(Component):
-    def render(self) -> dict: ...
+class CardHeader(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -66,46 +71,38 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Title":
+    ) -> "CardHeader":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class Meta(Component):
+class CardBody(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        char_set: Optional[str] = None,
-        content: Optional[str] = None,
-        name: Optional[str] = None,
-        property: Optional[str] = None,
-        http_equiv: Optional[str] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -150,51 +147,38 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Meta":
+    ) -> "CardBody":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            char_set: The description of character encoding.
-            content: The value of meta.
-            name: The name of metadata.
-            property: The type of metadata value.
-            http_equiv: The type of metadata value.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class Description(Meta):
+class CardFooter(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        name: Optional[str] = None,
-        char_set: Optional[str] = None,
-        content: Optional[str] = None,
-        property: Optional[str] = None,
-        http_equiv: Optional[str] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -239,51 +223,100 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Description":
+    ) -> "CardFooter":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            name: The name of metadata.
-            char_set: The description of character encoding.
-            content: The value of meta.
-            property: The type of metadata value.
-            http_equiv: The type of metadata value.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class Image(Meta):
+class Card(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        property: Optional[str] = None,
-        char_set: Optional[str] = None,
-        content: Optional[str] = None,
-        name: Optional[str] = None,
-        http_equiv: Optional[str] = None,
+        header: Optional[Component] = None,
+        footer: Optional[Component] = None,
+        align: Optional[Union[Var[str], str]] = None,
+        direction: Optional[Union[Var[str], str]] = None,
+        justify: Optional[Union[Var[str], str]] = None,
+        color_scheme: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "none",
+                        "gray",
+                        "red",
+                        "orange",
+                        "yellow",
+                        "green",
+                        "teal",
+                        "blue",
+                        "cyan",
+                        "purple",
+                        "pink",
+                        "whiteAlpha",
+                        "blackAlpha",
+                        "linkedin",
+                        "facebook",
+                        "messenger",
+                        "whatsapp",
+                        "twitter",
+                        "telegram",
+                    ]
+                ],
+                Literal[
+                    "none",
+                    "gray",
+                    "red",
+                    "orange",
+                    "yellow",
+                    "green",
+                    "teal",
+                    "blue",
+                    "cyan",
+                    "purple",
+                    "pink",
+                    "whiteAlpha",
+                    "blackAlpha",
+                    "linkedin",
+                    "facebook",
+                    "messenger",
+                    "whatsapp",
+                    "twitter",
+                    "telegram",
+                ],
+            ]
+        ] = None,
+        size: Optional[
+            Union[Var[Literal["sm", "md", "lg"]], Literal["sm", "md", "lg"]]
+        ] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["outline", "filled", "elevated", "unstyled"]],
+                Literal["outline", "filled", "elevated", "unstyled"],
+            ]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -328,32 +361,23 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Image":
-        """Create the component.
+    ) -> "Card":
+        """Creates a Chakra Card with a body and optionally header and/or footer, and returns it.
+        If header, body or footer are not already instances of Chead, Cbody or Cfoot respectively,
+        they will be wrapped as such for layout purposes. If you want to modify their props,
+        e.g. padding_left, you should wrap them yourself.
 
         Args:
-            *children: The children of the component.
-            property: The type of metadata value.
-            char_set: The description of character encoding.
-            content: The value of meta.
-            name: The name of metadata.
-            http_equiv: The type of metadata value.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
+            body (Component): The main content of the Card that will be created.
+            header (Optional[Component]): The header of the Card.
+            footer (Optional[Component]): The footer of the Card.
+            props: The properties to be passed to the component.
 
         Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
+            The `create()` method returns a Card object.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/base/script.py` & `reflex-0.4.8a1/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/base/script.pyi` & `reflex-0.4.8a1/reflex/components/base/script.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/__init__.py` & `reflex-0.4.8a1/reflex/components/chakra/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/base.py` & `reflex-0.4.8a1/reflex/components/chakra/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/base.pyi` & `reflex-0.4.8a1/reflex/components/chakra/base.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -82,17 +82,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ChakraProvider(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -230,17 +227,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 chakra_color_mode_provider = ChakraColorModeProvider.create()
 LiteralColorScheme = Literal[
     "none",
     "gray",
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/badge.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/container.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-"""Stub file for reflex/components/chakra/datadisplay/badge.py"""
+"""Stub file for reflex/components/chakra/layout/container.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex.components.chakra import ChakraComponent, LiteralVariant
+from reflex.components.chakra import ChakraComponent
 from reflex.vars import Var
 
-class Badge(ChakraComponent):
+class Container(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        variant: Optional[
-            Union[
-                Var[Literal["solid", "subtle", "outline"]],
-                Literal["solid", "subtle", "outline"],
-            ]
-        ] = None,
-        color_scheme: Optional[Union[Var[str], str]] = None,
+        center_content: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -71,29 +65,25 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Badge":
+    ) -> "Container":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            variant: Variant of the badge ("solid" | "subtle" | "outline")
-            color_scheme: The color of the badge
+            center_content: If true, container will center its children regardless of their width.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/code.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/code.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -78,12 +78,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/divider.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/divider.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -93,12 +93,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/keyboard_key.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/spacer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Stub file for reflex/components/chakra/datadisplay/keyboard_key.py"""
+"""Stub file for reflex/components/chakra/layout/spacer.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from reflex.components.chakra import ChakraComponent
 
-class KeyboardKey(ChakraComponent):
+class Spacer(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -63,27 +63,24 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "KeyboardKey":
+    ) -> "Spacer":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/list.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/list.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -165,17 +165,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class OrderedList(List):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/stat.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/stat.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -164,17 +164,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StatNumber(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -243,17 +240,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StatHelpText(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -322,17 +316,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StatArrow(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -403,17 +394,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StatGroup(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -482,12 +470,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/table.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/table.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -498,17 +498,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Td(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -579,17 +576,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TableCaption(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -660,17 +654,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TableContainer(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -739,12 +730,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/tag.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/datadisplay/tag.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TagLeftIcon(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -165,17 +162,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TagRightIcon(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -244,17 +238,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TagCloseButton(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -323,17 +314,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Tag(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/disclosure/accordion.py` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/disclosure/accordion.pyi` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -181,17 +181,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AccordionButton(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -260,17 +257,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AccordionPanel(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -339,17 +333,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AccordionIcon(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -418,12 +409,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/disclosure/tabs.py` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/disclosure/tabs.pyi` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -265,17 +265,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TabList(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -344,17 +341,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TabPanels(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -423,17 +417,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TabPanel(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -502,12 +493,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/disclosure/transition.py` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/disclosure/transition.pyi` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Fade(Transition):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -167,17 +164,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ScaleFade(Transition):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -254,17 +248,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Slide(Transition):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -339,17 +330,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class SlideFade(Transition):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -428,17 +416,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Collapse(Transition):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -517,12 +502,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/disclosure/visuallyhidden.pyi` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/visuallyhidden.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -78,12 +78,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/alert.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/alert.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/alert.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -176,17 +176,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AlertTitle(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -255,17 +252,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AlertDescription(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -334,12 +328,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/circularprogress.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/circularprogress.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -179,12 +179,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/progress.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/progress.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/progress.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -94,12 +94,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/skeleton.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/skeleton.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class SkeletonCircle(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -178,17 +175,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class SkeletonText(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -269,12 +263,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/spinner.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/feedback/spinner.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -94,12 +94,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/__init__.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/button.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/button.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/button.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -166,17 +166,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ButtonGroup(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -262,12 +259,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/checkbox.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/checkbox.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class CheckboxGroup(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -245,12 +242,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/colormodeswitch.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/colormodeswitch.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -464,12 +464,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/date_picker.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/date_time_picker.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/date_time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/editable.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/editable.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-"""Stub file for reflex/components/chakra/forms/editable.py"""
+"""Stub file for reflex/components/chakra/forms/rangeslider.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Union
-from reflex.components.chakra import ChakraComponent
+from typing import Any, List, Optional, Union
+from reflex.components.chakra import ChakraComponent, LiteralChakraDirection
+from reflex.components.component import Component
 from reflex.constants import EventTriggers
+from reflex.utils import format
 from reflex.vars import Var
 
-class Editable(ChakraComponent):
+class RangeSlider(ChakraComponent):
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+    def get_ref(self): ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        value: Optional[Union[Var[List[int]], List[int]]] = None,
+        default_value: Optional[Union[Var[List[int]], List[int]]] = None,
+        direction: Optional[
+            Union[Var[Literal["ltr", "rtl"]], Literal["ltr", "rtl"]]
+        ] = None,
+        focus_thumb_on_change: Optional[Union[Var[bool], bool]] = None,
         is_disabled: Optional[Union[Var[bool], bool]] = None,
-        is_preview_focusable: Optional[Union[Var[bool], bool]] = None,
-        placeholder: Optional[Union[Var[str], str]] = None,
-        select_all_on_focus: Optional[Union[Var[bool], bool]] = None,
-        start_with_edit_view: Optional[Union[Var[bool], bool]] = None,
-        submit_on_blur: Optional[Union[Var[bool], bool]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        default_value: Optional[Union[Var[str], str]] = None,
+        is_read_only: Optional[Union[Var[bool], bool]] = None,
+        is_reversed: Optional[Union[Var[bool], bool]] = None,
+        min_: Optional[Union[Var[int], int]] = None,
+        max_: Optional[Union[Var[int], int]] = None,
+        min_steps_between_thumbs: Optional[Union[Var[int], int]] = None,
+        name: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_cancel: Optional[
+        on_change: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
+        on_change_end: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_change_start: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_edit: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
@@ -80,51 +88,50 @@
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_submit: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Editable":
-        """Create the component.
+    ) -> "RangeSlider":
+        """Create a RangeSlider component.
+
+        If no children are provided, a default RangeSlider will be created.
 
         Args:
             *children: The children of the component.
-            is_disabled: If true, the Editable will be disabled.
-            is_preview_focusable: If true, the read only view, has a tabIndex set to 0 so it can receive focus via the keyboard or click.
-            placeholder: The placeholder text when the value is empty.
-            select_all_on_focus: If true, the input's text will be highlighted on focus.
-            start_with_edit_view: If true, the Editable will start with edit mode by default.
-            submit_on_blur: If true, it'll update the value onBlur and turn off the edit mode.
-            value: The value of the Editable in both edit & preview mode
-            default_value: The initial value of the Editable in both edit and preview mode.
+            value: State var to bind the input.
+            default_value: The default values.
+            direction: The writing mode ("ltr" | "rtl")
+            focus_thumb_on_change: If false, the slider handle will not capture focus when value changes.
+            is_disabled: If true, the slider will be disabled
+            is_read_only: If true, the slider will be in `read-only` state.
+            is_reversed: If true, the value will be incremented or decremented in reverse.
+            min_: The minimum value of the slider.
+            max_: The maximum value of the slider.
+            min_steps_between_thumbs: The minimum distance between slider thumbs. Useful for preventing the thumbs from being too close together.
+            name: The name of the form field
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: The properties of the component.
 
         Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
+            The RangeSlider component.
         """
         ...
 
-class EditableInput(ChakraComponent):
+class RangeSliderTrack(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -174,36 +181,33 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "EditableInput":
+    ) -> "RangeSliderTrack":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class EditableTextarea(ChakraComponent):
+class RangeSliderFilledTrack(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -253,41 +257,40 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "EditableTextarea":
+    ) -> "RangeSliderFilledTrack":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class EditablePreview(ChakraComponent):
+class RangeSliderThumb(ChakraComponent):
+    def get_ref(self): ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        index: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -332,27 +335,25 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "EditablePreview":
+    ) -> "RangeSliderThumb":
         """Create the component.
 
         Args:
             *children: The children of the component.
+            index: The position of the thumb.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/email.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/email.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/form.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/form.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/form.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -351,17 +351,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FormLabel(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -432,17 +429,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FormErrorMessage(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -511,12 +505,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/iconbutton.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/iconbutton.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -101,12 +101,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/input.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/input.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/input.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -261,17 +261,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class InputLeftAddon(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -340,17 +337,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class InputRightAddon(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -419,17 +413,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class InputLeftElement(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -498,17 +489,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class InputRightElement(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -577,12 +565,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/multiselect.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/numberinput.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/numberinput.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,37 @@
-"""Stub file for reflex/components/chakra/forms/numberinput.py"""
+"""Stub file for reflex/components/radix/themes/components/tabs.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from numbers import Number
-from typing import Any, Dict
-from reflex.components.chakra import (
-    ChakraComponent,
-    LiteralButtonSize,
-    LiteralInputVariant,
-)
-from reflex.components.component import Component
+from typing import Any, Dict, List, Literal
+from reflex.components.component import ComponentNamespace
 from reflex.constants import EventTriggers
 from reflex.vars import Var
+from ..base import RadixThemesComponent
 
-class NumberInput(ChakraComponent):
+class TabsRoot(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        value: Optional[Union[Var[Number], Number]] = None,
-        allow_mouse_wheel: Optional[Union[Var[bool], bool]] = None,
-        clamped_value_on_blur: Optional[Union[Var[bool], bool]] = None,
-        default_value: Optional[Union[Var[Number], Number]] = None,
-        error_border_color: Optional[Union[Var[str], str]] = None,
-        focus_border_color: Optional[Union[Var[str], str]] = None,
-        focus_input_on_change: Optional[Union[Var[bool], bool]] = None,
-        is_disabled: Optional[Union[Var[bool], bool]] = None,
-        is_invalid: Optional[Union[Var[bool], bool]] = None,
-        is_read_only: Optional[Union[Var[bool], bool]] = None,
-        is_required: Optional[Union[Var[bool], bool]] = None,
-        is_valid_character: Optional[Union[Var[str], str]] = None,
-        keep_within_range: Optional[Union[Var[bool], bool]] = None,
-        max_: Optional[Union[Var[Number], Number]] = None,
-        min_: Optional[Union[Var[Number], Number]] = None,
-        variant: Optional[
+        default_value: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        orientation: Optional[
             Union[
-                Var[Literal["outline", "filled", "flushed", "unstyled"]],
-                Literal["outline", "filled", "flushed", "unstyled"],
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
             ]
         ] = None,
-        size: Optional[
-            Union[Var[Literal["sm", "md", "lg", "xs"]], Literal["sm", "md", "lg", "xs"]]
-        ] = None,
-        name: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -101,58 +79,45 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "NumberInput":
-        """Create a number input component.
+    ) -> "TabsRoot":
+        """Create a new component instance.
 
-        If no children are provided, a default stepper will be used.
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
-            value: State var to bind the input.
-            allow_mouse_wheel: If true, the input's value will change based on mouse wheel.
-            clamped_value_on_blur: This controls the value update when you blur out of the input. - If true and the value is greater than max, the value will be reset to max - Else, the value remains the same.
-            default_value: The initial value of the counter. Should be less than max and greater than min
-            error_border_color: The border color when the input is invalid.
-            focus_border_color: The border color when the input is focused.
-            focus_input_on_change: If true, the input will be focused as you increment or decrement the value with the stepper
-            is_disabled: Hints at the type of data that might be entered by the user. It also determines the type of keyboard shown to the user on mobile devices ("text" | "search" | "none" | "tel" | "url" | "email" | "numeric" | "decimal")  input_mode: Var[LiteralInputNumberMode]  Whether the input should be disabled.
-            is_invalid: If true, the input will have `aria-invalid` set to true
-            is_read_only: If true, the input will be in readonly mode
-            is_required: Whether the input is required
-            is_valid_character: Whether the pressed key should be allowed in the input. The default behavior is to allow DOM floating point characters defined by /^[Ee0-9+\\-.]$/
-            keep_within_range: This controls the value update behavior in general. - If true and you use the stepper or up/down arrow keys, the value will not exceed the max or go lower than min - If false, the value will be allowed to go out of range.
-            max_: The maximum value of the counter
-            min_: The minimum value of the counter
-            variant: "outline" | "filled" | "flushed" | "unstyled"
-            size: "lg" | "md" | "sm" | "xs"
-            name: The name of the form field
+            *children: Child components.
+            default_value: The value of the tab that should be active when initially rendered. Use when you do not need to control the state of the tabs.
+            value: The controlled value of the tab that should be active. Use when you need to control the state of the tabs.
+            orientation: The orientation of the tabs.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
+            A new component instance.
         """
         ...
 
-class NumberInputField(ChakraComponent):
+class TabsList(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        size: Optional[Union[Var[Literal["1", "2"]], Literal["1", "2"]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -197,41 +162,44 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "NumberInputField":
-        """Create the component.
+    ) -> "TabsList":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
+            *children: Child components.
+            size: Tabs size "1" - "2"
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
+            A new component instance.
         """
         ...
 
-class NumberInputStepper(ChakraComponent):
+class TabsTrigger(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        value: Optional[Union[Var[str], str]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -276,41 +244,44 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "NumberInputStepper":
-        """Create the component.
+    ) -> "TabsTrigger":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
+            *children: Child components.
+            value: The value of the tab. Must be unique for each tab.
+            disabled: Whether the tab is disabled
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
+            A new component instance.
         """
         ...
 
-class NumberIncrementStepper(ChakraComponent):
+class TabsContent(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        value: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -355,50 +326,65 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "NumberIncrementStepper":
-        """Create the component.
+    ) -> "TabsContent":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
+            *children: Child components.
+            value: The value of the tab. Must be unique for each tab.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
+            A new component instance.
         """
         ...
 
-class NumberDecrementStepper(ChakraComponent):
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
+class Tabs(ComponentNamespace):
+    root = staticmethod(TabsRoot.create)
+    list = staticmethod(TabsList.create)
+    trigger = staticmethod(TabsTrigger.create)
+    content = staticmethod(TabsContent.create)
+
+    @staticmethod
+    def __call__(
         *children,
+        default_value: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        orientation: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -434,27 +420,32 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "NumberDecrementStepper":
-        """Create the component.
+    ) -> "TabsRoot":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
+            *children: Child components.
+            default_value: The value of the tab that should be active when initially rendered. Use when you do not need to control the state of the tabs.
+            value: The controlled value of the tab that should be active. Use when you need to control the state of the tabs.
+            orientation: The orientation of the tabs.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
+            A new component instance.
         """
         ...
+
+tabs = Tabs()
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/password.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/password.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/pininput.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/pininput.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class PinInput(ChakraComponent):
     """The component that provides context to all the pin-input fields."""
 
     tag = "PinInput"
 
-    # State var to bind the the input.
+    # State var to bind the input.
     value: Var[str]
 
     # If true, the pin input receives focus on mount
     auto_focus: Var[bool]
 
     # The default value of the pin input
     default_value: Var[str]
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/pininput.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/pininput.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         """Create a pin input component.
 
         If no children are passed in, the component will create a default pin input
         based on the length prop.
 
         Args:
             *children: The children of the component.
-            value: State var to bind the the input.
+            value: State var to bind the input.
             auto_focus: If true, the pin input receives focus on mount
             default_value: The default value of the pin input
             error_border_color: The border color when the input is invalid.
             focus_border_color: The border color when the input is focused.
             id_: The top-level id string that will be applied to the input fields. The index of the input will be appended to this top-level id.
             length: The length of the number input.
             is_disabled: If true, the pin input component is put in the disabled state
@@ -214,12 +214,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/radio.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/radio.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class RadioGroup(ChakraComponent):
     """A grouping of individual radio options."""
 
     tag = "RadioGroup"
 
-    # State var to bind the the input.
+    # State var to bind the input.
     value: Var[Any]
 
     # The default value.
     default_value: Var[Any]
 
     # The name of the form field
     name: Var[str]
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/radio.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/radio.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         ] = None,
         **props
     ) -> "RadioGroup":
         """Create a radio group component.
 
         Args:
             *children: The children of the component.
-            value: State var to bind the the input.
+            value: State var to bind the input.
             default_value: The default value.
             name: The name of the form field
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/rangeslider.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class RangeSlider(ChakraComponent):
     """The RangeSlider is a multi thumb slider used to select a range of related values. A common use-case of this component is a price range picker that allows a user to set the minimum and maximum price."""
 
     tag = "RangeSlider"
 
-    # State var to bind the the input.
+    # State var to bind the input.
     value: Var[List[int]]
 
     # The default values.
     default_value: Var[List[int]]
 
     # The writing mode ("ltr" | "rtl")
     direction: Var[LiteralChakraDirection]
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/rangeslider.pyi` & `reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,40 @@
-"""Stub file for reflex/components/chakra/forms/rangeslider.py"""
+"""Stub file for reflex/components/chakra/navigation/breadcrumb.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, List, Optional, Union
-from reflex.components.chakra import ChakraComponent, LiteralChakraDirection
+from reflex.components.chakra import ChakraComponent
+from reflex.components.chakra.navigation.link import Link
 from reflex.components.component import Component
-from reflex.constants import EventTriggers
-from reflex.utils import format
+from reflex.components.core.foreach import Foreach
 from reflex.vars import Var
 
-class RangeSlider(ChakraComponent):
-    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
-    def get_ref(self): ...
+class Breadcrumb(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        value: Optional[Union[Var[List[int]], List[int]]] = None,
-        default_value: Optional[Union[Var[List[int]], List[int]]] = None,
-        direction: Optional[
-            Union[Var[Literal["ltr", "rtl"]], Literal["ltr", "rtl"]]
-        ] = None,
-        focus_thumb_on_change: Optional[Union[Var[bool], bool]] = None,
-        is_disabled: Optional[Union[Var[bool], bool]] = None,
-        is_read_only: Optional[Union[Var[bool], bool]] = None,
-        is_reversed: Optional[Union[Var[bool], bool]] = None,
-        min_: Optional[Union[Var[int], int]] = None,
-        max_: Optional[Union[Var[int], int]] = None,
-        min_steps_between_thumbs: Optional[Union[Var[int], int]] = None,
-        name: Optional[Union[Var[str], str]] = None,
+        items=None,
+        separator: Optional[Union[Var[str], str]] = None,
+        separator_margin: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_change_end: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_change_start: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -92,51 +70,49 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "RangeSlider":
-        """Create a RangeSlider component.
+    ) -> "Breadcrumb":
+        """Create a breadcrumb component.
 
-        If no children are provided, a default RangeSlider will be created.
+        If the kw-args `items` is provided and is a list, they will be added as children.
 
         Args:
             *children: The children of the component.
-            value: State var to bind the the input.
-            default_value: The default values.
-            direction: The writing mode ("ltr" | "rtl")
-            focus_thumb_on_change: If false, the slider handle will not capture focus when value changes.
-            is_disabled: If true, the slider will be disabled
-            is_read_only: If true, the slider will be in `read-only` state.
-            is_reversed: If true, the value will be incremented or decremented in reverse.
-            min_: The minimum value of the slider.
-            max_: The maximum value of the slider.
-            min_steps_between_thumbs: The minimum distance between slider thumbs. Useful for preventing the thumbs from being too close together.
-            name: The name of the form field
+            items (list): The items of the breadcrumb: (label, link)
+            separator: The visual separator between each breadcrumb item
+            separator_margin: The left and right margin applied to the separator
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The properties of the component.
 
         Returns:
-            The RangeSlider component.
+            The breadcrumb component.
         """
         ...
 
-class RangeSliderTrack(ChakraComponent):
+class BreadcrumbItem(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        label=None,
+        href=None,
+        is_current_page: Optional[Union[Var[bool], bool]] = None,
+        is_last_child: Optional[Union[Var[bool], bool]] = None,
+        separator: Optional[Union[Var[str], str]] = None,
+        spacing: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -181,36 +157,39 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "RangeSliderTrack":
-        """Create the component.
+    ) -> "BreadcrumbItem":
+        """Create a Breadcrumb Item component.
 
         Args:
             *children: The children of the component.
+            label: The label used in the link. Defaults to None.
+            href: The URL of the link. Defaults to None.
+            is_current_page: Is the current page of the breadcrumb.
+            is_last_child: Is the last child of the breadcrumb.
+            separator: The visual separator between each breadcrumb item
+            spacing: The left and right margin applied to the separator
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: The properties of the component.
 
         Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
+            The BreadcrumbItem component
         """
         ...
 
-class RangeSliderFilledTrack(ChakraComponent):
+class BreadcrumbSeparator(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -260,43 +239,44 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "RangeSliderFilledTrack":
+    ) -> "BreadcrumbSeparator":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class RangeSliderThumb(ChakraComponent):
-    def get_ref(self): ...
+class BreadcrumbLink(Link):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        index: Optional[Union[Var[int], int]] = None,
+        is_current_page: Optional[Union[Var[bool], bool]] = None,
+        rel: Optional[Union[Var[str], str]] = None,
+        href: Optional[Union[Var[str], str]] = None,
+        text: Optional[Union[Var[str], str]] = None,
+        as_: Optional[Union[Var[str], str]] = None,
+        is_external: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -341,28 +321,33 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "RangeSliderThumb":
-        """Create the component.
+    ) -> "BreadcrumbLink":
+        """Create a Link component.
 
         Args:
             *children: The children of the component.
-            index: The position of the thumb.
+            is_current_page: Is the current page of the breadcrumb.
+            rel: The rel.
+            href: The page to link to.
+            text: The text to display.
+            as_: What the link renders to.
+            is_external: If true, the link will open in new tab.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
-        Returns:
-            The component.
-
         Raises:
-            TypeError: If an invalid child is passed.
+            ValueError: in case of missing children
+
+        Returns:
+            Component: The link component
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/select.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/select.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/slider.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/slider.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/slider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -215,17 +215,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class SliderFilledTrack(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -294,17 +291,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class SliderThumb(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -375,17 +369,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class SliderMark(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -454,12 +445,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/switch.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/switch.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/switch.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -154,12 +154,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/textarea.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/textarea.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/textarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/forms/time_picker.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/aspect_ratio.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/aspect_ratio.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -81,12 +81,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/box.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/box.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/box.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -86,12 +86,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/card.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/card.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/editable.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,63 @@
-"""Stub file for reflex/components/chakra/layout/card.py"""
+"""Stub file for reflex/components/chakra/forms/editable.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional
-from reflex.components.chakra import (
-    ChakraComponent,
-    LiteralCardVariant,
-    LiteralColorScheme,
-    LiteralTagSize,
-)
-from reflex.components.component import Component
+from typing import Any, Union
+from reflex.components.chakra import ChakraComponent
+from reflex.constants import EventTriggers
 from reflex.vars import Var
 
-class CardHeader(ChakraComponent):
+class Editable(ChakraComponent):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        is_disabled: Optional[Union[Var[bool], bool]] = None,
+        is_preview_focusable: Optional[Union[Var[bool], bool]] = None,
+        placeholder: Optional[Union[Var[str], str]] = None,
+        select_all_on_focus: Optional[Union[Var[bool], bool]] = None,
+        start_with_edit_view: Optional[Union[Var[bool], bool]] = None,
+        submit_on_blur: Optional[Union[Var[bool], bool]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_cancel: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_edit: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
@@ -67,40 +80,48 @@
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_submit: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "CardHeader":
+    ) -> "Editable":
         """Create the component.
 
         Args:
             *children: The children of the component.
+            is_disabled: If true, the Editable will be disabled.
+            is_preview_focusable: If true, the read only view, has a tabIndex set to 0 so it can receive focus via the keyboard or click.
+            placeholder: The placeholder text when the value is empty.
+            select_all_on_focus: If true, the input's text will be highlighted on focus.
+            start_with_edit_view: If true, the Editable will start with edit mode by default.
+            submit_on_blur: If true, it'll update the value onBlur and turn off the edit mode.
+            value: The value of the Editable in both edit & preview mode
+            default_value: The initial value of the Editable in both edit and preview mode.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class CardBody(ChakraComponent):
+class EditableInput(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -150,36 +171,33 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "CardBody":
+    ) -> "EditableInput":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class CardFooter(ChakraComponent):
+class EditableTextarea(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -229,103 +247,38 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "CardFooter":
+    ) -> "EditableTextarea":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class Card(ChakraComponent):
+class EditablePreview(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        header: Optional[Component] = None,
-        footer: Optional[Component] = None,
-        align: Optional[Union[Var[str], str]] = None,
-        direction: Optional[Union[Var[str], str]] = None,
-        justify: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "none",
-                        "gray",
-                        "red",
-                        "orange",
-                        "yellow",
-                        "green",
-                        "teal",
-                        "blue",
-                        "cyan",
-                        "purple",
-                        "pink",
-                        "whiteAlpha",
-                        "blackAlpha",
-                        "linkedin",
-                        "facebook",
-                        "messenger",
-                        "whatsapp",
-                        "twitter",
-                        "telegram",
-                    ]
-                ],
-                Literal[
-                    "none",
-                    "gray",
-                    "red",
-                    "orange",
-                    "yellow",
-                    "green",
-                    "teal",
-                    "blue",
-                    "cyan",
-                    "purple",
-                    "pink",
-                    "whiteAlpha",
-                    "blackAlpha",
-                    "linkedin",
-                    "facebook",
-                    "messenger",
-                    "whatsapp",
-                    "twitter",
-                    "telegram",
-                ],
-            ]
-        ] = None,
-        size: Optional[
-            Union[Var[Literal["sm", "md", "lg"]], Literal["sm", "md", "lg"]]
-        ] = None,
-        variant: Optional[
-            Union[
-                Var[Literal["outline", "filled", "elevated", "unstyled"]],
-                Literal["outline", "filled", "elevated", "unstyled"],
-            ]
-        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -370,23 +323,24 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Card":
-        """Creates a Chakra Card with a body and optionally header and/or footer, and returns it.
-        If header, body or footer are not already instances of Chead, Cbody or Cfoot respectively,
-        they will be wrapped as such for layout purposes. If you want to modify their props,
-        e.g. padding_left, you should wrap them yourself.
+    ) -> "EditablePreview":
+        """Create the component.
 
         Args:
-            body (Component): The main content of the Card that will be created.
-            header (Optional[Component]): The header of the Card.
-            footer (Optional[Component]): The footer of the Card.
-            props: The properties to be passed to the component.
+            *children: The children of the component.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
 
         Returns:
-            The `create()` method returns a Card object.
+            The component.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/center.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/center.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Square(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -157,17 +154,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Circle(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -236,12 +230,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/container.pyi` & `reflex-0.4.8a1/reflex/components/chakra/typography/highlight.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-"""Stub file for reflex/components/chakra/layout/container.py"""
+"""Stub file for reflex/components/chakra/typography/highlight.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
+from typing import Dict, List
 from reflex.components.chakra import ChakraComponent
+from reflex.components.tags import Tag
 from reflex.vars import Var
 
-class Container(ChakraComponent):
+class Highlight(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        center_content: Optional[Union[Var[bool], bool]] = None,
+        query: Optional[Union[Var[List[str]], List[str]]] = None,
+        styles: Optional[Union[Var[Dict], Dict]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -65,28 +68,26 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Container":
+    ) -> "Highlight":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            center_content: If true, container will center its children regardless of their width.
+            query: A query for the text to highlight. Can be a string or a list of strings.
+            styles: The style of the content.  Note: styles and style are different prop.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/flex.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/flex.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/flex.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,12 +96,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/grid.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/grid.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/grid.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class GridItem(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -187,17 +184,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ResponsiveGrid(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -292,12 +286,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/spacer.pyi` & `reflex-0.4.8a1/reflex/components/chakra/typography/span.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-"""Stub file for reflex/components/chakra/layout/spacer.py"""
+"""Stub file for reflex/components/chakra/typography/span.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from reflex.components.chakra import ChakraComponent
+from reflex.vars import Var
 
-class Spacer(ChakraComponent):
+class Span(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        as_: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -63,27 +65,25 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Spacer":
+    ) -> "Span":
         """Create the component.
 
         Args:
             *children: The children of the component.
+            as_: Override the tag. The default tag is `<span>`.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/stack.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/stack.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/stack.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Hstack(Stack):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -201,17 +198,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Vstack(Stack):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -301,12 +295,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/wrap.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/layout/wrap.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/wrap.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -172,12 +172,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/media/avatar.py` & `reflex-0.4.8a1/reflex/components/chakra/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/media/avatar.pyi` & `reflex-0.4.8a1/reflex/components/chakra/media/avatar.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -105,17 +105,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AvatarBadge(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -184,17 +181,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AvatarGroup(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -267,12 +261,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/media/icon.py` & `reflex-0.4.8a1/reflex/components/chakra/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/media/icon.pyi` & `reflex-0.4.8a1/reflex/components/chakra/media/icon.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Icon(ChakraIconComponent):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/media/image.py` & `reflex-0.4.8a1/reflex/components/chakra/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/media/image.pyi` & `reflex-0.4.8a1/reflex/components/chakra/media/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/navigation/breadcrumb.py` & `reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/navigation/breadcrumb.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/slider.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-"""Stub file for reflex/components/chakra/navigation/breadcrumb.py"""
+"""Stub file for reflex/components/radix/primitives/slider.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex.components.chakra import ChakraComponent
-from reflex.components.chakra.navigation.link import Link
-from reflex.components.component import Component
-from reflex.components.core.foreach import Foreach
+from typing import Any, Dict, List, Literal
+from reflex.components.component import Component, ComponentNamespace
+from reflex.components.radix.primitives.base import RadixPrimitiveComponentWithClassName
+from reflex.style import Style
 from reflex.vars import Var
 
-class Breadcrumb(ChakraComponent):
+LiteralSliderOrientation = Literal["horizontal", "vertical"]
+LiteralSliderDir = Literal["ltr", "rtl"]
+
+class SliderComponent(RadixPrimitiveComponentWithClassName):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        items=None,
-        separator: Optional[Union[Var[str], str]] = None,
-        separator_margin: Optional[Union[Var[str], str]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -70,49 +71,57 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Breadcrumb":
-        """Create a breadcrumb component.
-
-        If the kw-args `items` is provided and is a list, they will be added as children.
+    ) -> "SliderComponent":
+        """Create the component.
 
         Args:
             *children: The children of the component.
-            items (list): The items of the breadcrumb: (label, link)
-            separator: The visual separator between each breadcrumb item
-            separator_margin: The left and right margin applied to the separator
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The properties of the component.
+            **props: The props of the component.
 
         Returns:
-            The breadcrumb component.
+            The component.
         """
         ...
 
-class BreadcrumbItem(ChakraComponent):
+class SliderRoot(SliderComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        label=None,
-        href=None,
-        is_current_page: Optional[Union[Var[bool], bool]] = None,
-        is_last_child: Optional[Union[Var[bool], bool]] = None,
-        separator: Optional[Union[Var[str], str]] = None,
-        spacing: Optional[Union[Var[str], str]] = None,
+        default_value: Optional[Union[Var[List[int]], List[int]]] = None,
+        value: Optional[Union[Var[List[int]], List[int]]] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        orientation: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
+        dir: Optional[Union[Var[Literal["ltr", "rtl"]], Literal["ltr", "rtl"]]] = None,
+        inverted: Optional[Union[Var[bool], bool]] = None,
+        min: Optional[Union[Var[int], int]] = None,
+        max: Optional[Union[Var[int], int]] = None,
+        step: Optional[Union[Var[int], int]] = None,
+        min_steps_between_thumbs: Optional[Union[Var[int], int]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -156,45 +165,47 @@
         ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_value_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_value_commit: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         **props
-    ) -> "BreadcrumbItem":
-        """Create a Breadcrumb Item component.
+    ) -> "SliderRoot":
+        """Create the component.
 
         Args:
             *children: The children of the component.
-            label: The label used in the link. Defaults to None.
-            href: The URL of the link. Defaults to None.
-            is_current_page: Is the current page of the breadcrumb.
-            is_last_child: Is the last child of the breadcrumb.
-            separator: The visual separator between each breadcrumb item
-            spacing: The left and right margin applied to the separator
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The properties of the component.
+            **props: The props of the component.
 
         Returns:
-            The BreadcrumbItem component
+            The component.
         """
         ...
 
-class BreadcrumbSeparator(ChakraComponent):
+class SliderTrack(SliderComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -239,47 +250,40 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "BreadcrumbSeparator":
+    ) -> "SliderTrack":
         """Create the component.
 
         Args:
             *children: The children of the component.
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class BreadcrumbLink(Link):
+class SliderRange(SliderComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        is_current_page: Optional[Union[Var[bool], bool]] = None,
-        rel: Optional[Union[Var[str], str]] = None,
-        href: Optional[Union[Var[str], str]] = None,
-        text: Optional[Union[Var[str], str]] = None,
-        as_: Optional[Union[Var[str], str]] = None,
-        is_external: Optional[Union[Var[bool], bool]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -324,33 +328,114 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "BreadcrumbLink":
-        """Create a Link component.
+    ) -> "SliderRange":
+        """Create the component.
 
         Args:
             *children: The children of the component.
-            is_current_page: Is the current page of the breadcrumb.
-            rel: The rel.
-            href: The page to link to.
-            text: The text to display.
-            as_: What the link renders to.
-            is_external: If true, the link will open in new tab.
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
-        Raises:
-            ValueError: in case of missing children
+        Returns:
+            The component.
+        """
+        ...
+
+class SliderThumb(SliderComponent):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "SliderThumb":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            as_child: Change the default rendered element for the one passed as a child.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
 
         Returns:
-            Component: The link component
+            The component.
         """
         ...
+
+class Slider(ComponentNamespace):
+    root = staticmethod(SliderRoot.create)
+    track = staticmethod(SliderTrack.create)
+    range = staticmethod(SliderRange.create)
+    thumb = staticmethod(SliderThumb.create)
+
+    @staticmethod
+    def __call__(**props) -> Component: ...
+
+slider = Slider()
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/navigation/link.py` & `reflex-0.4.8a1/reflex/components/chakra/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/navigation/link.pyi` & `reflex-0.4.8a1/reflex/components/chakra/navigation/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/navigation/linkoverlay.py` & `reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/navigation/linkoverlay.pyi` & `reflex-0.4.8a1/reflex/components/core/client_side_routing.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-"""Stub file for reflex/components/chakra/navigation/linkoverlay.py"""
+"""Stub file for reflex/components/core/client_side_routing.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex.components.chakra import ChakraComponent
+from reflex import constants
+from reflex.components.component import Component
+from reflex.components.core.cond import cond
 from reflex.vars import Var
 
-class LinkOverlay(ChakraComponent):
+route_not_found: Var
+
+class ClientSideRouting(Component):
+    def render(self) -> str: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        is_external: Optional[Union[Var[bool], bool]] = None,
-        href: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -66,43 +69,41 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "LinkOverlay":
+    ) -> "ClientSideRouting":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            is_external: If true, the link will open in new tab
-            href: Href of the link overlay.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class LinkBox(ChakraComponent):
+def wait_for_client_redirect(component) -> Component: ...
+
+class Default404Page(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        status_code: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -147,27 +148,24 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "LinkBox":
+    ) -> "Default404Page":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/navigation/stepper.py` & `reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/navigation/stepper.pyi` & `reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -220,17 +220,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StepDescription(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -299,17 +296,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StepIcon(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -378,17 +372,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StepIndicator(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -457,17 +448,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StepNumber(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -536,17 +524,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StepSeparator(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -615,17 +600,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StepStatus(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -698,17 +680,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StepTitle(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -777,12 +756,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/__init__.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/alertdialog.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/alertdialog.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -228,17 +228,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AlertDialogHeader(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -307,17 +304,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AlertDialogFooter(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -386,17 +380,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AlertDialogContent(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -465,17 +456,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AlertDialogOverlay(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -544,17 +532,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AlertDialogCloseButton(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -623,12 +608,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/drawer.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/drawer.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -270,17 +270,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DrawerHeader(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -349,17 +346,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DrawerFooter(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -428,17 +422,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DrawerOverlay(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -507,17 +498,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DrawerContent(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -586,17 +574,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DrawerCloseButton(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -665,12 +650,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/menu.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/menu.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/menu.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -214,17 +214,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class MenuList(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -381,17 +378,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class MenuItemOption(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -478,17 +472,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class MenuGroup(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -557,17 +548,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class MenuOptionGroup(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -642,17 +630,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class MenuDivider(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -721,12 +706,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/modal.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/modal.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/modal.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -215,17 +215,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ModalHeader(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -294,17 +291,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ModalFooter(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -373,17 +367,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ModalContent(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -452,17 +443,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ModalBody(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -531,17 +519,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ModalCloseButton(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -610,12 +595,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/popover.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/popover.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/popover.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -223,17 +223,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PopoverHeader(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -302,17 +299,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PopoverFooter(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -381,17 +375,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PopoverBody(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -460,17 +451,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PopoverArrow(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -539,17 +527,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PopoverCloseButton(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -618,17 +603,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PopoverAnchor(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -697,17 +679,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PopoverTrigger(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -776,12 +755,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/tooltip.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/overlay/tooltip.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -123,12 +123,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/typography/heading.pyi` & `reflex-0.4.8a1/reflex/components/chakra/typography/heading.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -88,12 +88,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/typography/highlight.py` & `reflex-0.4.8a1/reflex/components/chakra/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/chakra/typography/highlight.pyi` & `reflex-0.4.8a1/reflex/components/core/debounce.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,48 @@
-"""Stub file for reflex/components/chakra/typography/highlight.py"""
+"""Stub file for reflex/components/core/debounce.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Dict, List
-from reflex.components.chakra import ChakraComponent
-from reflex.components.tags import Tag
-from reflex.vars import Var
+from typing import Any, Type
+from reflex.components.component import Component
+from reflex.constants import EventTriggers
+from reflex.vars import Var, VarData
 
-class Highlight(ChakraComponent):
+DEFAULT_DEBOUNCE_TIMEOUT = 300
+
+class DebounceInput(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        query: Optional[Union[Var[List[str]], List[str]]] = None,
-        styles: Optional[Union[Var[Dict], Dict]] = None,
+        min_length: Optional[Union[Var[int], int]] = None,
+        debounce_timeout: Optional[Union[Var[int], int]] = None,
+        force_notify_by_enter: Optional[Union[Var[bool], bool]] = None,
+        force_notify_on_blur: Optional[Union[Var[bool], bool]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        input_ref: Optional[Union[Var[str], str]] = None,
+        element: Optional[Union[Var[Type[Component]], Type[Component]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -68,29 +78,29 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Highlight":
-        """Create the component.
+    ) -> "DebounceInput":
+        """Create a DebounceInput component.
+
+        Carry first child props directly on this tag.
+
+        Since react-debounce-input wants to create and manage the underlying
+        input component itself, we carry all props, events, and styles from
+        the child, and then neuter the child's render method so it produces no output.
 
         Args:
-            *children: The children of the component.
-            query: A query for the text to highlight. Can be a string or a list of strings.
-            styles: The style of the content.  Note: styles and style are different prop.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
+            children: The child component to wrap.
+            props: The component props.
 
         Returns:
-            The component.
+            The DebounceInput component.
 
         Raises:
-            TypeError: If an invalid child is passed.
+            RuntimeError: unless exactly one child element is provided.
+            ValueError: if the child element does not have an on_change handler.
         """
         ...
+    def get_event_triggers(self) -> dict[str, Any]: ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/typography/span.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/keyboard_key.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-"""Stub file for reflex/components/chakra/typography/span.py"""
+"""Stub file for reflex/components/chakra/datadisplay/keyboard_key.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from reflex.components.chakra import ChakraComponent
-from reflex.vars import Var
 
-class Span(ChakraComponent):
+class KeyboardKey(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -65,28 +63,24 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Span":
+    ) -> "KeyboardKey":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            as_: Override the tag. The default tag is `<span>`.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/chakra/typography/text.pyi` & `reflex-0.4.8a1/reflex/components/chakra/typography/text.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,12 +83,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/component.py` & `reflex-0.4.8a1/reflex/components/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 
     # The library that the component is based on.
     library: Optional[str] = None
 
     # List here the non-react dependency needed by `library`
     lib_dependencies: List[str] = []
 
+    # List here the dependencies that need to be transpiled by Next.js
+    transpile_packages: List[str] = []
+
     # The tag to use when rendering the component.
     tag: Optional[str] = None
 
     @abstractmethod
     def render(self) -> dict:
         """Render the component.
 
@@ -364,15 +367,15 @@
         value: Union[
             Var, EventHandler, EventSpec, List[Union[EventHandler, EventSpec]], Callable
         ],
     ) -> Union[EventChain, Var]:
         """Create an event chain from a variety of input types.
 
         Args:
-            args_spec: The args_spec of the the event trigger being bound.
+            args_spec: The args_spec of the event trigger being bound.
             value: The value to create the event chain from.
 
         Returns:
             The event chain.
 
         Raises:
             ValueError: If the value is not a valid event chain.
@@ -467,17 +470,19 @@
             EventTriggers.ON_MOUNT: lambda: [],
             EventTriggers.ON_UNMOUNT: lambda: [],
         }
         # Look for component specific triggers,
         # e.g. variable declared as EventHandler types.
         for field in self.get_fields().values():
             if types._issubclass(field.type_, EventHandler):
-                default_triggers[field.name] = getattr(
-                    field.type_, "args_spec", lambda: []
-                )
+                args_spec = None
+                annotation = field.annotation
+                if hasattr(annotation, "__metadata__"):
+                    args_spec = annotation.__metadata__[0]
+                default_triggers[field.name] = args_spec or (lambda: [])
         return default_triggers
 
     def __repr__(self) -> str:
         """Represent the component in React.
 
         Returns:
             The code to render the component.
@@ -610,20 +615,18 @@
 
         Args:
             *children: The children of the component.
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         # Import here to avoid circular imports.
         from reflex.components.base.bare import Bare
+        from reflex.components.base.fragment import Fragment
 
         # Translate deprecated props to new names.
         new_prop_names = [
             prop for prop in cls.get_props() if prop in ["type", "min", "max"]
         ]
         for prop in new_prop_names:
             under_prop = f"{prop}_"
@@ -636,28 +639,35 @@
                     dedupe=False,
                 )
                 props[prop] = props.pop(under_prop)
 
         # Filter out None props
         props = {key: value for key, value in props.items() if value is not None}
 
+        def validate_children(children):
+            for child in children:
+                if isinstance(child, tuple):
+                    validate_children(child)
+                # Make sure the child is a valid type.
+                if not types._isinstance(child, ComponentChild):
+                    raise TypeError(
+                        "Children of Reflex components must be other components, "
+                        "state vars, or primitive Python types. "
+                        f"Got child {child} of type {type(child)}.",
+                    )
+
         # Validate all the children.
-        for child in children:
-            # Make sure the child is a valid type.
-            if not types._isinstance(child, ComponentChild):
-                raise TypeError(
-                    "Children of Reflex components must be other components, "
-                    "state vars, or primitive Python types. "
-                    f"Got child {child} of type {type(child)}.",
-                )
+        validate_children(children)
 
         children = [
             (
                 child
                 if isinstance(child, Component)
+                else Fragment.create(*child)
+                if isinstance(child, tuple)
                 else Bare.create(contents=Var.create(child, _var_is_string=True))
             )
             for child in children
         ]
 
         return cls(children=children, **props)
 
@@ -983,22 +993,43 @@
         """
         return [
             getattr(self, prop)._get_all_imports()
             for prop in self.get_component_props()
             if getattr(self, prop) is not None
         ]
 
+    def _should_transpile(self, dep: str | None) -> bool:
+        """Check if a dependency should be transpiled.
+
+        Args:
+            dep: The dependency to check.
+
+        Returns:
+            True if the dependency should be transpiled.
+        """
+        return (
+            dep in self.transpile_packages
+            or format.format_library_name(dep or "") in self.transpile_packages
+        )
+
     def _get_dependencies_imports(self) -> imports.ImportDict:
         """Get the imports from lib_dependencies for installing.
 
         Returns:
             The dependencies imports of the component.
         """
         return {
-            dep: [ImportVar(tag=None, render=False)] for dep in self.lib_dependencies
+            dep: [
+                ImportVar(
+                    tag=None,
+                    render=False,
+                    transpile=self._should_transpile(dep),
+                )
+            ]
+            for dep in self.lib_dependencies
         }
 
     def _get_hooks_imports(self) -> imports.ImportDict:
         """Get the imports required by certain hooks.
 
         Returns:
             The imports required for all selected hooks.
@@ -1246,15 +1277,20 @@
 
         Returns:
             An import var.
         """
         # If the tag is dot-qualified, only import the left-most name.
         tag = self.tag.partition(".")[0] if self.tag else None
         alias = self.alias.partition(".")[0] if self.alias else None
-        return ImportVar(tag=tag, is_default=self.is_default, alias=alias)
+        return ImportVar(
+            tag=tag,
+            is_default=self.is_default,
+            alias=alias,
+            transpile=self._should_transpile(self.library),
+        )
 
     @staticmethod
     def _get_app_wrap_components() -> dict[tuple[int, str], Component]:
         """Get the app wrap components for the component.
 
         Returns:
             The app wrap components.
@@ -1510,33 +1546,36 @@
         dynamic_import = {"next/dynamic": [ImportVar(tag="dynamic", is_default=True)]}
 
         # The normal imports for this component.
         _imports = super()._get_imports()
 
         # Do NOT import the main library/tag statically.
         if self.library is not None:
-            _imports[self.library] = [imports.ImportVar(tag=None, render=False)]
+            _imports[self.library] = [
+                imports.ImportVar(
+                    tag=None,
+                    render=False,
+                    transpile=self._should_transpile(self.library),
+                ),
+            ]
 
         return imports.merge_imports(
             dynamic_import,
             _imports,
             self._get_dependencies_imports(),
         )
 
     def _get_dynamic_imports(self) -> str:
         opts_fragment = ", { ssr: false });"
 
         # extract the correct import name from library name
         if self.library is None:
             raise ValueError("Undefined library for NoSSRComponent")
 
-        import_name_parts = [p for p in self.library.rpartition("@") if p != ""]
-        import_name = (
-            import_name_parts[0] if import_name_parts[0] != "@" else self.library
-        )
+        import_name = format.format_library_name(self.library)
 
         library_import = f"const {self.alias if self.alias else self.tag} = dynamic(() => import('{import_name}')"
         mod_import = (
             # https://nextjs.org/docs/pages/building-your-application/optimizing/lazy-loading#with-named-exports
             f".then((mod) => mod.{self.tag})"
             if not self.is_default
             else ""
```

### Comparing `reflex-0.4.7a3/reflex/components/core/__init__.py` & `reflex-0.4.8a1/reflex/components/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/banner.py` & `reflex-0.4.8a1/reflex/components/core/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/banner.pyi` & `reflex-0.4.8a1/reflex/components/core/banner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/client_side_routing.py` & `reflex-0.4.8a1/reflex/components/core/client_side_routing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/client_side_routing.pyi` & `reflex-0.4.8a1/reflex/components/plotly/plotly.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-"""Stub file for reflex/components/core/client_side_routing.py"""
+"""Stub file for reflex/components/plotly/plotly.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex import constants
-from reflex.components.component import Component
-from reflex.components.core.cond import cond
+from typing import Any, Dict, List
+from reflex.components.component import NoSSRComponent
 from reflex.vars import Var
 
-route_not_found: Var
+try:
+    from plotly.graph_objects import Figure  # type: ignore
+except ImportError:
+    Figure = Any  # type: ignore
 
-class ClientSideRouting(Component):
-    def render(self) -> str: ...
+class PlotlyLib(NoSSRComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -69,44 +70,44 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ClientSideRouting":
+    ) -> "PlotlyLib":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-def wait_for_client_redirect(component) -> Component: ...
-
-class Default404Page(Component):
+class Plotly(PlotlyLib):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        status_code: Optional[Union[Var[int], int]] = None,
+        data: Optional[Union[Var[Figure], Figure]] = None,  # type: ignore
+        layout: Optional[Union[Var[Dict], Dict]] = None,
+        config: Optional[Union[Var[Dict], Dict]] = None,
+        width: Optional[Union[Var[str], str]] = None,
+        height: Optional[Union[Var[str], str]] = None,
+        use_resize_handler: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -151,27 +152,30 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Default404Page":
+    ) -> "Plotly":
         """Create the component.
 
         Args:
             *children: The children of the component.
+            data: The figure to display. This can be a plotly figure or a plotly data json.
+            layout: The layout of the graph.
+            config: The config of the graph.
+            width: The width of the graph.
+            height: The height of the graph.
+            use_resize_handler: If true, the graph will resize when the window is resized.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/core/colors.py` & `reflex-0.4.8a1/reflex/components/core/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/cond.py` & `reflex-0.4.8a1/reflex/components/core/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/debounce.py` & `reflex-0.4.8a1/reflex/components/core/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/debounce.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/aspect_ratio.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,36 @@
-"""Stub file for reflex/components/core/debounce.py"""
+"""Stub file for reflex/components/radix/themes/components/aspect_ratio.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Type
-from reflex.components.component import Component
-from reflex.constants import EventTriggers
-from reflex.vars import Var, VarData
+from typing import Union
+from reflex.vars import Var
+from ..base import RadixThemesComponent
 
-DEFAULT_DEBOUNCE_TIMEOUT = 300
-
-class DebounceInput(Component):
+class AspectRatio(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        min_length: Optional[Union[Var[int], int]] = None,
-        debounce_timeout: Optional[Union[Var[int], int]] = None,
-        force_notify_by_enter: Optional[Union[Var[bool], bool]] = None,
-        force_notify_on_blur: Optional[Union[Var[bool], bool]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        input_ref: Optional[Union[Var[str], str]] = None,
-        element: Optional[Union[Var[Type[Component]], Type[Component]]] = None,
+        ratio: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -78,29 +66,30 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DebounceInput":
-        """Create a DebounceInput component.
+    ) -> "AspectRatio":
+        """Create a new component instance.
 
-        Carry first child props directly on this tag.
-
-        Since react-debounce-input wants to create and manage the underlying
-        input component itself, we carry all props, events, and styles from
-        the child, and then neuter the child's render method so it produces no output.
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            children: The child component to wrap.
-            props: The component props.
+            *children: Child components.
+            ratio: The ratio of the width to the height of the element
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: Component properties.
 
         Returns:
-            The DebounceInput component.
-
-        Raises:
-            RuntimeError: unless exactly one child element is provided.
-            ValueError: if the child element does not have an on_change handler.
+            A new component instance.
         """
         ...
-    def get_event_triggers(self) -> dict[str, Any]: ...
+
+aspect_ratio = AspectRatio.create
```

### Comparing `reflex-0.4.7a3/reflex/components/core/foreach.py` & `reflex-0.4.8a1/reflex/components/core/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/html.py` & `reflex-0.4.8a1/reflex/components/core/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/html.pyi` & `reflex-0.4.8a1/reflex/components/core/html.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/match.py` & `reflex-0.4.8a1/reflex/components/core/match.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/responsive.py` & `reflex-0.4.8a1/reflex/components/core/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/core/upload.py` & `reflex-0.4.8a1/reflex/components/core/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,17 @@
         file_path: The path of the uploaded file.
 
     Returns:
         The URL of the uploaded file to be rendered from the frontend (as a str-encoded Var).
     """
     Upload.is_used = True
 
-    return Var.create_safe(f"{uploaded_files_url_prefix}/{file_path}")
+    return Var.create_safe(
+        f"{uploaded_files_url_prefix}/{file_path}", _var_is_string=True
+    )
 
 
 def _on_drop_spec(files: Var):
     """Args spec for the on_drop event trigger.
 
     Args:
         files: The files to upload.
```

### Comparing `reflex-0.4.7a3/reflex/components/core/upload.pyi` & `reflex-0.4.8a1/reflex/components/core/upload.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -111,17 +111,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Upload(MemoizationLeaf):
     is_used: ClassVar[bool] = False
 
     @overload
```

### Comparing `reflex-0.4.7a3/reflex/components/datadisplay/code.py` & `reflex-0.4.8a1/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/datadisplay/code.pyi` & `reflex-0.4.8a1/reflex/components/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/datadisplay/dataeditor.py` & `reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/datadisplay/dataeditor.pyi` & `reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/datadisplay/logo.py` & `reflex-0.4.8a1/reflex/components/datadisplay/logo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/constants/html.py` & `reflex-0.4.8a1/reflex/components/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/constants/react.py` & `reflex-0.4.8a1/reflex/components/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/constants/reflex.py` & `reflex-0.4.8a1/reflex/components/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/element.pyi` & `reflex-0.4.8a1/reflex/components/next/video.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-"""Stub file for reflex/components/el/element.py"""
+"""Stub file for reflex/components/next/video.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
+from typing import Optional
 from reflex.components.component import Component
+from reflex.vars import Var
+from .base import NextComponent
 
-class Element(Component):
+class Video(NextComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        src: Optional[Union[Var[str], str]] = None,
+        as_: Optional[Component] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -63,27 +68,25 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Element":
-        """Create the component.
+    ) -> "Video":
+        """Create a Video component.
 
         Args:
             *children: The children of the component.
+            src: the URL
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
+            The Video component.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/__init__.py` & `reflex-0.4.8a1/reflex/components/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/base.py` & `reflex-0.4.8a1/reflex/components/el/elements/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/base.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -136,12 +136,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/forms.py` & `reflex-0.4.8a1/reflex/components/el/elements/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/forms.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/forms.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -185,17 +185,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Datalist(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -320,17 +317,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Fieldset(Element):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -407,17 +401,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Form(BaseHTML):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
@@ -834,17 +825,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Label(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -975,17 +963,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Legend(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1110,17 +1095,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Meter(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1263,17 +1245,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Optgroup(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1406,17 +1385,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Option(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1557,17 +1533,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Output(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1700,17 +1673,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Progress(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1843,17 +1813,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Select(BaseHTML):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
@@ -2008,17 +1975,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 AUTO_HEIGHT_JS = '\nconst autoHeightOnInput = (e, is_enabled) => {\n    if (is_enabled) {\n        const el = e.target;\n        el.style.overflowY = "hidden";\n        el.style.height = "auto";\n        el.style.height = (e.target.scrollHeight) + "px";\n        if (el.form && !el.form.data_resize_on_reset) {\n            el.form.addEventListener("reset", () => window.setTimeout(() => autoHeightOnInput(e, is_enabled), 0))\n            el.form.data_resize_on_reset = true;\n        }\n    }\n}\n'
 ENTER_KEY_SUBMIT_JS = "\nconst enterKeySubmitOnKeyDown = (e, is_enabled) => {\n    if (is_enabled && e.which === 13 && !e.shiftKey) {\n        e.preventDefault();\n        if (!e.repeat) {\n            if (e.target.form) {\n                e.target.form.requestSubmit();\n            }\n        }\n    }\n}\n"
 
 class Textarea(BaseHTML):
@@ -2210,12 +2174,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/inline.py` & `reflex-0.4.8a1/reflex/components/el/elements/inline.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/inline.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/inline.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -166,17 +166,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Abbr(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -301,17 +298,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class B(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -436,17 +430,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Bdi(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -571,17 +562,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Bdo(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -706,17 +694,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Br(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -841,17 +826,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Cite(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -976,17 +958,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Code(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1111,17 +1090,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Data(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1250,17 +1226,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Dfn(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1385,17 +1358,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Em(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1520,17 +1490,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class I(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1655,17 +1622,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Kbd(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1790,17 +1754,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Mark(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1925,17 +1886,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Q(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2062,17 +2020,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Rp(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2197,17 +2152,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Rt(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2332,17 +2284,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Ruby(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2467,17 +2416,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class S(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2602,17 +2548,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Samp(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2737,17 +2680,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Small(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2872,17 +2812,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Span(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -3007,17 +2944,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Strong(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -3142,17 +3076,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Sub(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -3277,17 +3208,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Sup(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -3412,17 +3340,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Time(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -3551,17 +3476,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class U(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -3686,17 +3608,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Wbr(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -3821,12 +3740,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/media.py` & `reflex-0.4.8a1/reflex/components/el/elements/media.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/media.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/media.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -172,17 +172,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Audio(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -335,17 +332,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Img(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -514,17 +508,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Map(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -651,17 +642,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Track(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -802,17 +790,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Video(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -973,17 +958,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Embed(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1112,17 +1094,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Iframe(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1277,17 +1256,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Object(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1424,17 +1400,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Picture(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1559,17 +1532,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Portal(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1694,17 +1664,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Source(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1845,17 +1812,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Svg(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1980,17 +1944,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Path(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2117,12 +2078,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/metadata.py` & `reflex-0.4.8a1/reflex/components/el/elements/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/metadata.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/metadata.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Head(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -276,17 +273,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Link(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -432,17 +426,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Meta(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -577,17 +568,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Title(Element):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -656,12 +644,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/other.py` & `reflex-0.4.8a1/reflex/components/el/elements/other.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/other.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/other.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Dialog(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -275,17 +272,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Summary(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -410,17 +404,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Slot(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -545,17 +536,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Template(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -680,17 +668,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Math(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -815,17 +800,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Html(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -954,12 +936,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/scripts.py` & `reflex-0.4.8a1/reflex/components/el/elements/scripts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/scripts.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/scripts.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Noscript(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -271,17 +268,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Script(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -438,12 +432,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/sectioning.py` & `reflex-0.4.8a1/reflex/components/el/elements/sectioning.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/sectioning.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/sectioning.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -135,17 +135,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Address(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -270,17 +267,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Article(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -405,17 +399,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Aside(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -540,17 +531,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Footer(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -675,17 +663,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Header(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -810,17 +795,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class H1(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -945,17 +927,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class H2(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1080,17 +1059,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class H3(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1215,17 +1191,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class H4(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1350,17 +1323,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class H5(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1485,17 +1455,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class H6(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1620,17 +1587,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Main(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1755,17 +1719,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Nav(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1890,17 +1851,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Section(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2025,12 +1983,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/tables.py` & `reflex-0.4.8a1/reflex/components/el/elements/tables.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/tables.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/tables.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Col(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -281,17 +278,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Colgroup(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -422,17 +416,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Table(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -565,17 +556,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Tbody(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -704,17 +692,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Td(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -855,17 +840,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Tfoot(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -994,17 +976,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Th(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1149,17 +1128,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Thead(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1288,17 +1264,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Tr(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1427,12 +1400,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/typography.py` & `reflex-0.4.8a1/reflex/components/el/elements/typography.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/el/elements/typography.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/typography.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Dd(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -273,17 +270,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Div(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -408,17 +402,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Dl(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -543,17 +534,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Dt(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -678,17 +666,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Figcaption(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -813,17 +798,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Hr(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -952,17 +934,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Li(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1087,17 +1066,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Menu(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1224,17 +1200,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Ol(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1369,17 +1342,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class P(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1504,17 +1474,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Pre(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1639,17 +1606,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Ul(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1774,17 +1738,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Ins(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1915,17 +1876,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Del(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -2056,12 +2014,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/gridjs/datatable.py` & `reflex-0.4.8a1/reflex/components/gridjs/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/gridjs/datatable.pyi` & `reflex-0.4.8a1/reflex/components/gridjs/datatable.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DataTable(Gridjs):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.4.7a3/reflex/components/lucide/icon.py` & `reflex-0.4.8a1/reflex/components/lucide/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/lucide/icon.pyi` & `reflex-0.4.8a1/reflex/components/lucide/icon.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -81,17 +81,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Icon(LucideIconComponent):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.4.7a3/reflex/components/markdown/markdown.py` & `reflex-0.4.8a1/reflex/components/markdown/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/markdown/markdown.pyi` & `reflex-0.4.8a1/reflex/components/markdown/markdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/moment/moment.py` & `reflex-0.4.8a1/reflex/components/moment/moment.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/moment/moment.pyi` & `reflex-0.4.8a1/reflex/components/moment/moment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/next/base.pyi` & `reflex-0.4.8a1/reflex/components/el/element.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-"""Stub file for reflex/components/next/base.py"""
+"""Stub file for reflex/components/el/element.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from reflex.components.component import Component
 
-class NextComponent(Component):
-    ...
-
+class Element(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -65,27 +63,24 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "NextComponent":
+    ) -> "Element":
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/next/image.py` & `reflex-0.4.8a1/reflex/components/next/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/next/image.pyi` & `reflex-0.4.8a1/reflex/components/next/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/next/link.pyi` & `reflex-0.4.8a1/reflex/components/next/link.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,12 +83,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/next/video.py` & `reflex-0.4.8a1/reflex/components/next/video.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/next/video.pyi` & `reflex-0.4.8a1/reflex/components/base/body.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-"""Stub file for reflex/components/next/video.py"""
+"""Stub file for reflex/components/base/body.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional
 from reflex.components.component import Component
-from reflex.vars import Var
-from .base import NextComponent
 
-class Video(NextComponent):
+class Body(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        src: Optional[Union[Var[str], str]] = None,
-        as_: Optional[Component] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -68,25 +63,24 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Video":
-        """Create a Video component.
+    ) -> "Body":
+        """Create the component.
 
         Args:
             *children: The children of the component.
-            src: the URL
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
-            The Video component.
+            The component.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/plotly/plotly.py` & `reflex-0.4.8a1/reflex/components/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/plotly/plotly.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/base.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-"""Stub file for reflex/components/plotly/plotly.py"""
+"""Stub file for reflex/components/radix/primitives/base.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, List
-from reflex.components.component import NoSSRComponent
+from typing import List
+from reflex.components.component import Component
+from reflex.components.tags.tag import Tag
+from reflex.utils import format
 from reflex.vars import Var
 
-try:
-    from plotly.graph_objects import Figure  # type: ignore
-except ImportError:
-    Figure = Any  # type: ignore
-
-class PlotlyLib(NoSSRComponent):
+class RadixPrimitiveComponent(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -70,47 +68,40 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "PlotlyLib":
+    ) -> "RadixPrimitiveComponent":
         """Create the component.
 
         Args:
             *children: The children of the component.
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class Plotly(PlotlyLib):
+class RadixPrimitiveComponentWithClassName(RadixPrimitiveComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        data: Optional[Union[Var[Figure], Figure]] = None,  # type: ignore
-        layout: Optional[Union[Var[Dict], Dict]] = None,
-        config: Optional[Union[Var[Dict], Dict]] = None,
-        width: Optional[Union[Var[str], str]] = None,
-        height: Optional[Union[Var[str], str]] = None,
-        use_resize_handler: Optional[Union[Var[bool], bool]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -155,33 +146,25 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Plotly":
+    ) -> "RadixPrimitiveComponentWithClassName":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            data: The figure to display. This can be a plotly figure or a plotly data json.
-            layout: The layout of the graph.
-            config: The config of the graph.
-            width: The width of the graph.
-            height: The height of the graph.
-            use_resize_handler: If true, the graph will resize when the window is resized.
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/accordion.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/accordion.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/accordion.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AccordionRoot(AccordionComponent):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/base.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/base.pyi` & `reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-"""Stub file for reflex/components/radix/primitives/base.py"""
+"""Stub file for reflex/components/chakra/navigation/linkoverlay.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import List
-from reflex.components.component import Component
-from reflex.components.tags.tag import Tag
-from reflex.utils import format
+from reflex.components.chakra import ChakraComponent
 from reflex.vars import Var
 
-class RadixPrimitiveComponent(Component):
+class LinkOverlay(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
+        is_external: Optional[Union[Var[bool], bool]] = None,
+        href: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -68,43 +66,40 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "RadixPrimitiveComponent":
+    ) -> "LinkOverlay":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
+            is_external: If true, the link will open in new tab
+            href: Href of the link overlay.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class RadixPrimitiveComponentWithClassName(RadixPrimitiveComponent):
+class LinkBox(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -149,28 +144,24 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "RadixPrimitiveComponentWithClassName":
+    ) -> "LinkBox":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/drawer.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/drawer.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/drawer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 LiteralDirectionType = Literal["top", "bottom", "left", "right"]
 
 class DrawerRoot(DrawerComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
@@ -196,17 +193,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DrawerTrigger(DrawerComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -348,17 +342,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DrawerContent(DrawerComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
@@ -527,17 +518,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DrawerClose(DrawerTrigger):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -679,17 +667,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DrawerDescription(DrawerComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -760,17 +745,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Drawer(ComponentNamespace):
     root = staticmethod(DrawerRoot.create)
     trigger = staticmethod(DrawerTrigger.create)
     portal = staticmethod(DrawerPortal.create)
@@ -874,14 +856,11 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 drawer = Drawer()
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/form.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/form.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/form.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -86,17 +86,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FormRoot(FormComponent, HTMLForm):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
@@ -350,17 +347,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FormLabel(FormComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -431,17 +425,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FormControl(FormComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -642,17 +633,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FormValidityState(FormComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -723,17 +711,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FormSubmit(FormComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -804,17 +789,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Form(FormRoot):
     pass
 
     @overload
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/progress.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/progress.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/progress.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -87,17 +87,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ProgressRoot(ProgressComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -175,17 +172,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ProgressIndicator(ProgressComponent):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -323,17 +317,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Progress(ProgressRoot):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/slider.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/primitives/slider.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,71 @@
-"""Stub file for reflex/components/radix/primitives/slider.py"""
+"""Stub file for reflex/components/chakra/forms/numberinput.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, List, Literal
-from reflex.components.component import Component, ComponentNamespace
-from reflex.components.radix.primitives.base import RadixPrimitiveComponentWithClassName
-from reflex.style import Style
+from numbers import Number
+from typing import Any, Dict
+from reflex.components.chakra import (
+    ChakraComponent,
+    LiteralButtonSize,
+    LiteralInputVariant,
+)
+from reflex.components.component import Component
+from reflex.constants import EventTriggers
 from reflex.vars import Var
 
-LiteralSliderOrientation = Literal["horizontal", "vertical"]
-LiteralSliderDir = Literal["ltr", "rtl"]
-
-class SliderComponent(RadixPrimitiveComponentWithClassName):
+class NumberInput(ChakraComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
+        value: Optional[Union[Var[Number], Number]] = None,
+        allow_mouse_wheel: Optional[Union[Var[bool], bool]] = None,
+        clamped_value_on_blur: Optional[Union[Var[bool], bool]] = None,
+        default_value: Optional[Union[Var[Number], Number]] = None,
+        error_border_color: Optional[Union[Var[str], str]] = None,
+        focus_border_color: Optional[Union[Var[str], str]] = None,
+        focus_input_on_change: Optional[Union[Var[bool], bool]] = None,
+        is_disabled: Optional[Union[Var[bool], bool]] = None,
+        is_invalid: Optional[Union[Var[bool], bool]] = None,
+        is_read_only: Optional[Union[Var[bool], bool]] = None,
+        is_required: Optional[Union[Var[bool], bool]] = None,
+        is_valid_character: Optional[Union[Var[str], str]] = None,
+        keep_within_range: Optional[Union[Var[bool], bool]] = None,
+        max_: Optional[Union[Var[Number], Number]] = None,
+        min_: Optional[Union[Var[Number], Number]] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["outline", "filled", "flushed", "unstyled"]],
+                Literal["outline", "filled", "flushed", "unstyled"],
+            ]
+        ] = None,
+        size: Optional[
+            Union[Var[Literal["sm", "md", "lg", "xs"]], Literal["sm", "md", "lg", "xs"]]
+        ] = None,
+        name: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -71,60 +101,58 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SliderComponent":
-        """Create the component.
+    ) -> "NumberInput":
+        """Create a number input component.
+
+        If no children are provided, a default stepper will be used.
 
         Args:
             *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
+            value: State var to bind the input.
+            allow_mouse_wheel: If true, the input's value will change based on mouse wheel.
+            clamped_value_on_blur: This controls the value update when you blur out of the input. - If true and the value is greater than max, the value will be reset to max - Else, the value remains the same.
+            default_value: The initial value of the counter. Should be less than max and greater than min
+            error_border_color: The border color when the input is invalid.
+            focus_border_color: The border color when the input is focused.
+            focus_input_on_change: If true, the input will be focused as you increment or decrement the value with the stepper
+            is_disabled: Hints at the type of data that might be entered by the user. It also determines the type of keyboard shown to the user on mobile devices ("text" | "search" | "none" | "tel" | "url" | "email" | "numeric" | "decimal")  input_mode: Var[LiteralInputNumberMode]  Whether the input should be disabled.
+            is_invalid: If true, the input will have `aria-invalid` set to true
+            is_read_only: If true, the input will be in readonly mode
+            is_required: Whether the input is required
+            is_valid_character: Whether the pressed key should be allowed in the input. The default behavior is to allow DOM floating point characters defined by /^[Ee0-9+\\-.]$/
+            keep_within_range: This controls the value update behavior in general. - If true and you use the stepper or up/down arrow keys, the value will not exceed the max or go lower than min - If false, the value will be allowed to go out of range.
+            max_: The maximum value of the counter
+            min_: The minimum value of the counter
+            variant: "outline" | "filled" | "flushed" | "unstyled"
+            size: "lg" | "md" | "sm" | "xs"
+            name: The name of the form field
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class SliderRoot(SliderComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class NumberInputField(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        default_value: Optional[Union[Var[List[int]], List[int]]] = None,
-        value: Optional[Union[Var[List[int]], List[int]]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        orientation: Optional[
-            Union[
-                Var[Literal["horizontal", "vertical"]],
-                Literal["horizontal", "vertical"],
-            ]
-        ] = None,
-        dir: Optional[Union[Var[Literal["ltr", "rtl"]], Literal["ltr", "rtl"]]] = None,
-        inverted: Optional[Union[Var[bool], bool]] = None,
-        min: Optional[Union[Var[int], int]] = None,
-        max: Optional[Union[Var[int], int]] = None,
-        step: Optional[Union[Var[int], int]] = None,
-        min_steps_between_thumbs: Optional[Union[Var[int], int]] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -168,50 +196,39 @@
         ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_value_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_value_commit: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         **props
-    ) -> "SliderRoot":
+    ) -> "NumberInputField":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class SliderTrack(SliderComponent):
+class NumberInputStepper(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -256,43 +273,38 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SliderTrack":
+    ) -> "NumberInputStepper":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class SliderRange(SliderComponent):
+class NumberIncrementStepper(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -337,43 +349,38 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SliderRange":
+    ) -> "NumberIncrementStepper":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class SliderThumb(SliderComponent):
+class NumberDecrementStepper(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -418,39 +425,24 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SliderThumb":
+    ) -> "NumberDecrementStepper":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-
-class Slider(ComponentNamespace):
-    root = staticmethod(SliderRoot.create)
-    track = staticmethod(SliderTrack.create)
-    range = staticmethod(SliderRange.create)
-    thumb = staticmethod(SliderThumb.create)
-
-    @staticmethod
-    def __call__(**props) -> Component: ...
-
-slider = Slider()
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/base.py` & `reflex-0.4.8a1/reflex/components/radix/themes/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/base.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/base.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -169,17 +169,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class RadixThemesComponent(Component):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -655,15 +652,12 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 theme = Theme.create
 theme_panel = ThemePanel.create
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/color_mode.py` & `reflex-0.4.8a1/reflex/components/radix/themes/color_mode.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/color_mode.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/color_mode.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/__init__.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/alert_dialog.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/alert_dialog.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/alertdialog.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/aspect_ratio.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/badge.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-"""Stub file for reflex/components/radix/themes/components/aspect_ratio.py"""
+"""Stub file for reflex/components/chakra/datadisplay/badge.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Union
+from reflex.components.chakra import ChakraComponent, LiteralVariant
 from reflex.vars import Var
-from ..base import RadixThemesComponent
 
-class AspectRatio(RadixThemesComponent):
+class Badge(ChakraComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        ratio: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["solid", "subtle", "outline"]],
+                Literal["solid", "subtle", "outline"],
+            ]
+        ] = None,
+        color_scheme: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -66,30 +71,26 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "AspectRatio":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Badge":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            ratio: The ratio of the width to the height of the element
+            *children: The children of the component.
+            variant: Variant of the badge ("solid" | "subtle" | "outline")
+            color_scheme: The color of the badge
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
-
-aspect_ratio = AspectRatio.create
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/aspectratio.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/aspectratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/avatar.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/avatar.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/badge.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/badge.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/badge.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/button.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/button.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/callout.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/callout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/callout.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/callout.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/card.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/card.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/checkbox.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/checkbox.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/context_menu.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/context_menu.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/contextmenu.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/contextmenu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/dialog.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/dialog.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/dropdown_menu.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/dropdown_menu.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/dropdownmenu.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dropdownmenu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/hover_card.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/hover_card.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/hovercard.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/hovercard.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/icon_button.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/icon_button.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/iconbutton.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/inset.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/inset.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/inset.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/inset.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/popover.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/popover.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/radio_group.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/radio_group.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/radiogroup.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/radiogroup.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/scroll_area.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/scroll_area.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/scrollarea.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/scrollarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/select.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/select.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/separator.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/separator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/separator.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/separator.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/slider.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/slider.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/switch.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/switch.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/table.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/table.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/tabs.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/tabs.pyi` & `reflex-0.4.8a1/reflex/components/base/meta.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,36 @@
-"""Stub file for reflex/components/radix/themes/components/tabs.py"""
+"""Stub file for reflex/components/base/meta.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, List, Literal
-from reflex.components.component import ComponentNamespace
-from reflex.constants import EventTriggers
-from reflex.vars import Var
-from ..base import RadixThemesComponent
+from typing import Optional
+from reflex.components.base.bare import Bare
+from reflex.components.component import Component
 
-class TabsRoot(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class Title(Component):
+    def render(self) -> dict: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        default_value: Optional[Union[Var[str], str]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        orientation: Optional[
-            Union[
-                Var[Literal["horizontal", "vertical"]],
-                Literal["horizontal", "vertical"],
-            ]
-        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -79,45 +66,43 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TabsRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Title":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            default_value: The value of the tab that should be active when initially rendered. Use when you do not need to control the state of the tabs.
-            value: The controlled value of the tab that should be active. Use when you need to control the state of the tabs.
-            orientation: The orientation of the tabs.
+            *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class TabsList(RadixThemesComponent):
+class Meta(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        size: Optional[Union[Var[Literal["1", "2"]], Literal["1", "2"]]] = None,
+        char_set: Optional[str] = None,
+        content: Optional[str] = None,
+        name: Optional[str] = None,
+        property: Optional[str] = None,
+        http_equiv: Optional[str] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -162,44 +147,48 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TabsList":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Meta":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            size: Tabs size "1" - "2"
+            *children: The children of the component.
+            char_set: The description of character encoding.
+            content: The value of meta.
+            name: The name of metadata.
+            property: The type of metadata value.
+            http_equiv: The type of metadata value.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class TabsTrigger(RadixThemesComponent):
+class Description(Meta):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        value: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
+        name: Optional[str] = None,
+        char_set: Optional[str] = None,
+        content: Optional[str] = None,
+        property: Optional[str] = None,
+        http_equiv: Optional[str] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -244,44 +233,48 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TabsTrigger":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Description":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            value: The value of the tab. Must be unique for each tab.
-            disabled: Whether the tab is disabled
+            *children: The children of the component.
+            name: The name of metadata.
+            char_set: The description of character encoding.
+            content: The value of meta.
+            property: The type of metadata value.
+            http_equiv: The type of metadata value.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class TabsContent(RadixThemesComponent):
+class Image(Meta):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        value: Optional[Union[Var[str], str]] = None,
+        property: Optional[str] = None,
+        char_set: Optional[str] = None,
+        content: Optional[str] = None,
+        name: Optional[str] = None,
+        http_equiv: Optional[str] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -326,126 +319,29 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TabsContent":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Image":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            value: The value of the tab. Must be unique for each tab.
+            *children: The children of the component.
+            property: The type of metadata value.
+            char_set: The description of character encoding.
+            content: The value of meta.
+            name: The name of metadata.
+            http_equiv: The type of metadata value.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
-
-class Tabs(ComponentNamespace):
-    root = staticmethod(TabsRoot.create)
-    list = staticmethod(TabsList.create)
-    trigger = staticmethod(TabsTrigger.create)
-    content = staticmethod(TabsContent.create)
-
-    @staticmethod
-    def __call__(
-        *children,
-        default_value: Optional[Union[Var[str], str]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        orientation: Optional[
-            Union[
-                Var[Literal["horizontal", "vertical"]],
-                Literal["horizontal", "vertical"],
-            ]
-        ] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        **props
-    ) -> "TabsRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
-
-        Args:
-            *children: Child components.
-            default_value: The value of the tab that should be active when initially rendered. Use when you do not need to control the state of the tabs.
-            value: The controlled value of the tab that should be active. Use when you need to control the state of the tabs.
-            orientation: The orientation of the tabs.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: Component properties.
-
-        Returns:
-            A new component instance.
-        """
-        ...
-
-tabs = Tabs()
```

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/text_area.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/text_area.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/text_field.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/text_field.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/textfield.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/textfield.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/tooltip.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/components/tooltip.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/__init__.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/base.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/base.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/box.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/center.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/container.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/container.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/container.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/flex.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/flex.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/grid.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/grid.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/list.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/list.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/section.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/section.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/spacer.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/stack.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/layout/stack.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/blockquote.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/blockquote.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/code.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/code.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/em.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/em.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/heading.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/heading.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/kbd.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/kbd.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/link.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/link.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/quote.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/quote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/strong.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/strong.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/text.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/text.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/radix/themes/typography/text.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/react_player/audio.pyi` & `reflex-0.4.8a1/reflex/components/react_player/audio.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -98,12 +98,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/react_player/react_player.py` & `reflex-0.4.8a1/reflex/components/react_player/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/react_player/react_player.pyi` & `reflex-0.4.8a1/reflex/components/react_player/react_player.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -97,12 +97,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/react_player/video.pyi` & `reflex-0.4.8a1/reflex/components/react_player/video.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -98,12 +98,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/recharts/__init__.py` & `reflex-0.4.8a1/reflex/components/recharts/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/recharts/cartesian.py` & `reflex-0.4.8a1/reflex/components/recharts/cartesian.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/recharts/cartesian.pyi` & `reflex-0.4.8a1/reflex/components/recharts/cartesian.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class XAxis(Axis):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -263,17 +260,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class YAxis(Axis):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -386,17 +380,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ZAxis(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -514,17 +505,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Brush(Recharts):
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
@@ -574,17 +562,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Cartesian(Recharts):
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
@@ -640,17 +625,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Area(Cartesian):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -760,17 +742,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Bar(Cartesian):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -841,17 +820,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Line(Cartesian):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -961,17 +937,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Scatter(Cartesian):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1059,17 +1032,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Funnel(Cartesian):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1137,17 +1107,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ErrorBar(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1228,17 +1195,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Reference(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1324,17 +1288,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ReferenceLine(Reference):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1422,17 +1383,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ReferenceDot(Reference):
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
@@ -1492,17 +1450,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ReferenceArea(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1598,17 +1553,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Grid(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1685,17 +1637,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class CartesianGrid(Grid):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1782,17 +1731,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class CartesianAxis(Grid):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -1897,12 +1843,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/recharts/charts.py` & `reflex-0.4.8a1/reflex/components/recharts/charts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/recharts/charts.pyi` & `reflex-0.4.8a1/reflex/components/recharts/charts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/recharts/general.py` & `reflex-0.4.8a1/reflex/components/recharts/general.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/recharts/general.pyi` & `reflex-0.4.8a1/reflex/components/recharts/general.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -215,17 +215,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class GraphingTooltip(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -310,17 +307,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Label(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -442,17 +436,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class LabelList(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -576,12 +567,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/recharts/polar.py` & `reflex-0.4.8a1/reflex/components/recharts/polar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/recharts/polar.pyi` & `reflex-0.4.8a1/reflex/components/recharts/polar.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -93,17 +93,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Radar(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -199,17 +196,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class RadialBar(Recharts):
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
@@ -262,17 +256,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PolarAngleAxis(Recharts):
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
@@ -341,17 +332,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PolarGrid(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -436,17 +424,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class PolarRadiusAxis(Recharts):
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
@@ -554,12 +539,9 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
```

### Comparing `reflex-0.4.7a3/reflex/components/recharts/recharts.py` & `reflex-0.4.8a1/reflex/components/recharts/recharts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/recharts/recharts.pyi` & `reflex-0.4.8a1/reflex/components/recharts/recharts.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -79,17 +79,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class RechartsCharts(NoSSRComponent, MemoizationLeaf):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.4.7a3/reflex/components/suneditor/editor.py` & `reflex-0.4.8a1/reflex/components/suneditor/editor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/suneditor/editor.pyi` & `reflex-0.4.8a1/reflex/components/suneditor/editor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/tags/iter_tag.py` & `reflex-0.4.8a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/tags/tag.py` & `reflex-0.4.8a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/components/tags/tagless.py` & `reflex-0.4.8a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/config.py` & `reflex-0.4.8a1/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/config.pyi` & `reflex-0.4.8a1/reflex/config.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/constants/__init__.py` & `reflex-0.4.8a1/reflex/constants/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The constants package."""
 
 from .base import (
     COOKIES,
     ENV_MODE_ENV_VAR,
     IS_WINDOWS,
+    IS_WINDOWS_BUN_SUPPORTED_MACHINE,  # type: ignore
     LOCAL_STORAGE,
     POLLING_MAX_HTTP_BUFFER_SIZE,
     PYTEST_CURRENT_TEST,
     REFLEX_VAR_CLOSING_TAG,
     REFLEX_VAR_OPENING_TAG,
     RELOAD_CONFIG,
     SKIP_COMPILE_ENV_VAR,
@@ -82,14 +83,15 @@
     Fnm,
     REFLEX_VAR_CLOSING_TAG,
     REFLEX_VAR_OPENING_TAG,
     GitIgnore,
     Hooks,
     Imports,
     IS_WINDOWS,
+    IS_WINDOWS_BUN_SUPPORTED_MACHINE,
     LOCAL_STORAGE,
     LogLevel,
     MemoizationDisposition,
     MemoizationMode,
     Next,
     Node,
     NOCOMPILE_FILE,
```

### Comparing `reflex-0.4.7a3/reflex/constants/base.py` & `reflex-0.4.8a1/reflex/constants/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 from enum import Enum
 from importlib import metadata
 from types import SimpleNamespace
 
 from platformdirs import PlatformDirs
 
 IS_WINDOWS = platform.system() == "Windows"
+# https://github.com/oven-sh/bun/blob/main/src/cli/install.ps1
+IS_WINDOWS_BUN_SUPPORTED_MACHINE = IS_WINDOWS and platform.machine() in [
+    "AMD64",
+    "x86_64",
+]  # filter out 32 bit + ARM
 
 
 class Dirs(SimpleNamespace):
     """Various directories/paths used by Reflex."""
 
     # The frontend directories in a project.
     # The web folder where the NextJS app is compiled to.
```

### Comparing `reflex-0.4.7a3/reflex/constants/base.pyi` & `reflex-0.4.8a1/reflex/constants/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/constants/colors.py` & `reflex-0.4.8a1/reflex/constants/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/constants/compiler.py` & `reflex-0.4.8a1/reflex/constants/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     JS = ".js"
     # The extension for python files.
     PY = ".py"
     # The extension for css files.
     CSS = ".css"
     # The extension for zip files.
     ZIP = ".zip"
+    # The extension for executable files on Windows.
+    EXE = ".exe"
 
 
 class CompileVars(SimpleNamespace):
     """The variables used during compilation."""
 
     # The expected variable name where the rx.App is stored.
     APP = "app"
```

### Comparing `reflex-0.4.7a3/reflex/constants/config.py` & `reflex-0.4.8a1/reflex/constants/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/constants/custom_components.py` & `reflex-0.4.8a1/reflex/constants/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/constants/event.py` & `reflex-0.4.8a1/reflex/constants/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/constants/installer.py` & `reflex-0.4.8a1/reflex/constants/installer.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 
 
 # Bun config.
 class Bun(SimpleNamespace):
     """Bun constants."""
 
     # The Bun version.
-    VERSION = "1.0.13"
+    VERSION = "1.1.3"
     # Min Bun Version
     MIN_VERSION = "0.7.0"
     # The directory to store the bun.
     ROOT_PATH = os.path.join(Reflex.DIR, "bun")
     # Default bun path.
-    DEFAULT_PATH = os.path.join(ROOT_PATH, "bin", "bun")
+    DEFAULT_PATH = os.path.join(
+        ROOT_PATH, "bin", "bun" if not IS_WINDOWS else "bun.exe"
+    )
     # URL to bun install script.
     INSTALL_URL = "https://bun.sh/install"
 
 
 # FNM config.
 class Fnm(SimpleNamespace):
     """FNM constants."""
```

### Comparing `reflex-0.4.7a3/reflex/constants/route.py` & `reflex-0.4.8a1/reflex/constants/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/constants/style.py` & `reflex-0.4.8a1/reflex/constants/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/custom_components/custom_components.py` & `reflex-0.4.8a1/reflex/custom_components/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/event.py` & `reflex-0.4.8a1/reflex/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,28 @@
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Tuple,
     Union,
-    _GenericAlias,  # type: ignore
     get_type_hints,
 )
 
 from reflex import constants
 from reflex.base import Base
 from reflex.utils import console, format
 from reflex.utils.types import ArgsSpec
 from reflex.vars import BaseVar, Var
 
+try:
+    from typing import Annotated
+except ImportError:
+    from typing_extensions import Annotated
+
 
 class Event(Base):
     """An event that describes any state change in the app."""
 
     # The token to specify the client that the event is for.
     token: str
 
@@ -114,27 +118,24 @@
     class Config:
         """The Pydantic config."""
 
         # Needed to allow serialization of Callable.
         frozen = True
 
     @classmethod
-    def __class_getitem__(cls, args_spec: str) -> _GenericAlias:
+    def __class_getitem__(cls, args_spec: str) -> Annotated:
         """Get a typed EventHandler.
 
         Args:
             args_spec: The args_spec of the EventHandler.
 
         Returns:
             The EventHandler class item.
         """
-        gen = _GenericAlias(cls, Any)
-        # Cannot subclass special typing classes, so we need to set the args_spec dynamically as an attribute.
-        gen.args_spec = args_spec
-        return gen
+        return Annotated[cls, args_spec]
 
     @property
     def is_background(self) -> bool:
         """Whether the event handler is a background task.
 
         Returns:
             True if the event handler is marked as a background task.
```

### Comparing `reflex-0.4.7a3/reflex/experimental/hooks.py` & `reflex-0.4.8a1/reflex/experimental/hooks.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/middleware/hydrate_middleware.py` & `reflex-0.4.8a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/middleware/middleware.py` & `reflex-0.4.8a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/model.py` & `reflex-0.4.8a1/reflex/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 import alembic.config
 import alembic.operations.ops
 import alembic.runtime.environment
 import alembic.script
 import alembic.util
 import sqlalchemy
 import sqlalchemy.orm
-import sqlmodel
 
 from reflex import constants
 from reflex.base import Base
 from reflex.config import get_config
 from reflex.utils import console
+from reflex.utils.compat import sqlmodel
 
 
 def get_engine(url: str | None = None):
     """Get the database engine.
 
     Args:
         url: the DB url to use.
```

### Comparing `reflex-0.4.7a3/reflex/page.py` & `reflex-0.4.8a1/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/reflex.py` & `reflex-0.4.8a1/reflex/reflex.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,14 @@
     get_config(reload=True)
 
     console.rule("[bold]Starting Reflex App")
 
     prerequisites.check_latest_package_version(constants.Reflex.MODULE_NAME)
 
     if frontend:
-        prerequisites.update_next_config()
         # Get the app module.
         prerequisites.get_compiled_app()
 
     # Warn if schema is not up to date.
     prerequisites.check_schema_up_to_date()
 
     # Get the frontend and backend commands, based on the environment.
```

### Comparing `reflex-0.4.7a3/reflex/route.py` & `reflex-0.4.8a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/state.py` & `reflex-0.4.8a1/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/style.py` & `reflex-0.4.8a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/testing.py` & `reflex-0.4.8a1/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/utils/build.py` & `reflex-0.4.8a1/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/utils/console.py` & `reflex-0.4.8a1/reflex/utils/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,23 @@
     Args:
         log_level: The log level to set.
     """
     global _LOG_LEVEL
     _LOG_LEVEL = log_level
 
 
+def is_debug() -> bool:
+    """Check if the log level is debug.
+
+    Returns:
+        True if the log level is debug.
+    """
+    return _LOG_LEVEL <= LogLevel.DEBUG
+
+
 def print(msg: str, **kwargs):
     """Print a message.
 
     Args:
         msg: The message to print.
         kwargs: Keyword arguments to pass to the print function.
     """
@@ -41,15 +50,15 @@
 def debug(msg: str, **kwargs):
     """Print a debug message.
 
     Args:
         msg: The debug message.
         kwargs: Keyword arguments to pass to the print function.
     """
-    if _LOG_LEVEL <= LogLevel.DEBUG:
+    if is_debug():
         msg_ = f"[blue]Debug: {msg}[/blue]"
         if progress := kwargs.pop("progress", None):
             progress.console.print(msg_, **kwargs)
         else:
             print(msg_, **kwargs)
```

### Comparing `reflex-0.4.7a3/reflex/utils/exec.py` & `reflex-0.4.8a1/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/utils/export.py` & `reflex-0.4.8a1/reflex/utils/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,16 @@
     # Show system info
     exec.output_system_info()
 
     # Compile the app in production mode and export it.
     console.rule("[bold]Compiling production app and preparing for export.")
 
     if frontend:
-        # Update some parameters for export
-        prerequisites.update_next_config(export=True)
         # Ensure module can be imported and app.compile() is called.
-        prerequisites.get_compiled_app()
+        prerequisites.get_compiled_app(export=True)
         # Set up .web directory and install frontend dependencies.
         build.setup_frontend(Path.cwd())
 
     # Export the app.
     build.export(
         backend=backend,
         frontend=frontend,
```

### Comparing `reflex-0.4.7a3/reflex/utils/format.py` & `reflex-0.4.8a1/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/utils/imports.py` & `reflex-0.4.8a1/reflex/utils/imports.py`

 * *Files 23% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 
     # Whether this import need to install the associated lib
     install: Optional[bool] = True
 
     # whether this import should be rendered or not
     render: Optional[bool] = True
 
+    # whether this import package should be added to transpilePackages in next.config.js
+    # https://nextjs.org/docs/app/api-reference/next-config-js/transpilePackages
+    transpile: Optional[bool] = False
+
     @property
     def name(self) -> str:
         """The name of the import.
 
         Returns:
             The name(tag name with alias) of tag.
         """
@@ -68,11 +72,20 @@
 
     def __hash__(self) -> int:
         """Define a hash function for the import var.
 
         Returns:
             The hash of the var.
         """
-        return hash((self.tag, self.is_default, self.alias, self.install, self.render))
+        return hash(
+            (
+                self.tag,
+                self.is_default,
+                self.alias,
+                self.install,
+                self.render,
+                self.transpile,
+            )
+        )
 
 
 ImportDict = Dict[str, List[ImportVar]]
```

### Comparing `reflex-0.4.7a3/reflex/utils/path_ops.py` & `reflex-0.4.8a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/utils/prerequisites.py` & `reflex-0.4.8a1/reflex/utils/prerequisites.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import sys
 import tempfile
 import zipfile
 from datetime import datetime
 from fileinput import FileInput
 from pathlib import Path
 from types import ModuleType
-from typing import Callable, Optional
+from typing import Callable, List, Optional
 
 import httpx
 import pkg_resources
 import typer
 from alembic.util.exc import CommandError
 from packaging import version
 from redis import Redis as RedisSync
@@ -31,14 +31,15 @@
 
 import reflex
 from reflex import constants, model
 from reflex.base import Base
 from reflex.compiler import templates
 from reflex.config import Config, get_config
 from reflex.utils import console, path_ops, processes
+from reflex.utils.format import format_library_name
 
 CURRENTLY_INSTALLING_NODE = False
 
 
 class Template(Base):
     """A template for a Reflex app."""
 
@@ -162,24 +163,21 @@
             f"The detected bun version ({e.args[0]}) is not valid. Defaulting to None."
         )
         return None
 
 
 def get_install_package_manager() -> str | None:
     """Get the package manager executable for installation.
-      Currently on unix systems, bun is used for installation only.
+      Currently, bun is used for installation only.
 
     Returns:
         The path to the package manager.
     """
-    # On Windows, we use npm instead of bun.
-    if constants.IS_WINDOWS:
+    if constants.IS_WINDOWS and not constants.IS_WINDOWS_BUN_SUPPORTED_MACHINE:
         return get_package_manager()
-
-    # On other platforms, we use bun.
     return get_config().bun_path
 
 
 def get_package_manager() -> str | None:
     """Get the package manager executable for running app.
       Currently on unix systems, npm is used for running the app only.
 
@@ -223,29 +221,30 @@
 
         # Reload the app module.
         importlib.reload(app)
 
     return app
 
 
-def get_compiled_app(reload: bool = False) -> ModuleType:
+def get_compiled_app(reload: bool = False, export: bool = False) -> ModuleType:
     """Get the app module based on the default config after first compiling it.
 
     Args:
         reload: Re-import the app module from disk
+        export: Compile the app for export
 
     Returns:
         The compiled app based on the default config.
     """
     app_module = get_app(reload=reload)
     app = getattr(app_module, constants.CompileVars.APP)
     # For py3.8 and py3.9 compatibility when redis is used, we MUST add any decorator pages
     # before compiling the app in a thread to avoid event loop error (REF-2172).
     app._apply_decorated_pages()
-    app.compile_()
+    app.compile_(export=export)
     return app_module
 
 
 def get_redis() -> Redis | None:
     """Get the asynchronous redis client.
 
     Returns:
@@ -558,36 +557,45 @@
     reflex_json = {
         "version": constants.Reflex.VERSION,
         "project_hash": project_hash,
     }
     path_ops.update_json_file(constants.Reflex.JSON, reflex_json)
 
 
-def update_next_config(export=False):
+def update_next_config(export=False, transpile_packages: Optional[List[str]] = None):
     """Update Next.js config from Reflex config.
 
     Args:
         export: if the method run during reflex export.
+        transpile_packages: list of packages to transpile via next.config.js.
     """
     next_config_file = os.path.join(constants.Dirs.WEB, constants.Next.CONFIG_FILE)
 
-    next_config = _update_next_config(get_config(), export=export)
+    next_config = _update_next_config(
+        get_config(), export=export, transpile_packages=transpile_packages
+    )
 
     with open(next_config_file, "w") as file:
         file.write(next_config)
         file.write("\n")
 
 
-def _update_next_config(config, export=False):
+def _update_next_config(
+    config: Config, export: bool = False, transpile_packages: Optional[List[str]] = None
+):
     next_config = {
         "basePath": config.frontend_path or "",
         "compress": config.next_compression,
         "reactStrictMode": True,
         "trailingSlash": True,
     }
+    if transpile_packages:
+        next_config["transpilePackages"] = list(
+            set((format_library_name(p) for p in transpile_packages))
+        )
     if export:
         next_config["output"] = "export"
         next_config["distDir"] = constants.Dirs.STATIC
 
     next_config_json = re.sub(r'"([^"]+)"(?=:)', r"\1", json.dumps(next_config))
     return f"module.exports = {next_config_json};"
 
@@ -714,37 +722,46 @@
 
 def install_bun():
     """Install bun onto the user's system.
 
     Raises:
         FileNotFoundError: If required packages are not found.
     """
-    # Bun is not supported on Windows.
-    if constants.IS_WINDOWS:
-        console.debug("Skipping bun installation on Windows.")
-        return
+    if constants.IS_WINDOWS and not constants.IS_WINDOWS_BUN_SUPPORTED_MACHINE:
+        console.warn(
+            "Bun for Windows is currently only available for x86 64-bit Windows. Installation will fall back on npm."
+        )
 
     # Skip if bun is already installed.
     if os.path.exists(get_config().bun_path) and get_bun_version() == version.parse(
         constants.Bun.VERSION
     ):
         console.debug("Skipping bun installation as it is already installed.")
         return
 
     #  if unzip is installed
-    unzip_path = path_ops.which("unzip")
-    if unzip_path is None:
-        raise FileNotFoundError("Reflex requires unzip to be installed.")
-
-    # Run the bun install script.
-    download_and_run(
-        constants.Bun.INSTALL_URL,
-        f"bun-v{constants.Bun.VERSION}",
-        BUN_INSTALL=constants.Bun.ROOT_PATH,
-    )
+    if constants.IS_WINDOWS:
+        processes.new_process(
+            ["powershell", "-c", f"irm {constants.Bun.INSTALL_URL}.ps1|iex"],
+            env={"BUN_INSTALL": constants.Bun.ROOT_PATH},
+            shell=True,
+            run=True,
+            show_logs=console.is_debug(),
+        )
+    else:
+        unzip_path = path_ops.which("unzip")
+        if unzip_path is None:
+            raise FileNotFoundError("Reflex requires unzip to be installed.")
+
+        # Run the bun install script.
+        download_and_run(
+            constants.Bun.INSTALL_URL,
+            f"bun-v{constants.Bun.VERSION}",
+            BUN_INSTALL=constants.Bun.ROOT_PATH,
+        )
 
 
 def _write_cached_procedure_file(payload: str, cache_file: str):
     with open(cache_file, "w") as f:
         f.write(payload)
 
 
@@ -798,48 +815,52 @@
     Args:
         packages: A list of package names to be installed.
         config: The config object.
 
     Example:
         >>> install_frontend_packages(["react", "react-dom"], get_config())
     """
-    # Install the base packages.
-    process = processes.new_process(
+    # unsupported archs will use npm anyway. so we dont have to run npm twice
+    fallback_command = (
+        get_package_manager()
+        if constants.IS_WINDOWS and constants.IS_WINDOWS_BUN_SUPPORTED_MACHINE
+        else None
+    )
+    processes.run_process_with_fallback(
         [get_install_package_manager(), "install", "--loglevel", "silly"],
+        fallback=fallback_command,
+        show_status_message="Installing base frontend packages",
         cwd=constants.Dirs.WEB,
         shell=constants.IS_WINDOWS,
     )
 
-    processes.show_status("Installing base frontend packages", process)
-
     if config.tailwind is not None:
-        # install tailwind and tailwind plugins as dev dependencies.
-        process = processes.new_process(
+        processes.run_process_with_fallback(
             [
                 get_install_package_manager(),
                 "add",
                 "-d",
                 constants.Tailwind.VERSION,
                 *((config.tailwind or {}).get("plugins", [])),
             ],
+            fallback=fallback_command,
+            show_status_message="Installing tailwind",
             cwd=constants.Dirs.WEB,
             shell=constants.IS_WINDOWS,
         )
-        processes.show_status("Installing tailwind", process)
 
     # Install custom packages defined in frontend_packages
     if len(packages) > 0:
-        process = processes.new_process(
+        processes.run_process_with_fallback(
             [get_install_package_manager(), "add", *packages],
+            fallback=fallback_command,
+            show_status_message="Installing frontend packages from config and components",
             cwd=constants.Dirs.WEB,
             shell=constants.IS_WINDOWS,
         )
-        processes.show_status(
-            "Installing frontend packages from config and components", process
-        )
 
 
 def needs_reinit(frontend: bool = True) -> bool:
     """Check if an app needs to be reinitialized.
 
     Args:
         frontend: Whether to check if the frontend is initialized.
@@ -852,20 +873,24 @@
     """
     if not os.path.exists(constants.Config.FILE):
         console.error(
             f"[cyan]{constants.Config.FILE}[/cyan] not found. Move to the root folder of your project, or run [bold]{constants.Reflex.MODULE_NAME} init[/bold] to start a new project."
         )
         raise typer.Exit(1)
 
+    # Don't need to reinit if not running in frontend mode.
+    if not frontend:
+        return False
+
     # Make sure the .reflex directory exists.
     if not os.path.exists(constants.Reflex.DIR):
         return True
 
     # Make sure the .web directory exists in frontend mode.
-    if frontend and not os.path.exists(constants.Dirs.WEB):
+    if not os.path.exists(constants.Dirs.WEB):
         return True
 
     if constants.IS_WINDOWS:
         console.warn(
             """Windows Subsystem for Linux (WSL) is recommended for improving initial install times."""
         )
     # No need to reinitialize if the app is already initialized.
@@ -934,17 +959,14 @@
         if not check_node_version():
             node_version = get_node_version()
             console.error(
                 f"Reflex requires node version {constants.Node.MIN_VERSION} or higher to run, but the detected version is {node_version}",
             )
             raise typer.Exit(1)
 
-    if constants.IS_WINDOWS:
-        return
-
     if init:
         # we only need bun for package install on `reflex init`.
         validate_bun()
 
 
 def ensure_reflex_installation_id() -> Optional[int]:
     """Ensures that a reflex distinct id has been generated and stored in the reflex directory.
@@ -1365,15 +1387,17 @@
 
         # If user selects a template, it needs to exist.
         if template in templates:
             template_url = templates[template].code_url
         else:
             # Check if the template is a github repo.
             if template.startswith("https://github.com"):
-                template_url = f"{template.strip('/')}/archive/main.zip"
+                template_url = (
+                    f"{template.strip('/').replace('.git', '')}/archive/main.zip"
+                )
             else:
                 console.error(f"Template `{template}` not found.")
                 raise typer.Exit(1)
         create_config_init_app_from_remote_template(
             app_name=app_name,
             template_url=template_url,
         )
```

### Comparing `reflex-0.4.7a3/reflex/utils/processes.py` & `reflex-0.4.8a1/reflex/utils/processes.py`

 * *Files 12% similar despite different names*

```diff
@@ -283,7 +283,44 @@
                         progress.update(task, completed=len(checkpoints))
                     break
 
 
 def atexit_handler():
     """Display a custom message with the current time when exiting an app."""
     console.log("Reflex app stopped.")
+
+
+def run_process_with_fallback(args, *, show_status_message, fallback=None, **kwargs):
+    """Run subprocess and retry using fallback command if initial command fails.
+
+    Args:
+        args: A string, or a sequence of program arguments.
+        show_status_message: The status message to be displayed in the console.
+        fallback: The fallback command to run.
+        kwargs: Kwargs to pass to new_process function.
+    """
+
+    def execute_process(process):
+        if not constants.IS_WINDOWS:
+            show_status(show_status_message, process)
+        else:
+            process.wait()
+            if process.returncode != 0:
+                error_output = process.stderr if process.stderr else process.stdout
+                error_message = f"Error occurred during subprocess execution: {' '.join(args)}\n{error_output.read() if error_output else ''}"
+                # Only show error in debug mode.
+                if console.is_debug():
+                    console.error(error_message)
+
+                # retry with fallback command.
+                fallback_args = [fallback, *args[1:]] if fallback else None
+                console.warn(
+                    f"There was an error running command: {args}. Falling back to: {fallback_args}."
+                )
+                if fallback_args:
+                    process = new_process(fallback_args, **kwargs)
+                    execute_process(process)
+            else:
+                show_status(show_status_message, process)
+
+    process = new_process(args, **kwargs)
+    execute_process(process)
```

### Comparing `reflex-0.4.7a3/reflex/utils/pyi_generator.py` & `reflex-0.4.8a1/reflex/utils/pyi_generator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/utils/serializers.py` & `reflex-0.4.8a1/reflex/utils/serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import json
 import types as builtin_types
 import warnings
 from datetime import date, datetime, time, timedelta
+from enum import Enum
 from typing import Any, Callable, Dict, List, Set, Tuple, Type, Union, get_type_hints
 
 from reflex.base import Base
 from reflex.constants.colors import Color, format_color
 from reflex.utils import exceptions, format, types
 
 # Mapping from type to a serializer.
@@ -229,14 +230,27 @@
     Returns:
         The serialized datetime.
     """
     return str(dt)
 
 
 @serializer
+def serialize_enum(en: Enum) -> str:
+    """Serialize a enum to a JSON string.
+
+    Args:
+        en: The enum to serialize.
+
+    Returns:
+         The serialized enum.
+    """
+    return en.value
+
+
+@serializer
 def serialize_color(color: Color) -> str:
     """Serialize a color.
 
     Args:
         color: The color to serialize.
 
     Returns:
```

### Comparing `reflex-0.4.7a3/reflex/utils/telemetry.py` & `reflex-0.4.8a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/utils/types.py` & `reflex-0.4.8a1/reflex/utils/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import sqlalchemy
 
 try:
     # TODO The type checking guard can be removed once
     # reflex-hosting-cli tools are compatible with pydantic v2
 
     if not TYPE_CHECKING:
-        import pydantic.v1.fields as ModelField
+        from pydantic.v1.fields import ModelField
     else:
         raise ModuleNotFoundError
 except ModuleNotFoundError:
     from pydantic.fields import ModelField
 
 from sqlalchemy.ext.associationproxy import AssociationProxyInstance
 from sqlalchemy.ext.hybrid import hybrid_property
```

### Comparing `reflex-0.4.7a3/reflex/utils/watch.py` & `reflex-0.4.8a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/vars.py` & `reflex-0.4.8a1/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/reflex/vars.pyi` & `reflex-0.4.8a1/reflex/vars.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a3/PKG-INFO` & `reflex-0.4.8a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.4.7a3
+Version: 0.4.8a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.11.1,<2.0)
 Requires-Dist: build (>=1.0.3,<2.0)
 Requires-Dist: charset-normalizer (>=3.3.2,<4.0)
 Requires-Dist: dill (>=0.3.8,<0.4)
 Requires-Dist: distro (>=1.8.0,<2.0) ; sys_platform == "linux"
 Requires-Dist: fastapi (>=0.96.0,<1.0)
 Requires-Dist: gunicorn (>=20.1.0,<22.0)
```

