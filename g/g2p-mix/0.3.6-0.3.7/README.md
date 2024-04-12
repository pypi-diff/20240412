# Comparing `tmp/g2p_mix-0.3.6.tar.gz` & `tmp/g2p_mix-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p_mix-0.3.6.tar", last modified: Mon Apr  1 12:42:37 2024, max compression
+gzip compressed data, was "g2p_mix-0.3.7.tar", last modified: Fri Apr 12 06:55:30 2024, max compression
```

## Comparing `g2p_mix-0.3.6.tar` & `g2p_mix-0.3.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.872111 g2p_mix-0.3.6/
--rw-r--r--   0 admin      (501) staff       (20)     1066 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)       67 2024-03-29 02:45:49.000000 g2p_mix-0.3.6/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     1378 2024-04-01 12:42:37.871883 g2p_mix-0.3.6/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      775 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.866469 g2p_mix-0.3.6/g2p_mix/
--rw-r--r--   0 admin      (501) staff       (20)      630 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3147 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/constants.py
--rw-r--r--   0 admin      (501) staff       (20)     2455 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/g2p_eng.py
--rw-r--r--   0 admin      (501) staff       (20)     4433 2024-03-29 02:00:07.000000 g2p_mix-0.3.6/g2p_mix/g2p_mix.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.864655 g2p_mix-0.3.6/g2p_mix/nltk_data/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.867545 g2p_mix-0.3.6/g2p_mix/nltk_data/corpora/
--rw-r--r--   0 admin      (501) staff       (20)   896069 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/nltk_data/corpora/cmudict.zip
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.868854 g2p_mix-0.3.6/g2p_mix/nltk_data/taggers/
--rw-r--r--   0 admin      (501) staff       (20)  2526731 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
--rw-r--r--   0 admin      (501) staff       (20)     2047 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/token.py
--rw-r--r--   0 admin      (501) staff       (20)    11066 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/tone_sandhi.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.867389 g2p_mix-0.3.6/g2p_mix.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1378 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      423 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       87 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        8 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       48 2024-03-29 02:28:25.000000 g2p_mix-0.3.6/requirements.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-01 12:42:37.872156 g2p_mix-0.3.6/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-01 12:42:25.000000 g2p_mix-0.3.6/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:55:30.742450 g2p_mix-0.3.7/
+-rw-r--r--   0 admin      (501) staff       (20)     1066 2024-03-28 03:45:18.000000 g2p_mix-0.3.7/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)       67 2024-03-29 02:45:49.000000 g2p_mix-0.3.7/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     1378 2024-04-12 06:55:30.742147 g2p_mix-0.3.7/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      775 2024-03-28 03:45:18.000000 g2p_mix-0.3.7/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:55:30.735205 g2p_mix-0.3.7/g2p_mix/
+-rw-r--r--   0 admin      (501) staff       (20)      630 2024-03-28 03:45:18.000000 g2p_mix-0.3.7/g2p_mix/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     3147 2024-03-28 03:45:18.000000 g2p_mix-0.3.7/g2p_mix/constants.py
+-rw-r--r--   0 admin      (501) staff       (20)     2455 2024-03-28 03:45:18.000000 g2p_mix-0.3.7/g2p_mix/g2p_eng.py
+-rw-r--r--   0 admin      (501) staff       (20)     5007 2024-04-11 03:50:24.000000 g2p_mix-0.3.7/g2p_mix/g2p_mix.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:55:30.733153 g2p_mix-0.3.7/g2p_mix/nltk_data/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:55:30.736331 g2p_mix-0.3.7/g2p_mix/nltk_data/corpora/
+-rw-r--r--   0 admin      (501) staff       (20)   896069 2024-03-28 03:45:18.000000 g2p_mix-0.3.7/g2p_mix/nltk_data/corpora/cmudict.zip
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:55:30.738391 g2p_mix-0.3.7/g2p_mix/nltk_data/taggers/
+-rw-r--r--   0 admin      (501) staff       (20)  2526731 2024-03-28 03:45:18.000000 g2p_mix-0.3.7/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
+-rw-r--r--   0 admin      (501) staff       (20)     2047 2024-03-28 03:45:18.000000 g2p_mix-0.3.7/g2p_mix/token.py
+-rw-r--r--   0 admin      (501) staff       (20)    11066 2024-03-28 03:45:18.000000 g2p_mix-0.3.7/g2p_mix/tone_sandhi.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:55:30.736170 g2p_mix-0.3.7/g2p_mix.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1378 2024-04-12 06:55:30.000000 g2p_mix-0.3.7/g2p_mix.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      423 2024-04-12 06:55:30.000000 g2p_mix-0.3.7/g2p_mix.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-12 06:55:30.000000 g2p_mix-0.3.7/g2p_mix.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       87 2024-04-12 06:55:30.000000 g2p_mix-0.3.7/g2p_mix.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        8 2024-04-12 06:55:30.000000 g2p_mix-0.3.7/g2p_mix.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       48 2024-03-29 02:28:25.000000 g2p_mix-0.3.7/requirements.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-12 06:55:30.742500 g2p_mix-0.3.7/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-12 06:55:11.000000 g2p_mix-0.3.7/setup.py
```

### Comparing `g2p_mix-0.3.6/LICENSE` & `g2p_mix-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.6/PKG-INFO` & `g2p_mix-0.3.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p_mix
-Version: 0.3.6
+Version: 0.3.7
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p_mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
```

### Comparing `g2p_mix-0.3.6/README.md` & `g2p_mix-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.6/g2p_mix/__init__.py` & `g2p_mix-0.3.7/g2p_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.6/g2p_mix/constants.py` & `g2p_mix-0.3.7/g2p_mix/constants.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.6/g2p_mix/g2p_eng.py` & `g2p_mix-0.3.7/g2p_mix/g2p_eng.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.6/g2p_mix/g2p_mix.py` & `g2p_mix-0.3.7/g2p_mix/g2p_mix.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,22 +15,20 @@
 import os
 import re
 
 from jieba import posseg
 from pypinyin import lazy_pinyin, Style
 from pypinyin.constants import RE_HANS
 from pypinyin.contrib.tone_convert import to_initials, to_finals
-from pypinyin_dict.pinyin_data import zdic
 
 from .constants import POSTNASALS
 from .token import Token
 from .tone_sandhi import ToneSandhi
 
 
-zdic.load()  # 汉典
 os.environ["TRANSFORMERS_OFFLINE"] = "1"
 os.environ["HF_DATASETS_OFFLINE"] = "1"
 
 
 class G2pMix:
     def __init__(self, use_g2pw=False, repo_id=None, model_dir=None, model_source=None):
         if use_g2pw:
@@ -50,14 +48,28 @@
         else:
             self.lazy_pinyin = lazy_pinyin
         self.sandhier = ToneSandhi()
         # add space between ascii and chinese characters
         self.pattern = re.compile(
             r"(?<=[\u4e00-\u9fa5])(?=[\x00-\x19\x21-\x7F])|(?<=[\x00-\x19\x21-\x7F])(?=[\u4e00-\u9fa5])"
         )
+        # load dict to fix some badcase of pypinyin
+        self.load_dict()
+
+    def load_dict(self):
+        # 为、曾、更、长
+        # from pypinyin.constants import PINYIN_DICT
+        # print(hex(ord("为")), PINYIN_DICT[ord("为")])
+        from pypinyin import load_single_dict
+        load_single_dict({ord("长"): "cha2ng,zha4ng"}, "tone2")
+        load_single_dict({ord("为"): "we4i,we2i"}, "tone2")
+        # from pypinyin import load_phrases_dict
+        # load_phrases_dict({"长时间": [["cha2ng"], ["shi2"], ["jia1n"]]}, "tone2")
+        # from pypinyin_dict.pinyin_data import zdic
+        # zdic.load()  # 汉典
 
     def get_pinyins(self, text):
         segs = list(posseg.cut(text))
         words = [word for word, _ in segs]
         # tone_sandhi rules of pypinyin is not perfect
         pinyins = self.lazy_pinyin(words, neutral_tone_with_five=True, style=Style.TONE3)
```

### Comparing `g2p_mix-0.3.6/g2p_mix/nltk_data/corpora/cmudict.zip` & `g2p_mix-0.3.7/g2p_mix/nltk_data/corpora/cmudict.zip`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.6/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip` & `g2p_mix-0.3.7/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.6/g2p_mix/token.py` & `g2p_mix-0.3.7/g2p_mix/token.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.6/g2p_mix/tone_sandhi.py` & `g2p_mix-0.3.7/g2p_mix/tone_sandhi.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.6/g2p_mix.egg-info/PKG-INFO` & `g2p_mix-0.3.7/g2p_mix.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.3.6
+Version: 0.3.7
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p_mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
```

### Comparing `g2p_mix-0.3.6/setup.py` & `g2p_mix-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("requirements.txt", encoding="utf-8") as f:
     requirements = f.readlines()
 extras_require = {"g2pw": ["torch", "modelscope", "pypinyin-g2pw"]}
 
 setup(
     name="g2p_mix",
-    version=os.getenv("BUILD_VERSION") or "0.3.6",
+    version=os.getenv("BUILD_VERSION") or "0.3.7",
     author="Zhendong Peng",
     author_email="pzd17@tsinghua.org.cn",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="G2P mix",
     url="https://github.com/pengzhendong/g2p_mix",
     packages=find_packages(),
```

