# Comparing `tmp/pyiArduinoI2Cexpander-0.9.9.tar.gz` & `tmp/pyiArduinoI2Cexpander-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiArduinoI2Cexpander-0.9.9.tar", last modified: Wed Nov  6 16:48:27 2019, max compression
+gzip compressed data, was "pyiArduinoI2Cexpander-1.0.1.tar", last modified: Fri Apr 12 09:19:34 2024, max compression
```

## Comparing `pyiArduinoI2Cexpander-0.9.9.tar` & `pyiArduinoI2Cexpander-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,57 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-11-06 16:48:27.000000 pyiArduinoI2Cexpander-0.9.9/
--rw-r--r--   0 pi        (1000) pi        (1000)     2472 2019-11-06 16:48:27.000000 pyiArduinoI2Cexpander-0.9.9/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       24 2019-11-06 16:43:36.000000 pyiArduinoI2Cexpander-0.9.9/README
--rw-r--r--   0 pi        (1000) pi        (1000)     1919 2019-11-06 16:41:54.000000 pyiArduinoI2Cexpander-0.9.9/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-11-06 16:48:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/
--rw-r--r--   0 pi        (1000) pi        (1000)       31 2019-10-10 12:18:04.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-11-06 16:48:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/
--rw-r--r--   0 pi        (1000) pi        (1000)     9722 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/FindDevices.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3315 2019-11-06 14:55:06.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/NewAddress.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3614 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/analogAveraging.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3292 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/analogRead.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4184 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/analogWrite.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3219 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/digitalRead.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2831 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/digitalWrite.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     6401 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/freqPWM.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2319 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/getVersion.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4127 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/levelRead.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     6781 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/pinMode.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     6499 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/pinOutScheme.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4624 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/pinPull.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     2963 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/reset.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     7301 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/servoAttach.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3860 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/servoWrite.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     4522 2019-11-06 14:52:17.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/servoWriteMicroseconds.cpp
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-11-06 16:48:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)     5583 2019-11-06 14:47:04.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/FindDevices.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4084 2019-11-06 14:50:48.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/NewAddress.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2514 2019-11-06 15:59:41.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/analogAveraging.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2324 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/analogRead.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3309 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/analogWrite.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2192 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/digitalRead.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1791 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/digitalWrite.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4827 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/freqPWM.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1313 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/getVersion.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2844 2019-11-06 14:50:28.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/levelRead.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6438 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/pinMode.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5360 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/pinOutScheme.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3334 2019-11-06 14:51:07.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/pinPull.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2199 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/reset.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6066 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/servoAttach.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2787 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/servoWrite.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3199 2019-11-06 14:32:27.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/servoWriteMicroseconds.py
--rw-r--r--   0 pi        (1000) pi        (1000)    54100 2019-11-06 11:55:12.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/iarduino_I2C_Expander.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)    21194 2019-11-06 08:31:39.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/iarduino_I2C_Expander.h
--rw-r--r--   0 pi        (1000) pi        (1000)     1106 2019-11-06 08:27:21.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/iarduino_I2C_Expander.pxd
--rwxr-xr-x   0 pi        (1000) pi        (1000)    12632 2019-11-06 10:01:50.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/iarduino_I2C_Expander_PI.h
--rw-r--r--   0 pi        (1000) pi        (1000)   297473 2019-11-06 11:47:25.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.cpp
--rw-r--r--   0 pi        (1000) pi        (1000)     3963 2019-11-06 10:53:22.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.pyx
--rw-r--r--   0 pi        (1000) pi        (1000)      134 2019-10-10 12:18:04.000000 pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2019-10-10 12:18:04.000000 pyiArduinoI2Cexpander-0.9.9/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      772 2019-11-06 16:48:13.000000 pyiArduinoI2Cexpander-0.9.9/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.586280 pyiArduinoI2Cexpander-1.0.1/
+-rw-r--r--   0 dron      (1000) dron      (1000)     3289 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/LICENSE
+-rw-r--r--   0 dron      (1000) dron      (1000)       86 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/MANIFEST.in
+-rw-r--r--   0 dron      (1000) dron      (1000)     2223 2024-04-12 09:19:34.586280 pyiArduinoI2Cexpander-1.0.1/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)     1919 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/README.md
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.562280 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/
+-rw-r--r--   0 dron      (1000) dron      (1000)       31 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/__init__.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.574280 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/
+-rw-r--r--   0 dron      (1000) dron      (1000)     9722 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/FindDevices.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3315 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/NewAddress.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3614 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogAveraging.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3292 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogRead.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4184 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogWrite.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3219 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/digitalRead.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2831 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/digitalWrite.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     6401 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/freqPWM.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2319 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/getVersion.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4127 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/levelRead.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     6781 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinMode.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     6499 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinOutScheme.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4624 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinPull.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     2963 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/reset.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     7301 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoAttach.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     3860 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoWrite.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     4522 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoWriteMicroseconds.cpp
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.586280 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/
+-rw-r--r--   0 dron      (1000) dron      (1000)     5583 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/FindDevices.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     4084 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/NewAddress.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2514 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogAveraging.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2324 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogRead.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3309 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogWrite.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2192 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/digitalRead.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1791 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/digitalWrite.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     4827 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/freqPWM.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     1313 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/getVersion.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2844 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/levelRead.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     6438 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinMode.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     5360 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinOutScheme.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3334 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinPull.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2199 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/reset.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     6066 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoAttach.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     2787 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoWrite.py
+-rw-r--r--   0 dron      (1000) dron      (1000)     3199 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoWriteMicroseconds.py
+-rw-r--r--   0 dron      (1000) dron      (1000)    54927 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)    21194 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.h
+-rw-r--r--   0 dron      (1000) dron      (1000)     1106 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.pxd
+-rwxr-xr-x   0 dron      (1000) dron      (1000)    12628 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander_PI.h
+-rw-r--r--   0 dron      (1000) dron      (1000)   622689 2024-04-12 06:59:39.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.cpp
+-rw-r--r--   0 dron      (1000) dron      (1000)     5123 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/pyiArduinoI2Cexpander.pyx
+-rw-r--r--   0 dron      (1000) dron      (1000)      134 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/setup.py
+drwxr-xr-x   0 dron      (1000) dron      (1000)        0 2024-04-12 09:19:34.566280 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/
+-rw-r--r--   0 dron      (1000) dron      (1000)     2223 2024-04-12 09:19:34.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/PKG-INFO
+-rw-r--r--   0 dron      (1000) dron      (1000)     2062 2024-04-12 09:19:34.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/SOURCES.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)        1 2024-04-12 09:19:34.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/dependency_links.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       22 2024-04-12 09:19:34.000000 pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander.egg-info/top_level.txt
+-rw-r--r--   0 dron      (1000) dron      (1000)       79 2024-04-12 09:19:34.586280 pyiArduinoI2Cexpander-1.0.1/setup.cfg
+-rw-r--r--   0 dron      (1000) dron      (1000)      772 2024-04-12 06:57:35.000000 pyiArduinoI2Cexpander-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiArduinoI2Cexpander-0.9.9/PKG-INFO` & `pyiArduinoI2Cexpander-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,30 @@
-Metadata-Version: 1.1
-Name: pyiArduinoI2Cexpander
-Version: 0.9.9
-Summary: iarduino.ru module for Raspberry Pi
-Home-page: http://github.com/tremaru/pyiArduinoI2Cexpander
-Author: iarduino.ru
-Author-email: shop@iarduino.ru
-License: MIT
-Description: [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
-        
-        # pyiArduinoI2Cexpander
-        
-        **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) расширения выводов Expander и Trema Expander Hat от iArduino.ru по шине I2C на Raspberry Pi.**
-        
-        ## Установка ##
-        
-        [Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
-        
-        Установка из репозиториев PyPI в терминале Raspberry:
-        
-        `sudo pip3 install pyiArduinoI2Cexpander`
-        
-        Самостоятельная сборка из исходников:
-        
-        `git clone https://github.com/tremaru/pyiArduinoI2Cexpander.git && cd pyiArduinoI2Cexpander/pyiArduinoI2Cexpander && python3 setup.py build_ext --inplace`
-        
-        Примеры для Python находятся в папке `pyiArduinoI2Cexpander/examples`
-        
-        Примеры для С++ находятся в папке `pyiArduinoI2Cexpander/cpp`. Так же в этой папке лежит *Makefile* для сборки
-        из исходников. Можно собрать сразу все примеры командой:
-        `make all` или `make`
-        Для сборки конкретного примера: `make "название примера"`
-        Например:
-        `make reset`
-        Для удаления собранных исполняемых файлов:
-        `make clean`
-        
-        **This is a Python3 module for Raspberry Pi. It can work with Trema Expander i2c module and Trema Expander Hat by iarduino.ru**
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+[![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
+
+# pyiArduinoI2Cexpander
+
+**Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) расширения выводов Expander и Trema Expander Hat от iArduino.ru по шине I2C на Raspberry Pi.**
+
+## Установка ##
+
+[Статья на сайте iarduino.ru](https://wiki.iarduino.ru/page/raspberry-python-modules/)
+
+Установка из репозиториев PyPI в терминале Raspberry:
+
+`sudo pip3 install pyiArduinoI2Cexpander`
+
+Самостоятельная сборка из исходников:
+
+`git clone https://github.com/tremaru/pyiArduinoI2Cexpander.git && cd pyiArduinoI2Cexpander/pyiArduinoI2Cexpander && python3 setup.py build_ext --inplace`
+
+Примеры для Python находятся в папке `pyiArduinoI2Cexpander/examples`
+
+Примеры для С++ находятся в папке `pyiArduinoI2Cexpander/cpp`. Так же в этой папке лежит *Makefile* для сборки
+из исходников. Можно собрать сразу все примеры командой:
+`make all` или `make`
+Для сборки конкретного примера: `make "название примера"`
+Например:
+`make reset`
+Для удаления собранных исполняемых файлов:
+`make clean`
+
+**This is a Python3 module for Raspberry Pi. It can work with Trema Expander i2c module and Trema Expander Hat by iarduino.ru**
```

### Comparing `pyiArduinoI2Cexpander-0.9.9/README.md` & `pyiArduinoI2Cexpander-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pyiArduinoI2Cexpander
+Version: 1.0.1
+Summary: iarduino.ru module for Raspberry Pi
+Home-page: http://github.com/tremaru/pyiArduinoI2Cexpander
+Author: iarduino.ru
+Author-email: shop@iarduino.ru
+License: MIT
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
 [![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)
 
 # pyiArduinoI2Cexpander
 
 **Данная библилотека (модуль для Python3) позволяет управлять электронными модулями (устройствами) расширения выводов Expander и Trema Expander Hat от iArduino.ru по шине I2C на Raspberry Pi.**
 
 ## Установка ##
```

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/FindDevices.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/FindDevices.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/NewAddress.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/NewAddress.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/analogAveraging.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogAveraging.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/analogRead.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogRead.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/analogWrite.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/analogWrite.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/digitalRead.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/digitalRead.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/digitalWrite.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/digitalWrite.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/freqPWM.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/freqPWM.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/getVersion.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/getVersion.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/levelRead.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/levelRead.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/pinMode.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinMode.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/pinOutScheme.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinOutScheme.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/pinPull.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/pinPull.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/reset.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/reset.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/servoAttach.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoAttach.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/servoWrite.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoWrite.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/cpp/servoWriteMicroseconds.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/cpp/servoWriteMicroseconds.cpp`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/FindDevices.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/FindDevices.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/NewAddress.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/NewAddress.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/analogAveraging.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogAveraging.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/analogRead.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogRead.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/analogWrite.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/analogWrite.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/digitalRead.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/digitalRead.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/digitalWrite.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/digitalWrite.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/freqPWM.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/freqPWM.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/getVersion.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/getVersion.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/levelRead.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/levelRead.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/pinMode.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinMode.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/pinOutScheme.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinOutScheme.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/pinPull.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/pinPull.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/reset.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/reset.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/servoAttach.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoAttach.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/servoWrite.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoWrite.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/examples/servoWriteMicroseconds.py` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/examples/servoWriteMicroseconds.py`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/iarduino_I2C_Expander.cpp` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 #include "iarduino_I2C_Expander.h"																						//
+//#include <iostream>
 																														//
 //		Инициализация расширителя выводов:																				//	Возвращаемое значение: результат инициализации.
 bool	iarduino_I2C_Expander::begin			(void){																	//	Параметр: отсутствует
 		//	Инициируем работу с шиной I2C:																				//
 			objI2C->begin(100);																							//	Инициируем передачу данных по шине I2C на скорости 100 кГц.
 		//	Если адрес не указан, то ищим модуль на шине I2C:															//
 			if(valAddrTemp==0){																							//
 				for(int i=1; i<127; i++){																				//	Проходим по всем адресам на шине I2C
 					if( objI2C->checkAddress(i)											){	valAddr=i; delay(2);		//	Если на шине I2C есть устройство с адресом i, то используем этот адрес для проверки найденного модуля...
 					if(_readBytes(REG_MODEL,4)											){								//	Читаем 4 байта начиная с регистра «REG_MODEL» в массив «data».
 					if( data[0]     == DEF_MODEL_EXP									){								//	Если у модуля с адресом i в регистре «MODEL»   (data[0]) хранится значение DEF_MODEL_EXP, то ...
 					if((data[2]>>1) == i                 || data[2] == 0xFF				){								//	Если у модуля с адресом i в регистре «ADDRESS» (data[2]) хранится значение i (адрес+младший бит) или 0xFF (адрес не задавался), то ...
+                            //std::cout << int(data[3]) << '\n';
+                            // опять переварачивает старший бит случайным образом
+                            // на осциллографе этого переворота нет.
+                            if (data[3] != DEF_CHIP_ID_METRO)
+                                    data[3] &= 0x7F;
 					if( data[3]     == DEF_CHIP_ID_FLASH || data[3] == DEF_CHIP_ID_METRO){								//	Если у модуля с адресом i в регистре «CHIP_ID» (data[3]) хранится значение DEF_CHIP_ID_FLASH (идентификатор модулей Flash), или DEF_CHIP_ID_METRO (идентификатор модулей Metro), то ...
 						valAddrTemp=i; i=128;																			//	Считаем что модуль обнаружен, сохраняем значение i как найденный адрес и выходим из цикла.
 					}}}}}																								//
 				}																										//
 			}																											//
 		//	Если модуль не найден, то возвращаем ошибку инициализации:													//
 			if( valAddrTemp == 0														){	valAddr=0; return false;}	//
 		//	Проверяем наличие модуля на шине I2C:																		//
 			if( objI2C->checkAddress(valAddrTemp) == false								){	valAddr=0; return false;}	//	Если на шине I2C нет устройств с адресом valAddrTemp, то возвращаем ошибку инициализации
 			valAddr=valAddrTemp;																						//	Сохраняем адрес модуля на шине I2C.
 		//	Проверяем значения регистров модуля:																		//
 			if(_readBytes(REG_MODEL,4)==false											){	valAddr=0; return false;}	//	Если не удалось прочитать 4 байта в массив «data» из модуля начиная с регистра «REG_MODEL», то возвращаем ошибку инициализации.
 			if( data[0]     != DEF_MODEL_EXP											){	valAddr=0; return false;}	//	Если значение  регистра «MODEL»   (data[0]) не совпадает со значением DEF_MODEL_EXP, то возвращаем ошибку инициализации.
 			if((data[2]>>1) != valAddrTemp       && data[2] !=0xFF						){	valAddr=0; return false;}	//	Если значение  регистра «ADDRESS» (data[2]) не совпадает с адресом модуля и не совпадает со значением 0xFF, то возвращаем ошибку инициализации.
+            //std::cout << int(data[3]) << '\n';
+            // та же самая история, что и строка 18,
+            // но ещё иногда наблюдается сдвиг влево
+            // this feels wrong!
+            if (data[3] != DEF_CHIP_ID_METRO)
+                    data[3] &= 0x7F;
+            if (data[3] == 0x1E)
+                    data[3] <<= 1;
 			if( data[3]     != DEF_CHIP_ID_FLASH && data[3] != DEF_CHIP_ID_METRO		){	valAddr=0; return false;}	//	Если значение  регистра «CHIP_ID» (data[3]) не совпадает со значением DEF_CHIP_ID_FLASH и DEF_CHIP_ID_METRO, то возвращаем ошибку инициализации.
 			valVers=data[1];																							//	Сохраняем байт регистра «VERSION» (data[1]) в переменую «valVers».
 		//	Перезагружаем модуль устанавливая его регистры в значение по умолчанию:										//
 			reset();																									//	Выполняем программную перезагрузку.
 			delay(5);																									//
 			return true;																								//	Возвращаем флаг успешной инициализаии.
 }																														//
```

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/iarduino_I2C_Expander.h` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.h`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/iarduino_I2C_Expander.pxd` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander.pxd`

 * *Files identical despite different names*

### Comparing `pyiArduinoI2Cexpander-0.9.9/pyiArduinoI2Cexpander/iarduino_I2C_Expander_PI.h` & `pyiArduinoI2Cexpander-1.0.1/pyiArduinoI2Cexpander/iarduino_I2C_Expander_PI.h`

 * *Files 0% similar despite different names*

```diff
@@ -59,31 +59,31 @@
 //      Функция записи одного байта в модуль:
                 bool writeByte(uint8_t adr, uint8_t data)
                 {
                         return writeBytes(adr, &data, 1);
                 }
 
 //      Функция пакетного чтения нескольких байт данных из регистров модуля:
-                bool readBytes(uint8_t addr, uint8_t reg, uint8_t *data, uint8_t sum)
+/*              bool readBytes(uint8_t addr, uint8_t reg, uint8_t *data, uint8_t sum)
                 {   // аргументы: адрес_модуля, адрес_первого_регистра, указатель_на_массив, количество_байт
                         if (ioctl(file_i2c, I2C_SLAVE, addr) < 0) return false;
                         else if ((write(file_i2c, &reg, 1) != 1)) return false;
                         else if (read(file_i2c, data, sum) != sum) return false;
                         else return true;
                 }
-    
-/*              bool readBytes(uint8_t addr, uint8_t reg, uint8_t *data, uint8_t sum)
+*/  
+                bool readBytes(uint8_t addr, uint8_t reg, uint8_t *data, uint8_t sum)
                 {  // аргументы: адрес_модуля, адрес_первого_регистра, указатель_на_массив, количество_байт
                         if (ioctl(file_i2c, I2C_SLAVE, addr) < 0) return false;
                         else if ((write(file_i2c, &reg, 1) != 1)) return false;
                         usleep(10);
                         if (read(file_i2c, data, sum) != sum) return false;
                         else return true;
                 }
-*/  
+
 //      Функция пакетного чтения нескольких байт данных из модуля:
                 bool readBytes(uint8_t addr, uint8_t *data, uint8_t sum)
                 {  // аргументы: адрес_модуля, указатель_на_массив, количество_байт
                         if (ioctl(file_i2c, I2C_SLAVE, addr) < 0) return false;
                         else if (read(file_i2c, data, sum) != sum) return false;
                         else return true;
                 }
```

### Comparing `pyiArduinoI2Cexpander-0.9.9/setup.py` & `pyiArduinoI2Cexpander-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def readme():
     with open('README.md') as readme:
         return readme.read()
 
 setup(name='pyiArduinoI2Cexpander',
-    version='0.9.9',
+    version='1.0.1',
     description='iarduino.ru module for Raspberry Pi',
     long_description=readme(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     url='http://github.com/tremaru/pyiArduinoI2Cexpander',
     author='iarduino.ru',
```

