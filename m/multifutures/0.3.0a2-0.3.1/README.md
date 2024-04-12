# Comparing `tmp/multifutures-0.3.0a2.tar.gz` & `tmp/multifutures-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multifutures-0.3.0a2.tar", max compression
+gzip compressed data, was "multifutures-0.3.1.tar", max compression
```

## Comparing `multifutures-0.3.0a2.tar` & `multifutures-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1102 2024-01-26 01:23:48.898877 multifutures-0.3.0a2/LICENSE.txt
--rw-r--r--   0        0        0      647 2024-01-26 08:37:21.276648 multifutures-0.3.0a2/README.md
--rw-r--r--   0        0        0      644 2024-01-26 08:48:50.416917 multifutures-0.3.0a2/multifutures/__init__.py
--rw-r--r--   0        0        0     1302 2024-01-26 08:37:21.276648 multifutures-0.3.0a2/multifutures/_common.py
--rw-r--r--   0        0        0    10986 2024-01-26 08:37:21.276648 multifutures-0.3.0a2/multifutures/_multi.py
--rw-r--r--   0        0        0     2327 2024-01-26 08:37:21.276648 multifutures-0.3.0a2/multifutures/_rate_limit.py
--rw-r--r--   0        0        0        0 2024-01-26 01:23:48.902211 multifutures-0.3.0a2/multifutures/py.typed
--rw-r--r--   0        0        0     3884 2024-01-26 16:18:33.548704 multifutures-0.3.0a2/pyproject.toml
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 multifutures-0.3.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 08:43:36.006184 multifutures-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     1672 2024-04-12 08:43:36.006184 multifutures-0.3.1/README.md
+-rw-r--r--   0        0        0      644 2024-04-12 08:43:36.006184 multifutures-0.3.1/multifutures/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-12 08:43:36.006184 multifutures-0.3.1/multifutures/_common.py
+-rw-r--r--   0        0        0    13623 2024-04-12 08:43:36.006184 multifutures-0.3.1/multifutures/_multi.py
+-rw-r--r--   0        0        0     2327 2024-04-12 08:43:36.006184 multifutures-0.3.1/multifutures/_rate_limit.py
+-rw-r--r--   0        0        0        0 2024-04-12 08:43:36.006184 multifutures-0.3.1/multifutures/py.typed
+-rw-r--r--   0        0        0     4002 2024-04-12 08:43:36.006184 multifutures-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 multifutures-0.3.1/PKG-INFO
```

### Comparing `multifutures-0.3.0a2/LICENSE.txt` & `multifutures-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multifutures-0.3.0a2/multifutures/__init__.py` & `multifutures-0.3.1/multifutures/__init__.py`

 * *Files identical despite different names*

### Comparing `multifutures-0.3.0a2/multifutures/_common.py` & `multifutures-0.3.1/multifutures/_common.py`

 * *Files identical despite different names*

### Comparing `multifutures-0.3.0a2/multifutures/_multi.py` & `multifutures-0.3.1/multifutures/_multi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import dataclasses
 import logging
 import multiprocessing
 import typing as T
+import warnings
 from collections import abc
 from concurrent.futures import as_completed
 from concurrent.futures import ProcessPoolExecutor
 from concurrent.futures import ThreadPoolExecutor
 
 import exceptiongroup
 import tqdm.auto
@@ -18,43 +19,59 @@
 
 logger = logging.getLogger(__name__)
 
 if T.TYPE_CHECKING:
     from typing_extensions import reveal_type
 
 
-def _resolve_multiprocess_executor(executor: ExecutorProtocol | None) -> ExecutorProtocol:
-    if executor is not None:
+_DEPRECATION_PROGRESS_BAR_IS_NONE = "multifutures: Using `progress_bar=None` is deprecated and will be removed in a future release. Replace it with `progress_bar=True`"  # noqa: E501: Line too long
+
+
+def _resolve_multiprocess_executor(executor: ExecutorProtocol | None, max_workers: int | None) -> ExecutorProtocol:
+    if executor and max_workers:
+        raise ValueError("Can't specify both `executor` and `max_workers`. Choose one or the other")
+    elif executor:
         _executor = executor
     else:
         try:
             import loky
 
-            _executor = loky.get_reusable_executor()
+            _executor = loky.get_reusable_executor(max_workers=max_workers)
         except ImportError:
             ctx = multiprocessing.get_context("spawn")
-            _executor = ProcessPoolExecutor(mp_context=ctx)
+            _executor = ProcessPoolExecutor(mp_context=ctx, max_workers=max_workers)
     return _executor
 
 
-def _resolve_multithreading_executor(executor: ExecutorProtocol | None) -> ExecutorProtocol:
+def _resolve_multithreading_executor(executor: ExecutorProtocol | None, max_workers: int | None) -> ExecutorProtocol:
     _executor: ExecutorProtocol
-    if executor is not None:
+    if executor and max_workers:
+        raise ValueError("Can't specify both `executor` and `max_workers`. Choose one or the other")
+    elif executor:
         _executor = executor
     else:
-        _executor = ThreadPoolExecutor()
+        _executor = ThreadPoolExecutor(max_workers=max_workers)
     return _executor
 
 
 def _resolve_progress_bar(
-    progress_bar: ProgressBarProtocol | None,
+    progress_bar: ProgressBarProtocol | bool | None,
     func_kwargs: abc.Collection[dict[str, T.Any]],
 ) -> ProgressBarProtocol:
-    if progress_bar is not None:
+    if progress_bar is None:
+        warnings.warn(
+            _DEPRECATION_PROGRESS_BAR_IS_NONE,
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        progress_bar = True
+    if isinstance(progress_bar, tqdm.tqdm):
         _progress_bar = progress_bar
+    elif progress_bar is False:
+        _progress_bar = tqdm.auto.tqdm(total=len(func_kwargs), disable=True)
     else:
         _progress_bar = tqdm.auto.tqdm(total=len(func_kwargs))
     return _progress_bar
 
 
 @dataclasses.dataclass
 class FutureResult:
@@ -113,18 +130,17 @@
 
 def _multi(
     *,
     executor: ExecutorProtocol,
     func: abc.Callable[..., T.Any],
     func_kwargs: abc.Collection[dict[str, T.Any]],
     include_kwargs: bool,
-    progress_bar: ProgressBarProtocol | None,
+    progress_bar: ProgressBarProtocol,
     check: bool,
 ) -> list[FutureResult]:
-    progress_bar = _resolve_progress_bar(progress_bar, func_kwargs)
     with progress_bar:
         with executor as xctr:
             futures_to_kwargs = {xctr.submit(func, **kwargs): kwargs for kwargs in func_kwargs}
             results = []
             for future in as_completed(futures_to_kwargs):
                 func_result = None
                 exception = None
@@ -143,63 +159,77 @@
     return results
 
 
 def multithread(
     func: abc.Callable[..., T.Any],
     func_kwargs: abc.Collection[dict[str, T.Any]],
     *,
+    max_workers: int | None = None,
     executor: ExecutorProtocol | None = None,
     check: bool = False,
     include_kwargs: bool = True,
-    progress_bar: ProgressBarProtocol | None = None,
+    progress_bar: ProgressBarProtocol | bool | None = True,
 ) -> list[FutureResult]:
     """
     Call `func` over all the items of `func_kwargs` using a multithreading Pool
     and return a list of [FutureResult][multifutures.FutureResult] objects.
 
-    Users should control the Pool's configuration (e.g. number of workers) by passing
-    a custom `Executor` instance. For example:
+    The pool by default is an instance of [ThreadPoolExecutor][concurrent.futures.ThreadPoolExecutor].
+    The pool size can be limited with `max_workers`. If more control is needed,
+    then the caller should directly pass a [ThreadPoolExecutor][concurrent.futures.ThreadPoolExecutor]
+    instance to `executor`. For example:
 
     ``` python
-    executor = concurrent.futures.ThreadPoolExecutor(max_workers=4)
+    # Customize executor
+    executor = concurrent.futures.ThreadPoolExecutor(
+        max_workers=4, thread_name_prefix="AAA"
+    )
     multithread(func, func_kwargs, executor=executor)
     ```
 
-    The progress of the pool's workers can be monitored by a [tqdm][tqdm] based progress bar.
-    Customizing the progress bar should be done by creating a `progress_bar`.
-    For example, to disable the progress bar:
+    The progress of the pool's workers can be monitored by using a
+    [tqdm](https://tqdm.github.io/) based progress bar.
+    The progress bar is displayed by default.
+    Disabling the progress bar is possible by passing `progress_bar=False`.
+    Further customizing of the progress bar should be done by creating a `tqdm.tqdm`
+    instance and passing it as an argument to `progress_bar`. For example:
 
     ``` python
-    progress_bar = tqdm.auto.tqdm(func_kwargs, disable=True)
-    results = multithread(func, func_kwargs, progress_bar=progress_bar)
+    # Run without a progress bar
+    results = multithread(func, func_kwargs, progress_bar=False)
+
+    # Run with a rich based progress bar
+    rich_based_progress_bar = tqdm.rich.tqdm(func_kwargs)
+    results = multithread(func, func_kwargs, progress_bar=rich_based_progress_bar)
     ```
 
     Arguments:
         func: The function that will be scheduled for execution via multithreading.
         func_kwargs: A Collection of dictionaries that will be used for the calls of `func`.
         executor: The multithreading [Executor][concurrent.futures.Executor] instance that we want to use.
             Defaults to the standard library's [ThreadPoolExecutor][concurrent.futures.ThreadPoolExecutor].
         check: If `True` then if any of the `func` calls raised an exception, an
             [ExceptionGroup][ExceptionGroup] containing all the exceptions will be raised.
         include_kwargs: A boolean flag indicating whether the keyword arguments of the
             functions will be present in the [FurureResult][multifutures.FutureResult]
-            object. Useful for keeping memory usage down when the input are objects like
-            `xarray.Dataset` etc.
+            object. Setting this to `False` is useful for keeping memory usage down when
+            the input are "heavy" objects like [xarray.Dataset][xarray.Dataset] etc.
         progress_bar: An instance of a progress bar implementing the `tqdm` API. Defaults to
             `tqdm.auto.tqdm`.
 
     Returns:
         A list of [FutureResult][multifutures.FutureResult] objects. Each object
             will contain the output of `func(**func_kwarg)` or an `Exception`.
 
     Raises:
         exceptiongroup.ExceptionGroup: If any of the function calls raises an exception and `check` is True.
 
     """
-    executor = _resolve_multithreading_executor(executor=executor)
+    progress_bar = _resolve_progress_bar(progress_bar, func_kwargs)
+    executor = _resolve_multithreading_executor(executor=executor, max_workers=max_workers)
     results = _multi(
         executor=executor,
         func=func,
         func_kwargs=func_kwargs,
         include_kwargs=include_kwargs,
         progress_bar=progress_bar,
         check=check,
@@ -207,38 +237,54 @@
     return results
 
 
 def multiprocess(
     func: abc.Callable[..., T.Any],
     func_kwargs: abc.Collection[dict[str, T.Any]],
     *,
+    max_workers: int | None = None,
     executor: ExecutorProtocol | None = None,
     check: bool = False,
     include_kwargs: bool = True,
-    progress_bar: ProgressBarProtocol | None = None,
+    progress_bar: ProgressBarProtocol | bool | None = True,
 ) -> list[FutureResult]:
     """
     Call `func` over all the items of `func_kwargs` using a multiprocessing Pool
     and return a list of [FutureResult][multifutures.FutureResult] objects.
 
-    Users should control the Pool's configuration (e.g. number of workers) by passing
-    a custom `Executor` instance. For example:
+    The pool by default is an instance of [loky.ProcessPoolExecutor](https://loky.readthedocs.io/en/stable/),
+    or, if `loky` is not installed, an instance of
+    [concurrent.futures.ProcessPoolExecutor][concurrent.futures.ProcessPoolExecutor]
+    using the `spawn` multiprocessing context.
+
+    The pool size can be limited with `max_workers`. If more control is needed, e.g. to use a different
+    multiprocessing context, then the caller should directly pass a `ProcessPoolExecutor`
+    instance to `executor`. For example:
 
     ``` python
-    executor = concurrent.futures.ProcessPoolExecutor(max_workers=4)
+    # Customize executor
+    mp_context = multiprocessing.get_context("forkserver")
+    executor = concurrent.futures.ProcessPoolExecutor(max_workers=4, mp_context=mp_context)
     multiprocess(func, func_kwargs, executor=executor)
     ```
 
-    The progress of the pool's workers can be monitored by a [tqdm][tqdm] based progress bar.
-    Customizing the progress bar should be done by creating a `progress_bar` instance.
-    For example, to disable the progress bar:
+    The progress of the pool's workers can be monitored by using a
+    [tqdm](https://tqdm.github.io/) based progress bar.
+    The progress bar is displayed by default.
+    Disabling the progress bar is possible by passing `progress_bar=False`.
+    Further customizing of the progress bar should be done by creating a `tqdm.tqdm`
+    instance and passing it as an argument to `progress_bar`. For example:
 
     ``` python
-    progress_bar = tqdm.auto.tqdm(func_kwargs, disable=True)
-    results = multiprocess(func, func_kwargs, progress_bar=progress_bar)
+    # Run without a progress bar
+    results = multithread(func, func_kwargs, progress_bar=False)
+
+    # Run with a rich based progress bar
+    rich_based_progress_bar = tqdm.rich.tqdm(func_kwargs)
+    results = multithread(func, func_kwargs, progress_bar=rich_based_progress_bar)
     ```
 
     Arguments:
         func: The function that will be scheduled for execution via multiprocessing.
         func_kwargs: A Collection of dictionaries that will be used for the calls of `func`.
         executor: A multiprocessing [Executor][concurrent.futures.Executor] instance.
             Defaults to [loky.get_reusable_executor()][loky.get_reusable_executor],
@@ -247,28 +293,29 @@
             If [loky][loky] is not installed, it defaults to Standard Library's
             [ProcessPoolExecutor][concurrent.futures.ProcessPoolExecutor] with the `spawn` multiprocessing
             start method ([more info](https://docs.python.org/3/library/multiprocessing.html#multiprocessing-start-methods))
         check: If `True` then if any of the `func` calls raised an exception, an
             [ExceptionGroup][ExceptionGroup] containing all the exceptions will be raised.
         include_kwargs: A boolean flag indicating whether the keyword arguments of the
             functions will be present in the [FurureResult][multifutures.FutureResult]
-            object. Useful for keeping memory usage down when the input are objects like
-            `xarray.Dataset` etc.
+            object. Setting this to `False` is useful for keeping memory usage down when
+            the input are "heavy" objects like [xarray.Dataset][xarray.Dataset] etc.
         progress_bar: An instance of a progress bar implementing the `tqdm` API. Defaults to
             `tqdm.auto.tqdm`.
 
     Returns:
         A list of [FutureResult][multifutures.FutureResult] objects. Each object
             will contain the output of `func(**func_kwargs[i])` or an `Exception`.
 
     Raises:
         exceptiongroup.ExceptionGroup: If any of the function calls raises an exception and `check` is True.
 
     """
-    executor = _resolve_multiprocess_executor(executor)
+    progress_bar = _resolve_progress_bar(progress_bar, func_kwargs)
+    executor = _resolve_multiprocess_executor(executor=executor, max_workers=max_workers)
     results = _multi(
         executor=executor,
         func=func,
         func_kwargs=func_kwargs,
         include_kwargs=include_kwargs,
         progress_bar=progress_bar,
         check=check,
```

### Comparing `multifutures-0.3.0a2/multifutures/_rate_limit.py` & `multifutures-0.3.1/multifutures/_rate_limit.py`

 * *Files identical despite different names*

### Comparing `multifutures-0.3.0a2/pyproject.toml` & `multifutures-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "multifutures"
-version = "0.3.0a2"
+version = "0.3.1"
 description = ""
 authors = ["Panos Mavrogiorgos <pmav99@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9, <4.0"
+python = ">=3.9"
 exceptiongroup = "*"
 limits = "*"
 tqdm = "*"
 loky = {version = "*", optional = true}
 psutil = {version = "*", optional = true}
 
 [tool.poetry.extras]
@@ -32,15 +32,15 @@
 mkdocstrings-python = "*"
 pymdown-extensions = "*"
 black = "*"
 mkdocs-gen-files = "*"
 mike = "*"
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 dirty = false
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
@@ -52,14 +52,15 @@
 testpaths = [
   "tests",
 ]
 filterwarnings = [
     "error",
     'ignore:distutils Version classes are deprecated. Use packaging.version instead:DeprecationWarning',
     'ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning',
+    'ignore:This process \(pid=.*\) is multi-threaded, use of fork\(\) may lead to deadlocks in the child:DeprecationWarning',
 ]
 
 
 [tool.mypy]
 python_version = "3.9"
 plugins = []
 show_column_numbers = true
```

