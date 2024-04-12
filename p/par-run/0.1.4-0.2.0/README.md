# Comparing `tmp/par_run-0.1.4.tar.gz` & `tmp/par_run-0.2.0.tar.gz`

## Comparing `par_run-0.1.4.tar` & `par_run-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.1.4/.python-version
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.1.4/commands.ini
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 par_run-0.1.4/requirements-dev.lock
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 par_run-0.1.4/requirements.lock
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/coverage_html.js
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046___init___py.html
--rw-r--r--   0        0        0    78275 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046_cli_py.html
--rw-r--r--   0        0        0   106323 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046_executor_py.html
--rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046_web_cli_py.html
--rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046_web_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/favicon_32.png
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/keybd_open.png
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/status.json
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/style.css
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 par_run-0.1.4/.vscode/launch.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/conftest.py
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/test_cli.py
--rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/test_executor.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/test_main.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/test_web.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/__init__.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/cli.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/executor.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/web.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/static/css/style.css
--rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/static/js/app.js
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/templates/index.html
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.1.4/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.1.4/LICENSE
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 par_run-0.1.4/README.md
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 par_run-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 par_run-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.2.0/.python-version
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.2.0/commands.ini
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 par_run-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 par_run-0.2.0/requirements.lock
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/coverage_html.js
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046___init___py.html
+-rw-r--r--   0        0        0    83748 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046_cli_py.html
+-rw-r--r--   0        0        0   134028 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046_executor_py.html
+-rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046_web_cli_py.html
+-rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046_web_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/favicon_32.png
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/keybd_open.png
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/style.css
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 par_run-0.2.0/.vscode/launch.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/conftest.py
+-rw-r--r--   0        0        0    14105 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/test_cli.py
+-rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/test_executor.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/test_main.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/test_web.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/__init__.py
+-rw-r--r--   0        0        0     9370 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/cli.py
+-rw-r--r--   0        0        0    14943 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/executor.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/web.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/static/css/style.css
+-rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/static/js/app.js
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/templates/index.html
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 par_run-0.2.0/README.md
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 par_run-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 par_run-0.2.0/PKG-INFO
```

### Comparing `par_run-0.1.4/requirements-dev.lock` & `par_run-0.2.0/requirements-dev.lock`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 -e file:.
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via httpx
     # via starlette
     # via watchfiles
+asttokens==2.4.1
+    # via stack-data
 bump-my-version==0.20.0
 certifi==2024.2.2
     # via httpcore
     # via httpx
     # via requests
 cffi==1.16.0
     # via cryptography
@@ -28,19 +30,24 @@
     # via rich-click
     # via typer-slim
     # via uvicorn
 coverage==7.4.4
     # via pytest-cov
 cryptography==42.0.5
     # via secretstorage
+decorator==5.1.1
+    # via ipython
 docutils==0.20.1
     # via readme-renderer
 exceptiongroup==1.2.0
     # via anyio
+    # via ipython
     # via pytest
+executing==2.0.1
+    # via stack-data
 fastapi==0.110.0
     # via par-run
 h11==0.14.0
     # via httpcore
     # via uvicorn
 httpcore==1.0.5
     # via httpx
@@ -52,65 +59,80 @@
     # via httpx
     # via requests
 importlib-metadata==7.1.0
     # via keyring
     # via twine
 iniconfig==2.0.0
     # via pytest
+ipython==8.18.1
 jaraco-classes==3.4.0
     # via keyring
 jaraco-context==4.3.0
     # via keyring
 jaraco-functools==4.0.0
     # via keyring
+jedi==0.19.1
+    # via ipython
 jeepney==0.8.0
     # via keyring
     # via secretstorage
 jinja2==3.1.3
     # via par-run
 keyring==25.0.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
+matplotlib-inline==0.1.6
+    # via ipython
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
     # via jaraco-classes
     # via jaraco-functools
 mypy==1.9.0
 mypy-extensions==1.0.0
     # via mypy
 nh3==0.2.17
     # via readme-renderer
 packaging==24.0
     # via pytest
+parso==0.8.4
+    # via jedi
+pexpect==4.9.0
+    # via ipython
 pkginfo==1.10.0
     # via twine
 pluggy==1.4.0
     # via pytest
-prompt-toolkit==3.0.36
+prompt-toolkit==3.0.43
+    # via ipython
     # via questionary
 psutil==5.9.8
     # via par-run
+ptyprocess==0.7.0
+    # via pexpect
+pure-eval==0.2.2
+    # via stack-data
 py-cpuinfo==9.0.0
     # via pytest-benchmark
 pycparser==2.22
     # via cffi
 pydantic==2.6.4
     # via bump-my-version
     # via fastapi
     # via par-run
     # via pydantic-settings
 pydantic-core==2.16.3
     # via pydantic
 pydantic-settings==2.2.1
     # via bump-my-version
 pygments==2.17.2
+    # via ipython
     # via readme-renderer
     # via rich
 pytest==8.1.1
     # via pytest-asyncio
     # via pytest-benchmark
     # via pytest-cov
     # via pytest-mock
@@ -121,15 +143,15 @@
 pytest-mock==3.14.0
 pytest-random-order==1.1.1
 python-dotenv==1.0.1
     # via pydantic-settings
     # via uvicorn
 pyyaml==6.0.1
     # via uvicorn
-questionary==2.0.1
+questionary==1.10.0
     # via bump-my-version
 readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via requests-toolbelt
     # via twine
 requests-toolbelt==1.0.0
@@ -145,38 +167,47 @@
 rich-click==1.7.4
     # via bump-my-version
 ruff==0.3.4
 secretstorage==3.3.3
     # via keyring
 shellingham==1.5.4
     # via typer-slim
+six==1.16.0
+    # via asttokens
 sniffio==1.3.1
     # via anyio
     # via httpx
+stack-data==0.6.3
+    # via ipython
 starlette==0.36.3
     # via fastapi
 tomli==2.0.1
     # via coverage
     # via mypy
     # via pytest
 tomlkit==0.12.4
     # via bump-my-version
+    # via par-run
+traitlets==5.14.2
+    # via ipython
+    # via matplotlib-inline
 twine==5.0.0
 typer==0.12.0
     # via par-run
 typer-cli==0.12.0
     # via typer
 typer-slim==0.12.0
     # via typer
     # via typer-cli
 types-psutil==5.9.5.20240316
 types-toml==0.10.8.20240310
 typing-extensions==4.10.0
     # via anyio
     # via fastapi
+    # via ipython
     # via mypy
     # via pydantic
     # via pydantic-core
     # via rich-click
     # via starlette
     # via typer-slim
     # via uvicorn
```

### Comparing `par_run-0.1.4/requirements.lock` & `par_run-0.2.0/requirements.lock`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     # via typer-slim
 shellingham==1.5.4
     # via typer-slim
 sniffio==1.3.1
     # via anyio
 starlette==0.36.3
     # via fastapi
+tomlkit==0.12.4
+    # via par-run
 typer==0.12.0
     # via par-run
 typer-cli==0.12.0
     # via typer
 typer-slim==0.12.0
     # via typer
     # via typer-cli
```

### Comparing `par_run-0.1.4/.reports/html/coverage_html.js` & `par_run-0.2.0/.reports/html/coverage_html.js`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/.reports/html/d_417a353b6036f046___init___py.html` & `par_run-0.2.0/.reports/html/d_417a353b6036f046___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-01 07:45 -0400
+            created at 2024-04-10 15:41 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -78,23 +78,23 @@
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Main module for the py_runner package."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.1.2"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.1.4"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-01 07:45 -0400
+            created at 2024-04-10 15:41 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,13 +6,13 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 11 ssttaatteemmeennttss ?  11 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-01 07:45 -0400
+10 15:41 -0400
 _1"""Main module for the py_runner package.""" 
 _2 
-_3__version__ = "0.1.2" 
+_3__version__ = "0.1.4" 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-01 07:45 -0400
+10 15:41 -0400
```

### Comparing `par_run-0.1.4/.reports/html/d_417a353b6036f046_cli_py.html` & `par_run-0.2.0/.reports/html/d_417a353b6036f046_cli_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">162 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">147<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">15<span class="text"> missing</span></button>
+            <span class="text">172 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">156<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">16<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 17:05 -0400
+            created at 2024-04-12 08:38 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -86,15 +86,15 @@
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">enum</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">rich</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">executor</span> <span class="key">import</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">CommandStatus</span><span class="op">,</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">read_commands_ini</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">executor</span> <span class="key">import</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">CommandStatus</span><span class="op">,</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">read_commands_toml</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="nam">PID_FILE</span> <span class="op">=</span> <span class="str">".par-run.uvicorn.pid"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="nam">cli_app</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Typer</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="com"># Web only functions</span>&nbsp;</span><span class="r"></span></p>
@@ -246,117 +246,141 @@
     <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="str">"""Callback function for when a command receives output"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]{cmd.name}: Finished[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="key">elif</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="key">def</span> <span class="nam">run</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">    <span class="nam">style</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Processing strategy"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="str">"comp"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">    <span class="nam">show</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Show available groups and commands"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="nam">file</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"The commands.ini file to use"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">Path</span><span class="op">(</span><span class="str">"commands.ini"</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">    <span class="nam">groups</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="key">None</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Run a specific group of commands, comma spearated"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">    <span class="nam">cmds</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="key">None</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Run a specific commands, comma spearated"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">    <span class="str">"""Run commands in parallel"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">    <span class="com"># Overall exit code, need to track all command exit codes to update this</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="nam">exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="nam">master_groups</span> <span class="op">=</span> <span class="nam">read_commands_ini</span><span class="op">(</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="key">if</span> <span class="nam">show</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]{cmd.name}[/]: {cmd.cmd}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="key">if</span> <span class="nam">groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">g</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">g</span> <span class="key">in</span> <span class="nam">groups</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="key">if</span> <span class="nam">cmds</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">            <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">                <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">                    <span class="nam">cmd_name</span><span class="op">:</span> <span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">                    <span class="key">for</span> <span class="nam">cmd_name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">                    <span class="key">if</span> <span class="nam">cmd_name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">c</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">cmds</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">                <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]No groups or commands found.[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">        <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="key">def</span> <span class="nam">format_elapsed_time</span><span class="op">(</span><span class="nam">seconds</span><span class="op">:</span> <span class="nam">float</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t"><span class="str">    Converts a number of seconds into a human-readable time format of HH:MM:SS.xxx</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t"><span class="str">    seconds (float): The number of seconds elapsed.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t"><span class="str">    str: The formatted time string.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="nam">hours</span> <span class="op">=</span> <span class="nam">int</span><span class="op">(</span><span class="nam">seconds</span><span class="op">)</span> <span class="op">//</span> <span class="num">3600</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="nam">minutes</span> <span class="op">=</span> <span class="op">(</span><span class="nam">int</span><span class="op">(</span><span class="nam">seconds</span><span class="op">)</span> <span class="op">%</span> <span class="num">3600</span><span class="op">)</span> <span class="op">//</span> <span class="num">60</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="nam">seconds</span> <span class="op">=</span> <span class="nam">seconds</span> <span class="op">%</span> <span class="num">60</span>  <span class="com"># Keeping the fractional part of seconds</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">    <span class="com"># Return formatted string with seconds rounded to 2 d.p.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="key">return</span> <span class="str">f"{hours:02}:{minutes:02}:{seconds:06.2f}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t"><span class="key">def</span> <span class="nam">run</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="nam">style</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Processing strategy"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="str">"comp"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">    <span class="nam">show</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Show available groups and commands"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">    <span class="nam">file</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"The commands.ini file to use"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">Path</span><span class="op">(</span><span class="str">"pyproject.toml"</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="nam">groups</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="key">None</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Run a specific group of commands, comma spearated"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">    <span class="nam">cmds</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="key">None</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Run a specific commands, comma spearated"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">    <span class="str">"""Run commands in parallel"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">    <span class="com"># Overall exit code, need to track all command exit codes to update this</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">    <span class="nam">exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">    <span class="nam">master_groups</span> <span class="op">=</span> <span class="nam">read_commands_toml</span><span class="op">(</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="key">if</span> <span class="nam">show</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]{cmd.name}[/]: {cmd.cmd}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="key">if</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnComp</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">        <span class="key">elif</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnRecv</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">BadParameter</span><span class="op">(</span><span class="str">"Invalid processing strategy"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">    <span class="com"># Summarise the results</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">        <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">            <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]Command {cmd.name} succeeded ({cmd.num_non_empty_lines})[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[red bold]Command {cmd.name} failed ({cmd.num_non_empty_lines})[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">    <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">    <span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="key">import</span> <span class="nam">signal</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="key">import</span> <span class="nam">subprocess</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">    <span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">    <span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">    <span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">    <span class="key">import</span> <span class="nam">psutil</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]Web commands loaded[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">    <span class="nam">PID_FILE</span> <span class="op">=</span> <span class="str">".par-run.uvicorn.pid"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">    <span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">    <span class="key">def</span> <span class="nam">web</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">        <span class="nam">command</span><span class="op">:</span> <span class="nam">WebCommand</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"command to control/interract with the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="nam">port</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="num">8001</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Port to run the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="str">"""Run the web server"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="key">if</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">START</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STOP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">RESTART</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STATUS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="nam">get_web_server_status</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Not a valid command '{command}'"</span><span class="op">,</span> <span class="nam">err</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Abort</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="key">if</span> <span class="nam">groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">g</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">g</span> <span class="key">in</span> <span class="nam">groups</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">    <span class="key">if</span> <span class="nam">cmds</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">            <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">                <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">                    <span class="nam">cmd_name</span><span class="op">:</span> <span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">                    <span class="key">for</span> <span class="nam">cmd_name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">                    <span class="key">if</span> <span class="nam">cmd_name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">c</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">cmds</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">                <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]No groups or commands found.[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="key">if</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnComp</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="key">elif</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnRecv</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">BadParameter</span><span class="op">(</span><span class="str">"Invalid processing strategy"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">    <span class="com"># Summarise the results</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">        <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">            <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">                <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">                <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">elapsed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">                    <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">f", {format_elapsed_time(cmd.elapsed)}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]Command {cmd.name} succeeded ({cmd.num_non_empty_lines}{elap_str})[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[red bold]Command {cmd.name} failed ({cmd.num_non_empty_lines}{elap_str})[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">    <span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">    <span class="key">import</span> <span class="nam">signal</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">    <span class="key">import</span> <span class="nam">subprocess</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">    <span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">    <span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">    <span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">    <span class="key">import</span> <span class="nam">psutil</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]Web commands loaded[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="key">except</span> <span class="nam">ImportError</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">    <span class="key">pass</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="nam">PID_FILE</span> <span class="op">=</span> <span class="str">".par-run.uvicorn.pid"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">    <span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">    <span class="key">def</span> <span class="nam">web</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">        <span class="nam">command</span><span class="op">:</span> <span class="nam">WebCommand</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"command to control/interract with the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">        <span class="nam">port</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="num">8001</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Port to run the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">        <span class="str">"""Run the web server"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">        <span class="key">if</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">START</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STOP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">RESTART</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STATUS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">            <span class="nam">get_web_server_status</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Not a valid command '{command}'"</span><span class="op">,</span> <span class="nam">err</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Abort</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t"><span class="key">except</span> <span class="nam">ImportError</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">    <span class="key">pass</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">    <span class="nam">cli_app</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 17:05 -0400
+            created at 2024-04-12 08:38 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -4,29 +4,29 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 116622 ssttaatteemmeennttss ?  114477 rruunn 1155 mmiissssiinngg 22 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-31 17:05 -0400
+********** 117722 ssttaatteemmeennttss ?  115566 rruunn 1166 mmiissssiinngg 22 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+12 08:38 -0400
 _1"""CLI for running commands in parallel""" 
 _2 
 _3from collections import OrderedDict 
 _4from pathlib import Path 
 _5from typing import Optional 
 _6import enum 
 _7 
 _8import rich 
 _9import typer 
 _1_0 
 _1_1from .executor import Command, CommandStatus, ProcessingStrategy,
-read_commands_ini 
+read_commands_toml 
 _1_2 
 _1_3PID_FILE = ".par-run.uvicorn.pid" 
 _1_4 
 _1_5cli_app = typer.Typer() 
 _1_6 
 _1_7 
 _1_8# Web only functions 
@@ -183,113 +183,138 @@
 _1_6_4 """Callback function for when a command receives output""" 
 _1_6_5 if cmd.status == CommandStatus.SUCCESS: 
 _1_6_6 rich.print(f"[green bold]{cmd.name}: Finished[/]") 
 _1_6_7 elif cmd.status == CommandStatus.FAILURE: 
 _1_6_8 rich.print(f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]") 
 _1_6_9 
 _1_7_0 
-_1_7_1@cli_app.command() 
-_1_7_2def run( 
-_1_7_3 style: ProcessingStrategy = typer.Option(help="Processing strategy",
+_1_7_1def format_elapsed_time(seconds: float) -> str: 
+_1_7_2 """ 
+_1_7_3 Converts a number of seconds into a human-readable time format of HH:MM:
+SS.xxx 
+_1_7_4 
+_1_7_5 Args: 
+_1_7_6 seconds (float): The number of seconds elapsed. 
+_1_7_7 
+_1_7_8 Returns: 
+_1_7_9 str: The formatted time string. 
+_1_8_0 """ 
+_1_8_1 hours = int(seconds) // 3600 
+_1_8_2 minutes = (int(seconds) % 3600) // 60 
+_1_8_3 seconds = seconds % 60 # Keeping the fractional part of seconds 
+_1_8_4 
+_1_8_5 # Return formatted string with seconds rounded to 2 d.p. 
+_1_8_6 return f"{hours:02}:{minutes:02}:{seconds:06.2f}" 
+_1_8_7 
+_1_8_8 
+_1_8_9@cli_app.command() 
+_1_9_0def run( 
+_1_9_1 style: ProcessingStrategy = typer.Option(help="Processing strategy",
 default="comp"), 
-_1_7_4 show: bool = typer.Option(help="Show available groups and commands",
+_1_9_2 show: bool = typer.Option(help="Show available groups and commands",
 default=False), 
-_1_7_5 file: Path = typer.Option(help="The commands.ini file to use", default=Path
-("commands.ini")), 
-_1_7_6 groups: Optional[str] = typer.Option(None, help="Run a specific group of
+_1_9_3 file: Path = typer.Option(help="The commands.ini file to use", default=Path
+("pyproject.toml")), 
+_1_9_4 groups: Optional[str] = typer.Option(None, help="Run a specific group of
 commands, comma spearated"), 
-_1_7_7 cmds: Optional[str] = typer.Option(None, help="Run a specific commands,
+_1_9_5 cmds: Optional[str] = typer.Option(None, help="Run a specific commands,
 comma spearated"), 
-_1_7_8): 
-_1_7_9 """Run commands in parallel""" 
-_1_8_0 # Overall exit code, need to track all command exit codes to update this 
-_1_8_1 exit_code = 0 
-_1_8_2 
-_1_8_3 master_groups = read_commands_ini(file) 
-_1_8_4 if show: 
-_1_8_5 for grp in master_groups: 
-_1_8_6 rich.print(f"[blue bold]Group: {grp.name}[/]") 
-_1_8_7 for _, cmd in grp.cmds.items(): 
-_1_8_8 rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}") 
-_1_8_9 return 
-_1_9_0 
-_1_9_1 if groups: 
-_1_9_2 master_groups = [grp for grp in master_groups if grp.name in [g.strip() for
-g in groups.split(",")]] 
-_1_9_3 
-_1_9_4 if cmds: 
-_1_9_5 for grp in master_groups: 
-_1_9_6 grp.cmds = OrderedDict( 
-_1_9_7 { 
-_1_9_8 cmd_name: cmd 
-_1_9_9 for cmd_name, cmd in grp.cmds.items() 
-_2_0_0 if cmd_name in [c.strip() for c in cmds.split(",")] 
-_2_0_1 } 
-_2_0_2 ) 
-_2_0_3 master_groups = [grp for grp in master_groups if grp.cmds] 
-_2_0_4 
-_2_0_5 if not master_groups: 
-_2_0_6 rich.print("[blue]No groups or commands found.[/]") 
-_2_0_7 raise typer.Exit(0) 
+_1_9_6): 
+_1_9_7 """Run commands in parallel""" 
+_1_9_8 # Overall exit code, need to track all command exit codes to update this 
+_1_9_9 exit_code = 0 
+_2_0_0 
+_2_0_1 master_groups = read_commands_toml(file) 
+_2_0_2 if show: 
+_2_0_3 for grp in master_groups: 
+_2_0_4 rich.print(f"[blue bold]Group: {grp.name}[/]") 
+_2_0_5 for _, cmd in grp.cmds.items(): 
+_2_0_6 rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}") 
+_2_0_7 return 
 _2_0_8 
-_2_0_9 for grp in master_groups: 
-_2_1_0 if style == ProcessingStrategy.ON_COMP: 
-_2_1_1 exit_code = exit_code or grp.run(style, CLICommandCBOnComp()) 
-_2_1_2 elif style == ProcessingStrategy.ON_RECV: 
-_2_1_3 exit_code = exit_code or grp.run(style, CLICommandCBOnRecv()) 
-_2_1_4 else: 
-_2_1_5 raise typer.BadParameter("Invalid processing strategy") 
-_2_1_6 
-_2_1_7 # Summarise the results 
-_2_1_8 for grp in master_groups: 
-_2_1_9 rich.print(f"[blue bold]Group: {grp.name}[/]") 
-_2_2_0 for _, cmd in grp.cmds.items(): 
-_2_2_1 if cmd.status == CommandStatus.SUCCESS: 
-_2_2_2 rich.print(f"[green bold]Command {cmd.name} succeeded (
-{cmd.num_non_empty_lines})[/]") 
-_2_2_3 else: 
-_2_2_4 rich.print(f"[red bold]Command {cmd.name} failed (
-{cmd.num_non_empty_lines})[/]") 
-_2_2_5 
-_2_2_6 raise typer.Exit(exit_code) 
-_2_2_7 
-_2_2_8 
-_2_2_9try: 
-_2_3_0 import os 
-_2_3_1 import signal 
-_2_3_2 import subprocess 
-_2_3_3 import sys 
-_2_3_4 import time 
-_2_3_5 from pathlib import Path 
-_2_3_6 from typing import Optional 
-_2_3_7 
-_2_3_8 import psutil 
-_2_3_9 import typer 
-_2_4_0 
-_2_4_1 rich.print("[blue]Web commands loaded[/]") 
-_2_4_2 
-_2_4_3 PID_FILE = ".par-run.uvicorn.pid" 
-_2_4_4 
-_2_4_5 @cli_app.command() 
-_2_4_6 def web( 
-_2_4_7 command: WebCommand = typer.Argument(..., help="command to control/
-interract with the web server"), 
-_2_4_8 port: int = typer.Option(8001, help="Port to run the web server"), 
-_2_4_9 ): 
-_2_5_0 """Run the web server""" 
-_2_5_1 if command == WebCommand.START: 
-_2_5_2 start_web_server(port) 
-_2_5_3 elif command == WebCommand.STOP: 
-_2_5_4 stop_web_server() 
-_2_5_5 elif command == WebCommand.RESTART: 
-_2_5_6 stop_web_server() 
-_2_5_7 start_web_server(port) 
-_2_5_8 elif command == WebCommand.STATUS: 
-_2_5_9 get_web_server_status() 
-_2_6_0 else: 
-_2_6_1 typer.echo(f"Not a valid command '{command}'", err=True) 
-_2_6_2 raise typer.Abort() 
+_2_0_9 if groups: 
+_2_1_0 master_groups = [grp for grp in master_groups if grp.name in [g.strip() for
+g in groups.split(",")]] 
+_2_1_1 
+_2_1_2 if cmds: 
+_2_1_3 for grp in master_groups: 
+_2_1_4 grp.cmds = OrderedDict( 
+_2_1_5 { 
+_2_1_6 cmd_name: cmd 
+_2_1_7 for cmd_name, cmd in grp.cmds.items() 
+_2_1_8 if cmd_name in [c.strip() for c in cmds.split(",")] 
+_2_1_9 } 
+_2_2_0 ) 
+_2_2_1 master_groups = [grp for grp in master_groups if grp.cmds] 
+_2_2_2 
+_2_2_3 if not master_groups: 
+_2_2_4 rich.print("[blue]No groups or commands found.[/]") 
+_2_2_5 raise typer.Exit(0) 
+_2_2_6 
+_2_2_7 for grp in master_groups: 
+_2_2_8 if style == ProcessingStrategy.ON_COMP: 
+_2_2_9 exit_code = exit_code or grp.run(style, CLICommandCBOnComp()) 
+_2_3_0 elif style == ProcessingStrategy.ON_RECV: 
+_2_3_1 exit_code = exit_code or grp.run(style, CLICommandCBOnRecv()) 
+_2_3_2 else: 
+_2_3_3 raise typer.BadParameter("Invalid processing strategy") 
+_2_3_4 
+_2_3_5 # Summarise the results 
+_2_3_6 for grp in master_groups: 
+_2_3_7 rich.print(f"[blue bold]Group: {grp.name}[/]") 
+_2_3_8 for _, cmd in grp.cmds.items(): 
+_2_3_9 if cmd.status == CommandStatus.SUCCESS: 
+_2_4_0 elap_str = "" 
+_2_4_1 if cmd.elapsed: 
+_2_4_2 elap_str = f", {format_elapsed_time(cmd.elapsed)}" 
+_2_4_3 rich.print(f"[green bold]Command {cmd.name} succeeded (
+{cmd.num_non_empty_lines}{elap_str})[/]") 
+_2_4_4 else: 
+_2_4_5 rich.print(f"[red bold]Command {cmd.name} failed ({cmd.num_non_empty_lines}
+{elap_str})[/]") 
+_2_4_6 
+_2_4_7 raise typer.Exit(exit_code) 
+_2_4_8 
+_2_4_9 
+_2_5_0try: 
+_2_5_1 import os 
+_2_5_2 import signal 
+_2_5_3 import subprocess 
+_2_5_4 import sys 
+_2_5_5 import time 
+_2_5_6 from pathlib import Path 
+_2_5_7 from typing import Optional 
+_2_5_8 
+_2_5_9 import psutil 
+_2_6_0 import typer 
+_2_6_1 
+_2_6_2 rich.print("[blue]Web commands loaded[/]") 
 _2_6_3 
-_2_6_4except ImportError: # pragma: no cover 
-_2_6_5 pass # pragma: no cover 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-31 17:05 -0400
+_2_6_4 PID_FILE = ".par-run.uvicorn.pid" 
+_2_6_5 
+_2_6_6 @cli_app.command() 
+_2_6_7 def web( 
+_2_6_8 command: WebCommand = typer.Argument(..., help="command to control/
+interract with the web server"), 
+_2_6_9 port: int = typer.Option(8001, help="Port to run the web server"), 
+_2_7_0 ): 
+_2_7_1 """Run the web server""" 
+_2_7_2 if command == WebCommand.START: 
+_2_7_3 start_web_server(port) 
+_2_7_4 elif command == WebCommand.STOP: 
+_2_7_5 stop_web_server() 
+_2_7_6 elif command == WebCommand.RESTART: 
+_2_7_7 stop_web_server() 
+_2_7_8 start_web_server(port) 
+_2_7_9 elif command == WebCommand.STATUS: 
+_2_8_0 get_web_server_status() 
+_2_8_1 else: 
+_2_8_2 typer.echo(f"Not a valid command '{command}'", err=True) 
+_2_8_3 raise typer.Abort() 
+_2_8_4 
+_2_8_5except ImportError: # pragma: no cover 
+_2_8_6 pass # pragma: no cover 
+_2_8_7 
+_2_8_8if __name__ == "__main__": 
+_2_8_9 cli_app() 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+12 08:38 -0400
```

### Comparing `par_run-0.1.4/.reports/html/d_417a353b6036f046_executor_py.html` & `par_run-0.2.0/.reports/html/d_417a353b6036f046_executor_py.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/par_run/executor.py: 98%</title>
+    <title>Coverage for src/par_run/executor.py: 85%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/par_run/executor.py</b>:
-            <span class="pc_cov">98%</span>
+            <span class="pc_cov">85%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">203 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">198<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">5<span class="text"> missing</span></button>
+            <span class="text">251 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">213<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">38<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">7<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_web_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 17:02 -0400
+            created at 2024-04-12 08:32 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -82,362 +82,441 @@
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Todo"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">asyncio</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">configparser</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">enum</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">multiprocessing</span> <span class="key">as</span> <span class="nam">mp</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">queue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">subprocess</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">OrderedDict</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">concurrent</span><span class="op">.</span><span class="nam">futures</span> <span class="key">import</span> <span class="nam">Future</span><span class="op">,</span> <span class="nam">ProcessPoolExecutor</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">queue</span> <span class="key">import</span> <span class="nam">Queue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">List</span><span class="op">,</span> <span class="nam">Optional</span><span class="op">,</span> <span class="nam">Protocol</span><span class="op">,</span> <span class="nam">TypeVar</span><span class="op">,</span> <span class="nam">Union</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">pydantic</span> <span class="key">import</span> <span class="nam">BaseModel</span><span class="op">,</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">ConfigDict</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="com"># Type alias for a generic future.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="nam">GenFuture</span> <span class="op">=</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">Future</span><span class="op">,</span> <span class="nam">asyncio</span><span class="op">.</span><span class="nam">Future</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="nam">ContextT</span> <span class="op">=</span> <span class="nam">TypeVar</span><span class="op">(</span><span class="str">"ContextT"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">queue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">subprocess</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">OrderedDict</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">concurrent</span><span class="op">.</span><span class="nam">futures</span> <span class="key">import</span> <span class="nam">Future</span><span class="op">,</span> <span class="nam">ProcessPoolExecutor</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">queue</span> <span class="key">import</span> <span class="nam">Queue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">List</span><span class="op">,</span> <span class="nam">Optional</span><span class="op">,</span> <span class="nam">Protocol</span><span class="op">,</span> <span class="nam">TypeVar</span><span class="op">,</span> <span class="nam">Union</span><span class="op">,</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="nam">pydantic</span> <span class="key">import</span> <span class="nam">BaseModel</span><span class="op">,</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">ConfigDict</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="com"># Type alias for a generic future.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="nam">GenFuture</span> <span class="op">=</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">Future</span><span class="op">,</span> <span class="nam">asyncio</span><span class="op">.</span><span class="nam">Future</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="key">class</span> <span class="nam">ProcessingStrategy</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"""Enum for processing strategies."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">ON_COMP</span> <span class="op">=</span> <span class="str">"comp"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">ON_RECV</span> <span class="op">=</span> <span class="str">"recv"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandStatus</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"""Enum for command status."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">NOT_STARTED</span> <span class="op">=</span> <span class="str">"Not Started"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">RUNNING</span> <span class="op">=</span> <span class="str">"Running"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">SUCCESS</span> <span class="op">=</span> <span class="str">"Success"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">FAILURE</span> <span class="op">=</span> <span class="str">"Failure"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">def</span> <span class="nam">completed</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="str">"""Return True if the command has completed."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span> <span class="key">in</span> <span class="op">[</span><span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">,</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="key">class</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="str">"""Holder for a command and its name."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="nam">model_config</span> <span class="op">=</span> <span class="nam">ConfigDict</span><span class="op">(</span><span class="nam">arbitrary_types_allowed</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">ContextT</span> <span class="op">=</span> <span class="nam">TypeVar</span><span class="op">(</span><span class="str">"ContextT"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">class</span> <span class="nam">ProcessingStrategy</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"""Enum for processing strategies."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">ON_COMP</span> <span class="op">=</span> <span class="str">"comp"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="nam">ON_RECV</span> <span class="op">=</span> <span class="str">"recv"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandStatus</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"""Enum for command status."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">NOT_STARTED</span> <span class="op">=</span> <span class="str">"Not Started"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">RUNNING</span> <span class="op">=</span> <span class="str">"Running"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="nam">SUCCESS</span> <span class="op">=</span> <span class="str">"Success"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="nam">FAILURE</span> <span class="op">=</span> <span class="str">"Failure"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="key">def</span> <span class="nam">completed</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="str">"""Return True if the command has completed."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span> <span class="key">in</span> <span class="op">[</span><span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">,</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="key">class</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="str">"""Holder for a command and its name."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="nam">cmd</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">status</span><span class="op">:</span> <span class="nam">CommandStatus</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">NOT_STARTED</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="nam">unflushed</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="op">[</span><span class="op">]</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">num_non_empty_lines</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">0</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">ret_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="nam">fut</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">GenFuture</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="key">def</span> <span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">line</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="str">"""Increment the non-empty line count."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">if</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">num_non_empty_lines</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="key">def</span> <span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">line</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="str">"""Append a line to the output and increment the non-empty line count."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="key">def</span> <span class="nam">clear_unflushed</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="str">"""Clear the unflushed output."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="key">def</span> <span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">ret_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="str">"""Set the return code and status of the command."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">ret_code</span> <span class="op">=</span> <span class="nam">ret_code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span><span class="op">.</span><span class="nam">cancel</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="key">if</span> <span class="nam">ret_code</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="key">def</span> <span class="nam">set_running</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="str">"""Set the command status to running."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">RUNNING</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandCB</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandAsyncCB</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="key">class</span> <span class="nam">QRetriever</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">retries</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">q</span> <span class="op">=</span> <span class="nam">q</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span> <span class="op">=</span> <span class="nam">timeout</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span> <span class="op">=</span> <span class="nam">retries</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="key">def</span> <span class="nam">get</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="nam">retry_count</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">            <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">                <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">q</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">block</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">            <span class="key">except</span> <span class="nam">queue</span><span class="op">.</span><span class="nam">Empty</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                <span class="key">if</span> <span class="nam">retry_count</span> <span class="op">&lt;</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                    <span class="nam">retry_count</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">TimeoutError</span><span class="op">(</span><span class="str">"Timeout waiting for command output"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandGroup</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="str">"""Holder for a group of commands."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">    <span class="nam">cmds</span><span class="op">:</span> <span class="nam">OrderedDict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Command</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default_factory</span><span class="op">=</span><span class="nam">OrderedDict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">run_async</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandAsyncCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">q</span> <span class="op">=</span> <span class="nam">mp</span><span class="op">.</span><span class="nam">Manager</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">Queue</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">pool</span> <span class="op">=</span> <span class="nam">ProcessPoolExecutor</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="nam">futs</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">            <span class="nam">asyncio</span><span class="op">.</span><span class="nam">get_event_loop</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">run_in_executor</span><span class="op">(</span><span class="nam">pool</span><span class="op">,</span> <span class="nam">run_command</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">q</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="key">for</span> <span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">)</span><span class="op">,</span> <span class="nam">fut</span> <span class="key">in</span> <span class="nam">zip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">futs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="nam">fut</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_running</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_process_q_async</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">    <span class="key">def</span> <span class="nam">run</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="nam">q</span> <span class="op">=</span> <span class="nam">mp</span><span class="op">.</span><span class="nam">Manager</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">Queue</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="nam">pool</span> <span class="op">=</span> <span class="nam">ProcessPoolExecutor</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="nam">futs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">pool</span><span class="op">.</span><span class="nam">submit</span><span class="op">(</span><span class="nam">run_command</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">q</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="key">for</span> <span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">)</span><span class="op">,</span> <span class="nam">fut</span> <span class="key">in</span> <span class="nam">zip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">futs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="nam">fut</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_running</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_process_q</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">    <span class="key">def</span> <span class="nam">_process_q</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">                <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="nam">timeout</span> <span class="op">=</span> <span class="num">10</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="nam">retries</span> <span class="op">=</span> <span class="num">3</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="nam">q_ret</span> <span class="op">=</span> <span class="nam">QRetriever</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">,</span> <span class="nam">retries</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">            <span class="nam">q_result</span> <span class="op">=</span> <span class="nam">q_ret</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="nam">model_config</span> <span class="op">=</span> <span class="nam">ConfigDict</span><span class="op">(</span><span class="nam">arbitrary_types_allowed</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="nam">cmd</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">passenv</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">setenv</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="nam">status</span><span class="op">:</span> <span class="nam">CommandStatus</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">NOT_STARTED</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="nam">unflushed</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="op">[</span><span class="op">]</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="nam">num_non_empty_lines</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">0</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="nam">ret_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="nam">fut</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">GenFuture</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="nam">start_time</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">float</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">elapsed</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">float</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">exclude</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">def</span> <span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">line</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="str">"""Increment the non-empty line count."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="key">if</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">num_non_empty_lines</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="key">def</span> <span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">line</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="str">"""Append a line to the output and increment the non-empty line count."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">def</span> <span class="nam">clear_unflushed</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="str">"""Clear the unflushed output."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="key">def</span> <span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">ret_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="str">"""Set the return code and status of the command."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">start_time</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">elapsed</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">perf_counter</span><span class="op">(</span><span class="op">)</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">start_time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">ret_code</span> <span class="op">=</span> <span class="nam">ret_code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span><span class="op">.</span><span class="nam">cancel</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="key">if</span> <span class="nam">ret_code</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">FAILURE</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="key">def</span> <span class="nam">set_running</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="str">"""Set the command status to running."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">start_time</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">perf_counter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">status</span> <span class="op">=</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">RUNNING</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandCB</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandAsyncCB</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_start</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_recv</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">output</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">on_term</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">:</span> <span class="nam">Command</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span> <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="key">class</span> <span class="nam">QRetriever</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">retries</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">q</span> <span class="op">=</span> <span class="nam">q</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span> <span class="op">=</span> <span class="nam">timeout</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span> <span class="op">=</span> <span class="nam">retries</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="key">def</span> <span class="nam">get</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">        <span class="nam">retry_count</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">            <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">                <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">q</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">block</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">            <span class="key">except</span> <span class="nam">queue</span><span class="op">.</span><span class="nam">Empty</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">                <span class="key">if</span> <span class="nam">retry_count</span> <span class="op">&lt;</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                    <span class="nam">retry_count</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                    <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">TimeoutError</span><span class="op">(</span><span class="str">"Timeout waiting for command output"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="key">return</span> <span class="str">f"QRetriever(timeout={self.timeout}, retries={self.retries})"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="key">class</span> <span class="nam">CommandGroup</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="str">"""Holder for a group of commands."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="nam">desc</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="nam">cmds</span><span class="op">:</span> <span class="nam">OrderedDict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Command</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default_factory</span><span class="op">=</span><span class="nam">OrderedDict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="nam">timeout</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">30</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">    <span class="nam">retries</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">default</span><span class="op">=</span><span class="num">3</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">run_async</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandAsyncCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="nam">q</span> <span class="op">=</span> <span class="nam">mp</span><span class="op">.</span><span class="nam">Manager</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">Queue</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="nam">pool</span> <span class="op">=</span> <span class="nam">ProcessPoolExecutor</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="nam">futs</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="nam">asyncio</span><span class="op">.</span><span class="nam">get_event_loop</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">run_in_executor</span><span class="op">(</span><span class="nam">pool</span><span class="op">,</span> <span class="nam">run_command</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">setenv</span><span class="op">,</span> <span class="nam">q</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="key">for</span> <span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">)</span><span class="op">,</span> <span class="nam">fut</span> <span class="key">in</span> <span class="nam">zip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">futs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="nam">fut</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_running</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_process_q_async</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">    <span class="key">def</span> <span class="nam">run</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandCB</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="nam">q</span> <span class="op">=</span> <span class="nam">mp</span><span class="op">.</span><span class="nam">Manager</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">Queue</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="nam">pool</span> <span class="op">=</span> <span class="nam">ProcessPoolExecutor</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">futs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">pool</span><span class="op">.</span><span class="nam">submit</span><span class="op">(</span><span class="nam">run_command</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">setenv</span><span class="op">,</span> <span class="nam">q</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="key">for</span> <span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">)</span><span class="op">,</span> <span class="nam">fut</span> <span class="key">in</span> <span class="nam">zip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">futs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">fut</span> <span class="op">=</span> <span class="nam">fut</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_running</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_process_q</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">strategy</span><span class="op">,</span> <span class="nam">callbacks</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">    <span class="key">def</span> <span class="nam">_process_q</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">            <span class="com"># Can only get here with a valid message from the Q</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="nam">cmd_name</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">            <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">            <span class="nam">output_line</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">            <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">            <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">[</span><span class="nam">cmd_name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">                    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">                        <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">clear_unflushed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="key">if</span> <span class="nam">all</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span><span class="op">.</span><span class="nam">completed</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="key">return</span> <span class="nam">grp_exit_code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">_process_q_async</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">        <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandAsyncCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">        <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">                <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">        <span class="nam">q_ret</span> <span class="op">=</span> <span class="nam">QRetriever</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">            <span class="nam">q_result</span> <span class="op">=</span> <span class="nam">q_ret</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">            <span class="com"># Can only get here with a valid message from the Q</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">            <span class="nam">cmd_name</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">            <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">            <span class="nam">output_line</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">            <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">            <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">[</span><span class="nam">cmd_name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                        <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">clear_unflushed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">                    <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">            <span class="key">if</span> <span class="nam">all</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span><span class="op">.</span><span class="nam">completed</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="key">return</span> <span class="nam">grp_exit_code</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">        <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">                <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="nam">timeout</span> <span class="op">=</span> <span class="num">10</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="nam">retries</span> <span class="op">=</span> <span class="num">3</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">        <span class="nam">q_ret</span> <span class="op">=</span> <span class="nam">QRetriever</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">,</span> <span class="nam">retries</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">            <span class="key">await</span> <span class="nam">asyncio</span><span class="op">.</span><span class="nam">sleep</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">            <span class="nam">q_result</span> <span class="op">=</span> <span class="nam">q_ret</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">            <span class="com"># Can only get here with a valid message from the Q</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">            <span class="nam">cmd_name</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">            <span class="com"># print(q_result, type(q_result[0]), type(q_result[1]))</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">            <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">            <span class="nam">output_line</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">            <span class="com"># print(output_line, exit_code)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">            <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">            <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">[</span><span class="nam">cmd_name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">                    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">                        <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">clear_unflushed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">            <span class="key">if</span> <span class="nam">all</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span><span class="op">.</span><span class="nam">completed</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">        <span class="key">return</span> <span class="nam">grp_exit_code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">_process_q_async</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="nam">strategy</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="nam">callbacks</span><span class="op">:</span> <span class="nam">CommandAsyncCB</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">                <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="nam">q_ret</span> <span class="op">=</span> <span class="nam">QRetriever</span><span class="op">(</span><span class="nam">q</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">timeout</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">retries</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">        <span class="key">while</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">            <span class="key">await</span> <span class="nam">asyncio</span><span class="op">.</span><span class="nam">sleep</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">            <span class="nam">q_result</span> <span class="op">=</span> <span class="nam">q_ret</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">            <span class="com"># Can only get here with a valid message from the Q</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">            <span class="nam">cmd_name</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">            <span class="nam">exit_code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">            <span class="nam">output_line</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">q_result</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">            <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">[</span><span class="nam">cmd_name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">            <span class="key">if</span> <span class="nam">strategy</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">                <span class="key">if</span> <span class="nam">output_line</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">incr_line_count</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">append_unflushed</span><span class="op">(</span><span class="nam">output_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                <span class="key">elif</span> <span class="nam">exit_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_start</span><span class="op">(</span><span class="nam">cmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                    <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">unflushed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                        <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_recv</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">clear_unflushed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">                    <span class="key">await</span> <span class="nam">callbacks</span><span class="op">.</span><span class="nam">on_term</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">                    <span class="nam">cmd</span><span class="op">.</span><span class="nam">set_ret_code</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">                    <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">                        <span class="nam">grp_exit_code</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">                    <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Invalid Q message"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t"><span class="key">def</span> <span class="nam">read_commands_ini</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">    <span class="str">"""Read a commands.ini file and return a list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">            <span class="key">if</span> <span class="nam">all</span><span class="op">(</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span><span class="op">.</span><span class="nam">completed</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">        <span class="key">return</span> <span class="nam">grp_exit_code</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t"><span class="str">        list[CommandGroup]: A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">configparser</span><span class="op">.</span><span class="nam">ConfigParser</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="nam">filename</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">    <span class="nam">command_groups</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="key">for</span> <span class="nam">section</span> <span class="key">in</span> <span class="nam">config</span><span class="op">.</span><span class="nam">sections</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">        <span class="key">if</span> <span class="nam">section</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"group."</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">            <span class="nam">group_name</span> <span class="op">=</span> <span class="nam">section</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"group."</span><span class="op">,</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">            <span class="nam">commands</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">            <span class="key">for</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">config</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="nam">section</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">                <span class="nam">name</span> <span class="op">=</span> <span class="nam">name</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">                <span class="nam">commands</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">=</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">            <span class="nam">command_group</span> <span class="op">=</span> <span class="nam">CommandGroup</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">group_name</span><span class="op">,</span> <span class="nam">cmds</span><span class="op">=</span><span class="nam">commands</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="nam">command_groups</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">command_group</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">    <span class="key">return</span> <span class="nam">command_groups</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t"><span class="key">def</span> <span class="nam">write_commands_ini</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">,</span> <span class="nam">command_groups</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="str">"""Write a list of CommandGroup objects to a commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t"><span class="key">def</span> <span class="nam">read_commands_ini</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="str">"""Read a commands.ini file and return a list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t"><span class="str">        list[CommandGroup]: A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">configparser</span><span class="op">.</span><span class="nam">ConfigParser</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="nam">filename</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">    <span class="nam">command_groups</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">    <span class="key">for</span> <span class="nam">section</span> <span class="key">in</span> <span class="nam">config</span><span class="op">.</span><span class="nam">sections</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">        <span class="key">if</span> <span class="nam">section</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"group."</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">            <span class="nam">group_name</span> <span class="op">=</span> <span class="nam">section</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"group."</span><span class="op">,</span> <span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">            <span class="nam">commands</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="key">for</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">config</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="nam">section</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">                <span class="nam">name</span> <span class="op">=</span> <span class="nam">name</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">                <span class="nam">commands</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">=</span><span class="nam">cmd</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">            <span class="nam">command_group</span> <span class="op">=</span> <span class="nam">CommandGroup</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">group_name</span><span class="op">,</span> <span class="nam">cmds</span><span class="op">=</span><span class="nam">commands</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">            <span class="nam">command_groups</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">command_group</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="key">return</span> <span class="nam">command_groups</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t"><span class="str">        command_groups (list[CommandGroup]): A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">configparser</span><span class="op">.</span><span class="nam">ConfigParser</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">    <span class="key">for</span> <span class="nam">group</span> <span class="key">in</span> <span class="nam">command_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">        <span class="nam">section_name</span> <span class="op">=</span> <span class="str">f"group.{group.name}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">        <span class="nam">config</span><span class="op">[</span><span class="nam">section_name</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">        <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">command</span> <span class="key">in</span> <span class="nam">group</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">            <span class="nam">config</span><span class="op">[</span><span class="nam">section_name</span><span class="op">]</span><span class="op">[</span><span class="nam">command</span><span class="op">.</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">command</span><span class="op">.</span><span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">filename</span><span class="op">,</span> <span class="str">"w"</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">configfile</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">        <span class="nam">config</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">configfile</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t"><span class="key">def</span> <span class="nam">write_commands_ini</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">,</span> <span class="nam">command_groups</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">    <span class="str">"""Write a list of CommandGroup objects to a commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.ini file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t"><span class="str">        command_groups (list[CommandGroup]): A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">configparser</span><span class="op">.</span><span class="nam">ConfigParser</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="key">for</span> <span class="nam">group</span> <span class="key">in</span> <span class="nam">command_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">        <span class="nam">section_name</span> <span class="op">=</span> <span class="str">f"group.{group.name}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="nam">config</span><span class="op">[</span><span class="nam">section_name</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">        <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">command</span> <span class="key">in</span> <span class="nam">group</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">            <span class="nam">config</span><span class="op">[</span><span class="nam">section_name</span><span class="op">]</span><span class="op">[</span><span class="nam">command</span><span class="op">.</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">command</span><span class="op">.</span><span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t"><span class="key">def</span> <span class="nam">run_command</span><span class="op">(</span><span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">command</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">    <span class="str">"""Run a command and put the output into a queue. The output is a tuple of the command</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="str">    name and the output line. The final output is a tuple of the command name and a dictionary</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t"><span class="str">    with the return code.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t"><span class="str">        name (str): Name of the command.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">        command (str): Command to run.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t"><span class="str">        q (Queue): Queue to put the output into.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="key">with</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">Popen</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">        <span class="str">f"{command}"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">        <span class="nam">shell</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">        <span class="nam">stdout</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">PIPE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">        <span class="nam">stderr</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">STDOUT</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">        <span class="nam">text</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="op">)</span> <span class="key">as</span> <span class="nam">process</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">        <span class="key">if</span> <span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">            <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">iter</span><span class="op">(</span><span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">readline</span><span class="op">,</span> <span class="str">""</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">                <span class="nam">q</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">            <span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">close</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">            <span class="nam">process</span><span class="op">.</span><span class="nam">wait</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">            <span class="nam">ret_code</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">returncode</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">            <span class="key">if</span> <span class="nam">ret_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">                <span class="nam">q</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">int</span><span class="op">(</span><span class="nam">ret_code</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Process has no return code"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">filename</span><span class="op">,</span> <span class="str">"w"</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">configfile</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">        <span class="nam">config</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">configfile</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t"><span class="key">def</span> <span class="nam">_validate_mandatory_keys</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">items</span><span class="op">.</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">keys</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">context</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">,</span> <span class="op">...</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">    <span class="str">"""Validate that the mandatory keys are present in the data.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t"><span class="str">        data (tomlkit.items.Table): The data to validate.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">        keys (list[str]): The mandatory keys.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="nam">vals</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span> <span class="key">in</span> <span class="nam">keys</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">        <span class="nam">val</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">val</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"{key} is mandatory, not found in {context}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">        <span class="nam">vals</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">val</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="key">return</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">vals</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t"><span class="key">def</span> <span class="nam">_get_optional_keys</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">items</span><span class="op">.</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">keys</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="op">...</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">    <span class="str">"""Get Optional keys or default.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">        data (tomlkit.items.Table): The data to use as source</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t"><span class="str">        keys (list[str]): The optional keys.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="key">return</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">default</span><span class="op">)</span> <span class="key">for</span> <span class="nam">key</span> <span class="key">in</span> <span class="nam">keys</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t"><span class="key">def</span> <span class="nam">read_commands_toml</span><span class="op">(</span><span class="nam">filename</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Path</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">CommandGroup</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">    <span class="str">"""Read a commands.toml file and return a list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">        filename (Union[str, Path]): The filename of the commands.toml file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="str">        list[CommandGroup]: A list of CommandGroup objects.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">filename</span><span class="op">,</span> <span class="str">"r"</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">toml_file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">        <span class="nam">toml_data</span> <span class="op">=</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">toml_file</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="nam">cmd_groups_data</span> <span class="op">=</span> <span class="nam">toml_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"tool"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"par-run"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">cmd_groups_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"No par-run data found in toml file"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">    <span class="nam">_</span> <span class="op">=</span> <span class="nam">cmd_groups_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"description"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">    <span class="nam">command_groups</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">for</span> <span class="nam">group_data</span> <span class="key">in</span> <span class="nam">cmd_groups_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"groups"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">        <span class="op">(</span><span class="nam">group_name</span><span class="op">,</span><span class="op">)</span> <span class="op">=</span> <span class="nam">_validate_mandatory_keys</span><span class="op">(</span><span class="nam">group_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"name"</span><span class="op">]</span><span class="op">,</span> <span class="str">"top level par-run group"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">        <span class="nam">group_desc</span><span class="op">,</span> <span class="nam">group_timeout</span><span class="op">,</span> <span class="nam">group_retries</span> <span class="op">=</span> <span class="nam">_get_optional_keys</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">            <span class="nam">group_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"desc"</span><span class="op">,</span> <span class="str">"timeout"</span><span class="op">,</span> <span class="str">"retries"</span><span class="op">]</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">group_timeout</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">            <span class="nam">group_timeout</span> <span class="op">=</span> <span class="num">30</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">group_retries</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">            <span class="nam">group_retries</span> <span class="op">=</span> <span class="num">3</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">        <span class="nam">commands</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">        <span class="key">for</span> <span class="nam">cmd_data</span> <span class="key">in</span> <span class="nam">group_data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"commands"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">            <span class="nam">name</span><span class="op">,</span> <span class="nam">exec</span> <span class="op">=</span> <span class="nam">_validate_mandatory_keys</span><span class="op">(</span><span class="nam">cmd_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"name"</span><span class="op">,</span> <span class="str">"exec"</span><span class="op">]</span><span class="op">,</span> <span class="str">f"command group {group_name}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">            <span class="nam">setenv</span><span class="op">,</span> <span class="nam">passenv</span> <span class="op">=</span> <span class="nam">_get_optional_keys</span><span class="op">(</span><span class="nam">cmd_data</span><span class="op">,</span> <span class="op">[</span><span class="str">"setenv"</span><span class="op">,</span> <span class="str">"passenv"</span><span class="op">]</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">            <span class="nam">commands</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">cmd</span><span class="op">=</span><span class="nam">exec</span><span class="op">,</span> <span class="nam">setenv</span><span class="op">=</span><span class="nam">setenv</span><span class="op">,</span> <span class="nam">passenv</span><span class="op">=</span><span class="nam">passenv</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">        <span class="nam">command_group</span> <span class="op">=</span> <span class="nam">CommandGroup</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">            <span class="nam">name</span><span class="op">=</span><span class="nam">group_name</span><span class="op">,</span> <span class="nam">desc</span><span class="op">=</span><span class="nam">group_desc</span><span class="op">,</span> <span class="nam">cmds</span><span class="op">=</span><span class="nam">commands</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">=</span><span class="nam">group_timeout</span><span class="op">,</span> <span class="nam">retries</span><span class="op">=</span><span class="nam">group_retries</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">        <span class="nam">command_groups</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">command_group</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="key">return</span> <span class="nam">command_groups</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t"><span class="key">def</span> <span class="nam">run_command</span><span class="op">(</span><span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">command</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">setenv</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">]</span><span class="op">,</span> <span class="nam">q</span><span class="op">:</span> <span class="nam">Queue</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">    <span class="str">"""Run a command and put the output into a queue. The output is a tuple of the command</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t"><span class="str">    name and the output line. The final output is a tuple of the command name and a dictionary</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t"><span class="str">    with the return code.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t"><span class="str">        name (Command): Command to run.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t"><span class="str">        q (Queue): Queue to put the output into.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="nam">new_env</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">    <span class="key">if</span> <span class="nam">setenv</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">        <span class="nam">new_env</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">environ</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">        <span class="nam">new_env</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">setenv</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="key">with</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">Popen</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">        <span class="nam">command</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">        <span class="nam">shell</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">        <span class="nam">env</span><span class="op">=</span><span class="nam">new_env</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">        <span class="nam">stdout</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">PIPE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">        <span class="nam">stderr</span><span class="op">=</span><span class="nam">subprocess</span><span class="op">.</span><span class="nam">STDOUT</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">        <span class="nam">text</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">    <span class="op">)</span> <span class="key">as</span> <span class="nam">process</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">        <span class="key">if</span> <span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">            <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">iter</span><span class="op">(</span><span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">readline</span><span class="op">,</span> <span class="str">""</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">                <span class="nam">q</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">            <span class="nam">process</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">close</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">            <span class="nam">process</span><span class="op">.</span><span class="nam">wait</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">            <span class="nam">ret_code</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">returncode</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">            <span class="key">if</span> <span class="nam">ret_code</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">                <span class="nam">q</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">int</span><span class="op">(</span><span class="nam">ret_code</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Process has no return code"</span><span class="op">)</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_web_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 17:02 -0400
+            created at 2024-04-12 08:32 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,370 +1,457 @@
-************ CCoovveerraaggee ffoorr ssrrcc//ppaarr__rruunn//eexxeeccuuttoorr..ppyy:: 9988%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//ppaarr__rruunn//eexxeeccuuttoorr..ppyy:: 8855%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 220033 ssttaatteemmeennttss ?  119988 rruunn 55 mmiissssiinngg 77 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-31 17:02 -0400
+********** 225511 ssttaatteemmeennttss ?  221133 rruunn 3388 mmiissssiinngg 77 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+12 08:32 -0400
 _1"""Todo""" 
 _2 
 _3import asyncio 
 _4import configparser 
 _5import enum 
 _6import multiprocessing as mp 
-_7import queue 
-_8import subprocess 
-_9from collections import OrderedDict 
-_1_0from concurrent.futures import Future, ProcessPoolExecutor 
-_1_1from pathlib import Path 
-_1_2from queue import Queue 
-_1_3from typing import List, Optional, Protocol, TypeVar, Union 
-_1_4from pydantic import BaseModel, Field, ConfigDict 
-_1_5 
-_1_6 
-_1_7# Type alias for a generic future. 
-_1_8GenFuture = Union[Future, asyncio.Future] 
-_1_9 
-_2_0ContextT = TypeVar("ContextT") 
+_7import os 
+_8import queue 
+_9import subprocess 
+_1_0from collections import OrderedDict 
+_1_1from concurrent.futures import Future, ProcessPoolExecutor 
+_1_2from pathlib import Path 
+_1_3from queue import Queue 
+_1_4import time 
+_1_5from typing import List, Optional, Protocol, TypeVar, Union, Any 
+_1_6from pydantic import BaseModel, Field, ConfigDict 
+_1_7import tomlkit 
+_1_8 
+_1_9# Type alias for a generic future. 
+_2_0GenFuture = Union[Future, asyncio.Future] 
 _2_1 
-_2_2 
-_2_3class ProcessingStrategy(enum.Enum): 
-_2_4 """Enum for processing strategies.""" 
-_2_5 
-_2_6 ON_COMP = "comp" 
-_2_7 ON_RECV = "recv" 
-_2_8 
-_2_9 
-_3_0class CommandStatus(enum.Enum): 
-_3_1 """Enum for command status.""" 
-_3_2 
-_3_3 NOT_STARTED = "Not Started" 
-_3_4 RUNNING = "Running" 
-_3_5 SUCCESS = "Success" 
-_3_6 FAILURE = "Failure" 
-_3_7 
-_3_8 def completed(self) -> bool: 
-_3_9 """Return True if the command has completed.""" 
-_4_0 return self in [CommandStatus.SUCCESS, CommandStatus.FAILURE] 
-_4_1 
-_4_2 
-_4_3class Command(BaseModel): 
-_4_4 """Holder for a command and its name.""" 
-_4_5 
-_4_6 model_config = ConfigDict(arbitrary_types_allowed=True) 
+_2_2ContextT = TypeVar("ContextT") 
+_2_3 
+_2_4 
+_2_5class ProcessingStrategy(enum.Enum): 
+_2_6 """Enum for processing strategies.""" 
+_2_7 
+_2_8 ON_COMP = "comp" 
+_2_9 ON_RECV = "recv" 
+_3_0 
+_3_1 
+_3_2class CommandStatus(enum.Enum): 
+_3_3 """Enum for command status.""" 
+_3_4 
+_3_5 NOT_STARTED = "Not Started" 
+_3_6 RUNNING = "Running" 
+_3_7 SUCCESS = "Success" 
+_3_8 FAILURE = "Failure" 
+_3_9 
+_4_0 def completed(self) -> bool: 
+_4_1 """Return True if the command has completed.""" 
+_4_2 return self in [CommandStatus.SUCCESS, CommandStatus.FAILURE] 
+_4_3 
+_4_4 
+_4_5class Command(BaseModel): 
+_4_6 """Holder for a command and its name.""" 
 _4_7 
-_4_8 name: str 
-_4_9 cmd: str 
-_5_0 status: CommandStatus = CommandStatus.NOT_STARTED 
-_5_1 unflushed: List[str] = Field(default=[], exclude=True) 
-_5_2 num_non_empty_lines: int = Field(default=0, exclude=True) 
-_5_3 ret_code: Optional[int] = Field(default=None, exclude=True) 
-_5_4 fut: Optional[GenFuture] = Field(default=None, exclude=True) 
-_5_5 
-_5_6 def incr_line_count(self, line: str) -> None: 
-_5_7 """Increment the non-empty line count.""" 
-_5_8 if line.strip(): 
-_5_9 self.num_non_empty_lines += 1 
-_6_0 
-_6_1 def append_unflushed(self, line: str) -> None: 
-_6_2 """Append a line to the output and increment the non-empty line count.""" 
-_6_3 self.unflushed.append(line) 
-_6_4 
-_6_5 def clear_unflushed(self) -> None: 
-_6_6 """Clear the unflushed output.""" 
-_6_7 self.unflushed.clear() 
-_6_8 
-_6_9 def set_ret_code(self, ret_code: int): 
-_7_0 """Set the return code and status of the command.""" 
-_7_1 self.ret_code = ret_code 
-_7_2 if self.fut: 
-_7_3 self.fut.cancel() 
-_7_4 self.fut = None 
-_7_5 if ret_code == 0: 
-_7_6 self.status = CommandStatus.SUCCESS 
-_7_7 else: 
-_7_8 self.status = CommandStatus.FAILURE 
-_7_9 
-_8_0 def set_running(self): 
-_8_1 """Set the command status to running.""" 
-_8_2 self.status = CommandStatus.RUNNING 
-_8_3 
-_8_4 
-_8_5class CommandCB(Protocol): 
-_8_6 def on_start(self, cmd: Command) -> None: ... 
-_8_7 def on_recv(self, cmd: Command, output: str) -> None: ... 
-_8_8 def on_term(self, cmd: Command, exit_code: int) -> None: ... 
-_8_9 
-_9_0 
-_9_1class CommandAsyncCB(Protocol): 
-_9_2 async def on_start(self, cmd: Command) -> None: ... 
-_9_3 async def on_recv(self, cmd: Command, output: str) -> None: ... 
-_9_4 async def on_term(self, cmd: Command, exit_code: int) -> None: ... 
-_9_5 
-_9_6 
-_9_7class QRetriever: 
-_9_8 def __init__(self, q: Queue, timeout: int, retries: int): 
-_9_9 self.q = q 
-_1_0_0 self.timeout = timeout 
-_1_0_1 self.retries = retries 
-_1_0_2 
-_1_0_3 def get(self): 
-_1_0_4 retry_count = 0 
-_1_0_5 while True: 
-_1_0_6 try: 
-_1_0_7 return self.q.get(block=True, timeout=self.timeout) 
-_1_0_8 except queue.Empty: 
-_1_0_9 if retry_count < self.retries: 
-_1_1_0 retry_count += 1 
-_1_1_1 continue 
-_1_1_2 else: 
-_1_1_3 raise TimeoutError("Timeout waiting for command output") 
-_1_1_4 
-_1_1_5 
-_1_1_6class CommandGroup(BaseModel): 
-_1_1_7 """Holder for a group of commands.""" 
-_1_1_8 
-_1_1_9 name: str 
-_1_2_0 cmds: OrderedDict[str, Command] = Field(default_factory=OrderedDict) 
-_1_2_1 
-_1_2_2 async def run_async( 
-_1_2_3 self, 
-_1_2_4 strategy: ProcessingStrategy, 
-_1_2_5 callbacks: CommandAsyncCB, 
-_1_2_6 ): 
-_1_2_7 q = mp.Manager().Queue() 
-_1_2_8 pool = ProcessPoolExecutor() 
-_1_2_9 futs = [ 
-_1_3_0 asyncio.get_event_loop().run_in_executor(pool, run_command, cmd.name,
-cmd.cmd, q) 
-_1_3_1 for _, cmd in self.cmds.items() 
-_1_3_2 ] 
-_1_3_3 
-_1_3_4 for (_, cmd), fut in zip(self.cmds.items(), futs): 
-_1_3_5 cmd.fut = fut 
-_1_3_6 cmd.set_running() 
-_1_3_7 
-_1_3_8 return await self._process_q_async(q, strategy, callbacks) 
-_1_3_9 
-_1_4_0 def run( 
-_1_4_1 self, 
-_1_4_2 strategy: ProcessingStrategy, 
-_1_4_3 callbacks: CommandCB, 
-_1_4_4 ): 
-_1_4_5 q = mp.Manager().Queue() 
-_1_4_6 pool = ProcessPoolExecutor() 
-_1_4_7 futs = [pool.submit(run_command, cmd.name, cmd.cmd, q) for _, cmd in
-self.cmds.items()] 
-_1_4_8 for (_, cmd), fut in zip(self.cmds.items(), futs): 
-_1_4_9 cmd.fut = fut 
-_1_5_0 cmd.set_running() 
-_1_5_1 
-_1_5_2 return self._process_q(q, strategy, callbacks) 
-_1_5_3 
-_1_5_4 def _process_q( 
-_1_5_5 self, 
-_1_5_6 q: Queue, 
-_1_5_7 strategy: ProcessingStrategy, 
-_1_5_8 callbacks: CommandCB, 
-_1_5_9 ) -> int: 
-_1_6_0 grp_exit_code = 0 
-_1_6_1 
-_1_6_2 if strategy == ProcessingStrategy.ON_RECV: 
-_1_6_3 for _, cmd in self.cmds.items(): 
-_1_6_4 callbacks.on_start(cmd) 
-_1_6_5 
-_1_6_6 timeout = 10 
-_1_6_7 retries = 3 
-_1_6_8 q_ret = QRetriever(q, timeout, retries) 
-_1_6_9 while True: 
-_1_7_0 q_result = q_ret.get() 
+_4_8 model_config = ConfigDict(arbitrary_types_allowed=True) 
+_4_9 
+_5_0 name: str 
+_5_1 cmd: str 
+_5_2 passenv: Optional[list[str]] = Field(default=None) 
+_5_3 setenv: Optional[dict[str, str]] = Field(default=None) 
+_5_4 status: CommandStatus = CommandStatus.NOT_STARTED 
+_5_5 unflushed: List[str] = Field(default=[], exclude=True) 
+_5_6 num_non_empty_lines: int = Field(default=0, exclude=True) 
+_5_7 ret_code: Optional[int] = Field(default=None, exclude=True) 
+_5_8 fut: Optional[GenFuture] = Field(default=None, exclude=True) 
+_5_9 start_time: Optional[float] = Field(default=None, exclude=True) 
+_6_0 elapsed: Optional[float] = Field(default=None, exclude=True) 
+_6_1 
+_6_2 def incr_line_count(self, line: str) -> None: 
+_6_3 """Increment the non-empty line count.""" 
+_6_4 if line.strip(): 
+_6_5 self.num_non_empty_lines += 1 
+_6_6 
+_6_7 def append_unflushed(self, line: str) -> None: 
+_6_8 """Append a line to the output and increment the non-empty line count.""" 
+_6_9 self.unflushed.append(line) 
+_7_0 
+_7_1 def clear_unflushed(self) -> None: 
+_7_2 """Clear the unflushed output.""" 
+_7_3 self.unflushed.clear() 
+_7_4 
+_7_5 def set_ret_code(self, ret_code: int): 
+_7_6 """Set the return code and status of the command.""" 
+_7_7 if self.start_time: 
+_7_8 self.elapsed = time.perf_counter() - self.start_time 
+_7_9 self.ret_code = ret_code 
+_8_0 if self.fut: 
+_8_1 self.fut.cancel() 
+_8_2 self.fut = None 
+_8_3 if ret_code == 0: 
+_8_4 self.status = CommandStatus.SUCCESS 
+_8_5 else: 
+_8_6 self.status = CommandStatus.FAILURE 
+_8_7 
+_8_8 def set_running(self): 
+_8_9 """Set the command status to running.""" 
+_9_0 self.start_time = time.perf_counter() 
+_9_1 self.status = CommandStatus.RUNNING 
+_9_2 
+_9_3 
+_9_4class CommandCB(Protocol): 
+_9_5 def on_start(self, cmd: Command) -> None: ... 
+_9_6 def on_recv(self, cmd: Command, output: str) -> None: ... 
+_9_7 def on_term(self, cmd: Command, exit_code: int) -> None: ... 
+_9_8 
+_9_9 
+_1_0_0class CommandAsyncCB(Protocol): 
+_1_0_1 async def on_start(self, cmd: Command) -> None: ... 
+_1_0_2 async def on_recv(self, cmd: Command, output: str) -> None: ... 
+_1_0_3 async def on_term(self, cmd: Command, exit_code: int) -> None: ... 
+_1_0_4 
+_1_0_5 
+_1_0_6class QRetriever: 
+_1_0_7 def __init__(self, q: Queue, timeout: int, retries: int): 
+_1_0_8 self.q = q 
+_1_0_9 self.timeout = timeout 
+_1_1_0 self.retries = retries 
+_1_1_1 
+_1_1_2 def get(self): 
+_1_1_3 retry_count = 0 
+_1_1_4 while True: 
+_1_1_5 try: 
+_1_1_6 return self.q.get(block=True, timeout=self.timeout) 
+_1_1_7 except queue.Empty: 
+_1_1_8 if retry_count < self.retries: 
+_1_1_9 retry_count += 1 
+_1_2_0 continue 
+_1_2_1 else: 
+_1_2_2 raise TimeoutError("Timeout waiting for command output") 
+_1_2_3 
+_1_2_4 def __str__(self) -> str: 
+_1_2_5 return f"QRetriever(timeout={self.timeout}, retries={self.retries})" 
+_1_2_6 
+_1_2_7 
+_1_2_8class CommandGroup(BaseModel): 
+_1_2_9 """Holder for a group of commands.""" 
+_1_3_0 
+_1_3_1 name: str 
+_1_3_2 desc: Optional[str] = None 
+_1_3_3 cmds: OrderedDict[str, Command] = Field(default_factory=OrderedDict) 
+_1_3_4 timeout: int = Field(default=30) 
+_1_3_5 retries: int = Field(default=3) 
+_1_3_6 
+_1_3_7 async def run_async( 
+_1_3_8 self, 
+_1_3_9 strategy: ProcessingStrategy, 
+_1_4_0 callbacks: CommandAsyncCB, 
+_1_4_1 ): 
+_1_4_2 q = mp.Manager().Queue() 
+_1_4_3 pool = ProcessPoolExecutor() 
+_1_4_4 futs = [ 
+_1_4_5 asyncio.get_event_loop().run_in_executor(pool, run_command, cmd.name,
+cmd.cmd, cmd.setenv, q) 
+_1_4_6 for _, cmd in self.cmds.items() 
+_1_4_7 ] 
+_1_4_8 
+_1_4_9 for (_, cmd), fut in zip(self.cmds.items(), futs): 
+_1_5_0 cmd.fut = fut 
+_1_5_1 cmd.set_running() 
+_1_5_2 
+_1_5_3 return await self._process_q_async(q, strategy, callbacks) 
+_1_5_4 
+_1_5_5 def run(self, strategy: ProcessingStrategy, callbacks: CommandCB): 
+_1_5_6 q = mp.Manager().Queue() 
+_1_5_7 pool = ProcessPoolExecutor() 
+_1_5_8 futs = [pool.submit(run_command, cmd.name, cmd.cmd, cmd.setenv, q) for _,
+cmd in self.cmds.items()] 
+_1_5_9 for (_, cmd), fut in zip(self.cmds.items(), futs): 
+_1_6_0 cmd.fut = fut 
+_1_6_1 cmd.set_running() 
+_1_6_2 return self._process_q(q, strategy, callbacks) 
+_1_6_3 
+_1_6_4 def _process_q( 
+_1_6_5 self, 
+_1_6_6 q: Queue, 
+_1_6_7 strategy: ProcessingStrategy, 
+_1_6_8 callbacks: CommandCB, 
+_1_6_9 ) -> int: 
+_1_7_0 grp_exit_code = 0 
 _1_7_1 
-_1_7_2 # Can only get here with a valid message from the Q 
-_1_7_3 cmd_name = q_result[0] 
-_1_7_4 exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else
+_1_7_2 if strategy == ProcessingStrategy.ON_RECV: 
+_1_7_3 for _, cmd in self.cmds.items(): 
+_1_7_4 callbacks.on_start(cmd) 
+_1_7_5 
+_1_7_6 q_ret = QRetriever(q, self.timeout, self.retries) 
+_1_7_7 while True: 
+_1_7_8 q_result = q_ret.get() 
+_1_7_9 
+_1_8_0 # Can only get here with a valid message from the Q 
+_1_8_1 cmd_name = q_result[0] 
+_1_8_2 exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else
 None 
-_1_7_5 output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str)
+_1_8_3 output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str)
 else None 
-_1_7_6 if exit_code is None and output_line is None: 
-_1_7_7 raise ValueError("Invalid Q message") # pragma: no cover 
-_1_7_8 
-_1_7_9 cmd = self.cmds[cmd_name] 
-_1_8_0 if strategy == ProcessingStrategy.ON_RECV: 
-_1_8_1 if output_line is not None: 
-_1_8_2 cmd.incr_line_count(output_line) 
-_1_8_3 callbacks.on_recv(cmd, output_line) 
-_1_8_4 elif exit_code is not None: 
-_1_8_5 cmd.set_ret_code(exit_code) 
-_1_8_6 callbacks.on_term(cmd, exit_code) 
-_1_8_7 if exit_code != 0: 
-_1_8_8 grp_exit_code = 1 
-_1_8_9 else: 
-_1_9_0 raise ValueError("Invalid Q message") # pragma: no cover 
-_1_9_1 
-_1_9_2 if strategy == ProcessingStrategy.ON_COMP: 
-_1_9_3 if output_line is not None: 
-_1_9_4 cmd.incr_line_count(output_line) 
-_1_9_5 cmd.append_unflushed(output_line) 
-_1_9_6 elif exit_code is not None: 
-_1_9_7 callbacks.on_start(cmd) 
-_1_9_8 for line in cmd.unflushed: 
-_1_9_9 callbacks.on_recv(cmd, line) 
-_2_0_0 cmd.clear_unflushed() 
-_2_0_1 callbacks.on_term(cmd, exit_code) 
-_2_0_2 cmd.set_ret_code(exit_code) 
-_2_0_3 if exit_code != 0: 
-_2_0_4 grp_exit_code = 1 
-_2_0_5 else: 
-_2_0_6 raise ValueError("Invalid Q message") # pragma: no cover 
-_2_0_7 
-_2_0_8 if all(cmd.status.completed() for _, cmd in self.cmds.items()): 
-_2_0_9 break 
-_2_1_0 return grp_exit_code 
-_2_1_1 
-_2_1_2 async def _process_q_async( 
-_2_1_3 self, 
-_2_1_4 q: Queue, 
-_2_1_5 strategy: ProcessingStrategy, 
-_2_1_6 callbacks: CommandAsyncCB, 
-_2_1_7 ) -> int: 
-_2_1_8 grp_exit_code = 0 
+_1_8_4 if exit_code is None and output_line is None: 
+_1_8_5 raise ValueError("Invalid Q message") # pragma: no cover 
+_1_8_6 
+_1_8_7 cmd = self.cmds[cmd_name] 
+_1_8_8 if strategy == ProcessingStrategy.ON_RECV: 
+_1_8_9 if output_line is not None: 
+_1_9_0 cmd.incr_line_count(output_line) 
+_1_9_1 callbacks.on_recv(cmd, output_line) 
+_1_9_2 elif exit_code is not None: 
+_1_9_3 cmd.set_ret_code(exit_code) 
+_1_9_4 callbacks.on_term(cmd, exit_code) 
+_1_9_5 if exit_code != 0: 
+_1_9_6 grp_exit_code = 1 
+_1_9_7 else: 
+_1_9_8 raise ValueError("Invalid Q message") # pragma: no cover 
+_1_9_9 
+_2_0_0 if strategy == ProcessingStrategy.ON_COMP: 
+_2_0_1 if output_line is not None: 
+_2_0_2 cmd.incr_line_count(output_line) 
+_2_0_3 cmd.append_unflushed(output_line) 
+_2_0_4 elif exit_code is not None: 
+_2_0_5 callbacks.on_start(cmd) 
+_2_0_6 for line in cmd.unflushed: 
+_2_0_7 callbacks.on_recv(cmd, line) 
+_2_0_8 cmd.clear_unflushed() 
+_2_0_9 callbacks.on_term(cmd, exit_code) 
+_2_1_0 cmd.set_ret_code(exit_code) 
+_2_1_1 if exit_code != 0: 
+_2_1_2 grp_exit_code = 1 
+_2_1_3 else: 
+_2_1_4 raise ValueError("Invalid Q message") # pragma: no cover 
+_2_1_5 
+_2_1_6 if all(cmd.status.completed() for _, cmd in self.cmds.items()): 
+_2_1_7 break 
+_2_1_8 return grp_exit_code 
 _2_1_9 
-_2_2_0 if strategy == ProcessingStrategy.ON_RECV: 
-_2_2_1 for _, cmd in self.cmds.items(): 
-_2_2_2 await callbacks.on_start(cmd) 
-_2_2_3 
-_2_2_4 timeout = 10 
-_2_2_5 retries = 3 
-_2_2_6 q_ret = QRetriever(q, timeout, retries) 
-_2_2_7 while True: 
-_2_2_8 await asyncio.sleep(0) 
-_2_2_9 q_result = q_ret.get() 
-_2_3_0 
-_2_3_1 # Can only get here with a valid message from the Q 
-_2_3_2 cmd_name = q_result[0] 
-_2_3_3 # print(q_result, type(q_result[0]), type(q_result[1])) 
-_2_3_4 exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else
+_2_2_0 async def _process_q_async( 
+_2_2_1 self, 
+_2_2_2 q: Queue, 
+_2_2_3 strategy: ProcessingStrategy, 
+_2_2_4 callbacks: CommandAsyncCB, 
+_2_2_5 ) -> int: 
+_2_2_6 grp_exit_code = 0 
+_2_2_7 
+_2_2_8 if strategy == ProcessingStrategy.ON_RECV: 
+_2_2_9 for _, cmd in self.cmds.items(): 
+_2_3_0 await callbacks.on_start(cmd) 
+_2_3_1 
+_2_3_2 q_ret = QRetriever(q, self.timeout, self.retries) 
+_2_3_3 while True: 
+_2_3_4 await asyncio.sleep(0) 
+_2_3_5 q_result = q_ret.get() 
+_2_3_6 
+_2_3_7 # Can only get here with a valid message from the Q 
+_2_3_8 cmd_name = q_result[0] 
+_2_3_9 exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else
 None 
-_2_3_5 output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str)
+_2_4_0 output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str)
 else None 
-_2_3_6 # print(output_line, exit_code) 
-_2_3_7 if exit_code is None and output_line is None: 
-_2_3_8 raise ValueError("Invalid Q message") # pragma: no cover 
-_2_3_9 
-_2_4_0 cmd = self.cmds[cmd_name] 
-_2_4_1 if strategy == ProcessingStrategy.ON_RECV: 
-_2_4_2 if output_line is not None: 
-_2_4_3 cmd.incr_line_count(output_line) 
-_2_4_4 await callbacks.on_recv(cmd, output_line) 
-_2_4_5 elif exit_code is not None: 
-_2_4_6 cmd.set_ret_code(exit_code) 
-_2_4_7 await callbacks.on_term(cmd, exit_code) 
-_2_4_8 if exit_code != 0: 
-_2_4_9 grp_exit_code = 1 
-_2_5_0 else: 
-_2_5_1 raise ValueError("Invalid Q message") # pragma: no cover 
-_2_5_2 
-_2_5_3 if strategy == ProcessingStrategy.ON_COMP: 
-_2_5_4 if output_line is not None: 
-_2_5_5 cmd.incr_line_count(output_line) 
-_2_5_6 cmd.append_unflushed(output_line) 
-_2_5_7 elif exit_code is not None: 
-_2_5_8 await callbacks.on_start(cmd) 
-_2_5_9 for line in cmd.unflushed: 
-_2_6_0 await callbacks.on_recv(cmd, line) 
-_2_6_1 cmd.clear_unflushed() 
-_2_6_2 await callbacks.on_term(cmd, exit_code) 
-_2_6_3 cmd.set_ret_code(exit_code) 
-_2_6_4 if exit_code != 0: 
-_2_6_5 grp_exit_code = 1 
-_2_6_6 else: 
-_2_6_7 raise ValueError("Invalid Q message") # pragma: no cover 
-_2_6_8 
-_2_6_9 if all(cmd.status.completed() for _, cmd in self.cmds.items()): 
-_2_7_0 break 
-_2_7_1 return grp_exit_code 
+_2_4_1 if exit_code is None and output_line is None: 
+_2_4_2 raise ValueError("Invalid Q message") # pragma: no cover 
+_2_4_3 
+_2_4_4 cmd = self.cmds[cmd_name] 
+_2_4_5 if strategy == ProcessingStrategy.ON_RECV: 
+_2_4_6 if output_line is not None: 
+_2_4_7 cmd.incr_line_count(output_line) 
+_2_4_8 await callbacks.on_recv(cmd, output_line) 
+_2_4_9 elif exit_code is not None: 
+_2_5_0 cmd.set_ret_code(exit_code) 
+_2_5_1 await callbacks.on_term(cmd, exit_code) 
+_2_5_2 if exit_code != 0: 
+_2_5_3 grp_exit_code = 1 
+_2_5_4 else: 
+_2_5_5 raise ValueError("Invalid Q message") # pragma: no cover 
+_2_5_6 
+_2_5_7 if strategy == ProcessingStrategy.ON_COMP: 
+_2_5_8 if output_line is not None: 
+_2_5_9 cmd.incr_line_count(output_line) 
+_2_6_0 cmd.append_unflushed(output_line) 
+_2_6_1 elif exit_code is not None: 
+_2_6_2 await callbacks.on_start(cmd) 
+_2_6_3 for line in cmd.unflushed: 
+_2_6_4 await callbacks.on_recv(cmd, line) 
+_2_6_5 cmd.clear_unflushed() 
+_2_6_6 await callbacks.on_term(cmd, exit_code) 
+_2_6_7 cmd.set_ret_code(exit_code) 
+_2_6_8 if exit_code != 0: 
+_2_6_9 grp_exit_code = 1 
+_2_7_0 else: 
+_2_7_1 raise ValueError("Invalid Q message") # pragma: no cover 
 _2_7_2 
-_2_7_3 
-_2_7_4def read_commands_ini(filename: Union[str, Path]) -> list[CommandGroup]: 
-_2_7_5 """Read a commands.ini file and return a list of CommandGroup objects. 
+_2_7_3 if all(cmd.status.completed() for _, cmd in self.cmds.items()): 
+_2_7_4 break 
+_2_7_5 return grp_exit_code 
 _2_7_6 
-_2_7_7 Args: 
-_2_7_8 filename (Union[str, Path]): The filename of the commands.ini file. 
-_2_7_9 
-_2_8_0 Returns: 
-_2_8_1 list[CommandGroup]: A list of CommandGroup objects. 
-_2_8_2 """ 
-_2_8_3 config = configparser.ConfigParser() 
-_2_8_4 config.read(filename) 
-_2_8_5 
-_2_8_6 command_groups = [] 
-_2_8_7 for section in config.sections(): 
-_2_8_8 if section.startswith("group."): 
-_2_8_9 group_name = section.replace("group.", "") 
-_2_9_0 commands = OrderedDict() 
-_2_9_1 for name, cmd in config.items(section): 
-_2_9_2 name = name.strip() 
-_2_9_3 commands[name] = Command(name=name, cmd=cmd.strip()) 
-_2_9_4 command_group = CommandGroup(name=group_name, cmds=commands) 
-_2_9_5 command_groups.append(command_group) 
-_2_9_6 
-_2_9_7 return command_groups 
-_2_9_8 
-_2_9_9 
-_3_0_0def write_commands_ini(filename: Union[str, Path], command_groups: list
-[CommandGroup]): 
-_3_0_1 """Write a list of CommandGroup objects to a commands.ini file. 
+_2_7_7 
+_2_7_8def read_commands_ini(filename: Union[str, Path]) -> list[CommandGroup]: 
+_2_7_9 """Read a commands.ini file and return a list of CommandGroup objects. 
+_2_8_0 
+_2_8_1 Args: 
+_2_8_2 filename (Union[str, Path]): The filename of the commands.ini file. 
+_2_8_3 
+_2_8_4 Returns: 
+_2_8_5 list[CommandGroup]: A list of CommandGroup objects. 
+_2_8_6 """ 
+_2_8_7 config = configparser.ConfigParser() 
+_2_8_8 config.read(filename) 
+_2_8_9 
+_2_9_0 command_groups = [] 
+_2_9_1 for section in config.sections(): 
+_2_9_2 if section.startswith("group."): 
+_2_9_3 group_name = section.replace("group.", "") 
+_2_9_4 commands = OrderedDict() 
+_2_9_5 for name, cmd in config.items(section): 
+_2_9_6 name = name.strip() 
+_2_9_7 commands[name] = Command(name=name, cmd=cmd.strip()) 
+_2_9_8 command_group = CommandGroup(name=group_name, cmds=commands) 
+_2_9_9 command_groups.append(command_group) 
+_3_0_0 
+_3_0_1 return command_groups 
 _3_0_2 
-_3_0_3 Args: 
-_3_0_4 filename (Union[str, Path]): The filename of the commands.ini file. 
-_3_0_5 command_groups (list[CommandGroup]): A list of CommandGroup objects. 
-_3_0_6 """ 
-_3_0_7 config = configparser.ConfigParser() 
-_3_0_8 
-_3_0_9 for group in command_groups: 
-_3_1_0 section_name = f"group.{group.name}" 
-_3_1_1 config[section_name] = {} 
-_3_1_2 for _, command in group.cmds.items(): 
-_3_1_3 config[section_name][command.name] = command.cmd 
-_3_1_4 
-_3_1_5 with open(filename, "w", encoding="utf-8") as configfile: 
-_3_1_6 config.write(configfile) 
-_3_1_7 
+_3_0_3 
+_3_0_4def write_commands_ini(filename: Union[str, Path], command_groups: list
+[CommandGroup]): 
+_3_0_5 """Write a list of CommandGroup objects to a commands.ini file. 
+_3_0_6 
+_3_0_7 Args: 
+_3_0_8 filename (Union[str, Path]): The filename of the commands.ini file. 
+_3_0_9 command_groups (list[CommandGroup]): A list of CommandGroup objects. 
+_3_1_0 """ 
+_3_1_1 config = configparser.ConfigParser() 
+_3_1_2 
+_3_1_3 for group in command_groups: 
+_3_1_4 section_name = f"group.{group.name}" 
+_3_1_5 config[section_name] = {} 
+_3_1_6 for _, command in group.cmds.items(): 
+_3_1_7 config[section_name][command.name] = command.cmd 
 _3_1_8 
-_3_1_9def run_command(name: str, command: str, q: Queue) -> None: 
-_3_2_0 """Run a command and put the output into a queue. The output is a tuple of
+_3_1_9 with open(filename, "w", encoding="utf-8") as configfile: 
+_3_2_0 config.write(configfile) 
+_3_2_1 
+_3_2_2 
+_3_2_3def _validate_mandatory_keys(data: tomlkit.items.Table, keys: list[str],
+context: str) -> tuple[Any, ...]: 
+_3_2_4 """Validate that the mandatory keys are present in the data. 
+_3_2_5 
+_3_2_6 Args: 
+_3_2_7 data (tomlkit.items.Table): The data to validate. 
+_3_2_8 keys (list[str]): The mandatory keys. 
+_3_2_9 """ 
+_3_3_0 vals = [] 
+_3_3_1 for key in keys: 
+_3_3_2 val = data.get(key, None) 
+_3_3_3 if not val: 
+_3_3_4 raise ValueError(f"{key} is mandatory, not found in {context}") 
+_3_3_5 vals.append(val) 
+_3_3_6 return tuple(vals) 
+_3_3_7 
+_3_3_8 
+_3_3_9def _get_optional_keys(data: tomlkit.items.Table, keys: list[str],
+default=None) -> tuple[Optional[Any], ...]: 
+_3_4_0 """Get Optional keys or default. 
+_3_4_1 
+_3_4_2 Args: 
+_3_4_3 data (tomlkit.items.Table): The data to use as source 
+_3_4_4 keys (list[str]): The optional keys. 
+_3_4_5 """ 
+_3_4_6 return tuple(data.get(key, default) for key in keys) 
+_3_4_7 
+_3_4_8 
+_3_4_9def read_commands_toml(filename: Union[str, Path]) -> list[CommandGroup]: 
+_3_5_0 """Read a commands.toml file and return a list of CommandGroup objects. 
+_3_5_1 
+_3_5_2 Args: 
+_3_5_3 filename (Union[str, Path]): The filename of the commands.toml file. 
+_3_5_4 
+_3_5_5 Returns: 
+_3_5_6 list[CommandGroup]: A list of CommandGroup objects. 
+_3_5_7 """ 
+_3_5_8 
+_3_5_9 with open(filename, "r", encoding="utf-8") as toml_file: 
+_3_6_0 toml_data = tomlkit.parse(toml_file.read()) 
+_3_6_1 
+_3_6_2 cmd_groups_data = toml_data.get("tool", {}).get("par-run", {}) 
+_3_6_3 if not cmd_groups_data: 
+_3_6_4 raise ValueError("No par-run data found in toml file") 
+_3_6_5 _ = cmd_groups_data.get("description", None) 
+_3_6_6 
+_3_6_7 command_groups = [] 
+_3_6_8 for group_data in cmd_groups_data.get("groups", []): 
+_3_6_9 (group_name,) = _validate_mandatory_keys(group_data, ["name"], "top level
+par-run group") 
+_3_7_0 group_desc, group_timeout, group_retries = _get_optional_keys( 
+_3_7_1 group_data, ["desc", "timeout", "retries"], default=None 
+_3_7_2 ) 
+_3_7_3 
+_3_7_4 if not group_timeout: 
+_3_7_5 group_timeout = 30 
+_3_7_6 if not group_retries: 
+_3_7_7 group_retries = 3 
+_3_7_8 
+_3_7_9 commands = OrderedDict() 
+_3_8_0 for cmd_data in group_data.get("commands", []): 
+_3_8_1 name, exec = _validate_mandatory_keys(cmd_data, ["name", "exec"], f"command
+group {group_name}") 
+_3_8_2 setenv, passenv = _get_optional_keys(cmd_data, ["setenv", "passenv"],
+default=None) 
+_3_8_3 
+_3_8_4 commands[name] = Command(name=name, cmd=exec, setenv=setenv,
+passenv=passenv) 
+_3_8_5 command_group = CommandGroup( 
+_3_8_6 name=group_name, desc=group_desc, cmds=commands, timeout=group_timeout,
+retries=group_retries 
+_3_8_7 ) 
+_3_8_8 command_groups.append(command_group) 
+_3_8_9 
+_3_9_0 return command_groups 
+_3_9_1 
+_3_9_2 
+_3_9_3def run_command(name: str, command: str, setenv: Optional[dict[str, str]],
+q: Queue) -> None: 
+_3_9_4 """Run a command and put the output into a queue. The output is a tuple of
 the command 
-_3_2_1 name and the output line. The final output is a tuple of the command name
+_3_9_5 name and the output line. The final output is a tuple of the command name
 and a dictionary 
-_3_2_2 with the return code. 
-_3_2_3 
-_3_2_4 Args: 
-_3_2_5 name (str): Name of the command. 
-_3_2_6 command (str): Command to run. 
-_3_2_7 q (Queue): Queue to put the output into. 
-_3_2_8 """ 
-_3_2_9 
-_3_3_0 with subprocess.Popen( 
-_3_3_1 f"{command}", 
-_3_3_2 shell=True, 
-_3_3_3 stdout=subprocess.PIPE, 
-_3_3_4 stderr=subprocess.STDOUT, 
-_3_3_5 text=True, 
-_3_3_6 ) as process: 
-_3_3_7 if process.stdout: 
-_3_3_8 for line in iter(process.stdout.readline, ""): 
-_3_3_9 q.put((name, line.strip())) 
-_3_4_0 process.stdout.close() 
-_3_4_1 process.wait() 
-_3_4_2 ret_code = process.returncode 
-_3_4_3 if ret_code is not None: 
-_3_4_4 q.put((name, int(ret_code))) 
-_3_4_5 else: 
-_3_4_6 raise ValueError("Process has no return code") # pragma: no cover 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-31 17:02 -0400
+_3_9_6 with the return code. 
+_3_9_7 
+_3_9_8 Args: 
+_3_9_9 name (Command): Command to run. 
+_4_0_0 q (Queue): Queue to put the output into. 
+_4_0_1 """ 
+_4_0_2 
+_4_0_3 new_env = None 
+_4_0_4 if setenv: 
+_4_0_5 new_env = os.environ.copy() 
+_4_0_6 new_env.update(setenv) 
+_4_0_7 
+_4_0_8 with subprocess.Popen( 
+_4_0_9 command, 
+_4_1_0 shell=True, 
+_4_1_1 env=new_env, 
+_4_1_2 stdout=subprocess.PIPE, 
+_4_1_3 stderr=subprocess.STDOUT, 
+_4_1_4 text=True, 
+_4_1_5 ) as process: 
+_4_1_6 if process.stdout: 
+_4_1_7 for line in iter(process.stdout.readline, ""): 
+_4_1_8 q.put((name, line.strip())) 
+_4_1_9 process.stdout.close() 
+_4_2_0 process.wait() 
+_4_2_1 ret_code = process.returncode 
+_4_2_2 if ret_code is not None: 
+_4_2_3 q.put((name, int(ret_code))) 
+_4_2_4 else: 
+_4_2_5 raise ValueError("Process has no return code") # pragma: no cover 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+12 08:32 -0400
```

### Comparing `par_run-0.1.4/.reports/html/d_417a353b6036f046_web_cli_py.html` & `par_run-0.2.0/.reports/html/d_417a353b6036f046_web_cli_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/.reports/html/d_417a353b6036f046_web_py.html` & `par_run-0.2.0/.reports/html/d_417a353b6036f046_web_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 17:02 -0400
+            created at 2024-04-12 07:35 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -150,13 +150,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 17:02 -0400
+            created at 2024-04-12 07:35 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 4411 ssttaatteemmeennttss ?  2299 rruunn 1122 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-31 17:02 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+12 07:35 -0400
 _1"""Web UI Module""" 
 _2 
 _3from pathlib import Path 
 _4import rich 
 _5from fastapi import Body, FastAPI, Request, WebSocket 
 _6from fastapi.staticfiles import StaticFiles 
 _7from fastapi.templating import Jinja2Templates 
@@ -77,9 +77,9 @@
 _6_0 await websocket.accept() 
 _6_1 cb = WebCommandCB(websocket) 
 _6_2 print("Running commands") 
 _6_3 exit_code = 0 
 _6_4 for grp in master_groups: 
 _6_5 exit_code = exit_code or await grp.run_async(ProcessingStrategy.ON_RECV,
 cb) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-31 17:02 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+12 07:35 -0400
```

### Comparing `par_run-0.1.4/.reports/html/favicon_32.png` & `par_run-0.2.0/.reports/html/favicon_32.png`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/.reports/html/index.html` & `par_run-0.2.0/.reports/html/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">92%</span>
+            <span class="pc_cov">86%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-01 07:45 -0400
+            created at 2024-04-12 08:39 -0400
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -66,53 +66,53 @@
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_417a353b6036f046_cli_py.html">src/par_run/cli.py</a></td>
-                <td>162</td>
-                <td>15</td>
+                <td>172</td>
+                <td>16</td>
                 <td>2</td>
-                <td class="right" data-ratio="147 162">91%</td>
+                <td class="right" data-ratio="156 172">91%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_417a353b6036f046_executor_py.html">src/par_run/executor.py</a></td>
-                <td>203</td>
-                <td>5</td>
+                <td>251</td>
+                <td>38</td>
                 <td>7</td>
-                <td class="right" data-ratio="198 203">98%</td>
+                <td class="right" data-ratio="213 251">85%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_417a353b6036f046_web_py.html">src/par_run/web.py</a></td>
                 <td>41</td>
                 <td>12</td>
                 <td>0</td>
                 <td class="right" data-ratio="29 41">71%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>407</td>
-                <td>32</td>
+                <td>465</td>
+                <td>66</td>
                 <td>9</td>
-                <td class="right" data-ratio="375 407">92%</td>
+                <td class="right" data-ratio="399 465">86%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-01 07:45 -0400
+            created at 2024-04-12 08:39 -0400
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_417a353b6036f046_web_py.html"/>
         <a id="nextFileLink" class="nav" href="d_417a353b6036f046___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-************ CCoovveerraaggee rreeppoorrtt:: 9922%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 8866%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-01 07:45 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-12 08:39 -0400
 MMoodduullee                  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _s_r_c_/_p_a_r___r_u_n_/_____i_n_i_t_____._p_y 1          0       0        100%
-_s_r_c_/_p_a_r___r_u_n_/_c_l_i_._p_y      162        15      2        91%
-_s_r_c_/_p_a_r___r_u_n_/_e_x_e_c_u_t_o_r_._p_y 203        5       7        98%
+_s_r_c_/_p_a_r___r_u_n_/_c_l_i_._p_y      172        16      2        91%
+_s_r_c_/_p_a_r___r_u_n_/_e_x_e_c_u_t_o_r_._p_y 251        38      7        85%
 _s_r_c_/_p_a_r___r_u_n_/_w_e_b_._p_y      41         12      0        71%
-Total                   407        32      9        92%
+Total                   465        66      9        86%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-01 07:45 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-12 08:39 -0400
```

### Comparing `par_run-0.1.4/.reports/html/keybd_closed.png` & `par_run-0.2.0/.reports/html/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/.reports/html/keybd_open.png` & `par_run-0.2.0/.reports/html/keybd_open.png`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/.reports/html/status.json` & `par_run-0.2.0/.reports/html/status.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921666666666666%*

 * *Differences: {"'files'": "{'d_417a353b6036f046___init___py': {'hash': 'f446efc7ead065ed9673c74ed99bd8b3'}, "*

 * *            "'d_417a353b6036f046_cli_py': {'hash': '1fb428d04dbdd753b2a6e2b27de6395d', 'index': "*

 * *            "{'nums': {insert: [(2, 172), (4, 16)], delete: [4, 2]}}}, "*

 * *            "'d_417a353b6036f046_executor_py': {'hash': '30a2e8e096771c03bce574b222368cf2', "*

 * *            "'index': {'nums': {insert: [(2, 251), (4, 38)], delete: [4, 2]}}}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_417a353b6036f046___init___py": {
-            "hash": "ccb563545275a070316909877460bbb9",
+            "hash": "f446efc7ead065ed9673c74ed99bd8b3",
             "index": {
                 "html_filename": "d_417a353b6036f046___init___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -14,40 +14,40 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/__init__.py"
             }
         },
         "d_417a353b6036f046_cli_py": {
-            "hash": "e0b14d46a4e843faf4f7d6bf90551efa",
+            "hash": "1fb428d04dbdd753b2a6e2b27de6395d",
             "index": {
                 "html_filename": "d_417a353b6036f046_cli_py.html",
                 "nums": [
                     0,
                     1,
-                    162,
+                    172,
                     2,
-                    15,
+                    16,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/cli.py"
             }
         },
         "d_417a353b6036f046_executor_py": {
-            "hash": "e6764cfe8a78651b32109ab27c9d08e2",
+            "hash": "30a2e8e096771c03bce574b222368cf2",
             "index": {
                 "html_filename": "d_417a353b6036f046_executor_py.html",
                 "nums": [
                     0,
                     1,
-                    203,
+                    251,
                     7,
-                    5,
+                    38,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/executor.py"
             }
         },
```

### Comparing `par_run-0.1.4/.reports/html/style.css` & `par_run-0.2.0/.reports/html/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/py_tests/conftest.py` & `par_run-0.2.0/py_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/py_tests/test_cli.py` & `par_run-0.2.0/py_tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     command1 = Command(name="cmd1", cmd="echo 'Hello, World!'")
     command2 = Command(name="cmd2", cmd="exit 1")
     commands = {"cmd1": command1, "cmd2": command2}
     return CommandGroup(name="group1", cmds=commands)
 
 
 def test_run(mocker, mock_command_group):
-    mocker.patch("par_run.cli.read_commands_ini", return_value=[mock_command_group])
+    mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--show"])
     assert result.exit_code == 0
 
 
 def test_CLICommandCB_on_start(mocker):
     mock_rich_print = mocker.patch("par_run.cli.rich.print")
@@ -162,47 +162,47 @@
     # Test with PID file and process
     mocker.patch("par_run.cli.psutil.pid_exists", return_value=True)
     mocker.patch("par_run.cli.get_process_port", return_value=8000)
     get_web_server_status()
 
 
 def test_run_with_specific_groups(mocker, mock_command_group):
-    read_mock = mocker.patch("par_run.cli.read_commands_ini", return_value=[mock_command_group])
+    read_mock = mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--groups", "group1"])
     assert result.exit_code == 0
     read_mock.assert_called_once()
 
 
 def test_run_with_fails(mocker, mock_command_group_part_fail):
-    read_mock = mocker.patch("par_run.cli.read_commands_ini", return_value=[mock_command_group_part_fail])
+    read_mock = mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group_part_fail])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run"])
     assert result.exit_code != 0
     read_mock.assert_called_once()
 
 
 def test_run_with_specific_cmds(mocker, mock_command_group):
-    mocker.patch("par_run.cli.read_commands_ini", return_value=[mock_command_group])
+    mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--cmds", "cmd1"])
     assert result.exit_code == 0
     # Add additional assertions to check if the command was filtered correctly
 
 
 def test_run_with_nonexistent_group(mocker, mock_command_group):
-    mocker.patch("par_run.cli.read_commands_ini", return_value=[mock_command_group])
+    mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--groups", "nonexistent"])
     assert result.exit_code == 0
     # Add assertion to ensure no commands are run and appropriate message is displayed
 
 
 def test_run_with_nonexistent_cmd(mocker, mock_command_group):
-    mocker.patch("par_run.cli.read_commands_ini", return_value=[mock_command_group])
+    mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--cmds", "nonexistent"])
     assert result.exit_code == 0
     # Add assertion to ensure no commands are run and appropriate message is displayed
 
 
 def test_start_web_server_already_running(mocker, tmp_path):
```

### Comparing `par_run-0.1.4/py_tests/test_executor.py` & `par_run-0.2.0/py_tests/test_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,17 @@
     command = Command(name="test", cmd="echo 'Hello, World!'")
     assert command.ret_code is None
     assert command.status == CommandStatus.NOT_STARTED
     assert not command.status.completed()
 
     q = mp.Manager().Queue()
     pool = ProcessPoolExecutor()
-    fut = pool.submit(run_command, command.name, command.cmd, q)
+    fut = pool.submit(run_command, command.name, command.cmd, {}, q)
     command.fut = fut
+    command.set_running()
     _ = fut.result()
 
     msg = q.get()
     assert isinstance(msg, tuple)
     assert len(msg) == 2
     assert msg[0] == command.name
     assert msg[1] == "Hello, World!"
@@ -63,15 +64,16 @@
     assert command.status.completed()
 
 
 def test_command_set_ret_code_failure():
     command = Command(name="test", cmd="exit 1")
     q = mp.Manager().Queue()
     pool = ProcessPoolExecutor()
-    fut = pool.submit(run_command, command.name, command.cmd, q)
+    fut = pool.submit(run_command, command.name, command.cmd, {}, q)
+    command.set_running()
     command.fut = fut
     _ = fut.result()
     msg = q.get()
 
     assert isinstance(msg, tuple)
     assert len(msg) == 2
     assert msg[0] == command.name
@@ -273,15 +275,15 @@
     assert all(cmd.status in [CommandStatus.SUCCESS, CommandStatus.FAILURE] for cmd in group.cmds.values())
     assert all(cmd.ret_code in [0, 1] for cmd in group.cmds.values())
     assert group_exit == 1
 
 
 def test_run_command():
     q = mp.Manager().Queue()
-    run_command("Test", "echo 'Hello, World!'", q)
+    run_command("Test", "echo 'Hello, World!'", {}, q)
 
     msg = q.get()
     assert isinstance(msg, tuple)
     assert len(msg) == 2
     assert msg[0] == "Test"
     assert msg[1] == "Hello, World!"
     exit_code = q.get()[1]
```

### Comparing `par_run-0.1.4/py_tests/test_web.py` & `par_run-0.2.0/py_tests/test_web.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/src/par_run/cli.py` & `par_run-0.2.0/src/par_run/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import Optional
 import enum
 
 import rich
 import typer
 
-from .executor import Command, CommandStatus, ProcessingStrategy, read_commands_ini
+from .executor import Command, CommandStatus, ProcessingStrategy, read_commands_toml
 
 PID_FILE = ".par-run.uvicorn.pid"
 
 cli_app = typer.Typer()
 
 
 # Web only functions
@@ -164,27 +164,45 @@
         """Callback function for when a command receives output"""
         if cmd.status == CommandStatus.SUCCESS:
             rich.print(f"[green bold]{cmd.name}: Finished[/]")
         elif cmd.status == CommandStatus.FAILURE:
             rich.print(f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]")
 
 
+def format_elapsed_time(seconds: float) -> str:
+    """
+    Converts a number of seconds into a human-readable time format of HH:MM:SS.xxx
+
+    Args:
+    seconds (float): The number of seconds elapsed.
+
+    Returns:
+    str: The formatted time string.
+    """
+    hours = int(seconds) // 3600
+    minutes = (int(seconds) % 3600) // 60
+    seconds = seconds % 60  # Keeping the fractional part of seconds
+
+    # Return formatted string with seconds rounded to 2 d.p.
+    return f"{hours:02}:{minutes:02}:{seconds:06.2f}"
+
+
 @cli_app.command()
 def run(
     style: ProcessingStrategy = typer.Option(help="Processing strategy", default="comp"),
     show: bool = typer.Option(help="Show available groups and commands", default=False),
-    file: Path = typer.Option(help="The commands.ini file to use", default=Path("commands.ini")),
+    file: Path = typer.Option(help="The commands.ini file to use", default=Path("pyproject.toml")),
     groups: Optional[str] = typer.Option(None, help="Run a specific group of commands, comma spearated"),
     cmds: Optional[str] = typer.Option(None, help="Run a specific commands, comma spearated"),
 ):
     """Run commands in parallel"""
     # Overall exit code, need to track all command exit codes to update this
     exit_code = 0
 
-    master_groups = read_commands_ini(file)
+    master_groups = read_commands_toml(file)
     if show:
         for grp in master_groups:
             rich.print(f"[blue bold]Group: {grp.name}[/]")
             for _, cmd in grp.cmds.items():
                 rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}")
         return
 
@@ -215,17 +233,20 @@
             raise typer.BadParameter("Invalid processing strategy")
 
     # Summarise the results
     for grp in master_groups:
         rich.print(f"[blue bold]Group: {grp.name}[/]")
         for _, cmd in grp.cmds.items():
             if cmd.status == CommandStatus.SUCCESS:
-                rich.print(f"[green bold]Command {cmd.name} succeeded ({cmd.num_non_empty_lines})[/]")
+                elap_str = ""
+                if cmd.elapsed:
+                    elap_str = f", {format_elapsed_time(cmd.elapsed)}"
+                rich.print(f"[green bold]Command {cmd.name} succeeded ({cmd.num_non_empty_lines}{elap_str})[/]")
             else:
-                rich.print(f"[red bold]Command {cmd.name} failed ({cmd.num_non_empty_lines})[/]")
+                rich.print(f"[red bold]Command {cmd.name} failed ({cmd.num_non_empty_lines}{elap_str})[/]")
 
     raise typer.Exit(exit_code)
 
 
 try:
     import os
     import signal
@@ -259,7 +280,10 @@
             get_web_server_status()
         else:
             typer.echo(f"Not a valid command '{command}'", err=True)
             raise typer.Abort()
 
 except ImportError:  # pragma: no cover
     pass  # pragma: no cover
+
+if __name__ == "__main__":
+    cli_app()
```

### Comparing `par_run-0.1.4/src/par_run/executor.py` & `par_run-0.2.0/src/par_run/executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Todo"""
 
 import asyncio
 import configparser
 import enum
 import multiprocessing as mp
+import os
 import queue
 import subprocess
 from collections import OrderedDict
 from concurrent.futures import Future, ProcessPoolExecutor
 from pathlib import Path
 from queue import Queue
-from typing import List, Optional, Protocol, TypeVar, Union
+import time
+from typing import List, Optional, Protocol, TypeVar, Union, Any
 from pydantic import BaseModel, Field, ConfigDict
-
+import tomlkit
 
 # Type alias for a generic future.
 GenFuture = Union[Future, asyncio.Future]
 
 ContextT = TypeVar("ContextT")
 
 
@@ -43,19 +45,23 @@
 class Command(BaseModel):
     """Holder for a command and its name."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     name: str
     cmd: str
+    passenv: Optional[list[str]] = Field(default=None)
+    setenv: Optional[dict[str, str]] = Field(default=None)
     status: CommandStatus = CommandStatus.NOT_STARTED
     unflushed: List[str] = Field(default=[], exclude=True)
     num_non_empty_lines: int = Field(default=0, exclude=True)
     ret_code: Optional[int] = Field(default=None, exclude=True)
     fut: Optional[GenFuture] = Field(default=None, exclude=True)
+    start_time: Optional[float] = Field(default=None, exclude=True)
+    elapsed: Optional[float] = Field(default=None, exclude=True)
 
     def incr_line_count(self, line: str) -> None:
         """Increment the non-empty line count."""
         if line.strip():
             self.num_non_empty_lines += 1
 
     def append_unflushed(self, line: str) -> None:
@@ -64,25 +70,28 @@
 
     def clear_unflushed(self) -> None:
         """Clear the unflushed output."""
         self.unflushed.clear()
 
     def set_ret_code(self, ret_code: int):
         """Set the return code and status of the command."""
+        if self.start_time:
+            self.elapsed = time.perf_counter() - self.start_time
         self.ret_code = ret_code
         if self.fut:
             self.fut.cancel()
             self.fut = None
         if ret_code == 0:
             self.status = CommandStatus.SUCCESS
         else:
             self.status = CommandStatus.FAILURE
 
     def set_running(self):
         """Set the command status to running."""
+        self.start_time = time.perf_counter()
         self.status = CommandStatus.RUNNING
 
 
 class CommandCB(Protocol):
     def on_start(self, cmd: Command) -> None: ...
     def on_recv(self, cmd: Command, output: str) -> None: ...
     def on_term(self, cmd: Command, exit_code: int) -> None: ...
@@ -108,68 +117,67 @@
             except queue.Empty:
                 if retry_count < self.retries:
                     retry_count += 1
                     continue
                 else:
                     raise TimeoutError("Timeout waiting for command output")
 
+    def __str__(self) -> str:
+        return f"QRetriever(timeout={self.timeout}, retries={self.retries})"
+
 
 class CommandGroup(BaseModel):
     """Holder for a group of commands."""
 
     name: str
+    desc: Optional[str] = None
     cmds: OrderedDict[str, Command] = Field(default_factory=OrderedDict)
+    timeout: int = Field(default=30)
+    retries: int = Field(default=3)
 
     async def run_async(
         self,
         strategy: ProcessingStrategy,
         callbacks: CommandAsyncCB,
     ):
         q = mp.Manager().Queue()
         pool = ProcessPoolExecutor()
         futs = [
-            asyncio.get_event_loop().run_in_executor(pool, run_command, cmd.name, cmd.cmd, q)
+            asyncio.get_event_loop().run_in_executor(pool, run_command, cmd.name, cmd.cmd, cmd.setenv, q)
             for _, cmd in self.cmds.items()
         ]
 
         for (_, cmd), fut in zip(self.cmds.items(), futs):
             cmd.fut = fut
             cmd.set_running()
 
         return await self._process_q_async(q, strategy, callbacks)
 
-    def run(
-        self,
-        strategy: ProcessingStrategy,
-        callbacks: CommandCB,
-    ):
+    def run(self, strategy: ProcessingStrategy, callbacks: CommandCB):
         q = mp.Manager().Queue()
         pool = ProcessPoolExecutor()
-        futs = [pool.submit(run_command, cmd.name, cmd.cmd, q) for _, cmd in self.cmds.items()]
+        futs = [pool.submit(run_command, cmd.name, cmd.cmd, cmd.setenv, q) for _, cmd in self.cmds.items()]
         for (_, cmd), fut in zip(self.cmds.items(), futs):
             cmd.fut = fut
             cmd.set_running()
-
         return self._process_q(q, strategy, callbacks)
 
     def _process_q(
         self,
         q: Queue,
         strategy: ProcessingStrategy,
         callbacks: CommandCB,
     ) -> int:
         grp_exit_code = 0
 
         if strategy == ProcessingStrategy.ON_RECV:
             for _, cmd in self.cmds.items():
                 callbacks.on_start(cmd)
 
-        timeout = 10
-        retries = 3
-        q_ret = QRetriever(q, timeout, retries)
+        q_ret = QRetriever(q, self.timeout, self.retries)
         while True:
             q_result = q_ret.get()
 
             # Can only get here with a valid message from the Q
             cmd_name = q_result[0]
             exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else None
             output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str) else None
@@ -217,27 +225,23 @@
     ) -> int:
         grp_exit_code = 0
 
         if strategy == ProcessingStrategy.ON_RECV:
             for _, cmd in self.cmds.items():
                 await callbacks.on_start(cmd)
 
-        timeout = 10
-        retries = 3
-        q_ret = QRetriever(q, timeout, retries)
+        q_ret = QRetriever(q, self.timeout, self.retries)
         while True:
             await asyncio.sleep(0)
             q_result = q_ret.get()
 
             # Can only get here with a valid message from the Q
             cmd_name = q_result[0]
-            # print(q_result, type(q_result[0]), type(q_result[1]))
             exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else None
             output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str) else None
-            # print(output_line, exit_code)
             if exit_code is None and output_line is None:
                 raise ValueError("Invalid Q message")  # pragma: no cover
 
             cmd = self.cmds[cmd_name]
             if strategy == ProcessingStrategy.ON_RECV:
                 if output_line is not None:
                     cmd.incr_line_count(output_line)
@@ -312,28 +316,103 @@
         for _, command in group.cmds.items():
             config[section_name][command.name] = command.cmd
 
     with open(filename, "w", encoding="utf-8") as configfile:
         config.write(configfile)
 
 
-def run_command(name: str, command: str, q: Queue) -> None:
+def _validate_mandatory_keys(data: tomlkit.items.Table, keys: list[str], context: str) -> tuple[Any, ...]:
+    """Validate that the mandatory keys are present in the data.
+
+    Args:
+        data (tomlkit.items.Table): The data to validate.
+        keys (list[str]): The mandatory keys.
+    """
+    vals = []
+    for key in keys:
+        val = data.get(key, None)
+        if not val:
+            raise ValueError(f"{key} is mandatory, not found in {context}")
+        vals.append(val)
+    return tuple(vals)
+
+
+def _get_optional_keys(data: tomlkit.items.Table, keys: list[str], default=None) -> tuple[Optional[Any], ...]:
+    """Get Optional keys or default.
+
+    Args:
+        data (tomlkit.items.Table): The data to use as source
+        keys (list[str]): The optional keys.
+    """
+    return tuple(data.get(key, default) for key in keys)
+
+
+def read_commands_toml(filename: Union[str, Path]) -> list[CommandGroup]:
+    """Read a commands.toml file and return a list of CommandGroup objects.
+
+    Args:
+        filename (Union[str, Path]): The filename of the commands.toml file.
+
+    Returns:
+        list[CommandGroup]: A list of CommandGroup objects.
+    """
+
+    with open(filename, "r", encoding="utf-8") as toml_file:
+        toml_data = tomlkit.parse(toml_file.read())
+
+    cmd_groups_data = toml_data.get("tool", {}).get("par-run", {})
+    if not cmd_groups_data:
+        raise ValueError("No par-run data found in toml file")
+    _ = cmd_groups_data.get("description", None)
+
+    command_groups = []
+    for group_data in cmd_groups_data.get("groups", []):
+        (group_name,) = _validate_mandatory_keys(group_data, ["name"], "top level par-run group")
+        group_desc, group_timeout, group_retries = _get_optional_keys(
+            group_data, ["desc", "timeout", "retries"], default=None
+        )
+
+        if not group_timeout:
+            group_timeout = 30
+        if not group_retries:
+            group_retries = 3
+
+        commands = OrderedDict()
+        for cmd_data in group_data.get("commands", []):
+            name, exec = _validate_mandatory_keys(cmd_data, ["name", "exec"], f"command group {group_name}")
+            setenv, passenv = _get_optional_keys(cmd_data, ["setenv", "passenv"], default=None)
+
+            commands[name] = Command(name=name, cmd=exec, setenv=setenv, passenv=passenv)
+        command_group = CommandGroup(
+            name=group_name, desc=group_desc, cmds=commands, timeout=group_timeout, retries=group_retries
+        )
+        command_groups.append(command_group)
+
+    return command_groups
+
+
+def run_command(name: str, command: str, setenv: Optional[dict[str, str]], q: Queue) -> None:
     """Run a command and put the output into a queue. The output is a tuple of the command
     name and the output line. The final output is a tuple of the command name and a dictionary
     with the return code.
 
     Args:
-        name (str): Name of the command.
-        command (str): Command to run.
+        name (Command): Command to run.
         q (Queue): Queue to put the output into.
     """
 
+    new_env = None
+    if setenv:
+        new_env = os.environ.copy()
+        new_env.update(setenv)
+
     with subprocess.Popen(
-        f"{command}",
+        command,
         shell=True,
+        env=new_env,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         text=True,
     ) as process:
         if process.stdout:
             for line in iter(process.stdout.readline, ""):
                 q.put((name, line.strip()))
```

### Comparing `par_run-0.1.4/src/par_run/web.py` & `par_run-0.2.0/src/par_run/web.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/src/par_run/static/css/style.css` & `par_run-0.2.0/src/par_run/static/css/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/src/par_run/static/js/app.js` & `par_run-0.2.0/src/par_run/static/js/app.js`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/src/par_run/templates/index.html` & `par_run-0.2.0/src/par_run/templates/index.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/.gitignore` & `par_run-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/LICENSE` & `par_run-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/README.md` & `par_run-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `par_run-0.1.4/PKG-INFO` & `par_run-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: par-run
-Version: 0.1.4
+Version: 0.2.0
 Summary: Parallel command runner
 Project-URL: Homepage, https://github.com/nazq/par-run
 Project-URL: Documentation, https://github.com/nazq/par-run
 Project-URL: Repository, https://github.com/nazq/par-run
 Project-URL: Issues, https://github.com/nazq/par-run/issues
 Project-URL: Changelog, https://github.com/nazq/par-run
 Author-email: Naz Quadri <naz.quadri@gmail.com>
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: rich>=13.0.0
+Requires-Dist: tomlkit>=0.12.4
 Requires-Dist: typer>=0.9.0
 Provides-Extra: web
 Requires-Dist: fastapi>=0.100.0; extra == 'web'
 Requires-Dist: jinja2>=3.0.0; extra == 'web'
 Requires-Dist: psutil>=5.9.0; extra == 'web'
 Requires-Dist: uvicorn[standard]>=0.29.0; extra == 'web'
 Description-Content-Type: text/markdown
```

