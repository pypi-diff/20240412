# Comparing `tmp/cs.progress-20230401.tar.gz` & `tmp/cs.progress-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.progress-20230401.tar", last modified: Sat Apr  1 05:07:04 2023, max compression
+gzip compressed data, was "cs.progress-20240412.tar", last modified: Fri Apr 12 05:06:10 2024, max compression
```

## Comparing `cs.progress-20230401.tar` & `cs.progress-20240412.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:07:04.538665 cs.progress-20230401/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-04-01 05:06:23.000000 cs.progress-20230401/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    10508 2023-04-01 05:07:04.538828 cs.progress-20230401/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    16599 2023-04-01 05:06:31.000000 cs.progress-20230401/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:07:04.533384 cs.progress-20230401/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:07:04.533755 cs.progress-20230401/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:07:04.535845 cs.progress-20230401/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    36512 2023-04-01 05:06:05.000000 cs.progress-20230401/lib/python/cs/progress.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:07:04.538392 cs.progress-20230401/lib/python/cs.progress.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    10508 2023-04-01 05:07:04.000000 cs.progress-20230401/lib/python/cs.progress.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      310 2023-04-01 05:07:04.000000 cs.progress-20230401/lib/python/cs.progress.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-04-01 05:07:04.000000 cs.progress-20230401/lib/python/cs.progress.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      114 2023-04-01 05:07:04.000000 cs.progress-20230401/lib/python/cs.progress.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-04-01 05:07:04.000000 cs.progress-20230401/lib/python/cs.progress.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    10831 2023-04-01 05:06:55.000000 cs.progress-20230401/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1032 2023-04-01 05:07:04.539464 cs.progress-20230401/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-04-01 05:06:31.000000 cs.progress-20230401/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:06:10.009623 cs.progress-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:05:39.000000 cs.progress-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    21486 2024-04-12 05:06:10.009370 cs.progress-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    20628 2024-04-12 05:05:49.000000 cs.progress-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:06:10.006353 cs.progress-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:06:10.006578 cs.progress-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:06:10.007625 cs.progress-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    34300 2024-04-12 05:05:26.000000 cs.progress-20240412/lib/python/cs/progress.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:06:10.009003 cs.progress-20240412/lib/python/cs.progress.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    21486 2024-04-12 05:06:09.000000 cs.progress-20240412/lib/python/cs.progress.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      291 2024-04-12 05:06:09.000000 cs.progress-20240412/lib/python/cs.progress.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:06:09.000000 cs.progress-20240412/lib/python/cs.progress.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      145 2024-04-12 05:06:09.000000 cs.progress-20240412/lib/python/cs.progress.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:06:09.000000 cs.progress-20240412/lib/python/cs.progress.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    22042 2024-04-12 05:06:08.000000 cs.progress-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:06:10.009706 cs.progress-20240412/setup.cfg
```

### Comparing `cs.progress-20230401/README.md` & `cs.progress-20240412/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 A progress tracker with methods for throughput, ETA and update notification;
 also a compound progress meter composed from other progress meters.
 
-*Latest release 20230401*:
-progressbar, BaseProgress.iterbar: use @uses_upd to provide a context Upd instance.
+*Latest release 20240412*:
+* BaseProgress.status: fixes for the arrow_width computation.
+* BaseProgress.bar: drop existing UpdProxy support, drop deferred, implement update_period using a ticker Thread.
+* BaseProgress.bar: set update_period=DEFAULT_UPDATE_PERIOD by default.
+* Progress.iterbar: drop preexisting UpdProxy support, update_frequency and update_min_size support.
+* Progress: new advance_total(delta) method so that we have a callable for this.
+* BaseProgress.bar: new optional poll parameter accepting a callable accepting a BaseProgress to update the state before updating the bar display.
+* BaseProgress.bar: new stalled='stalled' parameter to specify the term for no recent throughput, workers might prefer 'idle'.
+* progressbar() updated to match.
 
 ## Function `auto_progressbar(*da, **dkw)`
 
 Decorator for a function accepting an optional `progress`
 keyword parameter.
 If `progress` is `None` and the default `Upd` is not disabled,
 run the function with a progress bar.
@@ -49,41 +56,39 @@
 A Progress is less then another object `other`
 if its position is less than `int(other)`.
 
 *Method `BaseProgress.arrow(self, width, no_padding=False)`*:
 Construct a progress arrow representing completion
 to fit in the specified `width`.
 
-*Method `BaseProgress.bar(self, label=None, *, upd=None, proxy=None, statusfunc=None, width=None, window=None, report_print=None, insert_pos=1, deferred=False)`*:
+*Method `BaseProgress.bar(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x110fbd6c0>, **kw)`*:
 A context manager to create and withdraw a progress bar.
 It returns the `UpdProxy` which displays the progress bar.
 
 Parameters:
 * `label`: a label for the progress bar,
   default from `self.name`.
-* `proxy`: an optional `UpdProxy` to display the progress bar
-* `upd`: an optional `cs.upd.Upd` instance,
-  used to produce the progress bar status line if not supplied.
-  The default `upd` is `cs.upd.Upd()`
-  which uses `sys.stderr` for display.
 * `statusfunc`: an optional function to compute the progress bar text
   accepting `(self,label,width)`.
 * `width`: an optional width expressing how wide the progress bar
   text may be.
   The default comes from the `proxy.width` property.
-* `window`: optional timeframe to define "recent" in seconds;
+* `recent_window`: optional timeframe to define "recent" in seconds;
   if the default `statusfunc` (`Progress.status`) is used
   this is passed to it
 * `report_print`: optional `print` compatible function
   with which to write a report on completion;
   this may also be a `bool`, which if true will use `Upd.print`
   in order to interoperate with `Upd`.
+* `stalled`: optional string to replace the word `'stalled'`
+  in the status line; for a worked this might be betteer as `'idle'`
 * `insert_pos`: where to insert the progress bar, default `1`
-* `deferred`: optional flag; if true do not create the
-  progress bar until the first update occurs.
+* `poll`: an optional callable accepting a `BaseProgress`
+  which can be used to update the progress state before
+  updating the progress bar display
 
 Example use:
 
     # display progress reporting during upload_filename()
     # which updates the supplied Progress instance
     # during its operation
     P = Progress(name=label)
@@ -98,14 +103,57 @@
 
 If `remaining_time` is `None`, this is also `None`.
 
 *Method `BaseProgress.format_counter(self, value, scale=None, max_parts=2, sep=',', **kw)`*:
 Format `value` accoridng to `scale` and `max_parts`
 using `cs.units.transcribe`.
 
+*Method `BaseProgress.iterbar(self, it, label=None, *, itemlenfunc=None, incfirst=False, update_period=0.3, **bar_kw)`*:
+An iterable progress bar: a generator yielding values
+from the iterable `it` while updating a progress bar.
+
+Parameters:
+* `it`: the iterable to consume and yield.
+* `label`: a label for the progress bar,
+  default from `self.name`.
+* `itemlenfunc`: an optional function returning the "size" of each item
+  from `it`, used to advance `self.position`.
+  The default is to assume a size of `1`.
+  A convenient alternative choice may be the builtin function `len`.
+* `incfirst`: whether to advance `self.position` before we
+  `yield` an item from `it` or afterwards.
+  This reflects whether it is considered that progress is
+  made as items are obtained or only after items are processed
+  by whatever is consuming this generator.
+  The default is `False`, advancing after processing.
+* `update_period`: default `DEFAULT_UPDATE_PERIOD`; if `0`
+  then update on every iteration, otherwise every `update_period`
+  seconds
+Other parameters are passed to `Progress.bar`.
+
+Example use:
+
+    from cs.units import DECIMAL_SCALE
+    rows = [some list of data]
+    P = Progress(total=len(rows), units_scale=DECIMAL_SCALE)
+    for row in P.iterbar(rows, incfirst=True):
+        ... do something with each row ...
+
+    f = open(data_filename, 'rb')
+    datalen = os.stat(f).st_size
+    def readfrom(f):
+        while True:
+            bs = f.read(65536)
+            if not bs:
+                break
+            yield bs
+    P = Progress(total=datalen)
+    for bs in P.iterbar(readfrom(f), itemlenfunc=len):
+        ... process the file data in bs ...
+
 *Property `BaseProgress.ratio`*:
 The fraction of progress completed: `(position-start)/(total-start)`.
 Returns `None` if `total` is `None` or `total<=start`.
 
 Example:
 
     >>> P = Progress()
@@ -119,25 +167,27 @@
 
 *Property `BaseProgress.remaining_time`*:
 The projected time remaining to end
 based on the `throughput` and `total`.
 
 If `total` is `None`, this is `None`.
 
-*Method `BaseProgress.status(self, label, width, window=None)`*:
+*Method `BaseProgress.status(self, label, width, recent_window=None, stalled=None)`*:
 A progress string of the form:
 *label*`: `*pos*`/`*total*` ==>  ETA '*time*
 
 Parameters:
 * `label`: the label for the status line;
   if `None` use `self.name`
 * `width`: the available width for the status line;
   if not an `int` use `width.width`
-* `window`: optional timeframe to define "recent" in seconds,
+* `recent_window`: optional timeframe to define "recent" in seconds,
   default : `5`
+* `stalled`: the label to indicate no throughput, default `'stalled'`;
+  for a worker this might often b better as `'idle'`
 
 *Method `BaseProgress.text_pos_of_total(self, fmt=None, fmt_pos=None, fmt_total=None, pos_first=False)`*:
 Return a "total:position" or "position/total" style progress string.
 
 Parameters:
 * `fmt`: format string interpolating `pos_text` and `total_text`.
   Default: `"{pos_text}/{total_text}"` if `pos_first`,
@@ -326,14 +376,17 @@
 >>> P.advance(4)
 >>> P.position
 4
 >>> P.advance(4)
 >>> P.position
 8
 
+*Method `Progress.advance_total(self, delta)`*:
+Function form of addition to the total.
+
 *Property `Progress.latest`*:
 Latest datum.
 
 *Property `Progress.position`*:
 Latest position.
 
 *Property `Progress.throughput`*:
@@ -358,22 +411,57 @@
 >>> P = Progress()
 >>> P.position
 0
 >>> P.update(12)
 >>> P.position
 12
 
+## Function `progressbar(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x110fbedd0>, **kw)`
+
+Convenience function to construct and run a `Progress.iterbar`
+wrapping the iterable `it`,
+issuing and withdrawning a progress bar during the iteration.
+
+Parameters:
+* `it`: the iterable to consume
+* `label`: optional label, doubles as the `Progress.name`
+* `position`: optional starting position
+* `total`: optional value for `Progress.total`,
+  default from `len(it)` if supported.
+* `units_scale`: optional units scale for `Progress`,
+  default `UNSCALED_SCALE`
+
+If `total` is `None` and `it` supports `len()`
+then the `Progress.total` is set from it.
+
+All arguments are passed through to `Progress.iterbar`.
+
+Example use:
+
+    for row in progressbar(rows):
+        ... do something with row ...
+
 ## Function `selftest(argv)`
 
 Exercise some of the functionality.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* BaseProgress.status: fixes for the arrow_width computation.
+* BaseProgress.bar: drop existing UpdProxy support, drop deferred, implement update_period using a ticker Thread.
+* BaseProgress.bar: set update_period=DEFAULT_UPDATE_PERIOD by default.
+* Progress.iterbar: drop preexisting UpdProxy support, update_frequency and update_min_size support.
+* Progress: new advance_total(delta) method so that we have a callable for this.
+* BaseProgress.bar: new optional poll parameter accepting a callable accepting a BaseProgress to update the state before updating the bar display.
+* BaseProgress.bar: new stalled='stalled' parameter to specify the term for no recent throughput, workers might prefer 'idle'.
+* progressbar() updated to match.
+
 *Release 20230401*:
 progressbar, BaseProgress.iterbar: use @uses_upd to provide a context Upd instance.
 
 *Release 20230212*:
 BaseProgress: new update_period=0.2 parameter to constraint updates by elapsed time.
 
 *Release 20221207*:
```

### Comparing `cs.progress-20230401/lib/python/cs/progress.py` & `cs.progress-20240412/lib/python/cs/progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,54 +12,61 @@
 
 from collections import namedtuple
 from contextlib import contextmanager
 import functools
 import sys
 from threading import RLock
 import time
-from typing import Optional
+from typing import Callable, Optional
 
+from icontract import ensure
 from typeguard import typechecked
 
 from cs.deco import decorator
 from cs.logutils import debug, exception
 from cs.py.func import funcname
 from cs.seq import seq
+from cs.threads import bg
 from cs.units import (
     transcribe_time,
-    transcribe,
+    transcribe as transcribe_units,
     BINARY_BYTES_SCALE,
     DECIMAL_SCALE,
     TIME_SCALE,
     UNSCALED_SCALE,
 )
 from cs.upd import Upd, uses_upd, print  # pylint: disable=redefined-builtin
 
-__version__ = '20230401'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': [
         'cs.deco',
         'cs.logutils',
         'cs.py.func',
         'cs.seq',
+        'cs.threads',
         'cs.units',
         'cs.upd',
+        'icontract',
         'typeguard',
     ],
 }
 
 # default to 5s of position buffer for computing recent thoroughput
 DEFAULT_THROUGHPUT_WINDOW = 5
 
+# default update period
+DEFAULT_UPDATE_PERIOD = 0.3
+
 @functools.total_ordering
 class BaseProgress(object):
   ''' The base class for `Progress` and `OverProcess`
       with various common methods.
 
       Note that durations are in seconds
       and that absolute time is in seconds since the UNIX epoch
@@ -220,14 +227,15 @@
         If `remaining_time` is `None`, this is also `None`.
     '''
     remaining = self.remaining_time
     if remaining is None:
       return None
     return time.time() + remaining
 
+  @ensure(lambda width, result: len(result) <= width)
   def arrow(self, width, no_padding=False):
     ''' Construct a progress arrow representing completion
         to fit in the specified `width`.
     '''
     if width < 1:
       return ''
     ratio = self.ratio
@@ -249,15 +257,15 @@
     ''' Format `value` accoridng to `scale` and `max_parts`
         using `cs.units.transcribe`.
     '''
     if scale is None:
       scale = self.units_scale
     if scale is None:
       return str(value)
-    return transcribe(value, scale, max_parts=max_parts, sep=sep, **kw)
+    return transcribe_units(value, scale, max_parts=max_parts, sep=sep, **kw)
 
   def text_pos_of_total(
       self, fmt=None, fmt_pos=None, fmt_total=None, pos_first=False
   ):
     ''' Return a "total:position" or "position/total" style progress string.
 
         Parameters:
@@ -278,64 +286,70 @@
     if fmt is None:
       fmt = "{pos_text}/{total_text}" if pos_first else "{total_text}:{pos_text}"
     pos_text = fmt_pos(self.position)
     total_text = fmt_pos(self.total)
     return fmt.format(pos_text=pos_text, total_text=total_text)
 
   # pylint: disable=too-many-branches,too-many-statements
-  def status(self, label, width, window=None):
+  def status(self, label, width, recent_window=None, stalled=None):
     ''' A progress string of the form:
         *label*`: `*pos*`/`*total*` ==>  ETA '*time*
 
         Parameters:
         * `label`: the label for the status line;
           if `None` use `self.name`
         * `width`: the available width for the status line;
           if not an `int` use `width.width`
-        * `window`: optional timeframe to define "recent" in seconds,
+        * `recent_window`: optional timeframe to define "recent" in seconds,
           default : `5`
+        * `stalled`: the label to indicate no throughput, default `'stalled'`;
+          for a worker this might often b better as `'idle'`
     '''
     if label is None:
       label = self.name
+    if stalled is None:
+      stalled = 'stalled'
     if not isinstance(width, int):
       width = width.width
-    if window is None:
-      window = 5
+    if recent_window is None:
+      recent_window = 5
     leftv = []
     rightv = []
-    throughput = self.throughput_recent(window)
+    throughput = self.throughput_recent(recent_window)
     if throughput is not None:
       if throughput == 0:
         if self.total is not None and self.position >= self.total:
           return 'idle'
-        rightv.append('stalled')
+        rightv.append(stalled)
       else:
         if throughput >= 10:
           throughput = int(throughput)
         rightv.append(self.format_counter(throughput, max_parts=1) + '/s')
       remaining = self.remaining_time
       if remaining:
         remaining = int(remaining)
       if remaining is not None:
         rightv.append('ETA ' + transcribe_time(remaining))
     if self.total is not None and self.total > 0:
       leftv.append(self.text_pos_of_total())
     else:
       leftv.append(self.format_counter(self.position))
+    # the n/m display
     left = ' '.join(leftv)
+    # the throughput display
     right = ' '.join(rightv)
     if self.total is None:
       arrow_field = ' '
     else:
       # how much room for an arrow? we would like:
       # "label: left arrow right"
-      arrow_width = width - len(left) - len(right) - len(label) - 2
+      arrow_width = width - len(left) - len(right) - 2
       if label:  # allow for ': ' separator after label
-        arrow_width -= 2
-      if arrow_width < 1:  # no room for an arrow
+        arrow_width -= len(label) + 2
+      if arrow_width < 3:  # no room for an arrow
         arrow_field = ':'
       else:
         arrow_field = ' ' + self.arrow(arrow_width) + ' '
     status_line = left + arrow_field + right
     if label:
       label_width = width - len(status_line)
       if label_width >= len(label) + 2:
@@ -355,172 +369,160 @@
     else:
       prefix = ''
     status_line = prefix + status_line
     return status_line
 
   # pylint: disable=blacklisted-name,too-many-arguments
   @contextmanager
+  @uses_upd
   def bar(
       self,
       label=None,
       *,
-      upd=None,
-      proxy=None,
       statusfunc=None,
       width=None,
-      window=None,
+      recent_window=None,
+      stalled=None,
       report_print=None,
       insert_pos=1,
-      deferred=False,
+      poll: Optional[Callable[["BaseProgress"], None]] = None,
+      update_period=DEFAULT_UPDATE_PERIOD,
+      upd: Upd,
   ):
     ''' A context manager to create and withdraw a progress bar.
         It returns the `UpdProxy` which displays the progress bar.
 
         Parameters:
         * `label`: a label for the progress bar,
           default from `self.name`.
-        * `proxy`: an optional `UpdProxy` to display the progress bar
-        * `upd`: an optional `cs.upd.Upd` instance,
-          used to produce the progress bar status line if not supplied.
-          The default `upd` is `cs.upd.Upd()`
-          which uses `sys.stderr` for display.
         * `statusfunc`: an optional function to compute the progress bar text
           accepting `(self,label,width)`.
         * `width`: an optional width expressing how wide the progress bar
           text may be.
           The default comes from the `proxy.width` property.
-        * `window`: optional timeframe to define "recent" in seconds;
+        * `recent_window`: optional timeframe to define "recent" in seconds;
           if the default `statusfunc` (`Progress.status`) is used
           this is passed to it
         * `report_print`: optional `print` compatible function
           with which to write a report on completion;
           this may also be a `bool`, which if true will use `Upd.print`
           in order to interoperate with `Upd`.
+        * `stalled`: optional string to replace the word `'stalled'`
+          in the status line; for a worked this might be betteer as `'idle'`
         * `insert_pos`: where to insert the progress bar, default `1`
-        * `deferred`: optional flag; if true do not create the
-          progress bar until the first update occurs.
+        * `poll`: an optional callable accepting a `BaseProgress`
+          which can be used to update the progress state before
+          updating the progress bar display
 
         Example use:
 
             # display progress reporting during upload_filename()
             # which updates the supplied Progress instance
             # during its operation
             P = Progress(name=label)
             with P.bar(report_print=True):
                 upload_filename(src, progress=P)
 
     '''
     if label is None:
       label = self.name
-    if upd is None:
-      upd = Upd()
     if statusfunc is None:
-      # pylint: disable=unnecessary-lambda-assignment
-      statusfunc = lambda P, label, width: P.status(
-          label, width, window=window
-      )
-    pproxy = [proxy]
-    proxy_delete = proxy is None
 
-    def update(P, _):
-      proxy = pproxy[0]
-      if proxy is None:
-        proxy = pproxy[0] = upd.insert(insert_pos, 'LABEL=' + label)
-      proxy(statusfunc(P, label, width or proxy.width))
+      def statusfunc(P, label, width):
+        ''' Use the `Progress.status` method by default.
+        '''
+        return P.status(
+            label,
+            width,
+            recent_window=recent_window,
+            stalled=stalled,
+        )
 
-    try:
-      if not deferred:
-        if proxy is None:
-          proxy = pproxy[0] = upd.insert(insert_pos)
-        status = statusfunc(self, label, width or proxy.width)
-        proxy(status)
+    def text_auto():
+      ''' The current state of the `Progress`, to fit `width` and `proxy.width`.
+      '''
+      if poll is not None:
+        poll(self)
+      return statusfunc(self, "", min((width or proxy.width), proxy.width))
+
+    # pylint: disable=unused-argument
+    def update(P: Progress, _):
+      ''' Update the status bar `UpdProxy` with the current state.
+      '''
+      proxy.text = None
+
+    cancel_ticker = False
+
+    def ticker():
+      ''' Worker to update the progress bar every `update_period` seconds.
+      '''
+      time.sleep(update_period)
+      while not cancel_ticker:
+        update(self, None)
+        time.sleep(update_period)
+
+    if update_period == 0:
       self.notify_update.add(update)
+    try:
       start_pos = self.position
-      yield pproxy[0]
+      with upd.insert(
+          insert_pos,
+          prefix=label + ' ',
+          text_auto=text_auto,
+      ) as proxy:
+        update(self, None)
+        if update_period > 0:
+          bg(ticker, daemon=True)
+        yield proxy
     finally:
-      self.notify_update.remove(update)
-      if proxy and proxy_delete:
-        proxy.delete()
+      cancel_ticker = True
+      if update_period == 0:
+        self.notify_update.remove(update)
     if report_print:
       if isinstance(report_print, bool):
         report_print = print
       report_print(
           label + ':', self.format_counter(self.position - start_pos), 'in',
-          transcribe(
+          transcribe_units(
               self.elapsed_time, TIME_SCALE, max_parts=2, skip_zero=True
           )
       )
 
   # pylint: disable=too-many-arguments,too-many-branches,too-many-locals
-  @uses_upd
   def iterbar(
       self,
       it,
       label=None,
       *,
-      upd=None,
-      proxy=None,
       itemlenfunc=None,
-      statusfunc=None,
       incfirst=False,
-      width=None,
-      window=None,
-      update_frequency=1,
-      update_period=0.2,
-      update_min_size=None,
-      report_print=None,
-      runstate=None,
+      update_period=DEFAULT_UPDATE_PERIOD,
+      **bar_kw,
   ):
     ''' An iterable progress bar: a generator yielding values
         from the iterable `it` while updating a progress bar.
 
         Parameters:
         * `it`: the iterable to consume and yield.
+        * `label`: a label for the progress bar,
+          default from `self.name`.
         * `itemlenfunc`: an optional function returning the "size" of each item
           from `it`, used to advance `self.position`.
           The default is to assume a size of `1`.
           A convenient alternative choice may be the builtin function `len`.
         * `incfirst`: whether to advance `self.position` before we
           `yield` an item from `it` or afterwards.
           This reflects whether it is considered that progress is
           made as items are obtained or only after items are processed
           by whatever is consuming this generator.
           The default is `False`, advancing after processing.
-        * `label`: a label for the progress bar,
-          default from `self.name`.
-        * `width`: an optional width expressing how wide the progress bar
-          text may be.
-          The default comes from the `proxy.width` property.
-        * `window`: optional timeframe to define "recent" in seconds;
-          if the default `statusfunc` (`Progress.status`) is used
-          this is passed to it
-        * `statusfunc`: an optional function to compute the progress bar text
-          accepting `(self,label,width)`.
-        * `proxy`: an optional proxy for displaying the progress bar,
-          a callable accepting the result of `statusfunc`.
-          The default is a `cs.upd.UpdProxy` created from `upd`,
-          which inserts a progress bar above the main status line.
-        * `upd`: an optional `cs.upd.Upd` instance,
-          used only to produce the default `proxy` if that is not supplied.
-          The default `upd` is `cs.upd.Upd()`
-          which uses `sys.stderr` for display.
-        * `update_frequency`: optional update frequency, default `1`;
-          only update the progress bar after this many iterations,
-          useful if the iteration rate is quite high
-        * `update_min_size`: optional update step size;
-          only update the progress bar after an advance of this many units,
-          useful if the iteration size increment is quite small
-        * `update_period`: optional update time period, default `0.2`;
-          only update the progress bar after this much time has
-          elapsed since the last update
-        * `report_print`: optional `print` compatible function
-          with which to write a report on completion;
-          this may also be a `bool`, which if true will use `Upd.print`
-          in order to interoperate with `Upd`.
-        * `runstate`: optional `RunState` whose `.cancelled` property can be consulted
+        * `update_period`: default `DEFAULT_UPDATE_PERIOD`; if `0`
+          then update on every iteration, otherwise every `update_period`
+          seconds
+        Other parameters are passed to `Progress.bar`.
 
         Example use:
 
             from cs.units import DECIMAL_SCALE
             rows = [some list of data]
             P = Progress(total=len(rows), units_scale=DECIMAL_SCALE)
             for row in P.iterbar(rows, incfirst=True):
@@ -534,79 +536,27 @@
                     if not bs:
                         break
                     yield bs
             P = Progress(total=datalen)
             for bs in P.iterbar(readfrom(f), itemlenfunc=len):
                 ... process the file data in bs ...
     '''
-    if label is None:
-      label = self.name
-    delete_proxy = False
-    if proxy is None:
-      proxy = upd.insert(1, update_period=update_period)
-      delete_proxy = True
-    else:
-      old_update_period = proxy.update_period
-      proxy.update_period = update_period
-    if statusfunc is None:
-      # pylint: disable=unnecessary-lambda-assignment
-      statusfunc = lambda P, label, width: P.status(
-          label, width, window=window
-      )
-    iteration = 0
-    last_update_iteration = 0
-    last_update_pos = start_pos = self.position
-    last_update_time = None
-
-    def update_status(force=False):
-      nonlocal self, proxy, statusfunc, label, width
-      nonlocal iteration, last_update_iteration, last_update_pos, last_update_time
-      now = time.time()
-      # pylint: disable=too-many-boolean-expressions
-      if (force or iteration - last_update_iteration >= update_frequency
-          or (update_min_size is not None
-              and self.position - last_update_pos >= update_min_size)
-          or (update_period and now >= last_update_time + update_period)):
-        last_update_iteration = iteration
-        last_update_pos = self.position
-        proxy(statusfunc(self, label, width or proxy.width))
-        last_update_time = now
-
-    update_status(True)
-    try:
-      for iteration, item in enumerate(it):
+    with self.bar(label, update_period=update_period, **bar_kw) as proxy:
+      for item in it:
         length = itemlenfunc(item) if itemlenfunc else 1
         if incfirst:
           self += length
-          update_status()
-        yield item
-        if not incfirst:
+          if update_period == 0:
+            proxy.text = None
+          yield item
+        else:
+          yield item
           self += length
-          update_status()
-        if runstate is not None and runstate.cancelled:
-          break
-    finally:
-      if delete_proxy:
-        proxy.delete()
-      else:
-        # restore previous update frequency
-        proxy.update_period = old_update_period
-        update_status(True)
-      if report_print:
-        if isinstance(report_print, bool):
-          report_print = print
-        report_print(
-            label + (
-                ': (cancelled)'
-                if runstate is not None and runstate.cancelled else ':'
-            ), self.format_counter(self.position - start_pos), 'in',
-            transcribe(
-                self.elapsed_time, TIME_SCALE, max_parts=2, skip_zero=True
-            )
-        )
+          if update_period == 0:
+            proxy.text = None
 
 CheckPoint = namedtuple('CheckPoint', 'time position')
 
 class Progress(BaseProgress):
   ''' A progress counter to track task completion with various utility methods.
 
       Example:
@@ -735,14 +685,19 @@
   @total.setter
   def total(self, new_total):
     ''' Update the total.
     '''
     self._total = new_total
     self._updated()
 
+  def advance_total(self, delta):
+    ''' Function form of addition to the total.
+    '''
+    self.total += delta
+
   def update(self, new_position, update_time=None):
     ''' Record more progress.
 
             >>> P = Progress()
             >>> P.position
             0
             >>> P.update(12)
@@ -1051,15 +1006,15 @@
 def progressbar(
     it,
     label=None,
     *,
     position=None,
     total=None,
     units_scale=UNSCALED_SCALE,
-    **kw
+    **iterbar_kw
 ):
   ''' Convenience function to construct and run a `Progress.iterbar`
       wrapping the iterable `it`,
       issuing and withdrawning a progress bar during the iteration.
 
       Parameters:
       * `it`: the iterable to consume
@@ -1083,18 +1038,15 @@
   if total is None:
     try:
       total = len(it)
     except TypeError:
       total = None
   yield from Progress(
       name=label, position=position, total=total, units_scale=units_scale
-  ).iterbar(
-      it, label=label, **kw
-  )
-  ##pass  # former workaround for some bug, IIRC
+  ).iterbar(it, **iterbar_kw)
 
 @decorator
 def auto_progressbar(func, label=None, report_print=False):
   ''' Decorator for a function accepting an optional `progress`
       keyword parameter.
       If `progress` is `None` and the default `Upd` is not disabled,
       run the function with a progress bar.
@@ -1125,28 +1077,41 @@
 # pylint: disable=unused-argument
 def selftest(argv):
   ''' Exercise some of the functionality.
   '''
   with open(__file__, encoding='utf8') as f:
     lines = f.readlines()
   lines += lines
-  for _ in progressbar(lines, "lines"):
-    time.sleep(0.005)
-  for _ in progressbar(lines, "blines", units_scale=BINARY_BYTES_SCALE,
-                       itemlenfunc=len):
-    time.sleep(0.005)
-  for _ in progressbar(lines, "lines step 100", update_frequency=100,
-                       report_print=True):
-    time.sleep(0.005)
-  P = Progress(
-      name=__file__,
-      ##total=len(lines),
-      units_scale=DECIMAL_SCALE,
-  )
-  with open(__file__, encoding='utf8') as f:
-    for _ in P.iterbar(f):
-      time.sleep(0.005)
+  if True:  # pylint: disable=using-constant-test
+    for _ in progressbar(lines, "lines"):
+      pass
+  if True:  # pylint: disable=using-constant-test
+    for _ in progressbar(
+        lines,
+        "blines",
+        units_scale=BINARY_BYTES_SCALE,
+        itemlenfunc=len,
+        total=sum(len(line) for line in lines),
+    ):
+      pass
+  if True:  # pylint: disable=using-constant-test
+    for _ in progressbar(
+        lines,
+        "lines update 2s",
+        update_period=2,
+        report_print=True,
+    ):
+      pass
+  if True:  # pylint: disable=using-constant-test
+    P = Progress(
+        name=__file__,
+        ##total=len(lines),
+        units_scale=DECIMAL_SCALE,
+    )
+    with open(__file__, encoding='utf8') as f:
+      for _ in P.iterbar(f):
+        time.sleep(0.005)
   from cs.debug import selftest as runtests  # pylint: disable=import-outside-toplevel
   runtests('cs.progress_tests')
 
 if __name__ == '__main__':
   sys.exit(selftest(sys.argv))
```

