# Comparing `tmp/pabutools-1.1.6.tar.gz` & `tmp/pabutools-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pabutools-1.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pabutools-1.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pabutools-1.1.6.tar` & `pabutools-1.1.7.tar`

### file list

```diff
@@ -1,52 +1,55 @@
--rw-r--r--   0        0        0    35149 2024-03-27 09:51:37.912343 pabutools-1.1.6/LICENSE.md
--rw-r--r--   0        0        0     3352 2024-03-27 09:51:37.912343 pabutools-1.1.6/README.md
--rw-r--r--   0        0        0      134 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/__init__.py
--rw-r--r--   0        0        0     1547 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/analysis/__init__.py
--rw-r--r--   0        0        0     3606 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/analysis/category.py
--rw-r--r--   0        0        0     4426 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/analysis/cohesiveness.py
--rw-r--r--   0        0        0     2355 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/analysis/instanceproperties.py
--rw-r--r--   0        0        0     8892 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/analysis/justifiedrepresentation.py
--rw-r--r--   0        0        0     9227 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/analysis/mesanalytics.py
--rw-r--r--   0        0        0     7560 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/analysis/profileproperties.py
--rw-r--r--   0        0        0     7271 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/analysis/votersatisfaction.py
--rw-r--r--   0        0        0      354 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/__init__.py
--rw-r--r--   0        0        0     3204 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/ballot/__init__.py
--rw-r--r--   0        0        0     6982 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/ballot/approvalballot.py
--rw-r--r--   0        0        0     4021 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/ballot/ballot.py
--rw-r--r--   0        0        0     6598 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/ballot/cardinalballot.py
--rw-r--r--   0        0        0     6294 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/ballot/cumulativeballot.py
--rw-r--r--   0        0        0    10197 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/ballot/ordinalballot.py
--rw-r--r--   0        0        0    19273 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/instance.py
--rw-r--r--   0        0        0    17766 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/pabulib.py
--rw-r--r--   0        0        0    10769 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/preflib.py
--rw-r--r--   0        0        0     3348 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/profile/__init__.py
--rw-r--r--   0        0        0    20997 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/profile/approvalprofile.py
--rw-r--r--   0        0        0    19673 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/profile/cardinalprofile.py
--rw-r--r--   0        0        0    22245 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/profile/cumulativeprofile.py
--rw-r--r--   0        0        0    13634 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/profile/ordinalprofile.py
--rw-r--r--   0        0        0    15116 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/profile/profile.py
--rw-r--r--   0        0        0     7238 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/satisfaction/__init__.py
--rw-r--r--   0        0        0    28263 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/satisfaction/additivesatisfaction.py
--rw-r--r--   0        0        0    10650 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/satisfaction/functionalsatisfaction.py
--rw-r--r--   0        0        0     5005 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/satisfaction/positionalsatisfaction.py
--rw-r--r--   0        0        0     6353 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/satisfaction/satisfactionmeasure.py
--rw-r--r--   0        0        0    15184 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/election/satisfaction/satisfactionprofile.py
--rw-r--r--   0        0        0     2239 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/fractions.py
--rw-r--r--   0        0        0     2224 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/__init__.py
--rw-r--r--   0        0        0     2437 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/budgetallocation.py
--rw-r--r--   0        0        0     6126 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/composition.py
--rw-r--r--   0        0        0     7659 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/exhaustion.py
--rw-r--r--   0        0        0    11764 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/greedywelfare.py
--rw-r--r--   0        0        0    13029 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/maxwelfare.py
--rw-r--r--   0        0        0      451 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/mes/__init__.py
--rw-r--r--   0        0        0     7787 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/mes/mes_details.py
--rw-r--r--   0        0        0    29521 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/mes/mes_rule.py
--rw-r--r--   0        0        0     8080 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/rules/phragmen.py
--rw-r--r--   0        0        0     4934 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/tiebreaking.py
--rw-r--r--   0        0        0     3007 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/utils.py
--rw-r--r--   0        0        0        0 2024-03-27 09:51:37.948343 pabutools-1.1.6/pabutools/visualisation/__init__.py
--rw-r--r--   0        0        0    34383 2024-03-27 09:51:37.952343 pabutools-1.1.6/pabutools/visualisation/templates/mes_page_summary_template.html
--rw-r--r--   0        0        0    31671 2024-03-27 09:51:37.952343 pabutools-1.1.6/pabutools/visualisation/templates/mes_round_analysis_template.html
--rw-r--r--   0        0        0    11516 2024-03-27 09:51:37.952343 pabutools-1.1.6/pabutools/visualisation/visualisation.py
--rw-r--r--   0        0        0     1353 2024-03-27 09:51:37.952343 pabutools-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 pabutools-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-12 12:36:56.021838 pabutools-1.1.7/LICENSE.md
+-rw-r--r--   0        0        0     3352 2024-04-12 12:36:56.021838 pabutools-1.1.7/README.md
+-rw-r--r--   0        0        0      134 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/__init__.py
+-rw-r--r--   0        0        0     1547 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/analysis/__init__.py
+-rw-r--r--   0        0        0     3606 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/analysis/category.py
+-rw-r--r--   0        0        0     4426 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/analysis/cohesiveness.py
+-rw-r--r--   0        0        0     2355 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/analysis/instanceproperties.py
+-rw-r--r--   0        0        0     8892 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/analysis/justifiedrepresentation.py
+-rw-r--r--   0        0        0     9966 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/analysis/mesanalytics.py
+-rw-r--r--   0        0        0     7568 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/analysis/profileproperties.py
+-rw-r--r--   0        0        0     7271 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/analysis/votersatisfaction.py
+-rw-r--r--   0        0        0      354 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/__init__.py
+-rw-r--r--   0        0        0     3204 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/ballot/__init__.py
+-rw-r--r--   0        0        0     6982 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/ballot/approvalballot.py
+-rw-r--r--   0        0        0     4021 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/ballot/ballot.py
+-rw-r--r--   0        0        0     6598 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/ballot/cardinalballot.py
+-rw-r--r--   0        0        0     6294 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/ballot/cumulativeballot.py
+-rw-r--r--   0        0        0    10197 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/ballot/ordinalballot.py
+-rw-r--r--   0        0        0    19273 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/instance.py
+-rw-r--r--   0        0        0    17766 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/pabulib.py
+-rw-r--r--   0        0        0    10769 2024-04-12 12:36:56.057838 pabutools-1.1.7/pabutools/election/preflib.py
+-rw-r--r--   0        0        0     3348 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/profile/__init__.py
+-rw-r--r--   0        0        0    20997 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/profile/approvalprofile.py
+-rw-r--r--   0        0        0    19673 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/profile/cardinalprofile.py
+-rw-r--r--   0        0        0    22245 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/profile/cumulativeprofile.py
+-rw-r--r--   0        0        0    13634 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/profile/ordinalprofile.py
+-rw-r--r--   0        0        0    15116 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/profile/profile.py
+-rw-r--r--   0        0        0     7238 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/satisfaction/__init__.py
+-rw-r--r--   0        0        0    28263 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/satisfaction/additivesatisfaction.py
+-rw-r--r--   0        0        0    10650 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/satisfaction/functionalsatisfaction.py
+-rw-r--r--   0        0        0     5005 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/satisfaction/positionalsatisfaction.py
+-rw-r--r--   0        0        0     6353 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/satisfaction/satisfactionmeasure.py
+-rw-r--r--   0        0        0    15184 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/election/satisfaction/satisfactionprofile.py
+-rw-r--r--   0        0        0     2239 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/fractions.py
+-rw-r--r--   0        0        0     2225 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/__init__.py
+-rw-r--r--   0        0        0     2438 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/budgetallocation.py
+-rw-r--r--   0        0        0     6126 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/composition.py
+-rw-r--r--   0        0        0     8133 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/exhaustion.py
+-rw-r--r--   0        0        0      434 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/greedywelfare/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/greedywelfare/greedywelfare_details.py
+-rw-r--r--   0        0        0    12821 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/greedywelfare/greedywelfare_rule.py
+-rw-r--r--   0        0        0    13430 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/maxwelfare.py
+-rw-r--r--   0        0        0      451 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/mes/__init__.py
+-rw-r--r--   0        0        0     7785 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/mes/mes_details.py
+-rw-r--r--   0        0        0    29520 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/mes/mes_rule.py
+-rw-r--r--   0        0        0     8080 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/rules/phragmen.py
+-rw-r--r--   0        0        0     4934 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/tiebreaking.py
+-rw-r--r--   0        0        0     3007 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/utils.py
+-rw-r--r--   0        0        0      262 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/visualisation/__init__.py
+-rw-r--r--   0        0        0    32898 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/visualisation/templates/greedy_round_analysis_template.html
+-rw-r--r--   0        0        0    44846 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/visualisation/templates/mes_page_summary_template.html
+-rw-r--r--   0        0        0    40986 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/visualisation/templates/mes_round_analysis_template.html
+-rw-r--r--   0        0        0    23948 2024-04-12 12:36:56.061838 pabutools-1.1.7/pabutools/visualisation/visualisation.py
+-rw-r--r--   0        0        0     1353 2024-04-12 12:36:56.061838 pabutools-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 pabutools-1.1.7/PKG-INFO
```

### Comparing `pabutools-1.1.6/LICENSE.md` & `pabutools-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/README.md` & `pabutools-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/analysis/__init__.py` & `pabutools-1.1.7/pabutools/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/analysis/category.py` & `pabutools-1.1.7/pabutools/analysis/category.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/analysis/cohesiveness.py` & `pabutools-1.1.7/pabutools/analysis/cohesiveness.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/analysis/instanceproperties.py` & `pabutools-1.1.7/pabutools/analysis/instanceproperties.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/analysis/justifiedrepresentation.py` & `pabutools-1.1.7/pabutools/analysis/justifiedrepresentation.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/analysis/mesanalytics.py` & `pabutools-1.1.7/pabutools/analysis/mesanalytics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from pabutools.utils import Numeric
 from pabutools.election.instance import Instance, Project
 from pabutools.election.profile import Profile
-from pabutools.rules.budgetallocation import AllocationDetails
+from pabutools.rules.budgetallocation import BudgetAllocation, AllocationDetails
 from pabutools.rules.mes.mes_rule import method_of_equal_shares
 
 
 class ProjectLoss(Project):
     """
     Class used to represent the projects and how much budget they lost due to other projects being picked.
     This extends the :py:class:`~pabutools.election.instance.Project` and thus represents the project itself.
@@ -91,19 +91,20 @@
         if verbose:
             print(f"Rule did not have any iterations, returning empty list")
         return []
 
     project_losses = []
     voter_count = len(allocation_details.iterations[0].voters_budget)
     voter_multiplicity = allocation_details.voter_multiplicity
+    iterations_count = len(allocation_details.iterations)
     voter_spendings: dict[int, list[tuple[Project, Numeric]]] = {}
     for idx in range(voter_count):
         voter_spendings[idx] = []
 
-    for iteration in allocation_details.iterations:
+    for idx, iteration in enumerate(allocation_details.iterations):
         project_losses.append(
             _create_project_loss(
                 iteration.selected_project,
                 iteration.voters_budget,
                 voter_spendings,
                 voter_multiplicity,
                 verbose,
@@ -116,15 +117,18 @@
                     iteration.selected_project,
                     iteration.voters_budget[supporter_idx]
                     - iteration.voters_budget_after_selection[supporter_idx],
                 )
             )
 
         for project_detail in iteration:
-            if project_detail.discarded:
+            if project_detail.discarded or (
+                idx == iterations_count - 1
+                and project_detail.project != iteration.selected_project
+            ):
                 project_losses.append(
                     _create_project_loss(
                         project_detail.project,
                         iteration.voters_budget_after_selection,
                         voter_spendings,
                         voter_multiplicity,
                         verbose,
@@ -133,71 +137,79 @@
 
     return project_losses
 
 
 def calculate_effective_supports(
     instance: Instance,
     profile: Profile,
+    allocation: BudgetAllocation,
     mes_params: dict | None = None,
     final_budget: Numeric | None = None,
 ) -> dict[Project, int]:
     """
     Returns a dictionary of :py:class:`~pabutools.election.instance.project` and their effective support
     in a given instance, profile and mes election. Effective support for a project is an analytical metric
     which allows to measure the ratio of initial budget received to minimal budget required to win.
     Effective support is represented in percentages.
 
     Parameters
     ----------
         instance: :py:class:`~pabutools.election.instance.Instance`
             The instance.
-        profile : :py:class:`~pabutools.election.profile.profile.AbstractProfile`
+        profile: :py:class:`~pabutools.election.profile.profile.AbstractProfile`
             The profile.
+        allocation: :py:class:`~pabutools.rules.budgetallocation.BudgetAllocation`
+            Resulting allocation of the above instance & profile.
         mes_params: dict, optional
             Dictionary of additional parameters that are passed as keyword arguments to the MES rule.
             Defaults to None.
         final_budget: Numeric, optional
             Numeric value of the final budget which will replace the instance budget. Allows for simulating
             exhaustive MES.
 
     Returns
     -------
         dict[:py:class:`~pabutools.election.instance.Project`, int]
             Dictionary of pairs (:py:class:`~pabutools.election.instance.Project`, effective support).
     """
+    if mes_params is None:
+        mes_params = {}
     effective_supports: dict[Project, int] = {}
     if final_budget:
         instance.budget_limit = final_budget
     for project in instance:
         effective_supports[project] = calculate_effective_support(
-            instance, profile, project, mes_params
+            instance, profile, project, project in allocation, mes_params
         )
 
     return effective_supports
 
 
 def calculate_effective_support(
     instance: Instance,
     profile: Profile,
     project: Project,
+    was_picked: bool,
     mes_params: dict | None = None,
 ) -> int:
     """
     Calculates the effective support of a given project in a given instance, profile and mes election.
-    Effective support for a project is an analytical metric which allows to measure the ratio of 
+    Effective support for a project is an analytical metric which allows to measure the ratio of
     initial budget received to minimal budget required to win. Effective support is represented in percentages.
 
     Parameters
     ----------
         instance: :py:class:`~pabutools.election.instance.Instance`
             The instance.
         profile : :py:class:`~pabutools.election.profile.profile.AbstractProfile`
             The profile.
         project: :py:class:`~pabutools.election.instance.Project`
             Project for which effective support is calculated. Must be a part of the instance.
+        was_picked: bool
+            Whether the considerd project was picked as a winner in the allocation.
         mes_params: dict, optional
             Dictionary of additional parameters that are passed as keyword arguments to the MES rule.
             Defaults to `{}`.
 
     Returns
     -------
         int
@@ -206,17 +218,19 @@
     if project not in instance:
         raise RuntimeError("Provided instance does not match the allocation details")
     if mes_params is None:
         mes_params = {}
     mes_params["analytics"] = True
     mes_params["skipped_project"] = project
     mes_params["resoluteness"] = True
-    return method_of_equal_shares(
-        instance, profile, **mes_params
-    ).details.skipped_project_eff_support
+    details = method_of_equal_shares(instance, profile, **mes_params).details
+    effective_support = details.skipped_project_eff_support
+    if was_picked:
+        effective_support = max(effective_support, 100)
+    return effective_support
 
 
 def _create_project_loss(
     project: Project,
     current_voters_budget: list[Numeric],
     voter_spendings: dict[int, list[tuple[Project, Numeric]]],
     voter_multiplicity: list[int],
```

### Comparing `pabutools-1.1.6/pabutools/analysis/profileproperties.py` & `pabutools-1.1.7/pabutools/analysis/profileproperties.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,18 @@
                 project_votes[project_id] = 1
 
     for prof in profile:
         update_votes(list(prof))
 
     return project_votes
 
-def voter_flow_matrix(instance: Instance, profile: AbstractCardinalProfile) -> dict[str, dict[str, int]]:
+
+def voter_flow_matrix(
+    instance: Instance, profile: AbstractCardinalProfile
+) -> dict[str, dict[str, int]]:
     """
     Returns the voter flow matrix. The voter flow matrix is a 2D dictionary where voter_flow[a][b] is the number of
     voters for 'a' who voted for 'b'
 
     Parameters
     ----------
         instance : :py:class:`~pabutools.election.instance.Instance`
@@ -262,8 +265,8 @@
                 voter_flow[str(vote_list[j])][str(vote_list[i])] += 1
         if len(vote_list) == 1:
             voter_flow[str(vote_list[0])][str(vote_list[0])] += 1
 
     for vote in profile:
         update_voter_flow(list(vote))
 
-    return voter_flow
+    return voter_flow
```

### Comparing `pabutools-1.1.6/pabutools/analysis/votersatisfaction.py` & `pabutools-1.1.7/pabutools/analysis/votersatisfaction.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/ballot/__init__.py` & `pabutools-1.1.7/pabutools/election/ballot/__init__.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/ballot/approvalballot.py` & `pabutools-1.1.7/pabutools/election/ballot/approvalballot.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/ballot/ballot.py` & `pabutools-1.1.7/pabutools/election/ballot/ballot.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/ballot/cardinalballot.py` & `pabutools-1.1.7/pabutools/election/ballot/cardinalballot.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/ballot/cumulativeballot.py` & `pabutools-1.1.7/pabutools/election/ballot/cumulativeballot.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/ballot/ordinalballot.py` & `pabutools-1.1.7/pabutools/election/ballot/ordinalballot.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/instance.py` & `pabutools-1.1.7/pabutools/election/instance.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/pabulib.py` & `pabutools-1.1.7/pabutools/election/pabulib.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/preflib.py` & `pabutools-1.1.7/pabutools/election/preflib.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/profile/__init__.py` & `pabutools-1.1.7/pabutools/election/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/profile/approvalprofile.py` & `pabutools-1.1.7/pabutools/election/profile/approvalprofile.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/profile/cardinalprofile.py` & `pabutools-1.1.7/pabutools/election/profile/cardinalprofile.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/profile/cumulativeprofile.py` & `pabutools-1.1.7/pabutools/election/profile/cumulativeprofile.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/profile/ordinalprofile.py` & `pabutools-1.1.7/pabutools/election/profile/ordinalprofile.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/profile/profile.py` & `pabutools-1.1.7/pabutools/election/profile/profile.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/satisfaction/__init__.py` & `pabutools-1.1.7/pabutools/election/satisfaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/satisfaction/additivesatisfaction.py` & `pabutools-1.1.7/pabutools/election/satisfaction/additivesatisfaction.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/satisfaction/functionalsatisfaction.py` & `pabutools-1.1.7/pabutools/election/satisfaction/functionalsatisfaction.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/satisfaction/positionalsatisfaction.py` & `pabutools-1.1.7/pabutools/election/satisfaction/positionalsatisfaction.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/satisfaction/satisfactionmeasure.py` & `pabutools-1.1.7/pabutools/election/satisfaction/satisfactionmeasure.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/election/satisfaction/satisfactionprofile.py` & `pabutools-1.1.7/pabutools/election/satisfaction/satisfactionprofile.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/fractions.py` & `pabutools-1.1.7/pabutools/fractions.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/rules/__init__.py` & `pabutools-1.1.7/pabutools/rules/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pabutools.rules.exhaustion import (
     completion_by_rule_combination,
     exhaustion_by_budget_increase,
 )
 from pabutools.rules.greedywelfare import greedy_utilitarian_welfare
 from pabutools.rules.maxwelfare import (
     max_additive_utilitarian_welfare,
-    MaxAddUtilWelfareAlgo
+    MaxAddUtilWelfareAlgo,
 )
 from pabutools.rules.mes import (
     method_of_equal_shares,
     MESAllocationDetails,
     MESIteration,
 )
 from pabutools.rules.phragmen import sequential_phragmen
```

### Comparing `pabutools-1.1.6/pabutools/rules/budgetallocation.py` & `pabutools-1.1.7/pabutools/rules/budgetallocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from collections.abc import Iterable
 
 from pabutools.election.instance import Project
 
+
 class AllocationDetails:
     """
     Class representing participatory budgeting rule run details.
     Used as a parent class which can be inherited.
     """
 
     def __init__(self):
```

### Comparing `pabutools-1.1.6/pabutools/rules/composition.py` & `pabutools-1.1.7/pabutools/rules/composition.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/rules/exhaustion.py` & `pabutools-1.1.7/pabutools/rules/exhaustion.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,34 @@
     profile: AbstractProfile,
     rule_sequence: Collection[Callable],
     rule_params: Collection[dict] | None = None,
     initial_budget_allocation: Iterable[Project] | None = None,
     resoluteness: bool = True,
 ) -> BudgetAllocation | list[BudgetAllocation]:
     """
-    Runs the given rules on the given instance and profile in sequence until an exhaustive budget allocation has been
-    reached (or all rules have been applied). This is useful if the first rules are non-exhaustive.
-    In the irresolute version, all outcomes are completed separately.
+    Runs the given rules on the given instance and profile in sequence until an exhaustive budget
+    allocation has been reached (or all rules have been applied). This is useful if the first rules
+    are non-exhaustive. In the irresolute version, all outcomes are completed separately.
 
     Parameters
     ----------
         instance: :py:class:`~pabutools.election.instance.Instance`
             The instance.
         profile : :py:class:`~pabutools.election.profile.profile.AbstractProfile`
             The profile.
         rule_sequence: Iterable[Callable]
             Iterable of the rule functions.
         rule_params: Iterable[dict], optional
-            Iterable of dictionaries of additional parameters that are passed as keyword arguments to the rule
-            functions. Defaults to `{}`.
+            Iterable of dictionaries of additional parameters that are passed as keyword arguments
+            to the rule functions. Defaults to `{}`.
         initial_budget_allocation : Iterable[:py:class:`~pabutools.election.instance.Project`], optional
             An initial budget allocation, typically empty. Defaults to `[]`.
         resoluteness : bool, optional
-            Set to `False` to obtain an irresolute outcome, where all tied budget allocations are returned.
-            Defaults to True.
+            Set to `False` to obtain an irresolute outcome, where all tied budget allocations are
+            returned. Defaults to True.
 
     Returns
     -------
         :py:class:`~pabutools.rules.budgetallocation.BudgetAllocation` | list[:py:class:`~pabutools.rules.budgetallocation.BudgetAllocation`]
             The selected projects.
     """
     if rule_params is not None and len(rule_sequence) != len(rule_params):
@@ -99,49 +99,57 @@
 def exhaustion_by_budget_increase(
     instance: Instance,
     profile: AbstractProfile,
     rule: Callable,
     rule_params: dict | None = None,
     initial_budget_allocation: Iterable[Project] | None = None,
     resoluteness: bool = True,
+    exhaustive_stop: bool = True,
     budget_step: Numeric | None = None,
     budget_bound: Numeric | None = None,
 ) -> BudgetAllocation | list[BudgetAllocation]:
     """
-    Runs the given rule iteratively with increasing budget, until an exhaustive allocation is retrieved or
-    the budget limit is exceeded by the rule with increased budget. In the irresolute version, as soon as one outcome is
-    exhaustive or infeasible, the procedure stops.
+    Runs the given rule iteratively with increasing budget, until an exhaustive allocation is
+    retrieved or the budget limit is exceeded by the rule with increased budget. In the irresolute
+    version, as soon as one outcome is exhaustive or infeasible, the procedure stops.
+
+    If you are interested to only stop when the returned budget allocation is not feasible
+    (and thus not when it is exhaustive), set :code:`exhaustive_stop=False`.
 
     Parameters
     ----------
         instance: :py:class:`~pabutools.election.instance.Instance`
             The instance.
         profile : :py:class:`~pabutools.election.profile.profile.AbstractProfile`
             The profile.
         rule:
             The rule function
         rule_params: dict, optional
             Dictionary of additional parameters that are passed as keyword arguments to the rule
             function. Defaults to `{}`.
         initial_budget_allocation: Collection[Project], optional
-            An initial budget allocation, typically empty. Defaults to `[]`. Overrides the parameter in `rule_params`.
+            An initial budget allocation, typically empty. Defaults to `[]`. Overrides the parameter
+            in `rule_params`.
         resoluteness : bool, optional
-            Set to `False` to obtain an irresolute outcome, where all tied budget allocations are returned.
-            Defaults to True.
+            Set to `False` to obtain an irresolute outcome, where all tied budget allocations
+            are returned. Defaults to True.
+        exhaustive_stop: bool, optional
+            Set to `False` to disable the exhaustive allocation stop condition, leaving only
+            the non-feasibility as the stop condition of this rule. Defaults to True.
         budget_step: Numeric
             The step at which the budget is increased. Defaults to 1% of the budget limit.
         budget_bound: Numeric
-            An upper bound on the budget limit. The method stops if this bound is exceeded. Defaults to the budget limit
-            multiplied by the number of agents plus 1.
+            An upper bound on the budget limit. The method stops if this bound is exceeded. Defaults
+            to the budget limit multiplied by the number of agents plus 1.
 
     Returns
     -------
         BudgetAllocation | Iterable[BudgetAllocation]
-            The selected budget allocation if resolute (:code:`resoluteness == True`), or the set of budget allocations if irresolute
-            (:code:`resoluteness == False`).
+            The selected budget allocation if resolute (:code:`resoluteness == True`), or the set of
+            budget allocations if irresolute (:code:`resoluteness == False`).
     """
     if rule_params is None:
         rule_params = {}
     current_instance = deepcopy(instance)
     if initial_budget_allocation is None:
         initial_budget_allocation = BudgetAllocation()
     else:
@@ -157,19 +165,19 @@
         budget_bound = instance.budget_limit * (profile.num_ballots() + 1)
     rule_params["resoluteness"] = resoluteness
     while current_instance.budget_limit <= budget_bound:
         outcome = rule(current_instance, profile, **rule_params)
         if resoluteness:
             if not instance.is_feasible(outcome):
                 return previous_outcome
-            if instance.is_exhaustive(outcome):
+            if exhaustive_stop and instance.is_exhaustive(outcome):
                 return outcome
             current_instance.budget_limit += budget_step
             previous_outcome = outcome
         else:
             if any(not instance.is_feasible(o) for o in outcome):
                 return previous_outcome
-            if any(instance.is_exhaustive(o) for o in outcome):
+            if exhaustive_stop and any(instance.is_exhaustive(o) for o in outcome):
                 return outcome
             current_instance.budget_limit += budget_step
             previous_outcome = outcome
     return previous_outcome
```

### Comparing `pabutools-1.1.6/pabutools/rules/greedywelfare.py` & `pabutools-1.1.7/pabutools/rules/greedywelfare/greedywelfare_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from __future__ import annotations
 
 from copy import copy
 from collections.abc import Collection, Iterable
 from math import inf
 
 from pabutools.rules.budgetallocation import BudgetAllocation
+from pabutools.rules.greedywelfare.greedywelfare_details import (
+    GreedyWelfareAllocationDetails,
+    GreedyWelfareProjectDetails,
+)
 from pabutools.utils import Numeric
 
 from pabutools.election import AbstractBallot
 from pabutools.election.profile import AbstractProfile
 
 from pabutools.fractions import frac
 from pabutools.election.instance import Instance, total_cost, Project
@@ -24,18 +28,19 @@
 from pabutools.tiebreaking import lexico_tie_breaking, TieBreakingRule
 
 
 def greedy_utilitarian_scheme(
     instance: Instance,
     profile: AbstractProfile,
     sat_profile: GroupSatisfactionMeasure,
-    budget_allocation: Iterable[Project],
+    budget_allocation: BudgetAllocation,
     tie_breaking: TieBreakingRule,
     resoluteness: bool = True,
     sat_bounds: dict[AbstractBallot, Numeric] | None = None,
+    analytics: bool = False,
 ) -> BudgetAllocation | list[BudgetAllocation]:
     """
     The inner algorithm for the greedy rule. It selects projects in rounds, each time selecting a project that
     lead to the highest increase in total score divided by the cost of the project. Projects that would lead to a
     violation of the budget constraint are skipped.
 
     Parameters
@@ -49,14 +54,16 @@
         budget_allocation : Iterable[:py:class:`~pabutools.rules.budgetallocation.BudgetAllocation`]
             An initial budget allocation, typically empty.
         tie_breaking : :py:class:`~pabutools.tiebreaking.TieBreakingRule`
             The tie-breaking rule used.
         resoluteness : bool, optional
             Set to `False` to obtain an irresolute outcome, where all tied budget allocations are returned.
             Defaults to True.
+        analytics: bool, optional
+            (De)Activate the calculation of analytics. Defaults to False.
     Returns
     -------
         :py:class:`~pabutools.rules.budgetallocation.BudgetAllocation` | list[:py:class:`~pabutools.rules.budgetallocation.BudgetAllocation`]
             The selected projects if resolute (:code:`resoluteness == True`), or the set of selected projects if irresolute
             (:code:`resoluteness == False`).
     """
 
@@ -134,17 +141,18 @@
         return all_budget_allocations
 
 
 def greedy_utilitarian_scheme_additive(
     instance: Instance,
     profile: AbstractProfile,
     sat_profile: GroupSatisfactionMeasure,
-    budget_allocation: Collection[Project],
+    budget_allocation: BudgetAllocation,
     tie_breaking: TieBreakingRule,
     resoluteness: bool = True,
+    analytics: bool = False,
 ) -> BudgetAllocation | list[BudgetAllocation]:
     """
     Faster version of the inner algorithm for the greedy rule if the scores are additive.
 
     Parameters
     ----------
         instance: :py:class:`~pabutools.election.instance.Instance`
@@ -156,28 +164,31 @@
         budget_allocation : Iterable[:py:class:`~pabutools.election.instance.Project`]
             An initial budget allocation, typically empty.
         tie_breaking : :py:class:`~pabutools.tiebreaking.TieBreakingRule`
             The tie-breaking rule used.
         resoluteness : bool, optional
             Set to `False` to obtain an irresolute outcome, where all tied budget allocations are returned.
             Defaults to True.
+        analytics: bool, optional
+            (De)Activate the calculation of analytics. Defaults to False.
     Returns
     -------
         :py:class:`~pabutools.rules.budgetallocation.BudgetAllocation` | list[:py:class:`~pabutools.rules.budgetallocation.BudgetAllocation`]
             The selected projects if resolute (:code:`resoluteness == True`), or the set of selected projects if irresolute
             (:code:`resoluteness == False`).
     """
     if not resoluteness:
         return greedy_utilitarian_scheme(
             instance,
             profile,
             sat_profile,
             budget_allocation,
             tie_breaking,
             resoluteness,
+            analytics,
         )
 
     projects = sorted(instance)
     for project in budget_allocation:
         projects.remove(project)
     projects = tie_breaking.order(instance, profile, projects)
 
@@ -185,37 +196,51 @@
         total_sat = sat_profile.total_satisfaction_project(proj)
         if total_sat > 0:
             if proj.cost > 0:
                 return frac(total_sat, proj.cost)
             return inf
         return 0
 
+    selection = BudgetAllocation(
+        budget_allocation, details=GreedyWelfareAllocationDetails()
+    )
+    if analytics:
+        selection.details.projects.extend(
+            [
+                GreedyWelfareProjectDetails(
+                    project, score=satisfaction_density(project)
+                )
+                for project in projects
+            ]
+        )
     # We sort based on a tuple to ensure ties are broken as intended
     ordered_projects = sorted(
         projects, key=lambda p: (-satisfaction_density(p), projects.index(p))
     )
 
-    selection = BudgetAllocation(budget_allocation)
     remaining_budget = instance.budget_limit - total_cost(budget_allocation)
     for project in ordered_projects:
         if project.cost <= remaining_budget:
             selection.append(project)
             remaining_budget -= project.cost
+            if analytics:
+                selection.details.mark_as_selected(project, remaining_budget)
     return selection
 
 
 def greedy_utilitarian_welfare(
     instance: Instance,
     profile: AbstractProfile,
     sat_class: type[SatisfactionMeasure] | None = None,
     sat_profile: GroupSatisfactionMeasure | None = None,
     is_sat_additive: bool | None = None,
     tie_breaking: TieBreakingRule | None = None,
     resoluteness: bool = True,
     initial_budget_allocation: Collection[Project] | None = None,
+    analytics: bool = False,
 ) -> BudgetAllocation | list[BudgetAllocation]:
     """
     General greedy scheme for approximating the utilitarian welfare. It selects projects in rounds, each time selecting
     a project that lead to the highest increase in total satisfaction divided by the cost of the project. Projects that
     would lead to a violation of the budget constraint are skipped.
 
     Parameters
@@ -239,27 +264,30 @@
             An initial budget allocation, typically empty.
         tie_breaking : :py:class:`~pabutools.tiebreaking.TieBreakingRule`, optional
             The tie-breaking rule used.
             Defaults to the lexicographic tie-breaking.
         resoluteness : bool, optional
             Set to `False` to obtain an irresolute outcome, where all tied budget allocations are returned.
             Defaults to True.
+        analytics: bool, optional
+            (De)Activate the calculation of analytics. Defaults to False.
 
     Returns
     -------
         BudgetAllocation | Collection[BudgetAllocation]
             The selected budget allocation if resolute (:code:`resoluteness == True`), or the set of budget allocations if irresolute
             (:code:`resoluteness == False`).
     """
     if tie_breaking is None:
         tie_breaking = lexico_tie_breaking
     if initial_budget_allocation is not None:
         budget_allocation = BudgetAllocation(initial_budget_allocation)
     else:
         budget_allocation = BudgetAllocation()
+
     if sat_class is None:
         if sat_profile is None:
             raise ValueError("sat_class and sat_profile cannot both be None.")
     else:
         if sat_profile is None:
             sat_profile = profile.as_sat_profile(sat_class)
         if is_sat_additive is None:
@@ -269,16 +297,18 @@
         return greedy_utilitarian_scheme_additive(
             instance,
             profile,
             sat_profile,
             budget_allocation,
             tie_breaking,
             resoluteness=resoluteness,
+            analytics=analytics,
         )
     return greedy_utilitarian_scheme(
         instance,
         profile,
         sat_profile,
         budget_allocation,
         tie_breaking,
         resoluteness=resoluteness,
+        analytics=analytics,
     )
```

### Comparing `pabutools-1.1.6/pabutools/rules/maxwelfare.py` & `pabutools-1.1.7/pabutools/rules/maxwelfare.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,26 +25,32 @@
 
 class MaxAddUtilWelfareAlgo(DocEnum):
     """
     Constants use to represent different algorithms that can be used to compute budget allocations
     maximising the additive utilitarian welfare.
     """
 
-    ILP_SOLVER = 1, "Converts the instance into a integer linear program (ILP) and uses an ILP " \
-                    "solver to compute the outcome."
-
-    PRIMAL_DUAL = 2, "Uses state-of-the-art primal/dual solvers for knapsack problems to compute " \
-                     "the outcome."
+    ILP_SOLVER = (
+        1,
+        "Converts the instance into a integer linear program (ILP) and uses an ILP "
+        "solver to compute the outcome.",
+    )
+
+    PRIMAL_DUAL = (
+        2,
+        "Uses state-of-the-art primal/dual solvers for knapsack problems to compute "
+        "the outcome.",
+    )
 
 
 def max_additive_utilitarian_welfare_ilp_scheme(
-        instance: Instance,
-        sat_profile: GroupSatisfactionMeasure,
-        initial_budget_allocation: Collection[Project],
-        resoluteness: bool = True,
+    instance: Instance,
+    sat_profile: GroupSatisfactionMeasure,
+    initial_budget_allocation: Collection[Project],
+    resoluteness: bool = True,
 ) -> BudgetAllocation | list[BudgetAllocation]:
     """
     The inner algorithm for the welfare maximizing rule. It generates the corresponding budget allocations using a
     linear program solver. Note that there is no control over the way ties are broken.
 
     Parameters
     ----------
@@ -89,22 +95,22 @@
     previous_partial_alloc = [p for p in p_vars if p_vars[p].x >= 0.99]
     all_partial_allocs = [previous_partial_alloc]
 
     mip_model += xsum(p_vars[p] * score[p] for p in p_vars) == opt_value
     while True:
         # See http://yetanothermathprogrammingconsultant.blogspot.com/2011/10/integer-cuts.html
         mip_model += (
-                xsum(1 - p_vars[p] for p in previous_partial_alloc)
-                + xsum(p_vars[p] for p in p_vars if p not in previous_partial_alloc)
-                >= 1
+            xsum(1 - p_vars[p] for p in previous_partial_alloc)
+            + xsum(p_vars[p] for p in p_vars if p not in previous_partial_alloc)
+            >= 1
         )
         mip_model += (
-                xsum(p_vars[p] for p in previous_partial_alloc)
-                - xsum(p_vars[p] for p in p_vars if p not in previous_partial_alloc)
-                <= len(previous_partial_alloc) - 1
+            xsum(p_vars[p] for p in previous_partial_alloc)
+            - xsum(p_vars[p] for p in p_vars if p not in previous_partial_alloc)
+            <= len(previous_partial_alloc) - 1
         )
 
         opt_status = mip_model.optimize()
         if opt_status != mip.OptimizationStatus.OPTIMAL:
             break
 
         previous_partial_alloc = [p for p in p_vars if p_vars[p].x >= 0.99]
@@ -113,17 +119,17 @@
     return [
         BudgetAllocation(partial_alloc + list(initial_budget_allocation))
         for partial_alloc in all_partial_allocs
     ]
 
 
 def max_additive_utilitarian_welfare_primal_dual_scheme(
-        instance: Instance,
-        sat_profile: GroupSatisfactionMeasure,
-        initial_budget_allocation: Collection[Project],
+    instance: Instance,
+    sat_profile: GroupSatisfactionMeasure,
+    initial_budget_allocation: Collection[Project],
 ) -> BudgetAllocation:
     budget_allocation = BudgetAllocation(initial_budget_allocation)
 
     items = []
     for p in instance:
         if p not in budget_allocation:
             profit = sat_profile.total_satisfaction_project(p)
@@ -175,31 +181,42 @@
         split_weight += item.weight
         split_profit += item.profit
 
     solution = [0 for _ in range(len(items))]
     lower_bound = [0]
     a_star = [-1]
     b_star = [-1]
-    primal_dual_branch_impl(split_idx - 1, split_idx, split_profit, split_weight, items, capacity,
-                            solution, lower_bound, a_star, b_star)
+    primal_dual_branch_impl(
+        split_idx - 1,
+        split_idx,
+        split_profit,
+        split_weight,
+        items,
+        capacity,
+        solution,
+        lower_bound,
+        a_star,
+        b_star,
+    )
 
     result = []
     for i in range(len(items)):
         if i < len(items) and i < b_star[0]:
             if i < a_star[0] + 1:
                 solution[i] = 1
 
             if solution[i] == 1:
                 result.append(items[i])
 
     return result
 
 
-def primal_dual_branch_impl(a, b, profit_sum, weight_sum, items, capacity, x, lower_bound, a_star,
-                            b_star):
+def primal_dual_branch_impl(
+    a, b, profit_sum, weight_sum, items, capacity, x, lower_bound, a_star, b_star
+):
     improved = False
 
     if weight_sum <= capacity:
         if profit_sum > lower_bound[0]:
             lower_bound[0] = profit_sum
             a_star[0] = a
             b_star[0] = b
@@ -210,54 +227,94 @@
 
         upper_bound = math.floor((capacity - weight_sum) * items[b].efficiency)
         if profit_sum + upper_bound <= lower_bound[0]:
             return improved
 
         pb = items[b].profit
         wb = items[b].weight
-        if primal_dual_branch_impl(a, b + 1, profit_sum + pb, weight_sum + wb, items, capacity, x,
-                                   lower_bound, a_star, b_star):
+        if primal_dual_branch_impl(
+            a,
+            b + 1,
+            profit_sum + pb,
+            weight_sum + wb,
+            items,
+            capacity,
+            x,
+            lower_bound,
+            a_star,
+            b_star,
+        ):
             x[b] = 1
             improved = True
 
-        if primal_dual_branch_impl(a, b + 1, profit_sum, weight_sum, items, capacity, x,
-                                   lower_bound, a_star, b_star):
+        if primal_dual_branch_impl(
+            a,
+            b + 1,
+            profit_sum,
+            weight_sum,
+            items,
+            capacity,
+            x,
+            lower_bound,
+            a_star,
+            b_star,
+        ):
             x[b] = 0
             improved = True
     else:
         if a < 0:
             return False
 
         upper_bound = math.floor((capacity - weight_sum) * items[a].efficiency)
         if profit_sum + upper_bound <= lower_bound[0]:
             return False
 
         pa = items[a].profit
         wa = items[a].weight
-        if primal_dual_branch_impl(a - 1, b, profit_sum - pa, weight_sum - wa, items, capacity, x,
-                                   lower_bound, a_star, b_star):
+        if primal_dual_branch_impl(
+            a - 1,
+            b,
+            profit_sum - pa,
+            weight_sum - wa,
+            items,
+            capacity,
+            x,
+            lower_bound,
+            a_star,
+            b_star,
+        ):
             x[a] = 0
             improved = True
 
-        if primal_dual_branch_impl(a - 1, b, profit_sum, weight_sum, items, capacity, x,
-                                   lower_bound, a_star, b_star):
+        if primal_dual_branch_impl(
+            a - 1,
+            b,
+            profit_sum,
+            weight_sum,
+            items,
+            capacity,
+            x,
+            lower_bound,
+            a_star,
+            b_star,
+        ):
             x[a] = 1
             improved = True
 
     return improved
 
 
 def max_additive_utilitarian_welfare(
-        instance: Instance,
-        profile: AbstractProfile,
-        sat_class: type[SatisfactionMeasure] | None = None,
-        sat_profile: GroupSatisfactionMeasure | None = None,
-        resoluteness: bool = True,
-        initial_budget_allocation: Collection[Project] | None = None,
-        inner_algo: MaxAddUtilWelfareAlgo | None = None,
+    instance: Instance,
+    profile: AbstractProfile,
+    sat_class: type[SatisfactionMeasure] | None = None,
+    sat_profile: GroupSatisfactionMeasure | None = None,
+    resoluteness: bool = True,
+    initial_budget_allocation: Collection[Project] | None = None,
+    inner_algo: MaxAddUtilWelfareAlgo | None = None,
 ) -> BudgetAllocation | list[BudgetAllocation]:
     """
     Rule returning the budget allocation(s) maximizing the utilitarian social welfare. The
     utilitarian social welfare is defined as the sum of the satisfactin of the voters, where the
     satisfaction is computed using the satisfaction measure given as a parameter. The satisfaction
     measure is assumed to be additive.
 
@@ -307,24 +364,28 @@
         if sat_profile is None:
             raise ValueError("Satisfaction and sat_profile cannot both be None.")
     else:
         if sat_profile is None:
             sat_profile = profile.as_sat_profile(sat_class=sat_class)
     if inner_algo:
         if inner_algo == MaxAddUtilWelfareAlgo.PRIMAL_DUAL and not resoluteness:
-            raise ValueError("The primal/dual algorithm does not support irresolute outcomes.")
+            raise ValueError(
+                "The primal/dual algorithm does not support irresolute outcomes."
+            )
     else:
         if resoluteness:
             inner_algo = MaxAddUtilWelfareAlgo.PRIMAL_DUAL
         else:
             inner_algo = MaxAddUtilWelfareAlgo.ILP_SOLVER
     if inner_algo == MaxAddUtilWelfareAlgo.PRIMAL_DUAL:
         return max_additive_utilitarian_welfare_primal_dual_scheme(
             instance, sat_profile, budget_allocation
         )
     elif inner_algo == MaxAddUtilWelfareAlgo.ILP_SOLVER:
         return max_additive_utilitarian_welfare_ilp_scheme(
             instance, sat_profile, budget_allocation, resoluteness
         )
     else:
-        raise ValueError("The parameter 'inner_algo' needs to be a member of the "
-                         "MaxAddUtilWelfareAlgo enumeration.")
+        raise ValueError(
+            "The parameter 'inner_algo' needs to be a member of the "
+            "MaxAddUtilWelfareAlgo enumeration."
+        )
```

### Comparing `pabutools-1.1.6/pabutools/rules/mes/mes_details.py` & `pabutools-1.1.7/pabutools/rules/mes/mes_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,17 +146,17 @@
     def __init__(
         self,
         voters_budget: list[Numeric] | None = None,
         voters_budget_after_selection: list[Numeric] | None = None,
         selected_project: Project | None = None,
     ):
         self.voters_budget: list[Numeric] | None = voters_budget
-        self.voters_budget_after_selection: list[Numeric] | None = (
-            voters_budget_after_selection
-        )
+        self.voters_budget_after_selection: list[
+            Numeric
+        ] | None = voters_budget_after_selection
         self.selected_project: Project | None = selected_project
         super().__init__()
 
     def update_project_details_as_discarded(self, project: Project):
         """Updates the project details of the given project as discarded during this iteration."""
         project_details = self[self.index(project)]
         project_details.discarded = True
```

### Comparing `pabutools-1.1.6/pabutools/rules/mes/mes_rule.py` & `pabutools-1.1.7/pabutools/rules/mes/mes_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -647,17 +647,17 @@
     voter_budget_increment=None,
     binary_sat=None,
     skipped_project: Project | None = None,
     analytics: bool = False,
     verbose: bool = False,
 ) -> BudgetAllocation | list[BudgetAllocation]:
     """
-    The Method of Equal Shares (MES). See the website
-    `equalshares.net <https://equalshares.net/>`_ for details about how to compute the outcome of the rule. Note that
-    the satisfaction measure is asssumed to be additive.
+    The Method of Equal Shares (MES). See the website `equalshares.net <https://equalshares.net/>`_
+    for details about how to compute the outcome of the rule. Note that the satisfaction measure is
+    assumed to be additive.
 
     Parameters
     ----------
         instance: :py:class:`~pabutools.election.instance.Instance`
             The instance.
         profile : :py:class:`~pabutools.election.profile.profile.AbstractProfile`
             The profile.
```

### Comparing `pabutools-1.1.6/pabutools/rules/phragmen.py` & `pabutools-1.1.7/pabutools/rules/phragmen.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/tiebreaking.py` & `pabutools-1.1.7/pabutools/tiebreaking.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/utils.py` & `pabutools-1.1.7/pabutools/utils.py`

 * *Files identical despite different names*

### Comparing `pabutools-1.1.6/pabutools/visualisation/templates/mes_page_summary_template.html` & `pabutools-1.1.7/pabutools/visualisation/templates/greedy_round_analysis_template.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,221 +1,81 @@
-<!--Priority TODOs: 
-    Generate text inside rows
-    Adjust explanations in charts/website in general
-    Handle generated explanations when no funding has been lost. (i.e. rejected projects have incorrect statement when highlight blue bar)
-
-    Other TODOs:
-    Implement Comparisons
-    Implement Example
-    Add commas to separate large numbers
-    Make currency dynamic
-    Round float numbers to 2 decimal place using this '%0.2f' % number | float
-    Shorten project names in red bar tool-tip
-    Add animation
-    Remove projects that have 0 funding loss from list of funding lost projects within expandable row/chart
--->
-
 <!DOCTYPE html>
-<html translate="no">
+<html lang="en">
 
 <head>
-    <!-- <title>!FILE!</title> -->
-    <meta charset="utf-8">
-    <meta name="viewport" content="width=device-width, initial-scale=1">
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title> {{ election_name}}</title>
+    <!-- Bootstrap CSS -->
     <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
-    <script src='sorttable.js'></script>
-    <script type="text/javascript"> 
-        function showHiddenRow(projectId) { 
-            var hiddenRow = document.querySelector("#hidden-" + projectId);
-            hiddenRow.classList.toggle("hidden-row");
-
-            hiddenRow.parentElement.classList.toggle("clickable-row");
-
-            var span = document.getElementById("expand-symbol-".concat(projectId));
-            if (encodeURI(Array.from(span.innerHTML)[0]) === "%E2%80%BA") {
-                span.innerHTML = decodeURI("&#8964");   
-            } else {
-                span.innerHTML = decodeURI("&#8250;")
-            }
-
-        }
-    </script>
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css">
+    <script nonce="undefined" src="https://cdn.zingchart.com/zingchart.min.js"></script>
+    <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
     <style>
-        * {
+        /* Custom CSS to color the borders black */
+        .budget-container {
+            position: relative;
+            width: 100%;
+            padding: 10px;
             box-sizing: border-box;
-            font-family: Roboto, system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
-            --ifm-table-cell-padding: 0.75rem;
-            --ifm-table-background: #0000;
-            --ifm-table-stripe-background: #00000008;
-            --ifm-table-border-width: 1px;
-            --ifm-table-border-color: #0000001f;
-            --ifm-table-head-background: inherit;
-            --ifm-table-head-color: inherit;
-            --ifm-table-head-font-weight: 500;
-            --ifm-table-cell-color: inherit;
-        }
-
-        body {
-            font-family: "Helvetica-Neue", "Helvetica", Arial, sans-serif;
-            font-size: 16px;
-            line-height: 1.3;
-            margin: 0 auto;
-            text-align: left;
-        }
-
-        table {
-            border-collapse: collapse;
-            display: block;
-            margin-bottom: 1rem;
-            margin: 0 auto;
-            width: 50%;
-            padding-bottom: 1.5rem;
         }
-
-        table thead tr {
-            border-bottom: 2px solid var(--ifm-table-border-color)
-        }
-
-        table thead,
-        table tr:nth-child(2n) {
-            background-color: var(--ifm-table-stripe-background)
-        }
-
-        table tr {
-            background-color: var(--ifm-table-background);
-            border-top: var(--ifm-table-border-width) solid var(--ifm-table-border-color)
-        }
-
-        table td,
-        table th {
-            border: var(--ifm-table-border-width) solid var(--ifm-table-border-color);
-            padding: var(--ifm-table-cell-padding)
-        }
-
-        table th {
-            background-color: var(--ifm-table-head-background);
-            color: var(--ifm-table-head-color);
-            font-weight: var(--ifm-table-head-font-weight)
+        .budget{
+            color: black
         }
-
-        table td {
-            color: var(--ifm-table-cell-color)
-        }
-
-        table tr.winner td {
-            background-color: rgb(113, 166, 91);
-            color: #fff;
-        }
-
-        table tr.loser-first-phase td {
-            background-color: rgb(240, 200, 200);
-        }
-
-        table tr.highlighted td {
-            background-color: hsl(102, 30%, 70%);
-            color: #000;
-        }
-
-        .budget-chart-container {
-            display: flex;
-            justify-content: center;
-            align-items: center;
-            flex-direction: column;
+        .bar {
+            position: relative;
+            height: 30px;
             margin: 10px 0;
-        }
-
-        .chart-container {
-            display: flex;
-            flex-direction: column;
-            margin: -10px 0;
-        }
-
-
-        .cost-locator-container {
-            width: 300px;
-            height: 11px;
+            background-color: #ddd;
             position: relative;
+            align-items: center;
+            justify-content: center;
+            color: black;
         }
-
-        .split-cell {
+        .bar-inner {
+            position: relative;
+            height: 100%;
             display: flex;
-            justify-content: space-between;
+            align-items: center;
+            justify-content: center;
+            color: black;
+            position: absolute;
+            left: 0;
+            top: 0;
         }
-
-        .cost-locator {
+        .dashed-line {
             position: absolute;
             top: 0;
-            /* width: 15px; */
-            padding: 0 5px;
-            text-align: right;
-            cursor: default;
-            font-size: 10px;
-            font-weight: 300;
-            color: black;
-            white-space: nowrap;
+            height: 600%;
+            border-left: 2px dashed black;
         }
-
-        .chart {
-            background: #fff;
-            border: 0.5px solid #777;
-            width: 300px;
-            height: 15px;
-            display: flex;
-            align-items: center;
+        .green {
+            background-color: #4CAF50;
+            color: white;
+            justify-content: center;
         }
-
-        .chart-budget {
-            background: #fff;
-            border: 1.5px solid #000000;
-            width: 900px;
-            height: 45px;
+        .red {
+            background-color: #F44336;
+            color: white;
+            justify-content: center;
+        }
+        .rejected-mark {
+            position: absolute;
+            right: -50px;
+            top: 0;
+            width: 30px;
+            height: 30px;
             display: flex;
             align-items: center;
+            justify-content: center;
+            font-size: 20px;
+            color: black;
+            background-color: white;
+            border-radius: 15px; /* Circular */
         }
-
-        .bar {
-            height: 100%;
-            background: #00A000;
-        }
-
-        .bar-border {
-            border: 0.75px solid #000000;
-        }
-
-        .final-bar{
-            background: #aaa;
-        }
-        table tr.winner td .final-bar {
-            background: #cee9cc;
-        }
-
-        .bar-blue {
-            background: #83a8e6;
-        }
-        .bar-light {
-            background: #f6c8c8;
-        }
-        .bar-dark {
-            background: #dea0a0;
-        }
-
-        .center {
-            text-align: center;
-            width: 900px;
-        }
-
-        .hidden-row { 
-            display: none;
-        }
-
-        .clickable-row {
-            cursor: pointer;
-        }
-
-        /* CSS From Round Analysis page */
         .border-black {
             border: 1px solid black;
         }
         
         .nested {
             padding: 1rem;
         }
@@ -224,504 +84,629 @@
             padding: 0rem;
         }
         
         .spacer {
             padding: 1rem;
         }
         
+        .carousel-control-prev-icon,
+        .carousel-control-next-icon {
+            font-size: 24px;
+            color: black;
+        }
+        
+        .carousel-inner {
+            padding: 1rem;
+            padding-left: 7rem;
+            padding-right: 7rem;
+        }
+        
+        .carousel-inner-pie {
+            padding-top: 0.5rem;
+            height: 400px;
+        }
+        
         .hidden-section {
             display: none;
         }
         
         .chord-wrapper {
             height: 100%;
         }
         
-        /* zing-grid[loading] {
-            height: 800px;
+        #myChordChart {
+            height: 100%;
             width: 100%;
-        } */
+        }
         
-        h1,h2,
-        p {
-            text-align: center;
+        #myBarChart1,
+        #myStackedBarChart1 {
+            height: 100%;
+            width: 100%;
         }
-
-        .info-button {
-            padding: 12px 15px;
-            background-color: #007bff;
-            border: none;
-            border-radius: 50%;
-            color: white;
-            font-size: 30px;
-            cursor: pointer;
+        h1,
+        h3,
+        p {
             text-align: center;
-            line-height: 1; /* Align the icon vertically */
-            display: inline-block;
         }
-
-        /* Optional: add a hover effect */
-        .info-button:hover {
-            background-color: #0056b3;
-        }
-        .spacer-8{
-            padding: 8rem;
-        }
-        .spacer-4{
-            padding: 4rem;
-        }
-        .spacer-2{
+        .spacer-2 {
             padding: 2rem;
         }
-        .spacer-1{
-            padding: 1rem;
-        }
+  .bar-container {
+        position: relative;
+        width: 100%;
+    }
+    .budget {
+        color: black;
+    }
 
-        .upper-page{
-            background-color: gray;
-            color: white;
-        }
-
-        .carousel-control-prev{
-            background-color: gray;
-            width: 20px;
-        }
-
-        .carousel-control-next{
-            background-color: gray;
-            width: 20px;
-        }
 
-        .carousel-inner{
-            margin: 20px;
-        }
-</style>
+    </style>
 </head>
-
-<body>
-    <!-- <h1>!FILE!</h1> -->
-    <!-- !DESCRIPTION! -->
-
-    <!-- !SAMPLE_EXPLANATION1! -->
-
-    <!-- <table>
-        <tbody>
-            !SAMPLE_EXPLANATION_ROW!
-        </tbody>
-    </table> -->
-
-    <!-- !SAMPLE_EXPLANATION2! -->
+<body > 
     <header>
         <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-dark">
-          <a class="navbar-brand active" href="./summary.html">Summary<span class="sr-only">(current)</span></a>
+          <a class="navbar-brand" href="./summary.html">Summary</a>
           <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
             <span class="navbar-toggler-icon"></span>
           </button>
           <div class="collapse navbar-collapse" id="navbarCollapse">
             <ul class="navbar-nav mr-auto">
-              <li class="nav-item">
-                <a class="nav-link" href="./round_analysis.html">Round By Round</a>
-              </li>
-              <li class="nav-item">
-                <a class="nav-link" href="">Pabutools</a>
+              <li class="nav-item active">
+                <a class="nav-link" href="./round_analysis.html">Round By Round <span class="sr-only">(current)</span></a>
               </li>
               <li class="nav-item">
-                <a class="nav-link" href="">MES</a>
+                <a class="nav-link" href="https://pypi.org/project/pabutools/">Pabutools</a>
               </li>
             </ul>
-            <form class="form-inline mt-2 mt-md-0" data-dashlane-rid="586d21bb200ad9fc" data-form-type="">
-              <input class="form-control mr-sm-2" type="text" placeholder="Search" aria-label="Search" data-dashlane-rid="ebb02837c4029767" data-form-type="">
-              <button class="btn btn-outline-success my-2 my-sm-0" type="submit" data-dashlane-label="true" data-dashlane-rid="c66944f310795772" data-form-type="">Search</button>
-            </form>
           </div>
         </nav>
-    </header>
-
-    <main role="main">
+      </header>
 
+      <main role="main">
+    
         <div class="container-fluid upper-page">
             <!-- General Explanations -->
             <div class="container">
                 <div class="spacer-2"></div>
                 <div class="spacer-2"></div>
 
+
                 <div class="row mb-3">
                     <div class="col-12  justify-content-center">
                         <h1>
                             {{ election_name }}
                         </h1>
                         <div class="spacer-1"><hr></div>
+                        <p>
+                            This is the explanation for the outcome of the participatory budgeting election decided using the Greedy Utilitarian Welfare algorithm.<br>
+                            Some of the key features of the election are: The election has a total budget of {{ "{:,}".format((budget | int)) }} {{ currency }} of which {{ "{:,}".format((spent | int)) }} {{ currency }} was spent. The election had a 
+                            total of {{total_votes}} voters. Note that each participant can vote for multiple projects. Therefore, the total votes for all projects may be 
+                            higher than {{total_votes}}<br>
+                            This page shows and explains the outcome of the election. The first graph shows the number of votes for each project.
+                            The bars show the budget at each stage of the election and the projects selected or rejected in each round. Finally, the final bar chart shows an overview of the selected and rejected projects.
+                        </p>
+                        <p>
+                            To view the list of the projects selected, click this: <button type="button" id="electionOutcome" class="btn btn-secondary">View Election Outcome</button>
+                            <div style="display: none;" id="outcomeList" class="row">
+                                {% for round in rounds %}
+                                    <p>Project: "{{ projects[round.selected_project.id]["name"] }}" with cost: {{ "{:,}".format( (round.selected_project.cost | int) ) }} {{ currency }} and had {{round.selected_project.votes}} votes.</p>
+                                {% endfor %}
+                            </div>
+                        </p>
                     </div>
                 </div>
                 <div class="spacer-1"></div>
             </div>
         </div>
         <div class="container">
+
+            
+            
             <div class="spacer-1"></div>
             <hr>
             <div class="spacer-1"></div>
+            
 
-    </main>
-    <!-- Heading before table is displayed-->
-    <h2>Results</h2>
-    <p>The budget of {{ budget }} GBP was allocated across {{ rounds|length }} projects:</p><br>
-    <div class='budget-chart-container'>
-        <div class="center"><span><b>Budget allocation across selected projects.</b></span></div>
-        <div class='chart-budget'>
-            {% for round in rounds %}
-                <div class='bar bar-blue bar-border'
-                    style='width: {{ (round.cost / budget | float) * 100 }}&#37;;'
-                    data-tippy-content='Project {{ round.id }}: <q>{{ projects[round.id]["name"] }}</q> was voted in round {{ loop.index }}, costing {{ round.cost }} GBP. This is {{ ((round.cost / budget | int) * 100) | int }}&#37; of the budget.'>
-                </div>
-            {% endfor %}
-        </div>
-    </div>
+            <!-- Round specific visualisations -->
+                <section id="1">
 
-    <!-- Fix issue where extra comma appears on final item in list. -->
-    <p>
-        {{ election_name}} had a total of {{ total_votes }} voters participating.<br>
-        Between these voters there was a total of {{ budget }} GBP available, of which {{ spent }} GBP was spent.<br>
-
-        <!-- {% for project in projects %}
-            {{ project.name}}: {{project.totalvotes}} votes,
-        {% endfor %}
-        <br> -->
-
-        In total, there were {{ number_of_elected_projects }} projects elected, and {{ number_of_unelected_projects }} projects not elected.<br>
-        {# The elected projects were:<br>
-        {% for p in projects %}
-            {{ projects[p]["name"] }},
-        {% endfor %} #}
-        <br>
-    </p>
-
-    {# <p>
-        The projects and their descriptions are as follows:<br>
-        {% for p in projects %}
-            {{ projects[p]["name"] }}: {{ projects[p]["description"] }}<br>
-        {% endfor %}
-    </p> #}
-
-    <p>
-        {% set voter_budget = (budget | int) / (total_votes | int) %}
-        Each of the voters had a budget of {{ '%0.2f' % voter_budget | float }} GBP to allocate to the projects.<br>
-        The projects were elected using the Method of Equal Shares, where the total budget is virtually divided equally among the voters. <br>
-        The following web-page outlines the process of the election and the step by step process of how each project was chosen.
-    </p>
-
-    <table class='center'>
-        <thead>
-        <tr>
-        <th>Round</th>
-        <th>ID</th>
-        <th>Project Name</th>
-        <th>Cost</th>
-        <th>Number of Votes</th>
-        <th>Effective Support</th>
-        <th>Chart</th>
-        </tr>
-        </thead>
-        <tbody>
-            {% for round in rounds %}
-                <tr class='clickable-row winner' id='project-{{ round.id }}' onclick="showHiddenRow('{{ round.id }}');">
-                <td class='num' sorttable_customkey='{{ loop.index }}'><div class="split-cell"><span id="expand-symbol-{{ round.id }}">&#8250;</span><span>{{ loop.index }}</span></div></td>
-                <td class='num' style='text-align:right' sorttable_customkey='{{ round.id }}'>{{ round.id }}</td>
-                <td>{{ projects[round.id]["name"] }}</td>
-                <td class='num' style='text-align:right' sorttable_customkey='{{ round.cost }}'>{{ round.cost }}</td>
-                <td class='num' style='text-align:right' sorttable_customkey='{{ round.totalvotes }}'>{{ round.totalvotes }}</td>
-                <td style='text-align:right' sorttable_customkey='{{ round.effective_vote_count[round.id]}}'>{{ round.effective_vote_count[round.id] | int }}</td>
-                <td>
-                    <div class='chart-container'>
-                        <div class='cost-locator-container'>
-                            <div class='cost-locator' 
-                                style='left: calc({{ (round.cost / budget | float) * 100 }}&#37; - 9px);'
-                                data-tippy-content='Project Cost: {{ round.cost }} GBP.'>
-                                    <b>
-                                        &darr; {{ round.cost }}
-                                    </b>
+                    
+                    <div class="row featurette">
+                        <div class="col-1"></div>
+                        <div class="col-10" style="min-height: 600px;">
+                            <div id="SortableBarChart" style="height: 100%; width: 100%;">
+                                <button class = "info-button" style = "position: absolute; z-index: 2000; right: 50px;" data-tippy-content= "<b>Project Vote Counts:</b><br> The following graphs shows the votes for each of the projects along with the corresponding budget.">i</button>
                             </div>
                         </div>
-
-                        <div class='chart'>
-                            <div class='bar bar-blue'
-                                style='width: {{ (round.final_voter_funding / budget | float) * 100 }}&#37;;'
-                                data-tippy-content='&#10004; Supporters of the project have {{ round.final_voter_funding | int }} GBP, which is enough to cover the cost {{ round.cost }} GBP.'>
-                            </div>
-                            <div class='bar bar-light'
-                                
-                                onmouseover='highlight_project([
-                                    {% for r in round.funding_lost_per_round %}
-                                        {% if loop.index0 < 3 %}
-                                            "project-{{ rounds[r].id }}",
-                                        {% endif %}
-                                    {% endfor %}
-                                ])'
-                                onmouseout='unhighlight_project([
-                                    {% for r in round.funding_lost_per_round %}
-                                        {% if loop.index0 < 3 %}
-                                            "project-{{ rounds[r].id }}",
-                                        {% endif %}
-                                    {% endfor %}
-                                ])'
-                                style='width: {{ ((round.initial_voter_funding - round.final_voter_funding) / budget | float) * 100 }}&#37;;'
-                                data-tippy-content='<html lang=\"en\"><body">From the initial total funding, <b> {{ (round.initial_voter_funding - round.final_voter_funding) | int }} GBP </b> was spent on previously selected projects. </br> 
-                                Most of the funding was spent on:<br><br>
-                                <ul>
-                                    {% for r in round.funding_lost_per_round %}
-                                        {% if loop.index0 < 3 %}
-                                            <li>
-                                                <b>Project {{ rounds[r].id }} - {{ projects[rounds[r].id]["name"] }}:</b> {{ round.funding_lost_per_round[r] | int }} GBP
-                                                <hr style="width: {{ (round.funding_lost_per_round[r] / (round.initial_voter_funding - round.final_voter_funding)) * 100 }}&#37;;
-                                                    height: 10px;
-                                                    color: #f6c8c8;
-                                                    background-color: #f6c8c8;
-                                                    text-align: left;
-                                                    margin-left: 0;
-                                                    margin-right: 5px;
-                                                    margin-bottom: 7px;
-                                                    margin-top: 3px">
-                                                </hr>
-                                            </li>
-                                        {% endif %}
-                                    {% endfor %}
-                                </ul>
-                                '
-                                allowHTML: true>
-{#                          <li>Project {candidate.name} ({display_short_string(candidate.id)}): {display_int(int(paid))} zł. 
-                                <hr style=\"width:{100 * paid/ total_paid}%;
-                                            height:10px;
-                                            color:#f6c8c8;
-                                            background-color:#f6c8c8;
-                                            text-align:left;
-                                            margin-left:0\">
-                                </hr>
-                            </li>" #}
+                        <div class="col-1"></div>
+                    </div>
+                    <!-- Vote Count -->
+                    <div class="row">
+                        <div class="col-1"></div>
+                        <div class="col-10">
+                            <div class="row justify-content-center">
+                                <div class="col-auto">
+                                    <select id="sortingCriteria" class="form-control">
+                                        <option value="name-asc">Name Ascending</option>
+                                        <option value="name-desc">Name Descending</option>
+                                        <option value="cost-asc">Cost Ascending</option>
+                                        <option value="cost-desc">Cost Descending</option>
+                                        <option value="votes-asc">Votes Ascending</option>
+                                        <option value="votes-desc">Votes Descending</option>
+                                      </select>
+                                </div>
+                                <div class="col-auto">
+                                    <select class="form-control" id="filterBy">
+                                        <option value="all">All</option>
+                                        <option value="selected">Selected</option>
+                                        <option value="rejected">Rejected</option>
+                                      </select>
+                                </div>
                             </div>
                         </div>
+                        <div class="col-1"></div>
 
-                        <div class='cost-locator-container'>
-                            <div class='cost-locator'
-                                style='left: calc({{ (round.initial_voter_funding / budget | float) * 100 }}&#37; - 9px);'
-                                data-tippy-content='Project initially has a funding of {{ round.initial_voter_funding | int }} GBP.'>
-                                <b>
-                                    &uarr;
-                                </b>
-                                {{ round.initial_voter_funding | int}}
-                            </div>
+                    </div>
+                    <div class="spacer-1"></div>
+                    
+                    <div class="row">
+                        <div class="col-1"></div>
+                        <div class="col-10">
+                            <div class="spacer-1"></div>
+                            <div class="spacer-1"></div>
+                            <p> 
+                                The chart above shows the number of votes for each project. To investigate further, you can filter the bar chart by selected or rejected projects, and sort by name, cost or votes. Use the dropdowns above to filter and sort the data.
+                            </p>
                         </div>
+                        <div class="col-1"></div>
                     </div>
-                </td>
-                </tr>
-                <tr class='hidden-row' id='hidden-{{ round.id }}'>
-                    <td colspan=7>
-                        <div style='text-align: left'>
-                            <b>Round Analysis:</b><a href='round_analysis.html?projectId={{ round.id }}'> Click Me!</a> <br>
-                            <b>Description:</b> {{ projects[round.id]["description"] }} <br>
-                            <b>Categories:</b> <br>
-                            {% for category in projects[round.id]["categories"] %}
-                                {{ category }} <br>
-                            {% endfor %}
-                            <b>Other Details:</b><br>
-                            <br>
-                            <!-- Sample expalanations -->
-                            <div>
-                                <h4>Why was this project selected?</h4>
-                                {% if round.initial_voter_funding != round.final_voter_funding %}
-                                    This project was accepted because its cost (<b>{{ round.cost }}</b> GBP) was less than or equal to the combined funds of its supporters at round {{ loop.index }} - <b>{{ '%0.2f' % round.final_voter_funding | float }}</b> GBP.<br>
-                                    (sentence about its initial funding value)<br>
-                                    (sentence about how it lost some of its inital funding value)<br>
-                                    (conclusion sentence talking about the final funding value and comparing it to the cost?)<br>
-                                {% else %}
-                                    This project was accepted because its cost (<b>{{ round.cost }}</b> GBP) was less than or equal to the combined funds of its supporters (<b>{{ '%0.2f' % round.final_voter_funding | float }}</b> GBP),
-                                    and no funding for this project was lost in the previous rounds.
-                                {% endif %}
-                            </div>
-                            <br>
-                            <h4>Funding spent in previous rounds.</h4>
-                            {% if round.initial_voter_funding != round.final_voter_funding %}
-                                From the initial total funding, <b> {{ (round.initial_voter_funding - round.final_voter_funding) | int }} GBP </b> was spent on previously selected projects. <br> 
-                                The funding was spent on:
-                                <ul>
-                                    {% for r in round.funding_lost_per_round %}
-                                        <li>
-                                            <b>Project {{ rounds[r].id }} - {{ projects[rounds[r].id]["name"] }}:</b> {{ round.funding_lost_per_round[r] | int }} GBP
-                                            <hr style="width: {{ (round.funding_lost_per_round[r] / (round.initial_voter_funding - round.final_voter_funding))  * 100 }}&#37;;
-                                                        height: 10px;
-                                                        color: #f6c8c8;
-                                                        background-color: #f6c8c8;
-                                                        text-align: left;
-                                                        margin-left: 0;
-                                                        margin-right: 5px;
-                                                        margin-bottom: 7px;
-                                                        margin-top: 3px">
-                                        </li>
-                                    {% endfor %}
-                                </ul>
-                            {% else %}
-                                None of the initial total funding was spent on previously selected projects.
-                            {% endif %}
+
+                    <div class="spacer-1"></div>
+                    <hr>
+                    <div class="spacer-1"></div>
+                    <div class="row">
+                        <div class="col-2"></div>
+                        <div class="col-8" style="justify-content: center;">
+                            <div class="spacer-1"></div>
+
+                            <h3>Round by Round Analysis</h3>
+                            <hr>
+                            <p>
+                                    The following section of the visualisations allows you to click through 'round by round' of this section of the election. It shows at each point the remaining budget, and the projects with the most votes up to the selected project. The selected project is shown in green, and any rejected projects are shown in red. A project will be shown in red if it is the next most popular project however there is not enough budget remaining to purchase the project. This means, the next most popular project will be considered - and so on until a project is found that can be purchased with the remaining budget. Use the previous and next round buttons to move through the different rounds of the election.
+                            </p>
                         </div>
-                    </td>
-                </tr>
-                {% if round.dropped_projects %}
-                    {% for rejected in round.dropped_projects %}
-                        <tr class='clickable-row loser' id='project-{{ rejected.id }}' onclick="showHiddenRow('{{ rejected.id }}');">
-                        <td><div class="split-cell"><span id="expand-symbol-{{ rejected.id }}">&#8250;</span></div></td>
-                        <td class='num' style='text-align:right' sorttable_customkey='{{ rejected.id }}'>{{ rejected.id }}</td>
-                        <td>{{ projects[rejected.id]["name"] }}</td>
-                        <td class='num' style='text-align:right' sorttable_customkey='{{ rejected.cost }}'>{{ rejected.cost }}</td>
-                        <td class='num' style='text-align:right' sorttable_customkey='{{ rejected.totalvotes }}'>{{ rejected.totalvotes }}</td>
-                        <td style='text-align:right' sorttable_customkey='{{ round.effective_vote_count[rejected.id] }}'>{{ round.effective_vote_count[rejected.id] | int }}</td>
-                        <td>
-                            <div class='chart-container'>
-                                <div class='cost-locator-container'>
-                                    <div class='cost-locator' 
-                                        style='left: calc({{ (rejected.cost / budget | float) * 100 }}&#37; - 9px);'
-                                        data-tippy-content='Project Cost: {{ rejected.cost }} GBP.'>
-                                            <b>
-                                                &darr; {{ rejected.cost }}
-                                            </b>
-                                    </div>
-                                </div>
-        
-                                <div class='chart'>
-                                    <div class='bar bar-blue'
-                                        style='width: {{ (rejected.final_voter_funding / budget | float) * 100 }}&#37;;'
-                                        data-tippy-content='&#10004; Supporters of the project have {{ rejected.final_voter_funding | int }} GBP, which is enough to cover the cost {{ rejected.cost }} GBP.'>
-                                    </div>
-        
-                                    <div class='bar bar-light'
-                                        onmouseover='highlight_project([
-                                            {% for r in rejected.funding_lost_per_round %}
-                                                {% if loop.index0 < 3 %}
-                                                    "project-{{ rounds[r].id }}",
-                                                {% endif %}
-                                            {% endfor %}
-                                        ])'
-                                        onmouseout='unhighlight_project([
-                                            {% for r in rejected.funding_lost_per_round %}
-                                                {% if loop.index0 < 3 %}
-                                                    "project-{{ rounds[r].id }}",
-                                                {% endif %}
-                                            {% endfor %}
-                                        ])'
-                                        style='width: {{ ((rejected.initial_voter_funding - rejected.final_voter_funding) / budget | float) * 100 }}&#37;;'
-                                        data-tippy-content='<html lang=\"en\"><body>From the initial total funding, <b> {{ (rejected.initial_voter_funding - rejected.final_voter_funding) | int }} GBP </b> was spent on previously selected projects. </br> 
-                                        Most of the funding was spent on:<br><br>
-                                        <ul>
-                                            {% for r in rejected.funding_lost_per_round %}
-                                                {% if loop.index0 < 3 %}
-                                                    <li>
-                                                        <b>Project {{ rounds[r].id }} - {{ projects[rounds[r].id]["name"] }}:</b> {{ rejected.funding_lost_per_round[r] | int }} GBP
-                                                        <hr style="width: {{ (rejected.funding_lost_per_round[r] / (rejected.initial_voter_funding - rejected.final_voter_funding))  * 100 }}&#37;;
-                                                            height: 10px;
-                                                            color: #f6c8c8;
-                                                            background-color: #f6c8c8;
-                                                            text-align: left;
-                                                            margin-left: 0px;
-                                                            margin-right: 5px;
-                                                            margin-bottom: 7px;
-                                                            margin-top: 3px">
-                                                        </hr>
-                                                    </li>
-                                                {% endif %}
-                                            {% endfor %}
-                                        </ul>
-                                        '
-                                        allowHTML: true>
-                                    </div>
+                        <div class="col-2"></div>
+                    </div>
+                    <div class="row">
+                        <div class="col-1"></div>
+                        <div class="col-10">
+                            <div class="row justify-content-center">
+                                <div class="col-auto">
+                                    <button id="prevButton" class="btn btn-secondary">Previous Round</button>
                                 </div>
-        
-                                <div class='cost-locator-container'>
-                                    <div class='cost-locator'
-                                        style='left: calc({{ (rejected.initial_voter_funding / budget | float) * 100 }}&#37; - 9px);'
-                                        data-tippy-content='Project initially has a funding of {{ rejected.initial_voter_funding | int }} GBP.'>
-                                        <b>
-                                            &uarr;
-                                        </b>
-                                        {{ rejected.initial_voter_funding | int}}
-                                    </div>
+                                <div class="col-auto">
+                                    <button id="nextButton" class="btn btn-secondary">Next Round</button>
                                 </div>
                             </div>
-                        </td>
-                        </tr>
-                        <tr class="hidden-row" id="hidden-{{ rejected.id }}">
-                            <td colspan=7>
-                                <div style='text-align: left'>
-                                    <b>Description:</b> {{ projects[rejected.id]["description"] }} <br>
-                                    <b>Categories:</b> <br>
-                                    {% for category in projects[rejected.id]["categories"] %}
-                                        {{ category }} <br>
-                                    {% endfor %}
-                                    <b>Other Details:</b><br>
-                                    <br>
-
-                                    <!-- Sample expalanations -->
-                                    <div style="text-align: left">
-                                        <h4>Why was this project not selected?</h4>
-                                        {% if rejected.initial_voter_funding >= rejected.cost %}
-                                            Project initially had funding to be accepted but lost too much funding in previous rounds.<br>
-                                            (mention the important projects that made it lose funding to go below the required cost)<br>
-                                            (mention that these important projects had a higher effective vote count, meaning they were selected earlier than this project)<br>
-                                            (mention by current round that project cost is greater than combined funds of supporters, making it unaffordable)
-                                        {% else %}
-                                            This project was rejected because its cost (<b>{{ rejected.cost }}</b> GBP) was greater than the combined funds of its supporters (<b>{{ '%0.2f' % rejected.initial_voter_funding | float }}</b> GBP),
-                                            even before any funding was lost.
-                                        {% endif %}
+                        </div>
+                        <div class="col-1"></div>
+                    </div>
+
+                    {% for round in rounds %}
+                    <div class="container" id="{{round.id}}Bars" style="display: none;">
+                        
+                        <!-- Budget Breakdown -->
+                        <div class="row">
+                            <div class="col-2"></div>
+                            <div class="col-8">
+                                <div class="row">
+                                    <div class="budget-container">
+                                        <!-- Remaining Budget Bar -->
+                                        <div class="bar-container">
+                                            <h4>Round {{loop.index0 + 1}}</h4>
+                                            {% if (round.remaining_budget / round.max_cost) * 90 > 30 %}
+                                                <div class="bar budget" style="width: {{ (round.remaining_budget / round.max_cost) * 90 }}%;">
+                                                    <div class="bar-inner">&nbsp; Remaining Budget: {{ "{:,}".format( (round.remaining_budget | int) ) }} {{ currency }}</div>
+                                                </div>
+                                            {% else %}
+                                            <div>
+                                                <div class="bar budget" style="width: {{ (round.remaining_budget / round.max_cost) * 100 }}%; display: inline-flex; align-items: center;">
+                                                </div>
+                                                <div style="margin-left: 10px; display: inline-flex;"><p style="position:absolute; top: 12px;">&nbsp; Remaining Budget: {{ "{:,}".format( (round.remaining_budget | int) ) }} {{ currency }}</p></div>
+
+                                            </div>
+                                            {% endif %}
+                                        </div>
+
+                                        <!-- Project Bars -->
+                                        {% for proj in round.rejected_projects %}
+                                        <div class="bar-container">
+                                            {% if (proj.cost / round.max_cost) * 90 > 30 %}
+                                                <div class="bar red" style="width: {{ (proj.cost / round.max_cost) * 90 }}%;">
+                                                    <div class="bar-inner">&nbsp; {{proj.name}} - {{ proj.cost }} {{ currency }}</div>
+                                                    <div class="rejected-mark">✘</div>
+                                                </div>
+                                            {% else %}
+                                                <div>
+                                                    <div class="bar red" style="width: {{ (proj.cost / round.max_cost) * 90 }}%; display: inline-flex; align-items: center;">
+                                                    </div>
+                                                    <div class="rejected-mark">✘</div>
+                                                    <div style="margin-left: 10px; display: inline-flex;"><p style="position:absolute; top: 12px;">{{ round.selected_project.id }}: {{ projects[round.selected_project.id]["name"] }} - {{ "{:,}".format( (round.selected_project.cost | int) ) }} {{ currency }}</p></div>
+
+                                                </div>
+                                            {% endif %}
+                                        </div>
+                                        {% endfor %}
+
+                                        <!-- Selected Project Bar -->
+                                        <div class="bar-container">
+                                            {% if (round.selected_project.cost / round.max_cost) * 90  > 30 %}
+                                            <div class="bar green" style="width: {{ (round.selected_project.cost / round.max_cost) * 90 }}%;">
+                                                <div class="bar-inner"><nobr> {{ round.selected_project.id }}: {{ projects[round.selected_project.id]["name"] }} - {{ "{:,}".format( (round.selected_project.cost | int) ) }} {{ currency }}</nobr></div>
+                                            </div>
+                                            {% else %}
+                                            <div>
+                                                <div class="bar green" style="width: {{ (round.selected_project.cost / round.max_cost) * 90 }}%; display: inline-flex; align-items: center;">
+                                                </div>
+                                                <div style="margin-left: 10px; display: inline-flex;"><p style="position:absolute; top: 12px;">{{ round.selected_project.id }}: {{ projects[round.selected_project.id]["name"] }} - {{ "{:,}".format( (round.selected_project.cost | int) ) }} {{ currency }}</p></div>
+
+                                            </div>
+                                            {% endif %}
+                                        </div>
                                     </div>
-                                    <br>
-                                    <h4>Funding spent in previous rounds.</h4>
-                                    {% if rejected.initial_voter_funding != rejected.final_voter_funding %}
-                                        From the initial total funding, <b> {{ (rejected.initial_voter_funding - rejected.final_voter_funding) | int }} GBP </b> was spent on previously selected projects. <br> 
-                                        The funding was spent on:
-                                        <ul>
-                                            {% for r in rejected.funding_lost_per_round %}
-                                                <li>
-                                                    <b>Project {{ rounds[r].id }} - {{ projects[rounds[r].id]["name"] }}:</b> {{ rejected.funding_lost_per_round[r] | int }} GBP
-                                                    <hr style="width: {{ (rejected.funding_lost_per_round[r] / (rejected.initial_voter_funding - rejected.final_voter_funding))  * 100 }}&#37;;
-                                                                height: 10px;
-                                                                color: #f6c8c8;
-                                                                background-color: #f6c8c8;
-                                                                text-align: left;
-                                                                margin-left: 0px;
-                                                                margin-right: 5px;
-                                                                margin-bottom: 7px;
-                                                                margin-top: 3px">
-                                                </li>
-                                            {% endfor %}
-                                        </ul>
+                                </div>
+                                <div class="row">
+                                    {% if round.rejected_projects %}
+                                        <p>
+                                            The chart above shows the current budget of {{ "{:,}".format( (round.remaining_budget | int) ) }} {{ currency }}. Projects {% for proj in round.rejected_projects %} {{ projects[proj.id]["name"] }}, {% endfor %} were rejected in this round, even though they had more votes than the selected project which had {{projects[round.selected_project.id]["votes"]}} votes.  
+                                        </p>
                                     {% else %}
-                                        None of the initial total funding was spent on previously selected projects.
+                                        <p>
+                                            The chart above shows the current budget of {{ "{:,}".format( (round.remaining_budget | int) ) }} {{ currency }}, and the selected project "{{ projects[round.selected_project.id]["name"] }}" with cost {{ "{:,}".format( (round.selected_project.cost | int) ) }} {{ currency }}. The selected project was chosen because it had the most votes ({{projects[round.selected_project.id]["votes"]}}) and was within budget.
+                                        </p>
                                     {% endif %}
                                 </div>
-                            </td>
-                        </tr>
+                            </div>
+                            <div class="col-2"></div>
+                        </div>
+                    </div>
                     {% endfor %}
-                {% endif %}
-            {% endfor %}
-        </tbody>
-    </table>
+                    
+                    <div class="spacer-1"></div>
+                    <hr>
+                    <div class="spacer-1"></div>
+
+                    <!-- Green and Red Painted Chart -->
+                    <div class="row featurette">
+                            <div class="col-1"></div>
+                            <div class="col-10" style="min-height: 600px;">
+                                <div id="RGBarChart" style="height: 100%; width: 100%;">
+                                    <button class = "info-button" style = "position: absolute; z-index: 2000; right: 50px;" data-tippy-content= "<b>Project Vote Counts:</b><br> The following graphs shows the votes for each of the projects along with the corresponding budget.<br>The green bars correspond to selected projects, the red bars correspond to rejected projects.">i</button>
+                                </div>
+                            </div>
+                            <div class="col-1"></div>
+                        
+                    </div>
+                    <div class="row">
+                        <div class="col-1"></div>
+                        <div class="col-10">
+                            <p>
+                                The chart above shows a colour coded bar chart, which shows the selected projects in order. Red for selected, green for rejected. This is a quick over-view visualisation showing that it is not always the most popular project which is selected, but the most popular projects within budget.
+                            </p>
+                        </div>
+                        <div class="col-1"></div>
+                    </div>
+                </section>
+            
+            <div class="spacer-8"></div>
+        </div>
 
-    <!-- <h2>[GOOGLE TRANSLATE] Comparison of the method of equal shares with the greedy method</h2> -->
+        <div class="spacer-1"></div>
+        <hr>
+        <div class="spacer-1"></div>
+
+        <!-- FOOTER -->
+        <footer class="container">
+            <p>© Pabutools. · <a href="https://getbootstrap.com/docs/4.0/examples/carousel/#">Privacy</a> · <a href="https://getbootstrap.com/docs/4.0/examples/carousel/#">Terms</a></p>
+        </footer>
 
-    <!-- <p>[GOOGLE TRANSLATE] We conducted an analysis comparing the equal shares method to the greedy method, which is the most frequently used method in citizen budgets. </p> -->
+    </main>
+    <!-- Bootstrap JS and its dependencies -->
+    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
+    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.14.7/dist/umd/popper.min.js"></script>
+    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"></script>
+    <script>
+        document.getElementById("1Bars").style.display = "block";
+
+        let currentRoundIndex = 1;
+        const roundsIds = document.querySelectorAll('.container').length;
+
+        function displayRound(index) {
+            const currentRoundId = index + 'Bars'; 
+            const currentRound = document.getElementById(currentRoundId);
+            if (currentRound) currentRound.style.display = 'block';
+        }
+        function hideRound(index) {
+            const currentRoundId = index + 'Bars'; 
+            const currentRound = document.getElementById(currentRoundId);
+            if (currentRound) currentRound.style.display = 'none';
+        }
+
+        displayRound(currentRoundIndex);
+
+        document.getElementById('prevButton').addEventListener('click', function() {
+
+            if (currentRoundIndex > 1) {
+                hideRound(currentRoundIndex);
+                currentRoundIndex--;
+                displayRound(currentRoundIndex);
+            }
+        });
 
-    <!-- !COMPARISON! -->
+        document.getElementById('nextButton').addEventListener('click', function() {
+            if (currentRoundIndex < roundsIds - 3) {
+                hideRound(currentRoundIndex);
+                currentRoundIndex++; 
+                displayRound(currentRoundIndex);
+            }
+        });
 
-    <script src="https://unpkg.com/@popperjs/core@2"></script>
-    <script src="https://unpkg.com/tippy.js@6"></script>
-    <script>tippy('[data-tippy-content]', { allowHTML: true, maxWidth: 1000 });
+        document.getElementById('electionOutcome').addEventListener('click', function() {
+            const ul = document.getElementById('outcomeList');
+            if (ul.style.display === 'none') {
+                ul.style.display = 'block';
+            } else {
+                ul.style.display = 'none';
+            }
+        });
+        
+    </script>
+
+    <script>
+        document.addEventListener('DOMContentLoaded', function() {
+            projects_selected_or_rejected = JSON.parse('{{projects_selected_or_rejected | safe}}')
+            var projects = {};
+            {% for project_id in project_votes.keys() %}
+            projects["{{ project_id }}"] = {
+                name: "{{ projects[project_id]['name'][:15]|replace('\"', '\\\"') }}",
+                votes: parseInt({{ project_votes[project_id] }}),
+                cost: parseFloat({{ projects[project_id]['cost'] }}),
+                selected: projects_selected_or_rejected["{{ project_id }}"]
+            };
+            {% endfor %}
 
-        function highlight_project(ids) {
-            for (i = 0; i < ids.length; i++) {
-                document.getElementById(ids[i]).classList.add('highlighted');
+            
+            function sortAndRenderChart(criteria, filterBy) {
+                console.log(projects);
+                var filteredProjects = Object.values(projects).filter(function(project) {
+                    if (filterBy === 'all') {
+                        return true; 
+                    } else if (filterBy === 'selected') {
+                        return project.selected === true; 
+                    } else if (filterBy === 'rejected') {
+                        return project.selected === false; 
+                    }
+                });
+                    var sortOrder = criteria.split('-')[1];
+                    var sortBy = criteria.split('-')[0];
+                    var sortedProjects = Object.values(filteredProjects).sort(function(a, b) {
+                        if (sortBy === 'name') {
+                            return sortOrder === 'asc' ? a.name.localeCompare(b.name) : b.name.localeCompare(a.name);
+                        } else {
+                            return sortOrder === 'asc' ? a[sortBy] - b[sortBy] : b[sortBy] - a[sortBy];
+                        }
+                    });
+                  
+                    var labels = sortedProjects.map(function(p) { return p.name; });
+                    var values = sortedProjects.map(function(p) { return parseInt(p.votes, 10); });
+                    var data ={
+                        "type": "hbar",
+                        "title": {
+                            "text": "Vote Count Bar Chart"
+                        },
+                        shapes: [
+                            {
+                                "type": "circle",
+                                "background-color": "#5297b6",
+                                "size": 20,
+                                "x": 35,
+                                "y": 25,
+                                "tooltip": {
+                                    "text": "This bar chart shows the number of votes for each project.",
+                                    "background-color": "white",
+                                    "font-color": "gray",
+                                    "font-family": "Georgia",
+                                    "background-color": "white",
+                                    "border-color": "gray",
+                                    "border-width": 1,
+                                    "line-style": "dotted",
+                                    "padding": "15%",
+                                },
+                                label: {
+                                    text: 'i', 
+                                    fontSize: 28,
+                                    fontWeight: 'bold',
+                                    fontColor: '#fff'
+                                }
+                            }
+                        ],
+                        "scrollX": {
+                                        "bar": {
+                                        "backgroundColor": '#2596be',
+                                        "alpha": 0.5,
+                                        },
+                                        "handle": {
+                                        "backgroundColor": '#2596be',
+                                        },
+                                    },
+                        "plotarea": {
+                            "margin-left":"130px",
+                            "margin-right":"130px"
+                        },
+                        "scale-x": {
+                            "labels": labels,
+                            "title": {
+                            "text": "Project"
+                            },
+                            "item": { 
+                            "font-size": 14, 
+                            "offset-x": 0, 
+                            "offset-y": 0 
+                            },"zooming": true,
+                                "zoomTo": [0, 15]
+                        },
+                        "scale-y": {
+                            "title": {
+                            "text": "Number of Votes"
+                            }
+                        },
+                        "series": [{
+                            "values": values ,
+                            'hover-state': {
+                            'background-color': "orange",
+                        }
+                        }, ],
+                        "plot": {
+                            "tooltip": {
+                            "text": "Project %scale-key-label has %v votes"
+                        },
+                            "animation": {
+                            "effect": "ANIMATION_SLIDE_BOTTOM",
+                            "sequence": "ANIMATION_BY_PLOT_AND_NODE",
+                            "speed": 0
+                            }
+                        }
+                    }
+                    zingchart.render({
+                        id: 'SortableBarChart',
+                        data: data,
+                        height: '100%',
+                        width: '100%'
+                },
+                );
             }
-        }
-        function unhighlight_project(ids) {
-            for (i = 0; i < ids.length; i++) {
-                document.getElementById(ids[i]).classList.remove('highlighted');
+
+            sortAndRenderChart('votes-desc', 'all');
+
+            document.getElementById('sortingCriteria').addEventListener('change', function() {
+                filter = document.getElementById('filterBy').value;
+                sortAndRenderChart(this.value, filter);
+            });
+
+            document.getElementById('filterBy').addEventListener('change', function() {
+                sort = document.getElementById('sortingCriteria').value;
+                sortAndRenderChart(sort, this.value);
+            });
+        });
+</script>
+<script>
+    projects_selected_or_rejected = JSON.parse('{{projects_selected_or_rejected | safe}}')
+    var projectNames = {{ project_votes.keys() | list }};
+    var projectValues = {{ project_votes.values() | list }};
+    var seriesData = [];
+    var pNames = projectNames;
+    colorsList = [] 
+
+    for (var i = 0; i < projectNames.length; i++) {
+        var projectName = projectNames[i];
+        var projectValue = projectValues[i];
+        var selectedOrRejected = projects_selected_or_rejected[projectName];
+        var color = selectedOrRejected ? 'green' : 'red';
+        colorsList.push(color);
+
+    }
+
+
+    var config = {
+        "type": "hbar",
+        "title": {
+            "text": "Vote Count Bar Chart"
+        },
+        shapes: [{
+            "type": "circle",
+            "background-color": "#5297b6",
+            "size": 20,
+            "x": 35,
+            "y": 25,
+            "tooltip": {
+                "text": "<b>Project Vote Counts:</b><br> The following graphs shows the votes for each of the projects along with the corresponding budget.<br>The green bars correspond to selected projects, the red bars correspond to rejected projects.",
+                "background-color": "white",
+                "font-color": "gray",
+                "font-family": "Georgia",
+                "border-color": "gray",
+                "border-width": 1,
+                "line-style": "dotted",
+                "padding": "15%",
+            },
+            label: {
+                text: 'i',
+                fontSize: 28,
+                fontWeight: 'bold',
+                fontColor: '#fff'
+            }
+        }],
+        "scrollX": {
+            "bar": {
+                "backgroundColor": '#2596be',
+                "alpha": 0.5,
+            },
+            "handle": {
+                "backgroundColor": '#2596be',
+            },
+        },
+        "plotarea": {
+            "margin-left":"130px",
+            "margin-right":"130px"
+        },
+        "scale-x": {
+            "labels": [{% for project_id in project_votes.keys() %}"{{ projects[project_id]['name'][:15]|replace('\"', '\\\"') }}",{% endfor %}],
+            "title": {
+                "text": "Project"
+            },
+            "item": {
+                "font-size": 14,
+                "offset-x": 0,
+                "offset-y": 0
+            },
+            "zooming": true,
+            "zoomTo": [0, 15]
+        },
+        "scale-y": {
+            "title": {
+                "text": "Number of Votes"
+            }
+        },
+        "series": [{
+            "values": {{ project_votes.values() | list }},
+            'hover-state': { 
+                'background-color': "orange",
+            }
+        }, ],
+        "plot": {
+            "styles": colorsList,
+            "tooltip": {
+                "text": "Project %scale-key-label has %v votes"
+            },
+            "animation": {
+                "effect": "ANIMATION_SLIDE_BOTTOM",
+                "sequence": "ANIMATION_BY_PLOT_AND_NODE",
+                "speed": 0
             }
         }
-    </script>
-</body>
+    }
 
+
+
+    zingchart.render({
+    id: 'RGBarChart',
+    data: config,
+    height: '100%',
+    width: '100%'
+});
+</script>
+    <script src="https://unpkg.com/@popperjs/core@2"></script>
+    <script src="https://unpkg.com/tippy.js@6"></script>
+    <script>tippy('[data-tippy-content]', { allowHTML: true, maxWidth: 1000});</script>
+    <script type="text/javascript" src="https://unpkg.com/default-passive-events"></script>
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,105 +1,96 @@
-_S_u_m_m_a_r_y_(_c_u_r_r_e_n_t_)
-    * _R_o_u_n_d_ _B_y_ _R_o_u_n_d
-    * Pabutools
-    * MES
-[                    ]Search
+_S_u_m_m_a_r_y
+    * _R_o_u_n_d_ _B_y_ _R_o_u_n_d_ _(_c_u_r_r_e_n_t_)
+    * _P_a_b_u_t_o_o_l_s
 ************ {{{{ eelleeccttiioonn__nnaammee }}}} ************
 ===============================================================================
+This is the explanation for the outcome of the participatory budgeting election
+decided using the Greedy Utilitarian Welfare algorithm.
+Some of the key features of the election are: The election has a total budget
+of {{ "{:,}".format((budget | int)) }} {{ currency }} of which {{ "{:,}".format
+((spent | int)) }} {{ currency }} was spent. The election had a total of {
+{total_votes}} voters. Note that each participant can vote for multiple
+projects. Therefore, the total votes for all projects may be higher than {
+{total_votes}}
+This page shows and explains the outcome of the election. The first graph shows
+the number of votes for each project. The bars show the budget at each stage of
+the election and the projects selected or rejected in each round. Finally, the
+final bar chart shows an overview of the selected and rejected projects.
+To view the list of the projects selected, click this: View Election Outcome
+{% for round in rounds %}
+Project: "{{ projects[round.selected_project.id]["name"] }}" with cost: {{ "
+{:,}".format( (round.selected_project.cost | int) ) }} {{ currency }} and had {
+{round.selected_project.votes}} votes.
+{% endfor %}
+===============================================================================
+i
+[One of: Name Ascending/Name Descending/Cost Ascending/Cost Descending/Votes
+Ascending/Votes Descending]
+[One of: All/Selected/Rejected]
+The chart above shows the number of votes for each project. To investigate
+further, you can filter the bar chart by selected or rejected projects, and
+sort by name, cost or votes. Use the dropdowns above to filter and sort the
+data.
 ===============================================================================
-********** RReessuullttss **********
-The budget of {{ budget }} GBP was allocated across {{ rounds|length }}
-projects:
-
-BBuuddggeett aallllooccaattiioonn aaccrroossss sseelleecctteedd pprroojjeeccttss..
+******** RRoouunndd bbyy RRoouunndd AAnnaallyyssiiss ********
+===============================================================================
+The following section of the visualisations allows you to click through 'round
+by round' of this section of the election. It shows at each point the remaining
+budget, and the projects with the most votes up to the selected project. The
+selected project is shown in green, and any rejected projects are shown in red.
+A project will be shown in red if it is the next most popular project however
+there is not enough budget remaining to purchase the project. This means, the
+next most popular project will be considered - and so on until a project is
+found that can be purchased with the remaining budget. Use the previous and
+next round buttons to move through the different rounds of the election.
+Previous Round
+Next Round
 {% for round in rounds %}
+****** RRoouunndd {{{{lloooopp..iinnddeexx00 ++ 11}}}} ******
+{% if (round.remaining_budget / round.max_cost) * 90 > 30 %}
+  Remaining Budget: {{ "{:,}".format( (round.remaining_budget | int) ) }} {
+{ currency }}
+{% else %}
+  Remaining Budget: {{ "{:,}".format( (round.remaining_budget | int) ) }} {
+{ currency }}
+{% endif %}
+{% for proj in round.rejected_projects %}
+{% if (proj.cost / round.max_cost) * 90 > 30 %}
+  {{proj.name}} - {{ proj.cost }} {{ currency }}
+✘
+{% else %}
+✘
+{{ round.selected_project.id }}: {{ projects[round.selected_project.id]["name"]
+}} - {{ "{:,}".format( (round.selected_project.cost | int) ) }} {{ currency }}
+{% endif %}
 {% endfor %}
-{{ election_name}} had a total of {{ total_votes }} voters participating.
-Between these voters there was a total of {{ budget }} GBP available, of which
-{{ spent }} GBP was spent.
-In total, there were {{ number_of_elected_projects }} projects elected, and {
-{ number_of_unelected_projects }} projects not elected.
-{# The elected projects were:
-{% for p in projects %} {{ projects[p]["name"] }}, {% endfor %} #}
-{#
-The projects and their descriptions are as follows:
-{% for p in projects %} {{ projects[p]["name"] }}: {{ projects[p]
-["description"] }}
+{% if (round.selected_project.cost / round.max_cost) * 90 > 30 %}
+{{ round.selected_project.id }}: {{ projects[round.selected_project.id]
+["name"] }} - {{ "{:,}".format( (round.selected_project.cost | int) ) }} {
+{ currency }}
+{% else %}
+{{ round.selected_project.id }}: {{ projects[round.selected_project.id]["name"]
+}} - {{ "{:,}".format( (round.selected_project.cost | int) ) }} {{ currency }}
+{% endif %}
+{% if round.rejected_projects %}
+The chart above shows the current budget of {{ "{:,}".format(
+(round.remaining_budget | int) ) }} {{ currency }}. Projects {% for proj in
+round.rejected_projects %} {{ projects[proj.id]["name"] }}, {% endfor %} were
+rejected in this round, even though they had more votes than the selected
+project which had {{projects[round.selected_project.id]["votes"]}} votes.
+{% else %}
+The chart above shows the current budget of {{ "{:,}".format(
+(round.remaining_budget | int) ) }} {{ currency }}, and the selected project "{
+{ projects[round.selected_project.id]["name"] }}" with cost {{ "{:,}".format(
+(round.selected_project.cost | int) ) }} {{ currency }}. The selected project
+was chosen because it had the most votes ({{projects[round.selected_project.id]
+["votes"]}}) and was within budget.
+{% endif %}
 {% endfor %}
-#}
-{% set voter_budget = (budget | int) / (total_votes | int) %} Each of the
-voters had a budget of {{ '%0.2f' % voter_budget | float }} GBP to allocate to
-the projects.
-The projects were elected using the Method of Equal Shares, where the total
-budget is virtually divided equally among the voters.
-The following web-page outlines the process of the election and the step by
-step process of how each project was chosen.
-RRoouunndd      IIDD          PPrroojjeecctt NNaammee  CCoosstt          NNuummbbeerr ooff VVootteess     EEffffeeccttiivvee SSuuppppoorrtt          CChhaarrtt
-                                                                                                  ?↓ {{{{ rroouunndd..ccoosstt }}}}
-                                                                                                  {#
-                                                                                                  Project {candidate.name} (
-                                                                                                  {display_short_string
-                                                                                                  (candidate.id)}): {display_int
-›{                                                                     {                          (int(paid))} zł.
-{          {{ round.id {{ projects   {{ round.cost {{ round.totalvotes {                          paid/ total_paid}%; height:
-loop.index }}          [round.id]    }}            }}                  round.effective_vote_count 10px; color:#f6c8c8;
-}}                     ["name"] }}                                     [round.id] | int }}        background-color:#f6c8c8;
-                                                                                                  text-align:left; margin-left:
-                                                                                                  0\">
-                                                                                                  " #}
-                                                                                                  ?↑ {
-                                                                                                  { round.initial_voter_funding
-                                                                                                  | int}}
-RRoouunndd AAnnaallyyssiiss::_ _C_l_i_c_k_ _M_e_!
-DDeessccrriippttiioonn:: {{ projects[round.id]["description"] }}
-CCaatteeggoorriieess::
-{% for category in projects[round.id]["categories"] %} {{ category }}
-{% endfor %} OOtthheerr DDeettaaiillss::
-
-****** WWhhyy wwaass tthhiiss pprroojjeecctt sseelleecctteedd?? ******
-{% if round.initial_voter_funding != round.final_voter_funding %} This project was accepted because its cost ({{{{ rroouunndd..ccoosstt }}}}
-GBP) was less than or equal to the combined funds of its supporters at round {{ loop.index }} - {{{{ ''%%00..22ff'' %%
-rroouunndd..ffiinnaall__vvootteerr__ffuunnddiinngg || ffllooaatt }}}} GBP.
-(sentence about its initial funding value)
-(sentence about how it lost some of its inital funding value)
-(conclusion sentence talking about the final funding value and comparing it to the cost?)
-{% else %} This project was accepted because its cost ({{{{ rroouunndd..ccoosstt }}}} GBP) was less than or equal to the combined funds of its
-supporters ({{{{ ''%%00..22ff'' %% rroouunndd..ffiinnaall__vvootteerr__ffuunnddiinngg || ffllooaatt }}}} GBP), and no funding for this project was lost in the previous
-rounds. {% endif %}
-
-****** FFuunnddiinngg ssppeenntt iinn pprreevviioouuss rroouunnddss.. ******
-{% if round.initial_voter_funding != round.final_voter_funding %} From the initial total funding, {{{{
-((rroouunndd..iinniittiiaall__vvootteerr__ffuunnddiinngg -- rroouunndd..ffiinnaall__vvootteerr__ffuunnddiinngg)) || iinntt }}}} GGBBPP was spent on previously selected projects.
-The funding was spent on:
-    * {% for r in round.funding_lost_per_round %}
-    * PPrroojjeecctt {{{{ rroouunnddss[[rr]]..iidd }}}} -- {{{{ pprroojjeeccttss[[rroouunnddss[[rr]]..iidd]][[""nnaammee""]] }}}}:: {{ round.funding_lost_per_round[r] | int }} GBP
-      ==========================================================================================================================
-    * {% endfor %}
-{% else %} None of the initial total funding was spent on previously selected projects. {% endif %}
-           {                         {             {                   {                          ?↓ {{{{ rreejjeecctteedd..ccoosstt }}}}
-           {           {{ projects   {             {                   {                          ?↑ {
-›          rejected.id [rejected.id] rejected.cost rejected.totalvotes round.effective_vote_count {
-           }}          ["name"] }}   }}            }}                  [rejected.id] | int }}     rejected.initial_voter_funding
-                                                                                                  | int}}
-DDeessccrriippttiioonn:: {{ projects[rejected.id]["description"] }}
-CCaatteeggoorriieess::
-{% for category in projects[rejected.id]["categories"] %} {{ category }}
-{% endfor %} OOtthheerr DDeettaaiillss::
-
-****** WWhhyy wwaass tthhiiss pprroojjeecctt nnoott sseelleecctteedd?? ******
-{% if rejected.initial_voter_funding >= rejected.cost %} Project initially had funding to be accepted but lost too much funding
-in previous rounds.
-(mention the important projects that made it lose funding to go below the required cost)
-(mention that these important projects had a higher effective vote count, meaning they were selected earlier than this project)
-(mention by current round that project cost is greater than combined funds of supporters, making it unaffordable) {% else %}
-This project was rejected because its cost ({{{{ rreejjeecctteedd..ccoosstt }}}} GBP) was greater than the combined funds of its supporters ({{
-{{ ''%%00..22ff'' %% rreejjeecctteedd..iinniittiiaall__vvootteerr__ffuunnddiinngg || ffllooaatt }}}} GBP), even before any funding was lost. {% endif %}
-
-****** FFuunnddiinngg ssppeenntt iinn pprreevviioouuss rroouunnddss.. ******
-{% if rejected.initial_voter_funding != rejected.final_voter_funding %} From the initial total funding, {{{{
-((rreejjeecctteedd..iinniittiiaall__vvootteerr__ffuunnddiinngg -- rreejjeecctteedd..ffiinnaall__vvootteerr__ffuunnddiinngg)) || iinntt }}}} GGBBPP was spent on previously selected projects.
-The funding was spent on:
-    * {% for r in rejected.funding_lost_per_round %}
-    * PPrroojjeecctt {{{{ rroouunnddss[[rr]]..iidd }}}} -- {{{{ pprroojjeeccttss[[rroouunnddss[[rr]]..iidd]][[""nnaammee""]] }}}}:: {{ rejected.funding_lost_per_round[r] | int }} GBP
-      ==========================================================================================================================
-    * {% endfor %}
-{% else %} None of the initial total funding was spent on previously selected projects. {% endif %}
+===============================================================================
+i
+The chart above shows a colour coded bar chart, which shows the selected
+projects in order. Red for selected, green for rejected. This is a quick over-
+view visualisation showing that it is not always the most popular project which
+is selected, but the most popular projects within budget.
+===============================================================================
+© Pabutools. · _P_r_i_v_a_c_y · _T_e_r_m_s
```

### Comparing `pabutools-1.1.6/pabutools/visualisation/templates/mes_round_analysis_template.html` & `pabutools-1.1.7/pabutools/visualisation/templates/mes_round_analysis_template.html`

 * *Files 22% similar despite different names*

```diff
@@ -27,18 +27,16 @@
         
         .spacer {
             padding: 1rem;
         }
         
         .carousel-control-prev-icon,
         .carousel-control-next-icon {
+            filter: invert(100%);
             font-size: 24px;
-            /* Adjust the size as needed */
-            color: black;
-            /* Adjust the color as needed */
         }
         
         .carousel-inner {
             padding: 1rem;
             padding-left: 7rem;
             padding-right: 7rem;
         }
@@ -51,38 +49,107 @@
         .hidden-section {
             display: none;
         }
         
         .chord-wrapper {
             height: 100%;
         }
+
+        .sankey-wrapper {
+            height: 100%;
+            padding-top: 80px;
+        }
         
         #myChordChart {
             height: 100%;
             width: 100%;
         }
         
         #myBarChart1,
         #myStackedBarChart1 {
             height: 100%;
             width: 100%;
         }
-        /* zing-grid[loading] {
-            height: 800px;
-            width: 100%;
-        } */
         
         h1,
+        h2,
+        h3,
+        h4,
         p {
             text-align: center;
         }
+
+        header, nav {
+            z-index: 9999;
+        }
+
+      
+        main {
+            padding-top: 100px; /* Adjust based on the actual height of your header */
+            }
+
+        .info-button {
+            margin-top: 25px;
+            /* padding-top: 100px; */
+        }
+
+        .text-container {
+            max-height: 50px;
+            overflow: hidden;
+            }
+
+            .text-expanded {
+            max-height: none;
+            }
+
+        #toggleButton {
+            background-color: #007BFF;
+            color: white;
+            border: none;
+            border-radius: 5px;
+            cursor: pointer;
+            transition: background-color 0.3s;
+            padding: 5px 15px; /* Smaller padding */
+            font-size: 14px; /* Smaller font size */
+        }
+
+        #toggleButton:hover {
+            background-color: #0056b3; 
+        }
+
+        #toggleButtonChord {
+            background-color: #007BFF;
+            color: white;
+            border: none;
+            border-radius: 5px;
+            cursor: pointer;
+            transition: background-color 0.3s;
+            padding: 5px 15px; /* Smaller padding */
+            font-size: 14px; /* Smaller font size */
+        }
+
+        #toggleButtonChord:hover {
+            background-color: #0056b3; 
+        }
+
+        .button-container {
+            display: flex;
+            justify-content: center; /* Center horizontally */
+            align-items: center; /* Center vertically if needed */
+            margin-top: 10px; /* Add space between the text and the button */
+            }
     </style>
+    <script>
+    window.addEventListener('load', (event) => {
+        loadRound();
+    });
+    </script>
 </head>
 
-<body onload="loadRound()">
+<body>
     <header>
         <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-dark">
           <a class="navbar-brand" href="./summary.html">Summary</a>
           <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
             <span class="navbar-toggler-icon"></span>
           </button>
           <div class="collapse navbar-collapse" id="navbarCollapse">
@@ -93,23 +160,19 @@
               <li class="nav-item">
                 <a class="nav-link" href="">Pabutools</a>
               </li>
               <li class="nav-item">
                 <a class="nav-link" href="">MES</a>
               </li>
             </ul>
-            <form class="form-inline mt-2 mt-md-0" data-dashlane-rid="586d21bb200ad9fc" data-form-type="">
-              <input class="form-control mr-sm-2" type="text" placeholder="Search" aria-label="Search" data-dashlane-rid="ebb02837c4029767" data-form-type="">
-              <button class="btn btn-outline-success my-2 my-sm-0" type="submit" data-dashlane-label="true" data-dashlane-rid="c66944f310795772" data-form-type="">Search</button>
-            </form>
           </div>
         </nav>
-      </header>
+    </header>
 
-      <main role="main">
+    <main role="main">
     
         <div class="container-fluid upper-page">
             <!-- General Explanations -->
             <div class="container">
                 <div class="spacer-2"></div>
                 <div class="spacer-2"></div>
 
@@ -118,165 +181,179 @@
                         <h1>
                             {{ election_name }}
                         </h1>
                         <div class="spacer-1"><hr></div>
                         <p>
                             This is the round-by-round explanations for the results of this participatory budgeting election decided by the Method of Equal Shares (MES). For each round,
                             we provide visualisations to help you understand why each particular project was selected or not. The visualisations include effective vote counts, voter flows, and pie charts.
-                            If you hover over the 'i' buttons, you will see more detailed explanations of each visualisation.
                         </p>
                     </div>
                 </div>
                 <div class="spacer-1"></div>
             </div>
         </div>
         <center>
             <div id="spinner" class="spinner-border" role="status">
                 <span class="sr-only">Loading...</span>
             </div>
         </center>
         <div class="container">
+                      
+            <div class="col-12  justify-content-center">
+                <h3>
+                    Round <span class="round_number"></span>
+                </h3>
+                <h4>
+                    Winner - <span class="project_name"></span>
+                </h4>
+                <p>
+                    <b>Description:</b> <span class="description"></span>
+                    <br>
+                    <b>Project Cost:</b> <span class="project_cost"></span> {{ currency }}
+                    <br>
+                    <b>Election Budget Remaining:</b> <span class="budget_remaining"></span> {{ currency }}
+                </p>
+               
+                
+                <p>
+              
+                    <a href="#" class="btn btn-secondary my-2" onclick="renderRoundPrev()">Previous Round</a>
+                    <a href="#" class="btn btn-primary my-2" onclick="renderRoundNext()">Next Round</a>
+
+                </p>
+            </div>
+            <div class="row my-4 justify-content-center hidden-section" id="dropdown-container">
+                <div>
+                    <h4>Select Round:  </h4>
+                </div>
+                <div class="spacer-1"></div>
+                <div class="spacer-1"></div>
+                <div class="dropdown">
+                    <button class="btn btn-primary dropdown-toggle" type="button" id="projectDropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+                    Round 1: {{ projects[rounds[0].id]['name'] }}
+                </button>
+                    <div class="dropdown-menu" aria-labelledby="projectDropdown">
+                    {% for round in rounds %}
+                        <a id="dropdown-item-{{ round.id }}" class="dropdown-item {% if loop.index == 1 %}active{% endif %}" item="{{ round.id }}" onclick="renderRound({{ round.id }}, this)">Round {{loop.index0 + 1}}: '{{ projects[round.id]['name'] }}'</a>
+                    {% endfor %}
+    
+                    </div>
+                </div>
+            </div>
+        </div>
+
+
+
+
+        <div class="container">
             <div class="spacer-1"></div>
             <hr>
             <div class="spacer-1"></div>
-            
-
             <!-- Round specific visualisations -->
-            {% for round in rounds %}
-                <section id="{{round.id}}" class="hidden-section">
+                <section>
 
                     <!-- Effective Vote Count -->
                     <div class="row featurette">
                         <div class="col-5">
                           <h2 class="featurette-heading">Effective Vote Count</h2>
-                          <p class="lead">Donec ullamcorper nulla non metus auctor fringilla. Vestibulum id ligula porta felis euismod semper. Praesent commodo cursus magna, vel scelerisque nisl consectetur. Fusce dapibus, tellus ac cursus commodo.</p>
+                          <p class="lead">'<span class="project_name"></span>' has the highest effective vote count, as there is enough budget to support this project the project will recieve funding. 
+                            This project costs <span class="project_cost"></span>.
+                            <span class="project_votes"></span> people voted for this project, at the time the project was elected it had an effective vote count of <span class="effective_vote_count"></span>.     </p>
                         </div>
                         <div class="col-7" style="min-height: 400px;">
-                            <div id="{{ round.id }}BarChart" style="height: 100%; width: 100%;">
-                                <button class = "info-button" style = "position: absolute; z-index: 2000; right: 50px;" data-tippy-content= "<b>Effective Vote Count:</b><br> For a vote to count towards a project, the person who made the vote must have some of their budget remaining so they can contribute towards the project. Say Project A has 20 voters, but 5 of those 20 have already spent their entire budget on previous projects, the effective vote count will be 15. This graph shows the effective vote counts for all projects.">i</button>
+                            <div id="BarChart" style="height: 100%; width: 100%;">
                             </div>
                         </div>
                     </div>
 
                     <div class="spacer-1"></div>
                     <hr>
                     <div class="spacer-1"></div>
 
                     <!-- Sankey and Chord side by side -->
                     <div class="row" style="display: grid;">
-                        <h5 style="text-align: center; font-weight: bold;">'{{ projects[round.id]['name'][:15] }}' Voter Flows</h5>
+                        <h5 style="text-align: center; font-weight: bold;">Voter Flows</h5>
+                        <p>The following graphs demonstrate how voters of '<span class="project_name"></span>' voted for other projects, highlighting where funding may be lost for certain projects in future rounds as voters funds have been allocated to '<span class="project_name"></span>'. </p>
                     </div>
                     <div class="row">
-                        <div class="col-5" style="display: grid;">
+                        <div class="col-5 sankey-wrapper">
                             <div class="d-flex align-items-center justify-content-center">
-                                <button class = "info-button" style = "position: absolute; z-index: 2000; left: 10px; top: 30px" data-tippy-content="<b>Sankey Diagram</b><br>The provided Sankey diagram offers a visual representation of voting patterns among a set of participants with the option to vote for multiple projects. The individual bands flowing from this singular left bar to various bars on the right-hand side illustrate the distribution of voters who have also voted for other projects. Each band's thickness corresponds to the number of voters who voted for both the project on the left and the project on the right. The graph is designed to show the overlap in voting behaviour, making it clear which projects share a common voter base with the project displayed on the right-hand side.">i</button>
-                                <div id="{{ round.id }}SankeyChart">
-
+                                <div id="SankeyChart">
                                 </div>
                             </div>
+                            <div id="textContainer" class="text-container">
+                                <p id="text" class="text">
+                                    The provided Sankey diagram offers a visual representation of voting patterns among a set of participants with the option to vote for multiple projects. The individual bands flowing from this singular left bar to various bars on the right-hand side illustrate the distribution of voters who have also voted for other projects. Each band's thickness corresponds to the number of voters who voted for both the project on the left and the project on the right. The graph is designed to show the overlap in voting behaviour, making it clear which projects share a common voter base with the project displayed on the right-hand side.
+                                </p>
+                            </div>
+                            <div class="button-container">
+                                <button id="toggleButton" onclick="toggleText()">Show More</button>
+                              </div>
                         </div>
 
                         <div class="col-2"></div>
                         <div class="col-5 chord-wrapper">
-                            <button class = "info-button" style = "position: absolute; z-index: 2000; right: 10px; top: 30px" data-tippy-content="<b>Chord Diagram:</b><br> The chord diagram shows the voter flows between the project selected this round {{ round.id }}. Due to the nature of MES, if a project is selected, the voters who voted for it will have a reduction in their budget. Therefore, showing how {{ round.id }} voters’ voted shows which other projects will have had their support cut.">i</button>
-                            <div id='{{ round.id }}ChordChart'></div>
-
+                            <div id='ChordChart'></div>
+                            <div id="textContainerChord" class="text-container">
+                                <p id="text" class="text">
+                                    The chord diagram shows the voter flows between the project selected this round. Due to the nature of MES, if a project is selected, the voters who voted for it will have a reduction in their budget. Therefore, showing how voters’ voted shows which other projects will have had their support cut.
+                                </p>
+                            </div>
+                            <div class="button-container">
+                                <button id="toggleButtonChord" onclick="toggleTextChord()">Show More</button>
+                              </div>
                         </div>
                     </div>
                     <div class="spacer-1"></div>
                     <hr>
                     <div class="spacer-1"></div>
-
+                    <div class="row" style="display: grid;">
+                        <h5 style="text-align: center; font-weight: bold;">Proportion of voters from other projects</h5>
+                        <p>The pie charts represent how voters of other projects voted for '<span class="project_name"></span>', highlighting how the average in voters budget is affected for each project. </p>
+                    </div> 
                     <!-- Pie Charts Carousels -->
-                    <div id="secondCarousel-{{round.id}}" style="height: 500px; width: 100%;" class="carousel slide" data-ride="carousel" data-interval="false">
-                        <button class = "info-button" style = "position: absolute; z-index: 2000; right: 30px; top: 30px" data-tippy-content="<b>Pie Chart:</b><br> TODO">i</button>
-                            
-                        <div class="carousel-inner" style="height: 500px; width: calc(100% - 40px);" >
-                           
-                            {% for triplet in round.pie_chart_triplet %}
-                                {% set carouselNum = loop.index %}
-                                {% set carouselClass = "carousel-item" %}
-
-                                {% if loop.first %}
-                                    {% set carouselClass = "carousel-item active" %}
-                                {% endif %}
-
-                                <div class="{{ carouselClass }}">
-                                    <div class="wrapper" style="height:300px">
-                                        <!-- <div class="d-block w-100"> -->
-                                        <div class="container"> 
-                                            <div class="row" style = "width: 100%; padding: 0px;">
-
-                                                <!-- Single Pie Chart Carousel -->
-                                                {% for data in triplet%}
-                                                    <!-- Individual Pie Chart -->
-                                                    <div class="col-sm-4" style = "margin: 0px">
-                                                        <div>
-                                                            <div id='{{ round.id }}PieChart{{ carouselNum }}-{{ loop.index }}' style="height: 100%; width: 100%;"></div>
-                                                        </div>
-                                                        <div class="spacer"></div>
-                                                        <div class="pie-chart-text">
-                                                            <!-- TODO: What does this mean??? -->
-                                                            This resulted in an average reduction of $ per voter for the '{{ projects[data.project]['name'] }}' voters who also voted for '{{ projects[round.id]['name'] }}'.
-                                                        </div>
-                                                    </div>
-                                                {% endfor %}
-                                            </div>
-                                        </div>
-                                    </div>
-                                </div>
-                            {% endfor %}
+                    <div id="secondCarousel" style="height: 500px; width: 100%;" class="carousel slide" data-ride="carousel" data-interval="false">
+                        
+                        <div id="pieChartsCarousel" class="carousel-inner" style="height: 500px; width: 100%; padding: 0px" >
                         </div>
 
-                        <a class="carousel-control-prev" href="#secondCarousel-{{round.id}}" role="button" data-slide="prev">
+                        <a class="carousel-control-prev" href="#secondCarousel" role="button" data-slide="prev">
                             <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                             <span class="sr-only">Previous</span>
                           </a>
-                          <a class="carousel-control-next" href="#secondCarousel-{{round.id}}" role="button" data-slide="next">
+                          <a class="carousel-control-next" href="#secondCarousel" role="button" data-slide="next">
                             <span class="carousel-control-next-icon" aria-hidden="true"></span>
                             <span class="sr-only">Next</span>
                           </a>
                     </div>
-                    
+
+
+
                     <div class="spacer-1"></div>
                     <hr>
                     <div class="spacer-1"></div>
 
-                    <!-- Reduced Effective Vote Count Graph (Centred Div) -->
+                    <!-- Reduced Effective Vote Count Graph -->
                     <div class="row featurette">
                         <div class="col-5">
                           <h2 class="featurette-heading">Reduced Effective Vote Count</h2>
-                          <p class="lead">Donec ullamcorper nulla non metus auctor fringilla. Vestibulum id ligula porta felis euismod semper. Praesent commodo cursus magna, vel scelerisque nisl consectetur. Fusce dapibus, tellus ac cursus commodo.</p>
+                          <p class="lead">This graph visualises the current effective vote count after some of the voters' budgets have already been allocated against original vote count for the project.</p>
                         </div>
                         <div class="col-7" style="min-height: 400px;">
-                            <div id="{{ round.id }}AfterRoundBarChart" style="height: 100%; width: 100%;" >
-                                <button class = "info-button" style = "position: absolute; z-index: 2000; right: 50px;" data-tippy-content= "<b>Reduced Effective Vote Count</b><br>Voters who still have money left but not enough money to pay for the project when its cost is equally divided will count as a fraction. We do not count voters if they have already spent their entire budget share. This graph visualises the current vote count after some of the voters' budgets have already been allocated against original vote count for the project.">i</button>
+                            <div id="StackedBarChart" style="height: 100%; width: 100%;" >
                             </div>
                         </div>
                     </div>
-                </section>
-            {% endfor %}
-            
-            <div class="spacer-8"></div>
-            <div class="spacer-8"></div>
-
-            <!-- Dropdown UI -->
-            <div class="row my-4 justify-content-center hidden-section" id="dropdown-container">
-                <div class="dropdown">
-                    <button class="btn btn-primary dropdown-toggle" type="button" id="projectDropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
-                    {{ projects[rounds[0].id]['name'] }}
-                </button>
-                    <div class="dropdown-menu" aria-labelledby="projectDropdown">
-                    {% for round in rounds %}
-                        <a id="dropdown-item-{{ round.id }}" class="dropdown-item {% if loop.index == 1 %}active{% endif %}" item="{{ round.id }}" onclick="onClickDropdown(this)">'{{ projects[round.id]['name'] }}'</a>
-                    {% endfor %}
+                    <p>
+              
+                        <a href="#" class="btn btn-secondary my-2" onclick="renderRoundPrev()">Previous Round</a>
+                        <a href="#" class="btn btn-primary my-2" onclick="renderRoundNext()">Next Round</a>
     
-                    </div>
-                </div>
-            </div>
+                    </p>
+                </section>
         </div>
 
         <div class="spacer-1"></div>
         <hr>
         <div class="spacer-1"></div>
 
         <!-- FOOTER -->
@@ -286,193 +363,278 @@
 
     </main>
     <!-- Bootstrap JS and its dependencies -->
     <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
     <script src="https://cdn.jsdelivr.net/npm/popper.js@1.14.7/dist/umd/popper.min.js"></script>
     <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"></script>
 
-    <!-- Dropdown functionality -->
+    <!-- Effective vote count bar chart -->
     <script>
-        function loadRound() {
-            const urlParams = new URLSearchParams(window.location.search);
-            projectId = urlParams.get('projectId');
-            if (projectId === null) {
-                projectId = "{{ rounds[0].id }}";
+        zingchart.render({
+            id: 'BarChart',
+            data: {
+            "type": "hbar",
+            "title": {
+                "text": "Effective Vote Count",
+            "fontSize": 16, 
+            "adjustLayout": true 
+            },
+            "plotarea": {
+            "marginLeft":'dynamic',
+            "marginRight":'dynamic'
+        },
+            "scaleX": {
+                "labels": [], 
+                    "title": {
+                    "text": "Project"
+                    },
+                    "item": { 
+                    "font-size": 14, 
+                    "offset-x": 0, 
+                    "offset-y": 0 
+                    },"zooming": true,
+                "zoomTo": [0, 10],
+                "mirrored": true,
+                "itemsOverlap": true,
+                "maxItems": 999, 
+                "label": {
+                        "angle": 45 
+                    },
+            },
+
+            "scaleY": {
+                "title": {
+                "text": "Number of Votes"
+                },
+                "items-overlap": true,
+            },
+
+            "scrollX": {
+                "bar": {
+                "backgroundColor": '#2596be',
+                "alpha": 0.5,
+                },
+                "handle": {
+                "backgroundColor": '#2596be',
+                },
+            },
+            "series": [{
+                "values": [], 
+                'hover-state': { 
+                'background-color': "orange",
             }
-            // Display the round requested
-            onClickDropdown(document.getElementById("dropdown-item-".concat(projectId)));
-            document.getElementById("spinner").style.display = "none";
-            
-            // Display the dropdown
-            document.getElementById("dropdown-container").classList.add('active');
-            document.getElementById("dropdown-container").style.display = 'flex';
-        }
+            }, ],
+            "plot": {
+            "tooltip": {
+                "text": "Project %scale-key-label has %v votes"
+            },
+                "animation": {
+                "effect": "ANIMATION_SLIDE_BOTTOM",
+                "sequence": "ANIMATION_BY_PLOT_AND_NODE",
+                "speed": 0
+                }
+            }
+        },
+        height: '100%',
+        width: '100%'
+    });
     </script>
+    <!-- Effective vote count reduction bar chart -->
     <script>
-    // Object to store rendered charts for each round
-    var renderedCharts = {};
 
-    function onClickDropdown(element) {
-        var dropdownItems = document.querySelectorAll('.dropdown-item');
-        dropdownItems.forEach(item => item.classList.remove('active'));
-        element.classList.add('active');
-        document.getElementById('projectDropdown').innerText = element.innerText;
-
-        // Show the corresponding section and hide others
-        var sections = document.querySelectorAll('section');
-        sections.forEach(section => section.style.display = 'none');
-        var selectedSection = document.getElementById(element.getAttribute("item"));
-        selectedSection.style.display = 'block';
-
-        // Check if chart has been rendered for the selected round
-        var roundId = element.getAttribute("item"); // Ensure your round button has a data-round-id attribute
-        if (!renderedCharts[roundId]) {
-            // If not, render the chart
-            renderChordChart(roundId);
-            renderedCharts[roundId] = true; // Mark this round's chart as rendered
-        } else {
-            // Optional: Handle cases where the chart is already rendered (e.g., re-render, show/hide, etc.)
-            // This part depends on how you want to handle already rendered charts.
-        }
-    }
+    zingchart.render({
+        id: 'StackedBarChart',
+        data: {
+        "type": "hbar",
+        "stacked": true,
+        "title": {
+            "text": "Reduced Effective Vote Count",
+            "fontSize": 15, 
+            "adjustLayout": true 
+        },
+        "legend": {
+            "layout": "x4",
+            "background-color": "none",
+            "shadow": 0,
+            "align": "center",
+            "adjust-layout": true,
+            "item": {
+                "font-color": "#333"
+            },
+            "marker": {
+                "type": "square",
+                "border-width": 0,
+                "size": 5
+            },
+            "toggle-action": "remove",
+            "adjust-layout": true,
+        },
+        "plotarea": {
+            "marginLeft":'dynamic',
+            "marginRight":'dynamic'
+        },
+        "plot": {
+            "tooltip": {
+                "text": "Project %scale-key-label has %v votes"
+            },
+            "animation": {
+                "effect": "ANIMATION_SLIDE_BOTTOM",
+                "sequence": 1,
+                "speed": 0
+            }
+        },
+        "scale-x": {
+            "labels": [],
+            "title": {
+                "text": "Projects"
+            },
+            "item": { 
+                    "font-size": 14, 
+                    "offset-x": 0, 
+                    "offset-y": 0 
+                },"zooming": true,
+            "zoomTo": [0, 6]
+        },
+        "scale-y": {
+            "title": {
+                "text": "Votes"
+            },
+            "min-value": 0, 
+            "max-labels": 10, 
+            "decimals": 0, 
+        },
+        "scrollX": {
+                "bar": {
+                "backgroundColor": '#2596be',
+                "alpha": 0.5,
+                },
+                "handle": {
+                "backgroundColor": '#2596be',
+                }
+            },
+
+        "series": [{
+            "values":[], 
+            "background-color": "#0070C0",
+            "text": "Current Votes",
+            'hover-state': { 
+                    'background-color': "orange",
+                }
+        }, {
+            "values": [],
+            "background-color": "#FF0000",
+            "text": "Previous Votes"
+        }]
+    },
+    height: '100%',
+    width: '100%'
+});
     </script>
+    <!-- Rounds data -->
     <script>
-        chord_chart_dictionary = {};
-        {% for round in rounds %}
-            {% set project_name = projects[round.id]['name'][:15] %}
-            {% set selected_project = round.name %}
-            {% set project_votes = round.voter_flow[selected_project] | dictsort(by='value', reverse=True) %}
-            {% set top_projects = project_votes[:6] | map(attribute=0) | list %}
-            {% if selected_project not in top_projects %}
-                {% set top_projects = [selected_project] + top_projects %}
-            {% endif %}
-
-            chord_chart_dictionary["{{round.id}}"] = [
-                {% for projFrom in top_projects %}
-                {
-                    "values":[
-                        {% for projTo in top_projects %}
-                        {{ round.voter_flow[projFrom].get(projTo, 0) }},
-                        {% endfor %}
-                        {% if projFrom == selected_project %}
-                        {{ round.voter_flow[projFrom].get(projFrom, 0) }},
-                        {% endif %}
-                    ],
-                    "text": "{{ projects[projFrom]['name'][:15]|replace('\"', '\\\"') }}"
-                },
-                {% endfor %}
-                {% if selected_project not in top_projects %}
-                // Add a series for the selected project if it's not in the top_projects list
-                {
-                    "values": [
-                        {% for projTo in top_projects %}
-                        {{ round.voter_flow[selected_project].get(projTo, 0) }},
-                        {% endfor %}
-                        {{ round.voter_flow[selected_project].get(selected_project, 0) }},
-                    ],
-                    "text": '{{ project_name }}'
-                },
-                {% endif %}
-            ]
-        {% endfor %}
+        var numProjects = {{ rounds|length }};
+        
+        var rounds_data = {
+            {% for round in rounds %}
+                "{{ round.id }}": {
+                    "effective_vote_count_bar_chart": {"x_labels": [{% for roundID in round.effective_vote_count.keys()%}'{{ projects[roundID]['name'].split()[:2] | join(" ") |replace('\"', '\\\"')|replace("\'", "\\\'") }}',{% endfor %}], "values": {{ round.effective_vote_count.values() | list }} },
+                    "effective_vote_count_stacked_bar_chart": {"x_labels": [{% for roundID in round.effective_vote_count_reduction.keys()%}'{{ projects[roundID]['name'].split()[:2] | join(" ") |replace('\"', '\\\"')|replace("\'", "\\\'") }}',{% endfor %}], "initial_values": [{% for key in round.effective_vote_count_reduction.keys() %} {{ round.effective_vote_count[key]}},{% endfor %}], "reduced_values": {{ round.effective_vote_count_reduction.values() | list }} },
+                    "pie_chart_triplets": [{% for pie_chart in round.pie_chart_triplet %}[{% for data in pie_chart%}{"project_name": "{{ projects[data.project]['name']|replace('\"', '\\\"')|replace("\'", "\\\'") }}","round_name": "{{ projects[round.id]['name']|replace('\"', '\\\"')|replace("\'", "\\\'") }}","title":  "'{{ projects[data.project]['name'].split()[:2] | join(" ") |replace('\"', '\\\"')|replace("\'", "\\\'")}}' Voters'","values_1": [{{ data.roundVoters }}],"text_1":  "'{{ projects[round.id]['name'].split()[:2] | join(" ") |replace('\"', '\\\"')|replace("\'", "\\\'") }}' Voters","values_2": [{{ data.nonRoundVoters }}] ,"text_2": "Non '{{ projects[round.id]['name'].split()[:2] | join(" ") |replace('\"', '\\\"')|replace("\'", "\\\'") }}' Voters", "reduction":{{data.reduction  | round(2) }} },{% endfor %}], {% endfor %}],
+                    "sankey_chart": {"rows": [{% set data_items = round.voter_flow[round.id].items() | sort(attribute='1', reverse=True) %}{% set top_items = data_items[:6] %}{% set other_items = data_items[6:] %}{% set other_total = other_items | map(attribute='1') | sum %}{% for key, value in top_items %}{% if key != round.id %}['{{ projects[round.id]['name'].split()[:2] | join(" ") |replace('\"', '\\\"')|replace("\'", "\\\'") }}', '{{ projects[key]['name'].split()[:2] | join(" ") |replace('\"', '\\\"')|replace("\'", "\\\'") }}', {{ value }}],{% endif %}{% endfor %}{% if other_items %}['{{ projects[round.id]['name'].split()[:2] | join(" ") |replace('\"', '\\\"')|replace("\'", "\\\'") }}', 'Other', {{ other_total }}],{% endif %}]},
+                    "chord_chart": {"series": [{% set project_name = projects[round.id]['name'].split()[:2] | join(" ")  %}{% set selected_project = round.name %}{% set project_votes = round.voter_flow[selected_project] | dictsort(by='value', reverse=True) %}{% set top_projects = project_votes[:6] | map(attribute=0) | list %}{% if selected_project not in top_projects %}    {% set top_projects = [selected_project] + top_projects %}{% endif %}{% for projFrom in top_projects %}    {        "values":[{% for projTo in top_projects %}{{ round.voter_flow[projFrom].get(projTo, 0) }},{% endfor %}{% if projFrom == selected_project %}{{ round.voter_flow[projFrom].get(projFrom, 0) }},{% endif %}],        "text": "{{ projects[projFrom]['name'].split()[:2] | join(" ") |replace('\"', '\\\"')|replace("\'", "\\\'") }}"    },{% endfor %}{% if selected_project not in top_projects %}{"values": [{% for projTo in top_projects %}{{ round.voter_flow[selected_project].get(projTo, 0) }},{% endfor %}{{ round.voter_flow[selected_project].get(selected_project, 0) }},],        "text": '{{ project_name }}'    },{% endif %}]},
+                    "intro": {"project_name": "{{ projects[round.id]['name']|replace('\"', '\\\"')|replace("\'", "\\\'") }}", "round_number": "{{loop.index0 + 1}}", "description": "{{projects[round.id]['description']|replace('\"', '\\\"')|replace("\'", "\\\'") }}", "project_cost" : "{{ "{:,}".format((projects[round.id]['cost'] | int)) }}", "budget_remaining" : "{{ "{:,}".format((round['remaining_budget'] | int)) }}", "effective_vote_count" : "{{ round['effective_vote_count'][round.id]}}", "project_votes" : "{{projects[round.id]['votes']}}" },
+                    "roundNum": {{loop.index0}},
+                },
+            {% endfor %}}
+
     </script>
     <script>
-        function renderChordChart(roundId) {
+        function updateBarChart(x_labels, values) {
+           
             zingchart.render({
-                id: roundId + 'ChordChart',
+                id: 'BarChart',
                 data: {
-                    "type": "chord",
-                    "options": {
-                        "radius": "80%"
-                    },
-                    "plotarea": {
-                        "margin": "dynamic"
-                    },
-                    "series": chord_chart_dictionary[roundId]
-                
+                "type": "hbar",
+                "title": {
+                    "text": "Effective Vote Count",
+                "fontSize": 16, // Smaller font size to ensure it fits
+                // "adjustLayout": true // ZingChart will try to adjust the layout 
                 },
-                height: "60%",
-                width: "100%",
-            });
-        }
-    </script>
-    {% for round in rounds %}
-        <!-- Effective vote count bar chart -->
-        <script>
-                //   ZC.LICENSE = ["569d52cefae586f634c54f86dc99e6a9", "b55b025e438fa8a98e32482b5f768ff5"];
-               zingchart.render({
-                  id: '{{ round.id }}BarChart',
-                  data: {
-                  "type": "hbar",
-                  "title": {
-                     "text": "Effective Vote Count (Winner: '{{ projects[round.id]['name'][:15]|replace('\"', '\\\"')}}')"
-                  },
-                  "scale-x": {
-                    "labels": [
-                        {% for roundID in round.effective_vote_count.keys()%}
-                            '{{ projects[roundID]['name'][:15]|replace('\"', '\\\"') }}',
-                        {% endfor %}
-                    ], // Label that identifies each project in the round
-                     "title": {
+                "plotarea": {
+                "marginLeft":'dynamic',
+                "marginRight":'dynamic'
+            },
+                "scaleX": {
+                    "labels": x_labels,
+                        "title": {
                         "text": "Project"
-                     },
-                     "item": { // Explicitly control the appearance of the scale labels
-                        "font-size": 14, // Adjust font size as needed
-                        "offset-x": 0, // Adjust to move the label left or right if needed
-                        "offset-y": 0 // Adjust to move the label up or down if needed
-                     }
-                  },
-                  "scale-y": {
-                     "title": {
-                        "text": "Number of Votes"
-                     },
-                     "items-overlap": true,
-                  },
-                  "series": [{
-                     "values": {{ round.effective_vote_count.values() | list }}, // Current votes values
-                     'hover-state': { /* Hover object */
-                        'background-color': "orange",
-                    }
-                  }, ],
-                  "plot": {
-                    "tooltip": {
-                        "text": "Project %scale-key-label has %v votes"
+                        },
+                        "item": { 
+                        "font-size": 14, 
+                        "offset-x": 0, 
+                        "offset-y": 0 
+                        },"zooming": true,
+                    "zoomTo": [0, 10],
+                    "mirrored": true,
+                    "itemsOverlap": true, 
+                    "maxItems": 999, 
+                    "label": {
+                            "angle": 45 
+                        },
+                },
+
+                "scaleY": {
+                    "title": {
+                    "text": "Number of Votes"
                     },
-                     "animation": {
-                        "effect": "ANIMATION_SLIDE_BOTTOM",
-                        "sequence": "ANIMATION_BY_PLOT_AND_NODE",
-                        "speed": 0
-                     }
-                  }
+                    "items-overlap": true,
                 },
-                height: '100%',
-                width: '100%'
-            });
 
-            {/* zingchart.bind('{{ round.id }}BarChart', 'shape_click', function(e) {
-                if (e.shapeid === 'custom-cm-button') {
-                    zingchart.exec('{{ round.id }}BarChart', 'showmenu', {
-                    x: 55,
-                    y: 35
-                    });
+                "scrollX": {
+                    "bar": {
+                    "backgroundColor": '#2596be',
+                    "alpha": 0.5,
+                    },
+                    "handle": {
+                    "backgroundColor": '#2596be',
+                    },
+                },
+                "series": [{
+                    "values": values, 
+                    'hover-state': { 
+                    'background-color': "orange",
                 }
-            }) */}
+                }, ],
+                "plot": {
+                "tooltip": {
+                    "text": "Project %scale-key-label has %v votes"
+                },
+                    "animation": {
+                    "effect": "ANIMATION_SLIDE_BOTTOM",
+                    "sequence": "ANIMATION_BY_PLOT_AND_NODE",
+                    "speed": 0
+                    }
+                }
+            },
+            height: '100%',
+            width: '100%'
+            });
+        }
+
+        function updateStackedBarChart(x_labels, initial_values, reduced_values) {
 
-        </script>
-        <!-- Effective vote count reduction bar chart -->
-        <script>
-            // ZC.LICENSE = ["569d52cefae586f634c54f86dc99e6a9", "b55b025e438fa8a98e32482b5f768ff5"];
             zingchart.render({
-                id: '{{round.id}}AfterRoundBarChart',
+                id: 'StackedBarChart',
                 data: {
                 "type": "hbar",
                 "stacked": true,
                 "title": {
-                    "text": "Reduced Effective Vote Count {% if loop.index in range(rounds|length) %} (Next Winner: {{ projects[rounds[loop.index].id]['name'][:15]|replace('\"', '\\\"') }}) {% endif %}",
-                    "adjust-layout": true,
+                    "text": "Reduced Effective Vote Count",
+                    "fontSize": 15, 
+                    "adjustLayout": true 
                 },
                 "legend": {
                     "layout": "x4",
                     "background-color": "none",
                     "shadow": 0,
                     "align": "center",
                     "adjust-layout": true,
@@ -483,166 +645,319 @@
                         "type": "square",
                         "border-width": 0,
                         "size": 5
                     },
                     "toggle-action": "remove",
                     "adjust-layout": true,
                 },
+                "plotarea": {
+                    "marginLeft":'dynamic',
+                    "marginRight":'dynamic'
+                },
                 "plot": {
                     "tooltip": {
                         "text": "Project %scale-key-label has %v votes"
                     },
                     "animation": {
                         "effect": "ANIMATION_SLIDE_BOTTOM",
                         "sequence": 1,
                         "speed": 0
                     }
                 },
                 "scale-x": {
-                    "labels": [
-                        {% for roundID in round.effective_vote_count_reduction.keys()%}
-                            '{{ projects[roundID]['name'][:15]|replace('\"', '\\\"') }}',
-                        {% endfor %}
-                    ], // Label that identifies each project in the round
+                    "labels": x_labels, 
                     "title": {
                         "text": "Projects"
                     },
-                    "item": { // Explicitly control the appearance of the scale labels
-                            "font-size": 14, // Adjust font size as needed
-                            "offset-x": 0, // Adjust to move the label left or right if needed
-                            "offset-y": 0 // Adjust to move the label up or down if needed
-                        }
+                    "item": { 
+                            "font-size": 14, 
+                            "offset-x": 0,
+                            "offset-y": 0 
+                        },"zooming": true,
+                    "zoomTo": [0, 6]
                 },
                 "scale-y": {
                     "title": {
                         "text": "Votes"
-                    }
+                    },
+                    "min-value": 0, 
+                    "max-labels": 10,
+                    "decimals": 0, 
                 },
+                "scrollX": {
+                        "bar": {
+                        "backgroundColor": '#2596be',
+                        "alpha": 0.5,
+                        },
+                        "handle": {
+                        "backgroundColor": '#2596be',
+                        }
+                    },
+
                 "series": [{
-                    "values":[ 
-                        {% for key in round.effective_vote_count_reduction.keys() %}
-                            {{ round.effective_vote_count[key]}},
-                        {% endfor %}
-                    ], // Effective votes for next round
+                    "values":initial_values,
                     "background-color": "#0070C0",
                     "text": "Current Votes",
-                    'hover-state': { /* Hover object */
+                    'hover-state': { 
                             'background-color': "orange",
-                            // 'border-width':3,
-                            // 'border-color': "purple",
-                            // 'line-style': "dotted"
                         }
                 }, {
-                    "values": {{ round.effective_vote_count_reduction.values() | list }}, // Effective votes lost this round
+                    "values": reduced_values,
                     "background-color": "#FF0000",
                     "text": "Previous Votes"
                 }]
             },
             height: '100%',
             width: '100%'
         });
-        </script>
+        }
 
-        <!-- Sankey diagram -->
-        <script>
-            // Render Sankey Diagrams
-            google.charts.load('current', {
-            'packages': ['sankey']
-        });
-            google.charts.setOnLoadCallback(() => {
-                    var data = new google.visualization.DataTable();
-                    data.addColumn('string', 'From');
-                    data.addColumn('string', 'To');
-                    data.addColumn('number', 'Weight');
-                    
-                    // Adding data from render.py
-
-                    {% set data_items = round.voter_flow[round.id].items() | sort(attribute='1', reverse=True) %}
-                    {% set top_items = data_items[:6] %}
-                    {% set other_items = data_items[6:] %}
-                    {% set other_total = other_items | map(attribute='1') | sum %}
-
-                    data.addRows([
-                        {% for key, value in top_items %}
-                            {% if key != round.id %}
-                                ['{{ projects[round.id]['name'][:15]|replace('\"', '\\\"') }}', '{{ projects[key]['name'][:15]|replace('\"', '\\\"') }}', {{ value }}],
-                            {% endif %}
-                        {% endfor %}
-                        {% if other_items %}
-                            ['{{ projects[round.id]['name'][:15]|replace('\"', '\\\"') }}', 'Other', {{ other_total }}],
-                        {% endif %}
-                    ])
-
-                    // Sets chart options.
-                    var options = {
-                        title: 'Project Vote Sankey Diagram',
-                        width: 445,
-                        height: 280,
-                        sankey: {}
-                    };
-
-                    // Instantiates and draws our chart, passing in some options.
-                    var chart = new google.visualization.Sankey(document.getElementById('{{round.id}}SankeyChart'));
-                    chart.draw(data, options);
+        function renderChordChart(id) {
+            zingchart.render({
+                id: "ChordChart",
+                data: {
+                    "type": "chord",
+                    "options": {
+                        "radius": "80%"
+                    },
+                    "plotarea": {
+                        "margin": "dynamic"
+                    },
+                    "series": rounds_data[id].chord_chart.series,
+                
+                },
+                height: "60%",
+                width: "100%",
             });
-        </script>
-        <!-- List of Pie Chart Carousels -->
-        {% for dataList in round.pie_chart_triplet %}
-            {% set carouselNum = loop.index %}
-
-            <!-- Pie Chart Carousel -->
-            {% for data in dataList%}
-                <!-- Pie Chart -->
-                <script>
-                    //   ZC.LICENSE = ["569d52cefae586f634c54f86dc99e6a9", "b55b025e438fa8a98e32482b5f768ff5"];
-                    var myConfig = {
-                        "type": "pie",
-                        "title": {
-                            "text": "'{{ projects[data.project]['name'][:15]|replace('\"', '\\\"')}}' Voters"
-                        },
-                        "legend": {
-                            "toggle-action": "remove",
-                            "toggle-action": "remove",
-                            "layout": "x2", // Arrange the legend items horizontally
-                            "align": "center", // Align the legend items in the center
-                            "vertical-align": "bottom",
-                        },
-                        "plot": {
-                            "valueBox": {
-                                "visible": true, // Make value labels visible
-                                "type": 'all', // Show all value text including percentages and absolute values
-                                "placement": 'in', // Position the valueBox outside of the slice
-                                "text": "%v", // Display the absolute value
-                                "fontSize": 10 // Adjust font size as needed
-                            },
-                            "animation": {
-                                "effect": "ANIMATION_EXPAND_VERTICAL",
-                                "sequence": "ANIMATION_BY_PLOT",
-                                "speed": 0
-                            }
-                        },
-                        "series": [{
-                            "values": [{{ data.roundVoters }}],
-                            "text": "'{{ projects[round.id]['name'][:15]|replace('\"', '\\\"') }}' Voters",
-                        }, {
-                            "values": [{{ data.nonRoundVoters }}],
-                            "text": "Non '{{ projects[round.id]['name'][:15]|replace('\"', '\\\"') }}' Voters",
-                        }]
-                    };
-
-                    zingchart.render({
-                        id: '{{ round.id }}PieChart{{ carouselNum }}-{{ loop.index }}',
-                        data: myConfig,
-                        height: 300,
-                        width: "100%"
-                    });
-                </script>
-            {% endfor %}
-        {% endfor %}
-    {% endfor %}
+        }
+
+        function updateSankeyChart(rows) {
+            let chart = new google.visualization.Sankey(document.getElementById('SankeyChart'));
+            let options = {
+                title: 'Project Vote Sankey Diagram',
+                width: 445,
+                height: 280,
+                sankey: {}
+            };
+            let data = new google.visualization.DataTable();
+            data.addColumn('string', 'From');
+            data.addColumn('string', 'To');
+            data.addColumn('number', 'Weight');
+            data.addRows(rows);
+            // Instantiates and draws our chart, passing in some options.
+            chart.draw(data, options);
+        }
+
+        function updateIntro(project) {
+
+            var elements = document.getElementsByClassName("project_name");
+            for (var i = 0; i < elements.length; i++) {
+                elements[i].innerHTML = project.project_name;
+            }
+            var elements = document.getElementsByClassName("round_number");
+            for (var i = 0; i < elements.length; i++) {
+                elements[i].innerHTML = project.round_number;
+            }
+            var elements = document.getElementsByClassName("description");
+            for (var i = 0; i < elements.length; i++) {
+                elements[i].innerHTML = project.description;
+            }
+            var elements = document.getElementsByClassName("project_cost");
+            for (var i = 0; i < elements.length; i++) {
+                elements[i].innerHTML = project.project_cost;
+            }
+            var elements = document.getElementsByClassName("budget_remaining");
+            for (var i = 0; i < elements.length; i++) {
+                elements[i].innerHTML = project.budget_remaining;
+            }
+        
+            var elements = document.getElementsByClassName("effective_vote_count");
+            for (var i = 0; i < elements.length; i++) {
+                elements[i].innerHTML = project.effective_vote_count;
+            }
+            var elements = document.getElementsByClassName("project_votes");
+            for (var i = 0; i < elements.length; i++) {
+                elements[i].innerHTML = project.project_votes;
+            }
+        }
+           
+
+        function renderPieChart(id, title, values_1, text_1, values_2, text_2) {
+            let args = {
+                "type":"pie",
+                "title":{
+                    "text": title
+                },
+                "legend":{
+                    "toggle-action":"remove",
+                    "toggle-action":"remove",
+                    // "layout":"x2",
+                    "align":"center",
+                    "vertical-align":"bottom"
+                },
+                "plot":{
+                    "valueBox":{
+                        "visible":true,
+                        "type":"all",
+                        "placement":"in",
+                        "text":"%v",
+                        "fontSize":10 // Adjust font size as needed
+                    },
+                    "animation":{
+                        "effect":"ANIMATION_EXPAND_VERTICAL",
+                        "sequence":"ANIMATION_BY_PLOT",
+                        "speed":0
+                    }
+                },
+                "series":[
+                    {
+                        "values": values_1,
+                        "text": text_1
+                    },
+                    {
+                        "values": values_2,
+                        "text": text_2
+                    }
+                ]
+            };
+            zingchart.render({
+                id: id,
+                data: args,
+                height: 300,
+                width: "100%"
+            });
+        }
+
+        async function addPieChartsToCarousel(pie_chart_triplets, project_name) {
+            pie_chart_data_for_render = [];
+            let carouselElement = document.getElementById("pieChartsCarousel");
+            carouselElement.innerHTML = "";
+            let carouselNum = 0;
+            pie_chart_triplets.forEach(triplet => {
+                let carouselClass = "carousel-item";
+                if (carouselNum === 0) {
+                    carouselClass = "carousel-item active";
+                }
+                let carouselItem = document.createElement("div");
+                carouselItem.className = carouselClass;
+                let wrapper = document.createElement("div");
+                wrapper.className = "wrapper";
+                let container = document.createElement("div");
+                container.className = "container";
+                let row = document.createElement("div");
+                row.className = "row";
+                triplet.forEach(data => {
+                    let col = document.createElement("div");
+                    col.className = "col-sm-4";
+                    let div = document.createElement("div");
+                    let pieChart = document.createElement("div");
+                    pieChart.id = "PieChart" + carouselNum + "-" + triplet.indexOf(data);
+                    pieChart.style.height = "100%";
+                    pieChart.style.width = "100%";
+                    div.appendChild(pieChart);
+                    pie_chart_data_for_render.push([pieChart.id, data.title, data.values_1, data.text_1, data.values_2, data.text_2])
+                    // renderPieChart(pieChart.id, data.title, data.values_1, data.text_1, data.values_2, data.text_2);
+                    col.appendChild(div);
+                    let pieChartText = document.createElement("div");
+                    pieChartText.className = "pie-chart-text";
+                    pieChartText.innerHTML = data.values_1 + " out of the " + (+data.values_1 + +data.values_2) + " voters who voted for '" + data.project_name + "' also voted for " + project_name + ". Resulting in an average reduction of $ per voter for the '" + data.project_name + "' voters who also voted for '" + data.round_name + "'.";
+                    col.appendChild(pieChartText);
+                    row.appendChild(col);
+                });
+                container.appendChild(row);
+                wrapper.appendChild(container);
+                carouselItem.appendChild(wrapper);
+                carouselElement.appendChild(carouselItem);
+                carouselNum++;
+            });
+            return pie_chart_data_for_render;
+        }
+
+        async function renderRound(roundId) {
+            let element = document.getElementById("dropdown-item-".concat(roundId));
+            var dropdownItems = document.querySelectorAll('.dropdown-item');
+            dropdownItems.forEach(item => item.classList.remove('active'));
+            element.classList.add('active');
+            document.getElementById('projectDropdown').innerText = element.innerText;
+            let round_data = rounds_data[roundId];
+        
+            roundNum = round_data.roundNum
+            pie_chart_data_for_render = await addPieChartsToCarousel(round_data.pie_chart_triplets, round_data.intro.project_name);
+            updateBarChart(round_data.effective_vote_count_bar_chart.x_labels, round_data.effective_vote_count_bar_chart.values);
+            updateStackedBarChart(round_data.effective_vote_count_stacked_bar_chart.x_labels, round_data.effective_vote_count_stacked_bar_chart.initial_values, round_data.effective_vote_count_stacked_bar_chart.reduced_values);
+            updateSankeyChart(round_data.sankey_chart.rows);
+            updateIntro(round_data.intro);
+            pie_chart_data_for_render.forEach(data => {
+                renderPieChart(data[0], data[1], data[2], data[3], data[4], data[5]);
+            });
+        }
+
+        async function renderRoundNext() {
+            const nextRound = document.querySelector('.dropdown-item.active').nextElementSibling;
+            if (nextRound) {
+                renderRound(nextRound.getAttribute('item'));
+            }
+        }
 
+        async function renderRoundPrev() {
+            const prevRound = document.querySelector('.dropdown-item.active').previousElementSibling;
+            if (prevRound) {
+                renderRound(prevRound.getAttribute('item'));
+            }
+        }
+    </script>
+    <script>
+        async function loadRound() {
+            roundNum = 0
+            const urlParams = new URLSearchParams(window.location.search);
+            projectId = urlParams.get('projectId');
+            if (projectId === null) {
+                projectId = "{{ rounds[0].id }}";
+            }
+            await google.charts.load('current', {
+                'packages': ['sankey']
+            });
+            // Display the round requested
+            renderRound(projectId);
+            renderChordChart(projectId);
+            document.getElementById("spinner").style.display = "none";
+            // Display the dropdown
+            document.getElementById("dropdown-container").classList.add('active');
+            document.getElementById("dropdown-container").style.display = 'flex';
+        }
+
+        function toggleText() {
+            var container = document.getElementById("textContainer");
+            var button = document.getElementById("toggleButton");
+
+            if (container.classList.contains("text-expanded")) {
+                // If the text is expanded, collapse it
+                container.classList.remove("text-expanded");
+                button.innerHTML = "Show More";
+            } else {
+                // If the text is collapsed, expand it
+                container.classList.add("text-expanded");
+                button.innerHTML = "Show Less";
+            }
+        }
+
+        function toggleTextChord() {
+            var container = document.getElementById("textContainerChord");
+            var button = document.getElementById("toggleButtonChord");
+
+            if (container.classList.contains("text-expanded")) {
+                // If the text is expanded, collapse it
+                container.classList.remove("text-expanded");
+                button.innerHTML = "Show More";
+            } else {
+                // If the text is collapsed, expand it
+                container.classList.add("text-expanded");
+                button.innerHTML = "Show Less";
+            }
+        }
+    </script>
     <script src="https://unpkg.com/@popperjs/core@2"></script>
     <script src="https://unpkg.com/tippy.js@6"></script>
     <script>tippy('[data-tippy-content]', { allowHTML: true, maxWidth: 1000});</script>
     <script type="text/javascript" src="https://unpkg.com/default-passive-events"></script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,52 +1,61 @@
 _S_u_m_m_a_r_y
     * _R_o_u_n_d_ _B_y_ _R_o_u_n_d_ _(_c_u_r_r_e_n_t_)
     * Pabutools
     * MES
-[                    ]Search
 ************ {{{{ eelleeccttiioonn__nnaammee }}}} ************
 ===============================================================================
 This is the round-by-round explanations for the results of this participatory
 budgeting election decided by the Method of Equal Shares (MES). For each round,
 we provide visualisations to help you understand why each particular project
 was selected or not. The visualisations include effective vote counts, voter
-flows, and pie charts. If you hover over the 'i' buttons, you will see more
-detailed explanations of each visualisation.
+flows, and pie charts.
                                   Loading...
+******** RRoouunndd ********
+****** WWiinnnneerr -- ******
+DDeessccrriippttiioonn::
+PPrroojjeecctt CCoosstt:: {{ currency }}
+EElleeccttiioonn BBuuddggeett RReemmaaiinniinngg:: {{ currency }}
+_P_r_e_v_i_o_u_s_ _R_o_u_n_d _N_e_x_t_ _R_o_u_n_d
+****** SSeelleecctt RRoouunndd:: ******
+Round 1: {{ projects[rounds[0].id]['name'] }}
+{% for round in rounds %} Round {{loop.index0 + 1}}: '{{ projects[round.id]
+['name'] }}' {% endfor %}
 ===============================================================================
-{% for round in rounds %}
 ********** EEffffeeccttiivvee VVoottee CCoouunntt **********
-Donec ullamcorper nulla non metus auctor fringilla. Vestibulum id ligula porta
-felis euismod semper. Praesent commodo cursus magna, vel scelerisque nisl
-consectetur. Fusce dapibus, tellus ac cursus commodo.
-i
-===============================================================================
-**** ''{{{{ pprroojjeeccttss[[rroouunndd..iidd]][[''nnaammee'']][[::1155]] }}}}'' VVootteerr FFlloowwss ****
-i
-i
-===============================================================================
-i
-{% for triplet in round.pie_chart_triplet %} {% set carouselNum = loop.index %}
-{% set carouselClass = "carousel-item" %} {% if loop.first %} {% set
-carouselClass = "carousel-item active" %} {% endif %}
-{% for data in triplet%}
-This resulted in an average reduction of $ per voter for the '{{ projects
-[data.project]['name'] }}' voters who also voted for '{{ projects[round.id]
-['name'] }}'.
-{% endfor %}
-{% endfor %}
+'' has the highest effective vote count, as there is enough budget to support
+this project the project will recieve funding. This project costs . people
+voted for this project, at the time the project was elected it had an effective
+vote count of .
+===============================================================================
+**** VVootteerr FFlloowwss ****
+The following graphs demonstrate how voters of '' voted for other projects,
+highlighting where funding may be lost for certain projects in future rounds as
+voters funds have been allocated to ''.
+The provided Sankey diagram offers a visual representation of voting patterns
+among a set of participants with the option to vote for multiple projects. The
+individual bands flowing from this singular left bar to various bars on the
+right-hand side illustrate the distribution of voters who have also voted for
+other projects. Each band's thickness corresponds to the number of voters who
+voted for both the project on the left and the project on the right. The graph
+is designed to show the overlap in voting behaviour, making it clear which
+projects share a common voter base with the project displayed on the right-hand
+side.
+Show More
+The chord diagram shows the voter flows between the project selected this
+round. Due to the nature of MES, if a project is selected, the voters who voted
+for it will have a reduction in their budget. Therefore, showing how voters’
+voted shows which other projects will have had their support cut.
+Show More
+===============================================================================
+**** PPrrooppoorrttiioonn ooff vvootteerrss ffrroomm ootthheerr pprroojjeeccttss ****
+The pie charts represent how voters of other projects voted for '',
+highlighting how the average in voters budget is affected for each project.
 _P_r_e_v_i_o_u_s_ _N_e_x_t
 ===============================================================================
 ********** RReedduucceedd EEffffeeccttiivvee VVoottee CCoouunntt **********
-Donec ullamcorper nulla non metus auctor fringilla. Vestibulum id ligula porta
-felis euismod semper. Praesent commodo cursus magna, vel scelerisque nisl
-consectetur. Fusce dapibus, tellus ac cursus commodo.
-i
-{% endfor %}
-{{ projects[rounds[0].id]['name'] }}
-{% for round in rounds %} '{{ projects[round.id]['name'] }}' {% endfor %}
+This graph visualises the current effective vote count after some of the
+voters' budgets have already been allocated against original vote count for the
+project.
+_P_r_e_v_i_o_u_s_ _R_o_u_n_d _N_e_x_t_ _R_o_u_n_d
 ===============================================================================
 © Pabutools. · _P_r_i_v_a_c_y · _T_e_r_m_s
-{% for round in rounds %}
-{% for dataList in round.pie_chart_triplet %} {% set carouselNum = loop.index
-%} {% for data in dataList%}
-{% endfor %} {% endfor %} {% endfor %}
```

### Comparing `pabutools-1.1.6/pyproject.toml` & `pabutools-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pabutools"
-version = "1.1.6"
+version = "1.1.7"
 description = "Implementation of all the tools necessary to explore and analyse participatory budgeting elections"
 authors = [
   { name = "Simon Rey", email = "reysimon@orange.fr" },
   { name = "Grzegorz Pierczyński", email = "g.pierczynski@mimuw.edu.pl" },
   { name = "Markus Utke", email = "markusutke@gmx.de" },
   { name = "Piotr Skowron", email = "p.skowron@mimuw.edu.pl" },
 ]
```

### Comparing `pabutools-1.1.6/PKG-INFO` & `pabutools-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pabutools
-Version: 1.1.6
+Version: 1.1.7
 Summary: Implementation of all the tools necessary to explore and analyse participatory budgeting elections
 Author-email: Simon Rey <reysimon@orange.fr>, Grzegorz Pierczyński <g.pierczynski@mimuw.edu.pl>, Markus Utke <markusutke@gmx.de>, Piotr Skowron <p.skowron@mimuw.edu.pl>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

