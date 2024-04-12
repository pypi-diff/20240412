# Comparing `tmp/widgetastic.core-1.0.6-py3-none-any.whl.zip` & `tmp/widgetastic.core-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 60444 bytes, number of entries: 23
+Zip file size: 60458 bytes, number of entries: 23
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 widgetastic/__init__.py
 -rw-r--r--  2.0 unx    47045 b- defN 20-Feb-02 00:00 widgetastic/browser.py
 -rw-r--r--  2.0 unx     1144 b- defN 20-Feb-02 00:00 widgetastic/exceptions.py
 -rw-r--r--  2.0 unx     6509 b- defN 20-Feb-02 00:00 widgetastic/log.py
--rw-r--r--  2.0 unx      912 b- defN 20-Feb-02 00:00 widgetastic/types.py
--rw-r--r--  2.0 unx    26515 b- defN 20-Feb-02 00:00 widgetastic/utils.py
+-rw-r--r--  2.0 unx      904 b- defN 20-Feb-02 00:00 widgetastic/types.py
+-rw-r--r--  2.0 unx    26516 b- defN 20-Feb-02 00:00 widgetastic/utils.py
 -rw-r--r--  2.0 unx      701 b- defN 20-Feb-02 00:00 widgetastic/xpath.py
 -rw-r--r--  2.0 unx     3736 b- defN 20-Feb-02 00:00 widgetastic/ouia/__init__.py
 -rw-r--r--  2.0 unx      896 b- defN 20-Feb-02 00:00 widgetastic/ouia/checkbox.py
 -rw-r--r--  2.0 unx      743 b- defN 20-Feb-02 00:00 widgetastic/ouia/input.py
 -rw-r--r--  2.0 unx      474 b- defN 20-Feb-02 00:00 widgetastic/ouia/text.py
--rw-r--r--  2.0 unx      635 b- defN 20-Feb-02 00:00 widgetastic/widget/__init__.py
--rw-r--r--  2.0 unx    48883 b- defN 20-Feb-02 00:00 widgetastic/widget/base.py
+-rw-r--r--  2.0 unx      636 b- defN 20-Feb-02 00:00 widgetastic/widget/__init__.py
+-rw-r--r--  2.0 unx    48885 b- defN 20-Feb-02 00:00 widgetastic/widget/base.py
 -rw-r--r--  2.0 unx     1009 b- defN 20-Feb-02 00:00 widgetastic/widget/checkbox.py
 -rw-r--r--  2.0 unx      557 b- defN 20-Feb-02 00:00 widgetastic/widget/image.py
 -rw-r--r--  2.0 unx     3968 b- defN 20-Feb-02 00:00 widgetastic/widget/input.py
 -rw-r--r--  2.0 unx    10250 b- defN 20-Feb-02 00:00 widgetastic/widget/select.py
--rw-r--r--  2.0 unx    49913 b- defN 20-Feb-02 00:00 widgetastic/widget/table.py
+-rw-r--r--  2.0 unx    49914 b- defN 20-Feb-02 00:00 widgetastic/widget/table.py
 -rw-r--r--  2.0 unx      396 b- defN 20-Feb-02 00:00 widgetastic/widget/text.py
-?rw-r--r--  2.0 unx     4317 b- defN 20-Feb-02 00:00 widgetastic.core-1.0.6.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 widgetastic.core-1.0.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx      576 b- defN 20-Feb-02 00:00 widgetastic.core-1.0.6.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1889 b- defN 20-Feb-02 00:00 widgetastic.core-1.0.6.dist-info/RECORD
-23 files, 211155 bytes uncompressed, 57392 bytes compressed:  72.8%
+?rw-r--r--  2.0 unx     4419 b- defN 20-Feb-02 00:00 widgetastic.core-1.0.7.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 widgetastic.core-1.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx      576 b- defN 20-Feb-02 00:00 widgetastic.core-1.0.7.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1889 b- defN 20-Feb-02 00:00 widgetastic.core-1.0.7.dist-info/RECORD
+23 files, 211254 bytes uncompressed, 57406 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: widgetastic/widget/table.py
 Comment: 
 
 Filename: widgetastic/widget/text.py
 Comment: 
 
-Filename: widgetastic.core-1.0.6.dist-info/METADATA
+Filename: widgetastic.core-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: widgetastic.core-1.0.6.dist-info/WHEEL
+Filename: widgetastic.core-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: widgetastic.core-1.0.6.dist-info/licenses/LICENSE
+Filename: widgetastic.core-1.0.7.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: widgetastic.core-1.0.6.dist-info/RECORD
+Filename: widgetastic.core-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## widgetastic/types.py

```diff
@@ -17,16 +17,15 @@
     from .widget.base import Widget
     from .widget.base import ClickableMixin
 
 
 class LocatorProtocol(Protocol):
     CHECK_VISIBILITY: bool
 
-    def __locator__(self) -> Union[str, Locator, WebElement]:
-        ...
+    def __locator__(self) -> Union[str, Locator, WebElement]: ...
 
 
 LocatorAlias = Union[str, Dict[str, str], WebElement, LocatorProtocol, "Widget"]
 
 ElementParent = Union[LocatorAlias, "Browser"]
 
 ViewParent = Union["Browser", "View"]
```

## widgetastic/utils.py

```diff
@@ -1,8 +1,9 @@
 """This module contains some supporting classes."""
+
 import functools
 import re
 import string
 import time
 from threading import Lock
 
 from cached_property import cached_property
```

## widgetastic/widget/__init__.py

```diff
@@ -1,8 +1,9 @@
 """This module contains the base classes that are used to implement the more specific behaviour."""
+
 from .base import *  # noqa: F403 F401
 from .checkbox import Checkbox
 from .image import Image
 from .input import BaseInput
 from .input import ColourInput
 from .input import FileInput
 from .input import TextInput
```

## widgetastic/widget/base.py

```diff
@@ -368,17 +368,17 @@
                 return self.parent_browser.element(locator)
 
     def _get_included_widget(self, includer_id, widget_name, use_parent):
         if includer_id not in self._initialized_included_widgets:
             for widget_includer in self._included_widgets:
                 if widget_includer._seq_id == includer_id:
                     parent = self if use_parent else self.parent
-                    self._initialized_included_widgets[
-                        widget_includer._seq_id
-                    ] = widget_includer.widget_class(parent, self.logger)
+                    self._initialized_included_widgets[widget_includer._seq_id] = (
+                        widget_includer.widget_class(parent, self.logger)
+                    )
                     break
             else:
                 raise ValueError(f"Could not find includer #{includer_id}")
         return getattr(self._initialized_included_widgets[includer_id], widget_name)
 
     def flush_widget_cache(self):
         """Flush the widget cache recursively for the whole :py:class:`Widget` tree structure.
```

## widgetastic/widget/table.py

```diff
@@ -1,8 +1,9 @@
 """This module contains the base classes that are used to implement the more specific behaviour."""
+
 import itertools
 import re
 from collections import defaultdict
 from collections import deque
 from copy import copy
 from operator import attrgetter
```

## Comparing `widgetastic.core-1.0.6.dist-info/METADATA` & `widgetastic.core-1.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: widgetastic.core
-Version: 1.0.6
+Version: 1.0.7
 Summary: Making testing of UIs fantastic.
 Project-URL: repository, https://github.com/RedHatQE/widgetastic.core
 Maintainer-email: Mike Shriver <mshriver@redhat.com>, Nikhil Dhandre <ndhandre@redhat.com>, Egor Shamardin <eshamard@redhat.com>
 License: Copyright 2016 Red Hat, Inc. and/or its affiliates
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
@@ -21,14 +21,16 @@
 Keywords: selenium,widgetastic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Requires-Dist: anytree>=2.9.0
```

## Comparing `widgetastic.core-1.0.6.dist-info/licenses/LICENSE` & `widgetastic.core-1.0.7.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `widgetastic.core-1.0.6.dist-info/RECORD` & `widgetastic.core-1.0.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 widgetastic/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 widgetastic/browser.py,sha256=AY9kmXEGQ8OkiqlYGHD4QQjk08Zuqkch_ZlGS3MoV1E,47045
 widgetastic/exceptions.py,sha256=RvlE7KpzocwNQuD8j2ijbtSVtSK_cUkiQFknMPhubHQ,1144
 widgetastic/log.py,sha256=HhZuxJaQu5ja-lezLtItwa2vGp0ZisT8Zobk-GxiSDs,6509
-widgetastic/types.py,sha256=4FM9V43Z36reqXJDcAev1n0mvO3n0UCAjKwaOId8aHs,912
-widgetastic/utils.py,sha256=8tCq-zOCUgIGueLHmwiqzw88suHmPNv-dvsNbaf9IV8,26515
+widgetastic/types.py,sha256=rK1gXXiQEsZRMvh50HNjurmQtyRbVsfXr4KC6wq9j8I,904
+widgetastic/utils.py,sha256=jVCovAltPAZxgScP601RZAfEmibVcNpezZ3_KeZQtLE,26516
 widgetastic/xpath.py,sha256=nO2P3WezEWGtcxFVVM3r0CaKbfYmvC8GwIx9JGJ_vT0,701
 widgetastic/ouia/__init__.py,sha256=nLJfX_Skor-uJTq0Ru60Q0oQ-NB2S7vhs6E4srTwIi8,3736
 widgetastic/ouia/checkbox.py,sha256=FF4mjmprgM80QiUBNTqDkzliElClZwa6IMRfIJzEz_g,896
 widgetastic/ouia/input.py,sha256=fVbhXwwRWMj6UrhPmts7E1XYxVKjMVDedTdcflV0Npc,743
 widgetastic/ouia/text.py,sha256=XNmBy1PGO81otZ4tUSPXxcq9QiC8hJkxA2AVMVhQuu8,474
-widgetastic/widget/__init__.py,sha256=wOeVK1t7tEwkGoo2W0TKb4Qy1EQPFtuS0ViCcNW2rR4,635
-widgetastic/widget/base.py,sha256=IkPt1PhO2h7Ufl6Iq-rU1nGfjgJKI9kpKNARHMc5GME,48883
+widgetastic/widget/__init__.py,sha256=F9HabqzmzkUCDoDoLCdCbagOWUjdgsAhE6UaShwo39c,636
+widgetastic/widget/base.py,sha256=apTo8aWoO8HuT5YMtEtmAp127wXNOnHBXiVuzw0RT7Y,48885
 widgetastic/widget/checkbox.py,sha256=TC38ynfe7lihEZ52QnnElFOP5lYr2fXcjrnvSgUk4tk,1009
 widgetastic/widget/image.py,sha256=SCK2AEP4retoIXfFlQIkAIjX3SFWJXgrT4VDqkyw1ZM,557
 widgetastic/widget/input.py,sha256=lDc0OjrxV3d3wN0oktzTM9iYxIgOHhXlyDk57MEeY78,3968
 widgetastic/widget/select.py,sha256=W0WBNd7bE8-ivWc7FhcNjlWpn6bNk4kcjPQhEaHlft4,10250
-widgetastic/widget/table.py,sha256=jXWq5RO9NbTyt22nSI5Ri46oU3xKgIEDwImYbbWHR58,49913
+widgetastic/widget/table.py,sha256=eoZ6reMlCI2SGOVy09tulWTWyKbbmshNKzGKq7-1chA,49914
 widgetastic/widget/text.py,sha256=CYmx0Hk9D0RMDmjqq_lPI16rUPUqVw9awgh61CYfK1I,396
-widgetastic.core-1.0.6.dist-info/METADATA,sha256=YNfNB4unRbmvi7dvt6bgh7K0XJ1ZkuyRu9sRQkQL5N8,4317
-widgetastic.core-1.0.6.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-widgetastic.core-1.0.6.dist-info/licenses/LICENSE,sha256=NuGzUo4RDqzetocms7YRvD32-u4e0gqjS47Pqy2l830,576
-widgetastic.core-1.0.6.dist-info/RECORD,,
+widgetastic.core-1.0.7.dist-info/METADATA,sha256=lCPY-7qoRrRP5NEFM6fPIHwOPqlj3Bi4ZyelojHw4oQ,4419
+widgetastic.core-1.0.7.dist-info/WHEEL,sha256=as-1oFTWSeWBgyzh0O_qF439xqBe6AbBgt4MfYe5zwY,87
+widgetastic.core-1.0.7.dist-info/licenses/LICENSE,sha256=NuGzUo4RDqzetocms7YRvD32-u4e0gqjS47Pqy2l830,576
+widgetastic.core-1.0.7.dist-info/RECORD,,
```

