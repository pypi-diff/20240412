# Comparing `tmp/neuanwi02-0.0.3-py3-none-any.whl.zip` & `tmp/neuanwi02-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1603 bytes, number of entries: 6
--rw-r--r--  2.0 unx      363 b- defN 24-Apr-12 04:52 algo/easy.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-12 04:54 neuanwi02-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      124 b- defN 24-Apr-12 04:54 neuanwi02-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 04:54 neuanwi02-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-12 04:54 neuanwi02-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      460 b- defN 24-Apr-12 04:54 neuanwi02-0.0.3.dist-info/RECORD
-6 files, 1061 bytes uncompressed, 763 bytes compressed:  28.1%
+Zip file size: 1511 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      251 b- defN 24-Apr-12 05:08 algo/easy.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-12 05:10 neuanwi02-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      124 b- defN 24-Apr-12 05:10 neuanwi02-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 05:10 neuanwi02-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-12 05:10 neuanwi02-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      460 b- defN 24-Apr-12 05:10 neuanwi02-0.0.4.dist-info/RECORD
+6 files, 949 bytes uncompressed, 671 bytes compressed:  29.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: algo/easy.py
 Comment: 
 
-Filename: neuanwi02-0.0.3.dist-info/LICENSE
+Filename: neuanwi02-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: neuanwi02-0.0.3.dist-info/METADATA
+Filename: neuanwi02-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: neuanwi02-0.0.3.dist-info/WHEEL
+Filename: neuanwi02-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: neuanwi02-0.0.3.dist-info/top_level.txt
+Filename: neuanwi02-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: neuanwi02-0.0.3.dist-info/RECORD
+Filename: neuanwi02-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algo/easy.py

```diff
@@ -1,13 +1,11 @@
 import heapq
 from bisect import bisect_left, bisect_right
 
 def heapsort(iterable):
-		h = []
-   result = []
-   # 모든 원소를 차례대로 힙에 삽입
-   for value in iterable:
+    h = []
+    result = []
+    for value in iterable:
    	heapq.heappush(h, value)
-   # 힙에 삽입된 모든 원소를 차례대로 꺼내어 담기
-   for i in range(len(h)):
+    for i in range(len(h)):
        result.append(heapq.heappop(h))
-   return result
+    return result
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

