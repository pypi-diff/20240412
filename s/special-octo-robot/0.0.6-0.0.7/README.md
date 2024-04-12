# Comparing `tmp/special-octo-robot-0.0.6.tar.gz` & `tmp/special-octo-robot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special-octo-robot-0.0.6.tar", last modified: Sun Apr  7 14:14:57 2024, max compression
+gzip compressed data, was "special-octo-robot-0.0.7.tar", last modified: Fri Apr 12 07:41:09 2024, max compression
```

## Comparing `special-octo-robot-0.0.6.tar` & `special-octo-robot-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 14:14:57.686500 special-octo-robot-0.0.6/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0.0.6/LICENSE
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.6/MANIFEST.in
--rw-r--r--   0 nginx     (1000) nginx     (1000)     3718 2024-04-07 14:14:57.686500 special-octo-robot-0.0.6/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     3022 2024-04-07 04:26:45.000000 special-octo-robot-0.0.6/README.md
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 14:14:57.686500 special-octo-robot-0.0.6/app/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.6/app/__init__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.6/app/__main__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-04-07 14:14:18.000000 special-octo-robot-0.0.6/app/__version__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     6036 2024-04-07 14:14:48.000000 special-octo-robot-0.0.6/app/application.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     3423 2024-04-07 11:46:37.000000 special-octo-robot-0.0.6/app/console.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      396 2024-04-07 11:44:42.000000 special-octo-robot-0.0.6/app/constants.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1904 2024-04-07 14:10:51.000000 special-octo-robot-0.0.6/app/database.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     5680 2024-04-07 14:05:02.000000 special-octo-robot-0.0.6/devcord.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-04-07 14:14:57.686500 special-octo-robot-0.0.6/setup.cfg
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1200 2024-04-07 13:24:59.000000 special-octo-robot-0.0.6/setup.py
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 14:14:57.686500 special-octo-robot-0.0.6/special_octo_robot.egg-info/
--rw-r--r--   0 nginx     (1000) nginx     (1000)     3718 2024-04-07 14:14:57.000000 special-octo-robot-0.0.6/special_octo_robot.egg-info/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      421 2024-04-07 14:14:57.000000 special-octo-robot-0.0.6/special_octo_robot.egg-info/SOURCES.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-04-07 14:14:57.000000 special-octo-robot-0.0.6/special_octo_robot.egg-info/dependency_links.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-04-07 14:14:57.000000 special-octo-robot-0.0.6/special_octo_robot.egg-info/entry_points.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       26 2024-04-07 14:14:57.000000 special-octo-robot-0.0.6/special_octo_robot.egg-info/requires.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-04-07 14:14:57.000000 special-octo-robot-0.0.6/special_octo_robot.egg-info/top_level.txt
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-12 07:41:09.361891 special-octo-robot-0.0.7/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0.0.7/LICENSE
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.7/MANIFEST.in
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     4180 2024-04-12 07:41:09.361891 special-octo-robot-0.0.7/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     3484 2024-04-10 14:01:48.000000 special-octo-robot-0.0.7/README.md
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-12 07:41:09.357890 special-octo-robot-0.0.7/app/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.7/app/__init__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.7/app/__main__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-04-12 07:31:24.000000 special-octo-robot-0.0.7/app/__version__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     6033 2024-04-10 14:01:48.000000 special-octo-robot-0.0.7/app/application.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      803 2024-04-12 07:29:46.000000 special-octo-robot-0.0.7/app/config.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     3317 2024-04-12 07:28:09.000000 special-octo-robot-0.0.7/app/console.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      576 2024-04-12 07:29:46.000000 special-octo-robot-0.0.7/app/constants.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     2161 2024-04-12 06:27:07.000000 special-octo-robot-0.0.7/app/database.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     7149 2024-04-12 07:29:56.000000 special-octo-robot-0.0.7/devcord.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-04-12 07:41:09.361891 special-octo-robot-0.0.7/setup.cfg
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     1200 2024-04-07 13:24:59.000000 special-octo-robot-0.0.7/setup.py
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-12 07:41:09.361891 special-octo-robot-0.0.7/special_octo_robot.egg-info/
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     4180 2024-04-12 07:41:09.000000 special-octo-robot-0.0.7/special_octo_robot.egg-info/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      435 2024-04-12 07:41:09.000000 special-octo-robot-0.0.7/special_octo_robot.egg-info/SOURCES.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-04-12 07:41:09.000000 special-octo-robot-0.0.7/special_octo_robot.egg-info/dependency_links.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-04-12 07:41:09.000000 special-octo-robot-0.0.7/special_octo_robot.egg-info/entry_points.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       26 2024-04-12 07:41:09.000000 special-octo-robot-0.0.7/special_octo_robot.egg-info/requires.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-04-12 07:41:09.000000 special-octo-robot-0.0.7/special_octo_robot.egg-info/top_level.txt
```

### Comparing `special-octo-robot-0.0.6/LICENSE` & `special-octo-robot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.6/PKG-INFO` & `special-octo-robot-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: Windows
 Platform: MacOS X
@@ -191,7 +191,44 @@
 
 Mark as pending:
 
 ```bash
 $ devcord task 10 -pd
 $ devcord task 10 --pending
 ```
+
+
+Delete Task:
+
+```bash
+$ devcord task 10 -dl
+$ devcord task 10 --delete
+```
+
+
+Modify Title:
+
+```bash
+$ devcord task 10 -n "new title"
+$ devcord task 10 --name "new title"
+```
+
+Modify Priority:
+
+```bash
+$ devcord task 10 -p 3
+$ devcord task 10 --priority 3
+```
+
+Modify Deadline:
+
+```bash
+$ devcord task 10 -dd "dd/mm/yyyy"
+$ devcord task 10 --deadline "dd/mm/yyyy"
+```
+
+Modify Labels:
+
+```bash
+$ devcord task 10 -lb "label"
+$ devcord task 10 --label "label"
+```
```

### Comparing `special-octo-robot-0.0.6/README.md` & `special-octo-robot-0.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -170,7 +170,44 @@
 
 Mark as pending:
 
 ```bash
 $ devcord task 10 -pd
 $ devcord task 10 --pending
 ```
+
+
+Delete Task:
+
+```bash
+$ devcord task 10 -dl
+$ devcord task 10 --delete
+```
+
+
+Modify Title:
+
+```bash
+$ devcord task 10 -n "new title"
+$ devcord task 10 --name "new title"
+```
+
+Modify Priority:
+
+```bash
+$ devcord task 10 -p 3
+$ devcord task 10 --priority 3
+```
+
+Modify Deadline:
+
+```bash
+$ devcord task 10 -dd "dd/mm/yyyy"
+$ devcord task 10 --deadline "dd/mm/yyyy"
+```
+
+Modify Labels:
+
+```bash
+$ devcord task 10 -lb "label"
+$ devcord task 10 --label "label"
+```
```

### Comparing `special-octo-robot-0.0.6/app/application.py` & `special-octo-robot-0.0.7/app/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     label=None,
     parent=None,
 ):
     """
     Add a task to the database.
     """
     columns = ["title"]
-    values = [f'"{sanitize_text(title)}"' ""]
+    values = [f'"{sanitize_text(title)}"']
     if description:
         columns.append("description")
         values.append(f'"{sanitize_text(description)}"')
     if priority:
         columns.append("priority")
         values.append(str(priority))
     if today:
```

### Comparing `special-octo-robot-0.0.6/app/console.py` & `special-octo-robot-0.0.7/app/console.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return "#50C878"
     elif status == "Pending":
         return "bold red"
     else:
         return "#FFFFFF"
 
 
-def get_table(tasks, colored=True):
+def get_table(tasks, plain=True):
     table = Table(title="Tasks", highlight=True, leading=True)
     table.add_column("Priority", justify="center", style="white")
     table.add_column("Task", justify="left", style="white")
     table.add_column("Status", justify="center", style="white")
     table.add_column("Deadline", justify="center", style="white")
     table.add_column("Label", justify="center", style="white")
     table.add_column("ID", justify="center", style="white", no_wrap=True)
@@ -45,15 +45,15 @@
     bold_text_style = Style(color="#FFFFFF", bold=True)
     none_style = Style(color="magenta")
 
     for task in tasks:
         table.add_row(
             (
                 f"[{get_priority_color(task)}]●"
-                if colored
+                if plain
                 else f"[{text_style}]{task['priority']}"
             ),
             f'[{text_style}]{task["title"]}',
             f'[{get_status_color(task["status"])}][italic]{task["status"]}',
             task["deadline"],
             f'[{bold_text_style if task["label"] != "None" else none_style}]{task["label"]}',
             f"[{text_style}]{task['id']}",
@@ -77,15 +77,15 @@
                 fg="red",
             ),
         )
         return False
     return True
 
 
-def print_tasks(tasks, output=None, path=None):
+def print_tasks(tasks, output=None, path=None, plain=True):
 
     file = None
     if path:
         path = path.strip()
         if path[0] != "/":  # If path is not absolute
             path = os.path.join(os.getcwd(), path)
 
@@ -93,20 +93,16 @@
             return
 
         file = open(path, "w+")
         console = Console(file=file)
     else:
         console = Console()
 
-    colored = (
-        True  # If the output isn't colored, we need to show the data in number format
-    )
-
     if path:
-        colored = False
+        plain = False
     if output == "json":
         result = json.dumps(tasks, indent=4)
         console.print_json(result)
 
     elif output == "text":
         console.print("[bold]Tasks")
         console.rule()
@@ -114,12 +110,12 @@
         for task in tasks:
             console.print(
                 f"{index}) Title: {task['title']}\n- Description: {task['description']}\n- Deadline: {task['deadline']}\n",
             )
             index += 1
 
     else:
-        result = get_table(tasks, colored)
+        result = get_table(tasks, plain)
         console.print(result)
 
     if file:
         file.close()
```

### Comparing `special-octo-robot-0.0.6/app/database.py` & `special-octo-robot-0.0.7/app/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sqlite3
 
-from .constants import path
+from .constants import db_path
 
 
 def initialize():
     """
     Initialize the database with all the necessary tables.
     """
-    conn = sqlite3.connect(path)
+    conn = sqlite3.connect(db_path)
     cur = conn.cursor()
     cur.execute(
         """CREATE TABLE tasks(
         id INTEGER PRIMARY KEY AUTOINCREMENT,
         title VARCHAR NOT NULL, parent_id INTEGER,
         description TEXT,
         status VARCHAR DEFAULT 'Pending',
@@ -40,36 +40,47 @@
     group_clause: str = "",
     order_by: str = "",
 ) -> list:
     """
     List data from a table.
     """
     query = f"SELECT {', '.join(columns)} FROM {table} {where_clause} {group_clause} {order_by}"
-    conn = sqlite3.connect(path)
+    conn = sqlite3.connect(db_path)
     cur = conn.cursor()
     res = cur.execute(query).fetchall()
     return res
 
 
 def insert_into_table(table: str, columns: list, values: list) -> None:
     """
     Insert data into a table.
     """
     query = f"INSERT INTO {table} ({', '.join(columns)}) VALUES ({', '.join(values)})"
-    conn = sqlite3.connect(path)
+    conn = sqlite3.connect(db_path)
     cur = conn.cursor()
     cur.execute(query)
     conn.commit()
 
 
 def update_table(table: str, new_data: dict) -> None:
     """
     Update Values Of Given Table
     """
     set_clause = ", ".join(
         [f"{key} = {value}" for key, value in new_data.items() if key != "id"],
     )
     query = f"UPDATE {table} SET {set_clause} WHERE id = {new_data['id']}"
-    conn = sqlite3.connect(path)
+    conn = sqlite3.connect(db_path)
+    cur = conn.cursor()
+    cur.execute(query)
+    conn.commit()
+
+
+def delete_task(task_id: int) -> None:
+    """
+    Delete Task From Database
+    """
+    query = f"DELETE FROM tasks WHERE id = {task_id}"
+    conn = sqlite3.connect(db_path)
     cur = conn.cursor()
     cur.execute(query)
     conn.commit()
```

### Comparing `special-octo-robot-0.0.6/devcord.py` & `special-octo-robot-0.0.7/devcord.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import os
 from datetime import datetime
 
 import click
 
 import app.application as application
+from app.config import get_config
+from app.config import initialize_config
 from app.console import print_tasks
+from app.constants import config_path
+from app.constants import db_path
 from app.constants import path
+from app.database import delete_task
 from app.database import initialize
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 @click.pass_context
@@ -24,17 +29,21 @@
                 "Error: Could not find the path to the database, raise an issue with the developers.",
                 fg="red",
             ),
         )
         ctx.abort()
         return
 
-    if not os.path.exists(path):
-        os.makedirs(os.path.dirname(path), exist_ok=True)
+    if not os.path.exists(db_path):
+        os.makedirs(path, exist_ok=True)
         initialize()
+    if not os.path.exists(config_path):
+        ctx.obj["config"] = initialize_config(config_path)
+    else:
+        ctx.obj["config"] = get_config(config_path)
 
 
 @cli.command()
 @click.pass_context
 @click.option("-l", "--list", is_flag=True, help="List all the tasks")
 @click.option("-a", "--add", help="Add a new task", type=str)
 @click.option("-d", "--desc", is_flag=True, help="Add a description to a task")
@@ -121,18 +130,18 @@
                 inprogress=inprogress,
                 completed=completed,
                 pending=pending,
                 label=label,
             ),
             output,
             path,
+            ctx.obj["config"]["unicode"],
         )
     elif add:
         description = "No given description"
-        add = add
         if desc:
             description = click.edit()
         if parent:
             val = application.search_task(parent)
             if not val:
                 click.echo(
                     click.style(
@@ -185,28 +194,45 @@
 )
 @click.option(
     "-st",
     "--subtasks",
     is_flag=True,
     help="List All Subtask Of Task",
 )
+@click.option("-dl", "--delete", is_flag=True, help="Delete task")
+@click.option("-n", "--name", help="Change the name of the task", type=str)
+@click.option("-p", "--priority", help="Change the priority of the task", type=int)
+@click.option("-dd", "--deadline", help="Change the deadline of the task", type=str)
+@click.option("-lb", "--label", help="Change the label of the task", type=str)
 def task(
     ctx,
     task_id,
     desc=None,
     inprogress=None,
     completed=None,
     pending=None,
     subtasks=None,
+    delete=None,
+    name=None,
+    priority=None,
+    deadline=None,
+    label=None,
 ):
     """
     Modify a specific task.
     """
+    if delete:
+        delete_task(task_id)
+        return
+
     if subtasks:
-        print_tasks(application.get_subtasks(task_id))
+        print_tasks(
+            tasks=application.get_subtasks(task_id),
+            plain=ctx.obj["config"]["unicode"],
+        )
         return
 
     current_task = application.search_task(task_id)
     if not current_task:
         click.echo(
             click.style(
                 "Error: Task does not exist.",
@@ -224,14 +250,32 @@
     if inprogress:
         current_task["status"] = "In Progress"
     elif pending:
         current_task["status"] = "Pending"
     elif completed:
         current_task["status"] = "Completed"
 
+    if name:
+        current_task["title"] = name
+    if priority:
+        current_task["priority"] = priority
+    if label:
+        current_task["label"] = label
+    if deadline:
+        try:
+            current_task["deadline"] = convert_to_db_date(deadline)
+        except ValueError:
+            click.echo(
+                click.style(
+                    'Error: Invalid date format, please use "dd/mm/yyyy".',
+                    fg="red",
+                ),
+            )
+            return
+
     # update values in db
     application.update_task(current_task)
 
 
 def convert_to_db_date(date_str):
     # Convert date from "dd/mm/yyyy" to "YYYY-MM-DD"
     date_obj = datetime.strptime(date_str, "%d/%m/%Y")
```

### Comparing `special-octo-robot-0.0.6/setup.py` & `special-octo-robot-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.6/special_octo_robot.egg-info/PKG-INFO` & `special-octo-robot-0.0.7/special_octo_robot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: Windows
 Platform: MacOS X
@@ -191,7 +191,44 @@
 
 Mark as pending:
 
 ```bash
 $ devcord task 10 -pd
 $ devcord task 10 --pending
 ```
+
+
+Delete Task:
+
+```bash
+$ devcord task 10 -dl
+$ devcord task 10 --delete
+```
+
+
+Modify Title:
+
+```bash
+$ devcord task 10 -n "new title"
+$ devcord task 10 --name "new title"
+```
+
+Modify Priority:
+
+```bash
+$ devcord task 10 -p 3
+$ devcord task 10 --priority 3
+```
+
+Modify Deadline:
+
+```bash
+$ devcord task 10 -dd "dd/mm/yyyy"
+$ devcord task 10 --deadline "dd/mm/yyyy"
+```
+
+Modify Labels:
+
+```bash
+$ devcord task 10 -lb "label"
+$ devcord task 10 --label "label"
+```
```

