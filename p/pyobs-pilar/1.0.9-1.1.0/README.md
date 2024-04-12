# Comparing `tmp/pyobs_pilar-1.0.9.tar.gz` & `tmp/pyobs_pilar-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_pilar-1.0.9.tar", max compression
+gzip compressed data, was "pyobs_pilar-1.1.0.tar", max compression
```

## Comparing `pyobs_pilar-1.0.9.tar` & `pyobs_pilar-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1099 2023-12-04 21:06:23.143438 pyobs_pilar-1.0.9/LICENSE
--rw-r--r--   0        0        0       43 2023-12-04 21:06:23.143438 pyobs_pilar-1.0.9/pyobs_pilar/__init__.py
--rw-r--r--   0        0        0    26241 2023-12-04 21:06:23.147438 pyobs_pilar-1.0.9/pyobs_pilar/pilardriver.py
--rw-r--r--   0        0        0     4886 2023-12-04 21:06:23.147438 pyobs_pilar-1.0.9/pyobs_pilar/pilarerror.py
--rw-r--r--   0        0        0    28354 2023-12-04 21:06:23.147438 pyobs_pilar-1.0.9/pyobs_pilar/pilartelescope.py
--rw-r--r--   0        0        0      480 2023-12-04 21:06:23.147438 pyobs_pilar-1.0.9/pyproject.toml
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 pyobs_pilar-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-12 20:28:52.140924 pyobs_pilar-1.1.0/LICENSE
+-rw-r--r--   0        0        0       43 2024-04-12 20:28:52.140924 pyobs_pilar-1.1.0/pyobs_pilar/__init__.py
+-rw-r--r--   0        0        0    26241 2024-04-12 20:28:52.140924 pyobs_pilar-1.1.0/pyobs_pilar/pilardriver.py
+-rw-r--r--   0        0        0     4886 2024-04-12 20:28:52.140924 pyobs_pilar-1.1.0/pyobs_pilar/pilarerror.py
+-rw-r--r--   0        0        0    28589 2024-04-12 20:28:52.140924 pyobs_pilar-1.1.0/pyobs_pilar/pilartelescope.py
+-rw-r--r--   0        0        0      480 2024-04-12 20:28:52.140924 pyobs_pilar-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 pyobs_pilar-1.1.0/PKG-INFO
```

### Comparing `pyobs_pilar-1.0.9/LICENSE` & `pyobs_pilar-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_pilar-1.0.9/pyobs_pilar/pilardriver.py` & `pyobs_pilar-1.1.0/pyobs_pilar/pilardriver.py`

 * *Files identical despite different names*

### Comparing `pyobs_pilar-1.0.9/pyobs_pilar/pilarerror.py` & `pyobs_pilar-1.1.0/pyobs_pilar/pilarerror.py`

 * *Files identical despite different names*

### Comparing `pyobs_pilar-1.0.9/pyobs_pilar/pilartelescope.py` & `pyobs_pilar-1.1.0/pyobs_pilar/pilartelescope.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import asyncio
 import datetime
 import logging
 import os.path
 import time
 from typing import Tuple, List, Dict, Any, Optional, NamedTuple, Union
-from astropy.coordinates import SkyCoord
+
+from astroplan import Observer
+from astropy.coordinates import SkyCoord, EarthLocation
 import astropy.units as u
 import numpy as np
 
 from pyobs.mixins import FitsNamespaceMixin
 from pyobs.events import FilterChangedEvent, OffsetsAltAzEvent
 from pyobs.interfaces import IFilters, IFocuser, ITemperatures, IOffsetsAltAz, IPointingSeries
 from pyobs.modules import timeout
@@ -282,15 +284,14 @@
         # get headers from base
         hdr = await BaseTelescope.get_fits_header_before(self)
 
         # define values to request
         keys = {
             "TEL-FOCU": ("POSITION.INSTRUMENTAL.FOCUS.REALPOS", "Focus position [mm]"),
             "TEL-ROT": ("POSITION.INSTRUMENTAL.DEROTATOR[2].REALPOS", "Derotator instrumental position at end [deg]"),
-            "DEROTOFF": ("POINTING.SETUP.DEROTATOR.OFFSET", "Derotator offset [deg]"),
             "AZOFF": ("POSITION.INSTRUMENTAL.AZ.OFFSET", "Azimuth offset"),
             "ALTOFF": ("POSITION.INSTRUMENTAL.ZD.OFFSET", "Altitude offset"),
         }
 
         # add ones from config
         for var, h in self._pilar_fits_headers.items():
             keys[h[0]] = (var, h[1])
@@ -308,14 +309,20 @@
         hdr["ALTOFF"] = (-hdr["ALTOFF"][0], hdr["ALTOFF"][1])
 
         # filter
         if "POSITION.INSTRUMENTAL.FILTER[2].CURRPOS" in status:
             filter_id = status["POSITION.INSTRUMENTAL.FILTER[2].CURRPOS"]
             hdr["FILTER"] = (await self._pilar.filter_name(int(filter_id)), "Current filter")
 
+        # derotator offset
+        derotator_position = self._calculate_derotator_position(
+            hdr["TEL-RA"][0], hdr["TEL-DEC"][0], hdr["TEL-ALT"][0], Time.now()
+        )
+        hdr["DEROTOFF"] = (derotator_position - hdr["TEL-ROT"][0], "Derotator offset [deg]")
+
         # return it
         return self._filter_fits_namespace(hdr, namespaces=namespaces, **kwargs)
 
     async def get_radec(self, **kwargs: Any) -> Tuple[float, float]:
         """Returns current RA and Dec.
 
         Returns:
```

### Comparing `pyobs_pilar-1.0.9/PKG-INFO` & `pyobs_pilar-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobs-pilar
-Version: 1.0.9
+Version: 1.1.0
 Summary: pyobs module for Pilar TCS
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

