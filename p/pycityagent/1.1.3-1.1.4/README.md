# Comparing `tmp/pycityagent-1.1.3.tar.gz` & `tmp/pycityagent-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycityagent-1.1.3.tar", last modified: Fri Apr 12 02:57:18 2024, max compression
+gzip compressed data, was "pycityagent-1.1.4.tar", last modified: Fri Apr 12 04:41:15 2024, max compression
```

## Comparing `pycityagent-1.1.3.tar` & `pycityagent-1.1.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.067371 pycityagent-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 02:57:13.000000 pycityagent-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-12 02:57:18.067371 pycityagent-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-12 02:57:13.000000 pycityagent-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.055371 pycityagent-1.1.3/pycityagent/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.059371 pycityagent-1.1.3/pycityagent/ac/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/action_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.059371 pycityagent-1.1.3/pycityagent/ac/citizen_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/hub_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/sim_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/agent_citizen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/agent_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/brain/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/brain.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/brainfc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21934 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/brain/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/persistence/social.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/persistence/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/brain/reason/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/brain/retrive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/retrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/retrive/social.py
--rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28683 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/sence.py
--rw-r--r--   0 runner    (1001) docker     (127)    29081 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/cc/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/conve.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/hubconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/hubconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/hubconnector/hubconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/image/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/st/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/st/st.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.067371 pycityagent-1.1.3/pycityagent/urbanllm/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/urbanllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/urbanllm/urbanllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.067371 pycityagent-1.1.3/pycityagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 02:57:18.067371 pycityagent-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.370578 pycityagent-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 04:41:10.000000 pycityagent-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-12 04:41:15.370578 pycityagent-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-12 04:41:10.000000 pycityagent-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.362578 pycityagent-1.1.4/pycityagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.366578 pycityagent-1.1.4/pycityagent/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/action_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.366578 pycityagent-1.1.4/pycityagent/ac/citizen_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/citizen_actions/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/citizen_actions/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/citizen_actions/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/citizen_actions/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/citizen_actions/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/hub_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/sim_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/ac/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/agent_citizen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/agent_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.366578 pycityagent-1.1.4/pycityagent/brain/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/brainfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21934 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.366578 pycityagent-1.1.4/pycityagent/brain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/persistence/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/persistence/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.370578 pycityagent-1.1.4/pycityagent/brain/reason/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/reason/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/reason/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/reason/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/reason/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.370578 pycityagent-1.1.4/pycityagent/brain/retrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/retrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/retrive/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28683 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/sence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29081 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/brain/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.370578 pycityagent-1.1.4/pycityagent/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/cc/cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/cc/conve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/cc/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/cc/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/cc/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/cc/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.370578 pycityagent-1.1.4/pycityagent/hubconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/hubconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/hubconnector/hubconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.370578 pycityagent-1.1.4/pycityagent/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.370578 pycityagent-1.1.4/pycityagent/st/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/st/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/st/st.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.370578 pycityagent-1.1.4/pycityagent/urbanllm/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/urbanllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pycityagent/urbanllm/urbanllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:41:15.370578 pycityagent-1.1.4/pycityagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-12 04:41:15.000000 pycityagent-1.1.4/pycityagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-12 04:41:15.000000 pycityagent-1.1.4/pycityagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 04:41:15.000000 pycityagent-1.1.4/pycityagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 04:41:15.000000 pycityagent-1.1.4/pycityagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 04:41:15.000000 pycityagent-1.1.4/pycityagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 04:41:10.000000 pycityagent-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 04:41:15.370578 pycityagent-1.1.4/setup.cfg
```

### Comparing `pycityagent-1.1.3/LICENSE` & `pycityagent-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/PKG-INFO` & `pycityagent-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.3
+Version: 1.1.4
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -73,15 +73,15 @@
 - There are three parts of a config file: **llm_request**, **citysim_request** and **apphub_request**
 ```yaml
 llm_request:
   text_request:
     request_type: openai / qwen
     api_key: xxx
     model: xxx
-    http_client: xxx (if you use opanai and want to use your own backend LLM model)
+    (api_base): xxx (this is an optional config, if you use opanai and want to use your own backend LLM model, default to "https://api.openai.com/v1")
   img_understand_request:
     request_type: qwen
     api_key: xxx
     model: xxx
   img_generate_request:
     request_type: qwen
     api_key: xxx
@@ -109,15 +109,16 @@
 - Forget about **citysim_request**, let's focus on the other two.
 
 #### LLM_REQUEST
 - As you can see, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
 - By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
     - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
 - Get your **api_key** and chooce your **model**
-- If you want to use your backend models, set the **http_client** (only available when using **openai**)
+- If you want to use your backend models, set the **api_base** (only available when using **openai**)
+  - default value: "https://api.openai.com/v1"
 
 #### CITYSIM_REQUEST
 - Most of the configuration options in this part are determined, such as **simulator.server**, **map_request.mongo_coll**, **route_request.server**
 - **map_request.cache_dir**: used for storing map data your machine, you can justify the target dir as you wish (**create the dir first**)
 - **streetview_request**: used for obtaining streetview images, by now, we support baidumap engine and googlemap engine
   - if you choose baidumap engine, you need to get a baidumap api-key
     ``` yaml
```

### Comparing `pycityagent-1.1.3/README.md` & `pycityagent-1.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 - There are three parts of a config file: **llm_request**, **citysim_request** and **apphub_request**
 ```yaml
 llm_request:
   text_request:
     request_type: openai / qwen
     api_key: xxx
     model: xxx
-    http_client: xxx (if you use opanai and want to use your own backend LLM model)
+    (api_base): xxx (this is an optional config, if you use opanai and want to use your own backend LLM model, default to "https://api.openai.com/v1")
   img_understand_request:
     request_type: qwen
     api_key: xxx
     model: xxx
   img_generate_request:
     request_type: qwen
     api_key: xxx
@@ -62,15 +62,16 @@
 - Forget about **citysim_request**, let's focus on the other two.
 
 #### LLM_REQUEST
 - As you can see, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
 - By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
     - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
 - Get your **api_key** and chooce your **model**
-- If you want to use your backend models, set the **http_client** (only available when using **openai**)
+- If you want to use your backend models, set the **api_base** (only available when using **openai**)
+  - default value: "https://api.openai.com/v1"
 
 #### CITYSIM_REQUEST
 - Most of the configuration options in this part are determined, such as **simulator.server**, **map_request.mongo_coll**, **route_request.server**
 - **map_request.cache_dir**: used for storing map data your machine, you can justify the target dir as you wish (**create the dir first**)
 - **streetview_request**: used for obtaining streetview images, by now, we support baidumap engine and googlemap engine
   - if you choose baidumap engine, you need to get a baidumap api-key
     ``` yaml
```

### Comparing `pycityagent-1.1.3/pycityagent/ac/ac.py` & `pycityagent-1.1.4/pycityagent/ac/ac.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/action.py` & `pycityagent-1.1.4/pycityagent/ac/action.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/action_stream.py` & `pycityagent-1.1.4/pycityagent/ac/action_stream.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/citizen_actions/controled.py` & `pycityagent-1.1.4/pycityagent/ac/citizen_actions/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/citizen_actions/converse.py` & `pycityagent-1.1.4/pycityagent/ac/citizen_actions/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/citizen_actions/idle.py` & `pycityagent-1.1.4/pycityagent/ac/citizen_actions/idle.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/citizen_actions/shop.py` & `pycityagent-1.1.4/pycityagent/ac/citizen_actions/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/citizen_actions/trip.py` & `pycityagent-1.1.4/pycityagent/ac/citizen_actions/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/controled.py` & `pycityagent-1.1.4/pycityagent/ac/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/converse.py` & `pycityagent-1.1.4/pycityagent/ac/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/hub_actions.py` & `pycityagent-1.1.4/pycityagent/ac/hub_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/shop.py` & `pycityagent-1.1.4/pycityagent/ac/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/sim_actions.py` & `pycityagent-1.1.4/pycityagent/ac/sim_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/ac/trip.py` & `pycityagent-1.1.4/pycityagent/ac/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/agent.py` & `pycityagent-1.1.4/pycityagent/agent.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/agent_citizen.py` & `pycityagent-1.1.4/pycityagent/agent_citizen.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/agent_func.py` & `pycityagent-1.1.4/pycityagent/agent_func.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/brain.py` & `pycityagent-1.1.4/pycityagent/brain/brain.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/memory.py` & `pycityagent-1.1.4/pycityagent/brain/memory.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/persistence/spatial.py` & `pycityagent-1.1.4/pycityagent/brain/persistence/spatial.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/reason/shop.py` & `pycityagent-1.1.4/pycityagent/brain/reason/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/reason/social.py` & `pycityagent-1.1.4/pycityagent/brain/reason/social.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/reason/trip.py` & `pycityagent-1.1.4/pycityagent/brain/reason/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/reason/user.py` & `pycityagent-1.1.4/pycityagent/brain/reason/user.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/scheduler.py` & `pycityagent-1.1.4/pycityagent/brain/scheduler.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/sence.py` & `pycityagent-1.1.4/pycityagent/brain/sence.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/brain/static.py` & `pycityagent-1.1.4/pycityagent/brain/static.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/cc/cc.py` & `pycityagent-1.1.4/pycityagent/cc/cc.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/hubconnector/hubconnector.py` & `pycityagent-1.1.4/pycityagent/hubconnector/hubconnector.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/image/image.py` & `pycityagent-1.1.4/pycityagent/image/image.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/simulator.py` & `pycityagent-1.1.4/pycityagent/simulator.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/st/st.py` & `pycityagent-1.1.4/pycityagent/st/st.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pycityagent/urbanllm/urbanllm.py` & `pycityagent-1.1.4/pycityagent/urbanllm/urbanllm.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     """
     def __init__(
         self, 
         config: dict
     ) -> None:
         self.config = config
         self.text = config['text_request']
+        if 'api_base' in self.text.keys() and self.text['api_base'] == 'None':
+            self.text['api_base'] = None
         self.image_u = config['img_understand_request']
         self.image_g = config['img_generate_request']
 
 class UrbanLLM:
     """
     大语言模型对象
     The LLM Object used by Agent(Soul)
@@ -37,20 +39,22 @@
 
         Args:
         - dialog (list[dict]): 标准的LLM文本dialog. The standard text LLM dialog
 
         Returns:
         - (str): the response content
         """
-        client = None if self.config.text['http_client'] == None else self.config.text['http_client']
+        if 'api_base' in self.config.text.keys():
+            api_base = self.config.text['api_base']
+        else:
+            api_base = None
         if self.config.text['request_type'] == 'openai':
             client = OpenAI(
                 api_key=self.config.text['api_key'], 
-                base_url=self.config.text['api_base'],
-                http_client=client
+                base_url=api_base,
             )
             response = client.chat.completions.create(
                 model=self.config.text['model'],
                 messages=dialog,
                 temperature=1.0,
             )
             return response.choices[0].message.content
@@ -71,15 +75,15 @@
 
     def img_understand(self, img_path:str, prompt:str=None) -> str:
         """
         图像理解
         Image understanding
 
         Args:
-        - img_path: 图像的绝对路径. The absolute path of selected Image
+        - img_path: 目标图像的路径. The path of selected Image
         - prompt: 理解提示词 - 例如理解方向. The understanding prompts
 
         Returns:
         - (str): the understanding content
         """
         ppt = "如何理解这幅图像？"
         if prompt != None:
```

### Comparing `pycityagent-1.1.3/pycityagent.egg-info/PKG-INFO` & `pycityagent-1.1.4/pycityagent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.3
+Version: 1.1.4
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -73,15 +73,15 @@
 - There are three parts of a config file: **llm_request**, **citysim_request** and **apphub_request**
 ```yaml
 llm_request:
   text_request:
     request_type: openai / qwen
     api_key: xxx
     model: xxx
-    http_client: xxx (if you use opanai and want to use your own backend LLM model)
+    (api_base): xxx (this is an optional config, if you use opanai and want to use your own backend LLM model, default to "https://api.openai.com/v1")
   img_understand_request:
     request_type: qwen
     api_key: xxx
     model: xxx
   img_generate_request:
     request_type: qwen
     api_key: xxx
@@ -109,15 +109,16 @@
 - Forget about **citysim_request**, let's focus on the other two.
 
 #### LLM_REQUEST
 - As you can see, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
 - By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
     - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
 - Get your **api_key** and chooce your **model**
-- If you want to use your backend models, set the **http_client** (only available when using **openai**)
+- If you want to use your backend models, set the **api_base** (only available when using **openai**)
+  - default value: "https://api.openai.com/v1"
 
 #### CITYSIM_REQUEST
 - Most of the configuration options in this part are determined, such as **simulator.server**, **map_request.mongo_coll**, **route_request.server**
 - **map_request.cache_dir**: used for storing map data your machine, you can justify the target dir as you wish (**create the dir first**)
 - **streetview_request**: used for obtaining streetview images, by now, we support baidumap engine and googlemap engine
   - if you choose baidumap engine, you need to get a baidumap api-key
     ``` yaml
```

### Comparing `pycityagent-1.1.3/pycityagent.egg-info/SOURCES.txt` & `pycityagent-1.1.4/pycityagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.3/pyproject.toml` & `pycityagent-1.1.4/pyproject.toml`

 * *Files identical despite different names*

