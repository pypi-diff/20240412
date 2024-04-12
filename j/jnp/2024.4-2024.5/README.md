# Comparing `tmp/jnp-2024.4.tar.gz` & `tmp/jnp-2024.5.tar.gz`

## Comparing `jnp-2024.4.tar` & `jnp-2024.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jnp-2024.4/.gitlab-ci.yml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 jnp-2024.4/CITATION.cff
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 jnp-2024.4/TODO.md
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 jnp-2024.4/codemeta.json
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jnp-2024.4/config.yaml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jnp-2024.4/config/index.html
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jnp-2024.4/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jnp-2024.4/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 jnp-2024.4/doc/requirements.txt
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 jnp-2024.4/doc/source/conf.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jnp-2024.4/doc/source/index.rst
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 jnp-2024.4/doc/source/jnp.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jnp-2024.4/doc/source/modules.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jnp-2024.4/doc/source/readme.md
--rw-r--r--   0        0        0    13557 2020-02-02 00:00:00.000000 jnp-2024.4/presentations/img/url.svg
--rw-r--r--   0        0        0    98272 2020-02-02 00:00:00.000000 jnp-2024.4/presentations/notebooks/example_presentation_01.ipynb
--rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 jnp-2024.4/scripts/generate_url_qrcode.sh
--rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 jnp-2024.4/scripts/jupyter-lab-venv.sh
--rwxr-xr-x   0        0        0      425 2020-02-02 00:00:00.000000 jnp-2024.4/scripts/publish.sh
--rwxr-xr-x   0        0        0      228 2020-02-02 00:00:00.000000 jnp-2024.4/scripts/update_notebook.sh
--rwxr-xr-x   0        0        0     2933 2020-02-02 00:00:00.000000 jnp-2024.4/scripts/update_readme.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/__init__.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/bugfixes.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/common.py
--rw-r--r--   0        0        0     9858 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/config.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/css.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/file.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/main.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/manager.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/notebook.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/text.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/version.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/resources/index.css
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/resources/index.html
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/resources/main.css
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/resources/reveal.css
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jnp-2024.4/src/jnp/resources/sizes.css
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jnp-2024.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jnp-2024.4/LICENSE.txt
--rw-r--r--   0        0        0    14987 2020-02-02 00:00:00.000000 jnp-2024.4/README.md
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jnp-2024.4/pyproject.toml
--rw-r--r--   0        0        0    16900 2020-02-02 00:00:00.000000 jnp-2024.4/PKG-INFO
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jnp-2024.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 jnp-2024.5/CITATION.cff
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 jnp-2024.5/TODO.md
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 jnp-2024.5/codemeta.json
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jnp-2024.5/config.yaml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jnp-2024.5/config/index.html
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jnp-2024.5/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jnp-2024.5/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 jnp-2024.5/doc/requirements.txt
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 jnp-2024.5/doc/source/conf.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jnp-2024.5/doc/source/index.rst
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 jnp-2024.5/doc/source/jnp.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jnp-2024.5/doc/source/modules.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jnp-2024.5/doc/source/readme.md
+-rw-r--r--   0        0        0    13557 2020-02-02 00:00:00.000000 jnp-2024.5/presentations/img/url.svg
+-rw-r--r--   0        0        0    98272 2020-02-02 00:00:00.000000 jnp-2024.5/presentations/notebooks/example_presentation_01.ipynb
+-rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 jnp-2024.5/scripts/generate_url_qrcode.sh
+-rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 jnp-2024.5/scripts/jupyter-lab-venv.sh
+-rwxr-xr-x   0        0        0      425 2020-02-02 00:00:00.000000 jnp-2024.5/scripts/publish.sh
+-rwxr-xr-x   0        0        0      228 2020-02-02 00:00:00.000000 jnp-2024.5/scripts/update_notebook.sh
+-rwxr-xr-x   0        0        0     2933 2020-02-02 00:00:00.000000 jnp-2024.5/scripts/update_readme.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/__init__.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/bugfixes.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/common.py
+-rw-r--r--   0        0        0     9858 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/config.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/css.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/file.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/main.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/manager.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/notebook.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/text.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/version.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/resources/index.css
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/resources/index.html
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/resources/main.css
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/resources/reveal.css
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jnp-2024.5/src/jnp/resources/sizes.css
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jnp-2024.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jnp-2024.5/LICENSE.txt
+-rw-r--r--   0        0        0    14987 2020-02-02 00:00:00.000000 jnp-2024.5/README.md
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jnp-2024.5/pyproject.toml
+-rw-r--r--   0        0        0    16900 2020-02-02 00:00:00.000000 jnp-2024.5/PKG-INFO
```

### Comparing `jnp-2024.4/.gitlab-ci.yml` & `jnp-2024.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/CITATION.cff` & `jnp-2024.5/CITATION.cff`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 abstract: Export Jupyter notebook presentations with custom CSS.
 authors:
 - email: jan-michael.rye@inria.fr
   family-names: Rye
   given-names: Jan-Michael
   orcid: https://orcid.org/0009-0005-0109-6598
 cff-version: 1.2.0
-date-released: '2021-07-18'
 identifiers:
 - description: The Software Heritage URL.
   type: url
   value: https://archive.softwareheritage.org/browse/origin/?origin_url=https%3A//gitlab.inria.fr/jrye/jnp.git
 license: MIT
 message: If you use this software, please cite it using these metadata.
 repository-code: https://gitlab.inria.fr/jrye/jnp.git
 title: jnp
-version: '2024.4'
+version: '2024.5'
```

### Comparing `jnp-2024.4/TODO.md` & `jnp-2024.5/TODO.md`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/codemeta.json` & `jnp-2024.5/codemeta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'2024.5'"}*

```diff
@@ -79,9 +79,9 @@
         "@type": "CommandLineApplication",
         "description": "Export Jupyter notebooks to presentations",
         "executableName": "jnp",
         "name": "jnp",
         "runtimePlatform": "Python 3"
     },
     "url": "https://gitlab.inria.fr/jrye/jnp",
-    "version": "2024.4"
+    "version": "2024.5"
 }
```

### Comparing `jnp-2024.4/doc/Makefile` & `jnp-2024.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/doc/make.bat` & `jnp-2024.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/doc/source/conf.py` & `jnp-2024.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/doc/source/jnp.rst` & `jnp-2024.5/doc/source/jnp.rst`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/presentations/img/url.svg` & `jnp-2024.5/presentations/img/url.svg`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/presentations/notebooks/example_presentation_01.ipynb` & `jnp-2024.5/presentations/notebooks/example_presentation_01.ipynb`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/scripts/generate_url_qrcode.sh` & `jnp-2024.5/scripts/generate_url_qrcode.sh`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/scripts/jupyter-lab-venv.sh` & `jnp-2024.5/scripts/jupyter-lab-venv.sh`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/scripts/update_readme.py` & `jnp-2024.5/scripts/update_readme.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/bugfixes.py` & `jnp-2024.5/src/jnp/bugfixes.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/config.py` & `jnp-2024.5/src/jnp/config.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/css.py` & `jnp-2024.5/src/jnp/css.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/file.py` & `jnp-2024.5/src/jnp/file.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/main.py` & `jnp-2024.5/src/jnp/main.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/manager.py` & `jnp-2024.5/src/jnp/manager.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/notebook.py` & `jnp-2024.5/src/jnp/notebook.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/text.py` & `jnp-2024.5/src/jnp/text.py`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/resources/main.css` & `jnp-2024.5/src/jnp/resources/main.css`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/resources/reveal.css` & `jnp-2024.5/src/jnp/resources/reveal.css`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/src/jnp/resources/sizes.css` & `jnp-2024.5/src/jnp/resources/sizes.css`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/LICENSE.txt` & `jnp-2024.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/README.md` & `jnp-2024.5/README.md`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/pyproject.toml` & `jnp-2024.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jnp-2024.4/PKG-INFO` & `jnp-2024.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jnp
-Version: 2024.4
+Version: 2024.5
 Summary: Export Jupyter notebook presentations with custom CSS.
 Project-URL: Homepage, https://gitlab.inria.fr/jrye/jnp
 Project-URL: Source, https://gitlab.inria.fr/jrye/jnp.git
 Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/jnp
 Project-URL: Issues, https://gitlab.inria.fr/jrye/jnp/-/issues
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
 License: MIT License
```

