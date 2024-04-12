# Comparing `tmp/pyannotators_patterns-0.5.80.tar.gz` & `tmp/pyannotators-patterns-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyannotators_patterns-0.5.80.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyannotators-patterns-0.5.9.tar", last modified: Tue Oct  4 16:35:35 2022, max compression
```

## Comparing `pyannotators_patterns-0.5.80.tar` & `pyannotators-patterns-0.5.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      497 2023-10-27 06:19:47.009818 pyannotators_patterns-0.5.80/.bumpversion.cfg
--rw-r--r--   0        0        0     1386 2023-10-27 06:19:47.009818 pyannotators_patterns-0.5.80/.github/workflows/main.yml
--rw-r--r--   0        0        0     1786 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/.gitignore
--rw-r--r--   0        0        0      419 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/.readthedocs.yml
--rw-r--r--   0        0        0      117 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/AUTHORS.md
--rw-r--r--   0        0        0      268 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/CHANGELOG.md
--rw-r--r--   0        0        0      448 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/Dockerfile
--rw-r--r--   0        0        0    13976 2024-01-23 08:19:17.997878 pyannotators_patterns-0.5.80/Jenkinsfile
--rw-r--r--   0        0        0     1082 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/LICENSE
--rw-r--r--   0        0        0     1549 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/README.md
--rw-r--r--   0        0        0      941 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/RELEASE.md
--rw-r--r--   0        0        0     1559 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/bumpversion.py
--rw-r--r--   0        0        0       62 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/docs/.gitignore
--rw-r--r--   0        0        0      268 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/docs/LICENSE
--rw-r--r--   0        0        0        0 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2879 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/docs/conf.py
--rw-r--r--   0        0        0      142 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/docs/index.rst
--rw-r--r--   0        0        0    20480 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/hgnc_cache.sqlite
--rw-r--r--   0        0        0       98 2023-10-27 06:19:47.013818 pyannotators_patterns-0.5.80/mypy.ini
--rw-r--r--   0        0        0     2297 2024-01-23 11:54:06.911195 pyannotators_patterns-0.5.80/pyproject.toml
--rw-r--r--   0        0        0       76 2024-04-12 12:15:56.772127 pyannotators_patterns-0.5.80/src/pyannotators_patterns/__init__.py
--rw-r--r--   0        0        0     9503 2024-04-12 12:13:25.735459 pyannotators_patterns-0.5.80/src/pyannotators_patterns/patterns.py
--rw-r--r--   0        0        0      987 2023-10-27 06:19:47.017818 pyannotators_patterns-0.5.80/tests/assertions.py
--rw-r--r--   0        0        0     1817 2023-10-27 06:19:47.017818 pyannotators_patterns-0.5.80/tests/test_credit_cards.py
--rw-r--r--   0        0        0     1798 2023-10-27 06:19:47.017818 pyannotators_patterns-0.5.80/tests/test_emails.py
--rw-r--r--   0        0        0     1406 2023-10-27 06:19:47.017818 pyannotators_patterns-0.5.80/tests/test_zip.py
--rw-r--r--   0        0        0      943 2023-10-27 06:19:47.017818 pyannotators_patterns-0.5.80/tox.ini
--rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 pyannotators_patterns-0.5.80/setup.py
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 pyannotators_patterns-0.5.80/PKG-INFO
+-rw-r--r--   0        0        0      497 2022-10-04 13:12:34.795830 pyannotators-patterns-0.5.9/.bumpversion.cfg
+-rw-r--r--   0        0        0     1386 2022-10-04 13:12:34.797830 pyannotators-patterns-0.5.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1743 2022-10-04 13:12:34.798830 pyannotators-patterns-0.5.9/.gitignore
+-rw-r--r--   0        0        0      419 2022-10-04 13:12:34.798830 pyannotators-patterns-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/.readthedocs.yml
+-rw-r--r--   0        0        0      117 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/AUTHORS.md
+-rw-r--r--   0        0        0      268 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/CHANGELOG.md
+-rw-r--r--   0        0        0      448 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/Dockerfile
+-rw-r--r--   0        0        0     9926 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/LICENSE
+-rw-r--r--   0        0        0     1549 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/README.md
+-rw-r--r--   0        0        0      941 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/RELEASE.md
+-rw-r--r--   0        0        0     1559 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/bumpversion.py
+-rw-r--r--   0        0        0       62 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/docs/.gitignore
+-rw-r--r--   0        0        0      268 2022-10-04 13:12:34.799830 pyannotators-patterns-0.5.9/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2022-10-04 13:12:34.800830 pyannotators-patterns-0.5.9/docs/LICENSE
+-rw-r--r--   0        0        0        0 2022-10-04 13:12:34.800830 pyannotators-patterns-0.5.9/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-10-04 13:12:34.801830 pyannotators-patterns-0.5.9/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2879 2022-10-04 13:12:34.801830 pyannotators-patterns-0.5.9/docs/conf.py
+-rw-r--r--   0        0        0      142 2022-10-04 13:12:34.801830 pyannotators-patterns-0.5.9/docs/index.rst
+-rw-r--r--   0        0        0    20480 2022-10-04 13:12:34.801830 pyannotators-patterns-0.5.9/hgnc_cache.sqlite
+-rw-r--r--   0        0        0       98 2022-10-04 13:12:34.801830 pyannotators-patterns-0.5.9/mypy.ini
+-rw-r--r--   0        0        0     2309 2022-10-04 13:12:34.801830 pyannotators-patterns-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0       75 2022-10-04 16:35:33.833003 pyannotators-patterns-0.5.9/src/pyannotators_patterns/__init__.py
+-rw-r--r--   0        0        0     9227 2022-10-04 13:12:34.803830 pyannotators-patterns-0.5.9/src/pyannotators_patterns/patterns.py
+-rw-r--r--   0        0        0      987 2022-10-04 13:12:34.803830 pyannotators-patterns-0.5.9/tests/assertions.py
+-rw-r--r--   0        0        0     1817 2022-10-04 13:12:34.803830 pyannotators-patterns-0.5.9/tests/test_credit_cards.py
+-rw-r--r--   0        0        0     1798 2022-10-04 13:12:34.803830 pyannotators-patterns-0.5.9/tests/test_emails.py
+-rw-r--r--   0        0        0     1406 2022-10-04 13:12:34.803830 pyannotators-patterns-0.5.9/tests/test_zip.py
+-rw-r--r--   0        0        0      943 2022-10-04 13:12:34.803830 pyannotators-patterns-0.5.9/tox.ini
+-rw-r--r--   0        0        0     1404 1970-01-01 00:00:00.000000 pyannotators-patterns-0.5.9/setup.py
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 pyannotators-patterns-0.5.9/PKG-INFO
```

### Comparing `pyannotators_patterns-0.5.80/.github/workflows/main.yml` & `pyannotators-patterns-0.5.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/.gitignore` & `pyannotators-patterns-0.5.9/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -121,11 +121,8 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
-# Specific
-.idea/
-.groovylintrc.json
-.emailNotif
+.idea/
```

### Comparing `pyannotators_patterns-0.5.80/LICENSE` & `pyannotators-patterns-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/README.md` & `pyannotators-patterns-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/RELEASE.md` & `pyannotators-patterns-0.5.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/bumpversion.py` & `pyannotators-patterns-0.5.9/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/docs/LICENSE` & `pyannotators-patterns-0.5.9/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/docs/conf.py` & `pyannotators-patterns-0.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/hgnc_cache.sqlite` & `pyannotators-patterns-0.5.9/hgnc_cache.sqlite`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/pyproject.toml` & `pyannotators-patterns-0.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,19 @@
     "Topic :: Software Development",
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.8",
 ]
 requires = [
     "pymultirole-plugins>=0.5.0,<0.6.0",
-    "spacy[lookups]==3.4.4",
+    "spacy==3.4.0",
+    "spacy[lookups]",
     "collections_extended",
     "unidecode",
-    "presidio-analyzer>=2.2.352"
+    "presidio-analyzer>=2.2.29"
 ]
 dist-name = "pyannotators-patterns"
 
 [tool.flit.entrypoints."pyannotators.plugins"]
 patterns = "pyannotators_patterns.patterns:PatternsAnnotator"
 
 [tool.flit.metadata.requires-extra]
```

### Comparing `pyannotators_patterns-0.5.80/src/pyannotators_patterns/patterns.py` & `pyannotators-patterns-0.5.9/src/pyannotators_patterns/patterns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 from functools import lru_cache
 from typing import Type, List, cast, Dict
 
 import spacy
 from presidio_analyzer import Pattern, PatternRecognizer, RecognizerRegistry, AnalyzerEngine, LemmaContextAwareEnhancer
-from presidio_analyzer.nlp_engine import SpacyNlpEngine, NerModelConfiguration
+from presidio_analyzer.nlp_engine import SpacyNlpEngine
 from pydantic import BaseModel, Field
 from pymultirole_plugins.util import comma_separated_to_list
 from pymultirole_plugins.v1.annotator import AnnotatorParameters, AnnotatorBase
 from pymultirole_plugins.v1.schema import Document, Span, Annotation
 from spacy.cli.download import download_model, get_compatibility, get_version
 from spacy.language import Language
 from wasabi import msg
@@ -42,15 +42,15 @@
 
 
 class PatternsParameters(AnnotatorParameters):
     mapping: Dict[str, str] = Field(None,
                                     description="""List of regex patterns to be used by the annotator and optionnal list of context words to increase confidence in detection.<br/>
                             Each pattern is composed of a name, a list of python regular expressions and a score indicating the pattern's strength (values varies from 0 to 1).<br/>
                             For example you can define a regex pattern to recognize credit card numbers addresses along with some [context words](https://microsoft.github.io/presidio/tutorial/06_context/) like this:<br/>
-    ```""" + PATTERNS_EXAMPLE_STR + "```", extra="key:label,val:json")
+    ```""" + PATTERNS_EXAMPLE_STR + "```", extra="json")
 
     score_threshold: float = Field(0.0, description="Minimum confidence value for detected entities to be returned")
     context_similarity_factor: float = Field(0.0,
                                              description="How much to enhance confidence of match entity, as explained [here](https://microsoft.github.io/presidio/tutorial/06_context/)",
                                              extra="advanced")
     min_score_with_context_similarity: float = Field(0.4,
                                                      description="Minimum confidence score, as explained [here](https://microsoft.github.io/presidio/tutorial/06_context/)",
@@ -63,34 +63,34 @@
                                       extra="advanced")
 
 
 SUPPORTED_LANGUAGES = "en,fr,de,nl,es,pt,it,zh,ar,ru"
 
 
 class PatternsAnnotator(AnnotatorBase):
-    __doc__ = """Patterns annotator using the Presidio [regex pattern recognizer](https://microsoft.github.io/presidio/tutorial/02_regex/).
-    Regular expressions can be tested [here](https://regex101.com/).
+    """Patterns annotator using the Presidio [regex pattern recognizer](https://microsoft.github.io/presidio/tutorial/02_regex/).
     #need-segments
     #languages:""" + SUPPORTED_LANGUAGES
 
     def annotate(
             self, documents: List[Document], parameters: AnnotatorParameters
     ) -> List[Document]:
         params: PatternsParameters = cast(PatternsParameters, parameters)
         supported_languages = comma_separated_to_list(SUPPORTED_LANGUAGES)
 
         mapping = frozenset(params.mapping.items())
         labels = list(params.mapping.keys())
+        registry = get_registry(mapping)
+
         for document in documents:
             # Retrieve nlp pipe
             lang = document_language(document, None)
             if lang is None or lang not in supported_languages:
                 raise AttributeError(f"Metadata language {lang} is required and must be in {SUPPORTED_LANGUAGES}")
             nlp = get_nlp(lang)
-            registry = get_registry(mapping, lang)
             analyzer = AnalyzerEngine(registry=registry,
                                       nlp_engine=LoadedSpacyNlpEngine(lang, nlp),
                                       default_score_threshold=0,
                                       supported_languages=supported_languages,
                                       context_aware_enhancer=LemmaContextAwareEnhancer(params.context_similarity_factor,
                                                                                        params.min_score_with_context_similarity,
                                                                                        params.context_prefix_count,
@@ -151,27 +151,26 @@
     except BaseException:
         nlp = load_spacy_model(model)
     return nlp
 
 
 # Create a class inheriting from SpacyNlpEngine
 class LoadedSpacyNlpEngine(SpacyNlpEngine):
-    def __init__(self, lang, loaded_spacy_model, ner_model_configuration=None):
+    def __init__(self, lang, loaded_spacy_model):
         self.nlp = {lang: loaded_spacy_model}
-        self.ner_model_configuration = ner_model_configuration or NerModelConfiguration()
 
 
 @lru_cache(maxsize=None)
-def get_registry(mapping_items, lang):
+def get_registry(mapping_items):
     recognizers = []
     for pname, pvalue in mapping_items:
         pattern_definition = json.loads(pvalue)
         patterns = [Pattern.from_dict(pat) for pat in pattern_definition['patterns']]
         recognizer = PatternRecognizer(
-            supported_entity=pname, supported_language=lang, patterns=patterns, context=pattern_definition.get('context', None)
+            supported_entity=pname, patterns=patterns, context=pattern_definition.get('context', None)
         )
         recognizers.append(recognizer)
     registry = RecognizerRegistry(recognizers)
     return registry
 
 
 def load_spacy_model(model, *pip_args):
```

### Comparing `pyannotators_patterns-0.5.80/tests/assertions.py` & `pyannotators-patterns-0.5.9/tests/assertions.py`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/tests/test_credit_cards.py` & `pyannotators-patterns-0.5.9/tests/test_credit_cards.py`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/tests/test_emails.py` & `pyannotators-patterns-0.5.9/tests/test_emails.py`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/tests/test_zip.py` & `pyannotators-patterns-0.5.9/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/tox.ini` & `pyannotators-patterns-0.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `pyannotators_patterns-0.5.80/setup.py` & `pyannotators-patterns-0.5.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 {'': ['*']}
 
 package_dir = \
 {'': 'src'}
 
 install_requires = \
 ['pymultirole-plugins>=0.5.0,<0.6.0',
- 'spacy[lookups]==3.4.4',
+ 'spacy==3.4.0',
+ 'spacy[lookups]',
  'collections_extended',
  'unidecode',
- 'presidio-analyzer>=2.2.352']
+ 'presidio-analyzer>=2.2.29']
 
 extras_require = \
 {'dev': ['flit', 'pre-commit', 'bump2version'],
  'docs': ['sphinx',
           'sphinx-rtd-theme',
           'm2r2',
           'sphinxcontrib.apidoc',
@@ -35,15 +36,15 @@
           'dirty-equals']}
 
 entry_points = \
 {'pyannotators.plugins': ['patterns = '
                           'pyannotators_patterns.patterns:PatternsAnnotator']}
 
 setup(name='pyannotators-patterns',
-      version='0.5.80',
+      version='0.5.9',
       description='Annotator based on Presidio pattern recognizer',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyannotators_patterns/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyannotators_patterns-0.5.80/PKG-INFO` & `pyannotators-patterns-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannotators-patterns
-Version: 0.5.80
+Version: 0.5.9
 Summary: Annotator based on Presidio pattern recognizer
 Home-page: https://github.com/oterrier/pyannotators_patterns/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -16,18 +16,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: pymultirole-plugins>=0.5.0,<0.6.0
-Requires-Dist: spacy[lookups]==3.4.4
+Requires-Dist: spacy==3.4.0
+Requires-Dist: spacy[lookups]
 Requires-Dist: collections_extended
 Requires-Dist: unidecode
-Requires-Dist: presidio-analyzer>=2.2.352
+Requires-Dist: presidio-analyzer>=2.2.29
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: m2r2 ; extra == "docs"
 Requires-Dist: sphinxcontrib.apidoc ; extra == "docs"
```

