# Comparing `tmp/barbara_updater-3.2.0.tar.gz` & `tmp/barbara_updater-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barbara_updater-3.2.0.tar", last modified: Thu Mar 28 23:30:23 2024, max compression
+gzip compressed data, was "barbara_updater-3.3.0.tar", last modified: Fri Apr 12 00:23:41 2024, max compression
```

## Comparing `barbara_updater-3.2.0.tar` & `barbara_updater-3.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-03-28 23:30:23.491475 barbara_updater-3.2.0/
--rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-03-28 23:30:23.491475 barbara_updater-3.2.0/PKG-INFO
--rw-r--r--   0 santod    (1000) santod    (1000)   228768 2024-03-28 23:23:00.000000 barbara_updater-3.2.0/barbara3.py
-drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-03-28 23:30:23.491475 barbara_updater-3.2.0/barbara_updater.egg-info/
--rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-03-28 23:30:23.000000 barbara_updater-3.2.0/barbara_updater.egg-info/PKG-INFO
--rw-r--r--   0 santod    (1000) santod    (1000)      176 2024-03-28 23:30:23.000000 barbara_updater-3.2.0/barbara_updater.egg-info/SOURCES.txt
--rw-r--r--   0 santod    (1000) santod    (1000)        1 2024-03-28 23:30:23.000000 barbara_updater-3.2.0/barbara_updater.egg-info/dependency_links.txt
--rw-r--r--   0 santod    (1000) santod    (1000)        9 2024-03-28 23:30:23.000000 barbara_updater-3.2.0/barbara_updater.egg-info/top_level.txt
--rw-r--r--   0 santod    (1000) santod    (1000)       38 2024-03-28 23:30:23.491475 barbara_updater-3.2.0/setup.cfg
--rw-r--r--   0 santod    (1000) santod    (1000)      327 2024-02-23 03:13:41.000000 barbara_updater-3.2.0/setup.py
+drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-12 00:23:41.092323 barbara_updater-3.3.0/
+-rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-12 00:23:41.092323 barbara_updater-3.3.0/PKG-INFO
+-rw-r--r--   0 santod    (1000) santod    (1000)   235141 2024-04-12 00:09:26.000000 barbara_updater-3.3.0/barbara3.py
+drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-12 00:23:41.092323 barbara_updater-3.3.0/barbara_updater.egg-info/
+-rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-12 00:23:41.000000 barbara_updater-3.3.0/barbara_updater.egg-info/PKG-INFO
+-rw-r--r--   0 santod    (1000) santod    (1000)      176 2024-04-12 00:23:41.000000 barbara_updater-3.3.0/barbara_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 santod    (1000) santod    (1000)        1 2024-04-12 00:23:41.000000 barbara_updater-3.3.0/barbara_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 santod    (1000) santod    (1000)        9 2024-04-12 00:23:41.000000 barbara_updater-3.3.0/barbara_updater.egg-info/top_level.txt
+-rw-r--r--   0 santod    (1000) santod    (1000)       38 2024-04-12 00:23:41.092323 barbara_updater-3.3.0/setup.cfg
+-rw-r--r--   0 santod    (1000) santod    (1000)      327 2024-02-23 03:13:41.000000 barbara_updater-3.3.0/setup.py
```

### Comparing `barbara_updater-3.2.0/barbara3.py` & `barbara_updater-3.3.0/barbara3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# 3/28/24 maps for radar and radiosonde appear fine
+# 4/11/24 done - password protect escape key
+# increase security. password protect escape key, store email, terminal password
+# fixed 4-10E-24.py rewritten reg sat code to accommodate dark borders all views
+# accidentally may have fixed problem with reg sat and two streams while
+# working on resizing the two smaller reg sat views
+# adjust code at end of try/except in reg sat functions to prevent two streams
+# applied threading to lighting and station plot
+# versions after this mostly a waste of time until 4/10/24 
+# threading working for lcl radar and reg sat, but still no display before reg sat
+# fixed with NWS API a problem with baro_input out of nowhere. Can't print line 2870
+# work to include more responsiveness and leave image up before reg sat loop
+# 4/3/24 threading added to scrape, assemble, but not display reg sat loops
+# working to forget ntl radar image just before lcl radar loop ready to display
+# try to extend display of previous image while lcl radar is rendering
+# threading for lcl radar loop is done. Try to thread other heavy tasks
 # 3/25/24 enable functional screenshot button, email is next
 # 3/26/24 email is working - join scraped frame gracefully
 # 3/25/24 Two display buttons set. all button code in show_national_radar
 # done 3/24/24 keyborad to right, focus in tkinter box, larger buttons, remove escape key
 # timeout errors for lightning geopy nominatim may cause hang ups or double
 # scraped frame cycles - consider adding clearing frames function, currently code at
 # start of national radar
@@ -60,35 +74,36 @@
 from tkinter import IntVar, Checkbutton
 import tkinter.font as tkFont
 from tkinter import ttk, IntVar
 from tkinter import ttk, IntVar, messagebox
 from tkinter import PhotoImage
 from tkinter import font  # Import the font module
 from tkinter import Tk, Label
-from PIL import Image, ImageDraw, ImageFont, ImageTk
+from PIL import Image, ImageDraw, ImageFont, ImageTk, ImageChops
 import urllib.parse
 from collections import deque
 from matplotlib.widgets import Button
 import matplotlib.ticker as ticker
 import warnings
 #from memory_profiler import profile
 import itertools
 from itertools import cycle, islice
 import psutil
 import gc
 import threading
+from threading import Thread
+from functools import partial
 import logging
 import traceback
 import smtplib
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.mime.image import MIMEImage
 from tkinter import Tk, Button, simpledialog
 
-
 #logging.basicConfig(level=logging.DEBUG,
 #                    format='%(asctime)s - %(levelname)s - %(message)s')
 
 # Test logging
 #logging.debug('This is a debug message.')
 
 global inHg_correction_factor
@@ -110,14 +125,17 @@
 
 iterate_flag = False
 
 refresh_flag = False
 # to determine if user has chosen reg sat view
 has_submitted_choice = False
 
+# flag established to track whether img_label_national_radar is forgotten to smooth displays
+national_radar_hidden = False
+
 # Global variables for images
 img_tk_national_radar = None
 img_label_national_radar = None
 img_label_national_satellite = None
 img_label_satellite = None
 
 last_national_radar_scrape_time = None
@@ -140,29 +158,50 @@
 alternative_town_3 = ""
 alternative_state_3 = ""
 
 def reboot_system():
     root.quit()
     os.system('sudo reboot')
     
+def check_password(event):
+    global key_sequence
+    key_sequence += event.char  # Append pressed key to the sequence
+
+    # Define your password (key sequence)
+    password = '2barbaraterminal'  # You can choose a more complex password
+
+    # Check if the correct sequence was entered
+    if key_sequence.endswith(password):
+        exit_full_screen(event)
+        key_sequence = ''  # Reset sequence after successful password entry
+    elif len(key_sequence) > len(password):  # Reset if sequence gets too long without a match
+        key_sequence = key_sequence[-len(password):]  # Keep only the last few presses
+
 def exit_full_screen(event):
     root.attributes("-fullscreen", False)  # This exits full screen mode
+    root.bind('<Escape>', lambda e: None)  # Disable further Escape actions or rebind as needed
 
 def start_fullscreen():
     root.geometry("1024x600")
     root.attributes('-zoomed', True)
     root.title("The Weather Observer")
-    root.attributes('-fullscreen', True) #no decoration
-    
+    root.attributes('-fullscreen', True)  # no decoration
+
 # Create a tkinter window
 root = tk.Tk()
 root.title("The Weather Observer")
 root.geometry("1024x576+0+-1")
-# Bind the 'Escape' key to the exit_full_screen function
-root.bind('<Escape>', exit_full_screen)
+
+# Initialize key sequence storage
+key_sequence = ''
+
+# Bind all keypresses to the check_password function
+root.bind('<Key>', check_password)
+
+# Set up fullscreen and other startup configurations
 root.after(4000, start_fullscreen)
 
 # Define StringVar for labels
 left_site_text = tk.StringVar()
 left_temp_text = tk.StringVar()
 left_water_temp_text = tk.StringVar()
 left_wind_text = tk.StringVar()
@@ -194,43 +233,65 @@
             lon = data['lon']
             return lat, lon
     except requests.exceptions.RequestException:
         pass
     return None, None
 
 
-def get_aobs_site(latitude, longitude):
-    global baro_input
-    aobs_url = generate_aobs_url(latitude, longitude)
-    nearest_html = requests.get(aobs_url)
-    nearest_soup = BeautifulSoup(nearest_html.content, 'html.parser')
-    panel_title = nearest_soup.find('h2', class_='panel-title')
-    
-    if panel_title:
-        aobs_site = panel_title.text.strip()
-        current_conditions = nearest_soup.find(id='current_conditions_detail')
-        
-        if current_conditions and isinstance(current_conditions, Tag):
-            tds = current_conditions.find_all('td')
-            
-            if len(tds) > 5 and tds[5].string is not None:
-                baro_input = tds[5].string.strip()
+import requests
 
-                try:
-                    baro_input = float(baro_input[:5])
-                    return aobs_site
-                except ValueError:
-                    print("This site doesn't have a barometric pressure reading we can use.")
-                    print("Please choose an alternate site when given the chance.")
-        else:
-            print("The barometric reading at this site is not available for use.")
-    else:
-        print("Observation site not found.")
+# Function to convert pressure from Pascals to inches of mercury
+def pascals_to_inches_hg(pascals):
+    """Converts pressure in Pascals to inches of mercury."""
+    return pascals / 3386.389
+
+def get_aobs_site(latitude, longitude):
+    global baro_input  # Global variable for barometric pressure
+    global aobs_site   # Global variable for the name of the town and state
     
-    return None
+    # Make the initial API request to get location and station information
+    response = requests.get(f'https://api.weather.gov/points/{latitude},{longitude}')
+    data = response.json()
+
+    # Extract location information
+    location = data['properties']['relativeLocation']['properties']
+    town = location['city']
+    state = location['state']
+    aobs_site = f"{town}, {state}"  # Update global variable with location name
+
+    # Extract the URL to the nearest observation stations
+    stations_url = data['properties']['observationStations']
+
+    # Get the list of nearby weather stations
+    response = requests.get(stations_url)
+    stations_data = response.json()
+
+    # Loop through the stations to find one with a barometric pressure reading
+    for station_url in stations_data['observationStations']:
+        station_observation_response = requests.get(f"{station_url}/observations/latest")
+        if station_observation_response.status_code != 200:
+            continue  # Skip if the station's observation data can't be accessed
+        observation_data = station_observation_response.json()
+
+        # Attempt to get the barometric pressure
+        barometric_pressure_pascals = observation_data['properties']['barometricPressure']['value']
+        
+        if barometric_pressure_pascals is not None:
+            # Convert to inches of mercury
+            baro_input = pascals_to_inches_hg(barometric_pressure_pascals)  # Update global variable
+            #print(f"Location: {aobs_site}")
+            #print(f"Barometric Pressure: {baro_input:.2f} inches of mercury")
+            return aobs_site
+
+    # If the loop completes without finding a valid pressure reading
+    print(f"Location: {aobs_site}")
+    print("No stations with a current barometric pressure reading were found.")
+    return False
+
+
 #@profile
 def get_standard_radar_site_url(latitude, longitude):
     
     global radar_site, radar_site_url
     
     aobs_url = generate_aobs_url(latitude, longitude)
     nws_html = requests.get(aobs_url)
@@ -441,15 +502,15 @@
     to_email = email_entry.get()  # Get the email address from the entry widget
     if not to_email:
         print("No email address provided.")
         return
 
     # Email details
     from_email = 'picturesfromtheweatherobserver@gmail.com'
-    subject = 'Your Weather Observer Screenshot'
+    subject = 'Weather Observer Screenshot - Do Not Reply'
     body = 'Attached is the screenshot from the Weather Observer.'
 
     # Set up the email message
     msg = MIMEMultipart()
     msg['From'] = from_email
     msg['To'] = to_email
     msg['Subject'] = subject
@@ -461,14 +522,15 @@
         msg.attach(img)
 
     # For example:
     try:
         # Connect to Gmail's SMTP server and send the email
         server = smtplib.SMTP_SSL('smtp.gmail.com', 465)
         server.login(from_email, 'apedhdhxnyhkfepv')  # Use your app password
+        #server.login(from_email, os.getenv('EMAIL_APP_PASSWORD'))  # Use the environment variable 
         server.send_message(msg)
         server.quit()
         # Clear the current display
         for widget in frame1.winfo_children():
             if isinstance(widget, (tk.Checkbutton, tk.Label, tk.Button, tk.Entry)):
                 widget.destroy()
                 
@@ -493,14 +555,15 @@
         return_label = tk.Label(frame1, text=return_text, font=("Helvetica", 16), bg=tk_background_color, justify="left")
         return_label.grid(row=2, column=0, columnspan=20, padx=50, pady=25, sticky='nw') 
 
         return_button = tk.Button(frame1, text="Return", command=email_to_maps, font=("Helvetica", 16, "bold"))
         return_button.grid(row=3, column=0, columnspan=20, padx=50, pady=(15,0), sticky='nw')
         
     except Exception as e:
+        print("line 538. failed to send email: ", e)
         # Clear the current display
         for widget in frame1.winfo_children():
             if isinstance(widget, (tk.Checkbutton, tk.Label, tk.Button, tk.Entry)):
                 widget.destroy()
         
         transparent_frame.grid_forget()
         scraped_frame.grid_forget()
@@ -527,15 +590,23 @@
         
         maps_button = tk.Button(frame1, text="Maps", command=email_to_maps, font=("Helvetica", 16, "bold"))
         maps_button.grid(row=3, column=1, columnspan=20, padx=50, pady=(15,0), sticky='nw')
 
 def pic_email():
     global email_entry, refresh_flag  # Use the global variable
     refresh_flag = True
-    subprocess.run(['grim', screenshot_filename])
+    
+#    subprocess.run(['grim', screenshot_filename])
+
+    # use the following codes for rp4s in place of subprocess line above
+    # Specify the filename for the screenshot
+    screenshot_filename = 'screenshot.png'
+    
+    # Take the screenshot and overwrite the existing file
+    subprocess.run(['scrot', screenshot_filename, '--overwrite']) 
 
     # Clear the current display
     for widget in frame1.winfo_children():
         if isinstance(widget, (tk.Checkbutton, tk.Label, tk.Button, tk.Entry, tk.Radiobutton)):
             widget.destroy()
             
     # I think I need these. Maybe not if I do frame1.left()
@@ -1818,15 +1889,15 @@
         lightning_center_input()
     
     # Clear the current display
     for widget in frame1.winfo_children():
         widget.destroy()
 
     # Reset clean position for frame1
-    frame1.grid(row=0, column=0, sticky="nw") 
+    frame1.grid(row=0, column=0, sticky="nsew") 
 
     #Configure Chrome options for headless mode
     chrome_options = Options()
     chrome_options.add_argument("--headless")
     chrome_options.add_argument("--disable-gpu")
 
     # Use the system-installed ChromeDriver executable
@@ -1912,28 +1983,28 @@
                 min_distance = distance
                 closest_site = site
 
         return closest_site
 
     # Reset clean position for frame1
     # Before displaying the map, temporarily adjust the configuration
-    frame1.grid(row=0, column=0)
+    frame1.grid(row=0, column=0, sticky="nsew")
     root.grid_rowconfigure(0, weight=0)  # Reset to default which doesn't expand the row
     root.grid_columnconfigure(0, weight=0)  # Reset to default which doesn't expand the column
 
     # Create a label to display the map with radar sites
     label = tk.Label(frame1, width=target_width, height=target_height)
 
     # Display the resized radar sites map on the label
     photo = ImageTk.PhotoImage(map_screenshot_image)
     label.configure(image=photo)
     label.image = photo  # Keep a reference to the image to prevent it from being garbage-collected
 
     # Now, set the grid placement for the label
-    label.grid(row=0, column=0, sticky="nsew", padx=200, pady=70, columnspan=20)
+    label.grid(row=0, column=0, sticky="nsew", padx=100, pady=70)
 
     # Draw radar site links on the label
     lcl_radar_draw_links()
 
     # Bind the click function to the label click event
     label.bind("<Button-1>", lcl_radar_on_click)
 
@@ -2004,29 +2075,37 @@
     sonde_letter_identifier = ""
     
     if box_variables[8] ==1:        
         
         for widget in frame1.winfo_children():
             widget.destroy()
         
+#         # Clear the current display
+#         for widget in frame1.winfo_children():
+#             if isinstance(widget, (tk.Checkbutton, tk.Label, tk.Button, tk.Entry, tk.Radiobutton)):
+#                 widget.destroy()
+        
         # Reset clean position for frame1
-        frame1.grid(row=0, column=0, sticky="nw")
+        frame1.grid(row=0, column=0, sticky="nsew")
         #inserted 3/28/24
         # Before displaying the map, temporarily adjust the configuration
-        root.grid_rowconfigure(0, weight=0)  # Reset to default which doesn't expand the row
-        root.grid_columnconfigure(0, weight=0)  # Reset to default which doesn't expand the column 
-        
+        frame1.master.grid_rowconfigure(0, weight=0)  # Reset to default which doesn't expand the row
+        frame1.master.grid_columnconfigure(0, weight=0)  # Reset to default which doesn't expand the column 
+        frame1.grid_propagate(False)
+                
         chrome_options = Options()
         chrome_options.add_argument("--headless")
         chrome_options.add_argument("--disable-gpu")
         
         driver = webdriver.Chrome(service=Service("chromedriver"), options=chrome_options)
         
-        url = "https://www.spc.noaa.gov/exper/soundings/{}/".format(get_most_recent_gmt())
-
+        # trying to change this line as an experiment 4/3/24 - problem 00z-1z
+        url = "https://www.spc.noaa.gov/exper/soundings/{}/".format(get_most_recent_gmt())        
+        #url = "https://www.spc.noaa.gov/exper/soundings/{}/".format(most_recent_sonde_time()) 
+        
         driver.get(url)
 
         try:
             map_element = driver.find_element("xpath", "/html/body/table/tbody/tr/td[1]/center/img")
             valid_page_found = True
         except Exception as e:
             print(f"Error: {e}")
@@ -2043,24 +2122,24 @@
         active_links = soup.find('map', {'name': 'stations'}).find_all('area')
 
         target_width, target_height = 600, 450
         scale_factor = target_width / original_map_image.width
         enlarged_map_image = original_map_image.resize((target_width, target_height), Image.LANCZOS)
 
         label = tk.Label(frame1)
-        label.grid(row=0, column=0, padx=390, pady=85)
+        label.grid(row=0, column=1, padx=0, pady=85)
 
         enlarged_map_photo = ImageTk.PhotoImage(enlarged_map_image)
         label.configure(image=enlarged_map_photo)
         label.image = enlarged_map_photo
 
         draw_radiosonde_links(active_links, scale_factor)
 
         overlay_label = tk.Label(frame1, text="Sounding Stations", font=("Arial", 18, "bold"), bg="white", fg="black")
-        overlay_label.grid(row=0, column=0, pady=(400,0))
+        overlay_label.grid(row=0, column=1, pady=(400,0))
 
         match = re.search(r'<span class="style5">Observed Radiosonde Data<br>\s*([^<]+)\s*</span>', driver.page_source)
         if match:
             date_str = match.group(1)
             overlay_label["text"] += f" {date_str}"
         
         #frame1.grid(row=0, column=0, sticky="nw") 
@@ -2114,16 +2193,22 @@
             def inner():
                 if not has_submitted_choice:  # Check the flag
                     update_sat_checkboxes(index)
             return inner
 
         # Create and display the updated labels        
         # Reset clean position for frame1
+        #frame1.grid(row=0, column=0, sticky="nsew")
+        
         frame1.grid(row=0, column=0, sticky="nsew")
-        frame1.config(width=1024, height=600)        
+        #frame1.master.grid_rowconfigure(0, weight=0)
+        #frame1.master.grid_columnconfigure(0, weight=0)
+        #frame1.config(width=1024, height=600)
+        
+        #frame1.config(width=1024, height=600)        
         
         reg_sat_label1 = tk.Label(frame1, text="The Weather Observer", font=("Arial", 18, "bold"), bg=tk_background_color, justify="left")
         reg_sat_label1.grid(row=0, column=0, padx=50, pady=(50,10), sticky="w")
 
         instruction_text = "Please select your regional satellite view:"
         instructions_label = tk.Label(frame1, text=instruction_text, font=("Helvetica", 14, "bold"), bg=tk_background_color)
         instructions_label.grid(row=1, column=0, padx=50, pady=(0, 25), sticky='w') 
@@ -2380,15 +2465,15 @@
     if box_variables[7] == 1:
     
         # Clear the current display
         for widget in frame1.winfo_children():
             widget.destroy()
 
         frame1.grid(row=0, column=0, sticky="nsew")
-        frame1.grid_propagate(False)
+        frame1.grid_propagate(False) # another line later in this function 2533
 
         zoom_plot = tk.StringVar(value="9") 
 
         def submit_station_plot_center():
         
             global submit_station_plot_town, submit_station_plot_state, station_plot_town, station_plot_state, station_plot_lat, station_plot_lon, zoom_plot 
             global refresh_flag
@@ -2519,14 +2604,16 @@
         submit_button = tk.Button(frame1, text="Submit", command=submit_station_plot_center, font=("Helvetica", 16, "bold"))
         submit_button.grid(row=7, column=0, columnspan=20, padx=50, pady=15, sticky='nw')
 
         # Spacer to push the keyboard to the bottom
         #vertical_spacer = tk.Label(frame1, text="", bg=tk_background_color)
         #vertical_spacer.grid(row=8, column=0, sticky="nsew", pady=(0, 0))  # Adjust row and pady as necessary
 
+        frame1.grid_propagate(False) #prevent keyboard from skipping at refresh?
+        
         # Display the virtual keyboard, ensuring it appears below all widgets
         create_virtual_keyboard(frame1, 8)  # Adjust the row based on your layout needs
 
     else:
         
         if len(xs) == 0:
             frame1.grid_forget()            
@@ -2831,15 +2918,15 @@
  
     # Continue with other actions or functions as needed
     land_or_buoy()
 
 frame1.grid(row=0, column=0, sticky="nsew")
 
 # First line (bold)
-label1 = tk.Label(frame1, text="Welcome to The Weather Observer v3.2.0", font=("Arial", 18, "bold"), bg=tk_background_color, justify="left")
+label1 = tk.Label(frame1, text="Welcome to The Weather Observer v3.3.0", font=("Arial", 18, "bold"), bg=tk_background_color, justify="left")
 label1.grid(row=0, column=0, padx=50, pady=(50, 10), sticky="w")
 
 # Main block of text including the question
 info_text = f'''
 In order to begin, your new instrument needs to be calibrated,
 and you need to make choices about which weather to observe.
 
@@ -3852,20 +3939,14 @@
 
         right_wind_label = tk.Label(transparent_frame, textvariable=right_wind_text, fg="black", bg=tk_background_color, font=obs_font, anchor="w", justify="left")
         right_wind_label.grid(row=0, column=0, padx=750, pady=(40, 0), sticky='w') 
         
     except Exception as e:
         print("printing c land", e)
 
-# # Function to show frame1 and hide the other frames
-# def show_frame1():
-#     frame1.grid(row=0, column=0, sticky="nsew")
-#     baro_frame.grid_forget()
-#     scraped_frame.grid_forget()
-
 #@profile
 # Code for national radar
 def convert_gif_to_jpg_national_radar(gif_data):
     # Open the gif using PIL
     gif = Image.open(BytesIO(gif_data))
 
     # Convert to RGB mode
@@ -3880,15 +3961,15 @@
 
     return output.getvalue()
 
 #@profile
 def display_national_radar():
     try:
         global last_national_radar_scrape_time
-        global img_tk_national_radar
+        global img_label_national_radar, img_tk_national_radar, national_radar_hidden
 
         # Check if 10 minutes have passed since the last scrape or if it's the first time
         current_time = datetime.now()
         if last_national_radar_scrape_time is None or (current_time - last_national_radar_scrape_time).total_seconds() >= 600:
             #print("Getting new national radar. time ", current_time)
             radar_url = 'https://radar.weather.gov/ridge/standard/CONUS_0.gif'
             response = requests.get(radar_url)
@@ -3912,42 +3993,51 @@
                     img_label_national_radar.image = img_tk_national_radar
                     img_label_national_radar.grid(row=1, column=0, padx=130, pady=80, sticky="se")
 
                     # Right after resizing and before or after setting it to the label
                     img_national_radar.save('displayed_national_radar.png')
 
                     root.update()  # Update the tkinter window to show the image
-
+                    # setting national_radar_hidden to false because it's being shown
+                    national_radar_hidden = False
+                    
                     # Use after() to schedule hiding the image after some seconds
-                    root.after(12000, lambda: hide_national_radar(img_label_national_radar))
+                    root.after(12000, lambda: hide_national_radar())
                     
                 except Exception as img_err:
                     print("display_national_radar error:", img_err)
                     show_local_radar_loop()
 
         else:
             # If less than 10 minutes have passed, still display the most recently scraped image
             img_label_national_radar = tk.Label(scraped_frame, image=img_tk_national_radar)
             img_label_national_radar.image = img_tk_national_radar
             img_label_national_radar.grid(row=1, column=0, padx=130, pady=80, sticky="se")
 
             root.update()  # Update the tkinter window to show the image
-                        
+            
+            # setting national_radar_hidden to false because it's being shown
+            national_radar_hidden = False
+            
             # Use after() to schedule hiding the image after some seconds
-            root.after(12000, lambda: hide_national_radar(img_label_national_radar))
+            root.after(12000, lambda: hide_national_radar())
 
     except Exception as e:
         print("Scrape, Save, and Display national radar", e)
         show_local_radar_loop()
         
 #@profile
-def hide_national_radar(img_label_national_radar):
+def hide_national_radar():
+    global img_label_national_radar, national_radar_hidden
     global img_tk_national_radar  # Declare img_tk_national_radar as a global variable
 
-    if img_label_national_radar and img_label_national_radar.winfo_exists():
+    if img_label_national_radar and box_variables[2] != 1 and img_label_national_radar.winfo_exists():
+        # flag established to track whether img_label_national_radar is forgotten to smooth displays
+        national_radar_hidden = True
+
         img_label_national_radar.grid_forget()
 
     show_local_radar_loop()
     
 #@profile
 def show_national_radar():
     global img_tk_national_radar, img_label_national_radar, last_forget_clock, last_national_radar_scrape_time, last_national_sfc_map_scrape_time, last_station_model_scrape_time, last_sounding_scrape_time, last_vorticity_scrape_time, last_national_satellite_scrape_time  # Declare global variables
@@ -3956,15 +4046,15 @@
     current_time = datetime.now()
 
     # Ensure last_forget_clock is initialized
     if last_forget_clock is None:
         last_forget_clock = current_time
 
     if (current_time - last_forget_clock).total_seconds() >= 10800:
-        print("clearing frames")
+        print("clearing frames", current_time)
         # Clear frames
         transparent_frame.grid_forget()
         for widget in transparent_frame.winfo_children():
             widget.destroy()
 
         scraped_frame.grid_forget()
         for widget in scraped_frame.winfo_children():
@@ -4009,14 +4099,15 @@
         display_national_radar()
     else:
         #show_local_radar_loop()
         show_local_radar_loop()
 
 # Code begins for lcl radar loop
 def check_url_lcl_radar(lcl_radar_current_time):
+
     try:
         working_urls_lcl_radar = []
         while len(working_urls_lcl_radar) < 12:
             # Format the URL for the current time
             url = f"https://weather.ral.ucar.edu/data/radar/{lcl_radar_current_time.strftime('%Y%m%d')}/{radar_identifier}/BREF/{radar_identifier}_{lcl_radar_current_time.strftime('%Y%m%d_%H%M00')}_BREF_gray.png"
 
             try:
@@ -4040,97 +4131,118 @@
         # Return a tuple containing a boolean indicating if the current URL is working and the list of working URLs
         return len(working_urls_lcl_radar) == 12, working_urls_lcl_radar
     
     except Exception as e:
         print("check_url_lcl_radar:", e, "going to show_lightning")
         show_lightning()
 
+def start_check_url_lcl_radar_thread(lcl_radar_current_time, callback):
+    def thread_target():
+        success, working_urls_lcl_radar = check_url_lcl_radar(lcl_radar_current_time)
+        root.after(0, lambda: callback(success, working_urls_lcl_radar))
+    
+    Thread(target=thread_target, daemon=True).start()
+
+def resize_images_lcl_radar_threaded(image_urls, callback):
+    def thread_target():
+        resized_images = []
+        for url in image_urls:
+            try:
+                response = requests.get(url, stream=True, timeout=5)  # Added timeout
+                img = Image.open(response.raw)
+                resized_img = img.resize((545, 515), Image.LANCZOS)
+                resized_images.append(ImageTk.PhotoImage(resized_img))
+            except requests.exceptions.RequestException as e:
+                print(f"Request error for {url}: {e}")
+                hide_local_radar_loop(label_lcl_radar)
+            except IOError as e:
+                print(f"Image processing error for {url}: {e}")
+                hide_local_radar_loop(label_lcl_radar)
+        root.after(0, lambda: callback(resized_images))
+
+    Thread(target=thread_target, daemon=True).start()
+
+def on_urls_checked(success, urls):
+    global label_lcl_radar
+    if success:
+        resize_images_lcl_radar_threaded(urls, lambda resized_images: manage_lcl_radar_loop(label_lcl_radar, resized_images))
+    else:
+        print("Failed to find working URLs.")
 
-def resize_image_lcl_radar(img_tk_lcl_radar, width, height):
-    img_tk_lcl_radar_resized = ImageTk.PhotoImage(img_tk_lcl_radar.resize((width, height), Image.LANCZOS))
-    return img_tk_lcl_radar_resized
-
-def manage_lcl_radar_loop(label_lcl_radar, image_list):
-    # Set the parameters for the display function
-    frame_width = 545
-    frame_height = 515
-    frame_duration = 50
-    pause_duration = 2000
-    num_cycles = 3
 
-    try:
-        for cycle in range(num_cycles):
-            idx = 0
-            while idx < len(image_list):
-                # Resize the current frame
-                img_tk_lcl_radar = resize_image_lcl_radar(image_list[idx], frame_width, frame_height)
-
-                # Update the Tkinter window with blending frames
-                label_lcl_radar.config(image=img_tk_lcl_radar)
-                label_lcl_radar.image = img_tk_lcl_radar
-                root.update()
+def manage_lcl_radar_loop(label_lcl_radar, resized_images):
+    frame_duration = 100
+    pause_duration = 2000
+    num_cycles = 4
+    extended_display_duration = 6000 
 
-                # Schedule displaying the next frame after the specified frame duration
-                root.after(frame_duration)
+    # Reverse the order of resized_images to start with the oldest
+    reversed_images = list(reversed(resized_images))
 
-                # Move to the next frame
-                idx += 1
+    def display_next_image(index=0, cycle=0):
+        global img_label_national_radar
+        global national_radar_hidden  # Refer to the flag
+        # Forget national radar image before lcl radar loop is displayed, only once
+        #if not national_radar_hidden and img_label_national_radar and img_label_national_radar.winfo_exists():
+        if national_radar_hidden == False and img_label_national_radar and img_label_national_radar.winfo_exists():    
 
-            # Pause on the final frame for 2 seconds after completing each cycle
-            root.update()
-            root.after(pause_duration)
-    except Exception as e:
-        print("line 4070. Error displaying lcl radar frames:", e, "going to show_lightning")
-        show_lightning()
+            img_label_national_radar.grid_forget()
+            national_radar_hidden = True  # Set the flag to True after hiding
+        
+        try:
+            if index < len(reversed_images):  # Use reversed_images here
+                label_lcl_radar.config(image=reversed_images[index])  # And here
+                label_lcl_radar.image = reversed_images[index]  # And also here
+                root.after(frame_duration, display_next_image, index + 1, cycle)
+            elif cycle + 1 < num_cycles:
+                root.after(pause_duration, display_next_image, 0, cycle + 1)
+            else:
+                # After the last cycle, wait for the extended duration with the last image shown
+                root.after(extended_display_duration, lambda: hide_local_radar_loop(label_lcl_radar))
+        
+        except Exception as e:
+            print("line 4114. error while trying to display next image in lcl radar loop.", e)
+            hide_local_radar_loop(label_lcl_radar)
+            
+    display_next_image()
 
-    # Use after() to schedule hiding the image after the loop has completed
-    root.after(2000, lambda: hide_local_radar_loop(label_lcl_radar, img_tk_lcl_radar))
+def handle_url_check_results(success, urls, label_lcl_radar):
+    if success:
+        try:
+            image_list = [Image.open(requests.get(url, stream=True).raw) for url in urls]
+            #image_list.reverse()  # Reverse the order of images
+            manage_lcl_radar_loop(label_lcl_radar, image_list)
+        except Exception as display_error:
+            print(f"Error display local radar loop: {display_error}")
+            print("line 4121. on way to show_lightning")
+            show_lightning()
+    else:
+        print("Error: Unable to find working URLs.")
 
-def hide_local_radar_loop(label_lcl_radar, img_tk_lcl_radar):
-    img_tk_lcl_radar = None
 
+def hide_local_radar_loop(label_lcl_radar):
+    # Directly use 'label_lcl_radar' to check if it exists and forget it from the grid layout
     if label_lcl_radar and label_lcl_radar.winfo_exists():
         label_lcl_radar.grid_forget()
-
+    
+    # Proceed to the next function in your application's flow
     show_lightning()
 
+
 def display_local_radar_loop():
-    try:
-        # Initialize label
-        label_lcl_radar = tk.Label(scraped_frame)
-        label_lcl_radar.grid(row=1, column=0, padx=250, pady=80, sticky="se")
-
-        # Get the current GMT time minus 5 minutes
-        lcl_radar_current_time = datetime.utcnow() - timedelta(minutes=5)
-
-        # Check URLs and get the list of working URLs
-        is_urls_working, working_urls_lcl_radar = check_url_lcl_radar(lcl_radar_current_time)
-
-        # Print the final list of working URLs
-        #print("Final List of Working URLs:")
-        #for working_url in working_urls_lcl_radar:
-            #print(working_url)
+    global label_lcl_radar
 
-        # Display the radar loop using the function on 'scraped_frame'
-        if is_urls_working:
-            try:
-                image_list = [Image.open(requests.get(url, stream=True).raw) for url in working_urls_lcl_radar]
-                image_list.reverse()  # Reverse the order of images
-                manage_lcl_radar_loop(label_lcl_radar, image_list)
-            except Exception as display_error:
-                print(f"Error display local radar loop: {display_error}")
-                print("line 4112. on way to show_lightning")
-                show_lightning()
-        else:
-            print("Error: Unable to find working URLs.")
+    label_lcl_radar = tk.Label(scraped_frame)  # Assuming scraped_frame is defined
+    label_lcl_radar.grid(row=1, column=0, padx=250, pady=80, sticky="se")
+
+    lcl_radar_current_time = datetime.utcnow() - timedelta(minutes=5)  # Adjust as necessary
+
+    # Start checking URLs in a background thread
+    start_check_url_lcl_radar_thread(lcl_radar_current_time, on_urls_checked)
 
-    except Exception as main_error:
-        print(f"Error in main display function: {main_error}")
-        print("line 4119. on way to show_lightning")
-        show_lightning()
 
 #@profile
 def show_local_radar_loop():
     #global refresh_flag
     if box_variables[2] == 1 and refresh_flag == False :
         # show_national_satellite()
         display_local_radar_loop()
@@ -4232,21 +4344,22 @@
     img_tk_lightning = None  
     
     if img_label and img_label.winfo_exists():
         img_label.grid_forget()
 
     show_national_satellite()
     
-#@profile    
 def show_lightning():
-    #global refresh_flag
-    if box_variables[3] == 1 and refresh_flag == False:
-        display_lightning()
+    if box_variables[3] == 1 and not refresh_flag:
+        # Start display_lightning in a new thread
+        lightning_thread = threading.Thread(target=display_lightning)
+        lightning_thread.start()  # Start the thread
     else:
         show_national_satellite()
+
         
 # Code for national satellite
 #@profile
 def display_national_satellite():
     global img_tk_satellite, last_national_satellite_scrape_time, resized_image, img_label_national_satellite
 
     # Initialize img_label_national_satellite as None
@@ -4449,66 +4562,68 @@
         url = f"{base_url}{year}{day_of_year:03d}{time_code}_GOES{sat_goes}-ABI-{sat_reg}-GEOCOLOR-{image_suffix}"
         urls.append(url)
 
         current_time_utc -= timedelta(minutes=5)  # Go back 5 minutes for the next iteration
 
     return urls
 
-# Function to scrape and display images in a loop
+def trim_near_black_borders_reg_sat(img, threshold=30):
+    """Trim borders that are near-black by dynamically finding the content's bounding box."""
+    # Convert the image to grayscale to simplify finding the border
+    grayscale_img = img.convert("L")
+    # Create a binary image where pixels darker than the threshold are black, others are white
+    binary_img = grayscale_img.point(lambda p: 255 if p > threshold else 0, '1')
+    # Use the binary image to find the bounding box of the content
+    bbox = binary_img.getbbox()
+    if bbox:
+        return img.crop(bbox)
+    return img  # Return the original image if no cropping is needed
+
+
 def scrape_reg_sat_images(urls, sat_goes, sat_reg):
-    # Declare img_label_satellite as a global variable
     global img_label_satellite
-
     images = []
 
     chrome_options = Options()
     chrome_options.add_argument("--headless")
     chrome_options.add_argument("--disable-gpu")
     driver = webdriver.Chrome(service=Service("chromedriver"), options=chrome_options)
 
     try:
-        for url in reversed(urls):  # Reverse the order to start with the oldest image
-            #print(f"Scraping image from URL: {url}")
+        for url in reversed(urls):  # Iterate over URLs
+            try:
+                driver.get(url)
+                if "404 Not Found" in driver.title:
+                    print(f"No image found for URL: {url}")
+                    continue
+
+                screenshot = driver.get_screenshot_as_png()
+                screenshot = Image.open(BytesIO(screenshot))
+
+                #if sat_reg == 'eus' or sat_reg == 'wus':
+                    # Trim the near-black border dynamically
+                screenshot = trim_near_black_borders_reg_sat(screenshot)
+
+                # Resize the image to fit the target size using LANCZOS filter
+                target_size = (515, 515)
+                screenshot = screenshot.resize(target_size, Image.LANCZOS)
+
+                # Convert to Tkinter PhotoImage and append to images list
+                image = ImageTk.PhotoImage(screenshot)
+                images.append(image)
+            except Exception as e:
+                print(f"Error processing image from URL {url}: {e}")
 
-            driver.get(url)
+    finally:
+        driver.quit()
 
-            # Check if the page returned a 404 status code (no image available)
-            if "404 Not Found" in driver.title:
-                print(f"No image found for URL: {url}")
-                continue
+    # Your existing code to display images
+    display_reg_sat_loop(images)
 
-            # Capture the screenshot of the page
-            screenshot = driver.get_screenshot_as_png()
-            screenshot = Image.open(BytesIO(screenshot))
-
-            # Calculate resizing dimensions to fit the image within the 510x510 window
-            target_size = (515, 515)
-            ratio = max(target_size[0] / screenshot.width, target_size[1] / screenshot.height)
-            new_size = (int(screenshot.width * ratio), int(screenshot.height * ratio))
-
-            # Resize the image without stretching vertically
-            screenshot = screenshot.resize(new_size, Image.LANCZOS)
-
-            # Calculate margins to center the image in the window
-            left_margin = (target_size[0] - new_size[0]) // 2
-            top_margin = (target_size[1] - new_size[1]) // 2
-
-            # Create a blank canvas with the target size and a consistent background color
-            blank_canvas = Image.new("RGB", target_size, "lightblue")
-            blank_canvas.paste(screenshot, (left_margin, top_margin))
-
-            # Convert to Tkinter PhotoImage
-            image = ImageTk.PhotoImage(blank_canvas)
-            images.append(image)
 
-    except Exception as e:
-        print(f"Line 4504. Error scrape reg sat images from URL {url}: {e} on way to error_manage_loop")
-        show_national_sfc_map()
-    driver.quit()
-    display_reg_sat_loop(images)
 
 # Create a threading lock
 tkinter_lock = threading.Lock()
 
 # Function to display images in a Tkinter window
 def display_reg_sat_loop(images):
     # Declare img_label_satellite as a global variable
@@ -4533,58 +4648,65 @@
                 idx += 1
                 tkinter_lock.release()
 
                 scraped_frame.after(100, update_image)  # Schedule the next frame
             elif reg_sat_num_cycles == 5:
                 scraped_frame.after(2000, hide_reg_sat_loop)
             else:
-                # Reset index to start from the beginning for the next cycle
-                time.sleep(2)
-                idx = 0
-                reg_sat_num_cycles += 1
-                scraped_frame.after(100, update_image)  # Schedule the next frame
+                # Schedule to reset index and increment reg_sat_num_cycles after a 2-second pause
+                def reset_and_continue():
+                    nonlocal idx, reg_sat_num_cycles
+                    idx = 0
+                    reg_sat_num_cycles += 1
+                    update_image()  # Continue with the next image
+
+                scraped_frame.after(2000, reset_and_continue)
+
 
         # Use grid to specify the row and column, and padx/pady for padding
         img_label_satellite.grid(row=1, column=0, padx=250, pady=80, sticky='se')
 
         # Schedule the first call to update_image
         scraped_frame.after(0, update_image)
         
     except Exception as e:
         print("Line 4553. display_reg_sat_loop", e, "on way to national sfc map")
-        show_national_sfc_map()       
+        show_national_sfc_map()
+        
+        
 # Function to hide the Tkinter window after displaying images
 def hide_reg_sat_loop():
     global img_label_satellite
     if img_label_satellite:
         img_label_satellite.grid_forget()
         img_label_satellite = None
         
         
     show_national_sfc_map()
 
-def show_reg_sat_loop():
-    # global refresh_flag
-    # Is this a user choice?
-    if box_variables[5] == 1 and refresh_flag == False:        
-        base_url = "https://cdn.star.nesdis.noaa.gov/GOES{}/ABI/SECTOR/{}/GEOCOLOR/"
-                    
-        num_images_to_scrape = 12
 
-        sat_goes, sat_reg = get_reg_sat_settings()
+def threaded_satellite_scraping():
+    # Place the setup code here if any
+    base_url = "https://cdn.star.nesdis.noaa.gov/GOES{}/ABI/SECTOR/{}/GEOCOLOR/"
+    num_images_to_scrape = 12
+    sat_goes, sat_reg = get_reg_sat_settings()
+    urls_to_scrape = generate_sat_reg_urls(base_url.format(sat_goes, sat_reg), num_images_to_scrape, sat_goes, sat_reg)
 
-        # Pass sat_goes and sat_reg to generate_sat_reg_urls
-        urls_to_scrape = generate_sat_reg_urls(base_url.format(sat_goes, sat_reg), num_images_to_scrape, sat_goes,
-                                               sat_reg)
-
-        scrape_reg_sat_images(urls_to_scrape, sat_goes, sat_reg)
+    # Call the scraping function in the thread
+    scrape_reg_sat_images(urls_to_scrape, sat_goes, sat_reg)
 
+def show_reg_sat_loop():
+    if box_variables[5] == 1 and refresh_flag == False:
+        # Start the scraping process in a new thread to keep the GUI responsive
+        scraping_thread = threading.Thread(target=threaded_satellite_scraping)
+        scraping_thread.start()
     else:
         show_national_sfc_map()
-        
+
+
 #@profile
 def display_national_sfc_map():
     try:
         global last_national_sfc_map_scrape_time
         global img_tk_sfc_map  # Declare img_tk_sfc_map as a global variable
         global img_label_sfc_map  # Declare img_label_sfc_map as a global variable
 
@@ -4629,31 +4751,34 @@
 
             # Use after() to schedule hiding the image after some seconds
             root.after(12000, lambda: hide_national_sfc_map(img_label_sfc_map))
 
     except Exception as e:
         print("National surface map scrape error:", e, "on way to show_station_models")
         show_station_models()
+        
 #@profile
 def hide_national_sfc_map(img_label_sfc_map):
     
     if img_label_sfc_map and img_label_sfc_map.winfo_exists():
         img_label_sfc_map.grid_forget()
 
     show_station_models()
+    
 #@profile
 def show_national_sfc_map():
     #global refresh_flag
     if box_variables[6] == 1 and refresh_flag == False:
         # Move the variable assignment here
         last_national_sfc_map_scrape_time = None
 
         display_national_sfc_map()
     else:
         show_station_models()
+        
 #@profile        
 def display_station_models():
     global station_model_url, zoom_plot, img_tk_station_model, last_station_model_scrape_time
     timeout_seconds = 30
     try:
         # Check if 3 minutes have passed since the last scrape or if it's the first time
         current_timestamp = datetime.now()
@@ -4748,19 +4873,18 @@
         # Explicit garbage collection
         gc.collect()
         
     show_sounding()
     
 #@profile
 def show_station_models():
-    #global refresh_flag
-    # Is this a user choice?
-    if box_variables[7] == 1 and refresh_flag == False:
-        #timeout_seconds = 30 
-        display_station_models()
+    if box_variables[7] == 1 and not refresh_flag:
+        # Start display_station_models in a new thread to prevent GUI blockage
+        station_models_thread = threading.Thread(target=display_station_models)
+        station_models_thread.start()  # Start the thread
     else:
         show_sounding()
 
 def display_sounding():
     global last_sounding_scrape_time, sonde_letter_identifier, img_tk_sounding
 
     try:
```

