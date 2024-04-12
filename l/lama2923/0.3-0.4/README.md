# Comparing `tmp/lama2923-0.3.tar.gz` & `tmp/lama2923-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-0.3.tar", last modified: Fri Apr 12 00:57:22 2024, max compression
+gzip compressed data, was "lama2923-0.4.tar", last modified: Fri Apr 12 02:42:08 2024, max compression
```

## Comparing `lama2923-0.3.tar` & `lama2923-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 00:57:22.950246 lama2923-0.3/
--rw-rw-rw-   0        0        0      108 2024-04-12 00:57:22.948248 lama2923-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 00:57:22.848607 lama2923-0.3/lama2923/
--rw-rw-rw-   0        0        0    18561 2024-04-12 00:55:42.000000 lama2923-0.3/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:57:22.945245 lama2923-0.3/lama2923.egg-info/
--rw-rw-rw-   0        0        0      108 2024-04-12 00:57:22.000000 lama2923-0.3/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-04-12 00:57:22.000000 lama2923-0.3/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 00:57:22.000000 lama2923-0.3/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-12 00:57:22.000000 lama2923-0.3/lama2923.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 00:57:22.000000 lama2923-0.3/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 00:57:22.000000 lama2923-0.3/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 00:57:22.951247 lama2923-0.3/setup.cfg
--rw-rw-rw-   0        0        0      388 2024-04-12 00:57:02.000000 lama2923-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 02:42:08.826414 lama2923-0.4/
+-rw-rw-rw-   0        0        0      693 2024-04-12 02:42:08.820856 lama2923-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 02:42:08.762659 lama2923-0.4/lama2923/
+-rw-rw-rw-   0        0        0    20579 2024-04-12 02:29:09.000000 lama2923-0.4/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 02:42:08.804571 lama2923-0.4/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      693 2024-04-12 02:42:08.000000 lama2923-0.4/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-04-12 02:42:08.000000 lama2923-0.4/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 02:42:08.000000 lama2923-0.4/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-12 02:42:08.000000 lama2923-0.4/lama2923.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 02:42:08.000000 lama2923-0.4/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 02:42:08.000000 lama2923-0.4/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 02:42:08.826414 lama2923-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2024-04-12 02:41:36.000000 lama2923-0.4/setup.py
```

### Comparing `lama2923-0.3/lama2923/__init__.py` & `lama2923-0.4/lama2923/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -434,17 +434,59 @@
             
             if r.status_code == 200:
                 messages = r.json()
                 return messages
             else:
                 return r.status_code
             
+        def get_specific_message(self, Channel_id, Message_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return response.json()
+            else:
+                return response.status_code
+
+
+        def add_reaction(self, Channel_id, Message_id, emoji):
+            headers = {'Authorization': str(self.token)}
+            # Discord requires emojis to be URL encoded
+            emoji = requests.utils.quote(emoji)
+            url = f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}/reactions/{emoji}/@me'
+            response = requests.put(url, headers=headers)
+            return response.status_code
+
+
+        def get_channel_info(self, Channel_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/channels/{Channel_id}'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return response.json()
+            else:
+                return response.status_code
     
-    
-    
+        def list_guild_channels(self, Guild_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/guilds/{Guild_id}/channels'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return response.json()
+            else:
+                return response.status_code   
+
+        def send_tts_message(self, Channel_id, Message):
+            payload = {'content': str(Message), 'tts': True}
+            headers = {'Authorization': str(self.token)}
+            response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
+            return response.status_code
+        
+        
+
     
     class Webhook:
         def __init__(self, webhook_url):
             self.WebhookUrl = str(webhook_url)
             
         def send_webhook(self, Content='', embed=None, files=None):
             def format_embed(embed):
```

