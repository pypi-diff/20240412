# Comparing `tmp/pycotore-0.1.3.tar.gz` & `tmp/pycotore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycotore-0.1.3.tar", max compression
+gzip compressed data, was "pycotore-0.2.0.tar", max compression
```

## Comparing `pycotore-0.1.3.tar` & `pycotore-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.1.3/LICENSE
--rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.1.3/pycotore/__init__.py
--rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.1.3/pycotore/constants.py
--rw-r--r--   0        0        0      398 2024-04-11 13:49:12.930662 pycotore-0.1.3/pycotore/converter.py
--rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.1.3/pycotore/exceptions.py
--rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.1.3/pycotore/logger.py
--rw-r--r--   0        0        0     6543 2024-04-11 17:18:51.126199 pycotore-0.1.3/pycotore/progress.py
--rw-r--r--   0        0        0      597 2024-04-11 17:19:26.852089 pycotore-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.2.0/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.2.0/README.md
+-rw-r--r--   0        0        0      124 2024-04-12 06:18:55.434725 pycotore-0.2.0/pycotore/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-11 18:04:59.927935 pycotore-0.2.0/pycotore/_constants.py
+-rw-r--r--   0        0        0      398 2024-04-11 13:49:12.930662 pycotore-0.2.0/pycotore/converter.py
+-rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.2.0/pycotore/exceptions.py
+-rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.2.0/pycotore/logger.py
+-rw-r--r--   0        0        0     6671 2024-04-12 06:22:19.124560 pycotore-0.2.0/pycotore/progress.py
+-rw-r--r--   0        0        0      597 2024-04-12 06:24:06.634645 pycotore-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.2.0/PKG-INFO
```

### Comparing `pycotore-0.1.3/LICENSE` & `pycotore-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycotore-0.1.3/pycotore/logger.py` & `pycotore-0.2.0/pycotore/logger.py`

 * *Files identical despite different names*

### Comparing `pycotore-0.1.3/pycotore/progress.py` & `pycotore-0.2.0/pycotore/progress.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 import sys
 import os
 from datetime import datetime
-from logging import getLogger
-from pycotore.converter import convert_to_human
-
-# basicConfig(level=DEBUG)
-_logger = getLogger(__name__)
+from .converter import convert_to_human
 
 
 class ProgressBar():
     """
     Progress bar class
     """
 
     show_suffix: bool = False
     show_preffix: bool = False
     show_bar: bool = True
-    _speed = "[SPEED: {0: >7.2f} {1:<3}]"
+    _speed = "[SPEED: {0: ^7.2f}{1:<3}]"
     _percents = "[{0:>6.2f}%]"
     _time_left = "[LEFT: {0:0>2}:{1:0>2}:{2:0>2}]"
     _running = "[RUN: {0:0>2}:{1:0>2}:{2:0>2}]"
     _progress = "[{:{done_marker}>{done_size}}{}{:{base_marker}>{left_size}}]"
+    _completed: float = 0.00
     current_marker: list = ["-", "\\", "|", "/"]
     filler_marker: str = " "
+    bar_length: int = 0
+    bar_size: int = 0
+    _preffix: str = ""
+    _suffix: str = ""
+    _done_marker: str = "#"
+    _total = 100.00
 
     def __init__(
                 self,
-                done_marker: str = "#",
                 show_percents: bool = True,
                 show_estimate: bool = True,
                 show_runtime: bool = True,
                 show_speed: bool = True
             ):
-        self.preffix: str = ""
-        self.suffix: str = ""
-        self.bar_length: int = 0
-        self.bar_size: int = 0
         self.terminal_size: int = os.get_terminal_size().columns
-        self.progress: float = 0.00
-        self.total: float = 100.00
-        self.done_marker: str = done_marker
         self.percents: str = self._percents.format(0)
         self.show_percents: bool = show_percents
         self.show_numbers: bool = False
         self.time_start = datetime.now()
         self.show_estimate: bool = show_estimate
         self.time_left = self._time_left.format(99, 59, 59)
         self.run_time = self._running.format(0, 0, 0)
@@ -104,15 +99,15 @@
             self.time_left = self._time_left.format(99, 59, 59)
 
     def __update_percent_done(self) -> None:
         percents = float(self.progress * 100 / self.total)
         self.percents = self._percents.format(percents)
 
     def __format_bar(self) -> str:
-        bar = ["\r"]
+        bar = [""]
         bar_info = 0
         finished = int(self.bar_size * self.progress / self.total)
         if self.show_preffix:
             bar.append(self.preffix)
             bar_info += len(self.preffix)
         if self.show_bar:
             bar.append("")
@@ -129,70 +124,89 @@
         if self.show_speed:
             bar.append(self.speed)
             bar_info += len(self.speed)
         if self.show_suffix:
             bar.append(self.suffix)
             bar_info += len(self.suffix)
         if bar_index:
-            self.bar_size = self.terminal_size - bar_info - 4
+            self.bar_size = self.terminal_size - bar_info - 3
             left_size = self.bar_size - finished
             bar[bar_index] = self._progress.format(
-                    self.done_marker if finished > 1 else "",
+                    self._done_marker if finished > 1 else "",
                     self.__get_current_marker() if left_size > 0 else "",
                     self.filler_marker if left_size > 0 else "",
-                    done_marker=self.done_marker,
+                    done_marker=self._done_marker,
                     done_size=finished,
                     in_progress_marker=self.filler_marker,
                     base_marker=self.filler_marker,
                     left_size=left_size
                 )
         if self.bar_size <= finished:
             self.current_marker = ""
+        bar.append("\r")
         line = "".join(bar)
         return line
 
-    def flush_line(self) -> None:
-        sys.stdout.write("\n")
-        sys.stdout.flush()
-
-    def draw(self) -> None:
-        """
-        Draw a progress bar
-        """
-        self.__update_stats()
-        bar = self.__format_bar()
-        sys.stdout.write(bar)
-        sys.stdout.flush()
+    @property
+    def prefix(self) -> str:
+        return self._preffix
 
-    def set_prefix(self, preffix: str) -> None:
+    @prefix.setter
+    def prefix(self, preffix: str) -> None:
         """
         Change bar prefix
         """
         self.show_preffix = True
-        self.preffix = preffix
+        self._preffix = preffix
+
+    @property
+    def suffix(self) -> str:
+        return self._suffix
 
-    def set_suffix(self, suffix: str) -> None:
+    @suffix.setter
+    def suffix(self, suffix: str) -> None:
         """
         Change bar suffix
         """
         self.show_suffix = True
-        self.suffix = suffix
+        self._suffix = suffix
+
+    @property
+    def progress(self) -> float:
+        return self._completed
 
-    def update_progress(self, done: float) -> None:
+    @progress.setter
+    def progress(self, progress: float) -> None:
         """
         Update progress done percentage
         """
-        self.progress = done
+        if float(progress):
+            self._completed = float(progress)
+        else:
+            raise ValueError("Progress must be int or float")
 
-    def set_total(self, total) -> None:
+    @property
+    def total(self):
+        """
+        Return total value of progress calculation
+        """
+        return self._total
+
+    @total.setter
+    def total(self, total) -> None:
         """
         Set progress bar total value
         """
-        try:
-            if float(total):
-                self.total = total
-        except ValueError:
-            _logger.warning("Unable to set total")
+        self._total = total
+
+    def draw(self) -> None:
+        """
+        Draw a progress bar
+        """
+        self.__update_stats()
+        bar = self.__format_bar()
+        sys.stdout.write(bar)
+        sys.stdout.flush()
 
-    def __clear_line(self, line) -> None:
-        sys.stdout.write("\033[K")
+    def __del__(self) -> None:
+        sys.stdout.write("\n")
         sys.stdout.flush()
```

### Comparing `pycotore-0.1.3/pyproject.toml` & `pycotore-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pycotore"
 readme = "README.md"
 authors = ["Arunas Grigalionis <arunas.grigalionis@gmail.com>"]
 description = "Generic classes for reuse"
-version = "0.1.3"
+version = "0.2.0"
 license = "GPL-3.0-only"
 homepage = "https://github.com/niekosau"
 repository = "https://github.com/niekosau/pycotore"
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `pycotore-0.1.3/PKG-INFO` & `pycotore-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycotore
-Version: 0.1.3
+Version: 0.2.0
 Summary: Generic classes for reuse
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

