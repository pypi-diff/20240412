# Comparing `tmp/myRIO_library-1.2.2.tar.gz` & `tmp/myRIO_library-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myRIO_library-1.2.2.tar", last modified: Wed Apr 10 08:37:46 2024, max compression
+gzip compressed data, was "myRIO_library-1.3.1.tar", last modified: Fri Apr 12 15:02:00 2024, max compression
```

## Comparing `myRIO_library-1.2.2.tar` & `myRIO_library-1.3.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.933338 myRIO_library-1.2.2/
--rw-rw-rw-   0        0        0     3283 2024-04-10 08:37:46.928359 myRIO_library-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2249 2024-03-14 22:01:02.000000 myRIO_library-1.2.2/README.md
--rw-rw-rw-   0        0        0       78 2024-03-01 11:10:42.000000 myRIO_library-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0     1273 2024-04-10 08:37:46.935323 myRIO_library-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      969 2024-04-10 08:37:35.000000 myRIO_library-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.756363 myRIO_library-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.789328 myRIO_library-1.2.2/src/myRIO_API/
--rw-rw-rw-   0        0        0       73 2024-03-11 14:39:40.000000 myRIO_library-1.2.2/src/myRIO_API/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.800328 myRIO_library-1.2.2/src/myRIO_API/examples/
--rw-rw-rw-   0        0        0     1067 2024-03-11 16:34:21.000000 myRIO_library-1.2.2/src/myRIO_API/examples/README_server.txt
--rw-rw-rw-   0        0        0      602 2024-03-11 14:24:10.000000 myRIO_library-1.2.2/src/myRIO_API/examples/myRIO_API
--rw-rw-rw-   0        0        0     5802 2024-03-14 20:37:51.000000 myRIO_library-1.2.2/src/myRIO_API/myRIO_API.py
--rw-rw-rw-   0        0        0     1099 2024-04-10 08:34:21.000000 myRIO_library-1.2.2/src/myRIO_API/version.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.815329 myRIO_library-1.2.2/src/myRIO_API_client/
--rw-rw-rw-   0        0        0       80 2024-03-12 05:47:26.000000 myRIO_library-1.2.2/src/myRIO_API_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.826327 myRIO_library-1.2.2/src/myRIO_API_client/examples/
--rw-rw-rw-   0        0        0      612 2024-03-12 09:54:55.000000 myRIO_library-1.2.2/src/myRIO_API_client/examples/README_client.txt
--rw-rw-rw-   0        0        0     1617 2024-03-14 21:54:43.000000 myRIO_library-1.2.2/src/myRIO_API_client/examples/client_examples.py
--rw-rw-rw-   0        0        0     7676 2024-03-14 20:49:39.000000 myRIO_library-1.2.2/src/myRIO_API_client/myRIO_API_client.py
--rw-rw-rw-   0        0        0     1099 2024-04-10 08:34:30.000000 myRIO_library-1.2.2/src/myRIO_API_client/version.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.843326 myRIO_library-1.2.2/src/myRIO_base/
--rw-rw-rw-   0        0        0       74 2024-03-12 09:59:59.000000 myRIO_library-1.2.2/src/myRIO_base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.858326 myRIO_library-1.2.2/src/myRIO_base/data/
--rw-rw-rw-   0        0        0  2957199 2016-12-02 19:23:24.000000 myRIO_library-1.2.2/src/myRIO_base/data/Default.lvbitx
--rw-rw-rw-   0        0        0  2906853 2022-07-10 07:27:56.000000 myRIO_library-1.2.2/src/myRIO_base/data/High-throughput.lvbitx
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.894326 myRIO_library-1.2.2/src/myRIO_base/examples/
--rw-rw-rw-   0        0        0   211136 2024-04-10 08:32:38.000000 myRIO_library-1.2.2/src/myRIO_base/examples/PacManDeath.csv
--rw-rw-rw-   0        0        0     1756 2024-03-12 10:25:50.000000 myRIO_library-1.2.2/src/myRIO_base/examples/analog-inputs-and-outputs.py
--rw-rw-rw-   0        0        0     2626 2024-03-14 22:22:02.000000 myRIO_library-1.2.2/src/myRIO_base/examples/digital-inputs-and-outputs.py
--rw-rw-rw-   0        0        0     1435 2024-03-14 21:47:14.000000 myRIO_library-1.2.2/src/myRIO_base/examples/mxp-board-tests.py
--rw-rw-rw-   0        0        0      700 2024-04-10 08:33:00.000000 myRIO_library-1.2.2/src/myRIO_base/examples/waveform-test.py
--rw-rw-rw-   0        0        0    18956 2024-04-10 08:33:27.000000 myRIO_library-1.2.2/src/myRIO_base/myRIO_base.py
--rw-rw-rw-   0        0        0     1099 2024-04-10 08:33:59.000000 myRIO_library-1.2.2/src/myRIO_base/version.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:37:46.923325 myRIO_library-1.2.2/src/myRIO_library.egg-info/
--rw-rw-rw-   0        0        0     3283 2024-04-10 08:37:46.000000 myRIO_library-1.2.2/src/myRIO_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      993 2024-04-10 08:37:46.000000 myRIO_library-1.2.2/src/myRIO_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 08:37:46.000000 myRIO_library-1.2.2/src/myRIO_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2024-04-10 08:37:46.000000 myRIO_library-1.2.2/src/myRIO_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-04-10 08:37:46.000000 myRIO_library-1.2.2/src/myRIO_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 15:02:00.851824 myRIO_library-1.3.1/
+-rw-rw-rw-   0        0        0     3283 2024-04-12 15:02:00.846840 myRIO_library-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2249 2024-03-14 22:01:02.000000 myRIO_library-1.3.1/README.md
+-rw-rw-rw-   0        0        0       78 2024-03-01 11:10:42.000000 myRIO_library-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1273 2024-04-12 15:02:00.862797 myRIO_library-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      969 2024-04-12 14:33:54.000000 myRIO_library-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:01:59.717749 myRIO_library-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 15:01:59.845407 myRIO_library-1.3.1/src/myRIO_API/
+-rw-rw-rw-   0        0        0       73 2024-03-11 14:39:40.000000 myRIO_library-1.3.1/src/myRIO_API/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:01:59.900261 myRIO_library-1.3.1/src/myRIO_API/examples/
+-rw-rw-rw-   0        0        0     1067 2024-03-11 16:34:21.000000 myRIO_library-1.3.1/src/myRIO_API/examples/README_server.txt
+-rw-rw-rw-   0        0        0      602 2024-03-11 14:24:10.000000 myRIO_library-1.3.1/src/myRIO_API/examples/myRIO_API
+-rw-rw-rw-   0        0        0     6687 2024-04-12 14:53:00.000000 myRIO_library-1.3.1/src/myRIO_API/myRIO_API.py
+-rw-rw-rw-   0        0        0     1099 2024-04-10 08:34:21.000000 myRIO_library-1.3.1/src/myRIO_API/version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:01:59.946138 myRIO_library-1.3.1/src/myRIO_API_client/
+-rw-rw-rw-   0        0        0       80 2024-03-12 05:47:26.000000 myRIO_library-1.3.1/src/myRIO_API_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:01:59.993017 myRIO_library-1.3.1/src/myRIO_API_client/examples/
+-rw-rw-rw-   0        0        0      612 2024-03-12 09:54:55.000000 myRIO_library-1.3.1/src/myRIO_API_client/examples/README_client.txt
+-rw-rw-rw-   0        0        0     1617 2024-03-14 21:54:43.000000 myRIO_library-1.3.1/src/myRIO_API_client/examples/client_examples.py
+-rw-rw-rw-   0        0        0     8153 2024-04-12 14:56:50.000000 myRIO_library-1.3.1/src/myRIO_API_client/myRIO_API_client.py
+-rw-rw-rw-   0        0        0     1099 2024-04-10 08:34:30.000000 myRIO_library-1.3.1/src/myRIO_API_client/version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:02:00.065819 myRIO_library-1.3.1/src/myRIO_base/
+-rw-rw-rw-   0        0        0       74 2024-03-12 09:59:59.000000 myRIO_library-1.3.1/src/myRIO_base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:02:00.348062 myRIO_library-1.3.1/src/myRIO_base/data/
+-rw-rw-rw-   0        0        0  2957199 2016-12-02 19:23:24.000000 myRIO_library-1.3.1/src/myRIO_base/data/Default.lvbitx
+-rw-rw-rw-   0        0        0  2906853 2022-07-10 07:27:56.000000 myRIO_library-1.3.1/src/myRIO_base/data/High-throughput.lvbitx
+drwxrwxrwx   0        0        0        0 2024-04-12 15:02:00.688267 myRIO_library-1.3.1/src/myRIO_base/examples/
+-rw-rw-rw-   0        0        0     2453 2024-04-12 14:42:07.000000 myRIO_library-1.3.1/src/myRIO_base/examples/PWM_tests.py
+-rw-rw-rw-   0        0        0   211136 2024-04-10 08:32:38.000000 myRIO_library-1.3.1/src/myRIO_base/examples/PacManDeath.csv
+-rw-rw-rw-   0        0        0     1755 2024-04-12 14:42:41.000000 myRIO_library-1.3.1/src/myRIO_base/examples/analog-inputs-and-outputs.py
+-rw-rw-rw-   0        0        0     2625 2024-04-12 14:42:45.000000 myRIO_library-1.3.1/src/myRIO_base/examples/digital-inputs-and-outputs.py
+-rw-rw-rw-   0        0        0     1434 2024-04-12 14:42:18.000000 myRIO_library-1.3.1/src/myRIO_base/examples/mxp-board-tests.py
+-rw-rw-rw-   0        0        0      708 2024-04-10 08:53:54.000000 myRIO_library-1.3.1/src/myRIO_base/examples/waveform-test.py
+-rw-rw-rw-   0        0        0    27024 2024-04-12 14:31:51.000000 myRIO_library-1.3.1/src/myRIO_base/myRIO_base.py
+-rw-rw-rw-   0        0        0     1143 2024-04-12 14:33:04.000000 myRIO_library-1.3.1/src/myRIO_base/version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:02:00.831880 myRIO_library-1.3.1/src/myRIO_library.egg-info/
+-rw-rw-rw-   0        0        0     3283 2024-04-12 15:01:59.000000 myRIO_library-1.3.1/src/myRIO_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1030 2024-04-12 15:01:59.000000 myRIO_library-1.3.1/src/myRIO_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:01:59.000000 myRIO_library-1.3.1/src/myRIO_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2024-04-12 15:01:59.000000 myRIO_library-1.3.1/src/myRIO_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-12 15:01:59.000000 myRIO_library-1.3.1/src/myRIO_library.egg-info/top_level.txt
```

### Comparing `myRIO_library-1.2.2/PKG-INFO` & `myRIO_library-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myRIO_library
-Version: 1.2.2
+Version: 1.3.1
 Summary: A library to control the myRIO board from National Instruments
 Home-page: https://github.com/AitzolEzeizaUPVEHU/myRIO_library
 Download-URL: https://github.com/AitzolEzeizaUPVEHU/myRIO_library/archive/refs/heads/main.zip
 Author: Aitzol Ezeiza Ramos
 Author-email: aitzol.ezeiza@ehu.eus
 License: MIT
 Keywords: myRIO,NI,National Instruments,LabVIEW,Python,FPGA,Real-Time,Embedded Systems
```

### Comparing `myRIO_library-1.2.2/README.md` & `myRIO_library-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/setup.cfg` & `myRIO_library-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/setup.py` & `myRIO_library-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='myRIO_library',
-version='1.2.2',
+version='1.3.1',
 author='Aitzol Ezeiza Ramos',
 author_email='aitzol.ezeiza@ehu.eus',
 description='A library to control the myRIO board from National Instruments',
 long_description=long_description,
 long_description_content_type='text/markdown',
 
 packages=find_packages('src'),
```

### Comparing `myRIO_library-1.2.2/src/myRIO_API/examples/README_server.txt` & `myRIO_library-1.3.1/src/myRIO_API/examples/README_server.txt`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/src/myRIO_API/examples/myRIO_API` & `myRIO_library-1.3.1/src/myRIO_API/examples/myRIO_API`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/src/myRIO_API/myRIO_API.py` & `myRIO_library-1.3.1/src/myRIO_API/myRIO_API.py`

 * *Files 8% similar despite different names*

```diff
@@ -133,14 +133,33 @@
     """ Returns the luminosity (percentage in float type) of
         the LDR light sensor (MXP board)
     """
     port_in = request.args.get('port', default='A', type=str)
     value = myrio_handler.read_MXP_luminosity(port=port_in)
     return jsonify({'value': value})
 
+@app.route('/mxp_luminosity', methods=['GET'])
+def get_mxp_luminosity():
+    """ Returns the luminosity (percentage in float type) of
+        the LDR light sensor (MXP board)
+    """
+    port_in = request.args.get('port', default='A', type=str)
+    value = myrio_handler.read_MXP_luminosity(port=port_in)
+    return jsonify({'value': value})
+
+
+# Extra functions: set PWM output
+@app.route('/pwm_output/<int:channel_in>/<float:value_in>', methods=['POST'])
+def set_pwm_output(channel_in: int, value_in: float):
+    """ Sets the value (duty cycle in float type) of a PWM output """
+    port_in = request.args.get('port', default='A', type=str)
+    max_value = myrio_handler.config_PWM_output(channel=channel_in, port=port_in)
+    myrio_handler.write_PWM_output(channel=channel_in, port=port_in, duty_cycle=value_in, X=max_value)
+    return jsonify({'success': True})
+
 
 if __name__ == '__main__':
     from waitress import serve
     serve(app, host='0.0.0.0', port=DEFAULT_HTTP_PORT)
     # 0.0.0.0 means it will be served in all network interfaces
 
     # Instead of serving, you can debug the application
```

### Comparing `myRIO_library-1.2.2/src/myRIO_API/version.py` & `myRIO_library-1.3.1/src/myRIO_API/version.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/src/myRIO_API_client/examples/README_client.txt` & `myRIO_library-1.3.1/src/myRIO_API_client/examples/README_client.txt`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/src/myRIO_API_client/examples/client_examples.py` & `myRIO_library-1.3.1/src/myRIO_API_client/examples/client_examples.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/src/myRIO_API_client/myRIO_API_client.py` & `myRIO_library-1.3.1/src/myRIO_API_client/myRIO_API_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,17 @@
         get_onboard_accelerometer
     
     MXP board methods:
         get_mxp_button
         set_mxp_rgb_color
         get_mxp_temperature
         get_mxp_luminosity
+    
+    Extra methods:
+        set_pwm_output
 """
 
     def __init__(self, ip_address: str=DEFAULT_HOST_IP,
                  port: int=DEFAULT_HTTP_PORT):
         self.base_url = 'http://'+ip_address+':'+str(DEFAULT_HTTP_PORT)
 
     def make_request(self, method, endpoint, data=None, params=None):
@@ -192,14 +195,24 @@
         if port_in == 'A':
             endpoint = 'mxp_luminosity'
         else:
             endpoint = 'mxp_luminosity'+'?port='+port_in
         response=self.get_data(endpoint)
         return float(response)
 
+    # Extra methods
+
+    def set_pwm_output(self, channel_in: int, value_in: float, port_in: str='A'):
+        """ Sets the value (duty cycle in float type) of a PWM output """
+        if port_in == 'A':
+            endpoint = 'analog_output/'+str(channel_in)+'/'+str(value_in)
+        else:
+            endpoint = 'analog_output/'+str(channel_in)+'/'+str(value_in)+'?port='+port_in
+        self.post_data(endpoint)
+
 
 
 if __name__ == "__main__":
     myRIO = MyRIO_API_Client()
     print('Accelerometer:')
     print(myRIO.get_onboard_accelerometer())
     print('MXP temperature')
```

### Comparing `myRIO_library-1.2.2/src/myRIO_API_client/version.py` & `myRIO_library-1.3.1/src/myRIO_API_client/version.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/src/myRIO_base/data/Default.lvbitx` & `myRIO_library-1.3.1/src/myRIO_base/data/Default.lvbitx`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/src/myRIO_base/data/High-throughput.lvbitx` & `myRIO_library-1.3.1/src/myRIO_base/data/High-throughput.lvbitx`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/src/myRIO_base/examples/PacManDeath.csv` & `myRIO_library-1.3.1/src/myRIO_base/examples/PacManDeath.csv`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.2.2/src/myRIO_base/examples/analog-inputs-and-outputs.py` & `myRIO_library-1.3.1/src/myRIO_base/examples/analog-inputs-and-outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Usage examples of the MyRIO class: analog inputs and outputs
 
-    This examples shows how to use the analog inputs and outputs
+    This examples show how to use the analog inputs and outputs
     and the onboard Accelerometer.
 
     We have a set of myRIOs in our facilities that we complement
     with some MXP cards. These cards have a temperature sensor in
     AI0 and a Light sensor in AI1. We use these channels
     in our examples. The port that we use most is the A port, so
     we set it as default on our package.
```

### Comparing `myRIO_library-1.2.2/src/myRIO_base/examples/digital-inputs-and-outputs.py` & `myRIO_library-1.3.1/src/myRIO_base/examples/digital-inputs-and-outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Usage examples of the MyRIO class: digital inputs and outputs
 
-    This examples shows how to use the DIO ports and the
+    This examples show how to use the DIO ports and the
     onboard button and LEDs.
 
     We have a set of myRIOs in our facilities that we complement
     with some MXP cards. These cards have an RGB LED connected to
     DIO_2:0 and two push buttons on DIO_4:3. We use these channels
     in our examples. The port that we use most is the A port, so
     we set it as default on our package.
```

### Comparing `myRIO_library-1.2.2/src/myRIO_base/examples/mxp-board-tests.py` & `myRIO_library-1.3.1/src/myRIO_base/examples/mxp-board-tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Usage examples of the MyRIO class: MXP board tests
 
-    This examples shows how to use the electronic components
+    This examples show how to use the electronic components
     we already have on our MXP boards. It serves as example of
     more sophisticated functions we added to myRIO_base.
 
     Our MXP cards have an RGB LED connected to DIO_2:0 and 
     two push buttons on DIO_4:3. We also have an NTC temperature
     sensor in AI0 and an LDR light sensor in AI1. We use these
     channels in our examples. The port that we use most is the
```

### Comparing `myRIO_library-1.2.2/src/myRIO_base/examples/waveform-test.py` & `myRIO_library-1.3.1/src/myRIO_base/examples/waveform-test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 
 myrio1 = myRIO.MyRIO()
 
 # Play a simple waveform using raw data
 print("Playing a simple waveform")
 csv_file = pkg_resources.resource_filename('myRIO_base', 'examples/PacManDeath.csv')
 print("Waveform file: ", csv_file)
-my_waveform = extract_waveform_from_csv_file(csv_file)
-myrio1.play_waveform(my_waveform)
+my_waveform = myRIO.extract_waveform_from_csv_file(csv_file)
+myrio1.play_waveform(my_waveform)
```

### Comparing `myRIO_library-1.2.2/src/myRIO_base/myRIO_base.py` & `myRIO_library-1.3.1/src/myRIO_base/myRIO_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -167,14 +167,38 @@
         dir_string_low = 'DIO.' + port + '_' + '7:0' + '.DIR'
         dir_string_high = 'DIO.' + port + '_' + '15:8' + '.DIR'
         mask_handler_low = self.__session.registers[dir_string_low]
         mask_handler_high = self.__session.registers[dir_string_high]
         mask_handler_low.write(mask_low)    # 7 is 00000111 where 1 is OUT
         mask_handler_high.write(mask_high)    # 0 is 00000000 where 0 is IN
 
+    def update_DIO_mask(self, channel: int, is_output: bool, port: str ='A'):
+        """ Updates the current DIO mask to change the behaviour of one channe """
+
+        dir_string_low = 'DIO.' + port + '_' + '7:0' + '.DIR'
+        dir_string_high = 'DIO.' + port + '_' + '15:8' + '.DIR'
+        mask_handler_low = self.__session.registers[dir_string_low]
+        mask_handler_high = self.__session.registers[dir_string_high]
+        current_dio_mask_low = mask_handler_low.read()
+        current_dio_mask_high = mask_handler_high.read()
+
+        if is_output:  # change channel direction to output
+            if channel < 8:
+                new_dio_mask_low = only_one_bit_on(channel,current_dio_mask_low)
+                mask_handler_low.write(new_dio_mask_low)
+            else:
+                new_dio_mask_high = only_one_bit_on(channel-8,current_dio_mask_high)
+                mask_handler_high.write(new_dio_mask_high)
+        else:
+            if channel < 8:
+                new_dio_mask_low = only_one_bit_off(channel,current_dio_mask_low)
+                mask_handler_low.write(new_dio_mask_low)
+            else:
+                new_dio_mask_high = only_one_bit_off(channel-8,current_dio_mask_high)
+                mask_handler_high.write(new_dio_mask_high)
 
     def read_analog_input(self, channel: int, port: str ='A') -> float:
         """ returns the value in volts of one of the AI channels (default port: A) """
     
         channel_string = 'AI.' + port + '_' + str(channel) + '.VAL'
         channel_handler = self.__session.registers[channel_string]
         if port=='A' or port == 'B':
@@ -397,14 +421,39 @@
         else:
             #TODO how to report the exception (port name error)
             raw_value = 0
         channel_handler.write(raw_value)
         go_handler = self.__session.registers['AO.SYS.GO']
         go_handler.write(True)
 
+    def read_audio_input(self, channel: str='L') -> float:
+        """ returns the value in volts of one of the Audio Input channels """
+        if channel == 'L' or channel == 'R':
+            channel_string = 'AI.AudioIn_' + str(channel) + '.VAL'
+        else:
+            #TODO how to report the exception (channel name error)
+            channel_string = 'AI.AudioIn_L.VAL'
+        
+        channel_handler = self.__session.registers[channel_string]
+        return raw_to_volts_audio(channel_handler.read())
+
+    def write_audio_output(self, value: float, channel: str='L'):
+        """ writes a value (in volts) on an Audio Output channel """
+        if channel == 'L' or channel == 'R':
+            channel_string = 'AO.AudioOut_' + str(channel) + '.VAL'
+        else:
+            #TODO how to report the exception (channel name error)
+            channel_string = 'AO.AudioOut_L.VAL'
+        
+        channel_handler = self.__session.registers[channel_string]
+        raw_value = volts_to_raw_audio(value)
+        channel_handler.write(raw_value)
+        go_handler = self.__session.registers['AO.SYS.GO']
+        go_handler.write(True)
+
     def play_waveform(self, waveform: [int]):
         """ plays a waveform on the myRIO Audio Output channels """
     
         channel_string_left = 'AO.AudioOut_L.VAL'
         channel_string_right = 'AO.AudioOut_R.VAL'
         channel_handler_left = self.__session.registers[channel_string_left]
         channel_handler_right = self.__session.registers[channel_string_right]
@@ -412,22 +461,121 @@
         go_handler = self.__session.registers['AO.SYS.GO']
 
         for i in range(len(waveform)):
             channel_handler_left.write(waveform[i])
             channel_handler_right.write(waveform[i])
             go_handler.write(True)
 
+    def read_audio_input_noise_level(self) -> float:
+        """ returns the noise level % of the Audio Input channels """
+        window_size = 100
+        max_volts = 2.5
+
+        channel_string_L = 'AI.AudioIn_L.VAL'
+        channel_string_R = 'AI.AudioIn_R.VAL'
+        
+        channel_handler_L = self.__session.registers[channel_string_L]
+        channel_handler_R = self.__session.registers[channel_string_R]
+
+        noise_level_sum = 0.0
+        for i in range(window_size):
+            volume_L = raw_to_volts_audio(channel_handler_L.read())
+            volume_R = raw_to_volts_audio(channel_handler_R.read())
+            noise_level_sum += abs(volume_L) + abs(volume_R)
+
+        mean_value = noise_level_sum / (2*window_size)
+        return mean_value * 100.0 / max_volts
+
+    def config_PWM_output(self, channel: int, frequency: float=2000.0, port: str ='A') -> int:
+        """ configs a PWM output to work with a certain frequency (default port: A)
+            The frequency should be expressed in Hz (default 2000 Hz).
+            The range of frequency is 40Hz-40KHz 
+            Returns X (the value of the MAX register)
+        """
+        BASE_FREQUENCY = 40000000.0
+
+        if (frequency < 40.0) or (frequency > 40000.0):
+            raise Exception('Frequency out of range (40Hz-40KHz)')
+        elif frequency < 80.0 :
+            divider_N = 16
+            divider_code = 5
+        elif frequency < 160.0 :
+            divider_N = 8
+            divider_code = 4
+        elif frequency < 320.0 :
+            divider_N = 4
+            divider_code = 3
+        elif frequency < 800.0 :
+            divider_N = 2
+            divider_code = 2
+        else:
+            divider_N = 1
+            divider_code = 1
+        
+        max_value_X = int((BASE_FREQUENCY/frequency)/divider_N)-1
+        
+        self.update_DIO_mask(channel=8, is_output=True, port='B')
+        self.update_DIO_mask(channel=9, is_output=True, port='B')
+        self.update_DIO_mask(channel=10, is_output=True, port='B')
+
+        channel_string_sys = 'SYS.SELECT' + port
+        channel_handler_sys = self.__session.registers[channel_string_sys]
+        current_value = channel_handler_sys.read()
+        new_value = only_one_bit_on(bit_number=channel+2, input_number=current_value)
+        channel_handler_sys.write(new_value)
+        
+        channel_string_cnfg = 'PWM.' + port + '_' + str(channel) + '.CNFG'
+        channel_handler_cnfg = self.__session.registers[channel_string_cnfg]
+        channel_handler_cnfg.write(4)
+
+        channel_string_cs = 'PWM.' + port + '_' + str(channel) + '.CS'
+        channel_handler_cs = self.__session.registers[channel_string_cs]
+        channel_handler_cs.write(divider_code)
+
+        channel_string_max = 'PWM.' + port + '_' + str(channel) + '.MAX'
+        channel_handler_max = self.__session.registers[channel_string_max]
+        channel_handler_max.write(max_value_X)
+        return max_value_X
+
+
+    def write_PWM_output(self, channel: int, duty_cycle: float, X: int=19999, port: str ='A'):
+        """ writes a duty cycle value (in percentage) on a PWM channel (default port: A) """
+
+        duty_cycle_code = int((duty_cycle/100) * (X+1)) # X is the MAX value of the PWM counter
+
+        channel_string_cmp = 'PWM.' + port + '_' + str(channel) + '.CMP'
+        channel_handler_cmp = self.__session.registers[channel_string_cmp]
+        channel_handler_cmp.write(duty_cycle_code)
+
+    def display_color_PWM(self, R: int=0, G: int=0, B: int=0):
+        """ This is not a generic function, it is only an example.
+            It uses the PWM channels in port B to control an RGB
+            LED display. The frequencies of each channel and the resistors
+            used in the circuit are specific for each RGB LED display.
+        """
+
+        duty_cycle_R = int(R * 100 / 256)
+        duty_cycle_G = int(G * 100 / 256)
+        duty_cycle_B = int(B * 100 / 256)
+        
+        X_0 = self.config_PWM_output(channel=0, frequency=5000.0,port='B')
+        X_1 = self.config_PWM_output(channel=1, port='B')
+        X_2 = self.config_PWM_output(channel=2, port='B')
+        self.write_PWM_output(channel=0, duty_cycle=duty_cycle_R, X=X_0, port='B')
+        self.write_PWM_output(channel=1, duty_cycle=duty_cycle_G, X=X_1, port='B')
+        self.write_PWM_output(channel=2, duty_cycle=duty_cycle_B, X=X_2, port='B')
+
+
 if __name__ == "__main__":
     print("This is a library for working with NI myRIO in Python")
     print("It is not intended to be run directly, but to be imported in other programs.")
     print("Please, see the documentation for more information.")
     from time import sleep
     myrio1 = MyRIO()
 
-    
     print("Read digital port A:")
     print(myrio1.read_digital_port(port='A'))
     print("Read temperature from MXP port A, channel 0:")
     print(myrio1.read_MXP_temperature())
     print("Read luminosity from MXP port A, channel 1:")
     print(myrio1.read_MXP_luminosity())
     print("RGB LED in MXP port A: RED")
@@ -437,44 +585,73 @@
     myrio1.write_MXP_RGB_LED(GREEN)
     sleep(1)
     print("RGB LED in MXP port A: BLUE")
     myrio1.write_MXP_RGB_LED(BLUE)
     sleep(1)
     print("RGB LED in MXP port A: OFF")
     myrio1.write_MXP_RGB_LED(RGB_OFF)
-
     
-    # Play a simple waveform (2024/04/10)
+    # Play a simple waveform using raw data
     print("Playing a simple waveform")
     csv_file = pkg_resources.resource_filename('myRIO_base', 'examples/PacManDeath.csv')
     my_waveform = extract_waveform_from_csv_file(csv_file)
     myrio1.play_waveform(my_waveform)
 
+    # Get the noise level of the Audio Input channels
+    print("Noise level of the Audio Input channels:")
+    print(myrio1.read_audio_input_noise_level())
+
+    # Test the PWM outputs
+    print("PWM output test (port B: PWM0, PWM1, PWM2):")
+    print("Configuring...")
+    X_0 = myrio1.config_PWM_output(channel=0, frequency=5000.0,port='B')
+    X_1 = myrio1.config_PWM_output(channel=1, port='B')
+    X_2 = myrio1.config_PWM_output(channel=2, port='B')
+
+    print("10% 45% 11,5%")
+    myrio1.write_PWM_output(channel=0, duty_cycle=10, X=X_0, port='B')
+    myrio1.write_PWM_output(channel=1, duty_cycle=45, X=X_1, port='B')
+    myrio1.write_PWM_output(channel=2, duty_cycle=11.5, X=X_2, port='B')
+    sleep(2)
+
+    print("0% 0% 0%")
+    myrio1.write_PWM_output(channel=0, duty_cycle=0.0, port='B')
+    myrio1.write_PWM_output(channel=1, duty_cycle=0.0, port='B')
+    myrio1.write_PWM_output(channel=2, duty_cycle=0.0, port='B')
+    
+
+    print("Display RGB color orange (252, 161, 3):")
+    myrio1.display_color_PWM(252,161,3)
+    sleep(10)
+    myrio1.display_color_PWM(0,0,0)
+
+        
 
 
         
 """ TODO
 
 There are some extra features that we do not cover.
 They are interesting, but are not so commonly used, and given
 their complexity, we leave them for future development.
 The features we did not cover are:
-1.-PWM and ENC
+1.-ENC
 2.-I2C and SPI
 3.-IRQs
 
 It would be interesting too to improve the audio functions.
+They are very simple and it does not seem straightforward
+to improve them.
 """
 
 """ Credits
 This library has been developed from scratch by Aitzol Ezeiza Ramos
 from the University of the Basque Country (UPV/EHU)
 It is strongly based on nifpga the basic library for accessing the
 FPGA on NI RIO devices.
 
 https://github.com/ni/nifpga-python/
 
-We also use typing and ctypes.
 
 First version: 2024/02/28
-Current version: 2024/03/14
+Current version: 2024/04/12
 """
```

### Comparing `myRIO_library-1.2.2/src/myRIO_base/version.py` & `myRIO_library-1.3.1/src/myRIO_base/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # version.py
-__version__ = "1.2.2"
+__version__ = "1.3.1"
 
 """ version notes
 0.2.0: added __del__ method to myRio class to close the connection
        to the myRIO (2024/03/05)
 0.2.3: fixed the Default.lvbitx error: now the file is distributed 
        with the package. We use the relative folder of __file__ (2024/3/6)
 0.3.0: Added examples. Fixed a bug in the digital write function. (2024/3/7)
@@ -14,8 +14,9 @@
 1.0.2: minor change in the API client examples (2024/03/12)
 1.0.3: GitHub Actions (2024/03/14)
 1.1.0: MXP functions added to base, API and API client(2024/03/15)
 1.1.1: MXP function testing bugs fixed (2024/03/15)
 1.1.2: Bug fix: examples folder was not being copied to the site-packages (2024/03/15)
 1.2.1: Added play_waveform function to the myRIO class (2024/04/10)
 1.2.2: Minor fix in waveform example (2024/04/10)
+1.3.1: Added PWM capabilities (2024/04/12)
 """
```

### Comparing `myRIO_library-1.2.2/src/myRIO_library.egg-info/PKG-INFO` & `myRIO_library-1.3.1/src/myRIO_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myRIO_library
-Version: 1.2.2
+Version: 1.3.1
 Summary: A library to control the myRIO board from National Instruments
 Home-page: https://github.com/AitzolEzeizaUPVEHU/myRIO_library
 Download-URL: https://github.com/AitzolEzeizaUPVEHU/myRIO_library/archive/refs/heads/main.zip
 Author: Aitzol Ezeiza Ramos
 Author-email: aitzol.ezeiza@ehu.eus
 License: MIT
 Keywords: myRIO,NI,National Instruments,LabVIEW,Python,FPGA,Real-Time,Embedded Systems
```

### Comparing `myRIO_library-1.2.2/src/myRIO_library.egg-info/SOURCES.txt` & `myRIO_library-1.3.1/src/myRIO_library.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/myRIO_API_client/examples/README_client.txt
 src/myRIO_API_client/examples/client_examples.py
 src/myRIO_base/__init__.py
 src/myRIO_base/myRIO_base.py
 src/myRIO_base/version.py
 src/myRIO_base/data/Default.lvbitx
 src/myRIO_base/data/High-throughput.lvbitx
+src/myRIO_base/examples/PWM_tests.py
 src/myRIO_base/examples/PacManDeath.csv
 src/myRIO_base/examples/analog-inputs-and-outputs.py
 src/myRIO_base/examples/digital-inputs-and-outputs.py
 src/myRIO_base/examples/mxp-board-tests.py
 src/myRIO_base/examples/waveform-test.py
 src/myRIO_library.egg-info/PKG-INFO
 src/myRIO_library.egg-info/SOURCES.txt
```

