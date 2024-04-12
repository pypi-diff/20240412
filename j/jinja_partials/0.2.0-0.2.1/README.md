# Comparing `tmp/jinja_partials-0.2.0.tar.gz` & `tmp/jinja_partials-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja_partials-0.2.0.tar", last modified: Thu Feb  1 15:35:45 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jinja_partials-0.2.0.tar` & `jinja_partials-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 michaelkennedy   (501) staff       (20)        0 2024-02-01 15:35:45.058194 jinja_partials-0.2.0/
--rw-r--r--   0 michaelkennedy   (501) staff       (20)     1072 2021-07-26 19:14:33.000000 jinja_partials-0.2.0/LICENSE
--rw-r--r--   0 michaelkennedy   (501) staff       (20)     4973 2024-02-01 15:35:45.057994 jinja_partials-0.2.0/PKG-INFO
--rw-r--r--   0 michaelkennedy   (501) staff       (20)     4146 2024-02-01 15:25:47.000000 jinja_partials-0.2.0/README.md
-drwxr-xr-x   0 michaelkennedy   (501) staff       (20)        0 2024-02-01 15:35:45.055318 jinja_partials-0.2.0/jinja_partials/
--rw-r--r--   0 michaelkennedy   (501) staff       (20)     2385 2024-02-01 15:29:20.000000 jinja_partials-0.2.0/jinja_partials/__init__.py
-drwxr-xr-x   0 michaelkennedy   (501) staff       (20)        0 2024-02-01 15:35:45.057735 jinja_partials-0.2.0/jinja_partials.egg-info/
--rw-r--r--   0 michaelkennedy   (501) staff       (20)     4973 2024-02-01 15:35:45.000000 jinja_partials-0.2.0/jinja_partials.egg-info/PKG-INFO
--rw-r--r--   0 michaelkennedy   (501) staff       (20)      266 2024-02-01 15:35:45.000000 jinja_partials-0.2.0/jinja_partials.egg-info/SOURCES.txt
--rw-r--r--   0 michaelkennedy   (501) staff       (20)        1 2024-02-01 15:35:45.000000 jinja_partials-0.2.0/jinja_partials.egg-info/dependency_links.txt
--rw-r--r--   0 michaelkennedy   (501) staff       (20)        7 2024-02-01 15:35:45.000000 jinja_partials-0.2.0/jinja_partials.egg-info/requires.txt
--rw-r--r--   0 michaelkennedy   (501) staff       (20)       15 2024-02-01 15:35:45.000000 jinja_partials-0.2.0/jinja_partials.egg-info/top_level.txt
--rw-r--r--   0 michaelkennedy   (501) staff       (20)       38 2024-02-01 15:35:45.058240 jinja_partials-0.2.0/setup.cfg
--rw-r--r--   0 michaelkennedy   (501) staff       (20)     1886 2021-07-26 21:43:51.000000 jinja_partials-0.2.0/setup.py
-drwxr-xr-x   0 michaelkennedy   (501) staff       (20)        0 2024-02-01 15:35:45.057072 jinja_partials-0.2.0/tests/
--rw-r--r--   0 michaelkennedy   (501) staff       (20)     3174 2024-02-01 15:32:37.000000 jinja_partials-0.2.0/tests/test_rendering.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/requirements.txt
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/setup.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/.idea/jinja_partials.iml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/.idea/modules.xml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/.idea/ruff.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/.idea/vcs.xml
+-rw-r--r--   0        0        0    20350 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/jinja_partials/__init__.py
+-rw-r--r--   0        0        0   656529 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/readme_resources/home.png
+-rw-r--r--   0        0        0  1658797 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/readme_resources/listing.png
+-rw-r--r--   0        0        0   214998 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/readme_resources/reused-html-visual.jpg
+-rw-r--r--   0        0        0   536311 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/readme_resources/reused-html-visual.png
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/README.md
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 jinja_partials-0.2.1/PKG-INFO
```

### Comparing `jinja_partials-0.2.0/LICENSE` & `jinja_partials-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja_partials-0.2.0/PKG-INFO` & `jinja_partials-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jinja_partials
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple reuse of partial HTML page templates in the Jinja template language for Python web frameworks.
-Home-page: https://github.com/mikeckennedy/jinja_partials
-Author: Michael Kennedy
-Author-email: michael@talkpython.fm
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
+Project-URL: Homepage, https://github.com/mikeckennedy/jinja_partials
+Project-URL: Tracker, https://github.com/mikeckennedy/jinja_partials/issues
+Project-URL: Source, https://github.com/mikeckennedy/jinja_partials
+Author-email: Michael Kennedy <michael@talkpython.fm>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: html,templates,web
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Requires-Dist: jinja2
+Description-Content-Type: text/markdown
 
 # Jinja Partials
 
 Simple reuse of partial HTML page templates in the Jinja template language for Python web frameworks.
 (There is also a [Pyramid/Chameleon version here](https://github.com/mikeckennedy/chameleon_partials).)
 
 ## Overview
@@ -144,8 +147,8 @@
 This time, we reframe each item in the list from the outer template (called `v`) as the `video` model
 in the inner HTML section.
 
 
 ## Why not just use `include` or `macro` from Jinja?
 
 The short answer is they are nearly the same, but both fall short in different ways. 
-For a more detailed response, see the discussion on [**issue #1**](https://github.com/mikeckennedy/jinja_partials/issues/1)
+For a more detailed response, see the discussion on [**issue #1**](https://github.com/mikeckennedy/jinja_partials/issues/1)
```

#### html2text {}

```diff
@@ -1,55 +1,58 @@
-Metadata-Version: 2.1 Name: jinja_partials Version: 0.2.0 Summary: Simple reuse
+Metadata-Version: 2.3 Name: jinja_partials Version: 0.2.1 Summary: Simple reuse
 of partial HTML page templates in the Jinja template language for Python web
-frameworks. Home-page: https://github.com/mikeckennedy/jinja_partials Author:
-Michael Kennedy Author-email: michael@talkpython.fm License: MIT Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: jinja2 # Jinja Partials
-Simple reuse of partial HTML page templates in the Jinja template language for
-Python web frameworks. (There is also a [Pyramid/Chameleon version here](https:
-//github.com/mikeckennedy/chameleon_partials).) ## Overview When building real-
-world web apps with Flask + Jinja2, it's easy to end up with repeated HTML
-fragments. Just like organizing code for reuse, it would be ideal to reuse
-smaller sections of HTML template code. That's what this library is all about.
-## Example This project comes with a sample flask application (see the
-`example` folder). This app displays videos that can be played on YouTube. The
-image, subtitle of author and view count are reused throughout the app. Here's
-a visual: ![](https://raw.githubusercontent.com/mikeckennedy/jinja_partials/
-main/readme_resources/reused-html-visual.png) Check out the [**demo / example
-application**](https://github.com/mikeckennedy/jinja_partials/tree/main/
-example) to see it in action. ## Installation It's just `pip install jinja-
-partials` and you're all set with this pure Python package. ## Usage Using the
-library is incredible easy. The first step is to register the partial method
-with Jinja and Flask. Do this once at app startup: ```python import flask
-import jinja_partials app = flask.Flask(__name__)
-jinja_partials.register_extensions(app) # ... ``` You can also use this library
-in your FastAPI (or Starlette) project! ```python from fastapi.templating
-import Jinja2Templates # or `from starlette.templating import Jinja2Templates`
-import jinja_partials templates = Jinja2Templates("tests/test_templates")
-jinja_partials.register_starlette_extensions(templates) # ... ``` Or directly
-using a jijna environment! ```python import jinja_partials from jinja2 import
-Environment, FileSystemLoader environment = Environment(loader=FileSystemLoader
-("tests/test_templates")) jinja_partials.register_environment(environment) #
-... ``` Next, you define your main HTML (Jinja2) templates as usual. Then
-define your partial templates. I recommend locating and naming them
-accordingly: ``` âââ templates âÂ Â  âââ home âÂ Â  âÂ Â 
-âââ index.html âÂ Â  âÂ Â  âââ listing.html âÂ Â  âââ
-shared âÂ Â  âââ _layout.html âÂ Â  âââ partials âÂ Â 
-âââ video_image.html âÂ Â  âââ video_square.html ``` Notice the
-`partials` subfolder in the `templates/shared` folder. The templates are just
-HTML fragments. Here is a stand-alone one for the YouTube thumbnail from the
-example app: ```html [{{ video.title }}]``` Notice that an object called
-`video` and list of classes are passed in as the model. Templates can also be
-nested. Here is the whole single video fragment with the image as well as other
-info linking out to YouTube: ```html
+frameworks. Project-URL: Homepage, https://github.com/mikeckennedy/
+jinja_partials Project-URL: Tracker, https://github.com/mikeckennedy/
+jinja_partials/issues Project-URL: Source, https://github.com/mikeckennedy/
+jinja_partials Author-email: Michael Kennedy
+talkpython.fm> License-Expression: MIT License-File: LICENSE Keywords:
+html,templates,web Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Python: >=3.8 Requires-Dist: jinja2 Description-
+Content-Type: text/markdown # Jinja Partials Simple reuse of partial HTML page
+templates in the Jinja template language for Python web frameworks. (There is
+also a [Pyramid/Chameleon version here](https://github.com/mikeckennedy/
+chameleon_partials).) ## Overview When building real-world web apps with Flask
++ Jinja2, it's easy to end up with repeated HTML fragments. Just like
+organizing code for reuse, it would be ideal to reuse smaller sections of HTML
+template code. That's what this library is all about. ## Example This project
+comes with a sample flask application (see the `example` folder). This app
+displays videos that can be played on YouTube. The image, subtitle of author
+and view count are reused throughout the app. Here's a visual: ![](https://
+raw.githubusercontent.com/mikeckennedy/jinja_partials/main/readme_resources/
+reused-html-visual.png) Check out the [**demo / example application**](https://
+github.com/mikeckennedy/jinja_partials/tree/main/example) to see it in action.
+## Installation It's just `pip install jinja-partials` and you're all set with
+this pure Python package. ## Usage Using the library is incredible easy. The
+first step is to register the partial method with Jinja and Flask. Do this once
+at app startup: ```python import flask import jinja_partials app = flask.Flask
+(__name__) jinja_partials.register_extensions(app) # ... ``` You can also use
+this library in your FastAPI (or Starlette) project! ```python from
+fastapi.templating import Jinja2Templates # or `from starlette.templating
+import Jinja2Templates` import jinja_partials templates = Jinja2Templates
+("tests/test_templates") jinja_partials.register_starlette_extensions
+(templates) # ... ``` Or directly using a jijna environment! ```python import
+jinja_partials from jinja2 import Environment, FileSystemLoader environment =
+Environment(loader=FileSystemLoader("tests/test_templates"))
+jinja_partials.register_environment(environment) # ... ``` Next, you define
+your main HTML (Jinja2) templates as usual. Then define your partial templates.
+I recommend locating and naming them accordingly: ``` âââ templates
+âÂ Â  âââ home âÂ Â  âÂ Â  âââ index.html âÂ Â  âÂ Â 
+âââ listing.html âÂ Â  âââ shared âÂ Â  âââ _layout.html
+âÂ Â  âââ partials âÂ Â  âââ video_image.html âÂ Â  âââ
+video_square.html ``` Notice the `partials` subfolder in the `templates/shared`
+folder. The templates are just HTML fragments. Here is a stand-alone one for
+the YouTube thumbnail from the example app: ```html [{{ video.title }}]```
+Notice that an object called `video` and list of classes are passed in as the
+model. Templates can also be nested. Here is the whole single video fragment
+with the image as well as other info linking out to YouTube: ```html
 _{_{_ _r_e_n_d_e_r___p_a_r_t_i_a_l_(_'_s_h_a_r_e_d_/_p_a_r_t_i_a_l_s_/_v_i_d_e_o___i_m_a_g_e_._h_t_m_l_'_,_ _v_i_d_e_o_=_v_i_d_e_o_)_ _}_}_ _{
 _{_ _v_i_d_e_o_._a_u_t_h_o_r_ _}_}
 {{ "{:,}".format(video.views) }} views
 ``` Now you see the `render_partial()` method. It takes the subpath into the
 templates folder and any model data passed in as keyword arguments. We can
 finally generate the list of video blocks as follows: ```html {% for v in
 videos %}
```

### Comparing `jinja_partials-0.2.0/README.md` & `jinja_partials-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jinja_partials-0.2.0/jinja_partials/__init__.py` & `jinja_partials-0.2.1/jinja_partials/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 jinja_partials - Simple reuse of partial HTML page templates in the Jinja template language for Python web frameworks.
 """
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __author__ = 'Michael Kennedy <michael@talkpython.fm>'
 __all__ = [
     'register_extensions',
     'register_starlette_extensions',
     'register_environment',
     'render_partial',
     'generate_render_partial',
@@ -25,15 +25,15 @@
     flask = None
 
 try:
     import starlette
 except ImportError:
     starlette = None
 
-if TYPE_CHECKING:
+if TYPE_CHECKING and flask and starlette:
     from flask import Flask
     from starlette.templating import Jinja2Templates
 
 
 class PartialsException(Exception):
     pass
```

### Comparing `jinja_partials-0.2.0/setup.py` & `jinja_partials-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,57 +2,60 @@
 import os
 import re
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-def read(filename):
-    filename = os.path.join(os.path.dirname(__file__), filename)
-    text_type = type(u"")
-    with io.open(filename, mode="r", encoding='utf-8') as fd:
-        return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
-
-
-with open('./requirements.txt', 'r', encoding='utf-8') as fin:
-    requires_list = [line.strip() for line in fin if line and line.strip()]
+def read_readme(filename):
+    try:
+        filename = os.path.join(os.path.dirname(__file__), filename)
+        text_type = type(u"")
+        with io.open(filename, mode="r", encoding='utf-8') as fd:
+            return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
+    except:
+        return ''
 
 
 def read_version():
-    filename = os.path.join(os.path.dirname(__file__), 'jinja_partials', '__init__.py')
-    with open(filename, mode="r", encoding='utf-8') as fin2:
-        for line in fin2:
-            if line and line.strip() and line.startswith('__version__'):
-                return line.split('=')[1].strip().strip("'").strip('"')
-
-    return "0.0.0.0"
+    try:
+        filename = os.path.join(os.path.dirname(__file__), 'jinja_partials', '__init__.py')
+        with open(filename, mode="r", encoding='utf-8') as fin2:
+            for line in fin2:
+                if line and line.strip() and line.startswith('__version__'):
+                    return line.split('=')[1].strip().strip("'").strip('"')
+
+        return "0.0.0.0"
+    except:
+        return "0.0.0.0"
 
 
 setup(
     name="jinja_partials",
     version=read_version(),
     url="https://github.com/mikeckennedy/jinja_partials",
     license='MIT',
 
     author="Michael Kennedy",
     author_email="michael@talkpython.fm",
 
     description="Simple reuse of partial HTML page templates in the Jinja template language for Python web frameworks.",
-    long_description=read("README.md"),
+    long_description=read_readme("README.md"),
     long_description_content_type="text/markdown",
 
     packages=find_packages(exclude=('tests', 'example', 'readme_resources', 'build', 'dist',)),
 
-    install_requires=requires_list,
+    install_requires=['jinja2'],
+    exclude=['build', 'dist', '.github', 'example', 'tests'],
 
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

