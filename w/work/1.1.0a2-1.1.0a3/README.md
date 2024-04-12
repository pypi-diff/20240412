# Comparing `tmp/work-1.1.0a2.tar.gz` & `tmp/work-1.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work-1.1.0a2.tar", max compression
+gzip compressed data, was "work-1.1.0a3.tar", max compression
```

## Comparing `work-1.1.0a2.tar` & `work-1.1.0a3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0a2/README.md
--rw-r--r--   0        0        0      594 2024-04-10 16:15:46.405254 work-1.1.0a2/pyproject.toml
--rw-r--r--   0        0        0    90047 2024-04-10 16:15:05.052930 work-1.1.0a2/src/work.py
--rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0a2/src/work_components/__init__.py
--rw-r--r--   0        0        0    24511 2024-04-10 11:59:44.154278 work-1.1.0a2/src/work_components/arguments.py
--rw-r--r--   0        0        0     2190 2024-04-10 16:16:05.333403 work-1.1.0a2/src/work_components/consts.py
--rw-r--r--   0        0        0    22097 2024-04-10 16:15:05.068930 work-1.1.0a2/src/work_components/container.py
--rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0a2/src/work_components/dao/__init__.py
--rw-r--r--   0        0        0    17192 2024-04-10 16:15:05.056930 work-1.1.0a2/src/work_components/dao/core.py
--rw-r--r--   0        0        0      270 2024-04-08 19:32:29.853389 work-1.1.0a2/src/work_components/dao/env.py
--rw-r--r--   0        0        0     1643 2024-04-08 19:32:29.853389 work-1.1.0a2/src/work_components/dao/flags.py
--rw-r--r--   0        0        0    11503 2024-04-08 19:32:29.853389 work-1.1.0a2/src/work_components/dao/rc.py
--rw-r--r--   0        0        0    11011 2024-04-08 18:05:30.527145 work-1.1.0a2/src/work_components/dao/recess.py
--rw-r--r--   0        0        0     6238 2024-04-10 16:15:05.040930 work-1.1.0a2/src/work_components/dt_parse.py
--rw-r--r--   0        0        0     4470 2024-04-08 18:05:30.527145 work-1.1.0a2/src/work_components/migrate.py
--rw-r--r--   0        0        0      320 2024-04-10 12:10:12.266685 work-1.1.0a2/src/work_components/protocols.py
--rw-r--r--   0        0        0     2650 2024-04-10 16:15:05.064930 work-1.1.0a2/src/work_components/timestamps.py
--rw-r--r--   0        0        0     8067 2024-04-08 18:05:30.527145 work-1.1.0a2/src/work_components/util.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 work-1.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0a3/README.md
+-rw-r--r--   0        0        0      594 2024-04-12 15:03:30.774646 work-1.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0    91340 2024-04-12 15:03:12.714508 work-1.1.0a3/src/work.py
+-rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0a3/src/work_components/__init__.py
+-rw-r--r--   0        0        0    24511 2024-04-10 11:59:44.154278 work-1.1.0a3/src/work_components/arguments.py
+-rw-r--r--   0        0        0     2190 2024-04-12 15:03:29.658638 work-1.1.0a3/src/work_components/consts.py
+-rw-r--r--   0        0        0    22097 2024-04-10 16:48:42.800523 work-1.1.0a3/src/work_components/container.py
+-rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0a3/src/work_components/dao/__init__.py
+-rw-r--r--   0        0        0    17192 2024-04-10 16:48:42.792523 work-1.1.0a3/src/work_components/dao/core.py
+-rw-r--r--   0        0        0      270 2024-04-08 19:32:29.853389 work-1.1.0a3/src/work_components/dao/env.py
+-rw-r--r--   0        0        0     1643 2024-04-08 19:32:29.853389 work-1.1.0a3/src/work_components/dao/flags.py
+-rw-r--r--   0        0        0    11503 2024-04-08 19:32:29.853389 work-1.1.0a3/src/work_components/dao/rc.py
+-rw-r--r--   0        0        0    11011 2024-04-08 18:05:30.527145 work-1.1.0a3/src/work_components/dao/recess.py
+-rw-r--r--   0        0        0     6238 2024-04-10 16:48:42.780523 work-1.1.0a3/src/work_components/dt_parse.py
+-rw-r--r--   0        0        0     4470 2024-04-08 18:05:30.527145 work-1.1.0a3/src/work_components/migrate.py
+-rw-r--r--   0        0        0      320 2024-04-10 12:10:12.266685 work-1.1.0a3/src/work_components/protocols.py
+-rw-r--r--   0        0        0     2650 2024-04-10 16:48:42.796523 work-1.1.0a3/src/work_components/timestamps.py
+-rw-r--r--   0        0        0     8067 2024-04-08 18:05:30.527145 work-1.1.0a3/src/work_components/util.py
+-rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 work-1.1.0a3/PKG-INFO
```

### Comparing `work-1.1.0a2/README.md` & `work-1.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/pyproject.toml` & `work-1.1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "work"
-version = "1.1.0a2"
+version = "1.1.0a3"
 description = "Manual time tracking via a CLI that works similarly to git."
 authors = ["vauhochzett <vauhoch@zett.cc>"]
 readme = "README.md"
 homepage = "https://vauhoch.zett.cc/work/"
 packages = [
     { include = "work.py", from = "src" },
     { include = "work_components", from = "src" },
```

### Comparing `work-1.1.0a2/src/work.py` & `work-1.1.0a3/src/work.py`

 * *Files 2% similar despite different names*

```diff
@@ -1145,60 +1145,83 @@
     ) -> None:
         """Print the given list of dates. For more than one date: Print a summary."""
 
         if not days:
             raise ValueError("At least one element is required")
 
         active_start: Optional[dt.datetime] = self.dao.get_start_time()
-        # This variable stores two properties: include_active and the date to include
-        include_active_date: Optional[dt.date] = None
+        # This variable stores two properties: whether to include the active run (if
+        # it is set or not) and the dates to include (which values it contains)
+        include_active_days: List[dt.date] = []
         if active_start is not None and include_active:
-            if active_start.date() not in days:
+            include_active_days = [
+                active_day
+                for active_day in util.get_period(active_start.date(), dt.date.today())
+                if active_day in days
+            ]
+            if not include_active_days:
                 raise InvalidOperationWarning.cant(
                     "list the active run",
                     because="the selected period doesn't cover it",
                 )
-            include_active_date = active_start.date()
 
         output: List[str] = []
         total_includes_active_run: bool = False
 
         total_number_of_records: int = 0
         total_minutes_worked: float = 0.0
         for day in days:
             records: List[Record] = self.dao.get_entries(date=day)
 
-            active_start_to_include: Optional[dt.datetime] = None
-            # If it is None or not the current day, do not include the active run.
-            if include_active_date == day:
-                active_start_to_include = active_start
+            active_run_to_include: Optional[Record] = None
+            # Only include the active run (segment) if requested and it covers this day.
+            if day in include_active_days:
+                active_start = cast(dt.datetime, active_start)
+                zero_o_clock = dt.time(hour=0, minute=0)
+                # Only add minutes that cover the listed day
+                active_run_to_include = Record(
+                    # If started before this day, we only include the time from midnight
+                    start=max(
+                        dt.datetime.combine(day, zero_o_clock),
+                        active_start,
+                    ),
+                    # The fictional end time is chosen to be...
+                    end=min(
+                        max(  # now (default) or start (future run) - run started this day
+                            self._dt_now_stripped(),
+                            active_start,
+                        ),
+                        # or midnight of the listed day, if the other options are later
+                        dt.datetime.combine(day + dt.timedelta(days=1), zero_o_clock),
+                    ),
+                )
 
             # Filter entries based on passed filter parameters
             records = self.filter_records(
                 records, filter_category=filter_category, filter_message=filter_message
             )
 
-            if len(records) == 0 and not list_empty and active_start_to_include is None:
+            if len(records) == 0 and not list_empty and active_run_to_include is None:
                 continue
 
             output_lines = self._evaluate_day(
                 day=day,
                 records=records,
                 print_breaks=print_breaks,
                 only_time=only_time,
-                active_start_to_include=active_start_to_include,
+                active_run_to_include=active_run_to_include,
             )
             total_number_of_records += len(records)
             output.extend(output_lines)
             output.append("")
             total_minutes_worked += self._minutes_worked(records)
 
             # If we want to include the active run and it is today, add those minutes.
-            if active_start_to_include is not None:
-                total_minutes_worked += self._minutes_active_run()
+            if active_run_to_include is not None:
+                total_minutes_worked += active_run_to_include.get_minutes()
                 total_includes_active_run = True
 
         # Add info if no result (when omitting empty records)
         if not output:
             output.append(self._none_found_msg(days))
         # Remove empty last line if no summary is added
         elif len(days) <= 1:
@@ -1238,29 +1261,26 @@
 
     def _evaluate_day(
         self,
         day: dt.date,
         records: List[Record],
         print_breaks: bool,
         only_time: bool,
-        active_start_to_include: Optional[dt.datetime] = None,
+        active_run_to_include: Optional[Record] = None,
     ) -> List[str]:
         """
         Produce a list of output strings describing the records stored on the given day.
         Return the output list as well as the number of records.
 
         :param print_breaks: If true, intertwine the break times with the listed entries.
         :param only_time: If true, omit optional record fields from output.
         :param active_start_to_include: If given, the "active run" will be added to the output.
         """
 
-        if (
-            active_start_to_include is not None
-            and active_start_to_include.date() != day
-        ):
+        if active_run_to_include is not None and active_run_to_include.date != day:
             raise ValueError("Invalid day for active_start_to_include passed.")
 
         # Add the year to the printout if it's not the current year
         date_fmt: str = self._date_fmt(day)
 
         # Merge entries for only_time
         record_count: int = len(records)
@@ -1276,37 +1296,31 @@
                 day.strftime(date_fmt),
                 record_count,
                 (
                     f" (merged to {len(records)})"
                     if only_time and len(records) != record_count
                     else ""
                 ),
-                " (+ active run)" if active_start_to_include is not None else "",
+                " (+ active run)" if active_run_to_include is not None else "",
             )
         )
 
-        active_run_to_include: Optional[Record] = None
-        if active_start_to_include is not None:
-            # For a future run, we have to select an end time, so we just choose the
-            # start time (= 0m).
-            active_run_to_include = Record(
-                start=active_start_to_include,
-                end=max(active_start_to_include, self._dt_now_stripped()),
-            )
-
+        if active_run_to_include is not None:
             # Check and warn if active run would overlap the listed entries
             for other in records:
-                if (
-                    other.end > active_run_to_include.start
-                    and other.start < active_run_to_include.end
-                ):
+                if active_run_to_include.overlaps(other):
                     raise InvalidOperationWarning.cant(
                         "list active run",
                         "it overlaps with an already stored entry",
                     )
+                if other.start >= active_run_to_include.start:
+                    raise InvalidOperationWarning.cant(
+                        "list active run",
+                        "you have logged a future run, which is an undefined case",
+                    )
 
             records.append(active_run_to_include)
 
         total_minutes: float = 0.0
         total_break_minutes: float = 0.0
         prin_table: PrinTable = PrinTable()
 
@@ -1330,19 +1344,23 @@
             if print_breaks:
                 break_str, break_length = self._break_str(records, i)
                 total_break_minutes += break_length
                 if break_length > 0:
                     prin_table.add_row(["", Color.color(break_str, Color.GRAY)])
 
         # Replace time of active run with start time only, colored in blue.
-        if active_start_to_include is not None:
+        if active_run_to_include is not None:
             active_run_row: List[str] = prin_table.rows.pop()
-            active_run_time_str: str = (
-                f"{active_start_to_include.strftime(TIME_FORMAT)} ~      "
-            )
+            active_run_time_str: str = active_run_to_include.strftime(TIME_FORMAT)
+            # active_run_time_str = active_run_time_str.replace("–", "~")
+            # Do not print the end time if the listed day is today, which covers the
+            # fictional 'end' of the active run (now)
+            if ts.date_equals(day, dt.date.today()):
+                assert len(active_run_time_str) == 13 and " – " in active_run_time_str
+                active_run_time_str = active_run_time_str[:-7] + "~      "
             active_run_row[0] = Color.color(active_run_time_str, Color.BLUE)
             prin_table.add_row(active_run_row)
 
         for printable_row in prin_table.printable_str():
             result.append(printable_row)
 
         if len(records) > 0:
```

### Comparing `work-1.1.0a2/src/work_components/arguments.py` & `work-1.1.0a3/src/work_components/arguments.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/src/work_components/consts.py` & `work-1.1.0a3/src/work_components/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """ Shared constants """
 
 import os
 import pathlib
 from typing import List, Tuple
 
-VERSION: str = "1.1.0a2"
+VERSION: str = "1.1.0a3"
 RECORDS_VERSION: int = 3
 
 # Directories
 PARENT_DIR: pathlib.Path = pathlib.Path("~", ".local", "share").expanduser()
 DIRECTORY: pathlib.Path = PARENT_DIR.joinpath("work")
 DIRECTORY_DEBUG: pathlib.Path = PARENT_DIR.joinpath("debug", "work")
```

### Comparing `work-1.1.0a2/src/work_components/container.py` & `work-1.1.0a3/src/work_components/container.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/src/work_components/dao/core.py` & `work-1.1.0a3/src/work_components/dao/core.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/src/work_components/dao/flags.py` & `work-1.1.0a3/src/work_components/dao/flags.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/src/work_components/dao/rc.py` & `work-1.1.0a3/src/work_components/dao/rc.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/src/work_components/dao/recess.py` & `work-1.1.0a3/src/work_components/dao/recess.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/src/work_components/dt_parse.py` & `work-1.1.0a3/src/work_components/dt_parse.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/src/work_components/migrate.py` & `work-1.1.0a3/src/work_components/migrate.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/src/work_components/timestamps.py` & `work-1.1.0a3/src/work_components/timestamps.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/src/work_components/util.py` & `work-1.1.0a3/src/work_components/util.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a2/PKG-INFO` & `work-1.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: work
-Version: 1.1.0a2
+Version: 1.1.0a3
 Summary: Manual time tracking via a CLI that works similarly to git.
 Home-page: https://vauhoch.zett.cc/work/
 Author: vauhochzett
 Author-email: vauhoch@zett.cc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

