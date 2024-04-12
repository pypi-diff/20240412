# Comparing `tmp/BetheFluid-0.3.tar.gz` & `tmp/BetheFluid-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BetheFluid-0.3.tar", last modified: Thu Nov 23 17:52:13 2023, max compression
+gzip compressed data, was "BetheFluid-0.3.5.tar", last modified: Thu Nov 23 18:18:25 2023, max compression
```

## Comparing `BetheFluid-0.3.tar` & `BetheFluid-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-11-23 17:52:13.606594 BetheFluid-0.3/
-drwxrwxrwx   0        0        0        0 2023-11-23 17:52:13.595400 BetheFluid-0.3/BetheFluid/
--rw-rw-rw-   0        0        0       96 2023-11-20 16:19:57.000000 BetheFluid-0.3/BetheFluid/__init__.py
--rw-rw-rw-   0        0        0     5253 2023-11-20 16:19:57.000000 BetheFluid-0.3/BetheFluid/calc.py
--rw-rw-rw-   0        0        0     7002 2023-11-23 17:49:48.000000 BetheFluid-0.3/BetheFluid/observable.py
--rw-rw-rw-   0        0        0    10214 2023-11-20 16:19:57.000000 BetheFluid-0.3/BetheFluid/solver.py
-drwxrwxrwx   0        0        0        0 2023-11-23 17:52:13.604566 BetheFluid-0.3/BetheFluid.egg-info/
--rw-rw-rw-   0        0        0      141 2023-11-23 17:52:13.000000 BetheFluid-0.3/BetheFluid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-11-23 17:52:13.000000 BetheFluid-0.3/BetheFluid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-23 17:52:13.000000 BetheFluid-0.3/BetheFluid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-20 16:19:57.000000 BetheFluid-0.3/BetheFluid.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-11-23 17:52:13.000000 BetheFluid-0.3/BetheFluid.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-11-23 17:52:13.000000 BetheFluid-0.3/BetheFluid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      141 2023-11-23 17:52:13.605573 BetheFluid-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-11-23 17:52:13.606594 BetheFluid-0.3/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-11-23 17:51:39.000000 BetheFluid-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-23 18:18:25.663091 BetheFluid-0.3.5/
+drwxrwxrwx   0        0        0        0 2023-11-23 18:18:25.649948 BetheFluid-0.3.5/BetheFluid/
+-rw-rw-rw-   0        0        0       96 2023-11-20 16:19:57.000000 BetheFluid-0.3.5/BetheFluid/__init__.py
+-rw-rw-rw-   0        0        0     5253 2023-11-20 16:19:57.000000 BetheFluid-0.3.5/BetheFluid/calc.py
+-rw-rw-rw-   0        0        0     7147 2023-11-23 18:15:48.000000 BetheFluid-0.3.5/BetheFluid/observable.py
+-rw-rw-rw-   0        0        0    10214 2023-11-20 16:19:57.000000 BetheFluid-0.3.5/BetheFluid/solver.py
+drwxrwxrwx   0        0        0        0 2023-11-23 18:18:25.660086 BetheFluid-0.3.5/BetheFluid.egg-info/
+-rw-rw-rw-   0        0        0      143 2023-11-23 18:18:25.000000 BetheFluid-0.3.5/BetheFluid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-11-23 18:18:25.000000 BetheFluid-0.3.5/BetheFluid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-23 18:18:25.000000 BetheFluid-0.3.5/BetheFluid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-20 16:19:57.000000 BetheFluid-0.3.5/BetheFluid.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-11-23 18:18:25.000000 BetheFluid-0.3.5/BetheFluid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-11-23 18:18:25.000000 BetheFluid-0.3.5/BetheFluid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2023-11-23 18:18:25.662085 BetheFluid-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-11-23 18:18:25.663091 BetheFluid-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      371 2023-11-23 18:17:56.000000 BetheFluid-0.3.5/setup.py
```

### Comparing `BetheFluid-0.3/BetheFluid/calc.py` & `BetheFluid-0.3.5/BetheFluid/calc.py`

 * *Files identical despite different names*

### Comparing `BetheFluid-0.3/BetheFluid/observable.py` & `BetheFluid-0.3.5/BetheFluid/observable.py`

 * *Files 11% similar despite different names*

```diff
@@ -149,36 +149,44 @@
                 'local': {'x_axis': self.object.x, 'y_axis': self.energy('local'), 'x_label': 'x', 'y_label': 'energy'},
                 'theta': {'x_axis': self.object.l, 'y_axis': self.energy('theta'), 'x_label': 'theta',
                           'y_label': 'energy'},
                 'total': {'x_axis': self.object.t, 'y_axis': self.energy('total'), 'x_label': 'time',
                           'y_label': 'energy'}},
 
             'entropy': {
-                'local': {'x_axis': self.object.x, 'y_axis': self.entropy('local'), 'x_label': 'x', 'y_label': 'entropy'},
+                'local': {'x_axis': self.object.x, 'y_axis': self.entropy('local'), 'x_label': 'x',
+                          'y_label': 'entropy'},
                 'theta': {'x_axis': self.object.l, 'y_axis': self.entropy('theta'), 'x_label': 'theta',
                           'y_label': 'entropy'},
                 'total': {'x_axis': self.object.t, 'y_axis': self.entropy('total'), 'x_label': 'time',
                           'y_label': 'entropy'}}
         }
 
         option_mapping = main_options_dictionairy[observable]
 
         if option not in option_mapping:
-            raise ValueError('Incorrect argument, choose between: local, theta, total')
+            raise ValueError('Incorrect argument, choose between: local, theta or total')
+
+        if self.object.grid.shape[0] == 1:
+            y_axis = option_mapping[option]['y_axis']
+
+        else:
+
+            y_axis = option_mapping[option]['y_axis'][N, Ellipsis]
 
         if option == 'total':
-            plt.plot(option_mapping[option]['x_axis'], option_mapping[option]['y_axis'][Ellipsis, :], style,
+            plt.plot(option_mapping[option]['x_axis'], y_axis, style,
                      )
             plt.xlabel('time')
             plt.ylabel(option_mapping[option]['y_label'])
             plt.show()
 
         else:
             for item in frames:
-                plt.plot(option_mapping[option]['x_axis'], option_mapping[option]['y_axis'][Ellipsis, item], style,
+                plt.plot(option_mapping[option]['x_axis'], y_axis[:, item], style,
                          label='{} t = {}'.format(name, round(item * self.object.int_t, 3)))
             plt.xlabel(option_mapping[option]['x_label'])
             plt.ylabel(option_mapping[option]['y_label'])
             plt.legend()
             plt.show()
 
         if path is not None:
```

### Comparing `BetheFluid-0.3/BetheFluid/solver.py` & `BetheFluid-0.3.5/BetheFluid/solver.py`

 * *Files identical despite different names*

