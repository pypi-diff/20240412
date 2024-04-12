# Comparing `tmp/pi-folder-organizer-1.1.0.tar.gz` & `tmp/pi-folder-organizer-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi-folder-organizer-1.1.0.tar", last modified: Mon Apr  8 21:34:05 2024, max compression
+gzip compressed data, was "pi-folder-organizer-2.1.0.tar", last modified: Fri Apr 12 15:20:56 2024, max compression
```

## Comparing `pi-folder-organizer-1.1.0.tar` & `pi-folder-organizer-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:34:05.825415 pi-folder-organizer-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 21:34:02.000000 pi-folder-organizer-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-08 21:34:05.825415 pi-folder-organizer-1.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-04-08 21:34:02.000000 pi-folder-organizer-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:34:05.825415 pi-folder-organizer-1.1.0/pi_folder_organizer/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 21:34:02.000000 pi-folder-organizer-1.1.0/pi_folder_organizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 21:34:02.000000 pi-folder-organizer-1.1.0/pi_folder_organizer/_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13628 2024-04-08 21:34:02.000000 pi-folder-organizer-1.1.0/pi_folder_organizer/pi_folder_organizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:34:05.825415 pi-folder-organizer-1.1.0/pi_folder_organizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-08 21:34:05.000000 pi-folder-organizer-1.1.0/pi_folder_organizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 21:34:05.000000 pi-folder-organizer-1.1.0/pi_folder_organizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:34:05.000000 pi-folder-organizer-1.1.0/pi_folder_organizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 21:34:05.000000 pi-folder-organizer-1.1.0/pi_folder_organizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:34:05.825415 pi-folder-organizer-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-08 21:34:02.000000 pi-folder-organizer-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/pi_folder_organizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/pi_folder_organizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/pi_folder_organizer/_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13779 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/pi_folder_organizer/pi_folder_organizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-12 15:20:56.000000 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 15:20:56.000000 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:20:56.000000 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 15:20:56.000000 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/setup.py
```

### Comparing `pi-folder-organizer-1.1.0/LICENSE` & `pi-folder-organizer-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pi-folder-organizer-1.1.0/PKG-INFO` & `pi-folder-organizer-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-folder-organizer
-Version: 1.1.0
+Version: 2.1.0
 Summary: A Python package for cleaning up cluttered files and organizing them into respective folders.
 Author: Qadeer Ahmad
 Author-email: mrqdeer1231122@gmail.com
 Keywords: python,file organization,file cleanup,cluttered files,folder management,data organization,file management,data cleanup,Python package,developer tools,data processing,file sorting,data structuring,automated file organization,Python library,data management,data handling,file optimization,data optimization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pi-folder-organizer-1.1.0/README.md` & `pi-folder-organizer-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pi-folder-organizer-1.1.0/pi_folder_organizer/pi_folder_organizer.py` & `pi-folder-organizer-2.1.0/pi_folder_organizer/pi_folder_organizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import shutil
+from concurrent.futures import ThreadPoolExecutor
 from ._exceptions import DangerZone
 from ._exceptions import DestinationInsideSourceError
 
 class PiFolderOrganizer:
     """
     A class for organizing files based on their types into separate folders.
 
@@ -30,25 +31,26 @@
     new_counter = {"Images": [], "Documents": []}
     pi_organizer .set_counter(new_counter)
     new_extensions = {"Images": (".png", ".jpg"), "Documents": (".txt", ".docs")}
     pi_organizer .set_extensions(new_extensions)
     pi_organizer .pi_organizer(source_path, destination_path)
     ```
     """
+    
     def __init__(self) -> None:
         # System paths for Linux | Windows | MacOS
         self.__RESTRICTED_PATHS=["/bin","/usr", "/sbin", "/usr/bin", "/usr/sbin", "/etc", "/var/log", "/usr/lib", "/lib", "/tmp",
                           r"C:\Windows", r"C:\Program Files", r"C:\Program Files (x86)", r"C:\Users\Public", r"C:\ProgramData", r"C:\Windows\System32", r"C:\Temp",
                           "/Applications", "/System", "/Library", "/Users", "/var/log", "/private", "/tmp"]
        
     
         self.__counter = {
                 "Images": [],
                 "Audios": [],
-                "MediaFiles": [],
+                "Videos": [],
 
                 "Documents": [],
                 "Compressed": [],
                 "WindowsSoftwares": [],
                 "LinuxSoftwares": [],
                 "MacSoftwares": [],
                 "CodeFiles": [],
@@ -68,15 +70,15 @@
             }
 
         self.__extensions = {
                 "Images": (".png", ".jpg", ".jpeg", ".gif", ".bmp", ".svg",".svgz", ".tiff",".tif",".eps",".psd",
                         ".heic","heif",".ind",".indd",".indt",".raw",".arw",".cr2",".nrw",".k25",".dib",
                         ".jp2", ".j2k", ".jpf", ".jpx", ".jpm", ".mj2",".ico"),
                 "Audios": (".mp3", ".wav", ".ogg", ".aac", ".flac", ".wma",".opus"),
-                "MediaFiles": ('.mov', '.mp2v', '.3gp', '.mpg', '.hevc', '.ogg', '.avi', '.wmv', '.ts', '.ogv', 
+                "Videos": ('.mov', '.mp2v', '.3gp', '.mpg', '.hevc', '.ogg', '.avi', '.wmv', '.ts', '.ogv', 
                             '.swf', '.webp', '.rm', '.m2v', '.h264', '.m2ts', '.xvid', '.flv', '.mpeg', 
                             '.vp9', '.divx', '.mp4', '.webm', '.rmvb', '.avchd', '.dv', '.mpeg2', '.m4v',
                             '.vob', '.mpeg4', '.mkv', '.mpg2', '.h265', '.mxf', '.m1v', '.mts', '.3g2', '.mod'),
                 
                 "Documents": (".pdf",".aspx",".djvu",
                 ".csv",".xlsb",".odp",".doc", ".docx",".docs", ".xls", ".xlsx",".xlsm", ".ppt", ".pptx",".accdb", ".odt", ".ods",
                 ".txt",'.md','.rtf',".inp",".tex",".odf",".env"),
@@ -98,37 +100,41 @@
                 "VirtualMachinesFiles": (".vbox-extpack",'.vdi', '.vmdk', '.vhd', '.vhdx', 
                         '.vdi.bz2', '.vmdk.gz', '.vhd.gz',
                         '.vbox', '.vbox-prev', '.vbox-extpack', '.ovf', '.ova',
                         '.vbox-snAPSHOT', '.sav',
                         '.log','.vbox-tmp', '.vdi-tmp', '.cdr'),
                 "SerializedFiles": (".json", ".pkl", ".npy", ".joblib")
             }
+
     @staticmethod
     def __list_files(folder_path):
         files = []
         for dirpath, _, filenames in os.walk(folder_path):
             for file in filenames:
                 files.append(os.path.join(dirpath, file))
         return files
+
     @staticmethod
     def __get_empty_folders(folder_path):
         empty_folders = []
         for root, dirs, files in os.walk(folder_path, topdown=False):
             if not os.listdir(root):  # Check if the current folder is empty
                 empty_folders.append(root)
             else:
                 # Check if all subfolders are empty
                 all_subfolders_empty = all(os.listdir(os.path.join(root, d)) == [] for d in dirs)
                 if all_subfolders_empty:
                     empty_folders.append(root)
         return empty_folders
+
     @staticmethod
     def __is_subdirectory(parent_path, child_path):
         # Check if child_path is a subdirectory of parent_path
         return os.path.commonpath([parent_path, child_path]) == parent_path
+
     def get_counter(self):
         """
         Returns the current file counter dictionary used by PiFolderOrganizer.
 
         Returns:
         ------
             dict: The current file counter dictionary.
@@ -136,15 +142,16 @@
         Example:
         ------
             >>> pi_organizer = PiFolderOrganizer()
             >>> counter = pi_organizer.get_counter()
         """
 
         return self.__counter
-    def set_counter(self,new_counter:dict) -> dict:
+
+    def set_counter(self, new_counter: dict) -> dict:
         """
         Sets a new file counter dictionary for PiFolderOrganizer.
 
         Args:
         ______
             new_counter (dict): The new file counter dictionary to set.
 
@@ -155,31 +162,33 @@
         Example:
         ------
             >>> pi_organizer = PiFolderOrganizer()
             >>> new_counter = {"Images": [], "Documents": []}
             >>> pi_organizer.set_counter(new_counter)
             >>> counter = pi_organizer.get_counter()
         """
-        new_counter["Others"]=[]
-        self.__counter=new_counter
+        new_counter["Others"] = []
+        self.__counter = new_counter
+
     def get_extensions(self):
         """
         Returns the current file extensions dictionary used by PiFolderOrganizer.
 
         Returns:
         ------
             dict: The current file extensions dictionary.
 
         Example:
         ------
             >>> pi_organizer = PiFolderOrganizer()
             >>> extensions = pi_organizer.get_extensions()
         """
         return self.__extensions
-    def set_extensions(self,new_extensions:dict) -> dict:
+
+    def set_extensions(self, new_extensions: dict) -> dict:
         """
         Sets a new file extensions dictionary for PiFolderOrganizer.
 
         Args:
         ------
             new_extensions (dict): The new file extensions dictionary to set.
 
@@ -190,17 +199,26 @@
         Example:
         ------
             >>> pi_organizer = PiFolderOrganizer()
             >>> new_extensions = {"Images": (".png", ".jpg"), "Documents": (".txt", ".docs")}
             >>> pi_organizer.set_extensions(new_extensions)
             >>> extensions = pi_organizer.get_extensions()
         """
-        self.__extensions=new_extensions
-    
-    def pi_folder_organizer(self,source_path:str,destination_path:str)->None:
+        self.__extensions = new_extensions
+
+    def __move_files(self, category, file_paths, destination_path):
+        category_path = os.path.join(destination_path, category)
+        os.makedirs(category_path, exist_ok=True)
+        for file_path in file_paths:
+            dest_file = os.path.join(category_path, os.path.basename(file_path))
+            shutil.move(file_path, dest_file)
+            print(f"File {os.path.basename(file_path)} moved to {category} folder.")
+        print(20 * "+-*-+")
+
+    def pi_folder_organizer(self, source_path: str, destination_path: str) -> None:
         """
         Organizes files from the source_path into separate folders in the destination_path based on their types.
 
         Parameters:
         ------
         - source_path (str): The path to the folder containing the files to be organized.
         - destination_path (str): The path to the folder where the organized files will be stored.
@@ -234,33 +252,32 @@
         >>> pi_organizer.set_extensions(new_extensions)
         >>> pi_organizer.pi_organizer("/path/to/source_folder", "/path/to/destination_folder")
         
         """
         # Normalize paths
         source_path = os.path.abspath(source_path)
         destination_path = os.path.abspath(destination_path)
+
+        # Check for restricted paths
         for restricted_path in self.__RESTRICTED_PATHS:
-            
             if source_path.startswith(restricted_path) or destination_path.startswith(restricted_path):
                 raise DangerZone("Path is within restricted system directories can not be processed!")
-        if len(self.__counter)-1!=len(self.__extensions):
-            print("Counter Dictionary and Extension Dictionary must be of same length.")
-            
-        
-        elif source_path==destination_path:
-            print("Source folder and Destination Folder must be different")
-        
 
+        # Check other conditions before proceeding
+        if len(self.__counter) - 1 != len(self.__extensions):
+            print("Counter Dictionary and Extension Dictionary must be of the same length.")
+        elif source_path == destination_path:
+            print("Source folder and Destination Folder must be different")
         elif not os.path.exists(source_path):
-            print(f"Path {source_path} does not exist.Please make sure you have given correct path.")
+            print(f"Path {source_path} does not exist. Please make sure you have given the correct path.")
         elif self.__is_subdirectory(source_path, destination_path):
             raise DestinationInsideSourceError("Destination path should not be inside the Source path.")
-        elif not (os.path.isdir(source_path) or not os.path.isdir(destination_path)) :
+        elif not (os.path.isdir(source_path) or not os.path.isdir(destination_path)):
             raise NotADirectoryError
-            
+
         else:
             os.makedirs(destination_path, exist_ok=True)
             
             files = self.__list_files(source_path)
             
             print(20*"+-*-+")
             print(f"Total Files: {len(files)}")
@@ -282,34 +299,24 @@
             for key,value in self.__counter.items():
                 if len(value)>0:
                     print(f"Total {key} : {len(value)}")
             print(20*"+-*-+")
             if input("Would you like to proceed?[y/n]:\n").lower()=='y':
 
                 
-                for category, file_paths in self.__counter.items():
-                    if file_paths:
-                        category_path = os.path.join(destination_path, category)
-                        os.makedirs(category_path, exist_ok=True)
-                        for file_path in file_paths:
-                            dest_file = os.path.join(category_path, os.path.basename(file_path))
-                            shutil.move(file_path, dest_file)
-                            
-                            print(f"File {os.path.basename(file_path)} moved to {category} folder.")
-                        print(20*"+-*-+")
-                
-                
-                
+                with ThreadPoolExecutor() as executor:
+                    for category, file_paths in self.__counter.items():
+                        if file_paths:
+                            executor.submit(self.__move_files, category, file_paths, destination_path)
+
                 empty_folders=self.__get_empty_folders(source_path)
                 
                 print(f"We found {len(empty_folders)} Empty Folders after cleanup!")
                 
                 if input("Would you like to delete all empty folders?[y/n]: ").lower()=='y':
                     print(20*"+-*-+")
                     for empty_folder in empty_folders:
                         os.rmdir(empty_folder)
                         print(f"{empty_folder} Deleted successfully.")
             else:
                 print("Good Luck!")
-      
-
```

### Comparing `pi-folder-organizer-1.1.0/pi_folder_organizer.egg-info/PKG-INFO` & `pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-folder-organizer
-Version: 1.1.0
+Version: 2.1.0
 Summary: A Python package for cleaning up cluttered files and organizing them into respective folders.
 Author: Qadeer Ahmad
 Author-email: mrqdeer1231122@gmail.com
 Keywords: python,file organization,file cleanup,cluttered files,folder management,data organization,file management,data cleanup,Python package,developer tools,data processing,file sorting,data structuring,automated file organization,Python library,data management,data handling,file optimization,data optimization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pi-folder-organizer-1.1.0/setup.py` & `pi-folder-organizer-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.0'
+VERSION = '2.1.0'
 DESCRIPTION = "A Python package for cleaning up cluttered files and organizing them into respective folders."
 # Setting up
 setup(
     name="pi-folder-organizer",
     version=VERSION,
     author="Qadeer Ahmad",
     author_email="mrqdeer1231122@gmail.com",
```

