# Comparing `tmp/cs.cmdutils-20240316.tar.gz` & `tmp/cs.cmdutils-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.cmdutils-20240316.tar", last modified: Sat Mar 16 06:46:39 2024, max compression
+gzip compressed data, was "cs.cmdutils-20240412.tar", last modified: Fri Apr 12 05:25:38 2024, max compression
```

## Comparing `cs.cmdutils-20240316.tar` & `cs.cmdutils-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:46:39.967446 cs.cmdutils-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:45:58.000000 cs.cmdutils-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    17471 2024-03-16 06:46:39.966963 cs.cmdutils-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    29247 2024-03-16 06:46:12.000000 cs.cmdutils-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:46:39.960429 cs.cmdutils-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:46:39.960742 cs.cmdutils-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:46:39.963433 cs.cmdutils-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    50830 2024-03-16 06:45:40.000000 cs.cmdutils-20240316/lib/python/cs/cmdutils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:46:39.966427 cs.cmdutils-20240316/lib/python/cs.cmdutils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    17471 2024-03-16 06:46:39.000000 cs.cmdutils-20240316/lib/python/cs.cmdutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      291 2024-03-16 06:46:39.000000 cs.cmdutils-20240316/lib/python/cs.cmdutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:46:39.000000 cs.cmdutils-20240316/lib/python/cs.cmdutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      233 2024-03-16 06:46:39.000000 cs.cmdutils-20240316/lib/python/cs.cmdutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:46:39.000000 cs.cmdutils-20240316/lib/python/cs.cmdutils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    18160 2024-03-16 06:46:38.000000 cs.cmdutils-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:46:39.967593 cs.cmdutils-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.222527 cs.cmdutils-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:24:59.000000 cs.cmdutils-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    30680 2024-04-12 05:25:38.222192 cs.cmdutils-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    29810 2024-04-12 05:25:12.000000 cs.cmdutils-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.217738 cs.cmdutils-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.217991 cs.cmdutils-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.219329 cs.cmdutils-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    50878 2024-04-12 05:24:48.000000 cs.cmdutils-20240412/lib/python/cs/cmdutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.221723 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    30680 2024-04-12 05:25:37.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      291 2024-04-12 05:25:38.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:25:37.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      231 2024-04-12 05:25:38.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:25:38.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    31399 2024-04-12 05:25:36.000000 cs.cmdutils-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:25:38.222625 cs.cmdutils-20240412/setup.cfg
```

### Comparing `cs.cmdutils-20240316/README.md` & `cs.cmdutils-20240412/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20240316*:
-* New @uses_cmd_options decorator to provide an "options" parameter being the prevailing BaseCommandOptions instance.
-* BaseCommandOptions.popopts: get common options from BaseCommandOptions.COMMON_OPT_SPECS.
+*Latest release 20240412*:
+* BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
+* BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -230,14 +230,17 @@
 this can be overridden with a method which just returns `False`.
 
 Otherwise,
 the handler may perform any suitable action
 and return `True` to contain the exception
 or `False` to cause the exception to be reraised.
 
+*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10d5b1d80>)`*:
+The default signal handler, which cancels the default `RunState`.
+
 *Method `BaseCommand.poparg(argv: List[str], *a, unpop_on_error=False)`*:
 Pop the leading argument off `argv` and parse it.
 Return the parsed argument.
 Raises `getopt.GetoptError` on a missing or invalid argument.
 
 This is expected to be used inside a `main` or `cmd_*`
 command handler method or inside `apply_preargv`.
@@ -417,15 +420,15 @@
 Otherwise `self.main(argv)` is called
 and its value returned.
 
 If the command implementation requires some setup or teardown
 then this may be provided by the `run_context()`
 context manager method.
 
-*Method `BaseCommand.run_context(self, *, runstate: cs.resources.RunState, upd: cs.upd.Upd, **kw_options)`*:
+*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x10d48e290>, **kw)`*:
 The context manager which surrounds `main` or `cmd_`*subcmd*.
 
 This default does several things, and subclasses should
 override it like this:
 
     @contextmanager
     def run_context(self):
@@ -466,15 +469,15 @@
 A `cmd.Cmd` subclass used to provide interactive use of a
 command's subcommands.
 
 The `BaseCommand.cmdloop()` class method instantiates an
 instance of this cand calls its `.cmdloop()` method
 i.e. `cmd.Cmd.cmdloop`.
 
-## Class `BaseCommandOptions(cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `BaseCommandOptions(cs.threads.HasThreadState)`
 
 A base class for the `BaseCommand` `options` object.
 
 This is the default class for the `self.options` object
 available during `BaseCommand.run()`,
 and available as the `BaseCommand.Options` attribute.
 
@@ -614,14 +617,18 @@
             print("doing f with x =", x)
         ....
 
 # Release Log
 
 
 
+*Release 20240412*:
+* BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
+* BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
+
 *Release 20240316*:
 * New @uses_cmd_options decorator to provide an "options" parameter being the prevailing BaseCommandOptions instance.
 * BaseCommandOptions.popopts: get common options from BaseCommandOptions.COMMON_OPT_SPECS.
 
 *Release 20240211*:
 * Include the first sentence of the subcommand description in the short help.
 * BaseCommandOptions: move the runstate_signals into this directly.
```

### Comparing `cs.cmdutils-20240316/lib/python/cs/cmdutils.py` & `cs.cmdutils-20240412/lib/python/cs/cmdutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from inspect import isclass, ismethod
 from os.path import basename
 try:
   import readline  # pylint: disable=unused-import
 except ImportError:
   pass
 import shlex
-from signal import SIGHUP, SIGINT, SIGTERM
+from signal import SIGHUP, SIGINT, SIGQUIT, SIGTERM
 import sys
 from typing import Callable, List, Mapping, Optional, Tuple
 
 from typeguard import typechecked
 
 from cs.context import stackattrs
 from cs.deco import default_params, fmtdoc, Promotable
@@ -44,15 +44,15 @@
 from cs.py.doc import obj_docstring
 from cs.resources import RunState, uses_runstate
 from cs.result import CancellationError
 from cs.threads import HasThreadState, ThreadState
 from cs.typingutils import subtype
 from cs.upd import Upd, uses_upd
 
-__version__ = '20240316'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -154,25 +154,26 @@
     '''
     prefix = command_cls.SUBCOMMAND_METHOD_PREFIX
     subcommands_map = {}
     for attr in dir(command_cls):
       if attr.startswith(prefix):
         subcmd = cutprefix(attr, prefix)
         method = getattr(command_cls, attr)
-        subcommands_map[subcmd] = (
-            _ClassSubCommand(
-                subcmd,
-                method,
-                usage_mapping=dict(getattr(method, 'USAGE_KEYWORDS', ()))
-            ) if isclass(method) else _MethodSubCommand(
-                subcmd,
-                method,
-                usage_mapping=dict(getattr(command_cls, 'USAGE_KEYWORDS', ()))
-            )
-        )
+        if isclass(method):
+          subcommands_map[subcmd] = _ClassSubCommand(
+              subcmd,
+              method,
+              usage_mapping=dict(getattr(method, 'USAGE_KEYWORDS', ())),
+          )
+        else:
+          subcommands_map[subcmd] = _MethodSubCommand(
+              subcmd,
+              method,
+              usage_mapping=dict(getattr(command_cls, 'USAGE_KEYWORDS', ())),
+          )
     return subcommands_map
 
   def usage_text(
       self,
       short: bool,
       usage_format_mapping: Optional[Mapping] = None
   ) -> str:
@@ -248,15 +249,15 @@
 
   def __call__(
       self, subcmd: str, command: "BaseCommandSubType", argv: List[str]
   ):
     subcmd_class = self.method
     updates = dict(command.options.__dict__)
     updates.update(cmd=subcmd)
-    command = subcmd_class(argv, **updates)
+    command = pfx_call(subcmd_class, argv, **updates)
     return command.run()
 
   def usage_format(self) -> str:
     ''' Return the usage format string from the class.
     '''
     doc = self.method.usage_text(cmd=self.cmd)
     subusage_format, *_ = cutprefix(doc, 'Usage:').lstrip().split("\n\n", 1)
@@ -292,43 +293,45 @@
       Since `BaseCommandOptions` is a data class, this typically looks like:
 
           @dataclass
           class Options(BaseCommand.Options):
               ... optional extra fields etc ...
   '''
 
-  DEFAULT_SIGNALS = SIGHUP, SIGINT, SIGTERM
+  DEFAULT_SIGNALS = SIGHUP, SIGINT, SIGQUIT, SIGTERM
   COMMON_OPT_SPECS = _COMMON_OPT_SPECS
 
   cmd: Optional[str] = None
   dry_run: bool = False
   force: bool = False
   quiet: bool = False
-  runstate: Optional[RunState] = None
   runstate_signals: Tuple[int] = DEFAULT_SIGNALS
   verbose: bool = False
+
   perthread_state = ThreadState()
 
   def copy(self, **updates):
     ''' Return a new instance of `BaseCommandOptions` (well, `type(self)`)
         which is a shallow copy of the public attributes from `self.__dict__`.
 
         Any keyword arguments are applied as attribute updates to the copy.
     '''
-    copied = type(self)(
+    copied = pfx_call(
+        type(self),
         **{
             k: v
             for k, v in self.__dict__.items()
             if not k.startswith('_')
-        }
+        },
     )
     for k, v in updates.items():
       setattr(copied, k, v)
     return copied
 
+  # TODO: remove this - the overt make-a-copy-and-with-the-copy is clearer
   @contextmanager
   def __call__(self, **updates):
     ''' Calling the options object returns a context manager whose
         value is a copy of the options with any `suboptions` applied.
 
         Example showing the semantics:
 
@@ -632,15 +635,15 @@
     if cmd is None:
       cmd = basename(argv0)
     self.cmd = cmd
     log_level = getattr(options, 'log_level', None)
     loginfo = setup_logging(cmd, level=log_level)
     # post: argv is list of arguments after the command name
     self.loginfo = loginfo
-    options = self.options = self.Options()
+    options = self.options = self.Options(cmd=self.cmd)
     # override the default options
     for option, value in kw_options.items():
       setattr(options, option, value)
     self._argv = argv
     self._run = lambda subcmd, command, argv: 2
     self._subcmd = None
     self._printed_usage = False
@@ -1282,14 +1285,20 @@
         or `False` to cause the exception to be reraised.
     '''
     warning("%s", e)
     if usage:
       print(usage.rstrip(), file=sys.stderr)
     return True
 
+  @uses_runstate
+  def handle_signal(self, sig, frame, *, runstate: RunState):
+    ''' The default signal handler, which cancels the default `RunState`.
+    '''
+    runstate.cancel()
+
   @contextmanager
   @uses_runstate
   @uses_upd
   def run_context(self, *, runstate: RunState, upd: Upd, **kw_options):
     ''' The context manager which surrounds `main` or `cmd_`*subcmd*.
 
         This default does several things, and subclasses should
@@ -1302,30 +1311,26 @@
                   ... subclass context setup ...
                     yield
                 finally:
                   ... any unconditional cleanup ...
     '''
     # redundant try/finally to remind subclassers of correct structure
     try:
-      options = self.options
-      kw_options.setdefault('runstate', runstate)
-      kw_options.setdefault('upd', upd)
-      with options(**kw_options) as run_options:
-        with run_options:  # make the default ThreadState
-          with stackattrs(self, options=run_options):
-            handle_signal = getattr(
-                self, 'handle_signal', lambda *_: runstate.cancel()
-            )
-            with stackattrs(self, cmd=self._subcmd or self.cmd):
-              with upd:
-                with runstate:
-                  with runstate.catch_signal(options.runstate_signals,
-                                             call_previous=False,
-                                             handle_signal=handle_signal):
-                    yield
+      run_options = self.options.copy(**kw_options)
+      with run_options:  # make the default ThreadState
+        with stackattrs(self, options=run_options):
+          with stackattrs(self, cmd=self._subcmd or self.cmd):
+            with upd:
+              with runstate:
+                with runstate.catch_signal(
+                    run_options.runstate_signals,
+                    call_previous=False,
+                    handle_signal=self.handle_signal,
+                ):
+                  yield
 
     finally:
       pass
 
   # pylint: disable=unused-argument
   @classmethod
   def cmd_help(cls, argv):
```

