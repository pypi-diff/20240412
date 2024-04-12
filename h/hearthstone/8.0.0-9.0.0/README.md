# Comparing `tmp/hearthstone-8.0.0.tar.gz` & `tmp/hearthstone-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-8.0.0.tar", last modified: Tue Apr  2 11:16:16 2024, max compression
+gzip compressed data, was "hearthstone-9.0.0.tar", last modified: Fri Apr 12 09:55:12 2024, max compression
```

## Comparing `hearthstone-8.0.0.tar` & `hearthstone-9.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:16:16.751590 hearthstone-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-02 11:16:11.000000 hearthstone-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-02 11:16:16.751590 hearthstone-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-02 11:16:11.000000 hearthstone-8.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:16:16.751590 hearthstone-8.0.0/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14369 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    65012 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:16:16.751590 hearthstone-8.0.0/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:16:16.751590 hearthstone-8.0.0/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-02 11:16:16.751590 hearthstone-8.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-02 11:16:11.000000 hearthstone-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:55:12.276579 hearthstone-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-12 09:55:07.000000 hearthstone-9.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-12 09:55:12.276579 hearthstone-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-12 09:55:07.000000 hearthstone-9.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:55:12.276579 hearthstone-9.0.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60212 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:55:12.276579 hearthstone-9.0.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-12 09:55:07.000000 hearthstone-9.0.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:55:12.276579 hearthstone-9.0.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-12 09:55:12.000000 hearthstone-9.0.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-12 09:55:12.000000 hearthstone-9.0.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:55:12.000000 hearthstone-9.0.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 09:55:12.000000 hearthstone-9.0.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 09:55:12.000000 hearthstone-9.0.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:55:12.000000 hearthstone-9.0.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-12 09:55:12.276579 hearthstone-9.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-12 09:55:07.000000 hearthstone-9.0.0/setup.py
```

### Comparing `hearthstone-8.0.0/LICENSE` & `hearthstone-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/PKG-INFO` & `hearthstone-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 8.0.0
+Version: 9.0.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-8.0.0/README.md` & `hearthstone-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/hearthstone/bountyxml.py` & `hearthstone-9.0.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/hearthstone/cardxml.py` & `hearthstone-9.0.0/hearthstone/cardxml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tempfile
 from typing import Any, Callable, Iterator, Tuple
 
 from .enums import (
 	CardClass, CardSet, CardType, Faction, GameTag,
-	MultiClassGroup, PlayReq, Race, Rarity, Role, SpellSchool
+	MultiClassGroup, Race, Rarity, Role, SpellSchool
 )
 from .utils import ElementTree
 from .xmlutils import download_to_tempfile_retry
 
 
 LOCALIZED_TAGS = [
 	GameTag.CARDNAME, GameTag.CARDTEXT_INHAND, GameTag.FLAVORTEXT,
@@ -55,29 +55,14 @@
 	e.attrib["name"] = name
 	e.attrib["type"] = "Int"
 	e.attrib["value"] = value
 
 	return e
 
 
-def _read_power_tag(e):
-	ret = {"definition": e.attrib["definition"]}
-	reqs = e.findall("PlayRequirement")
-	if reqs is not None:
-		ret["requirements"] = {}
-		for pr in reqs:
-			reqid = int(pr.attrib["reqID"])
-			try:
-				req = PlayReq(reqid)
-			except ValueError:
-				req = reqid
-			ret["requirements"][req] = int(pr.attrib["param"] or 0)
-	return ret
-
-
 def _unpack_tag_xml(e):
 	value = int(e.attrib["enumID"])
 	try:
 		tag = GameTag(value)
 	except ValueError:
 		tag = value
 	type = e.attrib.get("type", "Int")
@@ -112,35 +97,23 @@
 
 		if self.hero_power is None and self.tags.get(GameTag.HERO_POWER):
 			i = int(GameTag.HERO_POWER)
 			t = xml.findall('./Tag[@enumID="%i"]' % (i))
 			if t is not None:
 				self.hero_power = t[0].attrib.get("cardID")
 
-		e = xml.findall("MasterPower")
-		self.master_power = e[0] if e else None
-
-		e = xml.findall("Power")
-		for power in e:
-			self.powers.append(_read_power_tag(power))
-
-		self.entourage = [t.attrib["cardID"] for t in xml.findall("EntourageCard")]
 		return self
 
 	def __init__(self, id, locale="enUS"):
 		self.card_id = self.id = id
 		self.dbf_id = 0
 		self.version = 2
 		self.tags = {}
 		self.hero_power = None
 		self.referenced_tags = {}
-		self.master_power = None
-		self.entourage = []
-		self.powers = []
-		self.triggered_power_history_info = []
 
 		self.locale = locale
 
 		self.strings = {
 			GameTag.CARDNAME: {},
 			GameTag.CARDTEXT_INHAND: {},
 			GameTag.FLAVORTEXT: {},
@@ -159,18 +132,14 @@
 		return "<%s: %r>" % (self.id, self.name)
 
 	def to_xml(self):
 		ret = ElementTree.Element("Entity", CardID=self.id, ID=str(self.dbf_id))
 		if self.version:
 			ret.attrib["version"] = str(self.version)
 
-		if self.master_power:
-			master_power = ElementTree.SubElement(ret, "MasterPower")
-			master_power.text = self.master_power
-
 		for tag in LOCALIZED_TAGS:
 			value = self.strings[tag]
 			if value:
 				e = ElementTree.SubElement(ret, "Tag", enumID=str(int(tag)), name=tag.name)
 				e.attrib["type"] = "LocString"
 				for locale, localized_value in sorted(value.items()):
 					if localized_value:
@@ -191,29 +160,14 @@
 				if tag == GameTag.HERO_POWER and self.hero_power:
 					e.attrib["type"] = "Card"
 					e.attrib["cardID"] = self.hero_power
 
 		for tag, value in sorted(self.referenced_tags.items()):
 			e = _make_tag_element(ret, "ReferencedTag", tag, value)
 
-		for entourage in self.entourage:
-			ElementTree.SubElement(ret, "EntourageCard", cardID=entourage)
-
-		for power in self.powers:
-			ep = ElementTree.SubElement(ret, "Power", definition=power["definition"])
-			reqs = power.get("requirements", {})
-			for reqid, param in reqs.items():
-				er = ElementTree.SubElement(ep, "PlayRequirement", reqID=str(int(reqid)))
-				er.attrib["param"] = str(param or "")
-
-		for tphi in self.triggered_power_history_info:
-			e = ElementTree.SubElement(ret, "TriggeredPowerHistoryInfo")
-			e.attrib["effectIndex"] = str(tphi["effectIndex"])
-			e.attrib["showInHistory"] = str(tphi["showInHistory"])
-
 		return ret
 
 	@property
 	def craftable(self):
 		if isinstance(self.card_set, CardSet) and not self.card_set.craftable:
 			return False
 		if not self.type.craftable:
@@ -361,14 +315,16 @@
 	autoattack = prop(GameTag.AUTOATTACK, bool)
 	can_summon_maxplusone_minion = prop(GameTag.CAN_SUMMON_MAXPLUSONE_MINION, bool)
 	cant_be_attacked = prop(GameTag.CANT_BE_ATTACKED, bool)
 	cant_be_fatigued = prop(GameTag.CANT_BE_FATIGUED, bool)
 	collectible = prop(GameTag.COLLECTIBLE, bool)
 	colossal = prop(GameTag.COLOSSAL, bool)
 	battlecry = prop(GameTag.BATTLECRY, bool)
+	choose_one = prop(GameTag.CHOOSE_ONE, bool)
+	combo = prop(GameTag.COMBO, bool)
 	corrupt = prop(GameTag.CORRUPT, bool)
 	deathrattle = prop(GameTag.DEATHRATTLE, bool)
 	discover = prop(GameTag.DISCOVER, bool)
 	divine_shield = prop(GameTag.DIVINE_SHIELD, bool)
 	double_spelldamage_bonus = prop(GameTag.RECEIVES_DOUBLE_SPELLDAMAGE_BONUS, bool)
 	dredge = prop(GameTag.DREDGE, bool)
 	echo = prop(GameTag.ECHO, bool)
```

### Comparing `hearthstone-8.0.0/hearthstone/dbf.py` & `hearthstone-9.0.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/hearthstone/deckstrings.py` & `hearthstone-9.0.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/hearthstone/entities.py` & `hearthstone-9.0.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/hearthstone/enums.py` & `hearthstone-9.0.0/hearthstone/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -1315,151 +1315,14 @@
 
 	INVALID = 0
 	HORDE = 1
 	ALLIANCE = 2
 	NEUTRAL = 3
 
 
-class PlayReq(IntEnum):
-	"""PlayErrors.ErrorType"""
-
-	INVALID = -1
-	REQ_MINION_TARGET = 1
-	REQ_FRIENDLY_TARGET = 2
-	REQ_ENEMY_TARGET = 3
-	REQ_DAMAGED_TARGET = 4
-	REQ_MAX_SECRETS = 5
-	REQ_FROZEN_TARGET = 6
-	REQ_CHARGE_TARGET = 7
-	REQ_TARGET_MAX_ATTACK = 8
-	REQ_NONSELF_TARGET = 9
-	REQ_TARGET_WITH_RACE = 10
-	REQ_TARGET_TO_PLAY = 11
-	REQ_NUM_MINION_SLOTS = 12
-	REQ_WEAPON_EQUIPPED = 13
-	REQ_ENOUGH_MANA = 14
-	REQ_YOUR_TURN = 15
-	REQ_NONSTEALTH_ENEMY_TARGET = 16
-	REQ_HERO_TARGET = 17
-	REQ_SECRET_ZONE_CAP = 18
-	REQ_MINION_CAP_IF_TARGET_AVAILABLE = 19
-	REQ_MINION_CAP = 20
-	REQ_TARGET_ATTACKED_THIS_TURN = 21
-	REQ_TARGET_IF_AVAILABLE = 22
-	REQ_MINIMUM_ENEMY_MINIONS = 23
-	REQ_TARGET_FOR_COMBO = 24
-	REQ_NOT_EXHAUSTED_ACTIVATE = 25
-	REQ_UNIQUE_SECRET_OR_QUEST = 26
-	REQ_TARGET_TAUNTER = 27
-	REQ_CAN_BE_ATTACKED = 28
-	REQ_ACTION_PWR_IS_MASTER_PWR = 29
-	REQ_TARGET_MAGNET = 30
-	REQ_ATTACK_GREATER_THAN_0 = 31
-	REQ_ATTACKER_NOT_FROZEN = 32
-	REQ_HERO_OR_MINION_TARGET = 33
-	REQ_CAN_BE_TARGETED_BY_SPELLS = 34
-	REQ_SUBCARD_IS_PLAYABLE = 35
-	REQ_TARGET_FOR_NO_COMBO = 36
-	REQ_NOT_MINION_JUST_PLAYED = 37
-	REQ_NOT_EXHAUSTED_HERO_POWER = 38
-	REQ_CAN_BE_TARGETED_BY_OPPONENTS = 39
-	REQ_ATTACKER_CAN_ATTACK = 40
-	REQ_TARGET_MIN_ATTACK = 41
-	REQ_CAN_BE_TARGETED_BY_HERO_POWERS = 42
-	REQ_ENEMY_TARGET_NOT_IMMUNE = 43
-	REQ_ALL_BASIC_TOTEMS_NOT_IN_PLAY = 44
-	REQ_MINIMUM_TOTAL_MINIONS = 45
-	REQ_MUST_TARGET_TAUNTER = 46
-	REQ_UNDAMAGED_TARGET = 47
-	REQ_CAN_BE_TARGETED_BY_BATTLECRIES = 48
-	REQ_STEADY_SHOT = 49
-	REQ_MINION_OR_ENEMY_HERO = 50
-	REQ_TARGET_IF_AVAILABLE_AND_DRAGON_IN_HAND = 51
-	REQ_LEGENDARY_TARGET = 52
-	REQ_FRIENDLY_MINION_DIED_THIS_TURN = 53
-	REQ_FRIENDLY_MINION_DIED_THIS_GAME = 54
-	REQ_ENEMY_WEAPON_EQUIPPED = 55
-	REQ_TARGET_IF_AVAILABLE_AND_MINIMUM_FRIENDLY_MINIONS = 56
-	REQ_TARGET_WITH_BATTLECRY = 57
-	REQ_TARGET_WITH_DEATHRATTLE = 58
-	REQ_TARGET_IF_AVAILABLE_AND_MINIMUM_FRIENDLY_SECRETS = 59
-	REQ_SECRET_ZONE_CAP_FOR_NON_SECRET = 60
-	REQ_TARGET_EXACT_COST = 61
-	REQ_STEALTHED_TARGET = 62
-	REQ_MINION_SLOT_OR_MANA_CRYSTAL_SLOT = 63
-	REQ_MAX_QUESTS = 64
-	REQ_TARGET_IF_AVAILABE_AND_ELEMENTAL_PLAYED_LAST_TURN = 65
-	REQ_TARGET_NOT_VAMPIRE = 66
-	REQ_TARGET_NOT_DAMAGEABLE_ONLY_BY_WEAPONS = 67
-	REQ_NOT_DISABLED_HERO_POWER = 68
-	REQ_MUST_PLAY_OTHER_CARD_FIRST = 69
-	REQ_HAND_NOT_FULL = 70
-	REQ_TARGET_IF_AVAILABLE_AND_NO_3_COST_CARD_IN_DECK = 71
-	REQ_CAN_BE_TARGETED_BY_COMBOS = 72
-	REQ_CANNOT_PLAY_THIS = 73
-	REQ_FRIENDLY_MINIONS_OF_RACE_DIED_THIS_GAME = 74
-	REQ_DRAG_TO_PLAY_PRE29933 = 75  # This value changes between patches 27845 and 29933
-	REQ_OPPONENT_PLAYED_CARDS_THIS_GAME = 77
-	REQ_LITERALLY_UNPLAYABLE = 78
-	REQ_TARGET_IF_AVAILABLE_AND_HERO_HAS_ATTACK = 79
-	REQ_FRIENDLY_MINION_OF_RACE_DIED_THIS_TURN = 80
-	REQ_TARGET_IF_AVAILABLE_AND_MINIMUM_SPELLS_PLAYED_THIS_TURN = 81
-	REQ_FRIENDLY_MINION_OF_RACE_IN_HAND = 82
-	REQ_DRAG_TO_PLAY_PRE31761 = 83  # This value changes between patches 31532 and 31761
-	REQ_FRIENDLY_DEATHRATTLE_MINION_DIED_THIS_GAME = 86
-	REQ_FRIENDLY_REBORN_MINION_DIED_THIS_GAME = 89
-	REQ_MINION_DIED_THIS_GAME = 90
-	REQ_BOARD_NOT_COMPLETELY_FULL = 92
-	REQ_TARGET_IF_AVAILABLE_AND_HAS_OVERLOADED_MANA = 93
-	REQ_TARGET_IF_AVAILABLE_AND_HERO_ATTACKED_THIS_TURN = 94
-	REQ_TARGET_IF_AVAILABLE_AND_DRAWN_THIS_TURN = 95
-	REQ_TARGET_IF_AVAILABLE_AND_NOT_DRAWN_THIS_TURN = 96
-	REQ_TARGET_NON_TRIPLED_MINION = 97
-	REQ_BOUGHT_MINION_THIS_TURN = 98
-	REQ_SOLD_MINION_THIS_TURN = 99
-	REQ_TARGET_IF_AVAILABLE_AND_PLAYER_HEALTH_CHANGED_THIS_TURN = 100
-	REQ_TARGET_IF_AVAILABLE_AND_SOUL_FRAGMENT_IN_DECK = 101
-	REQ_DAMAGED_TARGET_UNLESS_COMBO = 102
-	REQ_NOT_MINION_DORMANT = 103
-	REQ_TARGET_NOT_UNTOUCHABLE = 104
-	REQ_TARGET_IF_AVAILABLE_AND_BOUGHT_RACE_THIS_TURN = 105
-	REQ_TARGET_IF_AVAILABLE_AND_SOLD_RACE_THIS_TURN = 106
-	REQ_NOT_IN_COOLDOWN = 107
-	REQ_TARGET_IS_MERC = 108
-	REQ_TARGET_IS_NON_MERC = 109
-	REQ_TWO_OF_A_KIND = 110
-	REQ_HAS_OVERLOADED_MANA = 111
-	REQ_LETTUCE_ABILITY_CANNOT_TARGET_OWNER = 112
-	REQ_TARGET_NOT_HAVE_TAG = 116
-	REQ_TARGET_MUST_HAVE_TAG = 117
-	REQ_TRADEABLE = 119
-	REQ_NOT_LEGENDARY_TARGET = 123
-	REQ_MINIMUM_TAVERN_TIER_LEVEL_TO_PLAY = 128
-	REQ_CARD_TAVERN_TIER_LEVEL_TO_PLAY = 129
-	REQ_NOT_EXHAUSTED_LOCATION = 130
-	REQ_LOCATION_TARGET = 131
-	REQ_TARGET_SILVER_HAND_RECRUIT = 132
-	REQ_MINIMUM_CORPSES = 133
-	REQ_LOCATION_OR_MINION_TARGET = 134
-	REQ_CAN_BE_TARGETED_BY_LOCATIONS = 135
-	REQ_FORGE = 136
-	REQ_HAS_PLAYED_SPELL_THIS_GAME = 137
-	REQ_TARGET_IS_NON_TITAN = 141
-	REQ_TARGET_EXACT_ATTACK = 143
-	REQ_DRAG_TO_PLAY = 999
-
-	# Renamed
-	REQ_ENCHANTED_TARGET = REQ_MAX_SECRETS
-	REQ_ENTIRE_ENTOURAGE_NOT_IN_PLAY = REQ_ALL_BASIC_TOTEMS_NOT_IN_PLAY
-	REQ_UNIQUE_SECRET = REQ_UNIQUE_SECRET_OR_QUEST
-	REQ_SECRET_CAP = REQ_SECRET_ZONE_CAP
-	REQ_SECRET_CAP_FOR_NON_SECRET = REQ_SECRET_ZONE_CAP_FOR_NON_SECRET
-	REQ_TARGET_NOT_DORMANT = REQ_TARGET_NOT_UNTOUCHABLE
-
-
 class Race(IntEnum):
 	"""TAG_RACE"""
 
 	INVALID = 0
 	BLOODELF = 1
 	DRAENEI = 2
 	DWARF = 3
```

### Comparing `hearthstone-8.0.0/hearthstone/mercenaryxml.py` & `hearthstone-9.0.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/hearthstone/stringsfile.py` & `hearthstone-9.0.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/hearthstone/utils/__init__.py` & `hearthstone-9.0.0/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/hearthstone/xmlutils.py` & `hearthstone-9.0.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/hearthstone.egg-info/PKG-INFO` & `hearthstone-9.0.0/hearthstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 8.0.0
+Version: 9.0.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-8.0.0/hearthstone.egg-info/SOURCES.txt` & `hearthstone-9.0.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-8.0.0/setup.cfg` & `hearthstone-9.0.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 8.0.0
+version = 9.0.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

