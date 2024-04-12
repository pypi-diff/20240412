# Comparing `tmp/ul-api-utils-7.8.5.tar.gz` & `tmp/ul-api-utils-7.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-api-utils-7.8.5.tar", last modified: Wed Apr 10 07:00:43 2024, max compression
+gzip compressed data, was "ul-api-utils-7.8.6.tar", last modified: Fri Apr 12 14:13:18 2024, max compression
```

## Comparing `ul-api-utils-7.8.5.tar` & `ul-api-utils-7.8.6.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2022-01-13 12:55:17.000000 ul-api-utils-7.8.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13527 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12938 2023-06-20 10:17:45.000000 ul-api-utils-7.8.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:42.987094 ul-api-utils-7.8.5/example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:42.999094 ul-api-utils-7.8.5/example/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-09-06 09:19:02.000000 ul-api-utils-7.8.5/example/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-16 17:17:46.000000 ul-api-utils-7.8.5/example/pure_flask_example.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-11 16:20:02.000000 ul-api-utils-7.8.5/example/rate_limit_load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:42.999094 ul-api-utils-7.8.5/example/routes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/routes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12856 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/routes/api_some.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:42.999094 ul-api-utils-7.8.5/example/workers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/workers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/example/workers/worker.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.019095 ul-api-utils-7.8.5/ul_api_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.027095 ul-api-utils-7.8.5/ul_api_utils/access/
--rw-rw-rw-   0 root         (0) root         (0)     4526 2023-09-06 09:19:02.000000 ul-api-utils-7.8.5/ul_api_utils/access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.051096 ul-api-utils-7.8.5/ul_api_utils/api_resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3279 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_request.py
--rw-rw-rw-   0 root         (0) root         (0)    17766 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_error_handling.py
--rw-rw-rw-   0 root         (0) root         (0)    18224 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_fn_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_type.py
--rw-rw-rw-   0 root         (0) root         (0)     9676 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response_db.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response_payload_alias.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/db_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/signature_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.059096 ul-api-utils-7.8.5/ul_api_utils/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8453 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_enc_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_gen_api_user_token.py
--rw-rw-rw-   0 root         (0) root         (0)     4549 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_gen_new_api_user.py
--rw-rw-rw-   0 root         (0) root         (0)     8788 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_generate_api_docs.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_start.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_worker_start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.063097 ul-api-utils-7.8.5/ul_api_utils/commands/start/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/start/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/start/gunicorn.conf.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/commands/start/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.075097 ul-api-utils-7.8.5/ul_api_utils/conf/
--rw-rw-rw-   0 root         (0) root         (0)   999747 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/conf/ul-debugger-main.js
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/conf/ul-debugger-ui.js
--rw-rw-rw-   0 root         (0) root         (0)     3232 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.087098 ul-api-utils-7.8.5/ul_api_utils/debug/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/debug/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/debug/debugger.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/debug/malloc.py
--rw-rw-rw-   0 root         (0) root         (0)    14591 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/debug/stat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.091098 ul-api-utils-7.8.5/ul_api_utils/encrypt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/encrypt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
--rw-rw-rw-   0 root         (0) root         (0)     8137 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.095098 ul-api-utils-7.8.5/ul_api_utils/internal_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.103098 ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
--rw-rw-rw-   0 root         (0) root         (0)    14067 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_check_context.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_error.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.107098 ul-api-utils-7.8.5/ul_api_utils/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.107098 ul-api-utils-7.8.5/ul_api_utils/modules/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/modules/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10719 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)    25626 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)     2389 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15112 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/intermediate_state.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/worker_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4620 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/worker_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/worker_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.119099 ul-api-utils-7.8.5/ul_api_utils/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7516 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/caching.py
--rw-rw-rw-   0 root         (0) root         (0)     5077 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/debugger_scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.135099 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/const.py
--rw-rw-rw-   0 root         (0) root         (0)    18449 2023-09-19 22:04:40.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/health_check_template.py
--rw-rw-rw-   0 root         (0) root         (0)     4199 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/resource.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/not_implemented.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3358 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/rate_limitter.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/sockets.py
--rw-rw-rw-   0 root         (0) root         (0)     5359 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/swagger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.135099 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.135099 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_fields/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_fields/custom_checkbox_select.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.139099 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3777 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     2699 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/uni_form.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.159100 ul-api-utils-7.8.5/ul_api_utils/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.159100 ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_format.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_method.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_request_info.py
--rw-rw-rw-   0 root         (0) root         (0)     5021 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/avro.py
--rw-rw-rw-   0 root         (0) root         (0)     1556 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/utils/broker_topics_message_count.py
--rw-rw-rw-   0 root         (0) root         (0)      670 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/cached_per_request.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/colors.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/decode_base64.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/deprecated.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-09-06 09:19:02.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.163100 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.163100 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)    28944 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.167101 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/imports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.167101 ul-api-utils-7.8.5/ul_api_utils/utils/jinja/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/jinja/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/jinja/t_url_for.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/jinja/to_pretty_json.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/load_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/token_check.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/token_check_through_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/uuid_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/ul_api_utils/validators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/validators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/ul_api_utils/validators/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/validators/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/validators/__tests__/test_custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4023 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/validators/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/validators/validate_empty_object.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/validators/validate_uuid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.027095 ul-api-utils-7.8.5/ul_api_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13527 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6050 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      516 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.439874 ul-api-utils-7.8.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2022-01-13 12:55:17.000000 ul-api-utils-7.8.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13527 2024-04-12 14:13:18.439874 ul-api-utils-7.8.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12938 2023-06-20 10:17:45.000000 ul-api-utils-7.8.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.279868 ul-api-utils-7.8.6/example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/example/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/example/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.279868 ul-api-utils-7.8.6/example/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/example/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-09-06 09:19:02.000000 ul-api-utils-7.8.6/example/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-16 17:17:46.000000 ul-api-utils-7.8.6/example/pure_flask_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-11 16:20:02.000000 ul-api-utils-7.8.6/example/rate_limit_load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.279868 ul-api-utils-7.8.6/example/routes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/example/routes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13299 2024-04-12 14:13:15.000000 ul-api-utils-7.8.6/example/routes/api_some.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.279868 ul-api-utils-7.8.6/example/workers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/example/workers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/example/workers/worker.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 14:13:18.439874 ul-api-utils-7.8.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-12 14:13:15.000000 ul-api-utils-7.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.299869 ul-api-utils-7.8.6/ul_api_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.307869 ul-api-utils-7.8.6/ul_api_utils/access/
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2023-09-06 09:19:02.000000 ul-api-utils-7.8.6/ul_api_utils/access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.331870 ul-api-utils-7.8.6/ul_api_utils/api_resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    17766 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/api_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/api_resource_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/api_resource_error_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)    18224 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/api_resource_fn_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/api_resource_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/api_response_db.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/api_response_payload_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/db_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/api_resource/signature_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.335870 ul-api-utils-7.8.6/ul_api_utils/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8453 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/commands/cmd_enc_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2024-02-12 08:16:10.000000 ul-api-utils-7.8.6/ul_api_utils/commands/cmd_gen_api_user_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/commands/cmd_gen_new_api_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     8788 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/commands/cmd_generate_api_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/commands/cmd_start.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/commands/cmd_worker_start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.335870 ul-api-utils-7.8.6/ul_api_utils/commands/start/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/commands/start/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/commands/start/gunicorn.conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/commands/start/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.351871 ul-api-utils-7.8.6/ul_api_utils/conf/
+-rw-rw-rw-   0 root         (0) root         (0)   999747 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/conf/ul-debugger-main.js
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/conf/ul-debugger-ui.js
+-rw-rw-rw-   0 root         (0) root         (0)     3232 2024-02-12 08:16:10.000000 ul-api-utils-7.8.6/ul_api_utils/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-02-12 08:16:10.000000 ul-api-utils-7.8.6/ul_api_utils/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.355871 ul-api-utils-7.8.6/ul_api_utils/debug/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/debug/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/debug/debugger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/debug/malloc.py
+-rw-rw-rw-   0 root         (0) root         (0)    14591 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/debug/stat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.363871 ul-api-utils-7.8.6/ul_api_utils/encrypt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/encrypt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
+-rw-rw-rw-   0 root         (0) root         (0)     8137 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.363871 ul-api-utils-7.8.6/ul_api_utils/internal_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/internal_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.367871 ul-api-utils-7.8.6/ul_api_utils/internal_api/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/internal_api/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/internal_api/__tests__/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    14067 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/internal_api/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/internal_api/internal_api_check_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/internal_api/internal_api_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/internal_api/internal_api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.371872 ul-api-utils-7.8.6/ul_api_utils/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.371872 ul-api-utils-7.8.6/ul_api_utils/modules/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/modules/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10719 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)    25626 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/modules/api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/modules/api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15112 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/modules/api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/modules/intermediate_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/modules/worker_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4620 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/modules/worker_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/modules/worker_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.383872 ul-api-utils-7.8.6/ul_api_utils/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7516 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/resources/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/resources/debugger_scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.395872 ul-api-utils-7.8.6/ul_api_utils/resources/health_check/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/resources/health_check/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/resources/health_check/const.py
+-rw-rw-rw-   0 root         (0) root         (0)    18449 2023-09-19 22:04:40.000000 ul-api-utils-7.8.6/ul_api_utils/resources/health_check/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/resources/health_check/health_check_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     4199 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/resources/health_check/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/resources/not_implemented.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/resources/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3358 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/resources/rate_limitter.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/resources/sockets.py
+-rw-rw-rw-   0 root         (0) root         (0)     5359 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/resources/swagger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.403873 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.403873 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/custom_fields/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/custom_fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/custom_fields/custom_checkbox_select.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.403873 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/custom_widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/custom_widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3777 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/uni_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.423873 ul-api-utils-7.8.6/ul_api_utils/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.427873 ul-api-utils-7.8.6/ul_api_utils/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/__tests__/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/__tests__/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/api_encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/api_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-02-12 08:16:10.000000 ul-api-utils-7.8.6/ul_api_utils/utils/api_method.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/api_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/api_request_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     5021 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/avro.py
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2024-02-12 08:16:10.000000 ul-api-utils-7.8.6/ul_api_utils/utils/broker_topics_message_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      670 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/cached_per_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/decode_base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/deprecated.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-09-06 09:19:02.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.427873 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.427873 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    28944 2024-04-10 07:00:41.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.431873 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/imports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.431873 ul-api-utils-7.8.6/ul_api_utils/utils/jinja/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/utils/jinja/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/jinja/t_url_for.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/jinja/to_pretty_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/load_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/token_check.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/token_check_through_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/utils/uuid_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.439874 ul-api-utils-7.8.6/ul_api_utils/validators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/validators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.439874 ul-api-utils-7.8.6/ul_api_utils/validators/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 14:13:16.000000 ul-api-utils-7.8.6/ul_api_utils/validators/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/validators/__tests__/test_custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4023 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/validators/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/validators/validate_empty_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-08-10 09:58:03.000000 ul-api-utils-7.8.6/ul_api_utils/validators/validate_uuid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 14:13:18.307869 ul-api-utils-7.8.6/ul_api_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13527 2024-04-12 14:13:18.000000 ul-api-utils-7.8.6/ul_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6050 2024-04-12 14:13:18.000000 ul-api-utils-7.8.6/ul_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 14:13:18.000000 ul-api-utils-7.8.6/ul_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-12 14:13:18.000000 ul-api-utils-7.8.6/ul_api_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      516 2024-04-12 14:13:18.000000 ul-api-utils-7.8.6/ul_api_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 14:13:18.000000 ul-api-utils-7.8.6/ul_api_utils.egg-info/top_level.txt
```

### Comparing `ul-api-utils-7.8.5/LICENSE` & `ul-api-utils-7.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/PKG-INFO` & `ul-api-utils-7.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.8.5
+Version: 7.8.6
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.8.5/README.md` & `ul-api-utils-7.8.6/README.md`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/example/conf.py` & `ul-api-utils-7.8.6/example/conf.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/example/pure_flask_example.py` & `ul-api-utils-7.8.6/example/pure_flask_example.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/example/routes/api_some.py` & `ul-api-utils-7.8.6/example/routes/api_some.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import logging
 from time import sleep
 from datetime import datetime, timedelta
 from typing import List, Optional, Tuple, Any
+
+from flask_socketio import emit
+
 from ul_api_utils.resources.sockets import socket_io
 from flask import jsonify
 from pydantic import BaseModel
 from ul_db_utils.modules.db import db
 from werkzeug import Response as BaseResponse
-
+from flask import request
 from example.conf import sdk
 from example.permissions import SOME_PERMISSION, SOME_PERMISSION2
 from ul_api_utils.api_resource.api_request import ApiRequestQuery
 from ul_api_utils.api_resource.api_resource import ApiResource
 from ul_api_utils.api_resource.api_resource_config import ApiResourceConfig
 from ul_api_utils.api_resource.api_response import FileApiResponse, JsonApiResponsePayload, JsonApiResponse, \
     AnyJsonApiResponse, ProxyJsonApiResponse, HtmlApiResponse, EmptyJsonApiResponse
@@ -47,14 +51,17 @@
 
 
 class Some2Query(ApiRequestQuery):
     sleep: float = 0.4
     some: QueryParamsSeparatedList[str] = ''        # type: ignore
 
 
+logger = logging.getLogger(__name__)
+
+
 @sdk.rest_api('POST', '/example-resource-simple', access=sdk.ACCESS_PUBLIC)
 @sdk.cache_api('REFRESH', 'example')
 def some5(api_resource: ApiResource, body: SomeBody) -> JsonApiResponse[List[RespObject]]:
     """
     The API returns user details for a given username.
     The API can be invoked using *curl* like below:
     ```
@@ -314,8 +321,21 @@
         as_attachment=True,
         attachment_filename='import_devices_log.txt',
     )
 
 
 @socket_io.on('message')
 def handle(data: Any, message: Any) -> None:
-    ...
+    sid = request.sid
+    emit('message', {"data1": 1, "data": 2}, room=sid)
+
+
+@socket_io.event
+def connect():
+    logger.info("Connected!")
+    logger.info("SESSION INFO: " + str(request.sid))
+
+
+@socket_io.event('disconnect')
+def disconnect():
+    logger.info("Client disconnected!")
+    logger.info("SESSION INFO: " + str(request.sid))
```

### Comparing `ul-api-utils-7.8.5/example/workers/worker.py` & `ul-api-utils-7.8.6/example/workers/worker.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/setup.py` & `ul-api-utils-7.8.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-api-utils',
-    version='7.8.5',
+    version='7.8.6',
     description='Python api utils',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='',
     packages=find_packages(),
     package_data={
```

### Comparing `ul-api-utils-7.8.5/ul_api_utils/access/__init__.py` & `ul-api-utils-7.8.6/ul_api_utils/access/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_request.py` & `ul-api-utils-7.8.6/ul_api_utils/api_resource/api_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource.py` & `ul-api-utils-7.8.6/ul_api_utils/api_resource/api_resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_config.py` & `ul-api-utils-7.8.6/ul_api_utils/api_resource/api_resource_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_error_handling.py` & `ul-api-utils-7.8.6/ul_api_utils/api_resource/api_resource_error_handling.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_fn_typing.py` & `ul-api-utils-7.8.6/ul_api_utils/api_resource/api_resource_fn_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response.py` & `ul-api-utils-7.8.6/ul_api_utils/api_resource/api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response_db.py` & `ul-api-utils-7.8.6/ul_api_utils/api_resource/api_response_db.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response_payload_alias.py` & `ul-api-utils-7.8.6/ul_api_utils/api_resource/api_response_payload_alias.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/api_resource/signature_check.py` & `ul-api-utils-7.8.6/ul_api_utils/api_resource/signature_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_enc_keys.py` & `ul-api-utils-7.8.6/ul_api_utils/commands/cmd_enc_keys.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_gen_api_user_token.py` & `ul-api-utils-7.8.6/ul_api_utils/commands/cmd_gen_api_user_token.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_gen_new_api_user.py` & `ul-api-utils-7.8.6/ul_api_utils/commands/cmd_gen_new_api_user.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_generate_api_docs.py` & `ul-api-utils-7.8.6/ul_api_utils/commands/cmd_generate_api_docs.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_start.py` & `ul-api-utils-7.8.6/ul_api_utils/commands/cmd_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_worker_start.py` & `ul-api-utils-7.8.6/ul_api_utils/commands/cmd_worker_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/commands/start/wsgi.py` & `ul-api-utils-7.8.6/ul_api_utils/commands/start/wsgi.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/conf/ul-debugger-main.js` & `ul-api-utils-7.8.6/ul_api_utils/conf/ul-debugger-main.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/conf/ul-debugger-ui.js` & `ul-api-utils-7.8.6/ul_api_utils/conf/ul-debugger-ui.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/conf.py` & `ul-api-utils-7.8.6/ul_api_utils/conf.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/const.py` & `ul-api-utils-7.8.6/ul_api_utils/const.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/debug/debugger.py` & `ul-api-utils-7.8.6/ul_api_utils/debug/debugger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/debug/malloc.py` & `ul-api-utils-7.8.6/ul_api_utils/debug/malloc.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/debug/stat.py` & `ul-api-utils-7.8.6/ul_api_utils/debug/stat.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py` & `ul-api-utils-7.8.6/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/errors.py` & `ul-api-utils-7.8.6/ul_api_utils/errors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/internal_api.py` & `ul-api-utils-7.8.6/ul_api_utils/internal_api/__tests__/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/internal_api_content_type.py` & `ul-api-utils-7.8.6/ul_api_utils/internal_api/__tests__/internal_api_content_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api.py` & `ul-api-utils-7.8.6/ul_api_utils/internal_api/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_check_context.py` & `ul-api-utils-7.8.6/ul_api_utils/internal_api/internal_api_check_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_response.py` & `ul-api-utils-7.8.6/ul_api_utils/internal_api/internal_api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/main.py` & `ul-api-utils-7.8.6/ul_api_utils/main.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py` & `ul-api-utils-7.8.6/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk.py` & `ul-api-utils-7.8.6/ul_api_utils/modules/api_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk_config.py` & `ul-api-utils-7.8.6/ul_api_utils/modules/api_sdk_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk_jwt.py` & `ul-api-utils-7.8.6/ul_api_utils/modules/api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/modules/intermediate_state.py` & `ul-api-utils-7.8.6/ul_api_utils/modules/intermediate_state.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/modules/worker_context.py` & `ul-api-utils-7.8.6/ul_api_utils/modules/worker_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/modules/worker_sdk.py` & `ul-api-utils-7.8.6/ul_api_utils/modules/worker_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/caching.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/caching.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/debugger_scripts.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/debugger_scripts.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/health_check/health_check.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/health_check/health_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/health_check/health_check_template.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/health_check/health_check_template.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/health_check/resource.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/health_check/resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/not_implemented.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/not_implemented.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/permissions.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/rate_limitter.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/rate_limitter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/swagger.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/swagger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/uni_form.py` & `ul-api-utils-7.8.6/ul_api_utils/resources/web_forms/uni_form.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/sentry.py` & `ul-api-utils-7.8.6/ul_api_utils/sentry.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/api_path_version.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/__tests__/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/unwrap_typing.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/__tests__/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/api_encoding.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/api_encoding.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/api_format.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/api_format.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/api_method.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/api_method.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/api_pagination.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/api_pagination.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/api_path_version.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/avro.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/avro.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/broker_topics_message_count.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/broker_topics_message_count.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/cached_per_request.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/cached_per_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/colors.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/deprecated.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flags.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flags.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/json_encoder.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/load_modules.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/load_modules.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/token_check_through_request.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/token_check_through_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/unwrap_typing.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/utils/uuid_converter.py` & `ul-api-utils-7.8.6/ul_api_utils/utils/uuid_converter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/validators/__tests__/test_custom_fields.py` & `ul-api-utils-7.8.6/ul_api_utils/validators/__tests__/test_custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils/validators/custom_fields.py` & `ul-api-utils-7.8.6/ul_api_utils/validators/custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils.egg-info/PKG-INFO` & `ul-api-utils-7.8.6/ul_api_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.8.5
+Version: 7.8.6
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.8.5/ul_api_utils.egg-info/SOURCES.txt` & `ul-api-utils-7.8.6/ul_api_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.5/ul_api_utils.egg-info/requires.txt` & `ul-api-utils-7.8.6/ul_api_utils.egg-info/requires.txt`

 * *Files identical despite different names*

