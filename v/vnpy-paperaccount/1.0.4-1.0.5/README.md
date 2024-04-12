# Comparing `tmp/vnpy_paperaccount-1.0.4.tar.gz` & `tmp/vnpy_paperaccount-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_paperaccount-1.0.4.tar", last modified: Mon Apr  1 06:40:43 2024, max compression
+gzip compressed data, was "vnpy_paperaccount-1.0.5.tar", last modified: Fri Apr 12 04:45:41 2024, max compression
```

## Comparing `vnpy_paperaccount-1.0.4.tar` & `vnpy_paperaccount-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 06:40:43.733917 vnpy_paperaccount-1.0.4/
--rw-rw-rw-   0        0        0     1109 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1880 2024-04-01 06:40:43.733917 vnpy_paperaccount-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      926 2024-04-01 06:38:05.000000 vnpy_paperaccount-1.0.4/README.md
--rw-rw-rw-   0        0        0     1056 2024-04-01 06:40:43.736667 vnpy_paperaccount-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 06:40:43.672318 vnpy_paperaccount-1.0.4/vnpy_paperaccount/
--rw-rw-rw-   0        0        0     1780 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount/__init__.py
--rw-rw-rw-   0        0        0    22778 2024-04-01 06:39:31.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount/engine.py
-drwxrwxrwx   0        0        0        0 2024-04-01 06:40:43.731747 vnpy_paperaccount-1.0.4/vnpy_paperaccount/ui/
--rw-rw-rw-   0        0        0       34 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount/ui/__init__.py
--rw-rw-rw-   0        0        0    67134 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount/ui/paper.ico
--rw-rw-rw-   0        0        0     2460 2024-04-01 06:37:14.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount/ui/widget.py
-drwxrwxrwx   0        0        0        0 2024-04-01 06:40:43.727970 vnpy_paperaccount-1.0.4/vnpy_paperaccount.egg-info/
--rw-rw-rw-   0        0        0     1880 2024-04-01 06:40:43.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2024-04-01 06:40:43.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 06:40:43.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-01 06:40:43.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2024-04-01 06:40:43.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-01 06:40:43.000000 vnpy_paperaccount-1.0.4/vnpy_paperaccount.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 04:45:41.404796 vnpy_paperaccount-1.0.5/
+-rw-rw-rw-   0        0        0     1109 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1880 2024-04-12 04:45:41.405887 vnpy_paperaccount-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2024-04-12 04:44:55.000000 vnpy_paperaccount-1.0.5/README.md
+-rw-rw-rw-   0        0        0     1056 2024-04-12 04:45:41.409729 vnpy_paperaccount-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:45:40.198064 vnpy_paperaccount-1.0.5/vnpy_paperaccount/
+-rw-rw-rw-   0        0        0     1780 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount/__init__.py
+-rw-rw-rw-   0        0        0    22893 2024-04-12 04:44:14.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount/engine.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:45:41.404201 vnpy_paperaccount-1.0.5/vnpy_paperaccount/ui/
+-rw-rw-rw-   0        0        0       34 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount/ui/__init__.py
+-rw-rw-rw-   0        0        0    67134 2023-11-21 08:09:56.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount/ui/paper.ico
+-rw-rw-rw-   0        0        0     2460 2024-04-01 06:37:14.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount/ui/widget.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:45:41.136586 vnpy_paperaccount-1.0.5/vnpy_paperaccount.egg-info/
+-rw-rw-rw-   0        0        0     1880 2024-04-12 04:45:39.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2024-04-12 04:45:40.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 04:45:39.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-01 06:40:43.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2024-04-12 04:45:39.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 04:45:39.000000 vnpy_paperaccount-1.0.5/vnpy_paperaccount.egg-info/top_level.txt
```

### Comparing `vnpy_paperaccount-1.0.4/LICENSE` & `vnpy_paperaccount-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_paperaccount-1.0.4/PKG-INFO` & `vnpy_paperaccount-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_paperaccount
-Version: 1.0.4
+Version: 1.0.5
 Summary: Paper account application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,15 +24,15 @@
 # VeighNa框架的本地仿真交易模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.4-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.5-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_paperaccount-1.0.4/README.md` & `vnpy_paperaccount-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的本地仿真交易模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.4-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.5-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_paperaccount-1.0.4/setup.cfg` & `vnpy_paperaccount-1.0.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7061 7065 7261 6363   = vnpy_paperacc
 00000020: 6f75 6e74 0d0a 7665 7273 696f 6e20 3d20  ount..version = 
-00000030: 312e 302e 340d 0a75 726c 203d 2068 7474  1.0.4..url = htt
+00000030: 312e 302e 350d 0a75 726c 203d 2068 7474  1.0.5..url = htt
 00000040: 7073 3a2f 2f77 7777 2e76 6e70 792e 636f  ps://www.vnpy.co
 00000050: 6d0d 0a6c 6963 656e 7365 203d 204d 4954  m..license = MIT
 00000060: 0d0a 6175 7468 6f72 203d 2058 6961 6f79  ..author = Xiaoy
 00000070: 6f75 2043 6865 6e0d 0a61 7574 686f 725f  ou Chen..author_
 00000080: 656d 6169 6c20 3d20 7869 616f 796f 752e  email = xiaoyou.
 00000090: 6368 656e 406d 6169 6c2e 766e 7079 2e63  chen@mail.vnpy.c
 000000a0: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description
```

### Comparing `vnpy_paperaccount-1.0.4/vnpy_paperaccount/__init__.py` & `vnpy_paperaccount-1.0.5/vnpy_paperaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_paperaccount-1.0.4/vnpy_paperaccount/engine.py` & `vnpy_paperaccount-1.0.5/vnpy_paperaccount/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,18 @@
         elif self.ib_gateway and req.exchange in self.ib_gateway.exchanges:
             self._subscribe(req, "IB")
         else:
             return None
 
     def send_order(self, req: OrderRequest, gateway_name: str) -> str:
         """"""
+        if not req.volume:
+            self.write_log("委托数量非法，请检查")
+            return ""
+
         contract: Optional[ContractData] = self.main_engine.get_contract(req.vt_symbol)
         if not contract:
             self.write_log(f"委托失败，找不到该合约{req.vt_symbol}")
             return ""
 
         self.order_count += 1
         now: str = datetime.now().strftime("%y%m%d%H%M%S")
```

### Comparing `vnpy_paperaccount-1.0.4/vnpy_paperaccount/ui/paper.ico` & `vnpy_paperaccount-1.0.5/vnpy_paperaccount/ui/paper.ico`

 * *Files identical despite different names*

### Comparing `vnpy_paperaccount-1.0.4/vnpy_paperaccount/ui/widget.py` & `vnpy_paperaccount-1.0.5/vnpy_paperaccount/ui/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy_paperaccount-1.0.4/vnpy_paperaccount.egg-info/PKG-INFO` & `vnpy_paperaccount-1.0.5/vnpy_paperaccount.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-paperaccount
-Version: 1.0.4
+Version: 1.0.5
 Summary: Paper account application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,15 +24,15 @@
 # VeighNa框架的本地仿真交易模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.4-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.5-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

