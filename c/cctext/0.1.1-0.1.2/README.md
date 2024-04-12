# Comparing `tmp/cctext-0.1.1.tar.gz` & `tmp/cctext-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cctext-0.1.1.tar", last modified: Fri Apr 12 10:24:48 2024, max compression
+gzip compressed data, was "cctext-0.1.2.tar", last modified: Fri Apr 12 16:53:55 2024, max compression
```

## Comparing `cctext-0.1.1.tar` & `cctext-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 10:24:48.212272 cctext-0.1.1/
--rw-rw-rw-   0        0        0     1101 2024-04-12 07:07:09.000000 cctext-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1278 2024-04-12 10:24:48.212272 cctext-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-12 10:07:32.000000 cctext-0.1.1/README.md
--rw-rw-rw-   0        0        0        5 2024-04-12 10:18:14.000000 cctext-0.1.1/VERSION
-drwxrwxrwx   0        0        0        0 2024-04-12 10:24:48.196269 cctext-0.1.1/cctext/
--rw-rw-rw-   0        0        0      888 2024-04-11 20:12:00.000000 cctext-0.1.1/cctext/__init__.py
--rw-rw-rw-   0        0        0     2865 2024-04-11 20:11:26.000000 cctext-0.1.1/cctext/api.py
--rw-rw-rw-   0        0        0     2585 2024-04-11 19:52:19.000000 cctext-0.1.1/cctext/context.py
--rw-rw-rw-   0        0        0        0 2024-04-12 10:19:33.000000 cctext-0.1.1/cctext/py.typed
--rw-rw-rw-   0        0        0     1684 2024-04-11 20:24:09.000000 cctext-0.1.1/cctext/reference.py
--rw-rw-rw-   0        0        0     4815 2024-04-11 20:24:17.000000 cctext-0.1.1/cctext/resolver.py
--rw-rw-rw-   0        0        0     4868 2024-04-11 20:07:22.000000 cctext-0.1.1/cctext/rumodel.py
--rw-rw-rw-   0        0        0    20073 2024-04-11 20:10:47.000000 cctext-0.1.1/cctext/ruparser.py
--rw-rw-rw-   0        0        0     2620 2024-04-11 20:10:57.000000 cctext-0.1.1/cctext/syntax.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:24:48.211268 cctext-0.1.1/cctext.egg-info/
--rw-rw-rw-   0        0        0     1278 2024-04-12 10:24:48.000000 cctext-0.1.1/cctext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2024-04-12 10:24:48.000000 cctext-0.1.1/cctext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 10:24:48.000000 cctext-0.1.1/cctext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 10:18:13.000000 cctext-0.1.1/cctext.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-04-12 10:24:48.000000 cctext-0.1.1/cctext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-12 10:24:48.000000 cctext-0.1.1/cctext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2024-04-12 10:22:23.000000 cctext-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      869 2024-04-12 10:24:48.213269 cctext-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      121 2024-04-12 10:17:50.000000 cctext-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:24:48.210269 cctext-0.1.1/tests/
--rw-rw-rw-   0        0        0      197 2024-04-11 20:06:04.000000 cctext-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     4079 2024-04-11 20:06:14.000000 cctext-0.1.1/tests/t_api.py
--rw-rw-rw-   0        0        0     1414 2024-04-11 20:03:25.000000 cctext-0.1.1/tests/t_context.py
--rw-rw-rw-   0        0        0     1955 2024-04-11 20:03:38.000000 cctext-0.1.1/tests/t_reference.py
--rw-rw-rw-   0        0        0     7137 2024-04-11 20:15:57.000000 cctext-0.1.1/tests/t_resolver.py
--rw-rw-rw-   0        0        0      621 2024-04-11 19:41:33.000000 cctext-0.1.1/tests/t_rumodel.py
--rw-rw-rw-   0        0        0    30488 2024-04-11 19:55:39.000000 cctext-0.1.1/tests/t_ruparser.py
--rw-rw-rw-   0        0        0     3421 2023-08-18 16:45:24.000000 cctext-0.1.1/tests/t_syntax.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:53:55.193759 cctext-0.1.2/
+-rw-rw-rw-   0        0        0     1101 2024-04-12 07:07:09.000000 cctext-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1278 2024-04-12 16:53:55.192759 cctext-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-12 10:07:32.000000 cctext-0.1.2/README.md
+-rw-rw-rw-   0        0        0        5 2024-04-12 16:47:27.000000 cctext-0.1.2/VERSION
+drwxrwxrwx   0        0        0        0 2024-04-12 16:53:55.172758 cctext-0.1.2/cctext/
+-rw-rw-rw-   0        0        0      888 2024-04-11 20:12:00.000000 cctext-0.1.2/cctext/__init__.py
+-rw-rw-rw-   0        0        0     2865 2024-04-11 20:11:26.000000 cctext-0.1.2/cctext/api.py
+-rw-rw-rw-   0        0        0     2585 2024-04-11 19:52:19.000000 cctext-0.1.2/cctext/context.py
+-rw-rw-rw-   0        0        0        0 2024-04-12 10:19:33.000000 cctext-0.1.2/cctext/py.typed
+-rw-rw-rw-   0        0        0     1684 2024-04-11 20:24:09.000000 cctext-0.1.2/cctext/reference.py
+-rw-rw-rw-   0        0        0     4869 2024-04-12 16:45:21.000000 cctext-0.1.2/cctext/resolver.py
+-rw-rw-rw-   0        0        0     4868 2024-04-11 20:07:22.000000 cctext-0.1.2/cctext/rumodel.py
+-rw-rw-rw-   0        0        0    20073 2024-04-11 20:10:47.000000 cctext-0.1.2/cctext/ruparser.py
+-rw-rw-rw-   0        0        0     2620 2024-04-11 20:10:57.000000 cctext-0.1.2/cctext/syntax.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:53:55.191761 cctext-0.1.2/cctext.egg-info/
+-rw-rw-rw-   0        0        0     1278 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 10:18:13.000000 cctext-0.1.2/cctext.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2024-04-12 10:22:23.000000 cctext-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      869 2024-04-12 16:53:55.194759 cctext-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      121 2024-04-12 10:17:50.000000 cctext-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:53:55.189760 cctext-0.1.2/tests/
+-rw-rw-rw-   0        0        0      197 2024-04-11 20:06:04.000000 cctext-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     4079 2024-04-11 20:06:14.000000 cctext-0.1.2/tests/t_api.py
+-rw-rw-rw-   0        0        0     1414 2024-04-11 20:03:25.000000 cctext-0.1.2/tests/t_context.py
+-rw-rw-rw-   0        0        0     1955 2024-04-11 20:03:38.000000 cctext-0.1.2/tests/t_reference.py
+-rw-rw-rw-   0        0        0     7429 2024-04-12 16:46:51.000000 cctext-0.1.2/tests/t_resolver.py
+-rw-rw-rw-   0        0        0      621 2024-04-11 19:41:33.000000 cctext-0.1.2/tests/t_rumodel.py
+-rw-rw-rw-   0        0        0    30488 2024-04-11 19:55:39.000000 cctext-0.1.2/tests/t_ruparser.py
+-rw-rw-rw-   0        0        0     3421 2023-08-18 16:45:24.000000 cctext-0.1.2/tests/t_syntax.py
```

### Comparing `cctext-0.1.1/LICENSE` & `cctext-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/PKG-INFO` & `cctext-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cctext
-Version: 0.1.1
+Version: 0.1.2
 Summary: Text processing library for russian languange
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cctext-0.1.1/cctext/__init__.py` & `cctext-0.1.2/cctext/__init__.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/cctext/api.py` & `cctext-0.1.2/cctext/api.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/cctext/context.py` & `cctext-0.1.2/cctext/context.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/cctext/reference.py` & `cctext-0.1.2/cctext/reference.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/cctext/resolver.py` & `cctext-0.1.2/cctext/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,23 +42,25 @@
     master: Optional['ResolvedReference'] = None
     if offset > 0:
         index += 1
         while index < len(references):
             if isinstance(references[index].ref, EntityReference):
                 if offset == 1:
                     master = references[index]
+                    break
                 else:
                     offset -= 1
             index += 1
     else:
         index -= 1
         while index >= 0:
             if isinstance(references[index].ref, EntityReference):
                 if offset == -1:
                     master = references[index]
+                    break
                 else:
                     offset += 1
             index -= 1
     if master is None:
         return f'!Некорректное смещение: {ref.offset}!'
     return inflect_dependant(ref.nominal, master.resolved)
```

### Comparing `cctext-0.1.1/cctext/rumodel.py` & `cctext-0.1.2/cctext/rumodel.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/cctext/ruparser.py` & `cctext-0.1.2/cctext/ruparser.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/cctext/syntax.py` & `cctext-0.1.2/cctext/syntax.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/cctext.egg-info/PKG-INFO` & `cctext-0.1.2/cctext.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cctext
-Version: 0.1.1
+Version: 0.1.2
 Summary: Text processing library for russian languange
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cctext-0.1.1/cctext.egg-info/SOURCES.txt` & `cctext-0.1.2/cctext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/setup.cfg` & `cctext-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/tests/t_api.py` & `cctext-0.1.2/tests/t_api.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/tests/t_context.py` & `cctext-0.1.2/tests/t_context.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/tests/t_reference.py` & `cctext-0.1.2/tests/t_reference.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/tests/t_resolver.py` & `cctext-0.1.2/tests/t_resolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,40 +43,43 @@
         self.assertEqual(resolve_entity(ref, self.context), '!Неизвестная граммема: invalid!')
 
         ref = EntityReference('X123', 'plur')
         self.assertEqual(resolve_entity(ref, self.context), '!Неизвестная сущность: X123!')
 
 
     def test_resolve_syntactic(self):
-        ref = ResolvedReference(ref=EntityReference('X1', 'sing,datv'), resolved='человеку')
-        refs_list = [ref, ref, ref, ref]
+        ref1 = ResolvedReference(ref=EntityReference('X1', 'plur,nomn'), resolved='люди')
+        ref2 = ResolvedReference(ref=EntityReference('X1', 'sing,datv'), resolved='человеку')
+        ref3 = ResolvedReference(ref=EntityReference('X1', 'sing,loct'), resolved='человеке')
+        ref4 = ResolvedReference(ref=EntityReference('X1', 'plur,datv'), resolved='людям')
+        refs_list = [ref1, ref2, ref3, ref4]
 
         ref = SyntacticReference(text='умный', referral_offset=-1)
         self.assertEqual(resolve_syntactic(ref, 0, refs_list), '!Некорректное смещение: -1!')
 
         ref = SyntacticReference(text='умный', referral_offset=1)
         self.assertEqual(resolve_syntactic(ref, 3, refs_list), '!Некорректное смещение: 1!')
 
         ref = SyntacticReference(text='умный', referral_offset=1)
         self.assertEqual(resolve_syntactic(ref, 0, refs_list), 'умному')
 
         ref = SyntacticReference(text='умный', referral_offset=2)
-        self.assertEqual(resolve_syntactic(ref, 0, refs_list), 'умному')
+        self.assertEqual(resolve_syntactic(ref, 0, refs_list), 'умном')
 
         ref = SyntacticReference(text='умный', referral_offset=3)
-        self.assertEqual(resolve_syntactic(ref, 0, refs_list), 'умному')
+        self.assertEqual(resolve_syntactic(ref, 0, refs_list), 'умным')
 
         ref = SyntacticReference(text='умный', referral_offset=-1)
-        self.assertEqual(resolve_syntactic(ref, 3, refs_list), 'умному')
+        self.assertEqual(resolve_syntactic(ref, 3, refs_list), 'умном')
 
         ref = SyntacticReference(text='умный', referral_offset=-2)
         self.assertEqual(resolve_syntactic(ref, 3, refs_list), 'умному')
 
         ref = SyntacticReference(text='умный', referral_offset=-3)
-        self.assertEqual(resolve_syntactic(ref, 3, refs_list), 'умному')
+        self.assertEqual(resolve_syntactic(ref, 3, refs_list), 'умные')
 
 
     def test_resolve_invalid(self):
         self.assertEqual(self.resolver.resolve(''), '')
         self.assertEqual(len(self.resolver.refs), 0)
 
         self.assertEqual(self.resolver.resolve('simple text'), 'simple text')
```

### Comparing `cctext-0.1.1/tests/t_rumodel.py` & `cctext-0.1.2/tests/t_rumodel.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/tests/t_ruparser.py` & `cctext-0.1.2/tests/t_ruparser.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.1/tests/t_syntax.py` & `cctext-0.1.2/tests/t_syntax.py`

 * *Files identical despite different names*

