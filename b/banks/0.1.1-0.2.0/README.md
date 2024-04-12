# Comparing `tmp/banks-0.1.1.tar.gz` & `tmp/banks-0.2.0.tar.gz`

## Comparing `banks-0.1.1.tar` & `banks-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,42 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 banks-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 banks-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/__about__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/__init__.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/env.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/errors.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/loader.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/prompt.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/extensions/__init__.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/extensions/generate.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/filters/__init__.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/filters/lemmatize.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/templates/banks_macros.jinja
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/templates/blog.jinja
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/templates/generate_tweet.jinja
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/templates/run_prompt.jinja
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/templates/run_prompt_process.jinja
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/templates/summarize.jinja
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.1.1/src/banks/templates/summarize_lemma.jinja
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 banks-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 banks-0.1.1/tests/test_default_templates.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 banks-0.1.1/tests/test_env.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 banks-0.1.1/tests/test_loader.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 banks-0.1.1/tests/test_run_prompt.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 banks-0.1.1/tests/test_default_templates/blog.jinja.out
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 banks-0.1.1/tests/test_default_templates/generate_tweet.jinja.out
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 banks-0.1.1/tests/test_default_templates/summarize.jinja.out
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 banks-0.1.1/tests/test_default_templates/summarize_lemma.jinja.out
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.1.1/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 banks-0.1.1/README.md
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 banks-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 banks-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 banks-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 banks-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 banks-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 banks-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 banks-0.2.0/docs/extensions.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 banks-0.2.0/docs/filters.md
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 banks-0.2.0/docs/index.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 banks-0.2.0/docs/macros.md
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 banks-0.2.0/docs/python.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/__about__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/env.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/errors.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/loader.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/prompt.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/extensions/__init__.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/extensions/generate.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/extensions/inference_endpoint.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/filters/__init__.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/filters/lemmatize.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/banks_macros.jinja
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/blog.jinja
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/generate_tweet.jinja
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/run_prompt.jinja
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/run_prompt_process.jinja
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/summarize.jinja
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.2.0/src/banks/templates/summarize_lemma.jinja
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 banks-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_env.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_loader.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_run_prompt.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates/blog.jinja.out
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates/generate_tweet.jinja.out
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates/summarize.jinja.out
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 banks-0.2.0/tests/test_default_templates/summarize_lemma.jinja.out
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 banks-0.2.0/README.md
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 banks-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 banks-0.2.0/PKG-INFO
```

### Comparing `banks-0.1.1/.github/workflows/test.yml` & `banks-0.2.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   run:
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
```

### Comparing `banks-0.1.1/src/banks/loader.py` & `banks-0.2.0/src/banks/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from operator import itemgetter
-from typing import Optional
 
-from jinja2 import BaseLoader, PackageLoader, TemplateNotFound
+from jinja2 import BaseLoader, FileSystemLoader, PackageLoader, TemplateNotFound
 
 
 class MultiLoader(BaseLoader):
     """
     Similar to Jinja's ChoiceLoader with 2 notable differences:
       - Loaders can be added at runtime
       - Each loader has a priority so the caller can decide
         in which order the loaders are evaluated
     """
 
     def __init__(self) -> None:
         super().__init__()
-        self._loaders: list(BaseLoader) = []
-        # add a default loader
-        self.add_loader(PackageLoader("banks", "templates"), 1)
+        self._loaders: list[tuple[BaseLoader, int]] = []
+        # add default loaders
+        self.add_loader(PackageLoader("banks", "templates"), 10)
+        self.add_loader(FileSystemLoader("templates"), 20)
 
-    def add_loader(self, loader: BaseLoader, priority: Optional[int] = 100) -> None:
+    def add_loader(self, loader: BaseLoader, priority: int = 100) -> None:
         self._loaders.append((loader, priority))
 
     def get_source(self, environment, template):
         # Sort by priority, ascending
         for loader, _ in sorted(self._loaders, key=itemgetter(1)):
             try:
                 return loader.get_source(environment, template)
```

### Comparing `banks-0.1.1/src/banks/extensions/generate.py` & `banks-0.2.0/src/banks/extensions/generate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 # SPDX-FileCopyrightText: 2023-present Massimiliano Pippi <mpippi@gmail.com>
 #
 # SPDX-License-Identifier: MIT
-import openai
+from typing import cast
+
 from jinja2 import nodes
 from jinja2.ext import Extension
+from litellm import ModelResponse, completion
 
-CHAT_MODELS = [
-    "gpt-4",
-    "gpt-4-32k",
-    "gpt-3.5-turbo",
-]
 DEFAULT_MODEL = "gpt-3.5-turbo"
 
 
 class GenerateExtension(Extension):
+    """
+    `generate` can be used to call the OpenAI API passing the tag text as a prompt and get back some content.
+
+    Example:
+        ```
+        {% generate "write a tweet with positive sentiment" "gpt-3.5-turbo" %}
+        Feeling grateful for all the opportunities that come my way! #positivity #productivity
+        ```
+    """
+
     # a set of names that trigger the extension.
-    tags = {"generate"}
+    tags = {"generate"}  # noqa
 
     def parse(self, parser):
         # We get the line number of the first token so that we can give
         # that line number to the nodes we create by hand.
         lineno = next(parser.stream).lineno
 
         # The args passed to the extension:
         # - the prompt text used to generate new text
         # - (optional) the name of the model use to generate new text
         args = [parser.parse_expression()]
 
         return nodes.Output([self.call_method("_generate", args)]).set_lineno(lineno)
 
     def _generate(self, text, model_name=DEFAULT_MODEL):
-        """Helper callback."""
-        content = openai.ChatCompletion.create(
-            model=model_name,
-            messages=[
-                {"role": "system", "content": "You are a helpful assistant."},
-                {"role": "user", "content": text},
-            ],
-            temperature=0.5,
-        )["choices"][0]["message"]["content"]
+        """
+        Helper callback.
+
+        To tweak the prompt used to generate content, change the variable `messages` .
+        """
+        messages = [
+            {"role": "system", "content": "You are a helpful assistant."},
+            {"role": "user", "content": text},
+        ]
 
-        return content
+        response: ModelResponse = cast(ModelResponse, completion(model=model_name, messages=messages))
+        return response["choices"][0]["message"]["content"]
```

### Comparing `banks-0.1.1/tests/test_default_templates.py` & `banks-0.2.0/tests/test_default_templates.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: MIT
 import os
 from pathlib import Path
 from unittest import mock
 
 import pytest
 
-from banks import Prompt
+from banks import Prompt, env
 
 
 def _get_data(name):
     here = Path(os.path.dirname(os.path.abspath(__file__)))
     with open(here / "test_default_templates" / name) as f:
         return f.read()
 
@@ -36,10 +36,10 @@
 
     p = Prompt.from_template("summarize_lemma.jinja")
     assert _get_data("summarize_lemma.jinja.out") == p.text({"document": "The cats are running"})
 
 
 def test_generate_tweet():
     p = Prompt.from_template("generate_tweet.jinja")
-    p.env.extensions["banks.extensions.generate.GenerateExtension"]._generate = mock.MagicMock(return_value="foo")
+    env.extensions["banks.extensions.generate.GenerateExtension"]._generate = mock.MagicMock(return_value="foo")
 
     assert _get_data("generate_tweet.jinja.out") == p.text({"topic": "climate change"})
```

### Comparing `banks-0.1.1/tests/test_loader.py` & `banks-0.2.0/tests/test_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,34 +7,37 @@
 
 from banks import env
 from banks.loader import MultiLoader
 
 
 def test_defaults():
     test_loader = MultiLoader()
-    assert len(test_loader._loaders) == 1
+    assert len(test_loader._loaders) == 2
     loader, prio = test_loader._loaders[0]
     assert type(loader) == PackageLoader
-    assert prio == 1
+    assert prio == 10
+    loader, prio = test_loader._loaders[1]
+    assert type(loader) == FileSystemLoader
+    assert prio == 20
 
 
 def test_add_loader():
     test_loader = MultiLoader()
 
     # add a loader, default priority
     fs_loader = FileSystemLoader("")
     test_loader.add_loader(fs_loader)
-    assert test_loader._loaders[1][0] == fs_loader
-    assert test_loader._loaders[1][1] == 100
+    assert test_loader._loaders[2][0] == fs_loader
+    assert test_loader._loaders[2][1] == 100
 
     # add another one with priority
     another_loader = FileSystemLoader("")
     test_loader.add_loader(another_loader, 50)
-    assert test_loader._loaders[2][0] == another_loader
-    assert test_loader._loaders[2][1] == 50
+    assert test_loader._loaders[3][0] == another_loader
+    assert test_loader._loaders[3][1] == 50
 
 
 def test_get_source():
     test_loader = MultiLoader()
     # remove the default loader
     test_loader._loaders = []
```

### Comparing `banks-0.1.1/.gitignore` & `banks-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `banks-0.1.1/LICENSE.txt` & `banks-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `banks-0.1.1/README.md` & `banks-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 # banks
 
 [![PyPI - Version](https://img.shields.io/pypi/v/banks.svg)](https://pypi.org/project/banks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/banks.svg)](https://pypi.org/project/banks)
+
 [![PyPI Release](https://github.com/masci/banks/actions/workflows/release.yml/badge.svg)](https://github.com/masci/banks/actions/workflows/release.yml)
 [![test](https://github.com/masci/banks/actions/workflows/test.yml/badge.svg)](https://github.com/masci/banks/actions/workflows/test.yml)
+[![docs](https://github.com/masci/banks/actions/workflows/docs.yml/badge.svg)](https://github.com/masci/banks/actions/workflows/docs.yml)
+
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+[![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
 [Banks](https://en.wikipedia.org/wiki/Arrival_(film)) is the linguist professor who will help you generate meaningful LLM prompts using a template language that makes sense.
 If you're still using `f-strings` for the job, keep reading.
 
+> Docs are currently in the pipes and at the moment this README is the best resource for Banks' users, anyways they are
+> available [here](https://masci.github.io/banks/)
+
 -----
 
 **Table of Contents**
 
 - [banks](#banks)
   - [Installation](#installation)
   - [Examples](#examples)
@@ -175,14 +185,17 @@
 ```
 
 If you paste Banks' output into ChatGPT you would get something like this:
 ```txt
 Climate change is a pressing global issue, but together we can create positive change! Let's embrace renewable energy, protect our planet, and build a sustainable future for generations to come. 🌍💚 #ClimateAction #PositiveFuture
 ```
 
+The `generate` extension uses [LiteLLM](https://github.com/BerriAI/litellm) under the hood, and provided you have the
+proper environment variables set, you can use any model from the supported [model providers](https://docs.litellm.ai/docs/providers).
+
 ### Go meta: create a prompt and `generate` its response
 
 We can leverage Jinja's macro system to generate a prompt, send the result to OpenAI and get a response.
 Let's bring back the blog writing example:
 
 ```py
 from banks import Prompt
```

### Comparing `banks-0.1.1/pyproject.toml` & `banks-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "banks"
 dynamic = ["version"]
 description = 'A prompt programming language'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Massimiliano Pippi", email = "mpippi@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "jinja2",
-  "openai",
+  "litellm",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/banks#readme"
 Issues = "https://github.com/unknown/banks/issues"
 Source = "https://github.com/unknown/banks"
 
@@ -38,67 +38,70 @@
 path = "src/banks/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
 ]
+
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.lint]
-detached = true
+detached = false  # Normally the linting env can be detached, but mypy doesn't install all the stubs we need
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
 ]
+
 [tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:src/banks tests}"
+typing = "mypy --install-types --non-interactive {args:src/banks}"
 style = [
-  "ruff {args:.}",
+  "ruff check {args:.}",
   "black --check --diff {args:.}",
 ]
 fmt = [
   "black {args:.}",
-  "ruff --fix {args:.}",
+  "ruff check --fix {args:.}",
   "style",
 ]
 all = [
   "style",
-  # "typing",  # FIXME: re-enable once typing is good to go
+  "typing",
 ]
 
 [tool.hatch.build.targets.wheel]
 only-include = ["src/banks", "src/templates"]
 
 [tool.hatch.build.targets.wheel.sources]
 "src" = ""
 "templates" = "banks/templates"
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py39"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py39"
 line-length = 120
+[tool.ruff.lint]
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
@@ -133,21 +136,21 @@
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["banks"]
 
-[tool.ruff.flake8-tidy-imports]
-ban-relative-imports = "all"
+[tool.ruff.lint.flake8-tidy-imports]
+ban-relative-imports = "parents"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 source_pkgs = ["banks", "tests"]
 branch = true
 parallel = true
@@ -161,7 +164,14 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[[tool.mypy.overrides]]
+module = [
+  "simplemma.*",
+  "litellm.*"
+]
+ignore_missing_imports = true
```

### Comparing `banks-0.1.1/PKG-INFO` & `banks-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,51 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: banks
-Version: 0.1.1
+Version: 0.2.0
 Summary: A prompt programming language
 Project-URL: Documentation, https://github.com/unknown/banks#readme
 Project-URL: Issues, https://github.com/unknown/banks/issues
 Project-URL: Source, https://github.com/unknown/banks
 Author-email: Massimiliano Pippi <mpippi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: jinja2
-Requires-Dist: openai
+Requires-Dist: litellm
 Description-Content-Type: text/markdown
 
 # banks
 
 [![PyPI - Version](https://img.shields.io/pypi/v/banks.svg)](https://pypi.org/project/banks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/banks.svg)](https://pypi.org/project/banks)
+
 [![PyPI Release](https://github.com/masci/banks/actions/workflows/release.yml/badge.svg)](https://github.com/masci/banks/actions/workflows/release.yml)
 [![test](https://github.com/masci/banks/actions/workflows/test.yml/badge.svg)](https://github.com/masci/banks/actions/workflows/test.yml)
+[![docs](https://github.com/masci/banks/actions/workflows/docs.yml/badge.svg)](https://github.com/masci/banks/actions/workflows/docs.yml)
+
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+[![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
 [Banks](https://en.wikipedia.org/wiki/Arrival_(film)) is the linguist professor who will help you generate meaningful LLM prompts using a template language that makes sense.
 If you're still using `f-strings` for the job, keep reading.
 
+> Docs are currently in the pipes and at the moment this README is the best resource for Banks' users, anyways they are
+> available [here](https://masci.github.io/banks/)
+
 -----
 
 **Table of Contents**
 
 - [banks](#banks)
   - [Installation](#installation)
   - [Examples](#examples)
@@ -199,14 +209,17 @@
 ```
 
 If you paste Banks' output into ChatGPT you would get something like this:
 ```txt
 Climate change is a pressing global issue, but together we can create positive change! Let's embrace renewable energy, protect our planet, and build a sustainable future for generations to come. 🌍💚 #ClimateAction #PositiveFuture
 ```
 
+The `generate` extension uses [LiteLLM](https://github.com/BerriAI/litellm) under the hood, and provided you have the
+proper environment variables set, you can use any model from the supported [model providers](https://docs.litellm.ai/docs/providers).
+
 ### Go meta: create a prompt and `generate` its response
 
 We can leverage Jinja's macro system to generate a prompt, send the result to OpenAI and get a response.
 Let's bring back the blog writing example:
 
 ```py
 from banks import Prompt
```

