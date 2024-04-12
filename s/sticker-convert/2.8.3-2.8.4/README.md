# Comparing `tmp/sticker-convert-2.8.3.tar.gz` & `tmp/sticker_convert-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sticker-convert-2.8.3.tar", last modified: Thu Mar 28 12:40:13 2024, max compression
+gzip compressed data, was "sticker_convert-2.8.4.tar", last modified: Fri Apr 12 16:58:55 2024, max compression
```

## Comparing `sticker-convert-2.8.3.tar` & `sticker_convert-2.8.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.356036 sticker-convert-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49284 2024-03-28 12:40:13.356036 sticker-convert-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26818 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 12:40:13.356036 sticker-convert-2.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.328036 sticker-convert-2.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.332036 sticker-convert-2.8.3/src/sticker_convert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18579 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/downloaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2726 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/downloaders/download_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/downloaders/download_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/downloaders/download_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3160 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/downloaders/download_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/downloaders/download_telegram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30707 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/gui_components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/comp_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/config_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/control_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/cred_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/input_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/output_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/progress_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/right_clicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/gui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31688 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/advanced_compression_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/base_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/line_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.336036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.340036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.340036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.340036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.340036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.340036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.340036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.328036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.340036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
--rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.328036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.328036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.340036 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
--rwxr-xr-x   0 runner    (1001) docker     (127)    25608 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7732 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/job_option.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.352036 sticker-convert-2.8.3/src/sticker_convert/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/resources/NotoColorEmoji.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/resources/appicon.icns
--rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/resources/appicon.ico
--rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/resources/appicon.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    11163 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/resources/compression.json
--rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/resources/emoji.json
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/resources/help.json
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/resources/input.json
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/resources/output.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.352036 sticker-convert-2.8.3/src/sticker_convert/uploaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/uploaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/uploaders/compress_wastickers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/uploaders/upload_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6541 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/uploaders/upload_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14634 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/uploaders/upload_telegram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/uploaders/xcode_imessage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.352036 sticker-convert-2.8.3/src/sticker_convert/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.352036 sticker-convert-2.8.3/src/sticker_convert/utils/auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/auth/get_kakao_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2682 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/auth/get_line_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/auth/get_signal_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.356036 sticker-convert-2.8.3/src/sticker_convert/utils/files/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/files/cache_store.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/files/json_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/files/json_resources_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10088 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/files/metadata_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/files/run_bin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/files/sanitize_filename.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.356036 sticker-convert-2.8.3/src/sticker_convert/utils/media/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/media/apple_png_normalize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/media/codec_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/media/decrypt_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/media/format_verify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/utils/url_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/src/sticker_convert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.356036 sticker-convert-2.8.3/src/sticker_convert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49284 2024-03-28 12:40:13.000000 sticker-convert-2.8.3/src/sticker_convert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-03-28 12:40:13.000000 sticker-convert-2.8.3/src/sticker_convert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 12:40:13.000000 sticker-convert-2.8.3/src/sticker_convert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 12:40:13.000000 sticker-convert-2.8.3/src/sticker_convert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-28 12:40:13.000000 sticker-convert-2.8.3/src/sticker_convert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-28 12:40:13.000000 sticker-convert-2.8.3/src/sticker_convert.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:40:13.356036 sticker-convert-2.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-28 12:40:08.000000 sticker-convert-2.8.3/tests/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.810012 sticker_convert-2.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49307 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26818 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:58:55.810012 sticker_convert-2.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.782012 sticker_convert-2.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18579 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37353 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2726 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_telegram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30707 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/gui_components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/comp_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/config_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/control_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/cred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/input_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/output_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/progress_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/right_clicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/gui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31688 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/advanced_compression_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/line_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.798012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.798012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.786012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.798012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
+-rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.786012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.786012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.798012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25608 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7732 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/job_option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/NotoColorEmoji.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/appicon.icns
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/appicon.ico
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/appicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11163 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/compression.json
+-rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/emoji.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/help.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/output.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/compress_wastickers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6396 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15695 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_telegram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/xcode_imessage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/utils/auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_kakao_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_line_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_signal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/utils/files/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/cache_store.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/json_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/json_resources_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10088 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/metadata_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/run_bin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/sanitize_filename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/utils/media/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/media/apple_png_normalize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/media/codec_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/media/decrypt_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/media/format_verify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/url_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49307 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/tests/test_export.py
```

### Comparing `sticker-convert-2.8.3/LICENSE` & `sticker_convert-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/PKG-INFO` & `sticker_convert-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.3
+Version: 2.8.4
 Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -361,29 +361,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiolimiter~=1.1.0
-Requires-Dist: anyio~=3.7.1
+Requires-Dist: anyio~=4.3.0
 Requires-Dist: apngasm_python~=1.2.3
 Requires-Dist: av~=12.0.0
 Requires-Dist: beautifulsoup4~=4.12.3
-Requires-Dist: rookiepy~=0.3.6
+Requires-Dist: rookiepy~=0.3.7
 Requires-Dist: imagequant~=1.1.1
 Requires-Dist: memory-tempfile~=2.2.3
 Requires-Dist: mergedeep~=1.3.4
 Requires-Dist: numpy>=1.22.4
-Requires-Dist: Pillow==10.1.0
+Requires-Dist: Pillow~=10.3.0
 Requires-Dist: pyoxipng~=9.0.0
-Requires-Dist: python-telegram-bot~=20.5
+Requires-Dist: python-telegram-bot~=21.1
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rlottie_python~=1.3.4
-Requires-Dist: signalstickers-client~=3.3.0
+Requires-Dist: signalstickers-client-fork-laggykiller~=3.3.0.post1
 Requires-Dist: sqlcipher3-wheels~=0.5.2.post1
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: ttkbootstrap-fork-laggykiller~=1.5.1
 Requires-Dist: webp~=0.3.0
 
 # sticker-convert
 ![imgs/banner.png](imgs/banner.png)
```

### Comparing `sticker-convert-2.8.3/README.md` & `sticker_convert-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/pyproject.toml` & `sticker_convert-2.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/cli.py` & `sticker_convert-2.8.4/src/sticker_convert/cli.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/converter.py` & `sticker_convert-2.8.4/src/sticker_convert/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -700,15 +700,15 @@
             self._frames_export_webp()
         elif self.out_f.suffix == ".gif":
             self._frames_export_pil_anim()
         elif self.out_f.suffix in (".webm", ".mp4", ".mkv") or is_animated:
             self._frames_export_pyav()
         else:
             self._frames_export_pil()
-    
+
     def _check_dup(self) -> bool:
         if len(self.frames_processed) == 1:
             return False
 
         prev_frame = self.frames_processed[0]
         for frame in self.frames_processed[1:]:
             if np.array_equal(frame, prev_frame):
```

### Comparing `sticker-convert-2.8.3/src/sticker_convert/definitions.py` & `sticker_convert-2.8.4/src/sticker_convert/definitions.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/downloaders/download_base.py` & `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_base.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/downloaders/download_kakao.py` & `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/downloaders/download_line.py` & `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_line.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/downloaders/download_signal.py` & `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_signal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 from pathlib import Path
 from typing import Dict, Optional
 
 import anyio
-from signalstickers_client import StickersClient  # type: ignore
-from signalstickers_client.errors import SignalException  # type: ignore
-from signalstickers_client.models import StickerPack  # type: ignore
+from signalstickers_client.errors import SignalException
+from signalstickers_client.models import StickerPack
+from signalstickers_client.stickersclient import StickersClient
 
 from sticker_convert.downloaders.download_base import DownloadBase
 from sticker_convert.job_option import CredOption
 from sticker_convert.utils.callback import CallbackProtocol, CallbackReturn
 from sticker_convert.utils.files.metadata_handler import MetadataHandler
 from sticker_convert.utils.media.codec_info import CodecInfo
 
@@ -17,33 +17,33 @@
 class DownloadSignal(DownloadBase):
     # def __init__(self, *args: Any, **kwargs: Any) -> None:
     #     super().__init__(*args, **kwargs)
 
     @staticmethod
     async def get_pack(pack_id: str, pack_key: str) -> StickerPack:
         async with StickersClient() as client:
-            pack = await client.get_pack(pack_id, pack_key)  # type: ignore
+            pack = await client.get_pack(pack_id, pack_key)
 
         return pack
 
     def save_stickers(self, pack: StickerPack) -> None:
         self.cb.put(
             (
                 "bar",
                 None,
                 {
                     "set_progress_mode": "determinate",
-                    "steps": len(pack.stickers),  # type: ignore
+                    "steps": len(pack.stickers),
                 },
             )
         )
 
         emoji_dict: Dict[str, str] = {}
-        for sticker in pack.stickers:  # type: ignore
-            f_id = str(sticker.id).zfill(3)  # type: ignore
+        for sticker in pack.stickers:
+            f_id = str(sticker.id).zfill(3)
             f_path = Path(self.out_dir, f_id)
             with open(f_path, "wb") as f:
                 f.write(sticker.image_data)  # type: ignore
 
             emoji_dict[f_id] = sticker.emoji  # type: ignore
 
             codec = CodecInfo.get_file_codec(f_path)
```

### Comparing `sticker-convert-2.8.3/src/sticker_convert/downloaders/download_telegram.py` & `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_telegram.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui.py` & `sticker_convert-2.8.4/src/sticker_convert/gui.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/comp_frame.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/comp_frame.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/config_frame.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/config_frame.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/control_frame.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/control_frame.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/cred_frame.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/cred_frame.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/input_frame.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/input_frame.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/output_frame.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/output_frame.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/progress_frame.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/progress_frame.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/frames/right_clicker.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/right_clicker.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/gui_utils.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/gui_utils.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/advanced_compression_window.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/advanced_compression_window.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/base_window.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/base_window.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/line_get_auth_window.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/line_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/gui_components/windows/signal_get_auth_window.py` & `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/signal_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate` & `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/job.py` & `sticker_convert-2.8.4/src/sticker_convert/job.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/job_option.py` & `sticker_convert-2.8.4/src/sticker_convert/job_option.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/resources/NotoColorEmoji.ttf` & `sticker_convert-2.8.4/src/sticker_convert/resources/NotoColorEmoji.ttf`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/resources/appicon.icns` & `sticker_convert-2.8.4/src/sticker_convert/resources/appicon.icns`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/resources/appicon.ico` & `sticker_convert-2.8.4/src/sticker_convert/resources/appicon.ico`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/resources/appicon.png` & `sticker_convert-2.8.4/src/sticker_convert/resources/appicon.png`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/resources/compression.json` & `sticker_convert-2.8.4/src/sticker_convert/resources/compression.json`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/resources/emoji.json` & `sticker_convert-2.8.4/src/sticker_convert/resources/emoji.json`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/resources/help.json` & `sticker_convert-2.8.4/src/sticker_convert/resources/help.json`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/resources/input.json` & `sticker_convert-2.8.4/src/sticker_convert/resources/input.json`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/resources/output.json` & `sticker_convert-2.8.4/src/sticker_convert/resources/output.json`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/uploaders/compress_wastickers.py` & `sticker_convert-2.8.4/src/sticker_convert/uploaders/compress_wastickers.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/uploaders/upload_base.py` & `sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_base.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/uploaders/upload_signal.py` & `sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_signal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 import copy
 from pathlib import Path
 from typing import Any, Dict, List
 
 import anyio
-from signalstickers_client import StickersClient  # type: ignore
-from signalstickers_client.errors import SignalException  # type: ignore
-from signalstickers_client.models import LocalStickerPack, Sticker  # type: ignore
+from signalstickers_client.errors import SignalException
+from signalstickers_client.models import LocalStickerPack, Sticker
+from signalstickers_client.stickersclient import StickersClient
 
 from sticker_convert.converter import StickerConvert
 from sticker_convert.job_option import CompOption, CredOption, OutputOption
 from sticker_convert.uploaders.upload_base import UploadBase
 from sticker_convert.utils.callback import CallbackProtocol, CallbackReturn
 from sticker_convert.utils.files.metadata_handler import MetadataHandler
 from sticker_convert.utils.media.codec_info import CodecInfo
@@ -35,37 +35,37 @@
 
         self.opt_comp_merged = copy.deepcopy(self.opt_comp)
         self.opt_comp_merged.merge(self.base_spec)
 
     @staticmethod
     async def upload_pack(pack: LocalStickerPack, uuid: str, password: str) -> str:
         async with StickersClient(uuid, password) as client:
-            pack_id, pack_key = await client.upload_pack(pack)  # type: ignore
+            pack_id, pack_key = await client.upload_pack(pack)
 
         result = (
             f"https://signal.art/addstickers/#pack_id={pack_id}&pack_key={pack_key}"
         )
         return result
 
     def add_stickers_to_pack(
         self, pack: LocalStickerPack, stickers: List[Path], emoji_dict: Dict[str, str]
     ) -> None:
         for src in stickers:
             self.cb.put(f"Verifying {src} for uploading to signal")
 
             sticker = Sticker()
-            sticker.id = pack.nb_stickers  # type: ignore
+            sticker.id = pack.nb_stickers
 
             emoji = emoji_dict.get(Path(src).stem, None)
             if not emoji:
                 self.cb.put(
                     f"Warning: Cannot find emoji for file {Path(src).name}, skip uploading this file..."
                 )
                 continue
-            sticker.emoji = emoji[:1]  # type: ignore
+            sticker.emoji = emoji[:1]
 
             if Path(src).suffix == ".webp":
                 spec_choice = self.webp_spec
             else:
                 spec_choice = self.png_spec
 
             if not FormatVerify.check_file(src, spec=spec_choice):
@@ -80,18 +80,18 @@
                     self.cb.put(
                         f"Warning: Cannot compress file {Path(src).name}, skip uploading this file..."
                     )
                     continue
 
                 assert isinstance(image_data, bytes)
 
-                sticker.image_data = image_data  # type: ignore
+                sticker.image_data = image_data
             else:
                 with open(src, "rb") as f:
-                    sticker.image_data = f.read()  # type: ignore
+                    sticker.image_data = f.read()
 
             pack._addsticker(sticker)  # type: ignore
 
     def upload_stickers_signal(self) -> List[str]:
         urls: List[str] = []
 
         if not self.opt_cred.signal_uuid:
@@ -136,16 +136,16 @@
             self.opt_output.dir,
             title=title,
             file_per_pack=200,
             separate_image_anim=False,
         )
         for pack_title, stickers in packs.items():
             pack = LocalStickerPack()
-            pack.title = pack_title  # type: ignore
-            pack.author = author  # type: ignore
+            pack.title = pack_title
+            pack.author = author
 
             self.add_stickers_to_pack(pack, stickers, emoji_dict)
             self.cb.put(f"Uploading pack {pack_title}")
             self.cb.put("update_bar")
             try:
                 result = anyio.run(
                     UploadSignal.upload_pack,
```

### Comparing `sticker-convert-2.8.3/src/sticker_convert/uploaders/upload_telegram.py` & `sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_telegram.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 import copy
 import re
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Union, cast
 
 import anyio
 from telegram import InputSticker, Sticker
 from telegram.error import BadRequest, TelegramError
 from telegram.ext import AIORateLimiter, ApplicationBuilder
 
 from sticker_convert.converter import StickerConvert
@@ -92,15 +92,15 @@
             pack_short_name = (
                 pack_title.replace(" ", "_") + "_by_" + bot.name.replace("@", "")
             )
             pack_short_name = re.sub(
                 "[^0-9a-zA-Z]+", "_", pack_short_name
             )  # name used in url, only alphanum and underscore only
 
-            sticker_set = None
+            sticker_set: Any = None
             try:
                 sticker_set = await bot.get_sticker_set(
                     pack_short_name,
                     read_timeout=30,
                     write_timeout=30,
                     connect_timeout=30,
                     pool_timeout=30,
@@ -148,19 +148,18 @@
                     self.cb.put(f"Not deleting existing pack {pack_short_name}")
 
             if self.opt_output.option == "telegram_emoji":
                 sticker_type = Sticker.CUSTOM_EMOJI
             else:
                 sticker_type = Sticker.REGULAR
 
-            input_stickers: List[Tuple[Path, InputSticker]] = []
+            init_input_stickers: List[InputSticker] = []
             sticker_format = None
-            cover_spec_choice = None
-            ext = None
-            for src in stickers:
+            sticker_format_prev = None
+            for count, src in enumerate(stickers):
                 self.cb.put(f"Verifying {src} for uploading to telegram")
 
                 emoji = emoji_dict.get(Path(src).stem, None)
                 if emoji:
                     if len(emoji) > 20:
                         self.cb.put(
                             f"Warning: {len(emoji)} emoji for file {Path(src).name}, exceeding limit of 20, keep first 20 only..."
@@ -171,24 +170,21 @@
                         f"Warning: Cannot find emoji for file {Path(src).name}, skip uploading this file..."
                     )
                     continue
 
                 ext = Path(src).suffix
                 if ext == ".tgs":
                     spec_choice = self.tgs_spec
-                    cover_spec_choice = self.tgs_cover_spec
                     sticker_format = "animated"
                 elif ext == ".webm":
                     spec_choice = self.webm_spec
-                    cover_spec_choice = self.webm_cover_spec
                     sticker_format = "video"
                 else:
                     ext = ".png"
                     spec_choice = self.png_spec
-                    cover_spec_choice = self.png_cover_spec
                     sticker_format = "static"
 
                 if self.opt_output.option == "telegram_emoji":
                     spec_choice.set_res(100)
 
                 if FormatVerify.check_file(src, spec=spec_choice):
                     with open(src, "rb") as f:
@@ -199,89 +195,106 @@
                         Path(f"bytes{ext}"),
                         self.opt_comp_merged,
                         self.cb,
                         self.cb_return,
                     )
                     sticker_bytes = cast(bytes, convert_result)
 
-                input_stickers.append(
-                    (src, InputSticker(sticker=sticker_bytes, emoji_list=emoji_list))
+                input_sticker = InputSticker(
+                    sticker=sticker_bytes,
+                    emoji_list=emoji_list,
+                    format=sticker_format,
                 )
 
+                if sticker_set is None:
+                    if count < 50 and (
+                        sticker_format_prev is None
+                        or sticker_format_prev == sticker_format
+                    ):
+                        init_input_stickers.append(input_sticker)
+                    else:
+                        start_msg = f"Creating pack and bulk uploading {count} stickers with same format of {pack_short_name}"
+                        finish_msg = f"Created pack and bulk uploaded {count} stickers with same format of {pack_short_name}"
+                        error_msg = f"Cannot create pack and bulk upload {count} stickers with same format of {pack_short_name} due to"
+                        self.cb.put(start_msg)
+                        try:
+                            await bot.create_new_sticker_set(
+                                user_id=self.telegram_userid,
+                                name=pack_short_name,
+                                title=pack_title,
+                                stickers=init_input_stickers,
+                                sticker_type=sticker_type,
+                            )
+                            sticker_set = True
+                            self.cb.put(finish_msg)
+                        except TelegramError as e:
+                            self.cb.put(f"{error_msg} {e}")
+                            return None
+                else:
+                    try:
+                        # We could use tg.start_soon() here
+                        # But this would disrupt the order of stickers
+                        await bot.add_sticker_to_set(
+                            user_id=self.telegram_userid,
+                            name=pack_short_name,
+                            sticker=input_sticker,
+                        )
+                        self.cb.put(f"Uploaded sticker {src} of {pack_short_name}")
+                    except BadRequest as e:
+                        self.cb.put(
+                            f"Cannot upload sticker {src} of {pack_short_name} due to {e}"
+                        )
+                        if str(e) == "Stickerpack_not_found":
+                            self.cb.put(
+                                "Hint: You might had deleted and recreated pack too quickly. Wait about 3 minutes and try again."
+                            )
+                    except TelegramError as e:
+                        self.cb.put(
+                            f"Cannot upload sticker {src} of {pack_short_name} due to {e}"
+                        )
+
+                sticker_format_prev = sticker_format
+
             cover_path = MetadataHandler.get_cover(self.opt_output.dir)
-            thumbnail_bytes: Union[None, bytes, Path] = None
-            if cover_path and cover_spec_choice and ext:
+            if cover_path:
+                thumbnail_bytes: Union[None, bytes, Path] = None
+                cover_ext = Path(cover_path).suffix
+
+                if cover_ext == ".tgs":
+                    thumbnail_format = "animated"
+                    cover_spec_choice = self.tgs_cover_spec
+                elif cover_ext == ".webm":
+                    thumbnail_format = "video"
+                    cover_spec_choice = self.webm_cover_spec
+                else:
+                    cover_ext = ".png"
+                    thumbnail_format = "static"
+                    cover_spec_choice = self.png_cover_spec
+
                 if FormatVerify.check_file(cover_path, spec=cover_spec_choice):
                     with open(cover_path, "rb") as f:
                         thumbnail_bytes = f.read()
                 else:
                     _, _, thumbnail_bytes, _ = StickerConvert.convert(
                         cover_path,
-                        Path(f"bytes{ext}"),
+                        Path(f"bytes{cover_ext}"),
                         self.opt_comp_cover_merged,
                         self.cb,
                         self.cb_return,
                     )
 
-            if sticker_set is None and sticker_format is not None:
-                if len(input_stickers) > 50:
-                    amount_str = "first 50"
-                else:
-                    amount_str = "all"
-                start_msg = f"Creating pack and bulk uploading {amount_str} stickers of {pack_short_name}"
-                finish_msg = f"Created pack and bulk uploaded {amount_str} stickers of {pack_short_name}"
-                error_msg = f"Cannot create pack and bulk upload {amount_str} stickers of {pack_short_name} due to"
-                self.cb.put(start_msg)
-                try:
-                    await bot.create_new_sticker_set(
-                        user_id=self.opt_cred.telegram_userid,
-                        name=pack_short_name,
-                        title=pack_title,
-                        stickers=[a for _, a in input_stickers[:50]],
-                        sticker_format=sticker_format,
-                        sticker_type=sticker_type,
-                    )
-                    self.cb.put(finish_msg)
-                    input_stickers = input_stickers[50:]
-                except TelegramError as e:
-                    self.cb.put(f"{error_msg} {e}")
-                    return None
-
-            for src, sticker in input_stickers:
-                try:
-                    # We could use tg.start_soon() here
-                    # But this would disrupt the order of stickers
-                    await bot.add_sticker_to_set(
-                        user_id=self.opt_cred.telegram_userid,
-                        name=pack_short_name,
-                        sticker=sticker,
-                    )
-                    self.cb.put(f"Uploaded sticker {src} of {pack_short_name}")
-                except BadRequest as e:
-                    self.cb.put(
-                        f"Cannot upload sticker {src} of {pack_short_name} due to {e}"
-                    )
-                    if str(e) == "Stickerpack_not_found":
-                        self.cb.put(
-                            "Hint: You might had deleted and recreated pack too quickly. Wait about 3 minutes and try again."
-                        )
-                except TelegramError as e:
-                    self.cb.put(
-                        f"Cannot upload sticker {src} of {pack_short_name} due to {e}"
-                    )
-
-            if thumbnail_bytes is not None:
                 try:
                     self.cb.put(
                         f"Uploading cover (thumbnail) of pack {pack_short_name}"
                     )
                     await bot.set_sticker_set_thumbnail(
                         name=pack_short_name,
-                        user_id=self.opt_cred.telegram_userid,
+                        user_id=self.telegram_userid,
                         thumbnail=thumbnail_bytes,
+                        format=thumbnail_format,
                     )
                     self.cb.put(f"Uploaded cover (thumbnail) of pack {pack_short_name}")
                 except TelegramError as e:
                     self.cb.put(
                         f"Cannot upload cover (thumbnail) of pack {pack_short_name} due to {e}"
                     )
 
@@ -296,14 +309,20 @@
     def upload_stickers_telegram(self) -> List[str]:
         urls: List[str] = []
 
         if not (self.opt_cred.telegram_token and self.opt_cred.telegram_userid):
             self.cb.put("Token and userid required for uploading to telegram")
             return urls
 
+        if self.opt_cred.telegram_userid.isnumeric():
+            self.telegram_userid = int(self.opt_cred.telegram_userid)
+        else:
+            self.cb.put("Invalid userid, should contain numbers only")
+            return urls
+
         title, _, emoji_dict = MetadataHandler.get_metadata(
             self.opt_output.dir,
             title=self.opt_output.title,
             author=self.opt_output.author,
         )
         if title is None:
             raise TypeError("title cannot be", title)
@@ -323,19 +342,26 @@
             title, _, emoji_dict = MetadataHandler.get_metadata(
                 self.opt_output.dir,
                 title=self.opt_output.title,
                 author=self.opt_output.author,
             )
 
         assert title is not None
+        assert emoji_dict is not None
+
+        if self.opt_output.option == "telegram_emoji":
+            file_per_pack = 200
+        else:
+            file_per_pack = 120
+
         packs = MetadataHandler.split_sticker_packs(
             self.opt_output.dir,
             title=title,
-            file_per_anim_pack=50,
-            file_per_image_pack=120,
+            file_per_anim_pack=file_per_pack,
+            file_per_image_pack=file_per_pack,
             separate_image_anim=not self.opt_comp.fake_vid,
         )
 
         for pack_title, stickers in packs.items():
             self.cb.put(f"Uploading pack {pack_title}")
             result = anyio.run(self.upload_pack, pack_title, stickers, emoji_dict)
             if result:
```

### Comparing `sticker-convert-2.8.3/src/sticker_convert/uploaders/xcode_imessage.py` & `sticker_convert-2.8.4/src/sticker_convert/uploaders/xcode_imessage.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/auth/get_kakao_auth.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_kakao_auth.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/auth/get_signal_auth.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_signal_auth.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/callback.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/callback.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/files/cache_store.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/files/cache_store.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/files/json_manager.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/files/json_manager.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/files/json_resources_loader.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/files/json_resources_loader.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/files/metadata_handler.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/files/metadata_handler.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/files/run_bin.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/files/run_bin.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/files/sanitize_filename.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/files/sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/media/apple_png_normalize.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/media/apple_png_normalize.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/media/codec_info.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/media/codec_info.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/media/decrypt_kakao.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/media/decrypt_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/media/format_verify.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/media/format_verify.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert/utils/url_detect.py` & `sticker_convert-2.8.4/src/sticker_convert/utils/url_detect.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/src/sticker_convert.egg-info/PKG-INFO` & `sticker_convert-2.8.4/src/sticker_convert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.3
+Version: 2.8.4
 Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -361,29 +361,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiolimiter~=1.1.0
-Requires-Dist: anyio~=3.7.1
+Requires-Dist: anyio~=4.3.0
 Requires-Dist: apngasm_python~=1.2.3
 Requires-Dist: av~=12.0.0
 Requires-Dist: beautifulsoup4~=4.12.3
-Requires-Dist: rookiepy~=0.3.6
+Requires-Dist: rookiepy~=0.3.7
 Requires-Dist: imagequant~=1.1.1
 Requires-Dist: memory-tempfile~=2.2.3
 Requires-Dist: mergedeep~=1.3.4
 Requires-Dist: numpy>=1.22.4
-Requires-Dist: Pillow==10.1.0
+Requires-Dist: Pillow~=10.3.0
 Requires-Dist: pyoxipng~=9.0.0
-Requires-Dist: python-telegram-bot~=20.5
+Requires-Dist: python-telegram-bot~=21.1
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rlottie_python~=1.3.4
-Requires-Dist: signalstickers-client~=3.3.0
+Requires-Dist: signalstickers-client-fork-laggykiller~=3.3.0.post1
 Requires-Dist: sqlcipher3-wheels~=0.5.2.post1
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: ttkbootstrap-fork-laggykiller~=1.5.1
 Requires-Dist: webp~=0.3.0
 
 # sticker-convert
 ![imgs/banner.png](imgs/banner.png)
```

### Comparing `sticker-convert-2.8.3/src/sticker_convert.egg-info/SOURCES.txt` & `sticker_convert-2.8.4/src/sticker_convert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/tests/test_compression.py` & `sticker_convert-2.8.4/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/tests/test_download.py` & `sticker_convert-2.8.4/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `sticker-convert-2.8.3/tests/test_export.py` & `sticker_convert-2.8.4/tests/test_export.py`

 * *Files identical despite different names*

