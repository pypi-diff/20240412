# Comparing `tmp/pyrubino-1.0.0.tar.gz` & `tmp/pyrubino-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubino-1.0.0.tar", last modified: Thu Apr 11 20:49:44 2024, max compression
+gzip compressed data, was "pyrubino-1.1.0.tar", last modified: Thu Apr 11 20:54:37 2024, max compression
```

## Comparing `pyrubino-1.0.0.tar` & `pyrubino-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-11 20:49:44.185666 pyrubino-1.0.0/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-11 20:41:50.000000 pyrubino-1.0.0/LICENCE
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-11 20:49:44.185666 pyrubino-1.0.0/PKG-INFO
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-11 20:41:30.000000 pyrubino-1.0.0/README.md
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-11 20:49:44.185666 pyrubino-1.0.0/pyrubino/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       22 2024-04-11 20:29:28.000000 pyrubino-1.0.0/pyrubino/ __init__.py
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     2479 2024-04-11 20:28:40.000000 pyrubino-1.0.0/pyrubino/rubino.py
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-11 20:49:44.185666 pyrubino-1.0.0/pyrubino.egg-info/
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-11 20:49:44.000000 pyrubino-1.0.0/pyrubino.egg-info/PKG-INFO
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      195 2024-04-11 20:49:44.000000 pyrubino-1.0.0/pyrubino.egg-info/SOURCES.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-04-11 20:49:44.000000 pyrubino-1.0.0/pyrubino.egg-info/dependency_links.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        9 2024-04-11 20:49:44.000000 pyrubino-1.0.0/pyrubino.egg-info/top_level.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-04-11 20:49:44.185666 pyrubino-1.0.0/setup.cfg
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      562 2024-04-11 20:49:18.000000 pyrubino-1.0.0/setup.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-11 20:54:37.437857 pyrubino-1.1.0/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-11 20:41:50.000000 pyrubino-1.1.0/LICENCE
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-11 20:54:37.437857 pyrubino-1.1.0/PKG-INFO
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-11 20:41:30.000000 pyrubino-1.1.0/README.md
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-11 20:54:37.436858 pyrubino-1.1.0/pyrubino/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       22 2024-04-11 20:29:28.000000 pyrubino-1.1.0/pyrubino/ __init__.py
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     2481 2024-04-11 20:53:16.000000 pyrubino-1.1.0/pyrubino/rubino.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-11 20:54:37.437857 pyrubino-1.1.0/pyrubino.egg-info/
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-11 20:54:37.000000 pyrubino-1.1.0/pyrubino.egg-info/PKG-INFO
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      195 2024-04-11 20:54:37.000000 pyrubino-1.1.0/pyrubino.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-04-11 20:54:37.000000 pyrubino-1.1.0/pyrubino.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        9 2024-04-11 20:54:37.000000 pyrubino-1.1.0/pyrubino.egg-info/top_level.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-04-11 20:54:37.437857 pyrubino-1.1.0/setup.cfg
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      562 2024-04-11 20:54:11.000000 pyrubino-1.1.0/setup.py
```

### Comparing `pyrubino-1.0.0/LICENCE` & `pyrubino-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pyrubino-1.0.0/PKG-INFO` & `pyrubino-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubino
-Version: 1.0.0
+Version: 1.1.0
 Summary: Luis Rubika libry
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrubino-1.0.0/pyrubino/rubino.py` & `pyrubino-1.1.0/pyrubino/rubino.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 	def addLike(self,post_id,id,my):
 		input = {"action_type":"Like","post_id":post_id,"post_profile_id":id,"profile_id":my}
 		return self.req(input,'likePostAction')
 	def addViv(self,post_id,id):
 		input = {"post_id":post_id,"post_profile_id":id}
 		return self.req(input,"addPostViewCount")
 	def isExistUsername(self,name:str):
-		input = {"username": user}
+		input = {"username": name}
 		return self.req(input,"isExistUsername")
 	def createPage(self,name:str,bio,user):
 		input = {"bio": bio,"name": name,"username": user}
-		return self.req(input,createPage)
+		return self.req(input,'createPage')
 	def getPost(self,id):
 		input = {"limit":10,"sort":"FromMax","target_profile_id":id}
 		return self.req(input,"getProfilePosts")
```

### Comparing `pyrubino-1.0.0/pyrubino.egg-info/PKG-INFO` & `pyrubino-1.1.0/pyrubino.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubino
-Version: 1.0.0
+Version: 1.1.0
 Summary: Luis Rubika libry
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrubino-1.0.0/setup.py` & `pyrubino-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='pyrubino',
-    version="1.0.0",
+    version="1.1.0",
     packages= ['pyrubino'],
     url='https://guides.github.com/features/mastering-markdown/',
     license='MIT',
     author='Luis',
     author_email='mm12mok18@gmail.com',
     description='Luis Rubika libry',
     long_description= open("README.md",'r').read(),
```

