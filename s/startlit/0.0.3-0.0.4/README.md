# Comparing `tmp/startlit-0.0.3.tar.gz` & `tmp/startlit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "startlit-0.0.3.tar", max compression
+gzip compressed data, was "startlit-0.0.4.tar", max compression
```

## Comparing `startlit-0.0.3.tar` & `startlit-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-11 11:57:07.782928 startlit-0.0.3/LICENSE
--rw-r--r--   0        0        0     3441 2024-04-11 11:57:07.782928 startlit-0.0.3/README.md
--rw-r--r--   0        0        0      520 2024-04-11 11:57:07.782928 startlit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      137 2024-04-11 11:57:07.782928 startlit-0.0.3/src/startlit/__init__.py
--rw-r--r--   0        0        0      582 2024-04-11 11:57:07.782928 startlit-0.0.3/src/startlit/kill.py
--rw-r--r--   0        0        0     2323 2024-04-11 11:57:07.782928 startlit-0.0.3/src/startlit/list.py
--rw-r--r--   0        0        0     2903 2024-04-11 11:57:07.782928 startlit-0.0.3/src/startlit/start.py
--rw-r--r--   0        0        0     4090 1970-01-01 00:00:00.000000 startlit-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 16:07:54.315094 startlit-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3473 2024-04-12 16:07:54.315094 startlit-0.0.4/README.md
+-rw-r--r--   0        0        0      520 2024-04-12 16:07:54.315094 startlit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-04-12 16:07:54.315094 startlit-0.0.4/src/startlit/__init__.py
+-rw-r--r--   0        0        0      899 2024-04-12 16:07:54.315094 startlit-0.0.4/src/startlit/help.py
+-rw-r--r--   0        0        0      582 2024-04-12 16:07:54.315094 startlit-0.0.4/src/startlit/kill.py
+-rw-r--r--   0        0        0     2323 2024-04-12 16:07:54.315094 startlit-0.0.4/src/startlit/list.py
+-rw-r--r--   0        0        0     3218 2024-04-12 16:07:54.315094 startlit-0.0.4/src/startlit/start.py
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 startlit-0.0.4/PKG-INFO
```

### Comparing `startlit-0.0.3/LICENSE` & `startlit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `startlit-0.0.3/README.md` & `startlit-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # StartLit ⭐
-![PyPI - Version](https://img.shields.io/pypi/v/startlit) ![GitHub repo size](https://img.shields.io/github/repo-size/ineelhere/startlit) ![GitHub License](https://img.shields.io/github/license/ineelhere/startlit) ![example workflow](https://github.com/ineelhere/startlit/actions/workflows/python-publish.yml/badge.svg) 
+![PyPI - Version](https://img.shields.io/pypi/v/startlit?style=plastic) ![GitHub License](https://img.shields.io/github/license/ineelhere/startlit?style=plastic) ![PyPI - Downloads](https://img.shields.io/pypi/dm/startLit?style=plastic&logoColor=blue&color=blue) ![example workflow](https://github.com/ineelhere/startlit/actions/workflows/python-publish.yml/badge.svg?style=plastic) 
 
 **Welcome to StartLit!**
 
 StartLit is your gateway to building Streamlit apps with ease. It brings a simple, streamlined way to start your Streamlit projects. Here's what's included in the latest release:
 
 #### Features:
 - **Package Installation**: Now you can easily install StartLit from PYPI using `pip install startlit`.
-- **Simple Usage**: Import the package and run `hello()` to receive a friendly welcome message.
-- **Basic help**: Use the `help()` function to get started with more support
--  **Starter App**: Use the `starter()` function to download a very simple starter app template, including an `app.py` file and a `requirements.txt` file.
--  **Multipage App**: Use the `multipage()` function to download an app template for building multipage Streamlit apps. The files/folders will be available in your working directory.
--  **Fragments App**: Use the `fragments()` function to download an app that allows you to run independent components in the streamlit app.
--  **List active streamlit apps** - Use the `list_streamlit_apps()` function to get a list of currently running
--  **Kill active streamlit apps** - Use the `kill_streamlit_apps(app_id)` function to kill desired running streamlit apps. `app_id` is the app ID you get from the `list_streamlit_apps()` function.
+
+* 🤗 `hello()` - Just a welcome text. 
+* 📥 `starter()` - A very simple starter app template. Quick-peek: https://startlit-starter.streamlit.app/
+* 📃 `multipage()` - An app template for building multipage Streamlit apps. Quick-peek: https://startlit-multipage.streamlit.app/
+* 📚 `fragments()` - An app that allows you to run independent components in the streamlit app. Quick-peek: https://startlit-fragments.streamlit.app/
+* 💬 `chat()`- A dummy chatbot app. Quick-peek: https://startlit-chat.streamlit.app/
+* 📜 `list_streamlit_apps()` - List running Streamlit apps.
+* 🔪 `kill_streamlit_apps()` - Kill running Streamlit apps.
+* 💡 `help()` - Display help menu with list of available functions.
+* 🐙 Need more help? Post an issue at https://github.com/ineelhere/startlit/issues
 
 ### Install the package from PYPI
 
 ```python
 pip install startlit
 ```
 ### Import the package
@@ -83,28 +86,30 @@
 
 # Download a multipage app template
 multipage()
 
 # Download a fragment app template
 fragments()
 
+# Download a dummy chatbot app template
+chat()
+
 # List all active apps
 list_streamlit_apps()
 
-# Kill a specific app
+# Kill a specific app by app_id
 kill_streamlit_apps(app_id)
-
-
 ```
 ___
 
 ### Feedback and Contribution:
-Excited to hear your feedback and suggestions for improvements. 
+Excited to hear your feedback and suggestions for improvements.
+
+Collaborations and Contributions are welcome 🤝
 Feel free to open issues or submit pull requests.
 
 Enjoy your streamlit journey with StartLit and happy coding! 🚀🎉
+
+*Check package download stats at https://pypistats.org/packages/startlit*
 ___
 
 **© `Indraneel Chakraborty` | 2024** 🧑‍💻[LinkedIn](https://www.linkedin.com/in/indraneelchakraborty/) | [X/Twitter](https://twitter.com/ineelhere)
-
-
-`Collaborations and Contributions are welcome 🤝`
```

### Comparing `startlit-0.0.3/pyproject.toml` & `startlit-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "startlit"
-version = "0.0.3"
+version = "0.0.4"
 description = "Get started with a streamlit app template code in style"
 authors = ["Indraneel Chakraborty"]
 readme = "README.md"
 homepage = "https://github.com/ineelhere/startlit"
 license = "Apache License - Version 2.0"
 
 [tool.poetry.dependencies]
```

### Comparing `startlit-0.0.3/src/startlit/kill.py` & `startlit-0.0.4/src/startlit/kill.py`

 * *Files identical despite different names*

### Comparing `startlit-0.0.3/src/startlit/list.py` & `startlit-0.0.4/src/startlit/list.py`

 * *Files identical despite different names*

### Comparing `startlit-0.0.3/src/startlit/start.py` & `startlit-0.0.4/src/startlit/start.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,14 @@
 def hello():
     """
     A function that prints a greeting message to the console.
     No parameters required.
     """
     print("Hello there 👋 \nWelcome to Startlit! 🚀")
 
-def help():
-    """
-    A function that prints a list of available commands to the console.
-    """
-    print("Available commands:\n🤗 hello()\n📥 starter()\n📥 multipage()\n📚 fragments()\n🐙 Need more help? Post an issue at https://github.com/ineelhere/startlit/issues")
-
 def starter():
     """
     A function to download the starter app files from a specified URL and print a confirmation message.
     """
     urllib.request.urlretrieve("https://raw.githubusercontent.com/ineelhere/startlit/starter/app.py", "app.py")
     urllib.request.urlretrieve("https://raw.githubusercontent.com/ineelhere/startlit/starter/requirements.txt", "requirements.txt")
     print("📥 Starter app downloaded!📥\n👀 Look for 'app.py' and 'requirements.txt' file in your working directory 👀")
@@ -41,7 +35,16 @@
     """
     A function to download the fragments app files from a specified URL and print a confirmation message.
     """
     urllib.request.urlretrieve("https://raw.githubusercontent.com/ineelhere/startlit/fragments/app.py", "app.py")
     urllib.request.urlretrieve("https://raw.githubusercontent.com/ineelhere/startlit/starter/requirements.txt", "requirements.txt")
     print("📥 Fragments app downloaded!📥\n👀 Look for 'app.py' and 'requirements.txt' file in your working directory 👀")
     print("💡 Visit https://startlit-fragments.streamlit.app/ for a quick look to the deployed app")
+
+def chat():
+    """
+    A function to download a simple dummy chat app from a specified URL and print a confirmation message.
+    """
+    urllib.request.urlretrieve("https://raw.githubusercontent.com/ineelhere/startlit/chat/app.py", "app.py")
+    urllib.request.urlretrieve("https://raw.githubusercontent.com/ineelhere/startlit/starter/requirements.txt", "requirements.txt")
+    print("📥 Chat app downloaded!📥\n👀 Look for 'app.py' and 'requirements.txt' file in your working directory 👀")
+    print("💡 Visit https://startlit-chat.streamlit.app/ for a quick look to the deployed app")
```

### Comparing `startlit-0.0.3/PKG-INFO` & `startlit-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: startlit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Get started with a streamlit app template code in style
 Home-page: https://github.com/ineelhere/startlit
 License: Apache License - Version 2.0
 Author: Indraneel Chakraborty
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,29 +12,32 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # StartLit ⭐
-![PyPI - Version](https://img.shields.io/pypi/v/startlit) ![GitHub repo size](https://img.shields.io/github/repo-size/ineelhere/startlit) ![GitHub License](https://img.shields.io/github/license/ineelhere/startlit) ![example workflow](https://github.com/ineelhere/startlit/actions/workflows/python-publish.yml/badge.svg) 
+![PyPI - Version](https://img.shields.io/pypi/v/startlit?style=plastic) ![GitHub License](https://img.shields.io/github/license/ineelhere/startlit?style=plastic) ![PyPI - Downloads](https://img.shields.io/pypi/dm/startLit?style=plastic&logoColor=blue&color=blue) ![example workflow](https://github.com/ineelhere/startlit/actions/workflows/python-publish.yml/badge.svg?style=plastic) 
 
 **Welcome to StartLit!**
 
 StartLit is your gateway to building Streamlit apps with ease. It brings a simple, streamlined way to start your Streamlit projects. Here's what's included in the latest release:
 
 #### Features:
 - **Package Installation**: Now you can easily install StartLit from PYPI using `pip install startlit`.
-- **Simple Usage**: Import the package and run `hello()` to receive a friendly welcome message.
-- **Basic help**: Use the `help()` function to get started with more support
--  **Starter App**: Use the `starter()` function to download a very simple starter app template, including an `app.py` file and a `requirements.txt` file.
--  **Multipage App**: Use the `multipage()` function to download an app template for building multipage Streamlit apps. The files/folders will be available in your working directory.
--  **Fragments App**: Use the `fragments()` function to download an app that allows you to run independent components in the streamlit app.
--  **List active streamlit apps** - Use the `list_streamlit_apps()` function to get a list of currently running
--  **Kill active streamlit apps** - Use the `kill_streamlit_apps(app_id)` function to kill desired running streamlit apps. `app_id` is the app ID you get from the `list_streamlit_apps()` function.
+
+* 🤗 `hello()` - Just a welcome text. 
+* 📥 `starter()` - A very simple starter app template. Quick-peek: https://startlit-starter.streamlit.app/
+* 📃 `multipage()` - An app template for building multipage Streamlit apps. Quick-peek: https://startlit-multipage.streamlit.app/
+* 📚 `fragments()` - An app that allows you to run independent components in the streamlit app. Quick-peek: https://startlit-fragments.streamlit.app/
+* 💬 `chat()`- A dummy chatbot app. Quick-peek: https://startlit-chat.streamlit.app/
+* 📜 `list_streamlit_apps()` - List running Streamlit apps.
+* 🔪 `kill_streamlit_apps()` - Kill running Streamlit apps.
+* 💡 `help()` - Display help menu with list of available functions.
+* 🐙 Need more help? Post an issue at https://github.com/ineelhere/startlit/issues
 
 ### Install the package from PYPI
 
 ```python
 pip install startlit
 ```
 ### Import the package
@@ -100,28 +103,31 @@
 
 # Download a multipage app template
 multipage()
 
 # Download a fragment app template
 fragments()
 
+# Download a dummy chatbot app template
+chat()
+
 # List all active apps
 list_streamlit_apps()
 
-# Kill a specific app
+# Kill a specific app by app_id
 kill_streamlit_apps(app_id)
-
-
 ```
 ___
 
 ### Feedback and Contribution:
-Excited to hear your feedback and suggestions for improvements. 
+Excited to hear your feedback and suggestions for improvements.
+
+Collaborations and Contributions are welcome 🤝
 Feel free to open issues or submit pull requests.
 
 Enjoy your streamlit journey with StartLit and happy coding! 🚀🎉
+
+*Check package download stats at https://pypistats.org/packages/startlit*
 ___
 
 **© `Indraneel Chakraborty` | 2024** 🧑‍💻[LinkedIn](https://www.linkedin.com/in/indraneelchakraborty/) | [X/Twitter](https://twitter.com/ineelhere)
 
-
-`Collaborations and Contributions are welcome 🤝`
```

