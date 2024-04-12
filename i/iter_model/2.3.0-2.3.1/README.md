# Comparing `tmp/iter_model-2.3.0.tar.gz` & `tmp/iter_model-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iter_model-2.3.0.tar", max compression
+gzip compressed data, was "iter_model-2.3.1.tar", max compression
```

## Comparing `iter_model-2.3.0.tar` & `iter_model-2.3.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-11-21 01:19:10.295657 iter_model-2.3.0/LICENSE
--rw-r--r--   0        0        0     2412 2023-11-21 01:19:10.295657 iter_model-2.3.0/README.md
--rw-r--r--   0        0        0       89 2023-11-21 01:19:10.299656 iter_model-2.3.0/iter_model/__init__.py
--rw-r--r--   0        0        0    19656 2023-11-21 01:19:10.299656 iter_model-2.3.0/iter_model/async_iter.py
--rw-r--r--   0        0        0     4083 2023-11-21 01:19:10.299656 iter_model-2.3.0/iter_model/async_iter.pyi
--rw-r--r--   0        0        0      520 2023-11-21 01:19:10.299656 iter_model-2.3.0/iter_model/async_utils.py
--rw-r--r--   0        0        0      337 2023-11-21 01:19:10.299656 iter_model-2.3.0/iter_model/empty_iterator.py
--rw-r--r--   0        0        0    14810 2023-11-21 01:19:10.299656 iter_model-2.3.0/iter_model/sync_iter.py
--rw-r--r--   0        0        0     3774 2023-11-21 01:19:10.299656 iter_model-2.3.0/iter_model/sync_iter.pyi
--rw-r--r--   0        0        0     1353 2023-11-21 01:19:10.299656 iter_model-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     3192 1970-01-01 00:00:00.000000 iter_model-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-12 11:19:01.503756 iter_model-2.3.1/LICENSE
+-rw-r--r--   0        0        0     2412 2024-04-12 11:19:01.503756 iter_model-2.3.1/README.md
+-rw-r--r--   0        0        0       89 2024-04-12 11:19:01.503756 iter_model-2.3.1/iter_model/__init__.py
+-rw-r--r--   0        0        0      141 2024-04-12 11:19:01.503756 iter_model-2.3.1/iter_model/__init__.pyi
+-rw-r--r--   0        0        0    19707 2024-04-12 11:19:01.503756 iter_model-2.3.1/iter_model/async_iter.py
+-rw-r--r--   0        0        0     3646 2024-04-12 11:19:01.507756 iter_model-2.3.1/iter_model/async_iter.pyi
+-rw-r--r--   0        0        0      520 2024-04-12 11:19:01.507756 iter_model-2.3.1/iter_model/async_utils.py
+-rw-r--r--   0        0        0      198 2024-04-12 11:19:01.507756 iter_model-2.3.1/iter_model/async_utils.pyi
+-rw-r--r--   0        0        0      337 2024-04-12 11:19:01.507756 iter_model-2.3.1/iter_model/empty_iterator.py
+-rw-r--r--   0        0        0      226 2024-04-12 11:19:01.507756 iter_model-2.3.1/iter_model/empty_iterator.pyi
+-rw-r--r--   0        0        0    14779 2024-04-12 11:19:01.507756 iter_model-2.3.1/iter_model/sync_iter.py
+-rw-r--r--   0        0        0     3252 2024-04-12 11:19:01.507756 iter_model-2.3.1/iter_model/sync_iter.pyi
+-rw-r--r--   0        0        0     1353 2024-04-12 11:19:01.507756 iter_model-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3192 1970-01-01 00:00:00.000000 iter_model-2.3.1/PKG-INFO
```

### Comparing `iter_model-2.3.0/LICENSE` & `iter_model-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iter_model-2.3.0/README.md` & `iter_model-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `iter_model-2.3.0/iter_model/async_iter.py` & `iter_model-2.3.1/iter_model/async_iter.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 from typing import (
     TypeVar,
     Generic,
     Callable,
     Iterable,
     ParamSpec,
     Awaitable,
-    TypeAlias,
     AsyncIterable,
-    AsyncIterator, cast,
+    AsyncIterator,
+    cast,
 )
 
 from .async_utils import asyncify
 from .empty_iterator import EmptyAsyncIterator
 
 T = TypeVar('T')
 R = TypeVar('R')
 P = ParamSpec('P')
 DefaultT = TypeVar('DefaultT')
-KeyFunc: TypeAlias = Callable[[T], R | Awaitable[R]]
-BinaryFunc: TypeAlias = Callable[[T, T], R | Awaitable[R]]
-ConditionFunc: TypeAlias = Callable[[T], bool | Awaitable[bool]]
+KeyFunc = Callable[[T], R | Awaitable[R]]
+BinaryFunc = Callable[[T, T], R | Awaitable[R]]
+ConditionFunc = Callable[[T], bool | Awaitable[bool]]
 
 _EMPTY = object()
 
 
-def async_iter(func: Callable[P, AsyncIterable[T]]) -> Callable[P, 'AsyncIter[T]']:
+def async_iter(func: Callable[P, AsyncIterator[T]]) -> Callable[P, 'AsyncIter[T]']:
     """Convert result of the func to AsyncIter
 
     Usage:
     ```python
     @async_iter
     def my_generator() -> AsyncIter[int]:
         for i in range(10):
@@ -47,15 +47,15 @@
 
     return wrapper
 
 
 class AsyncIter(Generic[T]):
     __slots__ = ('_it',)
 
-    def __init__(self, it: AsyncIterable[T]):
+    def __init__(self, it: AsyncIterator[T] | AsyncIterable[T]):
         self._it = aiter(it)
 
     def __aiter__(self) -> AsyncIterator[T]:
         return self._it
 
     def __anext__(self) -> Awaitable[T]:
         return anext(self._it)
@@ -97,28 +97,28 @@
         """Convert to set
 
         :return: set of items
         """
         return {item async for item in self}
 
     @async_iter
-    async def enumerate(self, start: int = 0) -> 'AsyncIter[tuple[int, T]]':
+    async def enumerate(self, start: int = 0) -> AsyncIterator[tuple[int, T]]:
         """Returns a tuple containing a count (from start which defaults to 0)
         and the values obtained from iterating over self.
 
         :param start: start of index
         :return: interator of tuple[index, item]
         """
         index = start
         async for item in self:
             yield index, item
             index += 1
 
     @async_iter
-    async def take(self, limit: int) -> 'AsyncIter[T]':
+    async def take(self, limit: int) -> AsyncIterator[T]:
         """Take 'count' items from iterator
 
         :return: iterable that contains 'count' items
         """
 
         count = 0
         while True:
@@ -128,47 +128,47 @@
                 yield await self.next()
             except StopAsyncIteration:
                 break
             else:
                 count += 1
 
     @async_iter
-    async def map(self, func: Callable[[T], R | Awaitable[R]]) -> 'AsyncIter[R]':
+    async def map(self, func: Callable[[T], R | Awaitable[R]]) -> AsyncIterator[R]:
         """Return an iterator that applies function to every item of iterable,
         yielding the results
 
         :return: iterable
         """
         func = asyncify(func)
         async for item in self:
             yield await func(item)
 
     @async_iter
-    async def skip(self, count: int) -> 'AsyncIter[T]':
+    async def skip(self, count: int) -> AsyncIterator[T]:
         """Skip 'count' items from iterator
         :return: iterable without first 'count' items
         """
         async for index, item in self.enumerate():
             if index >= count:
                 yield item
 
     @async_iter
-    async def skip_while(self, func: ConditionFunc) -> 'AsyncIter[T]':
+    async def skip_while(self, func: ConditionFunc) -> AsyncIterator[T]:
         """Skips leading elements while conditional is satisfied
 
         :return: iterable
         """
         func = asyncify(func)
         async for item in self:  # pragma: no cover
             if await func(item):
                 break
             yield item
 
     @async_iter
-    async def skip_where(self, func: ConditionFunc) -> 'AsyncIter':
+    async def skip_where(self, func: ConditionFunc) -> AsyncIterator[T]:
         """Skip elements where conditional is satisfied
 
         :return: async iterable
         """
         func = asyncify(func)
         async for item in self:
             if not await func(item):
@@ -233,26 +233,26 @@
 
         if default is not _EMPTY:
             return default
 
         raise ValueError('Item not found')
 
     @async_iter
-    async def where(self, func: ConditionFunc) -> 'AsyncIter[T]':
+    async def where(self, func: ConditionFunc) -> AsyncIterator[T]:
         """Filter item by condition
 
         :return: iterable
         """
         func = asyncify(func)
         async for item in self:
             if await func(item):
                 yield item
 
     @async_iter
-    async def take_while(self, func: ConditionFunc) -> 'AsyncIter[T]':
+    async def take_while(self, func: ConditionFunc) -> AsyncIterator[T]:
         """Take items while the conditional is satisfied
 
         :return: iterable
         """
         func = asyncify(func)
         async for item in self:
             if await func(item):
@@ -281,15 +281,15 @@
 
         if last_item is initial:
             raise StopAsyncIteration('Iterable is empty')
 
         return last_item
 
     @async_iter
-    async def chain(self, *iterables: AsyncIterable[T]) -> 'AsyncIter[T]':
+    async def chain(self, *iterables: AsyncIterable[T]) -> AsyncIterator[T]:
         """Chain with other iterables
 
         :return: iterable
         """
         async for item in self:
             yield item
 
@@ -321,30 +321,30 @@
         """Returns first item
 
         :return: first item
         """
         return await self.next()
 
     @async_iter
-    async def mark_first(self) -> 'AsyncIter[tuple[T, bool]]':
+    async def mark_first(self) -> AsyncIterator[tuple[T, bool]]:
         """Mark first item
 
         :return: Yields: tuple[item, is_first]
         """
         try:
             first = await self.next()
         except StopAsyncIteration:
             return
 
         yield first, True
         async for item in self:
             yield item, False
 
     @async_iter
-    async def mark_last(self) -> 'AsyncIter[tuple[T, bool]]':
+    async def mark_last(self) -> AsyncIterator[tuple[T, bool]]:
         """Mark last item
 
         :return: Yields: tuple[item, is_last]
         """
         try:
             previous_item = await self.next()
         except StopAsyncIteration:
@@ -352,15 +352,15 @@
 
         async for current_item in self:
             yield previous_item, False
             previous_item = current_item
         yield previous_item, True
 
     @async_iter
-    async def mark_first_last(self) -> 'AsyncIter[tuple[T, bool, bool]]':
+    async def mark_first_last(self) -> AsyncIterator[tuple[T, bool, bool]]:
         """Mark first and last item
 
         :return: Yields: tuple[item, is_first, is_last]
         """
         try:
             previous_item = await self.next()
         except StopAsyncIteration:
@@ -460,15 +460,15 @@
         return max_item
 
     @async_iter
     async def accumulate(
         self,
         func: BinaryFunc = operator.add,
         initial: T | None = None,
-    ) -> 'AsyncIter[R]':
+    ) -> AsyncIterator[R]:
         """Return series of accumulated sums (by default).
 
         :param func: func[accumulated value, next value], by default operator.add
         :param initial: initial value of series
 
         :return: iterable
         """
@@ -482,49 +482,49 @@
         func = asyncify(func)
         yield total
         async for item in self:
             total = await func(total, item)
             yield total
 
     @async_iter
-    async def append_left(self, item: T) -> 'AsyncIter[T]':
+    async def append_left(self, item: T) -> AsyncIterator[T]:
         """Append an item to left of the iterable (start)
 
         :return: iterable
         """
         yield item
         async for item_ in self:
             yield item_
 
     @async_iter
-    async def append_right(self, item: T) -> 'AsyncIter[T]':
+    async def append_right(self, item: T) -> AsyncIterator[T]:
         """Append an item to right of the iterable (end)
 
         :return: iterable
         """
         async for item_ in self:
             yield item_
         yield item
 
     @async_iter
-    async def append_at(self, index: int, item: T) -> 'AsyncIter[T]':
+    async def append_at(self, index: int, item: T) -> AsyncIterator[T]:
         """Append at the position in to the iterable
 
         :return: iterable
         """
         i = 0
         async for i, item_ in self.enumerate():
             if i == index:
                 yield item
             yield item_
         if index > i:
             yield item
 
     @async_iter
-    async def zip(self, *iterables: AsyncIterable[T], strict: bool = False) -> 'AsyncIter[list[T]]':
+    async def zip(self, *iterables: AsyncIterator[T], strict: bool = False) -> AsyncIterator[list[T]]:
         """The zip object yields n-length tuples, where n is the number of iterables
         passed as positional arguments to zip().  The i-th element in every tuple
         comes from the i-th iterable argument to zip().  This continues until the
         shortest argument is exhausted.
 
         :return: iterable
 
@@ -544,15 +544,15 @@
             yield batch
 
     @async_iter
     async def zip_longest(
         self,
         *iterables: AsyncIterable[T],
         fillvalue: R = None,
-    ) -> 'AsyncIter[list[T | R]]':
+    ) -> AsyncIterator[list[T | R]]:
         """The zip object yields n-length tuples, where n is the number of iterables
         passed as positional arguments to zip().  The i-th element in every tuple
         comes from the i-th iterable argument to zip().  This continues until the
         longest argument is exhausted.
 
         :param fillvalue: when the shorter iterables are exhausted, the fillvalue is substituted in their place
 
@@ -569,15 +569,15 @@
                 except StopAsyncIteration:
                     batch.append(fillvalue)
             if not batch_has_any_value:
                 return
             yield batch
 
     @async_iter
-    async def get_slice(self, start: int = 0, stop: int | None = None, step: int = 1) -> 'AsyncIter[T]':
+    async def get_slice(self, start: int = 0, stop: int | None = None, step: int = 1) -> AsyncIterator[T]:
         """Return slice from the iterable
 
         :return: iterable
         """
         it = self.skip(start)
 
         if stop is not None:
@@ -619,15 +619,15 @@
         """Return True if iterable is not empty
 
         :return: True if iterable is not empty
         """
         return not await self.is_empty()
 
     @async_iter
-    async def pairwise(self) -> 'AsyncIter[tuple[T, T]]':
+    async def pairwise(self) -> AsyncIterator[tuple[T, T]]:
         """Return an iterable of overlapping pairs
 
         :return: tuple[item_0, item_1], tuple[item_1, item_2], ...
         """
         try:
             previous = await self.next()
         except StopAsyncIteration:
@@ -643,30 +643,30 @@
         """
         count = 0
         async for _ in self:
             count += 1
         return count
 
     @async_iter
-    async def batches(self, batch_size: int) -> 'AsyncIter[tuple[T, ...]]':
+    async def batches(self, batch_size: int) -> AsyncIterator[tuple[T, ...]]:
         """Create iterator of tuples whose length = batch_size
 
         :return: iterator of tuples whose length = batch_size
         """
         while True:
             try:
                 item = await self.next()
             except StopAsyncIteration:
                 break
             it = self.append_left(item)
             batch = await it.take(batch_size).to_tuple()
             yield batch
 
     @async_iter
-    async def flatten(self) -> AsyncIterable[T]:
+    async def flatten(self: 'AsyncIter[AsyncIterator[T]]') -> AsyncIterator[T]:
         """Return an iterator that flattens one level of nesting
 
         :return: async iterable of flattened items
 
         :raise TypeError: if an encountered item is neither an Iterable nor an AsyncIterable
         """
         async for iterable in self:
```

### Comparing `iter_model-2.3.0/iter_model/async_iter.pyi` & `iter_model-2.3.1/iter_model/async_iter.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,161 +1,69 @@
-from __future__ import annotations
-
-import operator
-from typing import (
-    TypeVar,
-    Generic,
-    overload,
-    Callable,
-    Iterable,
-    ParamSpec,
-    Awaitable,
-    TypeAlias,
-    AsyncIterable,
-    AsyncIterator,
-)
+from .async_utils import asyncify as asyncify
+from .empty_iterator import EmptyAsyncIterator as EmptyAsyncIterator
+from typing import AsyncIterable, AsyncIterator, Awaitable, Callable, Generic, Iterable, ParamSpec, TypeVar, overload
 
 T = TypeVar('T')
 R = TypeVar('R')
 P = ParamSpec('P')
 DefaultT = TypeVar('DefaultT')
-KeyFunc: TypeAlias = Callable[[T], R | Awaitable[R]]
-BinaryFunc: TypeAlias = Callable[[T, T], R | Awaitable[R]]
-ConditionFunc: TypeAlias = Callable[[T], bool | Awaitable[bool]]
-
-_EMPTY = object()
+KeyFunc = Callable[[T], R | Awaitable[R]]
+BinaryFunc = Callable[[T, T], R | Awaitable[R]]
+ConditionFunc = Callable[[T], bool | Awaitable[bool]]
 
+def async_iter(func: Callable[P, AsyncIterable[T]]) -> Callable[P, AsyncIter[T]]: ...
 
 class AsyncIter(Generic[T]):
+    _it: AsyncIterator[T]
 
-    def __init__(self, it: AsyncIterable[T]):
-        self._it: AsyncIterator[T] = NotImplemented
-
+    def __init__(self, it: AsyncIterable[T]) -> None: ...
     def __aiter__(self) -> AsyncIterator[T]: ...
-
     def __anext__(self) -> Awaitable[T]: ...
-
     @classmethod
     def from_sync(cls, it: Iterable[T]) -> AsyncIter[T]: ...
-
     @classmethod
     def empty(cls) -> AsyncIter[T]: ...
-
     async def to_list(self) -> list[T]: ...
-
     async def to_tuple(self) -> tuple[T, ...]: ...
-
     async def to_set(self) -> set[T]: ...
-
-    def enumerate(self, start: int = 0) -> AsyncIter[tuple[int, T]]: ...
-
+    def enumerate(self, start: int = ...) -> AsyncIter[tuple[int, T]]: ...
     def take(self, limit: int) -> AsyncIter[T]: ...
-
     def map(self, func: Callable[[T], R | Awaitable[R]]) -> AsyncIter[R]: ...
-
     def skip(self, count: int) -> AsyncIter[T]: ...
-
     def skip_while(self, func: ConditionFunc) -> AsyncIter[T]: ...
-
-    def skip_where(self, func: ConditionFunc) -> AsyncIter[T]: ...
-
+    def skip_where(self, func: ConditionFunc) -> AsyncIter: ...
     async def count(self) -> int: ...
-
-    async def first_where(
-        self,
-        func: ConditionFunc,
-        default: DefaultT = _EMPTY,  # type: ignore
-    ) -> T | DefaultT: ...
-
-    async def last_where(
-        self,
-        func: ConditionFunc,
-        default: DefaultT = _EMPTY,  # type: ignore
-    ) -> T | DefaultT: ...
-
+    async def first_where(self, func: ConditionFunc, default: DefaultT = ...) -> T | DefaultT: ...
+    async def last_where(self, func: ConditionFunc, default: DefaultT = ...) -> T | DefaultT: ...
     def where(self, func: ConditionFunc) -> AsyncIter[T]: ...
-
-    def take_while(self, func: ConditionFunc) -> AsyncIter[T]:  ...
-
+    def take_while(self, func: ConditionFunc) -> AsyncIter[T]: ...
     async def next(self) -> T: ...
-
     async def last(self) -> T: ...
-
-    def chain(self, *iterables: AsyncIterable[T]) -> AsyncIter[T]: ...
-
+    def chain(self, *iterables: AsyncIterator[T]) -> AsyncIter[T]: ...
     async def all(self) -> bool: ...
-
     async def any(self) -> bool: ...
-
     async def first(self) -> T: ...
-
     def mark_first(self) -> AsyncIter[tuple[T, bool]]: ...
-
     def mark_last(self) -> AsyncIter[tuple[T, bool]]: ...
-
     def mark_first_last(self) -> AsyncIter[tuple[T, bool, bool]]: ...
-
-    async def reduce(
-        self,
-        func: BinaryFunc,
-        initial: T = _EMPTY,  # type: ignore
-    ) -> T | R: ...
-
-    async def max(
-        self,
-        key: KeyFunc | None = None,
-        default: DefaultT = _EMPTY,  # type: ignore
-    ) -> T | DefaultT: ...
-
-    async def min(
-        self,
-        key: KeyFunc | None = None,
-        default: DefaultT = _EMPTY,  # type: ignore
-    ) -> T | DefaultT: ...
-
-    def accumulate(
-        self,
-        func: BinaryFunc = operator.add,
-        initial: T | None = None,
-    ) -> AsyncIter[R]: ...
-
+    async def reduce(self, func: BinaryFunc, initial: T = ...) -> T | R: ...
+    async def max(self, key: KeyFunc | None = ..., default: DefaultT = ...) -> T | DefaultT: ...
+    async def min(self, key: KeyFunc | None = ..., default: DefaultT = ...) -> T | DefaultT: ...
+    def accumulate(self, func: BinaryFunc = ..., initial: T | None = ...) -> AsyncIter[R]: ...
     def append_left(self, item: T) -> AsyncIter[T]: ...
-
     def append_right(self, item: T) -> AsyncIter[T]: ...
-
     def append_at(self, index: int, item: T) -> AsyncIter[T]: ...
-
-    def zip(self, *iterables: AsyncIterable[T], strict: bool = False) -> AsyncIter[list[T]]: ...
-
-    def zip_longest(
-        self,
-        *iterables: AsyncIterable[T],
-        fillvalue: R | None = None,
-    ) -> AsyncIter[list[T | R]]: ...
-
-    def get_slice(self, start: int = 0, stop: int | None = None, step: int = 1) -> AsyncIter[T]: ...
-
+    def zip(self, *iterables: AsyncIterator[T], strict: bool = ...) -> AsyncIter[list[T]]: ...
+    def zip_longest(self, *iterables: AsyncIterator[T], fillvalue: R = ...) -> AsyncIter[list[T | R]]: ...
+    def get_slice(self, start: int = ..., stop: int | None = ..., step: int = ...) -> AsyncIter[T]: ...
     async def item_at(self, index: int) -> T: ...
-
     async def contains(self, item: T) -> bool: ...
-
     async def is_empty(self) -> bool: ...
-
     async def is_not_empty(self) -> bool: ...
-
     def pairwise(self) -> AsyncIter[tuple[T, T]]: ...
-
     async def get_len(self) -> int: ...
-
     def batches(self, batch_size: int) -> AsyncIter[tuple[T, ...]]: ...
-
-    def flatten(self) -> AsyncIter[T]: ...
-
+    def flatten(self: AsyncIter[AsyncIterator[T]]) -> AsyncIter[T]: ...
     @overload
     def __getitem__(self, index: int) -> Awaitable[T]: ...
-
     @overload
     def __getitem__(self, index: slice) -> AsyncIter[T]: ...
-
-def async_iter(
-    func: Callable[P, AsyncIterable[T] | AsyncIterator[T]],
-) -> Callable[P, AsyncIter[T]]: ...
```

### Comparing `iter_model-2.3.0/iter_model/async_utils.py` & `iter_model-2.3.1/iter_model/async_utils.py`

 * *Files identical despite different names*

### Comparing `iter_model-2.3.0/iter_model/sync_iter.py` & `iter_model-2.3.1/iter_model/sync_iter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import operator
 import functools
 import itertools
 from functools import wraps
-from typing import Iterable, TypeVar, Callable, Generic, ParamSpec, TypeAlias, Iterator
+from typing import Iterable, TypeVar, Callable, Generic, ParamSpec, Iterator
 
 from .empty_iterator import EmptyIterator
 
 T = TypeVar('T')
 R = TypeVar('R')
 P = ParamSpec('P')
 DefaultT = TypeVar('DefaultT')
 
-KeyFunc: TypeAlias = Callable[[T], R]
-BinaryFunc: TypeAlias = Callable[[T, T], T]
-ConditionFunc: TypeAlias = Callable[[T], bool]
+KeyFunc = Callable[[T], R]
+BinaryFunc = Callable[[T, T], T]
+ConditionFunc = Callable[[T], bool]
 _EMPTY = object()
 
 
-def sync_iter(func: Callable[P, Iterable[T]]) -> Callable[P, 'SyncIter[T]']:
+def sync_iter(func: Callable[P, Iterator[T]]) -> Callable[P, 'SyncIter[T]']:
     """Convert result of the func to SyncIter
 
     Usage:
     ```python
     @sync_iter
     def my_generator() -> SyncIter[int]:
         for i in range(10):
@@ -250,29 +250,29 @@
         """Return first item. The same as next()
 
         :return: first item
         """
         return self.next()
 
     @sync_iter
-    def mark_first(self) -> 'SyncIter[tuple[T, bool]]':
+    def mark_first(self) -> Iterator[tuple[T, bool]]:
         """Mark first item.
 
         :return: Yields: tuple[item, is_first]
         """
         try:
             first = self.next()
         except StopIteration:
             return
 
         yield first, True
         yield from self.map(lambda item: (item, False))
 
     @sync_iter
-    def mark_last(self) -> 'SyncIter[tuple[T, bool]]':
+    def mark_last(self) -> Iterator[tuple[T, bool]]:
         """Mark last item
 
         :return: Yields: tuple[item, is_last]
         """
         try:
             previous_item = self.next()
         except StopIteration:
@@ -280,15 +280,15 @@
 
         for current_item in self:
             yield previous_item, False
             previous_item = current_item
         yield previous_item, True
 
     @sync_iter
-    def mark_first_last(self) -> 'SyncIter[tuple[T, bool, bool]]':
+    def mark_first_last(self) -> Iterator[tuple[T, bool, bool]]:
         """Mark first and last item
 
         :return: Yields: tuple[item, is_first, is_last]
         """
         try:
             previous_item = self.next()
         except StopIteration:
@@ -369,33 +369,33 @@
         :param initial: initial value of series
 
          :return: iterable
         """
         return SyncIter(itertools.accumulate(self, func=func, initial=initial))
 
     @sync_iter
-    def append_left(self, item: T) -> 'SyncIter[T]':
+    def append_left(self, item: T) -> Iterator[T]:
         """Append an item to left of the iterable (start)
 
          :return: iterable
         """
         yield item
         yield from self
 
     @sync_iter
-    def append_right(self, item: T) -> 'SyncIter[T]':
+    def append_right(self, item: T) -> Iterator[T]:
         """Append an item to right of the iterable (end)
 
          :return: iterable
         """
         yield from self
         yield item
 
     @sync_iter
-    def append_at(self, index: int, item: T) -> 'SyncIter[T]':
+    def append_at(self, index: int, item: T) -> Iterator[T]:
         """Append at the position in to the iterable
 
          :return: iterable
         """
         i = 0
         for i, item_ in self.enumerate():
             if i == index:
@@ -484,29 +484,29 @@
         """
         count = 0
         for _ in self:
             count += 1
         return count
 
     @sync_iter
-    def batches(self, batch_size: int) -> 'SyncIter[tuple[T, ...]]':
+    def batches(self, batch_size: int) -> Iterator[tuple[T, ...]]:
         """Create iterable of tuples whose length = batch_size
 
         :return: iterable of tuples whose length = batch_size
         """
         while True:
             try:
                 item = self.next()
             except StopIteration:
                 break
             it = self.append_left(item)
             batch = it.take(batch_size).to_tuple()
             yield batch
 
-    def flatten(self) -> Iterable[T]:
+    def flatten(self: 'SyncIter[Iterator[T]]') -> 'SyncIter[T]':
         """Return an iterator that flattens one level of nesting
 
         :return: iterable of flattened items
 
         :raise TypeError: if an encountered item is not an Iterable
         """
         return SyncIter(itertools.chain.from_iterable(self))
```

### Comparing `iter_model-2.3.0/pyproject.toml` & `iter_model-2.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iter_model"
-version = "2.3.0"
+version = "2.3.1"
 description = "iter-model uses a method approach instead of individual functions to work with iterable objects."
 authors = ["volodymyrb <volodymyr.borysiuk0@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://volodymyrbor.github.io/iter_model/"
 repository = "https://github.com/VolodymyrBor/iter_model"
 documentation = "https://volodymyrbor.github.io/iter_model/"
```

### Comparing `iter_model-2.3.0/PKG-INFO` & `iter_model-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iter_model
-Version: 2.3.0
+Version: 2.3.1
 Summary: iter-model uses a method approach instead of individual functions to work with iterable objects.
 Home-page: https://volodymyrbor.github.io/iter_model/
 License: MIT
 Keywords: iterator,iterable
 Author: volodymyrb
 Author-email: volodymyr.borysiuk0@gmail.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iter_model Version: 2.3.0 Summary: iter-model uses
+Metadata-Version: 2.1 Name: iter_model Version: 2.3.1 Summary: iter-model uses
 a method approach instead of individual functions to work with iterable
 objects. Home-page: https://volodymyrbor.github.io/iter_model/ License: MIT
 Keywords: iterator,iterable Author: volodymyrb Author-email:
 volodymyr.borysiuk0@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

