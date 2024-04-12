# Comparing `tmp/nyantip-0.7.1.tar.gz` & `tmp/nyantip-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nyantip-0.7.1.tar", last modified: Wed Mar  6 16:25:14 2024, max compression
+gzip compressed data, was "nyantip-0.8.tar", last modified: Fri Apr 12 16:44:47 2024, max compression
```

## Comparing `nyantip-0.7.1.tar` & `nyantip-0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 bboe       (501) staff       (20)        0 2024-03-06 16:25:14.832688 nyantip-0.7.1/
--rw-r--r--   0 bboe       (501) staff       (20)    18046 2024-03-06 16:13:01.000000 nyantip-0.7.1/LICENSE
--rw-r--r--   0 bboe       (501) staff       (20)       68 2024-03-06 16:13:01.000000 nyantip-0.7.1/MANIFEST.in
--rw-r--r--   0 bboe       (501) staff       (20)     2192 2024-03-06 16:25:14.832566 nyantip-0.7.1/PKG-INFO
--rw-r--r--   0 bboe       (501) staff       (20)     1893 2024-03-06 16:13:01.000000 nyantip-0.7.1/README.md
-drwxr-xr-x   0 bboe       (501) staff       (20)        0 2024-03-06 16:25:14.829371 nyantip-0.7.1/nyantip/
--rw-r--r--   0 bboe       (501) staff       (20)      690 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/__init__.py
--rw-r--r--   0 bboe       (501) staff       (20)    20212 2024-03-06 16:21:28.000000 nyantip-0.7.1/nyantip/actions.py
--rw-r--r--   0 bboe       (501) staff       (20)    15181 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/bot.py
--rw-r--r--   0 bboe       (501) staff       (20)     3152 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/coin.py
--rw-r--r--   0 bboe       (501) staff       (20)       22 2024-03-06 16:22:14.000000 nyantip-0.7.1/nyantip/const.py
--rw-r--r--   0 bboe       (501) staff       (20)      552 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/rpc.py
--rw-r--r--   0 bboe       (501) staff       (20)     5714 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/stats.py
-drwxr-xr-x   0 bboe       (501) staff       (20)        0 2024-03-06 16:25:14.832409 nyantip-0.7.1/nyantip/templates/
--rw-r--r--   0 bboe       (501) staff       (20)      167 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/address-invalid.tpl
--rw-r--r--   0 bboe       (501) staff       (20)        0 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/announcement.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      101 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/cant-send.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      701 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/confirmation.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      235 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/didnt-understand.tpl
--rw-r--r--   0 bboe       (501) staff       (20)     1285 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/footer.tpl
--rw-r--r--   0 bboe       (501) staff       (20)       79 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/history-empty.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      219 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/history.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      591 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/info.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      208 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/no-pending-tips.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      133 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/not-on-reddit.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      198 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/not-registered.tpl
--rw-r--r--   0 bboe       (501) staff       (20)       96 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/pending-tips-declined.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      173 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/tip-already-pending.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      383 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/tip-below-minimum.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      729 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/tip-low-balance.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      467 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/tip-pending.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      332 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/tip-received.tpl
--rw-r--r--   0 bboe       (501) staff       (20)      517 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/templates/tip-went-wrong.tpl
--rw-r--r--   0 bboe       (501) staff       (20)     2806 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/user.py
--rw-r--r--   0 bboe       (501) staff       (20)     1036 2024-03-06 16:13:01.000000 nyantip-0.7.1/nyantip/util.py
-drwxr-xr-x   0 bboe       (501) staff       (20)        0 2024-03-06 16:25:14.830229 nyantip-0.7.1/nyantip.egg-info/
--rw-r--r--   0 bboe       (501) staff       (20)     2192 2024-03-06 16:25:14.000000 nyantip-0.7.1/nyantip.egg-info/PKG-INFO
--rw-r--r--   0 bboe       (501) staff       (20)     1059 2024-03-06 16:25:14.000000 nyantip-0.7.1/nyantip.egg-info/SOURCES.txt
--rw-r--r--   0 bboe       (501) staff       (20)        1 2024-03-06 16:25:14.000000 nyantip-0.7.1/nyantip.egg-info/dependency_links.txt
--rw-r--r--   0 bboe       (501) staff       (20)       41 2024-03-06 16:25:14.000000 nyantip-0.7.1/nyantip.egg-info/entry_points.txt
--rw-r--r--   0 bboe       (501) staff       (20)      144 2024-03-06 16:25:14.000000 nyantip-0.7.1/nyantip.egg-info/requires.txt
--rw-r--r--   0 bboe       (501) staff       (20)        8 2024-03-06 16:25:14.000000 nyantip-0.7.1/nyantip.egg-info/top_level.txt
--rw-r--r--   0 bboe       (501) staff       (20)       38 2024-03-06 16:25:14.832726 nyantip-0.7.1/setup.cfg
--rw-r--r--   0 bboe       (501) staff       (20)     1340 2024-03-06 16:13:01.000000 nyantip-0.7.1/setup.py
+drwxr-xr-x   0 bboe       (501) staff       (20)        0 2024-04-12 16:44:47.408414 nyantip-0.8/
+-rw-r--r--   0 bboe       (501) staff       (20)    18046 2024-03-06 16:13:01.000000 nyantip-0.8/LICENSE
+-rw-r--r--   0 bboe       (501) staff       (20)       68 2024-03-06 16:13:01.000000 nyantip-0.8/MANIFEST.in
+-rw-r--r--   0 bboe       (501) staff       (20)     2538 2024-04-12 16:44:47.408197 nyantip-0.8/PKG-INFO
+-rw-r--r--   0 bboe       (501) staff       (20)     1893 2024-03-06 16:13:01.000000 nyantip-0.8/README.md
+drwxr-xr-x   0 bboe       (501) staff       (20)        0 2024-04-12 16:44:47.404723 nyantip-0.8/nyantip/
+-rw-r--r--   0 bboe       (501) staff       (20)      690 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/__init__.py
+-rw-r--r--   0 bboe       (501) staff       (20)    20215 2024-04-12 15:18:42.000000 nyantip-0.8/nyantip/actions.py
+-rw-r--r--   0 bboe       (501) staff       (20)    15181 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/bot.py
+-rw-r--r--   0 bboe       (501) staff       (20)     3152 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/coin.py
+-rw-r--r--   0 bboe       (501) staff       (20)       22 2024-04-12 16:42:44.000000 nyantip-0.8/nyantip/const.py
+-rw-r--r--   0 bboe       (501) staff       (20)      552 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/rpc.py
+-rw-r--r--   0 bboe       (501) staff       (20)     5714 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/stats.py
+drwxr-xr-x   0 bboe       (501) staff       (20)        0 2024-04-12 16:44:47.407552 nyantip-0.8/nyantip/templates/
+-rw-r--r--   0 bboe       (501) staff       (20)      167 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/address-invalid.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)        0 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/announcement.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      101 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/cant-send.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)     1252 2024-04-12 15:18:42.000000 nyantip-0.8/nyantip/templates/confirmation.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      235 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/didnt-understand.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)     1285 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/footer.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)       79 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/history-empty.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      219 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/history.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      591 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/info.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      208 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/no-pending-tips.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      133 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/not-on-reddit.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      198 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/not-registered.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)       96 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/pending-tips-declined.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      173 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/tip-already-pending.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      383 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/tip-below-minimum.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      729 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/tip-low-balance.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      467 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/tip-pending.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      332 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/tip-received.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)      517 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/templates/tip-went-wrong.tpl
+-rw-r--r--   0 bboe       (501) staff       (20)     2806 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/user.py
+-rw-r--r--   0 bboe       (501) staff       (20)     1036 2024-03-06 16:13:01.000000 nyantip-0.8/nyantip/util.py
+drwxr-xr-x   0 bboe       (501) staff       (20)        0 2024-04-12 16:44:47.407713 nyantip-0.8/nyantip.egg-info/
+-rw-r--r--   0 bboe       (501) staff       (20)     2538 2024-04-12 16:44:47.000000 nyantip-0.8/nyantip.egg-info/PKG-INFO
+-rw-r--r--   0 bboe       (501) staff       (20)     1059 2024-04-12 16:44:47.000000 nyantip-0.8/nyantip.egg-info/SOURCES.txt
+-rw-r--r--   0 bboe       (501) staff       (20)        1 2024-04-12 16:44:47.000000 nyantip-0.8/nyantip.egg-info/dependency_links.txt
+-rw-r--r--   0 bboe       (501) staff       (20)       41 2024-04-12 16:44:47.000000 nyantip-0.8/nyantip.egg-info/entry_points.txt
+-rw-r--r--   0 bboe       (501) staff       (20)      144 2024-04-12 16:44:47.000000 nyantip-0.8/nyantip.egg-info/requires.txt
+-rw-r--r--   0 bboe       (501) staff       (20)        8 2024-04-12 16:44:47.000000 nyantip-0.8/nyantip.egg-info/top_level.txt
+-rw-r--r--   0 bboe       (501) staff       (20)       38 2024-04-12 16:44:47.408457 nyantip-0.8/setup.cfg
+-rw-r--r--   0 bboe       (501) staff       (20)     1340 2024-03-06 16:13:01.000000 nyantip-0.8/setup.py
```

### Comparing `nyantip-0.7.1/LICENSE` & `nyantip-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/PKG-INFO` & `nyantip-0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: nyantip
-Version: 0.7.1
-Summary: Nyancoin tip bot for Reddit.
-Author: Bryce Boe
-Author-email: bbzbryce@gmail.com
-License: GPL
-Project-URL: Source Code, https://github.com/bboe/nyantip
-Requires-Python: ~= 3.6
-Provides-Extra: gpg
-Provides-Extra: lint
-License-File: LICENSE
-
 # It's nyantip!
 
 ## Getting started
 
 ### Install
 
 __Note__: If the following doesn't work, ensure you have pip installed:
```

### Comparing `nyantip-0.7.1/nyantip/__init__.py` & `nyantip-0.8/nyantip/__init__.py`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip/actions.py` & `nyantip-0.8/nyantip/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,15 +569,15 @@
 
         if row["path"] is not None:
             message = nyantip.reddit.comment(row["message_id"])
         else:
             message = nyantip.reddit.inbox.message(row["message_id"])
 
         if message.author is None:
-            log.warning("Cannot process item missing author. %r", message)
+            logger.warning("Cannot process item missing author. %r", message)
             continue
 
         results.append(
             Action(
                 action=action,
                 amount=amount,
                 destination=row["destination"],
```

### Comparing `nyantip-0.7.1/nyantip/bot.py` & `nyantip-0.8/nyantip/bot.py`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip/coin.py` & `nyantip-0.8/nyantip/coin.py`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip/rpc.py` & `nyantip-0.8/nyantip/rpc.py`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip/stats.py` & `nyantip-0.8/nyantip/stats.py`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip/templates/confirmation.tpl` & `nyantip-0.8/nyantip/templates/tip-went-wrong.tpl`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-{% set stats_url = "/r/{}/wiki/stats".format(config["reddit"]["subreddit"]) %}
-{% if to_address: %}
-{%   set explorer = config["coin"]["explorer"] %}
-{%   set arrow_formatted = "[->]({}{})".format(explorer["transaction"], transaction_id) %}
-{%   set destination_formatted = "[{}]({}{})".format(destination, explorer["address"], destination) %}
-{% else: %}
-{%   set arrow_formatted = "tipped" %}
-{%   set destination_formatted = "u/{}".format(destination) %}
+{% if to_address %}
+{%   set destination_formatted = " to __{}__".format(destination) %}
+{% elif destination %}
+{%   set destination_formatted = " to __u/{}__".format(destination) %}
+{% else %}
+{%   set destination_formatted = "" %}
 {% endif %}
-**^([{{ title }}]) u/{{ message.author }} {{ arrow_formatted }} {{ destination_formatted }} __{{ amount_formatted }}__** |[ wiki ]({{ "/r/{}/wiki/{}".format(config["reddit"]["subreddit"], "index") }}) | [ stats ]({{ stats_url }})|
+Hey u/{{ message.author }}, something went wrong and your {{ action_name }} of __{{ amount_formatted }}__{{ destination_formatted }} may not have been processed. My developer has been notified, and will look into the issue as soon as possible.
+
+{% include 'footer.tpl' %}
```

### Comparing `nyantip-0.7.1/nyantip/templates/footer.tpl` & `nyantip-0.8/nyantip/templates/footer.tpl`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip/templates/info.tpl` & `nyantip-0.8/nyantip/templates/info.tpl`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip/templates/tip-low-balance.tpl` & `nyantip-0.8/nyantip/templates/tip-low-balance.tpl`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip/user.py` & `nyantip-0.8/nyantip/user.py`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip/util.py` & `nyantip-0.8/nyantip/util.py`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/nyantip.egg-info/PKG-INFO` & `nyantip-0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Metadata-Version: 2.1
 Name: nyantip
-Version: 0.7.1
+Version: 0.8.0
 Summary: Nyancoin tip bot for Reddit.
 Author: Bryce Boe
 Author-email: bbzbryce@gmail.com
 License: GPL
 Project-URL: Source Code, https://github.com/bboe/nyantip
 Requires-Python: ~= 3.6
+License-File: LICENSE
+Requires-Dist: Jinja2~=3.0
+Requires-Dist: PyYAML~=6.0
+Requires-Dist: mysqlclient~=2.2
+Requires-Dist: praw~=7.3
+Requires-Dist: python-bitcoinrpc==1.0
+Requires-Dist: sqlalchemy~=1.4
 Provides-Extra: gpg
+Requires-Dist: python-gnupg==0.4.7; extra == "gpg"
 Provides-Extra: lint
-License-File: LICENSE
+Requires-Dist: black; extra == "lint"
+Requires-Dist: flake8; extra == "lint"
+Requires-Dist: isort; extra == "lint"
 
 # It's nyantip!
 
 ## Getting started
 
 ### Install
```

### Comparing `nyantip-0.7.1/nyantip.egg-info/SOURCES.txt` & `nyantip-0.8/nyantip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nyantip-0.7.1/setup.py` & `nyantip-0.8/setup.py`

 * *Files identical despite different names*

