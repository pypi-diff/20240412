# Comparing `tmp/python-telegram-bot-raw-21.0.1.tar.gz` & `tmp/python-telegram-bot-raw-21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-telegram-bot-raw-21.0.1.tar", last modified: Wed Mar  6 21:15:50 2024, max compression
+gzip compressed data, was "python-telegram-bot-raw-21.1.tar", last modified: Fri Apr 12 10:41:16 2024, max compression
```

## Comparing `python-telegram-bot-raw-21.0.1.tar` & `python-telegram-bot-raw-21.1.tar`

### file list

```diff
@@ -1,175 +1,177 @@
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.355302 python-telegram-bot-raw-21.0.1/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    32422 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.0.1/LICENSE
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    40192 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.0.1/LICENSE.dual
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7651 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.0.1/LICENSE.lesser
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.0.1/MANIFEST.in
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12541 2024-03-06 21:15:50.355302 python-telegram-bot-raw-21.0.1/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12714 2024-03-06 21:05:46.000000 python-telegram-bot-raw-21.0.1/README.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10852 2024-03-06 21:05:46.000000 python-telegram-bot-raw-21.0.1/README_RAW.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3682 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.0.1/pyproject.toml
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.335302 python-telegram-bot-raw-21.0.1/python_telegram_bot_raw.egg-info/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12541 2024-03-06 21:15:50.000000 python-telegram-bot-raw-21.0.1/python_telegram_bot_raw.egg-info/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5078 2024-03-06 21:15:50.000000 python-telegram-bot-raw-21.0.1/python_telegram_bot_raw.egg-info/SOURCES.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2024-03-06 21:15:50.000000 python-telegram-bot-raw-21.0.1/python_telegram_bot_raw.egg-info/dependency_links.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      203 2024-03-06 21:15:50.000000 python-telegram-bot-raw-21.0.1/python_telegram_bot_raw.egg-info/requires.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2024-03-06 21:15:50.000000 python-telegram-bot-raw-21.0.1/python_telegram_bot_raw.egg-info/top_level.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.0.1/requirements-opts.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      484 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.0.1/requirements.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      235 2024-03-06 21:15:50.355302 python-telegram-bot-raw-21.0.1/setup.cfg
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5073 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/setup.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.343302 python-telegram-bot-raw-21.0.1/telegram/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14857 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1820 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/__main__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   372226 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_bot.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3273 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_botcommand.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10380 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_botcommandscope.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2511 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_botdescription.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1805 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_botname.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    33026 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_callbackquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   141499 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_chat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11576 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_chatadministratorrights.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15478 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_chatboost.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6764 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_chatinvitelink.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8746 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_chatjoinrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3296 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_chatlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    27021 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_chatmember.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7991 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_chatmemberupdated.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10917 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_chatpermissions.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4274 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_choseninlineresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6956 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_dice.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.347302 python-telegram-bot-raw-21.0.1/telegram/_files/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3536 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/_basemedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3836 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/_basethumbedmedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4272 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/animation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4497 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/audio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7096 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/chatphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2720 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/contact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3552 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/document.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14644 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/file.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4191 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/inputfile.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26864 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/inputmedia.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4475 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/inputsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4762 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/location.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2826 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/photosize.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16142 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/sticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4466 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/venue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4114 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/video.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3516 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/videonote.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3031 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_files/voice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4383 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_forcereply.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6965 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_forumtopic.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.347302 python-telegram-bot-raw-21.0.1/telegram/_games/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_games/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1309 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_games/callbackgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8114 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_games/game.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2518 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_games/gamehighscore.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14854 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_giveaway.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.351302 python-telegram-bot-raw-21.0.1/telegram/_inline/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15174 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinekeyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5601 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinekeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9211 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2838 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5274 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultarticle.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5695 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5138 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5666 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcacheddocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5423 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5514 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5679 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3659 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5586 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5351 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5530 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcontact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7143 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultdocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2735 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7814 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9328 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7919 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7128 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5353 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultsbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7172 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultvenue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8610 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5587 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2746 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inputcontactmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12830 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inputinvoicemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6586 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inputlocationmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1567 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inputmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4804 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inputtextmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4561 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_inline/inputvenuemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9168 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_keyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2547 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_keyboardbuttonpolltype.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10427 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_keyboardbuttonrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4498 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_linkpreviewoptions.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5134 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_loginurl.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6856 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_menubutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   190232 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_message.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2015 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_messageautodeletetimerchanged.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8934 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_messageentity.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1704 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_messageid.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10097 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_messageorigin.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7958 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_messagereactionupdated.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.351302 python-telegram-bot-raw-21.0.1/telegram/_passport/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_passport/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22748 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_passport/credentials.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6373 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_passport/data.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12734 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_passport/encryptedpassportelement.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5171 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_passport/passportdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    18799 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_passport/passportelementerrors.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7123 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_passport/passportfile.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.351302 python-telegram-bot-raw-21.0.1/telegram/_payment/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_payment/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5012 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_payment/invoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2703 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_payment/labeledprice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3118 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_payment/orderinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5904 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_payment/precheckoutquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2977 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_payment/shippingaddress.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2502 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_payment/shippingoption.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4475 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_payment/shippingquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4939 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_payment/successfulpayment.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17858 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_poll.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2864 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_proximityalerttriggered.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6543 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_reaction.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20722 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_reply.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16464 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_replykeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3251 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_replykeyboardremove.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2199 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_sentwebappmessage.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4973 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_shared.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2551 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_story.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4136 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_switchinlinequerychosenchat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    27782 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_telegramobject.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    27448 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_update.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    77727 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_user.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2907 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_userprofilephotos.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.355302 python-telegram-bot-raw-21.0.1/telegram/_utils/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2310 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/argumentparsing.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8924 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/datetime.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4305 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/defaultvalue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2641 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/enum.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5747 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/files.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1970 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/logging.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/markup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1833 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/repr.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1441 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/strings.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3641 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/types.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1989 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/warnings.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3863 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_utils/warnings_transition.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2234 2024-03-06 21:06:30.000000 python-telegram-bot-raw-21.0.1/telegram/_version.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6022 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_videochat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2444 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_webappdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2124 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_webappinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7720 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_webhookinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3585 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/_writeaccessallowed.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   105292 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/constants.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7574 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/error.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7252 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/helpers.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.0.1/telegram/py.typed
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-03-06 21:15:50.355302 python-telegram-bot-raw-21.0.1/telegram/request/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/request/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20478 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/request/_baserequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12968 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/request/_httpxrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5204 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/request/_requestdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7408 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/request/_requestparameter.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1899 2024-03-06 21:05:44.000000 python-telegram-bot-raw-21.0.1/telegram/warnings.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    32422 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/LICENSE
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    40192 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/LICENSE.dual
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7651 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/LICENSE.lesser
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/MANIFEST.in
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12539 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12714 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/README.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10852 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/README_RAW.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3686 2024-04-12 10:02:06.000000 python-telegram-bot-raw-21.1/pyproject.toml
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.346938 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12539 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5123 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/SOURCES.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/dependency_links.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      203 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/requires.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/top_level.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.1/requirements-opts.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      484 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.1/requirements.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      235 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/setup.cfg
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5073 2024-04-12 10:34:12.000000 python-telegram-bot-raw-21.1/setup.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.354938 python-telegram-bot-raw-21.1/telegram/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15285 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1820 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/__main__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2861 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_birthdate.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   379065 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_bot.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3273 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_botcommand.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10380 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_botcommandscope.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2511 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_botdescription.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1805 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_botname.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15745 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_business.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    33026 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_callbackquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   147253 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11366 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatadministratorrights.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15478 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatboost.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6764 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatinvitelink.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8746 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatjoinrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3296 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26788 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatmember.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7991 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatmemberupdated.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10917 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatpermissions.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4274 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_choseninlineresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6956 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_dice.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.358938 python-telegram-bot-raw-21.1/telegram/_files/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3536 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/_basemedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3836 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/_basethumbedmedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4272 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/animation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4497 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/audio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7096 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/chatphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2720 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/contact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3552 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/document.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14644 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/file.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4191 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/inputfile.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26864 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/inputmedia.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5621 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/inputsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4762 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/location.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2826 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/photosize.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17443 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/sticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4466 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/venue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4114 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/video.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3516 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/videonote.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3031 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/voice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4383 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_forcereply.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6965 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_forumtopic.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.358938 python-telegram-bot-raw-21.1/telegram/_games/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_games/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1309 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_games/callbackgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8114 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_games/game.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2518 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_games/gamehighscore.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14854 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_giveaway.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.362939 python-telegram-bot-raw-21.1/telegram/_inline/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15174 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinekeyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5601 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinekeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9211 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2838 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5274 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultarticle.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5695 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5138 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5666 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcacheddocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5423 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5514 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5679 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3659 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5586 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5351 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5530 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcontact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7143 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultdocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2735 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7814 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9328 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7919 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7128 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5353 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultsbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7172 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvenue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8610 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5587 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2746 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputcontactmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12830 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputinvoicemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6586 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputlocationmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1567 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4804 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputtextmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4561 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputvenuemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9168 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_keyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2547 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_keyboardbuttonpolltype.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12851 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_keyboardbuttonrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4498 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_linkpreviewoptions.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5134 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_loginurl.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6856 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_menubutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   202095 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_message.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2015 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messageautodeletetimerchanged.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8934 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messageentity.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1704 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messageid.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10097 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messageorigin.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7958 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messagereactionupdated.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.362939 python-telegram-bot-raw-21.1/telegram/_passport/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22748 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/credentials.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6373 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/data.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12726 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/encryptedpassportelement.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5171 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/passportdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    18799 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/passportelementerrors.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7157 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/passportfile.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.362939 python-telegram-bot-raw-21.1/telegram/_payment/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5012 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/invoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2703 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/labeledprice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3118 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/orderinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5904 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/precheckoutquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2977 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/shippingaddress.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2502 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/shippingoption.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4475 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/shippingquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4939 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/successfulpayment.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17858 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_poll.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2864 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_proximityalerttriggered.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6543 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_reaction.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20722 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_reply.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16464 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_replykeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3251 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_replykeyboardremove.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2199 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_sentwebappmessage.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    13120 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_shared.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2551 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_story.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4136 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_switchinlinequerychosenchat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    27782 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_telegramobject.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    34486 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_update.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    80314 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_user.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2907 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_userprofilephotos.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/telegram/_utils/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2310 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/argumentparsing.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8924 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/datetime.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4305 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/defaultvalue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2641 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/enum.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5747 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/files.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1970 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/logging.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/markup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1833 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/repr.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1441 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/strings.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3641 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/types.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1989 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/warnings.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3863 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/warnings_transition.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2234 2024-04-12 10:35:28.000000 python-telegram-bot-raw-21.1/telegram/_version.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6022 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_videochat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2444 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_webappdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2124 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_webappinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7720 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_webhookinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3585 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_writeaccessallowed.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   106661 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/constants.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7574 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/error.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7252 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/helpers.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/telegram/py.typed
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/telegram/request/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20478 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/_baserequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12968 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/_httpxrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5204 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/_requestdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7408 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/_requestparameter.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1899 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/warnings.py
```

### Comparing `python-telegram-bot-raw-21.0.1/LICENSE` & `python-telegram-bot-raw-21.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/LICENSE.dual` & `python-telegram-bot-raw-21.1/LICENSE.dual`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/LICENSE.lesser` & `python-telegram-bot-raw-21.1/LICENSE.lesser`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/PKG-INFO` & `python-telegram-bot-raw-21.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 21.0.1
+Version: 21.1
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
@@ -49,15 +49,15 @@
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot-raw.svg
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-7.1-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-7.2-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
    :alt: Supported Bot API versions
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot-raw
    :target: https://pypistats.org/packages/python-telegram-bot-raw
    :alt: PyPi Package Monthly Download
 
@@ -120,15 +120,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **7.1** are supported.
+All types and methods of the Telegram Bot API **7.2** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-21.0.1/README.rst` & `python-telegram-bot-raw-21.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
    :target: https://pypi.org/project/python-telegram-bot/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot.svg
    :target: https://pypi.org/project/python-telegram-bot/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-7.1-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-7.2-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
    :alt: Supported Bot API versions
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot
    :target: https://pypistats.org/packages/python-telegram-bot
    :alt: PyPi Package Monthly Download
 
@@ -85,15 +85,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **7.1** are supported.
+All types and methods of the Telegram Bot API **7.2** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-21.0.1/README_RAW.rst` & `python-telegram-bot-raw-21.1/README_RAW.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot-raw.svg
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-7.1-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-7.2-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
    :alt: Supported Bot API versions
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot-raw
    :target: https://pypistats.org/packages/python-telegram-bot-raw
    :alt: PyPi Package Monthly Download
 
@@ -81,15 +81,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **7.1** are supported.
+All types and methods of the Telegram Bot API **7.2** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-21.0.1/pyproject.toml` & `python-telegram-bot-raw-21.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [tool.ruff.lint]
 preview = true
 explicit-preview-rules = true
 ignore = ["PLR2004", "PLR0911", "PLR0912", "PLR0913", "PLR0915", "PERF203"]
 select = ["E", "F", "I", "PL", "UP", "RUF", "PTH", "C4", "B", "PIE", "SIM", "RET", "RSE",
           "G", "ISC", "PT", "ASYNC", "TCH", "SLOT", "PERF", "PYI", "FLY", "AIR", "RUF022",
-          "RUF023", "Q", "INP",]
+          "RUF023", "Q", "INP", "W"]
 # Add "FURB" after it's out of preview
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*.py" = ["B018"]
 "tests/**.py" = ["RUF012", "ASYNC101"]
 "docs/**.py" = ["INP001"]
```

### Comparing `python-telegram-bot-raw-21.0.1/python_telegram_bot_raw.egg-info/PKG-INFO` & `python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 21.0.1
+Version: 21.1
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
@@ -49,15 +49,15 @@
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot-raw.svg
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-7.1-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-7.2-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
    :alt: Supported Bot API versions
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot-raw
    :target: https://pypistats.org/packages/python-telegram-bot-raw
    :alt: PyPi Package Monthly Download
 
@@ -120,15 +120,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **7.1** are supported.
+All types and methods of the Telegram Bot API **7.2** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-21.0.1/python_telegram_bot_raw.egg-info/SOURCES.txt` & `python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 python_telegram_bot_raw.egg-info/PKG-INFO
 python_telegram_bot_raw.egg-info/SOURCES.txt
 python_telegram_bot_raw.egg-info/dependency_links.txt
 python_telegram_bot_raw.egg-info/requires.txt
 python_telegram_bot_raw.egg-info/top_level.txt
 telegram/__init__.py
 telegram/__main__.py
+telegram/_birthdate.py
 telegram/_bot.py
 telegram/_botcommand.py
 telegram/_botcommandscope.py
 telegram/_botdescription.py
 telegram/_botname.py
+telegram/_business.py
 telegram/_callbackquery.py
 telegram/_chat.py
 telegram/_chatadministratorrights.py
 telegram/_chatboost.py
 telegram/_chatinvitelink.py
 telegram/_chatjoinrequest.py
 telegram/_chatlocation.py
```

### Comparing `python-telegram-bot-raw-21.0.1/requirements-opts.txt` & `python-telegram-bot-raw-21.1/requirements-opts.txt`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/setup.py` & `python-telegram-bot-raw-21.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/__init__.py` & `python-telegram-bot-raw-21.1/telegram/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,34 @@
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """A library that provides a Python interface to the Telegram Bot API"""
 
 __author__ = "devs@python-telegram-bot.org"
 __all__ = (
     "Animation",
     "Audio",
+    "Birthdate",
     "Bot",
     "BotCommand",
     "BotCommandScope",
     "BotCommandScopeAllChatAdministrators",
     "BotCommandScopeAllGroupChats",
     "BotCommandScopeAllPrivateChats",
     "BotCommandScopeChat",
     "BotCommandScopeChatAdministrators",
     "BotCommandScopeChatMember",
     "BotCommandScopeDefault",
     "BotDescription",
     "BotName",
     "BotShortDescription",
+    "BusinessConnection",
+    "BusinessIntro",
+    "BusinessLocation",
+    "BusinessMessagesDeleted",
+    "BusinessOpeningHours",
+    "BusinessOpeningHoursInterval",
     "CallbackGame",
     "CallbackQuery",
     "Chat",
     "ChatAdministratorRights",
     "ChatBoost",
     "ChatBoostAdded",
     "ChatBoostRemoved",
@@ -180,14 +187,15 @@
     "ReplyKeyboardMarkup",
     "ReplyKeyboardRemove",
     "ReplyParameters",
     "ResidentialAddress",
     "SecureData",
     "SecureValue",
     "SentWebAppMessage",
+    "SharedUser",
     "ShippingAddress",
     "ShippingOption",
     "ShippingQuery",
     "Sticker",
     "StickerSet",
     "Story",
     "SuccessfulPayment",
@@ -220,28 +228,37 @@
     "helpers",
     "request",
     "warnings",
 )
 
 
 from . import _version, constants, error, helpers, request, warnings
+from ._birthdate import Birthdate
 from ._bot import Bot
 from ._botcommand import BotCommand
 from ._botcommandscope import (
     BotCommandScope,
     BotCommandScopeAllChatAdministrators,
     BotCommandScopeAllGroupChats,
     BotCommandScopeAllPrivateChats,
     BotCommandScopeChat,
     BotCommandScopeChatAdministrators,
     BotCommandScopeChatMember,
     BotCommandScopeDefault,
 )
 from ._botdescription import BotDescription, BotShortDescription
 from ._botname import BotName
+from ._business import (
+    BusinessConnection,
+    BusinessIntro,
+    BusinessLocation,
+    BusinessMessagesDeleted,
+    BusinessOpeningHours,
+    BusinessOpeningHoursInterval,
+)
 from ._callbackquery import CallbackQuery
 from ._chat import Chat
 from ._chatadministratorrights import ChatAdministratorRights
 from ._chatboost import (
     ChatBoost,
     ChatBoostAdded,
     ChatBoostRemoved,
@@ -389,15 +406,15 @@
 from ._poll import Poll, PollAnswer, PollOption
 from ._proximityalerttriggered import ProximityAlertTriggered
 from ._reaction import ReactionCount, ReactionType, ReactionTypeCustomEmoji, ReactionTypeEmoji
 from ._reply import ExternalReplyInfo, ReplyParameters, TextQuote
 from ._replykeyboardmarkup import ReplyKeyboardMarkup
 from ._replykeyboardremove import ReplyKeyboardRemove
 from ._sentwebappmessage import SentWebAppMessage
-from ._shared import ChatShared, UsersShared
+from ._shared import ChatShared, SharedUser, UsersShared
 from ._story import Story
 from ._switchinlinequerychosenchat import SwitchInlineQueryChosenChat
 from ._telegramobject import TelegramObject
 from ._update import Update
 from ._user import User
 from ._userprofilephotos import UserProfilePhotos
 from ._videochat import (
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/__main__.py` & `python-telegram-bot-raw-21.1/telegram/__main__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_bot.py` & `python-telegram-bot-raw-21.1/telegram/_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# pylint: disable=no-self-argument, not-callable, no-member, too-many-arguments
+# pylint: disable=too-many-arguments
 #
 # A library that provides a Python interface to the Telegram Bot API
 # Copyright (C) 2015-2024
 # Leandro Toledo de Souza <devs@python-telegram-bot.org>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser Public License as published by
@@ -17,15 +17,14 @@
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Bot."""
 import asyncio
 import contextlib
 import copy
-import functools
 import pickle
 from datetime import datetime
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
@@ -54,14 +53,15 @@
     serialization = None  # type: ignore[assignment]
     CRYPTO_INSTALLED = False
 
 from telegram._botcommand import BotCommand
 from telegram._botcommandscope import BotCommandScope
 from telegram._botdescription import BotDescription, BotShortDescription
 from telegram._botname import BotName
+from telegram._business import BusinessConnection
 from telegram._chat import Chat
 from telegram._chatadministratorrights import ChatAdministratorRights
 from telegram._chatboost import UserChatBoosts
 from telegram._chatinvitelink import ChatInviteLink
 from telegram._chatmember import ChatMember
 from telegram._chatpermissions import ChatPermissions
 from telegram._files.animation import Animation
@@ -527,28 +527,14 @@
         cls, message: str, category: Type[Warning] = PTBUserWarning, stacklevel: int = 0
     ) -> None:
         """Convenience method to issue a warning. This method is here mostly to make it easier
         for ExtBot to add 1 level to all warning calls.
         """
         warn(message=message, category=category, stacklevel=stacklevel + 1)
 
-    # TODO: After https://youtrack.jetbrains.com/issue/PY-50952 is fixed, we can revisit this and
-    # consider adding Paramspec from typing_extensions to properly fix this. Currently a workaround
-    def _log(func: Any):  # type: ignore[no-untyped-def] # skipcq: PY-D0003
-        @functools.wraps(func)
-        async def decorator(self: "Bot", *args: Any, **kwargs: Any) -> Any:
-            # pylint: disable=protected-access
-            self._LOGGER.debug("Entering: %s", func.__name__)
-            result = await func(self, *args, **kwargs)
-            self._LOGGER.debug(result)
-            self._LOGGER.debug("Exiting: %s", func.__name__)
-            return result
-
-        return decorator
-
     def _parse_file_input(
         self,
         file_input: Union[FileInput, "TelegramObject"],
         tg_type: Optional[Type["TelegramObject"]] = None,
         filename: Optional[str] = None,
         attach: bool = False,
     ) -> Union[str, "InputFile", Any]:
@@ -650,36 +636,43 @@
         # to the default timezone in case this is called by ExtBot
         request_data = RequestData(
             parameters=[RequestParameter.from_input(key, value) for key, value in data.items()],
         )
 
         request = self._request[0] if endpoint == "getUpdates" else self._request[1]
 
-        return await request.post(
+        self._LOGGER.debug("Calling Bot API endpoint `%s` with parameters `%s`", endpoint, data)
+        result = await request.post(
             url=f"{self._base_url}/{endpoint}",
             request_data=request_data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
         )
+        self._LOGGER.debug(
+            "Call to Bot API endpoint `%s` finished with return value `%s`", endpoint, result
+        )
+
+        return result
 
     async def _send_message(
         self,
         endpoint: str,
         data: JSONDict,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         link_preview_options: ODVInput["LinkPreviewOptions"] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -728,14 +721,17 @@
 
         if caption is not None:
             data["caption"] = caption
 
         if caption_entities is not None:
             data["caption_entities"] = caption_entities
 
+        if business_connection_id is not None:
+            data["business_connection_id"] = business_connection_id
+
         result = await self._post(
             endpoint,
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
@@ -780,15 +776,14 @@
         if not self._initialized:
             self._LOGGER.debug("This Bot is already shut down. Returning.")
             return
 
         await asyncio.gather(self._request[0].shutdown(), self._request[1].shutdown())
         self._initialized = False
 
-    @_log
     async def do_api_request(
         self,
         endpoint: str,
         api_kwargs: Optional[JSONDict] = None,
         return_type: Optional[Type[TelegramObject]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -839,15 +834,15 @@
         if hasattr(self, endpoint):
             self._warn(
                 (
                     f"Please use 'Bot.{endpoint}' instead of "
                     f"'Bot.do_api_request(\"{endpoint}\", ...)'"
                 ),
                 PTBDeprecationWarning,
-                stacklevel=3,
+                stacklevel=2,
             )
 
         camel_case_endpoint = to_camel_case(endpoint)
         try:
             result = await self._post(
                 camel_case_endpoint,
                 api_kwargs=api_kwargs,
@@ -875,15 +870,14 @@
         if return_type is None or isinstance(result, bool):
             return result
 
         if isinstance(result, list):
             return return_type.de_list(result, self)
         return return_type.de_json(result, self)
 
-    @_log
     async def get_me(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -906,27 +900,27 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         self._bot_user = User.de_json(result, self)
         return self._bot_user  # type: ignore[return-value]
 
-    @_log
     async def send_message(
         self,
         chat_id: Union[int, str],
         text: str,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         entities: Optional[Sequence["MessageEntity"]] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         message_thread_id: Optional[int] = None,
         link_preview_options: ODVInput["LinkPreviewOptions"] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         disable_web_page_preview: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -964,14 +958,17 @@
                 keyboard, instructions to remove reply keyboard or to force a reply from the user.
             message_thread_id (:obj:`int`, optional): |message_thread_id_arg|
 
                 .. versionadded:: 20.0
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -1017,25 +1014,25 @@
             data,
             reply_to_message_id=reply_to_message_id,
             disable_notification=disable_notification,
             reply_markup=reply_markup,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
             parse_mode=parse_mode,
             link_preview_options=link_preview_options,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def delete_message(
         self,
         chat_id: Union[str, int],
         message_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1086,15 +1083,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def delete_messages(
         self,
         chat_id: Union[int, str],
         message_ids: Sequence[int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1129,15 +1125,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def forward_message(
         self,
         chat_id: Union[int, str],
         from_chat_id: Union[str, int],
         message_id: int,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
@@ -1195,15 +1190,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def forward_messages(
         self,
         chat_id: Union[int, str],
         from_chat_id: Union[str, int],
         message_ids: Sequence[int],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
@@ -1258,28 +1252,28 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return MessageId.de_list(result, self)
 
-    @_log
     async def send_photo(
         self,
         chat_id: Union[int, str],
         photo: Union[FileInput, "PhotoSize"],
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         has_spoiler: Optional[bool] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1332,14 +1326,17 @@
             has_spoiler (:obj:`bool`, optional): Pass :obj:`True` if the photo needs to be covered
                 with a spoiler animation.
 
                 .. versionadded:: 20.0
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -1389,17 +1386,17 @@
             caption_entities=caption_entities,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_audio(
         self,
         chat_id: Union[int, str],
         audio: Union[FileInput, "Audio"],
         duration: Optional[int] = None,
         performer: Optional[str] = None,
         title: Optional[str] = None,
@@ -1408,14 +1405,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1477,14 +1475,17 @@
             thumbnail (:term:`file object` | :obj:`bytes` | :class:`pathlib.Path` | :obj:`str`, \
                 optional): |thumbdocstring|
 
                 .. versionadded:: 20.2
             reply_parameters (:obj:`ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -1537,31 +1538,32 @@
             caption_entities=caption_entities,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_document(
         self,
         chat_id: Union[int, str],
         document: Union[FileInput, "Document"],
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_content_type_detection: Optional[bool] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1622,14 +1624,17 @@
             thumbnail (:term:`file object` | :obj:`bytes` | :class:`pathlib.Path` | :obj:`str`, \
                 optional): |thumbdocstring|
 
                 .. versionadded:: 20.2
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -1678,27 +1683,28 @@
             caption_entities=caption_entities,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_sticker(
         self,
         chat_id: Union[int, str],
         sticker: Union[FileInput, "Sticker"],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         emoji: Optional[str] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1709,16 +1715,16 @@
 
         .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             sticker (:obj:`str` | :term:`file object` | :obj:`bytes` | :class:`pathlib.Path` | \
                 :class:`telegram.Sticker`): Sticker to send.
-                |fileinput| Video stickers can only be sent by a ``file_id``. Animated stickers
-                can't be sent via an HTTP URL.
+                |fileinput| Video stickers can only be sent by a ``file_id``. Video and animated
+                stickers can't be sent via an HTTP URL.
 
                 Lastly you can pass an existing :class:`telegram.Sticker` object to send.
 
                 .. versionchanged:: 13.2
                    Accept :obj:`bytes` as input.
 
                 .. versionchanged:: 20.0
@@ -1739,14 +1745,17 @@
             reply_markup (:class:`InlineKeyboardMarkup` | :class:`ReplyKeyboardMarkup` | \
                 :class:`ReplyKeyboardRemove` | :class:`ForceReply`, optional):
                 Additional interface options. An object for an inline keyboard, custom reply
                 keyboard, instructions to remove reply keyboard or to force a reply from the user.
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -1787,17 +1796,17 @@
             message_thread_id=message_thread_id,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_video(
         self,
         chat_id: Union[int, str],
         video: Union[FileInput, "Video"],
         duration: Optional[int] = None,
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
@@ -1808,14 +1817,15 @@
         supports_streaming: Optional[bool] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         has_spoiler: Optional[bool] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1885,14 +1895,17 @@
             thumbnail (:term:`file object` | :obj:`bytes` | :class:`pathlib.Path` | :obj:`str`, \
                 optional): |thumbdocstring|
 
                 .. versionadded:: 20.2
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -1947,29 +1960,30 @@
             caption_entities=caption_entities,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_video_note(
         self,
         chat_id: Union[int, str],
         video_note: Union[FileInput, "VideoNote"],
         duration: Optional[int] = None,
         length: Optional[int] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2024,14 +2038,17 @@
             thumbnail (:term:`file object` | :obj:`bytes` | :class:`pathlib.Path` | :obj:`str`, \
                 optional): |thumbdocstring|
 
                 .. versionadded:: 20.2
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -2080,17 +2097,17 @@
             message_thread_id=message_thread_id,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_animation(
         self,
         chat_id: Union[int, str],
         animation: Union[FileInput, "Animation"],
         duration: Optional[int] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
@@ -2100,14 +2117,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         has_spoiler: Optional[bool] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2171,14 +2189,17 @@
             thumbnail (:term:`file object` | :obj:`bytes` | :class:`pathlib.Path` | :obj:`str`, \
                 optional): |thumbdocstring|
 
                 .. versionadded:: 20.2
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -2232,30 +2253,31 @@
             caption_entities=caption_entities,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_voice(
         self,
         chat_id: Union[int, str],
         voice: Union[FileInput, "Voice"],
         duration: Optional[int] = None,
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2312,14 +2334,17 @@
             reply_markup (:class:`InlineKeyboardMarkup` | :class:`ReplyKeyboardMarkup` | \
                 :class:`ReplyKeyboardRemove` | :class:`ForceReply`, optional):
                 Additional interface options. An object for an inline keyboard, custom reply
                 keyboard, instructions to remove reply keyboard or to force a reply from the user.
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -2369,27 +2394,28 @@
             caption_entities=caption_entities,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_media_group(
         self,
         chat_id: Union[int, str],
         media: Sequence[
             Union["InputMediaAudio", "InputMediaDocument", "InputMediaPhoto", "InputMediaVideo"]
         ],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2429,14 +2455,17 @@
             message_thread_id (:obj:`int`, optional): |message_thread_id_arg|
 
                 .. versionadded:: 20.0
 
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -2521,43 +2550,44 @@
         data: JSONDict = {
             "chat_id": chat_id,
             "media": media,
             "disable_notification": disable_notification,
             "protect_content": protect_content,
             "message_thread_id": message_thread_id,
             "reply_parameters": reply_parameters,
+            "business_connection_id": business_connection_id,
         }
 
         result = await self._post(
             "sendMediaGroup",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return Message.de_list(result, self)
 
-    @_log
     async def send_location(
         self,
         chat_id: Union[int, str],
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         live_period: Optional[int] = None,
         horizontal_accuracy: Optional[float] = None,
         heading: Optional[int] = None,
         proximity_alert_radius: Optional[int] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         location: Optional[Location] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2601,14 +2631,17 @@
             reply_markup (:class:`InlineKeyboardMarkup` | :class:`ReplyKeyboardMarkup` | \
                 :class:`ReplyKeyboardRemove` | :class:`ForceReply`, optional):
                 Additional interface options. An object for an inline keyboard, custom reply
                 keyboard, instructions to remove reply keyboard or to force a reply from the user.
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -2669,17 +2702,17 @@
             message_thread_id=message_thread_id,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def edit_message_live_location(
         self,
         chat_id: Optional[Union[str, int]] = None,
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
@@ -2766,15 +2799,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def stop_message_live_location(
         self,
         chat_id: Optional[Union[str, int]] = None,
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
@@ -2814,15 +2846,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def send_venue(
         self,
         chat_id: Union[int, str],
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
         title: Optional[str] = None,
         address: Optional[str] = None,
@@ -2831,14 +2862,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         foursquare_type: Optional[str] = None,
         google_place_id: Optional[str] = None,
         google_place_type: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         venue: Optional[Venue] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2880,14 +2912,17 @@
             reply_markup (:class:`InlineKeyboardMarkup` | :class:`ReplyKeyboardMarkup` | \
                 :class:`ReplyKeyboardRemove` | :class:`ForceReply`, optional):
                 Additional interface options. An object for an inline keyboard, custom reply
                 keyboard, instructions to remove reply keyboard or to force a reply from the user.
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -2959,29 +2994,30 @@
             message_thread_id=message_thread_id,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_contact(
         self,
         chat_id: Union[int, str],
         phone_number: Optional[str] = None,
         first_name: Optional[str] = None,
         last_name: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         vcard: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         contact: Optional[Contact] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3013,14 +3049,17 @@
             reply_markup (:class:`InlineKeyboardMarkup` | :class:`ReplyKeyboardMarkup` | \
                 :class:`ReplyKeyboardRemove` | :class:`ForceReply`, optional):
                 Additional interface options. An object for an inline keyboard, custom reply
                 keyboard, instructions to remove reply keyboard or to force a reply from the user.
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -3083,26 +3122,27 @@
             message_thread_id=message_thread_id,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_game(
         self,
         chat_id: int,
         game_short_name: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3124,14 +3164,17 @@
 
             reply_markup (:class:`telegram.InlineKeyboardMarkup`, optional): An object for a new
                 inline keyboard. If empty, one "Play game_title" button will be
                 shown. If not empty, the first button must launch the game.
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -3169,22 +3212,23 @@
             message_thread_id=message_thread_id,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def send_chat_action(
         self,
         chat_id: Union[str, int],
         action: str,
         message_thread_id: Optional[int] = None,
+        business_connection_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
@@ -3198,26 +3242,30 @@
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             action(:obj:`str`): Type of action to broadcast. Choose one, depending on what the user
                 is about to receive. For convenience look at the constants in
                 :class:`telegram.constants.ChatAction`.
             message_thread_id (:obj:`int`, optional): |message_thread_id_arg|
 
                 .. versionadded:: 20.0
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Returns:
             :obj:`bool`:  On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {
             "chat_id": chat_id,
             "action": action,
             "message_thread_id": message_thread_id,
+            "business_connection_id": business_connection_id,
         }
         return await self._post(
             "sendChatAction",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
@@ -3315,15 +3363,14 @@
                 with res.input_message_content._unfrozen():
                     res.input_message_content.link_preview_options = DefaultValue.get_value(
                         res.input_message_content.link_preview_options
                     )
 
         return res
 
-    @_log
     async def answer_inline_query(
         self,
         inline_query_id: str,
         results: Union[
             Sequence["InlineQueryResult"], Callable[[int], Optional[Sequence["InlineQueryResult"]]]
         ],
         cache_time: Optional[int] = None,
@@ -3413,15 +3460,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_user_profile_photos(
         self,
         user_id: int,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3458,15 +3504,14 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return UserProfilePhotos.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def get_file(
         self,
         file_id: Union[
             str, Animation, Audio, ChatPhoto, Document, PhotoSize, Sticker, Video, VideoNote, Voice
         ],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3524,15 +3569,14 @@
 
         file_path = cast(dict, result).get("file_path")
         if file_path and not is_local_file(file_path):
             result["file_path"] = f"{self._base_file_url}/{file_path}"
 
         return File.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def ban_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: int,
         until_date: Optional[Union[int, datetime]] = None,
         revoke_messages: Optional[bool] = None,
         *,
@@ -3588,15 +3632,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def ban_chat_sender_chat(
         self,
         chat_id: Union[str, int],
         sender_chat_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3632,15 +3675,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def unban_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: int,
         only_if_banned: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3677,15 +3719,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def unban_chat_sender_chat(
         self,
         chat_id: Union[str, int],
         sender_chat_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3718,15 +3759,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def answer_callback_query(
         self,
         callback_query_id: str,
         text: Optional[str] = None,
         show_alert: Optional[bool] = None,
         url: Optional[str] = None,
         cache_time: Optional[int] = None,
@@ -3784,15 +3824,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def edit_message_text(
         self,
         text: str,
         chat_id: Optional[Union[str, int]] = None,
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
@@ -3886,15 +3925,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def edit_message_caption(
         self,
         chat_id: Optional[Union[str, int]] = None,
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
         caption: Optional[str] = None,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
@@ -3956,15 +3994,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def edit_message_media(
         self,
         media: "InputMedia",
         chat_id: Optional[Union[str, int]] = None,
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
@@ -4020,15 +4057,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def edit_message_reply_markup(
         self,
         chat_id: Optional[Union[str, int]] = None,
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
@@ -4076,15 +4112,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_updates(
         self,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         timeout: Optional[int] = None,
         allowed_updates: Optional[Sequence[str]] = None,
         *,
@@ -4160,15 +4195,15 @@
             except NotImplementedError:
                 arg_read_timeout = 2
                 self._warn(
                     f"The class {self._request[0].__class__.__name__} does not override "
                     "the property `read_timeout`. Overriding this property will be mandatory in "
                     "future versions. Using 2 seconds as fallback.",
                     PTBDeprecationWarning,
-                    stacklevel=3,
+                    stacklevel=2,
                 )
 
         # Ideally we'd use an aggressive read timeout for the polling. However,
         # * Short polling should return within 2 seconds.
         # * Long polling poses a different problem: the connection might have been dropped while
         #   waiting for the server to return and there's no way of knowing the connection had been
         #   dropped in real time.
@@ -4188,15 +4223,14 @@
         if result:
             self._LOGGER.debug("Getting updates: %s", [u["update_id"] for u in result])
         else:
             self._LOGGER.debug("No new updates found.")
 
         return Update.de_list(result, self)
 
-    @_log
     async def set_webhook(
         self,
         url: str,
         certificate: Optional[FileInput] = None,
         max_connections: Optional[int] = None,
         allowed_updates: Optional[Sequence[str]] = None,
         ip_address: Optional[str] = None,
@@ -4316,15 +4350,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def delete_webhook(
         self,
         drop_pending_updates: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4354,15 +4387,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def leave_chat(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4389,15 +4421,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_chat(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4428,15 +4459,14 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return Chat.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def get_chat_administrators(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4470,15 +4500,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return ChatMember.de_list(result, self)
 
-    @_log
     async def get_chat_member_count(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4506,15 +4535,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4544,15 +4572,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return ChatMember.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def set_chat_sticker_set(
         self,
         chat_id: Union[str, int],
         sticker_set_name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4580,15 +4607,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def delete_chat_sticker_set(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4613,15 +4639,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_webhook_info(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4642,15 +4667,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return WebhookInfo.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def set_game_score(
         self,
         user_id: int,
         score: int,
         chat_id: Optional[int] = None,
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
@@ -4707,15 +4731,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_game_high_scores(
         self,
         user_id: int,
         chat_id: Optional[int] = None,
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
         *,
@@ -4768,15 +4791,14 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return GameHighScore.de_list(result, self)
 
-    @_log
     async def send_invoice(
         self,
         chat_id: Union[int, str],
         title: str,
         description: str,
         payload: str,
         provider_token: str,
@@ -4973,15 +4995,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def answer_shipping_query(
         self,
         shipping_query_id: str,
         ok: bool,
         shipping_options: Optional[Sequence["ShippingOption"]] = None,
         error_message: Optional[str] = None,
         *,
@@ -5032,15 +5053,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def answer_pre_checkout_query(
         self,
         pre_checkout_query_id: str,
         ok: bool,
         error_message: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5089,15 +5109,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def answer_web_app_query(
         self,
         web_app_query_id: str,
         result: "InlineQueryResult",
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5136,15 +5155,14 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return SentWebAppMessage.de_json(api_result, self)  # type: ignore[return-value]
 
-    @_log
     async def restrict_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: int,
         permissions: ChatPermissions,
         until_date: Optional[Union[int, datetime]] = None,
         use_independent_chat_permissions: Optional[bool] = None,
@@ -5210,15 +5228,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def promote_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: int,
         can_change_info: Optional[bool] = None,
         can_post_messages: Optional[bool] = None,
         can_edit_messages: Optional[bool] = None,
@@ -5335,15 +5352,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_chat_permissions(
         self,
         chat_id: Union[str, int],
         permissions: ChatPermissions,
         use_independent_chat_permissions: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5394,15 +5410,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_chat_administrator_custom_title(
         self,
         chat_id: Union[int, str],
         user_id: int,
         custom_title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5437,15 +5452,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def export_chat_invite_link(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5481,15 +5495,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def create_chat_invite_link(
         self,
         chat_id: Union[str, int],
         expire_date: Optional[Union[int, datetime]] = None,
         member_limit: Optional[int] = None,
         name: Optional[str] = None,
         creates_join_request: Optional[bool] = None,
@@ -5559,15 +5572,14 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return ChatInviteLink.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def edit_chat_invite_link(
         self,
         chat_id: Union[str, int],
         invite_link: Union[str, "ChatInviteLink"],
         expire_date: Optional[Union[int, datetime]] = None,
         member_limit: Optional[int] = None,
         name: Optional[str] = None,
@@ -5641,15 +5653,14 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return ChatInviteLink.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def revoke_chat_invite_link(
         self,
         chat_id: Union[str, int],
         invite_link: Union[str, "ChatInviteLink"],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5689,15 +5700,14 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return ChatInviteLink.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def approve_chat_join_request(
         self,
         chat_id: Union[str, int],
         user_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5730,15 +5740,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def decline_chat_join_request(
         self,
         chat_id: Union[str, int],
         user_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5771,15 +5780,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_chat_photo(
         self,
         chat_id: Union[str, int],
         photo: FileInput,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5818,15 +5826,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def delete_chat_photo(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5855,15 +5862,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_chat_title(
         self,
         chat_id: Union[str, int],
         title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5896,15 +5902,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_chat_description(
         self,
         chat_id: Union[str, int],
         description: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5938,15 +5943,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def pin_chat_message(
         self,
         chat_id: Union[str, int],
         message_id: int,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5988,15 +5992,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def unpin_chat_message(
         self,
         chat_id: Union[str, int],
         message_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6031,15 +6034,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def unpin_all_chat_messages(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6070,15 +6072,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_sticker_set(
         self,
         name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6105,15 +6106,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return StickerSet.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def get_custom_emoji_stickers(
         self,
         custom_emoji_ids: Sequence[str],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6149,15 +6149,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return Sticker.de_list(result, self)
 
-    @_log
     async def upload_sticker_file(
         self,
         user_id: int,
         sticker: FileInput,
         sticker_format: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6209,15 +6208,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return File.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def add_sticker_to_set(
         self,
         user_id: int,
         name: str,
         sticker: "InputSticker",
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6225,17 +6223,15 @@
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to add a new sticker to a set created by the bot. The format of the added
         sticker must match the format of the other stickers in the set. Emoji sticker sets can have
-        up to :tg-const:`telegram.constants.StickerSetLimit.MAX_EMOJI_STICKERS` stickers. Animated
-        and video sticker sets can have up to
-        :tg-const:`telegram.constants.StickerSetLimit.MAX_ANIMATED_STICKERS` stickers. Static
+        up to :tg-const:`telegram.constants.StickerSetLimit.MAX_EMOJI_STICKERS` stickers. Other
         sticker sets can have up to
         :tg-const:`telegram.constants.StickerSetLimit.MAX_STATIC_STICKERS` stickers.
 
         .. versionchanged:: 20.2
             Since Bot API 6.6, the parameter :paramref:`sticker` replace the parameters
             ``png_sticker``, ``tgs_sticker``, ``webm_sticker``, ``emojis``, and ``mask_position``.
 
@@ -6271,15 +6267,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_sticker_position_in_set(
         self,
         sticker: str,
         position: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6307,22 +6302,21 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def create_new_sticker_set(
         self,
         user_id: int,
         name: str,
         title: str,
         stickers: Sequence["InputSticker"],
-        sticker_format: str,
+        sticker_format: Optional[str] = None,
         sticker_type: Optional[str] = None,
         needs_repainting: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6367,14 +6361,17 @@
             sticker_format (:obj:`str`): Format of stickers in the set, must be one of
                 :attr:`~telegram.constants.StickerFormat.STATIC`,
                 :attr:`~telegram.constants.StickerFormat.ANIMATED` or
                 :attr:`~telegram.constants.StickerFormat.VIDEO`.
 
                 .. versionadded:: 20.2
 
+                .. deprecated:: 21.1
+                    Use :paramref:`telegram.InputSticker.format` instead.
+
             sticker_type (:obj:`str`, optional): Type of stickers in the set, pass
                 :attr:`telegram.Sticker.REGULAR` or :attr:`telegram.Sticker.MASK`, or
                 :attr:`telegram.Sticker.CUSTOM_EMOJI`. By default, a regular sticker set is created
 
                 .. versionadded:: 20.0
 
             needs_repainting (:obj:`bool`, optional): Pass :obj:`True` if stickers in the sticker
@@ -6386,14 +6383,22 @@
 
         Returns:
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
         """
+        if sticker_format is not None:
+            warn(
+                "The parameter `sticker_format` is deprecated. Use the parameter"
+                " `InputSticker.format` in the parameter `stickers` instead.",
+                stacklevel=2,
+                category=PTBDeprecationWarning,
+            )
+
         data: JSONDict = {
             "user_id": user_id,
             "name": name,
             "title": title,
             "stickers": stickers,
             "sticker_format": sticker_format,
             "sticker_type": sticker_type,
@@ -6406,15 +6411,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def delete_sticker_from_set(
         self,
         sticker: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6440,15 +6444,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def delete_sticker_set(
         self,
         name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6477,35 +6480,47 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_sticker_set_thumbnail(
         self,
         name: str,
         user_id: int,
+        format: str,  # pylint: disable=redefined-builtin
         thumbnail: Optional[FileInput] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to set the thumbnail of a regular or mask sticker set. The format of the
         thumbnail file must match the format of the stickers in the set.
 
         .. versionadded:: 20.2
 
+        .. versionchanged:: 21.1
+            As per Bot API 7.2, the new argument :paramref:`format` will be required, and thus the
+            order of the arguments had to be changed.
+
         Args:
             name (:obj:`str`): Sticker set name
             user_id (:obj:`int`): User identifier of created sticker set owner.
+            format (:obj:`str`): Format of the added sticker, must be one of
+                :tg-const:`telegram.constants.StickerFormat.STATIC` for a
+                ``.WEBP`` or ``.PNG`` image, :tg-const:`telegram.constants.StickerFormat.ANIMATED`
+                for a ``.TGS`` animation, :tg-const:`telegram.constants.StickerFormat.VIDEO` for a
+                WEBM video.
+
+                .. versionadded:: 21.1
+
             thumbnail (:obj:`str` | :term:`file object` | :obj:`bytes` | :class:`pathlib.Path`, \
                 optional): A **.WEBP** or **.PNG** image with the thumbnail, must
                 be up to :tg-const:`telegram.constants.StickerSetLimit.MAX_STATIC_THUMBNAIL_SIZE`
                 kilobytes in size and have width and height of exactly
                 :tg-const:`telegram.constants.StickerSetLimit.STATIC_THUMB_DIMENSIONS` px, or a
                 **.TGS** animation with the thumbnail up to
                 :tg-const:`telegram.constants.StickerSetLimit.MAX_ANIMATED_THUMBNAIL_SIZE`
@@ -6530,27 +6545,27 @@
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {
             "name": name,
             "user_id": user_id,
             "thumbnail": self._parse_file_input(thumbnail) if thumbnail else None,
+            "format": format,
         }
 
         return await self._post(
             "setStickerSetThumbnail",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_sticker_set_title(
         self,
         name: str,
         title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6583,15 +6598,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_sticker_emoji_list(
         self,
         sticker: str,
         emoji_list: Sequence[str],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6625,15 +6639,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_sticker_keywords(
         self,
         sticker: str,
         keywords: Optional[Sequence[str]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6667,15 +6680,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_sticker_mask_position(
         self,
         sticker: str,
         mask_position: Optional[MaskPosition] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6708,15 +6720,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_custom_emoji_sticker_set_thumbnail(
         self,
         name: str,
         custom_emoji_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6750,15 +6761,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_passport_data_errors(
         self,
         user_id: int,
         errors: Sequence["PassportElementError"],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6797,15 +6807,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def send_poll(
         self,
         chat_id: Union[int, str],
         question: str,
         options: Sequence[str],
         is_anonymous: Optional[bool] = None,
         type: Optional[str] = None,  # pylint: disable=redefined-builtin
@@ -6818,14 +6827,15 @@
         explanation_parse_mode: ODVInput[str] = DEFAULT_NONE,
         open_period: Optional[int] = None,
         close_date: Optional[Union[int, datetime]] = None,
         explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6893,14 +6903,17 @@
             reply_markup (:class:`InlineKeyboardMarkup` | :class:`ReplyKeyboardMarkup` | \
                 :class:`ReplyKeyboardRemove` | :class:`ForceReply`, optional):
                 Additional interface options. An object for an inline keyboard, custom reply
                 keyboard, instructions to remove reply keyboard or to force a reply from the user.
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -6952,17 +6965,17 @@
             message_thread_id=message_thread_id,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def stop_poll(
         self,
         chat_id: Union[int, str],
         message_id: int,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7000,24 +7013,24 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return Poll.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def send_dice(
         self,
         chat_id: Union[int, str],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         emoji: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7053,14 +7066,17 @@
                 .. versionadded:: 13.10
             message_thread_id (:obj:`int`, optional): |message_thread_id_arg|
 
                 .. versionadded:: 20.0
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
+            business_connection_id (:obj:`str`, optional): |business_id_str|
+
+                .. versionadded:: 21.1
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -7099,17 +7115,17 @@
             message_thread_id=message_thread_id,
             reply_parameters=reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
-    @_log
     async def get_my_default_administrator_rights(
         self,
         for_channels: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7143,29 +7159,28 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return ChatAdministratorRights.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def set_my_default_administrator_rights(
         self,
         rights: Optional[ChatAdministratorRights] = None,
         for_channels: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to change the default administrator rights requested by the bot when
         it's added as an administrator to groups or channels. These rights will be suggested to
-        users, but they are are free to modify the list before adding the bot.
+        users, but they are free to modify the list before adding the bot.
 
         .. seealso:: :meth:`get_my_default_administrator_rights`
 
         .. versionadded:: 20.0
 
         Args:
             rights (:obj:`telegram.ChatAdministratorRights`, optional): A
@@ -7189,15 +7204,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_my_commands(
         self,
         scope: Optional[BotCommandScope] = None,
         language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7243,15 +7257,14 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
         return BotCommand.de_list(result, self)
 
-    @_log
     async def set_my_commands(
         self,
         commands: Sequence[Union[BotCommand, Tuple[str, str]]],
         scope: Optional[BotCommandScope] = None,
         language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7308,15 +7321,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def delete_my_commands(
         self,
         scope: Optional[BotCommandScope] = None,
         language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7356,15 +7368,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def log_out(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7389,15 +7400,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def close(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7421,15 +7431,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def copy_message(
         self,
         chat_id: Union[int, str],
         from_chat_id: Union[str, int],
         message_id: int,
         caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
@@ -7547,15 +7556,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return MessageId.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def copy_messages(
         self,
         chat_id: Union[int, str],
         from_chat_id: Union[str, int],
         message_ids: Sequence[int],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
@@ -7618,15 +7626,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return MessageId.de_list(result, self)
 
-    @_log
     async def set_chat_menu_button(
         self,
         chat_id: Optional[int] = None,
         menu_button: Optional[MenuButton] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7660,15 +7667,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_chat_menu_button(
         self,
         chat_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7700,15 +7706,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return MenuButton.de_json(result, bot=self)  # type: ignore[return-value]
 
-    @_log
     async def create_invoice_link(
         self,
         title: str,
         description: str,
         payload: str,
         provider_token: str,
         currency: str,
@@ -7829,15 +7834,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_forum_topic_icon_stickers(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7861,15 +7865,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return Sticker.de_list(result, self)
 
-    @_log
     async def create_forum_topic(
         self,
         chat_id: Union[str, int],
         name: str,
         icon_color: Optional[int] = None,
         icon_custom_emoji_id: Optional[str] = None,
         *,
@@ -7921,15 +7924,14 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
         return ForumTopic.de_json(result, self)  # type: ignore[return-value]
 
-    @_log
     async def edit_forum_topic(
         self,
         chat_id: Union[str, int],
         message_thread_id: int,
         name: Optional[str] = None,
         icon_custom_emoji_id: Optional[str] = None,
         *,
@@ -7978,15 +7980,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def close_forum_topic(
         self,
         chat_id: Union[str, int],
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8023,15 +8024,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def reopen_forum_topic(
         self,
         chat_id: Union[str, int],
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8068,15 +8068,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def delete_forum_topic(
         self,
         chat_id: Union[str, int],
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8112,15 +8111,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def unpin_all_forum_topic_messages(
         self,
         chat_id: Union[str, int],
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8157,15 +8155,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def unpin_all_general_forum_topic_messages(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8197,15 +8194,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def edit_general_forum_topic(
         self,
         chat_id: Union[str, int],
         name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8241,15 +8237,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def close_general_forum_topic(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8281,15 +8276,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def reopen_general_forum_topic(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8322,15 +8316,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def hide_general_forum_topic(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8363,15 +8356,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def unhide_general_forum_topic(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8403,15 +8395,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_my_description(
         self,
         description: Optional[str] = None,
         language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8449,15 +8440,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def set_my_short_description(
         self,
         short_description: Optional[str] = None,
         language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8495,15 +8485,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_my_description(
         self,
         language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8534,15 +8523,14 @@
                 connect_timeout=connect_timeout,
                 pool_timeout=pool_timeout,
                 api_kwargs=api_kwargs,
             ),
             bot=self,
         )
 
-    @_log
     async def get_my_short_description(
         self,
         language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8574,15 +8562,14 @@
                 connect_timeout=connect_timeout,
                 pool_timeout=pool_timeout,
                 api_kwargs=api_kwargs,
             ),
             bot=self,
         )
 
-    @_log
     async def set_my_name(
         self,
         name: Optional[str] = None,
         language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8623,15 +8610,14 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    @_log
     async def get_my_name(
         self,
         language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8662,15 +8648,14 @@
                 connect_timeout=connect_timeout,
                 pool_timeout=pool_timeout,
                 api_kwargs=api_kwargs,
             ),
             bot=self,
         )
 
-    @_log
     async def get_user_chat_boosts(
         self,
         chat_id: Union[str, int],
         user_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8705,15 +8690,14 @@
                 connect_timeout=connect_timeout,
                 pool_timeout=pool_timeout,
                 api_kwargs=api_kwargs,
             ),
             bot=self,
         )
 
-    @_log
     async def set_message_reaction(
         self,
         chat_id: Union[str, int],
         message_id: int,
         reaction: Optional[Union[Sequence[Union[ReactionType, str]], ReactionType, str]] = None,
         is_big: Optional[bool] = None,
         *,
@@ -8790,14 +8774,103 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
+    async def get_business_connection(
+        self,
+        business_connection_id: str,
+        *,
+        read_timeout: ODVInput[float] = DEFAULT_NONE,
+        write_timeout: ODVInput[float] = DEFAULT_NONE,
+        connect_timeout: ODVInput[float] = DEFAULT_NONE,
+        pool_timeout: ODVInput[float] = DEFAULT_NONE,
+        api_kwargs: Optional[JSONDict] = None,
+    ) -> BusinessConnection:
+        """
+        Use this method to get information about the connection of the bot with a business account.
+
+        .. versionadded:: 21.1
+
+        Args:
+            business_connection_id (:obj:`str`): Unique identifier of the business connection.
+
+        Returns:
+            :class:`telegram.BusinessConnection`: On success, the object containing the business
+                connection information is returned.
+
+        Raises:
+            :class:`telegram.error.TelegramError`
+        """
+        data: JSONDict = {"business_connection_id": business_connection_id}
+        return BusinessConnection.de_json(  # type: ignore[return-value]
+            await self._post(
+                "getBusinessConnection",
+                data,
+                read_timeout=read_timeout,
+                write_timeout=write_timeout,
+                connect_timeout=connect_timeout,
+                pool_timeout=pool_timeout,
+                api_kwargs=api_kwargs,
+            ),
+            bot=self,
+        )
+
+    async def replace_sticker_in_set(
+        self,
+        user_id: int,
+        name: str,
+        old_sticker: str,
+        sticker: "InputSticker",
+        *,
+        read_timeout: ODVInput[float] = DEFAULT_NONE,
+        write_timeout: ODVInput[float] = DEFAULT_NONE,
+        connect_timeout: ODVInput[float] = DEFAULT_NONE,
+        pool_timeout: ODVInput[float] = DEFAULT_NONE,
+        api_kwargs: Optional[JSONDict] = None,
+    ) -> bool:
+        """Use this method to replace an existing sticker in a sticker set with a new one.
+        The method is equivalent to calling :meth:`delete_sticker_from_set`,
+        then :meth:`add_sticker_to_set`, then :meth:`set_sticker_position_in_set`.
+
+        .. versionadded:: 21.1
+
+        Args:
+            user_id (:obj:`int`): User identifier of the sticker set owner.
+            name (:obj:`str`): Sticker set name.
+            old_sticker (:obj:`str`): File identifier of the replaced sticker.
+            sticker (:obj:`telegram.InputSticker`): An object with information about the added
+                sticker. If exactly the same sticker had already been added to the set, then the
+                set remains unchanged.
+
+        Returns:
+            :obj:`bool`: On success, :obj:`True` is returned.
+
+        Raises:
+            :class:`telegram.error.TelegramError`
+        """
+        data: JSONDict = {
+            "user_id": user_id,
+            "name": name,
+            "old_sticker": old_sticker,
+            "sticker": sticker,
+        }
+
+        return await self._post(
+            "replaceStickerInSet",
+            data,
+            read_timeout=read_timeout,
+            write_timeout=write_timeout,
+            connect_timeout=connect_timeout,
+            pool_timeout=pool_timeout,
+            api_kwargs=api_kwargs,
+        )
+
     def to_dict(self, recursive: bool = True) -> JSONDict:
         """See :meth:`telegram.TelegramObject.to_dict`."""
         data: JSONDict = {"id": self.id, "username": self.username, "first_name": self.first_name}
 
         if self.last_name:
             data["last_name"] = self.last_name
 
@@ -9036,7 +9109,11 @@
     """Alias for :meth:`get_my_name`"""
     unpinAllGeneralForumTopicMessages = unpin_all_general_forum_topic_messages
     """Alias for :meth:`unpin_all_general_forum_topic_messages`"""
     getUserChatBoosts = get_user_chat_boosts
     """Alias for :meth:`get_user_chat_boosts`"""
     setMessageReaction = set_message_reaction
     """Alias for :meth:`set_message_reaction`"""
+    getBusinessConnection = get_business_connection
+    """Alias for :meth:`get_business_connection`"""
+    replaceStickerInSet = replace_sticker_in_set
+    """Alias for :meth:`replace_sticker_in_set`"""
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_botcommand.py` & `python-telegram-bot-raw-21.1/telegram/_botcommand.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_botcommandscope.py` & `python-telegram-bot-raw-21.1/telegram/_botcommandscope.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_botdescription.py` & `python-telegram-bot-raw-21.1/telegram/_botdescription.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_botname.py` & `python-telegram-bot-raw-21.1/telegram/_botname.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_callbackquery.py` & `python-telegram-bot-raw-21.1/telegram/_callbackquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_chat.py` & `python-telegram-bot-raw-21.1/telegram/_chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Chat."""
 from datetime import datetime
 from html import escape
 from typing import TYPE_CHECKING, Final, Optional, Sequence, Tuple, Union
 
 from telegram import constants
+from telegram._birthdate import Birthdate
 from telegram._chatlocation import ChatLocation
 from telegram._chatpermissions import ChatPermissions
 from telegram._files.chatphoto import ChatPhoto
 from telegram._forumtopic import ForumTopic
 from telegram._menubutton import MenuButton
 from telegram._reaction import ReactionType
 from telegram._telegramobject import TelegramObject
@@ -40,14 +41,17 @@
 from telegram.helpers import mention_markdown as helpers_mention_markdown
 
 if TYPE_CHECKING:
     from telegram import (
         Animation,
         Audio,
         Bot,
+        BusinessIntro,
+        BusinessLocation,
+        BusinessOpeningHours,
         ChatInviteLink,
         ChatMember,
         Contact,
         Document,
         InlineKeyboardMarkup,
         InputMediaAudio,
         InputMediaDocument,
@@ -165,14 +169,29 @@
             .. versionadded:: 20.0
         active_usernames (Sequence[:obj:`str`], optional):  If set, the list of all `active chat
             usernames <https://telegram.org/blog/topics-in-groups-collectible-usernames\
             #collectible-usernames>`_; for private chats, supergroups and channels. Returned
             only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+        business_intro (:class:`telegram.BusinessIntro`, optional): For private chats with
+            business accounts, the intro of the business. Returned only in
+            :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
+        business_location (:class:`telegram.BusinessLocation`, optional): For private chats with
+            business accounts, the location of the business. Returned only in
+            :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
+        business_opening_hours (:class:`telegram.BusinessOpeningHours`, optional): For private
+            chats with business accounts, the opening hours of the business. Returned only in
+            :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
         available_reactions (Sequence[:class:`telegram.ReactionType`], optional): List of available
             reactions allowed in the chat. If omitted, then all of
             :const:`telegram.constants.ReactionEmoji` are allowed. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
         accent_color_id (:obj:`int`, optional): Identifier of the
@@ -225,14 +244,22 @@
 
             .. versionadded:: 21.0
         custom_emoji_sticker_set_name (:obj:`str`, optional): For supergroups, the name of the
             group's custom emoji sticker set. Custom emoji from this set can be used by all users
             and bots in the group. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.0
+        birthdate (:obj:`telegram.Birthdate`, optional): For private chats,
+            the date of birth of the user. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
+        personal_chat (:obj:`telegram.Chat`, optional): For private chats, the personal channel of
+            the user. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
 
     Attributes:
         id (:obj:`int`): Unique identifier for this chat. This number may be greater than 32 bits
             and some programming languages may have difficulty/silent defects in interpreting it.
             But it is smaller than 52 bits, so a signed 64-bit integer or double-precision float
             type are safe for storing this identifier.
         type (:obj:`str`): Type of chat, can be either :attr:`PRIVATE`, :attr:`GROUP`,
@@ -308,14 +335,29 @@
             usernames <https://telegram.org/blog/topics-in-groups-collectible-usernames\
             #collectible-usernames>`_; for private chats, supergroups and channels. Returned
             only in :meth:`telegram.Bot.get_chat`.
             This list is empty if the chat has no active usernames or this chat instance was not
             obtained via :meth:`~telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+        business_intro (:class:`telegram.BusinessIntro`): Optional. For private chats with
+            business accounts, the intro of the business. Returned only in
+            :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
+        business_location (:class:`telegram.BusinessLocation`): Optional. For private chats with
+            business accounts, the location of the business. Returned only in
+            :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
+        business_opening_hours (:class:`telegram.BusinessOpeningHours`): Optional. For private
+            chats with business accounts, the opening hours of the business. Returned only in
+            :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
         available_reactions (Tuple[:class:`telegram.ReactionType`]): Optional. List of available
             reactions allowed in the chat. If omitted, then all of
             :const:`telegram.constants.ReactionEmoji` are allowed. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
         accent_color_id (:obj:`int`): Optional. Identifier of the
@@ -368,25 +410,37 @@
 
             .. versionadded:: 21.0
         custom_emoji_sticker_set_name (:obj:`str`): Optional. For supergroups, the name of the
             group's custom emoji sticker set. Custom emoji from this set can be used by all users
             and bots in the group. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.0
+        birthdate (:obj:`telegram.Birthdate`): Optional. For private chats,
+            the date of birth of the user. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
+        personal_chat (:obj:`telegram.Chat`): Optional. For private chats, the personal channel of
+            the user. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. versionadded:: 21.1
 
     .. _topics: https://telegram.org/blog/topics-in-groups-collectible-usernames#topics-in-groups
     .. _accent colors: https://core.telegram.org/bots/api#accent-colors
     """
 
     __slots__ = (
         "accent_color_id",
         "active_usernames",
         "available_reactions",
         "background_custom_emoji_id",
         "bio",
+        "birthdate",
+        "business_intro",
+        "business_location",
+        "business_opening_hours",
         "can_set_sticker_set",
         "custom_emoji_sticker_set_name",
         "description",
         "emoji_status_custom_emoji_id",
         "emoji_status_expiration_date",
         "first_name",
         "has_aggressive_anti_spam_enabled",
@@ -401,14 +455,15 @@
         "join_by_request",
         "join_to_send_messages",
         "last_name",
         "linked_chat_id",
         "location",
         "message_auto_delete_time",
         "permissions",
+        "personal_chat",
         "photo",
         "pinned_message",
         "profile_accent_color_id",
         "profile_background_custom_emoji_id",
         "slow_mode_delay",
         "sticker_set_name",
         "title",
@@ -466,14 +521,19 @@
         accent_color_id: Optional[int] = None,
         background_custom_emoji_id: Optional[str] = None,
         profile_accent_color_id: Optional[int] = None,
         profile_background_custom_emoji_id: Optional[str] = None,
         has_visible_history: Optional[bool] = None,
         unrestrict_boost_count: Optional[int] = None,
         custom_emoji_sticker_set_name: Optional[str] = None,
+        birthdate: Optional[Birthdate] = None,
+        personal_chat: Optional["Chat"] = None,
+        business_intro: Optional["BusinessIntro"] = None,
+        business_location: Optional["BusinessLocation"] = None,
+        business_opening_hours: Optional["BusinessOpeningHours"] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.id: int = id
         self.type: str = enum.get_member(constants.ChatType, type, type)
@@ -515,14 +575,19 @@
         )
         self.accent_color_id: Optional[int] = accent_color_id
         self.background_custom_emoji_id: Optional[str] = background_custom_emoji_id
         self.profile_accent_color_id: Optional[int] = profile_accent_color_id
         self.profile_background_custom_emoji_id: Optional[str] = profile_background_custom_emoji_id
         self.unrestrict_boost_count: Optional[int] = unrestrict_boost_count
         self.custom_emoji_sticker_set_name: Optional[str] = custom_emoji_sticker_set_name
+        self.birthdate: Optional[Birthdate] = birthdate
+        self.personal_chat: Optional["Chat"] = personal_chat
+        self.business_intro: Optional["BusinessIntro"] = business_intro
+        self.business_location: Optional["BusinessLocation"] = business_location
+        self.business_opening_hours: Optional["BusinessOpeningHours"] = business_opening_hours
 
         self._id_attrs = (self.id,)
 
         self._freeze()
 
     @property
     def effective_name(self) -> Optional[str]:
@@ -577,20 +642,32 @@
         loc_tzinfo = extract_tzinfo_from_defaults(bot)
 
         data["emoji_status_expiration_date"] = from_timestamp(
             data.get("emoji_status_expiration_date"), tzinfo=loc_tzinfo
         )
 
         data["photo"] = ChatPhoto.de_json(data.get("photo"), bot)
-        from telegram import Message  # pylint: disable=import-outside-toplevel
+        from telegram import (  # pylint: disable=import-outside-toplevel
+            BusinessIntro,
+            BusinessLocation,
+            BusinessOpeningHours,
+            Message,
+        )
 
         data["pinned_message"] = Message.de_json(data.get("pinned_message"), bot)
         data["permissions"] = ChatPermissions.de_json(data.get("permissions"), bot)
         data["location"] = ChatLocation.de_json(data.get("location"), bot)
         data["available_reactions"] = ReactionType.de_list(data.get("available_reactions"), bot)
+        data["birthdate"] = Birthdate.de_json(data.get("birthdate"), bot)
+        data["personal_chat"] = cls.de_json(data.get("personal_chat"), bot)
+        data["business_intro"] = BusinessIntro.de_json(data.get("business_intro"), bot)
+        data["business_location"] = BusinessLocation.de_json(data.get("business_location"), bot)
+        data["business_opening_hours"] = BusinessOpeningHours.de_json(
+            data.get("business_opening_hours"), bot
+        )
 
         api_kwargs = {}
         # This is a deprecated field that TG still returns for backwards compatibility
         # Let's filter it out to speed up the de-json process
         if "all_members_are_administrators" in data:
             api_kwargs["all_members_are_administrators"] = data.pop(
                 "all_members_are_administrators"
@@ -1165,15 +1242,15 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def set_administrator_custom_title(
         self,
-        user_id: Union[int, str],
+        user_id: int,
         custom_title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
@@ -1440,14 +1517,15 @@
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         link_preview_options: ODVInput["LinkPreviewOptions"] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         disable_web_page_preview: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1479,14 +1557,15 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
     async def delete_message(
         self,
         message_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1554,14 +1633,15 @@
         media: Sequence[
             Union["InputMediaAudio", "InputMediaDocument", "InputMediaPhoto", "InputMediaVideo"]
         ],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1594,20 +1674,22 @@
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
             reply_parameters=reply_parameters,
+            business_connection_id=business_connection_id,
         )
 
     async def send_chat_action(
         self,
         action: str,
         message_thread_id: Optional[int] = None,
+        business_connection_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
@@ -1626,14 +1708,15 @@
             action=action,
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
     send_action = send_chat_action
     """Alias for :attr:`send_chat_action`"""
 
     async def send_photo(
         self,
@@ -1643,14 +1726,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         has_spoiler: Optional[bool] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1683,27 +1767,29 @@
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             has_spoiler=has_spoiler,
+            business_connection_id=business_connection_id,
         )
 
     async def send_contact(
         self,
         phone_number: Optional[str] = None,
         first_name: Optional[str] = None,
         last_name: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         vcard: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         contact: Optional["Contact"] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1735,14 +1821,15 @@
             pool_timeout=pool_timeout,
             contact=contact,
             vcard=vcard,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_audio(
         self,
         audio: Union[FileInput, "Audio"],
         duration: Optional[int] = None,
         performer: Optional[str] = None,
@@ -1752,14 +1839,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1795,14 +1883,15 @@
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             thumbnail=thumbnail,
+            business_connection_id=business_connection_id,
         )
 
     async def send_document(
         self,
         document: Union[FileInput, "Document"],
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
@@ -1810,14 +1899,15 @@
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_content_type_detection: Optional[bool] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1851,24 +1941,26 @@
             thumbnail=thumbnail,
             api_kwargs=api_kwargs,
             disable_content_type_detection=disable_content_type_detection,
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_dice(
         self,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         emoji: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1895,24 +1987,26 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             emoji=emoji,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_game(
         self,
         game_short_name: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1939,14 +2033,15 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_invoice(
         self,
         title: str,
         description: str,
         payload: str,
@@ -2048,14 +2143,15 @@
         live_period: Optional[int] = None,
         horizontal_accuracy: Optional[float] = None,
         heading: Optional[int] = None,
         proximity_alert_radius: Optional[int] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         location: Optional["Location"] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2089,14 +2185,15 @@
             api_kwargs=api_kwargs,
             horizontal_accuracy=horizontal_accuracy,
             heading=heading,
             proximity_alert_radius=proximity_alert_radius,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_animation(
         self,
         animation: Union[FileInput, "Animation"],
         duration: Optional[int] = None,
         width: Optional[int] = None,
@@ -2107,14 +2204,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         has_spoiler: Optional[bool] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2151,25 +2249,27 @@
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             has_spoiler=has_spoiler,
             thumbnail=thumbnail,
+            business_connection_id=business_connection_id,
         )
 
     async def send_sticker(
         self,
         sticker: Union[FileInput, "Sticker"],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         emoji: Optional[str] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2197,14 +2297,15 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             emoji=emoji,
+            business_connection_id=business_connection_id,
         )
 
     async def send_venue(
         self,
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
         title: Optional[str] = None,
@@ -2214,14 +2315,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         foursquare_type: Optional[str] = None,
         google_place_id: Optional[str] = None,
         google_place_type: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         venue: Optional["Venue"] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2257,14 +2359,15 @@
             foursquare_type=foursquare_type,
             api_kwargs=api_kwargs,
             google_place_id=google_place_id,
             google_place_type=google_place_type,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_video(
         self,
         video: Union[FileInput, "Video"],
         duration: Optional[int] = None,
         caption: Optional[str] = None,
@@ -2276,14 +2379,15 @@
         supports_streaming: Optional[bool] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         has_spoiler: Optional[bool] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2321,27 +2425,29 @@
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             has_spoiler=has_spoiler,
+            business_connection_id=business_connection_id,
         )
 
     async def send_video_note(
         self,
         video_note: Union[FileInput, "VideoNote"],
         duration: Optional[int] = None,
         length: Optional[int] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2373,28 +2479,30 @@
             pool_timeout=pool_timeout,
             thumbnail=thumbnail,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_voice(
         self,
         voice: Union[FileInput, "Voice"],
         duration: Optional[int] = None,
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2427,14 +2535,15 @@
             parse_mode=parse_mode,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_poll(
         self,
         question: str,
         options: Sequence[str],
         is_anonymous: Optional[bool] = None,
@@ -2448,14 +2557,15 @@
         explanation_parse_mode: ODVInput[str] = DEFAULT_NONE,
         open_period: Optional[int] = None,
         close_date: Optional[Union[int, datetime]] = None,
         explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2493,14 +2603,15 @@
             open_period=open_period,
             close_date=close_date,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             explanation_entities=explanation_entities,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_copy(
         self,
         from_chat_id: Union[str, int],
         message_id: int,
         caption: Optional[str] = None,
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_chatadministratorrights.py` & `python-telegram-bot-raw-21.1/telegram/_chatadministratorrights.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,19 @@
         :attr:`can_manage_topics` is considered as well when comparing objects of
         this type in terms of equality.
 
     .. versionchanged:: 20.6
         :attr:`can_post_stories`, :attr:`can_edit_stories`, and :attr:`can_delete_stories` are
         considered as well when comparing objects of this type in terms of equality.
 
+    .. versionchanged:: 21.1
+        As of this version, :attr:`can_post_stories`, :attr:`can_edit_stories`,
+        and :attr:`can_delete_stories` is now required. Thus, the order of arguments had to be
+        changed.
+
     Args:
         is_anonymous (:obj:`bool`): :obj:`True`, if the user's presence in the chat is hidden.
         can_manage_chat (:obj:`bool`): :obj:`True`, if the administrator can access the chat event
             log, get boost list, see hidden supergroup and channel members, report spam messages
             and ignore slow mode. Implied by any other administrator privilege.
         can_delete_messages (:obj:`bool`): :obj:`True`, if the administrator can delete messages of
             other users.
@@ -165,40 +170,34 @@
         can_manage_chat: bool,
         can_delete_messages: bool,
         can_manage_video_chats: bool,
         can_restrict_members: bool,
         can_promote_members: bool,
         can_change_info: bool,
         can_invite_users: bool,
+        can_post_stories: bool,
+        can_edit_stories: bool,
+        can_delete_stories: bool,
         can_post_messages: Optional[bool] = None,
         can_edit_messages: Optional[bool] = None,
         can_pin_messages: Optional[bool] = None,
         can_manage_topics: Optional[bool] = None,
-        can_post_stories: Optional[bool] = None,
-        can_edit_stories: Optional[bool] = None,
-        can_delete_stories: Optional[bool] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ) -> None:
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.is_anonymous: bool = is_anonymous
         self.can_manage_chat: bool = can_manage_chat
         self.can_delete_messages: bool = can_delete_messages
         self.can_manage_video_chats: bool = can_manage_video_chats
         self.can_restrict_members: bool = can_restrict_members
         self.can_promote_members: bool = can_promote_members
         self.can_change_info: bool = can_change_info
         self.can_invite_users: bool = can_invite_users
-        # Not actually optionals but because of backwards compatability we pretend they are
-        if can_post_stories is None or can_edit_stories is None or can_delete_stories is None:
-            raise TypeError(
-                "As of v21.0 can_post_stories, can_edit_stories and can_delete_stories"
-                " must be set in order to create this object."
-            )
         self.can_post_stories: bool = can_post_stories
         self.can_edit_stories: bool = can_edit_stories
         self.can_delete_stories: bool = can_delete_stories
         # Optionals
         self.can_post_messages: Optional[bool] = can_post_messages
         self.can_edit_messages: Optional[bool] = can_edit_messages
         self.can_pin_messages: Optional[bool] = can_pin_messages
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_chatboost.py` & `python-telegram-bot-raw-21.1/telegram/_chatboost.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_chatinvitelink.py` & `python-telegram-bot-raw-21.1/telegram/_chatinvitelink.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_chatjoinrequest.py` & `python-telegram-bot-raw-21.1/telegram/_chatjoinrequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_chatlocation.py` & `python-telegram-bot-raw-21.1/telegram/_chatlocation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_chatmember.py` & `python-telegram-bot-raw-21.1/telegram/_chatmember.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,19 @@
 
        * Argument and attribute ``can_manage_voice_chats`` were renamed to
          :paramref:`can_manage_video_chats` and  :attr:`can_manage_video_chats` in accordance to
          Bot API 6.0.
        * The argument :paramref:`can_manage_topics` was added, which changes the position of the
          optional argument :paramref:`custom_title`.
 
+    .. versionchanged:: 21.1
+        As of this version, :attr:`can_post_stories`, :attr:`can_edit_stories`,
+        and :attr:`can_delete_stories` is now required. Thus, the order of arguments had to be
+        changed.
+
     Args:
         user (:class:`telegram.User`): Information about the user.
         can_be_edited (:obj:`bool`): :obj:`True`, if the bot
             is allowed to edit administrator privileges of that user.
         is_anonymous (:obj:`bool`): :obj:`True`, if the  user's
             presence in the chat is hidden.
         can_manage_chat (:obj:`bool`): :obj:`True`, if the administrator can access the chat event
@@ -336,42 +341,36 @@
         can_manage_chat: bool,
         can_delete_messages: bool,
         can_manage_video_chats: bool,
         can_restrict_members: bool,
         can_promote_members: bool,
         can_change_info: bool,
         can_invite_users: bool,
+        can_post_stories: bool,
+        can_edit_stories: bool,
+        can_delete_stories: bool,
         can_post_messages: Optional[bool] = None,
         can_edit_messages: Optional[bool] = None,
         can_pin_messages: Optional[bool] = None,
         can_manage_topics: Optional[bool] = None,
         custom_title: Optional[str] = None,
-        can_post_stories: Optional[bool] = None,
-        can_edit_stories: Optional[bool] = None,
-        can_delete_stories: Optional[bool] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(status=ChatMember.ADMINISTRATOR, user=user, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.can_be_edited: bool = can_be_edited
             self.is_anonymous: bool = is_anonymous
             self.can_manage_chat: bool = can_manage_chat
             self.can_delete_messages: bool = can_delete_messages
             self.can_manage_video_chats: bool = can_manage_video_chats
             self.can_restrict_members: bool = can_restrict_members
             self.can_promote_members: bool = can_promote_members
             self.can_change_info: bool = can_change_info
             self.can_invite_users: bool = can_invite_users
-            # Not actually optionals but because of backwards compatability we pretend they are
-            if can_post_stories is None or can_edit_stories is None or can_delete_stories is None:
-                raise TypeError(
-                    "As of 21.0 can_post_stories, can_edit_stories and can_delete_stories "
-                    "must be set in order to create this object."
-                )
             self.can_post_stories: bool = can_post_stories
             self.can_edit_stories: bool = can_edit_stories
             self.can_delete_stories: bool = can_delete_stories
             # Optionals
             self.can_post_messages: Optional[bool] = can_post_messages
             self.can_edit_messages: Optional[bool] = can_edit_messages
             self.can_pin_messages: Optional[bool] = can_pin_messages
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_chatmemberupdated.py` & `python-telegram-bot-raw-21.1/telegram/_chatmemberupdated.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_chatpermissions.py` & `python-telegram-bot-raw-21.1/telegram/_chatpermissions.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_choseninlineresult.py` & `python-telegram-bot-raw-21.1/telegram/_choseninlineresult.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_dice.py` & `python-telegram-bot-raw-21.1/telegram/_dice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/_basemedium.py` & `python-telegram-bot-raw-21.1/telegram/_files/_basemedium.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/_basethumbedmedium.py` & `python-telegram-bot-raw-21.1/telegram/_files/_basethumbedmedium.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/animation.py` & `python-telegram-bot-raw-21.1/telegram/_files/animation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/audio.py` & `python-telegram-bot-raw-21.1/telegram/_files/audio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/chatphoto.py` & `python-telegram-bot-raw-21.1/telegram/_files/chatphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/contact.py` & `python-telegram-bot-raw-21.1/telegram/_files/contact.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/document.py` & `python-telegram-bot-raw-21.1/telegram/_files/document.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/file.py` & `python-telegram-bot-raw-21.1/telegram/_files/file.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/inputfile.py` & `python-telegram-bot-raw-21.1/telegram/_files/inputfile.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/inputmedia.py` & `python-telegram-bot-raw-21.1/telegram/_files/inputmedia.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/inputsticker.py` & `python-telegram-bot-raw-21.1/telegram/_files/inputsticker.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 
 class InputSticker(TelegramObject):
     """
     This object describes a sticker to be added to a sticker set.
 
     .. versionadded:: 20.2
 
+    .. versionchanged:: 21.1
+        As of Bot API 7.2, the new argument :paramref:`format` is a required argument, and thus the
+        order of the arguments has changed.
+
     Args:
         sticker (:obj:`str` | :term:`file object` | :obj:`bytes` | :class:`pathlib.Path`): The
             added sticker. |uploadinputnopath| Animated and video stickers can't be uploaded via
             HTTP URL.
         emoji_list (Sequence[:obj:`str`]): Sequence of
             :tg-const:`telegram.constants.StickerLimit.MIN_STICKER_EMOJI` -
             :tg-const:`telegram.constants.StickerLimit.MAX_STICKER_EMOJI` emoji associated with the
@@ -48,14 +52,21 @@
             placed on faces. For ":tg-const:`telegram.constants.StickerType.MASK`" stickers only.
         keywords (Sequence[:obj:`str`], optional): Sequence of
             0-:tg-const:`telegram.constants.StickerLimit.MAX_SEARCH_KEYWORDS` search keywords
             for the sticker with the total length of up to
             :tg-const:`telegram.constants.StickerLimit.MAX_KEYWORD_LENGTH` characters. For
             ":tg-const:`telegram.constants.StickerType.REGULAR`" and
             ":tg-const:`telegram.constants.StickerType.CUSTOM_EMOJI`" stickers only.
+        format (:obj:`str`): Format of the added sticker, must be one of
+            :tg-const:`telegram.constants.StickerFormat.STATIC` for a
+            ``.WEBP`` or ``.PNG`` image, :tg-const:`telegram.constants.StickerFormat.ANIMATED`
+            for a ``.TGS`` animation, :tg-const:`telegram.constants.StickerFormat.VIDEO` for a WEBM
+            video.
+
+            .. versionadded:: 21.1
 
     Attributes:
         sticker (:obj:`str` | :class:`telegram.InputFile`): The added sticker.
         emoji_list (Tuple[:obj:`str`]): Tuple of
             :tg-const:`telegram.constants.StickerLimit.MIN_STICKER_EMOJI` -
             :tg-const:`telegram.constants.StickerLimit.MAX_STICKER_EMOJI` emoji associated with the
             sticker.
@@ -63,23 +74,31 @@
             placed on faces. For ":tg-const:`telegram.constants.StickerType.MASK`" stickers only.
         keywords (Tuple[:obj:`str`]): Optional. Tuple of
             0-:tg-const:`telegram.constants.StickerLimit.MAX_SEARCH_KEYWORDS` search keywords
             for the sticker with the total length of up to
             :tg-const:`telegram.constants.StickerLimit.MAX_KEYWORD_LENGTH` characters. For
             ":tg-const:`telegram.constants.StickerType.REGULAR`" and
             ":tg-const:`telegram.constants.StickerType.CUSTOM_EMOJI`" stickers only.
+            ":tg-const:`telegram.constants.StickerType.CUSTOM_EMOJI`" stickers only.
+        format (:obj:`str`): Format of the added sticker, must be one of
+            :tg-const:`telegram.constants.StickerFormat.STATIC` for a
+            ``.WEBP`` or ``.PNG`` image, :tg-const:`telegram.constants.StickerFormat.ANIMATED`
+            for a ``.TGS`` animation, :tg-const:`telegram.constants.StickerFormat.VIDEO` for a WEBM
+            video.
 
+            .. versionadded:: 21.1
     """
 
-    __slots__ = ("emoji_list", "keywords", "mask_position", "sticker")
+    __slots__ = ("emoji_list", "format", "keywords", "mask_position", "sticker")
 
     def __init__(
         self,
         sticker: FileInput,
         emoji_list: Sequence[str],
+        format: str,  # pylint: disable=redefined-builtin
         mask_position: Optional[MaskPosition] = None,
         keywords: Optional[Sequence[str]] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
@@ -87,11 +106,12 @@
         # things to work in local mode.
         self.sticker: Union[str, InputFile] = parse_file_input(
             sticker,
             local_mode=True,
             attach=True,
         )
         self.emoji_list: Tuple[str, ...] = parse_sequence_arg(emoji_list)
+        self.format: str = format
         self.mask_position: Optional[MaskPosition] = mask_position
         self.keywords: Tuple[str, ...] = parse_sequence_arg(keywords)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/location.py` & `python-telegram-bot-raw-21.1/telegram/_files/location.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/photosize.py` & `python-telegram-bot-raw-21.1/telegram/_files/photosize.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/sticker.py` & `python-telegram-bot-raw-21.1/telegram/_files/sticker.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from telegram._files._basethumbedmedium import _BaseThumbedMedium
 from telegram._files.file import File
 from telegram._files.photosize import PhotoSize
 from telegram._telegramobject import TelegramObject
 from telegram._utils import enum
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.types import JSONDict
+from telegram._utils.warnings import warn
+from telegram.warnings import PTBDeprecationWarning
 
 if TYPE_CHECKING:
     from telegram import Bot
 
 
 class Sticker(_BaseThumbedMedium):
     """This object represents a sticker.
@@ -223,24 +225,36 @@
         As of v13.11 :paramref:`is_video` is a required argument and therefore the order of the
         arguments had to be changed. Use keyword arguments to make sure that the arguments are
         passed correctly.
 
     .. versionchanged:: 20.0
         The parameter ``contains_masks`` has been removed. Use :paramref:`sticker_type` instead.
 
+
+    .. versionchanged:: 21.1
+        The parameters ``is_video`` and ``is_animated`` are deprecated and now made optional. Thus,
+        the order of the arguments had to be changed.
+
     .. versionchanged:: 20.5
        |removed_thumb_note|
 
     Args:
         name (:obj:`str`): Sticker set name.
         title (:obj:`str`): Sticker set title.
         is_animated (:obj:`bool`): :obj:`True`, if the sticker set contains animated stickers.
-        is_video (:obj:`bool`): :obj:`True`, if the sticker set contains video stickers.
 
+            .. deprecated:: 21.1
+                Bot API 7.2 deprecated this field. This parameter will be removed in a future
+                version of the library.
+        is_video (:obj:`bool`): :obj:`True`, if the sticker set contains video stickers.
             .. versionadded:: 13.11
+
+            .. deprecated:: 21.1
+                Bot API 7.2 deprecated this field. This parameter will be removed in a future
+                version of the library.
         stickers (Sequence[:class:`telegram.Sticker`]): List of all set stickers.
 
             .. versionchanged:: 20.0
                 |sequenceclassargs|
 
         sticker_type (:obj:`str`): Type of stickers in the set, currently one of
             :attr:`telegram.Sticker.REGULAR`, :attr:`telegram.Sticker.MASK`,
@@ -252,17 +266,24 @@
 
             .. versionadded:: 20.2
 
     Attributes:
         name (:obj:`str`): Sticker set name.
         title (:obj:`str`): Sticker set title.
         is_animated (:obj:`bool`): :obj:`True`, if the sticker set contains animated stickers.
-        is_video (:obj:`bool`): :obj:`True`, if the sticker set contains video stickers.
 
+            .. deprecated:: 21.1
+                Bot API 7.2 deprecated this field. This parameter will be removed in a future
+                version of the library.
+        is_video (:obj:`bool`): :obj:`True`, if the sticker set contains video stickers.
             .. versionadded:: 13.11
+
+            .. deprecated:: 21.1
+                Bot API 7.2 deprecated this field. This parameter will be removed in a future
+                version of the library.
         stickers (Tuple[:class:`telegram.Sticker`]): List of all set stickers.
 
             .. versionchanged:: 20.0
                 |tupleclassattrs|
 
         sticker_type (:obj:`str`): Type of stickers in the set, currently one of
             :attr:`telegram.Sticker.REGULAR`, :attr:`telegram.Sticker.MASK`,
@@ -285,32 +306,38 @@
         "title",
     )
 
     def __init__(
         self,
         name: str,
         title: str,
-        is_animated: bool,
         stickers: Sequence[Sticker],
-        is_video: bool,
         sticker_type: str,
+        is_animated: Optional[bool] = None,
+        is_video: Optional[bool] = None,
         thumbnail: Optional[PhotoSize] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.name: str = name
         self.title: str = title
-        self.is_animated: bool = is_animated
-        self.is_video: bool = is_video
         self.stickers: Tuple[Sticker, ...] = parse_sequence_arg(stickers)
         self.sticker_type: str = sticker_type
         # Optional
-
         self.thumbnail: Optional[PhotoSize] = thumbnail
+        if is_animated is not None or is_video is not None:
+            warn(
+                "The parameters `is_animated` and `is_video` are deprecated and will be removed "
+                "in a future version.",
+                PTBDeprecationWarning,
+                stacklevel=2,
+            )
+        self.is_animated: Optional[bool] = is_animated
+        self.is_video: Optional[bool] = is_video
         self._id_attrs = (self.name,)
 
         self._freeze()
 
     @classmethod
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["StickerSet"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/venue.py` & `python-telegram-bot-raw-21.1/telegram/_files/venue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/video.py` & `python-telegram-bot-raw-21.1/telegram/_files/video.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/videonote.py` & `python-telegram-bot-raw-21.1/telegram/_files/videonote.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_files/voice.py` & `python-telegram-bot-raw-21.1/telegram/_files/voice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_forcereply.py` & `python-telegram-bot-raw-21.1/telegram/_forcereply.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_forumtopic.py` & `python-telegram-bot-raw-21.1/telegram/_forumtopic.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_games/callbackgame.py` & `python-telegram-bot-raw-21.1/telegram/_games/callbackgame.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_games/game.py` & `python-telegram-bot-raw-21.1/telegram/_games/game.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_games/gamehighscore.py` & `python-telegram-bot-raw-21.1/telegram/_games/gamehighscore.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_giveaway.py` & `python-telegram-bot-raw-21.1/telegram/_giveaway.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinekeyboardbutton.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinekeyboardbutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinekeyboardmarkup.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinekeyboardmarkup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequery.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresult.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresult.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultarticle.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultarticle.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultaudio.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultaudio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedaudio.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedaudio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcacheddocument.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcacheddocument.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedgif.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedgif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedphoto.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedsticker.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedsticker.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedvideo.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedvideo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcachedvoice.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedvoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultcontact.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcontact.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultdocument.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultdocument.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultgame.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultgame.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultgif.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultgif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultlocation.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultlocation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultmpeg4gif.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultmpeg4gif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultphoto.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultsbutton.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultsbutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultvenue.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvenue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultvideo.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvideo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inlinequeryresultvoice.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inputcontactmessagecontent.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inputcontactmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inputinvoicemessagecontent.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inputinvoicemessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inputlocationmessagecontent.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inputlocationmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inputmessagecontent.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inputmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inputtextmessagecontent.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inputtextmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_inline/inputvenuemessagecontent.py` & `python-telegram-bot-raw-21.1/telegram/_inline/inputvenuemessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_keyboardbutton.py` & `python-telegram-bot-raw-21.1/telegram/_keyboardbutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_keyboardbuttonpolltype.py` & `python-telegram-bot-raw-21.1/telegram/_keyboardbuttonpolltype.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_keyboardbuttonrequest.py` & `python-telegram-bot-raw-21.1/telegram/_keyboardbuttonrequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains two objects to request chats/users."""
+
 from typing import TYPE_CHECKING, Optional
 
 from telegram._chatadministratorrights import ChatAdministratorRights
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
@@ -52,14 +53,24 @@
         max_quantity (:obj:`int`, optional): The maximum number of users to be selected;
             :tg-const:`telegram.constants.KeyboardButtonRequestUsersLimit.MIN_QUANTITY` -
             :tg-const:`telegram.constants.KeyboardButtonRequestUsersLimit.MAX_QUANTITY`.
             Defaults to :tg-const:`telegram.constants.KeyboardButtonRequestUsersLimit.MIN_QUANTITY`
             .
 
             .. versionadded:: 20.8
+        request_name (:obj:`bool`, optional): Pass :obj:`True` to request the users' first and last
+            name.
+
+            .. versionadded:: 21.1
+        request_username (:obj:`bool`, optional): Pass :obj:`True` to request the users' username.
+
+            .. versionadded:: 21.1
+        request_photo (:obj:`bool`, optional): Pass :obj:`True` to request the users' photo.
+
+            .. versionadded:: 21.1
 
     Attributes:
         request_id (:obj:`int`): Identifier of the request.
         user_is_bot (:obj:`bool`): Optional. Pass :obj:`True` to request a bot, pass :obj:`False`
             to request a regular user. If not specified, no additional restrictions are applied.
         user_is_premium (:obj:`bool`): Optional. Pass :obj:`True` to request a premium user, pass
             :obj:`False` to request a non-premium user. If not specified, no additional
@@ -67,40 +78,60 @@
         max_quantity (:obj:`int`): Optional. The maximum number of users to be selected;
             :tg-const:`telegram.constants.KeyboardButtonRequestUsersLimit.MIN_QUANTITY` -
             :tg-const:`telegram.constants.KeyboardButtonRequestUsersLimit.MAX_QUANTITY`.
             Defaults to :tg-const:`telegram.constants.KeyboardButtonRequestUsersLimit.MIN_QUANTITY`
             .
 
             .. versionadded:: 20.8
+        request_name (:obj:`bool`): Optional. Pass :obj:`True` to request the users' first and last
+            name.
+
+            .. versionadded:: 21.1
+        request_username (:obj:`bool`): Optional. Pass :obj:`True` to request the users' username.
+
+            .. versionadded:: 21.1
+        request_photo (:obj:`bool`): Optional. Pass :obj:`True` to request the users' photo.
+
+            .. versionadded:: 21.1
+
     """
 
     __slots__ = (
         "max_quantity",
         "request_id",
+        "request_name",
+        "request_photo",
+        "request_username",
         "user_is_bot",
         "user_is_premium",
     )
 
     def __init__(
         self,
         request_id: int,
         user_is_bot: Optional[bool] = None,
         user_is_premium: Optional[bool] = None,
         max_quantity: Optional[int] = None,
+        request_name: Optional[bool] = None,
+        request_username: Optional[bool] = None,
+        request_photo: Optional[bool] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.request_id: int = request_id
 
         # Optionals
         self.user_is_bot: Optional[bool] = user_is_bot
         self.user_is_premium: Optional[bool] = user_is_premium
         self.max_quantity: Optional[int] = max_quantity
+        self.request_name: Optional[bool] = request_name
+        self.request_username: Optional[bool] = request_username
+        self.request_photo: Optional[bool] = request_photo
 
         self._id_attrs = (self.request_id,)
 
         self._freeze()
 
 
 class KeyboardButtonRequestChat(TelegramObject):
@@ -134,58 +165,82 @@
             restrictions are applied.
         bot_administrator_rights (:class:`ChatAdministratorRights`, optional): Specifies the
             required administrator rights of the bot in the chat. The rights must be a subset of
             :paramref:`user_administrator_rights`. If not specified, no additional restrictions are
             applied.
         bot_is_member (:obj:`bool`, optional): Pass :obj:`True` to request a chat with the bot
             as a member. Otherwise, no additional restrictions are applied.
+        request_title (:obj:`bool`, optional): Pass :obj:`True` to request the chat's title.
+
+            .. versionadded:: 21.1
+        request_username (:obj:`bool`, optional): Pass :obj:`True` to request the chat's username.
+
+            .. versionadded:: 21.1
+        request_photo (:obj:`bool`, optional): Pass :obj:`True` to request the chat's photo.
+
+            .. versionadded:: 21.1
     Attributes:
         request_id (:obj:`int`): Identifier of the request.
         chat_is_channel (:obj:`bool`): Pass :obj:`True` to request a channel chat, pass
             :obj:`False` to request a group or a supergroup chat.
         chat_is_forum (:obj:`bool`): Optional. Pass :obj:`True` to request a forum supergroup, pass
             :obj:`False` to request a non-forum chat. If not specified, no additional
             restrictions are applied.
-        chat_has_username (:obj:`bool`, optional): Pass :obj:`True` to request a supergroup or a
+        chat_has_username (:obj:`bool`): Optional. Pass :obj:`True` to request a supergroup or a
             channel with a username, pass :obj:`False` to request a chat without a username. If
             not specified, no additional restrictions are applied.
         chat_is_created (:obj:`bool`) Optional. Pass :obj:`True` to request a chat owned by the
             user. Otherwise, no additional restrictions are applied.
         user_administrator_rights (:class:`ChatAdministratorRights`) Optional. Specifies the
             required administrator rights of the user in the chat. If not specified, no additional
             restrictions are applied.
         bot_administrator_rights (:class:`ChatAdministratorRights`) Optional. Specifies the
             required administrator rights of the bot in the chat. The rights must be a subset of
             :attr:`user_administrator_rights`. If not specified, no additional restrictions are
             applied.
         bot_is_member (:obj:`bool`) Optional. Pass :obj:`True` to request a chat with the bot
             as a member. Otherwise, no additional restrictions are applied.
+        request_title (:obj:`bool`): Optional. Pass :obj:`True` to request the chat's title.
+
+            .. versionadded:: 21.1
+        request_username (:obj:`bool`): Optional. Pass :obj:`True` to request the chat's username.
+
+            .. versionadded:: 21.1
+        request_photo (:obj:`bool`): Optional. Pass :obj:`True` to request the chat's photo.
+
+            .. versionadded:: 21.1
     """
 
     __slots__ = (
         "bot_administrator_rights",
         "bot_is_member",
         "chat_has_username",
         "chat_is_channel",
         "chat_is_created",
         "chat_is_forum",
         "request_id",
+        "request_photo",
+        "request_title",
+        "request_username",
         "user_administrator_rights",
     )
 
     def __init__(
         self,
         request_id: int,
         chat_is_channel: bool,
         chat_is_forum: Optional[bool] = None,
         chat_has_username: Optional[bool] = None,
         chat_is_created: Optional[bool] = None,
         user_administrator_rights: Optional[ChatAdministratorRights] = None,
         bot_administrator_rights: Optional[ChatAdministratorRights] = None,
         bot_is_member: Optional[bool] = None,
+        request_title: Optional[bool] = None,
+        request_username: Optional[bool] = None,
+        request_photo: Optional[bool] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # required
         self.request_id: int = request_id
         self.chat_is_channel: bool = chat_is_channel
@@ -195,14 +250,17 @@
         self.chat_has_username: Optional[bool] = chat_has_username
         self.chat_is_created: Optional[bool] = chat_is_created
         self.user_administrator_rights: Optional[ChatAdministratorRights] = (
             user_administrator_rights
         )
         self.bot_administrator_rights: Optional[ChatAdministratorRights] = bot_administrator_rights
         self.bot_is_member: Optional[bool] = bot_is_member
+        self.request_title: Optional[bool] = request_title
+        self.request_username: Optional[bool] = request_username
+        self.request_photo: Optional[bool] = request_photo
 
         self._id_attrs = (self.request_id,)
 
         self._freeze()
 
     @classmethod
     def de_json(
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_linkpreviewoptions.py` & `python-telegram-bot-raw-21.1/telegram/_linkpreviewoptions.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_loginurl.py` & `python-telegram-bot-raw-21.1/telegram/_loginurl.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_menubutton.py` & `python-telegram-bot-raw-21.1/telegram/_menubutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_message.py` & `python-telegram-bot-raw-21.1/telegram/_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Message."""
+
 import datetime
 import re
 from html import escape
 from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Tuple, TypedDict, Union
 
 from telegram._chat import Chat
 from telegram._chatboost import ChatBoostAdded
@@ -297,14 +298,19 @@
 
             .. versionchanged:: 20.3
                 |datetime_localization|
         has_protected_content (:obj:`bool`, optional): :obj:`True`, if the message can't be
             forwarded.
 
             .. versionadded:: 13.9
+        is_from_offline (:obj:`bool`, optional): :obj:`True`, if the message was sent
+            by an implicit action, for example, as an away or a greeting business message,
+            or as a scheduled message.
+
+            .. versionadded:: 21.1
         media_group_id (:obj:`str`, optional): The unique identifier of a media message group this
             message belongs to.
         text (:obj:`str`, optional): For text messages, the actual UTF-8 text of the message,
             0-:tg-const:`telegram.constants.MessageLimit.MAX_TEXT_LENGTH` characters.
         entities (Sequence[:class:`telegram.MessageEntity`], optional): For text messages, special
             entities like usernames, URLs, bot commands, etc. that appear in the text. See
             :attr:`parse_entity` and :attr:`parse_entities` methods for how to use properly.
@@ -530,14 +536,26 @@
             the chat.
 
             .. versionadded:: 21.0
         sender_boost_count (:obj:`int`, optional): If the sender of the
             message boosted the chat, the number of boosts added by the user.
 
             .. versionadded:: 21.0
+        business_connection_id (:obj:`str`, optional): Unique identifier of the business connection
+            from which the message was received. If non-empty, the message belongs to a chat of the
+            corresponding business account that is independent from any potential bot chat which
+            might share the same identifier.
+
+            .. versionadded:: 21.1
+
+        sender_business_bot (:obj:`telegram.User`, optional): The bot that actually sent the
+            message on behalf of the business account. Available only for outgoing messages sent
+            on behalf of the connected business account.
+
+            .. versionadded:: 21.1
 
     Attributes:
         message_id (:obj:`int`): Unique message identifier inside this chat.
         from_user (:class:`telegram.User`): Optional. Sender of the message; empty for messages
             sent to channels. For backward compatibility, this will contain a fake sender user in
             non-channel chats, if the message was sent on behalf of a chat.
         sender_chat (:class:`telegram.Chat`): Optional. Sender of the message, sent on behalf of a
@@ -564,14 +582,19 @@
 
             .. versionchanged:: 20.3
                 |datetime_localization|
         has_protected_content (:obj:`bool`): Optional. :obj:`True`, if the message can't be
             forwarded.
 
             .. versionadded:: 13.9
+        is_from_offline (:obj:`bool`): Optional. :obj:`True`, if the message was sent
+            by an implicit action, for example, as an away or a greeting business message,
+            or as a scheduled message.
+
+            .. versionadded:: 21.1
         media_group_id (:obj:`str`): Optional. The unique identifier of a media message group this
             message belongs to.
         text (:obj:`str`): Optional. For text messages, the actual UTF-8 text of the message,
             0-:tg-const:`telegram.constants.MessageLimit.MAX_TEXT_LENGTH` characters.
         entities (Tuple[:class:`telegram.MessageEntity`]): Optional. For text messages, special
             entities like usernames, URLs, bot commands, etc. that appear in the text. See
             :attr:`parse_entity` and :attr:`parse_entities` methods for how to use properly.
@@ -813,30 +836,47 @@
 
             .. versionadded:: 21.0
         sender_boost_count (:obj:`int`): Optional. If the sender of the
             message boosted the chat, the number of boosts added by the user.
 
             .. versionadded:: 21.0
 
+        business_connection_id (:obj:`str`): Optional. Unique identifier of the business connection
+            from which the message was received. If non-empty, the message belongs to a chat of the
+            corresponding business account that is independent from any potential bot chat which
+            might share the same identifier.
+
+            .. versionadded:: 21.1
+
+        sender_business_bot (:obj:`telegram.User`): Optional. The bot that actually sent the
+            message on behalf of the business account. Available only for outgoing messages sent
+            on behalf of the connected business account.
+
+            .. versionadded:: 21.1
+
     .. |custom_emoji_no_md1_support| replace:: Since custom emoji entities are not supported by
        :attr:`~telegram.constants.ParseMode.MARKDOWN`, this method now raises a
        :exc:`ValueError` when encountering a custom emoji.
 
     .. |blockquote_no_md1_support| replace:: Since block quotation entities are not supported
        by :attr:`~telegram.constants.ParseMode.MARKDOWN`, this method now raises a
        :exc:`ValueError` when encountering a block quotation.
+
+    .. |reply_same_thread| replace:: If :paramref:`message_thread_id` is not provided,
+       this will reply to the same thread (topic) of the original message.
     """
 
     # fmt: on
     __slots__ = (
         "_effective_attachment",
         "animation",
         "audio",
         "author_signature",
         "boost_added",
+        "business_connection_id",
         "caption",
         "caption_entities",
         "channel_chat_created",
         "chat_shared",
         "connected_website",
         "contact",
         "delete_chat_photo",
@@ -859,14 +899,15 @@
         "giveaway_created",
         "giveaway_winners",
         "group_chat_created",
         "has_media_spoiler",
         "has_protected_content",
         "invoice",
         "is_automatic_forward",
+        "is_from_offline",
         "is_topic_message",
         "left_chat_member",
         "link_preview_options",
         "location",
         "media_group_id",
         "message_auto_delete_timer_changed",
         "message_thread_id",
@@ -881,14 +922,15 @@
         "poll",
         "proximity_alert_triggered",
         "quote",
         "reply_markup",
         "reply_to_message",
         "reply_to_story",
         "sender_boost_count",
+        "sender_business_bot",
         "sender_chat",
         "sticker",
         "story",
         "successful_payment",
         "supergroup_chat_created",
         "text",
         "users_shared",
@@ -980,14 +1022,17 @@
         link_preview_options: Optional[LinkPreviewOptions] = None,
         external_reply: Optional["ExternalReplyInfo"] = None,
         quote: Optional["TextQuote"] = None,
         forward_origin: Optional["MessageOrigin"] = None,
         reply_to_story: Optional[Story] = None,
         boost_added: Optional[ChatBoostAdded] = None,
         sender_boost_count: Optional[int] = None,
+        business_connection_id: Optional[str] = None,
+        sender_business_bot: Optional[User] = None,
+        is_from_offline: Optional[bool] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(chat=chat, message_id=message_id, date=date, api_kwargs=api_kwargs)
 
         with self._unfrozen():
             # Required
@@ -1075,14 +1120,17 @@
             self.link_preview_options: Optional[LinkPreviewOptions] = link_preview_options
             self.external_reply: Optional[ExternalReplyInfo] = external_reply
             self.quote: Optional[TextQuote] = quote
             self.forward_origin: Optional[MessageOrigin] = forward_origin
             self.reply_to_story: Optional[Story] = reply_to_story
             self.boost_added: Optional[ChatBoostAdded] = boost_added
             self.sender_boost_count: Optional[int] = sender_boost_count
+            self.business_connection_id: Optional[str] = business_connection_id
+            self.sender_business_bot: Optional[User] = sender_business_bot
+            self.is_from_offline: Optional[bool] = is_from_offline
 
             self._effective_attachment = DEFAULT_NONE
 
             self._id_attrs = (self.message_id, self.chat)
 
     @property
     def chat_id(self) -> int:
@@ -1217,14 +1265,15 @@
             data.get("link_preview_options"), bot
         )
         data["external_reply"] = ExternalReplyInfo.de_json(data.get("external_reply"), bot)
         data["quote"] = TextQuote.de_json(data.get("quote"), bot)
         data["forward_origin"] = MessageOrigin.de_json(data.get("forward_origin"), bot)
         data["reply_to_story"] = Story.de_json(data.get("reply_to_story"), bot)
         data["boost_added"] = ChatBoostAdded.de_json(data.get("boost_added"), bot)
+        data["sender_business_bot"] = User.de_json(data.get("sender_business_bot"), bot)
 
         api_kwargs = {}
         # This is a deprecated field that TG still returns for backwards compatibility
         # Let's filter it out to speed up the de-json process
         for key in (
             "user_shared",
             "forward_from",
@@ -1531,14 +1580,23 @@
             effective_reply_parameters = effective_do_quote["reply_parameters"]
             chat_id = effective_do_quote["chat_id"]
         else:
             effective_reply_parameters = self._quote(effective_do_quote)
 
         return chat_id, effective_reply_parameters
 
+    def _parse_message_thread_id(
+        self,
+        chat_id: Union[str, int],
+        message_thread_id: Optional[int] = None,
+    ) -> Optional[int]:
+        return message_thread_id or (
+            self.message_thread_id if chat_id in {self.chat_id, self.chat.username} else None
+        )
+
     async def reply_text(
         self,
         text: str,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         entities: Optional[Sequence["MessageEntity"]] = None,
@@ -1556,18 +1614,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_message(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_message(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_message`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -1577,14 +1644,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_message(
             chat_id=chat_id,
             text=text,
             parse_mode=parse_mode,
             disable_web_page_preview=disable_web_page_preview,
             link_preview_options=link_preview_options,
             disable_notification=disable_notification,
@@ -1595,14 +1663,15 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_markdown(
         self,
         text: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
@@ -1623,23 +1692,28 @@
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
             await bot.send_message(
                 update.effective_message.chat_id,
+                message_thread_id=update.effective_message.message_thread_id,
                 parse_mode=ParseMode.MARKDOWN,
+                business_connection_id=self.business_connection_id,
                 *args,
                 **kwargs,
             )
 
         Sends a message with Markdown version 1 formatting.
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_message`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Note:
             :tg-const:`telegram.constants.ParseMode.MARKDOWN` is a legacy mode, retained by
             Telegram for backward compatibility. You should use :meth:`reply_markdown_v2` instead.
 
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
@@ -1652,14 +1726,15 @@
 
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_message(
             chat_id=chat_id,
             text=text,
             parse_mode=ParseMode.MARKDOWN,
             disable_web_page_preview=disable_web_page_preview,
             link_preview_options=link_preview_options,
             disable_notification=disable_notification,
@@ -1670,14 +1745,15 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_markdown_v2(
         self,
         text: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
@@ -1698,23 +1774,28 @@
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
             await bot.send_message(
                 update.effective_message.chat_id,
+                message_thread_id=update.effective_message.message_thread_id,
                 parse_mode=ParseMode.MARKDOWN_V2,
+                business_connection_id=self.business_connection_id,
                 *args,
                 **kwargs,
             )
 
         Sends a message with markdown version 2 formatting.
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_message`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -1723,14 +1804,15 @@
 
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_message(
             chat_id=chat_id,
             text=text,
             parse_mode=ParseMode.MARKDOWN_V2,
             disable_web_page_preview=disable_web_page_preview,
             link_preview_options=link_preview_options,
             disable_notification=disable_notification,
@@ -1741,14 +1823,15 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_html(
         self,
         text: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
@@ -1769,23 +1852,28 @@
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
             await bot.send_message(
                 update.effective_message.chat_id,
+                message_thread_id=update.effective_message.message_thread_id,
                 parse_mode=ParseMode.HTML,
+                business_connection_id=self.business_connection_id,
                 *args,
                 **kwargs,
             )
 
         Sends a message with HTML formatting.
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_message`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -1794,14 +1882,15 @@
 
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_message(
             chat_id=chat_id,
             text=text,
             parse_mode=ParseMode.HTML,
             disable_web_page_preview=disable_web_page_preview,
             link_preview_options=link_preview_options,
             disable_notification=disable_notification,
@@ -1812,14 +1901,15 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_media_group(
         self,
         media: Sequence[
             Union["InputMediaAudio", "InputMediaDocument", "InputMediaPhoto", "InputMediaVideo"]
         ],
@@ -1839,18 +1929,27 @@
         api_kwargs: Optional[JSONDict] = None,
         caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
     ) -> Tuple["Message", ...]:
         """Shortcut for::
 
-             await bot.send_media_group(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_media_group(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_media_group`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -1862,14 +1961,15 @@
 
         Raises:
             :class:`telegram.error.TelegramError`
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_media_group(
             chat_id=chat_id,
             media=media,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
@@ -1878,14 +1978,15 @@
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_photo(
         self,
         photo: Union[FileInput, "PhotoSize"],
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
@@ -1906,18 +2007,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_photo(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_photo(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_photo`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -1927,14 +2037,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_photo(
             chat_id=chat_id,
             photo=photo,
             caption=caption,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
             reply_markup=reply_markup,
@@ -1946,14 +2057,15 @@
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             has_spoiler=has_spoiler,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_audio(
         self,
         audio: Union[FileInput, "Audio"],
         duration: Optional[int] = None,
         performer: Optional[str] = None,
@@ -1977,18 +2089,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_audio(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_audio(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_audio`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -1998,14 +2119,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_audio(
             chat_id=chat_id,
             audio=audio,
             duration=duration,
             performer=performer,
             title=title,
             caption=caption,
@@ -2020,14 +2142,15 @@
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             thumbnail=thumbnail,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_document(
         self,
         document: Union[FileInput, "Document"],
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
@@ -2049,18 +2172,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_document(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_document(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_document`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2070,14 +2202,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_document(
             chat_id=chat_id,
             document=document,
             filename=filename,
             caption=caption,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
@@ -2090,14 +2223,15 @@
             api_kwargs=api_kwargs,
             disable_content_type_detection=disable_content_type_detection,
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             thumbnail=thumbnail,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_animation(
         self,
         animation: Union[FileInput, "Animation"],
         duration: Optional[int] = None,
         width: Optional[int] = None,
@@ -2122,18 +2256,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_animation(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_animation(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_animation`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2143,14 +2286,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_animation(
             chat_id=chat_id,
             animation=animation,
             duration=duration,
             width=width,
             height=height,
             caption=caption,
@@ -2166,14 +2310,15 @@
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             has_spoiler=has_spoiler,
             thumbnail=thumbnail,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_sticker(
         self,
         sticker: Union[FileInput, "Sticker"],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
@@ -2190,18 +2335,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_sticker(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_sticker(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_sticker`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2211,14 +2365,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_sticker(
             chat_id=chat_id,
             sticker=sticker,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
             reply_markup=reply_markup,
             read_timeout=read_timeout,
@@ -2226,14 +2381,15 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             emoji=emoji,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_video(
         self,
         video: Union[FileInput, "Video"],
         duration: Optional[int] = None,
         caption: Optional[str] = None,
@@ -2259,18 +2415,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_video(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_video(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_video`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2280,14 +2445,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_video(
             chat_id=chat_id,
             video=video,
             duration=duration,
             caption=caption,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
@@ -2304,14 +2470,15 @@
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             has_spoiler=has_spoiler,
             thumbnail=thumbnail,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_video_note(
         self,
         video_note: Union[FileInput, "VideoNote"],
         duration: Optional[int] = None,
         length: Optional[int] = None,
@@ -2331,18 +2498,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_video_note(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_video_note(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_video_note`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2352,14 +2528,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_video_note(
             chat_id=chat_id,
             video_note=video_note,
             duration=duration,
             length=length,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
@@ -2370,14 +2547,15 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             thumbnail=thumbnail,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_voice(
         self,
         voice: Union[FileInput, "Voice"],
         duration: Optional[int] = None,
         caption: Optional[str] = None,
@@ -2398,18 +2576,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_voice(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_voice(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_voice`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2419,14 +2606,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_voice(
             chat_id=chat_id,
             voice=voice,
             duration=duration,
             caption=caption,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
@@ -2438,14 +2626,15 @@
             parse_mode=parse_mode,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_location(
         self,
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
@@ -2467,18 +2656,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_location(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_location(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_location`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2488,14 +2686,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_location(
             chat_id=chat_id,
             latitude=latitude,
             longitude=longitude,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
             reply_markup=reply_markup,
@@ -2508,14 +2707,15 @@
             api_kwargs=api_kwargs,
             horizontal_accuracy=horizontal_accuracy,
             heading=heading,
             proximity_alert_radius=proximity_alert_radius,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_venue(
         self,
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
         title: Optional[str] = None,
@@ -2539,18 +2739,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_venue(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_venue(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_venue`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2560,14 +2769,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_venue(
             chat_id=chat_id,
             latitude=latitude,
             longitude=longitude,
             title=title,
             address=address,
             foursquare_id=foursquare_id,
@@ -2582,14 +2792,15 @@
             foursquare_type=foursquare_type,
             api_kwargs=api_kwargs,
             google_place_id=google_place_id,
             google_place_type=google_place_type,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_contact(
         self,
         phone_number: Optional[str] = None,
         first_name: Optional[str] = None,
         last_name: Optional[str] = None,
@@ -2609,18 +2820,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_contact(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_contact(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_contact`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2630,14 +2850,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_contact(
             chat_id=chat_id,
             phone_number=phone_number,
             first_name=first_name,
             last_name=last_name,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
@@ -2648,14 +2869,15 @@
             pool_timeout=pool_timeout,
             contact=contact,
             vcard=vcard,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_poll(
         self,
         question: str,
         options: Sequence[str],
         is_anonymous: Optional[bool] = None,
@@ -2682,18 +2904,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_poll(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_poll(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_poll`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2703,14 +2934,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_poll(
             chat_id=chat_id,
             question=question,
             options=options,
             is_anonymous=is_anonymous,
             type=type,
             allows_multiple_answers=allows_multiple_answers,
@@ -2728,14 +2960,15 @@
             open_period=open_period,
             close_date=close_date,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             explanation_entities=explanation_entities,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_dice(
         self,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         emoji: Optional[str] = None,
@@ -2751,18 +2984,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_dice(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_dice(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_dice`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2772,28 +3014,30 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_dice(
             chat_id=chat_id,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
             reply_markup=reply_markup,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             emoji=emoji,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_chat_action(
         self,
         action: str,
         message_thread_id: Optional[int] = None,
         *,
@@ -2801,33 +3045,43 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
-             await bot.send_chat_action(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_chat_action(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_chat_action`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         .. versionadded:: 13.2
 
         Returns:
             :obj:`bool`: On success, :obj:`True` is returned.
 
         """
         return await self.get_bot().send_chat_action(
             chat_id=self.chat_id,
-            message_thread_id=message_thread_id,
+            message_thread_id=self._parse_message_thread_id(self.chat_id, message_thread_id),
             action=action,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_game(
         self,
         game_short_name: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
@@ -2843,18 +3097,27 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_game(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_game(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 business_connection_id=self.business_connection_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_game`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
                 Mutually exclusive with :paramref:`quote`.
@@ -2866,28 +3129,30 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_game(
-            chat_id=chat_id,
+            chat_id=chat_id,  # type: ignore[arg-type]
             game_short_name=game_short_name,
             disable_notification=disable_notification,
             reply_parameters=effective_reply_parameters,
             reply_markup=reply_markup,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=self.business_connection_id,
         )
 
     async def reply_invoice(
         self,
         title: str,
         description: str,
         payload: str,
@@ -2923,18 +3188,26 @@
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
-             await bot.send_invoice(update.effective_message.chat_id, *args, **kwargs)
+             await bot.send_invoice(
+                 update.effective_message.chat_id,
+                 message_thread_id=update.effective_message.message_thread_id,
+                 *args,
+                 **kwargs,
+             )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_invoice`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Warning:
             As of API 5.2 :paramref:`start_parameter <telegram.Bot.send_invoice.start_parameter>`
             is an optional argument and therefore the
             order of the arguments had to be changed. Use keyword arguments to make sure that the
             arguments are passed correctly.
 
         .. versionadded:: 13.2
@@ -2956,14 +3229,15 @@
         Returns:
             :class:`telegram.Message`: On success, instance representing the message posted.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().send_invoice(
             chat_id=chat_id,
             title=title,
             description=description,
             payload=payload,
             provider_token=provider_token,
             currency=currency,
@@ -3126,21 +3400,25 @@
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> "MessageId":
         """Shortcut for::
 
              await bot.copy_message(
                  chat_id=message.chat.id,
+                 message_thread_id=update.effective_message.message_thread_id,
                  message_id=message_id,
                  *args,
                  **kwargs
              )
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.copy_message`.
 
+        .. versionchanged:: 21.1
+                |reply_same_thread|
+
         Keyword Args:
             quote (:obj:`bool`, optional): |reply_quote|
 
                 .. versionadded:: 13.1
                 .. deprecated:: 20.8
                     This argument is deprecated in favor of :paramref:`do_quote`
             do_quote (:obj:`bool` | :obj:`dict`, optional): |do_quote|
@@ -3151,14 +3429,15 @@
         Returns:
             :class:`telegram.MessageId`: On success, returns the MessageId of the sent message.
 
         """
         chat_id, effective_reply_parameters = await self._parse_quote_arguments(
             do_quote, quote, reply_to_message_id, reply_parameters
         )
+        message_thread_id = self._parse_message_thread_id(chat_id, message_thread_id)
         return await self.get_bot().copy_message(
             chat_id=chat_id,
             from_chat_id=from_chat_id,
             message_id=message_id,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_messageautodeletetimerchanged.py` & `python-telegram-bot-raw-21.1/telegram/_messageautodeletetimerchanged.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_messageentity.py` & `python-telegram-bot-raw-21.1/telegram/_messageentity.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_messageid.py` & `python-telegram-bot-raw-21.1/telegram/_messageid.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_messageorigin.py` & `python-telegram-bot-raw-21.1/telegram/_messageorigin.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_messagereactionupdated.py` & `python-telegram-bot-raw-21.1/telegram/_messagereactionupdated.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_passport/credentials.py` & `python-telegram-bot-raw-21.1/telegram/_passport/credentials.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_passport/data.py` & `python-telegram-bot-raw-21.1/telegram/_passport/data.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_passport/encryptedpassportelement.py` & `python-telegram-bot-raw-21.1/telegram/_passport/encryptedpassportelement.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,34 +56,34 @@
             Decrypted or encrypted data; available only for "personal_details", "passport",
             "driver_license", "identity_card", "internal_passport" and "address" types.
         phone_number (:obj:`str`, optional): User's verified phone number; available only for
             "phone_number" type.
         email (:obj:`str`, optional): User's verified email address; available only for "email"
             type.
         files (Sequence[:class:`telegram.PassportFile`], optional): Array of encrypted/decrypted
-            files with documents provided by the user; available only for "utility_bill", 
-            "bank_statement", "rental_agreement", "passport_registration" and 
+            files with documents provided by the user; available only for "utility_bill",
+            "bank_statement", "rental_agreement", "passport_registration" and
             "temporary_registration" types.
 
             .. versionchanged:: 20.0
                 |sequenceclassargs|
 
         front_side (:class:`telegram.PassportFile`, optional): Encrypted/decrypted file with the
             front side of the document, provided by the user; Available only for "passport",
             "driver_license", "identity_card" and "internal_passport".
         reverse_side (:class:`telegram.PassportFile`, optional): Encrypted/decrypted file with the
             reverse side of the document, provided by the user; Available only for
             "driver_license" and "identity_card".
         selfie (:class:`telegram.PassportFile`, optional): Encrypted/decrypted file with the
-            selfie of the user holding a document, provided by the user; available if requested for 
+            selfie of the user holding a document, provided by the user; available if requested for
             "passport", "driver_license", "identity_card" and "internal_passport".
         translation (Sequence[:class:`telegram.PassportFile`], optional): Array of
-            encrypted/decrypted files with translated versions of documents provided by the user; 
-            available if requested requested for "passport", "driver_license", "identity_card", 
-            "internal_passport", "utility_bill", "bank_statement", "rental_agreement", 
+            encrypted/decrypted files with translated versions of documents provided by the user;
+            available if requested requested for "passport", "driver_license", "identity_card",
+            "internal_passport", "utility_bill", "bank_statement", "rental_agreement",
             "passport_registration" and "temporary_registration" types.
 
             .. versionchanged:: 20.0
                 |sequenceclassargs|
 
     Attributes:
         type (:obj:`str`): Element type. One of "personal_details", "passport", "driver_license",
@@ -97,16 +97,16 @@
             Optional. Decrypted or encrypted data; available only for "personal_details",
             "passport", "driver_license", "identity_card", "internal_passport" and "address" types.
         phone_number (:obj:`str`): Optional. User's verified phone number; available only for
             "phone_number" type.
         email (:obj:`str`): Optional. User's verified email address; available only for "email"
             type.
         files (Tuple[:class:`telegram.PassportFile`]): Optional. Array of encrypted/decrypted
-            files with documents provided by the user; available only for "utility_bill", 
-            "bank_statement", "rental_agreement", "passport_registration" and 
+            files with documents provided by the user; available only for "utility_bill",
+            "bank_statement", "rental_agreement", "passport_registration" and
             "temporary_registration" types.
 
             .. versionchanged:: 20.0
 
                 * |tupleclassattrs|
                 * |alwaystuple|
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_passport/passportdata.py` & `python-telegram-bot-raw-21.1/telegram/_passport/passportdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_passport/passportelementerrors.py` & `python-telegram-bot-raw-21.1/telegram/_passport/passportelementerrors.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_passport/passportfile.py` & `python-telegram-bot-raw-21.1/telegram/_passport/passportfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,9 +199,10 @@
             file_id=self.file_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        file.set_credentials(self._credentials)
+        if self._credentials:
+            file.set_credentials(self._credentials)
         return file
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_payment/invoice.py` & `python-telegram-bot-raw-21.1/telegram/_payment/invoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_payment/labeledprice.py` & `python-telegram-bot-raw-21.1/telegram/_payment/labeledprice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_payment/orderinfo.py` & `python-telegram-bot-raw-21.1/telegram/_payment/orderinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_payment/precheckoutquery.py` & `python-telegram-bot-raw-21.1/telegram/_payment/precheckoutquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_payment/shippingaddress.py` & `python-telegram-bot-raw-21.1/telegram/_payment/shippingaddress.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_payment/shippingoption.py` & `python-telegram-bot-raw-21.1/telegram/_payment/shippingoption.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_payment/shippingquery.py` & `python-telegram-bot-raw-21.1/telegram/_payment/shippingquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_payment/successfulpayment.py` & `python-telegram-bot-raw-21.1/telegram/_payment/successfulpayment.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_poll.py` & `python-telegram-bot-raw-21.1/telegram/_poll.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_proximityalerttriggered.py` & `python-telegram-bot-raw-21.1/telegram/_proximityalerttriggered.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_reaction.py` & `python-telegram-bot-raw-21.1/telegram/_reaction.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_reply.py` & `python-telegram-bot-raw-21.1/telegram/_reply.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_replykeyboardmarkup.py` & `python-telegram-bot-raw-21.1/telegram/_replykeyboardmarkup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_replykeyboardremove.py` & `python-telegram-bot-raw-21.1/telegram/_replykeyboardremove.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_sentwebappmessage.py` & `python-telegram-bot-raw-21.1/telegram/_sentwebappmessage.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_story.py` & `python-telegram-bot-raw-21.1/telegram/_story.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_switchinlinequerychosenchat.py` & `python-telegram-bot-raw-21.1/telegram/_switchinlinequerychosenchat.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_telegramobject.py` & `python-telegram-bot-raw-21.1/telegram/_telegramobject.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_update.py` & `python-telegram-bot-raw-21.1/telegram/_update.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Update."""
 
-from typing import TYPE_CHECKING, Final, List, Optional
+from typing import TYPE_CHECKING, Final, List, Optional, Union
 
 from telegram import constants
+from telegram._business import BusinessConnection, BusinessMessagesDeleted
 from telegram._callbackquery import CallbackQuery
 from telegram._chatboost import ChatBoostRemoved, ChatBoostUpdated
 from telegram._chatjoinrequest import ChatJoinRequest
 from telegram._chatmemberupdated import ChatMemberUpdated
 from telegram._choseninlineresult import ChosenInlineResult
 from telegram._inline.inlinequery import InlineQuery
 from telegram._message import Message
@@ -130,14 +131,36 @@
             updates (see :meth:`telegram.Bot.get_updates`, :meth:`telegram.Bot.set_webhook`,
             :meth:`telegram.ext.Application.run_polling` and
             :meth:`telegram.ext.Application.run_webhook`). The updates are grouped and can be sent
             with delay up to a few minutes.
 
             .. versionadded:: 20.8
 
+        business_connection (:class:`telegram.BusinessConnection`, optional): The bot was connected
+            to or disconnected from a business account, or a user edited an existing connection
+            with the bot.
+
+            .. versionadded:: 21.1
+
+        business_message (:class:`telegram.Message`, optional): New non-service message
+            from a connected business account.
+
+            .. versionadded:: 21.1
+
+        edited_business_message (:class:`telegram.Message`, optional): New version of a message
+            from a connected business account.
+
+            .. versionadded:: 21.1
+
+        deleted_business_messages (:class:`telegram.BusinessMessagesDeleted`, optional): Messages
+            were deleted from a connected business account.
+
+            .. versionadded:: 21.1
+
+
     Attributes:
         update_id (:obj:`int`): The update's unique identifier. Update identifiers start from a
             certain positive number and increase sequentially. This ID becomes especially handy if
             you're using Webhooks, since it allows you to ignore repeated updates or to restore the
             correct update sequence, should they get out of order. If there are no new updates for
             at least a week, then identifier of the next update will be chosen randomly instead of
             sequentially.
@@ -215,26 +238,52 @@
             :paramref:`telegram.ext.Application.run_polling.allowed_updates` to receive these
             updates (see :meth:`telegram.Bot.get_updates`, :meth:`telegram.Bot.set_webhook`,
             :meth:`telegram.ext.Application.run_polling` and
             :meth:`telegram.ext.Application.run_webhook`). The updates are grouped and can be sent
             with delay up to a few minutes.
 
             .. versionadded:: 20.8
+
+        business_connection (:class:`telegram.BusinessConnection`): Optional. The bot was connected
+            to or disconnected from a business account, or a user edited an existing connection
+            with the bot.
+
+            .. versionadded:: 21.1
+
+        business_message (:class:`telegram.Message`): Optional. New non-service message
+            from a connected business account.
+
+            .. versionadded:: 21.1
+
+        edited_business_message (:class:`telegram.Message`): Optional. New version of a message
+            from a connected business account.
+
+            .. versionadded:: 21.1
+
+        deleted_business_messages (:class:`telegram.BusinessMessagesDeleted`): Optional. Messages
+            were deleted from a connected business account.
+
+            .. versionadded:: 21.1
     """
 
     __slots__ = (
         "_effective_chat",
         "_effective_message",
+        "_effective_sender",
         "_effective_user",
+        "business_connection",
+        "business_message",
         "callback_query",
         "channel_post",
         "chat_boost",
         "chat_join_request",
         "chat_member",
         "chosen_inline_result",
+        "deleted_business_messages",
+        "edited_business_message",
         "edited_channel_post",
         "edited_message",
         "inline_query",
         "message",
         "message_reaction",
         "message_reaction_count",
         "my_chat_member",
@@ -314,14 +363,30 @@
     """:const:`telegram.constants.UpdateType.MESSAGE_REACTION`
 
     .. versionadded:: 20.8"""
     MESSAGE_REACTION_COUNT: Final[str] = constants.UpdateType.MESSAGE_REACTION_COUNT
     """:const:`telegram.constants.UpdateType.MESSAGE_REACTION_COUNT`
 
     .. versionadded:: 20.8"""
+    BUSINESS_CONNECTION: Final[str] = constants.UpdateType.BUSINESS_CONNECTION
+    """:const:`telegram.constants.UpdateType.BUSINESS_CONNECTION`
+
+    .. versionadded:: 21.1"""
+    BUSINESS_MESSAGE: Final[str] = constants.UpdateType.BUSINESS_MESSAGE
+    """:const:`telegram.constants.UpdateType.BUSINESS_MESSAGE`
+
+    .. versionadded:: 21.1"""
+    EDITED_BUSINESS_MESSAGE: Final[str] = constants.UpdateType.EDITED_BUSINESS_MESSAGE
+    """:const:`telegram.constants.UpdateType.EDITED_BUSINESS_MESSAGE`
+
+    .. versionadded:: 21.1"""
+    DELETED_BUSINESS_MESSAGES: Final[str] = constants.UpdateType.DELETED_BUSINESS_MESSAGES
+    """:const:`telegram.constants.UpdateType.DELETED_BUSINESS_MESSAGES`
+
+    .. versionadded:: 21.1"""
     ALL_TYPES: Final[List[str]] = list(constants.UpdateType)
     """List[:obj:`str`]: A list of all available update types.
 
     .. versionadded:: 13.5"""
 
     def __init__(
         self,
@@ -340,14 +405,18 @@
         my_chat_member: Optional[ChatMemberUpdated] = None,
         chat_member: Optional[ChatMemberUpdated] = None,
         chat_join_request: Optional[ChatJoinRequest] = None,
         chat_boost: Optional[ChatBoostUpdated] = None,
         removed_chat_boost: Optional[ChatBoostRemoved] = None,
         message_reaction: Optional[MessageReactionUpdated] = None,
         message_reaction_count: Optional[MessageReactionCountUpdated] = None,
+        business_connection: Optional[BusinessConnection] = None,
+        business_message: Optional[Message] = None,
+        edited_business_message: Optional[Message] = None,
+        deleted_business_messages: Optional[BusinessMessagesDeleted] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.update_id: int = update_id
         # Optionals
@@ -365,16 +434,23 @@
         self.my_chat_member: Optional[ChatMemberUpdated] = my_chat_member
         self.chat_member: Optional[ChatMemberUpdated] = chat_member
         self.chat_join_request: Optional[ChatJoinRequest] = chat_join_request
         self.chat_boost: Optional[ChatBoostUpdated] = chat_boost
         self.removed_chat_boost: Optional[ChatBoostRemoved] = removed_chat_boost
         self.message_reaction: Optional[MessageReactionUpdated] = message_reaction
         self.message_reaction_count: Optional[MessageReactionCountUpdated] = message_reaction_count
+        self.business_connection: Optional[BusinessConnection] = business_connection
+        self.business_message: Optional[Message] = business_message
+        self.edited_business_message: Optional[Message] = edited_business_message
+        self.deleted_business_messages: Optional[BusinessMessagesDeleted] = (
+            deleted_business_messages
+        )
 
         self._effective_user: Optional[User] = None
+        self._effective_sender: Optional[Union["User", "Chat"]] = None
         self._effective_chat: Optional[Chat] = None
         self._effective_message: Optional[Message] = None
 
         self._id_attrs = (self.update_id,)
 
         self._freeze()
 
@@ -387,17 +463,22 @@
 
         * :attr:`channel_post`
         * :attr:`edited_channel_post`
         * :attr:`poll`
         * :attr:`chat_boost`
         * :attr:`removed_chat_boost`
         * :attr:`message_reaction_count`
+        * :attr:`deleted_business_messages`
 
         is present.
 
+        .. versionchanged:: 21.1
+            This property now also considers :attr:`business_connection`, :attr:`business_message`
+            and :attr:`edited_business_message`.
+
         Example:
             * If :attr:`message` is present, this will give
               :attr:`telegram.Message.from_user`.
             * If :attr:`poll_answer` is present, this will give :attr:`telegram.PollAnswer.user`.
 
         """
         if self._effective_user:
@@ -437,27 +518,98 @@
 
         elif self.chat_join_request:
             user = self.chat_join_request.from_user
 
         elif self.message_reaction:
             user = self.message_reaction.user
 
+        elif self.business_message:
+            user = self.business_message.from_user
+
+        elif self.edited_business_message:
+            user = self.edited_business_message.from_user
+
+        elif self.business_connection:
+            user = self.business_connection.user
+
         self._effective_user = user
         return user
 
     @property
+    def effective_sender(self) -> Optional[Union["User", "Chat"]]:
+        """
+        :class:`telegram.User` or :class:`telegram.Chat`: The user or chat that sent this update,
+        no matter what kind of update this is.
+
+        Note:
+            * Depending on the type of update and the user's 'Remain anonymous' setting, this
+              could either be :class:`telegram.User`, :class:`telegram.Chat` or :obj:`None`.
+
+        If no user whatsoever is associated with this update, this gives :obj:`None`. This
+        is the case if any of
+
+        * :attr:`poll`
+        * :attr:`chat_boost`
+        * :attr:`removed_chat_boost`
+        * :attr:`message_reaction_count`
+        * :attr:`deleted_business_messages`
+
+        is present.
+
+        Example:
+            * If :attr:`message` is present, this will give either
+              :attr:`telegram.Message.from_user` or :attr:`telegram.Message.sender_chat`.
+            * If :attr:`poll_answer` is present, this will give either
+              :attr:`telegram.PollAnswer.user` or :attr:`telegram.PollAnswer.voter_chat`.
+            * If :attr:`channel_post` is present, this will give
+              :attr:`telegram.Message.sender_chat`.
+
+        .. versionadded:: 21.1
+        """
+        if self._effective_sender:
+            return self._effective_sender
+
+        sender: Optional[Union["User", "Chat"]] = None
+
+        if message := (
+            self.message
+            or self.edited_message
+            or self.channel_post
+            or self.edited_channel_post
+            or self.business_message
+            or self.edited_business_message
+        ):
+            sender = message.sender_chat
+
+        elif self.poll_answer:
+            sender = self.poll_answer.voter_chat
+
+        elif self.message_reaction:
+            sender = self.message_reaction.actor_chat
+
+        if sender is None:
+            sender = self.effective_user
+
+        self._effective_sender = sender
+        return sender
+
+    @property
     def effective_chat(self) -> Optional["Chat"]:
         """
         :class:`telegram.Chat`: The chat that this update was sent in, no matter what kind of
         update this is.
         If no chat is associated with this update, this gives :obj:`None`.
         This is the case, if :attr:`inline_query`,
         :attr:`chosen_inline_result`, :attr:`callback_query` from inline messages,
-        :attr:`shipping_query`, :attr:`pre_checkout_query`, :attr:`poll` or
-        :attr:`poll_answer` is present.
+        :attr:`shipping_query`, :attr:`pre_checkout_query`, :attr:`poll`,
+        :attr:`poll_answer`, or :attr:`business_connection` is present.
+
+        .. versionchanged:: 21.1
+            This property now also considers :attr:`business_message`,
+            :attr:`edited_business_message`, and :attr:`deleted_business_messages`.
 
         Example:
             If :attr:`message` is present, this will give :attr:`telegram.Message.chat`.
 
         """
         if self._effective_chat:
             return self._effective_chat
@@ -496,26 +648,39 @@
 
         elif self.message_reaction:
             chat = self.message_reaction.chat
 
         elif self.message_reaction_count:
             chat = self.message_reaction_count.chat
 
+        elif self.business_message:
+            chat = self.business_message.chat
+
+        elif self.edited_business_message:
+            chat = self.edited_business_message.chat
+
+        elif self.deleted_business_messages:
+            chat = self.deleted_business_messages.chat
+
         self._effective_chat = chat
         return chat
 
     @property
     def effective_message(self) -> Optional[Message]:
         """
         :class:`telegram.Message`: The message included in this update, no matter what kind of
             update this is. More precisely, this will be the message contained in :attr:`message`,
             :attr:`edited_message`, :attr:`channel_post`, :attr:`edited_channel_post` or
             :attr:`callback_query` (i.e. :attr:`telegram.CallbackQuery.message`) or :obj:`None`, if
             none of those are present.
 
+        .. versionchanged:: 21.1
+            This property now also considers :attr:`business_message`, and
+            :attr:`edited_business_message`.
+
         Tip:
             This property will only ever return objects of type :class:`telegram.Message` or
             :obj:`None`, never :class:`telegram.MaybeInaccessibleMessage` or
             :class:`telegram.InaccessibleMessage`.
             Currently, this is only relevant for :attr:`callback_query`, as
             :attr:`telegram.CallbackQuery.message` is the only attribute considered by this
             property that can be an object of these types.
@@ -550,14 +715,20 @@
 
         elif self.channel_post:
             message = self.channel_post
 
         elif self.edited_channel_post:
             message = self.edited_channel_post
 
+        elif self.business_message:
+            message = self.business_message
+
+        elif self.edited_business_message:
+            message = self.edited_business_message
+
         self._effective_message = message
         return message
 
     @classmethod
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["Update"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
         data = cls._parse_data(data)
@@ -585,9 +756,17 @@
         data["removed_chat_boost"] = ChatBoostRemoved.de_json(data.get("removed_chat_boost"), bot)
         data["message_reaction"] = MessageReactionUpdated.de_json(
             data.get("message_reaction"), bot
         )
         data["message_reaction_count"] = MessageReactionCountUpdated.de_json(
             data.get("message_reaction_count"), bot
         )
+        data["business_connection"] = BusinessConnection.de_json(
+            data.get("business_connection"), bot
+        )
+        data["business_message"] = Message.de_json(data.get("business_message"), bot)
+        data["edited_business_message"] = Message.de_json(data.get("edited_business_message"), bot)
+        data["deleted_business_messages"] = BusinessMessagesDeleted.de_json(
+            data.get("deleted_business_messages"), bot
+        )
 
         return super().de_json(data=data, bot=bot)
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_user.py` & `python-telegram-bot-raw-21.1/telegram/_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,27 +74,33 @@
         id (:obj:`int`): Unique identifier for this user or bot.
         is_bot (:obj:`bool`): :obj:`True`, if this user is a bot.
         first_name (:obj:`str`): User's or bot's first name.
         last_name (:obj:`str`, optional): User's or bot's last name.
         username (:obj:`str`, optional): User's or bot's username.
         language_code (:obj:`str`, optional): IETF language tag of the user's language.
         can_join_groups (:obj:`str`, optional): :obj:`True`, if the bot can be invited to groups.
-            Returned only in :attr:`telegram.Bot.get_me` requests.
+            Returned only in :meth:`telegram.Bot.get_me`.
         can_read_all_group_messages (:obj:`str`, optional): :obj:`True`, if privacy mode is
-            disabled for the bot. Returned only in :attr:`telegram.Bot.get_me` requests.
+            disabled for the bot. Returned only in :meth:`telegram.Bot.get_me`.
         supports_inline_queries (:obj:`str`, optional): :obj:`True`, if the bot supports inline
-            queries. Returned only in :attr:`telegram.Bot.get_me` requests.
+            queries. Returned only in :meth:`telegram.Bot.get_me`.
 
         is_premium (:obj:`bool`, optional): :obj:`True`, if this user is a Telegram Premium user.
 
             .. versionadded:: 20.0
         added_to_attachment_menu (:obj:`bool`, optional): :obj:`True`, if this user added
             the bot to the attachment menu.
 
             .. versionadded:: 20.0
+        can_connect_to_business (:obj:`bool`, optional): :obj:`True`,  if the bot can be connected
+            to a Telegram Business account to receive its messages. Returned only in
+            :meth:`telegram.Bot.get_me`.
+
+            .. versionadded:: 21.1
+
     Attributes:
         id (:obj:`int`): Unique identifier for this user or bot.
         is_bot (:obj:`bool`): :obj:`True`, if this user is a bot.
         first_name (:obj:`str`): User's or bot's first name.
         last_name (:obj:`str`): Optional. User's or bot's last name.
         username (:obj:`str`): Optional. User's or bot's username.
         language_code (:obj:`str`): Optional. IETF language tag of the user's language.
@@ -108,21 +114,27 @@
             Premium user.
 
             .. versionadded:: 20.0
         added_to_attachment_menu (:obj:`bool`): Optional. :obj:`True`, if this user added
             the bot to the attachment menu.
 
             .. versionadded:: 20.0
+        can_connect_to_business (:obj:`bool`): Optional. :obj:`True`,  if the bot can be connected
+            to a Telegram Business account to receive its messages. Returned only in
+            :meth:`telegram.Bot.get_me`.
+
+            .. versionadded:: 21.1
     .. |user_chat_id_note| replace:: This shortcuts build on the assumption that :attr:`User.id`
         coincides with the :attr:`Chat.id` of the private chat with the user. This has been the
         case so far, but Telegram does not guarantee that this stays this way.
     """
 
     __slots__ = (
         "added_to_attachment_menu",
+        "can_connect_to_business",
         "can_join_groups",
         "can_read_all_group_messages",
         "first_name",
         "id",
         "is_bot",
         "is_premium",
         "language_code",
@@ -140,14 +152,15 @@
         username: Optional[str] = None,
         language_code: Optional[str] = None,
         can_join_groups: Optional[bool] = None,
         can_read_all_group_messages: Optional[bool] = None,
         supports_inline_queries: Optional[bool] = None,
         is_premium: Optional[bool] = None,
         added_to_attachment_menu: Optional[bool] = None,
+        can_connect_to_business: Optional[bool] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.id: int = id
         self.first_name: str = first_name
@@ -157,14 +170,15 @@
         self.username: Optional[str] = username
         self.language_code: Optional[str] = language_code
         self.can_join_groups: Optional[bool] = can_join_groups
         self.can_read_all_group_messages: Optional[bool] = can_read_all_group_messages
         self.supports_inline_queries: Optional[bool] = supports_inline_queries
         self.is_premium: Optional[bool] = is_premium
         self.added_to_attachment_menu: Optional[bool] = added_to_attachment_menu
+        self.can_connect_to_business: Optional[bool] = can_connect_to_business
 
         self._id_attrs = (self.id,)
 
         self._freeze()
 
     @property
     def name(self) -> str:
@@ -389,14 +403,15 @@
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         link_preview_options: ODVInput["LinkPreviewOptions"] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         disable_web_page_preview: Optional[bool] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -431,14 +446,15 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
     async def delete_message(
         self,
         message_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -509,14 +525,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         has_spoiler: Optional[bool] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -552,25 +569,27 @@
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             has_spoiler=has_spoiler,
+            business_connection_id=business_connection_id,
         )
 
     async def send_media_group(
         self,
         media: Sequence[
             Union["InputMediaAudio", "InputMediaDocument", "InputMediaPhoto", "InputMediaVideo"]
         ],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -606,14 +625,15 @@
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
+            business_connection_id=business_connection_id,
         )
 
     async def send_audio(
         self,
         audio: Union[FileInput, "Audio"],
         duration: Optional[int] = None,
         performer: Optional[str] = None,
@@ -623,14 +643,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -669,20 +690,22 @@
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             thumbnail=thumbnail,
+            business_connection_id=business_connection_id,
         )
 
     async def send_chat_action(
         self,
         action: str,
         message_thread_id: Optional[int] = None,
+        business_connection_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
@@ -704,14 +727,15 @@
             action=action,
             message_thread_id=message_thread_id,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
+            business_connection_id=business_connection_id,
         )
 
     send_action = send_chat_action
     """Alias for :attr:`send_chat_action`"""
 
     async def send_contact(
         self,
@@ -720,14 +744,15 @@
         last_name: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         vcard: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         contact: Optional["Contact"] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -762,24 +787,26 @@
             pool_timeout=pool_timeout,
             contact=contact,
             vcard=vcard,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_dice(
         self,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         emoji: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -809,14 +836,15 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             emoji=emoji,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_document(
         self,
         document: Union[FileInput, "Document"],
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
@@ -824,14 +852,15 @@
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_content_type_detection: Optional[bool] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -868,24 +897,26 @@
             thumbnail=thumbnail,
             api_kwargs=api_kwargs,
             disable_content_type_detection=disable_content_type_detection,
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_game(
         self,
         game_short_name: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -915,14 +946,15 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_invoice(
         self,
         title: str,
         description: str,
         payload: str,
@@ -1027,14 +1059,15 @@
         live_period: Optional[int] = None,
         horizontal_accuracy: Optional[float] = None,
         heading: Optional[int] = None,
         proximity_alert_radius: Optional[int] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         location: Optional["Location"] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1071,14 +1104,15 @@
             api_kwargs=api_kwargs,
             horizontal_accuracy=horizontal_accuracy,
             heading=heading,
             proximity_alert_radius=proximity_alert_radius,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_animation(
         self,
         animation: Union[FileInput, "Animation"],
         duration: Optional[int] = None,
         width: Optional[int] = None,
@@ -1089,14 +1123,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         has_spoiler: Optional[bool] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1136,25 +1171,27 @@
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             has_spoiler=has_spoiler,
             thumbnail=thumbnail,
+            business_connection_id=business_connection_id,
         )
 
     async def send_sticker(
         self,
         sticker: Union[FileInput, "Sticker"],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         emoji: Optional[str] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1185,14 +1222,15 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             emoji=emoji,
+            business_connection_id=business_connection_id,
         )
 
     async def send_video(
         self,
         video: Union[FileInput, "Video"],
         duration: Optional[int] = None,
         caption: Optional[str] = None,
@@ -1204,14 +1242,15 @@
         supports_streaming: Optional[bool] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         has_spoiler: Optional[bool] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1252,14 +1291,15 @@
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             has_spoiler=has_spoiler,
+            business_connection_id=business_connection_id,
         )
 
     async def send_venue(
         self,
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
         title: Optional[str] = None,
@@ -1269,14 +1309,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         foursquare_type: Optional[str] = None,
         google_place_id: Optional[str] = None,
         google_place_type: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         venue: Optional["Venue"] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1315,27 +1356,29 @@
             foursquare_type=foursquare_type,
             api_kwargs=api_kwargs,
             google_place_id=google_place_id,
             google_place_type=google_place_type,
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_video_note(
         self,
         video_note: Union[FileInput, "VideoNote"],
         duration: Optional[int] = None,
         length: Optional[int] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1370,28 +1413,30 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             thumbnail=thumbnail,
+            business_connection_id=business_connection_id,
         )
 
     async def send_voice(
         self,
         voice: Union[FileInput, "Voice"],
         duration: Optional[int] = None,
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1427,14 +1472,15 @@
             parse_mode=parse_mode,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             caption_entities=caption_entities,
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_poll(
         self,
         question: str,
         options: Sequence[str],
         is_anonymous: Optional[bool] = None,
@@ -1448,14 +1494,15 @@
         explanation_parse_mode: ODVInput[str] = DEFAULT_NONE,
         open_period: Optional[int] = None,
         close_date: Optional[Union[int, datetime]] = None,
         explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
+        business_connection_id: Optional[str] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1496,14 +1543,15 @@
             open_period=open_period,
             close_date=close_date,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             explanation_entities=explanation_entities,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
+            business_connection_id=business_connection_id,
         )
 
     async def send_copy(
         self,
         from_chat_id: Union[str, int],
         message_id: int,
         caption: Optional[str] = None,
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_userprofilephotos.py` & `python-telegram-bot-raw-21.1/telegram/_userprofilephotos.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/argumentparsing.py` & `python-telegram-bot-raw-21.1/telegram/_utils/argumentparsing.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/datetime.py` & `python-telegram-bot-raw-21.1/telegram/_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/defaultvalue.py` & `python-telegram-bot-raw-21.1/telegram/_utils/defaultvalue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/enum.py` & `python-telegram-bot-raw-21.1/telegram/_utils/enum.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/files.py` & `python-telegram-bot-raw-21.1/telegram/_utils/files.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/logging.py` & `python-telegram-bot-raw-21.1/telegram/_utils/logging.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/markup.py` & `python-telegram-bot-raw-21.1/telegram/_utils/markup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/repr.py` & `python-telegram-bot-raw-21.1/telegram/_utils/repr.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/strings.py` & `python-telegram-bot-raw-21.1/telegram/_utils/strings.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/types.py` & `python-telegram-bot-raw-21.1/telegram/_utils/types.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/warnings.py` & `python-telegram-bot-raw-21.1/telegram/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_utils/warnings_transition.py` & `python-telegram-bot-raw-21.1/telegram/_utils/warnings_transition.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_version.py` & `python-telegram-bot-raw-21.1/telegram/_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         if self.releaselevel != "final":
             version = f"{version}{self._rl_shorthand()}{self.serial}"
 
         return version
 
 
 __version_info__: Final[Version] = Version(
-    major=21, minor=0, micro=1, releaselevel="final", serial=0
+    major=21, minor=1, micro=0, releaselevel="final", serial=0
 )
 __version__: Final[str] = str(__version_info__)
 
 # # SETUP.PY MARKER
 # Lines above this line will be `exec`-cuted in setup.py. Make sure that this only contains
 # std-lib imports!
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_videochat.py` & `python-telegram-bot-raw-21.1/telegram/_videochat.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_webappdata.py` & `python-telegram-bot-raw-21.1/telegram/_webappdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_webappinfo.py` & `python-telegram-bot-raw-21.1/telegram/_webappinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_webhookinfo.py` & `python-telegram-bot-raw-21.1/telegram/_webhookinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/_writeaccessallowed.py` & `python-telegram-bot-raw-21.1/telegram/_writeaccessallowed.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/constants.py` & `python-telegram-bot-raw-21.1/telegram/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 #: :class:`typing.NamedTuple`: A tuple containing the two components of the version number:
 # ``major`` and ``minor``. Both values are integers.
 #: The components can also be accessed by name, so ``BOT_API_VERSION_INFO[0]`` is equivalent
 #: to ``BOT_API_VERSION_INFO.major`` and so on. Also available as
 #: :data:`telegram.__bot_api_version_info__`.
 #:
 #: .. versionadded:: 20.0
-BOT_API_VERSION_INFO: Final[_BotAPIVersion] = _BotAPIVersion(major=7, minor=1)
+BOT_API_VERSION_INFO: Final[_BotAPIVersion] = _BotAPIVersion(major=7, minor=2)
 #: :obj:`str`: Telegram Bot API
 #: version supported by this version of `python-telegram-bot`. Also available as
 #: :data:`telegram.__bot_api_version__`.
 #:
 #: .. versionadded:: 13.4
 BOT_API_VERSION: Final[str] = str(BOT_API_VERSION_INFO)
 
@@ -1686,16 +1686,20 @@
     CHAT = "chat"
     """:obj:`str`: A :class:`telegram.MessageOrigin` who is sent by a chat."""
     CHANNEL = "channel"
     """:obj:`str`: A :class:`telegram.MessageOrigin` who is sent by a channel."""
 
 
 class MessageType(StringEnum):
-    """This enum contains the available types of :class:`telegram.Message`. The enum
-    members of this enumeration are instances of :class:`str` and can be treated as such.
+    """This enum contains the available types of :class:`telegram.Message`. Here, a "type" means
+    a kind of message that is visually distinct from other kinds of messages in the Telegram app.
+    In particular, auxiliary attributes that can be present for multiple types of messages are
+    not considered in this enumeration.
+
+    The enum members of this enumeration are instances of :class:`str` and can be treated as such.
 
     .. versionadded:: 20.0
     """
 
     __slots__ = ()
 
     # Make sure that all attachment type constants are also listed in the
@@ -1706,14 +1710,19 @@
     AUDIO = "audio"
     """:obj:`str`: Messages with :attr:`telegram.Message.audio`."""
     BOOST_ADDED = "boost_added"
     """:obj:`str`: Messages with :attr:`telegram.Message.boost_added`.
 
     .. versionadded:: 21.0
     """
+    BUSINESS_CONNECTION_ID = "business_connection_id"
+    """:obj:`str`: Messages with :attr:`telegram.Message.business_connection_id`.
+
+    .. versionadded:: 21.1
+    """
     CHANNEL_CHAT_CREATED = "channel_chat_created"
     """:obj:`str`: Messages with :attr:`telegram.Message.channel_chat_created`."""
     CHAT_SHARED = "chat_shared"
     """:obj:`str`: Messages with :attr:`telegram.Message.chat_shared`.
 
     .. versionadded:: 20.8
     """
@@ -1813,14 +1822,19 @@
     .. versionadded:: 21.0
     """
     SENDER_BOOST_COUNT = "sender_boost_count"
     """:obj:`str`: Messages with :attr:`telegram.Message.sender_boost_count`.
 
     .. versionadded:: 21.0
     """
+    SENDER_BUSINESS_BOT = "sender_business_bot"
+    """:obj:`str`: Messages with :attr:`telegram.Message.sender_business_bot`.
+
+    .. versionadded:: 21.1
+    """
     STICKER = "sticker"
     """:obj:`str`: Messages with :attr:`telegram.Message.sticker`."""
     STORY = "story"
     """:obj:`str`: Messages with :attr:`telegram.Message.story`."""
     SUPERGROUP_CHAT_CREATED = "supergroup_chat_created"
     """:obj:`str`: Messages with :attr:`telegram.Message.supergroup_chat_created`."""
     SUCCESSFUL_PAYMENT = "successful_payment"
@@ -2308,14 +2322,17 @@
     MAX_EMOJI_STICKERS = 200
     """:obj:`int`: Maximum number of stickers allowed in an emoji sticker set, as given in
     :meth:`telegram.Bot.add_sticker_to_set`.
     """
     MAX_ANIMATED_STICKERS = 50
     """:obj:`int`: Maximum number of stickers allowed in an animated or video sticker set, as given
     in :meth:`telegram.Bot.add_sticker_to_set`.
+
+    .. deprecated:: 21.1
+        The animated sticker limit is now 120, the same as :attr:`MAX_STATIC_STICKERS`.
     """
     MAX_STATIC_STICKERS = 120
     """:obj:`int`: Maximum number of stickers allowed in a static sticker set, as given in
     :meth:`telegram.Bot.add_sticker_to_set`.
     """
     MAX_STATIC_THUMBNAIL_SIZE = 128
     """:obj:`int`: Maximum size of the thumbnail if it is a **.WEBP** or **.PNG** in kilobytes,
@@ -2500,14 +2517,34 @@
     .. versionadded:: 20.8
     """
     MESSAGE_REACTION_COUNT = "message_reaction_count"
     """:obj:`str`: Updates with :attr:`telegram.Update.message_reaction_count`.
 
     .. versionadded:: 20.8
     """
+    BUSINESS_CONNECTION = "business_connection"
+    """:obj:`str`: Updates with :attr:`telegram.Update.business_connection`.
+
+    .. versionadded:: 21.1
+    """
+    BUSINESS_MESSAGE = "business_message"
+    """:obj:`str`: Updates with :attr:`telegram.Update.business_message`.
+
+    .. versionadded:: 21.1
+    """
+    EDITED_BUSINESS_MESSAGE = "edited_business_message"
+    """:obj:`str`: Updates with :attr:`telegram.Update.edited_business_message`.
+
+    .. versionadded:: 21.1
+    """
+    DELETED_BUSINESS_MESSAGES = "deleted_business_messages"
+    """:obj:`str`: Updates with :attr:`telegram.Update.deleted_business_messages`.
+
+    .. versionadded:: 21.1
+    """
 
 
 class InvoiceLimit(IntEnum):
     """This enum contains limitations for :class:`telegram.InputInvoiceMessageContent`,
     :meth:`telegram.Bot.send_invoice`, and :meth:`telegram.Bot.create_invoice_link`.
     The enum members of this enumeration are instances of :class:`int` and can be treated as such.
```

### Comparing `python-telegram-bot-raw-21.0.1/telegram/error.py` & `python-telegram-bot-raw-21.1/telegram/error.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/helpers.py` & `python-telegram-bot-raw-21.1/telegram/helpers.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/request/__init__.py` & `python-telegram-bot-raw-21.1/telegram/request/__init__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/request/_baserequest.py` & `python-telegram-bot-raw-21.1/telegram/request/_baserequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/request/_httpxrequest.py` & `python-telegram-bot-raw-21.1/telegram/request/_httpxrequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/request/_requestdata.py` & `python-telegram-bot-raw-21.1/telegram/request/_requestdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/request/_requestparameter.py` & `python-telegram-bot-raw-21.1/telegram/request/_requestparameter.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.0.1/telegram/warnings.py` & `python-telegram-bot-raw-21.1/telegram/warnings.py`

 * *Files identical despite different names*

