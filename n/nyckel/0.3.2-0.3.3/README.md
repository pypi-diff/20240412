# Comparing `tmp/nyckel-0.3.2.tar.gz` & `tmp/nyckel-0.3.3.tar.gz`

## Comparing `nyckel-0.3.2.tar` & `nyckel-0.3.3.tar`

### file list

```diff
@@ -1,55 +1,62 @@
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 nyckel-0.3.2/mkdocs.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.3.2/requirements.txt
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.3.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.3.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.3.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.3.2/.vscode/extensions.json
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nyckel-0.3.2/.vscode/settings.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/copy_function.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/credentials.md
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/data_classes.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/delete_label.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/delete_samples.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/image_classification.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/index.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/merge_labels.md
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/multimodal_classification.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/quickstart.md
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/tabular_classification.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/text_classification.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/assets/favicon.ico
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/assets/nyckel-logo.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.3.2/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/auth.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/config.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/data_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/py.typed
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/request_utils.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/classification/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/classification/classification.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/classification/factory.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/classification/function_handler.py
--rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/classification/image_classification.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/classification/label_handler.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/classification/sample_handler.py
--rw-r--r--   0        0        0    17493 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/classification/tabular_classification.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.3.2/src/nyckel/functions/classification/text_classification.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/flower.jpg
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/test_duplicates_handling.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/test_field_handler.py
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/test_image_classification_function.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/test_image_decoder.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/test_label_handler.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/test_sample_handler.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/test_tabular_classification_function.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.3.2/tests/test_text_classification_function.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.3.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.3.2/LICENSE
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nyckel-0.3.2/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 nyckel-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 nyckel-0.3.3/mkdocs.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.3.3/requirements.txt
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.3.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.3.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.3.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.3.3/.vscode/extensions.json
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nyckel-0.3.3/.vscode/settings.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/copy_function.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/credentials.md
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/data_classes.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/delete_label.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/delete_samples.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/image_classification.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/index.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/merge_labels.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/multimodal_classification.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/quickstart.md
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/tabular_classification.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/text_classification.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/text_tags.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/assets/nyckel-logo.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.3.3/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/auth.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/config.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/data_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/py.typed
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/classification/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/classification/classification.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/classification/factory.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/classification/function_handler.py
+-rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/classification/image_classification.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/classification/label_handler.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/classification/sample_handler.py
+-rw-r--r--   0        0        0    17493 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/classification/tabular_classification.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/classification/text_classification.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/tags/tags.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/tags/tags_function_factory.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/tags/tags_function_handler.py
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/tags/tags_sample_handler.py
+-rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 nyckel-0.3.3/src/nyckel/functions/tags/text_tags.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/conftest.py
+-rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/flower.jpg
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/test_duplicates_handling.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/test_field_handler.py
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/test_image_classification_function.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/test_image_decoder.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/test_label_handler.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/test_sample_handler.py
+-rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/test_tabular_classification_function.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 nyckel-0.3.3/tests/test_text_tags_function.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nyckel-0.3.3/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 nyckel-0.3.3/PKG-INFO
```

### Comparing `nyckel-0.3.2/mkdocs.yml` & `nyckel-0.3.3/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     - Merge labels: merge_labels.md
     - Delete samples: delete_samples.md
     - Multimodal classification: multimodal_classification.md
   - Reference:
     - Image Classification: image_classification.md
     - Text Classification: text_classification.md
     - Tabular Classification: tabular_classification.md
+    - Text Tags: text_tags.md
     - Credentials: credentials.md
     - Data classes: data_classes.md
 theme: 
   name: 'material'
   features:
     - content.code.copy
   logo: assets/nyckel-logo.png
```

### Comparing `nyckel-0.3.2/.github/workflows/build.yml` & `nyckel-0.3.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/.github/workflows/docs.yml` & `nyckel-0.3.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/.github/workflows/test.yml` & `nyckel-0.3.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/.vscode/settings.json` & `nyckel-0.3.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/docs/copy_function.md` & `nyckel-0.3.3/docs/copy_function.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/docs/delete_label.md` & `nyckel-0.3.3/docs/delete_label.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/docs/delete_samples.md` & `nyckel-0.3.3/docs/delete_samples.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/docs/index.md` & `nyckel-0.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/docs/merge_labels.md` & `nyckel-0.3.3/docs/merge_labels.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/docs/multimodal_classification.md` & `nyckel-0.3.3/docs/multimodal_classification.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # Multimodal classification
 
 Nyckel supports multi-modal (joint) classification of images and text data through our Tabular function type.
 
 Below is an e-commerce example:
 
 ``` py
-from nyckel import Credentials, TabularClassificationFunction, TabularFunctionField, TabularFunctionSample, ClassificationAnnotation
+from nyckel import Credentials, TabularClassificationFunction, TabularFunctionField, TabularClassificationSample, ClassificationAnnotation
 
 credentials = Credentials(client_id="...", client_secret="...")
 
 func = TabularClassificationFunction.create("Product categories", credentials)
 func.create_fields([
     TabularFunctionField(name="Product", type="Text"),
     TabularFunctionField(name="Description", type="Text"),
     TabularFunctionField(name="Picture", type="Image")
 ])
 
 # <image-data> entires can be provided as URLs, base64-encoded dataURIs, or local file paths.
 func.create_samples(
     [
-        TabularFunctionSample(
+        TabularClassificationSample(
             data={"Product": "Acme wrench", "Description": "Solid steel; never breaks", "Picture": "<image-data>"},
             annotation=ClassificationAnnotation(label_name="Hardware"),
         ),
-        TabularFunctionSample(
+        TabularClassificationSample(
             data={"Product": "ULINE Hammer", "Description": "Hammer with wood handle", "Picture": "<image-data>"},
             annotation=ClassificationAnnotation(label_name="Hardware"),
         ),
-        TabularFunctionSample(
+        TabularClassificationSample(
             data={"Product": "Brooklinen bedding","Description": "Queen size bedding","Picture": "<image-data>"},
             annotation=ClassificationAnnotation(label_name="Bedding"),
         ),
-        TabularFunctionSample(
+        TabularClassificationSamplefo(
             data={"Product": "Comforter", "Description": "Nice down comforter", "Picture": "<image-data>"},
             annotation=ClassificationAnnotation(label_name="Bedding"),
         ),
     ]
 )
 ```
```

### Comparing `nyckel-0.3.2/docs/quickstart.md` & `nyckel-0.3.3/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/docs/assets/favicon.ico` & `nyckel-0.3.3/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/docs/assets/nyckel-logo.png` & `nyckel-0.3.3/docs/assets/nyckel-logo.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/__init__.py` & `nyckel-0.3.3/src/nyckel/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,7 +23,18 @@
 from .functions.classification.image_classification import (
     ImageClassificationFunction,  # noqa: F401
     ImageDecoder,  # noqa: F401
     ImageEncoder,  # noqa: F401
 )
 from .functions.classification.tabular_classification import TabularClassificationFunction  # noqa: F401
 from .functions.classification.text_classification import TextClassificationFunction  # noqa: F401
+from .functions.tags.tags import (
+    ImageTagsSample,
+    TabularTagsSample,
+    TagsAnnotation,
+    TagsFunction,
+    TagsPrediction,
+    TagsSample,
+    TextSampleData,
+    TextTagsSample,
+)
+from .functions.tags.text_tags import TextTagsFunction  # noqa: F401
```

### Comparing `nyckel-0.3.2/src/nyckel/auth.py` & `nyckel-0.3.3/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/request_utils.py` & `nyckel-0.3.3/src/nyckel/request_utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/functions/classification/classification.py` & `nyckel-0.3.3/src/nyckel/functions/classification/classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/functions/classification/factory.py` & `nyckel-0.3.3/src/nyckel/functions/classification/factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/functions/classification/function_handler.py` & `nyckel-0.3.3/src/nyckel/functions/classification/function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/functions/classification/image_classification.py` & `nyckel-0.3.3/src/nyckel/functions/classification/image_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/functions/classification/label_handler.py` & `nyckel-0.3.3/src/nyckel/functions/classification/label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/functions/classification/sample_handler.py` & `nyckel-0.3.3/src/nyckel/functions/classification/sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/functions/classification/tabular_classification.py` & `nyckel-0.3.3/src/nyckel/functions/classification/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/src/nyckel/functions/classification/text_classification.py` & `nyckel-0.3.3/src/nyckel/functions/classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/tests/conftest.py` & `nyckel-0.3.3/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Credentials,
     ImageClassificationFunction,
     ImageClassificationSample,
     TabularClassificationFunction,
     TabularClassificationSample,
     TextClassificationFunction,
     TextClassificationSample,
+    TextTagsFunction,
 )
 from nyckel.functions.classification.image_classification import ImageEncoder
 from PIL import Image
 
 
 def make_random_image(size: int = 100) -> str:
     imarray = np.random.rand(size, size, 3) * 255
@@ -126,14 +127,21 @@
     ]
     func.create_samples(samples)
     hold_until_list_samples_available(func, len(samples))
     yield func
     func.delete()
 
 
+@pytest.fixture
+def text_tags_function(auth_test_credentials: Credentials) -> Iterator[TextTagsFunction]:
+    func = TextTagsFunction.create("PYTHON-SDK TEXT TAGS TEST FUNCTION", auth_test_credentials)
+    yield func
+    func.delete()
+
+
 def get_test_credentials() -> Credentials:
     if "NYCKEL_PYTHON_SDK_CLIENT_SECRET" in os.environ:
         credentials = Credentials(
             client_id="python-sdk-test",
             client_secret=os.environ["NYCKEL_PYTHON_SDK_CLIENT_SECRET"],
             server_url="https://www.nyckel-staging.com",
         )
@@ -155,12 +163,11 @@
     session.headers.update({"authorization": "Bearer " + credentials.token})
     response = session.get(f"{credentials.server_url}/v0.9/projects")
     assert response.status_code == 200
     return len(response.json()) > 0
 
 
 def create_project_for_credentials(credentials: Credentials) -> None:
-    session = requests.Session()
-    session.headers.update({"authorization": "Bearer " + credentials.token})
+    session = credentials.get_session()
     print("-> Creating project for credentials")
     response = session.post(f"{credentials.server_url}/v0.9/projects", json={"name": "my_project"})
     assert response.status_code == 200
```

### Comparing `nyckel-0.3.2/tests/flower.jpg` & `nyckel-0.3.3/tests/flower.jpg`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/tests/test_duplicates_handling.py` & `nyckel-0.3.3/tests/test_duplicates_handling.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/tests/test_field_handler.py` & `nyckel-0.3.3/tests/test_field_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/tests/test_image_classification_function.py` & `nyckel-0.3.3/tests/test_image_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/tests/test_image_decoder.py` & `nyckel-0.3.3/tests/test_image_decoder.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/tests/test_label_handler.py` & `nyckel-0.3.3/tests/test_label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/tests/test_sample_handler.py` & `nyckel-0.3.3/tests/test_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/tests/test_tabular_classification_function.py` & `nyckel-0.3.3/tests/test_tabular_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/tests/test_text_classification_function.py` & `nyckel-0.3.3/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/.gitignore` & `nyckel-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/LICENSE` & `nyckel-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/README.md` & `nyckel-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.2/pyproject.toml` & `nyckel-0.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 [project]
 name = "nyckel"
-version = "0.3.2"
+version = "0.3.3"
 authors = [{ name = "Oscar Beijbom", email = "oscar@nyckel.com" }]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `nyckel-0.3.2/PKG-INFO` & `nyckel-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nyckel
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

