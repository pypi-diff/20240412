# Comparing `tmp/plot_phylo-0.1.7.tar.gz` & `tmp/plot_phylo-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot_phylo-0.1.7.tar", last modified: Fri Apr 12 12:02:18 2024, max compression
+gzip compressed data, was "plot_phylo-0.1.8.tar", last modified: Fri Apr 12 13:16:46 2024, max compression
```

## Comparing `plot_phylo-0.1.7.tar` & `plot_phylo-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 katy      (1001) katy      (1001)        0 2024-04-12 12:02:18.910685 plot_phylo-0.1.7/
--rw-rw-r--   0 katy      (1001) katy      (1001)     1086 2024-01-12 19:51:01.000000 plot_phylo-0.1.7/LICENSE
--rw-rw-r--   0 katy      (1001) katy      (1001)     1425 2024-04-12 12:02:18.910685 plot_phylo-0.1.7/PKG-INFO
--rw-rw-r--   0 katy      (1001) katy      (1001)      987 2024-04-12 12:00:46.000000 plot_phylo-0.1.7/README.md
-drwxrwxr-x   0 katy      (1001) katy      (1001)        0 2024-04-12 12:02:18.910685 plot_phylo-0.1.7/plot_phylo/
--rw-rw-r--   0 katy      (1001) katy      (1001)       77 2024-04-12 11:57:36.000000 plot_phylo-0.1.7/plot_phylo/__init__.py
--rw-rw-r--   0 katy      (1001) katy      (1001)       22 2024-04-12 11:52:59.000000 plot_phylo-0.1.7/plot_phylo/_version.py
--rwxrwxr-x   0 katy      (1001) katy      (1001)    21600 2024-04-12 11:49:37.000000 plot_phylo-0.1.7/plot_phylo/plot_phylo.py
-drwxrwxr-x   0 katy      (1001) katy      (1001)        0 2024-04-12 12:02:18.910685 plot_phylo-0.1.7/plot_phylo.egg-info/
--rw-r--r--   0 katy      (1001) katy      (1001)     1425 2024-04-12 12:02:18.000000 plot_phylo-0.1.7/plot_phylo.egg-info/PKG-INFO
--rw-rw-r--   0 katy      (1001) katy      (1001)      375 2024-04-12 12:02:18.000000 plot_phylo-0.1.7/plot_phylo.egg-info/SOURCES.txt
--rw-rw-r--   0 katy      (1001) katy      (1001)        1 2024-04-12 12:02:18.000000 plot_phylo-0.1.7/plot_phylo.egg-info/dependency_links.txt
--rw-rw-r--   0 katy      (1001) katy      (1001)       16 2024-04-12 12:02:18.000000 plot_phylo-0.1.7/plot_phylo.egg-info/requires.txt
--rw-rw-r--   0 katy      (1001) katy      (1001)       11 2024-04-12 12:02:18.000000 plot_phylo-0.1.7/plot_phylo.egg-info/top_level.txt
--rw-rw-r--   0 katy      (1001) katy      (1001)      103 2024-01-15 12:08:14.000000 plot_phylo-0.1.7/pyproject.toml
--rw-rw-r--   0 katy      (1001) katy      (1001)       74 2024-04-12 12:02:18.910685 plot_phylo-0.1.7/setup.cfg
--rw-rw-r--   0 katy      (1001) katy      (1001)     1106 2024-01-15 10:33:04.000000 plot_phylo-0.1.7/setup.py
-drwxrwxr-x   0 katy      (1001) katy      (1001)        0 2024-04-12 12:02:18.910685 plot_phylo-0.1.7/tests/
--rw-rw-r--   0 katy      (1001) katy      (1001)     2734 2024-02-22 10:35:13.000000 plot_phylo-0.1.7/tests/test_get_boxes_data.py
--rw-rw-r--   0 katy      (1001) katy      (1001)    12460 2024-02-22 11:15:31.000000 plot_phylo-0.1.7/tests/test_plot_phylo.py
--rw-rw-r--   0 katy      (1001) katy      (1001)     5063 2024-02-22 10:35:58.000000 plot_phylo-0.1.7/tests/test_plot_phylo_data.py
+drwxrwxr-x   0 katy      (1001) katy      (1001)        0 2024-04-12 13:16:46.875406 plot_phylo-0.1.8/
+-rw-rw-r--   0 katy      (1001) katy      (1001)     1086 2024-01-12 19:51:01.000000 plot_phylo-0.1.8/LICENSE
+-rw-rw-r--   0 katy      (1001) katy      (1001)     1425 2024-04-12 13:16:46.875406 plot_phylo-0.1.8/PKG-INFO
+-rw-rw-r--   0 katy      (1001) katy      (1001)      987 2024-04-12 12:00:46.000000 plot_phylo-0.1.8/README.md
+drwxrwxr-x   0 katy      (1001) katy      (1001)        0 2024-04-12 13:16:46.871406 plot_phylo-0.1.8/plot_phylo/
+-rw-rw-r--   0 katy      (1001) katy      (1001)       77 2024-04-12 12:07:27.000000 plot_phylo-0.1.8/plot_phylo/__init__.py
+-rw-rw-r--   0 katy      (1001) katy      (1001)       22 2024-04-12 12:04:52.000000 plot_phylo-0.1.8/plot_phylo/_version.py
+-rwxrwxr-x   0 katy      (1001) katy      (1001)    20941 2024-04-12 12:04:12.000000 plot_phylo-0.1.8/plot_phylo/plot_phylo.py
+drwxrwxr-x   0 katy      (1001) katy      (1001)        0 2024-04-12 13:16:46.871406 plot_phylo-0.1.8/plot_phylo.egg-info/
+-rw-rw-r--   0 katy      (1001) katy      (1001)     1425 2024-04-12 13:16:46.000000 plot_phylo-0.1.8/plot_phylo.egg-info/PKG-INFO
+-rw-rw-r--   0 katy      (1001) katy      (1001)      375 2024-04-12 13:16:46.000000 plot_phylo-0.1.8/plot_phylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 katy      (1001) katy      (1001)        1 2024-04-12 13:16:46.000000 plot_phylo-0.1.8/plot_phylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 katy      (1001) katy      (1001)       16 2024-04-12 13:16:46.000000 plot_phylo-0.1.8/plot_phylo.egg-info/requires.txt
+-rw-rw-r--   0 katy      (1001) katy      (1001)       11 2024-04-12 13:16:46.000000 plot_phylo-0.1.8/plot_phylo.egg-info/top_level.txt
+-rw-rw-r--   0 katy      (1001) katy      (1001)      103 2024-01-15 12:08:14.000000 plot_phylo-0.1.8/pyproject.toml
+-rw-rw-r--   0 katy      (1001) katy      (1001)       74 2024-04-12 13:16:46.875406 plot_phylo-0.1.8/setup.cfg
+-rw-rw-r--   0 katy      (1001) katy      (1001)     1106 2024-01-15 10:33:04.000000 plot_phylo-0.1.8/setup.py
+drwxrwxr-x   0 katy      (1001) katy      (1001)        0 2024-04-12 13:16:46.875406 plot_phylo-0.1.8/tests/
+-rw-rw-r--   0 katy      (1001) katy      (1001)     2734 2024-02-22 10:35:13.000000 plot_phylo-0.1.8/tests/test_get_boxes_data.py
+-rw-rw-r--   0 katy      (1001) katy      (1001)    12460 2024-02-22 11:15:31.000000 plot_phylo-0.1.8/tests/test_plot_phylo.py
+-rw-rw-r--   0 katy      (1001) katy      (1001)     5063 2024-02-22 10:35:58.000000 plot_phylo-0.1.8/tests/test_plot_phylo_data.py
```

### Comparing `plot_phylo-0.1.7/LICENSE` & `plot_phylo-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `plot_phylo-0.1.7/PKG-INFO` & `plot_phylo-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot_phylo
-Version: 0.1.7
+Version: 0.1.8
 Summary: Module to draw a phylogenetic tree using matplotlib
 Home-page: https://github.com/KatyBrown/plot_phylo
 Author: Katy Brown, Duncan Cross
 Author-email: kab84@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plot_phylo-0.1.7/README.md` & `plot_phylo-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `plot_phylo-0.1.7/plot_phylo/plot_phylo.py` & `plot_phylo-0.1.8/plot_phylo/plot_phylo.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 def plot_phylo(tree, ax,
                xpos=0,
                ypos=0,
                width=10,
                height=10,
                show_axis=False,
                show_support=True,
-               show_node_labels=False,
                align_tips=False,
                rev_align_tips=False,
                branch_lengths=True,
                scale_bar=True,
                scale_bar_width=None,
                reverse=False,
                outgroup=None,
@@ -118,15 +117,14 @@
     # Dictionary to pass apperance params to the plotting function
     appearance = {'font_size': font_size,
                   'line_col': line_col,
                   'line_width': line_width,
                   'col_dict': col_dict,
                   'label_dict': label_dict,
                   'show_support': show_support,
-                  'show_node_labels': show_node_labels,
                   'bold': bold}
 
     # Calculate the total height and width of the original tree
     # in terms of number of nodes, total branch length, number of tips
     maxdist = ((T.get_farthest_leaf(topology_only=True)[1],
                 T.get_farthest_leaf(topology_only=False)[1],
                 len(T)))
@@ -427,33 +425,21 @@
             ax.plot([x, x+(td*xint)], [-ym, -ym],
                     color=appearance['line_col'],
                     lw=appearance['line_width'])
 
         # Add branch support if specified
         # TODO - currently lands on top of the branches if branch_lengths
         # is switched on
-        # addrows parameter moves the branch labels down a little
-        # if the node labels are also shown
         if appearance['show_support']:
             if not reverse:
                 ax.text(x, -ym, " %.2f" % tree.support, ha='left',
                         va='center', fontsize=appearance['font_size']-2)
             else:
                 ax.text(x, -ym, "%.2f " % tree.support, ha='right',
                         va='center', fontsize=appearance['font_size']-2)
-            addrows = "\n\n"
-        else:
-            addrows = ""
-        if appearance['show_node_labels']:
-            if not reverse:
-                ax.text(x, -ym, "%s %s" % (addrows, tree.name), ha='left',
-                        va='center', fontsize=appearance['font_size']-2)
-            else:
-                ax.text(x, -ym, "%s %s" % (addrows, tree.name), ha='right',
-                        va='center', fontsize=appearance['font_size']-2)
 
         return (y, ym, ps)
 
 
 def reverse_align(ax, ps, reverse):
     '''
     Realigns the text in the tip labels so that for a standard tree, the
```

### Comparing `plot_phylo-0.1.7/plot_phylo.egg-info/PKG-INFO` & `plot_phylo-0.1.8/plot_phylo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-phylo
-Version: 0.1.7
+Version: 0.1.8
 Summary: Module to draw a phylogenetic tree using matplotlib
 Home-page: https://github.com/KatyBrown/plot_phylo
 Author: Katy Brown, Duncan Cross
 Author-email: kab84@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plot_phylo-0.1.7/setup.py` & `plot_phylo-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `plot_phylo-0.1.7/tests/test_get_boxes_data.py` & `plot_phylo-0.1.8/tests/test_get_boxes_data.py`

 * *Files identical despite different names*

### Comparing `plot_phylo-0.1.7/tests/test_plot_phylo.py` & `plot_phylo-0.1.8/tests/test_plot_phylo.py`

 * *Files identical despite different names*

### Comparing `plot_phylo-0.1.7/tests/test_plot_phylo_data.py` & `plot_phylo-0.1.8/tests/test_plot_phylo_data.py`

 * *Files identical despite different names*
