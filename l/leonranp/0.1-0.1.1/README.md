# Comparing `tmp/leonranp-0.1.tar.gz` & `tmp/leonranp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leonranp-0.1.tar", last modified: Wed Mar 27 14:04:22 2024, max compression
+gzip compressed data, was "leonranp-0.1.1.tar", last modified: Fri Apr 12 13:17:03 2024, max compression
```

## Comparing `leonranp-0.1.tar` & `leonranp-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 14:04:22.070525 leonranp-0.1/
--rw-rw-rw-   0        0        0     1093 2024-03-09 04:33:19.000000 leonranp-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      887 2024-03-27 14:04:22.069527 leonranp-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-03-11 10:54:48.000000 leonranp-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 14:04:22.055531 leonranp-0.1/leonranp/
--rw-rw-rw-   0        0        0     5858 2024-03-27 14:03:44.000000 leonranp-0.1/leonranp/__init__.py
--rw-rw-rw-   0        0        0       78 2024-03-27 14:01:26.000000 leonranp-0.1/leonranp/test.py
-drwxrwxrwx   0        0        0        0 2024-03-27 14:04:22.069527 leonranp-0.1/leonranp.egg-info/
--rw-rw-rw-   0        0        0      887 2024-03-27 14:04:21.000000 leonranp-0.1/leonranp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-03-27 14:04:21.000000 leonranp-0.1/leonranp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 14:04:21.000000 leonranp-0.1/leonranp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-27 14:04:21.000000 leonranp-0.1/leonranp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 14:04:22.070525 leonranp-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1108 2024-03-27 14:04:20.000000 leonranp-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:17:03.346235 leonranp-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2024-03-09 04:33:19.000000 leonranp-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      889 2024-04-12 13:17:03.345235 leonranp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-03-11 10:54:48.000000 leonranp-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 13:17:03.335228 leonranp-0.1.1/leonranp/
+-rw-rw-rw-   0        0        0     1067 2024-04-12 12:32:27.000000 leonranp-0.1.1/leonranp/InfoWindow.py
+-rw-rw-rw-   0        0        0     6193 2024-04-12 13:12:02.000000 leonranp-0.1.1/leonranp/__init__.py
+-rw-rw-rw-   0        0        0       35 2024-04-12 12:46:20.000000 leonranp-0.1.1/leonranp/test.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:17:03.345235 leonranp-0.1.1/leonranp.egg-info/
+-rw-rw-rw-   0        0        0      889 2024-04-12 13:17:03.000000 leonranp-0.1.1/leonranp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-04-12 13:17:03.000000 leonranp-0.1.1/leonranp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:17:03.000000 leonranp-0.1.1/leonranp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 13:17:03.000000 leonranp-0.1.1/leonranp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:17:03.346235 leonranp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2024-04-12 13:16:52.000000 leonranp-0.1.1/setup.py
```

### Comparing `leonranp-0.1/LICENSE.txt` & `leonranp-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `leonranp-0.1/PKG-INFO` & `leonranp-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leonranp
-Version: 0.1
+Version: 0.1.1
 Summary: This is Leon Random Plus,that add more functions to the random!
 Home-page: https://github.com/Leonmmcoset/leonranp
 Author: LeonMMcoset
 Author-email: leonmmcoset@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leonranp-0.1/leonranp/__init__.py` & `leonranp-0.1.1/leonranp/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,23 @@
 #Code by LeonMMcoset
 '''
 This is Leon Random Plus,that add more functions to the random!
 To use it,code "import leonranp"
 
 Copyright LeonMMcoset.All rights reserved.
 
-Star my github project!
+Star my Github project!
 I will update more and more!
+Github project:https://github.com/Leonmmcoset/
 '''
-#Code Running Info Start
-print('-------------Leon Random Plus-------------')
-print('You are using Leon Random Plus')
-print('PyPI:https://pypi.org/project/leonranp/')
-print('Wiki:http://leonmmcoset.jjmm.ink:8002/doku.php?id=leonranp')
-print('Github:https://github.com/Leonmmcoset/leonranp/')
-print('To upgrade,use "upgrade()" on your shell')
-print('To have help,use "lrphelp()"')
-print('To delete Leon Random Plus,use "dellrp()"')
-print('------------------------------------------')
+class RandomError(Exception):
+    def __init__(self,text):
+        self.text = text
+    def __str__(self):
+        return self.text
 #Code Running Info End
 from random import *
 from os import *
 #Start Code#
 #randstr:just code "randstr()".
 def randstr():
     randstrlist = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
@@ -32,14 +28,16 @@
 #The randcode() values can be assigned in variables.
 #To print randcode,code "print(randcode())"
 def rcrandstr():
     rcrandstrlist = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
     rcrandstr = choice(rcrandstrlist)
     return rcrandstr
 def randcode(digits):
+    if digits == 0:
+        raise RandomError("Digits can't be 0!")
     randcode = ''
     for i in range(digits):
         if randint(0,1)==0:
             randcode = randcode + str(randint(0,9))
         else:
             randcode = randcode + str(rcrandstr())
     return randcode
@@ -58,25 +56,31 @@
         rsbool = 1
     else:
         rsbool = 0
     return bool(rsbool)
 #randlistint/str/code:Random list int or str.
 #To print it,"print(randlistint/str/code())"
 def randlistint(list,intfirst,intlast):
+    if list == 0:
+        raise RandomError("list can't be 0!")
     rlint = []
     for rli in range(list):
         rlint.append(randint(intfirst,intlast))
     return rlint
 def randliststr(list):
+    if list == 0:
+        raise RandomError("list can't be 0!")
     str = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
     rlsa = []
     for rls in range(list):
         rlsa.append(choice(str))
     return rlsa
 def randlistcode(list):
+    if list == 0:
+        raise RandomError("list can't be 0!")
     rlc = []
     rlca = ''
     for rlcr in range(list):
         if randint(0, 1) == 0:
             rlc.append(str(rlca) + str(randint(0, 9)))
         else:
             rlc.append(str(rlca) + str(rcrandstr()))
@@ -86,31 +90,40 @@
 def randstrbs():
     rsbsA = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U','V', 'W', 'X', 'Y', 'Z']
     rsbs = choice(rsbsA)
     return rsbs
 #randcodebs:random code string that is big and small.
 #To print it,"print(randcodebs())"
 def randcodebs(digits):
+    if digits == 0:
+        raise RandomError("digits can't be 0!")
     randcodebs = ''
     for rsbs in range(digits):
         rcbsR = randint(0,2)
         if rcbsR==0:
             randcodebs = randcodebs + str(randint(0, 9))
         elif rcbsR==1:
             randcodebs = randcodebs + str(rcrandstr())
         else:
             randcodebs = randcodebs + str(randstrbs())
     return randcodebs
 #THIS MAY CRASH YOUR IDLE,PLEASE SAVE YOUR ALL FILES!!!
 def crashidle():
     print('This may crash your IDLE!!!')
     print('Please sure you save your code!')
-    input('Press <Enter> to begin crash.')
     while True:
-        randcode(6)
+        yorn = str(input('Input Y/N:'))
+        if yorn =='Y' or yorn =='y':
+            while True:
+                randcode(6)
+        elif yorn =='N' or yorn =='n':
+            break
+        else:
+            print('Use Y as yes,N as no.')
+
 #End Code#
 #Start Upgrade Code(use "upgrade()" to upgrade Leon Random Plus)
 def upgrade():
     system(f'pip install leonranp')
 #End Upgrade Code
 #You can use "leonranp.help()" to get help!
 def lrphelp():
@@ -120,14 +133,15 @@
     print('upgrade() -> Upgrade Leon Random Plus')
     print('randbool() -> Random bool')
     print('dellrp() -> Delete Leon Random Plus')
     print('sample() -> Sample code')
     print('crashidle() -> Crash my IDLE')
     print('randstrbs() -> Random string that is big and small')
     print('randcodebs() -> Random code string that is big and small')
+    print('lrpinfo() -> Leon Random Plus info')
     print('---Leon Random Plus Help End---')
 #Del. Leon Random Plus
 #OMG you are gonna delete Leon Random Plus???
 def dellrp():
     system(f'pip uninstall leonranp')
     print('Thanks for using Leon Random Plus!')
     print('Please restart your IDLE.')
@@ -152,8 +166,11 @@
         sam2 = randspace(0,30)
         if sam2 == True:
             print('You are so lucky today!')
         else:
             print('Oh no!You are not lucky today!')
             print('Go to http://leonmmcoset.jjmm.ink:8002/doku.php?id=iamnotlucky')
     print('--------------------------')
-    print('Thanks for use!')
+    print('Thanks for use!')
+#Info for Leon Random Plus
+def lrpinfo():
+    import InfoWindow
```

### Comparing `leonranp-0.1/leonranp.egg-info/PKG-INFO` & `leonranp-0.1.1/leonranp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leonranp
-Version: 0.1
+Version: 0.1.1
 Summary: This is Leon Random Plus,that add more functions to the random!
 Home-page: https://github.com/Leonmmcoset/leonranp
 Author: LeonMMcoset
 Author-email: leonmmcoset@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leonranp-0.1/setup.py` & `leonranp-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="leonranp",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.1",  # 包版本号，便于维护版本
+    version="0.1.1",  # 包版本号，便于维护版本
     author="LeonMMcoset",  # 作者，可以写自己的姓名
     author_email="leonmmcoset@outlook.com",  # 作者联系方式，可写自己的邮箱地址
     description="This is Leon Random Plus,that add more functions to the random!",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/Leonmmcoset/leonranp",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

