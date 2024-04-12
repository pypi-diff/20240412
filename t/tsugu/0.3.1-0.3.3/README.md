# Comparing `tmp/tsugu-0.3.1.tar.gz` & `tmp/tsugu-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.3.1.tar", last modified: Fri Apr 12 06:06:13 2024, max compression
+gzip compressed data, was "tsugu-0.3.3.tar", last modified: Fri Apr 12 06:34:49 2024, max compression
```

## Comparing `tsugu-0.3.1.tar` & `tsugu-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:13.058664 tsugu-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 06:06:04.000000 tsugu-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 06:06:13.058664 tsugu-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-12 06:06:04.000000 tsugu-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:06:13.058664 tsugu-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 06:06:04.000000 tsugu-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:13.058664 tsugu-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-12 06:06:04.000000 tsugu-0.3.1/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:13.058664 tsugu-0.3.1/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19678 2024-04-12 06:06:04.000000 tsugu-0.3.1/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:13.058664 tsugu-0.3.1/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 06:06:12.000000 tsugu-0.3.1/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 06:06:13.000000 tsugu-0.3.1/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:06:12.000000 tsugu-0.3.1/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 06:06:12.000000 tsugu-0.3.1/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 06:06:12.000000 tsugu-0.3.1/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:34:49.804387 tsugu-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 06:34:40.000000 tsugu-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 06:34:49.804387 tsugu-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-12 06:34:40.000000 tsugu-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:34:49.804387 tsugu-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 06:34:40.000000 tsugu-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:34:49.804387 tsugu-0.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-12 06:34:40.000000 tsugu-0.3.3/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:34:49.804387 tsugu-0.3.3/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 06:34:40.000000 tsugu-0.3.3/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-12 06:34:40.000000 tsugu-0.3.3/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-12 06:34:40.000000 tsugu-0.3.3/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-12 06:34:40.000000 tsugu-0.3.3/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18493 2024-04-12 06:34:40.000000 tsugu-0.3.3/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:34:49.804387 tsugu-0.3.3/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 06:34:49.000000 tsugu-0.3.3/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 06:34:49.000000 tsugu-0.3.3/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:34:49.000000 tsugu-0.3.3/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 06:34:49.000000 tsugu-0.3.3/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 06:34:49.000000 tsugu-0.3.3/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.3.1/LICENSE` & `tsugu-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.1/PKG-INFO` & `tsugu-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.3.1
+Version: 0.3.3
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.3.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.3 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.3.1/README.md` & `tsugu-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.1/setup.py` & `tsugu-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.3.1',
+    version='0.3.3',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.3.1/test/test_main.py` & `tsugu-0.3.3/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.1/tsugu/bot.py` & `tsugu-0.3.3/tsugu/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,21 @@
 
     if message.startswith('绑定玩家') and len(message.replace('绑定玩家', '').strip()) < 4:
         # 如果匹配 绑定玩家 则绑定默认服务器的玩家 如果用户输入了服务器名 则绑定对应服务器的玩家，如果服务器名无效则 赋值为 None
         return bind_player_request(platform, user_id)
 
     if message.startswith('验证'):
         arg = message.replace('验证', '').strip()
-        # if len(arg_list) < 1:  # 如果长度小于2
-        #     return text_response('请输入正确')
-        # if not arg_list[0].isdigit():  # 如果第一个不是数字
-        #     return text_response('请确保输入正确(例如: 验证 123456 cn)')
-        # server = query_server_info(arg_list[-1])
-        # player_id = arg_list[0]
         # 正则出数字
         player_ids = re.findall(r'\d+', arg)
         if not player_ids or len(player_ids) > 1:
             return text_response('请确保输入正确(例如: 验证 10000xxxxx cn)')
         player_id = player_ids[0]
         server = query_server_info(arg.replace(player_id, ''))  # 后续自动处理 None
-        print(server, type(server))
+        # print(server, type(server))
         return bind_player_verification(platform, user_id, server, player_id, True)
 
     if message.startswith('解除绑定'):
         if message[4:].strip() == '':
             return unbind_player_request(platform, user_id)
         msg_list = message.split(' ')
         if len(msg_list) < 2:
@@ -101,25 +95,24 @@
         # 如果匹配 绑定玩家 则绑定默认服务器的玩家 如果用户输入了服务器名 则绑定对应服务器的玩家，如果服务器名无效则 赋值为 None
         server = Remote.get_user_data(platform, user_id)['data']['server_mode'] if message[4:].strip() == '' else (r_ if server_exists(r_ := query_server_info(message[4:])) else None)
         if not server_exists(server):
             return text_response(f'未找到名为 {message[4:]} 的服务器信息，请确保输入是服务器名而不是玩家ID，通常情况发送"绑定玩家"或"绑定玩家 服务器"即可')
 
         res = Remote.bind_player_request(platform, user_id, server, True)
         if res.get('status') != 'success':
-            print(res)
+            # print(res)
             # {'status': 'success', 'data': {'verifyCode': 12492}}
             return text_response(res.get('data'))
         # if not res.get('status') == 'failed':
         #     return text_response('未知错误喵')
         return text_response(f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{res.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证 + 空格 + 玩家ID 来完成本次身份验证\n验证 10000xxxx 国服''')
 
     if message.startswith('解除绑定'):
         server = Remote.get_user_data(platform, user_id)['data']['server_mode'] if message[4:].strip() == '' else (r_ if (config.server_list(r_ := query_server_info(message[4:]))) else None)
         if server_exists(server) is False:
-            # print(server)
             return text_response(f'未找到名为 {message[4:].strip()} 的服务器信息，请确保输入的是服务器名而不是玩家ID，通常情况发送"解除绑定"即可')
         response = Remote.bind_player_request(platform, user_id, server, False)  # 获取响应
         if response.get('status') == 'failed':  # 检查状态
             return text_response(response.get('data'))
         # 如果是200
         return text_response(f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{response.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {server}\n来完成本次身份验证(没错只需要加上 {server} 来确定需要解绑的服务器)''')
```

### Comparing `tsugu-0.3.1/tsugu/config.py` & `tsugu-0.3.3/tsugu/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,23 +214,23 @@
         return self.__doc__
 
     def output_config_json(self, path="./config.json"):
         config_pre_json = {
             "backend": "http://tsugubot.com:8080",
             "user_data_backend": "http://tsugubot.com:8080",
             "user_database_path": None,
-            "use_proxies": True,
+            "use_proxies": False,
             "proxies": {
                 "http": "http://localhost:7890",
                 "https": "http://localhost:7890",
             },
             "token_name": "Tsugu",
             "bandori_station_token": "ZtV4EX2K9Onb",
-            "use_easy_bg": False,
-            "compress": False,
+            "use_easy_bg": True,
+            "compress": True,
             "ban_gacha_simulate_group_data": [],
             "server_list": {
                 "0": "日服",
                 "1": "国际服",
                 "2": "台服",
                 "3": "国服",
                 "4": "韩服",
```

### Comparing `tsugu-0.3.1/tsugu/router.py` & `tsugu-0.3.3/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.1/tsugu/utils.py` & `tsugu-0.3.3/tsugu/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     data = {
         "default_servers": default_servers,
         "server": server,
         "text": text,
         "useEasyBG": config.use_easy_bg,
         "compress": config.compress
     }
-    print(data)
+    # print(data)
     res = requests_post(f"{config.backend}{path}", data)
     return res
 
 
 def v2_api_command(message, command_matched, api, platform, user_id, channel_id):
     text = message[len(command_matched):].strip()
 
@@ -126,52 +126,22 @@
 
     if api == 'gachaSimulate':
         if channel_id in config.ban_gacha_simulate_group_data:
             return text_response('此群禁止使用模拟抽卡功能')
 
     # 获取用户数据
     user_data = get_user_data(platform, user_id) if config.user_database_path else Remote.get_user_data(platform, user_id)
-    print(user_data)
+    # print(user_data)
     try:
         if user_data['status'] != 'success':
             return text_response('获取用户数据失败')
         return v2api_from_backend(api, text, user_data['data']['default_server'], user_data['data']['server_mode'])
     except Exception as e:
         return text_response('前端错误: ' + str(e))
 
-def set_car_forward(platform, user_id, status):
-    data = {
-        'platform': platform,
-        'user_id': user_id,
-        'status': status
-    }
-    result = requests_post(f"{config.user_data_backend}/user/changeUserData/setCarForwarding", data)
-    return result
-
-
-def set_default_server(platform, user_id, text):
-    data = {
-        'platform': platform,
-        'user_id': user_id,
-        'text': text
-    }
-    result = requests_post(f"{config.user_data_backend}/user/changeUserData/setDefaultServer", data)
-    return result
-
-
-def set_server_mode(platform, user_id, text):
-    data = {
-        'platform': platform,
-        'user_id': user_id,
-        'text': text
-    }
-    result = requests_post(f"{config.user_data_backend}/user/changeUserData/setServerMode", data)
-    return result
-
-
 def submit_car_number_msg(message, user_id, platform):
     # 检查car_config['car']中的关键字
     for keyword in config.car_config["car"]:
         if str(keyword) in message:
             break
     else:
         return False
@@ -257,36 +227,32 @@
         "data": data
     }
     return result
 
 
 def player_status(user_id, platform, args: str | int | None = None):
     user_data = get_user_data(platform, user_id)
-    print(user_data)
     game_ids = user_data['data']['game_ids']
     if game_ids == "[]" or not game_ids:
         return text_response(f'未绑定玩家，请发送 绑定玩家 进行绑定')
     game_ids = json.loads(game_ids)
     text = ''
-    print(args)
     if args is None:
         # 先查找默认服务器对应的记录
         server: int = user_data['data']['server_mode']
         for i in game_ids:
             if i.get("server") == server:
                 player_id = str(i.get("game_id"))
                 server = int(i.get("server"))
 
                 text = f'已查找默认服务器 {config.server_index_to_name[str(server)]} 的记录'
-                # print(player_id, server)
                 break
         else:
             # 再查找第一个记录
             if game_ids:
-                # print(player_id, server)
                 return text_response(f'未在 {len(game_ids)} 条记录中找到 {config.server_index_to_name[str(server)]} 的记录')
             else:
                 pass  # 前面已经判断过了没绑定任何的情况
     elif isinstance(args, int):
         # 查找对应数字的记录
         if args == 0:
             return text_response('哪来的0（')
@@ -327,15 +293,14 @@
     db_manager.conn.commit()
     return text_response('车牌转发设置成功')
 
 
 def set_default_server(platform, user_id, text):
 
     default_server = convert_server_names_to_indices(text)
-    # print(default_server)
     get_user_data(platform, user_id)
     cursor = db_manager.conn.cursor()
     cursor.execute("UPDATE users SET default_server = ? WHERE user_id = ? AND platform = ?",
                    (json.dumps(default_server), user_id, platform))
     db_manager.conn.commit()
     return text_response(f'默认服务器设置为 {text}')
 
@@ -391,40 +356,33 @@
     cursor = db_manager.conn.cursor()
     # 先检查verify_code是否正确
     # 使用 get
     user_data = get_user_data(platform, user_id)
     verify_code = user_data['data']['verify_code']
 
     if server is None:
-        print('server is None')
         server = user_data['data']['server_mode']
     if verify_code == "" or not verify_code:
         return text_response('请先获取验证代码')
     # 检测重复性
     game_ids = json.loads(user_data['data']['game_ids'])
-    print(game_ids)
-    print(type(game_ids))
     for i in game_ids:
         if i.get("game_id") == player_id and i.get("server") == server:
             return text_response('请勿重复绑定')
     server_s_name = config.server_index_to_s_name[str(server)]
-    print(server_s_name)
     url = f'https://bestdori.com/api/player/{server_s_name}/{player_id}?mode=2'
-    print(url)
     response = requests.get(url)
     data = response.json()
     if data.get("data").get("profile") is None or data.get("profile") == {}:
         return text_response('玩家ID不存在，请检查输入，或服务器是否对应')
     introduction = data.get("data", {}).get("profile", {}).get("introduction")
     deck_name = data.get("data", {}).get("profile", {}).get("mainUserDeck", {}).get("deckName")
-    print(verify_code, introduction, deck_name)
     if verify_code != introduction and verify_code != deck_name:
         return text_response('验证失败，签名或者乐队编队名称与验证代码不匹配喵，可以检查后再次尝试(无需重复发送绑定玩家)')
     # 验证成功
-    print(data['data'])
     game_ids = json.loads(user_data['data']['game_ids'])
     game_ids.append({"game_id": player_id, "server": server})
     cursor.execute("UPDATE users SET game_ids = ? WHERE user_id = ? AND platform = ?",
                    (json.dumps(game_ids), user_id, platform))  # 存入game_ids
     cursor.execute("UPDATE users SET verify_code = ? WHERE user_id = ? AND platform = ?",
                    ("", user_id, platform))  # 清空verify_code
     db_manager.conn.commit()
@@ -496,18 +454,16 @@
         return result
 
     @staticmethod
     def player_status(user_id, platform, server=None):
         user_data = Remote.get_user_data(platform, user_id)
         if user_data['status'] != 'success':
             return text_response('获取用户数据失败')
-        print(user_data)
         if server is None:
             server = user_data['data']['server_mode']
-        print(server)
         player_id = user_data['data']['server_list'][server]['playerId']
         if player_id == 0:
             return text_response(f'未绑定玩家，请使用 绑定玩家 进行绑定')
         return v2api_from_backend('player', str(player_id), server=server)
 
     @staticmethod
     def set_car_forward(platform, user_id, status):
```

### Comparing `tsugu-0.3.1/tsugu.egg-info/PKG-INFO` & `tsugu-0.3.3/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.3.1
+Version: 0.3.3
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.3.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.3 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

