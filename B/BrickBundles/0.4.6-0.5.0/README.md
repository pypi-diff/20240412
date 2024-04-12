# Comparing `tmp/brickbundles-0.4.6-py3-none-any.whl.zip` & `tmp/brickbundles-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 105758 bytes, number of entries: 271
+Zip file size: 107724 bytes, number of entries: 274
 -rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Actuator.brick
+-rw-r--r--  2.0 unx      742 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Differential.brick
 -rw-r--r--  2.0 unx      675 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Engine.brick
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Gear.brick
 -rw-r--r--  2.0 unx      112 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/HingeActuator.brick
 -rw-r--r--  2.0 unx      281 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/PrismaticActuator.brick
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Shaft.brick
--rw-r--r--  2.0 unx      152 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/GearTorqueOutput.brick
--rw-r--r--  2.0 unx      122 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueMotorInput.brick
+-rw-r--r--  2.0 unx      201 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/GearTorqueOutput.brick
+-rw-r--r--  2.0 unx      128 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueMotorInput.brick
+-rw-r--r--  2.0 unx     1193 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/TorqueLimitedSlipDifferential.brick
 -rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/TorqueMotor.brick
 -rw-r--r--  2.0 unx      112 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/config.brick
 -rw-r--r--  2.0 unx      420 b- defN 80-Jan-01 00:00 brickbundles/Math/AffineTransform.brick
 -rw-r--r--  2.0 unx      141 b- defN 80-Jan-01 00:00 brickbundles/Math/Constants.brick
 -rw-r--r--  2.0 unx      285 b- defN 80-Jan-01 00:00 brickbundles/Math/Functions.brick
 -rw-r--r--  2.0 unx       99 b- defN 80-Jan-01 00:00 brickbundles/Math/Line.brick
 -rw-r--r--  2.0 unx      975 b- defN 80-Jan-01 00:00 brickbundles/Math/Matrix3x3.brick
@@ -55,17 +57,18 @@
 -rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 brickbundles/Physics/Interactions/Slack/ConstantDistanceSlack.brick
 -rw-r--r--  2.0 unx      861 b- defN 80-Jan-01 00:00 brickbundles/Physics/Interactions/Slack/DefaultSlack.brick
 -rw-r--r--  2.0 unx      834 b- defN 80-Jan-01 00:00 brickbundles/Physics/Interactions/SurfaceContact/Model.brick
 -rw-r--r--  2.0 unx      419 b- defN 80-Jan-01 00:00 brickbundles/Physics/Interactions/SurfaceContact/PatchElasticity.brick
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 brickbundles/Physics/Interactions/SurfaceContact/PointwiseElasticity.brick
 -rw-r--r--  2.0 unx      403 b- defN 80-Jan-01 00:00 brickbundles/Physics/KinematicLock.brick
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/BoolInputSignal.brick
--rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/Input.brick
+-rw-r--r--  2.0 unx      495 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/Input.brick
+-rw-r--r--  2.0 unx      265 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/InputOutputType.brick
 -rw-r--r--  2.0 unx       33 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/InputSignal.brick
--rw-r--r--  2.0 unx        7 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/Output.brick
+-rw-r--r--  2.0 unx      278 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/Output.brick
 -rw-r--r--  2.0 unx       35 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/OutputSignal.brick
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/RealInputSignal.brick
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/RealOutputSignal.brick
 -rw-r--r--  2.0 unx     1489 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/Value.brick
 -rw-r--r--  2.0 unx     1714 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/ValueOutputSignal.brick
 -rw-r--r--  2.0 unx      131 b- defN 80-Jan-01 00:00 brickbundles/Physics/Signals/Vec3OutputSignal.brick
 -rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 brickbundles/Physics/System.brick
@@ -79,18 +82,18 @@
 -rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Bodies/RotationalKinematics.brick
 -rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Charges/LinearConnector.brick
 -rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Charges/MateConnector.brick
 -rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Charges/RotationalConnector.brick
 -rw-r--r--  2.0 unx       96 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Interactions/Mate.brick
 -rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Interactions/RotationalVelocityMotor.brick
 -rw-r--r--  2.0 unx      141 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Interactions/VelocityMotor.brick
--rw-r--r--  2.0 unx      182 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Signals/RotationalBodyAngleOutput.brick
--rw-r--r--  2.0 unx      204 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Signals/RotationalBodyAngularVelocityOutput.brick
--rw-r--r--  2.0 unx      125 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Signals/RotationalVelocityMotor1DTorqueOutput.brick
--rw-r--r--  2.0 unx      290 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Signals/RotationalVelocityMotor1DVelocityInput.brick
+-rw-r--r--  2.0 unx      229 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Signals/RotationalBodyAngleOutput.brick
+-rw-r--r--  2.0 unx      261 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Signals/RotationalBodyAngularVelocityOutput.brick
+-rw-r--r--  2.0 unx      174 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Signals/RotationalVelocityMotor1DTorqueOutput.brick
+-rw-r--r--  2.0 unx      296 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/Signals/RotationalVelocityMotor1DVelocityInput.brick
 -rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 brickbundles/Physics1D/config.brick
 -rw-r--r--  2.0 unx       78 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Bodies/Body.brick
 -rw-r--r--  2.0 unx      526 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Bodies/Inertia.brick
 -rw-r--r--  2.0 unx      196 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Bodies/Kinematics.brick
 -rw-r--r--  2.0 unx      138 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Bodies/RigidBody.brick
 -rw-r--r--  2.0 unx      161 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Bodies/RigidBodyKinematics.brick
 -rw-r--r--  2.0 unx      748 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Charges/AdaptiveMateConnector.brick
@@ -163,25 +166,25 @@
 -rw-r--r--  2.0 unx      443 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/SpringInteraction1DOF.brick
 -rw-r--r--  2.0 unx      512 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/SurfaceContact/PatchElasticityDryFrictionModel.brick
 -rw-r--r--  2.0 unx      818 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/SurfaceContact/PointwiseElasticityDryFrictionModel.brick
 -rw-r--r--  2.0 unx      266 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/TorqueMotor.brick
 -rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/TorsionSpring.brick
 -rw-r--r--  2.0 unx     1226 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Interactions/VelocityMotor.brick
 -rw-r--r--  2.0 unx      557 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/RelativeTransform.brick
--rw-r--r--  2.0 unx      181 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/HingeAngleOutput.brick
--rw-r--r--  2.0 unx      218 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/HingeAngularVelocityOutput.brick
--rw-r--r--  2.0 unx      282 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/LinearVelocityMotorVelocityInput.brick
--rw-r--r--  2.0 unx      228 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/PrismaticPositionOutput.brick
--rw-r--r--  2.0 unx      244 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/PrismaticVelocityOutput.brick
--rw-r--r--  2.0 unx      227 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RigidBodyPositionOutput.brick
--rw-r--r--  2.0 unx      243 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RigidBodyRPYOutput.brick
--rw-r--r--  2.0 unx      122 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RigidBodyVelocityOutput.brick
--rw-r--r--  2.0 unx      310 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RotationalVelocityMotorVelocityInput.brick
--rw-r--r--  2.0 unx      255 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/TorqueMotorTorqueInput.brick
--rw-r--r--  2.0 unx      143 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/TorsionSpringAngleInput.brick
+-rw-r--r--  2.0 unx      229 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/HingeAngleOutput.brick
+-rw-r--r--  2.0 unx      276 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/HingeAngularVelocityOutput.brick
+-rw-r--r--  2.0 unx      290 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/LinearVelocityMotorVelocityInput.brick
+-rw-r--r--  2.0 unx      281 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/PrismaticPositionOutput.brick
+-rw-r--r--  2.0 unx      297 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/PrismaticVelocityOutput.brick
+-rw-r--r--  2.0 unx      280 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RigidBodyPositionOutput.brick
+-rw-r--r--  2.0 unx      289 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RigidBodyRPYOutput.brick
+-rw-r--r--  2.0 unx      175 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RigidBodyVelocityOutput.brick
+-rw-r--r--  2.0 unx      316 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/RotationalVelocityMotorVelocityInput.brick
+-rw-r--r--  2.0 unx      261 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/TorqueMotorTorqueInput.brick
+-rw-r--r--  2.0 unx      149 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Signals/TorsionSpringAngleInput.brick
 -rw-r--r--  2.0 unx      299 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Snap/Utils.brick
 -rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/StructuralComponent.brick
 -rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/StructuralPlane.brick
 -rw-r--r--  2.0 unx      682 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/System.brick
 -rw-r--r--  2.0 unx       35 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/Transform.brick
 -rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 brickbundles/Physics3D/config.brick
 -rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 brickbundles/Robotics/EndEffectors/ConstantVacuumSystem.brick
@@ -216,21 +219,21 @@
 -rw-r--r--  2.0 unx      396 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Links/LinkData.brick
 -rw-r--r--  2.0 unx      909 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Links/RigidBoxLink.brick
 -rw-r--r--  2.0 unx      297 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Links/RigidLink.brick
 -rw-r--r--  2.0 unx      208 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Links/RigidTriMeshLink.brick
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Robots/Robot.brick
 -rw-r--r--  2.0 unx      104 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Robots/SerialManipulatorData.brick
 -rw-r--r--  2.0 unx     2886 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Robots/SixAxisSerialManipulator.brick
--rw-r--r--  2.0 unx      413 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/RobotInput.brick
+-rw-r--r--  2.0 unx      419 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/RobotInput.brick
 -rw-r--r--  2.0 unx      311 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/RobotInputSignal.brick
--rw-r--r--  2.0 unx     1292 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/RobotOutput.brick
+-rw-r--r--  2.0 unx     1179 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/RobotOutput.brick
 -rw-r--r--  2.0 unx      809 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/RobotOutputSignal.brick
 -rw-r--r--  2.0 unx      429 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/Sensor.brick
 -rw-r--r--  2.0 unx      157 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/SensorValues.brick
--rw-r--r--  2.0 unx      158 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/VacuumGripperStateInput.brick
+-rw-r--r--  2.0 unx      164 b- defN 80-Jan-01 00:00 brickbundles/Robotics/Signals/VacuumGripperStateInput.brick
 -rw-r--r--  2.0 unx      138 b- defN 80-Jan-01 00:00 brickbundles/Robotics/config.brick
 -rw-r--r--  2.0 unx      864 b- defN 80-Jan-01 00:00 brickbundles/Simulation/CollisionGroup.brick
 -rw-r--r--  2.0 unx      314 b- defN 80-Jan-01 00:00 brickbundles/Simulation/DisableCollisionPair.brick
 -rw-r--r--  2.0 unx      126 b- defN 80-Jan-01 00:00 brickbundles/Simulation/config.brick
 -rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 brickbundles/Terrain/Shovel.brick
 -rw-r--r--  2.0 unx     1030 b- defN 80-Jan-01 00:00 brickbundles/Terrain/Terrain.brick
 -rw-r--r--  2.0 unx       96 b- defN 80-Jan-01 00:00 brickbundles/Terrain/config.brick
@@ -263,11 +266,11 @@
 -rw-r--r--  2.0 unx      234 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick
 -rw-r--r--  2.0 unx       90 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Geometry.brick
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Sphere.brick
 -rw-r--r--  2.0 unx       96 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/TriMeshGeometry.brick
 -rw-r--r--  2.0 unx       10 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Materials/Material.brick
 -rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 brickbundles/Visuals/config.brick
 -rw-r--r--  2.0 unx     1346 b- defN 80-Jan-01 00:00 brickbundles/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.4.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.4.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx    30083 b- defN 16-Jan-01 00:00 brickbundles-0.4.6.dist-info/RECORD
-271 files, 124815 bytes uncompressed, 55132 bytes compressed:  55.8%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.5.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    30405 b- defN 16-Jan-01 00:00 brickbundles-0.5.0.dist-info/RECORD
+274 files, 127932 bytes uncompressed, 56568 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: brickbundles/DriveTrain/Actuator.brick
 Comment: 
 
+Filename: brickbundles/DriveTrain/Differential.brick
+Comment: 
+
 Filename: brickbundles/DriveTrain/Engine.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/Gear.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/HingeActuator.brick
@@ -18,14 +21,17 @@
 
 Filename: brickbundles/DriveTrain/Signals/GearTorqueOutput.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/Signals/TorqueMotorInput.brick
 Comment: 
 
+Filename: brickbundles/DriveTrain/TorqueLimitedSlipDifferential.brick
+Comment: 
+
 Filename: brickbundles/DriveTrain/TorqueMotor.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/config.brick
 Comment: 
 
 Filename: brickbundles/Math/AffineTransform.brick
@@ -177,14 +183,17 @@
 
 Filename: brickbundles/Physics/Signals/BoolInputSignal.brick
 Comment: 
 
 Filename: brickbundles/Physics/Signals/Input.brick
 Comment: 
 
+Filename: brickbundles/Physics/Signals/InputOutputType.brick
+Comment: 
+
 Filename: brickbundles/Physics/Signals/InputSignal.brick
 Comment: 
 
 Filename: brickbundles/Physics/Signals/Output.brick
 Comment: 
 
 Filename: brickbundles/Physics/Signals/OutputSignal.brick
@@ -798,17 +807,17 @@
 
 Filename: brickbundles/Visuals/config.brick
 Comment: 
 
 Filename: brickbundles/__init__.py
 Comment: 
 
-Filename: brickbundles-0.4.6.dist-info/METADATA
+Filename: brickbundles-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: brickbundles-0.4.6.dist-info/WHEEL
+Filename: brickbundles-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: brickbundles-0.4.6.dist-info/RECORD
+Filename: brickbundles-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## brickbundles/DriveTrain/Signals/GearTorqueOutput.brick

```diff
@@ -1,5 +1,6 @@
 GearTorqueOutput is Physics.Signals.Output:
     .doc: """
 Emits a ValueOutputSignal where the value is the torque in Nm
 """
+    type: Physics.Signals.InputOutputType.Torque
     gear is DriveTrain.Gear
```

## brickbundles/DriveTrain/Signals/TorqueMotorInput.brick

```diff
@@ -1,3 +1,3 @@
 TorqueMotorInput is Physics.Signals.Input:
-    type: Physics.Signals.InputType.Torque
+    type: Physics.Signals.InputOutputType.Torque
     motor is DriveTrain.TorqueMotor
```

## brickbundles/Physics/Signals/Input.brick

```diff
@@ -1,19 +1,11 @@
 
 Input:
     .doc: """
 An Input, ie a receiver of signals.
-- Each Input should have a type-attribute, e.g. InputType.Torque, Angle, AngularVelocity or any of above.
+- Each Input should have a type-attribute, e.g. InputOutputType.Torque, Angle, AngularVelocity or any of above.
 - Use type Composite when the Input receives a Signal with multiple values.
 - reference_id is optional and must be unique within each Robot and can be used to identify the sensor, e.g. when communicating using Click or ROS. Typically the full name will be used if not set.
 """
     type is Int
     reference_id is String: ""
 
-const InputType:
-    Position is Int: 1
-    Velocity is Int: 2
-    Angle is Int: 3
-    AngularVelocity is Int: 4
-    Torque is Int: 5
-    Composite is Int: 6
-    ControlEvent is Int: 7
```

## brickbundles/Physics/Signals/Output.brick

```diff
@@ -1 +1,8 @@
-Output
+Output:
+    .doc: """
+An Output, i.e. a sender of signals.
+- Each Output must have a type-attribute, e.g. InputOutputType.Torque, Angle, AngularVelocity or any other InputOutputType.
+- Use type Composite when the Output sends a Signal with multiple values.
+"""
+    type is Int
+
```

## brickbundles/Physics1D/Signals/RotationalBodyAngleOutput.brick

```diff
@@ -1,6 +1,6 @@
 RotationalBodyAngleOutput is Physics.Signals.Output:
     .doc: """
 Emits a ValueOutputSignal where the value is the angle in radians
 """
-
+    type: Physics.Signals.InputOutputType.Angle
     body is Physics1D.Bodies.RotationalBody
```

## brickbundles/Physics1D/Signals/RotationalBodyAngularVelocityOutput.brick

```diff
@@ -1,6 +1,6 @@
 RotationalBodyAngularVelocityOutput is Physics.Signals.Output:
     .doc: """
 Emits a ValueOutputSignal where the value is the anglular velocity in radians
 """
-
+    type: Physics.Signals.InputOutputType.AngularVelocity
     body is Physics1D.Bodies.RotationalBody
```

## brickbundles/Physics1D/Signals/RotationalVelocityMotor1DTorqueOutput.brick

```diff
@@ -1,2 +1,3 @@
 RotationalVelocityMotor1DTorqueOutput is Physics.Signals.Output:
+    type: Physics.Signals.InputOutputType.Torque
     motor is Physics1D.Interactions.RotationalVelocityMotor
```

## brickbundles/Physics1D/Signals/RotationalVelocityMotor1DVelocityInput.brick

```diff
@@ -1,4 +1,4 @@
 # Accepts a RealInputSignal where the motor target angular velocity in radians/s will be set to the signal value
 RotationalVelocityMotor1DVelocityInput is Physics.Signals.Input:
-    type: Physics.Signals.InputType.AngularVelocity
+    type: Physics.Signals.InputOutputType.AngularVelocity
     motor is Physics1D.Interactions.RotationalVelocityMotor
```

## brickbundles/Physics3D/Signals/HingeAngleOutput.brick

```diff
@@ -1,5 +1,6 @@
 HingeAngleOutput is Physics.Signals.Output:
   .doc: """
 Emits a ValueOutputSignal where the value is the angle of the hinge in radians
 """
+    type: Physics.Signals.InputOutputType.Angle
     hinge is Physics3D.Interactions.Hinge
```

## brickbundles/Physics3D/Signals/HingeAngularVelocityOutput.brick

```diff
@@ -1,5 +1,6 @@
 HingeAngularVelocityOutput is Physics.Signals.Output:
     .doc: """
 Emits a ValueOutputSignal where the signal value is the angular velocity of the hinge in radians/second
 """
+    type: Physics.Signals.InputOutputType.AngularVelocity
     hinge is Physics3D.Interactions.Hinge
```

## brickbundles/Physics3D/Signals/LinearVelocityMotorVelocityInput.brick

```diff
@@ -1,6 +1,6 @@
 LinearVelocityMotorVelocityInput is Physics.Signals.Input:
     .doc: """
 Accepts a RealInputSignal where the motors target velocity set to the signal value in meters per second
 """
-    type: Physics.Signals.InputType.Velocity
+    type: Physics.Signals.InputOutputType.Velocity1D
     motor is Physics3D.Interactions.LinearVelocityMotor
```

## brickbundles/Physics3D/Signals/PrismaticPositionOutput.brick

```diff
@@ -1,8 +1,9 @@
 PrismaticPositionOutput is Physics.Signals.Output:
     .doc: """
 Emits a ValueOutputSignal where the value is the offset of the prismatic in meters
 """
+    type: Physics.Signals.InputOutputType.Position1D
     prismatic is Physics3D.Interactions.Prismatic
 
 
 # TODO: Not implemented
```

## brickbundles/Physics3D/Signals/PrismaticVelocityOutput.brick

```diff
@@ -1,8 +1,9 @@
 PrismaticVelocityOutput is Physics.Signals.Output:
     .doc: """
 Emits a ValueOutputSignal where the signal value is the velocity of the prismatic in meters/second
 """
+    type: Physics.Signals.InputOutputType.Velocity1D
     prismatic is Physics3D.Interactions.Prismatic
 
 
 # TODO: Not implemented
```

## brickbundles/Physics3D/Signals/RigidBodyPositionOutput.brick

```diff
@@ -1,5 +1,6 @@
 RigidBodyPositionOutput is Physics.Signals.Output:
     .doc: """
 Emits a ValueOutputSignal where the signal value is the world coordinate position of the model frame of the body
 """
+    type: Physics.Signals.InputOutputType.Position3D
     rigid_body is Physics3D.Bodies.RigidBody
```

## brickbundles/Physics3D/Signals/RigidBodyRPYOutput.brick

```diff
@@ -1,6 +1,7 @@
 RigidBodyRPYOutput is Physics.Signals.Output:
     .doc: """
 Emits a ValueOutputSignal where the signal value is the Roll, Pitch & Yaw rotation of the model frame of the body
 in the world frame.
 """
+    type: Physics.Signals.InputOutputType.RPY
     rigid_body is Physics3D.Bodies.RigidBody
```

## brickbundles/Physics3D/Signals/RigidBodyVelocityOutput.brick

```diff
@@ -1,5 +1,6 @@
 RigidBodyVelocityOutput is Physics.Signals.Output:
+    type: Physics.Signals.InputOutputType.Velocity3D
     rigid_body is Physics3D.Bodies.RigidBody
 
 
 # TODO: Not implemented
```

## brickbundles/Physics3D/Signals/RotationalVelocityMotorVelocityInput.brick

```diff
@@ -1,6 +1,6 @@
 RotationalVelocityMotorVelocityInput is Physics.Signals.Input:
     .doc: """
 Accepts a RealInputSignal where the motor targets angular velocity will be set to the signal value in radians/second
 """
-    type: Physics.Signals.InputType.AngularVelocity
+    type: Physics.Signals.InputOutputType.AngularVelocity
     motor is Physics3D.Interactions.RotationalVelocityMotor
```

## brickbundles/Physics3D/Signals/TorqueMotorTorqueInput.brick

```diff
@@ -1,6 +1,6 @@
 TorqueMotorTorqueInput is Physics.Signals.Input:
     .doc: """
 Accepts a RealInputSignal where the motors target torque will be set to the signal value in [Nm]
 """
-    type: Physics.Signals.InputType.Torque
+    type: Physics.Signals.InputOutputType.Torque
     motor is Physics3D.Interactions.TorqueMotor
```

## brickbundles/Physics3D/Signals/TorsionSpringAngleInput.brick

```diff
@@ -1,3 +1,3 @@
 TorsionSpringAngleInput is Physics.Signals.Input:
-    type: Physics.Signals.InputType.Angle
+    type: Physics.Signals.InputOutputType.Angle
     spring is Physics3D.Interactions.TorsionSpring
```

## brickbundles/Robotics/Signals/RobotInput.brick

```diff
@@ -1,9 +1,9 @@
 
 RobotInput is Physics.Signals.Input:
   .doc: """
 A filter that accepts a RobotInputSignal and decomposes it into a RealInputSignal of the correct type for each target in targets.
 targets contains the Signal Inputs to map to in order.
 """
-    type: Physics.Signals.InputType.Composite
+    type: Physics.Signals.InputOutputType.Composite
     targets is Physics.Signals.Input[]: []
     fn process(signal: Physics.Signals.InputSignal) -> Physics.Signals.InputSignal[]
```

## brickbundles/Robotics/Signals/RobotOutput.brick

```diff
@@ -1,22 +1,19 @@
 RobotOutput is Physics.Signals.Output:
   .doc: """
 A filter that accepts signals from specified sources and composes them into a RobotOutputSignal
 - Signal values from `sensors` will be composed into `sensor_values` with possibly multiple values under the name of the sensor.
 
 The following signals are unnamed, so the order is important:
-- Signal values from `angle_sources` will be composed in order into `angles`
-- Signal values from `angular_velocity_sources` will be composed in irder into `angular_velocities`
-- Signal values from `torque_sources` will be composed in order into `torques`
+- Signal values from `joint_sources` with type InputOutputType.Angle will be composed in order into `angles`
+- Signal values from `joint_sources` with type InputOutputType.AngularVelocity will be composed in order into `angular_velocities`
+- Signal values from `joint_sources` with type InputOutputType.Torque will be composed in order into `torques`
 - Signal values from `object_sources` will be composed in order into `object_values`.
 
 """
-
-    # These three are per hinge, i.e the length of each list is the number of hinges - how reflect?
-    angle_sources is Physics3D.Signals.HingeAngleOutput[]: []
-    angular_velocity_sources is Physics3D.Signals.HingeAngularVelocityOutput[]: []
-    torque_sources is DriveTrain.Signals.GearTorqueOutput[]: []
+    type: Physics.Signals.InputOutputType.Composite
+    joint_sources is Physics.Signals.Output[]: []
     # object_sources are unnamed and arrives in the order defined by this list
     object_sources is Physics.Signals.Output[]: []
 
     sensors is Robotics.Signals.Sensor[]: []
     fn process(output: Physics.Signals.Output, signals: Physics.Signals.OutputSignal[]) -> Physics.Signals.OutputSignal
```

## brickbundles/Robotics/Signals/VacuumGripperStateInput.brick

```diff
@@ -1,4 +1,4 @@
 VacuumGripperStateInput is Physics.Signals.Input:
-    type: Physics.Signals.InputType.ControlEvent
+    type: Physics.Signals.InputOutputType.ControlEvent
     vacuum_gripper is Robotics.EndEffectors.VacuumGripper
```

## Comparing `brickbundles-0.4.6.dist-info/METADATA` & `brickbundles-0.5.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrickBundles
-Version: 0.4.6
+Version: 0.5.0
 Summary: Brick Bundles package, i.e. all Brick sourcefiles and convenience access method in a package
 License: Apache 2.0
 Author: Algoryx
 Author-email: algoryx@algoryx.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `brickbundles-0.4.6.dist-info/RECORD` & `brickbundles-0.5.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 brickbundles/DriveTrain/Actuator.brick,sha256=x2MlOtidmaIG8Q0FWMu5piL5R9OQMOmD7VIMC9Z3CNM,106
+brickbundles/DriveTrain/Differential.brick,sha256=0wcO8TMm85pxdDeQfNCq75BO7V85jpcYyFdfiCPyB5A,742
 brickbundles/DriveTrain/Engine.brick,sha256=Is3sdxaZfoGcV5D45wSgSN0puv_6cIV1VUUkyt0HSTU,675
 brickbundles/DriveTrain/Gear.brick,sha256=zlJtK6Ii-t08ZXLTZ38lGZlp3_qi8C-8GN5cwTfrbu8,133
 brickbundles/DriveTrain/HingeActuator.brick,sha256=A1eSKcju316hLDp4jZ5MsnKZsbmQXUZIAlHuy0vX7Ro,112
 brickbundles/DriveTrain/PrismaticActuator.brick,sha256=Cu0E814_u5OVhf6iAjzXi0R-qW86f0l5MBvMLfFiVow,281
 brickbundles/DriveTrain/Shaft.brick,sha256=5IwBB9q-73xngtKf3cLJt09lD-QoelUQYZ2miMzFZdw,133
-brickbundles/DriveTrain/Signals/GearTorqueOutput.brick,sha256=WJPR_GmUdwU51PxIGMAQ-YHnHRseql0msFcmk5HQD10,152
-brickbundles/DriveTrain/Signals/TorqueMotorInput.brick,sha256=79Iq2y2IAne_phQYkt6L_5LSAQfAeRhyN5bANzhwUFY,122
+brickbundles/DriveTrain/Signals/GearTorqueOutput.brick,sha256=Asi_heEYQ5C7aS3a4KUSyM6VxPBhnBZ0Etfm34PrhhU,201
+brickbundles/DriveTrain/Signals/TorqueMotorInput.brick,sha256=cUOqFfihVtsq2ZSLq_bDKb6Nl0BOI9zUknnhnFV5SR8,128
+brickbundles/DriveTrain/TorqueLimitedSlipDifferential.brick,sha256=rDsDLx-93miXe4vGLukv7zMU9YGlZywUDk73oAGQ34Q,1193
 brickbundles/DriveTrain/TorqueMotor.brick,sha256=eUs07jvCdqwdJiUdiXDmANVAnW1kYNtmwuxuBSUycRM,53
 brickbundles/DriveTrain/config.brick,sha256=v4CrbDzcvkJqxfoLuApV8NC7f1JxJW8F6haJiym0e90,112
 brickbundles/Math/AffineTransform.brick,sha256=YrFSwBjhHoLf72D2OawtrKYCFjp7aqVe8BTnv3aUSx8,420
 brickbundles/Math/Constants.brick,sha256=lripEIYTI9AkFuln4alNrGrsUA0U2i21Q5HZplTn38E,141
 brickbundles/Math/Functions.brick,sha256=ofmSeTWw8ppjOKG6WGkcMhl-WRqIeDWiFMZlQTZ8sX0,285
 brickbundles/Math/Line.brick,sha256=dLNzn34DGtT_hCQYBvucHjId--Y7E0781UhXvlwMzBo,99
 brickbundles/Math/Matrix3x3.brick,sha256=z0joC0XxJmqg0bZHkiLR368pQRAxQG3gby_81OLAEpE,975
@@ -54,17 +56,18 @@
 brickbundles/Physics/Interactions/Slack/ConstantDistanceSlack.brick,sha256=axerTakmTFOc5fAUs-8g7vbv7LaWgqOXC7QH66v2vZ0,109
 brickbundles/Physics/Interactions/Slack/DefaultSlack.brick,sha256=DbTXr9tyv-mtDQ7gwI8mjUktytXoi6WkrzOz2I0tlko,861
 brickbundles/Physics/Interactions/SurfaceContact/Model.brick,sha256=u4eFMWzRQFZJSL23quh-JvTuU22SqOh_i6e-bEVIkD0,834
 brickbundles/Physics/Interactions/SurfaceContact/PatchElasticity.brick,sha256=nWERqV2F0tJ7OxY22nGdKKFqAdmgbwVbKyhQBcgoAQ0,419
 brickbundles/Physics/Interactions/SurfaceContact/PointwiseElasticity.brick,sha256=NSZcYTfuhSrS0TWO8BfObhvpmamWnU21hjFQJqdM2dI,270
 brickbundles/Physics/KinematicLock.brick,sha256=ZWskoZziAF5YZg6BVaWMvoCiB5WL2HlmyD6ei_AoUzU,403
 brickbundles/Physics/Signals/BoolInputSignal.brick,sha256=yaDDXs5x33shckRfFJEVfz6F2uhilQTQG-S_gsYdUFY,121
-brickbundles/Physics/Signals/Input.brick,sha256=iTflGlAxW41kL-ocTsA4TB3LqPlDrab7YP0NQAr0Ugg,674
+brickbundles/Physics/Signals/Input.brick,sha256=I_9js19aE-ax-hT987QHFRvW9uq7adlSSL1q2BQCi6g,495
+brickbundles/Physics/Signals/InputOutputType.brick,sha256=TmkMsr3gs40w_p4lr4gU8lfRQO30Avu1dxqkWANX9Aw,265
 brickbundles/Physics/Signals/InputSignal.brick,sha256=S0msuXlEXdi6ZAFA-PkVF9-pFBpvF2W1DMg6RKp2a3E,33
-brickbundles/Physics/Signals/Output.brick,sha256=P8s1XE9RG2H_dWdMpxGTEgA2cg-SbVi_a84qBXtLT8U,7
+brickbundles/Physics/Signals/Output.brick,sha256=V1X3nnm4WAMtvMQ8XC9x2UPqNh4DcmlmHP2_tSrVdZc,278
 brickbundles/Physics/Signals/OutputSignal.brick,sha256=khcE8_joHePCV05IXWzYg_SD909fJE08bp3y5C-95VQ,35
 brickbundles/Physics/Signals/RealInputSignal.brick,sha256=MZkPcwAXloiairjyB_Y2RJBl-zEoYf63bc6DA0xuCnE,121
 brickbundles/Physics/Signals/RealOutputSignal.brick,sha256=--co-OVdG6x2CO1P5tmKPWvppOMxrZB7g-ckuMaZArM,121
 brickbundles/Physics/Signals/Value.brick,sha256=CPlTaz0qAjF83i2vASwJ9g-6201hbYZ9m5a3Kk-F1bw,1489
 brickbundles/Physics/Signals/ValueOutputSignal.brick,sha256=Y8Lav3R498DRhfHyfbph1RMlKc5MGdKnTFJfa-ByOvE,1714
 brickbundles/Physics/Signals/Vec3OutputSignal.brick,sha256=mpyUOkGzm2yfs3hu_raRbHbpuCqJgF1Stu1v7ADdqB8,131
 brickbundles/Physics/System.brick,sha256=owz_VZMWmb9WwRR6mc_T5azQutpVWVBenhdmnjGwogs,50
@@ -78,18 +81,18 @@
 brickbundles/Physics1D/Bodies/RotationalKinematics.brick,sha256=J3NNJSlrV9G3RJXuh7Q1icSV0WWxlx31KPd0X0zg-ZM,59
 brickbundles/Physics1D/Charges/LinearConnector.brick,sha256=FjNCOQngn3zwDOO_hrjKrJuerBqXbi_JqlK2s_kk56g,63
 brickbundles/Physics1D/Charges/MateConnector.brick,sha256=gJ1UxG0jiogmCvHUtjy54LuwdgbY-yhuBpa7OGeBVzU,64
 brickbundles/Physics1D/Charges/RotationalConnector.brick,sha256=JKThzVp_29xUXIgQ6NqF-61f36zYYwUTzSoPq4AOJuk,59
 brickbundles/Physics1D/Interactions/Mate.brick,sha256=nj9mN6oQysqVtTOFtXDXmR6qncNkJyHwQncTH974_LQ,96
 brickbundles/Physics1D/Interactions/RotationalVelocityMotor.brick,sha256=D4Kp7nsR5yGS25OVEb9nWSH3fRuZ5UjnBg_qFAkRHbQ,43
 brickbundles/Physics1D/Interactions/VelocityMotor.brick,sha256=QSRzfWNrd2PUaK_e_qjhkDRH_v6Ns-tWqSrd-R59T30,141
-brickbundles/Physics1D/Signals/RotationalBodyAngleOutput.brick,sha256=ubzhpN0ELMUaBV1jVPpbzI3hgtf3u-R2RETs1Cl8dJI,182
-brickbundles/Physics1D/Signals/RotationalBodyAngularVelocityOutput.brick,sha256=CdP9yDfCOZjBXy7HkAtvM-XcjvttP9gtYbvCVHUtU7c,204
-brickbundles/Physics1D/Signals/RotationalVelocityMotor1DTorqueOutput.brick,sha256=EZhm22kNrInC5MyZbxjlqa9WX2Er5L6gcdvkwjyEp2M,125
-brickbundles/Physics1D/Signals/RotationalVelocityMotor1DVelocityInput.brick,sha256=YQkSL_vqvtaUUz0rVXyxTEYDRYgYt3Rtr0_qaCT_pHs,290
+brickbundles/Physics1D/Signals/RotationalBodyAngleOutput.brick,sha256=mpv6dRvbcO5LaPpsIbnlRWfFB53L5-rUeUrD_0Y_NT8,229
+brickbundles/Physics1D/Signals/RotationalBodyAngularVelocityOutput.brick,sha256=6y7EdzWNZ7Yr8ElTEpffXSOWT_tmIWt7isEREQS5mi8,261
+brickbundles/Physics1D/Signals/RotationalVelocityMotor1DTorqueOutput.brick,sha256=GBAD-rIjOCshVEi3Y-r1h6WNo59sw_KfD_eXeYCaRWs,174
+brickbundles/Physics1D/Signals/RotationalVelocityMotor1DVelocityInput.brick,sha256=_L_19B8pvgbkVCaB9nersUCBOThmcfBaiXNhWUp4oWE,296
 brickbundles/Physics1D/config.brick,sha256=gjRyz5hAHU9xA2cnHL4IUjiCYjyWwBEDv9OloLuOBU8,85
 brickbundles/Physics3D/Bodies/Body.brick,sha256=Kax629Pnh5aPKIgCAfVmmFHfFjd02uRIRcxumoxTqCI,78
 brickbundles/Physics3D/Bodies/Inertia.brick,sha256=_byO4-rznjHShggZH37A4frt_x7UjbGP95XHjDzx2q8,526
 brickbundles/Physics3D/Bodies/Kinematics.brick,sha256=TIGYQo_Dqgmfo0EkIP9JAspHOCK_GNywmH700mDzv8A,196
 brickbundles/Physics3D/Bodies/RigidBody.brick,sha256=c9Mt93YOE_rXBlgQsydBJLMwtWSM1mcDyKag9WgTSrs,138
 brickbundles/Physics3D/Bodies/RigidBodyKinematics.brick,sha256=HRTI35MstZpyRzV4afZCvUgRcLNvXPXWe_o-NfpbdKk,161
 brickbundles/Physics3D/Charges/AdaptiveMateConnector.brick,sha256=aSfIPaHELPqz1hwuT_Q7slp0Hbi-JQVOvanQUaToZqg,748
@@ -162,25 +165,25 @@
 brickbundles/Physics3D/Interactions/SpringInteraction1DOF.brick,sha256=-34r7eo5Gq88wT9nH4xOrI8tAksn2XaqLH1UiRqb60w,443
 brickbundles/Physics3D/Interactions/SurfaceContact/PatchElasticityDryFrictionModel.brick,sha256=83N8JQ8kBb07fdh_6rx8pEcepGnjLCZXz-R7i75hAxs,512
 brickbundles/Physics3D/Interactions/SurfaceContact/PointwiseElasticityDryFrictionModel.brick,sha256=d_D0Ndchzm3BMB3DbKLw634cQcpiYmNSbkJVHjKoolM,818
 brickbundles/Physics3D/Interactions/TorqueMotor.brick,sha256=282nobtKKN3bunaaDNvwcH0YOfPkJdOgMIcUhZRXE2Y,266
 brickbundles/Physics3D/Interactions/TorsionSpring.brick,sha256=1BkWUdDTZEjQ6j89kdzwmx04nFyooCSOs_JSc7By4xY,63
 brickbundles/Physics3D/Interactions/VelocityMotor.brick,sha256=8VLOArZK2RbC1sD_WrA5XoWxm6Ta_kgM9dWy4ISSEA8,1226
 brickbundles/Physics3D/RelativeTransform.brick,sha256=gnAlq_yEiZnwPlOJO37f0CsqDG7vgMUrfs8j5qlvrLA,557
-brickbundles/Physics3D/Signals/HingeAngleOutput.brick,sha256=no7s_sFuSlLYFPlF9eTX3WsJ5lPvSRp11Zx3wOE5i1Q,181
-brickbundles/Physics3D/Signals/HingeAngularVelocityOutput.brick,sha256=yG3WyfCjO0svPFVyC8-xVYuLvMcIg7h4c2AHWUhgCak,218
-brickbundles/Physics3D/Signals/LinearVelocityMotorVelocityInput.brick,sha256=PAiGYx0d0KrylBCxvBuT7e4zepr3kuPy28hwMFnFQu8,282
-brickbundles/Physics3D/Signals/PrismaticPositionOutput.brick,sha256=lMgwIc61pgdkmJoFRvFTA7cFt4WSwDfo5v1uGuTZE24,228
-brickbundles/Physics3D/Signals/PrismaticVelocityOutput.brick,sha256=XD9Mug1gVCNQbJpo2VdTIAPviAO2BSB4BlSSS0jEQzg,244
-brickbundles/Physics3D/Signals/RigidBodyPositionOutput.brick,sha256=MmuuELbNk7IL127IdwlxcEK8HEIbaU7IvLfJnc4q8v4,227
-brickbundles/Physics3D/Signals/RigidBodyRPYOutput.brick,sha256=6v8CxeSw02imzO3W_Rg4PRBK70EMf1l2UaW5-5MgJFc,243
-brickbundles/Physics3D/Signals/RigidBodyVelocityOutput.brick,sha256=fpYHcKNbuwgudZ3MU7oNjvreBgu49lHIiC5jWtGdZX4,122
-brickbundles/Physics3D/Signals/RotationalVelocityMotorVelocityInput.brick,sha256=fQAYcaTXf4DE8bvK4gUyCbzMgw2hdjFnPTajG18367A,310
-brickbundles/Physics3D/Signals/TorqueMotorTorqueInput.brick,sha256=3JforIyiQdv-_1mTTuB139EZ6FSuETDGQkb05IUY6ZM,255
-brickbundles/Physics3D/Signals/TorsionSpringAngleInput.brick,sha256=o6Mv23uc_qQt9fjgOS-UyL_Y9EmOZ32Oe6NxJEtZlb8,143
+brickbundles/Physics3D/Signals/HingeAngleOutput.brick,sha256=m550Ce5IXDzvFKTdDUBWBNm8vToDMmEF6MYZDHWLMRk,229
+brickbundles/Physics3D/Signals/HingeAngularVelocityOutput.brick,sha256=4Ntn2lFfRJcg1_RLcZQElSBdpVIICslr-z4ht36WdeQ,276
+brickbundles/Physics3D/Signals/LinearVelocityMotorVelocityInput.brick,sha256=Nbe4DmMi7RqEGHW-Bbb0Bvbl5N7LtU9VKnV-LdtIrTs,290
+brickbundles/Physics3D/Signals/PrismaticPositionOutput.brick,sha256=nlATzEPWAoF8VwRXWZY6wLo3jrUttliWLdHA_yNIANY,281
+brickbundles/Physics3D/Signals/PrismaticVelocityOutput.brick,sha256=shVe_RZ5BLu4leqOxRAtFmIkJpA0e1RNNXszU5VW4KY,297
+brickbundles/Physics3D/Signals/RigidBodyPositionOutput.brick,sha256=mLGtyWb1x65XcXtvBycSd--t2ssmwSBiw8wTWGwhGQ4,280
+brickbundles/Physics3D/Signals/RigidBodyRPYOutput.brick,sha256=VTt0g1KwBEpnQNK3aoSRgfiGt10SgyoPnX_PLo9aaOs,289
+brickbundles/Physics3D/Signals/RigidBodyVelocityOutput.brick,sha256=178qyynryma8abwimrMIj1BxFrcexR4LxsVywhb6umQ,175
+brickbundles/Physics3D/Signals/RotationalVelocityMotorVelocityInput.brick,sha256=aObNKOvwVnGIkTnS9M5qmnpkeK1lcbeAfGVM9eEmtXQ,316
+brickbundles/Physics3D/Signals/TorqueMotorTorqueInput.brick,sha256=5wPFZjhet3zcMRMScm2NMGcfwP5ZfU_UwAmLo3cajbw,261
+brickbundles/Physics3D/Signals/TorsionSpringAngleInput.brick,sha256=ZnoOoyix_NFb9I_kxw81oxJN23KKKqR1pOSQfrLkSPU,149
 brickbundles/Physics3D/Snap/Utils.brick,sha256=KOBSnGIKc4UloVs60uvdhmgoYIsXfWUB32tX6RF8VuM,299
 brickbundles/Physics3D/StructuralComponent.brick,sha256=48umIByvntbXmgWMevKWyekbYxWpj0LWE_jELUMoNfM,544
 brickbundles/Physics3D/StructuralPlane.brick,sha256=gsCOiQHEtzaVB7dGDK0Gh-ConFBwFd4II4xQslFRIwE,132
 brickbundles/Physics3D/System.brick,sha256=3IFpmSSAA8pXQ4zK_Qv-eMOvJy0SOrATA56rlIJrq2I,682
 brickbundles/Physics3D/Transform.brick,sha256=4v5_TSCBa2sZxMi0C_NIUjMBDEWxp3Tq1VFJdf3Gv8E,35
 brickbundles/Physics3D/config.brick,sha256=Z_R3fizCNhULFroAImzg11C0ByEFWqySpYYme3aWADs,85
 brickbundles/Robotics/EndEffectors/ConstantVacuumSystem.brick,sha256=9pzRXfOgtqwrK4rjDZ45fXxNTF1ONacVigPj6XvOhio,68
@@ -215,21 +218,21 @@
 brickbundles/Robotics/Links/LinkData.brick,sha256=sMbRHwHYSG_CojsUqBQJ7NUAiVyOzdgF5JkNsjchFYM,396
 brickbundles/Robotics/Links/RigidBoxLink.brick,sha256=XWo279bqC0XNsqPK0JBJbMwA_6IVdJuSlQH2o0boJYc,909
 brickbundles/Robotics/Links/RigidLink.brick,sha256=yUxvisLz3Pwa2kUprTKqEe_-13DCPE3fNUsC-fJI1og,297
 brickbundles/Robotics/Links/RigidTriMeshLink.brick,sha256=S_7rJrzcJUJ8tlaKeTtMyBwFkeZaa_9_KtMp4Df2tOw,208
 brickbundles/Robotics/Robots/Robot.brick,sha256=PgwGFsQmMKTjCiNy_ro9c2E1nivBGxFadNfg-s90bC8,27
 brickbundles/Robotics/Robots/SerialManipulatorData.brick,sha256=xlJISb3WKMucxhaYonieh-OBhr02sdAEEvttN3Cy4ps,104
 brickbundles/Robotics/Robots/SixAxisSerialManipulator.brick,sha256=PW0iIP0Abf7FyMoiBmmQBDjl1FQee21r7DU8Ak0rQWY,2886
-brickbundles/Robotics/Signals/RobotInput.brick,sha256=5pCdTMxMh6-ydEq4NBMgAEC7gH-AwZjTc-s0YIcFhOU,413
+brickbundles/Robotics/Signals/RobotInput.brick,sha256=x912DH1dqq1cVMlpF9MdCtAfC7c3YwYZzGVv2SYier0,419
 brickbundles/Robotics/Signals/RobotInputSignal.brick,sha256=baMu2Kcn7PtwXE0Ev3ZEbNwdTbXEmGQCPRuTYQL_HNQ,311
-brickbundles/Robotics/Signals/RobotOutput.brick,sha256=48N2cBnZqNePth3cj4Lwb43uYyuE8zgbEzRWsMZtGiM,1292
+brickbundles/Robotics/Signals/RobotOutput.brick,sha256=J2ABe3lUokdhrhcnKF83kyx8myEHnaJRus7EWAFeLP4,1179
 brickbundles/Robotics/Signals/RobotOutputSignal.brick,sha256=SkonOL3W5V4NV9-ef5RxP1XvHhDUseddOWR7piagQ9A,809
 brickbundles/Robotics/Signals/Sensor.brick,sha256=k4-ZflLrTdQmsdWsbcifofcJ77OnvdTNWPuUBY5Zed8,429
 brickbundles/Robotics/Signals/SensorValues.brick,sha256=Fl1EThg7SApxcNGafMRmse8cKryAjYLJ7nMv8NL-9qA,157
-brickbundles/Robotics/Signals/VacuumGripperStateInput.brick,sha256=0E_ypJbtZZoo76C97qK2k_BuKCBtnvVCZWm_2iiuDwo,158
+brickbundles/Robotics/Signals/VacuumGripperStateInput.brick,sha256=zJjZircYr5rkx6aC0cYuX9iqfCwq0SVoXutsaD9asIY,164
 brickbundles/Robotics/config.brick,sha256=tpt5o0juqmFMaI7AVr0Cs6uUYVeA15eCLfjrvW0DmgY,138
 brickbundles/Simulation/CollisionGroup.brick,sha256=pBhquPE6znYXJtwFycRj00Wuz0_Nb5m7a02w_CyzpKY,864
 brickbundles/Simulation/DisableCollisionPair.brick,sha256=YAy254OjBTNwtaqkfrEyqjTufYTZWgfMM8apZCDaA6g,314
 brickbundles/Simulation/config.brick,sha256=Pi1wLoOkYwVx9VmD5tFbwMW5pXA69JKNz8lAv5ImhCI,126
 brickbundles/Terrain/Shovel.brick,sha256=IttetloPMlTdW4oUN0Et97h2awqo12Fe4sWMbpmkATs,592
 brickbundles/Terrain/Terrain.brick,sha256=9VVPI7KRo4_DOJ16dWISmzwCuZJ8aj1RdP2zGUHE8A4,1030
 brickbundles/Terrain/config.brick,sha256=KRur9iGXQ59G8WMfL-k0qsnW8FMJscb3IVykXXTTPKs,96
@@ -262,10 +265,10 @@
 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick,sha256=0cEEaVuE72vhJvAv6J1guVo6yZVOCf7Q4gFP9KvElGQ,234
 brickbundles/Visuals/Geometries/Geometry.brick,sha256=-tiwTgsHtKnrPvaPO6kj5LG_gfF0csLAxdJUXJJzywg,90
 brickbundles/Visuals/Geometries/Sphere.brick,sha256=K3DerE_AE6EnHc_2GmT1e9sYrCMUosmUlTXIcqYapBg,39
 brickbundles/Visuals/Geometries/TriMeshGeometry.brick,sha256=qctdVQYflyKPuuX6HK8QvTgRbKNYlI5JAB82UNmKTZs,96
 brickbundles/Visuals/Materials/Material.brick,sha256=hVvFGaQhcFJblZ1R0SLDhWjIY6lSKC84i9hBwmA3sq8,10
 brickbundles/Visuals/config.brick,sha256=Z7y-m-8BN9N4V0OvqKp8BKivcspo8_-IpA2xA5xvf80,72
 brickbundles/__init__.py,sha256=VC7H2Q-oD1kqfe06eBZdgPlW8tC1kzBRQXWHkOIYk24,1346
-brickbundles-0.4.6.dist-info/METADATA,sha256=Ji3qTMuCxrm6glB33mCKULiZcHxo58x-rwk6YsOdQS8,1066
-brickbundles-0.4.6.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-brickbundles-0.4.6.dist-info/RECORD,,
+brickbundles-0.5.0.dist-info/METADATA,sha256=7k4V8mNlCYDuMTlJsMGZWkbY6hc4bsKhpZqRa2d9aTQ,1066
+brickbundles-0.5.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+brickbundles-0.5.0.dist-info/RECORD,,
```

