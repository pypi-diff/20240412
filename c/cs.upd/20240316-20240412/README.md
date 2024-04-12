# Comparing `tmp/cs.upd-20240316.tar.gz` & `tmp/cs.upd-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.upd-20240316.tar", last modified: Sat Mar 16 07:02:57 2024, max compression
+gzip compressed data, was "cs.upd-20240412.tar", last modified: Fri Apr 12 05:01:20 2024, max compression
```

## Comparing `cs.upd-20240316.tar` & `cs.upd-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:02:57.617519 cs.upd-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 07:02:15.000000 cs.upd-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    14912 2024-03-16 07:02:57.617185 cs.upd-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    19976 2024-03-16 07:02:29.000000 cs.upd-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:02:57.613600 cs.upd-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:02:57.613868 cs.upd-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:02:57.615060 cs.upd-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    40471 2024-03-16 07:02:06.000000 cs.upd-20240316/lib/python/cs/upd.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:02:57.616752 cs.upd-20240316/lib/python/cs.upd.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    14912 2024-03-16 07:02:57.000000 cs.upd-20240316/lib/python/cs.upd.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      261 2024-03-16 07:02:57.000000 cs.upd-20240316/lib/python/cs.upd.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 07:02:57.000000 cs.upd-20240316/lib/python/cs.upd.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      155 2024-03-16 07:02:57.000000 cs.upd-20240316/lib/python/cs.upd.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 07:02:57.000000 cs.upd-20240316/lib/python/cs.upd.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    15472 2024-03-16 07:02:56.000000 cs.upd-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 07:02:57.617610 cs.upd-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:01:20.547513 cs.upd-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:00:39.000000 cs.upd-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    21266 2024-04-12 05:01:20.547195 cs.upd-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    20487 2024-04-12 05:00:53.000000 cs.upd-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:01:20.542972 cs.upd-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:01:20.543249 cs.upd-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:01:20.544993 cs.upd-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    40518 2024-04-12 05:00:25.000000 cs.upd-20240412/lib/python/cs/upd.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:01:20.546734 cs.upd-20240412/lib/python/cs.upd.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    21266 2024-04-12 05:01:19.000000 cs.upd-20240412/lib/python/cs.upd.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      261 2024-04-12 05:01:20.000000 cs.upd-20240412/lib/python/cs.upd.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:01:20.000000 cs.upd-20240412/lib/python/cs.upd.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      155 2024-04-12 05:01:20.000000 cs.upd-20240412/lib/python/cs.upd.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:01:20.000000 cs.upd-20240412/lib/python/cs.upd.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    21831 2024-04-12 05:01:19.000000 cs.upd-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:01:20.547614 cs.upd-20240412/setup.cfg
```

### Comparing `cs.upd-20240316/PKG-INFO` & `cs.upd-20240412/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,15 @@
-Metadata-Version: 2.1
-Name: cs.upd
-Version: 20240316
-Summary: Single and multiple line status updates with minimal update sequences.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 Single and multiple line status updates with minimal update sequences.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* Upd.run_task: provide the label as the new UpdProxy prefix.
+* Upd.insert: the supplied txt is the proxy.text, not the prefix.
+* UpdProxy.text: setting to None sets to self._text_auto() if present or makes no change.
+* New @without decorator to withdraw the Upd during a function.
+* print: use the builtin print directly if the Upd is disabled.
 
 This is available as an output mode in `cs.logutils`.
 
 Single line example:
 
     from cs.upd import Upd, nl, print
     .....
@@ -77,52 +63,39 @@
 The constructor has an optional parameter `disabled` to override
 this default behaviour.
 
 ## Function `demo()`
 
 A tiny demo function for visual checking of the basic functionality.
 
-## Function `nl(msg, *a, upd, **kw)`
+## Function `nl(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113604c0>, **kw)`
 
 Write `msg` to `file` (default `sys.stdout`),
 without interfering with the `Upd` instance.
 This is a thin shim for `Upd.print`.
 
-## Function `out(msg, *a, upd, **outkw)`
+## Function `out(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x11135ba30>, **kw)`
 
 Update the status line of the default `Upd` instance.
 Parameters are as for `Upd.out()`.
 
-## Function `pfxprint(*a, upd, **kw)`
+## Function `pfxprint(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x11135bf40>, **kw)`
 
 Wrapper for `cs.pfx.pfxprint` to pass `print_func=cs.upd.print`.
 
 Programmes integrating `cs.upd` with use of the `cs.pfx.pfxprint`
 function should use this at import time:
 
     from cs.upd import pfxprint
 
-## Function `print(*a, upd: cs.upd.Upd, end='\n', **kw)`
-
-Wrapper for the builtin print function
-to call it inside `Upd.above()` and enforce a flush.
-
-The function supports an addition parameter beyond the builtin print:
-* `upd`: the `Upd` instance to use, default `Upd()`
-
-Programmes integrating `cs.upd` with use of the builtin `print`
-function should use this at import time:
-
-    from cs.upd import print
-
-## Function `run_task(*a, upd, **kw)`
+## Function `run_task(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113601f0>, **kw)`
 
 Top level `run_task` function to call `Upd.run_task`.
 
-## Class `Upd(cs.obj.SingletonMixin, cs.resources.MultiOpenMixin, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `Upd(cs.obj.SingletonMixin, cs.resources.MultiOpenMixin, cs.threads.HasThreadState)`
 
 A `SingletonMixin` subclass for maintaining multiple status lines.
 
 The default backend is `sys.stderr`.
 
 *Method `Upd.__init__(self, backend=None, columns=None, disabled=None)`*:
 Initialise the `Upd`.
@@ -133,14 +106,160 @@
 * `columns`: the width of the output,
   default from the width of the `backend` tty if it is a tty,
   `80` otherwise
 * `disabled`: if true, disable the output - just keep state;
   default true if the output is not a tty;
   this automatically silences the `Upd` if stderr is not a tty
 
+*Method `Upd.__enter_exit__(self)`*:
+Generator supporting `__enter__` and `__exit__`.
+
+On shutdown, if we are exiting because of an exception
+which is not a `SystemExit` with a `code` of `None` or `0`
+then we preserve the status lines one screen.
+Otherwise we clean up the status lines.
+
+*Method `Upd.__getitem__(self, index)`*:
+The text of the status line at `index`.
+
+*Method `Upd.__len__(self)`*:
+The length of an `Upd` is the number of slots.
+
+*Method `Upd.above(self, need_newline=False)`*:
+Context manager to move to the top line of the `Upd` display,
+clear it, `yield`, redraw below.
+
+This context manager is for use when interleaving _another_
+stream with the `Upd` display;
+if you just want to write lines above the display
+for the same backend use `Upd.nl`.
+
+The usual situation for `Upd.above`
+is interleaving `sys.stdout` and `sys.stderr`,
+which are often attached to the same terminal.
+
+Note that the caller's output should be flushed
+before exiting the suite
+so that the output is completed before the `Upd` resumes.
+
+Example:
+
+    U = Upd()   # default sys.stderr Upd
+    ......
+    with U.above():
+        print('some message for stdout ...', flush=True)
+
+*Method `Upd.cursor_invisible(self)`*:
+Make the cursor vinisible.
+
+*Method `Upd.cursor_visible(self)`*:
+Make the cursor visible.
+
+*Method `Upd.delete(self, index)`*:
+Delete the status line at `index`.
+
+Return the `UpdProxy` of the deleted status line.
+
+*Method `Upd.diff(oldtxt, newtxt, columns, raw_text=False)`*:
+Compute the text sequences required to update `oldtxt` to `newtxt`
+presuming the cursor is at the right hand end of `oldtxt`.
+The available area is specified by `columns`.
+
+We normalise `newtxt` as using `self.normalise`.
+`oldtxt` is presumed to be already normalised.
+
+If `raw_text` is true (default `False`) we do not normalise `newtxt`
+before comparison.
+
+*Method `Upd.disable(self)`*:
+Disable updates.
+
+*Property `Upd.disabled`*:
+Whether this `Upd` is currently disabled.
+
+*Method `Upd.enable(self)`*:
+Enable updates.
+
+*Method `Upd.flush(self)`*:
+Flush the backend stream.
+
+*Method `Upd.insert(self, index, txt='', proxy=None, **proxy_kw) -> 'UpdProxy'`*:
+Insert a new status line at `index`.
+Return the `UpdProxy` for the new status line.
+
+*Method `Upd.nl(self, txt, *a, redraw=False)`*:
+Write `txt` to the backend followed by a newline.
+
+Parameters:
+* `txt`: the message to write.
+* `a`: optional positional parameters;
+  if not empty, `txt` is percent formatted against this list.
+* `redraw`: if true (default `False`) use the "redraw" method.
+
+This uses one of two methods:
+* insert above:
+  insert a line above the top status line and write the message there.
+* redraw:
+  clear the top slot, write txt and a newline,
+  redraw all the slots below.
+
+The latter method is used if `redraw` is true
+or if `txt` is wider than `self.columns`
+or if there is no "insert line" capability.
+
+*Method `Upd.normalise(txt)`*:
+Normalise `txt` for display,
+currently implemented as:
+`unctrl(txt.rstrip())`.
+
+*Method `Upd.out(self, txt, *a, slot=0, raw_text=False, redraw=False) -> str`*:
+Update the status line at `slot` to `txt`.
+Return the previous status line content.
+
+Parameters:
+* `txt`: the status line text.
+* `a`: optional positional parameters;
+  if not empty, `txt` is percent formatted against this list.
+* `slot`: which slot to update; default is `0`, the bottom slot
+* `raw_text`: if true (default `False`), do not normalise the text
+* `redraw`: if true (default `False`), redraw the whole line
+  instead of doing the minimal and less visually annoying
+  incremental change
+
+*`Upd.perthread_state`*
+
+*Method `Upd.proxy(self, index)`*:
+Return the `UpdProxy` for `index`.
+Returns `None` if `index` is out of range.
+The index `0` is never out of range;
+it will be autocreated if there are no slots yet.
+
+*Method `Upd.run_task(self, label: str, *, report_print=False, tick_delay: int = 0.3, tick_chars='|/-\\')`*:
+Context manager to display an `UpdProxy` for the duration of some task.
+It yields the proxy.
+
+*Method `Upd.selfcheck(self)`*:
+Sanity check the internal data structures.
+
+Warning: this uses asserts.
+
+*Method `Upd.shutdown(self, preserve_display=False)`*:
+Clean out this `Upd`, optionally preserving the displayed status lines.
+
+*Method `Upd.ti_str(self, ti_name)`*:
+Fetch the terminfo capability string named `ti_name`.
+Return the string or `None` if not available.
+
+*Method `Upd.without(self, temp_state='', slot=0)`*:
+Context manager to clear the status line around a suite.
+Returns the status line text as it was outside the suite.
+
+The `temp_state` parameter may be used to set the inner status line
+content if a value other than `''` is desired.
+
 ## Class `UpdProxy`
 
 A proxy for a status line of a multiline `Upd`.
 
 This provides a stable reference to a status line after it has been
 instantiated by `Upd.insert`.
 
@@ -150,24 +269,63 @@
 
     U = Upd()
     ....
     with U.insert(1, 'hello!') as proxy:
         .... set proxy.text as needed ...
     # proxy now removed
 
-*Method `UpdProxy.__init__(self, text: Optional[str] = None, *, upd: cs.upd.Upd, index: Optional[int] = 1, prefix: Optional[str] = None, suffix: Optional[str] = None, text_auto=None, update_period: Optional[float] = None)`*:
+*Method `UpdProxy.__init__(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x111360790>, **kw)`*:
 Initialise a new `UpdProxy` status line.
 
 Parameters:
 * `index`: optional position for the new proxy as for `Upd.insert`,
   default `1` (directly above the bottom status line)
 * `upd`: the `Upd` instance with which to associate this proxy,
   default the default `Upd` instance (associated with `sys.stderr`)
 * `text`: optional initial text for the new status line
 
+*Method `UpdProxy.__call__(self, msg, *a)`*:
+Calling the proxy sets its `.text` property
+in the form used by other messages: `(msg,*a)`
+
+*Method `UpdProxy.__del__(self)`*:
+Delete this proxy from its parent `Upd`.
+
+*Method `UpdProxy.delete(self)`*:
+Delete this proxy from its parent `Upd`.
+
+*Method `UpdProxy.extend_prefix(self, more_prefix, print_elapsed=False)`*:
+Context manager to append text to the prefix.
+
+*Method `UpdProxy.insert(self, index, txt='')`*:
+Insert a new `UpdProxy` at a position relative to this `UpdProxy`.
+Return the new proxy.
+
+This supports the positioning of related status lines.
+
+*Property `UpdProxy.prefix`*:
+The current prefix string.
+
+*Method `UpdProxy.reset(self)`*:
+Clear the proxy: set both the prefix and text to `''`.
+
+*Property `UpdProxy.suffix`*:
+The current suffix string.
+
+*Property `UpdProxy.text`*:
+The text of this proxy's slot, without the prefix.
+
+*Property `UpdProxy.width`*:
+The available space for text after `self.prefix` and before `self.suffix`.
+
+This is available width for uncropped text,
+intended to support presizing messages such as progress bars.
+Setting the text to something longer will crop the rightmost
+portion of the text which fits.
+
 ## Function `uses_upd(*da, **dkw)`
 
 Decorator for functions accepting an optional `upd:Upd` parameter,
 default from `Upd.default() or Upd()`.
 This also makes the `upd` the default `Upd` instance for this thread.
 
 ## Function `with_upd_proxy(*da, **dkw)`
@@ -177,29 +335,36 @@
 
 Example:
 
     @with_upd_proxy
     def func(*a, upd_proxy:UpdProxy, **kw):
       ... perform task, updating upd_proxy ...
 
-## Function `without(*, upd: cs.upd.Upd)`
+## Function `without(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113613f0>, **kw)`
 
 Context manager withdraw the `Upd` while something runs.
 
 Example:
 
     from cs.upd import without
     ...
     with without():
         os.system('ls -la')
 
 # Release Log
 
 
 
+*Release 20240412*:
+* Upd.run_task: provide the label as the new UpdProxy prefix.
+* Upd.insert: the supplied txt is the proxy.text, not the prefix.
+* UpdProxy.text: setting to None sets to self._text_auto() if present or makes no change.
+* New @without decorator to withdraw the Upd during a function.
+* print: use the builtin print directly if the Upd is disabled.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240216*:
 New without() context manager to withdraw the Upd while something runs.
 
 *Release 20240201*:
@@ -387,8 +552,7 @@
 * Upd.nl,out: accept optional positional parameters, use with %-formatting if supplied, just like logging.
 
 *Release 20150118*:
 metadata fix
 
 *Release 20150116*:
 Initial PyPI release.
-
```

### Comparing `cs.upd-20240316/README.md` & `cs.upd-20240412/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,33 @@
+Metadata-Version: 2.1
+Name: cs.upd
+Version: 20240412
+Summary: Single and multiple line status updates with minimal update sequences.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 Single and multiple line status updates with minimal update sequences.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* Upd.run_task: provide the label as the new UpdProxy prefix.
+* Upd.insert: the supplied txt is the proxy.text, not the prefix.
+* UpdProxy.text: setting to None sets to self._text_auto() if present or makes no change.
+* New @without decorator to withdraw the Upd during a function.
+* print: use the builtin print directly if the Upd is disabled.
 
 This is available as an output mode in `cs.logutils`.
 
 Single line example:
 
     from cs.upd import Upd, nl, print
     .....
@@ -59,52 +81,39 @@
 The constructor has an optional parameter `disabled` to override
 this default behaviour.
 
 ## Function `demo()`
 
 A tiny demo function for visual checking of the basic functionality.
 
-## Function `nl(msg, *a, upd, **kw)`
+## Function `nl(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113604c0>, **kw)`
 
 Write `msg` to `file` (default `sys.stdout`),
 without interfering with the `Upd` instance.
 This is a thin shim for `Upd.print`.
 
-## Function `out(msg, *a, upd, **outkw)`
+## Function `out(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x11135ba30>, **kw)`
 
 Update the status line of the default `Upd` instance.
 Parameters are as for `Upd.out()`.
 
-## Function `pfxprint(*a, upd, **kw)`
+## Function `pfxprint(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x11135bf40>, **kw)`
 
 Wrapper for `cs.pfx.pfxprint` to pass `print_func=cs.upd.print`.
 
 Programmes integrating `cs.upd` with use of the `cs.pfx.pfxprint`
 function should use this at import time:
 
     from cs.upd import pfxprint
 
-## Function `print(*a, upd: cs.upd.Upd, end='\n', **kw)`
-
-Wrapper for the builtin print function
-to call it inside `Upd.above()` and enforce a flush.
-
-The function supports an addition parameter beyond the builtin print:
-* `upd`: the `Upd` instance to use, default `Upd()`
-
-Programmes integrating `cs.upd` with use of the builtin `print`
-function should use this at import time:
-
-    from cs.upd import print
-
-## Function `run_task(*a, upd, **kw)`
+## Function `run_task(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113601f0>, **kw)`
 
 Top level `run_task` function to call `Upd.run_task`.
 
-## Class `Upd(cs.obj.SingletonMixin, cs.resources.MultiOpenMixin, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `Upd(cs.obj.SingletonMixin, cs.resources.MultiOpenMixin, cs.threads.HasThreadState)`
 
 A `SingletonMixin` subclass for maintaining multiple status lines.
 
 The default backend is `sys.stderr`.
 
 *Method `Upd.__init__(self, backend=None, columns=None, disabled=None)`*:
 Initialise the `Upd`.
@@ -130,15 +139,16 @@
 *Method `Upd.__getitem__(self, index)`*:
 The text of the status line at `index`.
 
 *Method `Upd.__len__(self)`*:
 The length of an `Upd` is the number of slots.
 
 *Method `Upd.above(self, need_newline=False)`*:
-Context manager to move to the top line of the display, clear it, yield, redraw below.
+Context manager to move to the top line of the `Upd` display,
+clear it, `yield`, redraw below.
 
 This context manager is for use when interleaving _another_
 stream with the `Upd` display;
 if you just want to write lines above the display
 for the same backend use `Upd.nl`.
 
 The usual situation for `Upd.above`
@@ -277,15 +287,15 @@
 
     U = Upd()
     ....
     with U.insert(1, 'hello!') as proxy:
         .... set proxy.text as needed ...
     # proxy now removed
 
-*Method `UpdProxy.__init__(self, text: Optional[str] = None, *, upd: cs.upd.Upd, index: Optional[int] = 1, prefix: Optional[str] = None, suffix: Optional[str] = None, text_auto=None, update_period: Optional[float] = None)`*:
+*Method `UpdProxy.__init__(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x111360790>, **kw)`*:
 Initialise a new `UpdProxy` status line.
 
 Parameters:
 * `index`: optional position for the new proxy as for `Upd.insert`,
   default `1` (directly above the bottom status line)
 * `upd`: the `Upd` instance with which to associate this proxy,
   default the default `Upd` instance (associated with `sys.stderr`)
@@ -343,29 +353,36 @@
 
 Example:
 
     @with_upd_proxy
     def func(*a, upd_proxy:UpdProxy, **kw):
       ... perform task, updating upd_proxy ...
 
-## Function `without(*, upd: cs.upd.Upd)`
+## Function `without(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113613f0>, **kw)`
 
 Context manager withdraw the `Upd` while something runs.
 
 Example:
 
     from cs.upd import without
     ...
     with without():
         os.system('ls -la')
 
 # Release Log
 
 
 
+*Release 20240412*:
+* Upd.run_task: provide the label as the new UpdProxy prefix.
+* Upd.insert: the supplied txt is the proxy.text, not the prefix.
+* UpdProxy.text: setting to None sets to self._text_auto() if present or makes no change.
+* New @without decorator to withdraw the Upd during a function.
+* print: use the builtin print directly if the Upd is disabled.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240216*:
 New without() context manager to withdraw the Upd while something runs.
 
 *Release 20240201*:
@@ -553,7 +570,8 @@
 * Upd.nl,out: accept optional positional parameters, use with %-formatting if supplied, just like logging.
 
 *Release 20150118*:
 metadata fix
 
 *Release 20150116*:
 Initial PyPI release.
+
```

### Comparing `cs.upd-20240316/lib/python/cs/upd.py` & `cs.upd-20240412/lib/python/cs/upd.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 the default behaviour is that this mode activates
 if the backend is not a tty (as tested by `backend.isatty()`).
 The constructor has an optional parameter `disabled` to override
 this default behaviour.
 '''
 
 import atexit
-from builtins import print as builtin_print
+from builtins import breakpoint as builtin_breakpoint, print as builtin_print
 from contextlib import contextmanager
 from functools import partial
 import os
 import sys
 from threading import RLock, Thread
 import time
 from typing import Optional, Union
@@ -87,15 +87,15 @@
 
 try:
   import curses
 except ImportError as curses_e:
   warning("cannot import curses: %s", curses_e)
   curses = None
 
-__version__ = '20240316'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -158,39 +158,42 @@
     if backend is None:
       try:
         backend_path = os.environ[CS_UPD_BACKEND_ENVVAR]
       except KeyError:
         backend = sys.stderr
       else:
         backend = open_append(backend_path)
-    self._backend = backend
-    assert self._backend is not None
+    assert backend is not None
     # test isatty and the associated file descriptor
     isatty = backend.isatty()
     if isatty:
       try:
         backend_fd = backend.fileno()
       except OSError:
         backend_fd = None
         isatty = False
     else:
       backend_fd = None
+    self._backend_isatty = isatty
+    self._backend_fd = backend_fd
     if columns is None:
       columns = 80
-      if backend.isatty():
+      if isatty:
         rc = ttysize(backend)
         if rc.columns is not None:
           columns = rc.columns
     if disabled is None:
-      try:
-        disabled = not backend.isatty()
-      except AttributeError:
-        disabled = True
-    self._backend_isatty = isatty
-    self._backend_fd = backend_fd
+      disabled = not isatty
+    self._disabled = disabled
+    if disabled:
+      self._backend = None
+      self._disabled_backend = backend
+    else:
+      self._backend = backend
+      self._disabled_backend = None
     # prepare the terminfo capability mapping, if any
     self._ti_strs = {}
     if isatty:
       if curses is not None:
         try:
           # pylint: disable=no-member
           curses.setupterm(fd=backend_fd)
@@ -206,16 +209,14 @@
               'el',  # clear to end of line
           ):
             # pylint: disable=no-member
             s = curses.tigetstr(ti_name)
             if s is not None:
               s = s.decode('ascii')
             self._ti_strs[ti_name] = s
-    self._disabled = disabled
-    self._disabled_backend = None
     self.columns = columns
     self._cursor_visible = True
     self._current_slot = None
     self._lock = RLock()
     self._reset()
 
   def _reset(self):
@@ -226,15 +227,18 @@
     self._above = None
     self._slot_text = ['']
     proxy0 = UpdProxy(index=None, upd=self)
     self._proxies = [proxy0]
     proxy0.index = 0
 
   def __str__(self):
-    backend = self._disabled_backend if self._disabled else self._backend
+    backend = (
+        self._disabled_backend if getattr(self, '_disabled', False) else
+        getattr(self, '_backend', None)
+    )
     return "%s(backend=%s)" % (self.__class__.__name__, backend)
 
   ############################################################
   # Context manager methods.
   #
 
   def __enter_exit__(self):
@@ -663,15 +667,16 @@
         txts.append(slots[top_slot])
         self._current_slot = top_slot
       self._backend.write(''.join(txts))
       self._backend.flush()
 
   @contextmanager
   def above(self, need_newline=False):
-    ''' Context manager to move to the top line of the display, clear it, yield, redraw below.
+    ''' Context manager to move to the top line of the `Upd` display,
+        clear it, `yield`, redraw below.
 
         This context manager is for use when interleaving _another_
         stream with the `Upd` display;
         if you just want to write lines above the display
         for the same backend use `Upd.nl`.
 
         The usual situation for `Upd.above`
@@ -784,15 +789,15 @@
       elif index > len(self):
         raise ValueError(
             "index should be in the range 0..%d inclusive: got %s" %
             (len(self), index)
         )
       if proxy is None:
         # create the proxy, which inserts it
-        return UpdProxy(index=index, upd=self, prefix=txt, **proxy_kw)
+        return UpdProxy(txt, index=index, upd=self, **proxy_kw)
 
       # associate the proxy with self
       assert proxy.upd is None
       proxy.index = index
       proxy.upd = self
 
       # no display? just insert the slot
@@ -934,37 +939,34 @@
         It yields the proxy.
     '''
     if tick_delay < 0:
       raise ValueError(
           "run_task(%r,...,tick_delay=%s): tick_delay should be >=0" %
           (label, tick_delay)
       )
-    with self.insert(1, label + ' ') as proxy:
+    with self.insert(1, prefix=label + ' ') as proxy:
       ticker_runstate = None
       if tick_delay > 0:
-        from cs.resources import RunState  # pylint: disable=import-outside-toplevel
-        ticker_runstate = RunState()
+        cancel_ticker = False
 
         def _ticker():
           i = 0
-          while not ticker_runstate.cancelled:
+          while not cancel_ticker:
             proxy.suffix = ' ' + tick_chars[i % len(tick_chars)]
             i += 1
             time.sleep(tick_delay)
 
         Thread(target=_ticker, daemon=True).start()
       proxy.text = '...'
       start_time = time.time()
       try:
         yield proxy
       finally:
         end_time = time.time()
-        if ticker_runstate:
-          # shut down the ticker
-          ticker_runstate.cancel()
+        cancel_ticker = True
     elapsed_time = end_time - start_time
     if report_print:
       if isinstance(report_print, bool):
         report_print = print
       report_print(
           label + ': in',
           transcribe(elapsed_time, TIME_SCALE, max_parts=2, skip_zero=True)
@@ -977,40 +979,40 @@
       This also makes the `upd` the default `Upd` instance for this thread.
   '''
 
   def with_func(*a, upd: Upd, **kw):
     with upd:
       return func(*a, upd=upd, **kw)
 
-  return default_params(with_func, upd=lambda: Upd.default() or Upd())
+  return default_params(with_func, upd=lambda: Upd.default(factory=True))
 
 @uses_upd
 def out(msg, *a, upd, **outkw):
   ''' Update the status line of the default `Upd` instance.
       Parameters are as for `Upd.out()`.
   '''
   return upd.out(msg, *a, **outkw)
 
-# pylint: disable=redefined-builtin
-@uses_upd
-def print(*a, upd: Upd, end='\n', **kw):
-  ''' Wrapper for the builtin print function
-      to call it inside `Upd.above()` and enforce a flush.
+@decorator
+def without(func):
+  ''' A decorator to withdraw the current `Upd` (if any) while running `func`.
+  '''
 
-      The function supports an addition parameter beyond the builtin print:
-      * `upd`: the `Upd` instance to use, default `Upd()`
+  def _without_upd_wrapper(*a, **kw):
+    upd = Upd.default()
+    if upd is None or upd.disabled:
+      return func(*a, **kw)
+    with upd.above():
+      return func(*a, **kw)
 
-      Programmes integrating `cs.upd` with use of the builtin `print`
-      function should use this at import time:
+  return _without_upd_wrapper
 
-          from cs.upd import print
-  '''
-  kw['flush'] = True
-  with upd.above(need_newline=not end.endswith('\n')):
-    builtin_print(*a, end=end, **kw)
+# pylint: disable=redefined-builtin
+breakpoint = without(builtin_breakpoint)
+print = without(partial(builtin_print, flush=True))
 
 @uses_upd
 def pfxprint(*a, upd, **kw):
   ''' Wrapper for `cs.pfx.pfxprint` to pass `print_func=cs.upd.print`.
 
       Programmes integrating `cs.upd` with use of the `cs.pfx.pfxprint`
       function should use this at import time:
@@ -1019,15 +1021,15 @@
   '''
   # pylint: disable=import-outside-toplevel
   from cs.pfx import pfxprint as base_pfxprint
   return base_pfxprint(*a, print_func=partial(print, upd=upd), **kw)
 
 @contextmanager
 @uses_upd
-def run_task(*a, upd, **kw):
+def run_task(*a, upd: Upd, **kw):
   ''' Top level `run_task` function to call `Upd.run_task`.
   '''
   with upd.run_task(*a, **kw) as proxy:
     yield proxy
 
 @uses_upd
 def nl(msg, *a, upd, **kw):
@@ -1190,17 +1192,25 @@
     '''
     return self._text or ('' if self._text_auto is None else self._text_auto())
 
   @text.setter
   def text(self, txt):
     ''' Set the text of the status line.
 
+        If `txt` is `None`: if a `text_auto` function was supplied,
+        use it to compute `txt` otherwise do not change the text.
+
         If the length of `self.prefix+txt` exceeds the available display
         width then the leftmost text is cropped to fit.
     '''
+    if txt is None:
+      if self._text_auto:
+        txt = self._text_auto()
+      else:
+        return
     self._text = txt
     self._update()
 
   @property
   def suffix(self):
     ''' The current suffix string.
     '''
```

### Comparing `cs.upd-20240316/lib/python/cs.upd.egg-info/PKG-INFO` & `cs.upd-20240412/lib/python/cs.upd.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.upd
-Version: 20240316
+Version: 20240412
 Summary: Single and multiple line status updates with minimal update sequences.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,16 +14,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Single and multiple line status updates with minimal update sequences.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* Upd.run_task: provide the label as the new UpdProxy prefix.
+* Upd.insert: the supplied txt is the proxy.text, not the prefix.
+* UpdProxy.text: setting to None sets to self._text_auto() if present or makes no change.
+* New @without decorator to withdraw the Upd during a function.
+* print: use the builtin print directly if the Upd is disabled.
 
 This is available as an output mode in `cs.logutils`.
 
 Single line example:
 
     from cs.upd import Upd, nl, print
     .....
@@ -77,52 +81,39 @@
 The constructor has an optional parameter `disabled` to override
 this default behaviour.
 
 ## Function `demo()`
 
 A tiny demo function for visual checking of the basic functionality.
 
-## Function `nl(msg, *a, upd, **kw)`
+## Function `nl(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113604c0>, **kw)`
 
 Write `msg` to `file` (default `sys.stdout`),
 without interfering with the `Upd` instance.
 This is a thin shim for `Upd.print`.
 
-## Function `out(msg, *a, upd, **outkw)`
+## Function `out(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x11135ba30>, **kw)`
 
 Update the status line of the default `Upd` instance.
 Parameters are as for `Upd.out()`.
 
-## Function `pfxprint(*a, upd, **kw)`
+## Function `pfxprint(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x11135bf40>, **kw)`
 
 Wrapper for `cs.pfx.pfxprint` to pass `print_func=cs.upd.print`.
 
 Programmes integrating `cs.upd` with use of the `cs.pfx.pfxprint`
 function should use this at import time:
 
     from cs.upd import pfxprint
 
-## Function `print(*a, upd: cs.upd.Upd, end='\n', **kw)`
-
-Wrapper for the builtin print function
-to call it inside `Upd.above()` and enforce a flush.
-
-The function supports an addition parameter beyond the builtin print:
-* `upd`: the `Upd` instance to use, default `Upd()`
-
-Programmes integrating `cs.upd` with use of the builtin `print`
-function should use this at import time:
-
-    from cs.upd import print
-
-## Function `run_task(*a, upd, **kw)`
+## Function `run_task(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113601f0>, **kw)`
 
 Top level `run_task` function to call `Upd.run_task`.
 
-## Class `Upd(cs.obj.SingletonMixin, cs.resources.MultiOpenMixin, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `Upd(cs.obj.SingletonMixin, cs.resources.MultiOpenMixin, cs.threads.HasThreadState)`
 
 A `SingletonMixin` subclass for maintaining multiple status lines.
 
 The default backend is `sys.stderr`.
 
 *Method `Upd.__init__(self, backend=None, columns=None, disabled=None)`*:
 Initialise the `Upd`.
@@ -133,14 +124,160 @@
 * `columns`: the width of the output,
   default from the width of the `backend` tty if it is a tty,
   `80` otherwise
 * `disabled`: if true, disable the output - just keep state;
   default true if the output is not a tty;
   this automatically silences the `Upd` if stderr is not a tty
 
+*Method `Upd.__enter_exit__(self)`*:
+Generator supporting `__enter__` and `__exit__`.
+
+On shutdown, if we are exiting because of an exception
+which is not a `SystemExit` with a `code` of `None` or `0`
+then we preserve the status lines one screen.
+Otherwise we clean up the status lines.
+
+*Method `Upd.__getitem__(self, index)`*:
+The text of the status line at `index`.
+
+*Method `Upd.__len__(self)`*:
+The length of an `Upd` is the number of slots.
+
+*Method `Upd.above(self, need_newline=False)`*:
+Context manager to move to the top line of the `Upd` display,
+clear it, `yield`, redraw below.
+
+This context manager is for use when interleaving _another_
+stream with the `Upd` display;
+if you just want to write lines above the display
+for the same backend use `Upd.nl`.
+
+The usual situation for `Upd.above`
+is interleaving `sys.stdout` and `sys.stderr`,
+which are often attached to the same terminal.
+
+Note that the caller's output should be flushed
+before exiting the suite
+so that the output is completed before the `Upd` resumes.
+
+Example:
+
+    U = Upd()   # default sys.stderr Upd
+    ......
+    with U.above():
+        print('some message for stdout ...', flush=True)
+
+*Method `Upd.cursor_invisible(self)`*:
+Make the cursor vinisible.
+
+*Method `Upd.cursor_visible(self)`*:
+Make the cursor visible.
+
+*Method `Upd.delete(self, index)`*:
+Delete the status line at `index`.
+
+Return the `UpdProxy` of the deleted status line.
+
+*Method `Upd.diff(oldtxt, newtxt, columns, raw_text=False)`*:
+Compute the text sequences required to update `oldtxt` to `newtxt`
+presuming the cursor is at the right hand end of `oldtxt`.
+The available area is specified by `columns`.
+
+We normalise `newtxt` as using `self.normalise`.
+`oldtxt` is presumed to be already normalised.
+
+If `raw_text` is true (default `False`) we do not normalise `newtxt`
+before comparison.
+
+*Method `Upd.disable(self)`*:
+Disable updates.
+
+*Property `Upd.disabled`*:
+Whether this `Upd` is currently disabled.
+
+*Method `Upd.enable(self)`*:
+Enable updates.
+
+*Method `Upd.flush(self)`*:
+Flush the backend stream.
+
+*Method `Upd.insert(self, index, txt='', proxy=None, **proxy_kw) -> 'UpdProxy'`*:
+Insert a new status line at `index`.
+Return the `UpdProxy` for the new status line.
+
+*Method `Upd.nl(self, txt, *a, redraw=False)`*:
+Write `txt` to the backend followed by a newline.
+
+Parameters:
+* `txt`: the message to write.
+* `a`: optional positional parameters;
+  if not empty, `txt` is percent formatted against this list.
+* `redraw`: if true (default `False`) use the "redraw" method.
+
+This uses one of two methods:
+* insert above:
+  insert a line above the top status line and write the message there.
+* redraw:
+  clear the top slot, write txt and a newline,
+  redraw all the slots below.
+
+The latter method is used if `redraw` is true
+or if `txt` is wider than `self.columns`
+or if there is no "insert line" capability.
+
+*Method `Upd.normalise(txt)`*:
+Normalise `txt` for display,
+currently implemented as:
+`unctrl(txt.rstrip())`.
+
+*Method `Upd.out(self, txt, *a, slot=0, raw_text=False, redraw=False) -> str`*:
+Update the status line at `slot` to `txt`.
+Return the previous status line content.
+
+Parameters:
+* `txt`: the status line text.
+* `a`: optional positional parameters;
+  if not empty, `txt` is percent formatted against this list.
+* `slot`: which slot to update; default is `0`, the bottom slot
+* `raw_text`: if true (default `False`), do not normalise the text
+* `redraw`: if true (default `False`), redraw the whole line
+  instead of doing the minimal and less visually annoying
+  incremental change
+
+*`Upd.perthread_state`*
+
+*Method `Upd.proxy(self, index)`*:
+Return the `UpdProxy` for `index`.
+Returns `None` if `index` is out of range.
+The index `0` is never out of range;
+it will be autocreated if there are no slots yet.
+
+*Method `Upd.run_task(self, label: str, *, report_print=False, tick_delay: int = 0.3, tick_chars='|/-\\')`*:
+Context manager to display an `UpdProxy` for the duration of some task.
+It yields the proxy.
+
+*Method `Upd.selfcheck(self)`*:
+Sanity check the internal data structures.
+
+Warning: this uses asserts.
+
+*Method `Upd.shutdown(self, preserve_display=False)`*:
+Clean out this `Upd`, optionally preserving the displayed status lines.
+
+*Method `Upd.ti_str(self, ti_name)`*:
+Fetch the terminfo capability string named `ti_name`.
+Return the string or `None` if not available.
+
+*Method `Upd.without(self, temp_state='', slot=0)`*:
+Context manager to clear the status line around a suite.
+Returns the status line text as it was outside the suite.
+
+The `temp_state` parameter may be used to set the inner status line
+content if a value other than `''` is desired.
+
 ## Class `UpdProxy`
 
 A proxy for a status line of a multiline `Upd`.
 
 This provides a stable reference to a status line after it has been
 instantiated by `Upd.insert`.
 
@@ -150,24 +287,63 @@
 
     U = Upd()
     ....
     with U.insert(1, 'hello!') as proxy:
         .... set proxy.text as needed ...
     # proxy now removed
 
-*Method `UpdProxy.__init__(self, text: Optional[str] = None, *, upd: cs.upd.Upd, index: Optional[int] = 1, prefix: Optional[str] = None, suffix: Optional[str] = None, text_auto=None, update_period: Optional[float] = None)`*:
+*Method `UpdProxy.__init__(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x111360790>, **kw)`*:
 Initialise a new `UpdProxy` status line.
 
 Parameters:
 * `index`: optional position for the new proxy as for `Upd.insert`,
   default `1` (directly above the bottom status line)
 * `upd`: the `Upd` instance with which to associate this proxy,
   default the default `Upd` instance (associated with `sys.stderr`)
 * `text`: optional initial text for the new status line
 
+*Method `UpdProxy.__call__(self, msg, *a)`*:
+Calling the proxy sets its `.text` property
+in the form used by other messages: `(msg,*a)`
+
+*Method `UpdProxy.__del__(self)`*:
+Delete this proxy from its parent `Upd`.
+
+*Method `UpdProxy.delete(self)`*:
+Delete this proxy from its parent `Upd`.
+
+*Method `UpdProxy.extend_prefix(self, more_prefix, print_elapsed=False)`*:
+Context manager to append text to the prefix.
+
+*Method `UpdProxy.insert(self, index, txt='')`*:
+Insert a new `UpdProxy` at a position relative to this `UpdProxy`.
+Return the new proxy.
+
+This supports the positioning of related status lines.
+
+*Property `UpdProxy.prefix`*:
+The current prefix string.
+
+*Method `UpdProxy.reset(self)`*:
+Clear the proxy: set both the prefix and text to `''`.
+
+*Property `UpdProxy.suffix`*:
+The current suffix string.
+
+*Property `UpdProxy.text`*:
+The text of this proxy's slot, without the prefix.
+
+*Property `UpdProxy.width`*:
+The available space for text after `self.prefix` and before `self.suffix`.
+
+This is available width for uncropped text,
+intended to support presizing messages such as progress bars.
+Setting the text to something longer will crop the rightmost
+portion of the text which fits.
+
 ## Function `uses_upd(*da, **dkw)`
 
 Decorator for functions accepting an optional `upd:Upd` parameter,
 default from `Upd.default() or Upd()`.
 This also makes the `upd` the default `Upd` instance for this thread.
 
 ## Function `with_upd_proxy(*da, **dkw)`
@@ -177,29 +353,36 @@
 
 Example:
 
     @with_upd_proxy
     def func(*a, upd_proxy:UpdProxy, **kw):
       ... perform task, updating upd_proxy ...
 
-## Function `without(*, upd: cs.upd.Upd)`
+## Function `without(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113613f0>, **kw)`
 
 Context manager withdraw the `Upd` while something runs.
 
 Example:
 
     from cs.upd import without
     ...
     with without():
         os.system('ls -la')
 
 # Release Log
 
 
 
+*Release 20240412*:
+* Upd.run_task: provide the label as the new UpdProxy prefix.
+* Upd.insert: the supplied txt is the proxy.text, not the prefix.
+* UpdProxy.text: setting to None sets to self._text_auto() if present or makes no change.
+* New @without decorator to withdraw the Upd during a function.
+* print: use the builtin print directly if the Upd is disabled.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240216*:
 New without() context manager to withdraw the Upd while something runs.
 
 *Release 20240201*:
```

### Comparing `cs.upd-20240316/pyproject.toml` & `cs.upd-20240412/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,47 +5,51 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
-    "cs.context>=20240316",
-    "cs.deco>=20240316",
+    "cs.context>=20240412",
+    "cs.deco>=20240412",
     "cs.gimmicks>=20240316",
     "cs.lex>=20240316",
     "cs.obj>=20210122",
-    "cs.resources>=20240316",
-    "cs.threads>=20240303",
+    "cs.resources>=20240412",
+    "cs.threads>=20240412",
     "cs.tty",
     "cs.units",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240316"
+version = "20240412"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Single and multiple line status updates with minimal update sequences.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* Upd.run_task: provide the label as the new UpdProxy prefix.
+* Upd.insert: the supplied txt is the proxy.text, not the prefix.
+* UpdProxy.text: setting to None sets to self._text_auto() if present or makes no change.
+* New @without decorator to withdraw the Upd during a function.
+* print: use the builtin print directly if the Upd is disabled.
 
 This is available as an output mode in `cs.logutils`.
 
 Single line example:
 
     from cs.upd import Upd, nl, print
     .....
@@ -99,52 +103,39 @@
 The constructor has an optional parameter `disabled` to override
 this default behaviour.
 
 ## Function `demo()`
 
 A tiny demo function for visual checking of the basic functionality.
 
-## Function `nl(msg, *a, upd, **kw)`
+## Function `nl(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113604c0>, **kw)`
 
 Write `msg` to `file` (default `sys.stdout`),
 without interfering with the `Upd` instance.
 This is a thin shim for `Upd.print`.
 
-## Function `out(msg, *a, upd, **outkw)`
+## Function `out(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x11135ba30>, **kw)`
 
 Update the status line of the default `Upd` instance.
 Parameters are as for `Upd.out()`.
 
-## Function `pfxprint(*a, upd, **kw)`
+## Function `pfxprint(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x11135bf40>, **kw)`
 
 Wrapper for `cs.pfx.pfxprint` to pass `print_func=cs.upd.print`.
 
 Programmes integrating `cs.upd` with use of the `cs.pfx.pfxprint`
 function should use this at import time:
 
     from cs.upd import pfxprint
 
-## Function `print(*a, upd: cs.upd.Upd, end='\\n', **kw)`
-
-Wrapper for the builtin print function
-to call it inside `Upd.above()` and enforce a flush.
-
-The function supports an addition parameter beyond the builtin print:
-* `upd`: the `Upd` instance to use, default `Upd()`
-
-Programmes integrating `cs.upd` with use of the builtin `print`
-function should use this at import time:
-
-    from cs.upd import print
-
-## Function `run_task(*a, upd, **kw)`
+## Function `run_task(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113601f0>, **kw)`
 
 Top level `run_task` function to call `Upd.run_task`.
 
-## Class `Upd(cs.obj.SingletonMixin, cs.resources.MultiOpenMixin, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `Upd(cs.obj.SingletonMixin, cs.resources.MultiOpenMixin, cs.threads.HasThreadState)`
 
 A `SingletonMixin` subclass for maintaining multiple status lines.
 
 The default backend is `sys.stderr`.
 
 *Method `Upd.__init__(self, backend=None, columns=None, disabled=None)`*:
 Initialise the `Upd`.
@@ -155,14 +146,160 @@
 * `columns`: the width of the output,
   default from the width of the `backend` tty if it is a tty,
   `80` otherwise
 * `disabled`: if true, disable the output - just keep state;
   default true if the output is not a tty;
   this automatically silences the `Upd` if stderr is not a tty
 
+*Method `Upd.__enter_exit__(self)`*:
+Generator supporting `__enter__` and `__exit__`.
+
+On shutdown, if we are exiting because of an exception
+which is not a `SystemExit` with a `code` of `None` or `0`
+then we preserve the status lines one screen.
+Otherwise we clean up the status lines.
+
+*Method `Upd.__getitem__(self, index)`*:
+The text of the status line at `index`.
+
+*Method `Upd.__len__(self)`*:
+The length of an `Upd` is the number of slots.
+
+*Method `Upd.above(self, need_newline=False)`*:
+Context manager to move to the top line of the `Upd` display,
+clear it, `yield`, redraw below.
+
+This context manager is for use when interleaving _another_
+stream with the `Upd` display;
+if you just want to write lines above the display
+for the same backend use `Upd.nl`.
+
+The usual situation for `Upd.above`
+is interleaving `sys.stdout` and `sys.stderr`,
+which are often attached to the same terminal.
+
+Note that the caller's output should be flushed
+before exiting the suite
+so that the output is completed before the `Upd` resumes.
+
+Example:
+
+    U = Upd()   # default sys.stderr Upd
+    ......
+    with U.above():
+        print('some message for stdout ...', flush=True)
+
+*Method `Upd.cursor_invisible(self)`*:
+Make the cursor vinisible.
+
+*Method `Upd.cursor_visible(self)`*:
+Make the cursor visible.
+
+*Method `Upd.delete(self, index)`*:
+Delete the status line at `index`.
+
+Return the `UpdProxy` of the deleted status line.
+
+*Method `Upd.diff(oldtxt, newtxt, columns, raw_text=False)`*:
+Compute the text sequences required to update `oldtxt` to `newtxt`
+presuming the cursor is at the right hand end of `oldtxt`.
+The available area is specified by `columns`.
+
+We normalise `newtxt` as using `self.normalise`.
+`oldtxt` is presumed to be already normalised.
+
+If `raw_text` is true (default `False`) we do not normalise `newtxt`
+before comparison.
+
+*Method `Upd.disable(self)`*:
+Disable updates.
+
+*Property `Upd.disabled`*:
+Whether this `Upd` is currently disabled.
+
+*Method `Upd.enable(self)`*:
+Enable updates.
+
+*Method `Upd.flush(self)`*:
+Flush the backend stream.
+
+*Method `Upd.insert(self, index, txt='', proxy=None, **proxy_kw) -> 'UpdProxy'`*:
+Insert a new status line at `index`.
+Return the `UpdProxy` for the new status line.
+
+*Method `Upd.nl(self, txt, *a, redraw=False)`*:
+Write `txt` to the backend followed by a newline.
+
+Parameters:
+* `txt`: the message to write.
+* `a`: optional positional parameters;
+  if not empty, `txt` is percent formatted against this list.
+* `redraw`: if true (default `False`) use the \"redraw\" method.
+
+This uses one of two methods:
+* insert above:
+  insert a line above the top status line and write the message there.
+* redraw:
+  clear the top slot, write txt and a newline,
+  redraw all the slots below.
+
+The latter method is used if `redraw` is true
+or if `txt` is wider than `self.columns`
+or if there is no \"insert line\" capability.
+
+*Method `Upd.normalise(txt)`*:
+Normalise `txt` for display,
+currently implemented as:
+`unctrl(txt.rstrip())`.
+
+*Method `Upd.out(self, txt, *a, slot=0, raw_text=False, redraw=False) -> str`*:
+Update the status line at `slot` to `txt`.
+Return the previous status line content.
+
+Parameters:
+* `txt`: the status line text.
+* `a`: optional positional parameters;
+  if not empty, `txt` is percent formatted against this list.
+* `slot`: which slot to update; default is `0`, the bottom slot
+* `raw_text`: if true (default `False`), do not normalise the text
+* `redraw`: if true (default `False`), redraw the whole line
+  instead of doing the minimal and less visually annoying
+  incremental change
+
+*`Upd.perthread_state`*
+
+*Method `Upd.proxy(self, index)`*:
+Return the `UpdProxy` for `index`.
+Returns `None` if `index` is out of range.
+The index `0` is never out of range;
+it will be autocreated if there are no slots yet.
+
+*Method `Upd.run_task(self, label: str, *, report_print=False, tick_delay: int = 0.3, tick_chars='|/-\\\\')`*:
+Context manager to display an `UpdProxy` for the duration of some task.
+It yields the proxy.
+
+*Method `Upd.selfcheck(self)`*:
+Sanity check the internal data structures.
+
+Warning: this uses asserts.
+
+*Method `Upd.shutdown(self, preserve_display=False)`*:
+Clean out this `Upd`, optionally preserving the displayed status lines.
+
+*Method `Upd.ti_str(self, ti_name)`*:
+Fetch the terminfo capability string named `ti_name`.
+Return the string or `None` if not available.
+
+*Method `Upd.without(self, temp_state='', slot=0)`*:
+Context manager to clear the status line around a suite.
+Returns the status line text as it was outside the suite.
+
+The `temp_state` parameter may be used to set the inner status line
+content if a value other than `''` is desired.
+
 ## Class `UpdProxy`
 
 A proxy for a status line of a multiline `Upd`.
 
 This provides a stable reference to a status line after it has been
 instantiated by `Upd.insert`.
 
@@ -172,24 +309,63 @@
 
     U = Upd()
     ....
     with U.insert(1, 'hello!') as proxy:
         .... set proxy.text as needed ...
     # proxy now removed
 
-*Method `UpdProxy.__init__(self, text: Optional[str] = None, *, upd: cs.upd.Upd, index: Optional[int] = 1, prefix: Optional[str] = None, suffix: Optional[str] = None, text_auto=None, update_period: Optional[float] = None)`*:
+*Method `UpdProxy.__init__(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x111360790>, **kw)`*:
 Initialise a new `UpdProxy` status line.
 
 Parameters:
 * `index`: optional position for the new proxy as for `Upd.insert`,
   default `1` (directly above the bottom status line)
 * `upd`: the `Upd` instance with which to associate this proxy,
   default the default `Upd` instance (associated with `sys.stderr`)
 * `text`: optional initial text for the new status line
 
+*Method `UpdProxy.__call__(self, msg, *a)`*:
+Calling the proxy sets its `.text` property
+in the form used by other messages: `(msg,*a)`
+
+*Method `UpdProxy.__del__(self)`*:
+Delete this proxy from its parent `Upd`.
+
+*Method `UpdProxy.delete(self)`*:
+Delete this proxy from its parent `Upd`.
+
+*Method `UpdProxy.extend_prefix(self, more_prefix, print_elapsed=False)`*:
+Context manager to append text to the prefix.
+
+*Method `UpdProxy.insert(self, index, txt='')`*:
+Insert a new `UpdProxy` at a position relative to this `UpdProxy`.
+Return the new proxy.
+
+This supports the positioning of related status lines.
+
+*Property `UpdProxy.prefix`*:
+The current prefix string.
+
+*Method `UpdProxy.reset(self)`*:
+Clear the proxy: set both the prefix and text to `''`.
+
+*Property `UpdProxy.suffix`*:
+The current suffix string.
+
+*Property `UpdProxy.text`*:
+The text of this proxy's slot, without the prefix.
+
+*Property `UpdProxy.width`*:
+The available space for text after `self.prefix` and before `self.suffix`.
+
+This is available width for uncropped text,
+intended to support presizing messages such as progress bars.
+Setting the text to something longer will crop the rightmost
+portion of the text which fits.
+
 ## Function `uses_upd(*da, **dkw)`
 
 Decorator for functions accepting an optional `upd:Upd` parameter,
 default from `Upd.default() or Upd()`.
 This also makes the `upd` the default `Upd` instance for this thread.
 
 ## Function `with_upd_proxy(*da, **dkw)`
@@ -199,29 +375,36 @@
 
 Example:
 
     @with_upd_proxy
     def func(*a, upd_proxy:UpdProxy, **kw):
       ... perform task, updating upd_proxy ...
 
-## Function `without(*, upd: cs.upd.Upd)`
+## Function `without(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x1113613f0>, **kw)`
 
 Context manager withdraw the `Upd` while something runs.
 
 Example:
 
     from cs.upd import without
     ...
     with without():
         os.system('ls -la')
 
 # Release Log
 
 
 
+*Release 20240412*:
+* Upd.run_task: provide the label as the new UpdProxy prefix.
+* Upd.insert: the supplied txt is the proxy.text, not the prefix.
+* UpdProxy.text: setting to None sets to self._text_auto() if present or makes no change.
+* New @without decorator to withdraw the Upd during a function.
+* print: use the builtin print directly if the Upd is disabled.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240216*:
 New without() context manager to withdraw the Upd while something runs.
 
 *Release 20240201*:
```

