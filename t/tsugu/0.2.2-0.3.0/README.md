# Comparing `tmp/tsugu-0.2.2.tar.gz` & `tmp/tsugu-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.2.2.tar", last modified: Sun Mar 17 11:29:00 2024, max compression
+gzip compressed data, was "tsugu-0.3.0.tar", last modified: Fri Apr 12 03:46:42 2024, max compression
```

## Comparing `tsugu-0.2.2.tar` & `tsugu-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:29:00.851662 tsugu-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-17 11:28:49.000000 tsugu-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-03-17 11:29:00.851662 tsugu-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-03-17 11:28:49.000000 tsugu-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 11:29:00.851662 tsugu-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-17 11:28:49.000000 tsugu-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:29:00.847662 tsugu-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-17 11:28:49.000000 tsugu-0.2.2/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:29:00.847662 tsugu-0.2.2/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-17 11:28:49.000000 tsugu-0.2.2/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-03-17 11:28:49.000000 tsugu-0.2.2/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-03-17 11:28:49.000000 tsugu-0.2.2/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-17 11:28:49.000000 tsugu-0.2.2/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19873 2024-03-17 11:28:49.000000 tsugu-0.2.2/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:29:00.851662 tsugu-0.2.2/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-03-17 11:29:00.000000 tsugu-0.2.2/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-17 11:29:00.000000 tsugu-0.2.2/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 11:29:00.000000 tsugu-0.2.2/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-17 11:29:00.000000 tsugu-0.2.2/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-17 11:29:00.000000 tsugu-0.2.2/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:42.430611 tsugu-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 03:46:32.000000 tsugu-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 03:46:42.430611 tsugu-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-12 03:46:32.000000 tsugu-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:46:42.430611 tsugu-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 03:46:32.000000 tsugu-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:42.430611 tsugu-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-12 03:46:32.000000 tsugu-0.3.0/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:42.430611 tsugu-0.3.0/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19678 2024-04-12 03:46:32.000000 tsugu-0.3.0/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:42.430611 tsugu-0.3.0/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 03:46:42.000000 tsugu-0.3.0/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.2.2/LICENSE` & `tsugu-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.2.2/PKG-INFO` & `tsugu-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.2.2
+Version: 0.3.0
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.2.2 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.0 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.2.2/README.md` & `tsugu-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.2.2/setup.py` & `tsugu-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.2.2',
+    version='0.3.0',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.2.2/test/test_main.py` & `tsugu-0.3.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.2.2/tsugu/bot.py` & `tsugu-0.3.0/tsugu/bot.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,45 +16,45 @@
     if config.user_database_path:
         return bot_extra_local_database(message, user_id, platform)
     return bot_extra_remote_server(message, user_id, platform)
 
 
 def bot_extra_local_database(message, user_id, platform):
     if message.endswith('服玩家状态'):
-        return player_status(user_id, platform, message[:-4]) if server_exists(r_ := query_server_info(message[:-4])) else text_response('服务器没找到喵') if len(message) <= 7 else None
+        return player_status(user_id, platform, message[:-4]) if server_exists(r_ := query_server_info(message[:-4])) else text_response('未找到被指定的服务器') if len(message) <= 7 else None
 
     if message.startswith('玩家状态'):
         if (arg_ := message[4:].strip()) == '':
             return player_status(user_id, platform)
         # 如果用户输入了数字
         if arg_.isdigit():
             return player_status(user_id, platform, int(arg_))
         # 如果用户输入了服务器名
         if server_exists(r_ := query_server_info(arg_)):
             return player_status(user_id, platform, arg_)
         else:
-            return text_response('没找到您要求的服务器或记录喵')
+            return text_response('未找到绑定记录')
 
 
     if message.startswith('绑定玩家') and len(message.replace('绑定玩家', '').strip()) < 4:
         # 如果匹配 绑定玩家 则绑定默认服务器的玩家 如果用户输入了服务器名 则绑定对应服务器的玩家，如果服务器名无效则 赋值为 None
         return bind_player_request(platform, user_id)
 
     if message.startswith('验证'):
         arg = message.replace('验证', '').strip()
         # if len(arg_list) < 1:  # 如果长度小于2
         #     return text_response('请输入正确')
         # if not arg_list[0].isdigit():  # 如果第一个不是数字
-        #     return text_response('请确保您输入正确(例如: 验证 123456 cn)')
+        #     return text_response('请确保输入正确(例如: 验证 123456 cn)')
         # server = query_server_info(arg_list[-1])
         # player_id = arg_list[0]
         # 正则出数字
         player_ids = re.findall(r'\d+', arg)
         if not player_ids or len(player_ids) > 1:
-            return text_response('请确保您输入正确(例如: 验证 123456 cn)')
+            return text_response('请确保输入正确(例如: 验证 10000xxxxx cn)')
         player_id = player_ids[0]
         server = query_server_info(arg.replace(player_id, ''))  # 后续自动处理 None
         print(server, type(server))
         return bind_player_verification(platform, user_id, server, player_id, True)
 
     if message.startswith('解除绑定'):
         if message[4:].strip() == '':
@@ -62,15 +62,15 @@
         msg_list = message.split(' ')
         if len(msg_list) < 2:
             return unbind_player_request(platform, user_id)
         if not msg_list[-1].isdigit():
             return unbind_player_request(platform, user_id)
         record = int(msg_list[-1])
         if record == 0:
-            return text_response('为什么会有0啊（')
+            return text_response('为什么会有0啊，服了')
         return unbind_player_verification(platform, user_id, record)
 
     if message in ['开启车牌转发', '开启个人车牌转发']:
         return set_car_forward(platform, user_id, True)
 
     if message in ['关闭车牌转发', '关闭个人车牌转发']:
         return set_car_forward(platform, user_id, False)
@@ -87,59 +87,60 @@
 
     return None
 
 
 def bot_extra_remote_server(message, user_id, platform):
     if message.endswith('服玩家状态'):
         # 如果匹配 *服玩家状态 则查询对应服务器的玩家状态 前提是用户输入的 * 是一个有效的服务器名 否则返回None
-        return Remote.player_status(user_id, platform, r_) if server_exists(r_ := query_server_info(message[:-4])) else text_response('服务器没找到喵') if len(message) <= 7 else None
+        return Remote.player_status(user_id, platform, r_) if server_exists(r_ := query_server_info(message[:-4])) else text_response('未找到服务器') if len(message) <= 7 else None
 
     if message.startswith('玩家状态'):
         # 如果匹配 玩家状态 则查询默认服务器的玩家状态 如果用户输入了服务器名 则查询对应服务器的玩家状态，如果服务器名无效则返回None
         return Remote.player_status(user_id, platform) if (arg_ := message[4:].strip()) == '' else (Remote.player_status(user_id, platform, r_) if server_exists(r_ := query_server_info(arg_)) else None)
 
     if message.startswith('绑定玩家'):
         # 如果匹配 绑定玩家 则绑定默认服务器的玩家 如果用户输入了服务器名 则绑定对应服务器的玩家，如果服务器名无效则 赋值为 None
         server = Remote.get_user_data(platform, user_id)['data']['server_mode'] if message[4:].strip() == '' else (r_ if server_exists(r_ := query_server_info(message[4:])) else None)
         if not server_exists(server):
-            return text_response(f'未找到名为 {message[4:]} 的服务器信息，请确保您输入的是服务器名而不是玩家ID，通常情况您只需要发送"绑定玩家"或"绑定玩家 服务器"即可')
+            return text_response(f'未找到名为 {message[4:]} 的服务器信息，请确保输入是服务器名而不是玩家ID，通常情况发送"绑定玩家"或"绑定玩家 服务器"即可')
 
         res = Remote.bind_player_request(platform, user_id, server, True)
         if res.get('status') != 'success':
             print(res)
             # {'status': 'success', 'data': {'verifyCode': 12492}}
-            return text_response(res.get('data') + ' 喵')
+            return text_response(res.get('data'))
         # if not res.get('status') == 'failed':
         #     return text_response('未知错误喵')
-        return text_response(f'''正在绑定账号，请将您的 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{res.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证 + 空格 + 您的玩家ID 来完成本次身份验证\n验证 10000xxxx 国服''')
+        return text_response(f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{res.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证 + 空格 + 玩家ID 来完成本次身份验证\n验证 10000xxxx 国服''')
 
     if message.startswith('解除绑定'):
         server = Remote.get_user_data(platform, user_id)['data']['server_mode'] if message[4:].strip() == '' else (r_ if (config.server_list(r_ := query_server_info(message[4:]))) else None)
-        if not server:
-            return text_response(f'未找到名为 {message[4:].strip()} 的服务器信息，请确保您输入的是服务器名而不是玩家ID，通常情况您只需要发送"解除绑定"即可')
+        if server_exists(server) is False:
+            # print(server)
+            return text_response(f'未找到名为 {message[4:].strip()} 的服务器信息，请确保输入的是服务器名而不是玩家ID，通常情况发送"解除绑定"即可')
         response = Remote.bind_player_request(platform, user_id, server, False)  # 获取响应
         if response.get('status') == 'failed':  # 检查状态
-            return text_response(response.get('data') + ' 喵')
+            return text_response(response.get('data'))
         # 如果是200
-        return text_response(f'''正在解除，请将您的 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{response.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {server}\n来完成本次身份验证(没错只需要加上 {server} 来确定您需要解绑的服务器)''')
+        return text_response(f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{response.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {server}\n来完成本次身份验证(没错只需要加上 {server} 来确定需要解绑的服务器)''')
 
     if message.startswith('验证解绑'):
         if not message[4:].strip().isdigit():
             return text_response('请输入解绑时提供的serverID(数字)')
         r = Remote.bind_player_verification(platform, user_id, int(message[4:].strip()), Remote.get_user_data(platform, user_id)['data']['server_list'][int(message[4:].strip())]['playerId'], False)
         if r.get('status') == 'failed':
-            return text_response(r.get('data') + ' 喵')
-        return text_response('解绑成功喵！')
+            return text_response(r.get('data'))
+        return text_response('解绑成功')
 
     if message.startswith('验证'):
         if not message[2:].strip().isdigit():
             return text_response('请输入正确的玩家ID(数字)')
         if r := Remote.bind_player_verification(platform, user_id, Remote.get_user_data(platform, user_id)['data']['server_mode'], message[2:].strip(), True).get('status') == 'failed':
-            return text_response(r.get('data') + ' 喵') if r.get('data') != '错误: 未请求绑定或解除绑定玩家' else None
-        return text_response('绑定成功！现在可以使用"玩家状态"来查询玩家信息了～')
+            return text_response(r.get('data')) if r.get('data') != '错误: 未请求绑定或解除绑定玩家' else None
+        return text_response('绑定成功！现在可以使用"玩家状态"来查询玩家信息')
 
     if message in ['开启车牌转发', '开启个人车牌转发']:
         r = Remote.set_car_forward(platform, user_id, True)
         return text_response('已开启车牌转发') if r.get('status') == 'success' else None
 
     if message in ['关闭车牌转发', '关闭个人车牌转发']:
         r = Remote.set_car_forward(platform, user_id, False)
```

### Comparing `tsugu-0.2.2/tsugu/config.py` & `tsugu-0.3.0/tsugu/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 
 class Config:
     def __init__(self):
         # 设置默认值
         self.backend = "http://tsugubot.com:8080"
         self.user_data_backend = "http://tsugubot.com:8080"
         self.user_database_path = None
@@ -143,52 +144,120 @@
     默认值: {"日服": "1", "国际服": "2", "台服": "3", "韩服": "4"}
     描述: 服务器名称到索引的映射。
 
 commands (list[dict])
     默认值: 包含多个字典，每个字典包含api和command_name键。
     描述: 应用程序支持的命令列表及其对应的API接口。
     查看默认值: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py/blob/main/tsugu/config.py#L29
-    可用函数: add_command_name, remove_command_name
 
 car_config (dict)
     默认值: 包含两个键car和fake，每个键对应一个字符串列表。
     描述: 车辆配置，包含车辆相关的命令及排除词汇。
     查看默认值: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py/blob/main/tsugu/config.py#L45
         '''
         print(self.show_docs.__doc__)
         return self.__doc__
-
-    def add_command_name(self, api: str, command_name: str):
-        """
-        添加指令名
-        """
-        for command in self.commands:
-            if command['api'] == api:
-                if command_name not in command['command_name']:
-                    command['command_name'].append(command_name)
-                else:
-                    print(f"command_name '{command_name}' already exists in api '{api}'.")
-                break
-        else:
-            print(f"command_name '{command_name}' not found.")
-        print(f"command_name '{command_name}' added to api '{api}'.")
-        return self
-
-    def remove_command_name(self, api: str, command_name: str):
-        """
-        删除指令名 (如果全删了则不会触发此命令)
-        """
-        for command in self.commands:
-            if command['api'] == api:
-                if command_name in command['command_name']:
-                    command['command_name'].remove(command_name)
-                else:
-                    print(f"command_name '{command_name}' does not exist in api '{api}'.")
-                break
-        else:
-            print(f"api '{api}' not found.")
-        print(f"command_name '{command_name}' removed from api '{api}'.")
+    
+    
+    def output_config_json(self, path="./config.json"):
+        config_pre_json = {
+    "backend": "http://tsugubot.com:8080",
+    "user_data_backend": "http://tsugubot.com:8080",
+    "user_database_path": None,
+
+    "use_proxies": True,
+    "proxies": {
+        "http": "http://localhost:7890",
+        "https": "http://localhost:7890"
+    },
+
+    "token_name": "TsuguToken",
+    "bandori_station_token": "NewToken123456",
+
+    "use_easy_bg": False,
+    "compress": False,
+
+    "ban_gacha_simulate_group_data": ["123456", "789010"],
+
+    "server_list": {
+        "0": "日服",
+        "1": "国际服",
+        "2": "台服",
+        "3": "国服",
+        "4": "韩服"
+    },
+
+    "server_name_to_index": {
+        "日服": "0",
+        "国际服": "1",
+        "台服": "2",
+        "国服": "3",
+        "韩服": "4",
+        "jp": "0",
+        "en": "1",
+        "tw": "2",
+        "cn": "3",
+        "kr": "4"
+    },
+
+    "server_index_to_name": {
+        "0": "日服",
+        "1": "国际服",
+        "2": "台服",
+        "3": "国服",
+        "4": "韩服"
+    },
+
+    "server_index_to_s_name": {
+        "0": "jp",
+        "1": "en",
+        "2": "tw",
+        "3": "cn",
+        "4": "kr"
+    },
+    "commands": [
+        {"api": "cardIllustration", "command_name": ["查插画", "查卡面"]},
+        {"api": "player", "command_name": ["查玩家", "查询玩家"]},
+        {"api": "gachaSimulate", "command_name": ["抽卡模拟", "卡池模拟"]},
+        {"api": "gacha", "command_name": ["查卡池"]},
+        {"api": "event", "command_name": ["查活动"]},
+        {"api": "song", "command_name": ["查歌曲", "查曲"]},
+        {"api": "songMeta", "command_name": ["查询分数表", "查分数表"]},
+        {"api": "character", "command_name": ["查角色"]},
+        {"api": "chart", "command_name": ["查铺面", "查谱面"]},
+        {"api": "ycxAll", "command_name": ["ycxall", "ycx all"]},
+        {"api": "ycx", "command_name": ["ycx", "预测线"]},
+        {"api": "lsycx", "command_name": ["lsycx"]},
+        {"api": "ycm", "command_name": ["ycm", "车来"]},
+        {"api": "card", "command_name": ["查卡"]}
+    ],
+    "car_config": {
+        "car": [
+            "q1", "q2", "q3", "q4", "Q1", "Q2", "Q3", "Q4", "缺1", "缺2", "缺3", "缺4",
+            "差1", "差2", "差3", "差4", "3火", "三火", "3把", "三把", "打满", "清火", "奇迹", "中途",
+            "大e", "大分e", "exi", "大分跳", "大跳", "大a", "大s", "大分a", "大分s", "长途", "生日车", "军训", "禁fc"
+        ],
+        "fake": [
+            "114514", "野兽", "恶臭", "1919", "下北泽", "粪", "糞", "臭", "11451", "xiabeize", "雀魂", "麻将", "打牌",
+            "maj", "麻", "[", "]", "断幺", "qq.com", "腾讯会议", "master", "疯狂星期四", "离开了我们", "日元", "av", "bv"
+        ]
+    }
+}
+        with open(path, 'w', encoding='utf-8') as f:
+            json.dump(config_pre_json, f, ensure_ascii=False, indent=4)
+        print(f"Config data has been output to '{path}'.")
+
+    def reload_from_json(self, path):
+        """Reloads configuration data from a JSON string or a JSON file path."""
+        with open(path, 'r') as file:
+            config_data = json.load(file)
+        # Iterate over all keys in the input JSON and update the config attributes
+        for key, value in config_data.items():
+            if hasattr(self, key):
+                setattr(self, key, value)
+            else:
+                print(f"Warning: {key} is not a recognized configuration attribute.")
 
 
 config = Config()
```

### Comparing `tsugu-0.2.2/tsugu/router.py` & `tsugu-0.3.0/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.2.2/tsugu/utils.py` & `tsugu-0.3.0/tsugu/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,16 @@
     # 获取用户数据
     user_data = get_user_data(platform, user_id) if config.user_database_path else Remote.get_user_data(platform, user_id)
     print(user_data)
     try:
         if user_data['status'] != 'success':
             return text_response('获取用户数据失败')
         return v2api_from_backend(api, text, user_data['data']['default_server'], user_data['data']['server_mode'])
-    except:
-
-        return text_response('前端错误')
-
+    except Exception as e:
+        return text_response('前端错误: ' + str(e))
 
 def set_car_forward(platform, user_id, status):
     data = {
         'platform': platform,
         'user_id': user_id,
         'status': status
     }
@@ -274,47 +272,47 @@
         # 先查找默认服务器对应的记录
         server: int = user_data['data']['server_mode']
         for i in game_ids:
             if i.get("server") == server:
                 player_id = str(i.get("game_id"))
                 server = int(i.get("server"))
 
-                text = f'已为您查找默认服务器 {config.server_index_to_name[str(server)]} 的记录。'
+                text = f'已查找默认服务器 {config.server_index_to_name[str(server)]} 的记录'
                 # print(player_id, server)
                 break
         else:
             # 再查找第一个记录
             if game_ids:
                 # print(player_id, server)
-                return text_response(f'未在您的 {len(game_ids)} 条记录中找到 {config.server_index_to_name[str(server)]} 的记录喵。')
+                return text_response(f'未在 {len(game_ids)} 条记录中找到 {config.server_index_to_name[str(server)]} 的记录')
             else:
                 pass  # 前面已经判断过了没绑定任何的情况
     elif isinstance(args, int):
         # 查找对应数字的记录
         if args == 0:
             return text_response('哪来的0（')
         if args > len(game_ids) or args < 1:
-            return text_response(f'您只有 {len(game_ids)} 条记录可以查喵')
+            return text_response(f'总共绑定了 {len(game_ids)} 条记录')
         player_id, server = str(game_ids[args - 1].get("game_id")), game_ids[args - 1].get("server")
-        text = f'已为您查找第{args}条记录。'
+        text = f'已为查找第{args}条记录'
         if not player_id:
-            return text_response(f'未找到此服务器的记录，请检查您的是否绑定过此服务器。')
+            return text_response(f'未找到此服务器的记录，请检查是否绑定过此服务器')
 
     elif isinstance(args, str):
         server = query_server_info(args)
         # 查找对应服务器的记录
         for i in game_ids:
             if i.get("server") == server:
                 player_id = str(i.get("game_id"))
-                text = f'已为您查找服务器 {config.server_index_to_name[str(server)]} 的记录。'
+                text = f'已查找服务器 {config.server_index_to_name[str(server)]} 的记录'
                 break
         else:
-            return text_response(f'未找到记录，请检查您的是否绑定过此服务器。')
+            return text_response(f'未找到记录，请检查是否绑定过此服务器')
     else:
-        return text_response('参数错误，您输入的服务器可能不合法。')
+        return text_response('参数错误，的服务器可能不合法')
     result: list = v2api_from_backend('player', player_id, server=server)
     new_item = {"type": "string", "string": text}
     result.append(new_item)
     return result
 
 
 def set_car_forward(platform, user_id, status: bool):
@@ -342,15 +340,15 @@
     return text_response(f'默认服务器设置为 {text}')
 
 
 def set_server_mode(platform, user_id, text):
 
     server = int(convert_server_names_to_indices(text)[0]) if convert_server_names_to_indices(text) else None
     if server is None:
-        return text_response(f'未找到名为 {text} 的服务器信息。')
+        return text_response(f'未找到名为 {text} 的服务器信息')
     get_user_data(platform, user_id)
     cursor = db_manager.conn.cursor()
     cursor.execute("UPDATE users SET server_mode = ? WHERE user_id = ? AND platform = ?",
                    (server, user_id, platform))
     db_manager.conn.commit()
     return text_response(f'服务器模式设置为 {text}')
 
@@ -367,74 +365,74 @@
             verify_code = random.randint(10000, 99999)
             if '64' not in str(verify_code) and '89' not in str(verify_code):
                 return verify_code
     # 不包含64和89的随机数
 
     verify_code = generate_verify_code()
     # verify_code = "000000"
-    rpl_true = f'正在绑定您的第{bind_count + 1}个记录，请将您的 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{verify_code}\n稍等片刻等待同步后，发送\n验证 您的玩家ID 来完成本次身份验证\n例如：验证 10000xxxx 国服'
+    rpl_true = f'正在绑定第{bind_count + 1}个记录，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{verify_code}\n稍等片刻等待同步后，发送\n验证 玩家ID 来完成本次身份验证\n例如：验证 10000xxxx 国服'
     # 存入verify_code
     cursor.execute("UPDATE users SET verify_code = ? WHERE user_id = ? AND platform = ?", (verify_code, user_id, platform))
     db_manager.conn.commit()
     return text_response(rpl_true)
 
 
 def unbind_player_request(platform: str, user_id: str):
 
      data = get_user_data(platform, user_id)
      record = json.loads(data['data']['game_ids'])
      if not record:
-         return text_response('你还没有绑定哦，是要解绑个吉他吗（？')
+         return text_response('未找到绑定记录')
 
-     return text_response(f'您当前有 {len(record)} 个记录，发送"解除绑定 {len(record)}"来获解除您的第{len(record)}个记录，以此类推。')
+     return text_response(f'当前有 {len(record)} 个记录，发送"解除绑定 {len(record)}"来获解除第{len(record)}个记录，以此类推')
 
 
 def bind_player_verification(platform: str, user_id: str, server: int | None, player_id: str, bind_type: bool):
 
     cursor = db_manager.conn.cursor()
     # 先检查verify_code是否正确
     # 使用 get
     user_data = get_user_data(platform, user_id)
     verify_code = user_data['data']['verify_code']
 
     if server is None:
         print('server is None')
         server = user_data['data']['server_mode']
     if verify_code == "" or not verify_code:
-        return text_response('请先获取验证代码。')
+        return text_response('请先获取验证代码')
     # 检测重复性
     game_ids = json.loads(user_data['data']['game_ids'])
     print(game_ids)
     print(type(game_ids))
     for i in game_ids:
         if i.get("game_id") == player_id and i.get("server") == server:
-            return text_response('您已经绑定过这个玩家了。')
+            return text_response('请勿重复绑定')
     server_s_name = config.server_index_to_s_name[str(server)]
     print(server_s_name)
     url = f'https://bestdori.com/api/player/{server_s_name}/{player_id}?mode=2'
     print(url)
     response = requests.get(url)
     data = response.json()
     if data.get("data").get("profile") is None or data.get("profile") == {}:
-        return text_response('玩家ID不存在，请检查您的输入是否正确，或服务器是否对应。')
+        return text_response('玩家ID不存在，请检查输入，或服务器是否对应')
     introduction = data.get("data", {}).get("profile", {}).get("introduction")
     deck_name = data.get("data", {}).get("profile", {}).get("mainUserDeck", {}).get("deckName")
     print(verify_code, introduction, deck_name)
     if verify_code != introduction and verify_code != deck_name:
-        return text_response('验证失败，您的签名或者乐队编队名称与您的验证代码不匹配喵，可以整顿后再次尝试(无需重复发送绑定玩家)。')
+        return text_response('验证失败，签名或者乐队编队名称与验证代码不匹配喵，可以检查后再次尝试(无需重复发送绑定玩家)')
     # 验证成功
     print(data['data'])
     game_ids = json.loads(user_data['data']['game_ids'])
     game_ids.append({"game_id": player_id, "server": server})
     cursor.execute("UPDATE users SET game_ids = ? WHERE user_id = ? AND platform = ?",
                    (json.dumps(game_ids), user_id, platform))  # 存入game_ids
     cursor.execute("UPDATE users SET verify_code = ? WHERE user_id = ? AND platform = ?",
                    ("", user_id, platform))  # 清空verify_code
     db_manager.conn.commit()
-    return text_response('绑定成功！现在可以使用"玩家状态"来查询玩家信息了～')
+    return text_response('绑定成功！现在可以使用"玩家状态"来查询玩家信息了')
 
 
 def unbind_player_verification(platform: str, user_id: str, record: int | None):
     user_data = get_user_data(platform, user_id)
 
     cursor = db_manager.conn.cursor()
 
@@ -456,16 +454,16 @@
             # 将更新后的game_ids列表转换回JSON字符串
             updated_game_ids_json = json.dumps(game_ids)
 
             # 更新数据库中的game_ids字段
             cursor.execute("UPDATE users SET game_ids = ? WHERE user_id = ? AND platform = ?", (updated_game_ids_json, user_id, platform))
             db_manager.conn.commit()
             return text_response('解绑成功喵')
-        return text_response(f'解绑失败，您当前有 {record} 个记录，发送"解除绑定 {record}"来获解除您的第{record}个记录，以此类推。')
-    return text_response('解绑失败，请检查您的输入是否正确。')
+        return text_response(f'解绑失败，当前有 {record} 个记录，发送"解除绑定 {record}"来获解除第{record}个记录，以此类推')
+    return text_response('解绑失败，请检查输入是否正确')
 
 
 class Remote:
     @staticmethod
     def get_user_data(platform: str, user_id: str):
         data = {
             'platform': platform,
```

### Comparing `tsugu-0.2.2/tsugu.egg-info/PKG-INFO` & `tsugu-0.3.0/tsugu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.2.2
+Version: 0.3.0
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.2.2 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.0 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

