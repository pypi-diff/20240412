# Comparing `tmp/dl-translate-0.3.0.tar.gz` & `tmp/dl-translate-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl-translate-0.3.0.tar", last modified: Tue Jul 18 05:38:53 2023, max compression
+gzip compressed data, was "dl-translate-0.3.1.tar", last modified: Fri Apr 12 19:40:00 2024, max compression
```

## Comparing `dl-translate-0.3.0.tar` & `dl-translate-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:38:53.349707 dl-translate-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-18 05:38:41.000000 dl-translate-0.3.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 05:38:41.000000 dl-translate-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 05:38:41.000000 dl-translate-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-07-18 05:38:53.349707 dl-translate-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-07-18 05:38:41.000000 dl-translate-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:38:53.349707 dl-translate-0.3.0/dl_translate/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/_translation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:38:53.349707 dl-translate-0.3.0/dl_translate/lang/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/lang/m2m100.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/lang/mbart50.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/lang/nllb200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:38:53.349707 dl-translate-0.3.0/dl_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 05:38:53.349707 dl-translate-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-18 05:38:41.000000 dl-translate-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:40:00.230414 dl-translate-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-12 19:39:46.000000 dl-translate-0.3.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 19:39:46.000000 dl-translate-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 19:39:46.000000 dl-translate-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-04-12 19:40:00.230414 dl-translate-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-04-12 19:39:46.000000 dl-translate-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:40:00.226414 dl-translate-0.3.1/dl_translate/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-12 19:39:46.000000 dl-translate-0.3.1/dl_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-12 19:39:46.000000 dl-translate-0.3.1/dl_translate/_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-04-12 19:39:46.000000 dl-translate-0.3.1/dl_translate/_translation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:40:00.230414 dl-translate-0.3.1/dl_translate/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 19:39:46.000000 dl-translate-0.3.1/dl_translate/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-12 19:39:46.000000 dl-translate-0.3.1/dl_translate/lang/m2m100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-12 19:39:46.000000 dl-translate-0.3.1/dl_translate/lang/mbart50.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-12 19:39:46.000000 dl-translate-0.3.1/dl_translate/lang/nllb200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-12 19:39:46.000000 dl-translate-0.3.1/dl_translate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:40:00.230414 dl-translate-0.3.1/dl_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-04-12 19:39:59.000000 dl-translate-0.3.1/dl_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 19:40:00.000000 dl-translate-0.3.1/dl_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:39:59.000000 dl-translate-0.3.1/dl_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 19:39:59.000000 dl-translate-0.3.1/dl_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 19:39:59.000000 dl-translate-0.3.1/dl_translate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:40:00.230414 dl-translate-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-12 19:39:46.000000 dl-translate-0.3.1/setup.py
```

### Comparing `dl-translate-0.3.0/LICENSE` & `dl-translate-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dl-translate-0.3.0/PKG-INFO` & `dl-translate-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dl-translate
-Version: 0.3.0
+Version: 0.3.1
 Summary: A deep learning-based translation library built on Huggingface transformers
 Home-page: https://github.com/xhlulu/dl-translate
 Author: Xing Han Lu
 Author-email: github@xinghanlu.com
 License: UNKNOWN
 Description: # DL Translate
         
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5230676.svg)](https://doi.org/10.5281/zenodo.5230676)
         [![Downloads](https://static.pepy.tech/personalized-badge/dl-translate?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/dl-translate)
         [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/xhluca/dl-translate/blob/main/LICENSE)
         
         
-        *A deep learning-based translation library built on Huggingface `transformers`*
+        *A translation library for 200 languages built on Huggingface `transformers`*
         
         💻 [GitHub Repository](https://github.com/xhluca/dl-translate)<br>
         📚 [Documentation](https://xhluca.github.io/dl-translate)<br>
         🐍 [PyPi project](https://pypi.org/project/dl-translate/)<br>
         🧪 [Colab Demo](https://colab.research.google.com/github/xhluca/dl-translate/blob/main/demos/colab_demo.ipynb) / [Kaggle Demo](https://www.kaggle.com/xhlulu/dl-translate-demo/)
         
         
@@ -36,15 +36,15 @@
         
         mt = dlt.TranslationModel()  # Slow when you load it for the first time
         
         text_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
         mt.translate(text_hi, source=dlt.lang.HINDI, target=dlt.lang.ENGLISH)
         ```
         
-        Above, you can see that `dlt.lang` contains variables representing each of the 50 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
+        Above, you can see that `dlt.lang` contains variables representing each of the 200 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
         ```python
         text_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
         mt.translate(text_ar, source="Arabic", target="fr")
         ```
         
         If you want to verify whether a language is available, you can check it:
         ```python
```

### Comparing `dl-translate-0.3.0/README.md` & `dl-translate-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # DL Translate
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5230676.svg)](https://doi.org/10.5281/zenodo.5230676)
 [![Downloads](https://static.pepy.tech/personalized-badge/dl-translate?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/dl-translate)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/xhluca/dl-translate/blob/main/LICENSE)
 
 
-*A deep learning-based translation library built on Huggingface `transformers`*
+*A translation library for 200 languages built on Huggingface `transformers`*
 
 💻 [GitHub Repository](https://github.com/xhluca/dl-translate)<br>
 📚 [Documentation](https://xhluca.github.io/dl-translate)<br>
 🐍 [PyPi project](https://pypi.org/project/dl-translate/)<br>
 🧪 [Colab Demo](https://colab.research.google.com/github/xhluca/dl-translate/blob/main/demos/colab_demo.ipynb) / [Kaggle Demo](https://www.kaggle.com/xhlulu/dl-translate-demo/)
 
 
@@ -28,15 +28,15 @@
 
 mt = dlt.TranslationModel()  # Slow when you load it for the first time
 
 text_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
 mt.translate(text_hi, source=dlt.lang.HINDI, target=dlt.lang.ENGLISH)
 ```
 
-Above, you can see that `dlt.lang` contains variables representing each of the 50 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
+Above, you can see that `dlt.lang` contains variables representing each of the 200 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
 ```python
 text_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
 mt.translate(text_ar, source="Arabic", target="fr")
 ```
 
 If you want to verify whether a language is available, you can check it:
 ```python
```

### Comparing `dl-translate-0.3.0/dl_translate/_pairs.py` & `dl-translate-0.3.1/dl_translate/_pairs.py`

 * *Files identical despite different names*

### Comparing `dl-translate-0.3.0/dl_translate/_translation_model.py` & `dl-translate-0.3.1/dl_translate/_translation_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,16 +173,19 @@
             "forced_bos_token_id", self._tokenizer.lang_code_to_id[target]
         )
         generation_options.setdefault("max_new_tokens", 512)
 
         data_loader = torch.utils.data.DataLoader(text, batch_size=batch_size)
         output_text = []
 
+        tqdm_iterator = data_loader
+        if verbose is True:
+            tqdm_iterator = tqdm(data_loader)
         with torch.no_grad():
-            for batch in tqdm(data_loader, disable=not verbose):
+            for batch in tqdm_iterator:
                 encoded = self._tokenizer(batch, return_tensors="pt", padding=True)
                 encoded.to(self.device)
 
                 generated_tokens = self._transformers_model.generate(
                     **encoded, **generation_options
                 ).cpu()
```

### Comparing `dl-translate-0.3.0/dl_translate/lang/m2m100.py` & `dl-translate-0.3.1/dl_translate/lang/m2m100.py`

 * *Files identical despite different names*

### Comparing `dl-translate-0.3.0/dl_translate/lang/mbart50.py` & `dl-translate-0.3.1/dl_translate/lang/mbart50.py`

 * *Files identical despite different names*

### Comparing `dl-translate-0.3.0/dl_translate/lang/nllb200.py` & `dl-translate-0.3.1/dl_translate/lang/nllb200.py`

 * *Files identical despite different names*

### Comparing `dl-translate-0.3.0/dl_translate/utils.py` & `dl-translate-0.3.1/dl_translate/utils.py`

 * *Files identical despite different names*

### Comparing `dl-translate-0.3.0/dl_translate.egg-info/PKG-INFO` & `dl-translate-0.3.1/dl_translate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dl-translate
-Version: 0.3.0
+Version: 0.3.1
 Summary: A deep learning-based translation library built on Huggingface transformers
 Home-page: https://github.com/xhlulu/dl-translate
 Author: Xing Han Lu
 Author-email: github@xinghanlu.com
 License: UNKNOWN
 Description: # DL Translate
         
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5230676.svg)](https://doi.org/10.5281/zenodo.5230676)
         [![Downloads](https://static.pepy.tech/personalized-badge/dl-translate?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/dl-translate)
         [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/xhluca/dl-translate/blob/main/LICENSE)
         
         
-        *A deep learning-based translation library built on Huggingface `transformers`*
+        *A translation library for 200 languages built on Huggingface `transformers`*
         
         💻 [GitHub Repository](https://github.com/xhluca/dl-translate)<br>
         📚 [Documentation](https://xhluca.github.io/dl-translate)<br>
         🐍 [PyPi project](https://pypi.org/project/dl-translate/)<br>
         🧪 [Colab Demo](https://colab.research.google.com/github/xhluca/dl-translate/blob/main/demos/colab_demo.ipynb) / [Kaggle Demo](https://www.kaggle.com/xhlulu/dl-translate-demo/)
         
         
@@ -36,15 +36,15 @@
         
         mt = dlt.TranslationModel()  # Slow when you load it for the first time
         
         text_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
         mt.translate(text_hi, source=dlt.lang.HINDI, target=dlt.lang.ENGLISH)
         ```
         
-        Above, you can see that `dlt.lang` contains variables representing each of the 50 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
+        Above, you can see that `dlt.lang` contains variables representing each of the 200 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
         ```python
         text_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
         mt.translate(text_ar, source="Arabic", target="fr")
         ```
         
         If you want to verify whether a language is available, you can check it:
         ```python
```

### Comparing `dl-translate-0.3.0/setup.py` & `dl-translate-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dl-translate",
-    version="0.3.0",
+    version="0.3.1",
     author="Xing Han Lu",
     author_email="github@xinghanlu.com",
     description="A deep learning-based translation library built on Huggingface transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xhlulu/dl-translate",
     classifiers=[
```

