# Comparing `tmp/reflex-chat-0.0.1a4.tar.gz` & `tmp/reflex-chat-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-chat-0.0.1a4.tar", last modified: Mon Apr  8 22:00:09 2024, max compression
+gzip compressed data, was "reflex-chat-0.0.1a5.tar", last modified: Fri Apr 12 01:10:48 2024, max compression
```

## Comparing `reflex-chat-0.0.1a4.tar` & `reflex-chat-0.0.1a5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-08 22:00:09.216578 reflex-chat-0.0.1a4/
--rw-r--r--   0 nikhil     (501) staff       (20)      570 2024-04-08 22:00:09.216375 reflex-chat-0.0.1a4/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)       93 2024-03-07 21:28:46.000000 reflex-chat-0.0.1a4/README.md
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-08 22:00:09.214466 reflex-chat-0.0.1a4/custom_components/
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-08 22:00:09.215119 reflex-chat-0.0.1a4/custom_components/reflex_chat/
--rw-r--r--   0 nikhil     (501) staff       (20)       19 2024-04-05 22:25:08.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat/__init__.py
--rw-r--r--   0 nikhil     (501) staff       (20)     4771 2024-03-27 23:06:34.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat/chat.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-08 22:00:09.216060 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/
--rw-r--r--   0 nikhil     (501) staff       (20)      570 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)      368 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/SOURCES.txt
--rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/dependency_links.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/requires.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/top_level.txt
--rw-r--r--   0 nikhil     (501) staff       (20)      669 2024-04-08 18:52:03.000000 reflex-chat-0.0.1a4/pyproject.toml
--rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-04-08 22:00:09.216624 reflex-chat-0.0.1a4/setup.cfg
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-12 01:10:48.838246 reflex-chat-0.0.1a5/
+-rw-r--r--   0 nikhil     (501) staff       (20)      672 2024-04-12 01:10:48.838040 reflex-chat-0.0.1a5/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)       93 2024-03-07 21:28:46.000000 reflex-chat-0.0.1a5/README.md
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-12 01:10:48.836637 reflex-chat-0.0.1a5/custom_components/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-12 01:10:48.837069 reflex-chat-0.0.1a5/custom_components/reflex_chat/
+-rw-r--r--   0 nikhil     (501) staff       (20)       19 2024-04-05 22:25:08.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     4421 2024-04-12 01:08:21.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat/chat.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-12 01:10:48.837762 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/
+-rw-r--r--   0 nikhil     (501) staff       (20)      672 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)      368 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/requires.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/top_level.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)      762 2024-04-12 01:10:23.000000 reflex-chat-0.0.1a5/pyproject.toml
+-rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-04-12 01:10:48.838279 reflex-chat-0.0.1a5/setup.cfg
```

### Comparing `reflex-chat-0.0.1a4/custom_components/reflex_chat/chat.py` & `reflex-chat-0.0.1a5/custom_components/reflex_chat/chat.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,36 +22,27 @@
         component = super().create(**props)
         component.State.process = process
         return component
 
     @classmethod
     def get_component(cls, **props) -> rx.Component:
         return rx.vstack(
-            rx.link(
-                rx.hstack(
-                    "Built with ",
-                    rx.image(src="/Reflex.svg"),
-                    align="center",
-                    background_color=rx.color("purple", 4),
-                    border_bottom=f"1px solid {rx.color('purple', 6)}",
-                    width="100%",
-                    padding="1em",
-                ),
+            rx.flex(
+                rx.logo(),
+                background_color=rx.color("accent", 4),
+                border_bottom=f"1px solid {rx.color('accent', 6)}",
                 width="100%",
-                href="https://reflex.dev",
-                _hover={
-                    "text_decoration": "none",
-                },
-                color=rx.color("mauve", 12),
-                is_external=True,
+                justify="start",
             ),
             rx.spacer(),
             rx.vstack(
                 rx.box(
-                    rx.foreach(cls.messages, lambda message, i: chat_bubble(message, i)),
+                    rx.foreach(
+                        cls.messages, lambda message, i: chat_bubble(message, i)
+                    ),
                     id=f"chatbox-{cls.__name__}",
                     overflow="auto",
                     width="100%",
                     padding_bottom="2em",
                 ),
                 rx.spacer(),
                 action_bar(cls),
@@ -111,16 +102,16 @@
     """
     return rx.cond(
         message["role"] == "system",
         rx.fragment(),
         rx.box(
             rx.markdown(
                 message["content"],
-                background_color=rx.cond(message["role"] == "user", rx.color("mauve", 4), rx.color("purple", 4)),
-                color=rx.cond(message["role"] == "user", rx.color("mauve", 12), rx.color("purple", 12)),
+                background_color=rx.cond(message["role"] == "user", rx.color("mauve", 4), rx.color("accent", 4)),
+                color=rx.cond(message["role"] == "user", rx.color("mauve", 12), rx.color("accent", 12)),
                 display="inline-block",
                 padding_x="1em",
                 border_radius="8px",
                 max_width=["30em", "30em", "50em", "50em", "50em", "50em"],
             ),
             id=f"message-{idx}",
             text_align=rx.cond(message["role"] == "user", "right", "left"),
```

### Comparing `reflex-chat-0.0.1a4/pyproject.toml` & `reflex-chat-0.0.1a5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,33 +3,35 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-chat"
-version = "0.0.1a4"
-description = "Reflex custom component chat"
+version = "0.0.1a5"
+description = "A chat component that can be hooked up to any LLM."
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
-authors = [{ name = "Your Name", email = "YOUREMAIL@domain.com" }]
+authors = [{ name = "Nikhil Rao", email = "nikhil@reflex.dev" }]
 keywords = [
     "reflex",
     "reflex-custom-components"]
 
 dependencies = [
     "reflex>=0.4.2"
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
 ]
 
 [project.urls]
-Homepage = "https://github.com"
+homepage = "https://github.com/picklelo/reflex-chat"
+source = "https://github.com/picklelo/reflex-chat"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
+
 [tool.setuptools.packages.find]
 where = ["custom_components"]
```

