# Comparing `tmp/pycotore-0.1.2.tar.gz` & `tmp/pycotore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycotore-0.1.2.tar", max compression
+gzip compressed data, was "pycotore-0.1.3.tar", max compression
```

## Comparing `pycotore-0.1.2.tar` & `pycotore-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.1.2/LICENSE
--rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.1.2/pycotore/__init__.py
--rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.1.2/pycotore/constants.py
--rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.1.2/pycotore/exceptions.py
--rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.1.2/pycotore/logger.py
--rw-r--r--   0        0        0     5196 2024-04-11 09:37:50.889172 pycotore-0.1.2/pycotore/progress.py
--rw-r--r--   0        0        0      597 2024-04-11 08:46:30.043071 pycotore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.1.3/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.1.3/pycotore/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.1.3/pycotore/constants.py
+-rw-r--r--   0        0        0      398 2024-04-11 13:49:12.930662 pycotore-0.1.3/pycotore/converter.py
+-rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.1.3/pycotore/exceptions.py
+-rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.1.3/pycotore/logger.py
+-rw-r--r--   0        0        0     6543 2024-04-11 17:18:51.126199 pycotore-0.1.3/pycotore/progress.py
+-rw-r--r--   0        0        0      597 2024-04-11 17:19:26.852089 pycotore-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.1.3/PKG-INFO
```

### Comparing `pycotore-0.1.2/LICENSE` & `pycotore-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycotore-0.1.2/pycotore/logger.py` & `pycotore-0.1.3/pycotore/logger.py`

 * *Files identical despite different names*

### Comparing `pycotore-0.1.2/pycotore/progress.py` & `pycotore-0.1.3/pycotore/progress.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,185 @@
 import sys
 import os
 from datetime import datetime
 from logging import getLogger
+from pycotore.converter import convert_to_human
 
 # basicConfig(level=DEBUG)
 _logger = getLogger(__name__)
 
 
 class ProgressBar():
     """
     Progress bar class
     """
 
-    show_suffix: bool = True
-    show_preffix: bool = True
+    show_suffix: bool = False
+    show_preffix: bool = False
     show_bar: bool = True
+    _speed = "[SPEED: {0: >7.2f} {1:<3}]"
+    _percents = "[{0:>6.2f}%]"
+    _time_left = "[LEFT: {0:0>2}:{1:0>2}:{2:0>2}]"
+    _running = "[RUN: {0:0>2}:{1:0>2}:{2:0>2}]"
+    _progress = "[{:{done_marker}>{done_size}}{}{:{base_marker}>{left_size}}]"
+    current_marker: list = ["-", "\\", "|", "/"]
+    filler_marker: str = " "
 
     def __init__(
                 self,
-                base_marker: str = ".",
-                done_marke: str = "#",
-                current_marker: str = ">",
+                done_marker: str = "#",
                 show_percents: bool = True,
                 show_estimate: bool = True,
-                show_runtime: bool = True
+                show_runtime: bool = True,
+                show_speed: bool = True
             ):
         self.preffix: str = ""
         self.suffix: str = ""
         self.bar_length: int = 0
         self.bar_size: int = 0
         self.terminal_size: int = os.get_terminal_size().columns
         self.progress: float = 0.00
         self.total: float = 100.00
-        self.done_marker: str = done_marke
-        self.in_progress_marker: str = base_marker
-        self.current_marker: str = current_marker
-        self.percents: float = "000.00%"
+        self.done_marker: str = done_marker
+        self.percents: str = self._percents.format(0)
         self.show_percents: bool = show_percents
         self.show_numbers: bool = False
         self.time_start = datetime.now()
         self.show_estimate: bool = show_estimate
-        self.estimate = "|ETA: 00:00:00"
-        self.run_time = "|RUN: 00:00:00"
+        self.time_left = self._time_left.format(99, 59, 59)
+        self.run_time = self._running.format(0, 0, 0)
+        self._run_time = datetime.now()
+        self.speed = self._speed.format(0, "b")
         self.show_runtime: bool = show_runtime
+        self.avg_speed = 0
+        self.show_speed = show_speed
 
-    def flush_line(self) -> None:
-        sys.stdout.write("\n")
-        sys.stdout.flush()
+    def __update_stats(self) -> None:
+        self.__run_time()
+        self.__update_avg_speed()
+        if self.show_percents:
+            self.__update_percent_done()
+        if self.show_estimate:
+            self.__calculate_estimate()
+        if self.show_runtime:
+            self.__update_run_time()
+        if self.show_speed:
+            self.__update_speed()
+        self.__update_terminal_size()
+
+    def __get_current_marker(self) -> str:
+        self.current_marker.append(self.current_marker.pop(0))
+        return self.current_marker[-1]
+
+    def __update_speed(self) -> None:
+        speed, units = convert_to_human(self.avg_speed)
+        self.speed = self._speed.format(speed, units)
+
+    def __run_time(self) -> None:
+        self._run_time = datetime.now() - self.time_start
 
     def __update_terminal_size(self) -> None:
         self.terminal_size = os.get_terminal_size().columns
-        self.__update_bar_length()
+
+    def __split_time(self, seconds: int) -> list:
+        result = []
+        result.append(int(seconds // 3600))
+        result.append(int(seconds // 60))
+        result.append(int(seconds % 60))
+        return result
 
     def __update_run_time(self) -> None:
-        now = datetime.now()
-        run_time = now - self.time_start
-        self.run_time = f"|RUN: {run_time.seconds // 3600:0>2}:{run_time.seconds // 60:0>2}:{run_time.seconds % 60:0>2}"
+        time = self.__split_time(self._run_time.total_seconds())
+        self.run_time = self._running.format(time[0], time[1], time[2])
+
+    def __update_avg_speed(self) -> None:
+        self.avg_speed = self.progress // self._run_time.total_seconds()
 
     def __calculate_estimate(self) -> None:
-        now = datetime.now()
-        run_time = now - self.time_start
         run_data_left = self.total - self.progress
-        run_avg_speed = int(self.progress // run_time.total_seconds())
-        run_estimate = int(run_data_left // run_avg_speed)
-        self.estimate = f"|ETA: {run_estimate // 3600:0>2}:{run_estimate // 60:0>2}:{run_estimate % 60:0>2}"
+        try:
+            run_estimate = run_data_left // self.avg_speed
+            time = self.__split_time(run_estimate)
+            self.time_left = self._time_left.format(time[0], time[1], time[2])
+        except ZeroDivisionError:
+            self.time_left = self._time_left.format(99, 59, 59)
 
     def __update_percent_done(self) -> None:
-        percents = round(self.progress * 100 / self.total, 2)
-        self.percents = f"{percents:0>6.2f}%"
-
-    def __update_bar_length(self) -> None:
-        """
-        Updating progress bar total size
-        """
-        self.bar_length = len(self.preffix) + len(self.suffix)
-        self.bar_size = self.terminal_size - self.bar_length - 3
-        if self.show_percents:
-            self.bar_size -= len(self.percents)
-        if self.show_estimate:
-            self.bar_size -= len(self.estimate)
-        if self.show_runtime:
-            self.bar_size -= len(self.run_time)
+        percents = float(self.progress * 100 / self.total)
+        self.percents = self._percents.format(percents)
 
     def __format_bar(self) -> str:
-        bar = []
+        bar = ["\r"]
+        bar_info = 0
         finished = int(self.bar_size * self.progress / self.total)
-        finished_mark = self.done_marker * finished
-        in_progress_mark = self.in_progress_marker * (self.bar_size - finished - 1)
-        if self.bar_size <= finished:
-            self.current_marker = ""
-        if self.preffix:
-            bar.append(f"{self.preffix} ")
+        if self.show_preffix:
+            bar.append(self.preffix)
+            bar_info += len(self.preffix)
         if self.show_bar:
-            bar.append(f"[{finished_mark}{self.current_marker}{in_progress_mark}]")
+            bar.append("")
+            bar_index = len(bar) - 1
         if self.show_percents:
             bar.append(self.percents)
-        if self.show_estimate:
-            bar.append(self.estimate)
+            bar_info += len(self.percents)
         if self.show_runtime:
             bar.append(self.run_time)
+            bar_info += len(self.run_time)
+        if self.show_estimate:
+            bar.append(self.time_left)
+            bar_info += len(self.time_left)
+        if self.show_speed:
+            bar.append(self.speed)
+            bar_info += len(self.speed)
         if self.show_suffix:
-            bar.append(f"|{self.suffix}")
-        bar.append("\r")
-        return "".join(bar)
+            bar.append(self.suffix)
+            bar_info += len(self.suffix)
+        if bar_index:
+            self.bar_size = self.terminal_size - bar_info - 4
+            left_size = self.bar_size - finished
+            bar[bar_index] = self._progress.format(
+                    self.done_marker if finished > 1 else "",
+                    self.__get_current_marker() if left_size > 0 else "",
+                    self.filler_marker if left_size > 0 else "",
+                    done_marker=self.done_marker,
+                    done_size=finished,
+                    in_progress_marker=self.filler_marker,
+                    base_marker=self.filler_marker,
+                    left_size=left_size
+                )
+        if self.bar_size <= finished:
+            self.current_marker = ""
+        line = "".join(bar)
+        return line
+
+    def flush_line(self) -> None:
+        sys.stdout.write("\n")
+        sys.stdout.flush()
 
     def draw(self) -> None:
         """
         Draw a progress bar
         """
-        if self.show_percents:
-            self.__update_percent_done()
-        if self.show_estimate:
-            self.__calculate_estimate()
-        if self.show_runtime:
-            self.__update_run_time()
-        self.__update_terminal_size()
+        self.__update_stats()
         bar = self.__format_bar()
         sys.stdout.write(bar)
         sys.stdout.flush()
 
     def set_prefix(self, preffix: str) -> None:
         """
         Change bar prefix
         """
+        self.show_preffix = True
         self.preffix = preffix
-        self.__update_bar_length()
 
     def set_suffix(self, suffix: str) -> None:
         """
         Change bar suffix
         """
+        self.show_suffix = True
         self.suffix = suffix
-        self.__update_bar_length()
-
-    def set_bar_size(self, size: int) -> None:
-        """
-        Change bar size
-        """
-        try:
-            if int(size):
-                self.bar_size = size
-        except ValueError:
-            _logger.warning("Unable to set bar size")
 
     def update_progress(self, done: float) -> None:
         """
         Update progress done percentage
         """
         self.progress = done
```

### Comparing `pycotore-0.1.2/pyproject.toml` & `pycotore-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pycotore"
 readme = "README.md"
 authors = ["Arunas Grigalionis <arunas.grigalionis@gmail.com>"]
 description = "Generic classes for reuse"
-version = "0.1.2"
+version = "0.1.3"
 license = "GPL-3.0-only"
 homepage = "https://github.com/niekosau"
 repository = "https://github.com/niekosau/pycotore"
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `pycotore-0.1.2/PKG-INFO` & `pycotore-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycotore
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generic classes for reuse
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

