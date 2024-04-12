# Comparing `tmp/jemma-0.1.4200.tar.gz` & `tmp/jemma-0.1.422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.4200.tar", last modified: Thu Apr 11 01:42:31 2024, max compression
+gzip compressed data, was "jemma-0.1.422.tar", last modified: Fri Apr 12 00:35:57 2024, max compression
```

## Comparing `jemma-0.1.4200.tar` & `jemma-0.1.422.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.729297 jemma-0.1.4200/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-11 01:42:31.728765 jemma-0.1.4200/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)     5201 2024-04-10 21:53:43.000000 jemma-0.1.4200/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.703963 jemma-0.1.4200/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2311 2024-04-10 04:55:55.000000 jemma-0.1.4200/jemma/huddle.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.709159 jemma-0.1.4200/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.710503 jemma-0.1.4200/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.714103 jemma-0.1.4200/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.716210 jemma-0.1.4200/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.718634 jemma-0.1.4200/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.725451 jemma-0.1.4200/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     7571 2024-04-11 01:32:04.000000 jemma-0.1.4200/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5439 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     3651 2024-04-11 01:30:43.000000 jemma-0.1.4200/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.727534 jemma-0.1.4200/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-10 21:15:08.000000 jemma-0.1.4200/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.708523 jemma-0.1.4200/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-11 01:42:31.729454 jemma-0.1.4200/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-11 01:42:24.000000 jemma-0.1.4200/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.242475 jemma-0.1.422/
+-rw-r--r--   0 tolitius   (503) staff       (20)      125 2024-04-12 00:35:57.240575 jemma-0.1.422/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)     5201 2024-04-10 21:53:43.000000 jemma-0.1.422/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.215776 jemma-0.1.422/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2353 2024-04-11 19:01:08.000000 jemma-0.1.422/jemma/huddle.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.221649 jemma-0.1.422/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.223277 jemma-0.1.422/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    19657 2024-04-11 22:22:14.000000 jemma-0.1.422/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.226685 jemma-0.1.422/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.228933 jemma-0.1.422/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.230940 jemma-0.1.422/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.236673 jemma-0.1.422/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4881 2024-04-11 20:01:12.000000 jemma-0.1.422/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     8229 2024-04-11 20:34:07.000000 jemma-0.1.422/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6803 2024-04-11 20:04:04.000000 jemma-0.1.422/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4584 2024-04-11 18:12:49.000000 jemma-0.1.422/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.239236 jemma-0.1.422/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2904 2024-04-12 00:33:39.000000 jemma-0.1.422/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.220692 jemma-0.1.422/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      125 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)      109 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-12 00:35:57.242767 jemma-0.1.422/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      532 2024-04-12 00:35:47.000000 jemma-0.1.422/setup.py
```

### Comparing `jemma-0.1.4200/README.md` & `jemma-0.1.422/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.4200/jemma/huddle.py` & `jemma-0.1.422/jemma/huddle.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
                                   business_owner,
                                   engineer)
     if args.build_prototype:
         flow.build_prototype(brain,
                              project_manager,
                              business_owner,
                              engineer,
-                             args.prompt)
+                             args.prompt,
+                             args.sketch)
 
     if args.build_user_stories:
         flow.build_user_stories(brain,
                                 project_manager,
                                 business_owner,
                                 engineer)
     if args.test_prototype:
```

### Comparing `jemma-0.1.4200/jemma/prompt/business/owner.py` & `jemma-0.1.422/jemma/prompt/business/owner.py`

 * *Files 20% similar despite different names*

```diff
@@ -318,7 +318,109 @@
 - Optimize the app's performance by minimizing DOM manipulation and using efficient algorithms for color generation and manipulation.
 - Add error handling and validation for user inputs to ensure a smooth user experience.
 - Consider adding a feature to share color palettes on social media or via unique URLs.
 - Provide a help section or tutorial to guide users on how to use the app effectively.
 
 By following this prompt, an AI model should be able to generate a self-sufficient and functional prototype of the Color Palette Generator web app using HTML, CSS, and JavaScript. The prototype should fulfill the specified requirements, provide an engaging user interface, and demonstrate the core functionality of the app idea.
 """
+
+def idea_with_sketch_to_intel(idea, sketch):
+    return f"""
+Analyze the UI sketch in the image and extract the following structured information to be used to recreate this interface with HTML, CSS and JavaScript:
+
+1. Identify all distinct UI components (text fields, labels, buttons, containers, etc.) and list them along with their:
+   - Component type (input, button, div, etc.)
+   - Text content
+   - Placeholder text (if applicable)
+   - Unique identifier (if applicable, e.g. "name", "toolbar", "upcoming-lesson", etc.)
+
+2. Describe the overall layout and visual structure of the interface, including:
+   - Relative positioning of components (e.g. "toolbar at top", "3 buttons below header", "2 column layout", etc.)
+   - Any visual grouping or separation of components
+   - Estimated dimensions and spacing (widths, heights, padding, margins)
+
+3. Identify any interactive elements and describe their apparent functionality, for example:
+   - "Courses dropdown opens menu on click"
+   - "New buttons add new slot on click"
+   - "'Concept' button likely opens a modal dialog", etc.
+
+4. Call out any key visual styling details, such as:
+   - Background colors
+   - Font sizes, weights, and styles
+   - Border styles
+   - Button styles
+
+Provide the extracted information in a structured JSON format like this:
+
+{{
+  "components": [
+    {{
+      "type": "input",
+      "id": "name",
+      "placeholder": "Name"
+    }},
+    ...
+  ],
+  "layout": {{
+    "positioning": [...],
+    "grouping": [...],
+    "spacing": [...]
+  }},
+  "interactivity": [...],
+  "styling": {{
+    "colors": [...],
+    "fonts": [...],
+    ...
+  }}
+}}
+    """
+
+def sketch_intel_to_requirements(idea, sketch_intel):
+    return f"""
+Title: Web App Prototype Prompt Generator
+
+Description:
+Create a prompt generator that takes a short-form web app idea and a description of a mockup and generates a detailed prompt for building a self-sufficient prototype using only HTML, CSS, and JavaScript. The generated prompt should guide an AI model to create a functional web app prototype based on the provided idea and the mockup description. The generated prompt should make sure that the prototype 100% aligns with the visual structure and interactivity described in the mockup.
+
+Web App Idea:
+{idea}
+
+Mockup Description:
+{sketch_intel}
+
+Prompt:
+[Web App Idea]
+Description: [A brief description of the web app idea]
+
+Desired Prompt Output:
+
+Title: [Web App Name]
+
+Description:
+[A detailed description of the web app, including its purpose, main features, and target audience]
+
+Requirements:
+1. [Requirement 1]
+2. [Requirement 2]
+3. [Requirement 3]
+...
+
+User Interface:
+[A description of the desired user interface, including layout, design elements, and user interactions based on the idea and mockup description]
+
+Functionality:
+[Detailed explanations of the app's functionality, including any necessary algorithms, data processing, or dynamic behavior based on the idea and mockup description]
+
+HTML Structure:
+[Guidelines for structuring the HTML code, including specific elements, classes, and IDs to be used based on the idea and mockup description]
+
+CSS Styling:
+[Instructions for styling the app using CSS, including color scheme, typography, layout, and responsive design considerations based on the idea and mockup description]
+
+JavaScript Interactivity:
+[Directions for implementing interactivity and dynamic functionality using JavaScript, including event handling, data manipulation, and API integration if applicable based on the idea and mockup description]
+
+Additional Considerations:
+[Any additional features, optimizations, or best practices to keep in mind while building the prototype based on the idea and mockup description]
+
+Note: The generated prompt should be clear, concise, and provide sufficient detail for an AI model to generate a functional web app prototype using only HTML, CSS, and JavaScript. The prompt should focus on guiding the model to create a self-sufficient prototype relying on jQuery, Twitter Bootstrap and DataTable libraries.
+"""
```

### Comparing `jemma-0.1.4200/jemma/prompt/engineer/clarify.py` & `jemma-0.1.422/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.4200/jemma/prompt/engineer/code.py` & `jemma-0.1.422/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.4200/jemma/prompt/tester/test.py` & `jemma-0.1.422/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.4200/jemma/requirements/feature.py` & `jemma-0.1.422/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.4200/jemma/team/business_owner.py` & `jemma-0.1.422/jemma/team/business_owner.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,7 +82,24 @@
 
 
     def idea_to_prompt(self, thinker, idea):
         say(self.title, "📚 creating detailed requirements ...🖋️", message_color=color.DARKCYAN)
         return thinker.think(prompt.idea_to_prompt(idea),
                              self.title,
                              mute=True)
+
+    def idea_with_sketch_to_intel(self,
+                                  thinker,
+                                  idea,
+                                  sketch):
+        say(self.title, "🔍 collecting intel about the sketch ...", message_color=color.DARKCYAN)
+        return thinker.see(prompt.idea_with_sketch_to_intel(idea, sketch),
+                           sketch,
+                           self.title)
+
+    def idea_with_sketch_to_prompt(self,
+                                   thinker,
+                                   idea,
+                                   sketch_intel):
+        say(self.title, "📚 creating detailed requirements (for: idea + sketch) ...🖋️", message_color=color.DARKCYAN)
+        return thinker.think(prompt.sketch_intel_to_requirements(idea, sketch_intel),
+                             self.title)
```

### Comparing `jemma-0.1.4200/jemma/team/engineer.py` & `jemma-0.1.422/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.4200/jemma/team/project_manager.py` & `jemma-0.1.422/jemma/team/project_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -154,15 +154,28 @@
     def user_stories_to_requirement(self):
         self.feature = Feature(self.feature.export_user_stories_titles_and_criteria())
 
     def meet_to_create_requirements(self,
                                     thinker,
                                     business_owner,
                                     idea,
+                                    sketch = None,
                                     store_path="requirements"):
         say(self.role, "\nDear Business Owner, in this meeting we'll work on creating requirements based on the 💡 idea",
             who_color = color.CYAN, message_color = color.YELLOW)
 
-        requirements = business_owner.idea_to_prompt(thinker, idea)
+        requirements = "requirements not created yet"
+        if sketch:
+            sketch_intel = business_owner.idea_with_sketch_to_intel(thinker,
+                                                                    idea,
+                                                                    sketch)
+            print(f"sketch intel: {sketch_intel}")
+
+            requirements = business_owner.idea_with_sketch_to_prompt(thinker,
+                                                                     idea,
+                                                                     sketch_intel)
+        else:
+            requirements = business_owner.idea_to_prompt(thinker, idea)
+
         self.record_requirement(idea, requirements, store_path)
 
         self.feature = Feature(requirements)
```

### Comparing `jemma-0.1.4200/jemma/team/tester.py` & `jemma-0.1.422/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.4200/jemma/thinker.py` & `jemma-0.1.422/jemma/thinker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os, time
-from jemma.tools import color, say
+from jemma.tools import color, say, image_path_to_data
 
 import ollama
 import replicate
 from anthropic import Anthropic
 from openai import OpenAI
 
 class Thinker:
@@ -71,14 +71,57 @@
     def __init__(self, model_name):
         super().__init__(model_name)
 
         ## make sure ANTHROPIC_API_KEY is exported in shell
         ## or it is exported in a .env file
         self.client = client = Anthropic()
 
+    def see(self,
+            prompt,
+            image_path,
+            who="user",
+            max_tokens=1024,
+            action="👀 looking at the image... ",
+            mute=False,
+            sleep_time=1):
+
+        say(who, action + image_path)
+
+        image_data, image_type = image_path_to_data(image_path).values()
+
+        response = self.client.messages.create(
+                model=self.model_name,
+                max_tokens=max_tokens,
+                messages=[
+                    {
+                        "role": "user",
+                        "content": [
+                            {
+                                "type": "image",
+                                "source": {
+                                    "type": "base64",
+                                    "media_type": image_type,
+                                    "data": image_data,
+                                    },
+                                },
+                            {
+                                "type": "text",
+                                "text": prompt,
+                                }
+                            ],
+                        }
+                    ],
+                )
+
+        saw_this = response.content[0].text
+
+        # print(color.RED + f">> {saw_this} <<" + color.END)
+
+        return saw_this
+
     def think(self, prompt, who="user", action="", mute=False, sleep_time=1): # sleep not to exceed the rate limit
 
         if action != "" or not mute:
             say(who, action)
 
         time.sleep(sleep_time)
```

### Comparing `jemma-0.1.4200/jemma/tools.py` & `jemma-0.1.422/jemma/tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import webbrowser
-import os, argparse, sys, re
+import os, argparse, sys, re, base64
 
 from datetime import datetime
 
 class color:
    PURPLE = '\033[95m'
    CYAN = '\033[96m'
    DARKCYAN = '\033[36m'
@@ -61,14 +61,15 @@
         usage='%(prog)s [-h] [--requirements path-to-file] [--prompt prompt] [--build-prototype]\n'
               '                 [--claude [model name]] [--openai [model name]] [--ollama [model name]] [--replicate [model name]]',
         epilog='thoughts in, software out'
     )
 
     parser.add_argument('--requirements', metavar='path', type=str, help='path to a text file with requirements')
     parser.add_argument('--prompt', metavar='prompt', type=str, help='short idea to convert to creation')
+    parser.add_argument('--sketch', metavar='sketch', type=str, help='a mockup or a hand drawn sketch to convert to a prototype')
 
     parser.add_argument('--user-stories', action='store_true', help='create and refine user stories')
     parser.add_argument('--build-user-stories', action='store_true', help='build prototype on combined (non-refined) user stories')
 
     parser.add_argument('--build-prototype', action='store_true', help='build prototype')
     parser.add_argument('--test-prototype', action='store_true', help='test prototype')
 
@@ -79,7 +80,40 @@
 
     if len(sys.argv) == 1 or '-h' in sys.argv or '--help' in sys.argv:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
     args = parser.parse_args()
     return args
+
+
+def file_to_utf8(path):
+
+   with open(path, "rb") as file:
+      image_data = file.read()
+      encoded = base64.b64encode(image_data)
+      return encoded.decode("utf-8")
+
+def image_path_to_type(path):
+
+    extension = path.split(".")[-1].lower()
+
+    media_types = {
+        "jpg": "image/jpeg",
+        "jpeg": "image/jpeg",
+        "png": "image/png",
+        "gif": "image/gif",
+        "bmp": "image/bmp",
+        "tiff": "image/tiff",
+        "webp": "image/webp",
+        "svg": "image/svg+xml"
+    }
+
+    if extension not in media_types:
+        raise ValueError(f"could not determine an image type. image path: {path}")
+
+    return media_types[extension]
+
+def image_path_to_data(path):
+
+   return {"image_data": file_to_utf8(path),
+           "image_type": image_path_to_type(path)}
```

### Comparing `jemma-0.1.4200/jemma/work/flow.py` & `jemma-0.1.422/jemma/work/flow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-import readline
+try:
+    from pyreadline3 import Readline # windows support
+    readline = Readline()
+except ImportError:
+    import readline
+
 from jemma.tools import color
 
 def create_user_stories(brain,
                         project_manager,
                         business_owner,
                         engineer):
 
@@ -43,20 +48,22 @@
         elif feedback == "":
             return None
 
 def build_prototype(brain,
                     project_manager,
                     business_owner,
                     engineer,
-                    prompt = None):
+                    prompt = None,
+                    sketch = None):
 
     if prompt:
         project_manager.meet_to_create_requirements(brain,
                                                     business_owner,
-                                                    prompt)
+                                                    prompt,
+                                                    sketch)
     prototype = project_manager.meet_to_build_prototype(brain,
                                                         engineer)
 
     while True:
         feedback = ask_for_feedback()
         if not feedback:
             break
```

### Comparing `jemma-0.1.4200/jemma.egg-info/SOURCES.txt` & `jemma-0.1.422/jemma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

