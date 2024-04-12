# Comparing `tmp/lytils-0.1.0.tar.gz` & `tmp/lytils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytils-0.1.0.tar", max compression
+gzip compressed data, was "lytils-0.1.1.tar", max compression
```

## Comparing `lytils-0.1.0.tar` & `lytils-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.0/LICENSE
--rw-r--r--   0        0        0      111 2024-02-21 21:27:17.496125 lytils-0.1.0/lytils/__init__.py
--rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.0/lytils/app.py
--rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.0/lytils/classes/__init__.py
--rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.0/lytils/classes/Regex.py
--rw-r--r--   0        0        0     1112 2023-10-18 01:09:58.336249 lytils-0.1.0/lytils/common.py
--rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.0/lytils/discord/__init__.py
--rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.0/lytils/discord/DiscordBot.py
--rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.0/lytils/email/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-10 19:21:06.149072 lytils-0.1.0/lytils/email/Email.py
--rw-r--r--   0        0        0     1577 2024-04-10 19:47:10.141707 lytils-0.1.0/lytils/file.py
--rw-r--r--   0        0        0      127 2024-04-10 19:52:11.636510 lytils-0.1.0/lytils/google_sheets/__init__.py
--rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.0/lytils/google_sheets/Column.py
--rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.0/lytils/google_sheets/format.py
--rw-r--r--   0        0        0      590 2024-01-29 19:06:31.147970 lytils-0.1.0/lytils/google_sheets/GoogleSheets.py
--rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.0/lytils/google_sheets/helpers.py
--rw-r--r--   0        0        0      263 2024-01-27 02:33:06.209559 lytils-0.1.0/lytils/google_sheets/Sheet.py
--rw-r--r--   0        0        0     7421 2024-04-10 19:21:06.136630 lytils-0.1.0/lytils/google_sheets/Tab.py
--rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.0/lytils/input.py
--rw-r--r--   0        0        0      616 2024-03-12 00:24:52.524374 lytils-0.1.0/lytils/logging.py
--rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.0/lytils/print.py
--rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.0/lytils/regex.py
--rw-r--r--   0        0        0     1212 2024-03-11 21:33:05.723960 lytils-0.1.0/lytils/surfshark.py
--rw-r--r--   0        0        0      316 2024-04-10 19:23:22.162623 lytils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.0/README.md
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.1/LICENSE
+-rw-r--r--   0        0        0      111 2024-02-21 21:27:17.496125 lytils-0.1.1/lytils/__init__.py
+-rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.1/lytils/app.py
+-rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.1/lytils/classes/__init__.py
+-rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.1/lytils/classes/Regex.py
+-rw-r--r--   0        0        0     1112 2023-10-18 01:09:58.336249 lytils-0.1.1/lytils/common.py
+-rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.1/lytils/discord/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.1/lytils/discord/DiscordBot.py
+-rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.1/lytils/email/__init__.py
+-rw-r--r--   0        0        0     2384 2024-04-12 07:06:16.170788 lytils-0.1.1/lytils/email/Email.py
+-rw-r--r--   0        0        0     1577 2024-04-10 19:47:10.141707 lytils-0.1.1/lytils/file.py
+-rw-r--r--   0        0        0      127 2024-04-10 19:52:11.636510 lytils-0.1.1/lytils/google_sheets/__init__.py
+-rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.1/lytils/google_sheets/Column.py
+-rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.1/lytils/google_sheets/format.py
+-rw-r--r--   0        0        0      590 2024-01-29 19:06:31.147970 lytils-0.1.1/lytils/google_sheets/GoogleSheets.py
+-rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.1/lytils/google_sheets/helpers.py
+-rw-r--r--   0        0        0      263 2024-01-27 02:33:06.209559 lytils-0.1.1/lytils/google_sheets/Sheet.py
+-rw-r--r--   0        0        0     7421 2024-04-10 19:21:06.136630 lytils-0.1.1/lytils/google_sheets/Tab.py
+-rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.1/lytils/input.py
+-rw-r--r--   0        0        0      616 2024-03-12 00:24:52.524374 lytils-0.1.1/lytils/logging.py
+-rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.1/lytils/print.py
+-rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.1/lytils/regex.py
+-rw-r--r--   0        0        0     1253 2024-04-12 07:03:04.806336 lytils-0.1.1/lytils/surfshark.py
+-rw-r--r--   0        0        0      318 2024-04-12 07:11:04.872541 lytils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.1/README.md
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.1/PKG-INFO
```

### Comparing `lytils-0.1.0/LICENSE` & `lytils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/app.py` & `lytils-0.1.1/lytils/app.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/classes/Regex.py` & `lytils-0.1.1/lytils/classes/Regex.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/common.py` & `lytils-0.1.1/lytils/common.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/discord/DiscordBot.py` & `lytils-0.1.1/lytils/discord/DiscordBot.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/email/Email.py` & `lytils-0.1.1/lytils/email/Email.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,53 +14,55 @@
             Expects 'email' key; email used to send the email
             Expects 'password' key; password for sender's email
         :param notify string:
             Instead of having to pass a recipient email to
             send_email every time, you can declare a default
             email, and use notify() to send email to that recipient
         """
-        self.__smtp = smtp
+        self._smtp = smtp
 
         # Set port by default if not specified
         if "port" not in smtp:
-            self.__smtp["port"] = 587
+            self._smtp["port"] = 587
 
-        self.__surfshark = None
+        self._surfshark = None
         if surfshark_path:
-            self.__surfshark = Surfshark(surfshark_path)
+            self._surfshark = Surfshark(surfshark_path)
 
-        self.__creds = credentials
-        self.__notify = notify
-        self.__server = None
+        self._creds = credentials
+        self._notify = notify
+        self._server = None
 
     def start_server(self):
-        # Kill surfshark as it blocks email SMTP and Selenium connections
-        self.__surfshark.kill()
+        # Kill surfshark if it is running as it blocks SMTP connections.
+        if self._surfshark and self._surfshark.running():
+            self._surfshark.kill()
+
         # Connect to the SMTP server
-        self.__server = smtplib.SMTP("smtp.gmail.com", 587)
-        # self.__server = smtplib.SMTP(smtp['server'], smtp['port'])
-        # self.__server.ehlo()
-        self.__server.starttls()
-        self.__server.login(self.__creds["email"], self.__creds["password"])
+        self._server = smtplib.SMTP("smtp.gmail.com", 587)
+        # self._server = smtplib.SMTP(smtp['server'], smtp['port'])
+        # self._server.ehlo()
+        self._server.starttls()
+        self._server.login(self._creds["email"], self._creds["password"])
 
     def send_email(self, recipient, subject, message):
         # Create the email
         msg = EmailMessage()
         msg.set_content(message)
         msg["subject"] = subject
         msg["to"] = recipient
-        msg["from"] = self.__creds["email"]
+        msg["from"] = self._creds["email"]
 
         # Send the email
-        self.__server.sendmail(self.__creds["email"], recipient, msg.as_string())
+        self._server.sendmail(self._creds["email"], recipient, msg.as_string())
 
     def notify(self, subject, message):
-        if self.__notify:
-            self.send_email(self.__notify, subject, message)
+        if self._notify:
+            self.send_email(self._notify, subject, message)
 
     def quit(self):
-        if self.__server:
-            self.__server.quit()
+        if self._server:
+            self._server.quit()
 
-            # Restart surfshark to stay safe
-            if self.__surfshark:
-                self.__surfshark.start()
+        # Restart surfshark if it is not currently running.
+        if self._surfshark and not self._surfshark.running():
+            self._surfshark.start()
```

### Comparing `lytils-0.1.0/lytils/file.py` & `lytils-0.1.1/lytils/file.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/google_sheets/Column.py` & `lytils-0.1.1/lytils/google_sheets/Column.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/google_sheets/format.py` & `lytils-0.1.1/lytils/google_sheets/format.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/google_sheets/GoogleSheets.py` & `lytils-0.1.1/lytils/google_sheets/GoogleSheets.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/google_sheets/Tab.py` & `lytils-0.1.1/lytils/google_sheets/Tab.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/input.py` & `lytils-0.1.1/lytils/input.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/logging.py` & `lytils-0.1.1/lytils/logging.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/print.py` & `lytils-0.1.1/lytils/print.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.0/lytils/surfshark.py` & `lytils-0.1.1/lytils/surfshark.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,30 @@
 from .print import cprint
 
 
 class Surfshark:
     def __init__(self, path: str):
         self.__path = path
 
+    def running(self):
+        return is_process_running("Surfshark.exe")
+
     def ensure(self):
-        # Pause if Surfshark is not running to allow user to connect to Surfshark
-        is_running = is_process_running("Surfshark.exe")
-        if not is_running:
+        """
+        Ensures Surfshark is running and pauses execution if not.
+        """
+        if not self.running():
             cprint("<y>Surfshark is not running. Starting Surfshark now...")
             self.start()  # Ensure
         else:
             print("Surfshark is running. Proceeding...")
-        while not is_running:
+
+        # Surfshark may take a while to start up and connect.
+        while not self.running():
             cinput("Press <y><ENTER><w> once Surfshark has connected to continue...")
-            is_running = is_process_running("Surfshark.exe")
 
     def kill(self):
         kill_process("Surfshark.exe")
         kill_service("Surfshark Service")
         kill_service("Surfshark WireGuard Service")
 
     def start(self):
```

