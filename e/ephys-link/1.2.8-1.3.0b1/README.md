# Comparing `tmp/ephys_link-1.2.8.tar.gz` & `tmp/ephys_link-1.3.0b1.tar.gz`

## Comparing `ephys_link-1.2.8.tar` & `ephys_link-1.3.0b1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ephys_link-1.2.8/ephys_link.spec
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 ephys_link-1.2.8/assets/icon.ico
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ephys_link-1.2.8/scripts/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 ephys_link-1.2.8/scripts/move_tester.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/__main__.py
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/common.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/emergency_stop.py
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/gui.py
--rw-r--r--   0        0        0    20071 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platform_handler.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platform_manipulator.py
--rw-r--r--   0        0        0    16931 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/server.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platforms/__init__.py
--rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platforms/new_scale_handler.py
--rw-r--r--   0        0        0    12004 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platforms/new_scale_manipulator.py
--rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platforms/new_scale_pathfinder_handler.py
--rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platforms/sensapex_handler.py
--rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platforms/sensapex_manipulator.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platforms/ump3_handler.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/platforms/ump3_manipulator.py
--rw-r--r--   0        0        0   810232 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/resources/CP210xManufacturing.dll
--rw-r--r--   0        0        0   155136 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/resources/NstMotorCtrl.dll
--rw-r--r--   0        0        0   469752 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/resources/SiUSBXp.dll
--rw-r--r--   0        0        0   316316 2020-02-02 00:00:00.000000 ephys_link-1.2.8/src/ephys_link/resources/libum.dll
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ephys_link-1.2.8/tests/__init__.py
--rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 ephys_link-1.2.8/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 ephys_link-1.2.8/LICENSE
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 ephys_link-1.2.8/README.md
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 ephys_link-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 ephys_link-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/ephys_link.spec
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/assets/icon.ico
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/scripts/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/scripts/move_tester.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/__main__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/common.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/emergency_stop.py
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/gui.py
+-rw-r--r--   0        0        0    19432 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platform_handler.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platform_manipulator.py
+-rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/server.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/__init__.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_handler.py
+-rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_manipulator.py
+-rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_pathfinder_handler.py
+-rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/sensapex_handler.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/sensapex_manipulator.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/ump3_handler.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/ump3_manipulator.py
+-rw-r--r--   0        0        0   810232 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/resources/CP210xManufacturing.dll
+-rw-r--r--   0        0        0   155136 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/resources/NstMotorCtrl.dll
+-rw-r--r--   0        0        0   469752 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/resources/SiUSBXp.dll
+-rw-r--r--   0        0        0   316316 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/resources/libum.dll
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/LICENSE
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/PKG-INFO
```

### Comparing `ephys_link-1.2.8/ephys_link.spec` & `ephys_link-1.3.0b1/ephys_link.spec`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/assets/icon.ico` & `ephys_link-1.3.0b1/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/scripts/move_tester.py` & `ephys_link-1.3.0b1/scripts/move_tester.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/src/ephys_link/__main__.py` & `ephys_link-1.3.0b1/src/ephys_link/__main__.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/src/ephys_link/emergency_stop.py` & `ephys_link-1.3.0b1/src/ephys_link/emergency_stop.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/src/ephys_link/gui.py` & `ephys_link-1.3.0b1/src/ephys_link/gui.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/src/ephys_link/platform_handler.py` & `ephys_link-1.3.0b1/src/ephys_link/platform_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,35 +13,49 @@
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
+from vbl_aquarium.models.ephys_link import (
+    AngularResponse,
+    BooleanStateResponse,
+    CanWriteRequest,
+    DriveToDepthRequest,
+    DriveToDepthResponse,
+    GetManipulatorsResponse,
+    GotoPositionRequest,
+    InsideBrainRequest,
+    PositionalResponse,
+    ShankCountResponse,
+)
+from vbl_aquarium.models.unity import Vector4
+
 from ephys_link import common as com
 
 if TYPE_CHECKING:
     import socketio
 
 
 class PlatformHandler(ABC):
     """An abstract class that defines the interface for a manipulator handler."""
 
     def __init__(self):
         """Initialize the manipulator handler with a dictionary of manipulators."""
 
         # Registered manipulators are stored as a dictionary of IDs (string) to
-        # manipulator objects
+        # manipulator objects.
         self.manipulators = {}
         self.num_axes = 4
 
         # Platform axes dimensions in mm
-        self.dimensions = [20, 20, 20, 20]
+        self.dimensions = Vector4(x=20, y=20, z=20, w=20)
 
-    # Platform Handler Methods
+    # Platform Handler Methods.
 
     def reset(self) -> bool:
         """Reset handler.
 
         :return: True if successful, False otherwise.
         :rtype: bool
         """
@@ -61,29 +75,29 @@
                     manipulator.stop()
         except Exception as e:
             print(f"[ERROR]\t\t Could not stop manipulators: {e}\n")
             return False
         else:
             return True
 
-    def get_manipulators(self) -> com.GetManipulatorsOutputData:
+    def get_manipulators(self) -> GetManipulatorsResponse:
         """Get all registered manipulators.
 
         :return: Result of connected manipulators, platform information, and error message (if any).
-        :rtype: :class:`ephys_link.common.GetManipulatorsOutputData`
+        :rtype: :class:`vbl_aquarium.models.ephys_link.GetManipulatorsResponse`
         """
-        error = "Error getting manipulators"
         try:
-            devices = self._get_manipulators()
-            error = ""
+            manipulators = self._get_manipulators()
         except Exception as e:
             print(f"[ERROR]\t\t Getting manipulators: {type(e)}: {e}\n")
-            return com.GetManipulatorsOutputData([], self.num_axes, self.dimensions, error)
+            return GetManipulatorsResponse(error="Error getting manipulators")
         else:
-            return com.GetManipulatorsOutputData(devices, self.num_axes, self.dimensions, error)
+            return GetManipulatorsResponse(
+                manipulators=manipulators, num_axes=self.num_axes, dimensions=self.dimensions
+            )
 
     def register_manipulator(self, manipulator_id: str) -> str:
         """Register a manipulator.
 
         :param manipulator_id: The ID of the manipulator to register.
         :type manipulator_id: str
         :return: Error message on error, empty string otherwise.
@@ -131,188 +145,173 @@
             print(f"[ERROR]\t\t Unregistering manipulator: {manipulator_id}")
             print(f"{e}\n")
             return "Error unregistering manipulator"
         else:
             com.dprint(f"[SUCCESS]\t Unregistered manipulator: {manipulator_id}\n")
             return ""
 
-    def get_pos(self, manipulator_id: str) -> com.PositionalOutputData:
+    def get_pos(self, manipulator_id: str) -> PositionalResponse:
         """Get the current position of a manipulator.
 
         :param manipulator_id: The ID of the manipulator to get the position of.
         :type manipulator_id: str
         :return: Positional information for the manipulator and error message (if any).
-        :rtype: :class:`ephys_link.common.PositionalOutputData`
+        :rtype: :class:`vbl_aquarium.models.ephys_link.PositionalResponse`
         """
         try:
-            # Check calibration status
+            # Check calibration status.
             if (
                 hasattr(self.manipulators[manipulator_id], "get_calibrated")
                 and not self.manipulators[manipulator_id].get_calibrated()
             ):
                 print(f"[ERROR]\t\t Calibration not complete: {manipulator_id}\n")
-                return com.PositionalOutputData([], "Manipulator not calibrated")
+                return PositionalResponse(error="Manipulator not calibrated")
 
-            # Get position and convert to unified space
+            # Get position and convert to unified space.
             manipulator_pos = self._get_pos(manipulator_id)
 
-            # Shortcut return for Pathfinder
+            # Shortcut return for Pathfinder.
             if self.num_axes == -1:
                 return manipulator_pos
 
-            # Error check and convert position to unified space
-            if manipulator_pos["error"] != "":
-                return manipulator_pos
-            return com.PositionalOutputData(self._platform_space_to_unified_space(manipulator_pos["position"]), "")
+            # Convert position to unified space.
+            return manipulator_pos.model_copy(
+                update={"position": self._platform_space_to_unified_space(manipulator_pos.position)}
+            )
         except KeyError:
-            # Manipulator not found in registered manipulators
+            # Manipulator not found in registered manipulators.
             print(f"[ERROR]\t\t Manipulator not registered: {manipulator_id}")
-            return com.PositionalOutputData([], "Manipulator not registered")
+            return PositionalResponse(error="Manipulator not registered")
 
-    def get_angles(self, manipulator_id: str) -> com.AngularOutputData:
+    def get_angles(self, manipulator_id: str) -> AngularResponse:
         """Get the current position of a manipulator.
 
         :param manipulator_id: The ID of the manipulator to get the angles of.
         :type manipulator_id: str
         :return: Angular information for the manipulator and error message (if any).
-        :rtype: :class:`ephys_link.common.AngularOutputData`
+        :rtype: :class:`vbl_aquarium.models.ephys_link.AngularResponse`
         """
         try:
             # Check calibration status
             if (
                 hasattr(self.manipulators[manipulator_id], "get_calibrated")
                 and not self.manipulators[manipulator_id].get_calibrated()
             ):
                 print(f"[ERROR]\t\t Calibration not complete: {manipulator_id}\n")
-                return com.AngularOutputData([], "Manipulator not calibrated")
+                return AngularResponse(error="Manipulator not calibrated")
 
             # Get position
             return self._get_angles(manipulator_id)
 
         except KeyError:
             # Manipulator not found in registered manipulators
             print(f"[ERROR]\t\t Manipulator not registered: {manipulator_id}")
-            return com.AngularOutputData([], "Manipulator not registered")
+            return AngularResponse(error="Manipulator not registered")
 
-    def get_shank_count(self, manipulator_id: str) -> com.ShankCountOutputData:
+    def get_shank_count(self, manipulator_id: str) -> ShankCountResponse:
         """Get the number of shanks on the probe
 
         :param manipulator_id: The ID of the manipulator to get the number of shanks of.
         :type manipulator_id: str
         :return: Number of shanks on the probe.
-        :rtype: :class:`ephys_link.common.ShankCountOutputData`
+        :rtype: :class:`vbl_aquarium.models.ephys_link.ShankCountResponse`
         """
         return self._get_shank_count(manipulator_id)
 
-    async def goto_pos(self, manipulator_id: str, position: list[float], speed: float) -> com.PositionalOutputData:
+    async def goto_pos(self, request: GotoPositionRequest) -> PositionalResponse:
         """Move manipulator to position
 
-        :param manipulator_id: The ID of the manipulator to move
-        :type manipulator_id: str
-        :param position: The position to move to in (x, y, z, w) in mm
-        :type position: list[float]
-        :param speed: The speed to move at (in mm/s)
-        :type speed: float
+        :param request: The goto request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.GotoPositionRequest`
         :return: Resulting position of the manipulator and error message (if any).
-        :rtype: :class:`ephys_link.common.PositionalOutputData`
+        :rtype: :class:`vbl_aquarium.models.ephys_link.PositionalResponse`
         """
         try:
-            # Check calibration status
-            if not self.manipulators[manipulator_id].get_calibrated():
-                print(f"[ERROR]\t\t Calibration not complete: {manipulator_id}\n")
-                return com.PositionalOutputData([], "Manipulator not calibrated")
-
-            # Check write state
-            if not self.manipulators[manipulator_id].get_can_write():
-                print(f"[ERROR]\t\t Cannot write to manipulator: {manipulator_id}")
-                return com.PositionalOutputData([], "Cannot write to manipulator")
+            # Check calibration status.
+            if not self.manipulators[request.manipulator_id].get_calibrated():
+                print(f"[ERROR]\t\t Calibration not complete: {request.manipulator_id}\n")
+                return PositionalResponse(error="Manipulator not calibrated")
+
+            # Check write state.
+            if not self.manipulators[request.manipulator_id].get_can_write():
+                print(f"[ERROR]\t\t Cannot write to manipulator: {request.manipulator_id}")
+                return PositionalResponse(error="Cannot write to manipulator")
 
             # Convert position to platform space, move, and convert final position back to
-            # unified space
-            end_position = await self._goto_pos(manipulator_id, self._unified_space_to_platform_space(position), speed)
-            if end_position["error"] != "":
-                return end_position
-            return com.PositionalOutputData(self._platform_space_to_unified_space(end_position["position"]), "")
-
+            # unified space.
+            end_position = await self._goto_pos(
+                request.model_copy(update={"position": self._unified_space_to_platform_space(request.position)})
+            )
+            return end_position.model_copy(
+                update={"position": self._platform_space_to_unified_space(end_position.position)}
+            )
         except KeyError:
-            # Manipulator not found in registered manipulators
-            print(f"[ERROR]\t\t Manipulator not registered: {manipulator_id}\n")
-            return com.PositionalOutputData([], "Manipulator not registered")
+            # Manipulator not found in registered manipulators.
+            print(f"[ERROR]\t\t Manipulator not registered: {request.manipulator_id}\n")
+            return PositionalResponse(error="Manipulator not registered")
 
-    async def drive_to_depth(self, manipulator_id: str, depth: float, speed: float) -> com.DriveToDepthOutputData:
+    async def drive_to_depth(self, request: DriveToDepthRequest) -> DriveToDepthResponse:
         """Drive manipulator to depth
 
-        :param manipulator_id: The ID of the manipulator to drive
-        :type manipulator_id: str
-        :param depth: The depth to drive to in mm
-        :type depth: float
-        :param speed: The speed to drive at (in mm/s)
-        :type speed: float
+        :param request: The drive to depth request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.DriveToDepthRequest`
         :return: Resulting depth of the manipulator and error message (if any).
         :rtype: :class:`ephys_link.common.DriveToDepthOutputData`
         """
         try:
             # Check calibration status
-            if not self.manipulators[manipulator_id].get_calibrated():
-                print(f"[ERROR]\t\t Calibration not complete: {manipulator_id}\n")
-                return com.DriveToDepthOutputData(0, "Manipulator not calibrated")
+            if not self.manipulators[request.manipulator_id].get_calibrated():
+                print(f"[ERROR]\t\t Calibration not complete: {request.manipulator_id}\n")
+                return DriveToDepthResponse(error="Manipulator not calibrated")
 
             # Check write state
-            if not self.manipulators[manipulator_id].get_can_write():
-                print(f"[ERROR]\t\t Cannot write to manipulator: {manipulator_id}")
-                return com.DriveToDepthOutputData(0, "Cannot write to manipulator")
+            if not self.manipulators[request.manipulator_id].get_can_write():
+                print(f"[ERROR]\t\t Cannot write to manipulator: {request.manipulator_id}")
+                return DriveToDepthResponse(error="Cannot write to manipulator")
 
             end_depth = await self._drive_to_depth(
-                manipulator_id,
-                self._unified_space_to_platform_space([0, 0, 0, depth])[3],
-                speed,
+                request.model_copy(update={"depth": self._unified_space_to_platform_space(Vector4(w=request.depth)).w})
             )
-            if end_depth["error"] != "":
-                return end_depth
-            return com.DriveToDepthOutputData(
-                self._platform_space_to_unified_space([0, 0, 0, end_depth["depth"]])[3],
-                "",
+            return end_depth.model_copy(
+                update={"depth": self._platform_space_to_unified_space(Vector4(w=end_depth.depth)).w}
             )
-
         except KeyError:
             # Manipulator not found in registered manipulators
-            print(f"[ERROR]\t\t Manipulator not registered: {manipulator_id}\n")
-            return com.DriveToDepthOutputData(0, "Manipulator " "not registered")
+            print(f"[ERROR]\t\t Manipulator not registered: {request.manipulator_id}\n")
+            return DriveToDepthResponse(error="Manipulator not registered")
 
-    def set_inside_brain(self, manipulator_id: str, inside: bool) -> com.StateOutputData:
+    def set_inside_brain(self, request: InsideBrainRequest) -> BooleanStateResponse:
         """Set manipulator inside brain state (restricts motion)
 
-        :param manipulator_id: The ID of the manipulator to set the state of
-        :type manipulator_id: str
-        :param inside: True if inside brain, False if outside
-        :type inside: bool
+        :param request: The inside brain request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.InsideBrainRequest`
         :return: New inside brain state of the manipulator and error message (if any).
-        :rtype: :class:`ephys_link.common.StateOutputData`
+        :rtype: :class:`vbl_aquarium.models.ephys_link.BooleanStateResponse`
         """
         try:
             # Check calibration status
             if (
-                hasattr(self.manipulators[manipulator_id], "get_calibrated")
-                and not self.manipulators[manipulator_id].get_calibrated()
+                hasattr(self.manipulators[request.manipulator_id], "get_calibrated")
+                and not self.manipulators[request.manipulator_id].get_calibrated()
             ):
                 print("[ERROR]\t\t Calibration not complete\n")
-                return com.StateOutputData(False, "Manipulator not calibrated")
+                return BooleanStateResponse(error="Manipulator not calibrated")
 
-            return self._set_inside_brain(manipulator_id, inside)
+            return self._set_inside_brain(request)
 
         except KeyError:
             # Manipulator not found in registered manipulators
-            print(f"[ERROR]\t\t Manipulator {manipulator_id} not registered\n")
-            return com.StateOutputData(False, "Manipulator not " "registered")
+            print(f"[ERROR]\t\t Manipulator {request.manipulator_id} not registered\n")
+            return BooleanStateResponse(error="Manipulator not " "registered")
 
         except Exception as e:
             # Other error
-            print(f"[ERROR]\t\t Set manipulator {manipulator_id} inside brain " f"state")
+            print(f"[ERROR]\t\t Set manipulator {request.manipulator_id} inside brain " f"state")
             print(f"{e}\n")
-            return com.StateOutputData(False, "Error setting " "inside brain")
+            return BooleanStateResponse(error="Error setting inside brain")
 
     async def calibrate(self, manipulator_id: str, sio: socketio.AsyncServer) -> str:
         """Calibrate manipulator
 
         :param manipulator_id: ID of manipulator to calibrate
         :type manipulator_id: str
         :param sio: SocketIO object (to call sleep)
@@ -360,43 +359,34 @@
             # Other error
             print(f"[ERROR]\t\t Bypass calibration of manipulator {manipulator_id}")
             print(f"{e}\n")
             return "Error bypassing calibration"
 
     def set_can_write(
         self,
-        manipulator_id: str,
-        can_write: bool,
-        hours: float,
-        sio: socketio.AsyncServer,
-    ) -> com.StateOutputData:
+        request: CanWriteRequest,
+    ) -> BooleanStateResponse:
         """Set manipulator can_write state (enables/disabled moving manipulator)
 
-        :param manipulator_id: The ID of the manipulator to set the state of
-        :type manipulator_id: str
-        :param can_write: True if allowed to move, False if outside
-        :type can_write: bool
-        :param hours: The number of hours to allow writing (0 = forever)
-        :type hours: float
-        :param sio: SocketIO object from server to emit reset event
-        :type sio: :class:`socketio.AsyncServer`
+        :param request: The can write request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.CanWriteRequest`
         :return: New can_write state of the manipulator and error message (if any).
         :rtype: :class:`ephys_link.common.StateOutputData`
         """
         try:
-            return self._set_can_write(manipulator_id, can_write, hours, sio)
+            return self._set_can_write(request)
         except KeyError:
             # Manipulator not found in registered manipulators
-            print(f"[ERROR]\t\t Manipulator not registered: {manipulator_id}\n")
-            return com.StateOutputData(False, "Manipulator not " "registered")
+            print(f"[ERROR]\t\t Manipulator not registered: {request.manipulator_id}\n")
+            return BooleanStateResponse(error="Manipulator not registered")
         except Exception as e:
             # Other error
-            print(f"[ERROR]\t\t Set manipulator {manipulator_id} can_write state")
+            print(f"[ERROR]\t\t Set manipulator {request.manipulator_id} can_write state")
             print(f"{e}\n")
-            return com.StateOutputData(False, "Error setting " "can_write")
+            return BooleanStateResponse(error="Error setting can_write")
 
     # Platform specific methods to override
 
     @abstractmethod
     def _get_manipulators(self) -> list:
         raise NotImplementedError
 
@@ -405,35 +395,35 @@
         raise NotImplementedError
 
     @abstractmethod
     def _unregister_manipulator(self, manipulator_id: str) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def _get_pos(self, manipulator_id: str) -> com.PositionalOutputData:
+    def _get_pos(self, manipulator_id: str) -> PositionalResponse:
         raise NotImplementedError
 
     @abstractmethod
-    def _get_angles(self, manipulator_id: str) -> com.AngularOutputData:
+    def _get_angles(self, manipulator_id: str) -> AngularResponse:
         raise NotImplementedError
 
     @abstractmethod
-    def _get_shank_count(self, manipulator_id: str) -> com.ShankCountOutputData:
+    def _get_shank_count(self, manipulator_id: str) -> ShankCountResponse:
         raise NotImplementedError
 
     @abstractmethod
-    async def _goto_pos(self, manipulator_id: str, position: list[float], speed: float) -> com.PositionalOutputData:
+    async def _goto_pos(self, request: GotoPositionRequest) -> PositionalResponse:
         raise NotImplementedError
 
     @abstractmethod
-    async def _drive_to_depth(self, manipulator_id: str, depth: float, speed: float) -> com.DriveToDepthOutputData:
+    async def _drive_to_depth(self, request: DriveToDepthRequest) -> DriveToDepthResponse:
         raise NotImplementedError
 
     @abstractmethod
-    def _set_inside_brain(self, manipulator_id: str, inside: bool) -> com.StateOutputData:
+    def _set_inside_brain(self, request: InsideBrainRequest) -> BooleanStateResponse:
         raise NotImplementedError
 
     @abstractmethod
     async def _calibrate(self, manipulator_id: str, sio: socketio.AsyncServer) -> str:
         """Calibrate manipulator
 
         :param manipulator_id: ID of manipulator to calibrate
@@ -445,37 +435,31 @@
         """
 
     @abstractmethod
     def _bypass_calibration(self, manipulator_id: str) -> str:
         raise NotImplementedError
 
     @abstractmethod
-    def _set_can_write(
-        self,
-        manipulator_id: str,
-        can_write: bool,
-        hours: float,
-        sio: socketio.AsyncServer,
-    ) -> com.StateOutputData:
+    def _set_can_write(self, request: CanWriteRequest) -> BooleanStateResponse:
         raise NotImplementedError
 
     @abstractmethod
-    def _platform_space_to_unified_space(self, platform_position: list[float]) -> list[float]:
+    def _platform_space_to_unified_space(self, platform_position: Vector4) -> Vector4:
         """Convert position in platform space to position in unified manipulator space
 
         :param platform_position: Position in platform space (x, y, z, w) in mm
-        :type platform_position: list[float]
+        :type platform_position: Vector4
         :return: Position in unified manipulator space (x, y, z, w) in mm
-        :rtype: list[float]
+        :rtype: Vector4
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _unified_space_to_platform_space(self, unified_position: list[float]) -> list[float]:
+    def _unified_space_to_platform_space(self, unified_position: Vector4) -> Vector4:
         """Convert position in unified manipulator space to position in platform space
 
         :param unified_position: Position in unified manipulator space (x, y, z, w) in mm
-        :type unified_position: list[float]
+        :type unified_position: Vector4
         :return: Position in platform space (x, y, z, w) in mm
-        :rtype: list[float]
+        :rtype: Vector4
         """
         raise NotImplementedError
```

### Comparing `ephys_link-1.2.8/src/ephys_link/platform_manipulator.py` & `ephys_link-1.3.0b1/src/ephys_link/platform_manipulator.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/src/ephys_link/server.py` & `ephys_link-1.3.0b1/src/ephys_link/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 from signal import SIGINT, SIGTERM, signal
 from sys import exit
 from typing import TYPE_CHECKING, Any
 
 from aiohttp import web
 from aiohttp.web_runner import GracefulExit
 from packaging import version
+from pydantic import ValidationError
 from requests import get
 from requests.exceptions import ConnectionError
 from socketio import AsyncServer
+from vbl_aquarium.models.ephys_link import (
+    BooleanStateResponse,
+    CanWriteRequest,
+    DriveToDepthRequest,
+    DriveToDepthResponse,
+    GotoPositionRequest,
+    InsideBrainRequest,
+    PositionalResponse,
+)
 
 from ephys_link.__about__ import __version__
 from ephys_link.common import (
     ASCII,
-    CanWriteInputDataFormat,
-    DriveToDepthInputDataFormat,
-    DriveToDepthOutputData,
-    GotoPositionInputDataFormat,
-    InsideBrainInputDataFormat,
-    PositionalOutputData,
-    StateOutputData,
     dprint,
 )
 from ephys_link.platforms.new_scale_handler import NewScaleHandler
 from ephys_link.platforms.new_scale_pathfinder_handler import NewScalePathfinderHandler
 from ephys_link.platforms.sensapex_handler import SensapexHandler
 from ephys_link.platforms.ump3_handler import UMP3Handler
 
@@ -62,15 +65,15 @@
         # Register server exit handlers.
         signal(SIGTERM, self.close_server)
         signal(SIGINT, self.close_server)
 
         # Attach server to the web app.
         self.sio.attach(self.app)
 
-        # Declare events
+        # Declare events and assign handlers.
         self.sio.on("connect", self.connect)
         self.sio.on("disconnect", self.disconnect)
         self.sio.on("get_version", self.get_version)
         self.sio.on("get_manipulators", self.get_manipulators)
         self.sio.on("register_manipulator", self.register_manipulator)
         self.sio.on("unregister_manipulator", self.unregister_manipulator)
         self.sio.on("get_pos", self.get_pos)
@@ -133,20 +136,20 @@
         return __version__
 
     async def get_manipulators(self, _) -> str:
         """Get the list of discoverable manipulators.
 
         :param _: Socket session ID (unused).
         :type _: str
-        :return: :class:`ephys_link.common.GetManipulatorsOutputData` as JSON formatted string.
+        :return: :class:`vbl_aquarium.models.ephys_link.GetManipulatorsResponse` as JSON formatted string.
         :rtype: str
         """
         dprint("[EVENT]\t\t Get discoverable manipulators")
 
-        return self.platform.get_manipulators().json()
+        return self.platform.get_manipulators().to_string()
 
     async def register_manipulator(self, _, manipulator_id: str) -> str:
         """Register a manipulator with the server.
 
         :param _: Socket session ID (unused).
         :type _: str
         :param manipulator_id: ID of the manipulator to register.
@@ -175,122 +178,114 @@
     async def get_pos(self, _, manipulator_id: str) -> str:
         """Position of manipulator request.
 
         :param _: Socket session ID (unused).
         :type _: str
         :param manipulator_id: ID of manipulator to pull position from.
         :type manipulator_id: str
-        :return: :class:`ephys_link.common.PositionalOutputData` as JSON formatted string.
+        :return: :class:`vbl_aquarium.models.ephys_link.PositionalResponse` as JSON formatted string.
         :rtype: str
         """
         # dprint(f"[EVENT]\t\t Get position of manipulator" f" {manipulator_id}")
 
-        return self.platform.get_pos(manipulator_id).json()
+        return self.platform.get_pos(manipulator_id).to_string()
 
-    async def get_angles(self, _, manipulator_id: str):
+    async def get_angles(self, _, manipulator_id: str) -> str:
         """Angles of manipulator request.
 
         :param _: Socket session ID (unused).
         :type _: str
         :param manipulator_id: ID of manipulator to pull angles from.
         :type manipulator_id: str
-        :return: :class:`ephys_link.common.AngularOutputData` as JSON formatted string.
+        :return: :class:`vbl_aquarium.models.ephys_link.AngularResponse` as JSON formatted string.
         :rtype: str
         """
 
-        return self.platform.get_angles(manipulator_id).json()
+        return self.platform.get_angles(manipulator_id).to_string()
 
     async def get_shank_count(self, _, manipulator_id: str) -> str:
         """Number of shanks of manipulator request.
 
         :param _: Socket session ID (unused).
         :type _: str
         :param manipulator_id: ID of manipulator to pull number of shanks from.
         :type manipulator_id: str
-        :return: :class:`ephys_link.common.ShankCountOutputData` as JSON formatted string.
+        :return: :class:`vbl_aquarium.models.ephys_link.ShankCountResponse` as JSON formatted string.
         :rtype: str
         """
 
-        return self.platform.get_shank_count(manipulator_id).json()
+        return self.platform.get_shank_count(manipulator_id).to_string()
 
     async def goto_pos(self, _, data: str) -> str:
         """Move manipulator to position.
 
         :param _: Socket session ID (unused).
         :type _: str
-        :param data: :class:`ephys_link.common.GotoPositionInputDataFormat` as JSON formatted string.
+        :param data: :class:`vbl_aquarium.models.ephys_link.GotoPositionRequest` as JSON formatted string.
         :type data: str
-        :return: :class:`ephys_link.common.PositionalOutputData` as JSON formatted string.
+        :return: :class:`vbl_aquarium.models.ephys_link.PositionalResponse` as JSON formatted string.
         :rtype: str
         """
         try:
-            parsed_data: GotoPositionInputDataFormat = loads(data)
-            manipulator_id = parsed_data["manipulator_id"]
-            pos = parsed_data["pos"]
-            speed = parsed_data["speed"]
-        except KeyError:
-            print(f"[ERROR]\t\t Invalid goto_pos data: {data}\n")
-            return PositionalOutputData([], "Invalid data format").json()
+            request = GotoPositionRequest(**loads(data))
+        except ValidationError as ve:
+            print(f"[ERROR]\t\t Invalid goto_pos data: {data}\n{ve}\n")
+            return PositionalResponse(error="Invalid data format").to_string()
         except Exception as e:
             print(f"[ERROR]\t\t Error in goto_pos: {e}\n")
-            return PositionalOutputData([], "Error in goto_pos").json()
+            return PositionalResponse(error="Error in goto_pos").to_string()
         else:
-            dprint(f"[EVENT]\t\t Move manipulator {manipulator_id} " f"to position {pos}")
-            goto_result = await self.platform.goto_pos(manipulator_id, pos, speed)
-            return goto_result.json()
+            dprint(f"[EVENT]\t\t Move manipulator {request.manipulator_id} to position {request.position}")
+            goto_result = await self.platform.goto_pos(request)
+            return goto_result.to_string()
 
     async def drive_to_depth(self, _, data: str) -> str:
         """Drive to depth.
 
         :param _: Socket session ID (unused).
         :type _: str
-        :param data: :class:`ephys_link.common.DriveToDepthInputDataFormat` as JSON formatted string.
+        :param data: :class:`vbl_aquarium.models.ephys_link.DriveToDepthRequest` as JSON formatted string.
         :type data: str
-        :return: :class:`ephys_link.common.DriveToDepthOutputData` as JSON formatted string.
+        :return: :class:`vbl_aquarium.models.ephys_link.DriveToDepthResponse` as JSON formatted string.
         :rtype: str
         """
         try:
-            parsed_data: DriveToDepthInputDataFormat = loads(data)
-            manipulator_id = parsed_data["manipulator_id"]
-            depth = parsed_data["depth"]
-            speed = parsed_data["speed"]
+            request = DriveToDepthRequest(**loads(data))
         except KeyError:
             print(f"[ERROR]\t\t Invalid drive_to_depth data: {data}\n")
-            return DriveToDepthOutputData(-1, "Invalid data " "format").json()
+            return DriveToDepthResponse(error="Invalid data " "format").to_string()
         except Exception as e:
             print(f"[ERROR]\t\t Error in drive_to_depth: {e}\n")
-            return DriveToDepthOutputData(-1, "Error in drive_to_depth").json()
+            return DriveToDepthResponse(error="Error in drive_to_depth").to_string()
         else:
-            dprint(f"[EVENT]\t\t Drive manipulator {manipulator_id} to depth {depth}")
-            drive_result = await self.platform.drive_to_depth(manipulator_id, depth, speed)
-            return drive_result.json()
+            dprint(f"[EVENT]\t\t Drive manipulator {request.manipulator_id} to depth {request.depth}")
+            drive_result = await self.platform.drive_to_depth(request)
+            return drive_result.to_string()
 
     async def set_inside_brain(self, _, data: str) -> str:
         """Set the inside brain state.
 
         :param _: Socket session ID (unused).
         :type _: str
-        :param data: :class:`ephys_link.common.InsideBrainInputDataFormat` as JSON formatted string.
+        :param data: :class:`vbl_aquarium.models.ephys_link.InsideBrainRequest` as JSON formatted string.
         :type data: str
-        :return: :class:`ephys_link.common.StateOutputData` as JSON formatted string.
+        :return: :class:`vbl_aquarium.models.ephys_link.BooleanStateResponse` as JSON formatted string.
         :rtype: str
         """
         try:
-            parsed_data: InsideBrainInputDataFormat = loads(data)
-            manipulator_id = parsed_data["manipulator_id"]
-            inside = parsed_data["inside"]
+            request = InsideBrainRequest(**loads(data))
         except KeyError:
             print(f"[ERROR]\t\t Invalid set_inside_brain data: {data}\n")
-            return StateOutputData(False, "Invalid data format").json()
+            return BooleanStateResponse(error="Invalid data format").to_string()
         except Exception as e:
             print(f"[ERROR]\t\t Error in inside_brain: {e}\n")
-            return StateOutputData(False, "Error in set_inside_brain").json()
+            return BooleanStateResponse(error="Error in set_inside_brain").to_string()
         else:
-            dprint(f"[EVENT]\t\t Set manipulator {manipulator_id} inside brain to {inside}")
-            return self.platform.set_inside_brain(manipulator_id, inside).json()
+            dprint(f"[EVENT]\t\t Set manipulator {request.manipulator_id} inside brain to {request.inside}")
+            return self.platform.set_inside_brain(request).to_string()
 
     async def calibrate(self, _, manipulator_id: str) -> str:
         """Calibrate manipulator.
 
         :param _: Socket session ID (unused).
         :type _: str
         :param manipulator_id: ID of manipulator to calibrate.
@@ -317,33 +312,30 @@
         return self.platform.bypass_calibration(manipulator_id)
 
     async def set_can_write(self, _, data: str) -> str:
         """Set manipulator can_write state.
 
         :param _: Socket session ID (unused)
         :type _: str
-        :param data: :class:`ephys_link.common.CanWriteInputDataFormat` as JSON formatted string.
+        :param data: :class:`vbl_aquarium.models.ephys_link.CanWriteRequest` as JSON formatted string.
         :type data: str
-        :return: :class:`ephys_link.common.StateOutputData` as JSON formatted string.
+        :return: :class:`vbl_aquarium.models.ephys_link.BooleanStateResponse` as JSON formatted string.
         :rtype: str
         """
         try:
-            parsed_data: CanWriteInputDataFormat = loads(data)
-            manipulator_id = parsed_data["manipulator_id"]
-            can_write = parsed_data["can_write"]
-            hours = parsed_data["hours"]
+            request = CanWriteRequest(**loads(data))
         except KeyError:
             print(f"[ERROR]\t\t Invalid set_can_write data: {data}\n")
-            return StateOutputData(False, "Invalid data " "format").json()
+            return BooleanStateResponse(error="Invalid data format").to_string()
         except Exception as e:
             print(f"[ERROR]\t\t Error in inside_brain: {e}\n")
-            return StateOutputData(False, "Error in set_can_write").json()
+            return BooleanStateResponse(error="Error in set_can_write").to_string()
         else:
-            dprint(f"[EVENT]\t\t Set manipulator {manipulator_id} can_write state to {can_write}")
-            return self.platform.set_can_write(manipulator_id, can_write, hours, self.sio).json()
+            dprint(f"[EVENT]\t\t Set manipulator {request.manipulator_id} can_write state to {request.can_write}")
+            return self.platform.set_can_write(request).to_string()
 
     def stop(self, _) -> bool:
         """Stop all manipulators.
 
         :param _: Socket session ID (unused).
         :type _: str
         :return: True if successful, False otherwise.
@@ -422,15 +414,15 @@
         print("This is the Ephys Link server window.")
         print("You may safely leave it running in the background.")
         print("To stop the it, close this window or press CTRL + Pause/Break.")
         print()
 
         # List available manipulators
         print("Available Manipulators:")
-        print(self.platform.get_manipulators()["manipulators"])
+        print(self.platform.get_manipulators().manipulators)
         print()
 
         # Mark that server is running
         self.is_running = True
         web.run_app(self.app, port=server_port)
 
     def close_server(self, _, __) -> None:
```

### Comparing `ephys_link-1.2.8/src/ephys_link/platforms/new_scale_handler.py` & `ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,26 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 # noinspection PyUnresolvedReferences
 from NstMotorCtrl import NstCtrlHostIntf
+from vbl_aquarium.models.ephys_link import (
+    AngularResponse,
+    BooleanStateResponse,
+    CanWriteRequest,
+    DriveToDepthRequest,
+    DriveToDepthResponse,
+    GotoPositionRequest,
+    InsideBrainRequest,
+    PositionalResponse,
+    ShankCountResponse,
+)
+from vbl_aquarium.models.unity import Vector4
 
 from ephys_link import common as com
 from ephys_link.platform_handler import PlatformHandler
 from ephys_link.platforms.new_scale_manipulator import NewScaleManipulator
 
 if TYPE_CHECKING:
     import socketio
@@ -24,15 +36,15 @@
     """Handler for New Scale platform"""
 
     def __init__(self) -> None:
         """Initialize New Scale handler"""
         super().__init__()
 
         self.num_axes = 3
-        self.dimensions = [15, 15, 15]
+        self.dimensions = Vector4(x=15, y=15, z=15, w=0)
 
         self.ctrl = NstCtrlHostIntf()
 
         # Connect manipulators and initialize
         self.ctrl.ShowProperties()
         self.ctrl.Initialize()
 
@@ -63,73 +75,67 @@
             self.ctrl.GetAxis(first_axis_index + 1),
             self.ctrl.GetAxis(first_axis_index + 2),
         )
 
     def _unregister_manipulator(self, manipulator_id: str) -> None:
         del self.manipulators[manipulator_id]
 
-    def _get_pos(self, manipulator_id: str) -> com.PositionalOutputData:
+    def _get_pos(self, manipulator_id: str) -> PositionalResponse:
         return self.manipulators[manipulator_id].get_pos()
 
-    def _get_angles(self, manipulator_id: str) -> com.AngularOutputData:
+    def _get_angles(self, manipulator_id: str) -> AngularResponse:
         raise NotImplementedError
 
-    def _get_shank_count(self, manipulator_id: str) -> com.ShankCountOutputData:
+    def _get_shank_count(self, manipulator_id: str) -> ShankCountResponse:
         raise NotImplementedError
 
-    async def _goto_pos(self, manipulator_id: str, position: list[float], speed: int) -> com.PositionalOutputData:
-        return await self.manipulators[manipulator_id].goto_pos(position, speed)
+    async def _goto_pos(self, request: GotoPositionRequest) -> PositionalResponse:
+        return await self.manipulators[request.manipulator_id].goto_pos(request)
 
-    async def _drive_to_depth(self, manipulator_id: str, depth: float, speed: int) -> com.DriveToDepthOutputData:
-        return await self.manipulators[manipulator_id].drive_to_depth(depth, speed)
+    async def _drive_to_depth(self, request: DriveToDepthRequest) -> DriveToDepthResponse:
+        return await self.manipulators[request.manipulator_id].drive_to_depth(request)
 
-    def _set_inside_brain(self, manipulator_id: str, inside: bool) -> com.StateOutputData:
-        self.manipulators[manipulator_id].set_inside_brain(inside)
-        com.dprint(f"[SUCCESS]\t Set inside brain state for manipulator:" f" {manipulator_id}\n")
-        return com.StateOutputData(inside, "")
+    def _set_inside_brain(self, request: InsideBrainRequest) -> BooleanStateResponse:
+        self.manipulators[request.manipulator_id].set_inside_brain(request.inside)
+        com.dprint(f"[SUCCESS]\t Set inside brain state for manipulator: {request.manipulator_id}\n")
+        return BooleanStateResponse(state=request.inside)
 
     async def _calibrate(self, manipulator_id: str, sio: socketio.AsyncServer) -> str:
         return "" if self.manipulators[manipulator_id].calibrate() else "Error calling calibrate"
 
     def _bypass_calibration(self, manipulator_id: str) -> str:
         self.manipulators[manipulator_id].set_calibrated()
         com.dprint(f"[SUCCESS]\t Bypassed calibration for manipulator" f" {manipulator_id}\n")
         return ""
 
-    def _set_can_write(
-        self,
-        manipulator_id: str,
-        can_write: bool,
-        hours: float,
-        sio: socketio.AsyncServer,
-    ) -> com.StateOutputData:
-        self.manipulators[manipulator_id].set_can_write(can_write, hours, sio)
-        com.dprint(f"[SUCCESS]\t Set can_write state for manipulator" f" {manipulator_id}\n")
-        return com.StateOutputData(can_write, "")
+    def _set_can_write(self, request: CanWriteRequest) -> BooleanStateResponse:
+        self.manipulators[request.manipulator_id].set_can_write(request)
+        com.dprint(f"[SUCCESS]\t Set can_write state for manipulator {request.manipulator_id}\n")
+        return BooleanStateResponse(state=request.can_write)
 
-    def _platform_space_to_unified_space(self, platform_position: list[float]) -> list[float]:
+    def _platform_space_to_unified_space(self, platform_position: Vector4) -> Vector4:
         # unified   <-  platform
         # +x        <-  -x
         # +y        <-  +z
         # +z        <-  +y
         # +d        <-  -d
 
-        return [
-            self.dimensions[0] - platform_position[0],
-            platform_position[2],
-            platform_position[1],
-            self.dimensions[2] - platform_position[3],
-        ]
+        return Vector4(
+            x=self.dimensions.x - platform_position.x,
+            y=platform_position.z,
+            z=platform_position.y,
+            w=self.dimensions.z - platform_position.w,
+        )
 
-    def _unified_space_to_platform_space(self, unified_position: list[float]) -> list[float]:
+    def _unified_space_to_platform_space(self, unified_position: Vector4) -> Vector4:
         # platform  <-  unified
         # +x        <-  -x
         # +y        <-  +z
         # +z        <-  +y
         # +d        <-  -d
 
-        return [
-            self.dimensions[0] - unified_position[0],
-            unified_position[2],
-            unified_position[1],
-            self.dimensions[2] - unified_position[3],
-        ]
+        return Vector4(
+            x=self.dimensions.x - unified_position.x,
+            y=unified_position.z,
+            z=unified_position.y,
+            w=self.dimensions.z - unified_position.w,
+        )
```

### Comparing `ephys_link-1.2.8/src/ephys_link/platforms/new_scale_manipulator.py` & `ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_manipulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,33 @@
 
 from __future__ import annotations
 
 import asyncio
 import threading
 from typing import TYPE_CHECKING
 
+from vbl_aquarium.models.ephys_link import (
+    CanWriteRequest,
+    DriveToDepthRequest,
+    DriveToDepthResponse,
+    GotoPositionRequest,
+    PositionalResponse,
+)
+from vbl_aquarium.models.unity import Vector4
+
 import ephys_link.common as com
+from ephys_link.common import vector4_to_array
 from ephys_link.platform_manipulator import (
     HOURS_TO_SECONDS,
     MM_TO_UM,
     POSITION_POLL_DELAY,
     PlatformManipulator,
 )
 
 if TYPE_CHECKING:
-    import socketio
-
     # noinspection PyUnresolvedReferences
     from NstMotorCtrl import NstCtrlAxis
 
 # Constants
 ACCELERATION_MULTIPLIER = 5
 CUTOFF_MULTIPLIER = 0.005
 AT_TARGET_FLAG = 0x040000
@@ -61,182 +69,183 @@
         self._z.SetCL_Enable(True)
 
     def query_all_axes(self):
         """Query all axes for their position and status"""
         for axis in self._axes:
             axis.QueryPosStatus()
 
-    def get_pos(self) -> com.PositionalOutputData:
+    def get_pos(self) -> PositionalResponse:
         """Get the current position of the manipulator and convert it into mm.
 
         :return: Position of manipulator in (x, y, z, z) in mm (or an empty array on error) and error message (if any).
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
         self.query_all_axes()
 
         # Get position data and convert from µm to mm
         try:
-            position = [
-                self._x.CurPosition / MM_TO_UM,
-                self._y.CurPosition / MM_TO_UM,
-                self._z.CurPosition / MM_TO_UM,
-                self._z.CurPosition / MM_TO_UM,
-            ]
             # com.dprint(f"[SUCCESS]\t Got position of manipulator {self._id}\n")
-            return com.PositionalOutputData(position, "")
+            return PositionalResponse(
+                position=Vector4(
+                    x=self._x.CurPosition / MM_TO_UM,
+                    y=self._y.CurPosition / MM_TO_UM,
+                    z=self._z.CurPosition / MM_TO_UM,
+                    w=self._z.CurPosition / MM_TO_UM,
+                )
+            )
         except Exception as e:
             print(f"[ERROR]\t\t Getting position of manipulator {self._id}")
             print(f"{e}\n")
-            return com.PositionalOutputData([], "Error getting position")
+            return PositionalResponse(error="Error getting position")
 
-    async def goto_pos(self, position: list[float], speed: float) -> com.PositionalOutputData:
+    async def goto_pos(self, request: GotoPositionRequest) -> PositionalResponse:
         """Move manipulator to position.
 
-        :param position: The position to move to in mm.
-        :type position: list[float]
-        :param speed: The speed to move at (in mm/s).
-        :type speed: float
+        :param request: The goto request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.GotoPositionRequest`
         :return: Resulting position of manipulator in (x, y, z, z) in mm (or an empty array on error)
          and error message (if any).
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
         # Check if able to write
         if not self._can_write:
             print(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
-            return com.PositionalOutputData([], "Manipulator movement canceled")
+            return PositionalResponse(error="Manipulator movement canceled")
 
         # Stop current movement
         if self._is_moving:
             for axis in self._axes:
                 axis.Stop()
             self._is_moving = False
 
         try:
-            target_position_um = [axis * MM_TO_UM for axis in position]
+            target_position_um = request.position * MM_TO_UM
 
             # Restrict target position to just z-axis if inside brain
             if self._inside_brain:
-                z_axis = target_position_um[2]
-                target_position_um = self.get_pos()["position"]
-                target_position_um[2] = z_axis
+                z_axis = target_position_um.z
+                target_position_um = target_position_um.model_copy(
+                    update={**self.get_pos().position.model_dump(), "z": z_axis}
+                )
 
             # Mark movement as started
             self._is_moving = True
 
             # Send move command
-            speed_um = speed * MM_TO_UM
+            speed_um = request.speed * MM_TO_UM
             for i in range(3):
                 self._axes[i].SetCL_Speed(
                     speed_um,
                     speed_um * ACCELERATION_MULTIPLIER,
                     speed_um * CUTOFF_MULTIPLIER,
                 )
-                self._axes[i].MoveAbsolute(target_position_um[i])
+                self._axes[i].MoveAbsolute(vector4_to_array(target_position_um)[i])
 
             # Check and wait for completion (while able to write)
             self.query_all_axes()
             while (
                 not (self._x.CurStatus & AT_TARGET_FLAG)
                 or not (self._y.CurStatus & AT_TARGET_FLAG)
                 or not (self._z.CurStatus & AT_TARGET_FLAG)
             ) and self._can_write:
                 await asyncio.sleep(POSITION_POLL_DELAY)
                 self.query_all_axes()
 
             # Get position
-            manipulator_final_position = self.get_pos()["position"]
+            final_position = self.get_pos().position
 
             # Mark movement as finished
             self._is_moving = False
 
             # Return success unless write was disabled during movement (meaning a stop occurred)
             if not self._can_write:
                 com.dprint(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
-                return com.PositionalOutputData([], "Manipulator movement canceled")
+                return PositionalResponse(error="Manipulator movement canceled")
 
             # Return error if movement did not reach target.
-            if not all(abs(manipulator_final_position[i] - position[i]) < self._movement_tolerance for i in range(3)):
+            if not all(
+                abs(axis) < self._movement_tolerance for axis in vector4_to_array(final_position - request.position)[:3]
+            ):
                 com.dprint(f"[ERROR]\t\t Manipulator {self._id} did not reach target position.")
-                com.dprint(f"\t\t\t Expected: {position}, Got: {manipulator_final_position}")
-                return com.PositionalOutputData([], "Manipulator did not reach target position")
+                com.dprint(f"\t\t\t Expected: {request.position}, Got: {final_position}")
+                return PositionalResponse(error="Manipulator did not reach target position")
 
             # Made it to the target.
-            com.dprint(f"[SUCCESS]\t Moved manipulator {self._id} to position" f" {manipulator_final_position}\n")
-            return com.PositionalOutputData(manipulator_final_position, "")
+            com.dprint(f"[SUCCESS]\t Moved manipulator {self._id} to position" f" {final_position}\n")
+            return PositionalResponse(position=final_position)
         except Exception as e:
-            print(f"[ERROR]\t\t Moving manipulator {self._id} to position {position}")
+            print(f"[ERROR]\t\t Moving manipulator {self._id} to position {request.position}")
             print(f"{e}\n")
-            return com.PositionalOutputData([], "Error moving manipulator")
+            return PositionalResponse(error="Error moving manipulator")
 
-    async def drive_to_depth(self, depth: float, speed: float) -> com.DriveToDepthOutputData:
+    async def drive_to_depth(self, request: DriveToDepthRequest) -> DriveToDepthResponse:
         """Drive the manipulator to a certain depth.
 
-        :param depth: The depth to drive to in mm.
-        :type depth: float
-        :param speed: The speed to drive at in mm/s.
-        :type speed: float
+        :param request: The drive to depth request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.DriveToDepthRequest`
         :return: Resulting depth of manipulator in mm (or 0 on error) and error message (if any).
         :rtype: :class:`ephys_link.common.DriveToDepthOutputData`
         """
         # Check if able to write
         if not self._can_write:
-            print(f"[ERROR]\t\t Manipulator {self._id} movement " f"canceled")
-            return com.DriveToDepthOutputData(0, "Manipulator movement canceled")
+            print(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
+            return DriveToDepthResponse(error="Manipulator movement canceled")
 
         # Stop current movement
         if self._is_moving:
             for axis in self._axes:
                 axis.Stop()
             self._is_moving = False
 
         try:
-            target_depth_um = depth * MM_TO_UM
+            target_depth_um = request.depth * MM_TO_UM
 
             # Mark movement as started
             self._is_moving = True
 
             # Send move command to just z axis
-            speed_um = speed * MM_TO_UM
+            speed_um = request.speed * MM_TO_UM
             self._z.SetCL_Speed(
                 speed_um,
                 speed_um * ACCELERATION_MULTIPLIER,
                 speed_um * CUTOFF_MULTIPLIER,
             )
             self._z.MoveAbsolute(target_depth_um)
 
             # Check and wait for completion (while able to write)
             self._z.QueryPosStatus()
             while not (self._z.CurStatus & AT_TARGET_FLAG) and self._can_write:
                 await asyncio.sleep(0.1)
                 self._z.QueryPosStatus()
 
             # Get position
-            manipulator_final_position = self.get_pos()["position"]
+            final_depth = self.get_pos().position.w
 
             # Mark movement as finished
             self._is_moving = False
 
             # Return success unless write was disabled during movement (meaning a stop occurred)
             if not self._can_write:
                 com.dprint(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
-                return com.DriveToDepthOutputData(0, "Manipulator movement canceled")
+                return DriveToDepthResponse(error="Manipulator movement canceled")
 
             # Return error if movement did not reach target.
-            if not abs(manipulator_final_position[3] - depth) < self._movement_tolerance:
+            if not abs(final_depth - request.depth) < self._movement_tolerance:
                 com.dprint(f"[ERROR]\t\t Manipulator {self._id} did not reach target depth")
-                return com.DriveToDepthOutputData(0, "Manipulator did not reach target depth")
+                com.dprint(f"\t\t\t Expected: {request.depth}, Got: {final_depth}")
+                return DriveToDepthResponse(error="Manipulator did not reach target depth")
 
             # Made it to the target.
-            com.dprint(f"[SUCCESS]\t Moved manipulator {self._id} to position" f" {manipulator_final_position}\n")
-            return com.DriveToDepthOutputData(manipulator_final_position[3], "")
+            com.dprint(f"[SUCCESS]\t Moved manipulator {self._id} to position" f" {final_depth}\n")
+            return DriveToDepthResponse(depth=final_depth)
         except Exception as e:
-            print(f"[ERROR]\t\t Moving manipulator {self._id} to depth {depth}")
+            print(f"[ERROR]\t\t Moving manipulator {self._id} to depth {request.depth}")
             print(f"{e}\n")
             # Return 0 and error message on failure
-            return com.DriveToDepthOutputData(0, "Error driving manipulator")
+            return DriveToDepthResponse(error="Error driving manipulator")
 
     def calibrate(self) -> bool:
         """Calibrate the manipulator.
 
         :return: None
         """
         return self._x.CalibrateFrequency() and self._y.CalibrateFrequency() and self._z.CalibrateFrequency()
@@ -252,51 +261,41 @@
     def set_calibrated(self) -> None:
         """Set the manipulator to calibrated
 
         :return: None
         """
         self._calibrated = True
 
-    def set_can_write(self, can_write: bool, hours: float, sio: socketio.AsyncServer) -> None:
+    def set_can_write(self, request: CanWriteRequest) -> None:
         """Set if the manipulator can move.
 
-        :param can_write: True if the manipulator can move, False otherwise.
-        :type can_write: bool
-        :param hours: The number of hours to allow the manipulator to move (0 = forever).
-        :type hours: float
-        :param sio: SocketIO object from server to emit reset event.
-        :type sio: :class:`socketio.AsyncServer`
+        :param request: The can write request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.CanWriteRequest`
         :return: None
         """
-        self._can_write = can_write
+        self._can_write = request.can_write
 
-        if can_write and hours > 0:
+        if request.can_write and request.hours > 0:
             if self._reset_timer:
                 self._reset_timer.cancel()
-            self._reset_timer = threading.Timer(hours * HOURS_TO_SECONDS, self.reset_can_write, [sio])
+            self._reset_timer = threading.Timer(request.hours * HOURS_TO_SECONDS, self.reset_can_write)
             self._reset_timer.start()
 
+    def reset_can_write(self) -> None:
+        """Reset the :attr:`can_write` flag."""
+        self._can_write = False
+
     def get_can_write(self) -> bool:
         """Return if the manipulator can move.
 
         :return: True if the manipulator can move, False otherwise.
         :rtype: bool
         """
         return self._can_write
 
-    def reset_can_write(self, sio: socketio.AsyncServer) -> None:
-        """Reset the :attr:`can_write` flag.
-
-        :param sio: SocketIO object from server to emit reset event.
-        :type sio: :class:`socketio.AsyncServer`
-        :return: None
-        """
-        self._can_write = False
-        asyncio.run(sio.emit("write_disabled", self._id))
-
     def set_inside_brain(self, inside: bool) -> None:
         """Set if the manipulator is inside the brain.
 
         :param inside: True if the manipulator is inside the brain, False otherwise.
         :type inside: bool
         :return: None
         """
```

### Comparing `ephys_link-1.2.8/src/ephys_link/platforms/new_scale_pathfinder_handler.py` & `ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_pathfinder_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,27 @@
 
 import json
 from sys import exit
 from typing import TYPE_CHECKING
 from urllib import request
 from urllib.error import URLError
 
-from ephys_link import common as com
+from vbl_aquarium.models.ephys_link import (
+    AngularResponse,
+    BooleanStateResponse,
+    CanWriteRequest,
+    DriveToDepthRequest,
+    DriveToDepthResponse,
+    GotoPositionRequest,
+    InsideBrainRequest,
+    PositionalResponse,
+    ShankCountResponse,
+)
+from vbl_aquarium.models.unity import Vector3, Vector4
+
 from ephys_link.platform_handler import PlatformHandler
 
 if TYPE_CHECKING:
     import socketio
 
 
 class NewScalePathfinderHandler(PlatformHandler):
@@ -73,15 +85,15 @@
 
         :param port: Port of New Scale Pathfinder HTTP server
         :type port: int
         """
         super().__init__()
 
         self.num_axes = -1
-        self.dimensions = [15, 15, 15]
+        self.dimensions = Vector4(x=15, y=15, z=15, w=0)
 
         self.port = port
 
         # Test connection to New Scale HTTP server
         try:
             request.urlopen(f"http://localhost:{self.port}")
         except URLError:
@@ -158,77 +170,66 @@
             msg = f"Unable to find manipulator {manipulator_id}"
             raise ValueError(msg)
         self.manipulators[manipulator_id] = manipulator_index
 
     def _unregister_manipulator(self, manipulator_id: str) -> None:
         del self.manipulators[manipulator_id]
 
-    def _get_pos(self, manipulator_id: str) -> com.PositionalOutputData:
+    def _get_pos(self, manipulator_id: str) -> PositionalResponse:
         """Get the current position of the manipulator in mm
 
         :param manipulator_id: manipulator ID
         :return: Callback parameters (position in (x, y, z, w) (or an empty array on
             error) in mm, error message)
         """
         manipulator_data = self.query_manipulator_data(manipulator_id)
 
-        return com.PositionalOutputData(
-            [
-                manipulator_data["Tip_X_ML"],
-                manipulator_data["Tip_Y_AP"],
-                manipulator_data["Tip_Z_DV"],
-                0,
-            ],
-            "",
+        return PositionalResponse(
+            position=Vector4(
+                x=manipulator_data["Tip_X_ML"], y=manipulator_data["Tip_Y_AP"], z=manipulator_data["Tip_Z_DV"], w=0
+            )
         )
 
-    def _get_angles(self, manipulator_id: str) -> com.AngularOutputData:
+    def _get_angles(self, manipulator_id: str) -> AngularResponse:
         manipulator_data = self.query_manipulator_data(manipulator_id)
 
         # Apply PosteriorAngle to Polar to get the correct angle.
         adjusted_polar = manipulator_data["Polar"] - self.query_data()["PosteriorAngle"]
 
-        return com.AngularOutputData(
-            [
-                adjusted_polar if adjusted_polar > 0 else 360 + adjusted_polar,
-                manipulator_data["Pitch"],
-                manipulator_data.get("ShankOrientation", 0),
-            ],
-            "",
+        return AngularResponse(
+            angles=Vector3(
+                x=adjusted_polar if adjusted_polar > 0 else 360 + adjusted_polar,
+                y=manipulator_data["Pitch"],
+                z=manipulator_data.get("ShankOrientation", 0),
+            )
         )
 
-    def _get_shank_count(self, manipulator_id: str) -> com.ShankCountOutputData:
+    def _get_shank_count(self, manipulator_id: str) -> ShankCountResponse:
         for probe in self.query_data()["ProbeArray"]:
             if probe["Id"] == manipulator_id:
-                return com.ShankCountOutputData(probe.get("ShankCount", 1), "")
+                return ShankCountResponse(shank_count=probe.get("ShankCount", 1))
 
-        return com.ShankCountOutputData(-1, "Unable to find manipulator")
+        return ShankCountResponse(error="Unable to find manipulator")
 
-    async def _goto_pos(self, manipulator_id: str, position: list[float], speed: int) -> com.PositionalOutputData:
+    async def _goto_pos(self, _: GotoPositionRequest) -> PositionalResponse:
         raise NotImplementedError
 
-    async def _drive_to_depth(self, manipulator_id: str, depth: float, speed: int) -> com.DriveToDepthOutputData:
+    async def _drive_to_depth(self, _: DriveToDepthRequest) -> DriveToDepthResponse:
         raise NotImplementedError
 
-    def _set_inside_brain(self, manipulator_id: str, inside: bool) -> com.StateOutputData:
+    def _set_inside_brain(self, _: InsideBrainRequest) -> BooleanStateResponse:
         raise NotImplementedError
 
     async def _calibrate(self, manipulator_id: str, sio: socketio.AsyncServer) -> str:
         raise NotImplementedError
 
     def _bypass_calibration(self, manipulator_id: str) -> str:
         return ""
 
-    def _set_can_write(
-        self,
-        manipulator_id: str,
-        can_write: bool,
-        hours: float,
-        sio: socketio.AsyncServer,
-    ) -> com.StateOutputData:
+    def _set_can_write(self, _: CanWriteRequest) -> BooleanStateResponse:
         raise NotImplementedError
 
     def _unified_space_to_platform_space(self, unified_position: list[float]) -> list[float]:
         raise NotImplementedError
 
     def _platform_space_to_unified_space(self, platform_position: list[float]) -> list[float]:
         raise NotImplementedError
```

### Comparing `ephys_link-1.2.8/src/ephys_link/platforms/sensapex_manipulator.py` & `ephys_link-1.3.0b1/src/ephys_link/platforms/sensapex_manipulator.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,32 @@
 
 from __future__ import annotations
 
 import asyncio
 import threading
 from typing import TYPE_CHECKING
 
-import ephys_link.common as com
+from vbl_aquarium.models.ephys_link import (
+    CanWriteRequest,
+    DriveToDepthRequest,
+    DriveToDepthResponse,
+    GotoPositionRequest,
+    PositionalResponse,
+)
+from vbl_aquarium.models.unity import Vector4
+
+from ephys_link.common import dprint, vector4_to_array
 from ephys_link.platform_manipulator import (
     HOURS_TO_SECONDS,
     MM_TO_UM,
     POSITION_POLL_DELAY,
     PlatformManipulator,
 )
 
 if TYPE_CHECKING:
-    import socketio
     from sensapex import SensapexDevice
 
 
 class SensapexManipulator(PlatformManipulator):
     """Representation of a single Sensapex manipulator
 
     :param device: A Sensapex device
@@ -37,117 +45,114 @@
         :param device: A Sensapex device
         """
         super().__init__()
         self._device = device
         self._id = device.dev_id
 
     # Device functions
-    def get_pos(self) -> com.PositionalOutputData:
+    def get_pos(self) -> PositionalResponse:
         """Get the current position of the manipulator and convert it into mm.
 
         :return: Position in (x, y, z, w) (or an empty array on error) in mm and error message (if any).
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
         try:
-            position = [axis / MM_TO_UM for axis in self._device.get_pos(1)]
             # com.dprint(f"[SUCCESS]\t Got position of manipulator {self._id}\n")
-            return com.PositionalOutputData(position, "")
+            return PositionalResponse(
+                position=Vector4(
+                    **dict(zip(Vector4.model_fields.keys(), [axis / MM_TO_UM for axis in self._device.get_pos(1)]))
+                )
+            )
         except Exception as e:
             print(f"[ERROR]\t\t Getting position of manipulator {self._id}")
             print(f"{e}\n")
-            return com.PositionalOutputData([], "Error getting position")
+            return PositionalResponse(error="Error getting position")
 
-    async def goto_pos(self, position: list[float], speed: float) -> com.PositionalOutputData:
+    async def goto_pos(self, request: GotoPositionRequest) -> PositionalResponse:
         """Move manipulator to position.
 
-        :param position: The position to move to in mm
-        :type position: list[float]
-        :param speed: The speed to move at (in mm/s)
-        :type speed: float
+        :param request: The goto request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.GotoPositionRequest`
         :return: Resulting position in (x, y, z, w) (or an empty array on error) in mm and error message (if any).
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
         # Check if able to write
         if not self._can_write:
             print(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
-            return com.PositionalOutputData([], "Manipulator movement canceled")
+            return PositionalResponse(error="Manipulator movement canceled")
 
         # Stop current movement
         if self._is_moving:
             self._device.stop()
             self._is_moving = False
 
         try:
-            target_position_um = [axis * MM_TO_UM for axis in position]
+            target_position_um = request.position * MM_TO_UM
 
             # Restrict target position to just depth-axis if inside brain
             if self._inside_brain:
-                d_axis = target_position_um[3]
-                target_position_um = self._device.get_pos()
-                target_position_um[3] = d_axis
+                d_axis = target_position_um.w
+                target_position_um = target_position_um.model_copy(
+                    update={**self.get_pos().position.model_dump(), "w": d_axis}
+                )
 
             # Mark movement as started
             self._is_moving = True
 
             # Send move command
-            movement = self._device.goto_pos(target_position_um, speed * MM_TO_UM)
+            movement = self._device.goto_pos(
+                vector4_to_array(target_position_um),
+                request.speed * MM_TO_UM,
+            )
 
             # Wait for movement to finish
             while not movement.finished:
                 await asyncio.sleep(POSITION_POLL_DELAY)
 
             # Get position
-            manipulator_final_position = self.get_pos()["position"]
+            final_position = self.get_pos().position
 
             # Mark movement as finished.
             self._is_moving = False
 
             # Return success unless write was disabled during movement (meaning a stop occurred).
             if not self._can_write:
-                com.dprint(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
-                return com.PositionalOutputData([], "Manipulator movement canceled")
+                dprint(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
+                return PositionalResponse(error="Manipulator movement canceled")
 
             # Return error if movement did not reach target.
             if not all(
-                abs(manipulator_final_position[i] - position[i]) < self._movement_tolerance
-                for i in range(len(position))
+                abs(axis) < self._movement_tolerance for axis in vector4_to_array(final_position - request.position)
             ):
-                com.dprint(f"[ERROR]\t\t Manipulator {self._id} did not reach target position")
-                return com.PositionalOutputData([], "Manipulator did not reach target position")
+                dprint(f"[ERROR]\t\t Manipulator {self._id} did not reach target position")
+                dprint(f"\t\t\t Expected: {request.position}, Got: {final_position}")
+                return PositionalResponse(error="Manipulator did not reach target position")
 
             # Made it to the target.
-            com.dprint(f"[SUCCESS]\t Moved manipulator {self._id} to position {manipulator_final_position}\n")
-            return com.PositionalOutputData(manipulator_final_position, "")
+            dprint(f"[SUCCESS]\t Moved manipulator {self._id} to position {final_position}\n")
+            return PositionalResponse(position=final_position)
         except Exception as e:
-            print(f"[ERROR]\t\t Moving manipulator {self._id} to position" f" {position}")
+            print(f"[ERROR]\t\t Moving manipulator {self._id} to position {request.position}")
             print(f"{e}\n")
-            return com.PositionalOutputData([], "Error moving manipulator")
+            return PositionalResponse(error="Error moving manipulator")
 
-    async def drive_to_depth(self, depth: float, speed: float) -> com.DriveToDepthOutputData:
+    async def drive_to_depth(self, request: DriveToDepthRequest) -> DriveToDepthResponse:
         """Drive the manipulator to a certain depth.
 
-        :param depth: The depth to drive to in mm.
-        :type depth: float
-        :param speed: The speed to drive at in mm/s
-        :type speed: float
+        :param request: The drive to depth request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.DriveToDepthRequest`
         :return: Resulting depth in mm (or 0 on error) and error message (if any).
         :rtype: :class:`ephys_link.common.DriveToDepthOutputData`
         """
         # Get position before this movement
-        target_pos = self.get_pos()["position"]
-
-        target_pos[3] = depth
-        movement_result = await self.goto_pos(target_pos, speed)
-
-        if movement_result["error"] == "":
-            # Return depth on success
-            return com.DriveToDepthOutputData(movement_result["position"][3], "")
+        target_pos = self.get_pos().position
 
-        # Return 0 and error message on failure
-        return com.DriveToDepthOutputData(0, movement_result["error"])
+        target_pos = target_pos.model_copy(update={"w": request.depth})
+        movement_result = await self.goto_pos(GotoPositionRequest(**request.model_dump(), position=target_pos))
+        return DriveToDepthResponse(depth=movement_result.position.w, error=movement_result.error)
 
     def set_inside_brain(self, inside: bool) -> None:
         """Set if the manipulator is inside the brain.
 
         Used to signal that the brain should move at :const:`INSIDE_BRAIN_SPEED_LIMIT`
 
         :param inside: True if the manipulator is inside the brain, False otherwise.
@@ -160,42 +165,32 @@
         """Return if the manipulator can move.
 
         :return: True if the manipulator can move, False otherwise.
         :rtype: bool
         """
         return self._can_write
 
-    def set_can_write(self, can_write: bool, hours: float, sio: socketio.AsyncServer) -> None:
+    def set_can_write(self, request: CanWriteRequest) -> None:
         """Set if the manipulator can move.
 
-        :param can_write: True if the manipulator can move, False otherwise.
-        :type can_write: bool
-        :param hours: The number of hours to allow the manipulator to move (0 = forever).
-        :type hours: float
-        :param sio: SocketIO object from server to emit reset event.
-        :type sio: :class:`socketio.AsyncServer`
+        :param request: The can write request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.CanWriteRequest`
         :return: None
         """
-        self._can_write = can_write
+        self._can_write = request.can_write
 
-        if can_write and hours > 0:
+        if request.can_write and request.hours > 0:
             if self._reset_timer:
                 self._reset_timer.cancel()
-            self._reset_timer = threading.Timer(hours * HOURS_TO_SECONDS, self.reset_can_write, [sio])
+            self._reset_timer = threading.Timer(request.hours * HOURS_TO_SECONDS, self.reset_can_write)
             self._reset_timer.start()
 
-    def reset_can_write(self, sio: socketio.AsyncServer) -> None:
-        """Reset the :attr:`can_write` flag.
-
-        :param sio: SocketIO object from server to emit reset event.
-        :type sio: :class:`socketio.AsyncServer`
-        :return: None
-        """
+    def reset_can_write(self) -> None:
+        """Reset the :attr:`can_write` flag."""
         self._can_write = False
-        asyncio.run(sio.emit("write_disabled", self._id))
 
     # Calibration
     def call_calibrate(self) -> None:
         """Calibrate the manipulator.
 
         :return: None
         """
@@ -219,8 +214,8 @@
     def stop(self) -> None:
         """Stop the manipulator
 
         :return: None
         """
         self._can_write = False
         self._device.stop()
-        com.dprint(f"[SUCCESS]\t Stopped manipulator {self._id}")
+        dprint(f"[SUCCESS]\t Stopped manipulator {self._id}")
```

### Comparing `ephys_link-1.2.8/src/ephys_link/platforms/ump3_handler.py` & `ephys_link-1.3.0b1/src/ephys_link/platforms/ump3_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 and extends it to support the uMp-3 manipulator.
 
 This is a subclass of :class:`ephys_link.platforms.sensapex_handler`.
 """
 
 from __future__ import annotations
 
+from vbl_aquarium.models.unity import Vector4
+
 from ephys_link.platforms.sensapex_handler import SensapexHandler
 from ephys_link.platforms.ump3_manipulator import UMP3Manipulator
 
 
 class UMP3Handler(SensapexHandler):
     def __init__(self):
         super().__init__()
 
         self.num_axes = 3
-        self.dimensions = [20, 20, 20]
+        self.dimensions = Vector4(x=20, y=20, z=20, w=0)
 
     def _register_manipulator(self, manipulator_id: str) -> None:
         if not manipulator_id.isnumeric():
             msg = "Manipulator ID must be numeric"
             raise ValueError(msg)
 
         self.manipulators[manipulator_id] = UMP3Manipulator(self.ump.get_device(int(manipulator_id)))
```

### Comparing `ephys_link-1.2.8/src/ephys_link/platforms/ump3_manipulator.py` & `ephys_link-1.3.0b1/src/ephys_link/platforms/ump3_manipulator.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 """
 
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING
 
-import ephys_link.common as com
+from vbl_aquarium.models.ephys_link import (
+    DriveToDepthRequest,
+    DriveToDepthResponse,
+    GotoPositionRequest,
+    PositionalResponse,
+)
+from vbl_aquarium.models.unity import Vector4
+
+from ephys_link.common import dprint, vector4_to_array
 from ephys_link.platform_manipulator import (
     MM_TO_UM,
     POSITION_POLL_DELAY,
 )
 from ephys_link.platforms.sensapex_manipulator import SensapexManipulator
 
 if TYPE_CHECKING:
@@ -30,114 +38,108 @@
         """Construct a new Manipulator object
 
         :param device: A Sensapex device
         """
         super().__init__(device)
 
     # Device functions
-    def get_pos(self) -> com.PositionalOutputData:
+    def get_pos(self) -> PositionalResponse:
         """Get the current position of the manipulator and convert it into mm.
 
         :return: Position in (x, y, z, x) (or an empty array on error) in mm and error message (if any).
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
         try:
             position = [axis / MM_TO_UM for axis in self._device.get_pos(1)]
 
-            # Duplicate x-axis for depth axis
+            # Add the depth axis to the end of the position.
             position.append(position[0])
 
             # com.dprint(f"[SUCCESS]\t Got position of manipulator {self._id}\n")
-            return com.PositionalOutputData(position, "")
+            return PositionalResponse(position=Vector4(**dict(zip(Vector4.model_fields.keys(), position))))
         except Exception as e:
             print(f"[ERROR]\t\t Getting position of manipulator {self._id}")
             print(f"{e}\n")
-            return com.PositionalOutputData([], "Error getting position")
+            return PositionalResponse(error="Error getting position")
 
-    async def goto_pos(self, position: list[float], speed: float) -> com.PositionalOutputData:
+    async def goto_pos(self, request: GotoPositionRequest) -> PositionalResponse:
         """Move manipulator to position.
 
-        :param position: The position to move to in mm.
-        :type position: list[float]
-        :param speed: The speed to move at (in mm/s).
-        :type speed: float
+        :param request: The goto request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.GotoPositionRequest`
         :return: Resulting position in (x, y, z, x) (or an empty array on error) in mm and error message (if any).
         :rtype: :class:`ephys_link.common.PositionalOutputData`
         """
         # Check if able to write
         if not self._can_write:
             print(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
-            return com.PositionalOutputData([], "Manipulator movement canceled")
+            return PositionalResponse(error="Manipulator movement canceled")
 
         # Stop current movement
         if self._is_moving:
             self._device.stop()
             self._is_moving = False
 
         try:
-            target_position_um = [axis * MM_TO_UM for axis in position[:3]]
+            target_position_um = request.position * MM_TO_UM
 
             # Restrict target position to just depth-axis if inside brain
             if self._inside_brain:
-                d_axis = target_position_um[0]
-                target_position_um = self._device.get_pos()
-                target_position_um[0] = d_axis
+                d_axis = target_position_um.x
+                target_position_um = target_position_um.model_copy(
+                    update={**self.get_pos().position.model_dump(), "x": d_axis}
+                )
 
             # Mark movement as started
             self._is_moving = True
 
             # Send move command
-            movement = self._device.goto_pos(target_position_um, speed * MM_TO_UM)
+            movement = self._device.goto_pos(
+                vector4_to_array(target_position_um),
+                request.speed * MM_TO_UM,
+            )
 
             # Wait for movement to finish
             while not movement.finished:
                 await asyncio.sleep(POSITION_POLL_DELAY)
 
             # Get position
-            manipulator_final_position = self.get_pos()["position"]
+            final_position = self.get_pos().position
 
             # Mark movement as finished
             self._is_moving = False
 
             # Return success unless write was disabled during movement (meaning a stop occurred)
             if not self._can_write:
-                com.dprint(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
-                return com.PositionalOutputData([], "Manipulator movement canceled")
+                dprint(f"[ERROR]\t\t Manipulator {self._id} movement canceled")
+                return PositionalResponse(error="Manipulator movement canceled")
 
             # Return error if movement did not reach target.
             if not all(
-                abs(manipulator_final_position[i] - position[i]) < self._movement_tolerance
-                for i in range(len(position))
+                abs(axis) < self._movement_tolerance for axis in vector4_to_array(final_position - request.position)
             ):
-                com.dprint(f"[ERROR]\t\t Manipulator {self._id} did not reach target position")
-                return com.PositionalOutputData([], "Manipulator did not reach target position")
+                dprint(f"[ERROR]\t\t Manipulator {self._id} did not reach target position")
+                dprint(f"\t\t\t Expected: {request.position}, Got: {final_position}")
+                return PositionalResponse(error="Manipulator did not reach target position")
 
             # Made it to the target.
-            com.dprint(f"[SUCCESS]\t Moved manipulator {self._id} to position" f" {manipulator_final_position}\n")
-            return com.PositionalOutputData(manipulator_final_position, "")
+            dprint(f"[SUCCESS]\t Moved manipulator {self._id} to position" f" {final_position}\n")
+            return PositionalResponse(position=final_position)
         except Exception as e:
-            print(f"[ERROR]\t\t Moving manipulator {self._id} to position" f" {position}")
+            print(f"[ERROR]\t\t Moving manipulator {self._id} to position {request.position}")
             print(f"{e}\n")
-            return com.PositionalOutputData([], "Error moving manipulator")
+            return PositionalResponse(error="Error moving manipulator")
 
-    async def drive_to_depth(self, depth: float, speed: float) -> com.DriveToDepthOutputData:
+    async def drive_to_depth(self, request: DriveToDepthRequest) -> DriveToDepthResponse:
         """Drive the manipulator to a certain depth.
 
-        :param depth: The depth to drive to in mm.
-        :type depth: float
-        :param speed: The speed to drive at in mm/s.
-        :type speed: float
+        :param request: The drive to depth request parsed from the server.
+        :type request: :class:`vbl_aquarium.models.ephys_link.DriveToDepthRequest`
         :return: Resulting depth in mm (or 0 on error) and error message (if any).
         :rtype: :class:`ephys_link.common.DriveToDepthOutputData`
         """
         # Get position before this movement
-        target_pos = self.get_pos()["position"]
-
-        target_pos[0] = depth
-        movement_result = await self.goto_pos(target_pos, speed)
-
-        if movement_result["error"] == "":
-            # Return depth on success
-            return com.DriveToDepthOutputData(movement_result["position"][3], "")
+        target_pos = self.get_pos().position
 
-        # Return 0 and error message on failure
-        return com.DriveToDepthOutputData(0, "Error driving " "manipulator")
+        target_pos = target_pos.model_copy(update={"x": request.depth})
+        movement_result = await self.goto_pos(GotoPositionRequest(**request.model_dump(), position=target_pos))
+        return DriveToDepthResponse(depth=movement_result.position.w, error=movement_result.error)
```

### Comparing `ephys_link-1.2.8/src/ephys_link/resources/CP210xManufacturing.dll` & `ephys_link-1.3.0b1/src/ephys_link/resources/CP210xManufacturing.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/src/ephys_link/resources/NstMotorCtrl.dll` & `ephys_link-1.3.0b1/src/ephys_link/resources/NstMotorCtrl.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/src/ephys_link/resources/SiUSBXp.dll` & `ephys_link-1.3.0b1/src/ephys_link/resources/SiUSBXp.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/src/ephys_link/resources/libum.dll` & `ephys_link-1.3.0b1/src/ephys_link/resources/libum.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/.gitignore` & `ephys_link-1.3.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/LICENSE` & `ephys_link-1.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/README.md` & `ephys_link-1.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `ephys_link-1.2.8/pyproject.toml` & `ephys_link-1.3.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,29 +19,29 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent",
+    "Operating System :: Microsoft :: Windows",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
 ]
 dependencies = [
     "aiohttp==3.9.3",
     "platformdirs==4.2.0",
     "pyserial==3.5",
-    "python-socketio==5.11.1",
+    "python-socketio==5.11.2",
     "pythonnet==3.0.3",
     "requests==2.31.0",
-    "wheel==0.42.0",
     "sensapex==1.400.0",
+    "vbl-aquarium==0.0.12"
 ]
 
 [project.urls]
 Documentation = "https://virtualbrainlab.org/ephys_link/installation_and_use.html"
 Issues = "https://github.com/VirtualBrainLab/ephys-link/issues"
 Source = "https://github.com/VirtualBrainLab/ephys-link"
```

### Comparing `ephys_link-1.2.8/PKG-INFO` & `ephys_link-1.3.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ephys-link
-Version: 1.2.8
+Version: 1.3.0b1
 Summary: A Python Socket.IO server that allows any Socket.IO-compliant application to communicate with manipulators used in electrophysiology experiments.
 Project-URL: Documentation, https://virtualbrainlab.org/ephys_link/installation_and_use.html
 Project-URL: Issues, https://github.com/VirtualBrainLab/ephys-link/issues
 Project-URL: Source, https://github.com/VirtualBrainLab/ephys-link
 Author-email: Kenneth Yang <kjy5@uw.edu>
 Maintainer-email: Kenneth Yang <kjy5@uw.edu>
 License-Expression: GPL-3.0-only
 License-File: LICENSE
 Keywords: electrophysiology,ephys,manipulator,neuroscience,neurotech,new-scale,sensapex,socket-io,virtualbrainlab
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: <3.13,>=3.8
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: platformdirs==4.2.0
 Requires-Dist: pyserial==3.5
-Requires-Dist: python-socketio==5.11.1
+Requires-Dist: python-socketio==5.11.2
 Requires-Dist: pythonnet==3.0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: sensapex==1.400.0
-Requires-Dist: wheel==0.42.0
+Requires-Dist: vbl-aquarium==0.0.12
 Description-Content-Type: text/markdown
 
 # Electrophysiology Manipulator Link
 
 [![PyPI version](https://badge.fury.io/py/ephys-link.svg)](https://badge.fury.io/py/ephys-link)
 [![CodeQL](https://github.com/VirtualBrainLab/ephys-link/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/VirtualBrainLab/ephys-link/actions/workflows/codeql-analysis.yml)
 [![Dependency Review](https://github.com/VirtualBrainLab/ephys-link/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/VirtualBrainLab/ephys-link/actions/workflows/dependency-review.yml)
```

