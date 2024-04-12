# Comparing `tmp/pybud-gui-0.9.6.tar.gz` & `tmp/pybud-gui-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybud-gui-0.9.6.tar", last modified: Mon Apr  8 16:25:45 2024, max compression
+gzip compressed data, was "pybud-gui-0.9.7.tar", last modified: Fri Apr 12 10:32:48 2024, max compression
```

## Comparing `pybud-gui-0.9.6.tar` & `pybud-gui-0.9.7.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.328108 pybud-gui-0.9.6/
--rw-rw-rw-   0        0        0     4160 2024-04-08 16:25:45.326603 pybud-gui-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     3728 2024-04-06 18:44:39.000000 pybud-gui-0.9.6/README.md
--rw-rw-rw-   0        0        0      564 2024-04-08 16:25:36.000000 pybud-gui-0.9.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 16:25:45.328108 pybud-gui-0.9.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.297587 pybud-gui-0.9.6/src/
--rw-rw-rw-   0        0        0     2324 2024-04-08 15:08:08.000000 pybud-gui-0.9.6/src/example1.py
--rw-rw-rw-   0        0        0     3548 2024-04-08 16:20:34.000000 pybud-gui-0.9.6/src/example2.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.301587 pybud-gui-0.9.6/src/pybud/
--rw-rw-rw-   0        0        0     5789 2024-04-08 16:24:06.000000 pybud-gui-0.9.6/src/pybud/ansi.py
--rw-rw-rw-   0        0        0     1912 2024-04-08 14:53:41.000000 pybud-gui-0.9.6/src/pybud/deftypes.py
--rw-rw-rw-   0        0        0    20291 2024-04-08 16:15:46.000000 pybud-gui-0.9.6/src/pybud/drawer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.303588 pybud-gui-0.9.6/src/pybud/gui/
--rw-rw-rw-   0        0        0     7852 2024-04-08 15:10:27.000000 pybud-gui-0.9.6/src/pybud/gui/dialog.py
--rw-rw-rw-   0        0        0    10653 2024-04-08 16:23:39.000000 pybud-gui-0.9.6/src/pybud/gui/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.325606 pybud-gui-0.9.6/src/pybud_gui.egg-info/
--rw-rw-rw-   0        0        0     4160 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 10:32:48.325045 pybud-gui-0.9.7/
+-rw-rw-rw-   0        0        0     1715 2024-04-12 10:32:48.324076 pybud-gui-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2024-04-12 10:08:53.000000 pybud-gui-0.9.7/README.md
+-rw-rw-rw-   0        0        0      564 2024-04-12 10:31:48.000000 pybud-gui-0.9.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 10:32:48.325045 pybud-gui-0.9.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 10:32:48.276310 pybud-gui-0.9.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 10:32:48.288705 pybud-gui-0.9.7/src/pybud/
+-rw-rw-rw-   0        0        0     5789 2024-04-08 16:24:06.000000 pybud-gui-0.9.7/src/pybud/ansi.py
+-rw-rw-rw-   0        0        0     1911 2024-04-08 16:27:03.000000 pybud-gui-0.9.7/src/pybud/deftypes.py
+-rw-rw-rw-   0        0        0    20173 2024-04-10 09:15:49.000000 pybud-gui-0.9.7/src/pybud/drawing.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:32:48.303673 pybud-gui-0.9.7/src/pybud/gui/
+-rw-rw-rw-   0        0        0     7876 2024-04-12 10:30:31.000000 pybud-gui-0.9.7/src/pybud/gui/dialog.py
+-rw-rw-rw-   0        0        0    12040 2024-04-12 10:21:23.000000 pybud-gui-0.9.7/src/pybud/gui/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:32:48.323061 pybud-gui-0.9.7/src/pybud_gui.egg-info/
+-rw-rw-rw-   0        0        0     1715 2024-04-12 10:32:48.000000 pybud-gui-0.9.7/src/pybud_gui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-12 10:32:48.000000 pybud-gui-0.9.7/src/pybud_gui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 10:32:48.000000 pybud-gui-0.9.7/src/pybud_gui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-12 10:32:48.000000 pybud-gui-0.9.7/src/pybud_gui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 10:32:48.000000 pybud-gui-0.9.7/src/pybud_gui.egg-info/top_level.txt
```

### Comparing `pybud-gui-0.9.6/pyproject.toml` & `pybud-gui-0.9.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pybud-gui"
-version = "0.9.6"
+version = "0.9.7"
 dependencies = [
   "readchar==4.0.5",
 ]
 requires-python = ">= 3.10"
 authors = [
   {name = "Amirali Mollaei", email = "aam.products.mail@gmail.com"},
 ]
```

### Comparing `pybud-gui-0.9.6/src/pybud/ansi.py` & `pybud-gui-0.9.7/src/pybud/ansi.py`

 * *Files identical despite different names*

### Comparing `pybud-gui-0.9.6/src/pybud/deftypes.py` & `pybud-gui-0.9.7/src/pybud/deftypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DEFAULT_BACKGROUND_COLOR = None  # (50, 120, 200)
+DEFAULT_BACKGROUND_COLOR = None  # (90, 90, 255)
 
 
 class Point:
     def __init__(self, x: int = 0, y: int = 0) -> None:
         assert x >= 0
         assert y >= 0
         self.x = x
```

### Comparing `pybud-gui-0.9.6/src/pybud/drawer.py` & `pybud-gui-0.9.7/src/pybud/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     f = open("output.ansi", "w", encoding="utf-8")
     ansi.write = lambda x: f.write(x)
     ansi.writeln = lambda x: f.write(x + "\n")
     ansi.flush = lambda: f.flush()
 
 # ansilen = lambda x: len(ansi.remove_ansi(x))
 
-
 def get_rgb_if_exists(color: AnsiColor = None):
     return color.rgb if color is not None else None
 
 class ColoredString():
     def __init__(self, string: str, forecolor: tuple[int, int, int] = None, backcolor: tuple[int, int, int] = None, ctype: ColorType = ColorType.LEGACY):
         self.forecolor = AnsiColor(
             rgb=forecolor) if forecolor is not None else None
@@ -67,24 +66,24 @@
                 string=self.str * other,
                 forecolor=get_rgb_if_exists(self.forecolor),
                 backcolor=get_rgb_if_exists(self.backcolor)
             )
         else:
             raise NotImplementedError()
 
-    def __iadd__(self, other) -> str:
+    def __iadd__(self, other):
         return self + other
 
     @overload
     def __getitem__(self, __p: SupportsIndex): ...
 
     @overload
     def __getitem__(self, __s: slice): ...
 
-    def __getitem__(self, __p) -> 'ColoredString':
+    def __getitem__(self, __p):
         if isinstance(__p, SupportsIndex):
             return ColoredString(
                 string=self.str[__p],
                 forecolor=get_rgb_if_exists(self.forecolor),
                 backcolor=get_rgb_if_exists(self.backcolor)
             )
         elif isinstance(__p, slice):
@@ -176,15 +175,15 @@
 
     # def __add__(self, other:str):
     #    if self.forecolor == None and self.backcolor == None:
     #        return self.str + other
     #    else:
     #        other_ = ColoredString(string=self.str + other)
     #        return ColoredStringList([self, other_])
-    def __iadd__(self, other) -> str:
+    def __iadd__(self, other):
         return self + other
 
 # modify built-in string class
 # from forbiddenfruit import curse
 
 # def curse_str():
 #    def __add__(self, other: ColoredString):
@@ -233,23 +232,23 @@
     def __str__(self) -> str:
         return self.tostring(self.ctype)
 
     def __len__(self) -> int:
         return sum(map(len, self.strs))
 
     @overload
-    def __add__(self, other: 'ColoredStringList') -> 'ColoredStringList': ...
+    def __add__(self, other: 'ColoredStringList'): ...
 
     @overload
-    def __add__(self, other: ColoredString) -> 'ColoredStringList': ...
+    def __add__(self, other: ColoredString): ...
 
     @overload
-    def __add__(self, other: str) -> 'ColoredStringList': ...
+    def __add__(self, other: str): ...
 
-    def __add__(self, other) -> str:
+    def __add__(self, other):
         if isinstance(other, ColoredStringList):
             return ColoredStringList(self.strs + other.strs)
         elif isinstance(other, ColoredString):
             # return ColoredStringList(self.strs + [other]) (is not optimized)
 
             # if self.strs[-1] + other can be optimized to a single ColoredString object
             # this will return a ColoredString, else it will return a ColoredStringList
@@ -261,15 +260,15 @@
                 return ColoredStringList(self.strs[:-1] + new_last.strs)
         elif isinstance(other, str):
             return self + ColoredString(string=other)
         else:
             raise NotImplementedError(
                 f"`ColoredStringList` Only supports to be added to a \"ColoredString\", \"ColoredStringList\" or \"str\", but got \"{type(other)}\"")
 
-    def __iadd__(self, other) -> str:
+    def __iadd__(self, other):
         return self + other
 
     @overload
     def __getitem__(self, __p: SupportsIndex): ...
 
     @overload
     def __getitem__(self, __s: slice): ...
```

### Comparing `pybud-gui-0.9.6/src/pybud/gui/dialog.py` & `pybud-gui-0.9.7/src/pybud/gui/dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     from readchar import key as Key
     from readchar import readkey
 except ModuleNotFoundError:
     print("Unable to find dependency module named 'readchar', install using 'pip install readchar'")
     exit(1)
 
 import pybud.ansi as ansi
-from pybud.drawer import ColoredString as CStr
-from pybud.drawer import ColorType, Drawer
+from pybud.drawing import ColoredString as CStr
+from pybud.drawing import ColorType, Drawer
 from .widgets import Widget
 from ..deftypes import DEFAULT_BACKGROUND_COLOR
 
 LAST_SHOWN_DRAWABLE = None
 # ticks per second
 TPS = 20
 
@@ -91,15 +91,15 @@
     def draw(self):
         if not self.closed:
             self.drawing = True
             self.drawer = self.get_drawer()
 
 
 class DialogBase(Drawable):
-    def __init__(self, width: int, ctype: ColorType = None, background_color: ColorType = None):
+    def __init__(self, width: int, ctype: ColorType = None, background_color: tuple[int, int, int] = None):
         super().__init__(ctype)
         self.width = width
         self.background_color = background_color
         self.widgets: List[Widget] = []
         self.set_active_widget(0)
         self.result = None
         self.tick = 0
@@ -206,15 +206,15 @@
         s = "+ " + self.__class__.__name__ + ":\n"
         for w in self.widgets:
             s += "|   " + w.name + "\n"
         return s
 
 
 class AutoDialog(DialogBase):
-    def __init__(self, width: int, ctype: ColorType = None, background_color: ColorType = None, mode: str = "v"):
+    def __init__(self, width: int, ctype: ColorType = None, background_color: tuple[int, int, int] = None, mode: str = "v"):
         super().__init__(width, ctype)
         assert mode in ["v", "iv", "h", "ih"], f"Unknown mode \"{mode}\"!"
         self.mode = mode.lower()
         self.background_color = background_color
 
     def update(self, key):
         key = super().update(key, draw=False)
```

### Comparing `pybud-gui-0.9.6/src/pybud/gui/widgets.py` & `pybud-gui-0.9.7/src/pybud/gui/widgets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,666 +1,753 @@
 00000000: 0d0a 696d 706f 7274 2074 7970 6573 0d0a  ..import types..
 00000010: 0d0a 6672 6f6d 2070 7962 7564 2e64 7261  ..from pybud.dra
-00000020: 7765 7220 696d 706f 7274 2043 6f6c 6f72  wer import Color
-00000030: 6564 5374 7269 6e67 2061 7320 4353 7472  edString as CStr
-00000040: 0d0a 6672 6f6d 2070 7962 7564 2e64 7261  ..from pybud.dra
-00000050: 7765 7220 696d 706f 7274 2043 6f6c 6f72  wer import Color
-00000060: 6564 5374 7269 6e67 4c69 7374 2061 7320  edStringList as 
-00000070: 4353 7472 4c69 7374 0d0a 6672 6f6d 2070  CStrList..from p
-00000080: 7962 7564 2e64 7261 7765 7220 696d 706f  ybud.drawer impo
-00000090: 7274 2043 6f6c 6f72 5479 7065 2c20 4472  rt ColorType, Dr
-000000a0: 6177 6572 0d0a 6672 6f6d 2072 6561 6463  awer..from readc
-000000b0: 6861 7220 696d 706f 7274 206b 6579 2061  har import key a
-000000c0: 7320 4b65 790d 0a0d 0a66 726f 6d20 2e2e  s Key....from ..
-000000d0: 6465 6674 7970 6573 2069 6d70 6f72 7420  deftypes import 
-000000e0: 506f 696e 742c 2053 697a 652c 2044 4546  Point, Size, DEF
-000000f0: 4155 4c54 5f42 4143 4b47 524f 554e 445f  AULT_BACKGROUND_
-00000100: 434f 4c4f 520d 0a0d 0a64 6566 2064 6566  COLOR....def def
-00000110: 6175 6c74 2864 3a20 6469 6374 2c20 6b3a  ault(d: dict, k:
-00000120: 7374 722c 2064 6566 6175 6c74 293a 0d0a  str, default):..
-00000130: 2020 2020 6966 206b 2069 6e20 642e 6b65      if k in d.ke
-00000140: 7973 2829 3a0d 0a20 2020 2020 2020 2072  ys():..        r
-00000150: 6574 7572 6e20 645b 6b5d 0d0a 2020 2020  eturn d[k]..    
-00000160: 656c 7365 3a0d 0a20 2020 2020 2020 2072  else:..        r
-00000170: 6574 7572 6e20 6465 6661 756c 740d 0a0d  eturn default...
-00000180: 0a63 6c61 7373 2057 6964 6765 7442 6173  .class WidgetBas
-00000190: 6528 293a 0d0a 2020 2020 6465 6620 5f5f  e():..    def __
-000001a0: 696e 6974 5f5f 2873 656c 662c 2073 697a  init__(self, siz
-000001b0: 653a 2053 697a 6520 3d20 4e6f 6e65 2c20  e: Size = None, 
-000001c0: 706f 733a 2050 6f69 6e74 203d 2050 6f69  pos: Point = Poi
-000001d0: 6e74 2830 2c20 3029 2c20 2a2a 6b77 6172  nt(0, 0), **kwar
-000001e0: 6773 293a 0d0a 2020 2020 2020 2020 2320  gs):..        # 
-000001f0: 7365 7420 7661 7269 6162 6c65 640d 0a20  set variabled.. 
-00000200: 2020 2020 2020 2073 656c 662e 6374 7970         self.ctyp
-00000210: 6520 3d20 6465 6661 756c 7428 6b77 6172  e = default(kwar
-00000220: 6773 2c20 2263 7479 7065 222c 2043 6f6c  gs, "ctype", Col
-00000230: 6f72 5479 7065 2e4c 4547 4143 5929 0d0a  orType.LEGACY)..
-00000240: 2020 2020 2020 2020 7365 6c66 2e73 697a          self.siz
-00000250: 6520 3d20 5369 7a65 2831 302c 2032 3029  e = Size(10, 20)
-00000260: 2069 6620 7369 7a65 2069 7320 4e6f 6e65   if size is None
-00000270: 2065 6c73 6520 7369 7a65 0d0a 2020 2020   else size..    
-00000280: 2020 2020 7365 6c66 2e70 6f73 203d 2050      self.pos = P
-00000290: 6f69 6e74 2830 2c20 3029 2069 6620 706f  oint(0, 0) if po
-000002a0: 7320 6973 204e 6f6e 6520 656c 7365 2070  s is None else p
-000002b0: 6f73 0d0a 2020 2020 2020 2020 2320 6465  os..        # de
-000002c0: 6661 756c 7473 0d0a 2020 2020 2020 2020  faults..        
-000002d0: 7365 6c66 2e62 6163 6b67 726f 756e 645f  self.background_
-000002e0: 636f 6c6f 7220 3d20 4445 4641 554c 545f  color = DEFAULT_
-000002f0: 4241 434b 4752 4f55 4e44 5f43 4f4c 4f52  BACKGROUND_COLOR
-00000300: 0d0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-00000310: 616d 6520 3d20 6465 6661 756c 7428 6b77  ame = default(kw
-00000320: 6172 6773 2c20 226e 616d 6522 2c20 225f  args, "name", "_
-00000330: 5f6e 616d 655f 5f22 290d 0a20 2020 2020  _name__")..     
-00000340: 2020 2073 656c 662e 7061 7265 6e74 203d     self.parent =
-00000350: 204e 6f6e 650d 0a20 2020 2020 2020 200d   None..        .
-00000360: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00000370: 7375 6c74 203d 204e 6f6e 650d 0a0d 0a20  sult = None.... 
-00000380: 2020 2064 6566 2067 6574 5f6e 616d 6528     def get_name(
-00000390: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000003a0: 6e61 6d65 203d 2020 7365 6c66 2e5f 5f63  name =  self.__c
-000003b0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f0d  lass__.__name__.
-000003c0: 0a20 2020 2020 2020 2063 203d 2030 0d0a  .        c = 0..
-000003d0: 2020 2020 2020 2020 666f 7220 7720 696e          for w in
-000003e0: 2073 656c 662e 7061 7265 6e74 2e77 6964   self.parent.wid
-000003f0: 6765 7473 3a0d 0a20 2020 2020 2020 2020  gets:..         
-00000400: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00000410: 2877 2c20 7365 6c66 2e5f 5f63 6c61 7373  (w, self.__class
-00000420: 5f5f 293a 0d0a 2020 2020 2020 2020 2020  __):..          
-00000430: 2020 2020 2020 6320 2b3d 2031 0d0a 2020        c += 1..  
-00000440: 2020 2020 2020 7265 7475 726e 206e 616d        return nam
-00000450: 6520 2b20 225f 2220 2b20 7374 7228 632b  e + "_" + str(c+
-00000460: 3129 0d0a 0d0a 2020 2020 0d0a 2020 2020  1)....    ..    
-00000470: 6465 6620 6f6e 5f61 6464 2873 656c 662c  def on_add(self,
-00000480: 2070 6172 656e 7429 3a0d 0a20 2020 2020   parent):..     
-00000490: 2020 2073 656c 662e 7061 7265 6e74 203d     self.parent =
-000004a0: 2070 6172 656e 740d 0a20 2020 2020 2020   parent..       
-000004b0: 2069 6620 7365 6c66 2e6e 616d 6520 3d3d   if self.name ==
-000004c0: 2022 5f5f 6e61 6d65 5f5f 223a 0d0a 2020   "__name__":..  
-000004d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000004e0: 616d 6520 3d20 7365 6c66 2e67 6574 5f6e  ame = self.get_n
-000004f0: 616d 6528 290d 0a0d 0a20 2020 2064 6566  ame()....    def
-00000500: 206f 6e5f 696e 7465 7272 7570 7428 7365   on_interrupt(se
-00000510: 6c66 293a 0d0a 2020 2020 2020 2020 7061  lf):..        pa
-00000520: 7373 0d0a 0d0a 2020 2020 6465 6620 6765  ss....    def ge
-00000530: 745f 6472 6177 6572 2873 656c 6629 3a0d  t_drawer(self):.
-00000540: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000550: 4472 6177 6572 2873 697a 653d 2873 656c  Drawer(size=(sel
-00000560: 662e 7369 7a65 2e67 6574 5769 6474 6828  f.size.getWidth(
-00000570: 292c 2073 656c 662e 7369 7a65 2e67 6574  ), self.size.get
-00000580: 4865 6967 6874 2829 292c 2062 6163 6b67  Height()), backg
-00000590: 726f 756e 645f 636f 6c6f 723d 7365 6c66  round_color=self
-000005a0: 2e62 6163 6b67 726f 756e 645f 636f 6c6f  .background_colo
-000005b0: 7229 0d0a 0d0a 2020 2020 6465 6620 7265  r)....    def re
-000005c0: 6e64 6572 2873 656c 6629 3a0d 0a20 2020  nder(self):..   
-000005d0: 2020 2020 2070 6173 730d 0a0d 0a20 2020       pass....   
-000005e0: 2064 6566 2067 6574 5f72 656e 6465 7228   def get_render(
-000005f0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00000600: 7365 6c66 2e64 7261 7765 7220 3d20 7365  self.drawer = se
-00000610: 6c66 2e67 6574 5f64 7261 7765 7228 290d  lf.get_drawer().
-00000620: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00000630: 6e64 6572 2829 0d0a 2020 2020 2020 2020  nder()..        
-00000640: 7265 7475 726e 2073 656c 662e 6472 6177  return self.draw
-00000650: 6572 0d0a 0d0a 2020 2020 6465 6620 7570  er....    def up
-00000660: 6461 7465 2873 656c 662c 206b 6579 293a  date(self, key):
-00000670: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000680: 206b 6579 0d0a 0d0a 0d0a 636c 6173 7320   key......class 
-00000690: 5769 6467 6574 2857 6964 6765 7442 6173  Widget(WidgetBas
-000006a0: 6529 3a0d 0a20 2020 2064 6566 205f 5f69  e):..    def __i
-000006b0: 6e69 745f 5f28 7365 6c66 2c20 7369 7a65  nit__(self, size
-000006c0: 3a20 5369 7a65 203d 204e 6f6e 652c 2070  : Size = None, p
-000006d0: 6f73 3a20 506f 696e 7420 3d20 506f 696e  os: Point = Poin
-000006e0: 7428 302c 2030 292c 202a 2a6b 7761 7267  t(0, 0), **kwarg
-000006f0: 7329 3a0d 0a20 2020 2020 2020 2073 7570  s):..        sup
-00000700: 6572 2829 2e5f 5f69 6e69 745f 5f28 7369  er().__init__(si
-00000710: 7a65 2c20 706f 732c 202a 2a6b 7761 7267  ze, pos, **kwarg
-00000720: 7329 0d0a 2020 2020 2020 2020 2320 6465  s)..        # de
-00000730: 6661 756c 7473 0d0a 2020 2020 2020 2020  faults..        
-00000740: 7365 6c66 2e69 735f 6469 7361 626c 6564  self.is_disabled
-00000750: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
-00000760: 2020 7365 6c66 2e69 735f 7365 6c65 6374    self.is_select
-00000770: 6564 203d 2046 616c 7365 0d0a 2020 2020  ed = False..    
-00000780: 2020 2020 7365 6c66 2e73 656c 6563 7461      self.selecta
-00000790: 626c 6520 3d20 5472 7565 0d0a 0d0a 2020  ble = True....  
-000007a0: 2020 6465 6620 7275 6e5f 6361 6c6c 6261    def run_callba
-000007b0: 636b 7328 7365 6c66 293a 0d0a 2020 2020  cks(self):..    
-000007c0: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
-000007d0: 6465 6620 6f6e 5f65 6e74 6572 2873 656c  def on_enter(sel
-000007e0: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-000007f0: 7572 6e20 7365 6c66 2e72 756e 5f63 616c  urn self.run_cal
-00000800: 6c62 6163 6b73 2829 0d0a 0d0a 2020 2020  lbacks()....    
-00000810: 6465 6620 6f6e 5f69 6e74 6572 7275 7074  def on_interrupt
-00000820: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00000830: 2073 7570 6572 2829 2e6f 6e5f 696e 7465   super().on_inte
-00000840: 7272 7570 7428 290d 0a20 2020 2020 2020  rrupt()..       
-00000850: 2073 656c 662e 6973 5f64 6973 6162 6c65   self.is_disable
-00000860: 6420 3d20 5472 7565 0d0a 0d0a 2020 2020  d = True....    
-00000870: 6465 6620 7570 6461 7465 2873 656c 662c  def update(self,
-00000880: 206b 6579 293a 0d0a 2020 2020 2020 2020   key):..        
-00000890: 6b65 7920 3d20 7375 7065 7228 292e 7570  key = super().up
-000008a0: 6461 7465 286b 6579 290d 0a20 2020 2020  date(key)..     
-000008b0: 2020 2069 6620 6b65 7920 3d3d 204b 6579     if key == Key
-000008c0: 2e45 4e54 4552 3a0d 0a20 2020 2020 2020  .ENTER:..       
-000008d0: 2020 2020 2073 656c 662e 6f6e 5f65 6e74       self.on_ent
-000008e0: 6572 2829 0d0a 2020 2020 2020 2020 2020  er()..          
-000008f0: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
-00000900: 2020 7265 7475 726e 206b 6579 0d0a 0d0a    return key....
-00000910: 0d0a 636c 6173 7320 5769 6467 6574 4c61  ..class WidgetLa
-00000920: 6265 6c28 5769 6467 6574 293a 0d0a 2020  bel(Widget):..  
-00000930: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000940: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
-00000950: 2020 2020 2020 2074 6578 742c 0d0a 2020         text,..  
-00000960: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00000970: 656e 7465 7265 643a 2062 6f6f 6c20 3d20  entered: bool = 
-00000980: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00000990: 2020 2020 2020 2020 776f 7264 7772 6170          wordwrap
-000009a0: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2073 697a 653a 2053 697a 6520 3d20 4e6f   size: Size = No
-000009d0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-000009e0: 2020 2020 2020 706f 733a 2050 6f69 6e74        pos: Point
-000009f0: 203d 2050 6f69 6e74 2830 2c20 3029 2c0d   = Point(0, 0),.
-00000a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a10: 2020 2a2a 6b77 6172 6773 0d0a 2020 2020    **kwargs..    
-00000a20: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
-00000a30: 0a0d 0a20 2020 2020 2020 2073 7570 6572  ...        super
-00000a40: 2829 2e5f 5f69 6e69 745f 5f28 7369 7a65  ().__init__(size
-00000a50: 2c20 706f 732c 202a 2a6b 7761 7267 7329  , pos, **kwargs)
-00000a60: 0d0a 0d0a 2020 2020 2020 2020 6966 2069  ....        if i
-00000a70: 7369 6e73 7461 6e63 6528 7465 7874 2c20  sinstance(text, 
-00000a80: 7374 7229 3a0d 0a20 2020 2020 2020 2020  str):..         
-00000a90: 2020 2073 656c 662e 7465 7874 203d 2043     self.text = C
-00000aa0: 5374 7228 7465 7874 2c20 666f 7265 636f  Str(text, foreco
-00000ab0: 6c6f 723d 2832 3230 2c20 3232 302c 2032  lor=(220, 220, 2
-00000ac0: 3230 2929 0d0a 2020 2020 2020 2020 656c  20))..        el
-00000ad0: 6966 2069 7369 6e73 7461 6e63 6528 7465  if isinstance(te
-00000ae0: 7874 2c20 4353 7472 2920 6f72 2069 7369  xt, CStr) or isi
-00000af0: 6e73 7461 6e63 6528 7465 7874 2c20 4353  nstance(text, CS
-00000b00: 7472 4c69 7374 293a 0d0a 2020 2020 2020  trList):..      
-00000b10: 2020 2020 2020 7365 6c66 2e74 6578 7420        self.text 
-00000b20: 3d20 7465 7874 0d0a 2020 2020 2020 2020  = text..        
-00000b30: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00000b40: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-00000b50: 656d 656e 7465 6445 7272 6f72 2829 0d0a  ementedError()..
-00000b60: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00000b70: 697a 652e 6820 3d20 286c 656e 2874 6578  ize.h = (len(tex
-00000b80: 7429 202f 2f20 2873 656c 662e 7369 7a65  t) // (self.size
-00000b90: 2e77 202d 2038 2929 202b 2031 0d0a 2020  .w - 8)) + 1..  
-00000ba0: 2020 2020 2020 7365 6c66 2e63 656e 7465        self.cente
-00000bb0: 7265 6420 3d20 6365 6e74 6572 6564 0d0a  red = centered..
-00000bc0: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
-00000bd0: 6477 7261 7020 3d20 776f 7264 7772 6170  dwrap = wordwrap
-00000be0: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00000bf0: 656c 6563 7461 626c 6520 3d20 4661 6c73  electable = Fals
-00000c00: 650d 0a0d 0a20 2020 2064 6566 2072 756e  e....    def run
-00000c10: 5f63 616c 6c62 6163 6b73 2873 656c 6629  _callbacks(self)
-00000c20: 3a0d 0a20 2020 2020 2020 2070 6173 730d  :..        pass.
-00000c30: 0a0d 0a20 2020 2064 6566 205f 706c 6163  ...    def _plac
-00000c40: 655f 7465 7874 2873 656c 662c 2074 6578  e_text(self, tex
-00000c50: 742c 206c 6e5f 6964 7829 3a0d 0a20 2020  t, ln_idx):..   
-00000c60: 2020 2020 2069 6620 7365 6c66 2e63 656e       if self.cen
-00000c70: 7465 7265 643a 0d0a 2020 2020 2020 2020  tered:..        
-00000c80: 2020 2020 7365 6c66 2e64 7261 7765 722e      self.drawer.
-00000c90: 6365 6e74 6572 5f70 6c61 6365 2874 6578  center_place(tex
-00000ca0: 742c 206c 6e5f 6964 783d 6c6e 5f69 6478  t, ln_idx=ln_idx
-00000cb0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-00000cc0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000cd0: 6c66 2e64 7261 7765 722e 706c 6163 6528  lf.drawer.place(
-00000ce0: 7465 7874 2c20 706f 733d 2830 2c20 6c6e  text, pos=(0, ln
-00000cf0: 5f69 6478 2929 0d0a 0d0a 2020 2020 6465  _idx))....    de
-00000d00: 6620 706c 6163 655f 7465 7874 2873 656c  f place_text(sel
-00000d10: 662c 2074 2c20 6c6e 5f69 6478 293a 0d0a  f, t, ln_idx):..
-00000d20: 2020 2020 2020 2020 2370 7269 6e74 2874          #print(t
-00000d30: 290d 0a20 2020 2020 2020 2069 6620 6c65  )..        if le
-00000d40: 6e28 7429 203e 2028 7365 6c66 2e73 697a  n(t) > (self.siz
-00000d50: 652e 6765 7457 6964 7468 2829 202d 2038  e.getWidth() - 8
-00000d60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00000d70: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00000d80: 656e 2874 2929 3a0d 0a20 2020 2020 2020  en(t)):..       
-00000d90: 2020 2020 2020 2020 2069 5f20 3d20 6c65           i_ = le
-00000da0: 6e28 7429 202d 2069 202d 2031 0d0a 2020  n(t) - i - 1..  
-00000db0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00000dc0: 2069 5f20 3e20 2873 656c 662e 7369 7a65   i_ > (self.size
-00000dd0: 2e67 6574 5769 6474 6828 2920 2d20 3829  .getWidth() - 8)
-00000de0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000df0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00000e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e10: 2063 203d 2074 5b69 5f5d 0d0a 2020 2020   c = t[i_]..    
-00000e20: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00000e30: 7369 6e73 7461 6e63 6528 632c 2073 7472  sinstance(c, str
-00000e40: 2920 616e 6420 6320 3d3d 2022 2022 3a0d  ) and c == " ":.
-00000e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e60: 2020 2020 2073 656c 662e 5f70 6c61 6365       self._place
-00000e70: 5f74 6578 7428 745b 3a69 5f5d 2c20 6c6e  _text(t[:i_], ln
-00000e80: 5f69 6478 290d 0a20 2020 2020 2020 2020  _idx)..         
-00000e90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000ea0: 6e20 7365 6c66 2e70 6c61 6365 5f74 6578  n self.place_tex
-00000eb0: 7428 745b 695f 2b31 3a5d 2c20 6c6e 5f69  t(t[i_+1:], ln_i
-00000ec0: 6478 202b 2031 290d 0a20 2020 2020 2020  dx + 1)..       
-00000ed0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00000ee0: 7374 616e 6365 2863 2c20 4353 7472 2920  stance(c, CStr) 
-00000ef0: 616e 6420 632e 7374 7220 3d3d 2022 2022  and c.str == " "
-00000f00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000f10: 2020 2020 2020 2073 656c 662e 5f70 6c61         self._pla
-00000f20: 6365 5f74 6578 7428 745b 3a69 5f5d 2c20  ce_text(t[:i_], 
-00000f30: 6c6e 5f69 6478 290d 0a20 2020 2020 2020  ln_idx)..       
-00000f40: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00000f50: 7572 6e20 7365 6c66 2e70 6c61 6365 5f74  urn self.place_t
-00000f60: 6578 7428 745b 695f 2b31 3a5d 2c20 6c6e  ext(t[i_+1:], ln
-00000f70: 5f69 6478 202b 2031 290d 0a20 2020 2020  _idx + 1)..     
-00000f80: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000f90: 2020 2020 2020 7365 6c66 2e5f 706c 6163        self._plac
-00000fa0: 655f 7465 7874 2874 2c20 6c6e 5f69 6478  e_text(t, ln_idx
-00000fb0: 290d 0a0d 0a20 2020 2064 6566 2072 656e  )....    def ren
-00000fc0: 6465 7228 7365 6c66 293a 0d0a 2020 2020  der(self):..    
-00000fd0: 2020 2020 7365 6c66 2e70 6c61 6365 5f74      self.place_t
-00000fe0: 6578 7428 7365 6c66 2e74 6578 742c 206c  ext(self.text, l
-00000ff0: 6e5f 6964 783d 3029 0d0a 0d0a 0d0a 636c  n_idx=0)......cl
-00001000: 6173 7320 5769 6467 6574 4f70 7469 6f6e  ass WidgetOption
-00001010: 7328 5769 6467 6574 293a 0d0a 2020 2020  s(Widget):..    
-00001020: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00001030: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
-00001040: 2020 2020 206f 7074 696f 6e73 3a20 6c69       options: li
-00001050: 7374 5b74 7570 6c65 5b73 7472 2c20 7479  st[tuple[str, ty
-00001060: 7065 732e 4675 6e63 7469 6f6e 5479 7065  pes.FunctionType
-00001070: 5d5d 2c0d 0a20 2020 2020 2020 2020 2020  ]],..           
-00001080: 2020 2020 2020 7465 7874 3a20 7374 7220        text: str 
-00001090: 3d20 224f 7074 696f 6e73 3a22 2c0d 0a20  = "Options:",.. 
-000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010b0: 6465 6661 756c 745f 6f70 7469 6f6e 3a20  default_option: 
-000010c0: 696e 7420 3d20 302c 0d0a 2020 2020 2020  int = 0,..      
-000010d0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-000010e0: 2053 697a 6520 3d20 4e6f 6e65 2c0d 0a20   Size = None,.. 
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001100: 706f 733a 2050 6f69 6e74 203d 2050 6f69  pos: Point = Poi
-00001110: 6e74 2830 2c20 3029 2c0d 0a20 2020 2020  nt(0, 0),..     
-00001120: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
-00001130: 6172 6773 0d0a 2020 2020 2020 2020 2020  args..          
-00001140: 2020 2020 2020 2029 3a0d 0a0d 0a20 2020         ):....   
-00001150: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00001160: 6e69 745f 5f28 7369 7a65 2c20 706f 732c  nit__(size, pos,
-00001170: 202a 2a6b 7761 7267 7329 0d0a 2020 2020   **kwargs)..    
-00001180: 2020 2020 7365 6c66 2e6e 5f6f 7074 696f      self.n_optio
-00001190: 6e73 203d 206c 656e 286f 7074 696f 6e73  ns = len(options
-000011a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000011b0: 6f70 7469 6f6e 7320 3d20 6c69 7374 286d  options = list(m
-000011c0: 6170 286c 616d 6264 6120 783a 2078 5b30  ap(lambda x: x[0
-000011d0: 5d2c 206f 7074 696f 6e73 2929 0d0a 2020  ], options))..  
-000011e0: 2020 2020 2020 7365 6c66 2e74 6578 7420        self.text 
-000011f0: 3d20 7465 7874 0d0a 2020 2020 2020 2020  = text..        
-00001200: 7365 6c66 2e63 616c 6c62 6163 6b73 203d  self.callbacks =
-00001210: 206c 6973 7428 6d61 7028 6c61 6d62 6461   list(map(lambda
-00001220: 2078 3a20 785b 315d 2c20 6f70 7469 6f6e   x: x[1], option
-00001230: 7329 290d 0a20 2020 2020 2020 2073 656c  s))..        sel
-00001240: 662e 7365 6c65 6374 6564 203d 2064 6566  f.selected = def
-00001250: 6175 6c74 5f6f 7074 696f 6e0d 0a20 2020  ault_option..   
-00001260: 2020 2020 2073 656c 662e 7369 7a65 2e68       self.size.h
-00001270: 203d 2031 202b 2073 656c 662e 6e5f 6f70   = 1 + self.n_op
-00001280: 7469 6f6e 730d 0a0d 0a20 2020 2064 6566  tions....    def
-00001290: 2072 756e 5f63 616c 6c62 6163 6b73 2873   run_callbacks(s
-000012a0: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
-000012b0: 656c 662e 7265 7375 6c74 203d 2073 656c  elf.result = sel
-000012c0: 662e 6361 6c6c 6261 636b 735b 7365 6c66  f.callbacks[self
-000012d0: 2e73 656c 6563 7465 645d 2873 656c 662e  .selected](self.
-000012e0: 7061 7265 6e74 290d 0a20 2020 2020 2020  parent)..       
-000012f0: 2072 6574 7572 6e20 7365 6c66 2e72 6573   return self.res
-00001300: 756c 740d 0a0d 0a20 2020 2064 6566 2075  ult....    def u
-00001310: 7064 6174 6528 7365 6c66 2c20 6b65 7929  pdate(self, key)
-00001320: 3a0d 0a20 2020 2020 2020 206b 6579 203d  :..        key =
-00001330: 2073 7570 6572 2829 2e75 7064 6174 6528   super().update(
-00001340: 6b65 7929 0d0a 2020 2020 2020 2020 6966  key)..        if
-00001350: 206b 6579 203d 3d20 4b65 792e 5550 3a0d   key == Key.UP:.
-00001360: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001370: 662e 7365 6c65 6374 6564 203d 2028 7365  f.selected = (se
-00001380: 6c66 2e73 656c 6563 7465 6420 2d20 3129  lf.selected - 1)
-00001390: 2025 2073 656c 662e 6e5f 6f70 7469 6f6e   % self.n_option
-000013a0: 730d 0a20 2020 2020 2020 2020 2020 2072  s..            r
-000013b0: 6574 7572 6e0d 0a20 2020 2020 2020 2069  eturn..        i
-000013c0: 6620 6b65 7920 3d3d 204b 6579 2e44 4f57  f key == Key.DOW
-000013d0: 4e3a 0d0a 2020 2020 2020 2020 2020 2020  N:..            
-000013e0: 7365 6c66 2e73 656c 6563 7465 6420 3d20  self.selected = 
-000013f0: 2873 656c 662e 7365 6c65 6374 6564 202b  (self.selected +
-00001400: 2031 2920 2520 7365 6c66 2e6e 5f6f 7074   1) % self.n_opt
-00001410: 696f 6e73 0d0a 2020 2020 2020 2020 2020  ions..          
-00001420: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
-00001430: 2020 7265 7475 726e 206b 6579 0d0a 0d0a    return key....
-00001440: 2020 2020 6465 6620 7265 6e64 6572 2873      def render(s
-00001450: 656c 6629 3a0d 0a20 2020 2020 2020 2063  elf):..        c
-00001460: 6170 7469 6f6e 5f73 7461 7274 203d 2032  aption_start = 2
-00001470: 0d0a 2020 2020 2020 2020 5f5f 6f70 7469  ..        __opti
-00001480: 6f6e 7320 3d20 7365 6c66 2e74 6578 742e  ons = self.text.
-00001490: 6c6a 7573 7428 7365 6c66 2e73 697a 652e  ljust(self.size.
-000014a0: 6765 7457 6964 7468 2829 2d63 6170 7469  getWidth()-capti
-000014b0: 6f6e 5f73 7461 7274 290d 0a20 2020 2020  on_start)..     
-000014c0: 2020 2073 656c 662e 6472 6177 6572 2e70     self.drawer.p
-000014d0: 6c61 6365 2843 5374 7228 5f5f 6f70 7469  lace(CStr(__opti
-000014e0: 6f6e 732c 2066 6f72 6563 6f6c 6f72 3d28  ons, forecolor=(
-000014f0: 0d0a 2020 2020 2020 2020 2020 2020 3232  ..            22
-00001500: 302c 2032 3230 2c20 3232 3029 292c 2070  0, 220, 220)), p
-00001510: 6f73 3d28 6361 7074 696f 6e5f 7374 6172  os=(caption_star
-00001520: 742c 2030 2929 0d0a 2020 2020 2020 2020  t, 0))..        
-00001530: 666f 7220 692c 206f 7074 696f 6e20 696e  for i, option in
-00001540: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
-00001550: 6f70 7469 6f6e 7329 3a0d 0a20 2020 2020  options):..     
-00001560: 2020 2020 2020 2069 6620 6920 3d3d 2073         if i == s
-00001570: 656c 662e 7365 6c65 6374 6564 3a0d 0a20  elf.selected:.. 
-00001580: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00001590: 7074 696f 6e5f 636f 6c6f 7220 3d20 2835  ption_color = (5
-000015a0: 302c 2032 3230 2c20 3830 290d 0a20 2020  0, 220, 80)..   
-000015b0: 2020 2020 2020 2020 2020 2020 206f 7074               opt
-000015c0: 696f 6e5f 696e 6469 6361 746f 7220 3d20  ion_indicator = 
-000015d0: 4353 7472 2822 3e20 222c 2066 6f72 6563  CStr("> ", forec
-000015e0: 6f6c 6f72 3d28 3232 302c 2032 3230 2c20  olor=(220, 220, 
-000015f0: 3232 3029 290d 0a20 2020 2020 2020 2020  220))..         
-00001600: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00001610: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-00001620: 5f63 6f6c 6f72 203d 2028 3232 302c 2032  _color = (220, 2
-00001630: 3230 2c20 3232 3029 0d0a 2020 2020 2020  20, 220)..      
-00001640: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-00001650: 5f69 6e64 6963 6174 6f72 203d 2043 5374  _indicator = CSt
-00001660: 7228 2220 2022 2c20 666f 7265 636f 6c6f  r("  ", forecolo
-00001670: 723d 2832 3230 2c20 3232 302c 2032 3230  r=(220, 220, 220
-00001680: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00001690: 5f5f 6f70 7469 6f6e 203d 2043 5374 7228  __option = CStr(
-000016a0: 6f70 7469 6f6e 2c20 666f 7265 636f 6c6f  option, forecolo
-000016b0: 723d 6f70 7469 6f6e 5f63 6f6c 6f72 290d  r=option_color).
-000016c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000016d0: 662e 6472 6177 6572 2e70 6c61 6365 286f  f.drawer.place(o
-000016e0: 7074 696f 6e5f 696e 6469 6361 746f 7220  ption_indicator 
-000016f0: 2b20 5f5f 6f70 7469 6f6e 2c0d 0a20 2020  + __option,..   
+00000020: 7769 6e67 2069 6d70 6f72 7420 436f 6c6f  wing import Colo
+00000030: 7265 6453 7472 696e 6720 6173 2043 5374  redString as CSt
+00000040: 720d 0a66 726f 6d20 7079 6275 642e 6472  r..from pybud.dr
+00000050: 6177 696e 6720 696d 706f 7274 2043 6f6c  awing import Col
+00000060: 6f72 6564 5374 7269 6e67 4c69 7374 2061  oredStringList a
+00000070: 7320 4353 7472 4c69 7374 0d0a 6672 6f6d  s CStrList..from
+00000080: 2070 7962 7564 2e64 7261 7769 6e67 2069   pybud.drawing i
+00000090: 6d70 6f72 7420 436f 6c6f 7254 7970 652c  mport ColorType,
+000000a0: 2044 7261 7765 720d 0a66 726f 6d20 7265   Drawer..from re
+000000b0: 6164 6368 6172 2069 6d70 6f72 7420 6b65  adchar import ke
+000000c0: 7920 6173 204b 6579 0d0a 0d0a 6672 6f6d  y as Key....from
+000000d0: 202e 2e64 6566 7479 7065 7320 696d 706f   ..deftypes impo
+000000e0: 7274 2050 6f69 6e74 2c20 5369 7a65 2c20  rt Point, Size, 
+000000f0: 4445 4641 554c 545f 4241 434b 4752 4f55  DEFAULT_BACKGROU
+00000100: 4e44 5f43 4f4c 4f52 0d0a 0d0a 6465 6620  ND_COLOR....def 
+00000110: 6465 6661 756c 7428 643a 2064 6963 742c  default(d: dict,
+00000120: 206b 3a73 7472 2c20 6465 6661 756c 7429   k:str, default)
+00000130: 3a0d 0a20 2020 2069 6620 6b20 696e 2064  :..    if k in d
+00000140: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+00000150: 2020 7265 7475 726e 2064 5b6b 5d0d 0a20    return d[k].. 
+00000160: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000170: 2020 7265 7475 726e 2064 6566 6175 6c74    return default
+00000180: 0d0a 0d0a 636c 6173 7320 5769 6467 6574  ....class Widget
+00000190: 4261 7365 2829 3a0d 0a20 2020 2064 6566  Base():..    def
+000001a0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+000001b0: 7369 7a65 3a20 5369 7a65 203d 204e 6f6e  size: Size = Non
+000001c0: 652c 2070 6f73 3a20 506f 696e 7420 3d20  e, pos: Point = 
+000001d0: 506f 696e 7428 302c 2030 292c 202a 2a6b  Point(0, 0), **k
+000001e0: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+000001f0: 2023 2073 6574 2076 6172 6961 626c 6564   # set variabled
+00000200: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00000210: 7479 7065 203d 2064 6566 6175 6c74 286b  type = default(k
+00000220: 7761 7267 732c 2022 6374 7970 6522 2c20  wargs, "ctype", 
+00000230: 436f 6c6f 7254 7970 652e 4c45 4741 4359  ColorType.LEGACY
+00000240: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00000250: 7369 7a65 203d 2053 697a 6528 3130 2c20  size = Size(10, 
+00000260: 3230 2920 6966 2073 697a 6520 6973 204e  20) if size is N
+00000270: 6f6e 6520 656c 7365 2073 697a 650d 0a20  one else size.. 
+00000280: 2020 2020 2020 2073 656c 662e 706f 7320         self.pos 
+00000290: 3d20 506f 696e 7428 302c 2030 2920 6966  = Point(0, 0) if
+000002a0: 2070 6f73 2069 7320 4e6f 6e65 2065 6c73   pos is None els
+000002b0: 6520 706f 730d 0a20 2020 2020 2020 2023  e pos..        #
+000002c0: 2064 6566 6175 6c74 730d 0a20 2020 2020   defaults..     
+000002d0: 2020 2073 656c 662e 6261 636b 6772 6f75     self.backgrou
+000002e0: 6e64 5f63 6f6c 6f72 203d 2044 4546 4155  nd_color = DEFAU
+000002f0: 4c54 5f42 4143 4b47 524f 554e 445f 434f  LT_BACKGROUND_CO
+00000300: 4c4f 520d 0a20 2020 2020 2020 2073 656c  LOR..        sel
+00000310: 662e 6e61 6d65 203d 2064 6566 6175 6c74  f.name = default
+00000320: 286b 7761 7267 732c 2022 6e61 6d65 222c  (kwargs, "name",
+00000330: 2022 5f5f 6e61 6d65 5f5f 2229 0d0a 2020   "__name__")..  
+00000340: 2020 2020 2020 7365 6c66 2e70 6172 656e        self.paren
+00000350: 7420 3d20 4e6f 6e65 0d0a 2020 2020 2020  t = None..      
+00000360: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+00000370: 2e72 6573 756c 7420 3d20 4e6f 6e65 0d0a  .result = None..
+00000380: 0d0a 2020 2020 6465 6620 6765 745f 6e61  ..    def get_na
+00000390: 6d65 2873 656c 6629 3a0d 0a20 2020 2020  me(self):..     
+000003a0: 2020 206e 616d 6520 3d20 2073 656c 662e     name =  self.
+000003b0: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
+000003c0: 5f5f 0d0a 2020 2020 2020 2020 6320 3d20  __..        c = 
+000003d0: 300d 0a20 2020 2020 2020 2066 6f72 2077  0..        for w
+000003e0: 2069 6e20 7365 6c66 2e70 6172 656e 742e   in self.parent.
+000003f0: 7769 6467 6574 733a 0d0a 2020 2020 2020  widgets:..      
+00000400: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00000410: 6e63 6528 772c 2073 656c 662e 5f5f 636c  nce(w, self.__cl
+00000420: 6173 735f 5f29 3a0d 0a20 2020 2020 2020  ass__):..       
+00000430: 2020 2020 2020 2020 2063 202b 3d20 310d           c += 1.
+00000440: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000450: 6e61 6d65 202b 2022 5f22 202b 2073 7472  name + "_" + str
+00000460: 2863 2b31 290d 0a0d 0a20 2020 200d 0a20  (c+1)....    .. 
+00000470: 2020 2064 6566 206f 6e5f 6164 6428 7365     def on_add(se
+00000480: 6c66 2c20 7061 7265 6e74 293a 0d0a 2020  lf, parent):..  
+00000490: 2020 2020 2020 7365 6c66 2e70 6172 656e        self.paren
+000004a0: 7420 3d20 7061 7265 6e74 0d0a 2020 2020  t = parent..    
+000004b0: 2020 2020 6966 2073 656c 662e 6e61 6d65      if self.name
+000004c0: 203d 3d20 225f 5f6e 616d 655f 5f22 3a0d   == "__name__":.
+000004d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000004e0: 662e 6e61 6d65 203d 2073 656c 662e 6765  f.name = self.ge
+000004f0: 745f 6e61 6d65 2829 0d0a 0d0a 2020 2020  t_name()....    
+00000500: 6465 6620 6f6e 5f69 6e74 6572 7275 7074  def on_interrupt
+00000510: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000520: 2070 6173 730d 0a0d 0a20 2020 2064 6566   pass....    def
+00000530: 2067 6574 5f64 7261 7765 7228 7365 6c66   get_drawer(self
+00000540: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+00000550: 726e 2044 7261 7765 7228 7369 7a65 3d28  rn Drawer(size=(
+00000560: 7365 6c66 2e73 697a 652e 6765 7457 6964  self.size.getWid
+00000570: 7468 2829 2c20 7365 6c66 2e73 697a 652e  th(), self.size.
+00000580: 6765 7448 6569 6768 7428 2929 2c20 6261  getHeight()), ba
+00000590: 636b 6772 6f75 6e64 5f63 6f6c 6f72 3d73  ckground_color=s
+000005a0: 656c 662e 6261 636b 6772 6f75 6e64 5f63  elf.background_c
+000005b0: 6f6c 6f72 290d 0a0d 0a20 2020 2064 6566  olor)....    def
+000005c0: 2072 656e 6465 7228 7365 6c66 293a 0d0a   render(self):..
+000005d0: 2020 2020 2020 2020 7061 7373 0d0a 0d0a          pass....
+000005e0: 2020 2020 6465 6620 6765 745f 7265 6e64      def get_rend
+000005f0: 6572 2873 656c 6629 3a0d 0a20 2020 2020  er(self):..     
+00000600: 2020 2073 656c 662e 6472 6177 6572 203d     self.drawer =
+00000610: 2073 656c 662e 6765 745f 6472 6177 6572   self.get_drawer
+00000620: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+00000630: 2e72 656e 6465 7228 290d 0a20 2020 2020  .render()..     
+00000640: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
+00000650: 7261 7765 720d 0a0d 0a20 2020 2064 6566  rawer....    def
+00000660: 2075 7064 6174 6528 7365 6c66 2c20 6b65   update(self, ke
+00000670: 7929 3a0d 0a20 2020 2020 2020 2072 6574  y):..        ret
+00000680: 7572 6e20 6b65 790d 0a0d 0a0d 0a63 6c61  urn key......cla
+00000690: 7373 2057 6964 6765 7428 5769 6467 6574  ss Widget(Widget
+000006a0: 4261 7365 293a 0d0a 2020 2020 6465 6620  Base):..    def 
+000006b0: 5f5f 696e 6974 5f5f 2873 656c 662c 2073  __init__(self, s
+000006c0: 697a 653a 2053 697a 6520 3d20 4e6f 6e65  ize: Size = None
+000006d0: 2c20 706f 733a 2050 6f69 6e74 203d 2050  , pos: Point = P
+000006e0: 6f69 6e74 2830 2c20 3029 2c20 2a2a 6b77  oint(0, 0), **kw
+000006f0: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00000700: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00000710: 2873 697a 652c 2070 6f73 2c20 2a2a 6b77  (size, pos, **kw
+00000720: 6172 6773 290d 0a20 2020 2020 2020 2023  args)..        #
+00000730: 2064 6566 6175 6c74 730d 0a20 2020 2020   defaults..     
+00000740: 2020 2073 656c 662e 6973 5f64 6973 6162     self.is_disab
+00000750: 6c65 6420 3d20 4661 6c73 650d 0a20 2020  led = False..   
+00000760: 2020 2020 2073 656c 662e 6973 5f73 656c       self.is_sel
+00000770: 6563 7465 6420 3d20 4661 6c73 650d 0a20  ected = False.. 
+00000780: 2020 2020 2020 2073 656c 662e 7365 6c65         self.sele
+00000790: 6374 6162 6c65 203d 2054 7275 650d 0a0d  ctable = True...
+000007a0: 0a20 2020 2064 6566 2072 756e 5f63 616c  .    def run_cal
+000007b0: 6c62 6163 6b73 2873 656c 6629 3a0d 0a20  lbacks(self):.. 
+000007c0: 2020 2020 2020 2070 6173 730d 0a0d 0a20         pass.... 
+000007d0: 2020 2064 6566 206f 6e5f 656e 7465 7228     def on_enter(
+000007e0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000007f0: 7265 7475 726e 2073 656c 662e 7275 6e5f  return self.run_
+00000800: 6361 6c6c 6261 636b 7328 290d 0a0d 0a20  callbacks().... 
+00000810: 2020 2064 6566 206f 6e5f 696e 7465 7272     def on_interr
+00000820: 7570 7428 7365 6c66 293a 0d0a 2020 2020  upt(self):..    
+00000830: 2020 2020 7375 7065 7228 292e 6f6e 5f69      super().on_i
+00000840: 6e74 6572 7275 7074 2829 0d0a 2020 2020  nterrupt()..    
+00000850: 2020 2020 7365 6c66 2e69 735f 6469 7361      self.is_disa
+00000860: 626c 6564 203d 2054 7275 650d 0a0d 0a20  bled = True.... 
+00000870: 2020 2064 6566 2075 7064 6174 6528 7365     def update(se
+00000880: 6c66 2c20 6b65 7929 3a0d 0a20 2020 2020  lf, key):..     
+00000890: 2020 206b 6579 203d 2073 7570 6572 2829     key = super()
+000008a0: 2e75 7064 6174 6528 6b65 7929 0d0a 2020  .update(key)..  
+000008b0: 2020 2020 2020 6966 206b 6579 203d 3d20        if key == 
+000008c0: 4b65 792e 454e 5445 523a 0d0a 2020 2020  Key.ENTER:..    
+000008d0: 2020 2020 2020 2020 7365 6c66 2e6f 6e5f          self.on_
+000008e0: 656e 7465 7228 290d 0a20 2020 2020 2020  enter()..       
+000008f0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+00000900: 2020 2020 2072 6574 7572 6e20 6b65 790d       return key.
+00000910: 0a0d 0a0d 0a63 6c61 7373 2057 6964 6765  .....class Widge
+00000920: 744c 6162 656c 2857 6964 6765 7429 3a0d  tLabel(Widget):.
+00000930: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00000940: 5f28 7365 6c66 2c0d 0a20 2020 2020 2020  _(self,..       
+00000950: 2020 2020 2020 2020 2020 7465 7874 2c0d            text,.
+00000960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000970: 2020 6365 6e74 6572 6564 3a20 626f 6f6c    centered: bool
+00000980: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
+00000990: 2020 2020 2020 2020 2020 2077 6f72 6477             wordw
+000009a0: 7261 703a 2062 6f6f 6c20 3d20 5472 7565  rap: bool = True
+000009b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000009c0: 2020 2020 7369 7a65 3a20 5369 7a65 203d      size: Size =
+000009d0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+000009e0: 2020 2020 2020 2020 2070 6f73 3a20 506f           pos: Po
+000009f0: 696e 7420 3d20 506f 696e 7428 302c 2030  int = Point(0, 0
+00000a00: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00000a10: 2020 2020 202a 2a6b 7761 7267 730d 0a20       **kwargs.. 
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 293a 0d0a 0d0a 2020 2020 2020 2020 7375  ):....        su
+00000a40: 7065 7228 292e 5f5f 696e 6974 5f5f 2873  per().__init__(s
+00000a50: 697a 652c 2070 6f73 2c20 2a2a 6b77 6172  ize, pos, **kwar
+00000a60: 6773 290d 0a0d 0a20 2020 2020 2020 2069  gs)....        i
+00000a70: 6620 6973 696e 7374 616e 6365 2874 6578  f isinstance(tex
+00000a80: 742c 2073 7472 293a 0d0a 2020 2020 2020  t, str):..      
+00000a90: 2020 2020 2020 7365 6c66 2e74 6578 7420        self.text 
+00000aa0: 3d20 4353 7472 2874 6578 742c 2066 6f72  = CStr(text, for
+00000ab0: 6563 6f6c 6f72 3d28 3232 302c 2032 3230  ecolor=(220, 220
+00000ac0: 2c20 3232 3029 290d 0a20 2020 2020 2020  , 220))..       
+00000ad0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00000ae0: 2874 6578 742c 2043 5374 7229 206f 7220  (text, CStr) or 
+00000af0: 6973 696e 7374 616e 6365 2874 6578 742c  isinstance(text,
+00000b00: 2043 5374 724c 6973 7429 3a0d 0a20 2020   CStrList):..   
+00000b10: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00000b20: 7874 203d 2074 6578 740d 0a20 2020 2020  xt = text..     
+00000b30: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000b40: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+00000b50: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+00000b60: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+00000b70: 662e 7369 7a65 2e68 203d 2028 6c65 6e28  f.size.h = (len(
+00000b80: 7465 7874 2920 2f2f 2028 7365 6c66 2e73  text) // (self.s
+00000b90: 697a 652e 7720 2d20 3829 2920 2b20 310d  ize.w - 8)) + 1.
+00000ba0: 0a20 2020 2020 2020 2073 656c 662e 6365  .        self.ce
+00000bb0: 6e74 6572 6564 203d 2063 656e 7465 7265  ntered = centere
+00000bc0: 640d 0a20 2020 2020 2020 2073 656c 662e  d..        self.
+00000bd0: 776f 7264 7772 6170 203d 2077 6f72 6477  wordwrap = wordw
+00000be0: 7261 700d 0a20 2020 2020 2020 2073 656c  rap..        sel
+00000bf0: 662e 7365 6c65 6374 6162 6c65 203d 2046  f.selectable = F
+00000c00: 616c 7365 0d0a 0d0a 2020 2020 6465 6620  alse....    def 
+00000c10: 7275 6e5f 6361 6c6c 6261 636b 7328 7365  run_callbacks(se
+00000c20: 6c66 293a 0d0a 2020 2020 2020 2020 7061  lf):..        pa
+00000c30: 7373 0d0a 0d0a 2020 2020 6465 6620 5f70  ss....    def _p
+00000c40: 6c61 6365 5f74 6578 7428 7365 6c66 2c20  lace_text(self, 
+00000c50: 7465 7874 2c20 6c6e 5f69 6478 293a 0d0a  text, ln_idx):..
+00000c60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00000c70: 6365 6e74 6572 6564 3a0d 0a20 2020 2020  centered:..     
+00000c80: 2020 2020 2020 2073 656c 662e 6472 6177         self.draw
+00000c90: 6572 2e63 656e 7465 725f 706c 6163 6528  er.center_place(
+00000ca0: 7465 7874 2c20 6c6e 5f69 6478 3d6c 6e5f  text, ln_idx=ln_
+00000cb0: 6964 7829 0d0a 2020 2020 2020 2020 656c  idx)..        el
+00000cc0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000cd0: 2073 656c 662e 6472 6177 6572 2e70 6c61   self.drawer.pla
+00000ce0: 6365 2874 6578 742c 2070 6f73 3d28 302c  ce(text, pos=(0,
+00000cf0: 206c 6e5f 6964 7829 290d 0a0d 0a20 2020   ln_idx))....   
+00000d00: 2064 6566 2070 6c61 6365 5f74 6578 7428   def place_text(
+00000d10: 7365 6c66 2c20 742c 206c 6e5f 6964 7829  self, t, ln_idx)
+00000d20: 3a0d 0a20 2020 2020 2020 2023 7072 696e  :..        #prin
+00000d30: 7428 7429 0d0a 2020 2020 2020 2020 6966  t(t)..        if
+00000d40: 206c 656e 2874 2920 3e20 2873 656c 662e   len(t) > (self.
+00000d50: 7369 7a65 2e67 6574 5769 6474 6828 2920  size.getWidth() 
+00000d60: 2d20 3829 3a0d 0a20 2020 2020 2020 2020  - 8):..         
+00000d70: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00000d80: 6528 6c65 6e28 7429 293a 0d0a 2020 2020  e(len(t)):..    
+00000d90: 2020 2020 2020 2020 2020 2020 695f 203d              i_ =
+00000da0: 206c 656e 2874 2920 2d20 6920 2d20 310d   len(t) - i - 1.
+00000db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000dc0: 2069 6620 695f 203e 2028 7365 6c66 2e73   if i_ > (self.s
+00000dd0: 697a 652e 6765 7457 6964 7468 2829 202d  ize.getWidth() -
+00000de0: 2038 293a 0d0a 2020 2020 2020 2020 2020   8):..          
+00000df0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00000e00: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00000e10: 2020 2020 6320 3d20 745b 695f 5d0d 0a20      c = t[i_].. 
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000e30: 6620 6973 696e 7374 616e 6365 2863 2c20  f isinstance(c, 
+00000e40: 7374 7229 2061 6e64 2063 203d 3d20 2220  str) and c == " 
+00000e50: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00000e60: 2020 2020 2020 2020 7365 6c66 2e5f 706c          self._pl
+00000e70: 6163 655f 7465 7874 2874 5b3a 695f 5d2c  ace_text(t[:i_],
+00000e80: 206c 6e5f 6964 7829 0d0a 2020 2020 2020   ln_idx)..      
+00000e90: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000ea0: 7475 726e 2073 656c 662e 706c 6163 655f  turn self.place_
+00000eb0: 7465 7874 2874 5b69 5f2b 313a 5d2c 206c  text(t[i_+1:], l
+00000ec0: 6e5f 6964 7820 2b20 3129 0d0a 2020 2020  n_idx + 1)..    
+00000ed0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00000ee0: 7369 6e73 7461 6e63 6528 632c 2043 5374  sinstance(c, CSt
+00000ef0: 7229 2061 6e64 2063 2e73 7472 203d 3d20  r) and c.str == 
+00000f00: 2220 223a 0d0a 2020 2020 2020 2020 2020  " ":..          
+00000f10: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00000f20: 706c 6163 655f 7465 7874 2874 5b3a 695f  place_text(t[:i_
+00000f30: 5d2c 206c 6e5f 6964 7829 0d0a 2020 2020  ], ln_idx)..    
+00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f50: 7265 7475 726e 2073 656c 662e 706c 6163  return self.plac
+00000f60: 655f 7465 7874 2874 5b69 5f2b 313a 5d2c  e_text(t[i_+1:],
+00000f70: 206c 6e5f 6964 7820 2b20 3129 0d0a 2020   ln_idx + 1)..  
+00000f80: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00000f90: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+00000fa0: 6c61 6365 5f74 6578 7428 742c 206c 6e5f  lace_text(t, ln_
+00000fb0: 6964 7829 0d0a 0d0a 2020 2020 6465 6620  idx)....    def 
+00000fc0: 7265 6e64 6572 2873 656c 6629 3a0d 0a20  render(self):.. 
+00000fd0: 2020 2020 2020 2073 656c 662e 706c 6163         self.plac
+00000fe0: 655f 7465 7874 2873 656c 662e 7465 7874  e_text(self.text
+00000ff0: 2c20 6c6e 5f69 6478 3d30 290d 0a0d 0a0d  , ln_idx=0).....
+00001000: 0a63 6c61 7373 2057 6964 6765 744f 7074  .class WidgetOpt
+00001010: 696f 6e73 2857 6964 6765 7429 3a0d 0a20  ions(Widget):.. 
+00001020: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00001030: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00001040: 2020 2020 2020 2020 6f70 7469 6f6e 733a          options:
+00001050: 206c 6973 745b 7475 706c 655b 7374 722c   list[tuple[str,
+00001060: 2074 7970 6573 2e46 756e 6374 696f 6e54   types.FunctionT
+00001070: 7970 655d 5d2c 0d0a 2020 2020 2020 2020  ype]],..        
+00001080: 2020 2020 2020 2020 2074 6578 743a 2073           text: s
+00001090: 7472 203d 2022 4f70 7469 6f6e 733a 222c  tr = "Options:",
+000010a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000010b0: 2020 2064 6566 6175 6c74 5f6f 7074 696f     default_optio
+000010c0: 6e3a 2069 6e74 203d 2030 2c0d 0a20 2020  n: int = 0,..   
+000010d0: 2020 2020 2020 2020 2020 2020 2020 7369                si
+000010e0: 7a65 3a20 5369 7a65 203d 204e 6f6e 652c  ze: Size = None,
+000010f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001100: 2020 2070 6f73 3a20 506f 696e 7420 3d20     pos: Point = 
+00001110: 506f 696e 7428 302c 2030 292c 0d0a 2020  Point(0, 0),..  
+00001120: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00001130: 2a6b 7761 7267 730d 0a20 2020 2020 2020  *kwargs..       
+00001140: 2020 2020 2020 2020 2020 293a 0d0a 0d0a            ):....
+00001150: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00001160: 5f5f 696e 6974 5f5f 2873 697a 652c 2070  __init__(size, p
+00001170: 6f73 2c20 2a2a 6b77 6172 6773 290d 0a20  os, **kwargs).. 
+00001180: 2020 2020 2020 2073 656c 662e 6e5f 6f70         self.n_op
+00001190: 7469 6f6e 7320 3d20 6c65 6e28 6f70 7469  tions = len(opti
+000011a0: 6f6e 7329 0d0a 2020 2020 2020 2020 7365  ons)..        se
+000011b0: 6c66 2e6f 7074 696f 6e73 203d 206c 6973  lf.options = lis
+000011c0: 7428 6d61 7028 6c61 6d62 6461 2078 3a20  t(map(lambda x: 
+000011d0: 785b 305d 2c20 6f70 7469 6f6e 7329 290d  x[0], options)).
+000011e0: 0a20 2020 2020 2020 2073 656c 662e 7465  .        self.te
+000011f0: 7874 203d 2074 6578 740d 0a20 2020 2020  xt = text..     
+00001200: 2020 2073 656c 662e 6361 6c6c 6261 636b     self.callback
+00001210: 7320 3d20 6c69 7374 286d 6170 286c 616d  s = list(map(lam
+00001220: 6264 6120 783a 2078 5b31 5d2c 206f 7074  bda x: x[1], opt
+00001230: 696f 6e73 2929 0d0a 2020 2020 2020 2020  ions))..        
+00001240: 7365 6c66 2e73 656c 6563 7465 6420 3d20  self.selected = 
+00001250: 6465 6661 756c 745f 6f70 7469 6f6e 0d0a  default_option..
+00001260: 2020 2020 2020 2020 7365 6c66 2e73 697a          self.siz
+00001270: 652e 6820 3d20 3120 2b20 7365 6c66 2e6e  e.h = 1 + self.n
+00001280: 5f6f 7074 696f 6e73 0d0a 0d0a 2020 2020  _options....    
+00001290: 6465 6620 7275 6e5f 6361 6c6c 6261 636b  def run_callback
+000012a0: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
+000012b0: 2020 7365 6c66 2e72 6573 756c 7420 3d20    self.result = 
+000012c0: 7365 6c66 2e63 616c 6c62 6163 6b73 5b73  self.callbacks[s
+000012d0: 656c 662e 7365 6c65 6374 6564 5d28 7365  elf.selected](se
+000012e0: 6c66 2e70 6172 656e 7429 0d0a 2020 2020  lf.parent)..    
+000012f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00001300: 7265 7375 6c74 0d0a 0d0a 2020 2020 6465  result....    de
+00001310: 6620 7570 6461 7465 2873 656c 662c 206b  f update(self, k
+00001320: 6579 293a 0d0a 2020 2020 2020 2020 6b65  ey):..        ke
+00001330: 7920 3d20 7375 7065 7228 292e 7570 6461  y = super().upda
+00001340: 7465 286b 6579 290d 0a20 2020 2020 2020  te(key)..       
+00001350: 2069 6620 6b65 7920 3d3d 204b 6579 2e55   if key == Key.U
+00001360: 503a 0d0a 2020 2020 2020 2020 2020 2020  P:..            
+00001370: 7365 6c66 2e73 656c 6563 7465 6420 3d20  self.selected = 
+00001380: 2873 656c 662e 7365 6c65 6374 6564 202d  (self.selected -
+00001390: 2031 2920 2520 7365 6c66 2e6e 5f6f 7074   1) % self.n_opt
+000013a0: 696f 6e73 0d0a 2020 2020 2020 2020 2020  ions..          
+000013b0: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
+000013c0: 2020 6966 206b 6579 203d 3d20 4b65 792e    if key == Key.
+000013d0: 444f 574e 3a0d 0a20 2020 2020 2020 2020  DOWN:..         
+000013e0: 2020 2073 656c 662e 7365 6c65 6374 6564     self.selected
+000013f0: 203d 2028 7365 6c66 2e73 656c 6563 7465   = (self.selecte
+00001400: 6420 2b20 3129 2025 2073 656c 662e 6e5f  d + 1) % self.n_
+00001410: 6f70 7469 6f6e 730d 0a20 2020 2020 2020  options..       
+00001420: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+00001430: 2020 2020 2072 6574 7572 6e20 6b65 790d       return key.
+00001440: 0a0d 0a20 2020 2064 6566 2072 656e 6465  ...    def rende
+00001450: 7228 7365 6c66 293a 0d0a 2020 2020 2020  r(self):..      
+00001460: 2020 6361 7074 696f 6e5f 7374 6172 7420    caption_start 
+00001470: 3d20 320d 0a20 2020 2020 2020 205f 5f6f  = 2..        __o
+00001480: 7074 696f 6e73 203d 2073 656c 662e 7465  ptions = self.te
+00001490: 7874 2e6c 6a75 7374 2873 656c 662e 7369  xt.ljust(self.si
+000014a0: 7a65 2e67 6574 5769 6474 6828 292d 6361  ze.getWidth()-ca
+000014b0: 7074 696f 6e5f 7374 6172 7429 0d0a 2020  ption_start)..  
+000014c0: 2020 2020 2020 7365 6c66 2e64 7261 7765        self.drawe
+000014d0: 722e 706c 6163 6528 4353 7472 285f 5f6f  r.place(CStr(__o
+000014e0: 7074 696f 6e73 2c20 666f 7265 636f 6c6f  ptions, forecolo
+000014f0: 723d 280d 0a20 2020 2020 2020 2020 2020  r=(..           
+00001500: 2032 3230 2c20 3232 302c 2032 3230 2929   220, 220, 220))
+00001510: 2c20 706f 733d 2863 6170 7469 6f6e 5f73  , pos=(caption_s
+00001520: 7461 7274 2c20 3029 290d 0a20 2020 2020  tart, 0))..     
+00001530: 2020 2066 6f72 2069 2c20 6f70 7469 6f6e     for i, option
+00001540: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
+00001550: 6c66 2e6f 7074 696f 6e73 293a 0d0a 2020  lf.options):..  
+00001560: 2020 2020 2020 2020 2020 6966 2069 203d            if i =
+00001570: 3d20 7365 6c66 2e73 656c 6563 7465 643a  = self.selected:
+00001580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001590: 2020 6f70 7469 6f6e 5f63 6f6c 6f72 203d    option_color =
+000015a0: 2028 3530 2c20 3232 302c 2038 3029 0d0a   (50, 220, 80)..
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 6f70 7469 6f6e 5f69 6e64 6963 6174 6f72  option_indicator
+000015d0: 203d 2043 5374 7228 223e 2022 2c20 666f   = CStr("> ", fo
+000015e0: 7265 636f 6c6f 723d 2832 3230 2c20 3232  recolor=(220, 22
+000015f0: 302c 2032 3230 2929 0d0a 2020 2020 2020  0, 220))..      
+00001600: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00001610: 2020 2020 2020 2020 2020 2020 206f 7074               opt
+00001620: 696f 6e5f 636f 6c6f 7220 3d20 2832 3230  ion_color = (220
+00001630: 2c20 3232 302c 2032 3230 290d 0a20 2020  , 220, 220)..   
+00001640: 2020 2020 2020 2020 2020 2020 206f 7074               opt
+00001650: 696f 6e5f 696e 6469 6361 746f 7220 3d20  ion_indicator = 
+00001660: 4353 7472 2822 2020 222c 2066 6f72 6563  CStr("  ", forec
+00001670: 6f6c 6f72 3d28 3232 302c 2032 3230 2c20  olor=(220, 220, 
+00001680: 3232 3029 290d 0a20 2020 2020 2020 2020  220))..         
+00001690: 2020 205f 5f6f 7074 696f 6e20 3d20 4353     __option = CS
+000016a0: 7472 286f 7074 696f 6e2c 2066 6f72 6563  tr(option, forec
+000016b0: 6f6c 6f72 3d6f 7074 696f 6e5f 636f 6c6f  olor=option_colo
+000016c0: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
+000016d0: 7365 6c66 2e64 7261 7765 722e 706c 6163  self.drawer.plac
+000016e0: 6528 6f70 7469 6f6e 5f69 6e64 6963 6174  e(option_indicat
+000016f0: 6f72 202b 205f 5f6f 7074 696f 6e2c 0d0a  or + __option,..
 00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 2020 2020 2020 2020 2070 6f73 3d28             pos=(
-00001720: 6361 7074 696f 6e5f 7374 6172 742c 2031  caption_start, 1
-00001730: 202b 2069 2929 0d0a 0d0a 0d0a 636c 6173   + i))......clas
-00001740: 7320 5769 6467 6574 496e 7075 7428 5769  s WidgetInput(Wi
-00001750: 6467 6574 293a 0d0a 2020 2020 6465 6620  dget):..    def 
-00001760: 5f5f 696e 6974 5f5f 2873 656c 662c 0d0a  __init__(self,..
-00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001780: 2074 6578 743a 2073 7472 2c0d 0a20 2020   text: str,..   
-00001790: 2020 2020 2020 2020 2020 2020 2020 7369                si
-000017a0: 7a65 3a20 5369 7a65 203d 204e 6f6e 652c  ze: Size = None,
-000017b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000017c0: 2020 2070 6f73 3a20 506f 696e 7420 3d20     pos: Point = 
-000017d0: 506f 696e 7428 302c 2030 292c 0d0a 2020  Point(0, 0),..  
-000017e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000017f0: 6c6c 6f77 6564 5f63 6861 7261 6374 6572  llowed_character
-00001800: 733a 2073 7472 203d 2022 2061 6263 6465  s: str = " abcde
-00001810: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
-00001820: 7677 7879 7a30 3132 3334 3536 3738 395f  vwxyz0123456789_
-00001830: 2d2b 2f5c 5c28 295b 5d2e 222c 0d0a 2020  -+/\\()[].",..  
-00001840: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-00001850: 2a6b 7761 7267 730d 0a20 2020 2020 2020  *kwargs..       
-00001860: 2020 2020 2020 2020 2020 293a 0d0a 2020            ):..  
-00001870: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-00001880: 696e 6974 5f5f 2873 697a 652c 2070 6f73  init__(size, pos
-00001890: 2c20 2a2a 6b77 6172 6773 290d 0a20 2020  , **kwargs)..   
-000018a0: 2020 2020 2023 2070 203d 2031 0d0a 2020       # p = 1..  
-000018b0: 2020 2020 2020 7365 6c66 2e73 697a 652e        self.size.
-000018c0: 6820 3d20 310d 0a20 2020 2020 2020 2073  h = 1..        s
-000018d0: 656c 662e 7465 7874 203d 2074 6578 740d  elf.text = text.
-000018e0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-000018f0: 6967 6874 203d 2031 0d0a 2020 2020 2020  ight = 1..      
-00001900: 2020 7365 6c66 2e69 6e70 7574 203d 2022    self.input = "
-00001910: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00001920: 706f 696e 7465 7220 3d20 300d 0a20 2020  pointer = 0..   
-00001930: 2020 2020 2073 656c 662e 7669 6577 203d       self.view =
-00001940: 2030 0d0a 2020 2020 2020 2020 7365 6c66   0..        self
-00001950: 2e73 686f 775f 706f 696e 7465 7220 3d20  .show_pointer = 
-00001960: 4661 6c73 650d 0a20 2020 2020 2020 2023  False..        #
-00001970: 2063 6861 7261 6374 6572 7320 7468 6174   characters that
-00001980: 2074 6869 7320 6469 616c 6f75 6765 2077   this dialouge w
-00001990: 696c 6c20 6c69 7374 656e 2074 6f0d 0a20  ill listen to.. 
-000019a0: 2020 2020 2020 2073 656c 662e 616c 6c6f         self.allo
-000019b0: 7765 645f 6368 6172 6163 7465 7273 203d  wed_characters =
-000019c0: 2061 6c6c 6f77 6564 5f63 6861 7261 6374   allowed_charact
-000019d0: 6572 730d 0a20 2020 2020 2020 2073 656c  ers..        sel
-000019e0: 662e 7469 636b 203d 2030 0d0a 0d0a 2020  f.tick = 0....  
-000019f0: 2020 6465 6620 7275 6e5f 6361 6c6c 6261    def run_callba
-00001a00: 636b 7328 7365 6c66 293a 0d0a 2020 2020  cks(self):..    
-00001a10: 2020 2020 7375 7065 7228 292e 7275 6e5f      super().run_
-00001a20: 6361 6c6c 6261 636b 7328 290d 0a20 2020  callbacks()..   
-00001a30: 2020 2020 2073 656c 662e 7061 7265 6e74       self.parent
-00001a40: 2e63 6c6f 7365 2829 0d0a 2020 2020 2020  .close()..      
-00001a50: 2020 7365 6c66 2e72 6573 756c 7420 3d20    self.result = 
-00001a60: 7365 6c66 2e69 6e70 7574 0d0a 2020 2020  self.input..    
-00001a70: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00001a80: 7265 7375 6c74 0d0a 0d0a 2020 2020 6465  result....    de
-00001a90: 6620 7265 7365 7428 7365 6c66 293a 0d0a  f reset(self):..
-00001aa0: 2020 2020 2020 2020 7365 6c66 2e69 6e70          self.inp
-00001ab0: 7574 203d 2022 220d 0a20 2020 2020 2020  ut = ""..       
-00001ac0: 2073 656c 662e 706f 696e 7465 7220 3d20   self.pointer = 
-00001ad0: 300d 0a20 2020 2020 2020 2073 656c 662e  0..        self.
-00001ae0: 7669 6577 203d 2030 0d0a 0d0a 2020 2020  view = 0....    
-00001af0: 6465 6620 6765 745f 6d61 785f 6c65 6e67  def get_max_leng
-00001b00: 7468 2873 656c 6629 3a0d 0a20 2020 2020  th(self):..     
-00001b10: 2020 2070 203d 2032 0d0a 2020 2020 2020     p = 2..      
-00001b20: 2020 6d61 785f 696e 7075 745f 6c65 6e20    max_input_len 
-00001b30: 3d20 7365 6c66 2e73 697a 652e 6765 7457  = self.size.getW
-00001b40: 6964 7468 2829 2d28 7020 2a20 3229 2d6c  idth()-(p * 2)-l
-00001b50: 656e 2873 656c 662e 7465 7874 290d 0a20  en(self.text).. 
-00001b60: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
-00001b70: 785f 696e 7075 745f 6c65 6e0d 0a0d 0a20  x_input_len.... 
-00001b80: 2020 2064 6566 2075 7064 6174 6528 7365     def update(se
-00001b90: 6c66 2c20 6b65 7929 3a0d 0a20 2020 2020  lf, key):..     
-00001ba0: 2020 206b 6579 203d 2073 7570 6572 2829     key = super()
-00001bb0: 2e75 7064 6174 6528 6b65 7929 0d0a 2020  .update(key)..  
-00001bc0: 2020 2020 2020 6966 206b 6579 2069 7320        if key is 
-00001bd0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00001be0: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
-00001bf0: 2020 206d 6178 5f69 6e70 7574 5f6c 656e     max_input_len
-00001c00: 203d 2073 656c 662e 6765 745f 6d61 785f   = self.get_max_
-00001c10: 6c65 6e67 7468 2829 0d0a 2020 2020 2020  length()..      
-00001c20: 2020 2320 6361 7074 7572 6520 616e 6420    # capture and 
-00001c30: 706c 6163 6520 6368 6172 6163 7465 7273  place characters
-00001c40: 0d0a 2020 2020 2020 2020 6966 206b 6579  ..        if key
-00001c50: 2e6c 6f77 6572 2829 2069 6e20 7365 6c66  .lower() in self
-00001c60: 2e61 6c6c 6f77 6564 5f63 6861 7261 6374  .allowed_charact
-00001c70: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
-00001c80: 2020 7365 6c66 2e69 6e70 7574 203d 2073    self.input = s
-00001c90: 656c 662e 696e 7075 745b 3a73 656c 662e  elf.input[:self.
-00001ca0: 706f 696e 7465 725d 202b 205c 0d0a 2020  pointer] + \..  
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 6b65                ke
-00001cc0: 7920 2b20 7365 6c66 2e69 6e70 7574 5b73  y + self.input[s
-00001cd0: 656c 662e 706f 696e 7465 723a 5d0d 0a20  elf.pointer:].. 
-00001ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001cf0: 706f 696e 7465 7220 2b3d 2031 0d0a 2020  pointer += 1..  
-00001d00: 2020 2020 2020 2020 2020 6966 2028 6c65            if (le
-00001d10: 6e28 7365 6c66 2e69 6e70 7574 292d 7365  n(self.input)-se
-00001d20: 6c66 2e76 6965 7729 203e 2028 6d61 785f  lf.view) > (max_
-00001d30: 696e 7075 745f 6c65 6e2d 3129 3a0d 0a20  input_len-1):.. 
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001d50: 656c 662e 7669 6577 202b 3d20 310d 0a20  elf.view += 1.. 
-00001d60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001d70: 6e0d 0a0d 0a20 2020 2020 2020 2023 2062  n....        # b
-00001d80: 6163 6b73 7061 6365 0d0a 2020 2020 2020  ackspace..      
-00001d90: 2020 6966 206b 6579 203d 3d20 4b65 792e    if key == Key.
-00001da0: 4241 434b 5350 4143 453a 0d0a 2020 2020  BACKSPACE:..    
-00001db0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00001dc0: 706f 696e 7465 7220 213d 2030 3a0d 0a20  pointer != 0:.. 
-00001dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001de0: 656c 662e 696e 7075 7420 3d20 7365 6c66  elf.input = self
-00001df0: 2e69 6e70 7574 5b3a 7365 6c66 2e70 6f69  .input[:self.poi
-00001e00: 6e74 6572 202d 0d0a 2020 2020 2020 2020  nter -..        
-00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e30: 315d 202b 2073 656c 662e 696e 7075 745b  1] + self.input[
-00001e40: 7365 6c66 2e70 6f69 6e74 6572 3a5d 0d0a  self.pointer:]..
-00001e50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00001e60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001e70: 2020 2073 656c 662e 696e 7075 7420 3d20     self.input = 
-00001e80: 7365 6c66 2e69 6e70 7574 5b73 656c 662e  self.input[self.
-00001e90: 706f 696e 7465 723a 5d0d 0a20 2020 2020  pointer:]..     
-00001ea0: 2020 2020 2020 2073 656c 662e 706f 696e         self.poin
-00001eb0: 7465 7220 3d20 6d61 7828 7365 6c66 2e70  ter = max(self.p
-00001ec0: 6f69 6e74 6572 202d 2031 2c20 3029 0d0a  ointer - 1, 0)..
-00001ed0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00001ee0: 656c 662e 706f 696e 7465 722d 7365 6c66  elf.pointer-self
-00001ef0: 2e76 6965 7720 3c20 303a 0d0a 2020 2020  .view < 0:..    
-00001f00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001f10: 2e76 6965 7720 3d20 6d61 7828 7365 6c66  .view = max(self
-00001f20: 2e76 6965 7720 2d20 6d61 785f 696e 7075  .view - max_inpu
-00001f30: 745f 6c65 6e2c 2030 290d 0a20 2020 2020  t_len, 0)..     
-00001f40: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-00001f50: 0a20 2020 2020 2020 2023 2064 656c 6574  .        # delet
-00001f60: 650d 0a20 2020 2020 2020 2069 6620 6b65  e..        if ke
-00001f70: 7920 3d3d 204b 6579 2e44 454c 4554 453a  y == Key.DELETE:
-00001f80: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001f90: 6c66 2e69 6e70 7574 203d 2073 656c 662e  lf.input = self.
-00001fa0: 696e 7075 745b 3a73 656c 662e 706f 696e  input[:self.poin
-00001fb0: 7465 725d 202b 205c 0d0a 2020 2020 2020  ter] + \..      
-00001fc0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-00001fd0: 6e70 7574 5b73 656c 662e 706f 696e 7465  nput[self.pointe
-00001fe0: 722b 313a 5d0d 0a20 2020 2020 2020 2020  r+1:]..         
-00001ff0: 2020 2023 2073 656c 662e 706f 696e 7465     # self.pointe
-00002000: 7220 3d20 6d61 7828 7365 6c66 2e70 6f69  r = max(self.poi
-00002010: 6e74 6572 202d 2031 2c20 3029 0d0a 2020  nter - 1, 0)..  
-00002020: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002030: 0d0a 0d0a 2020 2020 2020 2020 2320 6c65  ....        # le
-00002040: 6674 2061 7272 6f77 0d0a 2020 2020 2020  ft arrow..      
-00002050: 2020 6966 206b 6579 203d 3d20 4b65 792e    if key == Key.
-00002060: 4c45 4654 3a0d 0a20 2020 2020 2020 2020  LEFT:..         
-00002070: 2020 2073 656c 662e 706f 696e 7465 7220     self.pointer 
-00002080: 3d20 6d61 7828 7365 6c66 2e70 6f69 6e74  = max(self.point
-00002090: 6572 202d 2031 2c20 3029 0d0a 2020 2020  er - 1, 0)..    
-000020a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000020b0: 706f 696e 7465 722d 7365 6c66 2e76 6965  pointer-self.vie
-000020c0: 7720 3c20 303a 0d0a 2020 2020 2020 2020  w < 0:..        
-000020d0: 2020 2020 2020 2020 7365 6c66 2e76 6965          self.vie
-000020e0: 7720 3d20 6d61 7828 7365 6c66 2e76 6965  w = max(self.vie
-000020f0: 7720 2d20 312c 2030 290d 0a20 2020 2020  w - 1, 0)..     
-00002100: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-00002110: 0a20 2020 2020 2020 2023 2072 6967 6874  .        # right
-00002120: 2061 7272 6f77 0d0a 2020 2020 2020 2020   arrow..        
-00002130: 6966 206b 6579 203d 3d20 4b65 792e 5249  if key == Key.RI
-00002140: 4748 543a 0d0a 2020 2020 2020 2020 2020  GHT:..          
-00002150: 2020 7365 6c66 2e70 6f69 6e74 6572 203d    self.pointer =
-00002160: 206d 696e 2873 656c 662e 706f 696e 7465   min(self.pointe
-00002170: 7220 2b20 312c 206c 656e 2873 656c 662e  r + 1, len(self.
-00002180: 696e 7075 7429 290d 0a20 2020 2020 2020  input))..       
-00002190: 2020 2020 2069 6620 7365 6c66 2e76 6965       if self.vie
-000021a0: 7720 3d3d 2028 7365 6c66 2e70 6f69 6e74  w == (self.point
-000021b0: 6572 2d6d 6178 5f69 6e70 7574 5f6c 656e  er-max_input_len
-000021c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000021d0: 2020 2020 7365 6c66 2e76 6965 7720 3d20      self.view = 
-000021e0: 6d69 6e28 7365 6c66 2e76 6965 7720 2b20  min(self.view + 
-000021f0: 312c 206c 656e 2873 656c 662e 696e 7075  1, len(self.inpu
-00002200: 7429 290d 0a20 2020 2020 2020 2020 2020  t))..           
-00002210: 2072 6574 7572 6e0d 0a0d 0a20 2020 2020   return....     
-00002220: 2020 2069 6620 6b65 7920 3d3d 2022 5550     if key == "UP
-00002230: 4441 5445 223a 0d0a 2020 2020 2020 2020  DATE":..        
-00002240: 2020 2020 7365 6c66 2e74 6963 6b20 2b3d      self.tick +=
-00002250: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00002260: 7365 6c66 2e73 686f 775f 706f 696e 7465  self.show_pointe
-00002270: 7220 3d20 2873 656c 662e 7469 636b 2025  r = (self.tick %
-00002280: 2031 3229 203e 3d20 360d 0a20 2020 2020   12) >= 6..     
-00002290: 2020 2072 6574 7572 6e20 6b65 790d 0a0d     return key...
-000022a0: 0a20 2020 2064 6566 2066 6f72 6d61 745f  .    def format_
-000022b0: 7465 7874 626f 7828 7365 6c66 293a 0d0a  textbox(self):..
-000022c0: 2020 2020 2020 2020 7465 7874 2c20 696e          text, in
-000022d0: 702c 2070 6f69 6e74 6572 2c20 7669 6577  p, pointer, view
-000022e0: 203d 2073 656c 662e 7465 7874 2c20 7365   = self.text, se
-000022f0: 6c66 2e69 6e70 7574 2c20 7365 6c66 2e70  lf.input, self.p
-00002300: 6f69 6e74 6572 2c20 7365 6c66 2e76 6965  ointer, self.vie
-00002310: 770d 0a20 2020 2020 2020 206d 6178 5f69  w..        max_i
-00002320: 6e70 7574 5f6c 656e 203d 2073 656c 662e  nput_len = self.
-00002330: 6765 745f 6d61 785f 6c65 6e67 7468 2829  get_max_length()
-00002340: 0d0a 2020 2020 2020 2020 2320 6765 7420  ..        # get 
-00002350: 7468 6520 696e 7075 7420 7465 7874 2077  the input text w
-00002360: 6974 6820 6669 7865 6420 6c65 6e67 7468  ith fixed length
-00002370: 2070 6c75 7320 6f6e 6520 6578 7472 6120   plus one extra 
-00002380: 7370 6163 6520 666f 7220 7468 6520 706f  space for the po
-00002390: 696e 7465 720d 0a20 2020 2020 2020 2069  inter..        i
-000023a0: 6620 7669 6577 2b6d 6178 5f69 6e70 7574  f view+max_input
-000023b0: 5f6c 656e 2d31 203c 206c 656e 2869 6e70  _len-1 < len(inp
-000023c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000023d0: 696e 705f 203d 2069 6e70 5b76 6965 773a  inp_ = inp[view:
-000023e0: 7669 6577 2b6d 6178 5f69 6e70 7574 5f6c  view+max_input_l
-000023f0: 656e 5d0d 0a20 2020 2020 2020 2065 6c73  en]..        els
-00002400: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002410: 696e 705f 203d 2069 6e70 5b76 6965 773a  inp_ = inp[view:
-00002420: 7669 6577 2b6d 6178 5f69 6e70 7574 5f6c  view+max_input_l
-00002430: 656e 2d31 5d20 2b20 2220 220d 0a0d 0a20  en-1] + " ".... 
-00002440: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00002450: 6c66 2e69 735f 6469 7361 626c 6564 2061  lf.is_disabled a
-00002460: 6e64 2073 656c 662e 7368 6f77 5f70 6f69  nd self.show_poi
-00002470: 6e74 6572 206f 7220 696e 705f 5b70 6f69  nter or inp_[poi
-00002480: 6e74 6572 2d76 6965 775d 2021 3d20 2220  nter-view] != " 
-00002490: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-000024a0: 706f 696e 7465 725f 7374 7220 3d20 4353  pointer_str = CS
-000024b0: 7472 280d 0a20 2020 2020 2020 2020 2020  tr(..           
-000024c0: 2020 2020 2069 6e70 5f5b 706f 696e 7465       inp_[pointe
-000024d0: 722d 7669 6577 5d2c 2062 6163 6b63 6f6c  r-view], backcol
-000024e0: 6f72 3d28 3232 302c 2032 3230 2c20 3232  or=(220, 220, 22
-000024f0: 3029 2c20 666f 7265 636f 6c6f 723d 2832  0), forecolor=(2
-00002500: 302c 2032 302c 2032 3029 290d 0a20 2020  0, 20, 20))..   
-00002510: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00002520: 2020 2020 2020 2020 706f 696e 7465 725f          pointer_
-00002530: 7374 7220 3d20 4353 7472 2869 6e70 5f5b  str = CStr(inp_[
-00002540: 706f 696e 7465 722d 7669 6577 5d29 0d0a  pointer-view])..
-00002550: 2020 2020 2020 2020 2320 696e 7365 7274          # insert
-00002560: 2074 6865 2070 6f69 6e74 6572 2069 6e74   the pointer int
-00002570: 6f20 696e 7075 7420 7465 7874 2061 7420  o input text at 
-00002580: 7468 6520 636f 7272 6563 7420 706f 7369  the correct posi
-00002590: 7469 6f6e 0d0a 2020 2020 2020 2020 696e  tion..        in
-000025a0: 7075 745f 706c 7573 5f70 6f69 6e74 6572  put_plus_pointer
-000025b0: 203d 2043 5374 7228 0d0a 2020 2020 2020   = CStr(..      
-000025c0: 2020 2020 2020 696e 705f 5b3a 706f 696e        inp_[:poin
-000025d0: 7465 722d 7669 6577 5d29 202b 2070 6f69  ter-view]) + poi
-000025e0: 6e74 6572 5f73 7472 202b 2043 5374 7228  nter_str + CStr(
-000025f0: 696e 705f 5b70 6f69 6e74 6572 2d76 6965  inp_[pointer-vie
-00002600: 772b 313a 5d29 0d0a 0d0a 2020 2020 2020  w+1:])....      
-00002610: 2020 7465 7874 5f63 203d 2028 3530 2c20    text_c = (50, 
-00002620: 3230 302c 2035 3029 0d0a 0d0a 2020 2020  200, 50)....    
-00002630: 2020 2020 6673 7472 203d 2043 5374 7228      fstr = CStr(
-00002640: 7465 7874 2c20 666f 7265 636f 6c6f 723d  text, forecolor=
-00002650: 7465 7874 5f63 290d 0a0d 0a20 2020 2020  text_c)....     
-00002660: 2020 2062 6163 6b5f 6578 6973 7473 203d     back_exists =
-00002670: 2043 5374 7228 223c 222c 2066 6f72 6563   CStr("<", forec
-00002680: 6f6c 6f72 3d74 6578 745f 6329 0d0a 2020  olor=text_c)..  
-00002690: 2020 2020 2020 666f 7277 6172 645f 6578        forward_ex
-000026a0: 6973 7473 203d 2043 5374 7228 223e 222c  ists = CStr(">",
-000026b0: 2066 6f72 6563 6f6c 6f72 3d74 6578 745f   forecolor=text_
-000026c0: 6329 0d0a 0d0a 2020 2020 2020 2020 6673  c)....        fs
-000026d0: 7472 202b 3d20 2862 6163 6b5f 6578 6973  tr += (back_exis
-000026e0: 7473 2069 6620 7669 6577 2021 3d20 3020  ts if view != 0 
-000026f0: 656c 7365 2022 2022 290d 0a20 2020 2020  else " ")..     
-00002700: 2020 2066 7374 7220 2b3d 2069 6e70 7574     fstr += input
-00002710: 5f70 6c75 735f 706f 696e 7465 7220 2b20  _plus_pointer + 
-00002720: 2220 2220 2a20 5c0d 0a20 2020 2020 2020  " " * \..       
-00002730: 2020 2020 2028 6d61 785f 696e 7075 745f       (max_input_
-00002740: 6c65 6e20 2d20 6c65 6e28 696e 7075 745f  len - len(input_
-00002750: 706c 7573 5f70 6f69 6e74 6572 2929 0d0a  plus_pointer))..
-00002760: 2020 2020 2020 2020 6673 7472 202b 3d20          fstr += 
-00002770: 2866 6f72 7761 7264 5f65 7869 7374 7320  (forward_exists 
-00002780: 6966 2076 6965 772b 6d61 785f 696e 7075  if view+max_inpu
-00002790: 745f 6c65 6e2d 3120 3c20 6c65 6e28 696e  t_len-1 < len(in
-000027a0: 7029 2065 6c73 6520 2220 2229 0d0a 0d0a  p) else " ")....
-000027b0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-000027c0: 7374 720d 0a0d 0a20 2020 2064 6566 2072  str....    def r
-000027d0: 656e 6465 7228 7365 6c66 293a 0d0a 2020  ender(self):..  
-000027e0: 2020 2020 2020 7020 3d20 310d 0a20 2020        p = 1..   
-000027f0: 2020 2020 2069 6620 7365 6c66 2e70 6172       if self.par
-00002800: 656e 742e 6261 636b 6772 6f75 6e64 5f63  ent.background_c
-00002810: 6f6c 6f72 2069 7320 6e6f 7420 4e6f 6e65  olor is not None
-00002820: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
-00002830: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-00002840: 745f 7368 6164 6f77 203d 2074 7570 6c65  t_shadow = tuple
-00002850: 286d 6170 286c 616d 6264 6120 783a 2078  (map(lambda x: x
-00002860: 202a 2030 2e38 2c20 6c69 7374 2873 656c   * 0.8, list(sel
-00002870: 662e 7061 7265 6e74 2e62 6163 6b67 726f  f.parent.backgro
-00002880: 756e 645f 636f 6c6f 7229 2929 0d0a 2020  und_color)))..  
-00002890: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000028a0: 7261 7765 722e 706c 6163 6528 4353 7472  rawer.place(CStr
-000028b0: 2822 2022 202a 2028 7365 6c66 2e73 697a  (" " * (self.siz
-000028c0: 652e 6765 7457 6964 7468 2829 202d 2028  e.getWidth() - (
-000028d0: 7020 2a20 3229 202d 206c 656e 2873 656c  p * 2) - len(sel
-000028e0: 662e 7465 7874 2929 2c20 6261 636b 636f  f.text)), backco
-000028f0: 6c6f 723d 7465 7874 5f73 6861 646f 7729  lor=text_shadow)
-00002900: 2c20 706f 733d 2870 202b 206c 656e 2873  , pos=(p + len(s
-00002910: 656c 662e 7465 7874 292c 2030 2929 0d0a  elf.text), 0))..
-00002920: 2020 2020 2020 2020 7365 6c66 2e64 7261          self.dra
-00002930: 7765 722e 706c 6163 6528 7365 6c66 2e66  wer.place(self.f
-00002940: 6f72 6d61 745f 7465 7874 626f 7828 292c  ormat_textbox(),
-00002950: 2070 6f73 3d28 702c 2030 2929 0d0a 2020   pos=(p, 0))..  
-00002960: 2020 2020 2020 2373 656c 662e 6472 6177        #self.draw
-00002970: 6572 2e77 7269 7465 5f74 6578 7428 7374  er.write_text(st
-00002980: 7228 7465 7874 5f73 6861 646f 7729 2c20  r(text_shadow), 
-00002990: 706f 733d 2830 2c20 3029 290d 0a         pos=(0, 0))..
+00001710: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00001720: 733d 2863 6170 7469 6f6e 5f73 7461 7274  s=(caption_start
+00001730: 2c20 3120 2b20 6929 290d 0a0d 0a0d 0a63  , 1 + i))......c
+00001740: 6c61 7373 2057 6964 6765 7449 6e70 7574  lass WidgetInput
+00001750: 2857 6964 6765 7429 3a0d 0a20 2020 2064  (Widget):..    d
+00001760: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00001770: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001780: 2020 2020 7465 7874 3a20 7374 722c 0d0a      text: str,..
+00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017a0: 2073 697a 653a 2053 697a 6520 3d20 4e6f   size: Size = No
+000017b0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+000017c0: 2020 2020 2020 706f 733a 2050 6f69 6e74        pos: Point
+000017d0: 203d 2050 6f69 6e74 2830 2c20 3029 2c0d   = Point(0, 0),.
+000017e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000017f0: 2020 2a2a 6b77 6172 6773 0d0a 2020 2020    **kwargs..    
+00001800: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
+00001810: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00001820: 2e5f 5f69 6e69 745f 5f28 7369 7a65 2c20  .__init__(size, 
+00001830: 706f 732c 202a 2a6b 7761 7267 7329 0d0a  pos, **kwargs)..
+00001840: 2020 2020 2020 2020 2320 7020 3d20 310d          # p = 1.
+00001850: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
+00001860: 7a65 2e68 203d 2031 0d0a 2020 2020 2020  ze.h = 1..      
+00001870: 2020 7365 6c66 2e74 6578 7420 3d20 7465    self.text = te
+00001880: 7874 0d0a 2020 2020 2020 2020 7365 6c66  xt..        self
+00001890: 2e68 6569 6768 7420 3d20 310d 0a20 2020  .height = 1..   
+000018a0: 2020 2020 2073 656c 662e 696e 7075 7420       self.input 
+000018b0: 3d20 2222 0d0a 2020 2020 2020 2020 7365  = ""..        se
+000018c0: 6c66 2e70 6f69 6e74 6572 203d 2030 0d0a  lf.pointer = 0..
+000018d0: 2020 2020 2020 2020 7365 6c66 2e76 6965          self.vie
+000018e0: 7720 3d20 300d 0a20 2020 2020 2020 2073  w = 0..        s
+000018f0: 656c 662e 7368 6f77 5f70 6f69 6e74 6572  elf.show_pointer
+00001900: 203d 2046 616c 7365 0d0a 0d0a 2020 2020   = False....    
+00001910: 2020 2020 2320 6368 6172 6163 7465 7273      # characters
+00001920: 2074 6861 7420 7468 6973 2064 6961 6c6f   that this dialo
+00001930: 7567 6520 7769 6c6c 206c 6973 7465 6e20  uge will listen 
+00001940: 746f 0d0a 2020 2020 2020 2020 7365 6c66  to..        self
+00001950: 2e61 6c6c 6f77 6564 5f63 6861 7261 6374  .allowed_charact
+00001960: 6572 7320 3d20 6465 6661 756c 7428 6b77  ers = default(kw
+00001970: 6172 6773 2c20 2261 6c6c 6f77 6564 5f63  args, "allowed_c
+00001980: 6861 7273 222c 2022 2229 0d0a 2020 2020  hars", "")..    
+00001990: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+000019a0: 2323 206b 6579 730d 0a20 2020 2020 2020  ## keys..       
+000019b0: 2063 7472 6c5f 6b65 7973 203d 205b 0d0a   ctrl_keys = [..
+000019c0: 2020 2020 2020 2020 2020 2020 4b65 792e              Key.
+000019d0: 4354 524c 5f41 2c0d 0a20 2020 2020 2020  CTRL_A,..       
+000019e0: 2020 2020 204b 6579 2e43 5452 4c5f 422c       Key.CTRL_B,
+000019f0: 0d0a 2020 2020 2020 2020 2020 2020 4b65  ..            Ke
+00001a00: 792e 4354 524c 5f43 2c0d 0a20 2020 2020  y.CTRL_C,..     
+00001a10: 2020 2020 2020 204b 6579 2e43 5452 4c5f         Key.CTRL_
+00001a20: 442c 0d0a 2020 2020 2020 2020 2020 2020  D,..            
+00001a30: 4b65 792e 4354 524c 5f45 2c0d 0a20 2020  Key.CTRL_E,..   
+00001a40: 2020 2020 2020 2020 204b 6579 2e43 5452           Key.CTR
+00001a50: 4c5f 462c 0d0a 2020 2020 2020 2020 2020  L_F,..          
+00001a60: 2020 4b65 792e 4354 524c 5f47 2c0d 0a20    Key.CTRL_G,.. 
+00001a70: 2020 2020 2020 2020 2020 204b 6579 2e43             Key.C
+00001a80: 5452 4c5f 482c 0d0a 2020 2020 2020 2020  TRL_H,..        
+00001a90: 2020 2020 4b65 792e 4354 524c 5f49 2c0d      Key.CTRL_I,.
+00001aa0: 0a20 2020 2020 2020 2020 2020 204b 6579  .            Key
+00001ab0: 2e43 5452 4c5f 4a2c 0d0a 2020 2020 2020  .CTRL_J,..      
+00001ac0: 2020 2020 2020 4b65 792e 4354 524c 5f4b        Key.CTRL_K
+00001ad0: 2c0d 0a20 2020 2020 2020 2020 2020 204b  ,..            K
+00001ae0: 6579 2e43 5452 4c5f 4c2c 0d0a 2020 2020  ey.CTRL_L,..    
+00001af0: 2020 2020 2020 2020 4b65 792e 4354 524c          Key.CTRL
+00001b00: 5f4d 2c0d 0a20 2020 2020 2020 2020 2020  _M,..           
+00001b10: 204b 6579 2e43 5452 4c5f 4e2c 0d0a 2020   Key.CTRL_N,..  
+00001b20: 2020 2020 2020 2020 2020 4b65 792e 4354            Key.CT
+00001b30: 524c 5f4f 2c0d 0a20 2020 2020 2020 2020  RL_O,..         
+00001b40: 2020 204b 6579 2e43 5452 4c5f 502c 0d0a     Key.CTRL_P,..
+00001b50: 2020 2020 2020 2020 2020 2020 4b65 792e              Key.
+00001b60: 4354 524c 5f51 2c0d 0a20 2020 2020 2020  CTRL_Q,..       
+00001b70: 2020 2020 204b 6579 2e43 5452 4c5f 522c       Key.CTRL_R,
+00001b80: 0d0a 2020 2020 2020 2020 2020 2020 4b65  ..            Ke
+00001b90: 792e 4354 524c 5f53 2c0d 0a20 2020 2020  y.CTRL_S,..     
+00001ba0: 2020 2020 2020 204b 6579 2e43 5452 4c5f         Key.CTRL_
+00001bb0: 542c 0d0a 2020 2020 2020 2020 2020 2020  T,..            
+00001bc0: 4b65 792e 4354 524c 5f55 2c0d 0a20 2020  Key.CTRL_U,..   
+00001bd0: 2020 2020 2020 2020 204b 6579 2e43 5452           Key.CTR
+00001be0: 4c5f 562c 0d0a 2020 2020 2020 2020 2020  L_V,..          
+00001bf0: 2020 4b65 792e 4354 524c 5f57 2c0d 0a20    Key.CTRL_W,.. 
+00001c00: 2020 2020 2020 2020 2020 204b 6579 2e43             Key.C
+00001c10: 5452 4c5f 582c 0d0a 2020 2020 2020 2020  TRL_X,..        
+00001c20: 2020 2020 4b65 792e 4354 524c 5f59 2c0d      Key.CTRL_Y,.
+00001c30: 0a20 2020 2020 2020 2020 2020 204b 6579  .            Key
+00001c40: 2e43 5452 4c5f 5a2c 0d0a 2020 2020 2020  .CTRL_Z,..      
+00001c50: 2020 5d0d 0a20 2020 2020 2020 200d 0a20    ]..        .. 
+00001c60: 2020 2020 2020 2066 756e 6369 6f6e 5f6b         funcion_k
+00001c70: 6579 7320 3d20 5b0d 0a20 2020 2020 2020  eys = [..       
+00001c80: 2020 2020 204b 6579 2e46 312c 0d0a 2020       Key.F1,..  
+00001c90: 2020 2020 2020 2020 2020 4b65 792e 4632            Key.F2
+00001ca0: 2c0d 0a20 2020 2020 2020 2020 2020 204b  ,..            K
+00001cb0: 6579 2e46 332c 0d0a 2020 2020 2020 2020  ey.F3,..        
+00001cc0: 2020 2020 4b65 792e 4634 2c0d 0a20 2020      Key.F4,..   
+00001cd0: 2020 2020 2020 2020 204b 6579 2e46 352c           Key.F5,
+00001ce0: 0d0a 2020 2020 2020 2020 2020 2020 4b65  ..            Ke
+00001cf0: 792e 4636 2c0d 0a20 2020 2020 2020 2020  y.F6,..         
+00001d00: 2020 204b 6579 2e46 372c 0d0a 2020 2020     Key.F7,..    
+00001d10: 2020 2020 2020 2020 4b65 792e 4638 2c0d          Key.F8,.
+00001d20: 0a20 2020 2020 2020 2020 2020 204b 6579  .            Key
+00001d30: 2e46 392c 0d0a 2020 2020 2020 2020 2020  .F9,..          
+00001d40: 2020 4b65 792e 4631 302c 0d0a 2020 2020    Key.F10,..    
+00001d50: 2020 2020 2020 2020 4b65 792e 4631 312c          Key.F11,
+00001d60: 0d0a 2020 2020 2020 2020 2020 2020 4b65  ..            Ke
+00001d70: 792e 4631 322c 0d0a 2020 2020 2020 2020  y.F12,..        
+00001d80: 5d0d 0a20 2020 2020 2020 2069 676e 6f72  ]..        ignor
+00001d90: 6564 5f6b 6579 7320 3d20 5b0d 0a20 2020  ed_keys = [..   
+00001da0: 2020 2020 2020 2020 204b 6579 2e43 522c           Key.CR,
+00001db0: 0d0a 2020 2020 2020 2020 2020 2020 4b65  ..            Ke
+00001dc0: 792e 444f 574e 2c0d 0a20 2020 2020 2020  y.DOWN,..       
+00001dd0: 2020 2020 204b 6579 2e55 502c 0d0a 2020       Key.UP,..  
+00001de0: 2020 2020 2020 2020 2020 4b65 792e 4c45            Key.LE
+00001df0: 4654 2c0d 0a20 2020 2020 2020 2020 2020  FT,..           
+00001e00: 204b 6579 2e52 4947 4854 2c0d 0a20 2020   Key.RIGHT,..   
+00001e10: 2020 2020 2020 2020 204b 6579 2e45 4e44           Key.END
+00001e20: 2c0d 0a20 2020 2020 2020 2020 2020 204b  ,..            K
+00001e30: 6579 2e48 4f4d 452c 0d0a 2020 2020 2020  ey.HOME,..      
+00001e40: 2020 2020 2020 4b65 792e 4553 432c 0d0a        Key.ESC,..
+00001e50: 2020 2020 2020 2020 2020 2020 4b65 792e              Key.
+00001e60: 4553 435f 322c 0d0a 2020 2020 2020 2020  ESC_2,..        
+00001e70: 2020 2020 4b65 792e 454e 5445 522c 0d0a      Key.ENTER,..
+00001e80: 2020 2020 2020 2020 2020 2020 4b65 792e              Key.
+00001e90: 454e 5445 525f 322c 0d0a 2020 2020 2020  ENTER_2,..      
+00001ea0: 2020 2020 2020 4b65 792e 494e 5345 5254        Key.INSERT
+00001eb0: 2c0d 0a20 2020 2020 2020 2020 2020 204b  ,..            K
+00001ec0: 6579 2e4c 462c 0d0a 2020 2020 2020 2020  ey.LF,..        
+00001ed0: 2020 2020 4b65 792e 5041 4745 5f44 4f57      Key.PAGE_DOW
+00001ee0: 4e2c 200d 0a20 2020 2020 2020 2020 2020  N, ..           
+00001ef0: 204b 6579 2e50 4147 455f 5550 2c20 0d0a   Key.PAGE_UP, ..
+00001f00: 2020 2020 2020 2020 2020 2020 4b65 792e              Key.
+00001f10: 5355 5052 2c0d 0a20 2020 2020 2020 205d  SUPR,..        ]
+00001f20: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00001f30: 2e5f 5f69 676e 6f72 6564 5f6b 6579 7320  .__ignored_keys 
+00001f40: 3d20 6374 726c 5f6b 6579 7320 2b20 6675  = ctrl_keys + fu
+00001f50: 6e63 696f 6e5f 6b65 7973 202b 2069 676e  ncion_keys + ign
+00001f60: 6f72 6564 5f6b 6579 730d 0a0d 0a20 2020  ored_keys....   
+00001f70: 2064 6566 2072 756e 5f63 616c 6c62 6163   def run_callbac
+00001f80: 6b73 2873 656c 6629 3a0d 0a20 2020 2020  ks(self):..     
+00001f90: 2020 2073 7570 6572 2829 2e72 756e 5f63     super().run_c
+00001fa0: 616c 6c62 6163 6b73 2829 0d0a 2020 2020  allbacks()..    
+00001fb0: 2020 2020 7365 6c66 2e70 6172 656e 742e      self.parent.
+00001fc0: 636c 6f73 6528 290d 0a20 2020 2020 2020  close()..       
+00001fd0: 2073 656c 662e 7265 7375 6c74 203d 2073   self.result = s
+00001fe0: 656c 662e 696e 7075 740d 0a20 2020 2020  elf.input..     
+00001ff0: 2020 2072 6574 7572 6e20 7365 6c66 2e72     return self.r
+00002000: 6573 756c 740d 0a0d 0a20 2020 2064 6566  esult....    def
+00002010: 2072 6573 6574 2873 656c 6629 3a0d 0a20   reset(self):.. 
+00002020: 2020 2020 2020 2073 656c 662e 696e 7075         self.inpu
+00002030: 7420 3d20 2222 0d0a 2020 2020 2020 2020  t = ""..        
+00002040: 7365 6c66 2e70 6f69 6e74 6572 203d 2030  self.pointer = 0
+00002050: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
+00002060: 6965 7720 3d20 300d 0a0d 0a20 2020 2064  iew = 0....    d
+00002070: 6566 2067 6574 5f6d 6178 5f6c 656e 6774  ef get_max_lengt
+00002080: 6828 7365 6c66 293a 0d0a 2020 2020 2020  h(self):..      
+00002090: 2020 7020 3d20 320d 0a20 2020 2020 2020    p = 2..       
+000020a0: 206d 6178 5f69 6e70 7574 5f6c 656e 203d   max_input_len =
+000020b0: 2073 656c 662e 7369 7a65 2e67 6574 5769   self.size.getWi
+000020c0: 6474 6828 292d 2870 202a 2032 292d 6c65  dth()-(p * 2)-le
+000020d0: 6e28 7365 6c66 2e74 6578 7429 0d0a 2020  n(self.text)..  
+000020e0: 2020 2020 2020 7265 7475 726e 206d 6178        return max
+000020f0: 5f69 6e70 7574 5f6c 656e 0d0a 0d0a 2020  _input_len....  
+00002100: 2020 6465 6620 7570 6461 7465 2873 656c    def update(sel
+00002110: 662c 206b 6579 293a 0d0a 2020 2020 2020  f, key):..      
+00002120: 2020 6b65 7920 3d20 7375 7065 7228 292e    key = super().
+00002130: 7570 6461 7465 286b 6579 290d 0a20 2020  update(key)..   
+00002140: 2020 2020 2069 6620 6b65 7920 6973 204e       if key is N
+00002150: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00002160: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
+00002170: 2020 2020 6d61 785f 696e 7075 745f 6c65      max_input_le
+00002180: 6e20 3d20 7365 6c66 2e67 6574 5f6d 6178  n = self.get_max
+00002190: 5f6c 656e 6774 6828 290d 0a20 2020 2020  _length()..     
+000021a0: 2020 2023 2063 6170 7475 7265 2061 6e64     # capture and
+000021b0: 2070 6c61 6365 2063 6861 7261 6374 6572   place character
+000021c0: 730d 0a20 2020 2020 2020 2069 6620 6b65  s..        if ke
+000021d0: 7920 213d 2022 5550 4441 5445 2220 616e  y != "UPDATE" an
+000021e0: 6420 6b65 7920 6e6f 7420 696e 2073 656c  d key not in sel
+000021f0: 662e 5f5f 6967 6e6f 7265 645f 6b65 7973  f.__ignored_keys
+00002200: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00002210: 656c 662e 696e 7075 7420 3d20 7365 6c66  elf.input = self
+00002220: 2e69 6e70 7574 5b3a 7365 6c66 2e70 6f69  .input[:self.poi
+00002230: 6e74 6572 5d20 2b20 5c0d 0a20 2020 2020  nter] + \..     
+00002240: 2020 2020 2020 2020 2020 206b 6579 202b             key +
+00002250: 2073 656c 662e 696e 7075 745b 7365 6c66   self.input[self
+00002260: 2e70 6f69 6e74 6572 3a5d 0d0a 2020 2020  .pointer:]..    
+00002270: 2020 2020 2020 2020 7365 6c66 2e70 6f69          self.poi
+00002280: 6e74 6572 202b 3d20 310d 0a20 2020 2020  nter += 1..     
+00002290: 2020 2020 2020 2069 6620 286c 656e 2873         if (len(s
+000022a0: 656c 662e 696e 7075 7429 2d73 656c 662e  elf.input)-self.
+000022b0: 7669 6577 2920 3e20 286d 6178 5f69 6e70  view) > (max_inp
+000022c0: 7574 5f6c 656e 2d31 293a 0d0a 2020 2020  ut_len-1):..    
+000022d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000022e0: 2e76 6965 7720 2b3d 2031 0d0a 2020 2020  .view += 1..    
+000022f0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00002300: 0d0a 2020 2020 2020 2020 2320 6261 636b  ..        # back
+00002310: 7370 6163 650d 0a20 2020 2020 2020 2069  space..        i
+00002320: 6620 6b65 7920 3d3d 204b 6579 2e42 4143  f key == Key.BAC
+00002330: 4b53 5041 4345 3a0d 0a20 2020 2020 2020  KSPACE:..       
+00002340: 2020 2020 2069 6620 7365 6c66 2e70 6f69       if self.poi
+00002350: 6e74 6572 2021 3d20 303a 0d0a 2020 2020  nter != 0:..    
+00002360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002370: 2e69 6e70 7574 203d 2073 656c 662e 696e  .input = self.in
+00002380: 7075 745b 3a73 656c 662e 706f 696e 7465  put[:self.pointe
+00002390: 7220 2d0d 0a20 2020 2020 2020 2020 2020  r -..           
+000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023b0: 2020 2020 2020 2020 2020 2020 2031 5d20               1] 
+000023c0: 2b20 7365 6c66 2e69 6e70 7574 5b73 656c  + self.input[sel
+000023d0: 662e 706f 696e 7465 723a 5d0d 0a20 2020  f.pointer:]..   
+000023e0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 7365 6c66 2e69 6e70 7574 203d 2073 656c  self.input = sel
+00002410: 662e 696e 7075 745b 7365 6c66 2e70 6f69  f.input[self.poi
+00002420: 6e74 6572 3a5d 0d0a 2020 2020 2020 2020  nter:]..        
+00002430: 2020 2020 7365 6c66 2e70 6f69 6e74 6572      self.pointer
+00002440: 203d 206d 6178 2873 656c 662e 706f 696e   = max(self.poin
+00002450: 7465 7220 2d20 312c 2030 290d 0a20 2020  ter - 1, 0)..   
+00002460: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00002470: 2e70 6f69 6e74 6572 2d73 656c 662e 7669  .pointer-self.vi
+00002480: 6577 203c 2030 3a0d 0a20 2020 2020 2020  ew < 0:..       
+00002490: 2020 2020 2020 2020 2073 656c 662e 7669           self.vi
+000024a0: 6577 203d 206d 6178 2873 656c 662e 7669  ew = max(self.vi
+000024b0: 6577 202d 206d 6178 5f69 6e70 7574 5f6c  ew - max_input_l
+000024c0: 656e 2c20 3029 0d0a 2020 2020 2020 2020  en, 0)..        
+000024d0: 2020 2020 7265 7475 726e 0d0a 0d0a 2020      return....  
+000024e0: 2020 2020 2020 2320 6465 6c65 7465 0d0a        # delete..
+000024f0: 2020 2020 2020 2020 6966 206b 6579 203d          if key =
+00002500: 3d20 4b65 792e 4445 4c45 5445 3a0d 0a20  = Key.DELETE:.. 
+00002510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002520: 696e 7075 7420 3d20 7365 6c66 2e69 6e70  input = self.inp
+00002530: 7574 5b3a 7365 6c66 2e70 6f69 6e74 6572  ut[:self.pointer
+00002540: 5d20 2b20 5c0d 0a20 2020 2020 2020 2020  ] + \..         
+00002550: 2020 2020 2020 2073 656c 662e 696e 7075         self.inpu
+00002560: 745b 7365 6c66 2e70 6f69 6e74 6572 2b31  t[self.pointer+1
+00002570: 3a5d 0d0a 2020 2020 2020 2020 2020 2020  :]..            
+00002580: 2320 7365 6c66 2e70 6f69 6e74 6572 203d  # self.pointer =
+00002590: 206d 6178 2873 656c 662e 706f 696e 7465   max(self.pointe
+000025a0: 7220 2d20 312c 2030 290d 0a20 2020 2020  r - 1, 0)..     
+000025b0: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+000025c0: 0a20 2020 2020 2020 2023 206c 6566 7420  .        # left 
+000025d0: 6172 726f 770d 0a20 2020 2020 2020 2069  arrow..        i
+000025e0: 6620 6b65 7920 3d3d 204b 6579 2e4c 4546  f key == Key.LEF
+000025f0: 543a 0d0a 2020 2020 2020 2020 2020 2020  T:..            
+00002600: 7365 6c66 2e70 6f69 6e74 6572 203d 206d  self.pointer = m
+00002610: 6178 2873 656c 662e 706f 696e 7465 7220  ax(self.pointer 
+00002620: 2d20 312c 2030 290d 0a20 2020 2020 2020  - 1, 0)..       
+00002630: 2020 2020 2069 6620 7365 6c66 2e70 6f69       if self.poi
+00002640: 6e74 6572 2d73 656c 662e 7669 6577 203c  nter-self.view <
+00002650: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00002660: 2020 2020 2073 656c 662e 7669 6577 203d       self.view =
+00002670: 206d 6178 2873 656c 662e 7669 6577 202d   max(self.view -
+00002680: 2031 2c20 3029 0d0a 2020 2020 2020 2020   1, 0)..        
+00002690: 2020 2020 7265 7475 726e 0d0a 0d0a 2020      return....  
+000026a0: 2020 2020 2020 2320 7269 6768 7420 6172        # right ar
+000026b0: 726f 770d 0a20 2020 2020 2020 2069 6620  row..        if 
+000026c0: 6b65 7920 3d3d 204b 6579 2e52 4947 4854  key == Key.RIGHT
+000026d0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000026e0: 656c 662e 706f 696e 7465 7220 3d20 6d69  elf.pointer = mi
+000026f0: 6e28 7365 6c66 2e70 6f69 6e74 6572 202b  n(self.pointer +
+00002700: 2031 2c20 6c65 6e28 7365 6c66 2e69 6e70   1, len(self.inp
+00002710: 7574 2929 0d0a 2020 2020 2020 2020 2020  ut))..          
+00002720: 2020 6966 2073 656c 662e 7669 6577 203d    if self.view =
+00002730: 3d20 2873 656c 662e 706f 696e 7465 722d  = (self.pointer-
+00002740: 6d61 785f 696e 7075 745f 6c65 6e29 3a0d  max_input_len):.
+00002750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002760: 2073 656c 662e 7669 6577 203d 206d 696e   self.view = min
+00002770: 2873 656c 662e 7669 6577 202b 2031 2c20  (self.view + 1, 
+00002780: 6c65 6e28 7365 6c66 2e69 6e70 7574 2929  len(self.input))
+00002790: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000027a0: 7475 726e 0d0a 0d0a 2020 2020 2020 2020  turn....        
+000027b0: 6966 206b 6579 203d 3d20 2255 5044 4154  if key == "UPDAT
+000027c0: 4522 3a0d 0a20 2020 2020 2020 2020 2020  E":..           
+000027d0: 2073 656c 662e 7368 6f77 5f70 6f69 6e74   self.show_point
+000027e0: 6572 203d 2028 7365 6c66 2e70 6172 656e  er = (self.paren
+000027f0: 742e 7469 636b 2025 2032 3029 203e 3d20  t.tick % 20) >= 
+00002800: 3132 0d0a 2020 2020 2020 2020 7265 7475  12..        retu
+00002810: 726e 206b 6579 0d0a 0d0a 2020 2020 6465  rn key....    de
+00002820: 6620 666f 726d 6174 5f74 6578 7462 6f78  f format_textbox
+00002830: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00002840: 2074 6578 742c 2069 6e70 2c20 706f 696e   text, inp, poin
+00002850: 7465 722c 2076 6965 7720 3d20 7365 6c66  ter, view = self
+00002860: 2e74 6578 742c 2073 656c 662e 696e 7075  .text, self.inpu
+00002870: 742c 2073 656c 662e 706f 696e 7465 722c  t, self.pointer,
+00002880: 2073 656c 662e 7669 6577 0d0a 2020 2020   self.view..    
+00002890: 2020 2020 6d61 785f 696e 7075 745f 6c65      max_input_le
+000028a0: 6e20 3d20 7365 6c66 2e67 6574 5f6d 6178  n = self.get_max
+000028b0: 5f6c 656e 6774 6828 290d 0a20 2020 2020  _length()..     
+000028c0: 2020 2023 2067 6574 2074 6865 2069 6e70     # get the inp
+000028d0: 7574 2074 6578 7420 7769 7468 2066 6978  ut text with fix
+000028e0: 6564 206c 656e 6774 6820 706c 7573 206f  ed length plus o
+000028f0: 6e65 2065 7874 7261 2073 7061 6365 2066  ne extra space f
+00002900: 6f72 2074 6865 2070 6f69 6e74 6572 0d0a  or the pointer..
+00002910: 2020 2020 2020 2020 6966 2076 6965 772b          if view+
+00002920: 6d61 785f 696e 7075 745f 6c65 6e2d 3120  max_input_len-1 
+00002930: 3c20 6c65 6e28 696e 7029 3a0d 0a20 2020  < len(inp):..   
+00002940: 2020 2020 2020 2020 2069 6e70 5f20 3d20           inp_ = 
+00002950: 696e 705b 7669 6577 3a76 6965 772b 6d61  inp[view:view+ma
+00002960: 785f 696e 7075 745f 6c65 6e5d 0d0a 2020  x_input_len]..  
+00002970: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00002980: 2020 2020 2020 2020 2069 6e70 5f20 3d20           inp_ = 
+00002990: 696e 705b 7669 6577 3a76 6965 772b 6d61  inp[view:view+ma
+000029a0: 785f 696e 7075 745f 6c65 6e2d 315d 202b  x_input_len-1] +
+000029b0: 2022 2022 0d0a 0d0a 2020 2020 2020 2020   " "....        
+000029c0: 6966 206e 6f74 2073 656c 662e 6973 5f64  if not self.is_d
+000029d0: 6973 6162 6c65 6420 616e 6420 7365 6c66  isabled and self
+000029e0: 2e73 686f 775f 706f 696e 7465 7220 6f72  .show_pointer or
+000029f0: 2069 6e70 5f5b 706f 696e 7465 722d 7669   inp_[pointer-vi
+00002a00: 6577 5d20 213d 2022 2022 3a0d 0a20 2020  ew] != " ":..   
+00002a10: 2020 2020 2020 2020 2070 6f69 6e74 6572           pointer
+00002a20: 5f73 7472 203d 2043 5374 7228 0d0a 2020  _str = CStr(..  
+00002a30: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00002a40: 705f 5b70 6f69 6e74 6572 2d76 6965 775d  p_[pointer-view]
+00002a50: 2c20 6261 636b 636f 6c6f 723d 2832 3230  , backcolor=(220
+00002a60: 2c20 3232 302c 2032 3230 292c 2066 6f72  , 220, 220), for
+00002a70: 6563 6f6c 6f72 3d28 3230 2c20 3230 2c20  ecolor=(20, 20, 
+00002a80: 3230 2929 0d0a 2020 2020 2020 2020 656c  20))..        el
+00002a90: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00002aa0: 2070 6f69 6e74 6572 5f73 7472 203d 2043   pointer_str = C
+00002ab0: 5374 7228 696e 705f 5b70 6f69 6e74 6572  Str(inp_[pointer
+00002ac0: 2d76 6965 775d 290d 0a20 2020 2020 2020  -view])..       
+00002ad0: 2023 2069 6e73 6572 7420 7468 6520 706f   # insert the po
+00002ae0: 696e 7465 7220 696e 746f 2069 6e70 7574  inter into input
+00002af0: 2074 6578 7420 6174 2074 6865 2063 6f72   text at the cor
+00002b00: 7265 6374 2070 6f73 6974 696f 6e0d 0a20  rect position.. 
+00002b10: 2020 2020 2020 2069 6e70 7574 5f70 6c75         input_plu
+00002b20: 735f 706f 696e 7465 7220 3d20 4353 7472  s_pointer = CStr
+00002b30: 280d 0a20 2020 2020 2020 2020 2020 2069  (..            i
+00002b40: 6e70 5f5b 3a70 6f69 6e74 6572 2d76 6965  np_[:pointer-vie
+00002b50: 775d 2920 2b20 706f 696e 7465 725f 7374  w]) + pointer_st
+00002b60: 7220 2b20 4353 7472 2869 6e70 5f5b 706f  r + CStr(inp_[po
+00002b70: 696e 7465 722d 7669 6577 2b31 3a5d 290d  inter-view+1:]).
+00002b80: 0a0d 0a20 2020 2020 2020 2074 6578 745f  ...        text_
+00002b90: 6320 3d20 2835 302c 2032 3030 2c20 3530  c = (50, 200, 50
+00002ba0: 290d 0a0d 0a20 2020 2020 2020 2066 7374  )....        fst
+00002bb0: 7220 3d20 4353 7472 2874 6578 742c 2066  r = CStr(text, f
+00002bc0: 6f72 6563 6f6c 6f72 3d74 6578 745f 6329  orecolor=text_c)
+00002bd0: 0d0a 0d0a 2020 2020 2020 2020 6261 636b  ....        back
+00002be0: 5f65 7869 7374 7320 3d20 4353 7472 2822  _exists = CStr("
+00002bf0: 3c22 2c20 666f 7265 636f 6c6f 723d 7465  <", forecolor=te
+00002c00: 7874 5f63 290d 0a20 2020 2020 2020 2066  xt_c)..        f
+00002c10: 6f72 7761 7264 5f65 7869 7374 7320 3d20  orward_exists = 
+00002c20: 4353 7472 2822 3e22 2c20 666f 7265 636f  CStr(">", foreco
+00002c30: 6c6f 723d 7465 7874 5f63 290d 0a0d 0a20  lor=text_c).... 
+00002c40: 2020 2020 2020 2066 7374 7220 2b3d 2028         fstr += (
+00002c50: 6261 636b 5f65 7869 7374 7320 6966 2076  back_exists if v
+00002c60: 6965 7720 213d 2030 2065 6c73 6520 2220  iew != 0 else " 
+00002c70: 2229 0d0a 2020 2020 2020 2020 6673 7472  ")..        fstr
+00002c80: 202b 3d20 696e 7075 745f 706c 7573 5f70   += input_plus_p
+00002c90: 6f69 6e74 6572 202b 2022 2022 202a 205c  ointer + " " * \
+00002ca0: 0d0a 2020 2020 2020 2020 2020 2020 286d  ..            (m
+00002cb0: 6178 5f69 6e70 7574 5f6c 656e 202d 206c  ax_input_len - l
+00002cc0: 656e 2869 6e70 7574 5f70 6c75 735f 706f  en(input_plus_po
+00002cd0: 696e 7465 7229 290d 0a20 2020 2020 2020  inter))..       
+00002ce0: 2066 7374 7220 2b3d 2028 666f 7277 6172   fstr += (forwar
+00002cf0: 645f 6578 6973 7473 2069 6620 7669 6577  d_exists if view
+00002d00: 2b6d 6178 5f69 6e70 7574 5f6c 656e 2d31  +max_input_len-1
+00002d10: 203c 206c 656e 2869 6e70 2920 656c 7365   < len(inp) else
+00002d20: 2022 2022 290d 0a0d 0a20 2020 2020 2020   " ")....       
+00002d30: 2072 6574 7572 6e20 6673 7472 0d0a 0d0a   return fstr....
+00002d40: 2020 2020 6465 6620 7265 6e64 6572 2873      def render(s
+00002d50: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
+00002d60: 203d 2031 0d0a 2020 2020 2020 2020 6966   = 1..        if
+00002d70: 2073 656c 662e 7061 7265 6e74 2e62 6163   self.parent.bac
+00002d80: 6b67 726f 756e 645f 636f 6c6f 7220 6973  kground_color is
+00002d90: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00002da0: 2020 2020 2020 2020 7465 7874 5f73 6861          text_sha
+00002db0: 646f 7720 3d20 7475 706c 6528 6d61 7028  dow = tuple(map(
+00002dc0: 6c61 6d62 6461 2078 3a20 7820 2a20 302e  lambda x: x * 0.
+00002dd0: 382c 206c 6973 7428 7365 6c66 2e70 6172  8, list(self.par
+00002de0: 656e 742e 6261 636b 6772 6f75 6e64 5f63  ent.background_c
+00002df0: 6f6c 6f72 2929 290d 0a20 2020 2020 2020  olor)))..       
+00002e00: 2020 2020 2073 656c 662e 6472 6177 6572       self.drawer
+00002e10: 2e70 6c61 6365 2843 5374 7228 2220 2220  .place(CStr(" " 
+00002e20: 2a20 2873 656c 662e 7369 7a65 2e67 6574  * (self.size.get
+00002e30: 5769 6474 6828 2920 2d20 2870 202a 2032  Width() - (p * 2
+00002e40: 2920 2d20 6c65 6e28 7365 6c66 2e74 6578  ) - len(self.tex
+00002e50: 7429 292c 2062 6163 6b63 6f6c 6f72 3d74  t)), backcolor=t
+00002e60: 6578 745f 7368 6164 6f77 292c 2070 6f73  ext_shadow), pos
+00002e70: 3d28 7020 2b20 6c65 6e28 7365 6c66 2e74  =(p + len(self.t
+00002e80: 6578 7429 2c20 3029 290d 0a20 2020 2020  ext), 0))..     
+00002e90: 2020 2073 656c 662e 6472 6177 6572 2e70     self.drawer.p
+00002ea0: 6c61 6365 2873 656c 662e 666f 726d 6174  lace(self.format
+00002eb0: 5f74 6578 7462 6f78 2829 2c20 706f 733d  _textbox(), pos=
+00002ec0: 2870 2c20 3029 290d 0a20 2020 2020 2020  (p, 0))..       
+00002ed0: 2023 7365 6c66 2e64 7261 7765 722e 7772   #self.drawer.wr
+00002ee0: 6974 655f 7465 7874 2873 7472 2874 6578  ite_text(str(tex
+00002ef0: 745f 7368 6164 6f77 292c 2070 6f73 3d28  t_shadow), pos=(
+00002f00: 302c 2030 2929 0d0a                      0, 0))..
```

