# Comparing `tmp/ndbioimage-2024.4.4.tar.gz` & `tmp/ndbioimage-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2024.4.4.tar", max compression
+gzip compressed data, was "ndbioimage-2024.4.5.tar", max compression
```

## Comparing `ndbioimage-2024.4.4.tar` & `ndbioimage-2024.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.4/LICENSE
--rw-r--r--   0        0        0     2608 2024-04-03 13:37:34.891216 ndbioimage-2024.4.4/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.4/ndbioimage/.DS_Store
--rwxr-xr-x   0        0        0    50979 2024-04-05 15:20:31.941526 ndbioimage-2024.4.4/ndbioimage/__init__.py
--rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.4/ndbioimage/jvm.py
--rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.4/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.4/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    28629 2024-04-02 16:23:36.764150 ndbioimage-2024.4.4/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.4/ndbioimage/readers/fijiread.py
--rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.4/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6381 2024-03-29 16:56:03.400728 ndbioimage-2024.4.4/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.4/ndbioimage/readers/tifread.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.4/ndbioimage/transform.txt
--rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.4/ndbioimage/transforms.py
--rw-r--r--   0        0        0     1010 2024-04-10 13:19:26.813381 ndbioimage-2024.4.4/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 ndbioimage-2024.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.5/LICENSE
+-rw-r--r--   0        0        0     2608 2024-04-03 13:37:34.891216 ndbioimage-2024.4.5/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.5/ndbioimage/.DS_Store
+-rwxr-xr-x   0        0        0    54071 2024-04-12 13:42:57.566891 ndbioimage-2024.4.5/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.5/ndbioimage/jvm.py
+-rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.5/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.5/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    29149 2024-04-12 14:01:22.722103 ndbioimage-2024.4.5/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.5/ndbioimage/readers/fijiread.py
+-rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.5/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.4.5/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.5/ndbioimage/readers/tifread.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.5/ndbioimage/transform.txt
+-rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.5/ndbioimage/transforms.py
+-rw-r--r--   0        0        0     1246 2024-04-12 13:36:02.623186 ndbioimage-2024.4.5/pyproject.toml
+-rw-r--r--   0        0        0     4066 1970-01-01 00:00:00.000000 ndbioimage-2024.4.5/PKG-INFO
```

### Comparing `ndbioimage-2024.4.4/LICENSE` & `ndbioimage-2024.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.4/README.md` & `ndbioimage-2024.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.4/ndbioimage/.DS_Store` & `ndbioimage-2024.4.5/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.4/ndbioimage/__init__.py` & `ndbioimage-2024.4.5/ndbioimage/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from __future__ import annotations
 
 import multiprocessing
-import re
 import os
+import re
 import warnings
 from abc import ABC, ABCMeta, abstractmethod
 from argparse import ArgumentParser
 from collections import OrderedDict
 from datetime import datetime
 from functools import cached_property, wraps
 from importlib.metadata import version
 from itertools import product
-from numbers import Number
 from operator import truediv
-from pathlib import Path, PosixPath, WindowsPath, PurePath
+from pathlib import Path
 from traceback import print_exc
-from typing import Any, Callable, Mapping, Optional
+from typing import Any, Callable, Generator, Iterable, Optional, Sequence, TypeVar
 
 import numpy as np
-import ome_types
 import yaml
-from ome_types import OME, model, ureg
+from numpy.typing import ArrayLike, DTypeLike
+from ome_types import OME, from_xml, model, ureg
 from pint import set_application_registry
-from tiffwrite import IFD, IJTiffFile
+from tiffwrite import IFD, IJTiffFile  # noqa
 from tqdm.auto import tqdm
 
 from .jvm import JVM
 from .transforms import Transform, Transforms
 
 try:
     __version__ = version(Path(__file__).parent.name)
@@ -40,14 +39,15 @@
         __git_commit_hash__ = h.read().rstrip('\n')
 except Exception:  # noqa
     __git_commit_hash__ = 'unknown'
 
 ureg.default_format = '~P'
 set_application_registry(ureg)
 warnings.filterwarnings('ignore', 'Reference to unknown ID')
+Number = int | float | np.integer | np.floating
 
 
 class ReaderNotFoundError(Exception):
     pass
 
 
 class TransformTiff(IJTiffFile):
@@ -75,54 +75,57 @@
         self.__truncate__()
 
     def update(self, *args: Any, **kwargs: Any) -> None:
         super().update(*args, **kwargs)
         self.__truncate__()
 
 
-def find(obj: Mapping, **kwargs: Any) -> Any:
+def find(obj: Sequence[Any], **kwargs: Any) -> Any:
     for item in obj:
         try:
             if all([getattr(item, key) == value for key, value in kwargs.items()]):
                 return item
         except AttributeError:
             pass
 
 
-def try_default(fun: Callable, default: Any, *args: Any, **kwargs: Any) -> Any:
+R = TypeVar('R')
+
+
+def try_default(fun: Callable[..., R], default: Any, *args: Any, **kwargs: Any) -> R:
     try:
         return fun(*args, **kwargs)
     except Exception:  # noqa
         return default
 
 
 def bioformats_ome(path: str | Path) -> OME:
     from .readers.bfread import jars
     try:
         jvm = JVM(jars)  # noqa
         ome_meta = jvm.metadata_tools.createOMEXMLMetadata()
         reader = jvm.image_reader()
         reader.setMetadataStore(ome_meta)
         reader.setId(str(path))
-        ome = ome_types.from_xml(str(ome_meta.dumpXML()), parser='lxml')
+        ome = from_xml(str(ome_meta.dumpXML()), parser='lxml')
     except Exception:  # noqa
         print_exc()
         ome = model.OME()
     finally:
         jvm.kill_vm()  # noqa
     return ome
 
 
 class Shape(tuple):
-    def __new__(cls, shape: tuple[int] | Shape[int], axes: str = 'yxczt') -> Shape[int]:
+    def __new__(cls, shape: Sequence[int] | Shape, axes: str = 'yxczt') -> Shape:
         if isinstance(shape, Shape):
             axes = shape.axes  # type: ignore
-        instance = super().__new__(cls, shape)
-        instance.axes = axes.lower()
-        return instance  # type: ignore
+        new = super().__new__(cls, shape)
+        new.axes = axes.lower()
+        return new  # type: ignore
 
     def __getitem__(self, n: int | str) -> int | tuple[int]:
         if isinstance(n, str):
             if len(n) == 1:
                 return self[self.axes.find(n.lower())] if n.lower() in self.axes else 1
             else:
                 return tuple(self[i] for i in n)  # type: ignore
@@ -166,124 +169,145 @@
 
 
 class Imread(np.lib.mixins.NDArrayOperatorsMixin, ABC):
     """ class to read image files, while taking good care of important metadata,
         currently optimized for .czi files, but can open anything that bioformats can handle
             path: path to the image file
             optional:
-            series: in case multiple experiments are saved in one file, like in .lif files
+            axes: order of axes, default: cztyx, but omitting any axes with lenght 1
             dtype: datatype to be used when returning frames
-            meta: define metadata, used for pickle-ing
-
-            NOTE: run imread.kill_vm() at the end of your script/program, otherwise python might not terminate
 
             modify images on the fly with a decorator function:
                 define a function which takes an instance of this object, one image frame,
                 and the coordinates c, z, t as arguments, and one image frame as return
                 >> imread.frame_decorator = fun
                 then use imread as usually
 
             Examples:
-                >> im = imread('/DATA/lenstra_lab/w.pomp/data/20190913/01_YTL639_JF646_DefiniteFocus.czi')
+                >> im = Imread('/path/to/file.image', axes='czt)
                 >> im
                  << shows summary
                 >> im.shape
-                 << (256, 256, 2, 1, 600)
-                >> plt.imshow(im(1, 0, 100))
-                 << plots frame at position c=1, z=0, t=100 (python type indexing), note: round brackets; always 2d array
-                    with 1 frame
-                >> data = im[:,:,0,0,:25]
-                 << retrieves 5d numpy array containing first 25 frames at c=0, z=0, note: square brackets; always 5d array
-                >> plt.imshow(im.max(0, None, 0))
-                 << plots max-z projection at c=0, t=0
-                >> len(im)
-                 << total number of frames
-                >> im.pxsize
+                 << (15, 26, 1000, 1000)
+                >> im.axes
+                 << 'ztyx'
+                >> plt.imshow(im[1, 0])
+                 << plots frame at position z=1, t=0 (python type indexing)
+                >> plt.imshow(im[:, 0].max('z'))
+                 << plots max-z projection at t=0
+                >> im.pxsize_um
                  << 0.09708737864077668 image-plane pixel size in um
                 >> im.laserwavelengths
                  << [642, 488]
                 >> im.laserpowers
                  << [0.02, 0.0005] in %
 
                 See __init__ and other functions for more ideas.
 
             Subclassing:
                 Subclass AbstractReader to add more file types. A subclass should always have at least the following
                 methods:
                     staticmethod _can_open(path): returns True when the subclass can open the image in path
-                    __metadata__(self): pulls some metadata from the file and do other format specific things,
-                                        it needs to define a few properties, like shape, etc.
                     __frame__(self, c, z, t): this should return a single frame at channel c, slice z and time t
+                    optional open(self): code to be run during initialization, e.g. to open a file handle
                     optional close(self): close the file in a proper way
-                    optional field priority: subclasses with lower priority will be tried first, default = 99
+                    optional class field priority: subclasses with lower priority will be tried first, default = 99
+                    optional get_ome(self) -> OME: return an OME structure with metadata,
+                        if not present bioformats will be used to generate an OME
                     Any other method can be overridden as needed
-            wp@tl2019-2023 """
+    """
 
-    def __new__(cls, path=None, *args, **kwargs):
+    isclosed: Optional[bool]
+    channel_names: Optional[list[str]]
+    series: Optional[int]
+    pxsize_um: Optional[float]
+    deltaz_um: Optional[float]
+    exposuretime_s: Optional[list[float]]
+    timeinterval: Optional[float]
+    binning: Optional[list[int]]
+    laserwavelengths: Optional[list[tuple[float]]]
+    laserpowers: Optional[list[tuple[float]]]
+    objective: Optional[model.Objective]
+    magnification: Optional[float]
+    tubelens: Optional[model.Objective]
+    filter: Optional[str]
+    powermode: Optional[str]
+    collimator: Optional[str]
+    tirfangle: Optional[list[float]]
+    gain: Optional[list[float]]
+    pcf: Optional[list[float]]
+    __frame__: Callable[[int, int, int], np.ndarray]
+
+    def __new__(cls, path: Path | str | Imread | Any = None, dtype: DTypeLike = None, axes: str = None) -> Imread:
         if cls is not Imread:
             return super().__new__(cls)
         if len(AbstractReader.__subclasses__()) == 0:
             raise Exception('Restart python kernel please!')
         if isinstance(path, Imread):
             return path
         path, _ = AbstractReader.split_path_series(path)
         for subclass in sorted(AbstractReader.__subclasses__(), key=lambda subclass_: subclass_.priority):
-            if subclass._can_open(path):
+            if subclass._can_open(path):  # noqa
                 do_not_pickle = (AbstractReader.do_not_pickle,) if isinstance(AbstractReader.do_not_pickle, str) \
                     else AbstractReader.do_not_pickle
                 subclass_do_not_pickle = (subclass.do_not_pickle,) if isinstance(subclass.do_not_pickle, str) \
                     else subclass.do_not_pickle if hasattr(subclass, 'do_not_pickle') else ()
                 subclass.do_not_pickle = set(do_not_pickle).union(set(subclass_do_not_pickle))
 
                 return super().__new__(subclass)
         raise ReaderNotFoundError(f'No reader found for {path}.')
 
-    def __init__(self, base=None, slice=None, shape=(0, 0, 0, 0, 0), dtype=None, frame_decorator=None):
+    def __init__(self, base: Imread = None,
+                 slice: tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray] = None,  # noqa
+                 shape: tuple[int, ...] = (0, 0, 0, 0, 0),
+                 dtype: DTypeLike = None,
+                 frame_decorator: Callable[[Imread, np.ndarray, int, int, int], np.ndarray] = None) -> None:
         self.base = base or self
         self.slice = slice
         self._shape = Shape(shape)
         self.dtype = dtype
         self.frame_decorator = frame_decorator
         self.transform = Transforms()
         self.flags = dict(C_CONTIGUOUS=False, F_CONTIGUOUS=False, OWNDATA=False, WRITEABLE=False,
                           ALIGNED=False, WRITEBACKIFCOPY=False, UPDATEIFCOPY=False)
 
-    def __call__(self, c=None, z=None, t=None, x=None, y=None):
+    def __call__(self, c: int = None, z: int = None, t: int = None, x: int = None, y: int = None) -> np.ndarray:
         """ same as im[] but allowing keyword axes, but slices need to made with slice() or np.s_ """
         return self[{k: slice(v) if v is None else v for k, v in dict(c=c, z=z, t=t, x=x, y=y).items()}]
 
-    def __copy__(self):
+    def __copy__(self) -> Imread:
         return self.copy()
 
-    def __contains__(self, item):
-        def unique_yield(a, b):
+    def __contains__(self, item: Number) -> bool:
+        def unique_yield(a: Iterable[Any], b: Iterable[Any]) -> Generator[Any, None, None]:
             for k in a:
                 yield k
             for k in b:
                 if k not in a:
                     yield k
 
         for idx in unique_yield([key[:3] for key in self.cache.keys()],
                                 product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t']))):
             yxczt = (slice(None), slice(None)) + idx
             in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
             if item in np.asarray(self[in_idx]):
                 return True
         return False
 
-    def __enter__(self):
+    def __enter__(self) -> Imread:
         return self
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(self, *args: Any, **kwargs: Any) -> None:
         if not self.isclosed:
             self.isclosed = True
             if hasattr(self, 'close'):
                 self.close()
 
-    def __getitem__(self, n):
+    def __getitem__(self, n: int | Sequence[int] | slice | type(Ellipsis) |
+                    dict[str, int | Sequence[int] | slice | type(Ellipsis)]) -> Number | Imread | np.ndarray:
         """ slice like a numpy array but return an Imread instance """
         if self.isclosed:
             raise OSError('file is closed')
         if isinstance(n, (slice, Number)):  # None = :
             n = (n,)
         elif isinstance(n, type(Ellipsis)):
             n = (None,) * len(self.axes)
@@ -322,61 +346,62 @@
             new = View(self)
             new.slice = new_slice
             new._shape = Shape([1 if isinstance(s, Number) else len(s) for s in new_slice])
             new.axes = ''.join(j for j in self.axes if j in [i for i, s in zip('yxczt', new_slice)
                                                              if not isinstance(s, Number)])
             return new
 
-    def __getstate__(self):
+    def __getstate__(self) -> dict[str: Any]:
         return {key: value for key, value in self.__dict__.items() if key not in self.do_not_pickle}
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.shape[0]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.summary
 
-    def __setstate__(self, state):
+    def __setstate__(self, state: dict[str, Any]) -> None:
         """ What happens during unpickling """
         self.__dict__.update(state)
         if isinstance(self, AbstractReader):
             self.open()
         self.cache = DequeDict(16)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.path)
 
-    def __array__(self, dtype=None):
+    def __array__(self, dtype: DTypeLike = None) -> np.ndarray:
         block = self.block(*self.slice)
         axes_idx = [self.shape.axes.find(i) for i in 'yxczt']
         axes_squeeze = tuple({i for i, j in enumerate(axes_idx) if j == -1}.union(
             {i for i, j in enumerate(self.slice) if isinstance(j, Number)}))
         block = block.squeeze(axes_squeeze)
         if dtype is not None:
             block = block.astype(dtype)
         if block.ndim == 0:
             return block.item()
         axes = ''.join(j for i, j in enumerate('yxczt') if i not in axes_squeeze)
         return block.transpose([axes.find(i) for i in self.shape.axes if i in axes])
 
-    def __array_arg_fun__(self, fun, axis=None, out=None):
+    def __array_arg_fun__(self, fun: Callable[[ArrayLike, Optional[int]], Number | np.ndarray],
+                          axis: int | str = None, out: np.ndarray = None) -> Number | np.ndarray:
         """ frame-wise application of np.argmin and np.argmax """
         if axis is None:
             value = arg = None
             for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
                 yxczt = (slice(None), slice(None)) + idx
                 in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
                 new = np.asarray(self[in_idx])
-                new_arg = np.unravel_index(fun(new), new.shape)
+                new_arg = np.unravel_index(fun(new), new.shape)  # type: ignore
                 new_value = new[new_arg]
                 if value is None:
                     arg = new_arg + idx
                     value = new_value
                 else:
-                    i = fun((value, new_value))
+                    i = fun((value, new_value))  # type: ignore
                     arg = (arg, new_arg + idx)[i]
                     value = (value, new_value)[i]
             axes = ''.join(i for i in self.axes if i in 'yx') + 'czt'
             arg = np.ravel_multi_index([arg[axes.find(i)] for i in self.axes], self.shape)
             if out is None:
                 return arg
             else:
@@ -416,29 +441,32 @@
                     else:
                         old_value = value[out_idx]
                         i = fun((old_value, new_value), 0)
                         value[out_idx] = np.where(i, new_value, old_value)
                         out[out_idx] = np.where(i, new_arg, out[out_idx])
             return out
 
-    def __array_fun__(self, funs, axis=None, dtype=None, out=None, keepdims=False, initials=None, where=True,
-                      ffuns=None, cfun=None):
+    def __array_fun__(self, funs: Sequence[Callable[[ArrayLike], Number | np.ndarray]], axis: int | str = None,
+                      dtype: DTypeLike = None, out: np.ndarray = None, keepdims: bool = False,
+                      initials: list[Number | np.ndarray] = None, where: bool | int | np.ndarray = True,
+                      ffuns: Sequence[Callable[[ArrayLike], np.ndarray]] = None,
+                      cfun: Callable[..., np.ndarray] = None) -> Number | np.ndarray:
         """ frame-wise application of np.min, np.max, np.sum, np.mean and their nan equivalents """
         p = re.compile(r'\d')
         dtype = self.dtype if dtype is None else np.dtype(dtype)
         if initials is None:
             initials = [None for _ in funs]
         if ffuns is None:
             ffuns = [None for _ in funs]
 
-        def ffun_(frame):
+        def ffun_(frame: ArrayLike) -> np.ndarray:
             return np.asarray(frame)
         ffuns = [ffun_ if ffun is None else ffun for ffun in ffuns]
         if cfun is None:
-            def cfun(*res):
+            def cfun(*res):  # noqa
                 return res[0]
 
         # TODO: smarter transforms
         if axis is None:
             for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
                 yxczt = (slice(None), slice(None)) + idx
                 in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
@@ -497,68 +525,68 @@
                         for tmp, fun, ffun in zip(tmps, funs, ffuns):
                             tmp[out_idx] = fun((tmp[out_idx], ffun(self[in_idx])), 0, where=w)
                 out[...] = (np.round(cfun(*tmps)) if out.dtype.kind in 'ui' else
                             cfun(*tmps)).astype(p.sub('', dtype.name))
             return out
 
     @property
-    def axes(self):
+    def axes(self) -> str:
         return self.shape.axes
 
     @axes.setter
-    def axes(self, value):
+    def axes(self, value: str) -> None:
         shape = self.shape[value]
         if isinstance(shape, Number):
             shape = (shape,)
         self._shape = Shape(shape, value)
 
     @property
-    def dtype(self):
+    def dtype(self) -> np.dtype:
         return self._dtype
 
     @dtype.setter
-    def dtype(self, value):
+    def dtype(self, value: DTypeLike) -> None:
         self._dtype = np.dtype(value)
 
     @cached_property
-    def extrametadata(self):
+    def extrametadata(self) -> Optional[Any]:
         if isinstance(self.path, Path):
             if self.path.with_suffix('.pzl2').exists():
                 pname = self.path.with_suffix('.pzl2')
             elif self.path.with_suffix('.pzl').exists():
                 pname = self.path.with_suffix('.pzl')
             else:
                 return
             try:
                 return self.get_config(pname)
             except Exception:  # noqa
                 return
         return
 
     @property
-    def ndim(self):
+    def ndim(self) -> int:
         return len(self.shape)
 
     @property
-    def size(self):
+    def size(self) -> int:
         return np.prod(self.shape)
 
     @property
-    def shape(self):
+    def shape(self) -> Shape:
         return self._shape
 
     @shape.setter
-    def shape(self, value):
+    def shape(self, value: Shape | tuple[int, ...]) -> None:
         if isinstance(value, Shape):
             self._shape = value
         else:
-            self._shape = Shape((value['yxczt'.find(i.lower())] for i in self.axes), self.axes)
+            self._shape = Shape([value['yxczt'.find(i.lower())] for i in self.axes], self.axes)
 
     @property
-    def summary(self):
+    def summary(self) -> str:
         """ gives a helpful summary of the recorded experiment """
         s = [f'path/filename: {self.path}',
              f'series/pos:    {self.series}',
              f"reader:        {self.base.__class__.__module__.split('.')[-1]}"]
         s.extend((f'dtype:         {self.dtype}',
                   f'shape ({self.axes}):'.ljust(15) + f"{' x '.join(str(i) for i in self.shape)}"))
         if self.pxsize_um:
@@ -594,80 +622,80 @@
         if self.gain:
             s.append('gain:         ' + (' {:.0f}' * len(self.gain)).format(*self.gain))
         if self.pcf:
             s.append('pcf:          ' + (' {:.2f}' * len(self.pcf)).format(*self.pcf))
         return '\n'.join(s)
 
     @property
-    def T(self):
+    def T(self) -> Imread:  # noqa
         return self.transpose()
 
     @cached_property
-    def timeseries(self):
+    def timeseries(self) -> bool:
         return self.shape['t'] > 1
 
     @cached_property
-    def zstack(self):
+    def zstack(self) -> bool:
         return self.shape['z'] > 1
 
-    @wraps(np.argmax)
+    @wraps(np.ndarray.argmax)
     def argmax(self, *args, **kwargs):
         return self.__array_arg_fun__(np.argmax, *args, **kwargs)
 
-    @wraps(np.argmin)
+    @wraps(np.ndarray.argmin)
     def argmin(self, *args, **kwargs):
         return self.__array_arg_fun__(np.argmin, *args, **kwargs)
 
-    @wraps(np.max)
-    def max(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+    @wraps(np.ndarray.max)
+    def max(self, axis=None, out=None, keepdims=False, initial=None, where=True, **_):
         return self.__array_fun__([np.max], axis, None, out, keepdims, [initial], where)
 
-    @wraps(np.mean)
-    def mean(self, axis=None, dtype=None, out=None, keepdims=False, *, where=True, **kwargs):
+    @wraps(np.ndarray.mean)
+    def mean(self, axis=None, dtype=None, out=None, keepdims=False, *, where=True, **_):
         dtype = dtype or float
         n = np.prod(self.shape) if axis is None else self.shape[axis]
 
-        def sfun(frame):
+        def sfun(frame: ArrayLike) -> np.ndarray:
             return np.asarray(frame).astype(float)
 
-        def cfun(res):
+        def cfun(res: np.ndarray) -> np.ndarray:
             return res / n
 
         return self.__array_fun__([np.sum], axis, dtype, out, keepdims, None, where, [sfun], cfun)
 
-    @wraps(np.min)
-    def min(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+    @wraps(np.ndarray.min)
+    def min(self, axis=None, out=None, keepdims=False, initial=None, where=True, **_):
         return self.__array_fun__([np.min], axis, None, out, keepdims, [initial], where)
 
     @wraps(np.moveaxis)
     def moveaxis(self, source, destination):
         raise NotImplementedError('moveaxis is not implemented')
 
     @wraps(np.nanmax)
-    def nanmax(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+    def nanmax(self, axis=None, out=None, keepdims=False, initial=None, where=True, **_):
         return self.__array_fun__([np.nanmax], axis, None, out, keepdims, [initial], where)
 
     @wraps(np.nanmean)
-    def nanmean(self, axis=None, dtype=None, out=None, keepdims=False, *, where=True, **kwargs):
+    def nanmean(self, axis=None, dtype=None, out=None, keepdims=False, *, where=True, **_):
         dtype = dtype or float
 
         def sfun(frame):
             return np.asarray(frame).astype(float)
 
         def nfun(frame):
             return np.invert(np.isnan(frame))
 
         return self.__array_fun__([np.nansum, np.sum], axis, dtype, out, keepdims, None, where, (sfun, nfun), truediv)
 
     @wraps(np.nanmin)
-    def nanmin(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+    def nanmin(self, axis=None, out=None, keepdims=False, initial=None, where=True, **_):
         return self.__array_fun__([np.nanmin], axis, None, out, keepdims, [initial], where)
 
     @wraps(np.nansum)
-    def nansum(self, axis=None, dtype=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+    def nansum(self, axis=None, dtype=None, out=None, keepdims=False, initial=None, where=True, **_):
         return self.__array_fun__([np.nansum], axis, dtype, out, keepdims, [initial], where)
 
     @wraps(np.nanstd)
     def nanstd(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=None):
         return self.nanvar(axis, dtype, out, ddof, keepdims, where=where, std=True)
 
     @wraps(np.nanvar)
@@ -688,65 +716,66 @@
                 return np.sqrt((s2 - s ** 2 / n) / (n - ddof))
         else:
             def cfun(s, s2, n):
                 return (s2 - s ** 2 / n) / (n - ddof)
         return self.__array_fun__([np.nansum, np.nansum, np.sum], axis, dtype, out, keepdims, None, where,
                                   (sfun, s2fun, nfun), cfun)
 
+    @wraps(np.ndarray.flatten)
     def flatten(self, *args, **kwargs):
         return np.asarray(self).flatten(*args, **kwargs)
 
-    @wraps(np.reshape)
+    @wraps(np.ndarray.reshape)
     def reshape(self, *args, **kwargs):
         return np.asarray(self).reshape(*args, **kwargs)
 
-    @wraps(np.squeeze)
+    @wraps(np.ndarray.squeeze)
     def squeeze(self, axes=None):
         new = self.copy()
         if axes is None:
             axes = tuple(i for i, j in enumerate(new.shape) if j == 1)
         elif isinstance(axes, Number):
             axes = (axes,)
         else:
             axes = tuple(new.axes.find(ax) if isinstance(ax, str) else ax for ax in axes)
         if any([new.shape[ax] != 1 for ax in axes]):
             raise ValueError('cannot select an axis to squeeze out which has size not equal to one')
         new.axes = ''.join(j for i, j in enumerate(new.axes) if i not in axes)
         return new
 
-    @wraps(np.std)
+    @wraps(np.ndarray.std)
     def std(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=True):
         return self.var(axis, dtype, out, ddof, keepdims, where=where, std=True)
 
-    @wraps(np.sum)
-    def sum(self, axis=None, dtype=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+    @wraps(np.ndarray.sum)
+    def sum(self, axis=None, dtype=None, out=None, keepdims=False, initial=None, where=True, **_):
         return self.__array_fun__([np.sum], axis, dtype, out, keepdims, [initial], where)
 
-    @wraps(np.swapaxes)
+    @wraps(np.ndarray.swapaxes)
     def swapaxes(self, axis1, axis2):
         new = self.copy()
         axes = new.axes
         if isinstance(axis1, str):
             axis1 = axes.find(axis1)
         if isinstance(axis2, str):
             axis2 = axes.find(axis2)
         axes[axis1], axes[axis2] = axes[axis2], axes[axis1]
         new.axes = axes
         return new
 
-    @wraps(np.transpose)
+    @wraps(np.ndarray.transpose)
     def transpose(self, *axes):
         new = self.copy()
         if not axes:
             new.axes = new.axes[::-1]
         else:
             new.axes = ''.join(ax if isinstance(ax, str) else new.axes[ax] for ax in axes)
         return new
 
-    @wraps(np.var)
+    @wraps(np.ndarray.var)
     def var(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=True, std=False):
         dtype = dtype or float
         n = np.prod(self.shape) if axis is None else self.shape[axis]
 
         def sfun(frame):
             return np.asarray(frame).astype(float)
 
@@ -757,40 +786,43 @@
             def cfun(s, s2):
                 return np.sqrt((s2 - s ** 2 / n) / (n - ddof))
         else:
             def cfun(s, s2):
                 return (s2 - s ** 2 / n) / (n - ddof)
         return self.__array_fun__([np.sum, np.sum], axis, dtype, out, keepdims, None, where, (sfun, s2fun), cfun)
 
-    def asarray(self):
+    def asarray(self) -> np.ndarray:
         return self.__array__()
 
-    def astype(self, dtype, *args, **kwargs):
+    @wraps(np.ndarray.astype)
+    def astype(self, dtype, *_, **__):
         new = self.copy()
         new.dtype = dtype
         return new
 
-    def block(self, y=None, x=None, c=None, z=None, t=None):
+    def block(self, y: int | Sequence[int] = None, x: int | Sequence[int] = None,
+              c: int | Sequence[int] = None, z: int | Sequence[int] = None,
+              t: int | Sequence[int] = None) -> np.ndarray:
         """ returns 5D block of frames """
         y, x, c, z, t = (np.arange(self.shape[i]) if e is None else np.array(e, ndmin=1)
                          for i, e in zip('yxczt', (y, x, c, z, t)))
         d = np.empty((len(y), len(x), len(c), len(z), len(t)), self.dtype)
         for (ci, cj), (zi, zj), (ti, tj) in product(enumerate(c), enumerate(z), enumerate(t)):
             d[:, :, ci, zi, ti] = self.frame(cj, zj, tj)[y][:, x]
         return d
 
-    def copy(self):
+    def copy(self) -> View:
         return View(self)
 
-    def data(self, c=0, z=0, t=0):
+    def data(self, c: int | Sequence[int] = 0, z: int | Sequence[int] = 0, t: int | Sequence[int] = 0) -> np.ndarray:
         """ returns 3D stack of frames """
         c, z, t = (np.arange(self.shape[i]) if e is None else np.array(e, ndmin=1) for i, e in zip('czt', (c, z, t)))
         return np.dstack([self.frame(ci, zi, ti) for ci, zi, ti in product(c, z, t)])
 
-    def frame(self, c=0, z=0, t=0):
+    def frame(self, c: int = 0, z: int = 0, t: int = 0) -> np.ndarray:
         """ returns single 2D frame """
         c = self.get_channel(c)
         c %= self.base.shape['c']
         z %= self.base.shape['z']
         t %= self.base.shape['t']
 
         # cache last n (default 16) frames in memory for speed (~250x faster)
@@ -804,58 +836,59 @@
                 f = self.frame_decorator(self, f, c, z, t)
             self.cache[key] = f
         if self.dtype is not None:
             return f.copy().astype(self.dtype)
         else:
             return f.copy()
 
-    def get_channel(self, channel_name):
+    def get_channel(self, channel_name: str | int) -> int:
         if not isinstance(channel_name, str):
             return channel_name
         else:
             c = [i for i, c in enumerate(self.channel_names) if c.lower().startswith(channel_name.lower())]
             assert len(c) > 0, f'Channel {c} not found in {self.channel_names}'
             assert len(c) < 2, f'Channel {c} not unique in {self.channel_names}'
             return c[0]
 
     @staticmethod
-    def get_config(file):
+    def get_config(file: Path | str) -> Any:
         """ Open a yml config file """
         loader = yaml.SafeLoader
         loader.add_implicit_resolver(
             r'tag:yaml.org,2002:float',
             re.compile(r'''^(?:
-                     [-+]?(?:[0-9][0-9_]*)\.[0-9_]*(?:[eE][-+]?[0-9]+)?
-                    |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)
+                     [-+]?([0-9][0-9_]*)\.[0-9_]*(?:[eE][-+]?[0-9]+)?
+                    |[-+]?([0-9][0-9_]*)([eE][-+]?[0-9]+)
                     |\.[0-9_]+(?:[eE][-+][0-9]+)?
                     |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\.[0-9_]*
                     |[-+]?\\.(?:inf|Inf|INF)
                     |\.(?:nan|NaN|NAN))$''', re.X),
             list(r'-+0123456789.'))
         with open(file) as f:
             return yaml.load(f, loader)
 
-    def get_czt(self, c, z, t):
+    def get_czt(self, c: int | Sequence[int], z: int | Sequence[int],
+                t: int | Sequence[int]) -> tuple[list[int], list[int], list[int]]:
         czt = []
         for i, n in zip('czt', (c, z, t)):
             if n is None:
                 czt.append(list(range(self.shape[i])))
             elif isinstance(n, range):
                 if n.stop < 0:
                     stop = n.stop % self.shape[i]
                 elif n.stop > self.shape[i]:
                     stop = self.shape[i]
                 else:
                     stop = n.stop
                 czt.append(list(range(n.start % self.shape[i], stop, n.step)))
             elif isinstance(n, Number):
-                czt.append([n % self.shape[i]])  # noqa
+                czt.append([n % self.shape[i]])
             else:
                 czt.append([k % self.shape[i] for k in n])
-        return [self.get_channel(c) for c in czt[0]], *czt[1:]
+        return [self.get_channel(c) for c in czt[0]], *czt[1:3]  # type: ignore
 
     @staticmethod
     def bioformats_ome(path: [str, Path]) -> OME:
         """ Use java BioFormats to make an ome metadata structure. """
         with multiprocessing.get_context('spawn').Pool(1) as pool:
             return pool.map(bioformats_ome, (path,))[0]
 
@@ -868,15 +901,15 @@
                                                                      for plane in image.pixels.planes])) > 1:
                     z = np.array([(plane.position_z * ureg.Quantity(plane.position_z_unit.value).to(ureg.m).magnitude,
                                    plane.the_z)
                                   for plane in image.pixels.planes if plane.the_c == 0 and plane.the_t == 0])
                     i = np.argsort(z[:, 1])
                     image.pixels.physical_size_z = np.nanmean(np.true_divide(*np.diff(z[i], axis=0).T)) * 1e6
                     image.pixels.physical_size_z_unit = 'µm'
-            except Exception:
+            except Exception:   # noqa
                 pass
         return ome
 
     @staticmethod
     def read_ome(path: [str, Path]) -> Optional[OME]:
         path = Path(path)
         if path.with_suffix('.ome.xml').exists():
@@ -892,33 +925,36 @@
         if self.path not in cache:
             ome = self.read_ome(self.path)
             if ome is None:
                 ome = self.get_ome()
             cache[self.path] = self.fix_ome(ome)
         return cache[self.path]
 
-    def is_noise(self, volume=None):
+    def is_noise(self, volume: ArrayLike = None) -> bool:
         """ True if volume only has noise """
         if volume is None:
             volume = self
         fft = np.fft.fftn(volume)
         corr = np.fft.fftshift(np.fft.ifftn(fft * fft.conj()).real / np.sum(volume ** 2))
         return 1 - corr[tuple([0] * corr.ndim)] < 0.0067
 
     @staticmethod
-    def kill_vm():
+    def kill_vm() -> None:
         JVM().kill_vm()
 
-    def new(self, *args, **kwargs):
+    def new(self, *args: Any, **kwargs: Any) -> View:
         warnings.warn('Imread.new has been deprecated, use Imread.view instead.', DeprecationWarning, 2)
         return self.view(*args, **kwargs)
 
-    def save_as_tiff(self, fname=None, c=None, z=None, t=None, split=False, bar=True, pixel_type='uint16', **kwargs):
+    def save_as_tiff(self, fname: Path | str = None, c: int | Sequence[int] = None, z: int | Sequence[int] = None,
+                     t: int | Sequence[int] = None, split: bool = False, bar: bool = True, pixel_type: str = 'uint16',
+                     **kwargs: Any) -> None:
         """ saves the image as a tif file
             split: split channels into different files """
+        fname = Path(fname)
         if fname is None:
             fname = self.path.with_suffix('.tif')
             if fname == self.path:
                 raise FileExistsError(f'File {fname} exists already.')
         if not isinstance(fname, Path):
             fname = Path(fname)
         if split:
@@ -940,29 +976,32 @@
             shape = [len(i) for i in n]
             with TransformTiff(self, fname.with_suffix('.tif'), shape, pixel_type,
                                pxsize=self.pxsize_um, deltaz=self.deltaz_um, **kwargs) as tif:
                 for i, m in tqdm(zip(product(*[range(s) for s in shape]), product(*n)),  # noqa
                                  total=np.prod(shape), desc='Saving tiff', disable=not bar):
                     tif.save(m, *i)
 
-    def with_transform(self, channels=True, drift=False, file=None, bead_files=()):
+    def with_transform(self, channels: bool = True, drift: bool = False, file: Path | str = None,
+                       bead_files: Sequence[Path | str] = ()) -> View:
         """ returns a view where channels and/or frames are registered with an affine transformation
             channels: True/False register channels using bead_files
             drift: True/False register frames to correct drift
             file: load registration from file with name file, default: transform.yml in self.path.parent
             bead_files: files used to register channels, default: files in self.path.parent,
                 with names starting with 'beads'
             """
         view = self.view()
         if file is None:
             file = Path(view.path.parent) / 'transform.yml'
+        else:
+            file = Path(file)
         if not bead_files:
             try:
                 bead_files = Transforms.get_bead_files(view.path.parent)
-            except Exception:
+            except Exception:  # noqa
                 if not file.exists():
                     raise Exception('No transform file and no bead file found.')
                 bead_files = ()
 
         if channels:
             try:
                 view.transform = Transforms.from_file(file, T=drift)
@@ -977,58 +1016,62 @@
                 view.transform = Transforms.from_file(file, C=False)
             except Exception:  # noqa
                 view.transform = Transforms().with_drift(self)
         view.transform.adapt(view.frameoffset, view.shape.yxczt, view.channel_names)
         return view
 
     @staticmethod
-    def split_path_series(path):
+    def split_path_series(path: Path | str) -> tuple[Path, int]:
         if isinstance(path, str):
             path = Path(path)
         if isinstance(path, Path) and path.name.startswith('Pos') and path.name.lstrip('Pos').isdigit():
             return path.parent, int(path.name.lstrip('Pos'))
         return path, 0
 
-    def view(self, *args, **kwargs):
+    def view(self, *args: Any, **kwargs: Any) -> View:
         return View(self, *args, **kwargs)
 
 
 class View(Imread, ABC):
-    def __init__(self, base, dtype=None):
+    def __init__(self, base: Imread, dtype: DTypeLike = None) -> None:
         super().__init__(base.base, base.slice, base.shape, dtype or base.dtype, base.frame_decorator)
         self.transform = base.transform
 
-    def __getattr__(self, item):
+    def __getattr__(self, item: str) -> Any:
         if not hasattr(self.base, item):
             raise AttributeError(f'{self.__class__} object has no attribute {item}')
         return self.base.__getattribute__(item)
 
 
 class AbstractReader(Imread, metaclass=ABCMeta):
     priority = 99
     do_not_pickle = 'cache'
     ureg = ureg
 
     @staticmethod
     @abstractmethod
-    def _can_open(path):  # Override this method, and return true when the subclass can open the file
+    def _can_open(path: Path | str) -> bool:
+        """ Override this method, and return true when the subclass can open the file """
         return False
 
     @abstractmethod
-    def __frame__(self, c, z, t):  # Override this, return the frame at c, z, t
+    def __frame__(self, c: int, z: int, t: int) -> np.ndarray:
+        """ Override this, return the frame at c, z, t """
         return np.random.randint(0, 255, self.shape['yx'])
 
-    def open(self):  # Optionally override this, open file handles etc.
-        """ filehandles cannot be pickled and should be marked such by setting do_not_pickle = 'file_handle_name' """
+    def open(self) -> None:
+        """ Optionally override this, open file handles etc.
+            filehandles cannot be pickled and should be marked such by setting do_not_pickle = 'file_handle_name' """
         return
 
-    def close(self):  # Optionally override this, close file handles etc.
+    def close(self) -> None:
+        """ Optionally override this, close file handles etc. """
         return
 
-    def __init__(self, path, dtype=None, axes=None):
+    def __init__(self, path: Path | str | Imread | Any = None, dtype: DTypeLike = None, axes: str = None) -> None:
         if isinstance(path, Imread):
             return
         super().__init__()
         self.isclosed = False
         if isinstance(path, str):
             path = Path(path)
         self.path, self.series = self.split_path_series(path)
@@ -1110,16 +1153,17 @@
                      for channel in image.pixels.channels
                      if channel.detector_settings
                      and find(instrument.detectors, id=channel.detector_settings.id).amplification_gain]
         self.laserwavelengths = [(channel.excitation_wavelength_quantity.to(self.ureg.nm).m,)
                                  for channel in pixels.channels if channel.excitation_wavelength_quantity]
         self.laserpowers = try_default(lambda: [(1 - channel.light_source_settings.attenuation,)
                                                 for channel in pixels.channels], [])
-        self.filter = try_default(lambda: [find(instrument.filter_sets, id=channel.filter_set_ref.id).model
-                                           for channel in image.pixels.channels], None)
+        self.filter = try_default(  # type: ignore
+            lambda: [find(instrument.filter_sets, id=channel.filter_set_ref.id).model
+                     for channel in image.pixels.channels], None)
         self.pxsize_um = None if self.pxsize is None else self.pxsize.to(self.ureg.um).m
         self.exposuretime_s = [None if i is None else i.to(self.ureg.s).m for i in self.exposuretime]
 
         if axes is None:
             self.axes = ''.join(i for i in 'cztyx' if self.shape[i] > 1)
         elif axes.lower() == 'full':
             self.axes = 'cztyx'
@@ -1153,15 +1197,15 @@
             sigma = []
             for c, d in enumerate(self.detector):
                 emission = (np.hstack(self.laserwavelengths[c]) + 22) * ureg.nm
                 sigma.append([emission[emission > s].max(initial=0), emission[emission < s].max(initial=0)][d])
             sigma = np.hstack(sigma)
             sigma[sigma == 0] = 600 * ureg.nm
             sigma /= 2 * self.NA * self.pxsize
-            self.sigma = sigma.magnitude.tolist()
+            self.sigma = sigma.magnitude.tolist()  # type: ignore
         except Exception:  # noqa
             self.sigma = [2] * self.shape['c']
         if not self.NA:
             self.immersionN = 1
         elif 1.5 < self.NA:
             self.immersionN = 1.661
         elif 1.3 < self.NA < 1.5:
@@ -1172,19 +1216,19 @@
             self.immersionN = 1
 
         p = re.compile(r'(\d+):(\d+)$')
         try:
             self.track, self.detector = zip(*[[int(i) for i in p.findall(find(
                 self.ome.images[self.series].pixels.channels, id=f'Channel:{c}').detector_settings.id)[0]]
                                               for c in range(self.shape['c'])])
-        except Exception:
+        except Exception:  # noqa
             pass
 
 
-def main():
+def main() -> None:
     parser = ArgumentParser(description='Display info and save as tif')
     parser.add_argument('file', help='image_file')
     parser.add_argument('out', help='path to tif out', type=str, default=None, nargs='?')
     parser.add_argument('-o', '--extract_ome', help='extract ome to xml file', action='store_true')
     parser.add_argument('-r', '--register', help='register channels', action='store_true')
     parser.add_argument('-c', '--channel', help='channel', type=int, default=None)
     parser.add_argument('-z', '--zslice', help='z-slice', type=int, default=None)
@@ -1205,8 +1249,8 @@
             else:
                 im.save_as_tiff(out, args.channel, args.zslice, args.time, args.split)
         if args.extract_ome:
             with open(im.path.with_suffix('.ome.xml'), 'w') as f:
                 f.write(im.ome.to_xml())
 
 
-from .readers import *
+from .readers import *  # noqa
```

### Comparing `ndbioimage-2024.4.4/ndbioimage/jvm.py` & `ndbioimage-2024.4.5/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.4/ndbioimage/readers/bfread.py` & `ndbioimage-2024.4.5/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.4/ndbioimage/readers/cziread.py` & `ndbioimage-2024.4.5/ndbioimage/readers/cziread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import re
 import warnings
 from abc import ABC
 from io import BytesIO
 from itertools import product
 from pathlib import Path
+from typing import Any, TypeVar, Optional
 
 import czifile
 import imagecodecs
 import numpy as np
 from lxml import etree
-from ome_types import model
+from ome_types import model, OME
 from tifffile import repeat_nd
 
 from .. import AbstractReader
 
 try:
     # TODO: use zoom from imagecodecs implementation when available
     from scipy.ndimage.interpolation import zoom
 except ImportError:
     try:
         from ndimage.interpolation import zoom
     except ImportError:
         zoom = None
 
 
-def zstd_decode(data: bytes) -> bytes:
+Element = TypeVar('Element')
+
+
+def zstd_decode(data: bytes) -> bytes:  # noqa
     """ decode zstd bytes, copied from BioFormats ZeissCZIReader """
-    def read_var_int(stream: BytesIO) -> int:
+    def read_var_int(stream: BytesIO) -> int:  # noqa
         a = stream.read(1)[0]
         if a & 128:
             b = stream.read(1)[0]
             if b & 128:
                 c = stream.read(1)[0]
                 return (c << 14) | ((b & 127) << 7) | (a & 127)
             return (b << 7) | (a & 127)
@@ -44,63 +48,63 @@
                 chunk_id = read_var_int(stream)
                 # only one chunk ID defined so far
                 if chunk_id == 1:
                     high_low_unpacking = (stream.read(1)[0] & 1) == 1
                 else:
                     raise ValueError(f'Invalid chunk id: {chunk_id}')
             pointer = stream.tell()
-    except Exception:
+    except Exception:  # noqa
         high_low_unpacking = False
         pointer = 0
 
     decoded = imagecodecs.zstd_decode(data[pointer:])
     if high_low_unpacking:
         second_half = len(decoded) // 2
         return bytes([decoded[second_half + i // 2] if i % 2 else decoded[i // 2] for i in range(len(decoded))])
     else:
         return decoded
 
 
-def data(self, raw=False, resize=True, order=0):
+def data(self, raw: bool = False, resize: bool = True, order: int = 0) -> np.ndarray:
     """Read image data from file and return as numpy array."""
-    DECOMPRESS = czifile.czifile.DECOMPRESS
+    DECOMPRESS = czifile.czifile.DECOMPRESS  # noqa
     DECOMPRESS[5] = imagecodecs.zstd_decode
     DECOMPRESS[6] = zstd_decode
 
     de = self.directory_entry
     fh = self._fh
     if raw:
         with fh.lock:
             fh.seek(self.data_offset)
-            data = fh.read(self.data_size)
+            data = fh.read(self.data_size)  # noqa
         return data
     if de.compression:
         # if de.compression not in DECOMPRESS:
         #     raise ValueError('compression unknown or not supported')
         with fh.lock:
             fh.seek(self.data_offset)
-            data = fh.read(self.data_size)
-        data = DECOMPRESS[de.compression](data)
+            data = fh.read(self.data_size)  # noqa
+        data = DECOMPRESS[de.compression](data)  # noqa
         if de.compression == 2:
             # LZW
             data = np.fromstring(data, de.dtype)  # noqa
         elif de.compression in (5, 6):
             # ZSTD
-            data = np.frombuffer(data, de.dtype)
+            data = np.frombuffer(data, de.dtype)  # noqa
     else:
         dtype = np.dtype(de.dtype)
         with fh.lock:
             fh.seek(self.data_offset)
-            data = fh.read_array(dtype, self.data_size // dtype.itemsize)
+            data = fh.read_array(dtype, self.data_size // dtype.itemsize)  # noqa
 
-    data = data.reshape(de.stored_shape)
+    data = data.reshape(de.stored_shape)  # noqa
     if de.compression != 4 and de.stored_shape[-1] in (3, 4):
         if de.stored_shape[-1] == 3:
             # BGR -> RGB
-            data = data[..., ::-1]
+            data = data[..., ::-1]  # noqa
         else:
             # BGRA -> RGBA
             tmp = data[..., 0].copy()
             data[..., 0] = data[..., 2]
             data[..., 2] = tmp
     if de.stored_shape == de.shape or not resize:
         return data
@@ -108,15 +112,15 @@
     # sub / supersampling
     factors = [j / i for i, j in zip(de.stored_shape, de.shape)]
     factors = [(int(round(f)) if abs(f - round(f)) < 0.0001 else f)
                for f in factors]
 
     # use repeat if possible
     if order == 0 and all(isinstance(f, int) for f in factors):
-        data = repeat_nd(data, factors).copy()
+        data = repeat_nd(data, factors).copy()  # noqa
         data.shape = de.shape
         return data
 
     # remove leading dimensions with size 1 for speed
     shape = list(de.stored_shape)
     i = 0
     for s in shape:
@@ -129,55 +133,55 @@
 
     # resize RGB components separately for speed
     if zoom is None:
         raise ImportError("cannot import 'zoom' from scipy or ndimage")
     if shape[-1] in (3, 4) and factors[-1] == 1.0:
         factors = factors[:-1]
         old = data
-        data = np.empty(de.shape, de.dtype[-2:])
+        data = np.empty(de.shape, de.dtype[-2:])  # noqa
         for i in range(shape[-1]):
             data[..., i] = zoom(old[..., i], zoom=factors, order=order)
     else:
-        data = zoom(data, zoom=factors, order=order)
+        data = zoom(data, zoom=factors, order=order)  # noqa
 
     data.shape = de.shape
     return data
 
 
 # monkeypatch zstd into czifile
 czifile.czifile.SubBlockSegment.data = data
 
 
 class Reader(AbstractReader, ABC):
     priority = 0
     do_not_pickle = 'reader', 'filedict'
 
     @staticmethod
-    def _can_open(path):
+    def _can_open(path: Path) -> bool:
         return isinstance(path, Path) and path.suffix == '.czi'
 
-    def open(self):
+    def open(self) -> None:
         self.reader = czifile.CziFile(self.path)
         filedict = {}
         for directory_entry in self.reader.filtered_subblock_directory:
             idx = self.get_index(directory_entry, self.reader.start)
             if 'S' not in self.reader.axes or self.series in range(*idx[self.reader.axes.index('S')]):
                 for c in range(*idx[self.reader.axes.index('C')]):
                     for z in range(*idx[self.reader.axes.index('Z')]):
                         for t in range(*idx[self.reader.axes.index('T')]):
                             if (c, z, t) in filedict:
                                 filedict[c, z, t].append(directory_entry)
                             else:
                                 filedict[c, z, t] = [directory_entry]
         self.filedict = filedict  # noqa
 
-    def close(self):
+    def close(self) -> None:
         self.reader.close()
 
-    def get_ome(self):
+    def get_ome(self) -> OME:
         xml = self.reader.metadata()
         attachments = {i.attachment_entry.name: i.attachment_entry.data_segment()
                        for i in self.reader.attachments()}
         tree = etree.fromstring(xml)
         metadata = tree.find('Metadata')
         version = metadata.find('Version')
         if version is not None:
@@ -186,22 +190,22 @@
             version = metadata.find('Experiment').attrib['Version']
 
         if version == '1.0':
             return self.ome_10(tree, attachments)
         elif version == '1.2':
             return self.ome_12(tree, attachments)
 
-    def ome_12(self, tree, attachments):
-        def text(item, default=""):
+    def ome_12(self, tree: etree, attachments: dict[str, Any]) -> OME:
+        def text(item: Optional[Element], default: str = "") -> str:
             return default if item is None else item.text
 
-        def def_list(item):
+        def def_list(item: Any) -> list[Any]:
             return [] if item is None else item
 
-        ome = model.OME()
+        ome = OME()
 
         metadata = tree.find('Metadata')
 
         information = metadata.find('Information')
         display_setting = metadata.find('DisplaySetting')
         ome.experimenters = [model.Experimenter(id='Experimenter:0',
                                                 user_name=information.find('Document').find('UserName').text)]
@@ -231,15 +235,15 @@
                     lens_na=float(text(objective.find('LensNA'))),
                     nominal_magnification=float(text(objective.find('NominalMagnification')))))
 
         for tubelens in instrument.find('TubeLenses'):
             try:
                 nominal_magnification = float(re.findall(r'\d+(?:[,.]\d*)?',
                                                          tubelens.attrib['Name'])[0].replace(',', '.'))
-            except Exception:
+            except Exception:  # noqa
                 nominal_magnification = 1.0
 
             ome.instruments[0].objectives.append(
                 model.Objective(
                     id=f"Objective:{tubelens.attrib['Id']}",
                     model=tubelens.attrib['Name'],
                     nominal_magnification=nominal_magnification))
@@ -372,22 +376,22 @@
                         x=float(text(geometry.find('Left'))),
                         y=float(text(geometry.find('Top')))))
                 ome.rois.append(roi)
                 ome.images[0].roi_refs.append(model.ROIRef(id=f'ROI:{idx}'))
                 idx += 1
         return ome
 
-    def ome_10(self, tree, attachments):
-        def text(item, default=""):
+    def ome_10(self, tree: etree, attachments: dict[str, Any]) -> OME:
+        def text(item: Optional[Element], default: str = "") -> str:
             return default if item is None else item.text
 
-        def def_list(item):
+        def def_list(item: Any) -> list[Any]:
             return [] if item is None else item
 
-        ome = model.OME()
+        ome = OME()
 
         metadata = tree.find('Metadata')
 
         information = metadata.find('Information')
         display_setting = metadata.find('DisplaySetting')
         experiment = metadata.find('Experiment')
         acquisition_block = experiment.find('ExperimentBlocks').find('AcquisitionBlock')
@@ -576,15 +580,15 @@
                         x=float(text(geometry.find('Left'))),
                         y=float(text(geometry.find('Top')))))
                 ome.rois.append(roi)
                 ome.images[0].roi_refs.append(model.ROIRef(id=f'ROI:{idx}'))
                 idx += 1
         return ome
 
-    def __frame__(self, c=0, z=0, t=0):
+    def __frame__(self, c: int = 0, z: int = 0, t: int = 0) -> np.ndarray:
         f = np.zeros(self.base.shape['yx'], self.dtype)
         if (c, z, t) in self.filedict:
             directory_entries = self.filedict[c, z, t]
             x_min = min([f.start[f.axes.index('X')] for f in directory_entries])
             y_min = min([f.start[f.axes.index('Y')] for f in directory_entries])
             xy_min = {'X': x_min, 'Y': y_min}
             for directory_entry in directory_entries:
@@ -594,9 +598,9 @@
                 index = [slice(i - j - m, i - j + k)
                          for i, j, k, m in zip(directory_entry.start, self.reader.start, tile.shape, axes_min)]
                 index = tuple(index[self.reader.axes.index(i)] for i in 'YX')
                 f[index] = tile.squeeze()
         return f
 
     @staticmethod
-    def get_index(directory_entry, start):
+    def get_index(directory_entry: czifile.DirectoryEntryDV, start: tuple[int]) -> list[tuple[int, int]]:
         return [(i - j, i - j + k) for i, j, k in zip(directory_entry.start, start, directory_entry.shape)]
```

### Comparing `ndbioimage-2024.4.4/ndbioimage/readers/fijiread.py` & `ndbioimage-2024.4.5/ndbioimage/readers/fijiread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.4/ndbioimage/readers/ndread.py` & `ndbioimage-2024.4.5/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.4/ndbioimage/readers/seqread.py` & `ndbioimage-2024.4.5/ndbioimage/readers/seqread.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
                 pass
         return self.__dict__[field]
     return property(lazy)
 
 
 class Plane(model.Plane):
     """ Lazily retrieve delta_t from metadata """
-    def __init__(self, t0, file, **kwargs):
+    def __init__(self, t0, file, **kwargs):  # noqa
         super().__init__(**kwargs)
         # setting fields here because they would be removed by ome_types/pydantic after class definition
         setattr(self.__class__, 'delta_t', lazy_property(self.get_delta_t, 'delta_t', 't0', 'file'))
         setattr(self.__class__, 'delta_t_quantity', _quantity_property('delta_t'))
-        self.__dict__['t0'] = t0
-        self.__dict__['file'] = file
+        self.__dict__['t0'] = t0  # noqa
+        self.__dict__['file'] = file  # noqa
 
     @staticmethod
     def get_delta_t(t0, file):
         with tifffile.TiffFile(file) as tif:
             info = yaml.safe_load(tif.pages[0].tags[50839].value['Info'])
         return float((datetime.strptime(info['Time'], '%Y-%m-%d %H:%M:%S %z') - t0).seconds)
```

### Comparing `ndbioimage-2024.4.4/ndbioimage/readers/tifread.py` & `ndbioimage-2024.4.5/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.4/ndbioimage/transforms.py` & `ndbioimage-2024.4.5/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.4/pyproject.toml` & `ndbioimage-2024.4.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2024.4.4"
+version = "2024.4.5"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
-exclude = [ "ndbioimage/jars" ]
+exclude = ["ndbioimage/jars"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "*"
 pandas = "*"
 tifffile = "*"
 czifile = "2019.7.2"
@@ -20,25 +20,32 @@
 ome-types = "^0.4.0"
 pint = "*"
 tqdm = "*"
 lxml = "*"
 pyyaml = "*"
 parfor = ">=2024.3.0"
 JPype1 = "*"
-SimpleITK-SimpleElastix = "*"
+SimpleITK-SimpleElastix = [
+    { version = "*", python = "<3.12" },
+    { version = "*", python = ">=3.12", markers = "sys_platform != 'darwin'" },
+    { version = "*", python = ">=3.12", markers = "platform_machine == 'aarch64'" },
+]
 scikit-image = "*"
 imagecodecs = "*"
 xsdata = "^23"  # until pydantic is up-to-date
 pytest = { version = "*", optional = true }
 
 [tool.poetry.extras]
 test = ["pytest-xdist"]
 
 [tool.poetry.scripts]
 ndbioimage = "ndbioimage:main"
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore:::(colorcet)"]
 
+[tool.isort]
+line_length = 119
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ndbioimage-2024.4.4/PKG-INFO` & `ndbioimage-2024.4.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2024.4.4
+Version: 2024.4.5
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.8,<4.0
@@ -13,15 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: test
 Requires-Dist: JPype1
-Requires-Dist: SimpleITK-SimpleElastix
+Requires-Dist: SimpleITK-SimpleElastix ; platform_machine == "aarch64" and python_version >= "3.12"
+Requires-Dist: SimpleITK-SimpleElastix ; python_version < "3.12"
+Requires-Dist: SimpleITK-SimpleElastix ; sys_platform != "darwin" and python_version >= "3.12"
 Requires-Dist: czifile (==2019.7.2)
 Requires-Dist: imagecodecs
 Requires-Dist: lxml
 Requires-Dist: numpy
 Requires-Dist: ome-types (>=0.4.0,<0.5.0)
 Requires-Dist: pandas
 Requires-Dist: parfor (>=2024.3.0)
```

