# Comparing `tmp/monterey-0.0.5.tar.gz` & `tmp/monterey-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monterey-0.0.5.tar", last modified: Fri Apr 12 05:37:04 2024, max compression
+gzip compressed data, was "monterey-0.0.6.tar", last modified: Fri Apr 12 05:41:14 2024, max compression
```

## Comparing `monterey-0.0.5.tar` & `monterey-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:37:04.108706 monterey-0.0.5/
--rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:37:04.107789 monterey-0.0.5/PKG-INFO
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:37:04.090917 monterey-0.0.5/monterey/
--rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.5/monterey/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:37:04.099014 monterey-0.0.5/monterey/tools/
--rw-r--r--   0 hammad     (501) staff       (20)      255 2024-04-12 05:02:38.000000 monterey-0.0.5/monterey/tools/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.5/monterey/tools/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.5/monterey/tools/dialogs.py
--rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.5/monterey/tools/frontend.py
--rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.5/monterey/tools/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.5/monterey/tools/live_table.py
--rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.5/monterey/tools/loaders.py
--rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.5/monterey/tools/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.5/monterey/tools/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.5/monterey/tools/progress_bar.py
--rw-r--r--   0 hammad     (501) staff       (20)     5299 2024-04-12 05:36:48.000000 monterey-0.0.5/monterey/tools/text.py
--rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.5/monterey/tools/tools.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:37:04.099512 monterey-0.0.5/monterey.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:37:04.000000 monterey-0.0.5/monterey.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      505 2024-04-12 05:37:04.000000 monterey-0.0.5/monterey.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 05:37:04.000000 monterey-0.0.5/monterey.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-12 05:37:04.000000 monterey-0.0.5/monterey.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 05:37:04.000000 monterey-0.0.5/monterey.egg-info/top_level.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 05:37:04.108918 monterey-0.0.5/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      560 2024-04-12 05:36:35.000000 monterey-0.0.5/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:41:14.918055 monterey-0.0.6/
+-rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:41:14.916849 monterey-0.0.6/PKG-INFO
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:41:14.894184 monterey-0.0.6/monterey/
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.6/monterey/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:41:14.914396 monterey-0.0.6/monterey/tools/
+-rw-r--r--   0 hammad     (501) staff       (20)      255 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/dialogs.py
+-rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/frontend.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/live_table.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/loaders.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.6/monterey/tools/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.6/monterey/tools/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/progress_bar.py
+-rw-r--r--   0 hammad     (501) staff       (20)     7323 2024-04-12 05:40:58.000000 monterey-0.0.6/monterey/tools/text.py
+-rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.6/monterey/tools/tools.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:41:14.915505 monterey-0.0.6/monterey.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      505 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/top_level.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 05:41:14.918861 monterey-0.0.6/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      560 2024-04-12 05:41:05.000000 monterey-0.0.6/setup.py
```

### Comparing `monterey-0.0.5/monterey/tools/cli.py` & `monterey-0.0.6/monterey/tools/cli.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/monterey/tools/dialogs.py` & `monterey-0.0.6/monterey/tools/dialogs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/monterey/tools/frontend.py` & `monterey-0.0.6/monterey/tools/frontend.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/monterey/tools/inputs.py` & `monterey-0.0.6/monterey/tools/inputs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/monterey/tools/live_table.py` & `monterey-0.0.6/monterey/tools/live_table.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/monterey/tools/loaders.py` & `monterey-0.0.6/monterey/tools/loaders.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/monterey/tools/logger.py` & `monterey-0.0.6/monterey/tools/logger.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/monterey/tools/preconditions.py` & `monterey-0.0.6/monterey/tools/preconditions.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/monterey/tools/progress_bar.py` & `monterey-0.0.6/monterey/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/monterey/tools/text.py` & `monterey-0.0.6/monterey/tools/text.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from rich.console import Console
 from rich.panel import Panel
 from rich import box
 from rich.columns import Columns
 from rich.syntax import Syntax
+from rich.emoji import Emoji
+from rich.table import Table
 from art import text2art
 import random
 
 #==============================================================================
 
 class Text:
     """
@@ -14,14 +16,25 @@
     
     Attributes:
         console: A Rich Console instance for styled output.
     """
     def __init__(self):
         self.console = Console()
 
+    def emoji(self, name: str = "thumbs_up", style: str = "bold white"):
+        """
+        Display an emoji using Rich.
+
+        Args:
+            name (str, optional): The name of the emoji. Defaults to "thumbs_up".
+            style (str, optional): The style of the emoji. Defaults to "bold white".
+        """
+        emoji = Emoji(name)
+        self.console.print(emoji, style=style)
+
     def display(self, message: str = None, style: str = "bold white", use_box: bool = False):
             """
             Displays a message on the console.
 
             Args:
                 message (str, optional): The message to be displayed. Defaults to None.
                 style (str, optional): The style of the message. Defaults to "bold white".
@@ -106,15 +119,53 @@
             style (str, optional): The style of the text. Defaults to "bold white".
             underline (str, optional): The character to use for underlining. Defaults to "=".
             overline (str, optional): The character to use for overlining. Defaults to "=".
         """
         self.console.print(message, style=style)
         self.console.print(underline * len(message), style=style)
 
+    def table(self, data: list, title: str = None, title_style: str = "bold yellow", header_style: str = "bold cyan", row_styles: list = None):
+        """
+        Display a set of data as a table using Rich.
+
+        Args:
+            data (list): A list of lists representing the table data.
+            title (str, optional): The title of the table. Defaults to None.
+            title_style (str, optional): The style of the table title. Defaults to "bold yellow".
+            header_style (str, optional): The style of the table header. Defaults to "bold cyan".
+            row_styles (list, optional): A list of styles for each row. Defaults to None.
+        """
+        table = Table(title=title, title_style=title_style, header_style=header_style)
+
+        # Add columns based on the number of elements in the first row
+        for _ in data[0]:
+            table.add_column()
+
+        # Add rows to the table
+        for i, row in enumerate(data):
+            if row_styles and i < len(row_styles):
+                table.add_row(*row, style=row_styles[i])
+            else:
+                table.add_row(*row)
+
+        self.console.print(table)
+
 #==============================================================================
 
 if __name__ == "__main__":
     text = Text()
-    text.splash("hammadpy", art="random")
+    text.art("hammadpy", art="random")
+    text.emoji("thumbs_up", style="bold white")
     text.display("Hello, Rich!", style="bold red", use_box=True)
     text.code("print('Hello, Rich!')", language="python", theme="monokai", line_numbers=True)
-    text.header("Hello, Rich!", style="bold red", underline="-", overline="-")
+    text.header("Hello, Rich!", style="bold red", underline="-", overline="-")
+
+    data = [
+        ["Name", "Age", "Location"],
+        ["Alice", "25", "New York"],
+        ["Bob", "30", "San Francisco"],
+        ["Charlie", "35", "Los Angeles"]
+    ]
+
+    row_styles = ["bold green", "bold blue", "bold magenta", "bold cyan"]
+
+    text.table(data, title="User Information", title_style="bold yellow", header_style="bold cyan", row_styles=row_styles)
```

### Comparing `monterey-0.0.5/monterey/tools/tools.py` & `monterey-0.0.6/monterey/tools/tools.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.5/setup.py` & `monterey-0.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="monterey",
-    version="0.0.05",
+    version="0.0.06",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="monterey tools",
     long_description="""
 Monterey Tools
     """,
     packages=setuptools.find_packages(),
```

