# Comparing `tmp/sodata-0.0.5.tar.gz` & `tmp/sodata-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sodata-0.0.5.tar", last modified: Wed Apr 10 10:28:29 2024, max compression
+gzip compressed data, was "sodata-0.0.6.tar", last modified: Fri Apr 12 12:13:42 2024, max compression
```

## Comparing `sodata-0.0.5.tar` & `sodata-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 10:28:29.951897 sodata-0.0.5/
--rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      318 2024-04-10 10:28:29.951897 sodata-0.0.5/PKG-INFO
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      298 2024-04-09 07:45:32.000000 sodata-0.0.5/README.md
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       38 2024-04-10 10:28:29.951897 sodata-0.0.5/setup.cfg
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      380 2024-04-10 10:28:23.000000 sodata-0.0.5/setup.py
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 10:28:29.951897 sodata-0.0.5/sodata/
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      129 2024-04-10 06:25:35.000000 sodata-0.0.5/sodata/__init__.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      139 2024-04-09 12:56:22.000000 sodata-0.0.5/sodata/chunk_split.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)     1822 2024-04-10 07:23:18.000000 sodata-0.0.5/sodata/file_process.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)    14260 2024-04-10 10:25:15.000000 sodata-0.0.5/sodata/text_clean.py
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 10:28:29.951897 sodata-0.0.5/sodata.egg-info/
--rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      318 2024-04-10 10:28:29.000000 sodata-0.0.5/sodata.egg-info/PKG-INFO
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      252 2024-04-10 10:28:29.000000 sodata-0.0.5/sodata.egg-info/SOURCES.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        1 2024-04-10 10:28:29.000000 sodata-0.0.5/sodata.egg-info/dependency_links.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       48 2024-04-10 10:28:29.000000 sodata-0.0.5/sodata.egg-info/requires.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        7 2024-04-10 10:28:29.000000 sodata-0.0.5/sodata.egg-info/top_level.txt
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-12 12:13:42.610291 sodata-0.0.6/
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      165 2024-04-12 12:13:42.610291 sodata-0.0.6/PKG-INFO
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      298 2024-04-09 07:45:32.000000 sodata-0.0.6/README.md
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       38 2024-04-12 12:13:42.610291 sodata-0.0.6/setup.cfg
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      380 2024-04-12 12:13:11.000000 sodata-0.0.6/setup.py
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-12 12:13:42.610291 sodata-0.0.6/sodata/
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      129 2024-04-10 06:25:35.000000 sodata-0.0.6/sodata/__init__.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      139 2024-04-09 12:56:22.000000 sodata-0.0.6/sodata/chunk_split.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)     1818 2024-04-12 11:50:05.000000 sodata-0.0.6/sodata/file_process.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)    14292 2024-04-12 11:55:39.000000 sodata-0.0.6/sodata/text_clean.py
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-12 12:13:42.610291 sodata-0.0.6/sodata.egg-info/
+-rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      165 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/PKG-INFO
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      252 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        1 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       48 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/requires.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        7 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/top_level.txt
```

### Comparing `sodata-0.0.5/sodata/file_process.py` & `sodata-0.0.6/sodata/file_process.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,9 +39,7 @@
                     text_data = process_txt_file(filepath)
                     with open(output_file, 'a', encoding='utf-8') as fp:
                         fp.write(json.dumps({"text": text_data}, ensure_ascii=False) + '\n')
                     print(f"Processed and saved {file} successfully.")
                 except UnicodeDecodeError as e:
                     print(e)
 
-
-
```

### Comparing `sodata-0.0.5/sodata/text_clean.py` & `sodata-0.0.6/sodata/text_clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,26 +219,34 @@
     # unique_paragraphs, ordered_repeated= remove_duplicates_minhash(paragraphs)
 
     text_clean = '\n'.join(unique_paragraphs)
     return text_clean, repeated_text
 
 
 def clean_text(text):
-    """
+    '''
     对文本chunk块清洗
-    @param text:文本chunk块
-    @return: 清洗后的文本：str;去重的段落列表：list
-    """
+    Args:
+        text:文本chunk块
+
+    Returns:
+        清洗后的文本：str;去重的段落列表：list
+    '''
+
+
+
+
+
     raw_text = text
     # 应用替换规则清洗
     for pattern, replacement in rules:
         # dirty_text_list.extend(re.findall(pattern, text))
         text = re.sub(pattern, replacement, text)
      # 通用清洗
     text = jio.clean_text(text, remove_parentheses=False, delete_prefix=True)#remove_parentheses=False 表示不移除括号，delete_prefix=True 表示删除前缀
 
     text, ordered_repeated = cascade_deduplication(text)
     # dirty_text_list.append(ordered_repeated)
     if "@" in text or "^" in text or "PS：" in text or "更新时间" in text or "回复时间" in text or "回复日期" in text or (
             "《" in text and "》" in text):
-        return ''
+        return '',[]
     return text,ordered_repeated
```

