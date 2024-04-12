# Comparing `tmp/ssvc-1.0.2.tar.gz` & `tmp/ssvc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssvc-1.0.2.tar", max compression
+gzip compressed data, was "ssvc-1.0.3.tar", max compression
```

## Comparing `ssvc-1.0.2.tar` & `ssvc-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2024-03-25 11:16:25.817155 ssvc-1.0.2/LICENSE
--rw-r--r--   0        0        0     2158 2024-03-25 11:16:25.817155 ssvc-1.0.2/PYPI.md
--rw-r--r--   0        0        0      503 2024-03-25 11:39:05.689219 ssvc-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6129 2024-03-25 11:36:45.774276 ssvc-1.0.2/src/ssvc/__init__.py
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 ssvc-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-24 22:36:13.565774 ssvc-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2138 2024-04-12 12:00:09.207812 ssvc-1.0.3/PYPI.md
+-rw-r--r--   0        0        0      618 2024-04-12 12:09:36.251085 ssvc-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6463 2024-04-12 12:03:21.776208 ssvc-1.0.3/src/ssvc/__init__.py
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ssvc-1.0.3/PKG-INFO
```

### Comparing `ssvc-1.0.2/LICENSE` & `ssvc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.2/PYPI.md` & `ssvc-1.0.3/PYPI.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,44 +18,44 @@
 ### Example
 
 To use SSVC:
 - Determine the exploitation status of the vulnerability
 - Assess the technical impact, considering the automatability
 
 ```python
-from ssvc import Decision, ExploitationLevel, Automatable, TechnicalImpact, MissionWellbeingImpact, DecisionAction, DecisionPriority
+from ssvc import Decision, ExploitationLevel, Automatable, TechnicalImpact, MissionWellbeingImpact, ActionCISA, DecisionPriority
 decision = Decision(
     ExploitationLevel.POC,
     Automatable.YES,
     TechnicalImpact.PARTIAL,
     MissionWellbeingImpact.MEDIUM,
 )
 assert decision.outcome.priority == DecisionPriority.LOW, "SSVC priority should be LOW"
-assert decision.outcome.action == DecisionAction.TRACK, "SSVC decision should be TRACK"
+assert decision.outcome.action == ActionCISA.TRACK, "SSVC decision should be TRACK"
 ```
 
 Using strings also works
 
 ```python
 import ssvc
 
 decision = ssvc.Decision(
     exploitation='active',
     automatable='no',
     technical_impact='total',
     mission_wellbeing='high',
 )
 assert decision.outcome.priority == ssvc.DecisionPriority.HIGH, "SSVC priority should be HIGH"
-assert decision.outcome.action == ssvc.DecisionAction.ACT, "SSVC decision should be ACT"
+assert decision.outcome.action == ssvc.ActionCISA.ACT, "SSVC decision should be ACT"
 ```
 
 Input incrementally and control how to handle decisions
 
 ```python
-from ssvc import Decision, ExploitationLevel, Automatable, TechnicalImpact, MissionWellbeingImpact, DecisionAction, DecisionPriority
+from ssvc import Decision, ExploitationLevel, Automatable, TechnicalImpact, MissionWellbeingImpact, ActionCISA, DecisionPriority
 decision = Decision()
 # what is the ExploitationLevel?
 decision.exploitation = ExploitationLevel.POC
 # is it Automatable?
 decision.automatable = Automatable.YES
 # figure out the technical impact
 decision.technical_impact = TechnicalImpact.PARTIAL
@@ -64,9 +64,9 @@
 
 # Get a decision outcome
 outcome = decision.evaluate()
 
 # decisions are return and available as a new variable
 assert outcome.priority == DecisionPriority.LOW, "SSVC priority should be LOW"
 # or use the `decision.outcome` like before
-assert decision.outcome.action == DecisionAction.TRACK, "SSVC decision should be TRACK"
+assert decision.outcome.action == ActionCISA.TRACK, "SSVC decision should be TRACK"
 ```
```

### Comparing `ssvc-1.0.2/src/ssvc/__init__.py` & `ssvc-1.0.3/src/ssvc/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,163 +1,185 @@
 from enum import Enum
 
+
 class ExploitationLevel(Enum):
-    NONE = 'none'
-    POC = 'poc'
-    ACTIVE = 'active'
+    NONE = "none"
+    POC = "poc"
+    ACTIVE = "active"
+
 
 class Automatable(Enum):
-    YES = 'yes'
-    NO = 'no'
+    YES = "yes"
+    NO = "no"
+
 
 class TechnicalImpact(Enum):
-    PARTIAL = 'partial'
-    TOTAL = 'total'
+    PARTIAL = "partial"
+    TOTAL = "total"
+
 
 class MissionWellbeingImpact(Enum):
-    LOW = 'low'
-    MEDIUM = 'medium'
-    HIGH = 'high'
+    LOW = "low"
+    MEDIUM = "medium"
+    HIGH = "high"
+
 
 class DecisionPriority(Enum):
-    LOW = 'low'
-    MEDIUM = 'medium'
-    HIGH = 'high'
-    IMMEDIATE = 'immediate'
-
-class DecisionAction(Enum):
-    TRACK = 'Track'
-    TRACK_STAR = 'Track*'
-    ATTEND = 'Attend'
-    ACT = 'Act'
+    LOW = "low"
+    MEDIUM = "medium"
+    HIGH = "high"
+    IMMEDIATE = "immediate"
+
+
+class ActionCISA(Enum):
+    TRACK = "Track"
+    TRACK_STAR = "Track*"
+    ATTEND = "Attend"
+    ACT = "Act"
+
+class Methodology(Enum):
+    FIRST = "FIRST"
+    CISA = "CISA"
+
 
 priority_map = {
-    DecisionAction.TRACK: DecisionPriority.LOW,
-    DecisionAction.TRACK_STAR: DecisionPriority.MEDIUM,
-    DecisionAction.ATTEND: DecisionPriority.MEDIUM,
-    DecisionAction.ACT: DecisionPriority.IMMEDIATE,
+    ActionCISA.TRACK: DecisionPriority.LOW,
+    ActionCISA.TRACK_STAR: DecisionPriority.MEDIUM,
+    ActionCISA.ATTEND: DecisionPriority.MEDIUM,
+    ActionCISA.ACT: DecisionPriority.IMMEDIATE,
 }
 
-class DecisionOutcome:
-    def __init__(self,
-            action: DecisionAction
-        ):
+
+class OutcomeCISA:
+    def __init__(self, action: ActionCISA):
         self.priority: DecisionPriority = priority_map[action]
-        self.action: DecisionAction = action
+        self.action: ActionCISA = action
+
 
 class Decision:
     exploitation: ExploitationLevel
     automatable: Automatable
     technical_impact: TechnicalImpact
     mission_wellbeing: MissionWellbeingImpact
-    outcome: DecisionOutcome
+    outcome: OutcomeCISA
+    methodology: Methodology = Methodology.CISA
 
-    def __init__(self,
-        exploitation: ExploitationLevel = None,
-        automatable: Automatable = None,
-        technical_impact: TechnicalImpact = None,
-        mission_wellbeing: MissionWellbeingImpact = None
+    def __init__(
+        self,
+        exploitation: ExploitationLevel | str = None,
+        automatable: Automatable | str = None,
+        technical_impact: TechnicalImpact | str = None,
+        mission_wellbeing: MissionWellbeingImpact | str = None,
+        methodology: Methodology | str = Methodology.CISA,
     ):
         if isinstance(exploitation, str):
             exploitation = ExploitationLevel(exploitation)
         if isinstance(automatable, str):
             automatable = Automatable(automatable)
         if isinstance(technical_impact, str):
             technical_impact = TechnicalImpact(technical_impact)
         if isinstance(mission_wellbeing, str):
             mission_wellbeing = MissionWellbeingImpact(mission_wellbeing)
+        if isinstance(methodology, str):
+            methodology = Methodology(methodology)
 
         self.exploitation = exploitation
         self.automatable = automatable
         self.technical_impact = technical_impact
         self.mission_wellbeing = mission_wellbeing
-        if all([
-            isinstance(self.exploitation, ExploitationLevel),
-            isinstance(self.automatable, Automatable),
-            isinstance(self.technical_impact, TechnicalImpact),
-            isinstance(self.mission_wellbeing, MissionWellbeingImpact)
-        ]):
+        self.methodology = methodology
+        if all(
+            [
+                isinstance(self.exploitation, ExploitationLevel),
+                isinstance(self.automatable, Automatable),
+                isinstance(self.technical_impact, TechnicalImpact),
+                isinstance(self.mission_wellbeing, MissionWellbeingImpact),
+            ]
+        ):
             self.evaluate()
 
-    def evaluate(self) -> DecisionOutcome:
+    def evaluate(self) -> OutcomeCISA:
+        if self.methodology == Methodology.CISA:
+            return self.cisa()
+
+    def cisa(self) -> OutcomeCISA:
         """
-        Evaluates the decision based on the provided attributes and returns a DecisionOutcome object.
+        Evaluates the decision based on the provided attributes and returns a OutcomeCISA object.
 
         Raises:
             AttributeError: If any of the required attributes (exploitation, automatable, technical_impact, mission_wellbeing) are not provided.
         """
-        self._validate_attributes()
+        self._validate_cisa()
         decision_matrix = {
             ExploitationLevel.NONE: {
                 Automatable.YES: {
                     TechnicalImpact.TOTAL: {
-                        MissionWellbeingImpact.HIGH: DecisionAction.ATTEND
+                        MissionWellbeingImpact.HIGH: ActionCISA.ATTEND
                     },
                 },
                 Automatable.NO: {
                     TechnicalImpact.TOTAL: {
-                        MissionWellbeingImpact.HIGH: DecisionAction.TRACK_STAR
+                        MissionWellbeingImpact.HIGH: ActionCISA.TRACK_STAR
                     },
-                }
+                },
             },
             ExploitationLevel.POC: {
                 Automatable.YES: {
                     TechnicalImpact.TOTAL: {
-                        MissionWellbeingImpact.MEDIUM: DecisionAction.TRACK_STAR,
-                        MissionWellbeingImpact.HIGH: DecisionAction.ATTEND
+                        MissionWellbeingImpact.MEDIUM: ActionCISA.TRACK_STAR,
+                        MissionWellbeingImpact.HIGH: ActionCISA.ATTEND,
                     },
                     TechnicalImpact.PARTIAL: {
-                        MissionWellbeingImpact.HIGH: DecisionAction.ATTEND
+                        MissionWellbeingImpact.HIGH: ActionCISA.ATTEND
                     },
                 },
                 Automatable.NO: {
                     TechnicalImpact.PARTIAL: {
-                        MissionWellbeingImpact.HIGH: DecisionAction.TRACK_STAR
+                        MissionWellbeingImpact.HIGH: ActionCISA.TRACK_STAR
                     },
                     TechnicalImpact.TOTAL: {
-                        MissionWellbeingImpact.MEDIUM: DecisionAction.TRACK_STAR,
-                        MissionWellbeingImpact.HIGH: DecisionAction.ATTEND
-                    }
-                }
+                        MissionWellbeingImpact.MEDIUM: ActionCISA.TRACK_STAR,
+                        MissionWellbeingImpact.HIGH: ActionCISA.ATTEND,
+                    },
+                },
             },
             ExploitationLevel.ACTIVE: {
                 Automatable.YES: {
                     TechnicalImpact.PARTIAL: {
-                        MissionWellbeingImpact.LOW: DecisionAction.ATTEND,
-                        MissionWellbeingImpact.MEDIUM: DecisionAction.ATTEND,
-                        MissionWellbeingImpact.HIGH: DecisionAction.ACT
+                        MissionWellbeingImpact.LOW: ActionCISA.ATTEND,
+                        MissionWellbeingImpact.MEDIUM: ActionCISA.ATTEND,
+                        MissionWellbeingImpact.HIGH: ActionCISA.ACT,
                     },
                     TechnicalImpact.TOTAL: {
-                        MissionWellbeingImpact.LOW: DecisionAction.ATTEND,
-                        MissionWellbeingImpact.MEDIUM: DecisionAction.ACT,
-                        MissionWellbeingImpact.HIGH: DecisionAction.ACT
-                    }
+                        MissionWellbeingImpact.LOW: ActionCISA.ATTEND,
+                        MissionWellbeingImpact.MEDIUM: ActionCISA.ACT,
+                        MissionWellbeingImpact.HIGH: ActionCISA.ACT,
+                    },
                 },
                 Automatable.NO: {
                     TechnicalImpact.PARTIAL: {
-                        MissionWellbeingImpact.HIGH: DecisionAction.ATTEND
+                        MissionWellbeingImpact.HIGH: ActionCISA.ATTEND
                     },
                     TechnicalImpact.TOTAL: {
-                        MissionWellbeingImpact.MEDIUM: DecisionAction.ATTEND,
-                        MissionWellbeingImpact.HIGH: DecisionAction.ACT
-                    }
-                }
-            }
+                        MissionWellbeingImpact.MEDIUM: ActionCISA.ATTEND,
+                        MissionWellbeingImpact.HIGH: ActionCISA.ACT,
+                    },
+                },
+            },
         }
         # Lookup decision based on attributes and return outcome
-        return DecisionOutcome(
-            decision_matrix
-                .get(self.exploitation, {})
-                .get(self.automatable, {})
-                .get(self.technical_impact, {})
-                .get(self.mission_wellbeing, DecisionAction.TRACK)
+        return OutcomeCISA(
+            decision_matrix.get(self.exploitation, {})
+            .get(self.automatable, {})
+            .get(self.technical_impact, {})
+            .get(self.mission_wellbeing, ActionCISA.TRACK)
         )
 
-    def _validate_attributes(self):
+    def _validate_cisa(self):
         if not isinstance(self.exploitation, ExploitationLevel):
-            raise AttributeError('ExploitationLevel has not been provided')
+            raise AttributeError("ExploitationLevel has not been provided")
         if not isinstance(self.automatable, Automatable):
-            raise AttributeError('Automatable has not been provided')
+            raise AttributeError("Automatable has not been provided")
         if not isinstance(self.technical_impact, TechnicalImpact):
-            raise AttributeError('TechnicalImpact has not been provided')
+            raise AttributeError("TechnicalImpact has not been provided")
         if not isinstance(self.mission_wellbeing, MissionWellbeingImpact):
-            raise AttributeError('MissionWellbeingImpact has not been provided')
+            raise AttributeError("MissionWellbeingImpact has not been provided")
```

### Comparing `ssvc-1.0.2/PKG-INFO` & `ssvc-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssvc
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python implementation of the Stakeholder-Specific Vulnerability Categorization framework.
 Author: Christopher Langton
 Author-email: chris@langton.cloud
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -31,44 +31,44 @@
 ### Example
 
 To use SSVC:
 - Determine the exploitation status of the vulnerability
 - Assess the technical impact, considering the automatability
 
 ```python
-from ssvc import Decision, ExploitationLevel, Automatable, TechnicalImpact, MissionWellbeingImpact, DecisionAction, DecisionPriority
+from ssvc import Decision, ExploitationLevel, Automatable, TechnicalImpact, MissionWellbeingImpact, ActionCISA, DecisionPriority
 decision = Decision(
     ExploitationLevel.POC,
     Automatable.YES,
     TechnicalImpact.PARTIAL,
     MissionWellbeingImpact.MEDIUM,
 )
 assert decision.outcome.priority == DecisionPriority.LOW, "SSVC priority should be LOW"
-assert decision.outcome.action == DecisionAction.TRACK, "SSVC decision should be TRACK"
+assert decision.outcome.action == ActionCISA.TRACK, "SSVC decision should be TRACK"
 ```
 
 Using strings also works
 
 ```python
 import ssvc
 
 decision = ssvc.Decision(
     exploitation='active',
     automatable='no',
     technical_impact='total',
     mission_wellbeing='high',
 )
 assert decision.outcome.priority == ssvc.DecisionPriority.HIGH, "SSVC priority should be HIGH"
-assert decision.outcome.action == ssvc.DecisionAction.ACT, "SSVC decision should be ACT"
+assert decision.outcome.action == ssvc.ActionCISA.ACT, "SSVC decision should be ACT"
 ```
 
 Input incrementally and control how to handle decisions
 
 ```python
-from ssvc import Decision, ExploitationLevel, Automatable, TechnicalImpact, MissionWellbeingImpact, DecisionAction, DecisionPriority
+from ssvc import Decision, ExploitationLevel, Automatable, TechnicalImpact, MissionWellbeingImpact, ActionCISA, DecisionPriority
 decision = Decision()
 # what is the ExploitationLevel?
 decision.exploitation = ExploitationLevel.POC
 # is it Automatable?
 decision.automatable = Automatable.YES
 # figure out the technical impact
 decision.technical_impact = TechnicalImpact.PARTIAL
@@ -77,10 +77,10 @@
 
 # Get a decision outcome
 outcome = decision.evaluate()
 
 # decisions are return and available as a new variable
 assert outcome.priority == DecisionPriority.LOW, "SSVC priority should be LOW"
 # or use the `decision.outcome` like before
-assert decision.outcome.action == DecisionAction.TRACK, "SSVC decision should be TRACK"
+assert decision.outcome.action == ActionCISA.TRACK, "SSVC decision should be TRACK"
 ```
```

