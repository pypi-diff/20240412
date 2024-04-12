# Comparing `tmp/NexR_qc-0.0.8.tar.gz` & `tmp/NexR_qc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NexR_qc-0.0.8.tar", last modified: Thu Feb 29 05:19:29 2024, max compression
+gzip compressed data, was "NexR_qc-0.0.9.tar", last modified: Thu Feb 29 05:25:05 2024, max compression
```

## Comparing `NexR_qc-0.0.8.tar` & `NexR_qc-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 donghyun   (501) staff       (20)        0 2024-02-29 05:19:29.099187 NexR_qc-0.0.8/
-drwxr-xr-x   0 donghyun   (501) staff       (20)        0 2024-02-29 05:19:29.097741 NexR_qc-0.0.8/NexR_qc/
--rw-r--r--   0 donghyun   (501) staff       (20)     1761 2024-02-28 12:25:31.000000 NexR_qc-0.0.8/NexR_qc/Logging.py
--rw-r--r--   0 donghyun   (501) staff       (20)    32874 2024-02-28 12:25:31.000000 NexR_qc-0.0.8/NexR_qc/QualityCheck.py
--rw-r--r--   0 donghyun   (501) staff       (20)      962 2024-02-28 12:25:31.000000 NexR_qc-0.0.8/NexR_qc/Timer.py
--rw-r--r--   0 donghyun   (501) staff       (20)       22 2024-02-29 05:19:03.000000 NexR_qc-0.0.8/NexR_qc/__init__.py
-drwxr-xr-x   0 donghyun   (501) staff       (20)        0 2024-02-29 05:19:29.098782 NexR_qc-0.0.8/NexR_qc.egg-info/
--rw-r--r--   0 donghyun   (501) staff       (20)     3370 2024-02-29 05:19:29.000000 NexR_qc-0.0.8/NexR_qc.egg-info/PKG-INFO
--rw-r--r--   0 donghyun   (501) staff       (20)      282 2024-02-29 05:19:29.000000 NexR_qc-0.0.8/NexR_qc.egg-info/SOURCES.txt
--rw-r--r--   0 donghyun   (501) staff       (20)        1 2024-02-29 05:19:29.000000 NexR_qc-0.0.8/NexR_qc.egg-info/dependency_links.txt
--rw-r--r--   0 donghyun   (501) staff       (20)        1 2024-02-28 08:59:10.000000 NexR_qc-0.0.8/NexR_qc.egg-info/not-zip-safe
--rw-r--r--   0 donghyun   (501) staff       (20)       22 2024-02-29 05:19:29.000000 NexR_qc-0.0.8/NexR_qc.egg-info/requires.txt
--rw-r--r--   0 donghyun   (501) staff       (20)        8 2024-02-29 05:19:29.000000 NexR_qc-0.0.8/NexR_qc.egg-info/top_level.txt
--rw-r--r--   0 donghyun   (501) staff       (20)     3370 2024-02-29 05:19:29.098994 NexR_qc-0.0.8/PKG-INFO
--rw-r--r--   0 donghyun   (501) staff       (20)     2893 2024-02-29 04:58:37.000000 NexR_qc-0.0.8/README.md
--rw-r--r--   0 donghyun   (501) staff       (20)       38 2024-02-29 05:19:29.099237 NexR_qc-0.0.8/setup.cfg
--rw-r--r--   0 donghyun   (501) staff       (20)      939 2024-02-29 05:19:09.000000 NexR_qc-0.0.8/setup.py
+drwxr-xr-x   0 donghyun   (501) staff       (20)        0 2024-02-29 05:25:05.550543 NexR_qc-0.0.9/
+drwxr-xr-x   0 donghyun   (501) staff       (20)        0 2024-02-29 05:25:05.549331 NexR_qc-0.0.9/NexR_qc/
+-rw-r--r--   0 donghyun   (501) staff       (20)     1761 2024-02-28 12:25:31.000000 NexR_qc-0.0.9/NexR_qc/Logging.py
+-rw-r--r--   0 donghyun   (501) staff       (20)    32874 2024-02-28 12:25:31.000000 NexR_qc-0.0.9/NexR_qc/QualityCheck.py
+-rw-r--r--   0 donghyun   (501) staff       (20)      962 2024-02-28 12:25:31.000000 NexR_qc-0.0.9/NexR_qc/Timer.py
+-rw-r--r--   0 donghyun   (501) staff       (20)       22 2024-02-29 05:24:11.000000 NexR_qc-0.0.9/NexR_qc/__init__.py
+drwxr-xr-x   0 donghyun   (501) staff       (20)        0 2024-02-29 05:25:05.550213 NexR_qc-0.0.9/NexR_qc.egg-info/
+-rw-r--r--   0 donghyun   (501) staff       (20)     3363 2024-02-29 05:25:05.000000 NexR_qc-0.0.9/NexR_qc.egg-info/PKG-INFO
+-rw-r--r--   0 donghyun   (501) staff       (20)      282 2024-02-29 05:25:05.000000 NexR_qc-0.0.9/NexR_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 donghyun   (501) staff       (20)        1 2024-02-29 05:25:05.000000 NexR_qc-0.0.9/NexR_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 donghyun   (501) staff       (20)        1 2024-02-28 08:59:10.000000 NexR_qc-0.0.9/NexR_qc.egg-info/not-zip-safe
+-rw-r--r--   0 donghyun   (501) staff       (20)       22 2024-02-29 05:25:05.000000 NexR_qc-0.0.9/NexR_qc.egg-info/requires.txt
+-rw-r--r--   0 donghyun   (501) staff       (20)        8 2024-02-29 05:25:05.000000 NexR_qc-0.0.9/NexR_qc.egg-info/top_level.txt
+-rw-r--r--   0 donghyun   (501) staff       (20)     3363 2024-02-29 05:25:05.550377 NexR_qc-0.0.9/PKG-INFO
+-rw-r--r--   0 donghyun   (501) staff       (20)     2886 2024-02-29 05:24:11.000000 NexR_qc-0.0.9/README.md
+-rw-r--r--   0 donghyun   (501) staff       (20)       38 2024-02-29 05:25:05.550595 NexR_qc-0.0.9/setup.cfg
+-rw-r--r--   0 donghyun   (501) staff       (20)      939 2024-02-29 05:21:52.000000 NexR_qc-0.0.9/setup.py
```

### Comparing `NexR_qc-0.0.8/NexR_qc/Logging.py` & `NexR_qc-0.0.9/NexR_qc/Logging.py`

 * *Files identical despite different names*

### Comparing `NexR_qc-0.0.8/NexR_qc/QualityCheck.py` & `NexR_qc-0.0.9/NexR_qc/QualityCheck.py`

 * *Files identical despite different names*

### Comparing `NexR_qc-0.0.8/NexR_qc/Timer.py` & `NexR_qc-0.0.9/NexR_qc/Timer.py`

 * *Files identical despite different names*

### Comparing `NexR_qc-0.0.8/NexR_qc.egg-info/PKG-INFO` & `NexR_qc-0.0.9/NexR_qc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NexR-qc
-Version: 0.0.8
+Version: 0.0.9
 Summary: PYPI package creation written by NexR-qc
 Home-page: https://github.com/mata-1223/NexR_qc
 Author: mata.lee
 Author-email: ldh3810@gmail.com
 License: UNKNOWN
 Keywords: qc,NexR,mata.lee,NexR_qc,python,python tutorial,pypi
 Platform: UNKNOWN
@@ -27,15 +27,15 @@
 <br>
 
 ## 설치
 
 ### pip 설치
 ```
 #!/bin/bash
-pip install NexR_qc==0.0.7
+pip install NexR_qc
 ```
 
 ### 디렉토리 기본 구성
 - documents 하위 항목(테이블정의서, 컬럼정의서, 코드정의서)은 필수 항목은 아니지만, 테이블별 정확한 정보를 얻기위해서 작성되는 문서임 ([Github 링크](https://github.com/mata-1223/NexR_qc)의 document 폴더 내 문서 양식 참고)
 - log, output 폴더는 초기에 생성되어 있지않아도 수행 결과로 자동 생성됨
 - config.json 파일은 데이터 내 결측값을 커스텀하기 위한 파일로 초기에 생성되어 있지않아도 수행 결과로 자동 생성됨 (결측처리 default 값: "?", "na", "null", "Null", "NULL", " ", "[NULL]")
```

### Comparing `NexR_qc-0.0.8/PKG-INFO` & `NexR_qc-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NexR_qc
-Version: 0.0.8
+Version: 0.0.9
 Summary: PYPI package creation written by NexR-qc
 Home-page: https://github.com/mata-1223/NexR_qc
 Author: mata.lee
 Author-email: ldh3810@gmail.com
 License: UNKNOWN
 Keywords: qc,NexR,mata.lee,NexR_qc,python,python tutorial,pypi
 Platform: UNKNOWN
@@ -27,15 +27,15 @@
 <br>
 
 ## 설치
 
 ### pip 설치
 ```
 #!/bin/bash
-pip install NexR_qc==0.0.7
+pip install NexR_qc
 ```
 
 ### 디렉토리 기본 구성
 - documents 하위 항목(테이블정의서, 컬럼정의서, 코드정의서)은 필수 항목은 아니지만, 테이블별 정확한 정보를 얻기위해서 작성되는 문서임 ([Github 링크](https://github.com/mata-1223/NexR_qc)의 document 폴더 내 문서 양식 참고)
 - log, output 폴더는 초기에 생성되어 있지않아도 수행 결과로 자동 생성됨
 - config.json 파일은 데이터 내 결측값을 커스텀하기 위한 파일로 초기에 생성되어 있지않아도 수행 결과로 자동 생성됨 (결측처리 default 값: "?", "na", "null", "Null", "NULL", " ", "[NULL]")
```

### Comparing `NexR_qc-0.0.8/README.md` & `NexR_qc-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 <br>
 
 ## 설치
 
 ### pip 설치
 ```
 #!/bin/bash
-pip install NexR_qc==0.0.7
+pip install NexR_qc
 ```
 
 ### 디렉토리 기본 구성
 - documents 하위 항목(테이블정의서, 컬럼정의서, 코드정의서)은 필수 항목은 아니지만, 테이블별 정확한 정보를 얻기위해서 작성되는 문서임 ([Github 링크](https://github.com/mata-1223/NexR_qc)의 document 폴더 내 문서 양식 참고)
 - log, output 폴더는 초기에 생성되어 있지않아도 수행 결과로 자동 생성됨
 - config.json 파일은 데이터 내 결측값을 커스텀하기 위한 파일로 초기에 생성되어 있지않아도 수행 결과로 자동 생성됨 (결측처리 default 값: "?", "na", "null", "Null", "NULL", " ", "[NULL]")
```

### Comparing `NexR_qc-0.0.8/setup.py` & `NexR_qc-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="NexR_qc",
-    version="0.0.8",
+    version="0.0.9",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="PYPI package creation written by NexR-qc",
     author="mata.lee",
     author_email="ldh3810@gmail.com",
     url="https://github.com/mata-1223/NexR_qc",
     install_requires=[
```

