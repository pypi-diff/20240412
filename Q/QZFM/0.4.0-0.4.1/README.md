# Comparing `tmp/QZFM-0.4.0.tar.gz` & `tmp/QZFM-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QZFM-0.4.0.tar", last modified: Mon Mar 18 20:50:54 2024, max compression
+gzip compressed data, was "QZFM-0.4.1.tar", last modified: Fri Apr 12 15:40:15 2024, max compression
```

## Comparing `QZFM-0.4.0.tar` & `QZFM-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2024-03-18 20:50:54.688408 QZFM-0.4.0/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2024-01-10 20:24:12.000000 QZFM-0.4.0/LICENSE
--rw-r--r--   0 dfujimoto  (1000) dfujimoto  (1000)    10294 2024-03-18 20:50:54.688408 QZFM-0.4.0/PKG-INFO
--rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)     9526 2024-01-15 17:36:24.000000 QZFM-0.4.0/README.md
--rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)      828 2024-03-18 20:49:40.000000 QZFM-0.4.0/pyproject.toml
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2024-03-18 20:50:54.688408 QZFM-0.4.0/setup.cfg
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2024-03-18 20:50:54.684408 QZFM-0.4.0/src/
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2024-03-18 20:50:54.684408 QZFM-0.4.0/src/QZFM/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     6986 2024-01-12 21:23:16.000000 QZFM-0.4.0/src/QZFM/LabJack.py
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    40289 2024-03-18 20:48:29.000000 QZFM-0.4.0/src/QZFM/QZFM.py
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       70 2024-01-10 20:23:42.000000 QZFM-0.4.0/src/QZFM/__init__.py
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2024-03-18 20:50:54.688408 QZFM-0.4.0/src/QZFM.egg-info/
--rw-r--r--   0 dfujimoto  (1000) dfujimoto  (1000)    10294 2024-03-18 20:50:54.000000 QZFM-0.4.0/src/QZFM.egg-info/PKG-INFO
--rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)      249 2024-03-18 20:50:54.000000 QZFM-0.4.0/src/QZFM.egg-info/SOURCES.txt
--rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)        1 2024-03-18 20:50:54.000000 QZFM-0.4.0/src/QZFM.egg-info/dependency_links.txt
--rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)       62 2024-03-18 20:50:54.000000 QZFM-0.4.0/src/QZFM.egg-info/requires.txt
--rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)        5 2024-03-18 20:50:54.000000 QZFM-0.4.0/src/QZFM.egg-info/top_level.txt
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2024-04-12 15:40:15.459522 QZFM-0.4.1/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2024-01-10 20:24:12.000000 QZFM-0.4.1/LICENSE
+-rw-r--r--   0 dfujimoto  (1000) dfujimoto  (1000)    10294 2024-04-12 15:40:15.459522 QZFM-0.4.1/PKG-INFO
+-rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)     9526 2024-01-15 17:36:24.000000 QZFM-0.4.1/README.md
+-rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)      828 2024-04-12 15:39:16.000000 QZFM-0.4.1/pyproject.toml
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2024-04-12 15:40:15.459522 QZFM-0.4.1/setup.cfg
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2024-04-12 15:40:15.455522 QZFM-0.4.1/src/
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2024-04-12 15:40:15.455522 QZFM-0.4.1/src/QZFM/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     6986 2024-01-12 21:23:16.000000 QZFM-0.4.1/src/QZFM/LabJack.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    47177 2024-04-12 15:39:01.000000 QZFM-0.4.1/src/QZFM/QZFM.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       70 2024-01-10 20:23:42.000000 QZFM-0.4.1/src/QZFM/__init__.py
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2024-04-12 15:40:15.459522 QZFM-0.4.1/src/QZFM.egg-info/
+-rw-r--r--   0 dfujimoto  (1000) dfujimoto  (1000)    10294 2024-04-12 15:40:15.000000 QZFM-0.4.1/src/QZFM.egg-info/PKG-INFO
+-rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)      249 2024-04-12 15:40:15.000000 QZFM-0.4.1/src/QZFM.egg-info/SOURCES.txt
+-rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)        1 2024-04-12 15:40:15.000000 QZFM-0.4.1/src/QZFM.egg-info/dependency_links.txt
+-rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)       62 2024-04-12 15:40:15.000000 QZFM-0.4.1/src/QZFM.egg-info/requires.txt
+-rwxr-xr-x   0 dfujimoto  (1000) dfujimoto  (1000)        5 2024-04-12 15:40:15.000000 QZFM-0.4.1/src/QZFM.egg-info/top_level.txt
```

### Comparing `QZFM-0.4.0/LICENSE` & `QZFM-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QZFM-0.4.0/PKG-INFO` & `QZFM-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QZFM
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python class for serial communication with QuSpin Zero Field Magnetometer
 Author-email: Derek Fujimoto <dfujimoto@triumf.ca>
 Project-URL: Homepage, https://github.com/ucn-triumf/QZFM
 Project-URL: Bug Tracker, https://github.com/ucn-triumf/QZFM/issues
 Keywords: QZFM,QuSpin,Magnetometer,Zero Field
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `QZFM-0.4.0/README.md` & `QZFM-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `QZFM-0.4.0/pyproject.toml` & `QZFM-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "QZFM"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Derek Fujimoto", email="dfujimoto@triumf.ca" },
 ]
 description = "Python class for serial communication with QuSpin Zero Field Magnetometer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `QZFM-0.4.0/src/QZFM/LabJack.py` & `QZFM-0.4.1/src/QZFM/LabJack.py`

 * *Files identical despite different names*

### Comparing `QZFM-0.4.0/src/QZFM/QZFM.py` & `QZFM-0.4.1/src/QZFM/QZFM.py`

 * *Files 22% similar despite different names*

```diff
@@ -58,17 +58,18 @@
                         'stopbits':     1,
                         'write_timeout':10,     # seconds
                         'xonxoff':      False,
                         'rtscts':       False,
                         'dsrdtr':       False,
                         }
 
-    data_read_rate = 200 # Hz
+    data_read_rate = 200 # Hz reading rate from digital output
+    status_read_rate = 7.5 # Hz reading rate from status of sensor, including compensation coil values
     zero_wait_duration = 5 # seconds, time waiting for zeroing to succeed
-
+    
     def __init__(self, device_name=None, nbytes_status=1000):
         """Args:
             device_name (str): name of device to look for (connection)
                                 for windows this is likely COM3 or COM5
                                 for linux, search Z3T0 or similar
             nbytes_status (int): serial read chunk size in bytes for status updates
         """
@@ -208,22 +209,22 @@
         elif axis == 'z':   self.ser.write(b'?')
         else:
             raise RuntimeError(f'Unknown axis "{axis}"')
 
         self.read_axis = axis
         self._get_next_message()
 
-    def auto_start(self, block=True, show=True, zero_calibrate=True):
+    def auto_start(self, block=True, show=True, zero_calibrate=True, zero_cond = 100):
         """Initiate the automated sensor startup routines
 
         Args:
             block (bool): if True, wait until laser is locked and temperature stabilized before unblocking
             show (bool): print status continuously to screen until finished
             zero_calibrate (bool): if true, also field zero and calibrate the sensor. Forces block = True
-
+            zero_cond: field zeroing goal/stopping condition, in units of pT/s. The field zeroing will terminate after the set stability is reached for 5 consecutive seconds
         Returns:
             None
         """
 
         # start autostart
         self.ser.write(b'>')
 
@@ -235,59 +236,85 @@
             while not self.led["laser lock (LED3)"] or not self.led["cell temp lock (LED2)"]:
                 self.update_status(clear_buffer=False)
                 if show:
                     self.print_status(overwrite_last=True)
 
         # field zero and calibrate
         if zero_calibrate:
-
+            
+            # lists to hold compensation coil fields and time stamps
+            x_comp, y_comp, z_comp = [], [], []
+            t = []
+            
             # start field zero
             print('\nField zeroing...')
             self.field_zero(show=False)
 
-            # wait 5 seconds
+            #zero until field is stable (fluctuate less than 200 pT/s for 5 consecutive differences)
             self.update_status()
             self.print_status(print_last_message=False)
-            for i in range(self.zero_wait_duration):
-                sleep(1)
+            while len(x_comp) < 6 and len(y_comp) < 6 and len(z_comp) < 6:
                 self.update_status()
                 self.print_status(print_last_message=False, overwrite_last=True)
-
-            # check stability over wait duration
-            temp_lock_ok = False
-            temp_err_ok = False
-
-            t0 = time()
-            while temp_lock_ok and temp_err_ok and (time.time() - t0 > self.zero_wait_duration):
-
-                # check temperature lock
-                temp_lock_ok = self.led['cell temp lock (LED2)']
-
-                # check temperature error
-                temp_err_ok = self.sensor_par['cell temp error'] <= 0.001
-
-                # reset timer
-                if not temp_lock_ok or not temp_err_ok:
-                    t0 = time()
-
-                self.update_status()
-                self.print_status(overwrite_last=True, print_last_message=False)
+                t.append(self.status_last_updated)
+                x_comp.append(self.sensor_par['B0 field (pT)'])
+                y_comp.append(self.sensor_par['By field (pT)'])
+                z_comp.append(self.sensor_par['Bz field (pT)'])
+            
+            zeroed = False
+            while not zeroed:
+                # calculate field gradients (pT/s) 
+                # difference in times
+                t_diff = [j-i for i, j in zip(t[-5:][:-1], t[-5:][1:])]
+                
+                # differences in fields
+                x_diff = [j-i for i, j in zip(x_comp[-5:][:-1], x_comp[-5:][1:])]
+                y_diff = [j-i for i, j in zip(y_comp[-5:][:-1], y_comp[-5:][1:])]
+                z_diff = [j-i for i, j in zip(z_comp[-5:][:-1], z_comp[-5:][1:])]
+                
+                # calculate gradients
+                x_grad = [i/j for i, j in zip(x_diff, t_diff)]
+                y_grad = [i/j for i, j in zip(y_diff, t_diff)]
+                z_grad = [i/j for i, j in zip(z_diff, t_diff)]
+                
+                # check if gradients satisfy condition
+                if all(x < zero_cond for x in x_grad) and all(y < zero_cond for y in y_grad) and all(z < zero_cond for z in z_grad):
+                    zeroed = True
+                else:
+                    self.update_status()
+                    self.print_status(print_last_message=False, overwrite_last=True)
+                    t.append(self.status_last_updated)
+                    x_comp.append(self.sensor_par['B0 field (pT)'])
+                    y_comp.append(self.sensor_par['By field (pT)'])
+                    z_comp.append(self.sensor_par['Bz field (pT)'])
 
             # stop and print zeroing values
             self.field_zero(False)
             self.update_status()
             self.print_status(overwrite_last=True, print_last_message=False)
             print('Field zeroing finished.')
-
+            
+            
+            # field zeroing destroys temp_err, wait until temp err stabilizes again
+            print('Re-establishing cell temp lock')
+            temp_err_ok = False
+            temp_err_last = np.inf
+            while not temp_err_ok:
+                temp_err_ok = abs(self.sensor_par['cell temp error']) <= 0.001 or abs(temp_err_last-self.sensor_par['cell temp error']) <= 0.001
+                temp_err_last = self.sensor_par['cell temp error']
+                self.update_status()
+                print('Cell T error: {}\n Cell T error change: {}\n'.format(self.sensor_par['cell temp error'],
+                                                                            abs(temp_err_last-self.sensor_par['cell temp error'])))
+                
             # start calibrate
             print('\nCalibrating...')
             self.calibrate()
 
             # save data
-            self.save_state()
+            self.save_state()    
 
     def calibrate(self, show=True):
         """Calibrate the response (field to voltage) of the magnetometer with an internal signal reference
 
         Args:
             show (bool): if true, print to screen
         """
@@ -692,15 +719,15 @@
                     print('\033[F'*(nlines+1))
 
         except KeyboardInterrupt:
             # save data
             self.time = t
             self.field = y
             print()
-
+    
     def monitor_status(self):
         """Continuously update and print status"""
 
         # do first update
         self.update_status()
         self.print_status()
 
@@ -708,14 +735,149 @@
         try:
             while True:
                 self.update_status(clear_buffer=False)
                 self.print_status(overwrite_last=True)
         except KeyboardInterrupt:
             print()
 
+    def monitor_zeroing(self, window_s=20, figsize=(10, 6)):
+        """Continuously stream compensation coil fields to figure
+
+            See https://matplotlib.org/stable/tutorials/advanced/blitting.html
+
+        Args:
+            window_s (int): show the last window_s seconds of data on the stream
+            figsize (tuple): size of display
+        """
+
+        # get initial point
+        self.update_status()
+
+        # make figure
+        fig, ax = plt.subplots(figsize=figsize)
+
+        # draw initial window
+        x = np.array([self.status_last_updated])
+        bx = np.array([self.sensor_par['B0 field (pT)']]) 
+        by = np.array([self.sensor_par['By field (pT)']])
+        bz = np.array([self.sensor_par['Bz field (pT)']])
+        
+        (line_x,) = plt.plot(np.zeros(1), bx, animated=True, marker='o', fillstyle='none')
+        (line_y,) = plt.plot(np.zeros(1), by, animated=True, marker='o', fillstyle='none')
+        (line_z,) = plt.plot(np.zeros(1), bz, animated=True, marker='o', fillstyle='none')
+
+        # plot elements
+        plt.ylabel(f'Compensation Field (pT)')
+        plt.xlabel(f'Time (s)')
+        plt.tight_layout()
+
+        # render
+        plt.show(block=False)
+        plt.pause(0.05)
+
+        # get bounding box
+        bg = fig.canvas.copy_from_bbox(fig.bbox)
+
+        # draw
+        ax.draw_artist(line_x)
+        ax.draw_artist(line_y)
+        ax.draw_artist(line_z)
+
+        # show
+        fig.canvas.blit(fig.bbox)
+
+        # set x bounds
+        ax.set_xlim(-window_s*1.1, window_s*0.1)
+
+        # get bounds
+        ylim = ax.get_ylim()
+        xlim = ax.get_xlim()
+
+        # start zeroing
+        self.field_zero(show=False)
+        
+        try:
+            # draw forever
+            while True:
+
+                # get data
+                self.update_status(clear_buffer=True)
+                bx_new = self.sensor_par['B0 field (pT)']
+                by_new = self.sensor_par['By field (pT)']
+                bz_new = self.sensor_par['Bz field (pT)']
+                t = self.status_last_updated
+
+                x = np.append(x, t)
+                bx = np.append(bx, bx_new)
+                by = np.append(by, by_new)
+                bz = np.append(bz, bz_new)
+                dx = x-t
+
+                # check data limits
+                idx = np.abs(dx) < window_s
+                x = x[idx]
+                bx = bx[idx]
+                by = by[idx]
+                bz = bz[idx]
+                dx = dx[idx]
+
+                # check for figure
+                if not plt.fignum_exists(fig.number):
+                    break
+
+                # if out of bounds, redraw
+                if not (max(max(bx), max(by), max(bz)) < ylim[1] and min(min(bx), min(by), min(bz)) > ylim[0]) or not (max(dx) < xlim[1] and min(dx) > xlim[0]):
+                    plt.cla()
+                    (line_x,) = plt.plot(dx, bx, animated=True, marker='o', fillstyle='none')
+                    (line_y,) = plt.plot(dx, by, animated=True, marker='o', fillstyle='none')
+                    (line_z,) = plt.plot(dx, bz, animated=True, marker='o', fillstyle='none')
+
+                    # plot elements
+                    plt.ylabel(f'Compensation Field (pT)')
+                    plt.xlabel(f'Time (s)')
+                    plt.tight_layout()
+
+                    # redraw
+                    plt.pause(0.05)
+                    bg = fig.canvas.copy_from_bbox(fig.bbox)
+                    ax.draw_artist(line_x)
+                    ax.draw_artist(line_y)
+                    ax.draw_artist(line_z)
+                    fig.canvas.blit(fig.bbox)
+
+                else:
+                    # reset background
+                    fig.canvas.restore_region(bg)
+
+                    # set data
+                    line_x.set_xdata(dx)
+                    line_x.set_ydata(bx)
+                    ax.draw_artist(line_x)
+                    
+                    line_y.set_xdata(dx)
+                    line_y.set_ydata(by)
+                    ax.draw_artist(line_y)
+                    
+                    line_z.set_xdata(dx)
+                    line_z.set_ydata(bz)
+                    ax.draw_artist(line_z)
+
+                # update screen
+                fig.canvas.blit(fig.bbox)
+                fig.canvas.flush_events()
+
+                # print n events in buffer
+                # print(f'N events remaining in buffer: {self.ser.in_waiting}',
+                #       flush=True, end='\r')
+
+        except KeyboardInterrupt:
+            self.field_zero(False)
+            print('Field zeroing off')
+            print()
+            
     def print_messages(self, last_n=None):
         """Print messages to screen
 
         Args:
             last_n (float|None): print the last_n number of messages. If None, print all.
         """
 
@@ -1053,34 +1215,34 @@
             self.gain = 2.7     # V/nT
 
         elif mode == '3x':
             self.ser.write(b'b')
             self.gain = 8.1     # V/nT
 
         elif mode == '0.1x':
-            self.ser.write(30)
+            self.ser.write(b'x1e')
             self.gain = 0.27     # V/nT
 
         else:
-            raise RuntimeError(f'Bad gain setting ("{gain}"), must be 0.1x|0.33x|1x|3x')
+            raise RuntimeError(f'Bad gain setting ("{mode}"), must be 0.1x|0.33x|1x|3x')
 
         # print gain set
         self._get_next_message(timeout=10)
         self.print_messages(1)
 
     def set_master(self, master=True):
         """Set master/slave status
 
         Args:
             master (bool): If true set as master, else set as slave
         """
         if master:
-            self.ser.write(113)
+            self.ser.write(b'q')
         else:
-            self.ser.write(114)
+            self.ser.write(b'r')
 
     def to_csv(self, filename=None, *notes):
         """Write data to csv, if no filename, use default
 
         Args:
             filename (str): name of file to write
             notes: things to add to file header
```

### Comparing `QZFM-0.4.0/src/QZFM.egg-info/PKG-INFO` & `QZFM-0.4.1/src/QZFM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QZFM
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python class for serial communication with QuSpin Zero Field Magnetometer
 Author-email: Derek Fujimoto <dfujimoto@triumf.ca>
 Project-URL: Homepage, https://github.com/ucn-triumf/QZFM
 Project-URL: Bug Tracker, https://github.com/ucn-triumf/QZFM/issues
 Keywords: QZFM,QuSpin,Magnetometer,Zero Field
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

