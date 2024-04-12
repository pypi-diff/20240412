# Comparing `tmp/st_common-1.3.9.tar.gz` & `tmp/st_common-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_common-1.3.9.tar", last modified: Fri Dec  1 03:57:28 2023, max compression
+gzip compressed data, was "st_common-1.4.1.tar", last modified: Fri Apr 12 01:23:32 2024, max compression
```

## Comparing `st_common-1.3.9.tar` & `st_common-1.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-12-01 03:57:28.331927 st_common-1.3.9/
--rw-rw-rw-   0        0        0      747 2023-08-31 07:53:31.000000 st_common-1.3.9/LICENSE
--rw-rw-rw-   0        0        0     4503 2023-12-01 03:57:28.331927 st_common-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-09-26 06:50:51.000000 st_common-1.3.9/README.md
--rw-rw-rw-   0        0        0      112 2023-12-01 03:57:28.333520 st_common-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     2125 2023-08-31 07:59:18.000000 st_common-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-01 03:57:28.280628 st_common-1.3.9/st_common/
--rw-rw-rw-   0        0        0      789 2023-12-01 03:56:05.000000 st_common-1.3.9/st_common/__init__.py
--rw-rw-rw-   0        0        0     7707 2023-09-12 06:04:39.000000 st_common-1.3.9/st_common/ccookies.py
--rw-rw-rw-   0        0        0    15311 2023-11-28 03:57:25.000000 st_common-1.3.9/st_common/commonbase.py
--rw-rw-rw-   0        0        0    28421 2023-11-24 01:09:12.000000 st_common-1.3.9/st_common/dbmodule.py
--rw-rw-rw-   0        0        0     2880 2023-11-28 06:13:37.000000 st_common-1.3.9/st_common/emailmodule.py
--rw-rw-rw-   0        0        0     4534 2023-09-12 06:05:05.000000 st_common-1.3.9/st_common/famodule.py
--rw-rw-rw-   0        0        0     4717 2023-10-30 03:39:50.000000 st_common-1.3.9/st_common/msgreport.py
--rw-rw-rw-   0        0        0    30216 2023-12-01 03:53:19.000000 st_common-1.3.9/st_common/rpamodule.py
--rw-rw-rw-   0        0        0     4107 2023-08-31 06:54:18.000000 st_common-1.3.9/st_common/securemodule.py
-drwxrwxrwx   0        0        0        0 2023-12-01 03:57:28.308184 st_common-1.3.9/st_common.egg-info/
--rw-rw-rw-   0        0        0     4503 2023-12-01 03:57:27.000000 st_common-1.3.9/st_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-12-01 03:57:28.000000 st_common-1.3.9/st_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-01 03:57:27.000000 st_common-1.3.9/st_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-12-01 03:57:27.000000 st_common-1.3.9/st_common.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-12-01 03:57:27.000000 st_common-1.3.9/st_common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-01 03:57:27.000000 st_common-1.3.9/st_common.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-01 03:57:28.310514 st_common-1.3.9/test/
--rw-rw-rw-   0        0        0     2817 2023-11-28 07:21:09.000000 st_common-1.3.9/test/test.py
-drwxrwxrwx   0        0        0        0 2023-12-01 03:57:28.329285 st_common-1.3.9/tests/
--rw-rw-rw-   0        0        0     1754 2023-10-20 07:41:43.000000 st_common-1.3.9/tests/test_commonbase.py
--rw-rw-rw-   0        0        0    18156 2023-11-21 02:11:06.000000 st_common-1.3.9/tests/test_dbmodule.py
--rw-rw-rw-   0        0        0      797 2023-09-26 05:45:13.000000 st_common-1.3.9/tests/test_msgreport.py
--rw-rw-rw-   0        0        0     6919 2023-09-28 01:57:04.000000 st_common-1.3.9/tests/test_rpamodule.py
--rw-rw-rw-   0        0        0     1833 2023-09-26 06:03:22.000000 st_common-1.3.9/tests/test_securemodule.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:23:32.296389 st_common-1.4.1/
+-rw-rw-rw-   0        0        0      747 2023-08-31 07:53:31.000000 st_common-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     4806 2024-04-12 01:23:32.296895 st_common-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-09-26 06:50:51.000000 st_common-1.4.1/README.md
+-rw-rw-rw-   0        0        0      112 2024-04-12 01:23:32.297910 st_common-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2125 2023-08-31 07:59:18.000000 st_common-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:23:32.270028 st_common-1.4.1/st_common/
+-rw-rw-rw-   0        0        0      785 2024-04-08 07:36:47.000000 st_common-1.4.1/st_common/__init__.py
+-rw-rw-rw-   0        0        0     7707 2023-09-12 06:04:39.000000 st_common-1.4.1/st_common/ccookies.py
+-rw-rw-rw-   0        0        0    15290 2024-02-05 06:03:22.000000 st_common-1.4.1/st_common/commonbase.py
+-rw-rw-rw-   0        0        0    28002 2024-01-31 01:28:10.000000 st_common-1.4.1/st_common/dbmodule.py
+-rw-rw-rw-   0        0        0     2880 2023-11-28 06:13:37.000000 st_common-1.4.1/st_common/emailmodule.py
+-rw-rw-rw-   0        0        0     4534 2023-09-12 06:05:05.000000 st_common-1.4.1/st_common/famodule.py
+-rw-rw-rw-   0        0        0     7396 2024-04-08 08:06:12.000000 st_common-1.4.1/st_common/msgreport.py
+-rw-rw-rw-   0        0        0    33714 2024-04-07 06:42:10.000000 st_common-1.4.1/st_common/rpamodule.py
+-rw-rw-rw-   0        0        0     4107 2023-08-31 06:54:18.000000 st_common-1.4.1/st_common/securemodule.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:23:32.282894 st_common-1.4.1/st_common.egg-info/
+-rw-rw-rw-   0        0        0     4806 2024-04-12 01:23:31.000000 st_common-1.4.1/st_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2024-04-12 01:23:31.000000 st_common-1.4.1/st_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 01:23:31.000000 st_common-1.4.1/st_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 01:23:31.000000 st_common-1.4.1/st_common.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2024-04-12 01:23:31.000000 st_common-1.4.1/st_common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 01:23:31.000000 st_common-1.4.1/st_common.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 01:23:32.284413 st_common-1.4.1/test/
+-rw-rw-rw-   0        0        0     2817 2023-11-28 07:21:09.000000 st_common-1.4.1/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:23:32.294861 st_common-1.4.1/tests/
+-rw-rw-rw-   0        0        0     1754 2023-10-20 07:41:43.000000 st_common-1.4.1/tests/test_commonbase.py
+-rw-rw-rw-   0        0        0    19249 2024-01-31 02:03:17.000000 st_common-1.4.1/tests/test_dbmodule.py
+-rw-rw-rw-   0        0        0      797 2023-09-26 05:45:13.000000 st_common-1.4.1/tests/test_msgreport.py
+-rw-rw-rw-   0        0        0     6919 2023-09-28 01:57:04.000000 st_common-1.4.1/tests/test_rpamodule.py
+-rw-rw-rw-   0        0        0     1833 2023-09-26 06:03:22.000000 st_common-1.4.1/tests/test_securemodule.py
```

### Comparing `st_common-1.3.9/LICENSE` & `st_common-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/PKG-INFO` & `st_common-1.4.1/st_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: st_common
-Version: 1.3.9
+Name: st-common
+Version: 1.4.1
 Summary: suitcase in st st_common module
 Home-page: https://github.com/VinMing/common
 Author: St
 Author-email: st@gmail.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -166,7 +166,18 @@
 
 # v1.3.8 (29 November 2023)
 - add commonbase extract_email
 
 
 # v1.3.9 (1 December 2023)
 - add rpamodule BaseBrowser parameter debuggerAddress
+
+# v1.3.11 (5 February 2024)
+- FIX commonbase get_filename_dict_in_filepath
+
+# v1.4.0 (8 April 2024)
+- [FIX] rpa BaseBrowser parameter chrome_options
+- add rpa get_print_options_normal
+- add rpa capture_from_element_xpath and capture_from_points
+
+# v1.4.1 (10 April 2024)
+- add msgreport DFS
```

### Comparing `st_common-1.3.9/setup.py` & `st_common-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/st_common/ccookies.py` & `st_common-1.4.1/st_common/ccookies.py`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/st_common/commonbase.py` & `st_common-1.4.1/st_common/commonbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,16 +74,14 @@
         elif record.levelno == logging.WARNING:
             self.warning_count += 1
             self.warning_messages.append(record.getMessage())
 class BaseLogger:
     def __init__(self, level=logging.DEBUG, log_file=None):
         self.logger = logging.getLogger(self.__class__.__name__)
         self.logger.setLevel(level)
-        
-        
         if log_file or not self.logger.hasHandlers():   # 这行代码会防止在logger上重复添加handler
         # if log_file:
             handler = logging.FileHandler(log_file)
         else:
             handler = logging.StreamHandler()
         formatter = logging.Formatter('%(asctime)s %(filename)s[line:%(lineno)d] %(levelname)s: %(message)s')
         handler.setFormatter(formatter)
@@ -107,15 +105,14 @@
         """
         if isinstance(strs, str):
             for _char in strs:
                 if '\u4e00' <= _char <= '\u9fa5':
                     return True
         return False
 
-
     def extract_email(self, text:str):
         """
         Description:
             extract_email
         Args:
             text (str): The first integer to add.
         Returns:
@@ -129,16 +126,15 @@
             Exception: error
         """
         # 定义一个正则表达式，匹配邮箱地址
         email_regex = r'[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}'
         # 在文本中查找匹配的邮箱地址
         emails = re.findall(email_regex, text)
         return emails
-
-    
+ 
     def is_valid_filename(self, filename, platform="linux"):
         """
         Description:
             检查字符串是否符合win系统或者linux系统的文件命名
         Args:
             filename (str): filename 
             platform (str): linux / windows
@@ -203,15 +199,15 @@
                 result_list.append(absolute_path)
 
         # 按创建时间降序排列，最新的在前
         # result_list.sort(key=lambda x: x[1], reverse=True) if is_sort else None
         result_list.sort(key=lambda x: os.path.getctime(x), reverse=True) if is_sort else None
         num = sort_num if sort_num else max(result_list)
         return [file for file in result_list[:num]]  # 返回文件的路径
-    def get_filename_dict_in_filepath(dirpath:str, file_ext: str) -> dict :
+    def get_filename_dict_in_filepath(self, dirpath:str, file_ext: str) -> dict :
         """
         Description:
             get filename with dict in filepath 
         Args:
             dirpath (str): dir path
             file_ext (str): file extender
         Returns:
```

### Comparing `st_common-1.3.9/st_common/dbmodule.py` & `st_common-1.4.1/st_common/dbmodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 在Python中,我们可以创建一个通用的数据驱动层接口,然后分别为MongoDB,MySQL和Oracle,Redis实现这个接口。
 SQLAlchemy 主要用于关系型数据库，并且不直接支持 MongoDB 和 Redis,所以对于这两种类型的数据库我们需要单独处理。
 '''
 
 # import logging
 
 
-import hashlib
+from urllib.parse import quote_plus
 
 def orm_update_or_insert(session, data, filtkeys, table, update=False, updatekeys=None):
     """
     基于orm更新/插入数据
     :param session: sessionmaker(),
     :param data: dict/series,
     :param filtkeys: list, 键名, 用于筛选数据
@@ -436,18 +436,14 @@
             db_string (str): mongodb://[username:password@]host1[:port1][,host2[:port2],...[,hostN[:portN]]][/[database][?options]]
         Returns:
             None
         Raises:
             Exception: error
         """
         super().__init__()
-        # mongodb_username = quote_plus(mongodb_username)
-        # mongodb_password = quote_plus(mongodb_password)
-        # connection_string = f"mongodb://{mongodb_username}:{mongodb_password}@{mongodb_host}:{mongodb_port}/{database_name}"
-        # print(connection_string)
         self.client = MongoClient(db_string)
     def save_to_mongo(self,database_name: str, collection_name: str, doc: dict) -> bool:
         """
         Description:
             根据集合名字和文档保存在mongodb
         Args:
             database_name(str): 数据库名称
@@ -460,18 +456,16 @@
             3
         Raises:
             Exception: error
         """
         acknowledged, message = self.insert_document(database_name= database_name,
                                           collection_name= collection_name, document=doc)
         if acknowledged:
-            self.logger.info("Inserted document with  in collection: %s",collection_name)
             return True
         else:
-            self.logger.error("插入失败，错误为：%s",message )
             return False
         
     def get_database(self, database_name:str):
         """
         Description:
            获取指定名称的数据库。
         Args:
```

### Comparing `st_common-1.3.9/st_common/emailmodule.py` & `st_common-1.4.1/st_common/emailmodule.py`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/st_common/famodule.py` & `st_common-1.4.1/st_common/famodule.py`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/st_common/msgreport.py` & `st_common-1.4.1/st_common/msgreport.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import json
 import traceback
+import os
 ### time costs
 from functools import wraps
 def ISZ_main_exception_report_args(msg):
     def main_exception_report(function):
         @wraps(function)
         def function_main_exception_report(*args, **kwargs):
             try:
@@ -93,7 +94,73 @@
         })
         headers = {
             'Content-Type': 'application/json'
         }
 
         response = requests.request("POST", self.webhook, headers=headers, data=payload)
         return response
+
+
+
+
+class DFS():
+    ###上传文件，包含图片
+    def __init__(self,tracker_conf_file="client-test.conf",file_base_url="http://192.168.6.253") -> None:
+        """__init__ _summary_
+
+        update issyzone dfs
+
+        Args:
+            tracker_conf_file (str, optional): confine file . Defaults to "client-test.conf".
+            file_base_url (str, optional): url. Defaults to "http://192.168.6.253".
+        """
+        self.tracker_conf =tracker_conf_file
+        self.file_base_url = file_base_url
+        from fdfs_client.client import get_tracker_conf, Fdfs_client
+        tracker_conf = get_tracker_conf(self.tracker_conf)
+        self.client = Fdfs_client(tracker_conf)
+        pass
+    def uploadDfs(self, local_path, file_name=None):
+        """
+        Description:
+            upload file with dfs
+        Args:
+            local_path (str): file abspath
+
+            file_name [option](str) : file name
+        Returns:
+            None
+        Example:
+        Raises:
+            Exception: error
+        """
+        
+        ext = ''
+        if local_path.rindex('.') + 2 < len(local_path):
+            ext = local_path[local_path.rindex('.') + 1:]
+        if file_name is None:
+            file_name = 'auto.' + ext
+        meta = {'fileExt': ext, 'fileLength': str(os.path.getsize(local_path)), 'fileName': file_name}
+        result = self.client.upload_by_filename(local_path, meta)
+        if result["Status"] == "Upload successed.":
+          remote_file = result["Remote file_id"]
+          file_path = str(remote_file, encoding="utf-8")
+          return file_path
+        else:
+            return None
+    def get_absolute_path(self, relative_path):
+      return os.path.abspath(relative_path) if os.path.exists(relative_path) else None
+    
+
+    def upload_file_remote_id(self,picture_path):
+        result_remote_file_id = self.uploadDfs(local_path=picture_path)
+        if not result_remote_file_id:
+            self.logger.error(f"{picture_path}, result_remote_file_id:None, please check!")
+            return (None,None)
+        file_down = self.file_base_url + "/system/file/origin?filePath=" + result_remote_file_id
+        ### update table relationship
+        # one_dict = {
+        #     "local_name":os.path.split(picture_path)[-1],
+        #     "remote": file_down,
+        # }
+        # self.logger.error(f"update table relationship error: {one_dict}") if not self.sqldatabase.update_or_insert_data(table_name="relation_weatherology_picture",data_dict=one_dict,deduplicate_mode="unique") else None
+        return (os.path.split(picture_path)[-1] , file_down)
```

### Comparing `st_common-1.3.9/st_common/rpamodule.py` & `st_common-1.4.1/st_common/rpamodule.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.ui import Select
 
 from typing import Union
 import time
 import random
 import pandas as pd
+import json
+from PIL import Image
 def get_options_lab():
     """
     Description:
         set chrome options in lab
     Args:
     Returns: ChromeOptions
     Example:
@@ -59,49 +61,86 @@
     Args:
         download_dir(str): download file dir
     Returns: ChromeOptions
     Example:
     Raises:
         Exception: error
     """
-    pass
     options = ChromeOptions()
     prefs = {
         # 'profile.managed_default_content_settings.images': 2,  # not load picture
         'profile.default_content_settings.popups': 0,  # No Popups
         'download.default_directory': download_dir,  
     }
     options.add_experimental_option('prefs', prefs)
     print("add get_options_normal argument")
     return options
 
+def get_print_options_normal(download_dir=r'D:\issyzone\workspace\track'):
+    """
+    Description:
+        set chrome options in normal
+    Args:
+        
+    Returns: ChromeOptions
+    Example:
+    Raises:
+        Exception: error
+    """
+    options = ChromeOptions()
+    options.add_argument('--enable-print-browser')  # 启用PrintBrowser模式，其中所有内容都呈现为打印
+    options.add_argument('--kiosk-printing')  # 在打印预览中自动按下打印按钮
+    settings = {
+        "recentDestinations": [
+        {
+            "id": "Save as PDF",
+            "origin": "local"
+        }
+        ],
+        "selectedDestinationId": "Save as PDF",
+        "version": 2
+    }
+    prefs = {
+        'printing.print_preview_sticky_settings.appState': json.dumps(settings),
+        'savefile.default_directory': download_dir  # 下载文件保存的路径
+    }
+    options.add_experimental_option('prefs', prefs)
+    print("add get_print_options_normal argument")
+    return options
+
 from st_common import CommonBase
 class BaseBrowser(CommonBase):
-    def __init__(self,headless=False,impli_waitime=8,expli_waitime=24,log_file=None,debuggerAddress=None):
+    def __init__(self,headless=False,
+                 impli_waitime=8,expli_waitime=24,
+                 log_file=None,debuggerAddress=None,chrome_options=None):
         """
         Description:
             base browser init
         Args:
             headless (bool): headless browser
             impli_waitime (int): implicitly wait time
             expli_waitime (int): explicitly wait time
-            expli_waitime = impli_waitime * 3 (common)
+                expli_waitime = impli_waitime * 3 (common)
+            log_file (str): logger file
+            debuggerAddress (str): '127.0.0.1:9992'
         Returns:
             int: The sum of a and b.
         Example:
             >>> add(1, 2)
             3
         Raises:
             Exception: error
         """
         super().__init__(log_file=log_file)
-        options = get_options_lab() if headless else get_options_normal()
-        options.add_experimental_option("debuggerAddress", debuggerAddress) if debuggerAddress else None
+        if not chrome_options:
+            chrome_options = get_options_lab() if headless else get_options_normal()
+        # options = get_print_options_normal() if print_status else get_options_normal()
+        chrome_options.add_experimental_option("debuggerAddress", debuggerAddress) if debuggerAddress else None
         self.logger.info("webdriver chrome initing....")
-        self.browser = webdriver.Chrome(options=options)
+        self.browser = webdriver.Chrome(options=chrome_options)
         self.logger.info("webdriver chrome init Over")
         self.browser.implicitly_wait(impli_waitime)
         self.__wait = WebDriverWait(self.browser, expli_waitime)
     def __del__(self):
         """
         Description:
             befor del 
@@ -208,28 +247,28 @@
             WebElement: selenium.webdriver.remote.webelement.WebElement
         Example:
         Raises:
             Exception: error
         """
         return self.browser.find_element_by_partial_link_text(partial_link_text)
     
-    def click_by_xpath(self, element_xpath) -> bool:
+    def click_by_xpath(self, element_xpath,attempts=3) -> bool:
         """
         Description:
             according to xpath, click
         Args:
             element_xpath (str): input box with xpath
         Returns:
             bool: True / Flase
         Example:
         Raises:
             Exception: error
         """
         try:
-            element_click = self.get_element_by_xpath_wait(xpath=element_xpath)
+            element_click = self.get_element_by_xpath_wait(xpath=element_xpath,attempts=attempts)
             element_click.click()
         except AttributeError as err:
             self.logger.error(err,exc_info=True,stack_info=False)
             self.logger.error('click_by_xpath: %s , click NoneType object' % element_xpath)
             return False
         except Exception as err:
             self.logger.error(err,exc_info=True,stack_info=False)
@@ -401,14 +440,67 @@
             cell_data = [cell.text for cell in cells]
             table_data.append(cell_data)
         
         # 将数据转换成pandas DataFrame
         df = pd.DataFrame(table_data, columns=headers)
         
         return df
+    
+    #### snapshot
+    def capture_from_element_xpath(self,xpath='//*[@id="forecast-map-wrap"]',
+                                        picture_name="tmp.png",
+                                        picture_dir=None,
+                                        direct=None
+                                        ,direct_num=2,
+                                        width=0,height=0):
+
+
+        ### 滚动到指定位置
+        map = self.get_element_by_xpath_wait(xpath=xpath)
+        
+        self.scroll_to_element(element=map)
+        if direct:
+            actions = ActionChains(self.browser)
+            ## 按键 次
+            for i in range(0,direct_num):
+                actions.send_keys(direct).perform()
+                time.sleep(1)
+        
+        ### 保存到缓存本地，一定要保存到本地，不然页面会重新刷新，有广告页出现会导致像素定位错误
+        map.screenshot(picture_name)
+
+        ### 保存到本地
+        # im = Image.open(picture_name)
+
+        # if width != 0 and height != 0:
+        #     im = im.crop((0,0,width,height))
+        # im.save(os.path.join(picture_dir,picture_name)) if picture_dir else im.save(picture_name)
+        return True
+
+
+    def capture_from_points(self,left_top_point, right_bottom_point,picture_name,start_element_xpath=None):
+        
+        ### 可视化
+        if start_element_xpath:
+            self.scroll_to_element(element=self.get_element_by_xpath_wait(xpath=start_element_xpath))
+        ####
+        """
+        p1 = (425: start., 130)
+        p2 = (1125, 824)
+        tmp_element_xpath = '//*[@id="main-column"]/section/ul'
+        tmp_element = self.get_element_by_xpath_wait(xpath=tmp_element_xpath)
+        """
+        time.sleep(2)
+        tmp_png = '_full_screenshot.png'
+        self.browser.save_screenshot(filename=tmp_png)
+        im = Image.open(tmp_png)
+        im = im.crop((left_top_point[0],left_top_point[1], right_bottom_point[0],right_bottom_point[1]))
+        im.save(os.path.join(self.picture_dir,picture_name))
+
+    
     def select_from_name(self,select_name_value:str="pjname",visible_text:str=None)-> bool:
         """select_from_name _summary_
 
         _extended_summary_
 
         Args:
             select_name_value (str, optional): _description_. Defaults to "pjname".
```

### Comparing `st_common-1.3.9/st_common/securemodule.py` & `st_common-1.4.1/st_common/securemodule.py`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/st_common.egg-info/PKG-INFO` & `st_common-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: st-common
-Version: 1.3.9
+Name: st_common
+Version: 1.4.1
 Summary: suitcase in st st_common module
 Home-page: https://github.com/VinMing/common
 Author: St
 Author-email: st@gmail.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -166,7 +166,18 @@
 
 # v1.3.8 (29 November 2023)
 - add commonbase extract_email
 
 
 # v1.3.9 (1 December 2023)
 - add rpamodule BaseBrowser parameter debuggerAddress
+
+# v1.3.11 (5 February 2024)
+- FIX commonbase get_filename_dict_in_filepath
+
+# v1.4.0 (8 April 2024)
+- [FIX] rpa BaseBrowser parameter chrome_options
+- add rpa get_print_options_normal
+- add rpa capture_from_element_xpath and capture_from_points
+
+# v1.4.1 (10 April 2024)
+- add msgreport DFS
```

### Comparing `st_common-1.3.9/st_common.egg-info/SOURCES.txt` & `st_common-1.4.1/st_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/test/test.py` & `st_common-1.4.1/test/test.py`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/tests/test_commonbase.py` & `st_common-1.4.1/tests/test_commonbase.py`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/tests/test_dbmodule.py` & `st_common-1.4.1/tests/test_dbmodule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,41 @@
 import unittest
 from parameterized import parameterized
 
-from st_common import SQLDatabase,RedisPriorityQueue
+from st_common import SQLDatabase,RedisPriorityQueue,MongoDBClient
 from st_common import CommonBase
 from st_common import Secure
 
 import pandas as pd
 from table_strcture import TableSellersCompetitor, TableCommonSess,TableVideoIcRaw,TableSellersCompetitor
 from sqlalchemy import text
 import pandas as pd
 import os
+from urllib.parse import quote_plus
+class MongoDBDatabaseTest(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        print("在每个类之前执行，如创建一个类，创建数据库链接，初始化日志对象")
+        # 使用 quote_plus 来进行URL编码
+        username = "spider_user"
+        password = "Syz2022"
+        # 构造数据库连接字符串
+        # db_string = f"mongodb://{username}:{password}@host:port/database"
+        cls.my_mongodb = MongoDBClient(db_string=f"mongodb://{username}:{password}@192.168.6.243:27017/spider_data")
+        ### mongodb://[username:password@]host1[:
+    @classmethod
+    def tearDownClass(cls) -> None:
+        print("在每个类之后执行，如销毁一个类，销毁数据库链接，销毁日志对象")
 
-
+    # @unittest.skip(reason="test_push pass")
+    def test_insert(self,):
+        status = self.my_mongodb.insert_document(database_name="spider_data",collection_name="cache_tiktok_api_search",document={"a":1})
+        print(status)
+        print("over")
+        pass
 class RedisDatabaseTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         print("在每个类之前执行，如创建一个类，创建数据库链接，初始化日志对象")
         cls.my_redis = RedisPriorityQueue(name="seller_priority_queue", host="192.168.6.247", port=6379, db=0)
     @classmethod
     def tearDownClass(cls) -> None:
@@ -100,15 +120,14 @@
     def test_create_table_03(self):
         self.assertTrue(expr=self.sqldatabase.create_table(table_name=TableVideoIcRaw.__tablename__,declarative_base_table=TableVideoIcRaw))
 
     @unittest.skip(reason="table structure with base pass")
     def test_create_table_04(self):
         self.assertTrue(expr=self.sqldatabase.create_table(table_name=TableSellersCompetitor.__tablename__,declarative_base_table=TableSellersCompetitor))
    
-   
     @parameterized.expand(
             [
                 ("all_account", {"station_name":"test","username":"test01","password":"testpw","status":"0"}),
                 # ("all_account_orm", {"station_name":"test","username":"test01","password":"testpw","status":"0"})
                 ]
     )
     @unittest.skip(reason="test_insert_data_01 pass")
```

### Comparing `st_common-1.3.9/tests/test_msgreport.py` & `st_common-1.4.1/tests/test_msgreport.py`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/tests/test_rpamodule.py` & `st_common-1.4.1/tests/test_rpamodule.py`

 * *Files identical despite different names*

### Comparing `st_common-1.3.9/tests/test_securemodule.py` & `st_common-1.4.1/tests/test_securemodule.py`

 * *Files identical despite different names*

