# Comparing `tmp/chiefgram-3.5.tar.gz` & `tmp/chiefgram-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiefgram-3.5.tar", last modified: Fri Apr 12 03:02:08 2024, max compression
+gzip compressed data, was "chiefgram-4.0.tar", last modified: Fri Apr 12 03:08:58 2024, max compression
```

## Comparing `chiefgram-3.5.tar` & `chiefgram-4.0.tar`

### file list

```diff
@@ -1,514 +1,514 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.722126 chiefgram-3.5/
--rw-r--r--   0 root         (0) root         (0)      310 2024-04-12 02:13:07.000000 chiefgram-3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      370 2024-04-12 03:02:08.722126 chiefgram-3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2490 2024-04-12 02:13:07.000000 chiefgram-3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.626127 chiefgram-3.5/chiefgram/
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.626127 chiefgram-3.5/chiefgram/chiefmod/
--rw-r--r--   0 root         (0) root         (0)     1303 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.626127 chiefgram-3.5/chiefgram/chiefmod/config/
--rw-r--r--   0 root         (0) root         (0)      317 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      263 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.626127 chiefgram-3.5/chiefgram/chiefmod/exceptions/
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/exceptions/listener_stopped.py
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/exceptions/listener_timeout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.626127 chiefgram-3.5/chiefgram/chiefmod/helpers/
--rw-r--r--   0 root         (0) root         (0)      931 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2149 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/helpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.638127 chiefgram-3.5/chiefgram/chiefmod/listen/
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5013 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/listen/callback_query_handler.py
--rw-r--r--   0 root         (0) root         (0)      621 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/listen/chat.py
--rw-r--r--   0 root         (0) root         (0)     8284 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/listen/client.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/listen/message.py
--rw-r--r--   0 root         (0) root         (0)     3559 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/listen/message_handler.py
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/listen/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.638127 chiefgram-3.5/chiefgram/chiefmod/nav/
--rw-r--r--   0 root         (0) root         (0)      832 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/nav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3543 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/nav/pagination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.638127 chiefgram-3.5/chiefgram/chiefmod/types/
--rw-r--r--   0 root         (0) root         (0)      163 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/types/identifier.py
--rw-r--r--   0 root         (0) root         (0)      402 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/types/listener.py
--rw-r--r--   0 root         (0) root         (0)      113 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/types/listener_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.638127 chiefgram-3.5/chiefgram/chiefmod/utils/
--rw-r--r--   0 root         (0) root         (0)      859 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3384 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/chiefmod/utils/patch.py
--rw-r--r--   0 root         (0) root         (0)    40500 2024-04-12 03:01:36.000000 chiefgram-3.5/chiefgram/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.638127 chiefgram-3.5/chiefgram/connection/
--rw-r--r--   0 root         (0) root         (0)      858 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2546 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.638127 chiefgram-3.5/chiefgram/connection/transport/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/transport/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.638127 chiefgram-3.5/chiefgram/connection/transport/tcp/
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/transport/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4093 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/transport/tcp/tcp.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 root         (0) root         (0)     2838 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 root         (0) root         (0)     1910 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 root         (0) root         (0)     1515 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 root         (0) root         (0)     2458 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.638127 chiefgram-3.5/chiefgram/crypto/
--rw-r--r--   0 root         (0) root         (0)      823 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/crypto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4013 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/crypto/aes.py
--rw-r--r--   0 root         (0) root         (0)     4025 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/crypto/mtproto.py
--rw-r--r--   0 root         (0) root         (0)     2451 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/crypto/prime.py
--rw-r--r--   0 root         (0) root         (0)    13442 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/crypto/rsa.py
--rw-r--r--   0 root         (0) root         (0)    10075 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)   208025 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/emoji.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.642127 chiefgram-3.5/chiefgram/enums/
--rw-r--r--   0 root         (0) root         (0)     1741 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1008 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/auto_name.py
--rw-r--r--   0 root         (0) root         (0)     2314 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4209 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/chat_event_action.py
--rw-r--r--   0 root         (0) root         (0)     1271 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/chat_member_status.py
--rw-r--r--   0 root         (0) root         (0)     1453 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/chat_members_filter.py
--rw-r--r--   0 root         (0) root         (0)     1244 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/chat_type.py
--rw-r--r--   0 root         (0) root         (0)     2474 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/message_entity_type.py
--rw-r--r--   0 root         (0) root         (0)     1605 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/message_media_type.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/message_service_type.py
--rw-r--r--   0 root         (0) root         (0)     2414 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/messages_filter.py
--rw-r--r--   0 root         (0) root         (0)     1528 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/next_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1193 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/parse_mode.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/poll_type.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/sent_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/enums/user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.642127 chiefgram-3.5/chiefgram/errors/
--rw-r--r--   0 root         (0) root         (0)     2610 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3324 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/errors/rpc_error.py
--rw-r--r--   0 root         (0) root         (0)    15160 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/file_id.py
--rw-r--r--   0 root         (0) root         (0)    24874 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.650127 chiefgram-3.5/chiefgram/handlers/
--rw-r--r--   0 root         (0) root         (0)     1480 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2035 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/callback_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     2020 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/chat_join_request_handler.py
--rw-r--r--   0 root         (0) root         (0)     2055 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 root         (0) root         (0)     2556 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/deleted_messages_handler.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/disconnect_handler.py
--rw-r--r--   0 root         (0) root         (0)     1988 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/edited_message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/handler.py
--rw-r--r--   0 root         (0) root         (0)     1993 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/inline_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     1944 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1923 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/poll_handler.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/raw_update_handler.py
--rw-r--r--   0 root         (0) root         (0)     1998 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/handlers/user_status_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.650127 chiefgram-3.5/chiefgram/methods/
--rw-r--r--   0 root         (0) root         (0)     1325 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.650127 chiefgram-3.5/chiefgram/methods/advanced/
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/advanced/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/advanced/invoke.py
--rw-r--r--   0 root         (0) root         (0)     4571 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/advanced/resolve_peer.py
--rw-r--r--   0 root         (0) root         (0)     8432 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/advanced/save_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.654127 chiefgram-3.5/chiefgram/methods/auth/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 root         (0) root         (0)     1953 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/check_password.py
--rw-r--r--   0 root         (0) root         (0)     1757 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/connect.py
--rw-r--r--   0 root         (0) root         (0)     1511 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/disconnect.py
--rw-r--r--   0 root         (0) root         (0)     1315 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/get_password_hint.py
--rw-r--r--   0 root         (0) root         (0)     1769 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1634 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/log_out.py
--rw-r--r--   0 root         (0) root         (0)     1841 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/recover_password.py
--rw-r--r--   0 root         (0) root         (0)     2161 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/resend_code.py
--rw-r--r--   0 root         (0) root         (0)     2798 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/send_code.py
--rw-r--r--   0 root         (0) root         (0)     1481 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/send_recovery_code.py
--rw-r--r--   0 root         (0) root         (0)     3098 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/sign_in.py
--rw-r--r--   0 root         (0) root         (0)     2735 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/sign_in_bot.py
--rw-r--r--   0 root         (0) root         (0)     2366 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/sign_up.py
--rw-r--r--   0 root         (0) root         (0)     2051 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/auth/terminate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.658127 chiefgram-3.5/chiefgram/methods/bots/
--rw-r--r--   0 root         (0) root         (0)     2046 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3319 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/answer_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     5001 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/answer_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2000 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 root         (0) root         (0)     2370 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2584 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/get_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2328 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     2808 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 root         (0) root         (0)     3377 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/request_callback_answer.py
--rw-r--r--   0 root         (0) root         (0)     3967 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/send_game.py
--rw-r--r--   0 root         (0) root         (0)     2836 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 root         (0) root         (0)     2723 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/set_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     3197 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2059 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     3956 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/bots/set_game_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.662127 chiefgram-3.5/chiefgram/methods/chats/
--rw-r--r--   0 root         (0) root         (0)     3444 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3372 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/add_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2224 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/archive_chats.py
--rw-r--r--   0 root         (0) root         (0)     4630 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/ban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1827 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/create_channel.py
--rw-r--r--   0 root         (0) root         (0)     2292 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/create_group.py
--rw-r--r--   0 root         (0) root         (0)     1966 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/create_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1593 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/delete_channel.py
--rw-r--r--   0 root         (0) root         (0)     2315 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1611 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/delete_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/delete_user_history.py
--rw-r--r--   0 root         (0) root         (0)     3295 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_chat.py
--rw-r--r--   0 root         (0) root         (0)     4043 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 root         (0) root         (0)     3349 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2272 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 root         (0) root         (0)     3369 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_dialogs.py
--rw-r--r--   0 root         (0) root         (0)     2104 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 root         (0) root         (0)     2146 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 root         (0) root         (0)     2706 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/join_chat.py
--rw-r--r--   0 root         (0) root         (0)     2613 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/leave_chat.py
--rw-r--r--   0 root         (0) root         (0)     1536 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 root         (0) root         (0)     3166 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/pin_chat_message.py
--rw-r--r--   0 root         (0) root         (0)     3870 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/promote_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     4324 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3144 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/set_administrator_title.py
--rw-r--r--   0 root         (0) root         (0)     2255 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/set_chat_description.py
--rw-r--r--   0 root         (0) root         (0)     3427 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     4613 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/set_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1735 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 root         (0) root         (0)     2580 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/set_chat_title.py
--rw-r--r--   0 root         (0) root         (0)     2305 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/set_chat_username.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 root         (0) root         (0)     2091 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/set_slow_mode.py
--rw-r--r--   0 root         (0) root         (0)     2238 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/unarchive_chats.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/unban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1948 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.670127 chiefgram-3.5/chiefgram/methods/contacts/
--rw-r--r--   0 root         (0) root         (0)     1159 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/contacts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2576 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/contacts/add_contact.py
--rw-r--r--   0 root         (0) root         (0)     2458 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/contacts/delete_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/contacts/get_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1430 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 root         (0) root         (0)     1945 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.670127 chiefgram-3.5/chiefgram/methods/decorators/
--rw-r--r--   0 root         (0) root         (0)     1629 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2194 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2182 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2203 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     2230 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     2196 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_disconnect.py
--rw-r--r--   0 root         (0) root         (0)     2185 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_edited_message.py
--rw-r--r--   0 root         (0) root         (0)     2180 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_message.py
--rw-r--r--   0 root         (0) root         (0)     2133 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_poll.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_raw_update.py
--rw-r--r--   0 root         (0) root         (0)     2167 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.678127 chiefgram-3.5/chiefgram/methods/invite_links/
--rw-r--r--   0 root         (0) root         (0)     2440 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1932 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     3380 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1933 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2039 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1759 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3543 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2592 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3577 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     2343 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 root         (0) root         (0)     2006 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1935 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 root         (0) root         (0)     1937 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     2339 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.686127 chiefgram-3.5/chiefgram/methods/messages/
--rw-r--r--   0 root         (0) root         (0)     3926 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5972 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/copy_media_group.py
--rw-r--r--   0 root         (0) root         (0)     5194 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/copy_message.py
--rw-r--r--   0 root         (0) root         (0)     3156 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/delete_messages.py
--rw-r--r--   0 root         (0) root         (0)     7541 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/download_media.py
--rw-r--r--   0 root         (0) root         (0)     2281 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 root         (0) root         (0)    10390 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/edit_inline_media.py
--rw-r--r--   0 root         (0) root         (0)     2476 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3127 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/edit_inline_text.py
--rw-r--r--   0 root         (0) root         (0)     2990 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/edit_message_caption.py
--rw-r--r--   0 root         (0) root         (0)    13037 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/edit_message_media.py
--rw-r--r--   0 root         (0) root         (0)     2988 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     4575 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/forward_messages.py
--rw-r--r--   0 root         (0) root         (0)     4051 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/get_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2398 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 root         (0) root         (0)     2238 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/get_discussion_message.py
--rw-r--r--   0 root         (0) root         (0)     2816 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 root         (0) root         (0)     2955 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/get_media_group.py
--rw-r--r--   0 root         (0) root         (0)     4753 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/get_messages.py
--rw-r--r--   0 root         (0) root         (0)     2186 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/inline_session.py
--rw-r--r--   0 root         (0) root         (0)     2535 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/read_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2134 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/retract_vote.py
--rw-r--r--   0 root         (0) root         (0)     4176 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/search_global.py
--rw-r--r--   0 root         (0) root         (0)     2166 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/search_global_count.py
--rw-r--r--   0 root         (0) root         (0)     5361 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/search_messages.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/search_messages_count.py
--rw-r--r--   0 root         (0) root         (0)    12605 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_animation.py
--rw-r--r--   0 root         (0) root         (0)    11140 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_audio.py
--rw-r--r--   0 root         (0) root         (0)     5496 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_cached_media.py
--rw-r--r--   0 root         (0) root         (0)     2827 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4881 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_contact.py
--rw-r--r--   0 root         (0) root         (0)     4855 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_dice.py
--rw-r--r--   0 root         (0) root         (0)    10489 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_document.py
--rw-r--r--   0 root         (0) root         (0)     4590 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_location.py
--rw-r--r--   0 root         (0) root         (0)    19923 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_media_group.py
--rw-r--r--   0 root         (0) root         (0)     7285 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_message.py
--rw-r--r--   0 root         (0) root         (0)     9459 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_photo.py
--rw-r--r--   0 root         (0) root         (0)     8091 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_poll.py
--rw-r--r--   0 root         (0) root         (0)     2369 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_reaction.py
--rw-r--r--   0 root         (0) root         (0)     8357 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_sticker.py
--rw-r--r--   0 root         (0) root         (0)     5411 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_venue.py
--rw-r--r--   0 root         (0) root         (0)    11975 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_video.py
--rw-r--r--   0 root         (0) root         (0)     9331 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_video_note.py
--rw-r--r--   0 root         (0) root         (0)     9449 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/send_voice.py
--rw-r--r--   0 root         (0) root         (0)     2830 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/stop_poll.py
--rw-r--r--   0 root         (0) root         (0)     3947 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/stream_media.py
--rw-r--r--   0 root         (0) root         (0)     2514 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/messages/vote_poll.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.686127 chiefgram-3.5/chiefgram/methods/password/
--rw-r--r--   0 root         (0) root         (0)     1093 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2806 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/password/change_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/password/enable_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.690127 chiefgram-3.5/chiefgram/methods/users/
--rw-r--r--   0 root         (0) root         (0)     1664 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/block_user.py
--rw-r--r--   0 root         (0) root         (0)     2248 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/delete_profile_photos.py
--rw-r--r--   0 root         (0) root         (0)     4430 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/get_chat_photos.py
--rw-r--r--   0 root         (0) root         (0)     2517 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 root         (0) root         (0)     2369 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/get_common_chats.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/get_me.py
--rw-r--r--   0 root         (0) root         (0)     2573 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/get_users.py
--rw-r--r--   0 root         (0) root         (0)     1892 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/set_emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/set_profile_photo.py
--rw-r--r--   0 root         (0) root         (0)     1885 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/set_username.py
--rw-r--r--   0 root         (0) root         (0)     1789 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/unblock_user.py
--rw-r--r--   0 root         (0) root         (0)     2387 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/users/update_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.690127 chiefgram-3.5/chiefgram/methods/utilities/
--rw-r--r--   0 root         (0) root         (0)     1258 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2357 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/add_handler.py
--rw-r--r--   0 root         (0) root         (0)     2243 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/compose.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/export_session_string.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/idle.py
--rw-r--r--   0 root         (0) root         (0)     2222 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/remove_handler.py
--rw-r--r--   0 root         (0) root         (0)     2305 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/restart.py
--rw-r--r--   0 root         (0) root         (0)     2872 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/run.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/start.py
--rw-r--r--   0 root         (0) root         (0)     2126 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/stop.py
--rw-r--r--   0 root         (0) root         (0)     1717 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/methods/utilities/stop_transmission.py
--rw-r--r--   0 root         (0) root         (0)    61920 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/mime_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.690127 chiefgram-3.5/chiefgram/parser/
--rw-r--r--   0 root         (0) root         (0)      851 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8695 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/parser/html.py
--rw-r--r--   0 root         (0) root         (0)     5778 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/parser/markdown.py
--rw-r--r--   0 root         (0) root         (0)     2085 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1550 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/parser/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.690127 chiefgram-3.5/chiefgram/raw/
--rw-r--r--   0 root         (0) root         (0)     1044 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.694126 chiefgram-3.5/chiefgram/raw/core/
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1696 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/future_salt.py
--rw-r--r--   0 root         (0) root         (0)     1895 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/future_salts.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/gzip_packed.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/list.py
--rw-r--r--   0 root         (0) root         (0)     1855 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/message.py
--rw-r--r--   0 root         (0) root         (0)     1618 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/msg_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.694126 chiefgram-3.5/chiefgram/raw/core/primitives/
--rw-r--r--   0 root         (0) root         (0)     1016 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1501 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/primitives/bool.py
--rw-r--r--   0 root         (0) root         (0)     1763 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/primitives/bytes.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/primitives/double.py
--rw-r--r--   0 root         (0) root         (0)     1362 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/primitives/int.py
--rw-r--r--   0 root         (0) root         (0)     1198 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/primitives/string.py
--rw-r--r--   0 root         (0) root         (0)     2026 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/primitives/vector.py
--rw-r--r--   0 root         (0) root         (0)     2500 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/raw/core/tl_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.694126 chiefgram-3.5/chiefgram/session/
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/session/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11458 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/session/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.694126 chiefgram-3.5/chiefgram/session/internals/
--rw-r--r--   0 root         (0) root         (0)      922 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/session/internals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/session/internals/data_center.py
--rw-r--r--   0 root         (0) root         (0)     1382 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/session/internals/msg_factory.py
--rw-r--r--   0 root         (0) root         (0)     1161 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/session/internals/msg_id.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/session/internals/seq_no.py
--rw-r--r--   0 root         (0) root         (0)    13434 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/session/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.694126 chiefgram-3.5/chiefgram/storage/
--rw-r--r--   0 root         (0) root         (0)      932 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1963 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/storage/file_storage.py
--rw-r--r--   0 root         (0) root         (0)     2754 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/storage/memory_storage.py
--rw-r--r--   0 root         (0) root         (0)     6229 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2785 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/storage/storage.py
--rw-r--r--   0 root         (0) root         (0)     3747 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.698126 chiefgram-3.5/chiefgram/types/
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.698126 chiefgram-3.5/chiefgram/types/authorization/
--rw-r--r--   0 root         (0) root         (0)      943 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/authorization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2300 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/authorization/sent_code.py
--rw-r--r--   0 root         (0) root         (0)     1939 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.702126 chiefgram-3.5/chiefgram/types/bots_and_keyboards/
--rw-r--r--   0 root         (0) root         (0)     2835 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 root         (0) root         (0)     2803 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 root         (0) root         (0)     1301 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 root         (0) root         (0)     1257 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 root         (0) root         (0)     1647 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1825 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 root         (0) root         (0)    12826 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2391 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 root         (0) root         (0)     2226 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 root         (0) root         (0)     8133 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     2470 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     3521 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     3718 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 root         (0) root         (0)     1217 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 root         (0) root         (0)     1220 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 root         (0) root         (0)     1819 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 root         (0) root         (0)     4585 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     2347 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 root         (0) root         (0)     1318 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.706126 chiefgram-3.5/chiefgram/types/inline_mode/
--rw-r--r--   0 root         (0) root         (0)     2760 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     7313 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 root         (0) root         (0)     5788 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 root         (0) root         (0)     3315 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 root         (0) root         (0)     4517 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 root         (0) root         (0)     4257 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 root         (0) root         (0)     4041 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 root         (0) root         (0)     4400 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 root         (0) root         (0)     4324 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 root         (0) root         (0)     3041 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 root         (0) root         (0)     4406 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 root         (0) root         (0)     4214 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 root         (0) root         (0)     4142 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 root         (0) root         (0)     5252 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 root         (0) root         (0)     4629 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 root         (0) root         (0)     5273 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 root         (0) root         (0)     5486 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 root         (0) root         (0)     4372 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.706126 chiefgram-3.5/chiefgram/types/input_media/
--rw-r--r--   0 root         (0) root         (0)     1319 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_media/input_media.py
--rw-r--r--   0 root         (0) root         (0)     3435 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_media/input_media_animation.py
--rw-r--r--   0 root         (0) root         (0)     3290 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_media/input_media_audio.py
--rw-r--r--   0 root         (0) root         (0)     2778 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_media/input_media_document.py
--rw-r--r--   0 root         (0) root         (0)     2693 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_media/input_media_photo.py
--rw-r--r--   0 root         (0) root         (0)     3628 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_media/input_media_video.py
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.706126 chiefgram-3.5/chiefgram/types/input_message_content/
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_message_content/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_message_content/input_message_content.py
--rw-r--r--   0 root         (0) root         (0)     2648 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 root         (0) root         (0)     1099 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.714126 chiefgram-3.5/chiefgram/types/messages_and_media/
--rw-r--r--   0 root         (0) root         (0)     1841 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4055 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/animation.py
--rw-r--r--   0 root         (0) root         (0)     4080 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/audio.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/contact.py
--rw-r--r--   0 root         (0) root         (0)     1595 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/dice.py
--rw-r--r--   0 root         (0) root         (0)     3420 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/document.py
--rw-r--r--   0 root         (0) root         (0)     3055 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/game.py
--rw-r--r--   0 root         (0) root         (0)     1668 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/location.py
--rw-r--r--   0 root         (0) root         (0)   144740 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/message.py
--rw-r--r--   0 root         (0) root         (0)     4367 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/message_entity.py
--rw-r--r--   0 root         (0) root         (0)     1810 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/photo.py
--rw-r--r--   0 root         (0) root         (0)     7049 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/poll.py
--rw-r--r--   0 root         (0) root         (0)     1539 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/poll_option.py
--rw-r--r--   0 root         (0) root         (0)     2627 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/reaction.py
--rw-r--r--   0 root         (0) root         (0)     6921 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/sticker.py
--rw-r--r--   0 root         (0) root         (0)     1439 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     3764 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     2301 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/venue.py
--rw-r--r--   0 root         (0) root         (0)     4400 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/video.py
--rw-r--r--   0 root         (0) root         (0)     3612 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/video_note.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/voice.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 root         (0) root         (0)     6365 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/messages_and_media/web_page.py
--rw-r--r--   0 root         (0) root         (0)     3875 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/object.py
--rw-r--r--   0 root         (0) root         (0)     1010 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.718126 chiefgram-3.5/chiefgram/types/user_and_chats/
--rw-r--r--   0 root         (0) root         (0)     2302 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32619 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat.py
--rw-r--r--   0 root         (0) root         (0)     2246 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)    19882 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_event.py
--rw-r--r--   0 root         (0) root         (0)     5520 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 root         (0) root         (0)     4589 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     4260 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2575 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 root         (0) root         (0)     9461 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3689 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     4388 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     3976 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     2603 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 root         (0) root         (0)     4957 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2365 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 root         (0) root         (0)     2693 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/dialog.py
--rw-r--r--   0 root         (0) root         (0)     2431 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     1959 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 root         (0) root         (0)     1669 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/restriction.py
--rw-r--r--   0 root         (0) root         (0)    12857 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/user.py
--rw-r--r--   0 root         (0) root         (0)     1352 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 root         (0) root         (0)    10582 2024-04-12 02:13:07.000000 chiefgram-3.5/chiefgram/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.722126 chiefgram-3.5/chiefgram.egg-info/
--rw-r--r--   0 root         (0) root         (0)      370 2024-04-12 03:02:08.000000 chiefgram-3.5/chiefgram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19905 2024-04-12 03:02:08.000000 chiefgram-3.5/chiefgram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 03:02:08.000000 chiefgram-3.5/chiefgram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 03:02:08.000000 chiefgram-3.5/chiefgram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-12 03:02:08.000000 chiefgram-3.5/chiefgram.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.718126 chiefgram-3.5/compiler/
--rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.718126 chiefgram-3.5/compiler/api/
--rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22426 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/api/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.718126 chiefgram-3.5/compiler/api/source/
--rw-r--r--   0 root         (0) root         (0)     2233 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/api/source/auth_key.tl
--rw-r--r--   0 root         (0) root         (0)   168867 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/api/source/main_api.tl
--rw-r--r--   0 root         (0) root         (0)     3425 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.718126 chiefgram-3.5/compiler/api/template/
--rw-r--r--   0 root         (0) root         (0)      746 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/api/template/combinator.txt
--rw-r--r--   0 root         (0) root         (0)      639 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/api/template/type.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.718126 chiefgram-3.5/compiler/errors/
--rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4925 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/compiler.py
--rw-r--r--   0 root         (0) root         (0)     1269 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.722126 chiefgram-3.5/compiler/errors/source/
--rw-r--r--   0 root         (0) root         (0)      470 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 root         (0) root         (0)    22642 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 root         (0) root         (0)      678 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 root         (0) root         (0)     2000 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 root         (0) root         (0)     1177 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 root         (0) root         (0)      470 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 root         (0) root         (0)      155 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.722126 chiefgram-3.5/compiler/errors/template/
--rw-r--r--   0 root         (0) root         (0)      178 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/template/class.txt
--rw-r--r--   0 root         (0) root         (0)      120 2024-04-12 02:13:07.000000 chiefgram-3.5/compiler/errors/template/sub_class.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 02:13:07.000000 chiefgram-3.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 03:02:08.722126 chiefgram-3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      667 2024-04-12 03:01:36.000000 chiefgram-3.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.722126 chiefgram-3.5/tests/
--rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-3.5/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.722126 chiefgram-3.5/tests/filters/
--rw-r--r--   0 root         (0) root         (0)     1207 2024-04-12 02:13:07.000000 chiefgram-3.5/tests/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-12 02:13:07.000000 chiefgram-3.5/tests/filters/test_command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:02:08.722126 chiefgram-3.5/tests/parser/
--rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-3.5/tests/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6329 2024-04-12 02:13:07.000000 chiefgram-3.5/tests/parser/test_html.py
--rw-r--r--   0 root         (0) root         (0)     8215 2024-04-12 02:13:07.000000 chiefgram-3.5/tests/test_file_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.899876 chiefgram-4.0/
+-rw-r--r--   0 root         (0) root         (0)      310 2024-04-12 02:13:07.000000 chiefgram-4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      370 2024-04-12 03:08:58.899876 chiefgram-4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-12 02:13:07.000000 chiefgram-4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.803878 chiefgram-4.0/chiefgram/
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.803878 chiefgram-4.0/chiefgram/chiefmod/
+-rw-r--r--   0 root         (0) root         (0)     1303 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.803878 chiefgram-4.0/chiefgram/chiefmod/config/
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      263 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.803878 chiefgram-4.0/chiefgram/chiefmod/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/exceptions/listener_stopped.py
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/exceptions/listener_timeout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.803878 chiefgram-4.0/chiefgram/chiefmod/helpers/
+-rw-r--r--   0 root         (0) root         (0)      931 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/helpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.807878 chiefgram-4.0/chiefgram/chiefmod/listen/
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5013 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/listen/callback_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/listen/chat.py
+-rw-r--r--   0 root         (0) root         (0)     8284 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/listen/client.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/listen/message.py
+-rw-r--r--   0 root         (0) root         (0)     3559 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/listen/message_handler.py
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/listen/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.807878 chiefgram-4.0/chiefgram/chiefmod/nav/
+-rw-r--r--   0 root         (0) root         (0)      832 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/nav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3543 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/nav/pagination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.807878 chiefgram-4.0/chiefgram/chiefmod/types/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/types/identifier.py
+-rw-r--r--   0 root         (0) root         (0)      402 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/types/listener.py
+-rw-r--r--   0 root         (0) root         (0)      113 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/types/listener_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.807878 chiefgram-4.0/chiefgram/chiefmod/utils/
+-rw-r--r--   0 root         (0) root         (0)      859 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/chiefmod/utils/patch.py
+-rw-r--r--   0 root         (0) root         (0)    40500 2024-04-12 03:01:36.000000 chiefgram-4.0/chiefgram/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.807878 chiefgram-4.0/chiefgram/connection/
+-rw-r--r--   0 root         (0) root         (0)      858 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.807878 chiefgram-4.0/chiefgram/connection/transport/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/transport/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.807878 chiefgram-4.0/chiefgram/connection/transport/tcp/
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4093 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.811878 chiefgram-4.0/chiefgram/crypto/
+-rw-r--r--   0 root         (0) root         (0)      823 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4013 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/crypto/aes.py
+-rw-r--r--   0 root         (0) root         (0)     4025 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/crypto/mtproto.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/crypto/prime.py
+-rw-r--r--   0 root         (0) root         (0)    13442 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/crypto/rsa.py
+-rw-r--r--   0 root         (0) root         (0)    10075 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)   208025 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/emoji.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.811878 chiefgram-4.0/chiefgram/enums/
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/auto_name.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4209 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/chat_event_action.py
+-rw-r--r--   0 root         (0) root         (0)     1271 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/chat_member_status.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/chat_members_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/chat_type.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/message_entity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/message_media_type.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/message_service_type.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/messages_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/next_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/parse_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/poll_type.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/sent_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/enums/user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.815878 chiefgram-4.0/chiefgram/errors/
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/errors/rpc_error.py
+-rw-r--r--   0 root         (0) root         (0)    15160 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/file_id.py
+-rw-r--r--   0 root         (0) root         (0)    24874 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.815878 chiefgram-4.0/chiefgram/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1480 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/callback_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/disconnect_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/edited_message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/handler.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/inline_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/poll_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/raw_update_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/handlers/user_status_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.815878 chiefgram-4.0/chiefgram/methods/
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.815878 chiefgram-4.0/chiefgram/methods/advanced/
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/advanced/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/advanced/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 root         (0) root         (0)     8432 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/advanced/save_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.819878 chiefgram-4.0/chiefgram/methods/auth/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/check_password.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/connect.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/get_password_hint.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2024-04-12 03:08:17.000000 chiefgram-4.0/chiefgram/methods/auth/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/log_out.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/recover_password.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/resend_code.py
+-rw-r--r--   0 root         (0) root         (0)     2798 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/send_code.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/sign_in.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/auth/sign_up.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-04-12 03:08:17.000000 chiefgram-4.0/chiefgram/methods/auth/terminate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.823878 chiefgram-4.0/chiefgram/methods/bots/
+-rw-r--r--   0 root         (0) root         (0)     2046 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     5001 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/send_game.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/bots/set_game_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.831878 chiefgram-4.0/chiefgram/methods/chats/
+-rw-r--r--   0 root         (0) root         (0)     3444 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/add_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/archive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     4630 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/create_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/create_group.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/create_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/delete_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/delete_user_history.py
+-rw-r--r--   0 root         (0) root         (0)     3295 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_chat.py
+-rw-r--r--   0 root         (0) root         (0)     4043 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 root         (0) root         (0)     3349 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2706 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/join_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/leave_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     4324 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/set_chat_description.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 root         (0) root         (0)     2580 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/set_chat_title.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/set_chat_username.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.835877 chiefgram-4.0/chiefgram/methods/contacts/
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/contacts/add_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/contacts/get_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.835877 chiefgram-4.0/chiefgram/methods/decorators/
+-rw-r--r--   0 root         (0) root         (0)     1629 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_message.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_poll.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.839877 chiefgram-4.0/chiefgram/methods/invite_links/
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     3380 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1933 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3543 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     2343 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.851877 chiefgram-4.0/chiefgram/methods/messages/
+-rw-r--r--   0 root         (0) root         (0)     3926 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5972 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/copy_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     5194 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/copy_message.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/delete_messages.py
+-rw-r--r--   0 root         (0) root         (0)     7541 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/download_media.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 root         (0) root         (0)    10390 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 root         (0) root         (0)     2990 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 root         (0) root         (0)    13037 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/edit_message_media.py
+-rw-r--r--   0 root         (0) root         (0)     2988 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/forward_messages.py
+-rw-r--r--   0 root         (0) root         (0)     4051 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/get_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/get_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/get_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/inline_session.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/read_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/retract_vote.py
+-rw-r--r--   0 root         (0) root         (0)     4176 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/search_global.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/search_global_count.py
+-rw-r--r--   0 root         (0) root         (0)     5361 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/search_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/search_messages_count.py
+-rw-r--r--   0 root         (0) root         (0)    12605 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_animation.py
+-rw-r--r--   0 root         (0) root         (0)    11140 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_audio.py
+-rw-r--r--   0 root         (0) root         (0)     5496 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_cached_media.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_contact.py
+-rw-r--r--   0 root         (0) root         (0)     4855 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_dice.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_document.py
+-rw-r--r--   0 root         (0) root         (0)     4590 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_location.py
+-rw-r--r--   0 root         (0) root         (0)    19923 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     7285 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_message.py
+-rw-r--r--   0 root         (0) root         (0)     9459 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_photo.py
+-rw-r--r--   0 root         (0) root         (0)     8091 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     8357 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     5411 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_venue.py
+-rw-r--r--   0 root         (0) root         (0)    11975 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_video.py
+-rw-r--r--   0 root         (0) root         (0)     9331 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_video_note.py
+-rw-r--r--   0 root         (0) root         (0)     9449 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/send_voice.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/stop_poll.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/stream_media.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/messages/vote_poll.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.851877 chiefgram-4.0/chiefgram/methods/password/
+-rw-r--r--   0 root         (0) root         (0)     1093 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/password/change_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.855877 chiefgram-4.0/chiefgram/methods/users/
+-rw-r--r--   0 root         (0) root         (0)     1664 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/block_user.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 root         (0) root         (0)     4430 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/get_chat_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/get_common_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/get_me.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/get_users.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/set_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/set_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/set_username.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/unblock_user.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/users/update_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.855877 chiefgram-4.0/chiefgram/methods/utilities/
+-rw-r--r--   0 root         (0) root         (0)     1258 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/add_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/compose.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/export_session_string.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/idle.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/remove_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/restart.py
+-rw-r--r--   0 root         (0) root         (0)     2872 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/run.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/start.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/stop.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 root         (0) root         (0)    61920 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/mime_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.859877 chiefgram-4.0/chiefgram/parser/
+-rw-r--r--   0 root         (0) root         (0)      851 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8695 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/parser/html.py
+-rw-r--r--   0 root         (0) root         (0)     5778 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/parser/markdown.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.859877 chiefgram-4.0/chiefgram/raw/
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.859877 chiefgram-4.0/chiefgram/raw/core/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/future_salt.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/future_salts.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/gzip_packed.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/list.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/msg_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.863877 chiefgram-4.0/chiefgram/raw/core/primitives/
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/primitives/bool.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/primitives/bytes.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/primitives/double.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/primitives/int.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/primitives/string.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/primitives/vector.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/raw/core/tl_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.863877 chiefgram-4.0/chiefgram/session/
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/session/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11458 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/session/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.867877 chiefgram-4.0/chiefgram/session/internals/
+-rw-r--r--   0 root         (0) root         (0)      922 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/session/internals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/session/internals/data_center.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/session/internals/msg_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1161 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/session/internals/msg_id.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/session/internals/seq_no.py
+-rw-r--r--   0 root         (0) root         (0)    13434 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/session/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.871877 chiefgram-4.0/chiefgram/storage/
+-rw-r--r--   0 root         (0) root         (0)      932 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/storage/file_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2754 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/storage/memory_storage.py
+-rw-r--r--   0 root         (0) root         (0)     6229 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/storage/storage.py
+-rw-r--r--   0 root         (0) root         (0)     3747 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.871877 chiefgram-4.0/chiefgram/types/
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.871877 chiefgram-4.0/chiefgram/types/authorization/
+-rw-r--r--   0 root         (0) root         (0)      943 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/authorization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/authorization/sent_code.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.875877 chiefgram-4.0/chiefgram/types/bots_and_keyboards/
+-rw-r--r--   0 root         (0) root         (0)     2835 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 root         (0) root         (0)     2803 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 root         (0) root         (0)     8133 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     1217 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 root         (0) root         (0)     4585 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.883877 chiefgram-4.0/chiefgram/types/inline_mode/
+-rw-r--r--   0 root         (0) root         (0)     2760 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     7313 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 root         (0) root         (0)     5788 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 root         (0) root         (0)     4517 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 root         (0) root         (0)     4041 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 root         (0) root         (0)     4324 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3041 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 root         (0) root         (0)     4214 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 root         (0) root         (0)     4142 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     4629 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 root         (0) root         (0)     5273 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 root         (0) root         (0)     5486 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 root         (0) root         (0)     4372 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.883877 chiefgram-4.0/chiefgram/types/input_media/
+-rw-r--r--   0 root         (0) root         (0)     1319 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_media/input_media.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_media/input_media_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_media/input_media_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_media/input_media_document.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_media/input_media_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3628 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_media/input_media_video.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.883877 chiefgram-4.0/chiefgram/types/input_message_content/
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_message_content/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.891877 chiefgram-4.0/chiefgram/types/messages_and_media/
+-rw-r--r--   0 root         (0) root         (0)     1841 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4055 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/animation.py
+-rw-r--r--   0 root         (0) root         (0)     4080 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/audio.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/contact.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/dice.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/document.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/game.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/location.py
+-rw-r--r--   0 root         (0) root         (0)   144740 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/message.py
+-rw-r--r--   0 root         (0) root         (0)     4367 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/photo.py
+-rw-r--r--   0 root         (0) root         (0)     7049 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/poll.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/reaction.py
+-rw-r--r--   0 root         (0) root         (0)     6921 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/sticker.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/venue.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/video.py
+-rw-r--r--   0 root         (0) root         (0)     3612 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/video_note.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/voice.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 root         (0) root         (0)     6365 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/messages_and_media/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/object.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.895877 chiefgram-4.0/chiefgram/types/user_and_chats/
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32619 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)    19882 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 root         (0) root         (0)     5520 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4589 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     4260 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 root         (0) root         (0)     9461 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3689 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     4388 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3976 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 root         (0) root         (0)     4957 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/dialog.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/restriction.py
+-rw-r--r--   0 root         (0) root         (0)    12857 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/user.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 root         (0) root         (0)    10582 2024-04-12 02:13:07.000000 chiefgram-4.0/chiefgram/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.899876 chiefgram-4.0/chiefgram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      370 2024-04-12 03:08:58.000000 chiefgram-4.0/chiefgram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19905 2024-04-12 03:08:58.000000 chiefgram-4.0/chiefgram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 03:08:58.000000 chiefgram-4.0/chiefgram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 03:08:58.000000 chiefgram-4.0/chiefgram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-12 03:08:58.000000 chiefgram-4.0/chiefgram.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.895877 chiefgram-4.0/compiler/
+-rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.895877 chiefgram-4.0/compiler/api/
+-rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22426 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/api/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.895877 chiefgram-4.0/compiler/api/source/
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/api/source/auth_key.tl
+-rw-r--r--   0 root         (0) root         (0)   168867 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/api/source/main_api.tl
+-rw-r--r--   0 root         (0) root         (0)     3425 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.895877 chiefgram-4.0/compiler/api/template/
+-rw-r--r--   0 root         (0) root         (0)      746 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/api/template/combinator.txt
+-rw-r--r--   0 root         (0) root         (0)      639 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/api/template/type.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.895877 chiefgram-4.0/compiler/errors/
+-rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.899876 chiefgram-4.0/compiler/errors/source/
+-rw-r--r--   0 root         (0) root         (0)      470 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 root         (0) root         (0)    22642 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 root         (0) root         (0)      678 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 root         (0) root         (0)     2000 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 root         (0) root         (0)      470 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 root         (0) root         (0)      155 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.899876 chiefgram-4.0/compiler/errors/template/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/template/class.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2024-04-12 02:13:07.000000 chiefgram-4.0/compiler/errors/template/sub_class.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 02:13:07.000000 chiefgram-4.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 03:08:58.899876 chiefgram-4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      667 2024-04-12 03:08:49.000000 chiefgram-4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.899876 chiefgram-4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-4.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.899876 chiefgram-4.0/tests/filters/
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-04-12 02:13:07.000000 chiefgram-4.0/tests/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-12 02:13:07.000000 chiefgram-4.0/tests/filters/test_command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:08:58.899876 chiefgram-4.0/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)      824 2024-04-12 02:13:07.000000 chiefgram-4.0/tests/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6329 2024-04-12 02:13:07.000000 chiefgram-4.0/tests/parser/test_html.py
+-rw-r--r--   0 root         (0) root         (0)     8215 2024-04-12 02:13:07.000000 chiefgram-4.0/tests/test_file_id.py
```

### Comparing `chiefgram-3.5/README.md` & `chiefgram-4.0/README.md`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/__init__.py` & `chiefgram-4.0/chiefgram/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/__init__.py` & `chiefgram-4.0/chiefgram/chiefmod/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/helpers/__init__.py` & `chiefgram-4.0/chiefgram/chiefmod/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/helpers/helpers.py` & `chiefgram-4.0/chiefgram/chiefmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/listen/__init__.py` & `chiefgram-4.0/chiefgram/chiefmod/listen/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/listen/callback_query_handler.py` & `chiefgram-4.0/chiefgram/chiefmod/listen/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/listen/chat.py` & `chiefgram-4.0/chiefgram/chiefmod/listen/chat.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/listen/client.py` & `chiefgram-4.0/chiefgram/chiefmod/listen/client.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/listen/message.py` & `chiefgram-4.0/chiefgram/chiefmod/listen/message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/listen/message_handler.py` & `chiefgram-4.0/chiefgram/chiefmod/listen/message_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/listen/user.py` & `chiefgram-4.0/chiefgram/chiefmod/listen/user.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/nav/__init__.py` & `chiefgram-4.0/chiefgram/chiefmod/nav/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/nav/pagination.py` & `chiefgram-4.0/chiefgram/chiefmod/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/types/identifier.py` & `chiefgram-4.0/chiefgram/chiefmod/types/identifier.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/utils/__init__.py` & `chiefgram-4.0/chiefgram/chiefmod/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/chiefmod/utils/patch.py` & `chiefgram-4.0/chiefgram/chiefmod/utils/patch.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/client.py` & `chiefgram-4.0/chiefgram/client.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/__init__.py` & `chiefgram-4.0/chiefgram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/connection.py` & `chiefgram-4.0/chiefgram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/transport/__init__.py` & `chiefgram-4.0/chiefgram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/transport/tcp/__init__.py` & `chiefgram-4.0/chiefgram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/transport/tcp/tcp.py` & `chiefgram-4.0/chiefgram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_abridged.py` & `chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_abridged_o.py` & `chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_full.py` & `chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_intermediate.py` & `chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/connection/transport/tcp/tcp_intermediate_o.py` & `chiefgram-4.0/chiefgram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/crypto/__init__.py` & `chiefgram-4.0/chiefgram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/crypto/aes.py` & `chiefgram-4.0/chiefgram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/crypto/mtproto.py` & `chiefgram-4.0/chiefgram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/crypto/prime.py` & `chiefgram-4.0/chiefgram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/crypto/rsa.py` & `chiefgram-4.0/chiefgram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/dispatcher.py` & `chiefgram-4.0/chiefgram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/emoji.py` & `chiefgram-4.0/chiefgram/emoji.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/__init__.py` & `chiefgram-4.0/chiefgram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/auto_name.py` & `chiefgram-4.0/chiefgram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/chat_action.py` & `chiefgram-4.0/chiefgram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/chat_event_action.py` & `chiefgram-4.0/chiefgram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/chat_member_status.py` & `chiefgram-4.0/chiefgram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/chat_members_filter.py` & `chiefgram-4.0/chiefgram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/chat_type.py` & `chiefgram-4.0/chiefgram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/message_entity_type.py` & `chiefgram-4.0/chiefgram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/message_media_type.py` & `chiefgram-4.0/chiefgram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/message_service_type.py` & `chiefgram-4.0/chiefgram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/messages_filter.py` & `chiefgram-4.0/chiefgram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/next_code_type.py` & `chiefgram-4.0/chiefgram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/parse_mode.py` & `chiefgram-4.0/chiefgram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/poll_type.py` & `chiefgram-4.0/chiefgram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/sent_code_type.py` & `chiefgram-4.0/chiefgram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/enums/user_status.py` & `chiefgram-4.0/chiefgram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/errors/__init__.py` & `chiefgram-4.0/chiefgram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/errors/rpc_error.py` & `chiefgram-4.0/chiefgram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/file_id.py` & `chiefgram-4.0/chiefgram/file_id.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/filters.py` & `chiefgram-4.0/chiefgram/filters.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/__init__.py` & `chiefgram-4.0/chiefgram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/callback_query_handler.py` & `chiefgram-4.0/chiefgram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/chat_join_request_handler.py` & `chiefgram-4.0/chiefgram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/chat_member_updated_handler.py` & `chiefgram-4.0/chiefgram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/chosen_inline_result_handler.py` & `chiefgram-4.0/chiefgram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/deleted_messages_handler.py` & `chiefgram-4.0/chiefgram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/disconnect_handler.py` & `chiefgram-4.0/chiefgram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/edited_message_handler.py` & `chiefgram-4.0/chiefgram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/handler.py` & `chiefgram-4.0/chiefgram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/inline_query_handler.py` & `chiefgram-4.0/chiefgram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/message_handler.py` & `chiefgram-4.0/chiefgram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/poll_handler.py` & `chiefgram-4.0/chiefgram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/raw_update_handler.py` & `chiefgram-4.0/chiefgram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/handlers/user_status_handler.py` & `chiefgram-4.0/chiefgram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/__init__.py` & `chiefgram-4.0/chiefgram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/advanced/__init__.py` & `chiefgram-4.0/chiefgram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/advanced/invoke.py` & `chiefgram-4.0/chiefgram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/advanced/resolve_peer.py` & `chiefgram-4.0/chiefgram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/advanced/save_file.py` & `chiefgram-4.0/chiefgram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/__init__.py` & `chiefgram-4.0/chiefgram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/accept_terms_of_service.py` & `chiefgram-4.0/chiefgram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/check_password.py` & `chiefgram-4.0/chiefgram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/connect.py` & `chiefgram-4.0/chiefgram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/disconnect.py` & `chiefgram-4.0/chiefgram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/get_password_hint.py` & `chiefgram-4.0/chiefgram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/initialize.py` & `chiefgram-4.0/chiefgram/methods/auth/initialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,10 +43,8 @@
         if self.is_initialized:
             raise ConnectionError("Client is already initialized")
 
         self.load_plugins()
 
         await self.dispatcher.start()
 
-        self.updates_watchdog_task = asyncio.create_task(self.updates_watchdog())
-
         self.is_initialized = True
```

### Comparing `chiefgram-3.5/chiefgram/methods/auth/log_out.py` & `chiefgram-4.0/chiefgram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/recover_password.py` & `chiefgram-4.0/chiefgram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/resend_code.py` & `chiefgram-4.0/chiefgram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/send_code.py` & `chiefgram-4.0/chiefgram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/send_recovery_code.py` & `chiefgram-4.0/chiefgram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/sign_in.py` & `chiefgram-4.0/chiefgram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/sign_in_bot.py` & `chiefgram-4.0/chiefgram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/sign_up.py` & `chiefgram-4.0/chiefgram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/auth/terminate.py` & `chiefgram-4.0/chiefgram/methods/auth/terminate.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,15 +47,8 @@
         await self.dispatcher.stop()
 
         for media_session in self.media_sessions.values():
             await media_session.stop()
 
         self.media_sessions.clear()
 
-        self.updates_watchdog_event.set()
-
-        if self.updates_watchdog_task is not None:
-            await self.updates_watchdog_task
-
-        self.updates_watchdog_event.clear()
-
         self.is_initialized = False
```

### Comparing `chiefgram-3.5/chiefgram/methods/bots/__init__.py` & `chiefgram-4.0/chiefgram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/answer_callback_query.py` & `chiefgram-4.0/chiefgram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/answer_inline_query.py` & `chiefgram-4.0/chiefgram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/answer_web_app_query.py` & `chiefgram-4.0/chiefgram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/delete_bot_commands.py` & `chiefgram-4.0/chiefgram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/get_bot_commands.py` & `chiefgram-4.0/chiefgram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/get_bot_default_privileges.py` & `chiefgram-4.0/chiefgram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/get_chat_menu_button.py` & `chiefgram-4.0/chiefgram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/get_game_high_scores.py` & `chiefgram-4.0/chiefgram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/get_inline_bot_results.py` & `chiefgram-4.0/chiefgram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/request_callback_answer.py` & `chiefgram-4.0/chiefgram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/send_game.py` & `chiefgram-4.0/chiefgram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/send_inline_bot_result.py` & `chiefgram-4.0/chiefgram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/set_bot_commands.py` & `chiefgram-4.0/chiefgram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/set_bot_default_privileges.py` & `chiefgram-4.0/chiefgram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/set_chat_menu_button.py` & `chiefgram-4.0/chiefgram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/bots/set_game_score.py` & `chiefgram-4.0/chiefgram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/__init__.py` & `chiefgram-4.0/chiefgram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/add_chat_members.py` & `chiefgram-4.0/chiefgram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/archive_chats.py` & `chiefgram-4.0/chiefgram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/ban_chat_member.py` & `chiefgram-4.0/chiefgram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/create_channel.py` & `chiefgram-4.0/chiefgram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/create_group.py` & `chiefgram-4.0/chiefgram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/create_supergroup.py` & `chiefgram-4.0/chiefgram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/delete_channel.py` & `chiefgram-4.0/chiefgram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/delete_chat_photo.py` & `chiefgram-4.0/chiefgram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/delete_supergroup.py` & `chiefgram-4.0/chiefgram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/delete_user_history.py` & `chiefgram-4.0/chiefgram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_chat.py` & `chiefgram-4.0/chiefgram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_chat_event_log.py` & `chiefgram-4.0/chiefgram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_chat_member.py` & `chiefgram-4.0/chiefgram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_chat_members.py` & `chiefgram-4.0/chiefgram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_chat_members_count.py` & `chiefgram-4.0/chiefgram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_chat_online_count.py` & `chiefgram-4.0/chiefgram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_dialogs.py` & `chiefgram-4.0/chiefgram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_dialogs_count.py` & `chiefgram-4.0/chiefgram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_nearby_chats.py` & `chiefgram-4.0/chiefgram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/get_send_as_chats.py` & `chiefgram-4.0/chiefgram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/join_chat.py` & `chiefgram-4.0/chiefgram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/leave_chat.py` & `chiefgram-4.0/chiefgram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/mark_chat_unread.py` & `chiefgram-4.0/chiefgram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/pin_chat_message.py` & `chiefgram-4.0/chiefgram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/promote_chat_member.py` & `chiefgram-4.0/chiefgram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/restrict_chat_member.py` & `chiefgram-4.0/chiefgram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/set_administrator_title.py` & `chiefgram-4.0/chiefgram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/set_chat_description.py` & `chiefgram-4.0/chiefgram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/set_chat_permissions.py` & `chiefgram-4.0/chiefgram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/set_chat_photo.py` & `chiefgram-4.0/chiefgram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/set_chat_protected_content.py` & `chiefgram-4.0/chiefgram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/set_chat_title.py` & `chiefgram-4.0/chiefgram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/set_chat_username.py` & `chiefgram-4.0/chiefgram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/set_send_as_chat.py` & `chiefgram-4.0/chiefgram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/set_slow_mode.py` & `chiefgram-4.0/chiefgram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/unarchive_chats.py` & `chiefgram-4.0/chiefgram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/unban_chat_member.py` & `chiefgram-4.0/chiefgram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/unpin_all_chat_messages.py` & `chiefgram-4.0/chiefgram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/chats/unpin_chat_message.py` & `chiefgram-4.0/chiefgram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/contacts/__init__.py` & `chiefgram-4.0/chiefgram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/contacts/add_contact.py` & `chiefgram-4.0/chiefgram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/contacts/delete_contacts.py` & `chiefgram-4.0/chiefgram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/contacts/get_contacts.py` & `chiefgram-4.0/chiefgram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/contacts/get_contacts_count.py` & `chiefgram-4.0/chiefgram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/contacts/import_contacts.py` & `chiefgram-4.0/chiefgram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/__init__.py` & `chiefgram-4.0/chiefgram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_callback_query.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_chat_join_request.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_chat_member_updated.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_chosen_inline_result.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_deleted_messages.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_disconnect.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_edited_message.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_inline_query.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_message.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_poll.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_raw_update.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/decorators/on_user_status.py` & `chiefgram-4.0/chiefgram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/__init__.py` & `chiefgram-4.0/chiefgram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/approve_all_chat_join_requests.py` & `chiefgram-4.0/chiefgram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/approve_chat_join_request.py` & `chiefgram-4.0/chiefgram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/create_chat_invite_link.py` & `chiefgram-4.0/chiefgram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/decline_all_chat_join_requests.py` & `chiefgram-4.0/chiefgram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/decline_chat_join_request.py` & `chiefgram-4.0/chiefgram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/delete_chat_admin_invite_links.py` & `chiefgram-4.0/chiefgram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/delete_chat_invite_link.py` & `chiefgram-4.0/chiefgram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/edit_chat_invite_link.py` & `chiefgram-4.0/chiefgram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/export_chat_invite_link.py` & `chiefgram-4.0/chiefgram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/get_chat_admin_invite_links.py` & `chiefgram-4.0/chiefgram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/get_chat_admin_invite_links_count.py` & `chiefgram-4.0/chiefgram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/get_chat_admins_with_invite_links.py` & `chiefgram-4.0/chiefgram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/get_chat_invite_link.py` & `chiefgram-4.0/chiefgram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/get_chat_invite_link_joiners.py` & `chiefgram-4.0/chiefgram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `chiefgram-4.0/chiefgram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/get_chat_join_requests.py` & `chiefgram-4.0/chiefgram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/invite_links/revoke_chat_invite_link.py` & `chiefgram-4.0/chiefgram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/__init__.py` & `chiefgram-4.0/chiefgram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/copy_media_group.py` & `chiefgram-4.0/chiefgram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/copy_message.py` & `chiefgram-4.0/chiefgram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/delete_messages.py` & `chiefgram-4.0/chiefgram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/download_media.py` & `chiefgram-4.0/chiefgram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/edit_inline_caption.py` & `chiefgram-4.0/chiefgram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/edit_inline_media.py` & `chiefgram-4.0/chiefgram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/edit_inline_reply_markup.py` & `chiefgram-4.0/chiefgram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/edit_inline_text.py` & `chiefgram-4.0/chiefgram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/edit_message_caption.py` & `chiefgram-4.0/chiefgram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/edit_message_media.py` & `chiefgram-4.0/chiefgram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/edit_message_reply_markup.py` & `chiefgram-4.0/chiefgram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/edit_message_text.py` & `chiefgram-4.0/chiefgram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/forward_messages.py` & `chiefgram-4.0/chiefgram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/get_chat_history.py` & `chiefgram-4.0/chiefgram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/get_chat_history_count.py` & `chiefgram-4.0/chiefgram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/get_custom_emoji_stickers.py` & `chiefgram-4.0/chiefgram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/get_discussion_message.py` & `chiefgram-4.0/chiefgram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/get_discussion_replies.py` & `chiefgram-4.0/chiefgram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/get_discussion_replies_count.py` & `chiefgram-4.0/chiefgram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/get_media_group.py` & `chiefgram-4.0/chiefgram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/get_messages.py` & `chiefgram-4.0/chiefgram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/inline_session.py` & `chiefgram-4.0/chiefgram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/read_chat_history.py` & `chiefgram-4.0/chiefgram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/retract_vote.py` & `chiefgram-4.0/chiefgram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/search_global.py` & `chiefgram-4.0/chiefgram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/search_global_count.py` & `chiefgram-4.0/chiefgram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/search_messages.py` & `chiefgram-4.0/chiefgram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/search_messages_count.py` & `chiefgram-4.0/chiefgram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_animation.py` & `chiefgram-4.0/chiefgram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_audio.py` & `chiefgram-4.0/chiefgram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_cached_media.py` & `chiefgram-4.0/chiefgram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_chat_action.py` & `chiefgram-4.0/chiefgram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_contact.py` & `chiefgram-4.0/chiefgram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_dice.py` & `chiefgram-4.0/chiefgram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_document.py` & `chiefgram-4.0/chiefgram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_location.py` & `chiefgram-4.0/chiefgram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_media_group.py` & `chiefgram-4.0/chiefgram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_message.py` & `chiefgram-4.0/chiefgram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_photo.py` & `chiefgram-4.0/chiefgram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_poll.py` & `chiefgram-4.0/chiefgram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_reaction.py` & `chiefgram-4.0/chiefgram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_sticker.py` & `chiefgram-4.0/chiefgram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_venue.py` & `chiefgram-4.0/chiefgram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_video.py` & `chiefgram-4.0/chiefgram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_video_note.py` & `chiefgram-4.0/chiefgram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/send_voice.py` & `chiefgram-4.0/chiefgram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/stop_poll.py` & `chiefgram-4.0/chiefgram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/stream_media.py` & `chiefgram-4.0/chiefgram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/messages/vote_poll.py` & `chiefgram-4.0/chiefgram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/password/__init__.py` & `chiefgram-4.0/chiefgram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/password/change_cloud_password.py` & `chiefgram-4.0/chiefgram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/password/enable_cloud_password.py` & `chiefgram-4.0/chiefgram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/password/remove_cloud_password.py` & `chiefgram-4.0/chiefgram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/__init__.py` & `chiefgram-4.0/chiefgram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/block_user.py` & `chiefgram-4.0/chiefgram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/delete_profile_photos.py` & `chiefgram-4.0/chiefgram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/get_chat_photos.py` & `chiefgram-4.0/chiefgram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/get_chat_photos_count.py` & `chiefgram-4.0/chiefgram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/get_common_chats.py` & `chiefgram-4.0/chiefgram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/get_default_emoji_statuses.py` & `chiefgram-4.0/chiefgram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/get_me.py` & `chiefgram-4.0/chiefgram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/get_users.py` & `chiefgram-4.0/chiefgram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/set_emoji_status.py` & `chiefgram-4.0/chiefgram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/set_profile_photo.py` & `chiefgram-4.0/chiefgram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/set_username.py` & `chiefgram-4.0/chiefgram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/unblock_user.py` & `chiefgram-4.0/chiefgram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/users/update_profile.py` & `chiefgram-4.0/chiefgram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/__init__.py` & `chiefgram-4.0/chiefgram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/add_handler.py` & `chiefgram-4.0/chiefgram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/compose.py` & `chiefgram-4.0/chiefgram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/export_session_string.py` & `chiefgram-4.0/chiefgram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/idle.py` & `chiefgram-4.0/chiefgram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/remove_handler.py` & `chiefgram-4.0/chiefgram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/restart.py` & `chiefgram-4.0/chiefgram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/run.py` & `chiefgram-4.0/chiefgram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/start.py` & `chiefgram-4.0/chiefgram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/stop.py` & `chiefgram-4.0/chiefgram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/methods/utilities/stop_transmission.py` & `chiefgram-4.0/chiefgram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/mime_types.py` & `chiefgram-4.0/chiefgram/mime_types.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/parser/__init__.py` & `chiefgram-4.0/chiefgram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/parser/html.py` & `chiefgram-4.0/chiefgram/parser/html.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/parser/markdown.py` & `chiefgram-4.0/chiefgram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/parser/parser.py` & `chiefgram-4.0/chiefgram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/parser/utils.py` & `chiefgram-4.0/chiefgram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/__init__.py` & `chiefgram-4.0/chiefgram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/__init__.py` & `chiefgram-4.0/chiefgram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/future_salt.py` & `chiefgram-4.0/chiefgram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/future_salts.py` & `chiefgram-4.0/chiefgram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/gzip_packed.py` & `chiefgram-4.0/chiefgram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/list.py` & `chiefgram-4.0/chiefgram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/message.py` & `chiefgram-4.0/chiefgram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/msg_container.py` & `chiefgram-4.0/chiefgram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/primitives/__init__.py` & `chiefgram-4.0/chiefgram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/primitives/bool.py` & `chiefgram-4.0/chiefgram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/primitives/bytes.py` & `chiefgram-4.0/chiefgram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/primitives/double.py` & `chiefgram-4.0/chiefgram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/primitives/int.py` & `chiefgram-4.0/chiefgram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/primitives/string.py` & `chiefgram-4.0/chiefgram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/primitives/vector.py` & `chiefgram-4.0/chiefgram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/raw/core/tl_object.py` & `chiefgram-4.0/chiefgram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/session/__init__.py` & `chiefgram-4.0/chiefgram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/session/auth.py` & `chiefgram-4.0/chiefgram/session/auth.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/session/internals/__init__.py` & `chiefgram-4.0/chiefgram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/session/internals/data_center.py` & `chiefgram-4.0/chiefgram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/session/internals/msg_factory.py` & `chiefgram-4.0/chiefgram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/session/internals/msg_id.py` & `chiefgram-4.0/chiefgram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/session/internals/seq_no.py` & `chiefgram-4.0/chiefgram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/session/session.py` & `chiefgram-4.0/chiefgram/session/session.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/storage/__init__.py` & `chiefgram-4.0/chiefgram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/storage/file_storage.py` & `chiefgram-4.0/chiefgram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/storage/memory_storage.py` & `chiefgram-4.0/chiefgram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/storage/sqlite_storage.py` & `chiefgram-4.0/chiefgram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/storage/storage.py` & `chiefgram-4.0/chiefgram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/sync.py` & `chiefgram-4.0/chiefgram/sync.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/__init__.py` & `chiefgram-4.0/chiefgram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/authorization/__init__.py` & `chiefgram-4.0/chiefgram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/authorization/sent_code.py` & `chiefgram-4.0/chiefgram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/authorization/terms_of_service.py` & `chiefgram-4.0/chiefgram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/__init__.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_chat.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/bot_command_scope_default.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/callback_game.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/callback_query.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/force_reply.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/game_high_score.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/inline_keyboard_button.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/inline_keyboard_markup.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/keyboard_button.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/login_url.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/menu_button.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/menu_button_commands.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/menu_button_default.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/menu_button_web_app.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/reply_keyboard_markup.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/reply_keyboard_remove.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/sent_web_app_message.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/bots_and_keyboards/web_app_info.py` & `chiefgram-4.0/chiefgram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/__init__.py` & `chiefgram-4.0/chiefgram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/chosen_inline_result.py` & `chiefgram-4.0/chiefgram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_animation.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_article.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_audio.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_animation.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_audio.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_document.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_photo.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_sticker.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_video.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_cached_voice.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_contact.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_document.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_location.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_photo.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_venue.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_video.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/inline_mode/inline_query_result_voice.py` & `chiefgram-4.0/chiefgram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_media/__init__.py` & `chiefgram-4.0/chiefgram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_media/input_media.py` & `chiefgram-4.0/chiefgram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_media/input_media_animation.py` & `chiefgram-4.0/chiefgram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_media/input_media_audio.py` & `chiefgram-4.0/chiefgram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_media/input_media_document.py` & `chiefgram-4.0/chiefgram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_media/input_media_photo.py` & `chiefgram-4.0/chiefgram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_media/input_media_video.py` & `chiefgram-4.0/chiefgram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_media/input_phone_contact.py` & `chiefgram-4.0/chiefgram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_message_content/__init__.py` & `chiefgram-4.0/chiefgram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_message_content/input_message_content.py` & `chiefgram-4.0/chiefgram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/input_message_content/input_text_message_content.py` & `chiefgram-4.0/chiefgram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/list.py` & `chiefgram-4.0/chiefgram/types/list.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/__init__.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/animation.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/audio.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/contact.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/dice.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/document.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/game.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/location.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/message.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/message_entity.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/message_reactions.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/photo.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/poll.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/poll_option.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/reaction.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/sticker.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/stripped_thumbnail.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/thumbnail.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/venue.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/video.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/video_note.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/voice.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/web_app_data.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/messages_and_media/web_page.py` & `chiefgram-4.0/chiefgram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/object.py` & `chiefgram-4.0/chiefgram/types/object.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/update.py` & `chiefgram-4.0/chiefgram/types/update.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/__init__.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_admin_with_invite_links.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_event.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_event_filter.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_invite_link.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_join_request.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_joiner.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_member.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_member_updated.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_permissions.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_photo.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_preview.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_privileges.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/chat_reactions.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/dialog.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/emoji_status.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/invite_link_importer.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/restriction.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/user.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/video_chat_ended.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/video_chat_members_invited.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/video_chat_scheduled.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/types/user_and_chats/video_chat_started.py` & `chiefgram-4.0/chiefgram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram/utils.py` & `chiefgram-4.0/chiefgram/utils.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/chiefgram.egg-info/SOURCES.txt` & `chiefgram-4.0/chiefgram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/__init__.py` & `chiefgram-4.0/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/api/__init__.py` & `chiefgram-4.0/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/api/compiler.py` & `chiefgram-4.0/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/api/source/auth_key.tl` & `chiefgram-4.0/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/api/source/main_api.tl` & `chiefgram-4.0/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/api/source/sys_msgs.tl` & `chiefgram-4.0/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/api/template/combinator.txt` & `chiefgram-4.0/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/api/template/type.txt` & `chiefgram-4.0/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/errors/__init__.py` & `chiefgram-4.0/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/errors/compiler.py` & `chiefgram-4.0/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/errors/sort.py` & `chiefgram-4.0/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/errors/source/400_BAD_REQUEST.tsv` & `chiefgram-4.0/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/errors/source/401_UNAUTHORIZED.tsv` & `chiefgram-4.0/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/errors/source/403_FORBIDDEN.tsv` & `chiefgram-4.0/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `chiefgram-4.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `chiefgram-4.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/setup.py` & `chiefgram-4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Membaca isi dari requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='chiefgram',
-    version='3.5',
+    version='4.0',
     packages=find_packages(),
     description='Hanya Buat Senang',
     author='GatauTeh',
     author_email='rizaldaitona@gmail.com',
     url='https://example.com',  # Ganti dengan URL proyek Anda
     classifiers=[
         'Programming Language :: Python :: 3.10',
```

### Comparing `chiefgram-3.5/tests/__init__.py` & `chiefgram-4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/tests/filters/__init__.py` & `chiefgram-4.0/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/tests/filters/test_command.py` & `chiefgram-4.0/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/tests/parser/__init__.py` & `chiefgram-4.0/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/tests/parser/test_html.py` & `chiefgram-4.0/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `chiefgram-3.5/tests/test_file_id.py` & `chiefgram-4.0/tests/test_file_id.py`

 * *Files identical despite different names*

