# Comparing `tmp/cfbd_json_py-0.1.1.tar.gz` & `tmp/cfbd_json_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfbd_json_py-0.1.1.tar", last modified: Sat Feb 24 22:01:18 2024, max compression
+gzip compressed data, was "cfbd_json_py-0.1.2.tar", last modified: Fri Apr 12 00:38:11 2024, max compression
```

## Comparing `cfbd_json_py-0.1.1.tar` & `cfbd_json_py-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 22:01:18.794014 cfbd_json_py-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-02-24 22:01:18.794014 cfbd_json_py-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 22:01:18.794014 cfbd_json_py-0.1.1/cfbd_json_py/
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/_early_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    17635 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/betting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16452 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/coaches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/conferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    25765 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/draft.py
--rw-r--r--   0 runner    (1001) docker     (127)    22924 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/drives.py
--rw-r--r--   0 runner    (1001) docker     (127)   156826 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/games.py
--rw-r--r--   0 runner    (1001) docker     (127)    93844 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    90992 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/players.py
--rw-r--r--   0 runner    (1001) docker     (127)    44307 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/plays.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/rankings.py
--rw-r--r--   0 runner    (1001) docker     (127)    50126 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/ratings.py
--rw-r--r--   0 runner    (1001) docker     (127)    33542 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/recruiting.py
--rw-r--r--   0 runner    (1001) docker     (127)    70217 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    41292 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/utls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-02-24 22:00:59.000000 cfbd_json_py-0.1.1/cfbd_json_py/venues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 22:01:18.794014 cfbd_json_py-0.1.1/cfbd_json_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-02-24 22:01:18.000000 cfbd_json_py-0.1.1/cfbd_json_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-24 22:01:18.000000 cfbd_json_py-0.1.1/cfbd_json_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 22:01:18.000000 cfbd_json_py-0.1.1/cfbd_json_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-24 22:01:18.000000 cfbd_json_py-0.1.1/cfbd_json_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-24 22:01:18.000000 cfbd_json_py-0.1.1/cfbd_json_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-24 22:01:00.000000 cfbd_json_py-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 22:01:18.794014 cfbd_json_py-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:38:11.155919 cfbd_json_py-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-12 00:38:11.155919 cfbd_json_py-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:38:11.155919 cfbd_json_py-0.1.2/cfbd_json_py/
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/_early_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17245 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/betting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/coaches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/conferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/draft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22951 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/drives.py
+-rw-r--r--   0 runner    (1001) docker     (127)   157032 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/games.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93878 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91135 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/players.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44340 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/plays.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/rankings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50160 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33561 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/recruiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70247 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41330 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/utls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/cfbd_json_py/venues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:38:11.155919 cfbd_json_py-0.1.2/cfbd_json_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-12 00:38:11.000000 cfbd_json_py-0.1.2/cfbd_json_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 00:38:11.000000 cfbd_json_py-0.1.2/cfbd_json_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:38:11.000000 cfbd_json_py-0.1.2/cfbd_json_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-12 00:38:11.000000 cfbd_json_py-0.1.2/cfbd_json_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 00:38:11.000000 cfbd_json_py-0.1.2/cfbd_json_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-12 00:37:58.000000 cfbd_json_py-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:38:11.155919 cfbd_json_py-0.1.2/setup.cfg
```

### Comparing `cfbd_json_py-0.1.1/LICENSE` & `cfbd_json_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cfbd_json_py-0.1.1/PKG-INFO` & `cfbd_json_py-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfbd_json_py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Allows users to access the CFBD API, and get the resulting data in either a dictionary (think JSON), or in a pandas DataFrame (think spreadsheet).
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/cfbd-json-py
 Project-URL: documentation, https://armstjc.github.io/cfbd-json-py/cfbd_json_py.html
 Project-URL: repository, https://github.com/armstjc/cfbd-json-py.git
```

### Comparing `cfbd_json_py-0.1.1/README.md` & `cfbd_json_py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/__init__.py` & `cfbd_json_py-0.1.2/cfbd_json_py/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: __init__.py
 # Purpose: Allows for the python package to function,
 #          by allowing you to to access functions within
 #          this package.
 ###############################################################################
 """
@@ -12,27 +12,27 @@
 
 To the left of this page are various endpoints for this python package.
 - `cfbd_json_py.betting`:
     Holds functions for betting lines and betting data from the CFBD API.
 - `cfbd_json_py.coaches`:
     Holds functions for you to get coaching data (past and present).
 - `cfbd_json_py.conferences`:
-    Holds functions for you to get information for CFB confrences.
+    Holds functions for you to get information for CFB conferences.
 - `cfbd_json_py.draft`:
     Holds functions for you to get NFL draft information/data for
     various players in the CFBD API
 - `cfbd_json_py.drives`:
     Holds functions for you to get data for offensive and/or defensive drives
     within the CFBD API.
 - `cfbd_json_py.games`:
-    Holds functions for you to get various datapoints pertaining to
+    Holds functions for you to get various data points pertaining to
     actual CFB games within the CFBD API.
 - `cfbd_json_py.metrics`:
     Holds functions to allow you to calculate
-    or retrive various advanced metrics
+    or retrieve various advanced metrics
     from the CFBD API.
 - `cfbd_json_py.players`:
     Holds functions for you to get various
     data endpoints related to player stats,
     player information, and player data.
 - `cfbd_json_py.plays`:
     Holds functions for play-by-play (PBP) data for CFB games,
@@ -40,15 +40,15 @@
 - `cfbd_json_py.rankings`:
     Holds functions for various CFB team ranking polls,
     and their results.
 - `cfbd_json_py.ratings`:
     Holds functions to allow you to get various team ratings data
     (like SP+, SRS, and Elo team ratings) from the CFBD API.
 - `cfbd_json_py.recruiting`:
-    Holds functions for you to access CFB recruting data and information,
+    Holds functions for you to access CFB recruiting data and information,
     as well as team and player ratings for recruiting.
 - `cfbd_json_py.stats`:
     Holds functions for you to get various team stats from the CFBD API.
 - `cfbd_json_py.teams`:
     Holds functions for you to get team information and data,
     as well as head-to-head records and matchup history.
 - `cfbd_json_py.utls`:
@@ -60,15 +60,15 @@
     various venues/stadiums within the college football world.
 
 # Basic Setup
 
 If you have a CFBD API key,
 you have three ways to set it for this python package to use:
 1. Declare the API key as a string variable
-    in a python script (not reccomended, extreme security risk).
+    in a python script (not recommended, extreme security risk).
 2. Declare the API key in your environment as `CFBD_API_KEY`.
     - `cfbd_json_py` will first look for your environment,
     if you don't declare the API key as a string variable,
     when calling any function in this python package that uses a CFBD API call.
     - If you're using GitHub Actions with this package,
     just set a repository secret with the name `CFBD_API_KEY`.
     Again, this package will automatically know where to look,
@@ -83,15 +83,15 @@
 from cfbd_api_key.utls import set_cfbd_api_token
 
 cfbd_api_key = "TigersAreAwesome" # replace this with your actual API key
 set_cfbd_api_token(api_key=cfbd_api_key)
 ```
 
 > **NOTE:** *In a future version,
-    there will be an executable application seperate from this package
+    there will be an executable application separate from this package
     for Windows, Mac, and Linux users to effectively do the same thing
     as the above code block, but with a graphical user interface (GUI).*
 
 If you want to see how to use this
 python package after setting up your API key,
 click on one of the submodules on the left
 to view the various functions within each submodule.
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/_early_access.py` & `cfbd_json_py-0.1.2/cfbd_json_py/_early_access.py`

 * *Files identical despite different names*

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/betting.py` & `cfbd_json_py-0.1.2/cfbd_json_py/betting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: betting.py
 # Purpose: Houses functions pertaining to betting data within the CFBD API.
 ###############################################################################
 """
 
 import warnings
@@ -31,22 +31,22 @@
     home: str = None,
     away: str = None,
     # cache_data: bool = False,
     # cache_dir: str = None,
     return_as_dict: bool = False,
 ):
     """
-    Retrives betting information from the CFBD API for a given season,
+    Retrieves betting information from the CFBD API for a given season,
     or you could only get betting information for a single game.
 
     Parameters
     ----------
 
     `season` (int, mandatory):
-        The season you want to retrive betting information from.
+        The season you want to retrieve betting information from.
 
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
         from the python environment, or from a file on this computer.
         If `api_key` is not null,
         this function will automatically assume that the
@@ -62,24 +62,24 @@
         this function will assume that `api_key_dir` is a directory,
         and will try to find a CFBD API key file in that directory.
 
     `game_id` (int, optional):
         Optional argument.
         If `game_id` is set to a game ID,
         `get_cfb_betting_lines()` will try to get
-        all betting informaiton for that game ID.
+        all betting information for that game ID.
 
     `week` (int, optional):
         Optional argument.
         If `week` is set to an integer, this function will attempt
         to load betting data from games in that season, and that week.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want postseason betting data, set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `team` (str, optional):
         Optional argument.
         If you only want betting information for a team,
@@ -101,17 +101,17 @@
         where that team was the away team in this season,
         set `away_team` to the name of the team
         you want game-level betting data from.
 
     `conference` (str, optional):
         Optional argument.
         If you only want betting information from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
-        of the conference you want betting informaiton from.
+        of the conference you want betting information from.
 
     `year` (int):
         Alternative keyword for `season`
 
     `home` (str):
         Alternative keyword for `home_team`
 
@@ -128,17 +128,17 @@
     Usage
     ----------
     ```
     import time
 
     from cfbd_json_py.betting import get_cfbd_betting_lines
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared " +
             "in this script for this example."
         )
 
 
         # Get all available betting info for the 2020 CFB season, in week 2.
@@ -248,15 +248,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get all available betting info for the 2020 CFB season, in week 2.
         print(
             "Get all available betting info for the 2020 CFB season, " +
             "in week 2."
@@ -398,24 +398,14 @@
             "Inconsistent inputs for `away` and `away_team`."
             + "\nPlease use either `away` OR `away_team` "
             + "when calling this function"
         )
     elif away is not None:
         away_team = away
 
-    # if conference is not None and conference is not None \
-    #     and (conferenceis notconference):
-    #     raise ValueError(
-    #         "Inconsistent inputs for `conference` and `conference`."+
-    #         "\nPlease use either `conference` OR `conference` "+
-    #         "when calling this function"
-    #     )
-    # elif conference is not None:
-    #     conference = conference
-
     del year, home, away
 
     if game_id is not None and season is not None:
         warnings.warn(
             "If you are getting betting information for a single game, "
             + "only set `game_id` to the game ID, " +
             "and leave `season` as `NULL`."
@@ -435,15 +425,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/coaches.py` & `cfbd_json_py-0.1.2/cfbd_json_py/coaches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: coaches.py
 # Purpose: Houses functions pertaining to coaching data within the CFBD API.
 ###############################################################################
 """
 
 import logging
@@ -26,15 +26,15 @@
     season: int = None,
     min_season: int = None,
     max_season: int = None,
     year: int = None,
     return_as_dict: bool = False,
 ):
     """
-    Retrives information from the CFBD API on CFB Head Coaches.
+    Retrieves information from the CFBD API on CFB Head Coaches.
 
     Parameters
     ----------
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
         from the python environment, or from a file on this computer.
@@ -97,17 +97,17 @@
     Usage
     ----------
     ```
     import time
 
     from cfbd_json_py.coaches import get_cfbd_coaches_info
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script "+
             "for this example."
         )
 
         # Getting all coaches in the 2020 CFB season
         print("Getting every coach in the 2020 CFB season.")
@@ -185,15 +185,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Getting every coach in the 2020 CFB season.
         print("Getting every coach in the 2020 CFB season.")
         json_data = get_cfbd_coaches_info(season=2020)
         print(json_data)
@@ -294,15 +294,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -323,23 +323,23 @@
                 + "set `min_season` and `max_season` to the range of seasons "
                 + "you want coaching information from."
             )
         elif season is not None and min_season is season:
             logging.warning(
                 "If you only want coaching information for a single season, "
                 + "and not for a range of seasons, only set `year` "
-                + "to the seaon you want coaching info for, "
+                + "to the season you want coaching info for, "
                 + "and leave `min_season` and `max_season` as `None` (NULL)."
             )
             min_season = None
         elif season is None:
             logging.warning(
                 "If you only want coaching information for a single season, "
                 + "and not for a range of seasons, only set `year` to "
-                + "the seaon you want coaching info for, "
+                + "the season you want coaching info for, "
                 + "and leave `min_season` and `max_season` as `None` (NULL)."
             )
             season = min_season
             min_season = None
 
     elif min_season is None and max_season is not None:
         if season is not None and max_season is not season:
@@ -356,23 +356,23 @@
                 + "set `min_season` and `max_season` to the range of seasons "
                 + "you want coaching information from."
             )
         elif season is not None and max_season == season:
             logging.warning(
                 "If you only want coaching information for "
                 + "a single season, and not for a range of seasons, "
-                + "only set `year` to the seaon you want coaching info for, "
+                + "only set `year` to the season you want coaching info for, "
                 + "and leave `min_season` and `max_season` as `None` (NULL)."
             )
             min_season = None
         elif season is None:
             logging.warning(
                 "If you only want coaching information for "
                 + "a single season, and not for a range of seasons, "
-                + "only set `year` to the seaon you want coaching info for, "
+                + "only set `year` to the season you want coaching info for, "
                 + "and leave `min_season` and `max_season` as `None` (NULL)."
             )
             season = max_season
             max_season = None
 
     if min_season is not None and max_season is not None:
         if season is not None:
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/conferences.py` & `cfbd_json_py-0.1.2/cfbd_json_py/conferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: conferences.py
 # Purpose: Houses functions pertaining to CFB conference data
     within the CFBD API.
 ###############################################################################
 """
 
@@ -14,15 +14,15 @@
 from cfbd_json_py.utls import get_cfbd_api_token
 
 
 def get_cfbd_conference_info(
     api_key: str = None, api_key_dir: str = None, return_as_dict: bool = False
 ):
     """
-    Retrives a list of CFB conferences from the CFBD API.
+    Retrieves a list of CFB conferences from the CFBD API.
 
     Parameters
     ----------
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
         from the python environment, or from a file on this computer.
@@ -50,24 +50,24 @@
     Usage
     ----------
     ```
     import time
 
     from cfbd_json_py.conferences import get_cfbd_conference_info
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
-        # Gets CFB confrence info from the CFBD API.
-        print("Gets CFB confrence info from the CFBD API.")
+        # Gets CFB conference info from the CFBD API.
+        print("Gets CFB conference info from the CFBD API.")
         json_data = get_cfbd_conference_info(api_key=cfbd_key)
         print(json_data)
         time.sleep(5)
 
         # You can also tell this function to just return the API call
         # as a Dictionary (read: JSON) object.
         print(
@@ -81,20 +81,20 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
-        # Gets CFB confrence info from the CFBD API.
-        print("Gets CFB confrence info from the CFBD API.")
+        # Gets CFB conference info from the CFBD API.
+        print("Gets CFB conference info from the CFBD API.")
         json_data = get_cfbd_conference_info()
         print(json_data)
         time.sleep(5)
 
         # You can also tell this function to just return the API call
         # as a Dictionary (read: JSON) object.
         print(
@@ -122,15 +122,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/draft.py` & `cfbd_json_py-0.1.2/cfbd_json_py/draft.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: draft.py
 # Purpose: Houses functions pertaining to NFL Draft data within the CFBD API.
 ###############################################################################
 """
 
 from datetime import datetime
@@ -17,15 +17,15 @@
 from cfbd_json_py.utls import get_cfbd_api_token
 
 
 def get_cfbd_nfl_teams(
     api_key: str = None, api_key_dir: str = None, return_as_dict: bool = False
 ):
     """
-    Retrives a list of NFL teams from the CFBD API.
+    Retrieves a list of NFL teams from the CFBD API.
 
     Parameters
     ----------
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
         from the python environment, or from a file on this computer.
@@ -53,17 +53,17 @@
     Usage
     ----------
     ```
     import time
 
     from cfbd_json_py.draft import get_cfbd_nfl_teams
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Gets NFL team info from the CFBD API.
         print("Gets NFL team info from the CFBD API.")
@@ -84,15 +84,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
         # Gets NFL team info from the CFBD API.
         print("Gets NFL team info from the CFBD API.")
         json_data = get_cfbd_nfl_teams()
         print(json_data)
@@ -126,15 +126,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -170,15 +170,15 @@
     return nfl_teams_df
 
 
 def get_cfbd_nfl_positions(
     api_key: str = None, api_key_dir: str = None, return_as_dict: bool = False
 ):
     """
-    Retrives a list of player positions for the NFL Draft from the CFBD API.
+    Retrieves a list of player positions for the NFL Draft from the CFBD API.
 
     Parameters
     ----------
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
         from the python environment, or from a file on this computer.
@@ -206,17 +206,17 @@
     Usage
     ----------
     ```
     import time
 
     from cfbd_json_py.draft import get_cfbd_nfl_positions
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Gets a list of player positions for the NFL Draft from the CFBD API.
         print(
@@ -240,15 +240,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
         # Gets a list of player positions for the NFL Draft from the CFBD API.
         print(
             "Gets a list of player positions for the NFL Draft " +
             "from the CFBD API."
@@ -284,15 +284,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -357,15 +357,15 @@
     college: str = None,
     conference: str = None,
     position: str = None,
     year: int = None,
     return_as_dict: bool = False,
 ):
     """
-    Retrives a list of actual NFL Draft selections from the CFBD API.
+    Retrieves a list of actual NFL Draft selections from the CFBD API.
 
     Parameters
     ----------
 
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
@@ -380,18 +380,18 @@
         If `api_key_dir` is null, and `api_key` is null,
         this function will try to find
         a CFBD API key file in this user's home directory.
         If `api_key_dir` is set to a string, and `api_key` is null,
         this function will assume that `api_key_dir` is a directory,
         and will try to find a CFBD API key file in that directory.
 
-    The following paramaters are optional,
-    but it is highly reccomended to not call this function
-    withiout settting one of these five optional paramaters
-    to a non-null value.
+    The following parameters are optional,
+    but it is highly recommended to not call this function
+    without declaring one of these five optional parameters
+    as a non-null value.
 
     `season` (int, semi-optional):
         Semi-Optional argument.
         This is the season you want NFL Draft information for.
         For example, if you only want data for the 2020 NFL Draft,
         set `season` to `2020`.
 
@@ -409,22 +409,22 @@
         set `college` to the name of that team.
         For example, if you want to only get NFL Draft information for
         draft picks from the Clemson Tigers Football Program,
         set `college` to `Clemson`.
 
     `conference` (str, optional):
         Semi-Optional argument.
-        If you only want NFL Draft selections from a specific CFB confrence,
-        set `conference` to the abbreviation of that confrence.
-        A list of CFBD API confrence abbreviations can be found
+        If you only want NFL Draft selections from a specific CFB conference,
+        set `conference` to the abbreviation of that conference.
+        A list of CFBD API conference abbreviations can be found
         in the `conference_abbreviation` column from
         the pandas DataFrame that is returned by calling
         `cfbd_json_py.conferences.get_cfbd_conference_info()`.
         For example, if you want to only get NFL Draft information for
-        draft picks that played in the Big 12, set `confrence` to `B12`.
+        draft picks that played in the Big 12, set `conference` to `B12`.
 
     `year` (int):
         Alternative keyword for `season`
 
     `position` (str, optional):
         Semi-Optional argument.
         If you only want NFL Draft selections who played a specific position,
@@ -444,17 +444,17 @@
     ----------
 
     ```
     import time
 
     from cfbd_json_py.draft import get_cfbd_nfl_draft_info
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get NFL Draft selections from the 2020 NFL Draft.
         print("Get NFL Draft selections from the 2020 NFL Draft.")
@@ -490,18 +490,19 @@
             season=2020,
             college="Clemson"
         )
         print(json_data)
         time.sleep(5)
 
         # Get NFL Draft selections from the 2020 NFL Draft made involving
-        # players who played in the Southeastern Confrence (SEC).
+        # players who played in the Southeastern conference (SEC).
         print(
             "Get NFL Draft selections from the 2020 NFL Draft made " +
-            "involving players who played in the Southeastern Confrence (SEC)."
+            "involving players who played " +
+            "in the Southeastern conference (SEC)."
         )
         json_data = get_cfbd_nfl_draft_info(
             api_key=cfbd_key,
             season=2020,
             conference="SEC"
         )
         print(json_data)
@@ -537,15 +538,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get NFL Draft selections from the 2020 NFL Draft.
         print("Get NFL Draft selections from the 2020 NFL Draft.")
         json_data = get_cfbd_nfl_draft_info(season=2020)
         print(json_data)
@@ -574,18 +575,19 @@
             season=2020,
             college="Clemson"
         )
         print(json_data)
         time.sleep(5)
 
         # Get NFL Draft selections from the 2020 NFL Draft made involving
-        # players who played in the Southeastern Confrence (SEC).
+        # players who played in the Southeastern conference (SEC).
         print(
             "Get NFL Draft selections from the 2020 NFL Draft made " +
-            "involving players who played in the Southeastern Confrence (SEC)."
+            "involving players who played " +
+            "in the Southeastern conference (SEC)."
         )
         json_data = get_cfbd_nfl_draft_info(
             season=2020,
             conference="SEC"
         )
         print(json_data)
         time.sleep(5)
@@ -648,15 +650,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -666,17 +668,18 @@
     if season is None \
             and nfl_team is None \
             and college is None \
             and conference is None:
 
         logging.warning(
             "Not specifying a `season`, `nfl_team`, `college`, "
-            + "or `confrence` will still result in "
+            + "or `conference` will still result in "
             + "a successful get request (assuming the API key is valid)"
-            + ", but this is not a recomended method of calling this function."
+            + ", but this is not a recommended method "
+            + "of calling this function."
         )
 
     if season < 1936 or season > now.year:
         raise ValueError(
             f"`season` must be an integer between 1936 and {now.year}.\n" +
             f"You entered:\n{season}"
         )
@@ -704,15 +707,15 @@
         url += f"?college={college}"
         url_elements += 1
     elif college is not None:
         url += f"&college={college}"
         url_elements += 1
 
     if conference is not None and url_elements == 0:
-        # conference = "SEC", not "Southeastern Confrence"
+        # conference = "SEC", not "Southeastern conference"
         url += f"?conference={conference}"
         url_elements += 1
     elif conference is not None:
         url += f"&conference={conference}"
         url_elements += 1
 
     if position is not None and url_elements == 0:
@@ -766,12 +769,12 @@
             "hometownInfo.countyFips": "player_hometown_county_fips",
         },
         inplace=True,
     )
     if len(nfl_draft_df) == 0:
         logging.error(
             "The CFBD API accepted your inputs, "
-            + "but found no data within your specified input paramaters."
-            + " Please double check your input paramaters."
+            + "but found no data within your specified input parameters."
+            + " Please double check your input parameters."
         )
 
     return nfl_draft_df
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/drives.py` & `cfbd_json_py-0.1.2/cfbd_json_py/drives.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: drives.py
 # Purpose: Houses functions pertaining to CFB drive data within the CFBD API.
 ###############################################################################
 """
 
 from datetime import datetime
@@ -32,15 +32,15 @@
     year: int = None,
     offense: str = None,
     defense: str = None,
     classification: str = None,
     return_as_dict: bool = False,
 ):
     """
-    Retrives a list of CFB drives from the CFBD API.
+    Retrieves a list of CFB drives from the CFBD API.
 
     Parameters
     ----------
     `season` (int, mandatory):
         Required argument.
         Specifies the season you want CFB drive information from.
         This must be specified, otherwise this package, and by extension
@@ -62,15 +62,15 @@
         a CFBD API key file in this user's home directory.
         If `api_key_dir` is set to a string, and `api_key` is null,
         this function will assume that `api_key_dir` is a directory,
         and will try to find a CFBD API key file in that directory.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB drive data for non-regular season games,
         set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `week` (int, optional):
         Optional argument.
@@ -94,67 +94,68 @@
         If you only want CFB drive data from a team, while they are on defense,
         regardless if they are the home/away team,
         set `team` to the name of the team you want CFB drive data from.
 
     `conference` (str, optional):
         Optional argument.
         If you only want CFB drive data from games
-        involving teams from a specific confrence,
+        involving teams from a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB drive data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `offensive_conference` (str, optional):
         Optional argument.
         If you only want CFB drive data from games
-        where the offensive team is from a specific confrenece,
+        where the offensive team is from a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB drive data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `defensive_conference` (str, optional):
         Optional argument.
         If you only want CFB drive data from games
-        where the defensive team is from a specific confrenece,
+        where the defensive team is from a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB drive data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `ncaa_division` (str, semi-optional):
         Semi-optional argument.
         By default, `ncaa_division` will be set to "fbs",
         short for the Football Bowl Subdivision (FBS),
         formerly known as D1-A (read as "division one single A"),
         the highest level in the NCAA football pyramid,
-        where teams can scolarship up to 85 players
-        on their football team soley for athletic ability,
+        where teams can scholarship up to 85 players
+        on their football team solely for athletic ability,
         and often have the largest athletics budgets
         within the NCAA.
 
         Other valid inputs are:
         - "fcs": Football Championship Subdivision (FCS),
             formerly known as D1-AA (read as "division one double A").
             An FCS school is still in the 1st division of the NCAA,
-            making them elligable for the March Madness tournament,
+            making them eligible for the March Madness tournament,
             but may not have the resources to compete at the FBS level
-            at this time. FCS schools are limited to 63 athletic scolarships
+            at this time. FCS schools are limited to 63 athletic scholarships
             for football.
         - "ii": NCAA Division II. Schools in this and D3 are not
-            elligable for the March Madness tournament,
-            and are limited to 36 athletic scolarships for their football team.
+            eligible for the March Madness tournament,
+            and are limited to 36 athletic scholarships
+            for their football team.
         - "iii": NCAA Division III. The largest single division within the
             NCAA football pyramid.
             D3 schools have the distinction of being part of
-            the only NCAA division that cannot give out scolarships soley
+            the only NCAA division that cannot give out scholarships solely
             for athletic ability.
 
     `offense` (str):
         Alternative keyword for `offensive_team`
 
     `defense` (str):
         Alternative keyword for `defensive_team`
@@ -172,17 +173,17 @@
     Usage
     ----------
     ```
     import time
 
     from cfbd_json_py.drives import get_cfbd_drives_info
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get CFB Drive data from the 2020 CFB season.
         print("Get CFB Drive data from the 2020 CFB season.")
@@ -287,15 +288,15 @@
             season=2020,
             defensive_conference="MAC"
         )
         print(json_data)
         time.sleep(5)
 
         # Get CFB Drive data from Football Championship Subdivision (FCS) games
-        # in week 3 ofthe 2020 CFB season,
+        # in week 3 of the 2020 CFB season,
         # where the MAC team was on offense.
         print(
             "Get CFB Drive data from games involving " +
             "the 2020 Ohio State Buckeyes Football Team, " +
             "when Ohio State was on defense."
         )
         json_data = get_cfbd_drives_info(
@@ -323,15 +324,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get CFB Drive data from the 2020 CFB season.
         print("Get CFB Drive data from the 2020 CFB season.")
         json_data = get_cfbd_drives_info(
             season=2020
@@ -426,15 +427,15 @@
             season=2020,
             defensive_conference="MAC"
         )
         print(json_data)
         time.sleep(5)
 
         # Get CFB Drive data from Football Championship Subdivision (FCS) games
-        # in week 3 ofthe 2020 CFB season,
+        # in week 3 of the 2020 CFB season,
         # where the MAC team was on offense.
         print(
             "Get CFB Drive data from games involving " +
             "the 2020 Ohio State Buckeyes Football Team, " +
             "when Ohio State was on defense."
         )
         json_data = get_cfbd_drives_info(
@@ -538,15 +539,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -666,12 +667,12 @@
             "elapsed.seconds": "elapsed_seconds",
         },
         inplace=True,
     )
     if len(cfb_drives_df) == 0:
         logging.error(
             "The CFBD API accepted your inputs, "
-            + "but found no data within your specified input paramaters."
-            + " Please double check your input paramaters."
+            + "but found no data within your specified input parameters."
+            + " Please double check your input parameters."
         )
 
     return cfb_drives_df
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/games.py` & `cfbd_json_py-0.1.2/cfbd_json_py/games.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: games.py
 # Purpose: Houses functions pertaining to CFB game data within the CFBD API.
 ###############################################################################
 """
 from datetime import datetime
 import logging
@@ -27,15 +27,15 @@
     away_team: str = None,
     conference: str = None,
     ncaa_division: str = "fbs",
     game_id: int = None,
     return_as_dict: bool = False,
 ):
     """
-    Retrives game schedule data from the CFBD API.
+    Retrieves game schedule data from the CFBD API.
 
     Parameters
     ----------
     `season` (int, mandatory):
         Required argument.
         Specifies the season you want CFB game information from.
         This must be specified, otherwise this package, and by extension
@@ -57,15 +57,15 @@
         a CFBD API key file in this user's home directory.
         If `api_key_dir` is set to a string, and `api_key` is null,
         this function will assume that `api_key_dir` is a directory,
         and will try to find a CFBD API key file in that directory.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB game information for non-regular season games,
         set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `week` (int, optional):
         Optional argument.
@@ -89,44 +89,45 @@
         If you only want game information for a team,
         where that team was the away team in this season,
         set `away_team` to the name of the team you want game information for.
 
     `conference` (str, optional):
         Optional argument.
         If you only want game information from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want game information from.
 
     `ncaa_division` (str, semi-optional):
         Semi-optional argument.
         By default, `ncaa_division` will be set to "fbs",
         short for the Football Bowl Subdivision (FBS),
         formerly known as D1-A (read as "division one single A"),
         the highest level in the NCAA football pyramid,
-        where teams can scolarship up to 85 players
-        on their football team soley for athletic ability,
+        where teams can scholarship up to 85 players
+        on their football team solely for athletic ability,
         and often have the largest athletics budgets
         within the NCAA.
 
         Other valid inputs are:
         - "fcs": Football Championship Subdivision (FCS),
             formerly known as D1-AA (read as "division one double A").
             An FCS school is still in the 1st division of the NCAA,
-            making them elligable for the March Madness tournament,
+            making them eligible for the March Madness tournament,
             but may not have the resources to compete at the FBS level
-            at this time. FCS schools are limited to 63 athletic scolarships
+            at this time. FCS schools are limited to 63 athletic scholarships
             for football.
         - "ii": NCAA Division II. Schools in this and D3 are not
-            elligable for the March Madness tournament,
-            and are limited to 36 athletic scolarships for their football team.
+            eligible for the March Madness tournament,
+            and are limited to 36 athletic scholarships
+            for their football team.
         - "iii": NCAA Division III. The largest single division within the
             NCAA football pyramid.
             D3 schools have the distinction of being part of
-            the only NCAA division that cannot give out scolarships soley
+            the only NCAA division that cannot give out scholarships solely
             for athletic ability.
 
     `game_id` (int, optional):
         Optional argument.
         If `game_id` is set to a game ID,
         `get_cfb_betting_lines()` will try to get
         game information just for that game ID.
@@ -142,17 +143,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.games import get_cfbd_games
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get CFB games from the 2020 CFB season.
         print("Get CFB games from the 2020 CFB season.")
@@ -226,18 +227,18 @@
             season=2018,
             away_team="Ohio"
         )
         print(json_data)
         time.sleep(5)
 
         # Get game information for the
-        # 2021 American Athletic Confrence (AAC) Championship Game.
+        # 2021 American Athletic conference (AAC) Championship Game.
         print(
             "Get game information for " +
-            "the 2021 American Athletic Confrence (AAC) Championship Game."
+            "the 2021 American Athletic conference (AAC) Championship Game."
         )
         json_data = get_cfbd_games(
             api_key=cfbd_key,
             season=2018,
             game_id=401331162
         )
         print(json_data)
@@ -259,15 +260,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get CFB games from the 2020 CFB season.
         print("Get CFB games from the 2020 CFB season.")
         json_data = get_cfbd_games(
             season=2020
@@ -346,18 +347,18 @@
             season=2018,
             away_team="Ohio"
         )
         print(json_data)
         time.sleep(5)
 
         # Get game information for the
-        # 2021 American Athletic Confrence (AAC) Championship Game.
+        # 2021 American Athletic conference (AAC) Championship Game.
         print(
             "Get game information for " +
-            "the 2021 American Athletic Confrence (AAC) Championship Game."
+            "the 2021 American Athletic conference (AAC) Championship Game."
         )
         json_data = get_cfbd_games(
             season=2018,
             game_id=401331162
         )
         print(json_data)
         time.sleep(5)
@@ -391,15 +392,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -511,20 +512,20 @@
 
     json_data = response.json()
 
     if return_as_dict is True:
         return json_data
 
     cfb_games_df = pd.json_normalize(json_data)
-    print(cfb_games_df.columns)
+    # print(cfb_games_df.columns)
     if len(cfb_games_df) == 0:
         logging.error(
             "The CFBD API accepted your inputs, "
-            + "but found no data within your specified input paramaters."
-            + " Please double check your input paramaters."
+            + "but found no data within your specified input parameters."
+            + " Please double check your input parameters."
         )
 
     return cfb_games_df
 
 
 def get_cfbd_team_records(
     api_key: str = None,
@@ -533,15 +534,15 @@
     team: str = None,  # Must specify either a year or team
     conference: str = None,
     return_as_dict: bool = False,
 ):
     """
     Get a team, or multiple team's record (wins, losses, ties)
     for home games, away games,
-    confrence games, and the team's record for that season.
+    conference games, and the team's record for that season.
 
     Parameters
     ----------
 
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
@@ -564,28 +565,28 @@
         Semi-optional argument.
         Specifies the season you want CFB team records data from.
         You MUST set `season` or `team` to a non-null value for
         this function to work. If you don't, a `ValueError()`
         will be raised.
 
     `team` (str, optional):
-        Semi-ptional argument.
+        Semi-optional argument.
         If you only want CFB team records data for a specific team,
         set `team` to the name of the team you want CFB drive data from.
         You MUST set `season` or `team` to a non-null value for
         this function to work. If you don't, a `ValueError()`
         will be raised.
 
     `conference` (str, optional):
         Optional argument.
         If you only want CFB team records data from games
-        involving teams from a specific confrence,
+        involving teams from a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB team records data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -596,17 +597,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.games import get_cfbd_team_records
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get CFB team records from the 2020 CFB season.
         print("Get CFB team records from the 2020 CFB season.")
@@ -627,18 +628,18 @@
             api_key=cfbd_key,
             team="Cincinnati"
         )
         print(json_data)
         time.sleep(5)
 
         # Get team records from football teams that played
-        # in the Big 10 (B1G) Confrence in the 2017 CFB season
+        # in the Big 10 (B1G) conference in the 2017 CFB season
         print(
             "Get team records from football teams that played " +
-            "in the Big 10 (B1G) Confrence in the 2017 CFB season"
+            "in the Big 10 (B1G) conference in the 2017 CFB season"
         )
         json_data = get_cfbd_team_records(
             api_key=cfbd_key,
             season=2017,
             conference="B1G"
         )
         print(json_data)
@@ -660,15 +661,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get CFB team records from the 2020 CFB season.
         print("Get CFB team records from the 2020 CFB season.")
         json_data = get_cfbd_team_records(
             season=2020
@@ -685,18 +686,18 @@
         json_data = get_cfbd_team_records(
             team="Cincinnati"
         )
         print(json_data)
         time.sleep(5)
 
         # Get team records from football teams that played
-        # in the Big 10 (B1G) Confrence in the 2017 CFB season
+        # in the Big 10 (B1G) conference in the 2017 CFB season
         print(
             "Get team records from football teams that played " +
-            "in the Big 10 (B1G) Confrence in the 2017 CFB season"
+            "in the Big 10 (B1G) conference in the 2017 CFB season"
         )
         json_data = get_cfbd_team_records(
             season=2017,
             conference="B1G"
         )
         print(json_data)
         time.sleep(5)
@@ -732,15 +733,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -751,15 +752,15 @@
         raise ValueError(f"`season` cannot be greater than {season}.")
     elif season is not None and season < 1869:
         raise ValueError("`season` cannot be less than 1869.")
 
     if season is None and team is None:
         raise ValueError(
             "If you call `cfbd_json_py.games.get_cfbd_team_records()`, "
-            + "you must specifiy at least a team or CFB season."
+            + "you must specify at least a team or CFB season."
         )
 
     # URL builder
     ##########################################################################
 
     url_elements = 0
 
@@ -842,25 +843,25 @@
 def get_cfbd_season_weeks(
     season: int,
     api_key: str = None,
     api_key_dir: str = None,
     return_as_dict: bool = False,
 ):
     """
-    Retrives a list of weeks that occured in a given CFB season.
+    Retrieves a list of weeks that occurred in a given CFB season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         Required argument.
-        Specifies the season you want a list of weeks that occured
+        Specifies the season you want a list of weeks that occurred
         in a given CFB season information from.
         This must be specified, otherwise this package, and by extension
         the CFBD API, will not accept the request
-        to get a list of weeks that occured in a given CFB season information.
+        to get a list of weeks that occurred in a given CFB season information.
 
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
         from the python environment, or from a file on this computer.
         If `api_key` is not null,
         this function will automatically assume that the
@@ -888,17 +889,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.games import get_cfbd_season_weeks
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get a list of weeks in the 2020 CFB season.
         print("Get a list of weeks in the 2020 CFB season.")
@@ -925,15 +926,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get a list of weeks in the 2020 CFB season.
         print("Get a list of weeks in the 2020 CFB season.")
         json_data = get_cfbd_season_weeks(
             season=2020
@@ -971,15 +972,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1083,18 +1084,18 @@
         a CFBD API key file in this user's home directory.
         If `api_key_dir` is set to a string, and `api_key` is null,
         this function will assume that `api_key_dir` is a directory,
         and will try to find a CFBD API key file in that directory.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB media information for non-regular season games,
         set `season_type` to "postseason".
-        If you want both "regular" and "postseason" games retunred,
+        If you want both "regular" and "postseason" games returned,
         set `season_type` to "both"
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `week` (int, optional):
         Optional argument.
         If `week` is set to an integer, this function will attempt
@@ -1106,64 +1107,65 @@
         If you only want CFB media information for a team,
         regardless if they are the home/away team,
         set `team` to the name of the team you want CFB media information from.
 
     `conference` (str, optional):
         Optional argument.
         If you only want media information from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want game information from.
 
     `media_type` (str, semi-optional):
         Semi-optional argument.
         If you only want game broadcast information
         for a specific type of broadcast,
         set this to the type of broadcast.
 
         Valid inputs are:
         - `all` (default): Returns all games,
             and all known broadcasters for those games.
         - `tv`: Returns all known TV broadcasters for CFB games
-            in the requested timeframe.
+            in the requested time frame.
         - `radio`: Returns all known radio broadcasters
-            for CFB games in the requested timeframe.
+            for CFB games in the requested time frame.
         - `web`: Returns all known web broadcasts (like ESPN+)
-            for CFB games in the requested timeframe.
+            for CFB games in the requested time frame.
         - `ppv`: Returns all known Pay Per View (PPV) broadcasts
-            for CFB games in the requested timeframe.
+            for CFB games in the requested time frame.
         - `mobile`: Returns all known broadcasters that only broadcasted
             games on mobile devices (?)
 
     `ncaa_division` (str, semi-optional):
         Semi-optional argument.
         By default, `ncaa_division` will be set to "fbs",
         short for the Football Bowl Subdivision (FBS),
         formerly known as D1-A (read as "division one single A"),
         the highest level in the NCAA football pyramid,
-        where teams can scolarship up to 85 players
-        on their football team soley for athletic ability,
+        where teams can scholarship up to 85 players
+        on their football team solely for athletic ability,
         and often have the largest athletics budgets
         within the NCAA.
 
         Other valid inputs are:
         - "fcs": Football Championship Subdivision (FCS),
             formerly known as D1-AA (read as "division one double A").
             An FCS school is still in the 1st division of the NCAA,
-            making them elligable for the March Madness tournament,
+            making them eligible for the March Madness tournament,
             but may not have the resources to compete at the FBS level
-            at this time. FCS schools are limited to 63 athletic scolarships
+            at this time. FCS schools are limited to 63 athletic scholarships
             for football.
         - "ii": NCAA Division II. Schools in this and D3 are not
-            elligable for the March Madness tournament,
-            and are limited to 36 athletic scolarships for their football team.
+            eligible for the March Madness tournament,
+            and are limited to 36 athletic scholarships
+            for their football team.
         - "iii": NCAA Division III. The largest single division within the
             NCAA football pyramid.
             D3 schools have the distinction of being part of
-            the only NCAA division that cannot give out scolarships soley
+            the only NCAA division that cannot give out scholarships solely
             for athletic ability.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
         instead of a pandas `DataFrame` object,
@@ -1173,17 +1175,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.games import get_cfbd_game_media_info
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get a media information for the 2020 CFB season.
         print("Get a media information for the 2020 CFB season.")
@@ -1227,19 +1229,19 @@
             season=2020,
             team="Ohio State"
         )
         print(json_data)
         time.sleep(5)
 
         # Get all known radio broadcasters for games played by teams
-        # within the American Athletic Confrence (AAC)
+        # within the American Athletic conference (AAC)
         # in the the 2021 CFB season.
         print(
             "Get all known radio broadcasters for games played " +
-            "by teams within the American Athletic Confrence (AAC) " +
+            "by teams within the American Athletic conference (AAC) " +
             "in the the 2021 CFB season."
         )
         json_data = get_cfbd_game_media_info(
             api_key=cfbd_key,
             season=2020,
             conference="AAC"
         )
@@ -1291,15 +1293,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get a media information for the 2020 CFB season.
         print("Get a media information for the 2020 CFB season.")
         json_data = get_cfbd_game_media_info(
             season=2020
@@ -1337,19 +1339,19 @@
             season=2020,
             team="Ohio State"
         )
         print(json_data)
         time.sleep(5)
 
         # Get all known radio broadcasters for games played by teams
-        # within the American Athletic Confrence (AAC)
+        # within the American Athletic conference (AAC)
         # in the the 2021 CFB season.
         print(
             "Get all known radio broadcasters for games played " +
-            "by teams within the American Athletic Confrence (AAC) " +
+            "by teams within the American Athletic conference (AAC) " +
             "in the the 2021 CFB season."
         )
         json_data = get_cfbd_game_media_info(
             season=2020,
             conference="AAC"
         )
         print(json_data)
@@ -1414,15 +1416,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1587,15 +1589,15 @@
     # `week`, `team`, and/or `conference`
     # must be not null for this function to work.
     stat_category: str = None,
     game_id: int = None,
     return_as_dict: bool = False,
 ):
     """
-    Retrives player game stats for a given time frame.
+    Retrieves player game stats for a given time frame.
 
     Parameters
     ----------
     `season` (int, mandatory):
         Required argument.
         Specifies the season you want CFB player game stats from.
         This must be specified, otherwise this package, and by extension
@@ -1617,15 +1619,15 @@
         a CFBD API key file in this user's home directory.
         If `api_key_dir` is set to a string, and `api_key` is null,
         this function will assume that `api_key_dir` is a directory,
         and will try to find a CFBD API key file in that directory.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB player game stats for non-regular season games,
         set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     **For the following three variables,
     at least one must be set to
@@ -1642,15 +1644,15 @@
         If you only want CFB player game stats for a team,
         regardless if they are the home/away team,
         set `team` to the name of the team you want CFB player game stats from.
 
     `conference` (str, optional):
         Optional argument.
         If you only want player game stats from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want stats from.
 
     `stat_category` (str, optional):
         Optional argument.
         If only want stats for a specific stat category,
         set this variable to that category.
@@ -1666,15 +1668,15 @@
         - `kicking`
         - `kickReturns`
         - `puntReturns`
 
     `game_id` (int, optional):
         Optional argument.
         If `game_id` is set to a game ID, `get_cfbd_player_game_stats()`
-        will try to getplayer game stats just for that game ID.
+        will try to get player game stats just for that game ID.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
         instead of a pandas `DataFrame` object,
         set `return_as_dict` to `True`.
@@ -1683,17 +1685,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.games import get_cfbd_player_game_stats
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get player game stats for week 10 of the 2020 CFB season.
         print("Get player game stats for week 10 of the 2020 CFB season.")
@@ -1713,18 +1715,18 @@
             season_type="postseason",
             week=1
         )
         print(json_data)
         time.sleep(5)
 
         # Get player game stats for
-        # the Alabma Crimson Tide Football Team for the 2018 CFB season.
+        # the Alabama Crimson Tide Football Team for the 2018 CFB season.
         print(
             "Get player game stats for " +
-            "the Alabma Crimson Tide Football Team for the 2018 CFB season."
+            "the Alabama Crimson Tide Football Team for the 2018 CFB season."
         )
         json_data = get_cfbd_player_game_stats(
             api_key=cfbd_key,
             season=2018,
             team="Alabama"
         )
         print(json_data)
@@ -1750,15 +1752,15 @@
             "Get get passing stats from players who played " +
             "in week 7 of the 2017 CFB season."
         )
         json_data = get_cfbd_player_game_stats(
             api_key=cfbd_key,
             season=2017,
             week=7,
-            stat_category="pasing"
+            stat_category="passing"
         )
         print(json_data)
         time.sleep(5)
 
         # Get player game stats from the 2021 Virbo Citrus Bowl,
         # a bowl game that happened in the 2020 CFB season.
         print(
@@ -1789,15 +1791,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get player game stats for week 10 of the 2020 CFB season.
         print("Get player game stats for week 10 of the 2020 CFB season.")
         json_data = get_cfbd_player_game_stats(
             season=2020,
@@ -1813,18 +1815,18 @@
             season_type="postseason",
             week=1
         )
         print(json_data)
         time.sleep(5)
 
         # Get player game stats for
-        # the Alabma Crimson Tide Football Team for the 2018 CFB season.
+        # the Alabama Crimson Tide Football Team for the 2018 CFB season.
         print(
             "Get player game stats for " +
-            "the Alabma Crimson Tide Football Team for the 2018 CFB season."
+            "the Alabama Crimson Tide Football Team for the 2018 CFB season."
         )
         json_data = get_cfbd_player_game_stats(
             season=2018,
             team="Alabama"
         )
         print(json_data)
         time.sleep(5)
@@ -1898,15 +1900,15 @@
     cfb_games_df = pd.DataFrame()
     row_df = pd.DataFrame()
     url = "https://api.collegefootballdata.com/games/players"
     stat_columns = [
         "season",
         "game_id",
         "team_name",
-        "team_confrence",
+        "team_conference",
         "player_id",
         "player_name",
         "home_away",
         # PASS
         "passing_C/ATT",
         "passing_COMP",
         "passing_ATT",
@@ -1978,15 +1980,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -2130,15 +2132,15 @@
         return json_data
 
     for game in tqdm(json_data):
         game_id = game["id"]
 
         for team in game["teams"]:
             team_name = team["school"]
-            team_confrence = team["conference"]
+            team_conference = team["conference"]
             home_away = team["homeAway"]
 
             for s_category in team["categories"]:
                 if s_category["name"] == "passing":
                     for stat in s_category["types"]:
                         if stat["name"] == "C/ATT":  # passing_C/ATT
                             for i in stat["athletes"]:
@@ -2149,16 +2151,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2174,16 +2176,16 @@
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id][
                                     "game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2198,16 +2200,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2222,16 +2224,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2246,16 +2248,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2273,16 +2275,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2304,16 +2306,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2328,16 +2330,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2352,16 +2354,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2376,16 +2378,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2400,16 +2402,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2431,16 +2433,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2455,16 +2457,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2479,16 +2481,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2503,16 +2505,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2527,16 +2529,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2558,16 +2560,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2582,16 +2584,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2606,16 +2608,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2637,16 +2639,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2661,16 +2663,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2685,16 +2687,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2709,16 +2711,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2734,16 +2736,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2758,16 +2760,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2782,16 +2784,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2813,16 +2815,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2838,16 +2840,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2863,16 +2865,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2895,16 +2897,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2919,16 +2921,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2943,16 +2945,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2967,16 +2969,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -2991,16 +2993,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3015,16 +3017,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3046,16 +3048,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3070,16 +3072,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3094,16 +3096,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3118,16 +3120,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3142,16 +3144,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3166,16 +3168,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3197,16 +3199,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3221,16 +3223,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3245,16 +3247,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3269,16 +3271,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3293,16 +3295,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3325,16 +3327,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3349,16 +3351,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3373,16 +3375,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3397,16 +3399,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3421,16 +3423,16 @@
                                 if rebuilt_json.get(player_id) is None:
                                     rebuilt_json[player_id] = {}
 
                                 rebuilt_json[player_id]["game_id"] = game_id
                                 rebuilt_json[player_id][
                                     "team_name"] = team_name
                                 rebuilt_json[player_id][
-                                    "team_confrence"
-                                ] = team_confrence
+                                    "team_conference"
+                                ] = team_conference
                                 rebuilt_json[player_id][
                                     "player_id"] = player_id
                                 rebuilt_json[player_id][
                                     "player_name"] = player_name
                                 rebuilt_json[player_id][
                                     "home_away"] = home_away
                                 rebuilt_json[player_id][
@@ -3485,15 +3487,15 @@
 
     elif filter_by_stat_category is True and stat_category == "passing":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # PASS
                 "passing_C/ATT",
                 "passing_COMP",
                 "passing_ATT",
@@ -3507,15 +3509,15 @@
 
     elif filter_by_stat_category is True and stat_category == "rushing":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # RUSH
                 "rushing_CAR",
                 "rushing_YDS",
                 "rushing_AVG",
@@ -3526,15 +3528,15 @@
 
     elif filter_by_stat_category is True and stat_category == "receiving":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # REC
                 "receiving_REC",
                 "receiving_YDS",
                 "receiving_AVG",
@@ -3545,15 +3547,15 @@
 
     elif filter_by_stat_category is True and stat_category == "fumbles":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # FUM
                 "fumbles_FUM",
                 "fumbles_LOST",
                 "fumbles_REC",
@@ -3562,15 +3564,15 @@
 
     elif filter_by_stat_category is True and stat_category == "defensive":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # DEFENSE
                 "defensive_TOT",
                 "defensive_SOLO",
                 "defensive_TFL",
@@ -3583,15 +3585,15 @@
 
     elif filter_by_stat_category is True and stat_category == "interceptions":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # INT
                 "interceptions_INT",
                 "interceptions_YDS",
                 "interceptions_TD",
@@ -3600,15 +3602,15 @@
 
     elif filter_by_stat_category is True and stat_category == "punting":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # PUNT
                 "punting_NO",
                 "punting_YDS",
                 "punting_AVG",
@@ -3620,15 +3622,15 @@
 
     elif filter_by_stat_category is True and stat_category == "kicking":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # KICK
                 "kicking_FG",
                 "kicking_FGM",
                 "kicking_FGA",
@@ -3643,15 +3645,15 @@
 
     elif filter_by_stat_category is True and stat_category == "kickReturns":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # KR
                 "kickReturns_NO",
                 "kickReturns_YDS",
                 "kickReturns_AVG",
@@ -3662,15 +3664,15 @@
 
     elif filter_by_stat_category is True and stat_category == "puntReturns":
         cfb_games_df = cfb_games_df[
             [
                 "season",
                 "game_id",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 "home_away",
                 # KR
                 "puntReturns_NO",
                 "puntReturns_YDS",
                 "puntReturns_AVG",
@@ -3685,15 +3687,15 @@
 def get_cfbd_player_advanced_game_stats(
     game_id: int,
     api_key: str = None,
     api_key_dir: str = None,
     return_as_dict: bool = False,
 ):
     """
-    Retrives advanced game stats from the CFBD API.
+    Retrieves advanced game stats from the CFBD API.
 
     Parameters
     ----------
     `game_id` (int, mandatory):
         Mandatory requirement.
         Specifies the game you want advanced game stats from.
 
@@ -3726,17 +3728,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.games import get_cfbd_player_advanced_game_stats
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key is not "tigersAreAwsome":
+    if cfbd_key is not "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get advanced player stats for a 2019 CFB game
         # between the LSU Tigers Football Program,
@@ -3769,15 +3771,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get advanced player stats for a 2019 CFB game
         # between the LSU Tigers Football Program,
         # and the Oklahoma Sooners Football Program.
         print(
@@ -3823,15 +3825,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -3956,15 +3958,15 @@
     adv_stats_df["game_excitement_score"] = game_excitement_score
 
     return adv_stats_df
 
 
 ###############################################################################
 # Patreon Only Functions.
-#   No cacheing, because the entire point of these functions are to get people
+#   No caching, because the entire point of these functions are to get people
 #   data ASAP, and right before kickoff.
 ###############################################################################
 
 
 def get_cfbd_live_scoreboard(
     api_key: str = None,
     api_key_dir: str = None,
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/metrics.py` & `cfbd_json_py-0.1.2/cfbd_json_py/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: metrics.py
 # Purpose: Houses functions pertaining to various CFB
     stats within the CFBD API.
 ###############################################################################
 """
 
@@ -44,15 +44,15 @@
         Mandatory argument.
         This is the down (a number between 1 and 4 in normal situations)
         for this play you want PPA for.
 
     `distance` (int, mandatory):
         Mandatory argument.
         This variable should be set to the number of yards between
-        the line of scrimage (LOS), and the first down line on the field.
+        the line of scrimmage (LOS), and the first down line on the field.
 
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
         from the python environment, or from a file on this computer.
         If `api_key` is not null,
         this function will automatically assume that the
@@ -78,17 +78,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.metrics import get_cfbd_predicted_ppa_from_down_distance
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared " +
             "in this script for this example."
         )
 
         # Get the predicted PPA for a 1st and 10 play,
         # in every possible situation.
@@ -121,15 +121,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
 
         # Get the predicted PPA for a 1st and 10 play,
         # in every possible situation.
         print(
@@ -156,17 +156,17 @@
             return_as_dict=True
         )
         print(json_data)
 
     ```
     Returns
     ----------
-    A pandas `DataFrame` object with a calculated PPA from a dwon and distance,
+    A pandas `DataFrame` object with a calculated PPA from a down and distance,
     or (if `return_as_dict` is set to `True`)
-    a dictionary object with a calculated PPA from a dwon and distance.
+    a dictionary object with a calculated PPA from a down and distance.
 
 
     """
 
     ppa_df = pd.DataFrame()
     url = "https://api.collegefootballdata.com/ppa/predicted"
 
@@ -174,15 +174,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -283,15 +283,15 @@
     exclude_garbage_time: bool = False,
     return_as_dict: bool = False,
 ):
     """
     Allows you to get team PPA data,
     over an entire season,
     with or without garbage time plays,
-    for a specificed team and/or time period.
+    for a specified team and/or time period.
 
     PPA is the CFBD API's equivalent metric to Expected Points Added (EPA).
 
     Parameters
     ----------
     `api_key` (str, optional):
         Semi-optional argument.
@@ -315,28 +315,28 @@
         Semi-optional argument.
         Specifies the season you want team PPA data from.
         You MUST set `season` or `team` to a non-null value for
         this function to work. If you don't, a `ValueError()`
         will be raised.
 
     `team` (str, optional):
-        Semi-ptional argument.
+        Semi-optional argument.
         If you only want team PPA data for a specific team,
         set `team` to the name of the team you want team PPA data from.
         You MUST set `season` or `team` to a non-null value for
         this function to work. If you don't, a `ValueError()`
         will be raised.
 
     `conference` (str, optional):
         Optional argument.
         If you only want team PPA data from games
-        involving teams from a specific confrence,
+        involving teams from a specific conference,
         set `conference` to the abbreviation
         of the conference you want team PPA data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `exclude_garbage_time` (bool, optional):
         Optional argument.
         If you want to filter out plays
         where the result of the game is largely decided,
@@ -355,17 +355,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.metrics import get_cfbd_team_season_ppa_data
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get team season PPA data for the 2020 CFB season.
         print("Get team PPA data for the 2020 CFB season.")
@@ -431,15 +431,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
         # Get team season PPA data for the 2020 CFB season.
         print("Get team PPA data for the 2020 CFB season.")
         json_data = get_cfbd_team_season_ppa_data(
             season=2020
@@ -514,15 +514,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -647,15 +647,15 @@
     season_type: str = "regular",  # "regular" or "postseason"
     return_as_dict: bool = False,
 ):
     """
     Allows you to get team PPA data,
     at a game level,
     with or without garbage time plays,
-    for a specificed team and/or time period.
+    for a specified team and/or time period.
 
     PPA is the CFBD API's equivalent metric to Expected Points Added (EPA).
 
     Parameters
     ----------
     `season` (int, mandatory):
         Required argument.
@@ -692,29 +692,29 @@
         If you only want team game PPA data for a team,
         regardless if they are the home/away team,
         set `team` to the name of the team you want team game PPA data from.
 
     `conference` (str, optional):
         Optional argument.
         If you only want team game PPA data from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want team game PPA data from.
 
     `exclude_garbage_time` (bool, optional):
         Optional argument.
         If you want to filter out plays where
         the result of the game is largely decided,
         set `exclude_garbage_time = True`.
         Default behavior is that this variable is set to
         `False` when this function is called.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want team game PPA data for non-regular season games,
         set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
@@ -727,17 +727,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.metrics import get_cfbd_team_game_ppa_data
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get team PPA data for individual games within the 2020 CFB season.
         print(
@@ -834,15 +834,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into this " +
+            "Using the user's API key supposedly loaded into this " +
             "python environment for this example."
         )
 
         # Get team PPA data for individual games within the 2020 CFB season.
         print(
             "Get team PPA data for individual games " +
             "within the 2020 CFB season."
@@ -946,15 +946,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1086,15 +1086,15 @@
     season_type: str = "regular",  # "regular" or "postseason"
     return_as_dict: bool = False,
 ):
     """
     Allows you to get player PPA data,
     at a game level,
     with or without garbage time plays,
-    for a specificed time period and/or team.
+    for a specified time period and/or team.
 
     PPA is the CFBD API's equivalent metric to Expected Points Added (EPA).
 
     Parameters
     ----------
 
     `api_key` (str, optional):
@@ -1163,15 +1163,15 @@
         the result of the game is largely decided,
         set `exclude_garbage_time = True`.
         Default behavior is that this variable is set to
         `False` when this function is called.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want player game PPA data for non-regular season games,
         set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
@@ -1184,17 +1184,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.metrics import get_cfbd_player_game_ppa_data
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get player game PPA data for week 10 of the 2020 CFB season.
         print("Get player game PPA data for week 10 of the 2020 CFB season.")
@@ -1296,15 +1296,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
         # Get player game PPA data for week 10 of the 2020 CFB season.
         print("Get player game PPA data for week 10 of the 2020 CFB season.")
         json_data = get_cfbd_player_game_ppa_data(
             season=2020,
@@ -1412,15 +1412,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1588,15 +1588,15 @@
     exclude_garbage_time: bool = False,
     return_as_dict: bool = False,
 ):
     """
     Allows you to get player PPA data,
     at a season level,
     with or without garbage time plays,
-    for a specificed time period and/or team.
+    for a specified time period and/or team.
 
     PPA is the CFBD API's equivalent metric to Expected Points Added (EPA).
 
     Parameters
     ----------
 
     `api_key` (str, optional):
@@ -1633,18 +1633,18 @@
         you want player season PPA data from.
         `week` and/or `team` must be set to a non-null value for this function
         to work.
 
     `conference` (str, optional):
         Optional argument.
         If you only want player season PPA data from games
-        involving teams from a specific confrence,
+        involving teams from a specific conference,
         set `conference` to the abbreviation
         of the conference you want player season PPA data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `position` (str, optional):
         Optional argument.
         If you only want player season PPA data
         for players of a specific position,
@@ -1683,17 +1683,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.metrics import get_cfbd_player_season_ppa_data
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get player season PPA data for the 2020 CFB season.
         print("Get player season PPA data for the 2020 CFB season.")
@@ -1753,19 +1753,19 @@
             player_id=3915511
         )
         print(json_data)
         time.sleep(5)
 
         # Get player season PPA data from
         # former Ohio State and LSU QB Joe Burrow (player ID #3915511),
-        # but exclude plays that occured in garbage time.
+        # but exclude plays that occurred in garbage time.
         print(
             "Get player season PPA data from former " +
             "Ohio State and LSU QB Joe Burrow (player ID #3915511), " +
-            "but exclude plays that occured in garbage time."
+            "but exclude plays that occurred in garbage time."
         )
         json_data = get_cfbd_player_season_ppa_data(
             api_key=cfbd_key,
             player_id=3915511,
             exclude_garbage_time=True
         )
         print(json_data)
@@ -1800,15 +1800,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
         # Get player season PPA data for the 2020 CFB season.
         print("Get player season PPA data for the 2020 CFB season.")
         json_data = get_cfbd_player_season_ppa_data(
             season=2020
@@ -1861,19 +1861,19 @@
             player_id=3915511
         )
         print(json_data)
         time.sleep(5)
 
         # Get player season PPA data from
         # former Ohio State and LSU QB Joe Burrow (player ID #3915511),
-        # but exclude plays that occured in garbage time.
+        # but exclude plays that occurred in garbage time.
         print(
             "Get player season PPA data from former " +
             "Ohio State and LSU QB Joe Burrow (player ID #3915511), " +
-            "but exclude plays that occured in garbage time."
+            "but exclude plays that occurred in garbage time."
         )
         json_data = get_cfbd_player_season_ppa_data(
             player_id=3915511,
             exclude_garbage_time=True
         )
         print(json_data)
         time.sleep(5)
@@ -1920,15 +1920,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -2063,15 +2063,15 @@
 def get_cfbd_game_win_probability_data(
     game_id: int,
     api_key: str = None,
     api_key_dir: str = None,
     return_as_dict: bool = False,
 ):
     """
-    Allows one to get win probabliity data for a given game ID.
+    Allows one to get win probability data for a given game ID.
 
     Parameters
     ----------
 
     `game_id` (int, mandatory):
         Mandatory argument.
         This is the game ID for the game you want win probability data from,
@@ -2106,40 +2106,40 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.metrics import get_cfbd_game_win_probability_data
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
-        # Get the win probablility data for a 2017 game between
+        # Get the win probability data for a 2017 game between
         # the University of Cincinnati and UConn (game ID #400941851).
         print(
-            "Get the win probablility data for a 2017 game between " +
+            "Get the win probability data for a 2017 game between " +
             "the University of Cincinnati and UConn (game ID #400941851)."
         )
         json_data = get_cfbd_game_win_probability_data(
             api_key=cfbd_key,
             game_id=400941851
         )
         print(json_data)
         time.sleep(5)
 
-        # Get the win probablility data for a 2023 game between
+        # Get the win probability data for a 2023 game between
         # the University of Duke and
         # the University of Louisville (game ID #401525535).
         print(
-            "Get the win probablility data for a 2023 game between " +
+            "Get the win probability data for a 2023 game between " +
             "the University of Duke and " +
             "the University of Louisville (game ID #401525535)."
         )
         json_data = get_cfbd_game_win_probability_data(
             api_key=cfbd_key,
             game_id=401525535
         )
@@ -2162,35 +2162,35 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
-        # Get win probablility data for a 2017 game between
+        # Get win probability data for a 2017 game between
         # the University of Cincinnati and UConn (game ID #400941851).
         print(
-            "Get the win probablility data for a 2017 game between " +
+            "Get the win probability data for a 2017 game between " +
             "the University of Cincinnati and UConn (game ID #400941851)."
         )
         json_data = get_cfbd_game_win_probability_data(
             game_id=400941851
         )
         print(json_data)
         time.sleep(5)
 
-        # Get win probablility data for a 2023 game between
+        # Get win probability data for a 2023 game between
         # the University of Duke and
         # the University of Louisville (game ID #401525535).
         print(
-            "Get the win probablility data for a 2023 game between " +
+            "Get the win probability data for a 2023 game between " +
             "the University of Duke and " +
             "the University of Louisville (game ID #401525535)."
         )
         json_data = get_cfbd_game_win_probability_data(
             game_id=401525535
         )
         print(json_data)
@@ -2227,15 +2227,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -2288,16 +2288,16 @@
             "yardLine": "yard_line",
         },
         inplace=True,
     )
     if len(wp_df) == 0:
         logging.error(
             "The CFBD API accepted your inputs, "
-            + "but found no data within your specified input paramaters."
-            + " Please double check your input paramaters."
+            + "but found no data within your specified input parameters."
+            + " Please double check your input parameters."
         )
     else:
         wp_df = wp_df.astype({"home_win_probability": "float"})
         wp_df["away_win_probability"] = 1 - wp_df["home_win_probability"]
 
     return wp_df
 
@@ -2309,15 +2309,15 @@
     week: int = None,
     team: str = None,
     season_type: str = "regular",  # "regular" or "postseason"
     return_as_dict: bool = False,
 ):
     """
     Allows you to get pregame win probability data
-    for games within a timeframe.
+    for games within a time frame.
 
     Parameters
     ----------
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
         from the python environment, or from a file on this computer.
@@ -2341,22 +2341,22 @@
 
     `week` (int, optional):
         Optional argument.
         If `week` is set to an integer, this function will attempt
         to load CFB game data from games in that season, and in that week.
 
     `team` (str, optional):
-        Semi-ptional argument.
+        Semi-optional argument.
         If you only want pregame win probability data for a specific team,
         set `team` to the name of the team
         you want pregame win probability data from.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB game information for non-regular season games,
         set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
@@ -2369,17 +2369,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.metrics import get_cfbd_pregame_win_probability_data
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get pregame win probabilities for games in the 2023 CFB season.
         print(
@@ -2452,15 +2452,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
     # Get pregame win probabilities for games in the 2023 CFB season.
         print(
             "Get pregame win probabilities for games in the 2023 CFB season."
         )
@@ -2542,15 +2542,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -2640,29 +2640,29 @@
             "homeWinProb": "home_win_probability",
         },
         inplace=True,
     )
     if len(wp_df) == 0:
         logging.error(
             "The CFBD API accepted your inputs, "
-            + "but found no data within your specified input paramaters."
-            + " Please double check your input paramaters."
+            + "but found no data within your specified input parameters."
+            + " Please double check your input parameters."
         )
     else:
         wp_df = wp_df.astype({"home_win_probability": "float"})
         wp_df["away_win_probability"] = 1 - wp_df["home_win_probability"]
 
     return wp_df
 
 
 def get_cfbd_fg_expected_points(
     api_key: str = None, api_key_dir: str = None, return_as_dict: bool = False
 ):
     """
-    Retrives Expected Points data for field goals from the CFBD API.
+    Retrieves Expected Points data for field goals from the CFBD API.
 
     Parameters
     ----------
     `api_key` (str, optional):
         Semi-optional argument.
         If `api_key` is null, this function will attempt to load a CFBD API key
         from the python environment, or from a file on this computer.
@@ -2691,17 +2691,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.metrics import get_cfbd_fg_expected_points
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get Expected Points (EP) data, specifically for field goals,
         # from the CFBD API.
@@ -2730,15 +2730,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get Expected Points (EP) data,
         # specifically for field goals, from the CFBD API.
         print(
             "Get Expected Points (EP) data, " +
@@ -2777,15 +2777,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/players.py` & `cfbd_json_py-0.1.2/cfbd_json_py/players.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: players.py
 # Purpose: Houses functions pertaining to CFB player data within the CFBD API.
 ###############################################################################
 """
 
 import logging
@@ -81,17 +81,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.players import cfbd_player_search
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get a list of every known "Joe" in the CFBD API.
         print("Get a list of every known \"Joe\" in the CFBD API.")
@@ -160,18 +160,18 @@
             search_str="Jim",
             position="QB"
         )
         print(json_data)
         time.sleep(5)
 
         # Get a list of every known "Joe" in the CFBD API,
-        # who happened to play in the 2020 CFB sesason.
+        # who happened to play in the 2020 CFB season.
         print(
             "Get a list of every known \"Joe\" in the CFBD API," +
-            " who happened to play in the 2020 CFB sesason."
+            " who happened to play in the 2020 CFB season."
         )
         json_data = cfbd_player_search(
             api_key=cfbd_key,
             search_str="Joe",
             season=2020
         )
         print(json_data)
@@ -194,15 +194,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get a list of every known "Joe" in the CFBD API.
         print("Get a list of every known \"Joe\" in the CFBD API.")
         json_data = cfbd_player_search(
             search_str="Joe"
@@ -264,18 +264,18 @@
             search_str="Jim",
             position="QB"
         )
         print(json_data)
         time.sleep(5)
 
         # Get a list of every known "Joe" in the CFBD API,
-        # who happened to play in the 2020 CFB sesason.
+        # who happened to play in the 2020 CFB season.
         print(
             "Get a list of every known \"Joe\" in the CFBD API, " +
-            "who happened to play in the 2020 CFB sesason."
+            "who happened to play in the 2020 CFB season."
         )
         json_data = cfbd_player_search(
             search_str="Joe",
             season=2020
         )
         print(json_data)
         time.sleep(5)
@@ -312,15 +312,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -437,15 +437,15 @@
         this function will try to find
         a CFBD API key file in this user's home directory.
         If `api_key_dir` is set to a string, and `api_key` is null,
         this function will assume that `api_key_dir` is a directory,
         and will try to find a CFBD API key file in that directory.
 
     `team` (str, optional):
-        Semi-ptional argument.
+        Semi-optional argument.
         If you only want player usage data for a specific team,
         set `team` to the name of the team you want player usage data from.
         You MUST set `season` or `team` to a non-null value for
         this function to work. If you don't, a `ValueError()`
         will be raised.
 
     `position` (str, optional):
@@ -457,18 +457,18 @@
         in the `position_abbreviation` column from
         the pandas DataFrame that is returned
         by calling `cfbd_json_py.draft.get_cfbd_nfl_positions()`.
 
     `conference` (str, optional):
         Optional argument.
         If you only want player usage data from games
-        involving teams from a specific confrence,
+        involving teams from a specific conference,
         set `conference` to the abbreviation
         of the conference you want player usage data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `player_id` (int, optional):
         Optional argument.
         If you only want player usage data for a specific player ID,
         set this variable to the player ID
@@ -493,17 +493,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.players import get_cfbd_player_usage
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get player usage data from the 2020 CFB season.
         print("Get player usage data from the 2020 CFB season.")
@@ -541,18 +541,18 @@
             season=2020,
             position="RB"
         )
         print(json_data)
         time.sleep(5)
 
         # Get player usage data from players who played on
-        # Big 10 Confrence (B1G) teams during the 2020 CFB Season.
+        # Big 10 conference (B1G) teams during the 2020 CFB Season.
         print(
             "Get player usage data from players who played " +
-            "on Big 10 Confrence (B1G) teams during the 2020 CFB Season."
+            "on Big 10 conference (B1G) teams during the 2020 CFB Season."
         )
         json_data = get_cfbd_player_usage(
             api_key=cfbd_key,
             season=2020,
             conference="B1G"
         )
         print(json_data)
@@ -573,15 +573,15 @@
         )
         print(json_data)
         time.sleep(5)
 
         # Get player usage data from
         # former LSU Tigers quarterback Joe Burrow (player ID #3915511),
         # during the 2019 CFB season,
-        # but filter out plays that occured in garbage time.
+        # but filter out plays that occurred in garbage time.
         print(
             "Get player usage data from " +
             "former LSU Tigers quarterback Joe Burrow " +
             "(player ID #3915511), during the 2019 CFB season."
         )
         json_data = get_cfbd_player_usage(
             api_key=cfbd_key,
@@ -608,15 +608,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get player usage data from the 2020 CFB season.
         print("Get player usage data from the 2020 CFB season.")
         json_data = get_cfbd_player_usage(
             season=2020
@@ -649,18 +649,18 @@
             season=2020,
             position="RB"
         )
         print(json_data)
         time.sleep(5)
 
         # Get player usage data from players who played on
-        # Big 10 Confrence (B1G) teams during the 2020 CFB Season.
+        # Big 10 conference (B1G) teams during the 2020 CFB Season.
         print(
             "Get player usage data from players " +
-            "who played on Big 10 Confrence (B1G) teams " +
+            "who played on Big 10 conference (B1G) teams " +
             "during the 2020 CFB Season."
         )
         json_data = get_cfbd_player_usage(
             season=2020,
             conference="B1G"
         )
         print(json_data)
@@ -680,15 +680,15 @@
         )
         print(json_data)
         time.sleep(5)
 
         # Get player usage data from
         # former LSU Tigers quarterback Joe Burrow (player ID #3915511),
         # during the 2019 CFB season,
-        # but filter out plays that occured in garbage time.
+        # but filter out plays that occurred in garbage time.
         print(
             "Get player usage data from " +
             "former LSU Tigers quarterback Joe Burrow " +
             "(player ID #3915511), during the 2019 CFB season."
         )
         json_data = get_cfbd_player_usage(
             season=2019,
@@ -729,15 +729,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -872,28 +872,28 @@
         Semi-optional argument.
         Specifies the season you want team PPA data from.
         You MUST set `season` or `team` to a non-null value for
         this function to work. If you don't, a `ValueError()`
         will be raised.
 
     `team` (str, optional):
-        Semi-ptional argument.
+        Semi-optional argument.
         If you only want team PPA data for a specific team,
         set `team` to the name of the team you want team PPA data from.
         You MUST set `season` or `team` to a non-null value for
         this function to work. If you don't, a `ValueError()`
         will be raised.
 
     `conference` (str, optional):
         Optional argument.
         If you only want team PPA data from games
-        involving teams from a specific confrence,
+        involving teams from a specific conference,
         set `conference` to the abbreviation
         of the conference you want team PPA data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -904,17 +904,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.players import get_cfbd_returning_production
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get returning production
         # for teams who competed in the 2020 CFB season.
@@ -984,15 +984,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get returning production
         # for teams who competed in the 2020 CFB season.
         print(
             "Get returning production for teams " +
@@ -1071,15 +1071,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1184,15 +1184,15 @@
     end_week: int = None,
     season_type: str = "both",  # "regular", "postseason", or "both"
     stat_category: str = None,
     return_as_dict: bool = False,
 ):
     """
     Get player season stats,
-    or the stats of players in a specific timeframe, from the CFBD API.
+    or the stats of players in a specific time frame, from the CFBD API.
 
     Parameters
     ----------
     `season` (int, mandatory):
         Required argument.
         Specifies the season you want CFB player season stats from.
         This must be specified, otherwise this package, and by extension
@@ -1223,15 +1223,15 @@
         regardless if they are the home/away team,
         set `team` to the name of the team
         you want CFB player season stats from.
 
     `conference` (str, optional):
         Optional argument.
         If you only want player season stats from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want stats from.
 
     `start_week` (int, semi-optional):
         Optional argument.
         If you only want player stats for a range of weeks,
         set `start_week` and `end_week` to
@@ -1252,15 +1252,15 @@
     - `start_week is None and end_week is not None`
         (will be changed in a future version)
     - `end_week < start_week`
     - `end_week = start_week`
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB media information for non-regular season games,
         set `season_type` to "postseason".
         If you want ***both*** regular
         and postseason stats, set `season_type = "both"`.
         If `season_type` is set to anything but "regular",
         "postseason",  or "both", a `ValueError()` will be raised.
 
@@ -1292,17 +1292,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.players import get_cfbd_player_season_stats
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get player season stats for
         # the Ohio Bobcats Football team in the 2020 CFB season.
@@ -1315,33 +1315,33 @@
             season=2020,
             team="Ohio"
         )
         print(json_data)
         time.sleep(5)
 
         # Get player season stats for teams who competed in
-        # the Southeastern Confrence (SEC) in the 2023 CFB season.
+        # the Southeastern conference (SEC) in the 2023 CFB season.
         print(
             "Get player season stats for teams who competed " +
-            "in the Southeastern Confrence (SEC) in the 2023 CFB season."
+            "in the Southeastern conference (SEC) in the 2023 CFB season."
         )
         json_data = get_cfbd_player_season_stats(
             api_key=cfbd_key,
             season=2020,
             conference="SEC"
         )
         print(json_data)
         time.sleep(5)
 
         # Get player season stats for teams who competed in
-        # the Southeastern Confrence (SEC) in the 2023 CFB season,
+        # the Southeastern conference (SEC) in the 2023 CFB season,
         # but only between weeks 1 and 5.
         print(
             "Get player season stats for teams who competed " +
-            "in the Southeastern Confrence (SEC) in the 2023 CFB season."
+            "in the Southeastern conference (SEC) in the 2023 CFB season."
         )
         json_data = get_cfbd_player_season_stats(
             api_key=cfbd_key,
             season=2020,
             conference="SEC",
             start_week=1,
             end_week=5
@@ -1372,18 +1372,18 @@
             team="Ohio",
             season_type="regular"
         )
         print(json_data)
         time.sleep(5)
 
         # Get passing stats for teams who competed in
-        # the Southeastern Confrence (SEC) in the 2023 CFB season.
+        # the Southeastern conference (SEC) in the 2023 CFB season.
         print(
             "Get passing stats for teams who competed " +
-            "in the Southeastern Confrence (SEC) in the 2023 CFB season."
+            "in the Southeastern conference (SEC) in the 2023 CFB season."
         )
         json_data = get_cfbd_player_season_stats(
             api_key=cfbd_key,
             season=2020,
             conference="SEC",
             stat_category="passing"
         )
@@ -1407,15 +1407,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get player season stats for
         # the Ohio Bobcats Football team in the 2020 CFB season.
         print(
             "Get player season stats for " +
@@ -1425,32 +1425,32 @@
             season=2020,
             team="Ohio"
         )
         print(json_data)
         time.sleep(5)
 
         # Get player season stats for teams who competed in
-        # the Southeastern Confrence (SEC) in the 2023 CFB season.
+        # the Southeastern conference (SEC) in the 2023 CFB season.
         print(
             "Get player season stats for teams who competed " +
-            "in the Southeastern Confrence (SEC) in the 2023 CFB season."
+            "in the Southeastern conference (SEC) in the 2023 CFB season."
         )
         json_data = get_cfbd_player_season_stats(
             season=2020,
             conference="SEC"
         )
         print(json_data)
         time.sleep(5)
 
         # Get player season stats for teams who competed in
-        # the Southeastern Confrence (SEC) in the 2023 CFB season,
+        # the Southeastern conference (SEC) in the 2023 CFB season,
         # but only between weeks 1 and 5.
         print(
             "Get player season stats for teams who competed " +
-            "in the Southeastern Confrence (SEC) in the 2023 CFB season."
+            "in the Southeastern conference (SEC) in the 2023 CFB season."
         )
         json_data = get_cfbd_player_season_stats(
             season=2020,
             conference="SEC",
             start_week=1,
             end_week=5
         )
@@ -1478,18 +1478,18 @@
             team="Ohio",
             season_type="regular"
         )
         print(json_data)
         time.sleep(5)
 
         # Get passing stats for teams who competed in
-        # the Southeastern Confrence (SEC) in the 2023 CFB season.
+        # the Southeastern conference (SEC) in the 2023 CFB season.
         print(
             "Get passing stats for teams who competed " +
-            "in the Southeastern Confrence (SEC) in the 2023 CFB season."
+            "in the Southeastern conference (SEC) in the 2023 CFB season."
         )
         json_data = get_cfbd_player_season_stats(
             season=2020,
             conference="SEC",
             stat_category="passing"
         )
         print(json_data)
@@ -1519,15 +1519,15 @@
 
     """
 
     rebuilt_json = {}
     stat_columns = [
         "season",
         "team_name",
-        "team_confrence",
+        "team_conference",
         "player_id",
         "player_name",
         # PASS
         "passing_COMP",
         "passing_ATT",
         "passing_COMP%",
         "passing_YDS",
@@ -1598,15 +1598,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1751,51 +1751,51 @@
     if return_as_dict is True:
         return json_data
 
     for player in tqdm(json_data):
         player_id = int(player["playerId"])
         player_name = player["player"]
         team_name = player["team"]
-        team_confrence = player["conference"]
+        team_conference = player["conference"]
         s_category = player["category"]
         s_type = player["statType"]
         s_num = player["stat"]
 
         if rebuilt_json.get(player_id) is None:
             rebuilt_json[player_id] = {}
 
         if s_category == "passing":
             if s_type == "COMPLETIONS":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["passing_COMP"] = s_num
 
             elif s_type == "ATT":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["passing_ATT"] = s_num
 
             elif s_type == "YDS":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["passing_YDS"] = s_num
 
             elif s_type == "TD":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["passing_TD"] = s_num
 
             elif s_type == "INT":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["passing_INT"] = s_num
             # we can calculate these two later
             elif s_type == "PCT":
                 pass
 
             elif s_type == "YPA":
                 pass
@@ -1803,231 +1803,231 @@
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         elif s_category == "rushing":
             if s_type == "CAR":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["rushing_CAR"] = s_num
 
             elif s_type == "YDS":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["rushing_YDS"] = s_num
 
             elif s_type == "TD":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["rushing_TD"] = s_num
 
             elif s_type == "LONG":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["rushing_LONG"] = s_num
             # we can calculate this later
             elif s_type == "YPC":
                 pass
 
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         elif s_category == "receiving":
             if s_type == "REC":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["receiving_REC"] = s_num
 
             elif s_type == "YDS":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["receiving_YDS"] = s_num
 
             elif s_type == "TD":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["receiving_TD"] = s_num
 
             elif s_type == "LONG":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["receiving_LONG"] = s_num
             # we can calculate this later
             elif s_type == "YPR":
                 pass
 
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         elif s_category == "fumbles":
             if s_type == "FUM":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["fumbles_FUM"] = s_num
 
             elif s_type == "LOST":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["fumbles_LOST"] = s_num
 
             elif s_type == "REC":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["fumbles_LOST"] = s_num
 
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         elif s_category == "defensive":
             if s_type == "TOT":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["defensive_TOT"] = s_num
 
             elif s_type == "SOLO":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["defensive_SOLO"] = s_num
 
             elif s_type == "TFL":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["defensive_TFL"] = s_num
 
             elif s_type == "QB HUR":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["defensive_QB HUR"] = s_num
 
             elif s_type == "SACKS":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["defensive_SACKS"] = s_num
 
             elif s_type == "PD":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["defensive_PD"] = s_num
 
             elif s_type == "TD":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["defensive_TD"] = s_num
 
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         elif s_category == "interceptions":
             if s_type == "INT":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["interceptions_INT"] = s_num
 
             elif s_type == "YDS":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["interceptions_YDS"] = s_num
 
             elif s_type == "TD":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["interceptions_TD"] = s_num
 
             elif s_type == "AVG":
                 pass
 
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         elif s_category == "punting":
             if s_type == "NO":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["punting_NO"] = s_num
 
             elif s_type == "YDS":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["punting_YDS"] = s_num
 
             elif s_type == "TB":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["punting_TB"] = s_num
 
             elif s_type == "In 20":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["punting_In 20"] = s_num
 
             elif s_type == "LONG":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["punting_LONG"] = s_num
 
             elif s_type == "YPP":
                 pass
 
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         elif s_category == "kicking":
             if s_type == "FGM":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["kicking_FGM"] = s_num
 
             elif s_type == "FGA":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["kicking_FGA"] = s_num
 
             elif s_type == "LONG":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["kicking_LONG"] = s_num
 
             elif s_type == "XPM":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["kicking_XPM"] = s_num
 
             elif s_type == "XPA":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["kicking_XPA"] = s_num
 
             elif s_type == "PTS":
                 pass
 
             elif s_type == "PCT":
                 pass
@@ -2035,77 +2035,77 @@
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         elif s_category == "kickReturns":
             if s_type == "NO":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["kickReturns_NO"] = s_num
 
             elif s_type == "YDS":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["kickReturns_YDS"] = s_num
 
             elif s_type == "TD":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["kickReturns_TD"] = s_num
 
             elif s_type == "LONG":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["kickReturns_LONG"] = s_num
             # we can calculate this later
             elif s_type == "AVG":
                 pass
 
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         elif s_category == "puntReturns":
             if s_type == "NO":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["puntReturns_NO"] = s_num
 
             elif s_type == "YDS":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["puntReturns_YDS"] = s_num
 
             elif s_type == "TD":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["puntReturns_TD"] = s_num
 
             elif s_type == "LONG":
                 rebuilt_json[player_id]["player_name"] = player_name
                 rebuilt_json[player_id]["team_name"] = team_name
-                rebuilt_json[player_id]["team_confrence"] = team_confrence
+                rebuilt_json[player_id]["team_conference"] = team_conference
                 rebuilt_json[player_id]["puntReturns_LONG"] = s_num
             # we can calculate this later
             elif s_type == "AVG":
                 pass
 
             else:
                 raise ValueError(f"Unhandled stat type: {s_type}")
 
         else:
             raise ValueError(f"Unhandled stat category: {s_category}")
 
         del player_id, player_name, team_name, \
-            team_confrence, s_category, s_type, s_num
+            team_conference, s_category, s_type, s_num
 
     for key, value in tqdm(rebuilt_json.items()):
         row_df = pd.json_normalize(value)
         final_df = pd.concat([final_df, row_df], ignore_index=True)
         del row_df
 
     final_df = final_df.fillna(0)
@@ -2186,15 +2186,15 @@
             final_df["passing_COMP"] / final_df["passing_ATT"]
         )
 
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 # "player_id",
                 "player_name",
                 # PASS
                 "passing_COMP",
                 "passing_ATT",
                 "passing_YDS",
                 "passing_TD",
@@ -2221,15 +2221,15 @@
             final_df["rushing_YDS"] / final_df["rushing_CAR"]
         )
 
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 # RUSH
                 "rushing_CAR",
                 "rushing_YDS",
                 "rushing_AVG",
                 "rushing_TD",
@@ -2256,15 +2256,15 @@
             final_df["receiving_YDS"] / final_df["receiving_REC"]
         )
 
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 # REC
                 "receiving_REC",
                 "receiving_YDS",
                 "receiving_AVG",
                 "receiving_TD",
@@ -2273,30 +2273,30 @@
         ]
 
     elif filter_by_stat_category is True and stat_category == "fumbles":
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 # FUM
                 "fumbles_FUM",
                 "fumbles_LOST",
                 "fumbles_REC",
             ]
         ]
 
     elif filter_by_stat_category is True and stat_category == "defensive":
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 # DEFENSE
                 "defensive_TOT",
                 "defensive_SOLO",
                 "defensive_TFL",
                 "defensive_QB HUR",
@@ -2307,15 +2307,15 @@
         ]
 
     elif filter_by_stat_category is True and stat_category == "interceptions":
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 # INT
                 "interceptions_INT",
                 "interceptions_YDS",
                 "interceptions_TD",
             ]
@@ -2340,15 +2340,15 @@
             final_df["punting_YDS"] / final_df["punting_NO"]
         )
 
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 # PUNT
                 "punting_NO",
                 "punting_YDS",
                 "punting_AVG",
                 "punting_TB",
@@ -2385,15 +2385,15 @@
             final_df["kicking_XPM"] / final_df["kicking_XPA"]
         )
 
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 # KICK
                 "kicking_FGM",
                 "kicking_FGA",
                 "kicking_FG%",
                 "kicking_LONG",
@@ -2421,15 +2421,15 @@
             final_df["kickReturns_YDS"] / final_df["kickReturns_NO"]
         )
 
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 # KR
                 "kickReturns_NO",
                 "kickReturns_YDS",
                 "kickReturns_AVG",
                 "kickReturns_TD",
@@ -2456,15 +2456,15 @@
             final_df["puntReturns_YDS"] / final_df["puntReturns_NO"]
         )
 
         final_df = final_df[
             [
                 "season",
                 "team_name",
-                "team_confrence",
+                "team_conference",
                 "player_id",
                 "player_name",
                 # KR
                 "puntReturns_NO",
                 "puntReturns_YDS",
                 "puntReturns_AVG",
                 "puntReturns_TD",
@@ -2524,17 +2524,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.players import get_cfbd_transfer_portal_data
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get Transfer Portal data for the 2021 CFB season.
         print("Get Transfer Portal data for the 2021 CFB season.")
@@ -2560,15 +2560,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get Transfer Portal data for the 2021 CFB season.
         print("Get Transfer Portal data for the 2021 CFB season.")
         json_data = get_cfbd_transfer_portal_data(
             season=2021
@@ -2604,15 +2604,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/plays.py` & `cfbd_json_py-0.1.2/cfbd_json_py/plays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: plays.py
 # Purpose: Houses functions pertaining to CFB play data within the CFBD API.
 ###############################################################################
 """
 from datetime import datetime
 import logging
@@ -72,15 +72,15 @@
         Optional argument.
         If `week` is set to an integer, this function will attempt
         to load CFB poll rankings data from games in that season,
         and in that week.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB poll rankings data for non-regular season games,
         set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `offensive_team` (str, optional):
         Optional argument.
@@ -93,75 +93,76 @@
         If you only want CFB drive data from a team, while they are on defense,
         regardless if they are the home/away team,
         set `team` to the name of the team you want CFB drive data from.
 
     `conference` (str, optional):
         Optional argument.
         If you only want CFB drive data from games
-        involving teams from a specific confrence,
+        involving teams from a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB drive data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `offensive_conference` (str, optional):
         Optional argument.
         If you only want CFB drive data from games
-        where the offensive team is from a specific confrenece,
+        where the offensive team is from a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB drive data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `defensive_conference` (str, optional):
         Optional argument.
         If you only want CFB drive data from games
-        where the defensive team is from a specific confrenece,
+        where the defensive team is from a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB drive data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `play_type` (int, optional):
         Optional argument.
         If want to drill down, and only get plays of a specific type,
         (like rushing, passing, kicking plays),
         set `play_type` to the ID for the play type you want returned.
-        To retrive a list of valid play type IDs,
+        To retrieve a list of valid play type IDs,
         use `cfbd_json_py.plays.get_cfbd_pbp_play_types()`.
 
     `ncaa_division` (str, semi-optional):
         Semi-optional argument.
         By default, `ncaa_division` will be set to "fbs",
         short for the Football Bowl Subdivision (FBS),
         formerly known as D1-A (read as "division one single A"),
         the highest level in the NCAA football pyramid,
-        where teams can scolarship up to 85 players
-        on their football team soley for athletic ability,
+        where teams can scholarship up to 85 players
+        on their football team solely for athletic ability,
         and often have the largest athletics budgets
         within the NCAA.
 
         Other valid inputs are:
         - "fcs": Football Championship Subdivision (FCS),
             formerly known as D1-AA (read as "division one double A").
             An FCS school is still in the 1st division of the NCAA,
-            making them elligable for the March Madness tournament,
+            making them eligible for the March Madness tournament,
             but may not have the resources to compete at the FBS level
-            at this time. FCS schools are limited to 63 athletic scolarships
+            at this time. FCS schools are limited to 63 athletic scholarships
             for football.
         - "ii": NCAA Division II. Schools in this and D3 are not
-            elligable for the March Madness tournament,
-            and are limited to 36 athletic scolarships for their football team.
+            eligible for the March Madness tournament,
+            and are limited to 36 athletic scholarships
+            for their football team.
         - "iii": NCAA Division III. The largest single division within the
             NCAA football pyramid.
             D3 schools have the distinction of being part of
-            the only NCAA division that cannot give out scolarships soley
+            the only NCAA division that cannot give out scholarships solely
             for athletic ability.
 
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -172,17 +173,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.plays import get_cfbd_pbp_data
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get CFB PBP data for
         # the University of Cincinnati Football Team
@@ -329,15 +330,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get CFB PBP data for the University of Cincinnati Football Team
         # for week 10 of the 2021 season
         print(
             "Get CFB play-by-play (PBP) data for " +
@@ -493,15 +494,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -688,15 +689,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -805,32 +806,32 @@
         set `athlete_id` to the ID of the player you want stats for.
 
     `stats_type_id` (int, optional):
         Optional argument.
         If want to drill down, and only get plays of a specific type,
         (like rushing, passing, kicking plays),
         set `play_type` to the ID for the play type you want returned.
-        To retrive a list of valid play type IDs,
+        To retrieve a list of valid play type IDs,
         use `cfbd_json_py.plays.get_cfbd_pbp_play_types()`.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB poll rankings data for non-regular season games,
         set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `conference` (str, optional):
         Optional argument.
         If you only want CFB drive data from games
-        involving teams from a specific confrence,
+        involving teams from a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB drive data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -841,17 +842,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.plays import get_cfbd_pbp_stats
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get CFB PBP stats data for the 2020 CFB season.
         print("Get CFB PBP stats data for the 2020 CFB season.")
@@ -956,15 +957,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get CFB PBP stats data for the 2020 CFB season.
         print("Get CFB PBP stats data for the 2020 CFB season.")
         json_data = get_cfbd_pbp_stats(
             season=2020
@@ -1065,15 +1066,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1095,15 +1096,15 @@
             '"regular", "postseason", or "both" for this function to work.'
         )
 
     if season is None and game_id is None:
         logging.warn(
             "This endpoint only returns the top 1,000 results. "
             + "Not setting a value for `season` or `game_id` "
-            + "is not a reccomended practice."
+            + "is not a recommended practice."
         )
     elif season is not None and game_id is None:
         logging.warn(
             "Setting a value for both `season` and `game_id` "
             + "may not yeld the results you want. "
             + "If you just want PBP stats for a valid game ID, "
             + "just set `game_id` to a valid game ID."
@@ -1269,15 +1270,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1318,15 +1319,15 @@
         del p_id
 
     return plays_df
 
 
 ###############################################################################
 # Patreon Only Functions.
-#   No cacheing, because the entire point of these functions are to get people
+#   No caching, because the entire point of these functions are to get people
 #   data ASAP, and right before kickoff.
 ###############################################################################
 
 
 def get_cfbd_live_pbp_data(
     game_id: int,
     api_key: str = None,
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/rankings.py` & `cfbd_json_py-0.1.2/cfbd_json_py/rankings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: rankings.py
 # Purpose: Houses functions pertaining to CFB poll data within the CFBD API.
 ###############################################################################
 """
 from datetime import datetime
 
@@ -56,15 +56,15 @@
         Optional argument.
         If `week` is set to an integer, this function will attempt
         to load CFB poll rankings data from games in that season,
         and in that week.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB poll rankings data for non-regular season games,
         set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
@@ -77,17 +77,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.rankings import get_cfbd_poll_rankings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this " +
             "script for this example."
         )
 
         # Get CFB poll data for the 2020 CFB season.
         print("Get CFB poll data for the 2020 CFB season.")
@@ -136,15 +136,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
         # Get CFB poll data for the 2020 CFB season.
         print("Get CFB poll data for the 2020 CFB season.")
         json_data = get_cfbd_poll_rankings(
             season=2020
@@ -203,15 +203,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/ratings.py` & `cfbd_json_py-0.1.2/cfbd_json_py/ratings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: ratings.py
 # Purpose: Houses functions pertaining to CFB team rating data
     within the CFBD API.
 ###############################################################################
 """
 
@@ -81,17 +81,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.ratings import get_cfbd_sp_plus_ratings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get S&P+ ratings data for the 2020 CFB season.
         print("Get S&P+ ratings data for the 2020 CFB season.")
@@ -144,15 +144,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get S&P+ ratings data for the 2020 CFB season.
         print("Get S&P+ ratings data for the 2020 CFB season.")
         json_data = get_cfbd_sp_plus_ratings(
             season=2020
@@ -212,15 +212,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -278,24 +278,24 @@
         columns={
             "team": "team_name",
             "conference": "conference_name",
             "rating": "S&P+_rating",
             "secondOrderWins": "second_order_wins",
             "offense.rating": "offense_S&P+_rating",
             "offense.success": "offense_S&P+_success",
-            "offense.explosiveness": "offense_S&P+_esplosiveness",
+            "offense.explosiveness": "offense_S&P+_explosiveness",
             "offense.rushing": "offense_S&P+_rushing",
             "offense.passing": "offense_S&P+_passing",
             "offense.standardDowns": "offense_S&P+_standard_downs",
             "offense.passingDowns": "offense_S&P+_passing_downs",
             "offense.runRate": "offense_S&P+_run_rate",
             "offense.pace": "offense_S&P+_pace",
             "defense.rating": "defense_S&P+_rating",
             "defense.success": "defense_S&P+_success",
-            "defense.explosiveness": "defense_S&P+_esplosiveness",
+            "defense.explosiveness": "defense_S&P+_explosiveness",
             "defense.rushing": "defense_S&P+_rushing",
             "defense.passing": "defense_S&P+_passing",
             "defense.standardDowns": "defense_S&P+_standard_downs",
             "defense.passingDowns": "defense_S&P+_passing_downs",
             "defense.havoc.total": "defense_S&P+_havoc_total",
             "defense.havoc.frontSeven": "defense_S&P+_havoc_front_seven",
             "defense.havoc.db": "defense_S&P+_havoc_db",
@@ -359,15 +359,15 @@
         the CFBD API, will not accept the request to get SRS ratings data.
         This or `season` must be set to a valid non-null variable
         for this to function.
 
     `conference` (str, optional):
         Optional argument.
         If you only want game information from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want game information from.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -378,17 +378,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.ratings import get_cfbd_srs_ratings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get SRS ratings data for the 2020 CFB season.
         print("Get SRS ratings data for the 2020 CFB season.")
@@ -441,15 +441,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get SRS ratings data for the 2020 CFB season.
         print("Get SRS ratings data for the 2020 CFB season.")
         json_data = get_cfbd_srs_ratings(
             season=2020
@@ -508,15 +508,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -627,15 +627,15 @@
         the CFBD API, will not accept the request to get S&P+ ratings data.
         This or `season` must be set to a valid non-null variable
         for this to function.
 
     `conference` (str, optional):
         Optional argument.
         If you only want S&P+ ratings data from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want S&P+ ratings data from.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -646,17 +646,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.ratings import get_cfbd_sp_plus_conference_ratings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get S&P+ ratings data for the 2020 CFB season.
         print("Get S&P+ ratings data for the 2020 CFB season.")
@@ -682,15 +682,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get S&P+ ratings data for the 2020 CFB season.
         print("Get S&P+ ratings data for the 2020 CFB season.")
         json_data = get_cfbd_sp_plus_conference_ratings(
             season=2020
@@ -725,15 +725,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -798,24 +798,24 @@
     final_df.rename(
         columns={
             "conference": "conference_name",
             "rating": "S&P+_rating",
             "secondOrderWins": "second_order_wins",
             "offense.rating": "offense_S&P+_rating",
             "offense.success": "offense_S&P+_success",
-            "offense.explosiveness": "offense_S&P+_esplosiveness",
+            "offense.explosiveness": "offense_S&P+_explosiveness",
             "offense.rushing": "offense_S&P+_rushing",
             "offense.passing": "offense_S&P+_passing",
             "offense.standardDowns": "offense_S&P+_standard_downs",
             "offense.passingDowns": "offense_S&P+_passing_downs",
             "offense.runRate": "offense_S&P+_run_rate",
             "offense.pace": "offense_S&P+_pace",
             "defense.rating": "defense_S&P+_rating",
             "defense.success": "defense_S&P+_success",
-            "defense.explosiveness": "defense_S&P+_esplosiveness",
+            "defense.explosiveness": "defense_S&P+_explosiveness",
             "defense.rushing": "defense_S&P+_rushing",
             "defense.passing": "defense_S&P+_passing",
             "defense.standardDowns": "defense_S&P+_standard_downs",
             "defense.passingDowns": "defense_S&P+_passing_downs",
             "defense.havoc.total": "defense_S&P+_havoc_total",
             "defense.havoc.frontSeven": "defense_S&P+_havoc_front_seven",
             "defense.havoc.db": "defense_S&P+_havoc_db",
@@ -875,15 +875,15 @@
         Optional argument.
         If `week` is set to a valid, non-null integer,
         the CFBD API will return back Elo data for a team up to that week
         in a season.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "postseason".
+        By default, this will be set to "postseason".
         If `season_type` is set to "regular",
         the API will ignore postseason games
         (like bowls and CFP games) when calculating elo.
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `team` (str, optional):
@@ -893,15 +893,15 @@
         the CFBD API, will not accept the request to get S&P+ ratings data.
         This or `season` must be set to a valid non-null variable
         for this to function.
 
     `conference` (str, optional):
         Optional argument.
         If you only want S&P+ ratings data from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want S&P+ ratings data from.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -912,17 +912,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.ratings import get_cfbd_elo_ratings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get Elo ratings data for the 2020 CFB season.
         print("Get Elo ratings data for the 2020 CFB season.")
@@ -968,18 +968,18 @@
             team="Cincinnati"
         )
         print(json_data)
         time.sleep(5)
 
 
         # Get Elo ratings data for teams competing in the
-        # Atlantic Coast Confrence (ACC) in the 2021 CFB season.
+        # Atlantic Coast conference (ACC) in the 2021 CFB season.
         print(
             "Get Elo ratings data for teams competing in " +
-            "the Atlantic Coast Confrence (ACC) in the 2021 CFB season."
+            "the Atlantic Coast conference (ACC) in the 2021 CFB season."
         )
         json_data = get_cfbd_elo_ratings(
             api_key=cfbd_key,
             season=2021,
             conference="ACC"
         )
         print(json_data)
@@ -1001,15 +1001,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get Elo ratings data for the 2020 CFB season.
         print("Get Elo ratings data for the 2020 CFB season.")
         json_data = get_cfbd_elo_ratings(
             season=2020
@@ -1049,18 +1049,18 @@
             team="Cincinnati"
         )
         print(json_data)
         time.sleep(5)
 
 
         # Get Elo ratings data for teams competing in the
-        # Atlantic Coast Confrence (ACC) in the 2021 CFB season.
+        # Atlantic Coast conference (ACC) in the 2021 CFB season.
         print(
             "Get Elo ratings data for teams competing in " +
-            "the Atlantic Coast Confrence (ACC) in the 2021 CFB season."
+            "the Atlantic Coast conference (ACC) in the 2021 CFB season."
         )
         json_data = get_cfbd_elo_ratings(
             season=2021,
             conference="ACC"
         )
         print(json_data)
         time.sleep(5)
@@ -1092,15 +1092,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1228,15 +1228,15 @@
         the CFBD API, will not accept the request to get FPI ratings data.
         This or `season` must be set to a valid non-null variable
         for this to function.
 
     `conference` (str, optional):
         Optional argument.
         If you only want FPI ratings data from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want FPI ratings data from.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -1247,17 +1247,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.ratings import get_cfbd_fpi_ratings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get FPI ratings data for the 2020 CFB season.
         print("Get FPI ratings data for the 2020 CFB season.")
@@ -1289,18 +1289,18 @@
             team="Cincinnati"
         )
         print(json_data)
         time.sleep(5)
 
 
         # Get FPI ratings data for teams competing in the
-        # Atlantic Coast Confrence (ACC) in the 2021 CFB season.
+        # Atlantic Coast conference (ACC) in the 2021 CFB season.
         print(
             "Get FPI ratings data for teams competing in the " +
-            "Atlantic Coast Confrence (ACC) in the 2021 CFB season."
+            "Atlantic Coast conference (ACC) in the 2021 CFB season."
         )
         json_data = get_cfbd_fpi_ratings(
             api_key=cfbd_key,
             season=2021,
             conference="ACC"
         )
         print(json_data)
@@ -1322,15 +1322,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get FPI ratings data for the 2020 CFB season.
         print("Get FPI ratings data for the 2020 CFB season.")
         json_data = get_cfbd_fpi_ratings(
             season=2020
@@ -1359,18 +1359,18 @@
             team="Cincinnati"
         )
         print(json_data)
         time.sleep(5)
 
 
         # Get FPI ratings data for teams competing in the
-        # Atlantic Coast Confrence (ACC) in the 2021 CFB season.
+        # Atlantic Coast conference (ACC) in the 2021 CFB season.
         print(
             "Get FPI ratings data for teams competing in the " +
-            "Atlantic Coast Confrence (ACC) in the 2021 CFB season."
+            "Atlantic Coast conference (ACC) in the 2021 CFB season."
         )
         json_data = get_cfbd_fpi_ratings(
             season=2021,
             conference="ACC"
         )
         print(json_data)
         time.sleep(5)
@@ -1404,15 +1404,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1474,19 +1474,19 @@
     final_df = pd.json_normalize(json_data)
 
     final_df.rename(
         columns={
             "year": "season",
             "team": "team_name",
             "conference": "conference_name",
-            "resumeRanks.strenghOfRecord": "resume_strength_of_record",
+            "resumeRanks.strengthOfRecord": "resume_strength_of_record",
             "resumeRanks.fpi": "fpi_rank",
             "resumeRanks.averageWinProbability": "resume_avg_win_probability",
             "resumeRanks.strengthOfSchedule": "resume_strength_of_schedule",
-            "resumeRanks.remaningStrengthOfSchedule":
+            "resumeRanks.remainingStrengthOfSchedule":
                 "resume_remaining_strength_of_schedule",
             "resumeRanks.gameControl": "resume_game_control",
             "efficiencies.overall": "efficiency_overall",
             "efficiencies.offense": "efficiency_offense",
             "efficiencies.defense": "efficiency_defense",
             "efficiencies.specialTeams": "efficiency_special_teams",
         },
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/recruiting.py` & `cfbd_json_py-0.1.2/cfbd_json_py/recruiting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: recruiting.py
 # Purpose: Houses functions pertaining to CFB recruiting data
     within the CFBD API.
 ###############################################################################
 """
 
@@ -74,15 +74,15 @@
         By default, this is sent to `None`,
         so one can get all recruits from a given season and/or team.
 
         If you want to filter by what type of recruit,
         the following values are valid for `recruit_classification`:
         - `HighSchool`: Exactly what it says on the tin. These are HS recruits.
         - `JUCO`: JUnior COllege recruits.
-            These are recruits who are transfering from a
+            These are recruits who are transferring from a
             junior college to an NCAA college.
         - `PrepSchool`: College Prep school recruits.
             These are recruits from places such as
             the Fork Union Military Academy in Fort Union, VA
             or Palmetto Prep in Columbia, SC.
 
     `position` (str, optional):
@@ -109,17 +109,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.recruiting import get_cfbd_player_recruit_ratings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get a list of all recruits for the 2020 recruiting class.
         print("Get a list of all recruits for the 2020 recruiting class.")
@@ -202,15 +202,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
 
         # Get a list of all recruits for the 2020 recruiting class.
         print("Get a list of all recruits for the 2020 recruiting class.")
         json_data = get_cfbd_player_recruit_ratings(
@@ -302,15 +302,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -472,17 +472,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.recruiting import get_cfbd_team_recruiting_ratings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get a team recruiting rankings for the 2020 CFB season.
         print("Get a team recruiting rankings for the 2020 CFB season.")
@@ -522,15 +522,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
 
         # Get a team recruiting rankings for the 2020 CFB season.
         print("Get a team recruiting rankings for the 2020 CFB season.")
         json_data = get_cfbd_team_recruiting_ratings(
@@ -581,15 +581,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -710,18 +710,18 @@
         the CFBD API, will not accept the request to get CFB recruiting data.
         This or `season` must be set to a valid non-null variable
         for this to function.
 
     `conference` (str, optional):
         Optional argument.
         If you only want CFB recruiting data
-        from teams in a specific confrence,
+        from teams in a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB recruiting data from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -732,17 +732,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.recruiting import get_cfbd_team_recruiting_group_ratings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get recruiting data between 2020 and 2023,
         # grouped by team and position.
@@ -798,19 +798,19 @@
             start_season=2020
         )
         print(json_data)
         time.sleep(5)
 
         # Get recruiting data starting in 2020,
         # grouped by team and position,
-        # but only for Mountain West Confrence (MWC) teams.
+        # but only for Mountain West conference (MWC) teams.
         print(
             "Get recruiting data starting in 2020, " +
             "grouped by team and position, " +
-            "but only for Mountain West Confrence (MWC) teams."
+            "but only for Mountain West conference (MWC) teams."
         )
         json_data = get_cfbd_team_recruiting_group_ratings(
             api_key=cfbd_key,
             start_season=2020,
             conference="MWC"
         )
         print(json_data)
@@ -833,15 +833,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
 
         # Get recruiting data between 2020 and 2023,
         # grouped by team and position.
         print(
@@ -892,19 +892,19 @@
             end_season=2018
         )
         print(json_data)
         time.sleep(5)
 
         # Get recruiting data starting in 2020,
         # grouped by team and position,
-        # but only for Mountain West Confrence (MWC) teams.
+        # but only for Mountain West conference (MWC) teams.
         print(
             "Get recruiting data starting in 2020, " +
             "grouped by team and position, " +
-            "but only for Mountain West Confrence (MWC) teams."
+            "but only for Mountain West conference (MWC) teams."
         )
         json_data = get_cfbd_team_recruiting_group_ratings(
             start_season=2020,
             conference="MWC"
         )
         print(json_data)
         time.sleep(5)
@@ -938,15 +938,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/stats.py` & `cfbd_json_py-0.1.2/cfbd_json_py/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 PM EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: stats.py
 # Purpose: Houses functions pertaining to CFB team/player
     stats data within the CFBD API.
 ###############################################################################
 """
 
@@ -24,15 +24,15 @@
     season: int = None,
     team: str = None,
     # `year` and/or `team` need to be not null for this function to work.
     conference: str = None,
     start_week: int = None,
     end_week: int = None,
     return_as_dict: bool = False,
-    use_origional_column_names: bool = False,
+    use_original_column_names: bool = False,
 ):
     """
     Allows you to get CFB team season stats data from the CFBD API.
 
     Parameters
     ----------
 
@@ -71,15 +71,15 @@
         the request to get CFB team season stats data.
         This or `season` must be set
         to a valid non-null variable for this to function.
 
     `conference` (str, optional):
         Optional argument.
         If you only want team season stats from games
-        involving teams a specific confrence,
+        involving teams a specific conference,
         set `conference` to the abbreviation
         of the conference you want stats from.
 
     `start_week` (int, semi-optional):
         Optional argument.
         If you only want team stats for a range of weeks,
         set `start_week` and `end_week` to
@@ -114,17 +114,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.stats import get_cfbd_team_season_stats
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get team season stats for the 2020 CFB season.
         print("Get team season stats for the 2020 CFB season.")
@@ -133,18 +133,18 @@
             season=2020
         )
         print(json_data)
         time.sleep(5)
 
 
         # Get team season stats for teams competing in
-        # the Big 10 (B1G) Confrence the 2020 CFB season.
+        # the Big 10 (B1G) conference the 2020 CFB season.
         print(
             "Get team season stats for teams competing in " +
-            "the Big 10 (B1G) Confrence the 2020 CFB season."
+            "the Big 10 (B1G) conference the 2020 CFB season."
         )
         json_data = get_cfbd_team_season_stats(
             api_key=cfbd_key,
             conference="B1G",
             season=2020
         )
         print(json_data)
@@ -177,33 +177,33 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
 
         # Get team season stats for the 2020 CFB season.
         print("Get team season stats for the 2020 CFB season.")
         json_data = get_cfbd_team_season_stats(
             season=2020
         )
         print(json_data)
         time.sleep(5)
 
 
         # Get team season stats for teams competing in
-        # the Big 10 (B1G) Confrence the 2020 CFB season.
+        # the Big 10 (B1G) conference the 2020 CFB season.
         print(
             "Get team season stats for teams competing in " +
-            "the Big 10 (B1G) Confrence the 2020 CFB season."
+            "the Big 10 (B1G) conference the 2020 CFB season."
         )
         json_data = get_cfbd_team_season_stats(
             conference="B1G",
             season=2020
         )
         print(json_data)
         time.sleep(5)
@@ -294,15 +294,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -716,17 +716,17 @@
     ```
 
     import time
 
     from cfbd_json_py.stats import get_cfbd_advanced_team_season_stats
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get advanced team season stats for the 2020 CFB season.
         print("Get team season stats for the 2020 CFB season.")
@@ -796,15 +796,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
     # Get advanced team season stats for the 2020 CFB season.
         print("Get team season stats for the 2020 CFB season.")
         json_data = get_cfbd_advanced_team_season_stats(
             season=2020
@@ -879,15 +879,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1005,18 +1005,18 @@
             ]
             row_df["offense_second_level_yards_total"] = team["offense"][
                 "secondLevelYardsTotal"
             ]
             row_df["offense_open_field_yards_avg"] = team["offense"][
                 "openFieldYards"
             ]
-            row_df["offense_open_field_yards_otal"] = team["offense"][
+            row_df["offense_open_field_yards_total"] = team["offense"][
                 "secondLevelYardsTotal"
             ]
-            row_df["offense_total_opportunies"] = team["offense"][
+            row_df["offense_total_opportunities"] = team["offense"][
                 "totalOpportunies"
             ]
             row_df["offense_points_per_opportunity"] = team["offense"][
                 "pointsPerOpportunity"
             ]
 
             row_df["offense_field_position_avg_start"] = team["offense"][
@@ -1099,18 +1099,18 @@
             ]
             row_df["defense_second_level_yards_total"] = team["defense"][
                 "secondLevelYardsTotal"
             ]
             row_df["defense_open_field_yards_avg"] = team["defense"][
                 "openFieldYards"
             ]
-            row_df["defense_open_field_yards_otal"] = team["defense"][
+            row_df["defense_open_field_yards_total"] = team["defense"][
                 "secondLevelYardsTotal"
             ]
-            row_df["defense_total_opportunies"] = team["defense"][
+            row_df["defense_total_opportunities"] = team["defense"][
                 "totalOpportunies"
             ]
             row_df["defense_points_per_opportunity"] = team["defense"][
                 "pointsPerOpportunity"
             ]
 
             row_df["defense_field_position_avg_start"] = team["defense"][
@@ -1251,15 +1251,15 @@
         the result of the game is largely decided,
         set `exclude_garbage_time = True`.
         Default behavior is that this variable is set to
         `False` when this function is called.
 
     `season_type` (str, semi-optional):
         Semi-optional argument.
-        By defualt, this will be set to "regular", for the CFB regular season.
+        By default, this will be set to "regular", for the CFB regular season.
         If you want CFB team game stats, set `season_type` to "postseason".
         If `season_type` is set to anything but "regular" or "postseason",
         a `ValueError()` will be raised.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
@@ -1272,17 +1272,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.stats import get_cfbd_advanced_team_game_stats
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get advanced CFBD team game stats for week 10 of the 2020 CFB season.
         print("Get advanced CFBD team game stats for the 2020 CFB season.")
@@ -1327,18 +1327,18 @@
             season=2020,
             opponent="Ohio"
         )
         print(json_data)
         time.sleep(5)
 
         # Get advanced CFBD team game stats for teams that faced off
-        # agianst the Ohio Bobcats Football Team in the 2020 CFB season.
+        # against the Ohio Bobcats Football Team in the 2020 CFB season.
         print(
             "Get advanced CFBD team game stats for teams that " +
-            "faced off agianst the Ohio Bobcats Football Team " +
+            "faced off against the Ohio Bobcats Football Team " +
             "in the 2020 CFB season."
         )
         json_data = get_cfbd_advanced_team_game_stats(
             api_key=cfbd_key,
             season=2020,
             opponent="Ohio"
         )
@@ -1376,15 +1376,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get advanced CFBD team game stats for week 10 of the 2020 CFB season.
         print("Get advanced CFBD team game stats for the 2020 CFB season.")
         json_data = get_cfbd_advanced_team_game_stats(
             season=2020,
@@ -1423,18 +1423,18 @@
             season=2020,
             opponent="Ohio"
         )
         print(json_data)
         time.sleep(5)
 
         # Get advanced CFBD team game stats for teams that faced off
-        # agianst the Ohio Bobcats Football Team in the 2020 CFB season.
+        # against the Ohio Bobcats Football Team in the 2020 CFB season.
         print(
             "Get advanced CFBD team game stats for teams that " +
-            "faced off agianst the Ohio Bobcats Football Team " +
+            "faced off against the Ohio Bobcats Football Team " +
             "in the 2020 CFB season."
         )
         json_data = get_cfbd_advanced_team_game_stats(
             season=2020,
             opponent="Ohio"
         )
         print(json_data)
@@ -1481,15 +1481,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1614,15 +1614,15 @@
             ]
             row_df["offense_second_level_yards_total"] = team["offense"][
                 "secondLevelYardsTotal"
             ]
             row_df["offense_open_field_yards_avg"] = team["offense"][
                 "openFieldYards"
             ]
-            row_df["offense_open_field_yards_otal"] = team["offense"][
+            row_df["offense_open_field_yards_total"] = team["offense"][
                 "secondLevelYardsTotal"
             ]
 
             row_df["offense_standard_downs_ppa"] = team[
                 "offense"]["standardDowns"]["ppa"]
             row_df["offense_standard_downs_success_rate"] = team[
                 "offense"]["standardDowns"]["successRate"]
@@ -1681,18 +1681,18 @@
             ]
             row_df["defense_second_level_yards_total"] = team["defense"][
                 "secondLevelYardsTotal"
             ]
             row_df["defense_open_field_yards_avg"] = team["defense"][
                 "openFieldYards"
             ]
-            row_df["defense_open_field_yards_otal"] = team["defense"][
+            row_df["defense_open_field_yards_total"] = team["defense"][
                 "secondLevelYardsTotal"
             ]
-            row_df["defense_total_opportunies"] = team["defense"][
+            row_df["defense_total_opportunities"] = team["defense"][
                 "totalOpportunies"
             ]
             row_df["defense_points_per_opportunity"] = team["defense"][
                 "pointsPerOpportunity"
             ]
 
             row_df["defense_standard_downs_ppa"] = team[
@@ -1781,17 +1781,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.stats import get_cfbd_team_stat_categories
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get a list of CFBD stat categories for team stats.
         print("Get a list of CFBD stat categories for team stats.")
@@ -1815,15 +1815,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
         # Get a list of CFBD stat categories for team stats.
         print("Get a list of CFBD stat categories for team stats.")
         json_data = get_cfbd_team_stat_categories()
         print(json_data)
@@ -1852,15 +1852,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/teams.py` & `cfbd_json_py-0.1.2/cfbd_json_py/teams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: teams.py
 # Purpose: Houses functions pertaining to CFB team data within the CFBD API.
 ###############################################################################
 """
 
 
@@ -45,18 +45,18 @@
         a CFBD API key file in this user's home directory.
         If `api_key_dir` is set to a string, and `api_key` is null,
         this function will assume that `api_key_dir` is a directory,
         and will try to find a CFBD API key file in that directory.
 
     `conference` (str, optional):
         Optional argument.
-        If you only want CFB team information from a specific confrence,
+        If you only want CFB team information from a specific conference,
         set `conference` to the abbreviation
         of the conference you want CFB team information from.
-        For a list of confrences,
+        For a list of conferences,
         use the `cfbd_json_py.conferences.get_cfbd_conference_info()`
         function.
 
     `return_as_dict` (bool, semi-optional):
         Semi-optional argument.
         If you want this function to return
         the data as a dictionary (read: JSON object),
@@ -67,17 +67,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.teams import get_cfbd_team_information
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared "+
             "in this script for this example."
         )
 
         # Get CFB team information for all known CFB teams.
         print("Get CFB team information for all known CFB teams.")
@@ -85,18 +85,18 @@
             api_key=cfbd_key
         )
         print(json_data)
         time.sleep(5)
 
 
         # Get CFB team information for all known
-        # Southeastern Confrence (SEC) CFB teams.
+        # Southeastern conference (SEC) CFB teams.
         print(
             "Get CFB team information for all known " +
-            "Southeastern Confrence (SEC) CFB teams."
+            "Southeastern conference (SEC) CFB teams."
         )
         json_data = get_cfbd_team_information(
             api_key=cfbd_key,
             conference="SEC"
         )
         print(json_data)
         time.sleep(5)
@@ -117,30 +117,30 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
         # Get CFB team information for all known CFB teams.
         print("Get CFB team information for all known CFB teams.")
         json_data = get_cfbd_team_information()
         print(json_data)
         time.sleep(5)
 
 
         # Get CFB team information for all known
-        # Southeastern Confrence (SEC) CFB teams.
+        # Southeastern conference (SEC) CFB teams.
         print(
             "Get CFB team information for all known " +
-            "Southeastern Confrence (SEC) CFB teams."
+            "Southeastern conference (SEC) CFB teams."
         )
         json_data = get_cfbd_team_information(
             conference="SEC"
         )
         print(json_data)
         time.sleep(5)
 
@@ -175,15 +175,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -311,17 +311,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.teams import get_cfbd_fbs_team_list
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared " +
             "in this script for this example."
         )
 
         # Get the current list of FBS teams.
         print("Get the current list of FBS teams.")
@@ -358,15 +358,15 @@
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key
         # in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
         # Get the current list of FBS teams.
         print("Get the current list of FBS teams.")
         json_data = get_cfbd_fbs_team_list()
         print(json_data)
@@ -411,15 +411,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -555,17 +555,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.teams import get_cfbd_team_rosters
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get the team roster for the 2019 LSU Tigers Football Team.
         print("Get the team rosters for the 2020 CFB season.")
@@ -616,15 +616,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
 
         # Get the team roster for the 2019 LSU Tigers Football Team.
         print("Get the team roster for the 2019 LSU Tigers Football Team.")
         json_data = get_cfbd_team_rosters(
@@ -685,15 +685,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -798,17 +798,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.teams import get_cfbd_team_talent_rankings
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get team talent rankings data for the 2020 CFB season.
         print("Get team talent rankings data for the 2020 CFB season.")
@@ -842,15 +842,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
 
         # Get team talent rankings data for the 2020 CFB season.
         print("Get team talent rankings data for the 2020 CFB season.")
         json_data = get_cfbd_team_talent_rankings(
@@ -893,15 +893,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
@@ -1009,58 +1009,58 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.teams import get_cfbd_team_matchup_history
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
-        # Get the matchup history betwen the University of Cincinnati
+        # Get the matchup history between the University of Cincinnati
         # and the Miami (OH) Redhawks football teams.
         print(
-            "Get the matchup history betwen the University of Cincinnati " +
+            "Get the matchup history between the University of Cincinnati " +
             "and the Miami (OH) Redhawks football teams."
         )
         json_data = get_cfbd_team_matchup_history(
             api_key=cfbd_key,
             team_1="Cincinnati",
             team_2="Miami (OH)"
         )
         print(json_data)
         time.sleep(5)
 
-        # Get the matchup history betwen the Ohio State Buckeyes
+        # Get the matchup history between the Ohio State Buckeyes
         # and the Michigan Wolverines football teams,
         # starting in 2002.
         print(
-            "Get the matchup history betwen the Ohio State Buckeyes " +
+            "Get the matchup history between the Ohio State Buckeyes " +
             "and the University of Michigan Wolverines " +
             "football teams, starting in 2002."
         )
         json_data = get_cfbd_team_matchup_history(
             api_key=cfbd_key,
             team_1="Ohio State",
             team_2="Michigan",
             min_season=2002
         )
         print(json_data)
         time.sleep(5)
 
-        # Get the matchup history betwen the Ohio Bobcats
+        # Get the matchup history between the Ohio Bobcats
         # and the Miami (OH) Redhawks football teams,
         # starting in 1990 and ending in 2005.
         print(
-            "Get the matchup history betwen the University of Cincinnati " +
+            "Get the matchup history between the University of Cincinnati " +
             "and the Miami (OH) Redhawks football teams."
         )
         json_data = get_cfbd_team_matchup_history(
             api_key=cfbd_key,
             team_1="Ohio",
             team_2="Miami (OH)",
             min_season=1990,
@@ -1086,53 +1086,53 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded " +
+            "Using the user's API key supposedly loaded " +
             "into this python environment for this example."
         )
 
 
-        # Get the matchup history betwen the University of Cincinnati
+        # Get the matchup history between the University of Cincinnati
         # and the Miami (OH) Redhawks football teams.
         print(
-            "Get the matchup history betwen the University of Cincinnati " +
+            "Get the matchup history between the University of Cincinnati " +
             "and the Miami (OH) Redhawks football teams."
         )
         json_data = get_cfbd_team_matchup_history(
             team_1="Cincinnati",
             team_2="Miami (OH)"
         )
         print(json_data)
         time.sleep(5)
 
-        # Get the matchup history betwen the Ohio State Buckeyes
+        # Get the matchup history between the Ohio State Buckeyes
         # and the Michigan Wolverines football teams,
         # starting in 2002.
         print(
-            "Get the matchup history betwen the Ohio State Buckeyes " +
+            "Get the matchup history between the Ohio State Buckeyes " +
             "and the University of Michigan Wolverines " +
             "football teams, starting in 2002."
         )
         json_data = get_cfbd_team_matchup_history(
             team_1="Ohio State",
             team_2="Michigan",
             min_season=2002
         )
         print(json_data)
         time.sleep(5)
 
-        # Get the matchup history betwen the Ohio Bobcats
+        # Get the matchup history between the Ohio Bobcats
         # and the Miami (OH) Redhawks football teams,
         # starting in 1990 and ending in 2005.
         print(
-            "Get the matchup history betwen the University of Cincinnati " +
+            "Get the matchup history between the University of Cincinnati " +
             "and the Miami (OH) Redhawks football teams."
         )
         json_data = get_cfbd_team_matchup_history(
             team_1="Ohio",
             team_2="Miami (OH)",
             min_season=1990,
             max_season=2005
@@ -1169,15 +1169,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/utls.py` & `cfbd_json_py-0.1.2/cfbd_json_py/utls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: utls.py
 # Purpose: Houses utility functions for this python package.
 ###############################################################################
 """
 import json
 import os
@@ -12,15 +12,15 @@
 import logging
 
 
 def reverse_cipher_encrypt(plain_text_str: str):
     """
     NOT INTENDED TO BE CALLED BY THE USER!
 
-    Implements a reverse cipher encription to a plain text string.
+    Implements a reverse cipher encryption to a plain text string.
 
     Parameters
     ----------
     `plain_text_str` (mandatory, str):
         The string you want to encrypt through reverse cipher encryption.
 
     Returns
@@ -74,20 +74,20 @@
     NOT INTENDED TO BE CALLED BY THE USER!
 
     If you've already set the API key using
     `cfbd_json_py.utls.set_cfbd_api_token()`,
     you don't need to use this function.
 
     If the CFBD API key exists in the environment,
-    or is in a file, this function retrives the CFBD API key,
+    or is in a file, this function Retrieves the CFBD API key,
     and returns it as a string.
 
     If this package is being used in a GitHub Actions action,
     set the key in the environment by
-    creating a repository secret nammed `CFBD_API_KEY`.
+    creating a repository secret named `CFBD_API_KEY`.
 
     Parameters
     ----------
     `api_key_dir` (str, optional):
         Optional argument. If `api_key_dir` is set to a non-null string,
         `set_cfbd_api_token()` will attempt
         to save the key file in that directory,
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py/venues.py` & `cfbd_json_py-0.1.2/cfbd_json_py/venues.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Creation Date: 08/30/2023 01:13 EDT
-# Last Updated Date: 02/24/2023 03:30 PM EST
+# Last Updated Date: 04/04/2024 05:10 PM EDT
 # Author: Joseph Armstrong (armstrongjoseph08@gmail.com)
 # File Name: venues.py
 # Purpose: Houses functions pertaining to
     CFB team venues/stadium data within the CFBD API.
 ###############################################################################
 """
 
@@ -52,17 +52,17 @@
     ----------
     ```
     import time
 
     from cfbd_json_py.venues import get_cfbd_venues
 
 
-    cfbd_key = "tigersAreAwsome"  # placeholder for your CFBD API Key.
+    cfbd_key = "tigersAreAwesome"  # placeholder for your CFBD API Key.
 
-    if cfbd_key != "tigersAreAwsome":
+    if cfbd_key != "tigersAreAwesome":
         print(
             "Using the user's API key declared in this script " +
             "for this example."
         )
 
         # Get CFB venue/stadium data from the CFBD API.
         print("Get CFB venue/stadium data from the CFBD API.")
@@ -86,15 +86,15 @@
 
     else:
         # Alternatively, if the CFBD API key exists in this python environment,
         # or it's been set by cfbd_json_py.utls.set_cfbd_api_token(),
         # you could just call these functions directly,
         # without setting the API key in the script.
         print(
-            "Using the user's API key suposedly loaded into " +
+            "Using the user's API key supposedly loaded into " +
             "this python environment for this example."
         )
 
         # Get CFB venue/stadium data from the CFBD API.
         print("Get CFB venue/stadium data from the CFBD API.")
         json_data = get_cfbd_venues()
         print(json_data)
@@ -127,15 +127,15 @@
 
     if api_key is not None:
         real_api_key = api_key
         del api_key
     else:
         real_api_key = get_cfbd_api_token(api_key_dir=api_key_dir)
 
-    if real_api_key == "tigersAreAwsome":
+    if real_api_key == "tigersAreAwesome":
         raise ValueError(
             "You actually need to change `cfbd_key` to your CFBD API key."
         )
     elif "Bearer " in real_api_key:
         pass
     elif "Bearer" in real_api_key:
         real_api_key = real_api_key.replace("Bearer", "Bearer ")
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py.egg-info/PKG-INFO` & `cfbd_json_py-0.1.2/cfbd_json_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfbd_json_py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Allows users to access the CFBD API, and get the resulting data in either a dictionary (think JSON), or in a pandas DataFrame (think spreadsheet).
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/cfbd-json-py
 Project-URL: documentation, https://armstjc.github.io/cfbd-json-py/cfbd_json_py.html
 Project-URL: repository, https://github.com/armstjc/cfbd-json-py.git
```

### Comparing `cfbd_json_py-0.1.1/cfbd_json_py.egg-info/SOURCES.txt` & `cfbd_json_py-0.1.2/cfbd_json_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfbd_json_py-0.1.1/pyproject.toml` & `cfbd_json_py-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","wheel","pandas","tqdm","requests","lxml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfbd_json_py"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 
 authors = [
     {name = "Joseph Armstrong", email="armstrongjoseph08@gmail.com"}
 ]
```

