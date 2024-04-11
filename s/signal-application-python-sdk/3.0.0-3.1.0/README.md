# Comparing `tmp/signal-application-python-sdk-3.0.0.tar.gz` & `tmp/signal-application-python-sdk-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-application-python-sdk-3.0.0.tar", last modified: Fri Jan 26 19:50:57 2024, max compression
+gzip compressed data, was "signal-application-python-sdk-3.1.0.tar", last modified: Thu Apr 11 23:07:13 2024, max compression
```

## Comparing `signal-application-python-sdk-3.0.0.tar` & `signal-application-python-sdk-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 19:50:57.458499 signal-application-python-sdk-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-01-26 19:50:57.458499 signal-application-python-sdk-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 19:50:57.458499 signal-application-python-sdk-3.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1719 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 19:50:57.458499 signal-application-python-sdk-3.0.0/signal_application_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-01-26 19:50:57.000000 signal-application-python-sdk-3.0.0/signal_application_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-01-26 19:50:57.000000 signal-application-python-sdk-3.0.0/signal_application_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 19:50:57.000000 signal-application-python-sdk-3.0.0/signal_application_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-26 19:50:57.000000 signal-application-python-sdk-3.0.0/signal_application_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-26 19:50:57.000000 signal-application-python-sdk-3.0.0/signal_application_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 19:50:57.458499 signal-application-python-sdk-3.0.0/signalsdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/signalsdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/signalsdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/signalsdk/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/signalsdk/local_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/signalsdk/signal_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/signalsdk/signal_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/signalsdk/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 19:50:57.458499 signal-application-python-sdk-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/tests/test_local_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-01-26 19:50:32.000000 signal-application-python-sdk-3.0.0/tests/test_signal_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:07:13.964935 signal-application-python-sdk-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-11 23:07:13.964935 signal-application-python-sdk-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:07:13.964935 signal-application-python-sdk-3.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1711 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:07:13.964935 signal-application-python-sdk-3.1.0/signal_application_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-11 23:07:13.000000 signal-application-python-sdk-3.1.0/signal_application_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-11 23:07:13.000000 signal-application-python-sdk-3.1.0/signal_application_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:07:13.000000 signal-application-python-sdk-3.1.0/signal_application_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 23:07:13.000000 signal-application-python-sdk-3.1.0/signal_application_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 23:07:13.000000 signal-application-python-sdk-3.1.0/signal_application_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:07:13.964935 signal-application-python-sdk-3.1.0/signalsdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/signalsdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/signalsdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/signalsdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/signalsdk/local_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/signalsdk/signal_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/signalsdk/signal_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/signalsdk/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:07:13.964935 signal-application-python-sdk-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/tests/test_local_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15243 2024-04-11 23:06:56.000000 signal-application-python-sdk-3.1.0/tests/test_signal_app.py
```

### Comparing `signal-application-python-sdk-3.0.0/PKG-INFO` & `signal-application-python-sdk-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-application-python-sdk
-Version: 3.0.0
+Version: 3.1.0
 Summary: signal application services
 Author: Wesley Clover
 Author-email: burak.cakmak@wesleyclover.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.26.0
 Requires-Dist: paho-mqtt==1.6.1
 Requires-Dist: urllib3==1.26.8
@@ -25,16 +25,17 @@
 ```
 
 Entry point for Signal Application SDK
 * Creates a bi-directional communication between device agent and application
 
 ### Initialize SDK
 ```
-self.app = SignalApp()
-self.app.initialize(self.onConfigUpdated, self.onEventReceived, self.onCommandReceived)
+from signalsdk.signal_app import SignalApp
+app = SignalApp()
+app.initialize(onConfigUpdated, onEventReceived, onCommandReceived)
 ```
 
 ### Provide a callback method to get notified when a configuration change is requested
 ```
 def onConfigUpdated(self, config):
 ```
 * Will be triggered when a new configuration change requested from the cloud
```

### Comparing `signal-application-python-sdk-3.0.0/README.md` & `signal-application-python-sdk-3.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 ```
 
 Entry point for Signal Application SDK
 * Creates a bi-directional communication between device agent and application
 
 ### Initialize SDK
 ```
-self.app = SignalApp()
-self.app.initialize(self.onConfigUpdated, self.onEventReceived, self.onCommandReceived)
+from signalsdk.signal_app import SignalApp
+app = SignalApp()
+app.initialize(onConfigUpdated, onEventReceived, onCommandReceived)
 ```
 
 ### Provide a callback method to get notified when a configuration change is requested
 ```
 def onConfigUpdated(self, config):
 ```
 * Will be triggered when a new configuration change requested from the cloud
```

### Comparing `signal-application-python-sdk-3.0.0/setup.py` & `signal-application-python-sdk-3.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,40 +15,37 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from os import path
 from setuptools import setup
 
-__version__ = '3.0.0'
+__version__ = "3.1.0"
 
 # Utility function to read the README file.
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as file:
+with open(path.join(this_directory, "README.md"), encoding="utf-8") as file:
     readme_file = file.read()
 
 DEPENDENCIES = [
     "requests>=2.26.0",
     "paho-mqtt==1.6.1",
     "urllib3==1.26.8",
-    "python-dateutil==2.8.2"
+    "python-dateutil==2.8.2",
 ]
 
-TEST_DEPENDENCIES = [
-    "pytest==7.1.2",
-    "pylint==2.13.9"
-]
+TEST_DEPENDENCIES = ["pytest==7.1.2", "pylint==2.13.9"]
 setup(
     name="signal-application-python-sdk",
     version=__version__,
-    packages=['signalsdk'],
+    packages=["signalsdk"],
     description="signal application services",
     long_description=readme_file,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     install_requires=DEPENDENCIES,
     test_require=TEST_DEPENDENCIES,
-    author='Wesley Clover',
-    author_email='burak.cakmak@wesleyclover.com'
+    author="Wesley Clover",
+    author_email="burak.cakmak@wesleyclover.com",
 )
```

### Comparing `signal-application-python-sdk-3.0.0/signal_application_python_sdk.egg-info/PKG-INFO` & `signal-application-python-sdk-3.1.0/signal_application_python_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-application-python-sdk
-Version: 3.0.0
+Version: 3.1.0
 Summary: signal application services
 Author: Wesley Clover
 Author-email: burak.cakmak@wesleyclover.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.26.0
 Requires-Dist: paho-mqtt==1.6.1
 Requires-Dist: urllib3==1.26.8
@@ -25,16 +25,17 @@
 ```
 
 Entry point for Signal Application SDK
 * Creates a bi-directional communication between device agent and application
 
 ### Initialize SDK
 ```
-self.app = SignalApp()
-self.app.initialize(self.onConfigUpdated, self.onEventReceived, self.onCommandReceived)
+from signalsdk.signal_app import SignalApp
+app = SignalApp()
+app.initialize(onConfigUpdated, onEventReceived, onCommandReceived)
 ```
 
 ### Provide a callback method to get notified when a configuration change is requested
 ```
 def onConfigUpdated(self, config):
 ```
 * Will be triggered when a new configuration change requested from the cloud
```

### Comparing `signal-application-python-sdk-3.0.0/signal_application_python_sdk.egg-info/SOURCES.txt` & `signal-application-python-sdk-3.1.0/signal_application_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signal-application-python-sdk-3.0.0/signalsdk/__init__.py` & `signal-application-python-sdk-3.1.0/signalsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-application-python-sdk-3.0.0/signalsdk/api.py` & `signal-application-python-sdk-3.1.0/signalsdk/api.py`

 * *Files identical despite different names*

### Comparing `signal-application-python-sdk-3.0.0/signalsdk/local_mqtt.py` & `signal-application-python-sdk-3.1.0/signalsdk/local_mqtt.py`

 * *Files identical despite different names*

### Comparing `signal-application-python-sdk-3.0.0/signalsdk/signal_app.py` & `signal-application-python-sdk-3.1.0/signalsdk/signal_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     LOCALMQTT_SDK_APPLICATION_COMMAND_NOTIFICATION_TOPIC,
     LOCALMQTT_SDK_TOPIC_PREFIX,
     LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC,
 )
 from signalsdk.signal_exception import (
     SignalAppLocalMqttEventCallBackError,
     SignalAppConfigEnvError,
-    SignalAppOnCommandCallBackError,
     SignalAppOnConfigChangedCallBackError,
 )
 
 from .validator import throw_if_parameter_not_found_in
 
 OnConfigUpdated = Callable[[dict], None]
 OnCommandReceived = Callable[[str], None]
@@ -92,26 +91,28 @@
                 )
                 self.on_command_received_callback(command)
             except Exception as err:
                 logging.info(
                     f"{__name__}: signalsdk:__on_command_received_handler "
                     f"function threw an error: {err}"
                 )
-                raise SignalAppOnCommandCallBackError from err
 
     def __on_event_received_handler(self, event):
         try:
             if self.on_event_received_callback:
                 logging.debug(
                     f"{__name__}: signalsdk:on_event_received_callback "
                     f"received event: {event}"
                 )
                 self.on_event_received_callback(event)
         except Exception as error:
-            logging.debug(f"{__name__}: App Event received: event: {event}")
+            logging.debug(
+                f"{__name__}: signalsdk: event:__on_event_received_handler"
+                f" function threw an error: {error}"
+            )
             raise SignalAppLocalMqttEventCallBackError from error
 
     def __on_config_updated_handler(self, event):
         try:
             logging.debug(
                 f"{__name__}: signalsdk:on_config_change_requested"
                 f" received event: {event}"
@@ -141,18 +142,23 @@
             )
         )
         self.local_mqtt.set_on_event_received(
             app_command_notification_topic, self.__on_command_received_handler
         )
         self.local_mqtt.subscribe(app_command_notification_topic, False)
         app_local_event_topic = LOCALMQTT_SDK_TOPIC_PREFIX + self.app_id
+        app_broadcast_event_topic = LOCALMQTT_SDK_TOPIC_PREFIX + "broadcast"
         self.local_mqtt.set_on_event_received(
             app_local_event_topic, self.__on_event_received_handler
         )
+        self.local_mqtt.set_on_event_received(
+            app_broadcast_event_topic, self.__on_event_received_handler
+        )
         self.local_mqtt.subscribe(app_local_event_topic, False)
+        self.local_mqtt.subscribe(app_broadcast_event_topic, False)
 
     def __renew_topic_subscription(self, current_topic, desired_topic):
         logging.debug(
             f"{__name__}: signalsdk:__renew_topic_subscription "
             f"current_topic: {current_topic} "
             f"desired_topic: {desired_topic}"
         )
@@ -219,20 +225,26 @@
             if self.local_pub_topic:
                 logging.debug(
                     f"{__name__}: signalsdk next() publishing to sdk topic: "
                     f"{self.local_pub_topic}"
                 )
                 self.local_mqtt.publish(self.local_pub_topic, event)
             else:
-                topic = LOCALMQTT_SDK_TOPIC_PREFIX + "broadcast"
-                logging.debug(
-                    f"{__name__}: signalsdk next() publishing to "
-                    f"broadcast topic: {topic}"
+                logging.warning(
+                    f"{__name__}: signalsdk next() no topic to publish event: "
+                    f"{event}"
                 )
-                self.local_mqtt.publish(topic, event)
+
+    def broadcast(self, event):
+        broadcast_topic = LOCALMQTT_SDK_TOPIC_PREFIX + "broadcast"
+        logging.debug(
+            f"{__name__}: signalsdk next() publishing to "
+            f"broadcast topic: {broadcast_topic}"
+        )
+        self.local_mqtt.publish(broadcast_topic, event)
 
     def nextNode(self, event):
         """Publish the event to next Node
         Note: nodered edgesignal-connector will subscribe to target topic
         :param event: event received on local event bus
         :return:
         """
```

### Comparing `signal-application-python-sdk-3.0.0/signalsdk/signal_exception.py` & `signal-application-python-sdk-3.1.0/signalsdk/signal_exception.py`

 * *Files identical despite different names*

### Comparing `signal-application-python-sdk-3.0.0/tests/test_api_client.py` & `signal-application-python-sdk-3.1.0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `signal-application-python-sdk-3.0.0/tests/test_signal_app.py` & `signal-application-python-sdk-3.1.0/tests/test_signal_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,27 +122,27 @@
             "settingsForApp": [{"key": "key1", "value": "value1"}]
         }
         sig_app.initialize(self.mock_config_change_cb, self.mock_event_cb)
         mock_localMqtt.assert_called()
         sig_app._SignalApp__start_listening_app_config_updates()
         mock_get_app.assert_called()
         # check set_on_event_receive called twice for app config and sdk config
-        self.assertEqual(mock_set_on_event_received.call_count, 3)
+        self.assertEqual(mock_set_on_event_received.call_count, 4)
         # check set_on_event_receive called with app config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             sig_app._SignalApp__on_config_updated_handler,
         )
         # check set_on_event_receive called with sdk config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_TOPIC_PREFIX + "12345",
             sig_app._SignalApp__on_event_received_handler,
         )
         # check subscribe called twice for app config and sdk config
-        self.assertEqual(mock_subscribe.call_count, 3)
+        self.assertEqual(mock_subscribe.call_count, 4)
         # check subscribe called with app config topic
         mock_subscribe.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             False,
         )
         # check subscribe called with sdk config topic
         mock_subscribe.assert_any_call(LOCALMQTT_SDK_TOPIC_PREFIX + "12345", False)
@@ -155,15 +155,29 @@
         mock_env.return_value = "12345"
         mock_get_app.return_value = {
             "settingsForApp": [{"key": "key1", "value": "value1"}]
         }
         sig_app.initialize(self.mock_config_change_cb, self.mock_event_cb)
         mock_event = MagicMock()
         sig_app.next(mock_event)
-        mock_localpub.assert_called()
+        mock_localpub.assert_not_called()
+
+    def test_app_broadcast(
+        self, mock_env, mock_localMqtt, mock_localpub, mock_get_app
+    ):
+        sig_app = SignalApp()
+        mock_env.return_value = "12345"
+        mock_get_app.return_value = {
+            "settingsForApp": [{"key": "key1", "value": "value1"}]
+        }
+        sig_app.initialize(self.mock_config_change_cb, self.mock_event_cb)
+        mock_event = MagicMock()
+        sig_app.broadcast(mock_event)
+        mock_localpub.assert_called_with(LOCALMQTT_SDK_TOPIC_PREFIX +
+                                         "broadcast", mock_event)
 
     @patch("signalsdk.signal_app.LocalMqtt.subscribe")
     @patch("signalsdk.signal_app.LocalMqtt.set_on_event_received")
     def test_app_next_no_pub_topic(
         self,
         mock_set_on_event_received,
         mock_subscribe,
@@ -179,39 +193,39 @@
             "settingsForSDK": {"sdkPubTopic": ""},
         }
         sig_app.initialize(self.mock_config_change_cb, self.mock_event_cb)
         mock_localMqtt.assert_called()
         sig_app._SignalApp__start_listening_app_config_updates()
         mock_get_app.assert_called()
         # check set_on_event_receive called twice for app config and sdk config
-        self.assertEqual(mock_set_on_event_received.call_count, 3)
+        self.assertEqual(mock_set_on_event_received.call_count, 4)
         # check set_on_event_receive called with app config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             sig_app._SignalApp__on_config_updated_handler,
         )
         # check set_on_event_receive called with sdk config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_TOPIC_PREFIX + "12345",
             sig_app._SignalApp__on_event_received_handler,
         )
         # check subscribe called twice for app config and sdk config
-        self.assertEqual(mock_subscribe.call_count, 3)
+        self.assertEqual(mock_subscribe.call_count, 4)
         # check subscribe called with app config topic
         mock_subscribe.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             False,
         )
         # check subscribe called with sdk config topic
         mock_subscribe.assert_any_call(LOCALMQTT_SDK_TOPIC_PREFIX + "12345", False)
 
         self.mock_config_change_cb.assert_called()
         mock_event = MagicMock()
         sig_app.next(mock_event)
-        mock_localpub.assert_called()
+        mock_localpub.assert_not_called()
 
     @patch("signalsdk.signal_app.LocalMqtt.subscribe")
     @patch("signalsdk.signal_app.LocalMqtt.set_on_event_received")
     def test_app_next_with_pub_topic(
         self,
         mock_set_on_event_received,
         mock_subscribe,
@@ -227,38 +241,40 @@
             "settingsForSDK": {"sdkPubTopic": "value2"},
         }
         sig_app.initialize(self.mock_config_change_cb, self.mock_event_cb)
         mock_localMqtt.assert_called()
         sig_app._SignalApp__start_listening_app_config_updates()
         mock_get_app.assert_called()
         # check set_on_event_receive called twice for app config and sdk config
-        self.assertEqual(mock_set_on_event_received.call_count, 3)
+        self.assertEqual(mock_set_on_event_received.call_count, 4)
         # check set_on_event_receive called with app config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             sig_app._SignalApp__on_config_updated_handler,
         )
         # check set_on_event_receive called with sdk config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_TOPIC_PREFIX + "12345",
             sig_app._SignalApp__on_event_received_handler,
         )
         # check subscribe called twice for app config and sdk config
-        self.assertEqual(mock_subscribe.call_count, 3)
+        self.assertEqual(mock_subscribe.call_count, 4)
         # check subscribe called with app config topic
         mock_subscribe.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             False,
         )
         # check subscribe called with sdk config topic
         mock_subscribe.assert_any_call(LOCALMQTT_SDK_TOPIC_PREFIX + "12345", False)
         self.mock_config_change_cb.assert_called()
         mock_event = MagicMock()
         sig_app.next(mock_event)
-        mock_localpub.assert_called()
+        mock_localpub.assert_called_with(
+            LOCALMQTT_SDK_TOPIC_PREFIX + "value2", mock_event
+        )
 
     @patch("signalsdk.signal_app.LocalMqtt.subscribe")
     @patch("signalsdk.signal_app.LocalMqtt.set_on_event_received")
     def test_app_nextNode_with_pub_topic(
         self,
         mock_set_on_event_received,
         mock_subscribe,
@@ -274,27 +290,27 @@
             "settingsForSDK": {"sdkPubTopic": "value2"},
         }
         sig_app.initialize(self.mock_config_change_cb, self.mock_event_cb)
         mock_localMqtt.assert_called()
         sig_app._SignalApp__start_listening_app_config_updates()
         mock_get_app.assert_called()
         # check set_on_event_receive called twice for app config and sdk config
-        self.assertEqual(mock_set_on_event_received.call_count, 3)
+        self.assertEqual(mock_set_on_event_received.call_count, 4)
         # check set_on_event_receive called with app config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             sig_app._SignalApp__on_config_updated_handler,
         )
         # check set_on_event_receive called with sdk config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_TOPIC_PREFIX + "12345",
             sig_app._SignalApp__on_event_received_handler,
         )
         # check subscribe called twice for app config and sdk config
-        self.assertEqual(mock_subscribe.call_count, 3)
+        self.assertEqual(mock_subscribe.call_count, 4)
         # check subscribe called with app config topic
         mock_subscribe.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             False,
         )
         # check subscribe called with sdk config topic
         mock_subscribe.assert_any_call(LOCALMQTT_SDK_TOPIC_PREFIX + "12345", False)
@@ -321,27 +337,27 @@
             "settingsForSDK": {"sdkPubTopic": "value2"},
         }
         sig_app.initialize(self.mock_config_change_cb, self.mock_event_cb)
         mock_localMqtt.assert_called()
         sig_app._SignalApp__start_listening_app_config_updates()
         mock_get_app.assert_called()
         # check set_on_event_receive called twice for app config and sdk config
-        self.assertEqual(mock_set_on_event_received.call_count, 3)
+        self.assertEqual(mock_set_on_event_received.call_count, 4)
         # check set_on_event_receive called with app config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             sig_app._SignalApp__on_config_updated_handler,
         )
         # check set_on_event_receive called with sdk config topic
         mock_set_on_event_received.assert_any_call(
             LOCALMQTT_SDK_TOPIC_PREFIX + "12345",
             sig_app._SignalApp__on_event_received_handler,
         )
         # check subscribe called twice for app config and sdk config
-        self.assertEqual(mock_subscribe.call_count, 3)
+        self.assertEqual(mock_subscribe.call_count, 4)
         # check subscribe called with app config topic
         mock_subscribe.assert_any_call(
             LOCALMQTT_SDK_APPLICATION_CONFIG_UPDATED_TOPIC.replace("${appId}", "12345"),
             False,
         )
         # check subscribe called with sdk config topic
         mock_subscribe.assert_any_call(LOCALMQTT_SDK_TOPIC_PREFIX + "12345", False)
```

