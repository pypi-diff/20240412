# Comparing `tmp/barbara_updater-3.3.0.tar.gz` & `tmp/barbara_updater-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barbara_updater-3.3.0.tar", last modified: Fri Apr 12 00:23:41 2024, max compression
+gzip compressed data, was "barbara_updater-3.3.1.tar", last modified: Fri Apr 12 00:40:06 2024, max compression
```

## Comparing `barbara_updater-3.3.0.tar` & `barbara_updater-3.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-12 00:23:41.092323 barbara_updater-3.3.0/
--rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-12 00:23:41.092323 barbara_updater-3.3.0/PKG-INFO
--rw-r--r--   0 santod    (1000) santod    (1000)   235141 2024-04-12 00:09:26.000000 barbara_updater-3.3.0/barbara3.py
-drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-12 00:23:41.092323 barbara_updater-3.3.0/barbara_updater.egg-info/
--rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-12 00:23:41.000000 barbara_updater-3.3.0/barbara_updater.egg-info/PKG-INFO
--rw-r--r--   0 santod    (1000) santod    (1000)      176 2024-04-12 00:23:41.000000 barbara_updater-3.3.0/barbara_updater.egg-info/SOURCES.txt
--rw-r--r--   0 santod    (1000) santod    (1000)        1 2024-04-12 00:23:41.000000 barbara_updater-3.3.0/barbara_updater.egg-info/dependency_links.txt
--rw-r--r--   0 santod    (1000) santod    (1000)        9 2024-04-12 00:23:41.000000 barbara_updater-3.3.0/barbara_updater.egg-info/top_level.txt
--rw-r--r--   0 santod    (1000) santod    (1000)       38 2024-04-12 00:23:41.092323 barbara_updater-3.3.0/setup.cfg
--rw-r--r--   0 santod    (1000) santod    (1000)      327 2024-02-23 03:13:41.000000 barbara_updater-3.3.0/setup.py
+drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-12 00:40:06.045894 barbara_updater-3.3.1/
+-rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-12 00:40:06.045894 barbara_updater-3.3.1/PKG-INFO
+-rw-r--r--   0 santod    (1000) santod    (1000)   235191 2024-04-12 00:33:01.000000 barbara_updater-3.3.1/barbara3.py
+drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-12 00:40:06.045894 barbara_updater-3.3.1/barbara_updater.egg-info/
+-rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-12 00:40:05.000000 barbara_updater-3.3.1/barbara_updater.egg-info/PKG-INFO
+-rw-r--r--   0 santod    (1000) santod    (1000)      176 2024-04-12 00:40:06.000000 barbara_updater-3.3.1/barbara_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 santod    (1000) santod    (1000)        1 2024-04-12 00:40:05.000000 barbara_updater-3.3.1/barbara_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 santod    (1000) santod    (1000)        9 2024-04-12 00:40:05.000000 barbara_updater-3.3.1/barbara_updater.egg-info/top_level.txt
+-rw-r--r--   0 santod    (1000) santod    (1000)       38 2024-04-12 00:40:06.045894 barbara_updater-3.3.1/setup.cfg
+-rw-r--r--   0 santod    (1000) santod    (1000)      327 2024-02-23 03:13:41.000000 barbara_updater-3.3.1/setup.py
```

### Comparing `barbara_updater-3.3.0/barbara3.py` & `barbara_updater-3.3.1/barbara3.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,16 +521,18 @@
         img = MIMEImage(attachment.read(), name=screenshot_filename)
         msg.attach(img)
 
     # For example:
     try:
         # Connect to Gmail's SMTP server and send the email
         server = smtplib.SMTP_SSL('smtp.gmail.com', 465)
-        server.login(from_email, 'apedhdhxnyhkfepv')  # Use your app password
-        #server.login(from_email, os.getenv('EMAIL_APP_PASSWORD'))  # Use the environment variable 
+        
+        # enter app password back here for development machine
+        
+        server.login(from_email, os.getenv('EMAIL_APP_PASSWORD'))  # Use the environment variable 
         server.send_message(msg)
         server.quit()
         # Clear the current display
         for widget in frame1.winfo_children():
             if isinstance(widget, (tk.Checkbutton, tk.Label, tk.Button, tk.Entry)):
                 widget.destroy()
                 
@@ -591,14 +593,15 @@
         maps_button = tk.Button(frame1, text="Maps", command=email_to_maps, font=("Helvetica", 16, "bold"))
         maps_button.grid(row=3, column=1, columnspan=20, padx=50, pady=(15,0), sticky='nw')
 
 def pic_email():
     global email_entry, refresh_flag  # Use the global variable
     refresh_flag = True
     
+    # use this code for rp5 development machine
 #    subprocess.run(['grim', screenshot_filename])
 
     # use the following codes for rp4s in place of subprocess line above
     # Specify the filename for the screenshot
     screenshot_filename = 'screenshot.png'
     
     # Take the screenshot and overwrite the existing file
@@ -2918,15 +2921,15 @@
  
     # Continue with other actions or functions as needed
     land_or_buoy()
 
 frame1.grid(row=0, column=0, sticky="nsew")
 
 # First line (bold)
-label1 = tk.Label(frame1, text="Welcome to The Weather Observer v3.3.0", font=("Arial", 18, "bold"), bg=tk_background_color, justify="left")
+label1 = tk.Label(frame1, text="Welcome to The Weather Observer v3.3.1", font=("Arial", 18, "bold"), bg=tk_background_color, justify="left")
 label1.grid(row=0, column=0, padx=50, pady=(50, 10), sticky="w")
 
 # Main block of text including the question
 info_text = f'''
 In order to begin, your new instrument needs to be calibrated,
 and you need to make choices about which weather to observe.
```

