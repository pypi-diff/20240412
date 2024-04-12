# Comparing `tmp/gctree-4.2.0.tar.gz` & `tmp/gctree-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gctree-4.2.0.tar", last modified: Mon Apr  8 20:11:12 2024, max compression
+gzip compressed data, was "gctree-4.2.1.tar", last modified: Fri Apr 12 02:58:59 2024, max compression
```

## Comparing `gctree-4.2.0.tar` & `gctree-4.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:11:12.132504 gctree-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-08 20:11:05.000000 gctree-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 20:11:05.000000 gctree-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-08 20:11:12.132504 gctree-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 20:11:05.000000 gctree-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:11:12.128504 gctree-4.2.0/gctree/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 20:11:12.132504 gctree-4.2.0/gctree/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    85481 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/branching_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26814 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7708 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/isotype.py
--rw-r--r--   0 runner    (1001) docker     (127)    20763 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/isotyping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2371 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/mkconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/mutation_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/phylip_parse.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1159 2024-04-08 20:11:05.000000 gctree-4.2.0/gctree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:11:12.132504 gctree-4.2.0/gctree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 20:11:12.000000 gctree-4.2.0/gctree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 20:11:12.132504 gctree-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-08 20:11:05.000000 gctree-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:11:12.132504 gctree-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-08 20:11:05.000000 gctree-4.2.0/tests/test_disambiguate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-08 20:11:05.000000 gctree-4.2.0/tests/test_isotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-08 20:11:05.000000 gctree-4.2.0/tests/test_likelihoods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-08 20:11:05.000000 gctree-4.2.0/tests/test_local_branching.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-08 20:11:05.000000 gctree-4.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:58:59.064236 gctree-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-12 02:58:50.000000 gctree-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 02:58:50.000000 gctree-4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-12 02:58:59.064236 gctree-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 02:58:50.000000 gctree-4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:58:59.064236 gctree-4.2.1/gctree/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 02:58:59.064236 gctree-4.2.1/gctree/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86336 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/branching_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26814 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7708 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/isotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20763 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/isotyping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2371 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/mkconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/mutation_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/phylip_parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1159 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:58:59.064236 gctree-4.2.1/gctree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 02:58:59.064236 gctree-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-12 02:58:50.000000 gctree-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:58:59.064236 gctree-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-12 02:58:50.000000 gctree-4.2.1/tests/test_disambiguate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-12 02:58:50.000000 gctree-4.2.1/tests/test_isotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-12 02:58:50.000000 gctree-4.2.1/tests/test_likelihoods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-12 02:58:50.000000 gctree-4.2.1/tests/test_local_branching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-12 02:58:50.000000 gctree-4.2.1/versioneer.py
```

### Comparing `gctree-4.2.0/LICENSE` & `gctree-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/PKG-INFO` & `gctree-4.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gctree
-Version: 4.2.0
+Version: 4.2.1
 Summary: phylogenetic inference of genotype-collapsed trees
 Home-page: https://github.com/matsengrp/gctree
 Author: Matsen Group
 Author-email: ematsen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `gctree-4.2.0/README.md` & `gctree-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/gctree/branching_processes.py` & `gctree-4.2.1/gctree/branching_processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1200,15 +1200,15 @@
         else:
             coeffs = [1] * 4
 
         (
             nz_coeff_bplikelihood,
             nz_coeff_isotype_pars,
             nz_coeff_context,
-            nz_coeff_alleles,
+            _,
         ) = [val != 0 for val in coeffs]
         coeff_bplikelihood, coeff_isotype_pars, coeff_context, coeff_alleles = coeffs
 
         dag_filters = []
         if nz_coeff_bplikelihood:
             if self.parameters is None:
                 self.mle(marginal=True)
@@ -1241,21 +1241,41 @@
             else:
                 mut_funcs = _context_poisson_likelihood_dagfuncs(
                     mutability_file=mutability_file,
                     substitution_file=substitution_file,
                     splits=[] if chain_split is None else [chain_split],
                 )
             dag_filters.append((mut_funcs, coeff_context))
-        if nz_coeff_alleles:
-            allele_funcs = _allele_dagfuncs()
-            dag_filters.append((allele_funcs, coeff_alleles))
+
+        # add allele funcs no matter what, for logging
+        allele_funcs = _allele_dagfuncs()
+        dag_filters.append((allele_funcs, coeff_alleles))
+        # add 0-returning functions so dagfuncs return tuples, even if allele funcs are the only ones used for filtering
+        dag_filters.append(
+            (
+                hdag.utils.HistoryDagFilter(
+                    hdag.utils.AddFuncDict(
+                        {
+                            "start_func": lambda n: 0,
+                            "edge_weight_func": lambda n1, n2: 0,
+                            "accum_func": lambda ls: 0,
+                        },
+                        name="",
+                    ),
+                    min,
+                    ordering_name="",
+                ),
+                0,
+            )
+        )
 
         combined_dag_filter = functools.reduce(
             lambda x, y: x + y, (dag_filter for dag_filter, _ in dag_filters)
         )
+
         if ranking_coeffs:
             if len(ranking_coeffs) != 3:
                 raise ValueError(
                     "If ranking_coeffs are provided to `filter_trees` method, a list of three values is expected."
                 )
             for dag_filter, coeff in dag_filters:
                 if dag_filter.optimal_func == max and coeff > 0:
@@ -1294,24 +1314,26 @@
                 ordering_name="LinearCombination",
             )
             ranking_description = (
                 "Ranking trees to minimize a linear combination of "
                 + " + ".join(
                     str(coeff) + "(" + fl.weight_funcs.name + ")"
                     for fl, coeff in dag_filters
+                    if coeff != 0
                 )
             )
         else:
             ranking_dag_filter = combined_dag_filter
             ranking_description = "Ranking trees to " + " then ".join(
                 opt_name[:3] + "imize " + ord_name
                 for (opt_name, _), ord_name in zip(
                     ranking_dag_filter.ordering_names,
                     ranking_dag_filter.weight_funcs.names,
                 )
+                if ord_name != ""
             )
         if verbose:
             print(ranking_description)
 
         def print_stats(statlist, title, file=None, suppress_score=False):
             show_score = ranking_coeffs and not suppress_score
 
@@ -1320,24 +1342,25 @@
                     return format(field, "<" + str(n))
                 else:
                     return f"{field:{n}.{n}}"
 
             print("\n" + title + ":", file=file)
             statstring = "\t".join(
                 tuple(
-                    reformat(dfilter.weight_funcs.name, n=14)
-                    for dfilter, _ in dag_filters
+                    reformat(dfilter.weight_funcs.name, n=15)
+                    for dfilter, _ in dag_filters[:-1]
                 )
             )
             print(
                 f"tree     \t{statstring}" + ("\ttreescore" if show_score else ""),
                 file=file,
             )
             for j, best_weighttuple in enumerate(statlist, 1):
-                statstring = "\t".join(reformat(it) for it in best_weighttuple)
+                # ignore always-0 entry at end:
+                statstring = "\t".join(reformat(it) for it in best_weighttuple[:-1])
                 print(
                     f"{j:<10}\t{statstring}"
                     + (
                         f"\t{reformat(linear_combinator(best_weighttuple))}"
                         if show_score
                         else ""
                     ),
@@ -1392,24 +1415,26 @@
             dag.optimal_weight_annotate(edge_weight_func=lambda n1, n2: 0)
             if ranking_coeffs:
                 minfunckey = linear_combinator
             else:
                 minfunckey = ranking_dag_filter.optimal_func
             dag_ls.sort(key=minfunckey)
 
-            df = pd.DataFrame(dag_ls, columns=combined_dag_filter.weight_funcs.names)
+            df = pd.DataFrame(
+                dag_ls, columns=combined_dag_filter.weight_funcs.names
+            ).drop(columns=[""])
             df.to_csv(outbase + ".tree_stats.csv")
             df["set"] = ["all_trees"] * len(df)
             bestdf = pd.DataFrame(
                 [best_weighttuple], columns=combined_dag_filter.weight_funcs.names
             )
             bestdf["set"] = ["best_tree"]
             toplot_df = pd.concat([df, bestdf], ignore_index=True)
             pplot = sns.pairplot(
-                toplot_df.drop(["Alleles"], errors="ignore"),
+                toplot_df.drop(columns=["Alleles", ""], errors="ignore"),
                 hue="set",
                 diag_kind="hist",
             )
             pplot.savefig(outbase + ".tree_stats.pairplot.pdf")
 
         return (self._trimmed_self(trimdag), best_weighttuple)
```

### Comparing `gctree-4.2.0/gctree/cli.py` & `gctree-4.2.1/gctree/cli.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/gctree/deduplicate.py` & `gctree-4.2.1/gctree/deduplicate.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/gctree/isotype.py` & `gctree-4.2.1/gctree/isotype.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/gctree/isotyping.py` & `gctree-4.2.1/gctree/isotyping.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/gctree/mkconfig.py` & `gctree-4.2.1/gctree/mkconfig.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/gctree/mutation_model.py` & `gctree-4.2.1/gctree/mutation_model.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/gctree/phylip_parse.py` & `gctree-4.2.1/gctree/phylip_parse.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/gctree/utils.py` & `gctree-4.2.1/gctree/utils.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/gctree.egg-info/PKG-INFO` & `gctree-4.2.1/gctree.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gctree
-Version: 4.2.0
+Version: 4.2.1
 Summary: phylogenetic inference of genotype-collapsed trees
 Home-page: https://github.com/matsengrp/gctree
 Author: Matsen Group
 Author-email: ematsen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `gctree-4.2.0/gctree.egg-info/SOURCES.txt` & `gctree-4.2.1/gctree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/setup.py` & `gctree-4.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/tests/test_disambiguate.py` & `gctree-4.2.1/tests/test_disambiguate.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/tests/test_isotype.py` & `gctree-4.2.1/tests/test_isotype.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/tests/test_likelihoods.py` & `gctree-4.2.1/tests/test_likelihoods.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/tests/test_local_branching.py` & `gctree-4.2.1/tests/test_local_branching.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.0/versioneer.py` & `gctree-4.2.1/versioneer.py`

 * *Files identical despite different names*

