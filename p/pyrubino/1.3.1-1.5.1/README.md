# Comparing `tmp/pyrubino-1.3.1.tar.gz` & `tmp/pyrubino-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubino-1.3.1.tar", last modified: Fri Apr 12 07:51:44 2024, max compression
+gzip compressed data, was "pyrubino-1.5.1.tar", last modified: Fri Apr 12 08:31:55 2024, max compression
```

## Comparing `pyrubino-1.3.1.tar` & `pyrubino-1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 07:51:44.617667 pyrubino-1.3.1/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-11 20:41:50.000000 pyrubino-1.3.1/LICENCE
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-12 07:51:44.617667 pyrubino-1.3.1/PKG-INFO
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-11 20:41:30.000000 pyrubino-1.3.1/README.md
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 07:51:44.616666 pyrubino-1.3.1/pyrubino/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       22 2024-04-11 20:29:28.000000 pyrubino-1.3.1/pyrubino/ __init__.py
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     2481 2024-04-12 07:51:13.000000 pyrubino-1.3.1/pyrubino/rubino.py
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 07:51:44.616666 pyrubino-1.3.1/pyrubino.egg-info/
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-12 07:51:44.000000 pyrubino-1.3.1/pyrubino.egg-info/PKG-INFO
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      195 2024-04-12 07:51:44.000000 pyrubino-1.3.1/pyrubino.egg-info/SOURCES.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-04-12 07:51:44.000000 pyrubino-1.3.1/pyrubino.egg-info/dependency_links.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        9 2024-04-12 07:51:44.000000 pyrubino-1.3.1/pyrubino.egg-info/top_level.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-04-12 07:51:44.617667 pyrubino-1.3.1/setup.cfg
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      562 2024-04-12 07:50:33.000000 pyrubino-1.3.1/setup.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 08:31:55.880289 pyrubino-1.5.1/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-11 20:41:50.000000 pyrubino-1.5.1/LICENCE
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-12 08:31:55.880289 pyrubino-1.5.1/PKG-INFO
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-11 20:41:30.000000 pyrubino-1.5.1/README.md
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 08:31:55.879289 pyrubino-1.5.1/pyrubino/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       29 2024-04-12 08:28:08.000000 pyrubino-1.5.1/pyrubino/ __init__.py
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)     2980 2024-04-12 08:28:29.000000 pyrubino-1.5.1/pyrubino/rubino.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 08:31:55.880289 pyrubino-1.5.1/pyrubino.egg-info/
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-12 08:31:55.000000 pyrubino-1.5.1/pyrubino.egg-info/PKG-INFO
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      195 2024-04-12 08:31:55.000000 pyrubino-1.5.1/pyrubino.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-04-12 08:31:55.000000 pyrubino-1.5.1/pyrubino.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        9 2024-04-12 08:31:55.000000 pyrubino-1.5.1/pyrubino.egg-info/top_level.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-04-12 08:31:55.880289 pyrubino-1.5.1/setup.cfg
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      562 2024-04-12 08:30:46.000000 pyrubino-1.5.1/setup.py
```

### Comparing `pyrubino-1.3.1/LICENCE` & `pyrubino-1.5.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pyrubino-1.3.1/PKG-INFO` & `pyrubino-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubino
-Version: 1.3.1
+Version: 1.5.1
 Summary: Luis Rubika libry
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrubino-1.3.1/pyrubino/rubino.py` & `pyrubino-1.5.1/pyrubino/rubino.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 from json import loads
 from random import randint, choice
 class Luis:
 	def __init__(self,auth:str='Luis'):
 		self.auth = auth
 	def req(self,input,name):
 		return loads(post(url="https://rubino5.iranlms.ir/",json={"api_version":"0","auth":self.auth,"client":{"app_name":"Main","app_version":"3.6.4","lang_code":"fa","package":"app.rbmain.a","platform":"Android"},"data":input,"method":name}).text)
-	def uploadFile(self,file:str):
+	def uploadFile(self,file:str,id):
 		with open(file) as f:
 			size = f.seek(0, 2)
-		id = self.getId()['data']['profiles'][0]["id"]
 		input = {"file_name":"m.jpg","file_size":size,"file_type":"Picture","profile_id":id}
 		p = self.req(input,'requestUploadFile')
 		url = p["data"]['server_url']
 		hash = p['data']['hash_file_request']
 		file_id = p['data']['file_id']
 		byte_file = open(file, 'rb').read()
 		headers = {"auth":self.auth,"file-id":file_id,"chunk-size":str(len(byte_file)),"total-part":"1","part-number":"1","hash-file-request":hash}
 		m = loads(post(url=url,headers=headers,data=byte_file).text)
 		hash_rec = m['data']['hash_file_receive']
 		return {"auth":self.auth,"id":file_id,"data":id,"hash_file_receive":hash_rec}
-	def addPost(self,file:str):
-		p = self.uploadFile(file)
+	def addPost(self,file:str,id):
+		p = self.uploadFile(file,id)
 		rnd = randint(100000, 999999999)
 		input = {"caption":"Luis","file_id":p['id'],"hash_file_receive":p['hash_file_receive'],"height":800,"profile_id":p['data'],"post_type":"Picture","rnd":rnd,"tagged_profiles":[],"thumbnail_file_id":p['id'],"thumbnail_hash_file_receive":p["hash_file_receive"],"width":800}
 		name = "addPost"
 		return self.req(input,name)
 	def getId(self):
 		return self.req({"equal":False,"limit":10,"sort": "FromMax"},"getProfileList")
-	def addText(self,post_id,id,my):
-		input = {"content":"Luis","post_id":post_id,"post_profile_id":id,"profile_id":my}
+	def addText(self,post_id,id,my,text):
+		input = {"content":text,"post_id":post_id,"post_profile_id":id,"profile_id":my}
 		return self.req(input,"addComment")
 	def addLike(self,post_id,id,my):
 		input = {"action_type":"Like","post_id":post_id,"post_profile_id":id,"profile_id":my}
 		return self.req(input,'likePostAction')
 	def addViv(self,post_id,id):
 		input = {"post_id":post_id,"post_profile_id":id}
 		return self.req(input,"addPostViewCount")
@@ -42,8 +41,17 @@
 		return self.req(input,"isExistUsername")
 	def createPage(self,name:str,bio,user):
 		input = {"bio": bio,"name": name,"username": user}
 		return self.req(input,'createPage')
 	def getPost(self,id):
 		input = {"limit":10,"sort":"FromMax","target_profile_id":id}
 		return self.req(input,"getProfilePosts")
+	def addStory(self,file,id):
+		p = self.uploadFile(file,id)
+		rnd = randint(100000, 999999999)
+		input = {"duration":0,"file_id":p['id'],"hash_file_receive":p['hash_file_receive'],"height":1280,"profile_id":id,"rnd":rnd,"story_type":"Picture","thumbnail_file_id":p['id'],"thumbnail_hash_file_receive":p['hash_file_receive'],"width":720}
+		return self.req(input,"addStory")
+	def addViewStory(self,idst,idto,id):
+		name = "addViewStory"
+		input = {"profile_id":id,"story_ids":[idst],"story_profile_id":idto}
+		return self.req(input,name)
```

### Comparing `pyrubino-1.3.1/pyrubino.egg-info/PKG-INFO` & `pyrubino-1.5.1/pyrubino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubino
-Version: 1.3.1
+Version: 1.5.1
 Summary: Luis Rubika libry
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrubino-1.3.1/setup.py` & `pyrubino-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='pyrubino',
-    version="1.3.1",
+    version="1.5.1",
     packages= ['pyrubino'],
     url='https://guides.github.com/features/mastering-markdown/',
     license='MIT',
     author='Luis',
     author_email='mm12mok18@gmail.com',
     description='Luis Rubika libry',
     long_description= open("README.md",'r').read(),
```

