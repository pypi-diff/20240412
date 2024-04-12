# Comparing `tmp/pycityagent-1.1.2.tar.gz` & `tmp/pycityagent-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycityagent-1.1.2.tar", last modified: Wed Apr 10 07:52:20 2024, max compression
+gzip compressed data, was "pycityagent-1.1.3.tar", last modified: Fri Apr 12 02:57:18 2024, max compression
```

## Comparing `pycityagent-1.1.2.tar` & `pycityagent-1.1.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.432150 pycityagent-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 07:52:15.000000 pycityagent-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-10 07:52:20.432150 pycityagent-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-10 07:52:15.000000 pycityagent-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.420150 pycityagent-1.1.2/pycityagent/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.424150 pycityagent-1.1.2/pycityagent/ac/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/action_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.424150 pycityagent-1.1.2/pycityagent/ac/citizen_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/citizen_actions/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/citizen_actions/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/citizen_actions/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/citizen_actions/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/citizen_actions/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/hub_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/sim_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/ac/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/agent_citizen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/agent_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.428150 pycityagent-1.1.2/pycityagent/brain/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/brain.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/brainfc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21934 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.428150 pycityagent-1.1.2/pycityagent/brain/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/persistence/social.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/persistence/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.428150 pycityagent-1.1.2/pycityagent/brain/reason/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/reason/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/reason/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/reason/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/reason/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.428150 pycityagent-1.1.2/pycityagent/brain/retrive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/retrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/retrive/social.py
--rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28683 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/sence.py
--rw-r--r--   0 runner    (1001) docker     (127)    29081 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/brain/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.428150 pycityagent-1.1.2/pycityagent/cc/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/cc/cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/cc/conve.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/cc/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/cc/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/cc/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/cc/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.428150 pycityagent-1.1.2/pycityagent/hubconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/hubconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/hubconnector/hubconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.428150 pycityagent-1.1.2/pycityagent/image/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.432150 pycityagent-1.1.2/pycityagent/st/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/st/st.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.432150 pycityagent-1.1.2/pycityagent/urbanllm/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/urbanllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pycityagent/urbanllm/urbanllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:52:20.432150 pycityagent-1.1.2/pycityagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-10 07:52:20.000000 pycityagent-1.1.2/pycityagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-10 07:52:20.000000 pycityagent-1.1.2/pycityagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:52:20.000000 pycityagent-1.1.2/pycityagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 07:52:20.000000 pycityagent-1.1.2/pycityagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 07:52:20.000000 pycityagent-1.1.2/pycityagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-10 07:52:15.000000 pycityagent-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:52:20.432150 pycityagent-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.067371 pycityagent-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 02:57:13.000000 pycityagent-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-12 02:57:18.067371 pycityagent-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-12 02:57:13.000000 pycityagent-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.055371 pycityagent-1.1.3/pycityagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.059371 pycityagent-1.1.3/pycityagent/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/action_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.059371 pycityagent-1.1.3/pycityagent/ac/citizen_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/citizen_actions/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/hub_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/sim_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/ac/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/agent_citizen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/agent_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/brain/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/brainfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21934 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/brain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/persistence/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/persistence/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/brain/reason/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/reason/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/brain/retrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/retrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/retrive/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28683 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/sence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29081 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/brain/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/conve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/cc/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/hubconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/hubconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/hubconnector/hubconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.063371 pycityagent-1.1.3/pycityagent/st/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/st/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/st/st.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.067371 pycityagent-1.1.3/pycityagent/urbanllm/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/urbanllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pycityagent/urbanllm/urbanllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:57:18.067371 pycityagent-1.1.3/pycityagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 02:57:18.000000 pycityagent-1.1.3/pycityagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 02:57:13.000000 pycityagent-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 02:57:18.067371 pycityagent-1.1.3/setup.cfg
```

### Comparing `pycityagent-1.1.2/LICENSE` & `pycityagent-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/PKG-INFO` & `pycityagent-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.2
+Version: 1.1.3
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycityagent-1.1.2/README.md` & `pycityagent-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/ac.py` & `pycityagent-1.1.3/pycityagent/ac/ac.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/action.py` & `pycityagent-1.1.3/pycityagent/ac/action.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/action_stream.py` & `pycityagent-1.1.3/pycityagent/ac/action_stream.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/citizen_actions/controled.py` & `pycityagent-1.1.3/pycityagent/ac/citizen_actions/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/citizen_actions/converse.py` & `pycityagent-1.1.3/pycityagent/ac/citizen_actions/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/citizen_actions/idle.py` & `pycityagent-1.1.3/pycityagent/ac/citizen_actions/idle.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/citizen_actions/shop.py` & `pycityagent-1.1.3/pycityagent/ac/citizen_actions/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/citizen_actions/trip.py` & `pycityagent-1.1.3/pycityagent/ac/citizen_actions/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/controled.py` & `pycityagent-1.1.3/pycityagent/ac/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/converse.py` & `pycityagent-1.1.3/pycityagent/ac/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/hub_actions.py` & `pycityagent-1.1.3/pycityagent/ac/hub_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/shop.py` & `pycityagent-1.1.3/pycityagent/ac/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/sim_actions.py` & `pycityagent-1.1.3/pycityagent/ac/sim_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/ac/trip.py` & `pycityagent-1.1.3/pycityagent/ac/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/agent.py` & `pycityagent-1.1.3/pycityagent/agent.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/agent_citizen.py` & `pycityagent-1.1.3/pycityagent/agent_citizen.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/agent_func.py` & `pycityagent-1.1.3/pycityagent/agent_func.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/brain.py` & `pycityagent-1.1.3/pycityagent/brain/brain.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/memory.py` & `pycityagent-1.1.3/pycityagent/brain/memory.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/persistence/spatial.py` & `pycityagent-1.1.3/pycityagent/brain/persistence/spatial.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/reason/shop.py` & `pycityagent-1.1.3/pycityagent/brain/reason/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/reason/social.py` & `pycityagent-1.1.3/pycityagent/brain/reason/social.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/reason/trip.py` & `pycityagent-1.1.3/pycityagent/brain/reason/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/reason/user.py` & `pycityagent-1.1.3/pycityagent/brain/reason/user.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/scheduler.py` & `pycityagent-1.1.3/pycityagent/brain/scheduler.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/sence.py` & `pycityagent-1.1.3/pycityagent/brain/sence.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/brain/static.py` & `pycityagent-1.1.3/pycityagent/brain/static.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/cc/cc.py` & `pycityagent-1.1.3/pycityagent/cc/cc.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/hubconnector/hubconnector.py` & `pycityagent-1.1.3/pycityagent/hubconnector/hubconnector.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/image/image.py` & `pycityagent-1.1.3/pycityagent/image/image.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/simulator.py` & `pycityagent-1.1.3/pycityagent/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self._perceive = SimPerceive(self)
         self.map = map.Map(
             mongo_uri = "mongodb://sim:FiblabSim1001@mgo.db.fiblab.tech:8635/",
             mongo_db = "srt",
             mongo_coll = config['map_request']['mongo_coll'],
             cache_dir = config['map_request']['cache_dir'],
         )
-        self.routing = RoutingClient(self.config['route_request']['server'], True)
+        self.routing = RoutingClient(self.config['route_request']['server'])
         self.time = 0
 
     # * Agent相关
     def FindAgentsByArea(self, req: dict, status=None):
         """
         通过区域范围查找agent/person
         Get agents/persons in the provided area
```

### Comparing `pycityagent-1.1.2/pycityagent/st/st.py` & `pycityagent-1.1.3/pycityagent/st/st.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent/urbanllm/urbanllm.py` & `pycityagent-1.1.3/pycityagent/urbanllm/urbanllm.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pycityagent.egg-info/PKG-INFO` & `pycityagent-1.1.3/pycityagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.2
+Version: 1.1.3
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycityagent-1.1.2/pycityagent.egg-info/SOURCES.txt` & `pycityagent-1.1.3/pycityagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.2/pyproject.toml` & `pycityagent-1.1.3/pyproject.toml`

 * *Files identical despite different names*

