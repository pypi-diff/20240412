# Comparing `tmp/nmfu-0.5.5.tar.gz` & `tmp/nmfu-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmfu-0.5.5.tar", last modified: Sat Nov  4 21:37:21 2023, max compression
+gzip compressed data, was "nmfu-0.5.6.tar", last modified: Fri Apr 12 15:06:37 2024, max compression
```

## Comparing `nmfu-0.5.5.tar` & `nmfu-0.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0     1001     1001        0 2023-11-04 21:37:21.455432 nmfu-0.5.5/
--rw-rw-r--   0     1001     1001    35150 2023-11-04 21:37:05.000000 nmfu-0.5.5/LICENSE
--rw-r--r--   0     1001     1001     3134 2023-11-04 21:37:21.451432 nmfu-0.5.5/PKG-INFO
--rw-rw-r--   0     1001     1001     1809 2023-11-04 21:37:05.000000 nmfu-0.5.5/README.md
-drwxr-xr-x   0     1001     1001        0 2023-11-04 21:37:21.451432 nmfu-0.5.5/nmfu.egg-info/
--rw-r--r--   0     1001     1001     3134 2023-11-04 21:37:21.000000 nmfu-0.5.5/nmfu.egg-info/PKG-INFO
--rw-r--r--   0     1001     1001      219 2023-11-04 21:37:21.000000 nmfu-0.5.5/nmfu.egg-info/SOURCES.txt
--rw-r--r--   0     1001     1001        1 2023-11-04 21:37:21.000000 nmfu-0.5.5/nmfu.egg-info/dependency_links.txt
--rw-r--r--   0     1001     1001       36 2023-11-04 21:37:21.000000 nmfu-0.5.5/nmfu.egg-info/entry_points.txt
--rw-r--r--   0     1001     1001       84 2023-11-04 21:37:21.000000 nmfu-0.5.5/nmfu.egg-info/requires.txt
--rw-r--r--   0     1001     1001        5 2023-11-04 21:37:21.000000 nmfu-0.5.5/nmfu.egg-info/top_level.txt
--rw-rw-r--   0     1001     1001   268165 2023-11-04 21:37:05.000000 nmfu-0.5.5/nmfu.py
--rw-rw-r--   0     1001     1001      100 2023-11-04 21:37:05.000000 nmfu-0.5.5/pyproject.toml
--rw-r--r--   0     1001     1001       41 2023-11-04 21:37:21.455432 nmfu-0.5.5/setup.cfg
--rw-rw-r--   0     1001     1001     1855 2023-11-04 21:37:05.000000 nmfu-0.5.5/setup.py
+drwxr-xr-x   0     1001     1001        0 2024-04-12 15:06:37.501599 nmfu-0.5.6/
+-rw-rw-r--   0     1001     1001    35150 2024-04-12 15:06:28.000000 nmfu-0.5.6/LICENSE
+-rw-r--r--   0     1001     1001     3134 2024-04-12 15:06:37.501599 nmfu-0.5.6/PKG-INFO
+-rw-rw-r--   0     1001     1001     1809 2024-04-12 15:06:28.000000 nmfu-0.5.6/README.md
+drwxr-xr-x   0     1001     1001        0 2024-04-12 15:06:37.501599 nmfu-0.5.6/nmfu.egg-info/
+-rw-r--r--   0     1001     1001     3134 2024-04-12 15:06:37.000000 nmfu-0.5.6/nmfu.egg-info/PKG-INFO
+-rw-r--r--   0     1001     1001      219 2024-04-12 15:06:37.000000 nmfu-0.5.6/nmfu.egg-info/SOURCES.txt
+-rw-r--r--   0     1001     1001        1 2024-04-12 15:06:37.000000 nmfu-0.5.6/nmfu.egg-info/dependency_links.txt
+-rw-r--r--   0     1001     1001       36 2024-04-12 15:06:37.000000 nmfu-0.5.6/nmfu.egg-info/entry_points.txt
+-rw-r--r--   0     1001     1001       84 2024-04-12 15:06:37.000000 nmfu-0.5.6/nmfu.egg-info/requires.txt
+-rw-r--r--   0     1001     1001        5 2024-04-12 15:06:37.000000 nmfu-0.5.6/nmfu.egg-info/top_level.txt
+-rw-rw-r--   0     1001     1001   277417 2024-04-12 15:06:28.000000 nmfu-0.5.6/nmfu.py
+-rw-rw-r--   0     1001     1001      100 2024-04-12 15:06:28.000000 nmfu-0.5.6/pyproject.toml
+-rw-r--r--   0     1001     1001       41 2024-04-12 15:06:37.501599 nmfu-0.5.6/setup.cfg
+-rw-rw-r--   0     1001     1001     1855 2024-04-12 15:06:28.000000 nmfu-0.5.6/setup.py
```

### Comparing `nmfu-0.5.5/LICENSE` & `nmfu-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nmfu-0.5.5/PKG-INFO` & `nmfu-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmfu
-Version: 0.5.5
+Version: 0.5.6
 Summary: A parser generator that turns procedural programs into C state machines
 Home-page: https://github.com/mincrmatt12/nmfu
 Author: Matthew Mirvish
 Author-email: matthew@mm12.xyz
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/mincrmatt12/nmfu/issues
 Project-URL: Source Code, https://github.com/mincrmatt12/nmfu
```

### Comparing `nmfu-0.5.5/README.md` & `nmfu-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nmfu-0.5.5/nmfu.egg-info/PKG-INFO` & `nmfu-0.5.6/nmfu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmfu
-Version: 0.5.5
+Version: 0.5.6
 Summary: A parser generator that turns procedural programs into C state machines
 Home-page: https://github.com/mincrmatt12/nmfu
 Author: Matthew Mirvish
 Author-email: matthew@mm12.xyz
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/mincrmatt12/nmfu/issues
 Project-URL: Source Code, https://github.com/mincrmatt12/nmfu
```

### Comparing `nmfu-0.5.5/nmfu.py` & `nmfu-0.5.6/nmfu.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 """
 
-__version__ = "0.5.5"
+__version__ = "0.5.6"
 
 import abc
 import enum
 import string
 import itertools
 import queue
 import io
@@ -545,33 +545,18 @@
 
         for transition in self.all_transitions():
             if transition.actions:
                 return False
 
         return True
 
-    def equivalent_on_values(self):
-        r"""
-        Compute an "equivalent" set of on_values, such that taking any one will have at least one valid path through all directly-attached condition points, in addition
-        to a set of on_values which map to the treat_as_else state in _all_ outcomes.
-
-        i.e. for  a -t-> b -<c>-> c
-                   \-f-> d -<else>-> e
-                          \-<f>-> ELSE
-
-        we'd return ({c, else}, {f}), since f should go to an error state in some equivalent state E replacing a, and c/else should continue on. This lets us rewrite the dfa as
-
-        E -{c,else}=> a -> ...
-         \-f=> ELSE 
-
-        which is a valid construction for append_after.
+    def non_proxy_frontiers(self):
+        """
+        Return the set of states reachable from following only proxy states, starting at this state.
         """
-
-        encountered = set()
-        candidate_else = set()
 
         visited = set()
         sources = set()
 
         def aux(state):
             if state in visited:
                 return
@@ -582,21 +567,46 @@
                     # Also consider actions with overrides
                     for action in t.actions:
                         if action.get_target_override_mode() in (ActionOverrideMode.MAY_GOTO_TARGET, ActionOverrideMode.ALWAYS_GOTO_OTHER):
                             for extra in action.get_target_override_targets():
                                 aux(extra)
             else:
                 sources.add(state)
-                for t in state.all_transitions():
-                    if t.error_handling:
-                        candidate_else.update(t.on_values)
-                    else:
-                        encountered.update(t.on_values)
 
         aux(self)
+        
+        return sources
+
+    def equivalent_on_values(self):
+        r"""
+        Compute an "equivalent" set of on_values, such that taking any one will have at least one valid path through all directly-attached condition points, in addition
+        to a set of on_values which map to the treat_as_else state in _all_ outcomes.
+
+        i.e. for  a -t-> b -<c>-> c
+                   \-f-> d -<else>-> e
+                          \-<f>-> ELSE
+
+        we'd return ({c, else}, {f}), since f should go to an error state in some equivalent state E replacing a, and c/else should continue on. This lets us rewrite the dfa as
+
+        E -{c,else}=> a -> ...
+         \-f=> ELSE 
+
+        which is a valid construction for append_after.
+        """
+
+        encountered = set()
+        candidate_else = set()
+
+        sources = self.non_proxy_frontiers()
+        for state in sources:
+            for t in state.all_transitions():
+                if t.error_handling:
+                    candidate_else.update(t.on_values)
+                else:
+                    encountered.update(t.on_values)
 
         filtered = set()
         for possible in candidate_else:
             for state in sources:
                 if state[possible] is None:
                     continue
                 if not state[possible].error_handling:
@@ -830,23 +840,44 @@
 
         if sub_states is None:
             sub_states = self.accepting_states
 
         if chain_actions is None:
             chain_actions = []
 
+        fake_initial_transition = None
+
+        def resolve_transitions_for_error(transition, symbolset):
+            if transition is not fake_initial_transition:
+                yield transition
+            else:
+                condition_point: DFConditionPoint = transition.target
+                visited = set()
+                for i in condition_point.non_proxy_frontiers():
+                    local_symbolset = symbolset.copy()
+                    if DFTransition.Else in local_symbolset:
+                        local_symbolset.remove(DFTransition.Else)
+                        local_symbolset |= i.compute_foreign_else_definition(condition_point)
+                    for symbol in local_symbolset:
+                        transition = i[symbol]
+                        if transition in visited:
+                            continue
+                        visited.add(transition)
+                        if not transition.error_handling:
+                            yield transition
+
         if isinstance(chained_dfa.starting_state, DFProxyState):
             # Add an extra state that will represent the condition point properly (see docs for equivalent_on_values)
             valid, to_else = chained_dfa.starting_state.equivalent_on_values()
             if valid and to_else:
                 fake_start = DFState()
                 chained_dfa.add(fake_start)
 
                 fake_start[valid] = chained_dfa.starting_state
-                fake_start[valid].fallthrough(True)
+                fake_initial_transition = fake_start[valid].fallthrough(True)
                 fake_start[to_else] = chained_dfa.starting_state
                 fake_start[to_else].fallthrough(True).handles_else()
                 chained_dfa.starting_state = fake_start
 
         # If the caller wants to chain actions into a DFA which potentially matches the empty string, we have to place the actions onto 
         # transitions going into the sub_states, instead of on transitions coming out of them that we generate. This adds more opportunities
         # for "unable to schedule strict"-type errors, but avoids missing actions in these cases.
@@ -877,47 +908,69 @@
 
             culled_chained_transitions = []
 
             for transition in chained_transitions:
                 culled_transition = transition.copy()
 
                 relevant_values = set(transition.on_values)
+                irrelevant_values = set()
                 if DFTransition.Else in relevant_values:
                     relevant_values.update(local_else_meaning)
                 target = sub_state[relevant_values]
                 if target is None:
                     targets = set()
-                    target_map = {}
                     for value in relevant_values:
                         v = sub_state[value]
                         if v is None:
+                            irrelevant_values.add(value)
                             continue
                         targets.add(v)
-                        if v not in target_map: target_map[v] = set()
-                        target_map[v].add(value)
+                    relevant_values -= irrelevant_values
                 else:
                     targets = {target} 
-                    target_map = {target: relevant_values}
+
+                # targets is the set of all (potentially) conflicting transitions
 
                 if transition.error_handling:
                     # Cull values
                     for j in relevant_values.copy():
                         if sub_state[j] is not None and not sub_state[j].error_handling:
                             relevant_values.remove(j)
                 elif not all(x.error_handling or x.target == transition.target for x in targets):
                     if ProgramData.dump(DebugDumpable.DFA) and ProgramData.do(ProgramFlag.VERBOSE_AMBIG_ERRORS): # pragma: no cover
                         debug_dump_dfa(self, "ae_dfa2", highlight=sub_state)
                         debug_dump_dfa(chained_dfa, "ae_dfa1")
                     dprint[ProgramFlag.VERBOSE_AMBIG_ERRORS]("TT", transition)
                     dprint[ProgramFlag.VERBOSE_AMBIG_ERRORS]("TA", targets)
+                    targets = [x for x in targets if not x.error_handling and x.target != transition.target]
+                    dprint[ProgramFlag.VERBOSE_AMBIG_ERRORS]("TAF", targets)
                     dprint[ProgramFlag.VERBOSE_AMBIG_ERRORS]("RV", relevant_values)
-                    raise IllegalDFAStateConflictsError("Ambiguous transitions detected while joining DFAs", sub_state, transition)
+                    for i in relevant_values:
+                        if sub_state[i] not in targets:
+                            irrelevant_values.add(i)
+                    relevant_values -= irrelevant_values
+                    dprint[ProgramFlag.VERBOSE_AMBIG_ERRORS]("RVF", relevant_values)
+                    
+                    # Come up with a reasonable description of which characters are ambiguous
+                    if relevant_values == {DFTransition.Else}: # wildcard notation hard to represent
+                        rv_suffix = ""
+                    else:
+                        relevant_values_in_msg = relevant_values - {DFTransition.Else}
+                        if len(relevant_values_in_msg) >= 3:
+                            relevant_values_in_msg = list(relevant_values_in_msg)[:3]
+                        if ProgramData.do(ProgramFlag.CODEPOINTS_IN_ERRORS):
+                            rv_suffix = f" on symbol{'s' if len(relevant_values_in_msg) > 1 else ''} {', '.join(format(ord(x), '02x') for x in relevant_values_in_msg)}"
+                        else:
+                            rv_suffix = f" on character{'s' if len(relevant_values_in_msg) > 1 else ''} {', '.join(repr(x) for x in (relevant_values_in_msg))}"
+
+                    raise IllegalDFAStateConflictsError("Ambiguous transitions detected while joining DFAs" + rv_suffix, *itertools.chain(
+                        *(resolve_transitions_for_error(x, relevant_values) for x in targets)), *resolve_transitions_for_error(transition, relevant_values))
 
                 # Create transition to add
-                culled_transition.on_values = list(relevant_values)
+                culled_transition.on_values = list(relevant_values | irrelevant_values)
                 culled_transition.attach(*chain_actions, prepend=True)
                 culled_chained_transitions.append(culled_transition)
 
             for new_transition in culled_chained_transitions:
                 sub_state.transition(new_transition, allow_replace_if=lambda x: x.error_handling or x.target in valid_replacers)
 
         # Adopt all the states
@@ -989,14 +1042,17 @@
 
     # Verbosity options (enabled by various levels of -v or, ofc, -f)
     VERBOSE_REGEX_CCLASS = 200
     VERBOSE_OPTIMIZE_RESULTS = 201
     VERBOSE_SIMPLIFY_TM = 202
     VERBOSE_AMBIG_ERRORS = 203
 
+    # Error reporting flags
+    CODEPOINTS_IN_ERRORS = (400, "Report codepoints instead of characters in error messages", False, (101,))
+
     # Optimization flags, set in ProgramData
     # DFA optimization options (enabled by various levels of -O)
     SIMPLIFY_ELSE_CONDITIONS = 300
     REMOVE_INACCESIBLE_STATES = 301
     USE_DELETE_FOR_EMPTY_STRING = 302
     SHORTCIRCUIT_FALLTHROUGHS = 303
 
@@ -1032,14 +1088,15 @@
     USE_PACKED_ENUMS = (32, "Define all enumerations with __attribute__((packed))", False)
 
     # Debug options
     DEBUG_DFA_HIDE_ERROR_HANDLING = (100, "", True)
     DEBUG_DFA_BINARY_LABELS = (101, "Show all transition labels as hex points", False)
     DEBUG_STRICT_PROGRAM_DATA_ERRORS = (102, "Throw an error if the ProgramData tree is updated in an invalid way", False)
     DEBUG_DTREE_HIDE_GC = (103, "Don't show entries in dtree if they've been garbage collected", True)
+    DEBUG_DTREE_AS_GRAPH = (104, "Dump the debug tag tree as a graphviz graph instead of to stdout", False)
 
 class ProgramOption(enum.Enum):
     def __init__(self, default, helpstr):
         self.default = default
         self.helpstr = helpstr
 
     # DFA optimization options
@@ -1146,14 +1203,17 @@
 
     @classmethod
     def lookup(cls, obj: object, tag: DTAG, recurse_upwards=True, default=None, recurse_downwards=True):
         """
         Find the imbued object's data, or -- if none exists -- find it's parents
         """
 
+        if obj is None:
+            return None
+
         if type(obj) is lark.Token:
             if tag == DTAG.SOURCE_LINE:
                 return obj.line
             elif tag == DTAG.SOURCE_COLUMN:
                 return obj.column
             else:
                 return default
@@ -1170,28 +1230,28 @@
 
         # Ensure consistency
         if type(obj) is int and obj in cls._refmap and cls._refmap[obj]() is None:
             del cls._refmap[id_obj]
             cls._collection[id_obj] = {}
 
         if tag not in ProgramData._collection[id_obj]:
-            if DTAG.PARENT in ProgramData._collection[id_obj] and recurse_upwards:
-                val = cls.lookup(ProgramData._collection[id_obj][DTAG.PARENT], tag)
-                if val is not None:
-                    return val
             if isinstance(obj, HasDefaultDebugInfo):
                 val = obj.debug_lookup(tag)
                 if val is not None:
                     return val
             elif isinstance(obj, int) and id_obj in cls._refmap:
                 v_obj = cls._refmap[id_obj]()
                 if isinstance(v_obj, HasDefaultDebugInfo):
                     val = v_obj.debug_lookup(tag)
                     if val is not None:
                         return val
+            if DTAG.PARENT in ProgramData._collection[id_obj] and recurse_upwards:
+                val = cls.lookup(ProgramData._collection[id_obj][DTAG.PARENT], tag)
+                if val is not None:
+                    return val
             if tag in (DTAG.SOURCE_COLUMN, DTAG.SOURCE_LINE) and recurse_downwards:
                 for i in cls._children[id_obj]:
                     val = cls.lookup(i, tag, recurse_upwards=False)
                     if val is not None:
                         return val
             return default
         return ProgramData._collection[id_obj][tag]
@@ -1494,15 +1554,15 @@
             if name:
                 info_str += f"- {name}:"
                 if line is not None:
                     info_str += f"\n  at line {line}:\n{ProgramData.get_source_line(line)}"
                     if column is not None:
                         info_str += "\n" + NMFUError._generate_whitespace_marker(line, column)
                 else:
-                    info_str = info_str[-1]
+                    info_str = info_str[:-1]
             else:
                 if line is not None:
                     info_str += f"- line {line}:\n{ProgramData.get_source_line(line)}"
                     if column is not None:
                         info_str += "\n" + NMFUError._generate_whitespace_marker(line, column)
                 else:
                     continue
@@ -2123,18 +2183,20 @@
 
         where i is the input string
         """
         for j, character in enumerate(self.match_contents):
             next_state = DFState()
             start_action_holder = (self.start_actions if j == 0 else [])
             t = DFTransition([character]).attach(*start_action_holder, *self.char_actions).to(next_state)
+            ProgramData.imbue(state, DTAG.NAME, f"direct match {self.match_contents!r}[{j}]")
             state[DFTransition.Else] = DFTransition().to(current_error_handlers[ErrorReasons.NO_MATCH]).attach(*start_action_holder).fallthrough().handles_else()
             if j == len(self.match_contents) - 1:
                 t.attach(*self.finish_actions)
                 sm.mark_accepting(next_state)
+                ProgramData.imbue(next_state, DTAG.NAME, f"direct match {self.match_contents!r}[{j}]")
             state.transition(t)
             sm.add(next_state)
             state = next_state
         return sm
 
 class CaseDirectMatch(Match, HasDefaultDebugInfo):
     """A direct string match w/ case insensitivity"""
@@ -2167,18 +2229,20 @@
 
         where i is the input string
         """
         for j, character in enumerate(self.match_contents):
             next_state = DFState()
             start_action_holder = (self.start_actions if j == 0 else [])
             t = DFTransition(self._create_casei_from(character)).attach(*start_action_holder, *self.char_actions).to(next_state)
+            ProgramData.imbue(state, DTAG.NAME, f"casei match {self.match_contents!r}[{j}]")
             state[DFTransition.Else] = DFTransition().to(current_error_handlers[ErrorReasons.NO_MATCH]).attach(*start_action_holder).fallthrough().handles_else()
             if j == len(self.match_contents) - 1:
                 t.attach(*self.finish_actions)
                 sm.mark_accepting(next_state)
+                ProgramData.imbue(next_state, DTAG.NAME, f"casei match {self.match_contents!r}[{j}]")
             state.transition(t)
             sm.add(next_state)
             state = next_state
         return sm
 
 class OutputStorageType(enum.Enum):
     BOOL = 0
@@ -2476,15 +2540,15 @@
 
         if self.op == CompareIntegerExprOp.LT:
             return left < right
         elif self.op == CompareIntegerExprOp.GT:
             return left > right
         elif self.op == CompareIntegerExprOp.LE:
             return left <= right
-        elif self.op == CompareIntegerExprOp.LE:
+        elif self.op == CompareIntegerExprOp.GE:
             return left >= right
         elif self.op == CompareIntegerExprOp.EQ:
             return left == right
         elif self.op == CompareIntegerExprOp.NE:
             return left != right
         else:
             return False
@@ -2632,14 +2696,17 @@
 # ==========
 # GENERAL RE 
 # ==========
 
 class RegexCharClass:
     def __init__(self, chars):
         self.chars = frozenset(chars)
+
+    def clone(self):
+        return RegexCharClass(self.chars)
         
     def isdisjoint(self, other):
         """
         Are these two character classes disjoint?
         """
         if isinstance(other, InvertedRegexCharClass):
             return self.chars <= other.chars
@@ -2683,14 +2750,17 @@
     def __repr__(self):
         return f"<{self.__class__.__name__} of {self.chars!r}>"
 
     def invert(self):
         return InvertedRegexCharClass(self.chars)
 
 class InvertedRegexCharClass(RegexCharClass):
+    def clone(self):
+        return InvertedRegexCharClass(self.chars)
+
     def isdisjoint(self, other):
         if isinstance(other, InvertedRegexCharClass):
             return len(self.chars | other.chars) >= 256 # TODO: add unicode/specific number of symbols support; for all real uses inverted sets are _never_ disjoint
         elif isinstance(other, RegexCharClass):
             return other.isdisjoint(self)
 
     def split(self, other):
@@ -2738,23 +2808,29 @@
         self.sub_matches = list(sub_matches)
         for sub_match in self.sub_matches:
             ProgramData.imbue(sub_match, DTAG.PARENT, self)
 
 class RegexNFState:
     Epsilon = object()
 
+    class TransitionMeta:
+        pass
+
     def __init__(self):
         self.transitions = {}
         self.epsilon_moves = set() 
+        self.transition_dbg_metas = {}
 
     def transition(self, symbol, target):
         if symbol == RegexNFState.Epsilon:
             self.epsilon_moves.add(target)
         else:
             self.transitions[symbol] = target
+        if symbol not in self.transition_dbg_metas:
+            self.transition_dbg_metas[symbol] = ProgramData.imbue(RegexNFState.TransitionMeta(), DTAG.PARENT, self)
         return self
 
     def epsilon_closure(self, visited=None):
         if visited is None:
             visited = set()
         total_moves = set((self,))
         for move in self.epsilon_moves:
@@ -2792,18 +2868,21 @@
             if state in index_cache:
                 return index_cache[state]
             index_cache[state] = self.states.index(state)
             return index_cache[state]
 
         def moves(states, on):
             results = set() 
+            upstream_meta = None
             for i in states:
                 if on in self.states[i].transitions:
                     results.add(get_index(self.states[i].transitions[on]))
-            return results
+                    if upstream_meta is None:
+                        upstream_meta = self.states[i].transition_dbg_metas[on]
+            return results, upstream_meta
 
         def epsilon_closure(states):
             total = set()
             for i in states:
                 total |= set(get_index(x) for x in self.states[i].epsilon_closure())
             return frozenset(total)
 
@@ -2818,27 +2897,28 @@
         ProgramData.imbue(visited_states[start_dfa_state], DTAG.PARENT, self.states[next(iter(start_dfa_state))])
 
         while not to_process.empty():
             processing = to_process.get()
             # find all potential edges
             for potential_move in alphabet:
                 # is there anything here
-                move_result = moves(processing, potential_move)
+                move_result, move_meta = moves(processing, potential_move)
                 if move_result:
                     # the new state is the e-closure
                     new_state = epsilon_closure(move_result)
                     if new_state not in visited_states:
                         # create the new state
                         visited_states[new_state] = RegexNFState()
                         ProgramData.imbue(visited_states[new_state], DTAG.PARENT, self.states[next(iter(new_state))])
                         # should it be a finishing state?
                         if finishing_idx in new_state:
                             target_dfa.mark_finishing(visited_states[new_state])
                         to_process.put(new_state)
                     visited_states[processing].transition(potential_move, visited_states[new_state])
+                    ProgramData.imbue(visited_states[processing].transition_dbg_metas[potential_move], DTAG.PARENT, move_meta)
 
         # add all the states
         for i in visited_states.values():
             target_dfa.add(i)
 
         return target_dfa
 
@@ -2914,14 +2994,15 @@
 
             for (character, target) in state.transitions.items():
                 target_subset = partition_containing(target)
 
                 if target_subset not in new_states:
                     add_back(target_subset)
                 new_state.transition(character, new_states[target_subset])
+                ProgramData.imbue(new_state.transition_dbg_metas[character], DTAG.PARENT, state.transition_dbg_metas[character])
 
             return new_state
 
         new_dfa.start_state = add_back(partition_containing(self.start_state))
         return new_dfa
 
 
@@ -2950,67 +3031,68 @@
         Convert the regex tree object into the NFA using Thompson construction. Return the finish state
         """
         ProgramData.imbue(start_state, DTAG.PARENT, r)
 
         if isinstance(r, RegexCharClass):
             # Simply convert to a boring form
             end_state = RegexNFState()
-            ProgramData.imbue(end_state, DTAG.PARENT, start_state)
             self.nfa.add(end_state)
             start_state.transition(r, end_state)
-            return end_state
+            ProgramData.imbue(start_state.transition_dbg_metas[r], DTAG.PARENT, r)
+            return ProgramData.imbue(end_state, DTAG.PARENT, r)
         elif isinstance(r, RegexAlternation):
             r"""
             Use the union form:
              /e-(s    f)-e\
             q              f 
              \e-(s2  f2)-e/
             """
             # Create a set of start states
             sub_starts = [RegexNFState() for x in r.sub_matches]
             end_state = RegexNFState()
             self.nfa.add(end_state, *sub_starts)
-            ProgramData.imbue(end_state, DTAG.PARENT, start_state)
             # Link everything up
             for i, j in zip(sub_starts, r.sub_matches):
                 # Link e from start to sub start
                 start_state.transition(RegexNFState.Epsilon, i)
                 # Create sub expr & link to end
                 self._convert_to_nfa(j, i).transition(RegexNFState.Epsilon, end_state)
-            return end_state
+            return ProgramData.imbue(end_state, DTAG.PARENT, r)
         elif isinstance(r, RegexSequence):
             # Chain them all together
             for i in r.sub_matches:
                 start_state = self._convert_to_nfa(i, start_state)
             return start_state
         elif isinstance(r, RegexOptional):
             # Create a kleene star without the repetition bit
             end_state = RegexNFState()
             sub_start = RegexNFState()
             self.nfa.add(end_state, sub_start)
-            ProgramData.imbue(end_state, DTAG.PARENT, start_state)
             start_state.transition(RegexNFState.Epsilon, end_state).transition(RegexNFState.Epsilon, sub_start)
-            self._convert_to_nfa(r.sub_match, sub_start).transition(RegexNFState.Epsilon, end_state)
-            return end_state
+            sub_end = self._convert_to_nfa(r.sub_match, sub_start)
+            sub_end.transition(RegexNFState.Epsilon, end_state)
+            ProgramData.imbue(sub_end.transition_dbg_metas[RegexNFState.Epsilon], DTAG.PARENT, r)
+            return ProgramData.imbue(end_state, DTAG.PARENT, r)
         elif isinstance(r, RegexKleene):
             r"""
             Use the kleene form:
                      <-e-
                     /    \
             q -e-> (s    f) -e-> f
              \                  /
               --- ----e--> -----
             """
             end_state = RegexNFState()
             sub_start = RegexNFState()
             self.nfa.add(end_state, sub_start)
-            ProgramData.imbue(end_state, DTAG.PARENT, start_state)
             start_state.transition(RegexNFState.Epsilon, end_state).transition(RegexNFState.Epsilon, sub_start)
-            self._convert_to_nfa(r.sub_match, sub_start).transition(RegexNFState.Epsilon, end_state).transition(RegexNFState.Epsilon, sub_start)
-            return end_state
+            sub_end = self._convert_to_nfa(r.sub_match, sub_start)
+            sub_end.transition(RegexNFState.Epsilon, end_state).transition(RegexNFState.Epsilon, sub_start)
+            ProgramData.imbue(sub_end.transition_dbg_metas[RegexNFState.Epsilon], DTAG.PARENT, r)
+            return ProgramData.imbue(end_state, DTAG.PARENT, r)
         else:
             raise NotImplementedError("unknown")
 
     def _simplify_regex_tree(self, r):
         """
         Simplify the regex tree recursively
         """
@@ -3028,27 +3110,27 @@
         tree_data = regex_tree.data
         if tree_data.startswith("binary_"):
             tree_data = tree_data[len("binary_"):]
         if tree_data in ("regex", "regex_group"):
             return RegexSequence(self._interpret_parse_tree(x) for x in regex_tree.children)
         elif tree_data in ("regex_any", "regex_char_class", "regex_set", "regex_inverted_set"):
             return ProgramData.imbue(
-                RegexAlternation(self.character_class_mappings[list(self._visit_all_char_classes(regex_tree))[0]]),
+                RegexAlternation([x.clone() for x in self.character_class_mappings[list(self._visit_all_char_classes(regex_tree))[0]]]),
                 DTAG.SOURCE_LINE, regex_tree.meta.line,
                 DTAG.SOURCE_COLUMN, regex_tree.meta.column
             )
         elif tree_data == "regex_alternation":
             return ProgramData.imbue(
                 RegexAlternation(self._interpret_parse_tree(x) for x in regex_tree.children),
                 DTAG.SOURCE_LINE, regex_tree.meta.line,
                 DTAG.SOURCE_COLUMN, regex_tree.meta.column
             )
         elif tree_data == "regex_raw_match":
             return ProgramData.imbue(
-                RegexAlternation(self.character_class_mappings[self._convert_raw_regex_unimportant(regex_tree.children[0])]),
+                RegexAlternation([x.clone() for x in self.character_class_mappings[self._convert_raw_regex_unimportant(regex_tree.children[0])]]),
                 DTAG.SOURCE_LINE, regex_tree.meta.line,
                 DTAG.SOURCE_COLUMN, regex_tree.meta.column
             )
         elif tree_data == "regex_operation":
             sub_match = self._interpret_parse_tree(regex_tree.children[0])
             if regex_tree.children[1].value == "+":
                 val = RegexSequence((sub_match, RegexKleene(sub_match)))
@@ -3211,25 +3293,30 @@
         new_transitions = {frozenset((DFTransition.Else,)): (else_path, False)}
 
         new_state = DFState()
         ProgramData.imbue(new_state, DTAG.PARENT, nfdfa_state)
         self.out_dfa_cache[id(nfdfa_state)] = new_state
         into.add(new_state)
 
+        new_transition_upstreams = {}
+
         if nfdfa_state in self.dfa_2.finishing_states:
             into.mark_accepting(new_state)
 
         for source, target in transitions.items():
             if isinstance(source, InvertedRegexCharClass):
                 # TODO: handle multiple of these
                 # Convert to a normal set
                 new_transitions[source.chars | frozenset((DFTransition.End,))] = (else_path, False)
                 new_transitions[frozenset((DFTransition.Else,))] = (self._create_dfa_state(target, into, False, else_path), target in self.dfa_2.finishing_states)
+                new_transition_upstreams[DFTransition.Else] = nfdfa_state.transition_dbg_metas[source]
             else:
                 new_transitions[source.chars] = (self._create_dfa_state(target, into, False, else_path), target in self.dfa_2.finishing_states)
+                for i in source.chars:
+                    new_transition_upstreams[i] = nfdfa_state.transition_dbg_metas[source]
 
         # Simplify
         new_transitions_inverse = defaultdict(list) 
         for source, target in new_transitions.items():
             new_transitions_inverse[target].append(source)
 
         new_transitions = {}
@@ -3261,19 +3348,21 @@
                     raise IllegalDFAStateConflictsError("Duplicate transition", target, new_state)
                 else:
                     # They are else, remove from them
                     for x in source:
                         if x in conflict.on_values:
                             conflict.on_values.remove(x)
 
-            new_state.transition(DFTransition(list(source)).to(target).attach(*actions).fallthrough(target == else_path).handles_else(target == else_path))
+            new_transition = DFTransition(list(source)).to(target).attach(*actions).fallthrough(target == else_path).handles_else(target == else_path)
+            if new_transition.on_values[0] in new_transition_upstreams:
+                ProgramData.imbue(new_transition, DTAG.PARENT, new_transition_upstreams[new_transition.on_values[0]])
+            new_state.transition(new_transition)
 
         return new_state
 
-
     def convert(self, current_error_handlers: dict):
         # First convert to an NFA
         self.nfa = RegexNFA()
         start_state = RegexNFState()
         self.nfa.add(start_state)
         self.nfa.mark_finishing(self._convert_to_nfa(self.regex_tree, start_state))
         # Then convert to a DFA
@@ -3482,32 +3571,40 @@
 
         new_dfa = DFA()
 
         converted_states = {}
         corresponding_finish_states = {dfa: [] for dfa in ds}
         to_process = queue.Queue()
 
-        def create_real_state_of(state):
+        def create_real_state_of(state, upstream_metas=None):
             new_state = DFState()
             ProgramData.imbue(new_state, DTAG.PARENT, next(iter(state))[1])
 
             corresponds_to_finishes_in = set() 
+            finish_upstream_metas = {}
+            upstream_meta_replacement = {}
+            
+            if upstream_metas is not None:
+                for trans in upstream_metas:
+                    upstream_meta_replacement[trans.target] = trans
+
             is_part_of = set()
             for sub_dfa, sub_state in state:
                 if sub_state in sub_dfa.accepting_states:
                     corresponds_to_finishes_in.add(sub_dfa)
+                    finish_upstream_metas[sub_dfa] = upstream_meta_replacement.get(sub_state, sub_state)
                 is_part_of.add(sub_dfa)
 
             if len(corresponds_to_finishes_in) > 1:
                 if not self.greedy:
-                    raise IllegalDFAStateConflictsError("Ambigious case label: multiple possible finishes", *corresponds_to_finishes_in)
+                    raise IllegalDFAStateConflictsError("Ambigious case label: multiple possible finishes", *finish_upstream_metas.values())
                 target = max(corresponds_to_finishes_in, key=lambda x: priorities[x])
                 if sum(1 for x in corresponds_to_finishes_in if priorities[x] == priorities[target]) > 1:
                     raise IllegalDFAStateConflictsError("Ambigious case label: multiple possible finishes with same priority {}".format(priorities[target]), 
-                            *(x for x in corresponds_to_finishes_in if priorities[x] == priorities[target]))
+                            *(finish_upstream_metas[x] for x in corresponds_to_finishes_in if priorities[x] == priorities[target]))
                 corresponding_finish_states[target].append(new_state)
                 new_dfa.mark_accepting(new_state)
             elif len(corresponds_to_finishes_in) == 1:
                 if len(is_part_of) != 1 and not self.greedy:
                     raise IllegalDFAStateConflictsError("Ambigious case label: should finish or check next. If you mean to finish, use a greedy case.", *is_part_of)
                 corresponding_finish_states[next(iter(corresponds_to_finishes_in))].append(new_state)
                 new_dfa.mark_accepting(new_state)
@@ -3563,38 +3660,42 @@
                 #   a) at least one state correctly matches this symbol, and the others do not
                 #      in this case, we should just discard those other states (since there is no
                 #      reason to "speculatively execute" the error state, obviously)
                 #   b) none of the states correctly match this symbol, in which case it is an overall error.
                 #      in this case, we should add the symbol to the list of symbols that we will assign
                 #      an error transition to
                 found_else_transition = False
+                upstream_metas = []
                 for (sub_dfa, sub_state) in processing:
                     potential_transition = sub_state[symbol]
                     if potential_transition is None:
                         continue
                     if potential_transition.error_handling:
                         found_else_transition = True
                         continue
                     else:
                         next_state.add((sub_dfa, potential_transition.target))
+                        upstream_metas.append(potential_transition)
 
                 # if case b) is met 
                 if not next_state:
                     actual_else |= symbol
                     continue
 
                 next_state = frozenset(next_state)
 
                 if next_state not in converted_states:
                     to_process.put(next_state)
-                    next_state = create_real_state_of(next_state)
+                    next_state = create_real_state_of(next_state, upstream_metas)
                 else:
                     next_state = converted_states[next_state]
 
-                converted_states[processing][symbol] = next_state
+                converted_states[processing].transition(
+                        ProgramData.imbue(DFTransition(symbol).to(next_state), DTAG.PARENT, upstream_metas[0]), 
+                        allow_replace=True)
 
             # check if we need else (is this a finishing state)
             if converted_states[processing] in new_dfa.accepting_states:
                 continue
 
             if DFTransition.Else in actual_else:
                 # just use it
@@ -3744,15 +3845,15 @@
                 self.start_actions.append(action)
             else:
                 self.finish_actions.append(action)
 
     def convert(self, current_error_handlers):
         sub_dfa = self.sub_contents.convert(current_error_handlers)
         if sub_dfa.starting_state in sub_dfa.accepting_states:
-            raise IllegalDFAStateError("Ambigious path in optional: should use optional or go to next", sub_dfa)
+            raise IllegalDFAStateError("Ambigious path in optional: should use optional or go to next", sub_dfa.starting_state)
 
         sub_dfa.mark_accepting(sub_dfa.starting_state)
 
         # Add starting actions
         for trans in sub_dfa.starting_state.transitions:
             trans.attach(*self.start_actions)
 
@@ -3841,15 +3942,15 @@
                     should_try_to_append = True
                     break
 
         # Verify that the accepting states are all distinct TODO: make this properly do ambiguity resolution
         for accept_state in sub_dfa.accepting_states:
             for transition in accept_state.all_transitions():
                 if transition.target in sub_dfa.accepting_states:
-                    raise IllegalDFAStateConflictsError("Ambigious loop: should loop or continue matching", accept_state, transition.target)
+                    raise IllegalDFAStateConflictsError("Ambigious loop: should loop or continue matching", transition)
 
         # If there are error-handling transitions on the accept node, point them to the starting node as fallthrough (so that anything that _isn't_ getting matched by 
         # the last node gets forwarded to the start, looping). If there are no transitions on the final node, point everything to the start.
         for accept_state in sub_dfa.accepting_states:
             for trans in accept_state.transitions:
                 if trans.error_handling:
                     trans.handles_else(False).fallthrough().to(sub_dfa.starting_state).attach(*self.loop_start_actions)
@@ -3858,15 +3959,15 @@
 
         for state in sub_dfa.states:
             parent_dfa.add(state)
 
         parent_dfa.starting_state = sub_dfa.starting_state
 
         if self.next and not should_try_to_append:
-            raise IllegalASTStateError("Unreachable states after loop", self.next)
+            raise IllegalASTStateError("Unreachable states after loop", self, self.next)
 
         return parent_dfa
 
 class TryExceptNode(ActionSinkNode, ActionSourceNode):
     def __init__(self, handles):
         self.handler_node = DFState()
         self.handles = handles
@@ -4153,26 +4254,26 @@
         self.finish_codes = []
     
     def parse(self):
         # Parse state_object_spec
         for out in self._parse_tree.find_data("out_decl"):
             out_obj = self._parse_out_decl(out)
             if out_obj.name in self.state_object_spec:
-                raise DuplicateDefinitionError("output variable", out_obj, out_obj.name)
+                raise DuplicateDefinitionError("output variable", out, out_obj.name)
             if out_obj.holds_a(OutputStorageType.ENUM):
                 if any(x.upper() == out_obj.name.upper() for x in self.state_object_spec):
-                    raise DuplicateDefinitionError("enum header name", out_obj, out_obj.name.upper())
+                    raise DuplicateDefinitionError("enum header name", out, out_obj.name.upper())
                 if out_obj.name == "finish":
                     raise IllegalParseTree("Enumerations cannot be named 'finish'", out)
             self.state_object_spec[out_obj.name] = out_obj
         # Parse macros
         for macro in self._parse_tree.find_data("macro_decl"):
             macro_obj = Macro(macro.children[0], macro.children[2:], self._parse_macro_arguments(macro.children[1]))
             if macro_obj.name in self.macros:
-                raise DuplicateDefinitionError("macro", macro_obj, macro_obj.name)
+                raise DuplicateDefinitionError("macro", macro, macro_obj.name)
             self.macros[macro_obj.name] = macro_obj
 
         for hook in self._parse_tree.find_data("hook_decl"):
             if hook.children[0].value in self.hooks:
                 raise DuplicateDefinitionError("hook", hook.children[0], hook.children[0].value)
             self.hooks.append(hook.children[0].value)
 
@@ -4240,15 +4341,15 @@
             }[context]
 
             if name not in storage:
                 raise UndefinedReferenceError({
                     MacroArgumentKind.MACRO: "macro",
                     MacroArgumentKind.OUT: "variable",
                     MacroArgumentKind.LOOP: "break target"
-                }, from_tree)
+                }[context], from_tree)
 
             return storage[name]
 
     def _parse_macro_arguments(self, args: lark.Tree):
         if args.data == "macro_arg_empty":
             return []
         defined = set()
@@ -4757,15 +4858,17 @@
             loop_node = LoopNode(loop_name)
             previous_break = self.innermost_break_handler
             self.break_handlers[loop_name] = loop_node.get_break_handler()
             self.innermost_break_handler = loop_node.get_break_handler()
             child_node = self._parse_stmt_seq(statements)
             self.innermost_break_handler = previous_break
             loop_node.set_child(child_node)
-            return loop_node
+            return ProgramData.imbue(loop_node,
+                DTAG.SOURCE_LINE, stmt.meta.line,
+                DTAG.SOURCE_COLUMN, stmt.meta.column)
         elif stmt.data == "try_stmt":
             catch_block = stmt.children[-1]
             # try to see if there are options, otherwise use all
             catch_block_stmts = catch_block.children[:]
             catch_handles = set(ErrorReasons)
 
             if catch_block.children and catch_block.children[0].data == "catch_options":
@@ -4800,15 +4903,18 @@
             if not isinstance(action_node, ActionSourceNode):
                 raise IllegalASTStateError("Invalid statement in foreach actions; must only be an action source", action_node)
 
             each_actions, action_node = action_node.adopt_actions_from()
             if action_node is not None:
                 raise IllegalASTStateError("Invalid statement in foreach actions; must only be action source with no DFA", action_node)
 
-            return ForeachNode(content_node, each_actions)
+            return ProgramData.imbue(
+                ForeachNode(content_node, each_actions),
+                DTAG.SOURCE_LINE, stmt.meta.line,
+                DTAG.SOURCE_COLUMN, stmt.meta.column)
         else:
             raise IllegalParseTree("Unknown statement", stmt)
 
     def _parse_stmt_seq(self, stmts: List[lark.Tree]) -> Node:
         """
         Parse a set of statements into one big node
         """
@@ -6371,16 +6477,100 @@
     for tag in DTAG:
         if tag in (DTAG.PARENT, DTAG.NAME): continue
         aux = ProgramData.lookup(v, tag, recurse_upwards=False, recurse_downwards=False)
         if aux is not None:
             lprint(f" {tag}: {aux}")
 
     for i in ProgramData._children[v]:
+        if id(ProgramData.lookup(i, DTAG.PARENT)) != v:
+            continue
         debug_dump_datatree(i, indent+2, disallow, target=target)
 
+def debug_dump_datatree_graph(v: object, out_name: str = "dtree"):
+    if not debug_enabled:
+        raise RuntimeError("Debugging was disabled! You probably need to install graphviz")
+
+    anon_counter = 0
+
+    def newid():
+        nonlocal anon_counter
+        anon_counter += 1
+        return f"anon-{anon_counter}"
+
+    g = graphviz.Graph(name='dfa', comment=ProgramData.lookup(v, DTAG.NAME))
+    g.attr(rankdir="LR")
+
+    def escape(x: str):
+        return graphviz.escape(x).replace("<", "\\<").replace(">", "\\>").replace("{", "\\{").replace("}", "\\}").replace("\n", "\\n")
+
+    def aux(v: object, disallow: list) -> str:
+        nonlocal g
+
+        if v in disallow or id(v) in disallow:
+            nid = newid()
+            g.node(nid, "<recerr>", color="red")
+            return nid
+
+        disallow = [v, *disallow]
+
+        if type(v) is int and v in ProgramData._refmap and ProgramData._refmap[v]() is not None:
+            v = ProgramData._refmap[v]()
+
+        nid = str(id(v) if type(v) is not int else v)
+
+        name = ProgramData.lookup(v, DTAG.NAME, recurse_upwards=False)
+        if name is None:
+            if type(v) is int and ProgramData.do(ProgramFlag.DEBUG_DTREE_HIDE_GC):
+                g.node(nid, "<gcd>", color="grey")
+                return nid
+            elif type(v) is int:
+                name = "<unk>"
+            else:
+                name = repr(v)
+
+        auxdat = []
+        for tag in DTAG:
+            if tag in (DTAG.PARENT, DTAG.NAME): continue
+            val = ProgramData.lookup(v, tag, recurse_upwards=False, recurse_downwards=False)
+            if val is not None:
+                auxdat.append(f"{tag}: {val}")
+
+        auxdat = '\n'.join(auxdat)
+        if auxdat:
+            contents = graphviz.nohtml(f"<head>{escape(name)}|{escape(auxdat)}")
+        else:
+            contents = graphviz.nohtml(f"<head>{escape(name)}")
+        g.node(nid, contents, shape="record")
+        
+        if type(v) is not int:
+            v = id(v)
+
+        for i in ProgramData._children[v]:
+            if id(ProgramData.lookup(i, DTAG.PARENT)) != v:
+                continue
+            childid = aux(i, disallow)
+            g.edge(nid, childid)
+
+        return nid + ":head"
+
+    if v is None:
+        for key in ProgramData._children.copy():
+            if ProgramData.lookup(key, DTAG.PARENT, recurse_upwards=False) is None:
+                if ProgramData.do(ProgramFlag.DEBUG_DTREE_HIDE_GC) and (key not in ProgramData._refmap or ProgramData._refmap[key]() is None):
+                    continue
+                aux(key, [])
+    else:
+        aux(v, [])
+
+    if ProgramData.option(ProgramOption.DEBUG_GRAPH_DUMP_FORMAT) == "dot":
+        g.save(out_name + ".dot")
+    else:
+        g.render(out_name, format=ProgramData.option(ProgramOption.DEBUG_GRAPH_DUMP_FORMAT), cleanup=True)
+
+
 def main(): # pragma: no cover
     try:
         input_file, program_name = ProgramData.load_commandline_flags(sys.argv[1:])
     except RuntimeError as e:
         print(str(e), file=sys.stderr)
         print("Try nmfu --help for more information", file=sys.stderr)
         exit(1)
@@ -6410,42 +6600,46 @@
             raise
         else:
             print("Parse error:", str(e), file=sys.stderr)
             exit(4)
 
     if ProgramData.dump(DebugDumpable.AST): debug_dump_ast(pctx.ast, ProgramData.dump_prefix + ".ast")
 
-    dctx = DfaCompileCtx(pctx)
-    try:
-        dctx.compile()
-    except NMFUError as e:
-        if ProgramData.dump(DebugDumpable.TRACEBACK):
-            raise
-        else:
-            print("Compile error:", str(e), file=sys.stderr)
-            exit(5)
-
-    if ProgramData.dump(DebugDumpable.DFA): debug_dump_dfa(dctx.dfa, ProgramData.dump_prefix + ".dfa")
-    if ProgramData.dry_run:
-        if ProgramData.dump(DebugDumpable.DTREE): debug_dump_datatree(None)
-        print("... dry run, skipping code generation")
-        exit(0)
-
-    cctx = CodegenCtx(dctx, program_name)
     try:
-        header = cctx.generate_header()
-        source = cctx.generate_source()
-    except NMFUError as e:
-        if ProgramData.dump(DebugDumpable.TRACEBACK):
-            raise
-        else:
-            print("Codegen error:", str(e), file=sys.stderr)
-            exit(5)
+        dctx = DfaCompileCtx(pctx)
+        try:
+            dctx.compile()
+        except NMFUError as e:
+            if ProgramData.dump(DebugDumpable.TRACEBACK):
+                raise
+            else:
+                print("Compile error:", str(e), file=sys.stderr)
+                exit(5)
+
+        if ProgramData.dump(DebugDumpable.DFA): debug_dump_dfa(dctx.dfa, ProgramData.dump_prefix + ".dfa")
+        if ProgramData.dry_run:
+            print("... dry run, skipping code generation")
+            exit(0)
 
-    if ProgramData.dump(DebugDumpable.DTREE): debug_dump_datatree(None)
+        cctx = CodegenCtx(dctx, program_name)
+        try:
+            header = cctx.generate_header()
+            source = cctx.generate_source()
+        except NMFUError as e:
+            if ProgramData.dump(DebugDumpable.TRACEBACK):
+                raise
+            else:
+                print("Codegen error:", str(e), file=sys.stderr)
+                exit(5)
+    finally:
+        if ProgramData.dump(DebugDumpable.DTREE): 
+            if ProgramData.do(ProgramFlag.DEBUG_DTREE_AS_GRAPH):
+                debug_dump_datatree_graph(None, ProgramData.dump_prefix + ".dtree")
+            else:
+                debug_dump_datatree(None)
 
     with open(program_name + ".h", "w") as f:
         f.write(header)
     with open(program_name + ".c", "w") as f:
         f.write(source)
 
 if __name__ == "__main__":
```

### Comparing `nmfu-0.5.5/setup.py` & `nmfu-0.5.6/setup.py`

 * *Files identical despite different names*

