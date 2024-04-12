# Comparing `tmp/RS2024-0.0.1-py3-none-any.whl.zip` & `tmp/RS2024-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1341 bytes, number of entries: 6
--rw-r--r--  2.0 unx       26 b- defN 24-Apr-12 07:55 RS/app.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-12 07:56 RS2024-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      121 b- defN 24-Apr-12 07:56 RS2024-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 07:56 RS2024-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 24-Apr-12 07:56 RS2024-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      441 b- defN 24-Apr-12 07:56 RS2024-0.0.1.dist-info/RECORD
-6 files, 700 bytes uncompressed, 537 bytes compressed:  23.3%
+Zip file size: 1686 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      689 b- defN 24-Apr-12 08:24 RS/app.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-12 08:25 RS2024-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      121 b- defN 24-Apr-12 08:25 RS2024-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 08:25 RS2024-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 24-Apr-12 08:25 RS2024-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      442 b- defN 24-Apr-12 08:25 RS2024-0.0.2.dist-info/RECORD
+6 files, 1364 bytes uncompressed, 882 bytes compressed:  35.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: RS/app.py
 Comment: 
 
-Filename: RS2024-0.0.1.dist-info/LICENSE
+Filename: RS2024-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: RS2024-0.0.1.dist-info/METADATA
+Filename: RS2024-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: RS2024-0.0.1.dist-info/WHEEL
+Filename: RS2024-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: RS2024-0.0.1.dist-info/top_level.txt
+Filename: RS2024-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: RS2024-0.0.1.dist-info/RECORD
+Filename: RS2024-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RS/app.py

```diff
@@ -1,3 +1,27 @@
 
 import re 
 import string
+
+
+def validate_email(email):
+    pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
+    if re.match(pattern, email):
+        return True
+    else:
+        return False
+
+def format_phone_number(phone_number):
+    pattern = r'(\d{3})(\d{3})(\d{4})'
+    formatted_number = re.sub(pattern, r'+XX-\1-\2-\3', phone_number)
+    return formatted_number
+
+
+def validate_name(name):
+    # 이름이 빈 문자열인지 확인
+    if not name:
+        return False
+    # 모든 문자가 알파벳 또는 공백인지 확인
+    if all(char in string.ascii_letters or char in string.whitespace for char in name):
+        return True
+    else:
+        return False
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

