# Comparing `tmp/serverish-1.1.0.tar.gz` & `tmp/serverish-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverish-1.1.0.tar", max compression
+gzip compressed data, was "serverish-1.1.1.tar", max compression
```

## Comparing `serverish-1.1.0.tar` & `serverish-1.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1066 2023-10-11 16:33:06.592284 serverish-1.1.0/LICENSE
--rw-r--r--   0        0        0     2071 2024-03-25 20:06:31.587064 serverish-1.1.0/README.md
--rw-r--r--   0        0        0      734 2024-03-25 20:03:32.991281 serverish-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-14 11:40:48.850571 serverish-1.1.0/serverish/__init__.py
--rw-r--r--   0        0        0      195 2023-10-06 16:16:27.308992 serverish-1.1.0/serverish/base/__init__.py
--rw-r--r--   0        0        0     1014 2023-08-29 15:23:29.780464 serverish-1.1.0/serverish/base/asyncio_util_functions.py
--rw-r--r--   0        0        0     1097 2023-08-30 16:59:30.775614 serverish-1.1.0/serverish/base/collector.py
--rw-r--r--   0        0        0     2067 2024-01-17 01:43:34.127846 serverish-1.1.0/serverish/base/datetime.py
--rw-r--r--   0        0        0      757 2024-01-26 13:30:13.897409 serverish-1.1.0/serverish/base/exceptions.py
--rw-r--r--   0        0        0     1065 2023-10-04 13:16:20.864296 serverish-1.1.0/serverish/base/fifoset.py
--rw-r--r--   0        0        0     7799 2023-12-03 14:45:17.826296 serverish-1.1.0/serverish/base/hasstatuses.py
--rw-r--r--   0        0        0     1847 2023-08-24 16:43:19.251509 serverish-1.1.0/serverish/base/idmanger.py
--rw-r--r--   0        0        0     1154 2023-10-04 13:16:20.865134 serverish-1.1.0/serverish/base/manageable.py
--rw-r--r--   0        0        0      517 2023-08-20 23:50:45.634240 serverish-1.1.0/serverish/base/singleton.py
--rw-r--r--   0        0        0     4163 2023-12-28 20:14:15.020952 serverish-1.1.0/serverish/base/status.py
--rw-r--r--   0        0        0     6061 2024-02-29 14:54:27.059067 serverish-1.1.0/serverish/base/task_manager.py
--rw-r--r--   0        0        0      128 2023-08-20 23:53:42.978995 serverish-1.1.0/serverish/connection/__init__.py
--rw-r--r--   0        0        0     6251 2023-12-03 12:26:33.223741 serverish-1.1.0/serverish/connection/connection.py
--rw-r--r--   0        0        0     8690 2023-12-28 17:19:10.771028 serverish-1.1.0/serverish/connection/connection_jets.py
--rw-r--r--   0        0        0     7174 2024-01-03 18:36:11.829698 serverish-1.1.0/serverish/connection/connection_nats.py
--rw-r--r--   0        0        0      728 2023-11-15 19:25:32.794403 serverish-1.1.0/serverish/messenger/__init__.py
--rw-r--r--   0        0        0     1664 2023-11-15 19:25:32.790153 serverish-1.1.0/serverish/messenger/logging.py
--rw-r--r--   0        0        0    20222 2024-01-17 01:43:34.128627 serverish-1.1.0/serverish/messenger/messenger.py
--rw-r--r--   0        0        0     3929 2024-02-13 12:22:16.963070 serverish-1.1.0/serverish/messenger/msg_callback_sub.py
--rw-r--r--   0        0        0     6546 2024-03-25 19:37:37.645850 serverish-1.1.0/serverish/messenger/msg_journal_pub.py
--rw-r--r--   0        0        0     1565 2023-11-15 20:02:56.352311 serverish-1.1.0/serverish/messenger/msg_journal_read.py
--rw-r--r--   0        0        0    11758 2024-03-25 19:37:37.639171 serverish-1.1.0/serverish/messenger/msg_progress_pub.py
--rw-r--r--   0        0        0     2474 2024-02-14 11:40:48.851719 serverish-1.1.0/serverish/messenger/msg_progress_read.py
--rw-r--r--   0        0        0     3196 2024-03-25 20:08:38.850877 serverish-1.1.0/serverish/messenger/msg_publisher.py
--rw-r--r--   0        0        0    21509 2024-02-29 15:53:35.762974 serverish-1.1.0/serverish/messenger/msg_reader.py
--rw-r--r--   0        0        0     5773 2024-01-04 20:57:03.918907 serverish-1.1.0/serverish/messenger/msg_rpc_req.py
--rw-r--r--   0        0        0     4948 2024-01-04 20:58:35.654379 serverish-1.1.0/serverish/messenger/msg_rpc_resp.py
--rw-r--r--   0        0        0     1516 2024-03-25 20:08:38.854339 serverish-1.1.0/serverish/messenger/msg_single_pub.py
--rw-r--r--   0        0        0     3024 2023-09-07 15:53:00.478662 serverish-1.1.0/serverish/messenger/msg_single_read.py
--rw-r--r--   0        0        0     3566 2023-10-11 16:33:00.174783 serverish-1.1.0/serverish/messenger/msgvalidator.py
--rw-r--r--   0        0        0      681 2023-10-13 14:50:40.963824 serverish-1.1.0/serverish/schema/config.schema.json
--rw-r--r--   0        0        0       78 2023-10-06 16:16:27.319362 serverish-1.1.0/serverish/schema/default.schema.json
--rw-r--r--   0        0        0      295 2023-10-06 16:16:27.320015 serverish-1.1.0/serverish/schema/include/timestamp.schema.json
--rw-r--r--   0        0        0     1759 2023-11-22 05:15:27.646489 serverish-1.1.0/serverish/schema/journal.schema.json
--rw-r--r--   0        0        0     3170 2024-03-25 19:03:59.754872 serverish-1.1.0/serverish/schema/meta.schema.json
--rw-r--r--   0        0        0      669 2023-10-25 13:45:37.331834 serverish-1.1.0/serverish/schema/program_current_state.schema.json
--rw-r--r--   0        0        0      669 2023-10-25 13:45:37.332649 serverish-1.1.0/serverish/schema/program_state.schema.json
--rw-r--r--   0        0        0     1328 2024-02-14 11:40:48.852151 serverish-1.1.0/serverish/schema/progress.schema.json
--rw-r--r--   0        0        0      690 2023-11-24 03:32:42.295542 serverish-1.1.0/serverish/schema/telemetry.schema.json
--rw-r--r--   0        0        0     1434 2023-08-03 12:52:34.425476 serverish-1.1.0/serverish/slog.py
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 serverish-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-10-11 16:33:06.592284 serverish-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2344 2024-03-30 05:37:46.705600 serverish-1.1.1/README.md
+-rw-r--r--   0        0        0      734 2024-04-12 20:17:25.810672 serverish-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-14 11:40:48.850571 serverish-1.1.1/serverish/__init__.py
+-rw-r--r--   0        0        0      195 2023-10-06 16:16:27.308992 serverish-1.1.1/serverish/base/__init__.py
+-rw-r--r--   0        0        0     1014 2023-08-29 15:23:29.780464 serverish-1.1.1/serverish/base/asyncio_util_functions.py
+-rw-r--r--   0        0        0     1097 2023-08-30 16:59:30.775614 serverish-1.1.1/serverish/base/collector.py
+-rw-r--r--   0        0        0     2067 2024-01-17 01:43:34.127846 serverish-1.1.1/serverish/base/datetime.py
+-rw-r--r--   0        0        0      757 2024-01-26 13:30:13.897409 serverish-1.1.1/serverish/base/exceptions.py
+-rw-r--r--   0        0        0     1065 2023-10-04 13:16:20.864296 serverish-1.1.1/serverish/base/fifoset.py
+-rw-r--r--   0        0        0     7799 2023-12-03 14:45:17.826296 serverish-1.1.1/serverish/base/hasstatuses.py
+-rw-r--r--   0        0        0     1847 2023-08-24 16:43:19.251509 serverish-1.1.1/serverish/base/idmanger.py
+-rw-r--r--   0        0        0     1154 2023-10-04 13:16:20.865134 serverish-1.1.1/serverish/base/manageable.py
+-rw-r--r--   0        0        0      517 2023-08-20 23:50:45.634240 serverish-1.1.1/serverish/base/singleton.py
+-rw-r--r--   0        0        0     4163 2023-12-28 20:14:15.020952 serverish-1.1.1/serverish/base/status.py
+-rw-r--r--   0        0        0     6070 2024-04-12 20:13:06.473737 serverish-1.1.1/serverish/base/task_manager.py
+-rw-r--r--   0        0        0      128 2023-08-20 23:53:42.978995 serverish-1.1.1/serverish/connection/__init__.py
+-rw-r--r--   0        0        0     6251 2023-12-03 12:26:33.223741 serverish-1.1.1/serverish/connection/connection.py
+-rw-r--r--   0        0        0     8690 2023-12-28 17:19:10.771028 serverish-1.1.1/serverish/connection/connection_jets.py
+-rw-r--r--   0        0        0     7174 2024-01-03 18:36:11.829698 serverish-1.1.1/serverish/connection/connection_nats.py
+-rw-r--r--   0        0        0      728 2023-11-15 19:25:32.794403 serverish-1.1.1/serverish/messenger/__init__.py
+-rw-r--r--   0        0        0     1664 2023-11-15 19:25:32.790153 serverish-1.1.1/serverish/messenger/logging.py
+-rw-r--r--   0        0        0    20222 2024-01-17 01:43:34.128627 serverish-1.1.1/serverish/messenger/messenger.py
+-rw-r--r--   0        0        0     3929 2024-02-13 12:22:16.963070 serverish-1.1.1/serverish/messenger/msg_callback_sub.py
+-rw-r--r--   0        0        0     6546 2024-03-25 19:37:37.645850 serverish-1.1.1/serverish/messenger/msg_journal_pub.py
+-rw-r--r--   0        0        0     1565 2023-11-15 20:02:56.352311 serverish-1.1.1/serverish/messenger/msg_journal_read.py
+-rw-r--r--   0        0        0    11758 2024-03-25 19:37:37.639171 serverish-1.1.1/serverish/messenger/msg_progress_pub.py
+-rw-r--r--   0        0        0     2474 2024-02-14 11:40:48.851719 serverish-1.1.1/serverish/messenger/msg_progress_read.py
+-rw-r--r--   0        0        0     3196 2024-03-25 20:08:38.850877 serverish-1.1.1/serverish/messenger/msg_publisher.py
+-rw-r--r--   0        0        0    22125 2024-04-01 01:52:33.343588 serverish-1.1.1/serverish/messenger/msg_reader.py
+-rw-r--r--   0        0        0     5773 2024-01-04 20:57:03.918907 serverish-1.1.1/serverish/messenger/msg_rpc_req.py
+-rw-r--r--   0        0        0     4948 2024-01-04 20:58:35.654379 serverish-1.1.1/serverish/messenger/msg_rpc_resp.py
+-rw-r--r--   0        0        0     1516 2024-03-25 20:08:38.854339 serverish-1.1.1/serverish/messenger/msg_single_pub.py
+-rw-r--r--   0        0        0     3024 2023-09-07 15:53:00.478662 serverish-1.1.1/serverish/messenger/msg_single_read.py
+-rw-r--r--   0        0        0     3566 2023-10-11 16:33:00.174783 serverish-1.1.1/serverish/messenger/msgvalidator.py
+-rw-r--r--   0        0        0      681 2023-10-13 14:50:40.963824 serverish-1.1.1/serverish/schema/config.schema.json
+-rw-r--r--   0        0        0       78 2023-10-06 16:16:27.319362 serverish-1.1.1/serverish/schema/default.schema.json
+-rw-r--r--   0        0        0      295 2023-10-06 16:16:27.320015 serverish-1.1.1/serverish/schema/include/timestamp.schema.json
+-rw-r--r--   0        0        0     1759 2023-11-22 05:15:27.646489 serverish-1.1.1/serverish/schema/journal.schema.json
+-rw-r--r--   0        0        0     3170 2024-03-25 19:03:59.754872 serverish-1.1.1/serverish/schema/meta.schema.json
+-rw-r--r--   0        0        0      669 2023-10-25 13:45:37.331834 serverish-1.1.1/serverish/schema/program_current_state.schema.json
+-rw-r--r--   0        0        0      669 2023-10-25 13:45:37.332649 serverish-1.1.1/serverish/schema/program_state.schema.json
+-rw-r--r--   0        0        0     1328 2024-02-14 11:40:48.852151 serverish-1.1.1/serverish/schema/progress.schema.json
+-rw-r--r--   0        0        0      690 2023-11-24 03:32:42.295542 serverish-1.1.1/serverish/schema/telemetry.schema.json
+-rw-r--r--   0        0        0     1434 2023-08-03 12:52:34.425476 serverish-1.1.1/serverish/slog.py
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 serverish-1.1.1/PKG-INFO
```

### Comparing `serverish-1.1.0/LICENSE` & `serverish-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/README.md` & `serverish-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 * Singletons
 * Connections management and diagnostics
 * NATS based Messenger
 
 See [`doc` directory](doc/) for more documentation.
 
 ## Optional (extras) dependencies
+Following extras are available:
+* `messenger` - for using NATS based Messenger. Will install `nats-py` package.
+* `dns` - for using `aiodns` DNS resolver for connection status diagnostics, it's extracted as an extra dependency because it's not available on all platforms.
+
 In order to use Messenger, you have to add extra 'messenger' to your `project.toml` serveris dependency, e.g.:
 ```toml
 serverish = {git="https://github.com/AkondLab/serverish.git", extras=["messenger"], branch="master"}
 ```
 or specify dpendency with extras in the `pip` convention: `serverish[messenger]`.
 this will install `nats-py` package.
```

### Comparing `serverish-1.1.0/pyproject.toml` & `serverish-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "serverish"
-version = "1.1.0"
+version = "1.1.1"
 description = "helpers for server alike projects"
 authors = ["Mikołaj Kałuszyński", "MMME team"]
 readme = "README.md"
 repository = "https://github.com/AkondLab/serverish"
 include = ["serverish/schema/*"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-aiodns = {version="^3.1.1", optional=true}
+aiodns = {version="^3.2.0", optional=true}
 param = "^2.1.0"
 nats-py = { version = "^2.7.2", optional= true}
 jsonschema = "^4.20.0"
 
 [tool.poetry.extras]
 messenger = ["nats-py"]
 dns = ["aiodns"]
```

### Comparing `serverish-1.1.0/serverish/base/asyncio_util_functions.py` & `serverish-1.1.1/serverish/base/asyncio_util_functions.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/collector.py` & `serverish-1.1.1/serverish/base/collector.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/datetime.py` & `serverish-1.1.1/serverish/base/datetime.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/exceptions.py` & `serverish-1.1.1/serverish/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/fifoset.py` & `serverish-1.1.1/serverish/base/fifoset.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/hasstatuses.py` & `serverish-1.1.1/serverish/base/hasstatuses.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/idmanger.py` & `serverish-1.1.1/serverish/base/idmanger.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/manageable.py` & `serverish-1.1.1/serverish/base/manageable.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/singleton.py` & `serverish-1.1.1/serverish/base/singleton.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/status.py` & `serverish-1.1.1/serverish/base/status.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/base/task_manager.py` & `serverish-1.1.1/serverish/base/task_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,26 +34,26 @@
     async def start(self):
         """Runs the task. Async - preferred - way"""
         self.start_sync()
 
     def start_sync(self):
         """Runs the task. Sync method"""
         def done_cb(task):
-            e = task.exception()
-            if e is not None:
-                if isinstance(e, asyncio.CancelledError):
-                    logger.debug(f'Task {self.name} canceled')
-                    self.set_status('running', Status.new_na(msg='Task canceled'))
-                else:
+            try:
+                e = task.exception()
+            except asyncio.CancelledError:
+                logger.debug(f'Task {self.name} canceled')
+                self.set_status('running', Status.new_na(msg='Task canceled'))
+            else:
+                if e is not None:
                     logger.error(f'Task {self.name} failed: {task.exception()}', exc_info=task.exception())
                     self.set_status('running', Status.new_fail(msg=f'Task failed: {task.exception()}'))
-            else:
-                logger.debug(f'Task {self.name} done')
-                self.set_status('running', Status.new_na(msg='Task finished'))
-
+                else:
+                    logger.debug(f'Task {self.name} done')
+                    self.set_status('running', Status.new_na(msg='Task finished'))
             self.remove_parent()
 
         self.task = asyncio.create_task(self.coro, name=self.name)
         self.task.add_done_callback(done_cb)
 
     def cancel(self):
         """Cancels the task"""
```

### Comparing `serverish-1.1.0/serverish/connection/connection.py` & `serverish-1.1.1/serverish/connection/connection.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/connection/connection_jets.py` & `serverish-1.1.1/serverish/connection/connection_jets.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/connection/connection_nats.py` & `serverish-1.1.1/serverish/connection/connection_nats.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/__init__.py` & `serverish-1.1.1/serverish/messenger/__init__.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/logging.py` & `serverish-1.1.1/serverish/messenger/logging.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/messenger.py` & `serverish-1.1.1/serverish/messenger/messenger.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_callback_sub.py` & `serverish-1.1.1/serverish/messenger/msg_callback_sub.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_journal_pub.py` & `serverish-1.1.1/serverish/messenger/msg_journal_pub.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_journal_read.py` & `serverish-1.1.1/serverish/messenger/msg_journal_read.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_progress_pub.py` & `serverish-1.1.1/serverish/messenger/msg_progress_pub.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_progress_read.py` & `serverish-1.1.1/serverish/messenger/msg_progress_read.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_publisher.py` & `serverish-1.1.1/serverish/messenger/msg_publisher.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_reader.py` & `serverish-1.1.1/serverish/messenger/msg_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,25 @@
                 timeout = min(0.2 + n/5, 5)  # start fast and slow down to 5s
                 batch = 1 if n > 1 else 100
                 log.debug(f"Pulling {batch} in {timeout}s from {self}")
                 self.pull_batch = deque(await self.pull_subscription.fetch(batch=batch, timeout=timeout))
                 log.debug(f"Pulled {len(self.pull_batch)} messages from {self}")
             except nats.errors.TimeoutError:
                 pass
+            except nats.errors.ConnectionClosedError:
+                if self.on_connection_close == 'RAISE':
+                    log.warning(f'Connection closed, raising exception on {self}')
+                    raise
+                elif self.on_connection_close == 'FINISH':
+                    log.warning(f'Connection closed, finishing iteration on {self}')
+                    self._stop.set()
+                else:
+                    assert self.on_connection_close == 'WAIT'
+                    log.warning(f'Connection closed, waiting for reconnect on {self}')
+                    await asyncio.sleep(1.0)
             n += 1
 
         self._emptied.clear()
         bmsg = self.pull_batch.popleft()
         await bmsg.ack()
         data, meta = self.messenger.unpack_nats_msg(bmsg)
         self.messenger.log_msg_trace(data, meta, f"SUB PULL iteration from {self.subject}")
```

### Comparing `serverish-1.1.0/serverish/messenger/msg_rpc_req.py` & `serverish-1.1.1/serverish/messenger/msg_rpc_req.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_rpc_resp.py` & `serverish-1.1.1/serverish/messenger/msg_rpc_resp.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_single_pub.py` & `serverish-1.1.1/serverish/messenger/msg_single_pub.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msg_single_read.py` & `serverish-1.1.1/serverish/messenger/msg_single_read.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/messenger/msgvalidator.py` & `serverish-1.1.1/serverish/messenger/msgvalidator.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/schema/config.schema.json` & `serverish-1.1.1/serverish/schema/config.schema.json`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/schema/journal.schema.json` & `serverish-1.1.1/serverish/schema/journal.schema.json`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/schema/meta.schema.json` & `serverish-1.1.1/serverish/schema/meta.schema.json`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/schema/program_current_state.schema.json` & `serverish-1.1.1/serverish/schema/program_current_state.schema.json`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/schema/program_state.schema.json` & `serverish-1.1.1/serverish/schema/program_state.schema.json`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/schema/progress.schema.json` & `serverish-1.1.1/serverish/schema/progress.schema.json`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/schema/telemetry.schema.json` & `serverish-1.1.1/serverish/schema/telemetry.schema.json`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/serverish/slog.py` & `serverish-1.1.1/serverish/slog.py`

 * *Files identical despite different names*

### Comparing `serverish-1.1.0/PKG-INFO` & `serverish-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: serverish
-Version: 1.1.0
+Version: 1.1.1
 Summary: helpers for server alike projects
 Home-page: https://github.com/AkondLab/serverish
 Author: Mikołaj Kałuszyński
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dns
 Provides-Extra: messenger
-Requires-Dist: aiodns (>=3.1.1,<4.0.0) ; extra == "dns"
+Requires-Dist: aiodns (>=3.2.0,<4.0.0) ; extra == "dns"
 Requires-Dist: jsonschema (>=4.20.0,<5.0.0)
 Requires-Dist: nats-py (>=2.7.2,<3.0.0) ; extra == "messenger"
 Requires-Dist: param (>=2.1.0,<3.0.0)
 Project-URL: Repository, https://github.com/AkondLab/serverish
 Description-Content-Type: text/markdown
 
 # serverish - helpers for server alike projects
@@ -28,14 +28,18 @@
 * Singletons
 * Connections management and diagnostics
 * NATS based Messenger
 
 See [`doc` directory](doc/) for more documentation.
 
 ## Optional (extras) dependencies
+Following extras are available:
+* `messenger` - for using NATS based Messenger. Will install `nats-py` package.
+* `dns` - for using `aiodns` DNS resolver for connection status diagnostics, it's extracted as an extra dependency because it's not available on all platforms.
+
 In order to use Messenger, you have to add extra 'messenger' to your `project.toml` serveris dependency, e.g.:
 ```toml
 serverish = {git="https://github.com/AkondLab/serverish.git", extras=["messenger"], branch="master"}
 ```
 or specify dpendency with extras in the `pip` convention: `serverish[messenger]`.
 this will install `nats-py` package.
```

