# Comparing `tmp/pybotx-0.65.0.tar.gz` & `tmp/pybotx-0.66.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotx-0.65.0.tar", max compression
+gzip compressed data, was "pybotx-0.66.0.tar", max compression
```

## Comparing `pybotx-0.65.0.tar` & `pybotx-0.66.0.tar`

### file list

```diff
@@ -1,141 +1,142 @@
--rw-r--r--   0        0        0     6078 2024-03-26 07:09:06.095389 pybotx-0.65.0/LICENSE
--rw-r--r--   0        0        0    24106 2024-03-26 07:09:06.095389 pybotx-0.65.0/README.md
--rw-r--r--   0        0        0     7254 2024-03-26 07:09:06.095389 pybotx-0.65.0/pybotx/__init__.py
--rw-r--r--   0        0        0      847 2024-03-26 07:09:06.095389 pybotx-0.65.0/pybotx/async_buffer.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.095389 pybotx-0.65.0/pybotx/bot/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.095389 pybotx-0.65.0/pybotx/bot/api/__init__.py
--rw-r--r--   0        0        0      560 2024-03-26 07:09:06.095389 pybotx-0.65.0/pybotx/bot/api/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.095389 pybotx-0.65.0/pybotx/bot/api/responses/__init__.py
--rw-r--r--   0        0        0     1048 2024-03-26 07:09:06.095389 pybotx-0.65.0/pybotx/bot/api/responses/bot_disabled.py
--rw-r--r--   0        0        0      275 2024-03-26 07:09:06.095389 pybotx-0.65.0/pybotx/bot/api/responses/command_accepted.py
--rw-r--r--   0        0        0     1185 2024-03-26 07:09:06.095389 pybotx-0.65.0/pybotx/bot/api/responses/unverified_request.py
--rw-r--r--   0        0        0    62210 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/bot.py
--rw-r--r--   0        0        0     1558 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/bot_accounts_storage.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/callbacks/__init__.py
--rw-r--r--   0        0        0     3101 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/callbacks/callback_manager.py
--rw-r--r--   0        0        0     2176 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/callbacks/callback_memory_repo.py
--rw-r--r--   0        0        0      983 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/callbacks/callback_repo_proto.py
--rw-r--r--   0        0        0      330 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/contextvars.py
--rw-r--r--   0        0        0     1324 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/exceptions.py
--rw-r--r--   0        0        0     2790 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/handler.py
--rw-r--r--   0        0        0    14811 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/handler_collector.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/middlewares/__init__.py
--rw-r--r--   0        0        0     1749 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/middlewares/exception_middleware.py
--rw-r--r--   0        0        0      293 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/bot/testing.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/__init__.py
--rw-r--r--   0        0        0     1617 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/authorized_botx_method.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/bots_api/__init__.py
--rw-r--r--   0        0        0     1946 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/bots_api/bot_catalog.py
--rw-r--r--   0        0        0     1235 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/bots_api/get_token.py
--rw-r--r--   0        0        0     6809 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/botx_method.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/__init__.py
--rw-r--r--   0        0        0     2201 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/add_admin.py
--rw-r--r--   0        0        0     1443 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/add_user.py
--rw-r--r--   0        0        0     2985 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/chat_info.py
--rw-r--r--   0        0        0     2177 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/create_chat.py
--rw-r--r--   0        0        0     1415 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/disable_stealth.py
--rw-r--r--   0        0        0     2004 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/list_chats.py
--rw-r--r--   0        0        0     1398 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/pin_message.py
--rw-r--r--   0        0        0     1430 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/remove_user.py
--rw-r--r--   0        0        0     1699 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/set_stealth.py
--rw-r--r--   0        0        0     1354 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/chats_api/unpin_message.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/events_api/__init__.py
--rw-r--r--   0        0        0     1355 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/events_api/delete_event.py
--rw-r--r--   0        0        0     3295 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/events_api/edit_event.py
--rw-r--r--   0        0        0     2324 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/events_api/message_status_event.py
--rw-r--r--   0        0        0     3770 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/events_api/reply_event.py
--rw-r--r--   0        0        0     1019 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/events_api/stop_typing_event.py
--rw-r--r--   0        0        0      955 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/events_api/typing_event.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/__init__.py
--rw-r--r--   0        0        0     1301 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/base.py
--rw-r--r--   0        0        0      889 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/callbacks.py
--rw-r--r--   0        0        0      424 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/chats.py
--rw-r--r--   0        0        0      429 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/common.py
--rw-r--r--   0        0        0      130 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/event.py
--rw-r--r--   0        0        0      289 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/files.py
--rw-r--r--   0        0        0      750 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/http.py
--rw-r--r--   0        0        0      134 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/message.py
--rw-r--r--   0        0        0      378 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/notifications.py
--rw-r--r--   0        0        0      293 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/exceptions/users.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/files_api/__init__.py
--rw-r--r--   0        0        0     2093 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/files_api/download_file.py
--rw-r--r--   0        0        0     2448 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/files_api/upload_file.py
--rw-r--r--   0        0        0      812 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/get_token.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/mertics_api/__init__.py
--rw-r--r--   0        0        0     1255 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/mertics_api/collect_bot_function.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/notifications_api/__init__.py
--rw-r--r--   0        0        0     5567 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/notifications_api/direct_notification.py
--rw-r--r--   0        0        0     2925 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/notifications_api/internal_bot_notification.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/openid_api/__init__.py
--rw-r--r--   0        0        0     1245 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/openid_api/refresh_access_token.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/smartapps_api/__init__.py
--rw-r--r--   0        0        0     2319 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/smartapps_api/smartapp_custom_notification.py
--rw-r--r--   0        0        0     2259 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/smartapps_api/smartapp_event.py
--rw-r--r--   0        0        0     1836 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/smartapps_api/smartapp_notification.py
--rw-r--r--   0        0        0     2195 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/smartapps_api/smartapps_list.py
--rw-r--r--   0        0        0     1652 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/smartapps_api/upload_file.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/__init__.py
--rw-r--r--   0        0        0     2883 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/add_sticker.py
--rw-r--r--   0        0        0     1689 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/create_sticker_pack.py
--rw-r--r--   0        0        0     1506 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/delete_sticker.py
--rw-r--r--   0        0        0     1426 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/delete_sticker_pack.py
--rw-r--r--   0        0        0     1793 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/edit_sticker_pack.py
--rw-r--r--   0        0        0      311 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/exceptions.py
--rw-r--r--   0        0        0     1984 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/get_sticker.py
--rw-r--r--   0        0        0     1397 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/get_sticker_pack.py
--rw-r--r--   0        0        0     2352 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/get_sticker_packs.py
--rw-r--r--   0        0        0     1321 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/stickers_api/sticker_pack.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/__init__.py
--rw-r--r--   0        0        0     1231 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/search_user_by_email.py
--rw-r--r--   0        0        0     1066 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/search_user_by_emails.py
--rw-r--r--   0        0        0     1257 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/search_user_by_huid.py
--rw-r--r--   0        0        0     1330 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/search_user_by_login.py
--rw-r--r--   0        0        0     1254 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/search_user_by_other_id.py
--rw-r--r--   0        0        0     3020 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/update_user_profile.py
--rw-r--r--   0        0        0     1737 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/user_from_csv.py
--rw-r--r--   0        0        0     2092 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/user_from_search.py
--rw-r--r--   0        0        0     1473 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/client/users_api/users_as_csv.py
--rw-r--r--   0        0        0      421 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/constants.py
--rw-r--r--   0        0        0      221 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/converters.py
--rw-r--r--   0        0        0      789 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/image_validators.py
--rw-r--r--   0        0        0     1341 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/logger.py
--rw-r--r--   0        0        0      648 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/missing.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/__init__.py
--rw-r--r--   0        0        0     2079 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/api_base.py
--rw-r--r--   0        0        0     7256 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/async_files.py
--rw-r--r--   0        0        0    13393 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/attachments.py
--rw-r--r--   0        0        0     2480 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/base_command.py
--rw-r--r--   0        0        0      644 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/bot_account.py
--rw-r--r--   0        0        0      435 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/bot_catalog.py
--rw-r--r--   0        0        0      199 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/bot_sender.py
--rw-r--r--   0        0        0     1635 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/chats.py
--rw-r--r--   0        0        0     1709 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/commands.py
--rw-r--r--   0        0        0     8788 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/enums.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/__init__.py
--rw-r--r--   0        0        0      670 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/edit_message.py
--rw-r--r--   0        0        0      524 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/forward.py
--rw-r--r--   0        0        0    10253 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/incoming_message.py
--rw-r--r--   0        0        0     4714 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/markup.py
--rw-r--r--   0        0        0     9106 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/mentions.py
--rw-r--r--   0        0        0      270 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/message_status.py
--rw-r--r--   0        0        0      882 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/outgoing_message.py
--rw-r--r--   0        0        0      696 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/reply.py
--rw-r--r--   0        0        0      825 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/message/reply_message.py
--rw-r--r--   0        0        0      538 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/method_callbacks.py
--rw-r--r--   0        0        0      547 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/smartapps.py
--rw-r--r--   0        0        0     2691 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/status.py
--rw-r--r--   0        0        0     1744 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/stickers.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/__init__.py
--rw-r--r--   0        0        0     1591 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/added_to_chat.py
--rw-r--r--   0        0        0     2964 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/chat_created.py
--rw-r--r--   0        0        0     1267 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/cts_login.py
--rw-r--r--   0        0        0     1277 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/cts_logout.py
--rw-r--r--   0        0        0     1746 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/deleted_from_chat.py
--rw-r--r--   0        0        0     2181 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/event_edit.py
--rw-r--r--   0        0        0     2144 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/internal_bot_notification.py
--rw-r--r--   0        0        0     1600 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/left_from_chat.py
--rw-r--r--   0        0        0     3744 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/system_events/smartapp_event.py
--rw-r--r--   0        0        0     1571 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/models/users.py
--rw-r--r--   0        0        0        0 2024-03-26 07:09:06.099389 pybotx-0.65.0/pybotx/py.typed
--rw-r--r--   0        0        0     1459 2024-03-26 07:09:06.099389 pybotx-0.65.0/pyproject.toml
--rw-r--r--   0        0        0    25202 1970-01-01 00:00:00.000000 pybotx-0.65.0/PKG-INFO
+-rw-r--r--   0        0        0     6078 2024-04-12 07:48:47.896246 pybotx-0.66.0/LICENSE
+-rw-r--r--   0        0        0    24562 2024-04-12 07:48:47.896246 pybotx-0.66.0/README.md
+-rw-r--r--   0        0        0     7504 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/__init__.py
+-rw-r--r--   0        0        0      847 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/async_buffer.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/__init__.py
+-rw-r--r--   0        0        0      560 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/responses/__init__.py
+-rw-r--r--   0        0        0     1048 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/responses/bot_disabled.py
+-rw-r--r--   0        0        0      275 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/responses/command_accepted.py
+-rw-r--r--   0        0        0     1185 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/responses/unverified_request.py
+-rw-r--r--   0        0        0    63728 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/bot.py
+-rw-r--r--   0        0        0     1558 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/bot_accounts_storage.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/callbacks/__init__.py
+-rw-r--r--   0        0        0     3101 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/callbacks/callback_manager.py
+-rw-r--r--   0        0        0     2176 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/callbacks/callback_memory_repo.py
+-rw-r--r--   0        0        0      983 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/callbacks/callback_repo_proto.py
+-rw-r--r--   0        0        0      330 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/contextvars.py
+-rw-r--r--   0        0        0     1324 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/exceptions.py
+-rw-r--r--   0        0        0     2790 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/handler.py
+-rw-r--r--   0        0        0    14811 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/handler_collector.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/middlewares/__init__.py
+-rw-r--r--   0        0        0     1749 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/middlewares/exception_middleware.py
+-rw-r--r--   0        0        0      293 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/testing.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/__init__.py
+-rw-r--r--   0        0        0     1617 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/authorized_botx_method.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/bots_api/__init__.py
+-rw-r--r--   0        0        0     1946 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/bots_api/bot_catalog.py
+-rw-r--r--   0        0        0     1235 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/bots_api/get_token.py
+-rw-r--r--   0        0        0     6809 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/botx_method.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/__init__.py
+-rw-r--r--   0        0        0     2201 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/add_admin.py
+-rw-r--r--   0        0        0     1443 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/add_user.py
+-rw-r--r--   0        0        0     2985 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/chat_info.py
+-rw-r--r--   0        0        0     2177 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/create_chat.py
+-rw-r--r--   0        0        0     1415 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/disable_stealth.py
+-rw-r--r--   0        0        0     2004 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/list_chats.py
+-rw-r--r--   0        0        0     1398 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/pin_message.py
+-rw-r--r--   0        0        0     1430 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/remove_user.py
+-rw-r--r--   0        0        0     1699 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/set_stealth.py
+-rw-r--r--   0        0        0     1354 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/unpin_message.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/__init__.py
+-rw-r--r--   0        0        0     1355 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/delete_event.py
+-rw-r--r--   0        0        0     3295 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/edit_event.py
+-rw-r--r--   0        0        0     2324 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/message_status_event.py
+-rw-r--r--   0        0        0     3770 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/reply_event.py
+-rw-r--r--   0        0        0     1019 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/stop_typing_event.py
+-rw-r--r--   0        0        0      955 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/typing_event.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/__init__.py
+-rw-r--r--   0        0        0     1301 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/base.py
+-rw-r--r--   0        0        0      889 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/callbacks.py
+-rw-r--r--   0        0        0      424 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/chats.py
+-rw-r--r--   0        0        0      429 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/common.py
+-rw-r--r--   0        0        0      130 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/event.py
+-rw-r--r--   0        0        0      289 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/files.py
+-rw-r--r--   0        0        0      750 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/http.py
+-rw-r--r--   0        0        0      134 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/message.py
+-rw-r--r--   0        0        0      378 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/notifications.py
+-rw-r--r--   0        0        0      293 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/users.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/files_api/__init__.py
+-rw-r--r--   0        0        0     2093 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/files_api/download_file.py
+-rw-r--r--   0        0        0     2448 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/files_api/upload_file.py
+-rw-r--r--   0        0        0      812 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/get_token.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/mertics_api/__init__.py
+-rw-r--r--   0        0        0     1255 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/mertics_api/collect_bot_function.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/notifications_api/__init__.py
+-rw-r--r--   0        0        0     5567 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/notifications_api/direct_notification.py
+-rw-r--r--   0        0        0     2925 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/notifications_api/internal_bot_notification.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/openid_api/__init__.py
+-rw-r--r--   0        0        0     1245 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/openid_api/refresh_access_token.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/__init__.py
+-rw-r--r--   0        0        0     2319 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_custom_notification.py
+-rw-r--r--   0        0        0     2259 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_event.py
+-rw-r--r--   0        0        0     1995 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_manifest.py
+-rw-r--r--   0        0        0     1836 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_notification.py
+-rw-r--r--   0        0        0     2195 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapps_list.py
+-rw-r--r--   0        0        0     1652 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/upload_file.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/stickers_api/__init__.py
+-rw-r--r--   0        0        0     2883 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/stickers_api/add_sticker.py
+-rw-r--r--   0        0        0     1689 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/stickers_api/create_sticker_pack.py
+-rw-r--r--   0        0        0     1506 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/stickers_api/delete_sticker.py
+-rw-r--r--   0        0        0     1426 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/delete_sticker_pack.py
+-rw-r--r--   0        0        0     1793 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/edit_sticker_pack.py
+-rw-r--r--   0        0        0      311 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/exceptions.py
+-rw-r--r--   0        0        0     1984 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/get_sticker.py
+-rw-r--r--   0        0        0     1397 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/get_sticker_pack.py
+-rw-r--r--   0        0        0     2352 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/get_sticker_packs.py
+-rw-r--r--   0        0        0     1321 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/sticker_pack.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/__init__.py
+-rw-r--r--   0        0        0     1231 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_email.py
+-rw-r--r--   0        0        0     1066 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_emails.py
+-rw-r--r--   0        0        0     1257 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_huid.py
+-rw-r--r--   0        0        0     1330 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_login.py
+-rw-r--r--   0        0        0     1254 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_other_id.py
+-rw-r--r--   0        0        0     3020 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/update_user_profile.py
+-rw-r--r--   0        0        0     1737 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/user_from_csv.py
+-rw-r--r--   0        0        0     2092 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/user_from_search.py
+-rw-r--r--   0        0        0     1473 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/users_as_csv.py
+-rw-r--r--   0        0        0      421 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/constants.py
+-rw-r--r--   0        0        0      221 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/converters.py
+-rw-r--r--   0        0        0      789 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/image_validators.py
+-rw-r--r--   0        0        0     1341 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/logger.py
+-rw-r--r--   0        0        0      648 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/missing.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/__init__.py
+-rw-r--r--   0        0        0     2079 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/api_base.py
+-rw-r--r--   0        0        0     7256 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/async_files.py
+-rw-r--r--   0        0        0    13393 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/attachments.py
+-rw-r--r--   0        0        0     2480 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/base_command.py
+-rw-r--r--   0        0        0      644 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/bot_account.py
+-rw-r--r--   0        0        0      435 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/bot_catalog.py
+-rw-r--r--   0        0        0      199 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/bot_sender.py
+-rw-r--r--   0        0        0     1635 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/chats.py
+-rw-r--r--   0        0        0     1709 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/commands.py
+-rw-r--r--   0        0        0     8899 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/enums.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/__init__.py
+-rw-r--r--   0        0        0      670 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/edit_message.py
+-rw-r--r--   0        0        0      742 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/forward.py
+-rw-r--r--   0        0        0    10453 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/incoming_message.py
+-rw-r--r--   0        0        0     7095 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/markup.py
+-rw-r--r--   0        0        0     9106 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/mentions.py
+-rw-r--r--   0        0        0      270 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/message_status.py
+-rw-r--r--   0        0        0      882 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/outgoing_message.py
+-rw-r--r--   0        0        0      696 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/reply.py
+-rw-r--r--   0        0        0      825 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/reply_message.py
+-rw-r--r--   0        0        0      538 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/method_callbacks.py
+-rw-r--r--   0        0        0      547 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/smartapps.py
+-rw-r--r--   0        0        0     2691 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/status.py
+-rw-r--r--   0        0        0     1744 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/stickers.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/__init__.py
+-rw-r--r--   0        0        0     1591 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/added_to_chat.py
+-rw-r--r--   0        0        0     2964 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/chat_created.py
+-rw-r--r--   0        0        0     1267 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/cts_login.py
+-rw-r--r--   0        0        0     1277 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/cts_logout.py
+-rw-r--r--   0        0        0     1746 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/deleted_from_chat.py
+-rw-r--r--   0        0        0     2181 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/event_edit.py
+-rw-r--r--   0        0        0     2144 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/internal_bot_notification.py
+-rw-r--r--   0        0        0     1600 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/left_from_chat.py
+-rw-r--r--   0        0        0     3744 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/smartapp_event.py
+-rw-r--r--   0        0        0     1571 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/users.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/py.typed
+-rw-r--r--   0        0        0     1459 2024-04-12 07:48:47.900246 pybotx-0.66.0/pyproject.toml
+-rw-r--r--   0        0        0    25658 1970-01-01 00:00:00.000000 pybotx-0.66.0/PKG-INFO
```

### Comparing `pybotx-0.65.0/LICENSE` & `pybotx-0.66.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/README.md` & `pybotx-0.66.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -386,14 +386,23 @@
         command="/choose",
         label="Blue",
         data={"pill": "blue"},
         background_color="#0000FF",
         new_row=False,
     )
 
+    # В кнопку можно добавит ссылку на ресурс,
+    # для этого нужно добавить url в аргумент `link`, а `command` оставить пустым,
+    # `alert` добавляется в окно подтверждения при переходе по ссылке.
+    bubbles.add_button(
+        label="Bubble with link",
+        alert="alert text",
+        link="https://example.com",
+    )
+
     await bot.answer_message(
         "The time has come to make a choice, Mr. Anderson:",
         bubbles=bubbles,
     )
 ```
```

### Comparing `pybotx-0.65.0/pybotx/__init__.py` & `pybotx-0.66.0/pybotx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 from pybotx.client.exceptions.message import MessageNotFoundError
 from pybotx.client.exceptions.notifications import (
     BotIsNotChatMemberError,
     FinalRecipientsListEmptyError,
     StealthModeDisabledError,
 )
 from pybotx.client.exceptions.users import UserNotFoundError
+from pybotx.client.smartapps_api.smartapp_manifest import (
+    SmartappManifest,
+    SmartappManifestWebParams,
+)
 from pybotx.client.stickers_api.exceptions import (
     InvalidEmojiError,
     InvalidImageError,
     StickerPackOrStickerNotFoundError,
 )
 from pybotx.logger import logger
 from pybotx.models.async_files import Document, File, Image, Video, Voice
@@ -74,14 +78,15 @@
 from pybotx.models.bot_sender import BotSender
 from pybotx.models.chats import Chat, ChatInfo, ChatInfoMember, ChatListItem
 from pybotx.models.enums import (
     AttachmentTypes,
     ChatTypes,
     ClientPlatforms,
     MentionTypes,
+    SmartappManifestWebLayoutChoices,
     SyncSourceTypes,
     UserKinds,
 )
 from pybotx.models.message.edit_message import EditMessage
 from pybotx.models.message.forward import Forward
 from pybotx.models.message.incoming_message import (
     IncomingMessage,
@@ -210,14 +215,17 @@
     "RateLimitReachedError",
     "Reply",
     "ReplyMessage",
     "RequestHeadersNotProvidedError",
     "SmartApp",
     "SmartAppEvent",
     "SmartAppEvent",
+    "SmartappManifest",
+    "SmartappManifestWebLayoutChoices",
+    "SmartappManifestWebParams",
     "StatusRecipient",
     "StealthModeDisabledError",
     "Sticker",
     "StickerPack",
     "StickerPackOrStickerNotFoundError",
     "SyncSourceTypes",
     "UnknownBotAccountError",
```

### Comparing `pybotx-0.65.0/pybotx/async_buffer.py` & `pybotx-0.66.0/pybotx/async_buffer.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/api/exceptions.py` & `pybotx-0.66.0/pybotx/bot/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/api/responses/bot_disabled.py` & `pybotx-0.66.0/pybotx/bot/api/responses/bot_disabled.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/api/responses/unverified_request.py` & `pybotx-0.66.0/pybotx/bot/api/responses/unverified_request.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/bot.py` & `pybotx-0.66.0/pybotx/bot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,19 @@
     BotXAPISmartAppCustomNotificationRequestPayload,
     SmartAppCustomNotificationMethod,
 )
 from pybotx.client.smartapps_api.smartapp_event import (
     BotXAPISmartAppEventRequestPayload,
     SmartAppEventMethod,
 )
+from pybotx.client.smartapps_api.smartapp_manifest import (
+    BotXAPISmartAppManifestRequestPayload,
+    SmartappManifest,
+    SmartAppManifestMethod,
+)
 from pybotx.client.smartapps_api.smartapp_notification import (
     BotXAPISmartAppNotificationRequestPayload,
     SmartAppNotificationMethod,
 )
 from pybotx.client.smartapps_api.smartapps_list import (
     BotXAPISmartAppsListRequestPayload,
     SmartAppsListMethod,
@@ -218,14 +223,15 @@
 from pybotx.models.async_files import File
 from pybotx.models.attachments import IncomingFileAttachment, OutgoingAttachment
 from pybotx.models.bot_account import BotAccountWithSecret
 from pybotx.models.bot_catalog import BotsListItem
 from pybotx.models.chats import ChatInfo, ChatListItem
 from pybotx.models.commands import BotAPICommand, BotCommand
 from pybotx.models.enums import ChatTypes
+from pybotx.models.enums import SmartappManifestWebLayoutChoices as WebLayoutChoices
 from pybotx.models.message.edit_message import EditMessage
 from pybotx.models.message.markup import BubbleMarkup, KeyboardMarkup
 from pybotx.models.message.message_status import MessageStatus
 from pybotx.models.message.outgoing_message import OutgoingMessage
 from pybotx.models.message.reply_message import ReplyMessage
 from pybotx.models.method_callbacks import BotXMethodCallback
 from pybotx.models.smartapps import SmartApp
@@ -1496,14 +1502,46 @@
         )
         payload = BotXAPISmartAppsListRequestPayload.from_domain(version=version)
 
         botx_api_smartapps_list = await method.execute(payload)
 
         return botx_api_smartapps_list.to_domain()
 
+    async def send_smartapp_manifest(
+        self,
+        *,
+        bot_id: UUID,
+        web_default_layout: WebLayoutChoices = WebLayoutChoices.minimal,
+        web_expanded_layout: WebLayoutChoices = WebLayoutChoices.half,
+        web_always_pinned: bool = False,
+    ) -> SmartappManifest:
+        """Send smartapp manifest with given parameters.
+
+        :param bot_id: Bot which should perform the request.
+        :param web_default_layout: default smartapp layout for web clients.
+        :param web_expanded_layout: expanded smartapp layout for web clients.
+        :param web_always_pinned: True if smartapp icon should be always pinned
+            in the web clients sidebar.
+
+        :return: Smartapp manifest with the set parameters received from BotX.
+        """
+
+        method = SmartAppManifestMethod(
+            bot_id,
+            self._httpx_client,
+            self._bot_accounts_storage,
+        )
+        payload = BotXAPISmartAppManifestRequestPayload.from_domain(
+            web_default_layout=web_default_layout,
+            web_expanded_layout=web_expanded_layout,
+            web_always_pinned=web_always_pinned,
+        )
+        smartapp_manifest_response = await method.execute(payload)
+        return smartapp_manifest_response.to_domain()
+
     async def upload_static_file(
         self,
         *,
         bot_id: UUID,
         async_buffer: AsyncBufferReadable,
         filename: str,
     ) -> str:
@@ -1970,15 +2008,15 @@
 
         try:
             jwt.decode(
                 jwt=token,
                 key=bot_account.secret_key,
                 algorithms=decode_algorithms,
                 issuer=bot_account.host,
-                leeway=0.5,
+                leeway=1,
                 options={
                     "verify_aud": False,
                 },
             )
         except jwt.InvalidTokenError as exc:
             raise UnverifiedRequestError(exc.args[0]) from exc
```

### Comparing `pybotx-0.65.0/pybotx/bot/bot_accounts_storage.py` & `pybotx-0.66.0/pybotx/bot/bot_accounts_storage.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/callbacks/callback_manager.py` & `pybotx-0.66.0/pybotx/bot/callbacks/callback_manager.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/callbacks/callback_memory_repo.py` & `pybotx-0.66.0/pybotx/bot/callbacks/callback_memory_repo.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/callbacks/callback_repo_proto.py` & `pybotx-0.66.0/pybotx/bot/callbacks/callback_repo_proto.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/exceptions.py` & `pybotx-0.66.0/pybotx/bot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/handler.py` & `pybotx-0.66.0/pybotx/bot/handler.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/handler_collector.py` & `pybotx-0.66.0/pybotx/bot/handler_collector.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/bot/middlewares/exception_middleware.py` & `pybotx-0.66.0/pybotx/bot/middlewares/exception_middleware.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/authorized_botx_method.py` & `pybotx-0.66.0/pybotx/client/authorized_botx_method.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/bots_api/bot_catalog.py` & `pybotx-0.66.0/pybotx/client/bots_api/bot_catalog.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/bots_api/get_token.py` & `pybotx-0.66.0/pybotx/client/bots_api/get_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/botx_method.py` & `pybotx-0.66.0/pybotx/client/botx_method.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/add_admin.py` & `pybotx-0.66.0/pybotx/client/chats_api/add_admin.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/add_user.py` & `pybotx-0.66.0/pybotx/client/chats_api/add_user.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/chat_info.py` & `pybotx-0.66.0/pybotx/client/chats_api/chat_info.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/create_chat.py` & `pybotx-0.66.0/pybotx/client/chats_api/create_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/disable_stealth.py` & `pybotx-0.66.0/pybotx/client/chats_api/disable_stealth.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/list_chats.py` & `pybotx-0.66.0/pybotx/client/chats_api/list_chats.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/pin_message.py` & `pybotx-0.66.0/pybotx/client/chats_api/pin_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/remove_user.py` & `pybotx-0.66.0/pybotx/client/chats_api/remove_user.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/set_stealth.py` & `pybotx-0.66.0/pybotx/client/chats_api/set_stealth.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/chats_api/unpin_message.py` & `pybotx-0.66.0/pybotx/client/chats_api/unpin_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/events_api/delete_event.py` & `pybotx-0.66.0/pybotx/client/events_api/delete_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/events_api/edit_event.py` & `pybotx-0.66.0/pybotx/client/events_api/edit_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/events_api/message_status_event.py` & `pybotx-0.66.0/pybotx/client/events_api/message_status_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/events_api/reply_event.py` & `pybotx-0.66.0/pybotx/client/events_api/reply_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/events_api/stop_typing_event.py` & `pybotx-0.66.0/pybotx/client/events_api/stop_typing_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/events_api/typing_event.py` & `pybotx-0.66.0/pybotx/client/events_api/typing_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/exceptions/base.py` & `pybotx-0.66.0/pybotx/client/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/exceptions/callbacks.py` & `pybotx-0.66.0/pybotx/client/exceptions/callbacks.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/exceptions/http.py` & `pybotx-0.66.0/pybotx/client/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/files_api/download_file.py` & `pybotx-0.66.0/pybotx/client/files_api/download_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/files_api/upload_file.py` & `pybotx-0.66.0/pybotx/client/files_api/upload_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/get_token.py` & `pybotx-0.66.0/pybotx/client/get_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/mertics_api/collect_bot_function.py` & `pybotx-0.66.0/pybotx/client/mertics_api/collect_bot_function.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/notifications_api/direct_notification.py` & `pybotx-0.66.0/pybotx/client/notifications_api/direct_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/notifications_api/internal_bot_notification.py` & `pybotx-0.66.0/pybotx/client/notifications_api/internal_bot_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/openid_api/refresh_access_token.py` & `pybotx-0.66.0/pybotx/client/openid_api/refresh_access_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/smartapps_api/smartapp_custom_notification.py` & `pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_custom_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/smartapps_api/smartapp_event.py` & `pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/smartapps_api/smartapp_notification.py` & `pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/smartapps_api/smartapps_list.py` & `pybotx-0.66.0/pybotx/client/smartapps_api/smartapps_list.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/smartapps_api/upload_file.py` & `pybotx-0.66.0/pybotx/client/smartapps_api/upload_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/stickers_api/add_sticker.py` & `pybotx-0.66.0/pybotx/client/stickers_api/add_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/stickers_api/create_sticker_pack.py` & `pybotx-0.66.0/pybotx/client/stickers_api/create_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/stickers_api/delete_sticker.py` & `pybotx-0.66.0/pybotx/client/stickers_api/delete_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/stickers_api/delete_sticker_pack.py` & `pybotx-0.66.0/pybotx/client/stickers_api/delete_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/stickers_api/edit_sticker_pack.py` & `pybotx-0.66.0/pybotx/client/stickers_api/edit_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/stickers_api/get_sticker.py` & `pybotx-0.66.0/pybotx/client/stickers_api/get_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/stickers_api/get_sticker_pack.py` & `pybotx-0.66.0/pybotx/client/stickers_api/get_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/stickers_api/get_sticker_packs.py` & `pybotx-0.66.0/pybotx/client/stickers_api/get_sticker_packs.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/stickers_api/sticker_pack.py` & `pybotx-0.66.0/pybotx/client/stickers_api/sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/users_api/search_user_by_email.py` & `pybotx-0.66.0/pybotx/client/users_api/search_user_by_email.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/users_api/search_user_by_emails.py` & `pybotx-0.66.0/pybotx/client/users_api/search_user_by_emails.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/users_api/search_user_by_huid.py` & `pybotx-0.66.0/pybotx/client/users_api/search_user_by_huid.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/users_api/search_user_by_login.py` & `pybotx-0.66.0/pybotx/client/users_api/search_user_by_login.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/users_api/search_user_by_other_id.py` & `pybotx-0.66.0/pybotx/client/users_api/search_user_by_other_id.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/users_api/update_user_profile.py` & `pybotx-0.66.0/pybotx/client/users_api/update_user_profile.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/users_api/user_from_csv.py` & `pybotx-0.66.0/pybotx/client/users_api/user_from_csv.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/users_api/user_from_search.py` & `pybotx-0.66.0/pybotx/client/users_api/user_from_search.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/client/users_api/users_as_csv.py` & `pybotx-0.66.0/pybotx/client/users_api/users_as_csv.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/image_validators.py` & `pybotx-0.66.0/pybotx/image_validators.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/logger.py` & `pybotx-0.66.0/pybotx/logger.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/missing.py` & `pybotx-0.66.0/pybotx/missing.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/api_base.py` & `pybotx-0.66.0/pybotx/models/api_base.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/async_files.py` & `pybotx-0.66.0/pybotx/models/async_files.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/attachments.py` & `pybotx-0.66.0/pybotx/models/attachments.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/base_command.py` & `pybotx-0.66.0/pybotx/models/base_command.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/bot_account.py` & `pybotx-0.66.0/pybotx/models/bot_account.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/chats.py` & `pybotx-0.66.0/pybotx/models/chats.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/commands.py` & `pybotx-0.66.0/pybotx/models/commands.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/enums.py` & `pybotx-0.66.0/pybotx/models/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,14 +147,20 @@
     AD = "ad"
     ADMIN = "admin"
     EMAIL = "email"
     OPENID = "openid"
     BOTX = "botx"
 
 
+class SmartappManifestWebLayoutChoices(StrEnum):
+    minimal = "minimal"
+    half = "half"
+    full = "full"
+
+
 def convert_client_platform_to_domain(
     client_platform: BotAPIClientPlatforms,
 ) -> ClientPlatforms:
     client_platforms_mapping = {
         BotAPIClientPlatforms.WEB: ClientPlatforms.WEB,
         BotAPIClientPlatforms.ANDROID: ClientPlatforms.ANDROID,
         BotAPIClientPlatforms.IOS: ClientPlatforms.IOS,
```

### Comparing `pybotx-0.65.0/pybotx/models/message/edit_message.py` & `pybotx-0.66.0/pybotx/models/message/edit_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/message/incoming_message.py` & `pybotx-0.66.0/pybotx/models/message/incoming_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,17 @@
     if api_entity.type == BotAPIEntityTypes.FORWARD:
         api_entity = cast(BotAPIForward, api_entity)
 
         return Forward(
             chat_id=api_entity.data.group_chat_id,
             author_id=api_entity.data.sender_huid,
             sync_id=api_entity.data.source_sync_id,
+            chat_name=api_entity.data.source_chat_name,
+            forward_type=convert_chat_type_to_domain(api_entity.data.forward_type),
+            inserted_at=api_entity.data.source_inserted_at,
         )
 
     if api_entity.type == BotAPIEntityTypes.REPLY:
         api_entity = cast(BotAPIReply, api_entity)
 
         mentions = MentionList()
         for api_mention_data in api_entity.data.mentions:
```

### Comparing `pybotx-0.65.0/pybotx/models/message/mentions.py` & `pybotx-0.66.0/pybotx/models/message/mentions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/message/outgoing_message.py` & `pybotx-0.66.0/pybotx/models/message/outgoing_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/message/reply.py` & `pybotx-0.66.0/pybotx/models/message/reply.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/message/reply_message.py` & `pybotx-0.66.0/pybotx/models/message/reply_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/method_callbacks.py` & `pybotx-0.66.0/pybotx/models/method_callbacks.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/smartapps.py` & `pybotx-0.66.0/pybotx/models/smartapps.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/status.py` & `pybotx-0.66.0/pybotx/models/status.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/stickers.py` & `pybotx-0.66.0/pybotx/models/stickers.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/system_events/added_to_chat.py` & `pybotx-0.66.0/pybotx/models/system_events/added_to_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/system_events/chat_created.py` & `pybotx-0.66.0/pybotx/models/system_events/chat_created.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/system_events/cts_login.py` & `pybotx-0.66.0/pybotx/models/system_events/cts_login.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/system_events/cts_logout.py` & `pybotx-0.66.0/pybotx/models/system_events/cts_logout.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/system_events/deleted_from_chat.py` & `pybotx-0.66.0/pybotx/models/system_events/deleted_from_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/system_events/event_edit.py` & `pybotx-0.66.0/pybotx/models/system_events/event_edit.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/system_events/internal_bot_notification.py` & `pybotx-0.66.0/pybotx/models/system_events/internal_bot_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/system_events/left_from_chat.py` & `pybotx-0.66.0/pybotx/models/system_events/left_from_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/system_events/smartapp_event.py` & `pybotx-0.66.0/pybotx/models/system_events/smartapp_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pybotx/models/users.py` & `pybotx-0.66.0/pybotx/models/users.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.65.0/pyproject.toml` & `pybotx-0.66.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybotx"
-version = "0.65.0"
+version = "0.66.0"
 description = "A python library for interacting with eXpress BotX API"
 authors = [
     "Sidnev Nikolay <nsidnev@ccsteam.ru>",
     "Maxim Gorbachev <mgorbachev@ccsteam.ru>",
     "Alexander Samoylenko <alexandr.samojlenko@ccsteam.ru>",
     "Arseniy Zhiltsov <arseniy.zhiltsov@ccsteam.ru>"
 ]
```

### Comparing `pybotx-0.65.0/PKG-INFO` & `pybotx-0.66.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybotx
-Version: 0.65.0
+Version: 0.66.0
 Summary: A python library for interacting with eXpress BotX API
 Home-page: https://github.com/ExpressApp/pybotx
 Author: Sidnev Nikolay
 Author-email: nsidnev@ccsteam.ru
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -413,14 +413,23 @@
         command="/choose",
         label="Blue",
         data={"pill": "blue"},
         background_color="#0000FF",
         new_row=False,
     )
 
+    # В кнопку можно добавит ссылку на ресурс,
+    # для этого нужно добавить url в аргумент `link`, а `command` оставить пустым,
+    # `alert` добавляется в окно подтверждения при переходе по ссылке.
+    bubbles.add_button(
+        label="Bubble with link",
+        alert="alert text",
+        link="https://example.com",
+    )
+
     await bot.answer_message(
         "The time has come to make a choice, Mr. Anderson:",
         bubbles=bubbles,
     )
 ```
```

