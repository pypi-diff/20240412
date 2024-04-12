# Comparing `tmp/par_run-0.2.0.tar.gz` & `tmp/par_run-0.2.1.tar.gz`

## Comparing `par_run-0.2.0.tar` & `par_run-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.2.0/.python-version
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.2.0/commands.ini
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 par_run-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 par_run-0.2.0/requirements.lock
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/coverage_html.js
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046___init___py.html
--rw-r--r--   0        0        0    83748 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046_cli_py.html
--rw-r--r--   0        0        0   134028 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046_executor_py.html
--rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046_web_cli_py.html
--rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/d_417a353b6036f046_web_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/favicon_32.png
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/keybd_open.png
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/status.json
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.2.0/.reports/html/style.css
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 par_run-0.2.0/.vscode/launch.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/conftest.py
--rw-r--r--   0        0        0    14105 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/test_cli.py
--rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/test_executor.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/test_main.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 par_run-0.2.0/py_tests/test_web.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/__init__.py
--rw-r--r--   0        0        0     9370 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/cli.py
--rw-r--r--   0        0        0    14943 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/executor.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/web.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/static/css/style.css
--rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/static/js/app.js
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.2.0/src/par_run/templates/index.html
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.2.0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.2.0/LICENSE
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 par_run-0.2.0/README.md
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 par_run-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 par_run-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.2.1/.python-version
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.2.1/commands.ini
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 par_run-0.2.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 par_run-0.2.1/requirements.lock
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/coverage_html.js
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/d_417a353b6036f046___init___py.html
+-rw-r--r--   0        0        0    88534 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/d_417a353b6036f046_cli_py.html
+-rw-r--r--   0        0        0   134028 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/d_417a353b6036f046_executor_py.html
+-rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/d_417a353b6036f046_web_cli_py.html
+-rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/d_417a353b6036f046_web_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/favicon_32.png
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/keybd_open.png
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.2.1/.reports/html/style.css
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 par_run-0.2.1/.vscode/launch.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 par_run-0.2.1/py_tests/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 par_run-0.2.1/py_tests/conftest.py
+-rw-r--r--   0        0        0    14105 2020-02-02 00:00:00.000000 par_run-0.2.1/py_tests/test_cli.py
+-rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 par_run-0.2.1/py_tests/test_executor.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.2.1/py_tests/test_main.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 par_run-0.2.1/py_tests/test_web.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.2.1/src/par_run/__init__.py
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 par_run-0.2.1/src/par_run/cli.py
+-rw-r--r--   0        0        0    14943 2020-02-02 00:00:00.000000 par_run-0.2.1/src/par_run/executor.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 par_run-0.2.1/src/par_run/web.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.2.1/src/par_run/static/css/style.css
+-rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.2.1/src/par_run/static/js/app.js
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.2.1/src/par_run/templates/index.html
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 par_run-0.2.1/README.md
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 par_run-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 par_run-0.2.1/PKG-INFO
```

### Comparing `par_run-0.2.0/requirements-dev.lock` & `par_run-0.2.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/requirements.lock` & `par_run-0.2.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.reports/html/coverage_html.js` & `par_run-0.2.1/.reports/html/coverage_html.js`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.reports/html/d_417a353b6036f046___init___py.html` & `par_run-0.2.1/.reports/html/d_417a353b6036f046___init___py.html`

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
-            created at 2024-04-10 15:41 -0400
+            created at 2024-04-12 08:48 -0400
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
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.1.4"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.2.0"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-10 15:41 -0400
+            created at 2024-04-12 08:48 -0400
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
-10 15:41 -0400
+12 08:48 -0400
 _1"""Main module for the py_runner package.""" 
 _2 
-_3__version__ = "0.1.4" 
+_3__version__ = "0.2.0" 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-10 15:41 -0400
+12 08:48 -0400
```

### Comparing `par_run-0.2.0/.reports/html/d_417a353b6036f046_cli_py.html` & `par_run-0.2.1/.reports/html/d_417a353b6036f046_cli_py.html`

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
-            <span class="text">172 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">156<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">16<span class="text"> missing</span></button>
+            <span class="text">180 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">163<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">17<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 08:38 -0400
+            created at 2024-04-12 10:21 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -261,126 +261,143 @@
     <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t"><span class="str">    str: The formatted time string.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="nam">hours</span> <span class="op">=</span> <span class="nam">int</span><span class="op">(</span><span class="nam">seconds</span><span class="op">)</span> <span class="op">//</span> <span class="num">3600</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="nam">minutes</span> <span class="op">=</span> <span class="op">(</span><span class="nam">int</span><span class="op">(</span><span class="nam">seconds</span><span class="op">)</span> <span class="op">%</span> <span class="num">3600</span><span class="op">)</span> <span class="op">//</span> <span class="num">60</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="nam">seconds</span> <span class="op">=</span> <span class="nam">seconds</span> <span class="op">%</span> <span class="num">60</span>  <span class="com"># Keeping the fractional part of seconds</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">    <span class="com"># Return formatted string with seconds rounded to 2 d.p.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="key">return</span> <span class="str">f"{hours:02}:{minutes:02}:{seconds:06.2f}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="key">return</span> <span class="str">f"{hours:02}:{minutes:02}:{seconds:06.3f}"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t"><span class="key">def</span> <span class="nam">run</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="nam">style</span><span class="op">:</span> <span class="nam">ProcessingStrategy</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Processing strategy"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="str">"comp"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">    <span class="nam">show</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"Show available groups and commands"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">    <span class="nam">file</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="nam">help</span><span class="op">=</span><span class="str">"The commands.ini file to use"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">Path</span><span class="op">(</span><span class="str">"pyproject.toml"</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="nam">groups</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="key">None</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Run a specific group of commands, comma spearated"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">    <span class="nam">cmds</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="key">None</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Run a specific commands, comma spearated"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">    <span class="str">"""Run commands in parallel"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">    <span class="com"># Overall exit code, need to track all command exit codes to update this</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">    <span class="nam">exit_code</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">    <span class="nam">master_groups</span> <span class="op">=</span> <span class="nam">read_commands_toml</span><span class="op">(</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="key">if</span> <span class="nam">show</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]{cmd.name}[/]: {cmd.cmd}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="key">if</span> <span class="nam">groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">g</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">g</span> <span class="key">in</span> <span class="nam">groups</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">    <span class="key">if</span> <span class="nam">cmds</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">            <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">                <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">                    <span class="nam">cmd_name</span><span class="op">:</span> <span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">                    <span class="key">for</span> <span class="nam">cmd_name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">                    <span class="key">if</span> <span class="nam">cmd_name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">c</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">cmds</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">                <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]No groups or commands found.[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="key">if</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnComp</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="key">elif</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnRecv</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">BadParameter</span><span class="op">(</span><span class="str">"Invalid processing strategy"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">    <span class="com"># Summarise the results</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">        <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">            <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">                <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">                <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">elapsed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">                    <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">f", {format_elapsed_time(cmd.elapsed)}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]Command {cmd.name} succeeded ({cmd.num_non_empty_lines}{elap_str})[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">    <span class="nam">st_all</span> <span class="op">=</span> <span class="nam">time</span><span class="op">.</span><span class="nam">perf_counter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">    <span class="com"># console = rich.console.Console()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="nam">master_groups</span> <span class="op">=</span> <span class="nam">read_commands_toml</span><span class="op">(</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">    <span class="key">if</span> <span class="nam">show</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[green bold]{cmd.name}[/]: {cmd.cmd}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">    <span class="key">if</span> <span class="nam">groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">g</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">g</span> <span class="key">in</span> <span class="nam">groups</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="key">if</span> <span class="nam">cmds</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">        <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">            <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span> <span class="op">=</span> <span class="nam">OrderedDict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">                <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">                    <span class="nam">cmd_name</span><span class="op">:</span> <span class="nam">cmd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">                    <span class="key">for</span> <span class="nam">cmd_name</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">                    <span class="key">if</span> <span class="nam">cmd_name</span> <span class="key">in</span> <span class="op">[</span><span class="nam">c</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">cmds</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">","</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">                <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="nam">master_groups</span> <span class="op">=</span> <span class="op">[</span><span class="nam">grp</span> <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span> <span class="key">if</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]No groups or commands found.[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">        <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="key">if</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_COMP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnComp</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="key">elif</span> <span class="nam">style</span> <span class="op">==</span> <span class="nam">ProcessingStrategy</span><span class="op">.</span><span class="nam">ON_RECV</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">            <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">exit_code</span> <span class="key">or</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">run</span><span class="op">(</span><span class="nam">style</span><span class="op">,</span> <span class="nam">CLICommandCBOnRecv</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">BadParameter</span><span class="op">(</span><span class="str">"Invalid processing strategy"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="com"># Summarise the results</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">    <span class="nam">console</span> <span class="op">=</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">console</span><span class="op">.</span><span class="nam">Console</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">    <span class="key">for</span> <span class="nam">grp</span> <span class="key">in</span> <span class="nam">master_groups</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">        <span class="nam">console</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[blue bold]Group: {grp.name}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">        <span class="key">for</span> <span class="nam">_</span><span class="op">,</span> <span class="nam">cmd</span> <span class="key">in</span> <span class="nam">grp</span><span class="op">.</span><span class="nam">cmds</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">            <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">            <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">elapsed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">f", {format_elapsed_time(cmd.elapsed)}"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"[red bold]Command {cmd.name} failed ({cmd.num_non_empty_lines}{elap_str})[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">                <span class="nam">elap_str</span> <span class="op">=</span> <span class="str">", XX:XX:XX.xxx"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">    <span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">    <span class="key">import</span> <span class="nam">signal</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">    <span class="key">import</span> <span class="nam">subprocess</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">    <span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">    <span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">    <span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">    <span class="key">import</span> <span class="nam">psutil</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]Web commands loaded[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="nam">PID_FILE</span> <span class="op">=</span> <span class="str">".par-run.uvicorn.pid"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">            <span class="key">if</span> <span class="nam">cmd</span><span class="op">.</span><span class="nam">status</span> <span class="op">==</span> <span class="nam">CommandStatus</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">                <span class="nam">left_seg</span> <span class="op">=</span> <span class="str">f"[green bold]Command {cmd.name} succeeded "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">                <span class="nam">left_seg</span> <span class="op">=</span> <span class="str">f"[red bold]Command {cmd.name} failed "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">            <span class="nam">right_seg</span> <span class="op">=</span> <span class="str">f"({cmd.num_non_empty_lines}{elap_str})[/]"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">            <span class="com"># Adjust total line width dynamically based on max width and other content</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">            <span class="nam">pad_length</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">                <span class="num">100</span> <span class="op">-</span> <span class="nam">len</span><span class="op">(</span><span class="nam">left_seg</span><span class="op">)</span> <span class="op">-</span> <span class="nam">len</span><span class="op">(</span><span class="nam">right_seg</span><span class="op">)</span> <span class="op">-</span> <span class="num">10</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">                <span class="key">if</span> <span class="str">"succeeded"</span> <span class="key">in</span> <span class="nam">left_seg</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">                <span class="key">else</span> <span class="num">100</span> <span class="op">-</span> <span class="nam">len</span><span class="op">(</span><span class="nam">left_seg</span><span class="op">)</span> <span class="op">-</span> <span class="nam">len</span><span class="op">(</span><span class="nam">right_seg</span><span class="op">)</span> <span class="op">-</span> <span class="num">12</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">            <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"{left_seg}{' ' * pad_length}{right_seg}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">    <span class="nam">end_style</span> <span class="op">=</span> <span class="str">"[green bold]"</span> <span class="key">if</span> <span class="nam">exit_code</span> <span class="op">==</span> <span class="num">0</span> <span class="key">else</span> <span class="str">"[red bold]"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">f"\n{end_style}Total elapsed time: {format_elapsed_time(time.perf_counter() - st_all)}[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Exit</span><span class="op">(</span><span class="nam">exit_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">    <span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">    <span class="key">def</span> <span class="nam">web</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">        <span class="nam">command</span><span class="op">:</span> <span class="nam">WebCommand</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"command to control/interract with the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">        <span class="nam">port</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="num">8001</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Port to run the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">        <span class="str">"""Run the web server"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">        <span class="key">if</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">START</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STOP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">RESTART</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STATUS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">            <span class="nam">get_web_server_status</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Not a valid command '{command}'"</span><span class="op">,</span> <span class="nam">err</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Abort</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t"><span class="key">except</span> <span class="nam">ImportError</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">    <span class="key">pass</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">    <span class="nam">cli_app</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">    <span class="key">import</span> <span class="nam">signal</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">    <span class="key">import</span> <span class="nam">subprocess</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">    <span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">    <span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">    <span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">    <span class="key">import</span> <span class="nam">psutil</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">    <span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"[blue]Web commands loaded[/]"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">    <span class="nam">PID_FILE</span> <span class="op">=</span> <span class="str">".par-run.uvicorn.pid"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">    <span class="op">@</span><span class="nam">cli_app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">    <span class="key">def</span> <span class="nam">web</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">        <span class="nam">command</span><span class="op">:</span> <span class="nam">WebCommand</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"command to control/interract with the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">        <span class="nam">port</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Option</span><span class="op">(</span><span class="num">8001</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Port to run the web server"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">        <span class="str">"""Run the web server"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">        <span class="key">if</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">START</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STOP</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">RESTART</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">            <span class="nam">stop_web_server</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="nam">start_web_server</span><span class="op">(</span><span class="nam">port</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">        <span class="key">elif</span> <span class="nam">command</span> <span class="op">==</span> <span class="nam">WebCommand</span><span class="op">.</span><span class="nam">STATUS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">            <span class="nam">get_web_server_status</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">            <span class="nam">typer</span><span class="op">.</span><span class="nam">echo</span><span class="op">(</span><span class="str">f"Not a valid command '{command}'"</span><span class="op">,</span> <span class="nam">err</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">            <span class="key">raise</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Abort</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t"><span class="key">except</span> <span class="nam">ImportError</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">    <span class="key">pass</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">    <span class="nam">cli_app</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_417a353b6036f046___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_executor_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 08:38 -0400
+            created at 2024-04-12 10:21 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -4,17 +4,17 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 117722 ssttaatteemmeennttss ?  115566 rruunn 1166 mmiissssiinngg 22 eexxcclluuddeedd **********
+********** 118800 ssttaatteemmeennttss ?  116633 rruunn 1177 mmiissssiinngg 22 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 08:38 -0400
+12 10:21 -0400
 _1"""CLI for running commands in parallel""" 
 _2 
 _3from collections import OrderedDict 
 _4from pathlib import Path 
 _5from typing import Optional 
 _6import enum 
 _7 
@@ -199,15 +199,15 @@
 _1_7_9 str: The formatted time string. 
 _1_8_0 """ 
 _1_8_1 hours = int(seconds) // 3600 
 _1_8_2 minutes = (int(seconds) % 3600) // 60 
 _1_8_3 seconds = seconds % 60 # Keeping the fractional part of seconds 
 _1_8_4 
 _1_8_5 # Return formatted string with seconds rounded to 2 d.p. 
-_1_8_6 return f"{hours:02}:{minutes:02}:{seconds:06.2f}" 
+_1_8_6 return f"{hours:02}:{minutes:02}:{seconds:06.3f}" 
 _1_8_7 
 _1_8_8 
 _1_8_9@cli_app.command() 
 _1_9_0def run( 
 _1_9_1 style: ProcessingStrategy = typer.Option(help="Processing strategy",
 default="comp"), 
 _1_9_2 show: bool = typer.Option(help="Show available groups and commands",
@@ -218,103 +218,119 @@
 commands, comma spearated"), 
 _1_9_5 cmds: Optional[str] = typer.Option(None, help="Run a specific commands,
 comma spearated"), 
 _1_9_6): 
 _1_9_7 """Run commands in parallel""" 
 _1_9_8 # Overall exit code, need to track all command exit codes to update this 
 _1_9_9 exit_code = 0 
-_2_0_0 
-_2_0_1 master_groups = read_commands_toml(file) 
-_2_0_2 if show: 
-_2_0_3 for grp in master_groups: 
-_2_0_4 rich.print(f"[blue bold]Group: {grp.name}[/]") 
-_2_0_5 for _, cmd in grp.cmds.items(): 
-_2_0_6 rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}") 
-_2_0_7 return 
-_2_0_8 
-_2_0_9 if groups: 
-_2_1_0 master_groups = [grp for grp in master_groups if grp.name in [g.strip() for
+_2_0_0 st_all = time.perf_counter() 
+_2_0_1 # console = rich.console.Console() 
+_2_0_2 master_groups = read_commands_toml(file) 
+_2_0_3 if show: 
+_2_0_4 for grp in master_groups: 
+_2_0_5 rich.print(f"[blue bold]Group: {grp.name}[/]") 
+_2_0_6 for _, cmd in grp.cmds.items(): 
+_2_0_7 rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}") 
+_2_0_8 return 
+_2_0_9 
+_2_1_0 if groups: 
+_2_1_1 master_groups = [grp for grp in master_groups if grp.name in [g.strip() for
 g in groups.split(",")]] 
-_2_1_1 
-_2_1_2 if cmds: 
-_2_1_3 for grp in master_groups: 
-_2_1_4 grp.cmds = OrderedDict( 
-_2_1_5 { 
-_2_1_6 cmd_name: cmd 
-_2_1_7 for cmd_name, cmd in grp.cmds.items() 
-_2_1_8 if cmd_name in [c.strip() for c in cmds.split(",")] 
-_2_1_9 } 
-_2_2_0 ) 
-_2_2_1 master_groups = [grp for grp in master_groups if grp.cmds] 
-_2_2_2 
-_2_2_3 if not master_groups: 
-_2_2_4 rich.print("[blue]No groups or commands found.[/]") 
-_2_2_5 raise typer.Exit(0) 
-_2_2_6 
-_2_2_7 for grp in master_groups: 
-_2_2_8 if style == ProcessingStrategy.ON_COMP: 
-_2_2_9 exit_code = exit_code or grp.run(style, CLICommandCBOnComp()) 
-_2_3_0 elif style == ProcessingStrategy.ON_RECV: 
-_2_3_1 exit_code = exit_code or grp.run(style, CLICommandCBOnRecv()) 
-_2_3_2 else: 
-_2_3_3 raise typer.BadParameter("Invalid processing strategy") 
-_2_3_4 
-_2_3_5 # Summarise the results 
-_2_3_6 for grp in master_groups: 
-_2_3_7 rich.print(f"[blue bold]Group: {grp.name}[/]") 
-_2_3_8 for _, cmd in grp.cmds.items(): 
-_2_3_9 if cmd.status == CommandStatus.SUCCESS: 
-_2_4_0 elap_str = "" 
-_2_4_1 if cmd.elapsed: 
-_2_4_2 elap_str = f", {format_elapsed_time(cmd.elapsed)}" 
-_2_4_3 rich.print(f"[green bold]Command {cmd.name} succeeded (
-{cmd.num_non_empty_lines}{elap_str})[/]") 
+_2_1_2 
+_2_1_3 if cmds: 
+_2_1_4 for grp in master_groups: 
+_2_1_5 grp.cmds = OrderedDict( 
+_2_1_6 { 
+_2_1_7 cmd_name: cmd 
+_2_1_8 for cmd_name, cmd in grp.cmds.items() 
+_2_1_9 if cmd_name in [c.strip() for c in cmds.split(",")] 
+_2_2_0 } 
+_2_2_1 ) 
+_2_2_2 master_groups = [grp for grp in master_groups if grp.cmds] 
+_2_2_3 
+_2_2_4 if not master_groups: 
+_2_2_5 rich.print("[blue]No groups or commands found.[/]") 
+_2_2_6 raise typer.Exit(0) 
+_2_2_7 
+_2_2_8 for grp in master_groups: 
+_2_2_9 if style == ProcessingStrategy.ON_COMP: 
+_2_3_0 exit_code = exit_code or grp.run(style, CLICommandCBOnComp()) 
+_2_3_1 elif style == ProcessingStrategy.ON_RECV: 
+_2_3_2 exit_code = exit_code or grp.run(style, CLICommandCBOnRecv()) 
+_2_3_3 else: 
+_2_3_4 raise typer.BadParameter("Invalid processing strategy") 
+_2_3_5 
+_2_3_6 # Summarise the results 
+_2_3_7 console = rich.console.Console() 
+_2_3_8 for grp in master_groups: 
+_2_3_9 console.print(f"[blue bold]Group: {grp.name}[/]") 
+_2_4_0 for _, cmd in grp.cmds.items(): 
+_2_4_1 elap_str = "" 
+_2_4_2 if cmd.elapsed: 
+_2_4_3 elap_str = f", {format_elapsed_time(cmd.elapsed)}" 
 _2_4_4 else: 
-_2_4_5 rich.print(f"[red bold]Command {cmd.name} failed ({cmd.num_non_empty_lines}
-{elap_str})[/]") 
+_2_4_5 elap_str = ", XX:XX:XX.xxx" 
 _2_4_6 
-_2_4_7 raise typer.Exit(exit_code) 
-_2_4_8 
-_2_4_9 
-_2_5_0try: 
-_2_5_1 import os 
-_2_5_2 import signal 
-_2_5_3 import subprocess 
-_2_5_4 import sys 
-_2_5_5 import time 
-_2_5_6 from pathlib import Path 
-_2_5_7 from typing import Optional 
-_2_5_8 
-_2_5_9 import psutil 
-_2_6_0 import typer 
-_2_6_1 
-_2_6_2 rich.print("[blue]Web commands loaded[/]") 
-_2_6_3 
-_2_6_4 PID_FILE = ".par-run.uvicorn.pid" 
+_2_4_7 if cmd.status == CommandStatus.SUCCESS: 
+_2_4_8 left_seg = f"[green bold]Command {cmd.name} succeeded " 
+_2_4_9 else: 
+_2_5_0 left_seg = f"[red bold]Command {cmd.name} failed " 
+_2_5_1 
+_2_5_2 right_seg = f"({cmd.num_non_empty_lines}{elap_str})[/]" 
+_2_5_3 
+_2_5_4 # Adjust total line width dynamically based on max width and other content 
+_2_5_5 pad_length = ( 
+_2_5_6 100 - len(left_seg) - len(right_seg) - 10 
+_2_5_7 if "succeeded" in left_seg 
+_2_5_8 else 100 - len(left_seg) - len(right_seg) - 12 
+_2_5_9 ) 
+_2_6_0 
+_2_6_1 rich.print(f"{left_seg}{' ' * pad_length}{right_seg}") 
+_2_6_2 end_style = "[green bold]" if exit_code == 0 else "[red bold]" 
+_2_6_3 rich.print(f"\n{end_style}Total elapsed time: {format_elapsed_time
+(time.perf_counter() - st_all)}[/]") 
+_2_6_4 raise typer.Exit(exit_code) 
 _2_6_5 
-_2_6_6 @cli_app.command() 
-_2_6_7 def web( 
-_2_6_8 command: WebCommand = typer.Argument(..., help="command to control/
+_2_6_6 
+_2_6_7try: 
+_2_6_8 import os 
+_2_6_9 import signal 
+_2_7_0 import subprocess 
+_2_7_1 import sys 
+_2_7_2 import time 
+_2_7_3 from pathlib import Path 
+_2_7_4 from typing import Optional 
+_2_7_5 
+_2_7_6 import psutil 
+_2_7_7 import typer 
+_2_7_8 
+_2_7_9 rich.print("[blue]Web commands loaded[/]") 
+_2_8_0 
+_2_8_1 PID_FILE = ".par-run.uvicorn.pid" 
+_2_8_2 
+_2_8_3 @cli_app.command() 
+_2_8_4 def web( 
+_2_8_5 command: WebCommand = typer.Argument(..., help="command to control/
 interract with the web server"), 
-_2_6_9 port: int = typer.Option(8001, help="Port to run the web server"), 
-_2_7_0 ): 
-_2_7_1 """Run the web server""" 
-_2_7_2 if command == WebCommand.START: 
-_2_7_3 start_web_server(port) 
-_2_7_4 elif command == WebCommand.STOP: 
-_2_7_5 stop_web_server() 
-_2_7_6 elif command == WebCommand.RESTART: 
-_2_7_7 stop_web_server() 
-_2_7_8 start_web_server(port) 
-_2_7_9 elif command == WebCommand.STATUS: 
-_2_8_0 get_web_server_status() 
-_2_8_1 else: 
-_2_8_2 typer.echo(f"Not a valid command '{command}'", err=True) 
-_2_8_3 raise typer.Abort() 
-_2_8_4 
-_2_8_5except ImportError: # pragma: no cover 
-_2_8_6 pass # pragma: no cover 
-_2_8_7 
-_2_8_8if __name__ == "__main__": 
-_2_8_9 cli_app() 
+_2_8_6 port: int = typer.Option(8001, help="Port to run the web server"), 
+_2_8_7 ): 
+_2_8_8 """Run the web server""" 
+_2_8_9 if command == WebCommand.START: 
+_2_9_0 start_web_server(port) 
+_2_9_1 elif command == WebCommand.STOP: 
+_2_9_2 stop_web_server() 
+_2_9_3 elif command == WebCommand.RESTART: 
+_2_9_4 stop_web_server() 
+_2_9_5 start_web_server(port) 
+_2_9_6 elif command == WebCommand.STATUS: 
+_2_9_7 get_web_server_status() 
+_2_9_8 else: 
+_2_9_9 typer.echo(f"Not a valid command '{command}'", err=True) 
+_3_0_0 raise typer.Abort() 
+_3_0_1 
+_3_0_2except ImportError: # pragma: no cover 
+_3_0_3 pass # pragma: no cover 
+_3_0_4 
+_3_0_5if __name__ == "__main__": 
+_3_0_6 cli_app() 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-12 08:38 -0400
+12 10:21 -0400
```

### Comparing `par_run-0.2.0/.reports/html/d_417a353b6036f046_executor_py.html` & `par_run-0.2.1/.reports/html/d_417a353b6036f046_executor_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.reports/html/d_417a353b6036f046_web_cli_py.html` & `par_run-0.2.1/.reports/html/d_417a353b6036f046_web_cli_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.reports/html/d_417a353b6036f046_web_py.html` & `par_run-0.2.1/.reports/html/d_417a353b6036f046_web_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.reports/html/favicon_32.png` & `par_run-0.2.1/.reports/html/favicon_32.png`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.reports/html/index.html` & `par_run-0.2.1/.reports/html/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-12 08:39 -0400
+            created at 2024-04-12 10:21 -0400
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -66,18 +66,18 @@
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_417a353b6036f046_cli_py.html">src/par_run/cli.py</a></td>
-                <td>172</td>
-                <td>16</td>
+                <td>180</td>
+                <td>17</td>
                 <td>2</td>
-                <td class="right" data-ratio="156 172">91%</td>
+                <td class="right" data-ratio="163 180">91%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_417a353b6036f046_executor_py.html">src/par_run/executor.py</a></td>
                 <td>251</td>
                 <td>38</td>
                 <td>7</td>
                 <td class="right" data-ratio="213 251">85%</td>
@@ -89,30 +89,30 @@
                 <td>0</td>
                 <td class="right" data-ratio="29 41">71%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>465</td>
-                <td>66</td>
+                <td>473</td>
+                <td>67</td>
                 <td>9</td>
-                <td class="right" data-ratio="399 465">86%</td>
+                <td class="right" data-ratio="406 473">86%</td>
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
-            created at 2024-04-12 08:39 -0400
+            created at 2024-04-12 10:21 -0400
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
 ************ CCoovveerraaggee rreeppoorrtt:: 8866%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-12 08:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-12 10:21 -0400
 MMoodduullee                  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _s_r_c_/_p_a_r___r_u_n_/_____i_n_i_t_____._p_y 1          0       0        100%
-_s_r_c_/_p_a_r___r_u_n_/_c_l_i_._p_y      172        16      2        91%
+_s_r_c_/_p_a_r___r_u_n_/_c_l_i_._p_y      180        17      2        91%
 _s_r_c_/_p_a_r___r_u_n_/_e_x_e_c_u_t_o_r_._p_y 251        38      7        85%
 _s_r_c_/_p_a_r___r_u_n_/_w_e_b_._p_y      41         12      0        71%
-Total                   465        66      9        86%
+Total                   473        67      9        86%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-12 08:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-12 10:21 -0400
```

### Comparing `par_run-0.2.0/.reports/html/keybd_closed.png` & `par_run-0.2.1/.reports/html/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.reports/html/keybd_open.png` & `par_run-0.2.1/.reports/html/keybd_open.png`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.reports/html/status.json` & `par_run-0.2.1/.reports/html/status.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9948333333333335%*

 * *Differences: {"'files'": "{'d_417a353b6036f046___init___py': {'hash': '2acd0f3f7d187411f827058d2663ad25'}, "*

 * *            "'d_417a353b6036f046_cli_py': {'hash': '0ccfe317a36b4e9ad5cd9d8c055c4c9e', 'index': "*

 * *            "{'nums': {insert: [(2, 180), (4, 17)], delete: [4, 2]}}}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_417a353b6036f046___init___py": {
-            "hash": "f446efc7ead065ed9673c74ed99bd8b3",
+            "hash": "2acd0f3f7d187411f827058d2663ad25",
             "index": {
                 "html_filename": "d_417a353b6036f046___init___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -14,23 +14,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/__init__.py"
             }
         },
         "d_417a353b6036f046_cli_py": {
-            "hash": "1fb428d04dbdd753b2a6e2b27de6395d",
+            "hash": "0ccfe317a36b4e9ad5cd9d8c055c4c9e",
             "index": {
                 "html_filename": "d_417a353b6036f046_cli_py.html",
                 "nums": [
                     0,
                     1,
-                    172,
+                    180,
                     2,
-                    16,
+                    17,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/par_run/cli.py"
             }
         },
```

### Comparing `par_run-0.2.0/.reports/html/style.css` & `par_run-0.2.1/.reports/html/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.vscode/launch.json` & `par_run-0.2.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/py_tests/conftest.py` & `par_run-0.2.1/py_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/py_tests/test_cli.py` & `par_run-0.2.1/py_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/py_tests/test_executor.py` & `par_run-0.2.1/py_tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/py_tests/test_web.py` & `par_run-0.2.1/py_tests/test_web.py`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/src/par_run/cli.py` & `par_run-0.2.1/src/par_run/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -179,29 +179,30 @@
     str: The formatted time string.
     """
     hours = int(seconds) // 3600
     minutes = (int(seconds) % 3600) // 60
     seconds = seconds % 60  # Keeping the fractional part of seconds
 
     # Return formatted string with seconds rounded to 2 d.p.
-    return f"{hours:02}:{minutes:02}:{seconds:06.2f}"
+    return f"{hours:02}:{minutes:02}:{seconds:06.3f}"
 
 
 @cli_app.command()
 def run(
     style: ProcessingStrategy = typer.Option(help="Processing strategy", default="comp"),
     show: bool = typer.Option(help="Show available groups and commands", default=False),
     file: Path = typer.Option(help="The commands.ini file to use", default=Path("pyproject.toml")),
     groups: Optional[str] = typer.Option(None, help="Run a specific group of commands, comma spearated"),
     cmds: Optional[str] = typer.Option(None, help="Run a specific commands, comma spearated"),
 ):
     """Run commands in parallel"""
     # Overall exit code, need to track all command exit codes to update this
     exit_code = 0
-
+    st_all = time.perf_counter()
+    # console = rich.console.Console()
     master_groups = read_commands_toml(file)
     if show:
         for grp in master_groups:
             rich.print(f"[blue bold]Group: {grp.name}[/]")
             for _, cmd in grp.cmds.items():
                 rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}")
         return
@@ -229,25 +230,41 @@
             exit_code = exit_code or grp.run(style, CLICommandCBOnComp())
         elif style == ProcessingStrategy.ON_RECV:
             exit_code = exit_code or grp.run(style, CLICommandCBOnRecv())
         else:
             raise typer.BadParameter("Invalid processing strategy")
 
     # Summarise the results
+    console = rich.console.Console()
     for grp in master_groups:
-        rich.print(f"[blue bold]Group: {grp.name}[/]")
+        console.print(f"[blue bold]Group: {grp.name}[/]")
         for _, cmd in grp.cmds.items():
+            elap_str = ""
+            if cmd.elapsed:
+                elap_str = f", {format_elapsed_time(cmd.elapsed)}"
+            else:
+                elap_str = ", XX:XX:XX.xxx"
+
             if cmd.status == CommandStatus.SUCCESS:
-                elap_str = ""
-                if cmd.elapsed:
-                    elap_str = f", {format_elapsed_time(cmd.elapsed)}"
-                rich.print(f"[green bold]Command {cmd.name} succeeded ({cmd.num_non_empty_lines}{elap_str})[/]")
+                left_seg = f"[green bold]Command {cmd.name} succeeded "
             else:
-                rich.print(f"[red bold]Command {cmd.name} failed ({cmd.num_non_empty_lines}{elap_str})[/]")
+                left_seg = f"[red bold]Command {cmd.name} failed "
+
+            right_seg = f"({cmd.num_non_empty_lines}{elap_str})[/]"
+
+            # Adjust total line width dynamically based on max width and other content
+            pad_length = (
+                100 - len(left_seg) - len(right_seg) - 10
+                if "succeeded" in left_seg
+                else 100 - len(left_seg) - len(right_seg) - 12
+            )
 
+            rich.print(f"{left_seg}{' ' * pad_length}{right_seg}")
+    end_style = "[green bold]" if exit_code == 0 else "[red bold]"
+    rich.print(f"\n{end_style}Total elapsed time: {format_elapsed_time(time.perf_counter() - st_all)}[/]")
     raise typer.Exit(exit_code)
 
 
 try:
     import os
     import signal
     import subprocess
```

### Comparing `par_run-0.2.0/src/par_run/executor.py` & `par_run-0.2.1/src/par_run/executor.py`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/src/par_run/web.py` & `par_run-0.2.1/src/par_run/web.py`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/src/par_run/static/css/style.css` & `par_run-0.2.1/src/par_run/static/css/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/src/par_run/static/js/app.js` & `par_run-0.2.1/src/par_run/static/js/app.js`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/src/par_run/templates/index.html` & `par_run-0.2.1/src/par_run/templates/index.html`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/.gitignore` & `par_run-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/LICENSE` & `par_run-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `par_run-0.2.0/pyproject.toml` & `par_run-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "par-run"
-version = "0.2.0"
+version = "0.2.1"
 description = "Parallel command runner"
 license = "MIT"
 authors = [
     { name = "Naz Quadri", email = "naz.quadri@gmail.com" }
 ]
 classifiers = [
     'Development Status :: 4 - Beta',
@@ -75,15 +75,15 @@
 packages = [
     "src/par_run",
     "static",
     "templates",
 ]
 
 [tool.bumpversion]
-current_version = "0.2.0"
+current_version = "0.2.1"
 commit = true
 tag = true
 tag_name = "{new_version}"
 tag_message = "Version {new_version}"
 message = "Bump version: {current_version} → {new_version}"
 allow_dirty = true
 parse = """(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"""
@@ -155,15 +155,15 @@
 [[tool.par-run.groups]]
 name = "ENV"
 desc = "Code Quality Tools. No code mutation"
 timeout = 5
 retries = 3
 
   [[tool.par-run.groups.commands]]
-  name = "my_var"
-  exec = "echo \"MY_VAR=$MY_VAR\""
+  name = "full_env"
+  exec = "env"
   setenv = {MY_VAR = "production", ENABLE_LOGS = "true"}
 
   [[tool.par-run.groups.commands]]
-  name = "full_env"
-  exec = "env"
-  setenv = {MY_VAR = "production", ENABLE_LOGS = "true"}
+  name = "my_var"
+  exec = "echo \"MY_VAR=$MY_VAR\", \"ENABLE_LOGS=$ENABLE_LOGS\""
+  setenv = {MY_VAR = "production", ENABLE_LOGS = "true"}
```

