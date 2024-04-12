# Comparing `tmp/easyoutput-0.1.0.tar.gz` & `tmp/easyoutput-0.1.1.tar.gz`

## Comparing `easyoutput-0.1.0.tar` & `easyoutput-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 easyoutput-0.1.0/README.MD
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.1.0/.github/ISSUE_TEMPLATE/🐞-bug-report.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.1.0/.github/ISSUE_TEMPLATE/🚀feature-request.md
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 easyoutput-0.1.0/img/EasyOutputSmallLogo.png
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 easyoutput-0.1.0/src/EasyOutput/EasyOutput.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 easyoutput-0.1.0/src/EasyOutput/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 easyoutput-0.1.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 easyoutput-0.1.0/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 easyoutput-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 easyoutput-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 easyoutput-0.1.1/README.MD
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 easyoutput-0.1.1/.github/ISSUE_TEMPLATE/🐞-bug-report.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 easyoutput-0.1.1/.github/ISSUE_TEMPLATE/🚀-feature-request-.md
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 easyoutput-0.1.1/src/EasyOutput/EasyOutput.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 easyoutput-0.1.1/src/EasyOutput/__init__.py
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 easyoutput-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 easyoutput-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 easyoutput-0.1.1/README.md
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 easyoutput-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 easyoutput-0.1.1/PKG-INFO
```

### Comparing `easyoutput-0.1.0/README.MD` & `easyoutput-0.1.1/README.MD`

 * *Files 12% similar despite different names*

```diff
@@ -1,182 +1,206 @@
-# Easy Output 
-```py 
+# Easy Output
+
+```py
 # How to use 👽
 from EasyOutput.EasyOutput import *
 ```
+
 ![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)\
-![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&label=Monthly%20Downloads&color=358)\
-![PyPI - Downloads](https://img.shields.io/pypi/dw/EasyOutput?style=for-the-badge&logo=pypi&label=Weekly%20Downloads&color=358)\
-![PyPI - Downloads](https://img.shields.io/pypi/dd/EasyOutput?style=for-the-badge&logo=pypi&label=Daily%20Downloads&color=358)\
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)\
+![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi)
+\
+![PyPI - Downloads](https://img.shields.io/pypi/dw/EasyOutput?style=for-the-badge&logo=pypi)
+\
+![PyPI - Downloads](https://img.shields.io/pypi/dd/EasyOutput?style=for-the-badge&logo=pypi)
+\
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/RasinBrand/EasyOutput?style=for-the-badge&logo=github)\
 ![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
 > [!IMPORTANT]
 > I am always updating this and sometimes those updates can go sideways. Please use the [issues](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) section on github to notify me of anything i have missed! If you would like me to add something, please use the [Feature Request](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) option!
 
+## Information ℹ️
 
-## Information
 **EasyOutput** consists of easy colored print options without the extra work.
 
 ```py
-# You can now highlight your message aswell! 
-Success_Message("New Highlight!", highlight=True)
-
-# Or keep it og 😄
-Success_Message("No Highlight!")
-# Same as
-Success_Message("No Highlight!", highlight=False)
-
 # As of v0.1.0 you can now change the color of your text.
 from EasyOutput.EasyOutput import Colors, Success_Message
 
 Success_Message("EasyOutput", color=Colors.Green)
+
+# As of v0.1.1 you can change the color of the title and highlight!
+from EasyOutput.EasyOutput import Colors, Highlights, Success_Message
+
+Success_Message("EasyOutput", color=Colors.Green, highlight=Highlights.Blue, title_color=Colors.White)
+
+
 ```
 
 In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing:
+
 ```py
 from colorama import Fore, Style
 
 def Success(message):
     print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
 
 print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
 # and calling it like so
 
 Success("Your Success Message")
 ```
 
-If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal! 
+If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal!
 
 ## Important Information 🥇
-[colorama](https://pypi.org/project/colorama/) and It's creator has done all heavy lifting here please show him some love!
 
-[Jonathan Hartley](https://github.com/tartley)\
-[colorama repo](https://github.com/tartley/colorama)
+**[colorama](https://pypi.org/project/colorama/) and It's creator has done all heavy lifting here please show him some love!** \
+ **[Jonathan Hartley](https://github.com/tartley)**\
+ **[colorama repo](https://github.com/tartley/colorama)**
 
 ## PYPI
 
 [EasyOutput](https://pypi.org/project/EasyOutput/)
 
-
 Badges from: [Shields.io](https://shields.io/badges)
 
 <details>
 <summary>Change-Log 📝</summary>
 
-[comment]: <> (v0.0.1)
 <details>
 <summary>v0.0.1</summary>
 
     ADDED
     - Success Message
     - Error Message
     - Wait Message
+
 </details>
 
-[comment]: <> (v0.0.2)
 <details>
 <summary>v0.0.2</summary>
     
     ADDED
     - Connection Success Message
     - Connection Error Message
 
 </details>
 
-[comment]: <> (v0.0.3)
 <details>
 <summary>v0.0.3</summary>
     
     ADDED
     - Function Notes
 
     FIXED
     - Small Success Message Bugs
+
 </details>
 
-[comment]: <> (v0.0.4)
 <details>
 <summary>v0.0.4</summary>
     
     ADDED
     - Info Mesage
     - Note Message
 </details>
 
-[comment]: <> (v0.0.5)
 <details>
 <summary>v0.0.5</summary>
 
     ADDED
     - Title Print
 
     FIXED
     - Calling issues
+
 </details>
 
-[comment]: <> (v0.0.6)
 <details>
 <summary>v0.0.6</summary>
 
     ADDED
     - REDACTED Message
 
     REMOVED
     - Usless Classes
+
 </details>
 
-[comment]: <> (v0.0.7)
 <details>
 <summary>v0.0.7</summary>
     
     REMOVED
-    - Wait Message 
+    - Wait Message
 
     ADDED
     - Warning Message
 
     FIXED
     - imports
+
 </details>
 
-[comment]: <> (v0.0.7.1)
 <details>
 <summary>v0.0.7.1</summary>
 
     FIXED
-    - 
+    -
+
 </details>
 
-[comment]: <> (v0.0.8)
 <details>
 <summary>v0.0.8</summary>
 
     ADDED
     - Highlight Message Option!
+
 </details>
 
-[comment]: <> (v0.0.8.1)
 <details>
 <summary>v0.0.8.1</summary>
 
     FIXED
     - Leaving all functions at the bottom of the file... IM SORRY
+
 </details>
 
-[comment]: <> (v0.0.9)
 <details>
 <summary>v0.0.9</summary>
 
     FIXED
     - Optioanl Highlight!
+
 </details>
 
-[comment]: <> (v0.0.9.1)
 <details>
 <summary>v0.0.9.1</summary>
 
     FIXED
     - Info message oddly popping up after every function
+
+</details>
+
+<details>
+<summary>v0.1.0</summary>
+
+    ADDED
+    - Colored text option
+    - Custom Message
+    - Show all colors function
+
+</details>
+
+<details>
+<summary>v0.1.1</summary>
+
+    ADDED
+    - Highlight any color!
+    - Ability to color any part of the message!
+
+    FIXED
+    - Highlights
+
 </details>
 
 </details>
```

### Comparing `easyoutput-0.1.0/.github/ISSUE_TEMPLATE/🚀feature-request.md` & `easyoutput-0.1.1/.github/ISSUE_TEMPLATE/🚀-feature-request-.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-name: "\U0001F680Feature Request"
+name: "\U0001F680 Feature Request "
 about: Suggest an idea for this project
 title: ''
 labels: ''
 assignees: ''
 
 ---
```

### Comparing `easyoutput-0.1.0/src/EasyOutput/EasyOutput.py` & `easyoutput-0.1.1/src/EasyOutput/EasyOutput.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import colorama
 
 reset = Style.RESET_ALL
 brighten = Style.BRIGHT
 dim_message = Style.DIM
 
 class Colors:
-    
     def Show():
         """
         Shows all available colors 
         """
         Title_Print("All Colors", color=Colors.Cyan)
         Colored_Message("Red", color=Colors.Red)
         Colored_Message("Light Red", color=Colors.Light_Red)
@@ -46,15 +45,36 @@
     Light_Yellow = Fore.LIGHTYELLOW_EX
     Light_Cyan = Fore.LIGHTCYAN_EX
     Light_White = Fore.LIGHTWHITE_EX
     Light_Magenta = Fore.LIGHTMAGENTA_EX
 
 
 class Highlights:
-    none = ""
+    def Show():
+        """
+        Shows all available highlight colors 
+        """
+        Title_Print("All Colors", color=Colors.Cyan)
+        Colored_Message("Red", color=Colors.Red)
+        Colored_Message("Light Red", color=Colors.Light_Red)
+        Colored_Message("Green", color=Colors.Green)
+        Colored_Message("Light Green", color=Colors.Light_Green)
+        Colored_Message("Blue", color=Colors.Blue)
+        Colored_Message("Light Blue", color=Colors.Light_Blue)
+        Colored_Message("Black", color=Colors.Black)
+        Colored_Message("Light Black", color=Colors.Light_Black)
+        Colored_Message("Yellow", color=Colors.Yellow)
+        Colored_Message("Light Yellow", color=Colors.Light_Yellow)
+        Colored_Message("Cyan", color=Colors.Cyan)
+        Colored_Message("Light Cyan", color=Colors.Light_Cyan)
+        Colored_Message("White", color=Colors.White)
+        Colored_Message("Light White", color=Colors.Light_White)
+        Colored_Message("Magenta", color=Colors.Magenta)
+        Colored_Message("Light Magenta", color=Colors.Light_Magenta)
+        
     Red = bg.RED
     Green = bg.GREEN
     Blue = bg.BLUE
     Black = bg.BLACK
     Yellow = bg.YELLOW
     Cyan = bg.CYAN
     White = bg.WHITE
@@ -65,153 +85,128 @@
     Light_Black = bg.LIGHTBLACK_EX
     Light_Yellow = bg.LIGHTYELLOW_EX
     Light_Cyan = bg.LIGHTCYAN_EX
     Light_White = bg.LIGHTWHITE_EX
     Light_Magenta = bg.LIGHTMAGENTA_EX
 
 
-def Info_Message(message, color: Colors = Colors.White, highlight: bool = False):  
+def Info_Message(message, color: Colors = Colors.White, highlight: Highlights = '', title_color: Colors = Colors.Blue):  
     """
-    Prints a message notifying the user of specific need to know information.
+    This function prints out an informational message.
+    
+    color: color your direct message a specific color, default is white.
     
-    color
-        Color your message! The standard is set to white.
+    highlight: highlight the message in a specific color!
     
-    highlight
-        Blue
+    title_color: Color the title of the message, default is blue.
     """
-
-    if highlight == True:
-        print(f"{Fore.BLUE + brighten}Info{reset}: {bg.BLUE + color + message + reset}")
-    elif highlight == False:    
-        print(f"{Fore.BLUE + brighten}Info{reset}: {color + message + reset}")
+    print(f"{title_color + brighten}Info{reset}: {highlight + color + message + reset}")
     
-def Error_Message(message, color: Colors = Colors.White, highlight: bool = False):
+def Error_Message(message, color: Colors = Colors.White, highlight: Highlights = '', title_color: Colors = Colors.Red):
     """
-    Prints a message notifying the user of an error.
+    This function prints out an error message.
+    
+    color: color your direct message a specific color, default is white.
     
-    colo
-        Color your message! The standard is set to white.
+    highlight: highlight the message in a specific color!
     
-    highlight
-        Red
+    title_color: Color the title of the message, default is red.
     """
-    if highlight == True:
-        print(f"{Fore.RED}Error{reset}: {bg.RED + color + message + reset}")
-    elif highlight == False:
-        print(f"{Fore.RED}Error{reset}: {color + message + reset}")
+    print(f"{title_color}Error{reset}: {highlight + color + message + reset}")
+
     
-def Connection_Error_Message(message, color: Colors = Colors.White, highlight: bool = False):
+def Connection_Error_Message(message, color: Colors = Colors.White, highlight: Highlights = '', title_color: Colors = Colors.Red):
     """
-    Prints a message notifying the user of a connection error.
+    This function prints out a failed connection message.
+    
+    color: color your direct message a specific color, default is white.
     
-    colo
-        Color your message! The standard is set to white.
+    highlight: highlight the message in a specific color!
     
-    highlight
-        Red
+    title_color: Color the title of the message, default is red.
     """
-    if highlight == True:
-        print(f"{Fore.RED}Connection Error{reset}: {bg.RED + color +  message + reset}")
-        
-    elif highlight == False:    
-        print(f"{Fore.RED}Connection Error{reset}: {color + message + reset}")
+    print(f"{title_color}Connection Error{reset}: {highlight + color +  message + reset}")
     
-def Success_Message(message, color: Colors = Colors.White, highlight: bool = False):
+def Success_Message(message, color: Colors = Colors.White, highlight: Highlights = '', title_color: Colors = Colors.Green):
     """
-    Prints a message notifying the user of a success.
+    This function prints out a success message.
     
-    color:
-        Color your message! The standard is set to white.
+    color: color your direct message a specific color, default is white.
     
-    highlight
-        Green
+    highlight: highlight the message in a specific color!
+    
+    title_color: Color the title of the message, default is green.
     """
-    if highlight == True:
-        print(f"{Fore.GREEN + brighten}Success{reset}: {bg.GREEN + color + message + reset}")
-    elif highlight == False:
-        print(f"{Fore.GREEN + brighten}Success{reset}: {color + message + reset}")
+    print(f"{title_color + brighten}Success{reset}: {highlight + color + message + reset}")
     
-def Successful_Connection_Message(message, color: Colors = Colors.White, highlight: bool = False):
+def Successful_Connection_Message(message, color: Colors = Colors.White, highlight: Highlights = '', title_color: Colors = Colors.Green):
     """
-    Prints a message notifying the user of a successful connection.
+    This function prints out a successful connection message.
+    
+    color: color your direct message a specific color, default is white.
     
-    color:
-        Color your message! The standard is set to white.
+    highlight: highlight the message in a specific color!
     
-    highlight
-        Green
+    title_color: Color the title of the message, default is green.
     """
-    if highlight == True:
-        print(f"{Fore.GREEN + brighten}Successful Connection{reset}: {bg.GREEN + color + message + reset}")
-    elif highlight == False:
-        print(f"{Fore.GREEN + brighten}Successful Connection{reset}: {color + message + reset}")
+    print(f"{title_color + brighten}Successful Connection{reset}: {highlight + color + message + reset}")
     
-def Note_Message(message, color: Colors = Colors.White, highlight: bool = False):
+def Note_Message(message, color: Colors = Colors.White, highlight: Highlights = '', title_color: Colors = Colors.Yellow):
     """
-    Prints a note notifying the user of something they should be made aware of.
+    This function prints out something the user should take note of.
     
-    color: 
-        Color your message! The standard is set to white.
+    color: color your direct message a specific color, default is white.
     
-    highlight
-        Yellow
+    highlight: highlight the message in a specific color!
+    
+    title_color: Color the title of the message, default is yellow.
     """
-    if highlight == True:
-        print(f"{Fore.YELLOW}Note{reset}: {bg.YELLOW + color +  message + reset}")
-    elif highlight == False:    
-        print(f"{Fore.YELLOW}Note{reset}: {color + message + reset}")
+    print(f"{title_color}Note{reset}: {highlight + color +  message + reset}")
     
-def Warning_Message(message, color: Colors = Colors.White, highlight: bool = False):
+def Warning_Message(message, color: Colors = Colors.White, highlight: Highlights = '', title_color: Colors = Colors.Yellow):
     """
-    Prints a warning message for the user indicating your code is running.
+    This function prints out a warning message.
+    
+    color: color your direct message a specific color, default is white.
     
-    color: 
-        Color your message! The standard is set to white.
+    highlight: highlight the message in a specific color!
     
-    highlight
-        Yellow
+    title_color: Color the title of the message, default is yellow.
     """
-    if highlight == True:
-        print(f"{Fore.YELLOW}Warning{reset}: {bg.YELLOW + color +  message + reset}")    
-    elif highlight == False:
-        print(f"{Fore.YELLOW}Warning{reset}: {color + message + reset}")
+    print(f"{title_color}Warning{reset}: {highlight + color +  message + reset}")    
+
     
-def Title_Print(title, color: Colors = Colors.Green, highlight: bool = False):
+def Title_Print(title, color: Colors = Colors.Green, highlight: Highlights = ''):
     """
-    Prints a title for grouping lists and anything else you can think of.
+    This function prtins out a title.
     
-    color:
-        Color your message! The standard is set to green.
+    color: color your direct message a specific color, default is green.
     
-    highlight
-        Green
+    highlight: highlight the message in a specific color!
     """
-    if highlight == True:
-        print(f"=== {bg.GREEN + color + brighten + title + reset} ===")    
-    elif highlight == False:
-        print(f"=== {color + brighten + title + reset} ===")
+    print(f"=== {highlight + color + brighten + title + reset} ===")    
+
      
-def Redacted_Message(message, color: Colors = Colors.White, highlight: bool = False):
+def Redacted_Message(message, color: Colors = Colors.White, highlight: Highlights = '', title_color: Colors = Colors.Red):
     """
-    Prints redacted message 
+    This function prints out a redacted message.
+    
+        The use of this is un-realistic, i just made it for fun.
     
-    color:
-        Color your message! The standard is set to white.
+    color: color your direct message a specific color, default is white.
     
-    highlight
-        Red
+    highlight: highlight the message in a specific color!
+    
+    title_color: Color the title of the message, default is yellow.
     """
-    if highlight == True:
-        print(f"{Fore.RED}REDACTED{reset}: {bg.RED + color + message + reset}")    
-    elif highlight == False:
-        print(f"{Fore.RED}REDACTED{reset}: {color + message + reset}")
+    print(f"{title_color}REDACTED{reset}: {highlight + color + message + reset}")    
+
 
-def Colored_Message(message, color: Colors = Colors.White):
+def Colored_Message(message, color: Colors = Colors.White, highlight: Highlights = ''):
     """
-    Prints user written message!
+    This function allows you to print out your own colored message with ease!
     
-    color:
-        Color your message! The standard is set to white.
-
+    color: color your direct message a specific color, default is white.
+    
+    highlight: highlight the message in a specific color!
     """
-    print(color + message + reset)
+    print(highlight + color + message + reset)
```

### Comparing `easyoutput-0.1.0/LICENSE.txt` & `easyoutput-0.1.1/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [2024] [FrankAustin]
+Copyright (c) 2024 Brandon McKinney
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `easyoutput-0.1.0/README.md` & `easyoutput-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,182 +1,206 @@
-# Easy Output 
-```py 
+# Easy Output
+
+```py
 # How to use 👽
 from EasyOutput.EasyOutput import *
 ```
+
 ![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)\
-![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&label=Monthly%20Downloads&color=358)\
-![PyPI - Downloads](https://img.shields.io/pypi/dw/EasyOutput?style=for-the-badge&logo=pypi&label=Weekly%20Downloads&color=358)\
-![PyPI - Downloads](https://img.shields.io/pypi/dd/EasyOutput?style=for-the-badge&logo=pypi&label=Daily%20Downloads&color=358)\
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)\
+![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi)
+\
+![PyPI - Downloads](https://img.shields.io/pypi/dw/EasyOutput?style=for-the-badge&logo=pypi)
+\
+![PyPI - Downloads](https://img.shields.io/pypi/dd/EasyOutput?style=for-the-badge&logo=pypi)
+\
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/RasinBrand/EasyOutput?style=for-the-badge&logo=github)\
 ![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
 > [!IMPORTANT]
 > I am always updating this and sometimes those updates can go sideways. Please use the [issues](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) section on github to notify me of anything i have missed! If you would like me to add something, please use the [Feature Request](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) option!
 
+## Information ℹ️
 
-## Information
 **EasyOutput** consists of easy colored print options without the extra work.
 
 ```py
-# You can now highlight your message aswell! 
-Success_Message("New Highlight!", highlight=True)
-
-# Or keep it og 😄
-Success_Message("No Highlight!")
-# Same as
-Success_Message("No Highlight!", highlight=False)
-
 # As of v0.1.0 you can now change the color of your text.
 from EasyOutput.EasyOutput import Colors, Success_Message
 
 Success_Message("EasyOutput", color=Colors.Green)
+
+# As of v0.1.1 you can change the color of the title and highlight!
+from EasyOutput.EasyOutput import Colors, Highlights, Success_Message
+
+Success_Message("EasyOutput", color=Colors.Green, highlight=Highlights.Blue, title_color=Colors.White)
+
+
 ```
 
 In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing:
+
 ```py
 from colorama import Fore, Style
 
 def Success(message):
     print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
 
 print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
 # and calling it like so
 
 Success("Your Success Message")
 ```
 
-If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal! 
+If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal!
 
 ## Important Information 🥇
-[colorama](https://pypi.org/project/colorama/) and It's creator has done all heavy lifting here please show him some love!
 
-[Jonathan Hartley](https://github.com/tartley)\
-[colorama repo](https://github.com/tartley/colorama)
+**[colorama](https://pypi.org/project/colorama/) and It's creator has done all heavy lifting here please show him some love!** \
+ **[Jonathan Hartley](https://github.com/tartley)**\
+ **[colorama repo](https://github.com/tartley/colorama)**
 
 ## PYPI
 
 [EasyOutput](https://pypi.org/project/EasyOutput/)
 
-
 Badges from: [Shields.io](https://shields.io/badges)
 
 <details>
 <summary>Change-Log 📝</summary>
 
-[comment]: <> (v0.0.1)
 <details>
 <summary>v0.0.1</summary>
 
     ADDED
     - Success Message
     - Error Message
     - Wait Message
+
 </details>
 
-[comment]: <> (v0.0.2)
 <details>
 <summary>v0.0.2</summary>
     
     ADDED
     - Connection Success Message
     - Connection Error Message
 
 </details>
 
-[comment]: <> (v0.0.3)
 <details>
 <summary>v0.0.3</summary>
     
     ADDED
     - Function Notes
 
     FIXED
     - Small Success Message Bugs
+
 </details>
 
-[comment]: <> (v0.0.4)
 <details>
 <summary>v0.0.4</summary>
     
     ADDED
     - Info Mesage
     - Note Message
 </details>
 
-[comment]: <> (v0.0.5)
 <details>
 <summary>v0.0.5</summary>
 
     ADDED
     - Title Print
 
     FIXED
     - Calling issues
+
 </details>
 
-[comment]: <> (v0.0.6)
 <details>
 <summary>v0.0.6</summary>
 
     ADDED
     - REDACTED Message
 
     REMOVED
     - Usless Classes
+
 </details>
 
-[comment]: <> (v0.0.7)
 <details>
 <summary>v0.0.7</summary>
     
     REMOVED
-    - Wait Message 
+    - Wait Message
 
     ADDED
     - Warning Message
 
     FIXED
     - imports
+
 </details>
 
-[comment]: <> (v0.0.7.1)
 <details>
 <summary>v0.0.7.1</summary>
 
     FIXED
-    - 
+    -
+
 </details>
 
-[comment]: <> (v0.0.8)
 <details>
 <summary>v0.0.8</summary>
 
     ADDED
     - Highlight Message Option!
+
 </details>
 
-[comment]: <> (v0.0.8.1)
 <details>
 <summary>v0.0.8.1</summary>
 
     FIXED
     - Leaving all functions at the bottom of the file... IM SORRY
+
 </details>
 
-[comment]: <> (v0.0.9)
 <details>
 <summary>v0.0.9</summary>
 
     FIXED
     - Optioanl Highlight!
+
 </details>
 
-[comment]: <> (v0.0.9.1)
 <details>
 <summary>v0.0.9.1</summary>
 
     FIXED
     - Info message oddly popping up after every function
+
+</details>
+
+<details>
+<summary>v0.1.0</summary>
+
+    ADDED
+    - Colored text option
+    - Custom Message
+    - Show all colors function
+
+</details>
+
+<details>
+<summary>v0.1.1</summary>
+
+    ADDED
+    - Highlight any color!
+    - Ability to color any part of the message!
+
+    FIXED
+    - Highlights
+
 </details>
 
 </details>
```

### Comparing `easyoutput-0.1.0/pyproject.toml` & `easyoutput-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EasyOutput"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
-  { name="FrankAustin", email="frankaustindev808@gmail.com" },
+  { name="Brandon McKinney", email="brandonaustinmck01@icloud.com" },
 ]
 description = "Colored messages in the palm of your hand"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 keywords = [
   "Error Message", "Success Message", "Warning Message", "Easy", "Colored Messages"
 ]
 maintainers = [
-  {name = "FrankAustin", email="frankaustindev808@gmail.com"}
+  {name = "Brandon McKinney", email="brandonaustinmck01@icloud.com"}
 ]
 requires-python = ">=3.12"
 install_requires= ['colorama']
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
@@ -30,10 +30,10 @@
 ]
 dependencies = [
   "colorama"
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/FrankAustin808/EasyOut/"
-"Issues" = "https://github.com/FrankAustin808/EasyOut/issues/new/choose"
-"Feature Request" = "https://github.com/FrankAustin808/EasyOut/issues/new/choose"
+"Homepage" = "https://github.com/RasinBrand/EasyOutput/"
+"Issues" = "https://github.com/RasinBrand/EasyOutput/issues/new/choose"
+"Feature Request" = "https://github.com/RasinBrand/EasyOutput/issues/new/choose"
```

### Comparing `easyoutput-0.1.0/PKG-INFO` & `easyoutput-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: EasyOutput
-Version: 0.1.0
+Version: 0.1.1
 Summary: Colored messages in the palm of your hand
-Project-URL: Homepage, https://github.com/FrankAustin808/EasyOut/
-Project-URL: Issues, https://github.com/FrankAustin808/EasyOut/issues/new/choose
-Project-URL: Feature Request, https://github.com/FrankAustin808/EasyOut/issues/new/choose
-Author-email: FrankAustin <frankaustindev808@gmail.com>
-Maintainer-email: FrankAustin <frankaustindev808@gmail.com>
+Project-URL: Homepage, https://github.com/RasinBrand/EasyOutput/
+Project-URL: Issues, https://github.com/RasinBrand/EasyOutput/issues/new/choose
+Project-URL: Feature Request, https://github.com/RasinBrand/EasyOutput/issues/new/choose
+Author-email: Brandon McKinney <brandonaustinmck01@icloud.com>
+Maintainer-email: Brandon McKinney <brandonaustinmck01@icloud.com>
 License: MIT License
         
-        Copyright (c) [2024] [FrankAustin]
+        Copyright (c) 2024 Brandon McKinney
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -37,189 +37,213 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Requires-Dist: colorama
 Description-Content-Type: text/markdown
 
-# Easy Output 
-```py 
+# Easy Output
+
+```py
 # How to use 👽
 from EasyOutput.EasyOutput import *
 ```
+
 ![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)\
-![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&label=Monthly%20Downloads&color=358)\
-![PyPI - Downloads](https://img.shields.io/pypi/dw/EasyOutput?style=for-the-badge&logo=pypi&label=Weekly%20Downloads&color=358)\
-![PyPI - Downloads](https://img.shields.io/pypi/dd/EasyOutput?style=for-the-badge&logo=pypi&label=Daily%20Downloads&color=358)\
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)\
+![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi)
+\
+![PyPI - Downloads](https://img.shields.io/pypi/dw/EasyOutput?style=for-the-badge&logo=pypi)
+\
+![PyPI - Downloads](https://img.shields.io/pypi/dd/EasyOutput?style=for-the-badge&logo=pypi)
+\
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/RasinBrand/EasyOutput?style=for-the-badge&logo=github)\
 ![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
 > [!IMPORTANT]
 > I am always updating this and sometimes those updates can go sideways. Please use the [issues](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) section on github to notify me of anything i have missed! If you would like me to add something, please use the [Feature Request](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) option!
 
+## Information ℹ️
 
-## Information
 **EasyOutput** consists of easy colored print options without the extra work.
 
 ```py
-# You can now highlight your message aswell! 
-Success_Message("New Highlight!", highlight=True)
-
-# Or keep it og 😄
-Success_Message("No Highlight!")
-# Same as
-Success_Message("No Highlight!", highlight=False)
-
 # As of v0.1.0 you can now change the color of your text.
 from EasyOutput.EasyOutput import Colors, Success_Message
 
 Success_Message("EasyOutput", color=Colors.Green)
+
+# As of v0.1.1 you can change the color of the title and highlight!
+from EasyOutput.EasyOutput import Colors, Highlights, Success_Message
+
+Success_Message("EasyOutput", color=Colors.Green, highlight=Highlights.Blue, title_color=Colors.White)
+
+
 ```
 
 In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing:
+
 ```py
 from colorama import Fore, Style
 
 def Success(message):
     print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
 
 print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
 # and calling it like so
 
 Success("Your Success Message")
 ```
 
-If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal! 
+If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal!
 
 ## Important Information 🥇
-[colorama](https://pypi.org/project/colorama/) and It's creator has done all heavy lifting here please show him some love!
 
-[Jonathan Hartley](https://github.com/tartley)\
-[colorama repo](https://github.com/tartley/colorama)
+**[colorama](https://pypi.org/project/colorama/) and It's creator has done all heavy lifting here please show him some love!** \
+ **[Jonathan Hartley](https://github.com/tartley)**\
+ **[colorama repo](https://github.com/tartley/colorama)**
 
 ## PYPI
 
 [EasyOutput](https://pypi.org/project/EasyOutput/)
 
-
 Badges from: [Shields.io](https://shields.io/badges)
 
 <details>
 <summary>Change-Log 📝</summary>
 
-[comment]: <> (v0.0.1)
 <details>
 <summary>v0.0.1</summary>
 
     ADDED
     - Success Message
     - Error Message
     - Wait Message
+
 </details>
 
-[comment]: <> (v0.0.2)
 <details>
 <summary>v0.0.2</summary>
     
     ADDED
     - Connection Success Message
     - Connection Error Message
 
 </details>
 
-[comment]: <> (v0.0.3)
 <details>
 <summary>v0.0.3</summary>
     
     ADDED
     - Function Notes
 
     FIXED
     - Small Success Message Bugs
+
 </details>
 
-[comment]: <> (v0.0.4)
 <details>
 <summary>v0.0.4</summary>
     
     ADDED
     - Info Mesage
     - Note Message
 </details>
 
-[comment]: <> (v0.0.5)
 <details>
 <summary>v0.0.5</summary>
 
     ADDED
     - Title Print
 
     FIXED
     - Calling issues
+
 </details>
 
-[comment]: <> (v0.0.6)
 <details>
 <summary>v0.0.6</summary>
 
     ADDED
     - REDACTED Message
 
     REMOVED
     - Usless Classes
+
 </details>
 
-[comment]: <> (v0.0.7)
 <details>
 <summary>v0.0.7</summary>
     
     REMOVED
-    - Wait Message 
+    - Wait Message
 
     ADDED
     - Warning Message
 
     FIXED
     - imports
+
 </details>
 
-[comment]: <> (v0.0.7.1)
 <details>
 <summary>v0.0.7.1</summary>
 
     FIXED
-    - 
+    -
+
 </details>
 
-[comment]: <> (v0.0.8)
 <details>
 <summary>v0.0.8</summary>
 
     ADDED
     - Highlight Message Option!
+
 </details>
 
-[comment]: <> (v0.0.8.1)
 <details>
 <summary>v0.0.8.1</summary>
 
     FIXED
     - Leaving all functions at the bottom of the file... IM SORRY
+
 </details>
 
-[comment]: <> (v0.0.9)
 <details>
 <summary>v0.0.9</summary>
 
     FIXED
     - Optioanl Highlight!
+
 </details>
 
-[comment]: <> (v0.0.9.1)
 <details>
 <summary>v0.0.9.1</summary>
 
     FIXED
     - Info message oddly popping up after every function
+
+</details>
+
+<details>
+<summary>v0.1.0</summary>
+
+    ADDED
+    - Colored text option
+    - Custom Message
+    - Show all colors function
+
+</details>
+
+<details>
+<summary>v0.1.1</summary>
+
+    ADDED
+    - Highlight any color!
+    - Ability to color any part of the message!
+
+    FIXED
+    - Highlights
+
 </details>
 
 </details>
```

