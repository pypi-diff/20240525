# Comparing `tmp/blaze_double_bot-0.2.0.tar.gz` & `tmp/blaze_double_bot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.2.0.tar", last modified: Fri May 24 00:49:38 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.2.1.tar", last modified: Fri May 24 23:47:18 2024, max compression
```

## Comparing `blaze_double_bot-0.2.0.tar` & `blaze_double_bot-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 00:49:38.965253 blaze_double_bot-0.2.0/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3146 2024-05-24 00:49:38.965253 blaze_double_bot-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2657 2024-05-23 12:04:16.000000 blaze_double_bot-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 00:49:38.911675 blaze_double_bot-0.2.0/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.0/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0     9795 2024-05-24 00:48:20.000000 blaze_double_bot-0.2.0/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-24 00:49:38.963465 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3146 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 00:49:38.965253 blaze_double_bot-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-24 00:48:45.000000 blaze_double_bot-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 23:47:18.951246 blaze_double_bot-0.2.1/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3272 2024-05-24 23:47:18.948625 blaze_double_bot-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2781 2024-05-24 23:44:12.000000 blaze_double_bot-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 23:47:18.927459 blaze_double_bot-0.2.1/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.1/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0     9929 2024-05-24 23:41:07.000000 blaze_double_bot-0.2.1/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-24 23:47:18.948625 blaze_double_bot-0.2.1/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3272 2024-05-24 23:47:18.000000 blaze_double_bot-0.2.1/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-24 23:47:18.000000 blaze_double_bot-0.2.1/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 23:47:18.000000 blaze_double_bot-0.2.1/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 23:47:18.000000 blaze_double_bot-0.2.1/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-24 23:47:18.000000 blaze_double_bot-0.2.1/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 23:47:18.951246 blaze_double_bot-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-24 23:44:59.000000 blaze_double_bot-0.2.1/setup.py
```

### Comparing `blaze_double_bot-0.2.0/LICENSE` & `blaze_double_bot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.2.0/PKG-INFO` & `blaze_double_bot-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.0
+Version: 0.2.1
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,17 +36,18 @@
 
 1. **Create a `config.json` file** with the following content:
 
 ```json
 {
     "username": "your blaze username",
     "password": "your blaze password",
-    "bet_amount":,
-    "stop_loss_ratio": ,
-    "stop_win_ratio":,
+    "bet_amount":0.1,
+    "stop_loss_ratio":0.9,
+    "stop_win_ratio":1.1,
+    "wait_after_bet":150,
     "strategies": {
         "red": [
             ["B", "R", "B", "R", "B"],
             ["B", "B", "B", "B", "B"]
         ],
         "black": [
             ["R", "B", "R", "B", "R"],
@@ -58,14 +59,15 @@
 ```
 
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
+- **wait_after_bet**: Waiting time, in seconds, to restart analyzes after the bet result.
 - **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
 
 from blaze_double_bot import BlazeDoubleBot
```

### Comparing `blaze_double_bot-0.2.0/README.md` & `blaze_double_bot-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 
 1. **Create a `config.json` file** with the following content:
 
 ```json
 {
     "username": "your blaze username",
     "password": "your blaze password",
-    "bet_amount":,
-    "stop_loss_ratio": ,
-    "stop_win_ratio":,
+    "bet_amount":0.1,
+    "stop_loss_ratio":0.9,
+    "stop_win_ratio":1.1,
+    "wait_after_bet":150,
     "strategies": {
         "red": [
             ["B", "R", "B", "R", "B"],
             ["B", "B", "B", "B", "B"]
         ],
         "black": [
             ["R", "B", "R", "B", "R"],
@@ -44,14 +45,15 @@
 ```
 
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
+- **wait_after_bet**: Waiting time, in seconds, to restart analyzes after the bet result.
 - **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
 
 from blaze_double_bot import BlazeDoubleBot
```

### Comparing `blaze_double_bot-0.2.0/blaze_double_bot/bot.py` & `blaze_double_bot-0.2.1/blaze_double_bot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class BlazeDoubleBot:
     def __init__(self, config):
         self.username = config['username']
         self.password = config['password']
         self.bet_amount = config['bet_amount']
         self.stop_loss_ratio = config['stop_loss_ratio']
         self.stop_win_ratio = config['stop_win_ratio']
+        self.wait_after_bet = config['wait_after_bet']
         self.strategies = config['strategies']
 
         self.color_dict = {'black': 'B', 'red': 'R', 'white': 'W'}
         print('Initializing the robot ...')
         chrome_options = Options()
         chrome_options.add_argument("--headless=new")
         self.driver = uc.Chrome(options=chrome_options)
@@ -201,34 +202,34 @@
                             self.place_bet(self.bet_amount)
                             self.print_bet(color)
                             self.wait_for_next_round()
                             sleep(1)
                             history = self.get_history_api(strategy_size)
                             self.current_balance = self.get_balance()
                             if history[-1] != self.color_dict[color] and self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
-                                print('Gale 1 -> ',history)
+                                print('Gale 1 -> ',history,f'$ {2 * self.bet_amount}')
                                 self.place_bet(2 * self.bet_amount)
                                 self.wait_for_next_round()
                                 sleep(1)
                                 history = self.get_history_api(strategy_size)
                                 self.current_balance = self.get_balance()
                                 if history[-1] != self.color_dict[color] and self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
-                                    print('Gale 2 -> ',history)
+                                    print('Gale 2 -> ',history,f'$ {4 * self.bet_amount}')
                                     self.place_bet(4 * self.bet_amount)
                                     self.wait_for_next_round()
                                     sleep(1)
                                     history = self.get_history_api(strategy_size)
                             self.print_bet_result(history, color)
                             sleep(8)
                             self.current_balance = self.get_balance()
                             print('Balance: $ ',self.current_balance)
                             print(datetime.now().strftime("%m/%d/%Y %H:%M"))
                             if self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
-                                print('Waiting 150 seconds(5 rounds) to restart analysis ...\n')
-                                sleep(150)
+                                print(f'Waiting {self.wait_after_bet} seconds to restart analysis ...\n')
+                                sleep(self.wait_after_bet)
                                 print(50*'*')
                                 print('Analyzes restarted! -> ',datetime.now().strftime("%m/%d/%Y %H:%M"))
                     
                             
                 else:
                     self.print_final_text()
                     self.close_driver()
```

### Comparing `blaze_double_bot-0.2.0/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.2.1/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.0
+Version: 0.2.1
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,17 +36,18 @@
 
 1. **Create a `config.json` file** with the following content:
 
 ```json
 {
     "username": "your blaze username",
     "password": "your blaze password",
-    "bet_amount":,
-    "stop_loss_ratio": ,
-    "stop_win_ratio":,
+    "bet_amount":0.1,
+    "stop_loss_ratio":0.9,
+    "stop_win_ratio":1.1,
+    "wait_after_bet":150,
     "strategies": {
         "red": [
             ["B", "R", "B", "R", "B"],
             ["B", "B", "B", "B", "B"]
         ],
         "black": [
             ["R", "B", "R", "B", "R"],
@@ -58,14 +59,15 @@
 ```
 
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
+- **wait_after_bet**: Waiting time, in seconds, to restart analyzes after the bet result.
 - **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
 
 from blaze_double_bot import BlazeDoubleBot
```

