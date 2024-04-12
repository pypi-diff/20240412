# Comparing `tmp/pyprland-2.2.4.tar.gz` & `tmp/pyprland-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.2.4.tar", max compression
+gzip compressed data, was "pyprland-2.2.5.tar", max compression
```

## Comparing `pyprland-2.2.4.tar` & `pyprland-2.2.5.tar`

### file list

```diff
@@ -1,34 +1,38 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.4/LICENSE
--rw-r--r--   0        0        0     4119 2024-04-08 17:57:27.722353 pyprland-2.2.4/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.4/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.4/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.4/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.4/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.4/pyprland/adapters/units.py
--rwxr-xr-x   0        0        0    16372 2024-04-09 21:30:26.098920 pyprland-2.2.4/pyprland/command.py
--rwxr-xr-x   0        0        0    15808 2024-04-05 22:08:40.562254 pyprland-2.2.4/pyprland/command.py.orig
--rw-r--r--   0        0        0     7410 2024-04-09 21:29:20.927222 pyprland-2.2.4/pyprland/common.py
--rw-r--r--   0        0        0     6555 2024-04-09 21:02:15.456507 pyprland-2.2.4/pyprland/ipc.py
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.4/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.4/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.4/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.4/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.4/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.4/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.4/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.4/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.4/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.4/pyprland/plugins/monitors.py.orig
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.4/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.4/pyprland/plugins/nohup.out
--rw-r--r--   0        0        0     1309 2024-04-06 13:35:25.146759 pyprland-2.2.4/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    35948 2024-04-09 21:16:20.505075 pyprland-2.2.4/pyprland/plugins/scratchpads.py
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.4/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.4/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     3983 2024-04-09 21:03:19.309538 pyprland-2.2.4/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.4/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.4/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     4003 2024-04-09 18:24:41.796795 pyprland-2.2.4/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.4/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0      725 2024-04-09 21:30:26.088919 pyprland-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     4658 1970-01-01 00:00:00.000000 pyprland-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.5/LICENSE
+-rw-r--r--   0        0        0     4380 2024-04-12 19:57:34.959057 pyprland-2.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.5/pyprland/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.5/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.5/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.5/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.5/pyprland/adapters/units.py
+-rwxr-xr-x   0        0        0    16372 2024-04-12 20:05:41.571463 pyprland-2.2.5/pyprland/command.py
+-rwxr-xr-x   0        0        0    15808 2024-04-05 22:08:40.562254 pyprland-2.2.5/pyprland/command.py.orig
+-rw-r--r--   0        0        0     7410 2024-04-09 21:29:20.927222 pyprland-2.2.5/pyprland/common.py
+-rw-r--r--   0        0        0     7197 2024-04-12 17:07:08.504043 pyprland-2.2.5/pyprland/ipc.py
+-rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.5/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.5/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.5/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.5/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.5/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.5/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.5/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.5/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.5/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.5/pyprland/plugins/monitors.py.orig
+-rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.5/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.5/pyprland/plugins/nohup.out
+-rw-r--r--   0        0        0     1515 2024-04-11 16:23:54.463967 pyprland-2.2.5/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    26125 2024-04-12 17:49:11.523202 pyprland-2.2.5/pyprland/plugins/scratchpads/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-12 17:24:50.007112 pyprland-2.2.5/pyprland/plugins/scratchpads/animations.py
+-rw-r--r--   0        0        0     2106 2024-04-12 17:23:41.858277 pyprland-2.2.5/pyprland/plugins/scratchpads/helpers.py
+-rw-r--r--   0        0        0     3436 2024-04-12 17:21:22.436949 pyprland-2.2.5/pyprland/plugins/scratchpads/lookup.py
+-rw-r--r--   0        0        0     4136 2024-04-12 17:19:16.255742 pyprland-2.2.5/pyprland/plugins/scratchpads/objects.py
+-rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.5/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.5/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     3983 2024-04-09 21:03:19.309538 pyprland-2.2.5/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.5/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.5/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     5071 2024-04-12 19:31:07.396989 pyprland-2.2.5/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.5/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0      725 2024-04-12 20:05:41.561462 pyprland-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 pyprland-2.2.5/PKG-INFO
```

### Comparing `pyprland-2.2.4/LICENSE` & `pyprland-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/README.md` & `pyprland-2.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 - Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues).
 - Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki)
 
 and if you have coding skills you can also
 
 - Enhance test coverage in our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests).
-- Write new plugins
+- Propose & write new plugins or enhancements
 
 ## Dependencies
 
 - **Hyprland** >= 0.37
 - **Python** >= 3.11
     - **aiofiles**
 
@@ -44,14 +44,17 @@
 
 > [!note]
 > Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 ### 2.2
 
 - Added [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/hyprland-community/pyprland/wiki/system_notifier) plugins.
+- Refactor in 2.2.5
+  - updated the syntax for [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers)
+  - deprecated `class_match` in [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
 
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) plugin improvements.
 
 ### 2.0
```

#### html2text {}

```diff
@@ -24,24 +24,27 @@
 www.w3schools.com/js/js_json_intro.asp)) ## Contributing Check out the
 [creating a pull request](https://docs.github.com/fr/pull-requests/
 collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-
 requests/creating-a-pull-request) document for guidance. - Report bugs or
 propose features [here](https://github.com/hyprland-community/pyprland/issues).
 - Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki) and
 if you have coding skills you can also - Enhance test coverage in our [tests]
-(https://github.com/hyprland-community/pyprland/tree/main/tests). - Write new
-plugins ## Dependencies - **Hyprland** >= 0.37 - **Python** >= 3.11 -
-**aiofiles** ## Latest major changes > [!note] > Check the [Releases change
-log](https://github.com/hyprland-community/pyprland/releases) for more
-information ### 2.2 - Added [wallpapers](https://github.com/hyprland-community/
-pyprland/wiki/wallpapers) and [system_notifier](https://github.com/hyprland-
-community/pyprland/wiki/system_notifier) plugins. ### 2.1 - Requires Hyprland
->= 0.37 - [Monitors](https://github.com/hyprland-community/pyprland/wiki/
-monitors) plugin improvements. ### 2.0 - New dependency: [aiofiles](https://
-pypi.org/project/aiofiles/) - Added [hysteresis](https://github.com/hyprland-
+(https://github.com/hyprland-community/pyprland/tree/main/tests). - Propose &
+write new plugins or enhancements ## Dependencies - **Hyprland** >= 0.37 -
+**Python** >= 3.11 - **aiofiles** ## Latest major changes > [!note] > Check the
+[Releases change log](https://github.com/hyprland-community/pyprland/releases)
+for more information ### 2.2 - Added [wallpapers](https://github.com/hyprland-
+community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/
+hyprland-community/pyprland/wiki/system_notifier) plugins. - Refactor in 2.2.5
+- updated the syntax for [wallpapers](https://github.com/hyprland-community/
+pyprland/wiki/wallpapers) - deprecated `class_match` in [scratchpads](https://
+github.com/hyprland-community/pyprland/wiki/scratchpads) ### 2.1 - Requires
+Hyprland >= 0.37 - [Monitors](https://github.com/hyprland-community/pyprland/
+wiki/monitors) plugin improvements. ### 2.0 - New dependency: [aiofiles](https:
+//pypi.org/project/aiofiles/) - Added [hysteresis](https://github.com/hyprland-
 community/pyprland/wiki/scratchpads#hysteresis-optional) support for
 [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads).
 ### 1.10 - New [fetch_client_menu](https://github.com/hyprland-community/
 pyprland/wiki/fetch_client_menu) and [shortcuts_menu](https://github.com/
 hyprland-community/pyprland/wiki/shortcuts_menu) plugins. ### 1.9 - Introduced
 [shortcuts_menu](https://github.com/hyprland-community/pyprland/wiki/
 shortcuts_menu) plugin. ### 1.8 - Requires Hyprland >= 0.30 - Added
```

### Comparing `pyprland-2.2.4/pyprland/adapters/menus.py` & `pyprland-2.2.5/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/adapters/units.py` & `pyprland-2.2.5/pyprland/adapters/units.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/command.py` & `pyprland-2.2.5/pyprland/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
 
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print("2.2.4")  # Automatically updated version
+        print("2.2.5")  # Automatically updated version
         return
 
     if sys.argv[1] == "edit":
         editor = os.environ.get("EDITOR", os.environ.get("VISUAL", "vi"))
         filename = os.path.expanduser(CONFIG_FILE)
         run_interactive_program(f'{editor} "{filename}"')
         sys.argv[1] = "reload"
```

### Comparing `pyprland-2.2.4/pyprland/command.py.orig` & `pyprland-2.2.5/pyprland/command.py.orig`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/common.py` & `pyprland-2.2.5/pyprland/common.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/ipc.py` & `pyprland-2.2.5/pyprland/ipc.py`

 * *Files 17% similar despite different names*

```diff
@@ -176,45 +176,58 @@
     for monitor in await hyprctlJSON("monitors", logger=logger):
         assert isinstance(monitor, dict)
         if match_fn(monitor):
             return monitor
     raise RuntimeError("no focused monitor")
 
 
-async def get_client_props(
-    addr: str | None = None, pid: int | None = None, cls: str | None = None, logger=None
-):
+async def get_client_props(logger=None, match_fn=None, **kw):
     """
-    Returns client properties
+    Returns the properties of a client that matches the given `match_fn` (or default to equality) given the keyword arguments
+
+    Eg.
+        # will return the properties of the client with address "0x1234"
+        get_client_props(logger, addr="0x1234")
+
+        # will return the properties of the client with initialClass containing "fooBar"
+        get_client_props(logger, match_fn=lambda x, y: y in x), initialClass="fooBar")
 
     Args:
-        addr (str): address of the client (includes "0x" prefix)
-        pid (int): PID of the client
-        cls (str): class of the client
+
         logger: logger to use in case of error
+        match_fn: function to match the client properties, takes 2 arguments (client_value, config_value)
+
+        Any other keyword argument will be used to match the client properties. Only one keyword argument is allowed.
+        `addr` aliases `address` and `cls` aliases `class`
+
+        Note: the address of the client must include the "0x" prefix
     """
-    assert addr or pid or cls
+    assert kw
 
-    prop_value: int | str
+    addr = kw.get("addr")
+    klass = kw.get("cls")
 
     if addr:
         assert len(addr) > 2, "Client address is invalid"
         prop_name = "address"
         prop_value = addr
-    elif cls:
+    elif klass:
         prop_name = "class"
-        prop_value = cls
+        prop_value = klass
     else:
-        assert pid, "Client pid is invalid"
-        prop_name = "pid"
-        prop_value = pid
+        prop_name, prop_value = next(iter(kw.items()))
+
+    if match_fn is None:
+
+        def match_fn(value1, value2):
+            return value1 == value2
 
     for client in await hyprctlJSON("clients", logger=logger):
         assert isinstance(client, dict)
-        if client.get(prop_name) == prop_value:
+        if match_fn(client.get(prop_name), prop_value):
             return client
 
 
 def init():
     "initialize logging"
     global log
     log = get_logger("ipc")
```

### Comparing `pyprland-2.2.4/pyprland/plugins/expose.py` & `pyprland-2.2.5/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.2.5/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/interface.py` & `pyprland-2.2.5/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/layout_center.py` & `pyprland-2.2.5/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/lost_windows.py` & `pyprland-2.2.5/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/magnify.py` & `pyprland-2.2.5/pyprland/plugins/magnify.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/monitors.py` & `pyprland-2.2.5/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/monitors.py.orig` & `pyprland-2.2.5/pyprland/plugins/monitors.py.orig`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/monitors_v0.py` & `pyprland-2.2.5/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/pyprland.py` & `pyprland-2.2.5/pyprland/plugins/pyprland.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,20 +18,23 @@
 
     async def on_reload(self):
         state.variables = self.config.get("variables", {})
 
     async def event_activewindowv2(self, addr):
         "keep track of focused client"
         state.active_window = "0x" + addr
+        self.log.debug("active_window = %s", state.active_window)
 
     async def event_workspace(self, wrkspace):
         "track the active workspace"
         state.active_workspace = wrkspace
+        self.log.debug("active_workspace = %s", state.active_workspace)
 
     async def event_focusedmon(self, mon):
         "track the active workspace"
         state.active_monitor, state.active_workspace = mon.rsplit(",", 1)
+        self.log.debug("active_monitor = %s", state.active_monitor)
 
     def set_commands(self, **cmd_map):
         "Set some commands, made available as run_`name` methods"
         for name, fn in cmd_map.items():
             setattr(self, f"run_{name}", fn)
```

### Comparing `pyprland-2.2.4/pyprland/plugins/scratchpads.py` & `pyprland-2.2.5/pyprland/plugins/scratchpads/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,343 +1,31 @@
 " Scratchpads addon "
-import os
 import time
-import logging
 import asyncio
-from typing import Any, cast, Callable
 from functools import partial
-from collections import defaultdict
 
-from aiofiles import os as aios
-from aiofiles import open as aiopen
-
-from ..ipc import notify_error, get_client_props, get_focused_monitor_props
-from .interface import Plugin
-from ..common import state, CastBoolMixin, apply_variables
-from ..adapters.units import convert_coords, convert_monitor_dimension
+from ...ipc import notify_error, get_client_props, get_focused_monitor_props
+from ..interface import Plugin
+from ...common import state, CastBoolMixin, apply_variables
+from ...adapters.units import convert_coords, convert_monitor_dimension
+
+from .animations import Animations
+from .objects import Scratch
+from .lookup import ScratchDB
+from .helpers import (
+    get_active_space_identifier,
+    get_all_space_identifiers,
+    get_match_fn,
+)
 
 AFTER_SHOW_INHIBITION = 0.3  # 300ms of ignorance after a show
 DEFAULT_MARGIN = 60  # in pixels
 DEFAULT_HIDE_DELAY = 0.2
 DEFAULT_HYSTERESIS = 0.4  # In seconds
 
-# Helper functions {{{
-
-
-def get_active_space_identifier():
-    "Returns a unique object for the workspace + monitor combination"
-    return (state.active_workspace, state.active_monitor)
-
-
-async def get_all_space_identifiers(monitors):
-    "Returns a list of every space identifiers (workspace + monitor) on active screens"
-    return [
-        (monitor["activeWorkspace"]["name"], monitor["name"]) for monitor in monitors
-    ]
-
-
-# }}}
-
-
-class Animations:  # {{{
-    "Animation store"
-
-    @staticmethod
-    def fromtop(monitor, client, client_uid, margin):
-        "Slide from/to top"
-        scale = float(monitor["scale"])
-        mon_x = monitor["x"]
-        mon_y = monitor["y"]
-        mon_width = int(monitor["width"] / scale)
-
-        client_width = client["size"][0]
-        margin_x = int((mon_width - client_width) / 2) + mon_x
-
-        corrected_margin = convert_monitor_dimension(margin, monitor["height"], monitor)
-
-        return (
-            f"movewindowpixel exact {margin_x} {mon_y + corrected_margin},{client_uid}"
-        )
-
-    @staticmethod
-    def frombottom(monitor, client, client_uid, margin):
-        "Slide from/to bottom"
-        scale = float(monitor["scale"])
-        mon_x = monitor["x"]
-        mon_y = monitor["y"]
-        mon_width = int(monitor["width"] / scale)
-        mon_height = int(monitor["height"] / scale)
-
-        client_width = client["size"][0]
-        client_height = client["size"][1]
-        margin_x = int((mon_width - client_width) / 2) + mon_x
-
-        corrected_margin = convert_monitor_dimension(margin, monitor["height"], monitor)
-
-        return f"movewindowpixel exact {margin_x} {mon_y + mon_height - client_height - corrected_margin},{client_uid}"
-
-    @staticmethod
-    def fromleft(monitor, client, client_uid, margin):
-        "Slide from/to left"
-        scale = float(monitor["scale"])
-        mon_x = monitor["x"]
-        mon_y = monitor["y"]
-        mon_height = int(monitor["height"] / scale)
-
-        client_height = client["size"][1]
-        margin_y = int((mon_height - client_height) / 2) + mon_y
-
-        corrected_margin = convert_monitor_dimension(margin, monitor["width"], monitor)
-
-        return (
-            f"movewindowpixel exact {corrected_margin + mon_x} {margin_y},{client_uid}"
-        )
-
-    @staticmethod
-    def fromright(monitor, client, client_uid, margin):
-        "Slide from/to right"
-        scale = float(monitor["scale"])
-        mon_x = monitor["x"]
-        mon_y = monitor["y"]
-        mon_width = int(monitor["width"] / scale)
-        mon_height = int(monitor["height"] / scale)
-
-        client_width = client["size"][0]
-        client_height = client["size"][1]
-        margin_y = int((mon_height - client_height) / 2) + mon_y
-
-        corrected_margin = convert_monitor_dimension(margin, monitor["width"], monitor)
-
-        return f"movewindowpixel exact {mon_width - client_width - corrected_margin + mon_x } {margin_y},{client_uid}"
-
-
-# }}}
-
-
-class OverridableConfig:
-    "A `dict`-like object allowing per-monitor overrides"
-
-    def __init__(self, ref, monitor_override):
-        self.ref = ref
-        self.mon_override = monitor_override
-
-    def __setitem__(self, name, value):
-        self.ref[name] = value
-
-    def __getitem__(self, name):
-        override = self.mon_override.get(state.active_monitor, {})
-        if name in override:
-            return override[name]
-        return self.ref[name]
-
-    def get(self, name, default=None):
-        "get the attribute `name`"
-        try:
-            return self[name]
-        except KeyError:
-            return default
-
-    def __str__(self):
-        return f"{self.ref} {self.mon_override}"
-
-
-class Scratch(CastBoolMixin):  # {{{
-    "A scratchpad state including configuration & client state"
-    log = logging.getLogger("scratch")
-    get_client_props: Callable
-
-    def __init__(self, uid, opts):
-        self.uid = uid
-        self.pid = 0
-        if self.cast_bool(opts.get("preserve_aspect")):
-            opts["lazy"] = True
-        if not opts.get("process_tracking", True):
-            opts["lazy"] = True
-            opts["class_match"] = True
-        self.conf = OverridableConfig(opts, opts.get("monitor", {}))
-        self.visible = False
-        self.client_info = {}
-        self.should_hide = False
-        self.initialized = False
-        self.meta = {}
-        self.space_identifier = None
-        self.monitor = ""
-
-    async def initialize(self, ex):
-        "Initialize the scratchpad"
-        if self.initialized:
-            return
-        self.initialized = True
-        await self.updateClientInfo()
-        await ex.hyprctl(
-            f"movetoworkspacesilent special:scratch_{self.uid},address:{self.full_address}"
-        )
-
-    async def isAlive(self) -> bool:
-        "is the process running ?"
-        if self.cast_bool(self.conf.get("process_tracking"), True):
-            path = f"/proc/{self.pid}"
-            if await aios.path.exists(path):
-                async with aiopen(
-                    os.path.join(path, "status"), mode="r", encoding="utf-8"
-                ) as f:
-                    for line in await f.readlines():
-                        if line.startswith("State"):
-                            proc_state = line.split()[1]
-                            return (
-                                proc_state not in "ZX"
-                            )  # not "Z (zombie)"or "X (dead)"
-        else:
-            if getattr(self, "bogus_pid", False):
-                return bool(await self.get_client_props(cls=self.conf["class"]))
-            return False
-
-        return False
-
-    def reset(self, pid: int) -> None:
-        "clear the object"
-        self.pid = pid
-        self.visible = False
-        self.client_info = {}
-        self.initialized = False
-
-    @property
-    def address(self) -> str:
-        "Returns the client address"
-        return str(self.client_info.get("address", ""))[2:]
-
-    @property
-    def full_address(self) -> str:
-        "Returns the client address"
-        return cast(str, self.client_info.get("address", ""))
-
-    async def updateClientInfo(self, client_info=None) -> None:
-        "update the internal client info property, if not provided, refresh based on the current address"
-        if client_info is None:
-            client_info = await self.get_client_props(addr=self.full_address)
-        if not isinstance(client_info, dict):
-            self.log.error(
-                "client_info of %s must be a dict: %s", self.address, client_info
-            )
-            raise AssertionError(f"Not a dict: {client_info}")
-
-        self.client_info.update(client_info)
-
-    def __str__(self):
-        return f"{self.uid} {self.address} : {self.client_info} / {self.conf}"
-
-
-# }}}
-
-
-class ScratchDB:  # {{{
-    """Single storage for every Scratch allowing a boring lookup & update API"""
-
-    _by_addr: dict[str, Scratch] = {}
-    _by_pid: dict[int, Scratch] = {}
-    _by_name: dict[str, Scratch] = {}
-    _states: defaultdict[str, set[Scratch]] = defaultdict(set)
-
-    # State management {{{
-    def getByState(self, status: str):
-        "get a set of `Scratch` being in `status`"
-        return self._states[status]
-
-    def hasState(self, scratch: Scratch, status: str):
-        "Returns true if `scratch` has state `status`"
-        return scratch in self._states[status]
-
-    def setState(self, scratch: Scratch, status: str):
-        "Sets `scratch` in the provided status"
-        self._states[status].add(scratch)
-
-    def clearState(self, scratch: Scratch, status: str):
-        "Unsets the the provided status from the scratch"
-        self._states[status].remove(scratch)
-
-    # }}}
-
-    # dict-like {{{
-    def __iter__(self):
-        "return all Scratch name"
-        return iter(self._by_name.keys())
-
-    def values(self):
-        "returns every Scratch"
-        return self._by_name.values()
-
-    def items(self):
-        "return an iterable list of (name, Scratch)"
-        return self._by_name.items()
-
-    # }}}
-
-    def reset(self, scratch: Scratch):
-        "clears registered address & pid"
-        if scratch.address in self._by_addr:
-            del self._by_addr[scratch.address]
-        if scratch.pid in self._by_pid:
-            del self._by_pid[scratch.pid]
-
-    def clear(self, name=None, pid=None, addr=None):
-        "clears the index by name, pid or address"
-        # {{{
-
-        assert any((name, pid, addr))
-        if name is not None and name in self._by_name:
-            del self._by_name[name]
-        if pid is not None and pid in self._by_pid:
-            del self._by_pid[pid]
-        if addr is not None and addr in self._by_addr:
-            del self._by_addr[addr]
-        # }}}
-
-    def register(self, scratch: Scratch, name=None, pid=None, addr=None):
-        "set the Scratch index by name, pid or address, or update every index of only `scratch` is provided"
-        # {{{
-        if not any((name, pid, addr)):
-            self._by_name[scratch.uid] = scratch
-            self._by_pid[scratch.pid] = scratch
-            self._by_addr[scratch.address] = scratch
-        else:
-            if name is not None:
-                d: dict[Any, Scratch] = cast(dict[str, Scratch], self._by_name)
-                v = name
-            elif pid is not None:
-                d = self._by_pid
-                v = pid
-            elif addr is not None:
-                d = self._by_addr
-                v = addr
-            d[v] = scratch
-        # }}}
-
-    def get(self, name=None, pid=None, addr=None) -> Scratch | None:
-        "return the Scratch matching given name, pid or address"
-        # {{{
-        assert 1 == len(list(filter(bool, (name, pid, addr)))), (
-            name,
-            pid,
-            addr,
-        )
-        if name is not None:
-            d: dict[Any, Scratch] = self._by_name
-            v = name
-        elif pid is not None:
-            d = self._by_pid
-            v = pid
-        elif addr is not None:
-            d = self._by_addr
-            v = addr
-        return d.get(v)
-        # }}}
-
-
-# }}}
-
 
 class Extension(CastBoolMixin, Plugin):  # pylint: disable=missing-class-docstring {{{
     procs: dict[str, asyncio.subprocess.Process] = {}  # pylint: disable=no-member
     scratches = ScratchDB()
 
     focused_window_tracking: dict[str, str] = {}
 
@@ -380,29 +68,28 @@
         scratches = {
             name: Scratch(name, options) for name, options in self.config.items()
         }
 
         scratches_to_spawn = set()
         for name in scratches:
             scratch = self.scratches.get(name)
-            if scratch:
-                # if existing scratch exists, overrides the conf object
-                scratch.conf = scratches[name].conf
+            if scratch:  # if existing scratch exists, overrides the conf object
+                scratch.set_config(scratches[name].conf)
             else:
                 # else register it
                 self.scratches.register(scratches[name], name)
                 is_lazy = self.cast_bool(scratches[name].conf.get("lazy"), False)
                 if not is_lazy:
                     scratches_to_spawn.add(name)
 
         for name in scratches_to_spawn:
             if await self.ensure_alive(name):
                 scratch = self.scratches.get(name)
                 assert scratch
-                scratch.should_hide = True
+                scratch.meta["should_hide"] = True
             else:
                 self.log.error("Failure starting %s", name)
 
         for scratch in list(self.scratches.getByState("configured")):
             assert scratch
             self.scratches.clearState(scratch, "configured")
 
@@ -421,47 +108,48 @@
             width, height = convert_coords(scratch.conf.get("size", "80% 80%"), monitor)
 
             ipc_commands = [
                 f"windowrule float,^({defined_class})$",
                 f"windowrule workspace special:scratch_{scratch.uid} silent,^({defined_class})$",
             ]
 
-            if not self.cast_bool(scratch.conf.get("preserve_aspect")):
-                if animation_type:
-                    margin_x = (monitor["width"] - width) // 2
-                    margin_y = (monitor["height"] - height) // 2
-
-                    t_pos = {
-                        "fromtop": f"{margin_x} -200%",
-                        "frombottom": f"{margin_x} 200%",
-                        "fromright": f"200% {margin_y}",
-                        "fromleft": f"-200% {margin_y}",
-                    }[animation_type]
-                    ipc_commands.append(f"windowrule move {t_pos},^({defined_class})$")
+            if animation_type:
+                margin_x = (monitor["width"] - width) // 2
+                margin_y = (monitor["height"] - height) // 2
 
-                ipc_commands.append(
-                    f"windowrule size {width} {height},^({defined_class})$"
-                )
+                t_pos = {
+                    "fromtop": f"{margin_x} -200%",
+                    "frombottom": f"{margin_x} 200%",
+                    "fromright": f"200% {margin_y}",
+                    "fromleft": f"-200% {margin_y}",
+                }[animation_type]
+                ipc_commands.append(f"windowrule move {t_pos},^({defined_class})$")
+
+            ipc_commands.append(f"windowrule size {width} {height},^({defined_class})$")
 
             await self.hyprctl(ipc_commands, "keyword")
 
     async def __wait_for_client(self, item, use_proc=True) -> bool:
         """Waits for a client to be up and running
-        if `class_match` is enabled, will use the class, else the process's PID will be used.
+        if `match_by=` is used, will use the match criteria, else the process's PID will be used.
         """
         self.log.info("==> Wait for %s spawning", item.uid)
         interval_range = [0.1] * 10 + [0.2] * 20 + [0.5] * 15
         for interval in interval_range:
             await asyncio.sleep(interval)
             is_alive = await item.isAlive()
 
             # skips the checks if the process isn't started (just wait)
             if is_alive or not use_proc:
-                if self.cast_bool(item.conf.get("class_match")):
-                    info = await self.get_client_props(cls=item.conf.get("class"))
+                match_by = item.conf.get("match_by", "pid")
+                if match_by != "pid":
+                    info = await self.get_client_props(
+                        match_fn=get_match_fn(match_by, item.conf[match_by]),
+                        **{match_by: item.conf[match_by]},
+                    )
                 else:
                     info = await self.get_client_props(pid=item.pid)
                 if info:
                     await item.updateClientInfo(info)
                     self.log.info(
                         "=> %s client (proc:%s, addr:%s) detected on time",
                         item.uid,
@@ -471,25 +159,25 @@
                     self.scratches.register(item)
                     self.scratches.clearState(item, "respawned")
                     return True
             if use_proc and not is_alive:
                 return False
         return False
 
-    async def _start_scratch_classbased(self, item) -> bool:
+    async def _start_scratch_nopid(self, item) -> bool:
         "Ensure alive, PWA version"
         uid = item.uid
-        started = getattr(item, "bogus_pid", False)
+        started = "nopid" in item.meta
         if not await item.isAlive():
             started = False
         if not started:
             self.scratches.reset(item)
             await self.start_scratch_command(uid)
             r = await self.__wait_for_client(item, use_proc=False)
-            item.bogus_pid = True
+            item.meta["nopid"] = r
             return r
         return True
 
     async def _start_scratch(self, item):
         "Ensure alive, standard version"
         uid = item.uid
         if uid in self.procs:
@@ -528,15 +216,15 @@
             if not await item.isAlive():
                 self.log.info("%s is not running, starting...", uid)
                 if not await self._start_scratch(item):
                     await notify_error(f'Failed to show scratch "{item.uid}"')
                     return False
             return True
 
-        return await self._start_scratch_classbased(item)
+        return await self._start_scratch_nopid(item)
 
     async def start_scratch_command(self, name: str) -> None:
         "spawns a given scratchpad's process"
         scratch = self.scratches.get(name)
         assert scratch
         self.scratches.setState(scratch, "respawned")
         old_pid = self.procs[name].pid if name in self.procs else 0
@@ -587,75 +275,73 @@
 
     async def event_activewindowv2(self, addr) -> None:
         "active windows hook"
         for uid, scratch in self.scratches.items():
             if not scratch.client_info:
                 continue
             if scratch.address == addr:
-                task = self._hysteresis_tasks.get(scratch.uid)
-                if task:
-                    task.cancel()
-                    if scratch.uid in self._hysteresis_tasks:
-                        del self._hysteresis_tasks[scratch.uid]
-                    self.log.debug("Canceled previous task for %s", uid)
+                self.cancel_task(uid)
             else:
                 if scratch.visible and scratch.conf.get("unfocus") == "hide":
                     last_shown = scratch.meta.get("last_shown", 0)
                     if last_shown + AFTER_SHOW_INHIBITION > time.time():
                         self.log.debug(
                             "(SKIPPED) hide %s because another client is active",
                             uid,
                         )
                         continue
 
                     hysteresis = scratch.conf.get("hysteresis", DEFAULT_HYSTERESIS)
                     if hysteresis:
-                        task = self._hysteresis_tasks.get(scratch.uid)
-                        if task:
-                            task.cancel()
-                            self.log.debug("Canceled previous task for %s", uid)
-                        self._hysteresis_tasks[scratch.uid] = asyncio.create_task(
-                            asyncio.sleep(hysteresis)
-                        )
+                        self.cancel_task(uid)
 
-                        async def _task(scratch, uid):
-                            if scratch.uid in self._hysteresis_tasks:
-                                await self._hysteresis_tasks[scratch.uid]
-                                del self._hysteresis_tasks[scratch.uid]
+                        async def _task(scratch, delay):
+                            await asyncio.sleep(delay)
                             if state.active_window == scratch.full_address:
                                 self.log.debug(
                                     "Skipped hidding %s because client got the focus back",
-                                    uid,
+                                    scratch.uid,
                                 )
                                 return
                             self.log.debug(
-                                "hide %s because another client is active", uid
+                                "hide %s because another client is active", scratch.uid
                             )
-                            await self.run_hide(uid, autohide=True)
+                            await self.run_hide(scratch.uid, autohide=True)
+
+                            try:
+                                del self._hysteresis_tasks[scratch.uid]
+                            except KeyError:
+                                pass
 
-                        asyncio.create_task(_task(scratch, uid))
+                        self._hysteresis_tasks[scratch.uid] = asyncio.create_task(
+                            _task(scratch, hysteresis)
+                        )
                     else:
                         self.log.debug("hide %s because another client is active", uid)
                         await self.run_hide(uid, autohide=True)
 
     async def _alternative_lookup(self):
-        "if class_match attribute is defined, use class matching and return True"
+        "if not matching by pid, use specific matching and return True"
         class_lookup_hack = [
             s
             for s in self.scratches.getByState("respawned")
-            if self.cast_bool(s.conf.get("class_match"))
+            if s.conf.get("match_by", "pid") != "pid"
         ]
         if not class_lookup_hack:
             return False
         self.log.debug("Lookup hack triggered")
-        # hack to update the client info from the provided class
-        for client in await self.hyprctlJSON("clients"):
-            assert isinstance(client, dict)
-            for pending_scratch in class_lookup_hack:
-                if pending_scratch.conf["class"] == client["class"]:
+        # hack to update the client info from the provided match_by attribute
+        clients = await self.hyprctlJSON("clients")
+        for pending_scratch in class_lookup_hack:
+            match_by = pending_scratch.conf["match_by"]
+            match_value = pending_scratch.conf[match_by]
+            match_fn = get_match_fn(match_by, match_value)
+            for client in clients:
+                assert isinstance(client, dict)
+                if match_fn(client[match_by], match_value):
                     self.scratches.register(pending_scratch, addr=client["address"][2:])
                     self.log.debug("client class found: %s", client)
                     await pending_scratch.updateClientInfo(client)
         return True
 
     async def event_openwindow(self, params) -> None:
         "open windows hook"
@@ -664,60 +350,70 @@
         rs = list(self.scratches.getByState("respawned"))
         if rs and not item:
             # hack for windows which aren't related to the process (see #8)
             if not await self._alternative_lookup():
                 self.log.info("Updating Scratch info")
                 await self.updateScratchInfo()
             item = self.scratches.get(addr=addr)
-            if item and item.should_hide:
+            if item and item.meta["should_hide"]:
                 await self.run_hide(item.uid, force=True)
         if item:
             await item.initialize(self)
 
     # }}}
+    def cancel_task(self, uid):
+        "cancel a task"
+        task = self._hysteresis_tasks.get(uid)
+        if task:
+            task.cancel()
+            self.log.debug("Canceled previous task for %s", uid)
+            if uid in self._hysteresis_tasks:
+                del self._hysteresis_tasks[uid]
+            return True
+        return False
+
     # Commands {{{
     async def run_toggle(self, uid_or_uids: str) -> None:
         """<name> toggles visibility of scratchpad "name" """
         if " " in uid_or_uids:
             uids = list(filter(bool, map(str.strip, uid_or_uids.split())))
         else:
             uids = [uid_or_uids.strip()]
 
+        for uid in uids:
+            self.cancel_task(uid)
+
         assert len(uids) > 0
         first_scratch = self.scratches.get(uids[0])
         if not first_scratch:
             self.log.warning("%s doesn't exist, can't toggle.", uids[0])
             await notify_error(
-                f"Scratchpad '{uids[0]}' not found, check your configuration or the toggle parameter"
+                f"Scratchpad '{uids[0]}' not found, check your configuration & the toggle parameter"
             )
             return
 
         if self.cast_bool(first_scratch.conf.get("alt_toggle")):
             # Needs to be on any monitor (if workspace matches)
-            extra_visibility_check = (
-                first_scratch.space_identifier
-                in await get_all_space_identifiers(await self.hyprctlJSON("monitors"))
-            )
+            extra_visibility_check = first_scratch.meta[
+                "space_identifier"
+            ] in await get_all_space_identifiers(await self.hyprctlJSON("monitors"))
         else:
             self.log.debug(
                 "visibility_check: %s == %s",
-                first_scratch.space_identifier,
+                first_scratch.meta["space_identifier"],
                 get_active_space_identifier(),
             )
             # Needs to be on the active monitor+workspace
             extra_visibility_check = (
-                first_scratch.space_identifier == get_active_space_identifier()
+                first_scratch.meta["space_identifier"] == get_active_space_identifier()
             )  # visible on the currently focused monitor
 
         is_visible = first_scratch.visible and (
-            first_scratch.conf.get(
-                "force_monitor"
-            )  # always showing on the same monitor
-            or extra_visibility_check
-        )
+            first_scratch.conf.get("force_monitor") or extra_visibility_check
+        )  # always showing on the same monitor
         tasks = []
 
         for uid in uids:
             item = self.scratches.get(uid)
             if not item:
                 self.log.warning("%s is not configured", uid)
             else:
@@ -795,14 +491,16 @@
             await notify_error(
                 f"Scratchpad '{uid}' not found, check your configuration or the show parameter"
             )
             return
 
         self.focused_window_tracking[uid] = state.active_window
 
+        self.cancel_task(uid)
+
         self.log.info("Showing %s", uid)
         was_alive = await item.isAlive()
         if not await self.ensure_alive(uid):
             self.log.error("Failed to show %s, aborting.", uid)
             return
 
         excluded = item.conf.get("excludes", [])
@@ -815,15 +513,15 @@
             assert scratch
             if scratch.visible:
                 await self.run_hide(e_uid, autohide=True)
         await item.updateClientInfo()
         await item.initialize(self)
 
         item.visible = True
-        item.space_identifier = get_active_space_identifier()
+        item.meta["space_identifier"] = get_active_space_identifier()
         monitor = await self.get_focused_monitor_props(
             name=item.conf.get("force_monitor")
         )
 
         assert monitor
         assert item.full_address, "No address !"
 
@@ -923,14 +621,15 @@
             self.log.warning("%s is not configured", uid)
             return
         if not scratch.visible and not force and not autohide:
             await notify_error(f"Scratchpad '{uid}' is not visible, will not hide.")
             self.log.warning("%s is already hidden", uid)
             return
         scratch.visible = False
+        scratch.meta["should_hide"] = False
         self.log.info("Hiding %s", uid)
         animated = await self._hide_transition(scratch, scratch.meta["monitor_info"])
 
         await self.hyprctl(
             f"movetoworkspacesilent special:scratch_{uid},address:{scratch.full_address}"
         )
```

### Comparing `pyprland-2.2.4/pyprland/plugins/shift_monitors.py` & `pyprland-2.2.5/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.2.5/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/system_notifier.py` & `pyprland-2.2.5/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/toggle_dpms.py` & `pyprland-2.2.5/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/toggle_special.py` & `pyprland-2.2.5/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.2.5/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.4/pyproject.toml` & `pyprland-2.2.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprland"
-version = "2.2.4"
+version = "2.2.5"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.2.4/PKG-INFO` & `pyprland-2.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.2.4
+Version: 2.2.5
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -44,15 +44,15 @@
 
 - Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues).
 - Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki)
 
 and if you have coding skills you can also
 
 - Enhance test coverage in our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests).
-- Write new plugins
+- Propose & write new plugins or enhancements
 
 ## Dependencies
 
 - **Hyprland** >= 0.37
 - **Python** >= 3.11
     - **aiofiles**
 
@@ -60,14 +60,17 @@
 
 > [!note]
 > Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 ### 2.2
 
 - Added [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/hyprland-community/pyprland/wiki/system_notifier) plugins.
+- Refactor in 2.2.5
+  - updated the syntax for [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers)
+  - deprecated `class_match` in [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
 
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) plugin improvements.
 
 ### 2.0
```

