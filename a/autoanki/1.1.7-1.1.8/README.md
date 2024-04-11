# Comparing `tmp/autoanki-1.1.7.tar.gz` & `tmp/autoanki-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.1.7.tar", last modified: Sun Apr  7 23:12:41 2024, max compression
+gzip compressed data, was "autoanki-1.1.8.tar", last modified: Thu Apr 11 22:10:28 2024, max compression
```

## Comparing `autoanki-1.1.7.tar` & `autoanki-1.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.601729 autoanki-1.1.7/
--rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.7/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.1.7/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     4836 2024-04-07 23:12:41.601662 autoanki-1.1.7/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     4303 2024-04-05 18:36:02.000000 autoanki-1.1.7/README.md
--rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.7/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      699 2024-04-07 23:12:41.602012 autoanki-1.1.7/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.593366 autoanki-1.1.7/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.594681 autoanki-1.1.7/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)     6488 2024-04-07 23:12:30.000000 autoanki-1.1.7/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.597349 autoanki-1.1.7/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     7249 2024-04-07 18:35:54.000000 autoanki-1.1.7/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.7/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.598800 autoanki-1.1.7/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    13764 2024-04-07 20:46:36.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/book_table.sql
--rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/book_table_view.sql
--rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.7/src/autoanki/DatabaseManager/databases_init.sql
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.599676 autoanki-1.1.7/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     4175 2024-04-07 18:11:20.000000 autoanki-1.1.7/src/autoanki/DeckManager/DeckManager.py
--rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.7/src/autoanki/DeckManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)     2676 2024-04-06 21:14:34.000000 autoanki-1.1.7/src/autoanki/DeckManager/template_decks.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.600967 autoanki-1.1.7/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)     4390 2024-04-07 20:47:34.000000 autoanki-1.1.7/src/autoanki/Dictionary/CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-05 16:04:00.000000 autoanki-1.1.7/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)     5320 2024-04-07 04:26:04.000000 autoanki-1.1.7/src/autoanki/Dictionary/YellowBridgeDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.7/src/autoanki/Dictionary/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.7/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-07 23:12:41.601398 autoanki-1.1.7/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     4836 2024-04-07 23:12:41.000000 autoanki-1.1.7/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)      878 2024-04-07 23:12:41.000000 autoanki-1.1.7/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-07 23:12:41.000000 autoanki-1.1.7/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.7/src/autoanki.egg-info/not-zip-safe
--rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-07 23:12:41.000000 autoanki-1.1.7/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.992928 autoanki-1.1.8/
+-rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.8/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.1.8/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     5008 2024-04-11 22:10:28.992849 autoanki-1.1.8/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     4475 2024-04-10 21:23:08.000000 autoanki-1.1.8/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.8/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      699 2024-04-11 22:10:28.993223 autoanki-1.1.8/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.984964 autoanki-1.1.8/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.986823 autoanki-1.1.8/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)    10590 2024-04-10 20:36:12.000000 autoanki-1.1.8/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.988498 autoanki-1.1.8/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     7455 2024-04-10 20:32:34.000000 autoanki-1.1.8/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.8/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.989820 autoanki-1.1.8/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    15691 2024-04-11 21:45:12.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/book_table.sql
+-rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/book_table_view.sql
+-rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/databases_init.sql
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.990916 autoanki-1.1.8/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     4210 2024-04-08 21:24:06.000000 autoanki-1.1.8/src/autoanki/DeckManager/DeckManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.8/src/autoanki/DeckManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)     2676 2024-04-06 21:14:34.000000 autoanki-1.1.8/src/autoanki/DeckManager/template_decks.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.992149 autoanki-1.1.8/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)     4627 2024-04-11 22:10:15.000000 autoanki-1.1.8/src/autoanki/Dictionary/CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-05 16:04:00.000000 autoanki-1.1.8/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)     5320 2024-04-07 04:26:04.000000 autoanki-1.1.8/src/autoanki/Dictionary/YellowBridgeDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.8/src/autoanki/Dictionary/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.8/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.992569 autoanki-1.1.8/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     5008 2024-04-11 22:10:28.000000 autoanki-1.1.8/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)      878 2024-04-11 22:10:28.000000 autoanki-1.1.8/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-11 22:10:28.000000 autoanki-1.1.8/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.8/src/autoanki.egg-info/not-zip-safe
+-rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-11 22:10:28.000000 autoanki-1.1.8/src/autoanki.egg-info/top_level.txt
```

### Comparing `autoanki-1.1.7/LICENSE.txt` & `autoanki-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.7/PKG-INFO` & `autoanki-1.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.7
+Version: 1.1.8
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -72,54 +72,35 @@
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
 1. BookCleaner: Cleans the input coming in from files that the user supplies 
 2. DatabaseManager: Takes the cleaned input and puts it into the database
 3. Dictionary: Finds definitions for words in the database
 4. DeckManager: Creates Decks
 
-### Database:
-There are 3 different types of tables in the DB, 
-1. dictionary, which holds all the definitions and other information 
-2. book_list, which holds the titles of the books in the database 
-3. book, based off of the name of the book, and holds the words in the book to find in the dictionary
-
-#### dictionary:
-- word_id
-- word
-- word_traditional
-- word_type (noun, verb, etc.)
-- pinyin
-- pinyin_numbers
-- number_of_strokes
-- sub_components
-- frequency
-- hsk_level
-- top_level
-- audio_path
-- image_path
-- definition
-
-<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/dictionary-table.jpg?raw=true" alt="Dictionary table" width="80%"/>
-
-#### book_list:
-- book_name
-- book_table_name
-- language
-
+### Dictionary
+This is an abstract class that can be implemented with the following methods
+- `__init__(debug_level)`
+- `find_word(word)` - Returns None, or a list of paramaters that match the input of DatabaseManager.update_definition()
+- `size()` - Number of entries in the dictionary
+
+There is one dictionary included as the default: an endpoint to [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict). 
+I have local versions of other dictionaries with copyrighted data, which I can not upload.
+
+### Database
+There are 3 different types of tables in the DB:
+- `dictionary` contains a information about each word, including the pinyin, traditional characters, and a definition
+- `book_list` contains the book name, table name, and language for each book added
+- `book` contains the book table id, dictionary word id, and the number of appearances for each word in the book
+  
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/dictionary-table.jpg?raw=true" alt="Dictionary table" width="60%"/>
 <img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_list_table.jpg?raw=true" alt="Book list table" width="50%"/>
-
-### book
- - book_table_word_id
- - dictionary_word_id
- - number_of_appearances 
-
-<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_table.jpg?raw=true" alt="Book table" width="80%"/>
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_table.jpg?raw=true" alt="Book table" width="40%"/>
 
 ## Planned features
 - See ROADMAP.md
 
 ## Other Info
 
 If you would like to get involved, or learn more information, reading Anki documentation is really important, especially the [Getting Started](https://docs.ankiweb.net/getting-started.html)
 
-To get definitions, this autoanki uses the [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict) under the creative commons licence. 
+To get definitions, this autoanki uses the [CC-CEDICT]() under the creative commons licence.
```

### Comparing `autoanki-1.1.7/README.md` & `autoanki-1.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -57,54 +57,35 @@
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
 1. BookCleaner: Cleans the input coming in from files that the user supplies 
 2. DatabaseManager: Takes the cleaned input and puts it into the database
 3. Dictionary: Finds definitions for words in the database
 4. DeckManager: Creates Decks
 
-### Database:
-There are 3 different types of tables in the DB, 
-1. dictionary, which holds all the definitions and other information 
-2. book_list, which holds the titles of the books in the database 
-3. book, based off of the name of the book, and holds the words in the book to find in the dictionary
-
-#### dictionary:
-- word_id
-- word
-- word_traditional
-- word_type (noun, verb, etc.)
-- pinyin
-- pinyin_numbers
-- number_of_strokes
-- sub_components
-- frequency
-- hsk_level
-- top_level
-- audio_path
-- image_path
-- definition
-
-<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/dictionary-table.jpg?raw=true" alt="Dictionary table" width="80%"/>
-
-#### book_list:
-- book_name
-- book_table_name
-- language
-
+### Dictionary
+This is an abstract class that can be implemented with the following methods
+- `__init__(debug_level)`
+- `find_word(word)` - Returns None, or a list of paramaters that match the input of DatabaseManager.update_definition()
+- `size()` - Number of entries in the dictionary
+
+There is one dictionary included as the default: an endpoint to [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict). 
+I have local versions of other dictionaries with copyrighted data, which I can not upload.
+
+### Database
+There are 3 different types of tables in the DB:
+- `dictionary` contains a information about each word, including the pinyin, traditional characters, and a definition
+- `book_list` contains the book name, table name, and language for each book added
+- `book` contains the book table id, dictionary word id, and the number of appearances for each word in the book
+  
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/dictionary-table.jpg?raw=true" alt="Dictionary table" width="60%"/>
 <img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_list_table.jpg?raw=true" alt="Book list table" width="50%"/>
-
-### book
- - book_table_word_id
- - dictionary_word_id
- - number_of_appearances 
-
-<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_table.jpg?raw=true" alt="Book table" width="80%"/>
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_table.jpg?raw=true" alt="Book table" width="40%"/>
 
 ## Planned features
 - See ROADMAP.md
 
 ## Other Info
 
 If you would like to get involved, or learn more information, reading Anki documentation is really important, especially the [Getting Started](https://docs.ankiweb.net/getting-started.html)
 
-To get definitions, this autoanki uses the [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict) under the creative commons licence. 
+To get definitions, this autoanki uses the [CC-CEDICT]() under the creative commons licence.
```

### Comparing `autoanki-1.1.7/setup.cfg` & `autoanki-1.1.8/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = autoanki
-version = 1.1.7
+version = 1.1.8
 author = Jarvis Coghlin
 author_email = jarviscoghlin@gmail.com
 description = Automatically make Anki Decks for Chinese text
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/timmy6figures/autoanki
 project_urls =
```

### Comparing `autoanki-1.1.7/src/autoanki/AutoAnki.py` & `autoanki-1.1.8/src/autoanki/AutoAnki.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import jieba
 
 from autoanki.Dictionary.YellowBridgeDictionary import YellowBridgeDictionary
 
 from .BookCleaner import BookCleaner
 from .DatabaseManager import DatabaseManager
 from .Dictionary import CEDictionary
 from .DeckManager import DeckManager
@@ -21,27 +22,29 @@
     level=logging.WARNING,
     format=f'{GREEN}%(asctime)s{RESET} {RED}%(levelname)8s{RESET} {YELLOW}%(name)16s{RESET}: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
 )
 
 class AutoAnki:
 
-    def __init__(self, database_filepath='autoanki.db', debug_level=20):
+    def __init__(self, database_filepath='autoanki.db', debug_level=20, force=False):
         """
         Creates an instance of autoanki.
-        This creates a book cleaner, database connection, and deck maker
+        This creates a book cleaner, database connection, dictioary connection, and deck maker
         :param database_filepath: The filepath for the database
         :param logging_level: between 0 (DEBUG) and 50(CRITICAL)
+        :param `force`: Skip conformations for cleaning large numbers of files
         """
         self.logger = logging.getLogger('autoanki')
         self.logger.setLevel(debug_level)
         self.logger.debug(f"logger active")
         self.logger.info("Connecting to database...")
 
-        self.book_cleaner = BookCleaner(debug_level)
+        self.force = force
+        self.book_cleaner = BookCleaner(debug_level, self.force)
 
         self.dictionary = CEDictionary(debug_level)
         self.online_dictionary = YellowBridgeDictionary(debug_level)
 
         self.database_filepath = database_filepath
         if not DatabaseManager.is_database(database_filepath):
             self.logger.info("Creating database...")
@@ -60,15 +63,15 @@
         :param book_name: The name of the book being added e.g. "Lost Prince"
         :return:
         """
         self.logger.debug(f"autoanki: Adding book from [{book_path}]")
 
         # Clean the book
         if not self.book_cleaner.clean(book_path):
-            # logger.warning("autoanki: Unable to clean book [" + book_name + "].")
+            # self.logger.warning("autoanki: Unable to clean book [" + book_name + "].")
             return
 
         # Add the book to the database
         if not self.database_manager.add_book(book_path, book_name):
             self.logger.warning("Unable to add [" + book_name + "] to database.")
             return
 
@@ -85,33 +88,119 @@
         # TODO Make progress bar for unfinished records
         self.logger.info("Checking for records...")
         self.database_manager.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
         response_rows = self.database_manager.cursor.fetchall()
         if len(response_rows) > 0:
             self.logger.info("Adding " + str(len(response_rows)) + " rows to dictionary table")
             for row in response_rows:
-                word = row[0]
+                word = str(row[0])
 
-                # self.logger.debug(f"Finding: [{word}]...")
+                # self.logger.info(f"Finding: [{word}]...")
 
                 # self.logger.debug("Trying local dictionary...")
                 params = self.dictionary.find_word(word)
                 if params:
                     # self.logger.debug(f"✅Found: [{params[8]}]")
                     self.database_manager.update_definition(params)
                     continue
 
+                subwords = jieba.cut(word)
+                if len(next(subwords)) == len(word):
+                    pass 
+                else: 
+                    self.database_manager.remove_word(word)
+                    subwords = jieba.cut(word)
+                    self.logger.debug(f"✅Splitting and inserting: [{word}]")
+                    for subword in subwords:
+                        self.database_manager.insert_word(subword)
+                        params = self.dictionary.find_word(subword)
+                        if params:
+                            self.logger.debug(f"✅  Found: [{params[8]}]")
+                            self.database_manager.update_definition(params)
+                        else:
+                            self.logger.debug(f"❌Could not find: [{word}]")
+
+                    continue
+
+                CHINESE_NUMBERS = "第一二两三四五五六七八九十百千万满"
+                # Remove all numbers from the front
+                # Lots of the words follow the following format:
+                #   Number + Subject
+                old_word = "" 
+                temp_word = word
+                while old_word != temp_word:
+                    old_word = temp_word 
+                    if len(temp_word) == 0:
+                        break
+                    if temp_word[0] in CHINESE_NUMBERS:
+                        temp_word = temp_word[1:]
+                params = self.dictionary.find_word(temp_word)
+                if params:
+                    self.database_manager.remove_word(word)
+                    self.database_manager.insert_word(temp_word)
+                    self.logger.debug(f"✅  Found: [{params[8]}]")
+                    self.database_manager.update_definition(params)
+                    continue
+
+                # Can we remove some modifiers and get it?
+                stripped_word = word.lstrip('小')
+                stripped_word = stripped_word.lstrip('大')
+                stripped_word = stripped_word.lstrip('这')
+                stripped_word = stripped_word.lstrip('那')
+                stripped_word = stripped_word.lstrip('不')
+                stripped_word = stripped_word.lstrip('几')
+                stripped_word = stripped_word.lstrip('无')
+                stripped_word = stripped_word.lstrip('没')
+                stripped_word = stripped_word.lstrip('全')
+                stripped_word = stripped_word.lstrip('上')
+                stripped_word = stripped_word.lstrip('下')
+                stripped_word = stripped_word.lstrip('太')
+                params = self.dictionary.find_word(stripped_word)
+                if params:
+                    self.database_manager.remove_word(word)
+                    self.database_manager.insert_word(stripped_word)
+                    self.logger.debug(f"✅  Found: [{params[8]}]")
+                    self.database_manager.update_definition(params)
+                    continue
+
+                # TODO 2 repeated, 1
+                # 点点头
+                # 长长的
+
+                # TODO 的 at the end
+
+                # TODO 2 repeated, 2 repeated
+                # 起起伏伏
+
+                # Nuclear option. TODO
+                if len(word) == 2:
+                    self.database_manager.remove_word(word)
+
+                    self.database_manager.insert_word(word[0])
+                    params = self.dictionary.find_word(word[0])
+                    if params:
+                        self.logger.debug(f"✅  Found: [{params[8]}]")
+                        self.database_manager.update_definition(params)
+                        
+
+                    self.database_manager.insert_word(word[1])
+                    params = self.dictionary.find_word(word[1])
+                    if params:
+                        self.logger.debug(f"✅  Found: [{params[8]}]")
+                        self.database_manager.update_definition(params)
+
+
                 # self.logger.debug("Trying YellowBridge...")
                 # params = self.online_dictionary.find_word(word)
                 # if params:
                     # self.logger.debug(f"✅Found: [{word}]")
                     # self.database_manager.update_definition(params)
                     # continue
 
-                self.logger.info(f"❌Could not find: [{word}]")
+                self.logger.debug(f"❌Could not find: [{word}]")
 
         else:
             self.logger.info("No new rows to complete in dictionary table")
 
     def deck_settings(self,
                       inclue_traditional = True, 
                       inclue_part_of_speech = True,
```

### Comparing `autoanki-1.1.7/src/autoanki/BookCleaner/BookCleaner.py` & `autoanki-1.1.8/src/autoanki/BookCleaner/BookCleaner.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,24 @@
                      "。",
                      "\n"]
 
 
 
 class BookCleaner:
 
-    def __init__(self, debug_level):
+    def __init__(self, debug_level, force=False):
         """ Internal tool used to sanatize input
         Use `clean(bookpath)` to sanatize files and remove junk data
+        `force` Ignore confirmations on if you want to clean >50 files
         """
         self.logger = logging.getLogger('autoanki.bookcleaner')
         self.logger.setLevel(debug_level)
         self.file_list = []
         self.bookpath = ""
+        self.force = force
 
     def clean(self, bookpath: str) -> None | list[str]:
         """
         Cleans the files contained in the bookpath. If bookpath is a single file, clean it.
         Args: 
             `bookpath: filepath of files to be cleaned`
         Return: 
@@ -45,15 +47,15 @@
                     # Only clean files that are not in cleaned_files directory
                     in_cleaned = str(root).find(CLEANED_FILES_DIRECTORY) != -1
                     if not in_cleaned:
                         if '.txt' in file:
                             dirty_files.append(os.path.join(root, file))
 
             # Check this cleaning won't be mean to the CPU
-            if len(dirty_files) > 50:
+            if len(dirty_files) > 50 and not self.force:
                 yn = input("Over 50 files. Are you sure you want to convert this many files? (Y/N)")
                 if yn.lower() != 'y':
                     return None
 
         # Now we have a list of files to convert in a list
         cleaned_files = []
 
@@ -83,16 +85,19 @@
             # TODO I'm suspicious that this works every time
             new_filepath = os.path.join(cleaned_files_root, '/'.join(filepath.split('/')[2:]))
         # self.logger.debug(f"Old filepath: [{filepath}]")
         # self.logger.debug(f"New filepath: [{new_filepath}]")
 
         # Clean page file of characters that may cause issues.
         page_file = open(filepath, encoding='utf-8')
-        page_sentences = page_file.read().split("。")
-        # f = open("test.txt", "w", encoding='utf-8')
+        try: 
+            page_sentences = page_file.read().split("。")
+        except:
+            self.logger.error(f"Critical error cleaning file: [{filepath}]")
+            return
         cleaned_file = open(new_filepath, "w", encoding='utf-8')
 
         for page_sentence in page_sentences:
             # Clean string
             page_sentence = page_sentence\
                 .lstrip()\
                 .rstrip()\
```

### Comparing `autoanki-1.1.7/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.1.8/src/autoanki/DatabaseManager/DatabaseManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 
 from pathlib import Path
 import jieba
 import chinese_converter
 
 from autoanki.BookCleaner.BookCleaner import CLEANED_FILES_DIRECTORY
 
-CHINESE_PUNC = "！？｡。＂＃＄％＆＇（）＊＋，－／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏."
-PUNC = "™∞•◎ "
+CHINESE_PUNC = "ｗ９ｌｉｔｂｎｅｐ ！？◇｡。．ｈ＂＃＄％＆＇（）＊＋，－／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏."
+PUNC = "™∞•◎ ♦⑽]■①"
+CHINESE_NUMBERS = "第一二两三四五六七八九十百千万满"
 
 class DatabaseManager:
 
     def __init__(self, database_path, debug_level):
         self.logger = logging.getLogger('autoanki.dbmngr')
         self.logger.setLevel(debug_level)
         if not os.path.exists(database_path):
@@ -62,14 +63,15 @@
     def create_database(database_path):
         """
         Creates an autoanki database file, including all tables needed for autoanki
         `database_path` The path to the database to create
         """
         logger = logging.getLogger('autoanki.dbmngr')
         logger.info("Creating database [" + database_path + "]")
+        # TODO Fix this logger
         path = os.path.join(os.path.dirname(__file__), 'databases_init.sql')
         try:
             with open(path, 'r') as sql_file:
                 sql_script = sql_file.read()
             connection = sqlite3.connect(database_path)
             cursor = connection.cursor()
             cursor.executescript(sql_script)
@@ -110,27 +112,53 @@
     def add_file_to_database(self, filepath, table_name):
         """
         Adds every word in a file to both the dictionary table and the book's table
         `filepath` The path to the file
         `table_name` The name of the table to add the words to.
             This should be the same for every wile in a given book
         """
-        self.logger.info(f"Adding file {filepath} to database...")
-
+        self.logger.info(f"Adding [{filepath}] to database...")
 
         word_appearances = {}
         with open(filepath,'r',encoding='utf-8') as f:
             line = " "
             while line:
                 line = f.readline()
                 if not line:
                     continue
                 words = jieba.lcut(line)
                 for word in words:
 
+                    # TODO There is a lot of shenanigans happening in this section. 
+                    #   This should be split into a Chinese-spesific file, and 
+                    #   some of these rules should be re-evaluated
+                    word = word.lstrip("第")
+                    word = word.lstrip("几")
+
+                    # Repeated characters (always?) contain the same meaning as one, just varied slightly
+                    # 人人 = everyone
+                    if len(word) == 2 and word[0] == word[1]:
+                        word = word[0]
+
+                    # Some gramatical patterns:
+                    if len(word) > 2 and word[0] == "在" and word[-1] == "上":
+                        word = word[1:-2]
+
+
+                    # Remove all numbers from the front
+                    # Lots of the words follow the following format:
+                    #   Number + Subject
+                    old_word = "" 
+                    while old_word != word:
+                        old_word = word
+                        if len(word) == 0:
+                            break
+                        if word[0] in CHINESE_NUMBERS:
+                            word = word[1:]
+
                     # Remove puncuation
                     word = word.translate(str.maketrans('', '', punctuation))
 
                     is_ascii = len(word) == len(word.encode())
 
                     is_ascii_special = False
                     if len(word) == 1:
@@ -151,17 +179,15 @@
         self.cursor.execute(f"SELECT word FROM dictionary")
         self.connection.commit()
         dictionary_words = self.cursor.fetchall()
         self.logger.info(f"{len(word_appearances.items())} words in file. {len(dictionary_words)} in dictionary.")
 
         for word, appearances in word_appearances.items():
             if (word,) not in dictionary_words:
-                # self.logger.debug("Adding word...")
-                self.cursor.execute(f"INSERT INTO dictionary (word) VALUES (?)", [word])
-                self.connection.commit()
+                self.insert_word(word)
 
         # Make a dictionary of word ids from dictionary
         self.cursor.execute(f"SELECT word_id, word FROM dictionary")
         result = self.cursor.fetchall()
         word_id_dict = {}
         for line in result:
             word_id_dict[line[1]] = line[0]
@@ -194,14 +220,31 @@
             else:
                 self.cursor.execute(f"INSERT INTO {table_name} (dictionary_word_id, number_of_appearances) "
                                     f"VALUES (?,?)", [dictionary_word_id, word_appearances[word]])
                 self.connection.commit()
 
         # self.logger.debug("Done adding file to database")
 
+    def insert_word(self, word):
+        # TODO Doing this breaks the `number_of_appearances`. This is a temporary fix
+        self.cursor.execute("SELECT word FROM dictionary WHERE word = ?", [word])
+        all_rows = self.cursor.fetchall()
+        
+        if len(all_rows) == 0:
+            # self.logger.info("  Inserting")
+            self.cursor.execute(f"INSERT INTO dictionary (word) VALUES (?)", [word])
+            self.connection.commit()
+
+    def remove_word(self, word:str):
+        if '*' in word:
+            self.logger.info(f"Not executing: [{word}]. Star in command")
+            return
+        self.cursor.execute(f"DELETE FROM dictionary WHERE word=(?)", [word])
+        self.connection.commit()
+
     def add_book(self, bookpath: str, book_name: str):
         """
         Adds a file to the autoanki database. This involves the following steps:\n
         1 - Add book to the book_list table
         2 - Add all the files in "bookpath" to the definitions table and book table
         3 - Add book to book_list property
```

### Comparing `autoanki-1.1.7/src/autoanki/DatabaseManager/databases_init.sql` & `autoanki-1.1.8/src/autoanki/DatabaseManager/databases_init.sql`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.7/src/autoanki/DeckManager/DeckManager.py` & `autoanki-1.1.8/src/autoanki/DeckManager/DeckManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
             if not pinyin:
                 pinyin = "Not found"
             if not definition:
                 definition = "Not found"
 
             note = genanki.Note(
                 model=template_decks.CHINESE_CARD_MODEL,
+                tags=['autoanki'],
                 fields=[word, word_traditional, pinyin, definition],
                 # sort_field can be used to sort when the cards appear.
                 # By default they are shown in the order they are addeed, so this is not currently used
                 sort_field=1,
 
             )
             self.deck.add_note(note)
```

### Comparing `autoanki-1.1.7/src/autoanki/DeckManager/template_decks.py` & `autoanki-1.1.8/src/autoanki/DeckManager/template_decks.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.7/src/autoanki/Dictionary/CEDictionary.py` & `autoanki-1.1.8/src/autoanki/Dictionary/CEDictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,28 @@
     'w':'puncuation',
 }
 
 class CEDictionary(Dictionary):
 
     def __init__(self, debug_level):
         """Chinese to English Dictionary
-
+        Parser for the CC-CEDICT Dictionary:
+            https://www.mdbg.net/chinese/dictionary?page=cedict
+        This is a file containing 122,839 entries
         """
         self.logger = logging.getLogger('autoanki.cedict')
         self.logger.setLevel(debug_level)
-        self.logger.info("Loading Chinese Dictionary")
+        self.logger.info("Loading Chinese Dictionary (CEDictionary)")
         self.dict = self._parse_file()
-        self.logger.info("Done!")
+        self.logger.debug("Done!")
         
         pass
 
     def _parse_file(self) -> dict[str, dict]:
-        self.logger.info("Parsing file...")
+        self.logger.debug("Parsing file...")
         if not path.isfile(PATH_TO_FILE):
             self.logger.critical("Could not open dictionary file")
 
         # TODO Some entries use a dot in the midde
         #   e.g. 哈利·波特
         #   this does not currently match
         definitions = {}
@@ -107,14 +109,15 @@
         """
         Find a word in the dictionary. This can be simplified, or traditional
         `return` Paramaters that get passed to the database
         """
         
         # Convert the word to simplified if needed
         word = chinese_converter.to_simplified(word)
+        # self.logger.info(f"[{word}] [{word in self.dict}]")
 
         if word in self.dict:
             """
             traditional_script = params[0]\n
             word_type = params[1]\n
             pinyin = params[2]\n
             pinyin_numbers = params[3]\n
```

### Comparing `autoanki-1.1.7/src/autoanki/Dictionary/YellowBridgeDictionary.py` & `autoanki-1.1.8/src/autoanki/Dictionary/YellowBridgeDictionary.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.7/src/autoanki.egg-info/PKG-INFO` & `autoanki-1.1.8/src/autoanki.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.7
+Version: 1.1.8
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -72,54 +72,35 @@
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
 1. BookCleaner: Cleans the input coming in from files that the user supplies 
 2. DatabaseManager: Takes the cleaned input and puts it into the database
 3. Dictionary: Finds definitions for words in the database
 4. DeckManager: Creates Decks
 
-### Database:
-There are 3 different types of tables in the DB, 
-1. dictionary, which holds all the definitions and other information 
-2. book_list, which holds the titles of the books in the database 
-3. book, based off of the name of the book, and holds the words in the book to find in the dictionary
-
-#### dictionary:
-- word_id
-- word
-- word_traditional
-- word_type (noun, verb, etc.)
-- pinyin
-- pinyin_numbers
-- number_of_strokes
-- sub_components
-- frequency
-- hsk_level
-- top_level
-- audio_path
-- image_path
-- definition
-
-<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/dictionary-table.jpg?raw=true" alt="Dictionary table" width="80%"/>
-
-#### book_list:
-- book_name
-- book_table_name
-- language
-
+### Dictionary
+This is an abstract class that can be implemented with the following methods
+- `__init__(debug_level)`
+- `find_word(word)` - Returns None, or a list of paramaters that match the input of DatabaseManager.update_definition()
+- `size()` - Number of entries in the dictionary
+
+There is one dictionary included as the default: an endpoint to [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict). 
+I have local versions of other dictionaries with copyrighted data, which I can not upload.
+
+### Database
+There are 3 different types of tables in the DB:
+- `dictionary` contains a information about each word, including the pinyin, traditional characters, and a definition
+- `book_list` contains the book name, table name, and language for each book added
+- `book` contains the book table id, dictionary word id, and the number of appearances for each word in the book
+  
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/dictionary-table.jpg?raw=true" alt="Dictionary table" width="60%"/>
 <img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_list_table.jpg?raw=true" alt="Book list table" width="50%"/>
-
-### book
- - book_table_word_id
- - dictionary_word_id
- - number_of_appearances 
-
-<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_table.jpg?raw=true" alt="Book table" width="80%"/>
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_table.jpg?raw=true" alt="Book table" width="40%"/>
 
 ## Planned features
 - See ROADMAP.md
 
 ## Other Info
 
 If you would like to get involved, or learn more information, reading Anki documentation is really important, especially the [Getting Started](https://docs.ankiweb.net/getting-started.html)
 
-To get definitions, this autoanki uses the [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict) under the creative commons licence. 
+To get definitions, this autoanki uses the [CC-CEDICT]() under the creative commons licence.
```

### Comparing `autoanki-1.1.7/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.1.8/src/autoanki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

