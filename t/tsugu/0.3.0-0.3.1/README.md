# Comparing `tmp/tsugu-0.3.0.tar.gz` & `tmp/tsugu-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.3.0.tar", last modified: Fri Apr 12 03:46:42 2024, max compression
+gzip compressed data, was "tsugu-0.3.1.tar", last modified: Fri Apr 12 06:06:13 2024, max compression
```

## Comparing `tsugu-0.3.0.tar` & `tsugu-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:42.430611 tsugu-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 03:46:32.000000 tsugu-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 03:46:42.430611 tsugu-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-12 03:46:32.000000 tsugu-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:46:42.430611 tsugu-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 03:46:32.000000 tsugu-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:42.430611 tsugu-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-12 03:46:32.000000 tsugu-0.3.0/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:42.430611 tsugu-0.3.0/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19678 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:42.430611 tsugu-0.3.0/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:13.058664 tsugu-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 06:06:04.000000 tsugu-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 06:06:13.058664 tsugu-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-12 06:06:04.000000 tsugu-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:06:13.058664 tsugu-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 06:06:04.000000 tsugu-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:13.058664 tsugu-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-12 06:06:04.000000 tsugu-0.3.1/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:13.058664 tsugu-0.3.1/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19678 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:13.058664 tsugu-0.3.1/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 06:06:12.000000 tsugu-0.3.1/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 06:06:13.000000 tsugu-0.3.1/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:06:12.000000 tsugu-0.3.1/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 06:06:12.000000 tsugu-0.3.1/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 06:06:12.000000 tsugu-0.3.1/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.3.0/LICENSE` & `tsugu-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.0/PKG-INFO` & `tsugu-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.3.0 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.1 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.3.0/README.md` & `tsugu-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.0/setup.py` & `tsugu-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.3.0',
+    version='0.3.1',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.3.0/test/test_main.py` & `tsugu-0.3.1/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.0/tsugu/bot.py` & `tsugu-0.3.1/tsugu/bot.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.0/tsugu/config.py` & `tsugu-0.3.1/tsugu/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 import json
 
+
 class Config:
     def __init__(self):
         # 设置默认值
         self.backend = "http://tsugubot.com:8080"
         self.user_data_backend = "http://tsugubot.com:8080"
         self.user_database_path = None
 
         self.use_proxies = False
         self.proxies = {
             "http": "http://127.0.0.1:7890",
-            "https": "http://127.0.0.1:7890"
+            "https": "http://127.0.0.1:7890",
         }
 
         self.token_name = "Tsugu"
         self.bandori_station_token = "ZtV4EX2K9Onb"
 
         self.use_easy_bg = True
         self.compress = True
 
         self.ban_gacha_simulate_group_data = []
 
-        self.server_list = {
-            0: "日服",
-            1: "国际服",
-            2: "台服",
-            3: "国服",
-            4: "韩服"
-        }
+        self.server_list = {0: "日服", 1: "国际服", 2: "台服", 3: "国服", 4: "韩服"}
         self.server_name_to_index = {
             "日服": "0",
             "国际服": "1",
             "台服": "2",
             "国服": "3",
             "韩服": "4",
             "jp": "0",
@@ -68,196 +63,304 @@
             {"api": "character", "command_name": ["查角色"]},
             {"api": "chart", "command_name": ["查铺面", "查谱面"]},
             {"api": "ycxAll", "command_name": ["ycxall", "ycx all"]},
             {"api": "ycx", "command_name": ["ycx", "预测线"]},
             {"api": "lsycx", "command_name": ["lsycx"]},
             {"api": "ycm", "command_name": ["ycm", "车来"]},
             {"api": "card", "command_name": ["查卡"]},
-
         ]
 
         self.car_config = {
-            "car": ["q1", "q2", "q3", "q4", "Q1", "Q2", "Q3", "Q4", "缺1", "缺2", "缺3", "缺4", "差1", "差2", "差3", "差4",
-                    "3火", "三火", "3把", "三把", "打满", "清火", "奇迹", "中途", "大e", "大分e", "exi", "大分跳", "大跳", "大a", "大s",
-                    "大分a", "大分s", "长途", "生日车", "军训", "禁fc"],
-            "fake": ["114514", "野兽", "恶臭", "1919", "下北泽", "粪", "糞", "臭", "11451", "xiabeize", "雀魂", "麻将", "打牌",
-                     "maj", "麻", "[", "]", "断幺", "qq.com", "腾讯会议", "master", "疯狂星期四", "离开了我们", "日元", "av", "bv"]
+            "car": [
+                "q1",
+                "q2",
+                "q3",
+                "q4",
+                "Q1",
+                "Q2",
+                "Q3",
+                "Q4",
+                "缺1",
+                "缺2",
+                "缺3",
+                "缺4",
+                "差1",
+                "差2",
+                "差3",
+                "差4",
+                "3火",
+                "三火",
+                "3把",
+                "三把",
+                "打满",
+                "清火",
+                "奇迹",
+                "中途",
+                "大e",
+                "大分e",
+                "exi",
+                "大分跳",
+                "大跳",
+                "大a",
+                "大s",
+                "大分a",
+                "大分s",
+                "长途",
+                "生日车",
+                "军训",
+                "禁fc",
+            ],
+            "fake": [
+                "114514",
+                "野兽",
+                "恶臭",
+                "1919",
+                "下北泽",
+                "粪",
+                "糞",
+                "臭",
+                "11451",
+                "xiabeize",
+                "雀魂",
+                "麻将",
+                "打牌",
+                "maj",
+                "麻",
+                "[",
+                "]",
+                "断幺",
+                "qq.com",
+                "腾讯会议",
+                "master",
+                "疯狂星期四",
+                "离开了我们",
+                "日元",
+                "av",
+                "bv",
+            ],
         }
 
     def show_docs(self):
-        '''
-Config 属性文档:
+        """
+        Config 属性文档:
 
-backend (str)
-    默认值: "http://tsugubot.com:8080"
-    描述: 应用程序的后端服务地址，需要 v2 API 。
-
-user_data_backend (str)
-    默认值: "http://tsugubot.com:8080"
-    描述: 应用程序的后端服务地址，需要 v2 API ， 需要启动数据库服务。
-
-utils_backend (str)
-    默认值: "http://tsugubot.com:8080"
-    描述: utils api 的后端地址，需要 v2 API 。
-
-use_proxies (bool)
-    默认值: False
-    描述: 是否通过代理服务器访问网络服务。
-
-proxies (dict)
-    默认值: {"http": "http://127.0.0.1:7890", "https": "http://127.0.0.1:7890"}
-    描述: 代理服务器的地址配置，use_proxies 为 True 时生效。
-
-token_name (str)
-    默认值: "Tsugu"
-    描述: Bandori 车站 的上传令牌名称，通常需要和 bandori_station_token 一对应。
-
-bandori_station_token (str)
-    默认值: "ZtV4EX2K9Onb"
-    描述: Bandori 车站 的上传令牌，通常需要和 token_name 一对应。
-
-use_easy_bg (bool)
-    默认值: True
-    描述: 是否使用简易背景模式。
-
-compress (bool)
-    默认值: True
-    描述: 是否开启数据压缩。
-
-ban_gacha_simulate_group_data (list)
-    默认值: []
-    描述: 禁止抽卡模拟的群组数据列表。
-    事例: ["114514", "1919810"]
-
-server_list (dict)
-    默认值: {1: "日服", 2: "国际服", 3: "台服", 4: "韩服"}
-    描述: 服务器列表及其对应的名称。
-
-server_index_to_name (dict)
-    默认值: {"1": "日服", "2": "国际服", "3": "台服", "4": "韩服"}
-    描述: 服务器索引到名称的映射。
-
-server_index_to_s_name (dict)
-    默认值: {"1": "jp", "2": "en", "3": "tw", "4": "kr"}
-    描述: 服务器索引到简称的映射。
-
-name_to_server_index (dict)
-    默认值: {"日服": "1", "国际服": "2", "台服": "3", "韩服": "4"}
-    描述: 服务器名称到索引的映射。
-
-commands (list[dict])
-    默认值: 包含多个字典，每个字典包含api和command_name键。
-    描述: 应用程序支持的命令列表及其对应的API接口。
-    查看默认值: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py/blob/main/tsugu/config.py#L29
-
-car_config (dict)
-    默认值: 包含两个键car和fake，每个键对应一个字符串列表。
-    描述: 车辆配置，包含车辆相关的命令及排除词汇。
-    查看默认值: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py/blob/main/tsugu/config.py#L45
-        '''
+        backend (str)
+            默认值: "http://tsugubot.com:8080"
+            描述: 应用程序的后端服务地址，需要 v2 API 。
+
+        user_data_backend (str)
+            默认值: "http://tsugubot.com:8080"
+            描述: 应用程序的后端服务地址，需要 v2 API ， 需要启动数据库服务。
+
+        utils_backend (str)
+            默认值: "http://tsugubot.com:8080"
+            描述: utils api 的后端地址，需要 v2 API 。
+
+        use_proxies (bool)
+            默认值: False
+            描述: 是否通过代理服务器访问网络服务。
+
+        proxies (dict)
+            默认值: {"http": "http://127.0.0.1:7890", "https": "http://127.0.0.1:7890"}
+            描述: 代理服务器的地址配置，use_proxies 为 True 时生效。
+
+        token_name (str)
+            默认值: "Tsugu"
+            描述: Bandori 车站 的上传令牌名称，通常需要和 bandori_station_token 一对应。
+
+        bandori_station_token (str)
+            默认值: "ZtV4EX2K9Onb"
+            描述: Bandori 车站 的上传令牌，通常需要和 token_name 一对应。
+
+        use_easy_bg (bool)
+            默认值: True
+            描述: 是否使用简易背景模式。
+
+        compress (bool)
+            默认值: True
+            描述: 是否开启数据压缩。
+
+        ban_gacha_simulate_group_data (list)
+            默认值: []
+            描述: 禁止抽卡模拟的群组数据列表。
+            事例: ["114514", "1919810"]
+
+        server_list (dict)
+            默认值: {1: "日服", 2: "国际服", 3: "台服", 4: "韩服"}
+            描述: 服务器列表及其对应的名称。
+
+        server_index_to_name (dict)
+            默认值: {"1": "日服", "2": "国际服", "3": "台服", "4": "韩服"}
+            描述: 服务器索引到名称的映射。
+
+        server_index_to_s_name (dict)
+            默认值: {"1": "jp", "2": "en", "3": "tw", "4": "kr"}
+            描述: 服务器索引到简称的映射。
+
+        name_to_server_index (dict)
+            默认值: {"日服": "1", "国际服": "2", "台服": "3", "韩服": "4"}
+            描述: 服务器名称到索引的映射。
+
+        commands (list[dict])
+            默认值: 包含多个字典，每个字典包含api和command_name键。
+            描述: 应用程序支持的命令列表及其对应的API接口。
+            查看默认值: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py/blob/main/tsugu/config.py#L29
+
+        car_config (dict)
+            默认值: 包含两个键car和fake，每个键对应一个字符串列表。
+            描述: 车辆配置，包含车辆相关的命令及排除词汇。
+            查看默认值: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py/blob/main/tsugu/config.py#L45
+        """
         print(self.show_docs.__doc__)
         return self.__doc__
-    
-    
+
     def output_config_json(self, path="./config.json"):
         config_pre_json = {
-    "backend": "http://tsugubot.com:8080",
-    "user_data_backend": "http://tsugubot.com:8080",
-    "user_database_path": None,
-
-    "use_proxies": True,
-    "proxies": {
-        "http": "http://localhost:7890",
-        "https": "http://localhost:7890"
-    },
-
-    "token_name": "TsuguToken",
-    "bandori_station_token": "NewToken123456",
-
-    "use_easy_bg": False,
-    "compress": False,
-
-    "ban_gacha_simulate_group_data": ["123456", "789010"],
-
-    "server_list": {
-        "0": "日服",
-        "1": "国际服",
-        "2": "台服",
-        "3": "国服",
-        "4": "韩服"
-    },
-
-    "server_name_to_index": {
-        "日服": "0",
-        "国际服": "1",
-        "台服": "2",
-        "国服": "3",
-        "韩服": "4",
-        "jp": "0",
-        "en": "1",
-        "tw": "2",
-        "cn": "3",
-        "kr": "4"
-    },
-
-    "server_index_to_name": {
-        "0": "日服",
-        "1": "国际服",
-        "2": "台服",
-        "3": "国服",
-        "4": "韩服"
-    },
-
-    "server_index_to_s_name": {
-        "0": "jp",
-        "1": "en",
-        "2": "tw",
-        "3": "cn",
-        "4": "kr"
-    },
-    "commands": [
-        {"api": "cardIllustration", "command_name": ["查插画", "查卡面"]},
-        {"api": "player", "command_name": ["查玩家", "查询玩家"]},
-        {"api": "gachaSimulate", "command_name": ["抽卡模拟", "卡池模拟"]},
-        {"api": "gacha", "command_name": ["查卡池"]},
-        {"api": "event", "command_name": ["查活动"]},
-        {"api": "song", "command_name": ["查歌曲", "查曲"]},
-        {"api": "songMeta", "command_name": ["查询分数表", "查分数表"]},
-        {"api": "character", "command_name": ["查角色"]},
-        {"api": "chart", "command_name": ["查铺面", "查谱面"]},
-        {"api": "ycxAll", "command_name": ["ycxall", "ycx all"]},
-        {"api": "ycx", "command_name": ["ycx", "预测线"]},
-        {"api": "lsycx", "command_name": ["lsycx"]},
-        {"api": "ycm", "command_name": ["ycm", "车来"]},
-        {"api": "card", "command_name": ["查卡"]}
-    ],
-    "car_config": {
-        "car": [
-            "q1", "q2", "q3", "q4", "Q1", "Q2", "Q3", "Q4", "缺1", "缺2", "缺3", "缺4",
-            "差1", "差2", "差3", "差4", "3火", "三火", "3把", "三把", "打满", "清火", "奇迹", "中途",
-            "大e", "大分e", "exi", "大分跳", "大跳", "大a", "大s", "大分a", "大分s", "长途", "生日车", "军训", "禁fc"
-        ],
-        "fake": [
-            "114514", "野兽", "恶臭", "1919", "下北泽", "粪", "糞", "臭", "11451", "xiabeize", "雀魂", "麻将", "打牌",
-            "maj", "麻", "[", "]", "断幺", "qq.com", "腾讯会议", "master", "疯狂星期四", "离开了我们", "日元", "av", "bv"
-        ]
-    }
-}
-        with open(path, 'w', encoding='utf-8') as f:
+            "backend": "http://tsugubot.com:8080",
+            "user_data_backend": "http://tsugubot.com:8080",
+            "user_database_path": None,
+            "use_proxies": True,
+            "proxies": {
+                "http": "http://localhost:7890",
+                "https": "http://localhost:7890",
+            },
+            "token_name": "Tsugu",
+            "bandori_station_token": "ZtV4EX2K9Onb",
+            "use_easy_bg": False,
+            "compress": False,
+            "ban_gacha_simulate_group_data": [],
+            "server_list": {
+                "0": "日服",
+                "1": "国际服",
+                "2": "台服",
+                "3": "国服",
+                "4": "韩服",
+            },
+            "server_name_to_index": {
+                "日服": "0",
+                "国际服": "1",
+                "台服": "2",
+                "国服": "3",
+                "韩服": "4",
+                "jp": "0",
+                "en": "1",
+                "tw": "2",
+                "cn": "3",
+                "kr": "4",
+            },
+            "server_index_to_name": {
+                "0": "日服",
+                "1": "国际服",
+                "2": "台服",
+                "3": "国服",
+                "4": "韩服",
+            },
+            "server_index_to_s_name": {
+                "0": "jp",
+                "1": "en",
+                "2": "tw",
+                "3": "cn",
+                "4": "kr",
+            },
+            "commands": [
+                {"api": "cardIllustration", "command_name": ["查插画", "查卡面"]},
+                {"api": "player", "command_name": ["查玩家", "查询玩家"]},
+                {"api": "gachaSimulate", "command_name": ["抽卡模拟", "卡池模拟"]},
+                {"api": "gacha", "command_name": ["查卡池"]},
+                {"api": "event", "command_name": ["查活动"]},
+                {"api": "song", "command_name": ["查歌曲", "查曲"]},
+                {"api": "songMeta", "command_name": ["查询分数表", "查分数表"]},
+                {"api": "character", "command_name": ["查角色"]},
+                {"api": "chart", "command_name": ["查铺面", "查谱面"]},
+                {"api": "ycxAll", "command_name": ["ycxall", "ycx all"]},
+                {"api": "ycx", "command_name": ["ycx", "预测线"]},
+                {"api": "lsycx", "command_name": ["lsycx"]},
+                {"api": "ycm", "command_name": ["ycm", "车来"]},
+                {"api": "card", "command_name": ["查卡"]},
+            ],
+            "car_config": {
+                "car": [
+                    "q1",
+                    "q2",
+                    "q3",
+                    "q4",
+                    "Q1",
+                    "Q2",
+                    "Q3",
+                    "Q4",
+                    "缺1",
+                    "缺2",
+                    "缺3",
+                    "缺4",
+                    "差1",
+                    "差2",
+                    "差3",
+                    "差4",
+                    "3火",
+                    "三火",
+                    "3把",
+                    "三把",
+                    "打满",
+                    "清火",
+                    "奇迹",
+                    "中途",
+                    "大e",
+                    "大分e",
+                    "exi",
+                    "大分跳",
+                    "大跳",
+                    "大a",
+                    "大s",
+                    "大分a",
+                    "大分s",
+                    "长途",
+                    "生日车",
+                    "军训",
+                    "禁fc",
+                ],
+                "fake": [
+                    "114514",
+                    "野兽",
+                    "恶臭",
+                    "1919",
+                    "下北泽",
+                    "粪",
+                    "糞",
+                    "臭",
+                    "11451",
+                    "xiabeize",
+                    "雀魂",
+                    "麻将",
+                    "打牌",
+                    "maj",
+                    "麻",
+                    "[",
+                    "]",
+                    "断幺",
+                    "qq.com",
+                    "腾讯会议",
+                    "master",
+                    "疯狂星期四",
+                    "离开了我们",
+                    "日元",
+                    "av",
+                    "bv",
+                ],
+            },
+        }
+        with open(path, "w", encoding="utf-8") as f:
             json.dump(config_pre_json, f, ensure_ascii=False, indent=4)
         print(f"Config data has been output to '{path}'.")
 
     def reload_from_json(self, path):
         """Reloads configuration data from a JSON string or a JSON file path."""
-        with open(path, 'r') as file:
+        with open(path, "r") as file:
             config_data = json.load(file)
         # Iterate over all keys in the input JSON and update the config attributes
         for key, value in config_data.items():
             if hasattr(self, key):
                 setattr(self, key, value)
             else:
                 print(f"Warning: {key} is not a recognized configuration attribute.")
 
 
 config = Config()
-
-
```

### Comparing `tsugu-0.3.0/tsugu/router.py` & `tsugu-0.3.1/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.0/tsugu/utils.py` & `tsugu-0.3.1/tsugu/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.0/tsugu.egg-info/PKG-INFO` & `tsugu-0.3.1/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.3.0 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.1 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

