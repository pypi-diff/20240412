# Comparing `tmp/pymysqls-0.1.tar.gz` & `tmp/pymysqls-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymysqls-0.1.tar", last modified: Fri Apr 12 17:04:45 2024, max compression
+gzip compressed data, was "pymysqls-0.2.tar", last modified: Fri Apr 12 17:26:57 2024, max compression
```

## Comparing `pymysqls-0.1.tar` & `pymysqls-0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.284483 pymysqls-0.1/
--rw-rw-rw-   0        0        0      197 2024-04-12 17:04:32.000000 pymysqls-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0       53 2024-04-12 17:04:45.284483 pymysqls-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.251837 pymysqls-0.1/pymysqls/
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.267828 pymysqls-0.1/pymysqls/1/
--rw-rw-rw-   0        0        0     1673 2024-02-20 20:54:29.000000 pymysqls-0.1/pymysqls/1/Ui_Form.py
--rw-rw-rw-   0        0        0     1088 2024-02-20 20:54:03.000000 pymysqls-0.1/pymysqls/1/Ui_Form.ui
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.269936 pymysqls-0.1/pymysqls/1/lib/
--rw-rw-rw-   0        0        0        0 2024-02-20 19:22:55.000000 pymysqls-0.1/pymysqls/1/lib/__init__.py
--rw-rw-rw-   0        0        0      813 2024-02-20 21:06:39.000000 pymysqls-0.1/pymysqls/1/lib/db.py
--rw-rw-rw-   0        0        0     1834 2024-02-20 21:12:50.000000 pymysqls-0.1/pymysqls/1/main.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.273038 pymysqls-0.1/pymysqls/2/
--rw-rw-rw-   0        0        0      742 2024-03-22 10:47:52.000000 pymysqls-0.1/pymysqls/2/db.sql
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.276584 pymysqls-0.1/pymysqls/2/libs/
--rw-rw-rw-   0        0        0        0 2024-03-22 09:00:24.000000 pymysqls-0.1/pymysqls/2/libs/__init__.py
--rw-rw-rw-   0        0        0      949 2024-03-22 10:08:42.000000 pymysqls-0.1/pymysqls/2/libs/db.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.279156 pymysqls-0.1/pymysqls/2/libs/enums/
--rw-rw-rw-   0        0        0      388 2024-03-22 09:00:24.000000 pymysqls-0.1/pymysqls/2/libs/enums/ImportType.py
--rw-rw-rw-   0        0        0        0 2024-03-22 09:00:24.000000 pymysqls-0.1/pymysqls/2/libs/enums/__init__.py
--rw-rw-rw-   0        0        0     4334 2024-03-22 09:45:06.000000 pymysqls-0.1/pymysqls/2/libs/import_fles.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.281252 pymysqls-0.1/pymysqls/2/libs/ui/
--rw-rw-rw-   0        0        0     2689 2024-03-22 09:48:40.000000 pymysqls-0.1/pymysqls/2/libs/ui/MainWindow.py
--rw-rw-rw-   0        0        0     1635 2024-03-22 09:00:24.000000 pymysqls-0.1/pymysqls/2/libs/ui/PieChartWindow.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.282965 pymysqls-0.1/pymysqls/2/libs/ui/ui_files/
--rw-rw-rw-   0        0        0     3925 2024-03-22 09:00:24.000000 pymysqls-0.1/pymysqls/2/libs/ui/ui_files/main_window.ui
--rw-rw-rw-   0        0        0      234 2024-03-22 09:00:24.000000 pymysqls-0.1/pymysqls/2/main.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:04:45.264759 pymysqls-0.1/pymysqls.egg-info/
--rw-rw-rw-   0        0        0       53 2024-04-12 17:04:45.000000 pymysqls-0.1/pymysqls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-04-12 17:04:45.000000 pymysqls-0.1/pymysqls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 17:04:45.000000 pymysqls-0.1/pymysqls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 17:04:45.000000 pymysqls-0.1/pymysqls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 17:04:45.000000 pymysqls-0.1/pymysqls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 17:04:45.284483 pymysqls-0.1/setup.cfg
--rw-rw-rw-   0        0        0      415 2024-04-12 17:04:38.000000 pymysqls-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.841105 pymysqls-0.2/
+-rw-rw-rw-   0        0        0      197 2024-04-12 17:26:20.000000 pymysqls-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0       53 2024-04-12 17:26:57.841105 pymysqls-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.815094 pymysqls-0.2/pymysqls/
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.826413 pymysqls-0.2/pymysqls/1/
+-rw-rw-rw-   0        0        0     1673 2024-02-20 20:54:29.000000 pymysqls-0.2/pymysqls/1/Ui_Form.py
+-rw-rw-rw-   0        0        0     1088 2024-02-20 20:54:03.000000 pymysqls-0.2/pymysqls/1/Ui_Form.ui
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.828434 pymysqls-0.2/pymysqls/1/lib/
+-rw-rw-rw-   0        0        0        0 2024-02-20 19:22:55.000000 pymysqls-0.2/pymysqls/1/lib/__init__.py
+-rw-rw-rw-   0        0        0      813 2024-02-20 21:06:39.000000 pymysqls-0.2/pymysqls/1/lib/db.py
+-rw-rw-rw-   0        0        0     1844 2024-04-12 17:26:34.000000 pymysqls-0.2/pymysqls/1/main.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.830449 pymysqls-0.2/pymysqls/2/
+-rw-rw-rw-   0        0        0      742 2024-03-22 10:47:52.000000 pymysqls-0.2/pymysqls/2/db.sql
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.833436 pymysqls-0.2/pymysqls/2/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-22 09:00:24.000000 pymysqls-0.2/pymysqls/2/libs/__init__.py
+-rw-rw-rw-   0        0        0      949 2024-03-22 10:08:42.000000 pymysqls-0.2/pymysqls/2/libs/db.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.835965 pymysqls-0.2/pymysqls/2/libs/enums/
+-rw-rw-rw-   0        0        0      388 2024-03-22 09:00:24.000000 pymysqls-0.2/pymysqls/2/libs/enums/ImportType.py
+-rw-rw-rw-   0        0        0        0 2024-03-22 09:00:24.000000 pymysqls-0.2/pymysqls/2/libs/enums/__init__.py
+-rw-rw-rw-   0        0        0     4334 2024-03-22 09:45:06.000000 pymysqls-0.2/pymysqls/2/libs/import_fles.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.837979 pymysqls-0.2/pymysqls/2/libs/ui/
+-rw-rw-rw-   0        0        0     2689 2024-03-22 09:48:40.000000 pymysqls-0.2/pymysqls/2/libs/ui/MainWindow.py
+-rw-rw-rw-   0        0        0     1635 2024-03-22 09:00:24.000000 pymysqls-0.2/pymysqls/2/libs/ui/PieChartWindow.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.839486 pymysqls-0.2/pymysqls/2/libs/ui/ui_files/
+-rw-rw-rw-   0        0        0     3925 2024-03-22 09:00:24.000000 pymysqls-0.2/pymysqls/2/libs/ui/ui_files/main_window.ui
+-rw-rw-rw-   0        0        0      244 2024-04-12 17:26:40.000000 pymysqls-0.2/pymysqls/2/main.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:26:57.823175 pymysqls-0.2/pymysqls.egg-info/
+-rw-rw-rw-   0        0        0       53 2024-04-12 17:26:57.000000 pymysqls-0.2/pymysqls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-04-12 17:26:57.000000 pymysqls-0.2/pymysqls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 17:26:57.000000 pymysqls-0.2/pymysqls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 17:26:57.000000 pymysqls-0.2/pymysqls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 17:26:57.000000 pymysqls-0.2/pymysqls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 17:26:57.841105 pymysqls-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      415 2024-04-12 17:26:19.000000 pymysqls-0.2/setup.py
```

### Comparing `pymysqls-0.1/pymysqls/1/Ui_Form.py` & `pymysqls-0.2/pymysqls/1/Ui_Form.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.1/pymysqls/1/Ui_Form.ui` & `pymysqls-0.2/pymysqls/1/Ui_Form.ui`

 * *Files identical despite different names*

### Comparing `pymysqls-0.1/pymysqls/1/lib/db.py` & `pymysqls-0.2/pymysqls/1/lib/db.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.1/pymysqls/1/main.py` & `pymysqls-0.2/pymysqls/1/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,12 +44,12 @@
         obj.addWidget(image)
         label = QtWidgets.QLabel()
         label.setText(f"{data[0]}\n{data[1]} руб.\n{data[2].strftime('%H:%M:%S %d.%m.%y')}\nСтатус: {data[3]}")
         obj.addWidget(label)
         self.verticalLayout.addLayout(obj)
 
 
-if __name__ == "__main__":
-    app = QtWidgets.QApplication([])
-    window = MainWindow()
-    window.show()
-    sys.exit(app.exec())
+# if __name__ == "__main__":
+#     app = QtWidgets.QApplication([])
+#     window = MainWindow()
+#     window.show()
+#     sys.exit(app.exec())
```

### Comparing `pymysqls-0.1/pymysqls/2/db.sql` & `pymysqls-0.2/pymysqls/2/db.sql`

 * *Files identical despite different names*

### Comparing `pymysqls-0.1/pymysqls/2/libs/db.py` & `pymysqls-0.2/pymysqls/2/libs/db.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.1/pymysqls/2/libs/import_fles.py` & `pymysqls-0.2/pymysqls/2/libs/import_fles.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.1/pymysqls/2/libs/ui/MainWindow.py` & `pymysqls-0.2/pymysqls/2/libs/ui/MainWindow.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.1/pymysqls/2/libs/ui/PieChartWindow.py` & `pymysqls-0.2/pymysqls/2/libs/ui/PieChartWindow.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.1/pymysqls/2/libs/ui/ui_files/main_window.ui` & `pymysqls-0.2/pymysqls/2/libs/ui/ui_files/main_window.ui`

 * *Files identical despite different names*

### Comparing `pymysqls-0.1/pymysqls.egg-info/SOURCES.txt` & `pymysqls-0.2/pymysqls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

