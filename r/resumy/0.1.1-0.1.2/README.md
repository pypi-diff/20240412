# Comparing `tmp/resumy-0.1.1.tar.gz` & `tmp/resumy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resumy-0.1.1.tar", last modified: Thu Sep 15 16:02:59 2022, max compression
+gzip compressed data, was "resumy-0.1.2.tar", last modified: Fri Apr 12 13:22:46 2024, max compression
```

## Comparing `resumy-0.1.1.tar` & `resumy-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.904892 resumy-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.900891 resumy-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.904892 resumy-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-09-15 16:02:30.000000 resumy-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-09-15 16:02:30.000000 resumy-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.904892 resumy-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-09-15 16:02:30.000000 resumy-0.1.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-09-15 16:02:30.000000 resumy-0.1.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-15 16:02:30.000000 resumy-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-09-15 16:02:30.000000 resumy-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-15 16:02:30.000000 resumy-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4675 2022-09-15 16:02:59.904892 resumy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-09-15 16:02:30.000000 resumy-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.904892 resumy-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)   248118 2022-09-15 16:02:30.000000 resumy-0.1.1/docs/demo.png
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-15 16:02:30.000000 resumy-0.1.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-09-15 16:02:30.000000 resumy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 16:02:59.904892 resumy-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.900891 resumy-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.904892 resumy-0.1.1/src/resumy/
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/config.example.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    12905 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/resumy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.904892 resumy-0.1.1/src/resumy/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)    11368 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/schemas/jsonresume.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4870 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/schemas/resumy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.900891 resumy-0.1.1/src/resumy/themes/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.904892 resumy-0.1.1/src/resumy/themes/prairie/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.904892 resumy-0.1.1/src/resumy/themes/prairie/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    63920 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/themes/prairie/fonts/Roboto-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    63692 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/themes/prairie/fonts/Roboto-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/themes/prairie/fonts/prairie.woff2
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/themes/prairie/icons.css
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/themes/prairie/theme.css
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-09-15 16:02:30.000000 resumy-0.1.1/src/resumy/themes/prairie/theme.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:02:59.904892 resumy-0.1.1/src/resumy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4675 2022-09-15 16:02:59.000000 resumy-0.1.1/src/resumy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-09-15 16:02:59.000000 resumy-0.1.1/src/resumy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 16:02:59.000000 resumy-0.1.1/src/resumy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-15 16:02:59.000000 resumy-0.1.1/src/resumy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-15 16:02:59.000000 resumy-0.1.1/src/resumy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-15 16:02:59.000000 resumy-0.1.1/src/resumy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-09-15 16:02:30.000000 resumy-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.074759 resumy-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.066758 resumy-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.070758 resumy-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-12 13:22:34.000000 resumy-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-12 13:22:34.000000 resumy-0.1.2/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.070758 resumy-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-12 13:22:34.000000 resumy-0.1.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-12 13:22:34.000000 resumy-0.1.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 13:22:34.000000 resumy-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 13:22:34.000000 resumy-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-12 13:22:34.000000 resumy-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-12 13:22:46.074759 resumy-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-12 13:22:34.000000 resumy-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.070758 resumy-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)   248118 2024-04-12 13:22:34.000000 resumy-0.1.2/docs/demo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 13:22:34.000000 resumy-0.1.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-12 13:22:34.000000 resumy-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:22:46.074759 resumy-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.070758 resumy-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.070758 resumy-0.1.2/src/resumy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/config.example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/resumy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.074759 resumy-0.1.2/src/resumy/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/schemas/jsonresume.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/schemas/resumy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.070758 resumy-0.1.2/src/resumy/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.074759 resumy-0.1.2/src/resumy/themes/prairie/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.074759 resumy-0.1.2/src/resumy/themes/prairie/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    63920 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/themes/prairie/fonts/Roboto-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63692 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/themes/prairie/fonts/Roboto-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/themes/prairie/fonts/prairie.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/themes/prairie/icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/themes/prairie/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-12 13:22:34.000000 resumy-0.1.2/src/resumy/themes/prairie/theme.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:22:46.074759 resumy-0.1.2/src/resumy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-12 13:22:46.000000 resumy-0.1.2/src/resumy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-12 13:22:46.000000 resumy-0.1.2/src/resumy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:22:46.000000 resumy-0.1.2/src/resumy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 13:22:46.000000 resumy-0.1.2/src/resumy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 13:22:46.000000 resumy-0.1.2/src/resumy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 13:22:46.000000 resumy-0.1.2/src/resumy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-12 13:22:34.000000 resumy-0.1.2/tox.ini
```

### Comparing `resumy-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `resumy-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `resumy-0.1.2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/.github/workflows/release.yaml` & `resumy-0.1.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/.github/workflows/tests.yaml` & `resumy-0.1.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/LICENSE` & `resumy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/PKG-INFO` & `resumy-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resumy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Resume builder
 Author-email: Alex Laurent <alex@i42.sh>
 License: MIT License
         
         Copyright (c) 2022 Alex Laurent
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,14 +27,18 @@
         
 Project-URL: homepage, https://github.com/alexlren/resumy
 Keywords: resume,cv
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML==6.0
+Requires-Dist: Jinja2>=3.1.2
+Requires-Dist: weasyprint>=56.1
+Requires-Dist: jsonschema>=4.16.0
 
 # resumy
 
 [![PyPI version](https://badge.fury.io/py/resumy.svg)](https://badge.fury.io/py/resumy)
 ![build status](https://github.com/alexlren/estel_secp256k1/actions/workflows/ci.yaml/badge.svg)
 
 <img src="/docs/demo.png" width="300"/>
@@ -51,14 +55,18 @@
 
 ```
 pip install resumy
 ```
 
 **It may not work out of the box as some external dynamic libraries are necessary depending on your platform, please take a look at the weasyprint documentation page: https://doc.courtbouillon.org/weasyprint/stable/first_steps.html**
 
+## CI
+
+An easy way to create your resume is to host your yaml file in a git repository and build it automatically + host it somewhere each time you push new changes. You can fork [resumy_workflow](https://github.com/alexlren/resumy_workflow) for an example on github.
+
 ## Commands
 
 ### Usage
 
 ```
 resumy --help
 ```
@@ -121,15 +129,15 @@
 ```
 resumy build -o myresume.pdf myconfig.yaml
 ```
 
 ### Create and use your own theme
 
 ```
-resumy theme mytheme -o /tmp/mytheme
+resumy theme -o /tmp/mytheme
 ```
 
 Now you can simply edit /tmp/mytheme/theme.html and /tmp/mytheme/theme.css, and use your custom theme with `--theme` option.
 
 ```
 resumy build -o myresume.pdf --theme /tmp/mytheme myconfig.yaml
 ```
```

### Comparing `resumy-0.1.1/README.md` & `resumy-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 ```
 pip install resumy
 ```
 
 **It may not work out of the box as some external dynamic libraries are necessary depending on your platform, please take a look at the weasyprint documentation page: https://doc.courtbouillon.org/weasyprint/stable/first_steps.html**
 
+## CI
+
+An easy way to create your resume is to host your yaml file in a git repository and build it automatically + host it somewhere each time you push new changes. You can fork [resumy_workflow](https://github.com/alexlren/resumy_workflow) for an example on github.
+
 ## Commands
 
 ### Usage
 
 ```
 resumy --help
 ```
@@ -87,15 +91,15 @@
 ```
 resumy build -o myresume.pdf myconfig.yaml
 ```
 
 ### Create and use your own theme
 
 ```
-resumy theme mytheme -o /tmp/mytheme
+resumy theme -o /tmp/mytheme
 ```
 
 Now you can simply edit /tmp/mytheme/theme.html and /tmp/mytheme/theme.css, and use your custom theme with `--theme` option.
 
 ```
 resumy build -o myresume.pdf --theme /tmp/mytheme myconfig.yaml
 ```
```

### Comparing `resumy-0.1.1/docs/demo.png` & `resumy-0.1.2/docs/demo.png`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/pyproject.toml` & `resumy-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/src/resumy/config.example.yaml` & `resumy-0.1.2/src/resumy/config.example.yaml`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/src/resumy/resumy.py` & `resumy-0.1.2/src/resumy/resumy.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,23 @@
 
 def create_resume(config: Yaml,
                   output_file: str,
                   theme_path: str,
                   metadata: DocumentMetadata) -> None:
     # 1. Retrieve theme
     env = jinja2.Environment(
-        loader=jinja2.FileSystemLoader('/'),
+        loader=jinja2.FileSystemLoader(theme_path),
     )
     try:
-        template = env.get_template(f'{theme_path}/theme.html')
+        template = env.get_template('theme.html')
     except jinja2.exceptions.TemplateNotFound as err:
         raise IOError(f"No such file or directory: '{err}'")
 
     # 2. Create a html from both the theme and the config file
-    html_resume = template.render(config)
+    html_resume = template.render(config, strptime=datetime.strptime)
 
     # 3. Add css automatically
     css_list = []
     theme_lsdir = os.listdir(theme_path)
     for theme_file in theme_lsdir:
         [_, ext] = os.path.splitext(theme_file)
         if ext != '.css':
```

### Comparing `resumy-0.1.1/src/resumy/schemas/jsonresume.yaml` & `resumy-0.1.2/src/resumy/schemas/jsonresume.yaml`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/src/resumy/schemas/resumy.yaml` & `resumy-0.1.2/src/resumy/schemas/resumy.yaml`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/src/resumy/themes/prairie/fonts/Roboto-Bold.woff2` & `resumy-0.1.2/src/resumy/themes/prairie/fonts/Roboto-Bold.woff2`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/src/resumy/themes/prairie/fonts/Roboto-Regular.woff2` & `resumy-0.1.2/src/resumy/themes/prairie/fonts/Roboto-Regular.woff2`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/src/resumy/themes/prairie/fonts/prairie.woff2` & `resumy-0.1.2/src/resumy/themes/prairie/fonts/prairie.woff2`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/src/resumy/themes/prairie/icons.css` & `resumy-0.1.2/src/resumy/themes/prairie/icons.css`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/src/resumy/themes/prairie/theme.css` & `resumy-0.1.2/src/resumy/themes/prairie/theme.css`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/src/resumy/themes/prairie/theme.html` & `resumy-0.1.2/src/resumy/themes/prairie/theme.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+{%- macro format_str_date(str_date) -%}
+{{ strptime(str_date, '%Y-%m-%d').strftime('%b %Y') }}
+{%- endmacro -%}
+
 {%- macro format_date_range(exp) -%}
-{{ exp.startDate }} - {% if exp.endDate %}{{ exp.endDate }}{% else %}Present{% endif %}
+{{ format_str_date(exp.startDate) }} - {% if exp.endDate %}{{ format_str_date(exp.endDate) }}{% else %}Present{% endif %}
 {%- endmacro -%}
 
 <h1>{{ basics.name }}</h1>
 {% if basics.label %}
 <p>{{ basics.label }}</p>
 {% endif %}
 <ul class="header">
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
-{%- macro format_date_range(exp) -%} {{ exp.startDate }} - {% if exp.endDate %}
-{{ exp.endDate }}{% else %}Present{% endif %} {%- endmacro -%}
+{%- macro format_str_date(str_date) -%} {{ strptime(str_date, '%Y-%m-
+%d').strftime('%b %Y') }} {%- endmacro -%} {%- macro format_date_range(exp) -%}
+{{ format_str_date(exp.startDate) }} - {% if exp.endDate %}{{ format_str_date
+(exp.endDate) }}{% else %}Present{% endif %} {%- endmacro -%}
 ************ {{{{ bbaassiiccss..nnaammee }}}} ************
 {% if basics.label %}
 {{ basics.label }}
 {% endif %}
     * {% if basics.phone %}
     * {{ basics.phone }}
     * {% endif %} {% if basics.email %}
```

### Comparing `resumy-0.1.1/src/resumy.egg-info/PKG-INFO` & `resumy-0.1.2/src/resumy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resumy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Resume builder
 Author-email: Alex Laurent <alex@i42.sh>
 License: MIT License
         
         Copyright (c) 2022 Alex Laurent
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,14 +27,18 @@
         
 Project-URL: homepage, https://github.com/alexlren/resumy
 Keywords: resume,cv
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML==6.0
+Requires-Dist: Jinja2>=3.1.2
+Requires-Dist: weasyprint>=56.1
+Requires-Dist: jsonschema>=4.16.0
 
 # resumy
 
 [![PyPI version](https://badge.fury.io/py/resumy.svg)](https://badge.fury.io/py/resumy)
 ![build status](https://github.com/alexlren/estel_secp256k1/actions/workflows/ci.yaml/badge.svg)
 
 <img src="/docs/demo.png" width="300"/>
@@ -51,14 +55,18 @@
 
 ```
 pip install resumy
 ```
 
 **It may not work out of the box as some external dynamic libraries are necessary depending on your platform, please take a look at the weasyprint documentation page: https://doc.courtbouillon.org/weasyprint/stable/first_steps.html**
 
+## CI
+
+An easy way to create your resume is to host your yaml file in a git repository and build it automatically + host it somewhere each time you push new changes. You can fork [resumy_workflow](https://github.com/alexlren/resumy_workflow) for an example on github.
+
 ## Commands
 
 ### Usage
 
 ```
 resumy --help
 ```
@@ -121,15 +129,15 @@
 ```
 resumy build -o myresume.pdf myconfig.yaml
 ```
 
 ### Create and use your own theme
 
 ```
-resumy theme mytheme -o /tmp/mytheme
+resumy theme -o /tmp/mytheme
 ```
 
 Now you can simply edit /tmp/mytheme/theme.html and /tmp/mytheme/theme.css, and use your custom theme with `--theme` option.
 
 ```
 resumy build -o myresume.pdf --theme /tmp/mytheme myconfig.yaml
 ```
```

### Comparing `resumy-0.1.1/src/resumy.egg-info/SOURCES.txt` & `resumy-0.1.2/src/resumy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resumy-0.1.1/tox.ini` & `resumy-0.1.2/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -2,36 +2,33 @@
 srcdir = src/resumy
 
 [tox]
 minversion = 3.20.1
 envlist = py38
 
 [testenv]
-basepython = python3
 skip_install = true
 deps =
     {[testenv:flake8]deps}
     {[testenv:mypy]deps}
 commands =
     {[testenv:flake8]commands}
     {[testenv:mypy]commands}
 
 [testenv:mypy]
-basepython = python3
 skip_install = true
 deps =
     mypy
     types-PyYAML
     types-Jinja2
     types-jsonschema
 commands =
     mypy {[main]srcdir} --strict
 
 [testenv:flake8]
-basepython = python3
 skip_install = true
 deps =
     flake8
     flake8-colors
     flake8-commas
     flake8-isort
     flake8-print
@@ -43,15 +40,14 @@
 basepython = python3
 skip_install = true
 deps = build
 commands =
     python -m build
 
 [testenv:release]
-basepython = python3
 skip_install = true
 passenv = TWINE_*
 deps =
     {[testenv:build]deps}
     twine >= 1.5.0
 commands =
     {[testenv:build]commands}
```

