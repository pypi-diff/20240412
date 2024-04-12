# Comparing `tmp/optioner-1.5.1.tar.gz` & `tmp/optioner-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optioner-1.5.1.tar", last modified: Fri Apr 12 19:05:00 2024, max compression
+gzip compressed data, was "optioner-1.5.2.tar", last modified: Fri Apr 12 20:35:22 2024, max compression
```

## Comparing `optioner-1.5.1.tar` & `optioner-1.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:05:00.339877 optioner-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 19:04:55.000000 optioner-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-12 19:05:00.339877 optioner-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-12 19:04:55.000000 optioner-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 19:04:55.000000 optioner-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:05:00.339877 optioner-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:05:00.335877 optioner-1.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:04:55.000000 optioner-1.5.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:05:00.339877 optioner-1.5.1/src/optioner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-12 19:05:00.000000 optioner-1.5.1/src/optioner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 19:05:00.000000 optioner-1.5.1/src/optioner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:05:00.000000 optioner-1.5.1/src/optioner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 19:05:00.000000 optioner-1.5.1/src/optioner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-12 19:04:55.000000 optioner-1.5.1/src/optioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:05:00.339877 optioner-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-12 19:04:55.000000 optioner-1.5.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 19:04:55.000000 optioner-1.5.1/tests/test_compulsory_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-12 19:04:55.000000 optioner-1.5.1/tests/test_ifthisthennotthat.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 19:04:55.000000 optioner-1.5.1/tests/test_ifthisthennotthat_vigorous.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 19:04:55.000000 optioner-1.5.1/tests/test_ignore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:35:22.501773 optioner-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 20:35:17.000000 optioner-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-12 20:35:22.501773 optioner-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-12 20:35:17.000000 optioner-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 20:35:17.000000 optioner-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:35:22.501773 optioner-1.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:35:22.501773 optioner-1.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:35:17.000000 optioner-1.5.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:35:22.501773 optioner-1.5.2/src/optioner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-12 20:35:22.000000 optioner-1.5.2/src/optioner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 20:35:22.000000 optioner-1.5.2/src/optioner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:35:22.000000 optioner-1.5.2/src/optioner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 20:35:22.000000 optioner-1.5.2/src/optioner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-12 20:35:17.000000 optioner-1.5.2/src/optioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:35:22.501773 optioner-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-12 20:35:17.000000 optioner-1.5.2/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 20:35:17.000000 optioner-1.5.2/tests/test_compulsory_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-12 20:35:17.000000 optioner-1.5.2/tests/test_ifthisthennotthat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 20:35:17.000000 optioner-1.5.2/tests/test_ifthisthennotthat_vigorous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 20:35:17.000000 optioner-1.5.2/tests/test_ignore.py
```

### Comparing `optioner-1.5.1/LICENSE` & `optioner-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optioner-1.5.1/PKG-INFO` & `optioner-1.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.5.1
+Version: 1.5.2
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -159,15 +159,32 @@
     Returns:
         str | tuple | None_: returns value of argument or None
 ```
 
 usage:
 ```console
 >>> optionCTRL = options(shortargs, longargs, gotargs)
->> optionCTRL._argparse()
+>>> args, check, error, falseargs = optionCTRL._argparse()
 
->>> optionCTRL._what_is_(shortargs[0])
+>>> optionCTRL._what_is_(args[0])
 
 or 
 
->>> optionCTRL._what_is_(longargs[0])
+>>> optionCTRL._what_is_(args[1])
+```
+```python
+# NOTE: if the user provided a longarg say --input, _what_is_ can be used with the corresponding shortarg, in this case it is -i, to find the value.
+
+## For example:
+optCTRL = options(shortargs, longargs, argv[1:])
+args, check, error, falseargs = optCTRL._argparse()
+
+# now it doesn't matter a longarg or a short arg is passed.
+# calling _what_is_ with the shortarg or longarg will return the value.
+
+if '-i' in args or '--input' in args:
+    print(optCTRL._what_is_('i')) # or print(optCTRL._what_is_('input'))
+
+# so if the user provided --input, if we call _what_is('i'), we can get the value.
+# or if the user provided -i, we can call _what_is_('input'), to get the value.
+# NOTE: this is an ease of use feature, only available for v1.5.2 and above.
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.5.1 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.5.2 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -78,10 +78,20 @@
 (shortargs, longargs, sys.argv[1:]) # get values >>> actualargs, argcheck,
 argerror, falseargs = optionCTRL._argparse() ``` ## Extra features Added a
 function to query argument value. ```console >>> help(options._what_is) Help on
 function _what_is_ in module optioner: _what_is_(self, arg: str) Returns the
 value of the argument that is passed. Args: arg (str): argument you need the
 value of count (int | optional): no of values you are expecting. Default is one
 Returns: str | tuple | None_: returns value of argument or None ``` usage:
-```console >>> optionCTRL = options(shortargs, longargs, gotargs) >>
-optionCTRL._argparse() >>> optionCTRL._what_is_(shortargs[0]) or >>>
-optionCTRL._what_is_(longargs[0]) ```
+```console >>> optionCTRL = options(shortargs, longargs, gotargs) >>> args,
+check, error, falseargs = optionCTRL._argparse() >>> optionCTRL._what_is_(args
+[0]) or >>> optionCTRL._what_is_(args[1]) ``` ```python # NOTE: if the user
+provided a longarg say --input, _what_is_ can be used with the corresponding
+shortarg, in this case it is -i, to find the value. ## For example: optCTRL =
+options(shortargs, longargs, argv[1:]) args, check, error, falseargs =
+optCTRL._argparse() # now it doesn't matter a longarg or a short arg is passed.
+# calling _what_is_ with the shortarg or longarg will return the value. if '-i'
+in args or '--input' in args: print(optCTRL._what_is_('i')) # or print
+(optCTRL._what_is_('input')) # so if the user provided --input, if we call
+_what_is('i'), we can get the value. # or if the user provided -i, we can call
+_what_is_('input'), to get the value. # NOTE: this is an ease of use feature,
+only available for v1.5.2 and above. ```
```

### Comparing `optioner-1.5.1/README.md` & `optioner-1.5.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -114,15 +114,32 @@
     Returns:
         str | tuple | None_: returns value of argument or None
 ```
 
 usage:
 ```console
 >>> optionCTRL = options(shortargs, longargs, gotargs)
->> optionCTRL._argparse()
+>>> args, check, error, falseargs = optionCTRL._argparse()
 
->>> optionCTRL._what_is_(shortargs[0])
+>>> optionCTRL._what_is_(args[0])
 
 or 
 
->>> optionCTRL._what_is_(longargs[0])
+>>> optionCTRL._what_is_(args[1])
 ```
+```python
+# NOTE: if the user provided a longarg say --input, _what_is_ can be used with the corresponding shortarg, in this case it is -i, to find the value.
+
+## For example:
+optCTRL = options(shortargs, longargs, argv[1:])
+args, check, error, falseargs = optCTRL._argparse()
+
+# now it doesn't matter a longarg or a short arg is passed.
+# calling _what_is_ with the shortarg or longarg will return the value.
+
+if '-i' in args or '--input' in args:
+    print(optCTRL._what_is_('i')) # or print(optCTRL._what_is_('input'))
+
+# so if the user provided --input, if we call _what_is('i'), we can get the value.
+# or if the user provided -i, we can call _what_is_('input'), to get the value.
+# NOTE: this is an ease of use feature, only available for v1.5.2 and above.
+```
```

#### html2text {}

```diff
@@ -50,10 +50,20 @@
 (shortargs, longargs, sys.argv[1:]) # get values >>> actualargs, argcheck,
 argerror, falseargs = optionCTRL._argparse() ``` ## Extra features Added a
 function to query argument value. ```console >>> help(options._what_is) Help on
 function _what_is_ in module optioner: _what_is_(self, arg: str) Returns the
 value of the argument that is passed. Args: arg (str): argument you need the
 value of count (int | optional): no of values you are expecting. Default is one
 Returns: str | tuple | None_: returns value of argument or None ``` usage:
-```console >>> optionCTRL = options(shortargs, longargs, gotargs) >>
-optionCTRL._argparse() >>> optionCTRL._what_is_(shortargs[0]) or >>>
-optionCTRL._what_is_(longargs[0]) ```
+```console >>> optionCTRL = options(shortargs, longargs, gotargs) >>> args,
+check, error, falseargs = optionCTRL._argparse() >>> optionCTRL._what_is_(args
+[0]) or >>> optionCTRL._what_is_(args[1]) ``` ```python # NOTE: if the user
+provided a longarg say --input, _what_is_ can be used with the corresponding
+shortarg, in this case it is -i, to find the value. ## For example: optCTRL =
+options(shortargs, longargs, argv[1:]) args, check, error, falseargs =
+optCTRL._argparse() # now it doesn't matter a longarg or a short arg is passed.
+# calling _what_is_ with the shortarg or longarg will return the value. if '-i'
+in args or '--input' in args: print(optCTRL._what_is_('i')) # or print
+(optCTRL._what_is_('input')) # so if the user provided --input, if we call
+_what_is('i'), we can get the value. # or if the user provided -i, we can call
+_what_is_('input'), to get the value. # NOTE: this is an ease of use feature,
+only available for v1.5.2 and above. ```
```

### Comparing `optioner-1.5.1/pyproject.toml` & `optioner-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optioner"
-version = "1.5.1"
+version = "1.5.2"
 description = "Argument Parser"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
```

### Comparing `optioner-1.5.1/src/optioner.egg-info/PKG-INFO` & `optioner-1.5.2/src/optioner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.5.1
+Version: 1.5.2
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -159,15 +159,32 @@
     Returns:
         str | tuple | None_: returns value of argument or None
 ```
 
 usage:
 ```console
 >>> optionCTRL = options(shortargs, longargs, gotargs)
->> optionCTRL._argparse()
+>>> args, check, error, falseargs = optionCTRL._argparse()
 
->>> optionCTRL._what_is_(shortargs[0])
+>>> optionCTRL._what_is_(args[0])
 
 or 
 
->>> optionCTRL._what_is_(longargs[0])
+>>> optionCTRL._what_is_(args[1])
+```
+```python
+# NOTE: if the user provided a longarg say --input, _what_is_ can be used with the corresponding shortarg, in this case it is -i, to find the value.
+
+## For example:
+optCTRL = options(shortargs, longargs, argv[1:])
+args, check, error, falseargs = optCTRL._argparse()
+
+# now it doesn't matter a longarg or a short arg is passed.
+# calling _what_is_ with the shortarg or longarg will return the value.
+
+if '-i' in args or '--input' in args:
+    print(optCTRL._what_is_('i')) # or print(optCTRL._what_is_('input'))
+
+# so if the user provided --input, if we call _what_is('i'), we can get the value.
+# or if the user provided -i, we can call _what_is_('input'), to get the value.
+# NOTE: this is an ease of use feature, only available for v1.5.2 and above.
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.5.1 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.5.2 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -78,10 +78,20 @@
 (shortargs, longargs, sys.argv[1:]) # get values >>> actualargs, argcheck,
 argerror, falseargs = optionCTRL._argparse() ``` ## Extra features Added a
 function to query argument value. ```console >>> help(options._what_is) Help on
 function _what_is_ in module optioner: _what_is_(self, arg: str) Returns the
 value of the argument that is passed. Args: arg (str): argument you need the
 value of count (int | optional): no of values you are expecting. Default is one
 Returns: str | tuple | None_: returns value of argument or None ``` usage:
-```console >>> optionCTRL = options(shortargs, longargs, gotargs) >>
-optionCTRL._argparse() >>> optionCTRL._what_is_(shortargs[0]) or >>>
-optionCTRL._what_is_(longargs[0]) ```
+```console >>> optionCTRL = options(shortargs, longargs, gotargs) >>> args,
+check, error, falseargs = optionCTRL._argparse() >>> optionCTRL._what_is_(args
+[0]) or >>> optionCTRL._what_is_(args[1]) ``` ```python # NOTE: if the user
+provided a longarg say --input, _what_is_ can be used with the corresponding
+shortarg, in this case it is -i, to find the value. ## For example: optCTRL =
+options(shortargs, longargs, argv[1:]) args, check, error, falseargs =
+optCTRL._argparse() # now it doesn't matter a longarg or a short arg is passed.
+# calling _what_is_ with the shortarg or longarg will return the value. if '-i'
+in args or '--input' in args: print(optCTRL._what_is_('i')) # or print
+(optCTRL._what_is_('input')) # so if the user provided --input, if we call
+_what_is('i'), we can get the value. # or if the user provided -i, we can call
+_what_is_('input'), to get the value. # NOTE: this is an ease of use feature,
+only available for v1.5.2 and above. ```
```

### Comparing `optioner-1.5.1/src/optioner.py` & `optioner-1.5.2/src/optioner.py`

 * *Files 14% similar despite different names*

```diff
@@ -145,20 +145,43 @@
         Args:
             arg (str): argument you need the value of
             count (int | optional): no of values you are expecting. Default is one
 
         Returns:
             str | tuple | None_: returns value of argument or None
         """
-        if len(arg)>2:
-            arg = '--' + arg
-        else:
-            arg = '-' + arg
+        # if len(arg)>2:
+        #     arg = '--' + arg
+        # else:
+        #     arg = '-' + arg
         
-        index = self._args.index(arg)
+        if '-'+arg in self._shortargs:
+            # if arg provided is shortarg
+            arg = '-'+arg
+            try:
+                # try finding the index of it.
+                index = self._args.index(arg)
+            except ValueError:
+                # if arg is not provided, find the corresponding long arg
+                sindex = self._shortargs.index(arg)
+                longarg = self._longargs[sindex]
+                # find the index of the corresponding long arg
+                index = self._args.index(longarg)
+        elif '--'+arg in self._longargs:
+            # if arg provided is longarg
+            arg = '--'+arg
+            try:
+                # try finding the index of it
+                index = self._args.index(arg)
+            except ValueError:
+                # if arg is not provided, find the corresponding short arg
+                lindex = self._longargs.index(arg)
+                shortarg = self._shortargs[lindex]
+                # find the index of the corresponding short arg
+                index = self._args.index(shortarg)
         
         result: list[str] = []
         
         try:
             for i in range(index+1, index+1+count):
                 result.append(self._args[i])
         except IndexError:
```

### Comparing `optioner-1.5.1/tests/test_basic.py` & `optioner-1.5.2/tests/test_basic.py`

 * *Files identical despite different names*

