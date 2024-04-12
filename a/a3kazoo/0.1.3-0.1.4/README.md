# Comparing `tmp/a3kazoo-0.1.3.tar.gz` & `tmp/a3kazoo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a3kazoo-0.1.3.tar", last modified: Sun Mar 31 09:41:54 2024, max compression
+gzip compressed data, was "a3kazoo-0.1.4.tar", last modified: Fri Apr 12 02:28:13 2024, max compression
```

## Comparing `a3kazoo-0.1.3.tar` & `a3kazoo-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-31 09:41:54.413436 a3kazoo-0.1.3/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3kazoo-0.1.3/LICENSE
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       65 2024-03-21 01:52:46.000000 a3kazoo-0.1.3/MANIFEST.in
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1236 2024-03-31 09:41:54.413436 a3kazoo-0.1.3/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      125 2024-03-21 01:53:02.000000 a3kazoo-0.1.3/README.md
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-31 09:41:54.413436 a3kazoo-0.1.3/a3kazoo/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       47 2024-03-29 06:10:38.000000 a3kazoo-0.1.3/a3kazoo/__init__.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-31 09:41:54.413436 a3kazoo-0.1.3/a3kazoo/scene_cases/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       24 2024-03-21 02:01:29.000000 a3kazoo-0.1.3/a3kazoo/scene_cases/__init__.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-31 09:41:54.413436 a3kazoo-0.1.3/a3kazoo/scene_cases/watch_nodes/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      169 2024-03-29 06:18:34.000000 a3kazoo-0.1.3/a3kazoo/scene_cases/watch_nodes/__init__.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1095 2024-03-28 03:52:34.000000 a3kazoo-0.1.3/a3kazoo/scene_cases/watch_nodes/abstract_node_change_service.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      942 2024-03-29 06:18:34.000000 a3kazoo-0.1.3/a3kazoo/scene_cases/watch_nodes/cmds.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1697 2024-03-29 06:08:27.000000 a3kazoo-0.1.3/a3kazoo/scene_cases/watch_nodes/node_thread.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1564 2024-03-28 03:39:40.000000 a3kazoo-0.1.3/a3kazoo/utils.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-31 09:41:54.413436 a3kazoo-0.1.3/a3kazoo.egg-info/
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1236 2024-03-31 09:41:54.000000 a3kazoo-0.1.3/a3kazoo.egg-info/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      496 2024-03-31 09:41:54.000000 a3kazoo-0.1.3/a3kazoo.egg-info/SOURCES.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-03-31 09:41:54.000000 a3kazoo-0.1.3/a3kazoo.egg-info/dependency_links.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-03-31 09:41:54.000000 a3kazoo-0.1.3/a3kazoo.egg-info/not-zip-safe
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       26 2024-03-31 09:41:54.000000 a3kazoo-0.1.3/a3kazoo.egg-info/requires.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        8 2024-03-31 09:41:54.000000 a3kazoo-0.1.3/a3kazoo.egg-info/top_level.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1131 2024-03-31 09:41:54.413436 a3kazoo-0.1.3/setup.cfg
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3kazoo-0.1.3/setup.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-12 02:28:13.947235 a3kazoo-0.1.4/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3kazoo-0.1.4/LICENSE
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       65 2024-03-21 01:52:46.000000 a3kazoo-0.1.4/MANIFEST.in
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1236 2024-04-12 02:28:13.947235 a3kazoo-0.1.4/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      125 2024-03-21 01:53:02.000000 a3kazoo-0.1.4/README.md
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-12 02:28:13.947235 a3kazoo-0.1.4/a3kazoo/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       47 2024-04-12 02:27:30.000000 a3kazoo-0.1.4/a3kazoo/__init__.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-12 02:28:13.947235 a3kazoo-0.1.4/a3kazoo/scene_cases/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       24 2024-03-21 02:01:29.000000 a3kazoo-0.1.4/a3kazoo/scene_cases/__init__.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-12 02:28:13.947235 a3kazoo-0.1.4/a3kazoo/scene_cases/watch_nodes/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      169 2024-03-29 06:18:34.000000 a3kazoo-0.1.4/a3kazoo/scene_cases/watch_nodes/__init__.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1095 2024-03-28 03:52:34.000000 a3kazoo-0.1.4/a3kazoo/scene_cases/watch_nodes/abstract_node_change_service.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      983 2024-04-12 02:20:20.000000 a3kazoo-0.1.4/a3kazoo/scene_cases/watch_nodes/cmds.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1832 2024-04-12 02:20:20.000000 a3kazoo-0.1.4/a3kazoo/scene_cases/watch_nodes/node_thread.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     2397 2024-04-12 02:20:20.000000 a3kazoo-0.1.4/a3kazoo/utils.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-12 02:28:13.947235 a3kazoo-0.1.4/a3kazoo.egg-info/
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1236 2024-04-12 02:28:13.000000 a3kazoo-0.1.4/a3kazoo.egg-info/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      496 2024-04-12 02:28:13.000000 a3kazoo-0.1.4/a3kazoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-12 02:28:13.000000 a3kazoo-0.1.4/a3kazoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-12 02:28:13.000000 a3kazoo-0.1.4/a3kazoo.egg-info/not-zip-safe
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       26 2024-04-12 02:28:13.000000 a3kazoo-0.1.4/a3kazoo.egg-info/requires.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        8 2024-04-12 02:28:13.000000 a3kazoo-0.1.4/a3kazoo.egg-info/top_level.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1131 2024-04-12 02:28:13.947235 a3kazoo-0.1.4/setup.cfg
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3kazoo-0.1.4/setup.py
```

### Comparing `a3kazoo-0.1.3/LICENSE` & `a3kazoo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `a3kazoo-0.1.3/PKG-INFO` & `a3kazoo-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3kazoo
-Version: 0.1.3
+Version: 0.1.4
 Summary: It is just a thin wrapper of kazoo.
 Home-page: https://github.com/three-kinds/a3kazoo
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3kazoo
 Project-URL: Source, https://github.com/three-kinds/a3kazoo
```

### Comparing `a3kazoo-0.1.3/a3kazoo/scene_cases/watch_nodes/abstract_node_change_service.py` & `a3kazoo-0.1.4/a3kazoo/scene_cases/watch_nodes/abstract_node_change_service.py`

 * *Files identical despite different names*

### Comparing `a3kazoo-0.1.3/a3kazoo/scene_cases/watch_nodes/cmds.py` & `a3kazoo-0.1.4/a3kazoo/scene_cases/watch_nodes/cmds.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from a3kazoo.utils import zk_state_listener, zk_ensure_path
 from .abstract_node_change_service import AbstractNodeChangeService
 
 
 def run_watch_nodes_server(conf: dict, nodes_path: str, node_change_service: AbstractNodeChangeService, exit_event: Event, logger: logging.Logger):
     zk = KazooClient(**conf)
-    zk.add_listener(zk_state_listener(logger, exit_event))
+    zk.add_listener(zk_state_listener(logger, exit_event, zk, timeout_seconds=conf.get('timeout')))
     zk.start()
 
     try:
         zk_ensure_path(zk=zk, path=nodes_path, logger=logger)
     except NoNodeError:
         logger.critical(f"NoNodeError: 请确认路径与ACL, {nodes_path}")
         zk.stop()
```

### Comparing `a3kazoo-0.1.3/a3kazoo/scene_cases/watch_nodes/node_thread.py` & `a3kazoo-0.1.4/a3kazoo/scene_cases/watch_nodes/node_thread.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,33 @@
         self._zk: Optional[KazooClient] = None
         self._exit_event = Event()
         # 配置为守护线程
         super().__init__(daemon=True, *args, **kwargs)
 
     def get_node_id(self) -> str:
         zk = KazooClient(**self._conf)
-        zk.add_listener(zk_state_listener(logger=logger, exit_event=self._exit_event))
+        zk.add_listener(zk_state_listener(logger=logger, exit_event=self._exit_event, zk=zk, timeout_seconds=self._conf.get('timeout')))
         zk.start()
 
         value = zk.create(path=self._nodes_path, ephemeral=True, sequence=True)
         node_id = value.rsplit('/', 2)[-1]
+        logger.info(f'获得节点id: {node_id}')
 
         def _close_zk(zk_client: KazooClient):
             logger.info(f'退出时断开zookeeper')
             zk_client.stop()
             zk_client.close()
 
         # 当进程退出时（非zookeeper影响），主动关闭连接
         atexit.register(_close_zk, zk)
         self._zk = zk
         return node_id
 
     def run(self):
         # 如果不使用线程等，当服务端挂掉，客户端还不知道，会继续执行
         self._exit_event.wait()
+
+        self._exit_event.clear()
+
         # 当与zookeeper服务端断开连接时，主动将进程退出
         if self._should_force_exit:
             force_exit_from_threads(f'因与zookeeper服务端断开连接，所以整个进程退出')
```

### Comparing `a3kazoo-0.1.3/a3kazoo.egg-info/PKG-INFO` & `a3kazoo-0.1.4/a3kazoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3kazoo
-Version: 0.1.3
+Version: 0.1.4
 Summary: It is just a thin wrapper of kazoo.
 Home-page: https://github.com/three-kinds/a3kazoo
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3kazoo
 Project-URL: Source, https://github.com/three-kinds/a3kazoo
```

### Comparing `a3kazoo-0.1.3/setup.cfg` & `a3kazoo-0.1.4/setup.cfg`

 * *Files identical despite different names*

