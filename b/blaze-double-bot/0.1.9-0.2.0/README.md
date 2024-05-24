# Comparing `tmp/blaze_double_bot-0.1.9.tar.gz` & `tmp/blaze_double_bot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.1.9.tar", last modified: Thu May 23 23:38:12 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.2.0.tar", last modified: Fri May 24 00:49:38 2024, max compression
```

## Comparing `blaze_double_bot-0.1.9.tar` & `blaze_double_bot-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 23:38:12.217370 blaze_double_bot-0.1.9/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     3146 2024-05-23 23:38:12.217370 blaze_double_bot-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2657 2024-05-23 12:04:16.000000 blaze_double_bot-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 23:38:12.163082 blaze_double_bot-0.1.9/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.1.9/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0     9974 2024-05-23 23:36:12.000000 blaze_double_bot-0.1.9/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:38:12.215056 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3146 2024-05-23 23:38:11.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-23 23:38:12.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 23:38:11.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 23:38:11.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 23:38:11.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 23:38:12.217370 blaze_double_bot-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-23 23:37:40.000000 blaze_double_bot-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:38.965253 blaze_double_bot-0.2.0/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3146 2024-05-24 00:49:38.965253 blaze_double_bot-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2657 2024-05-23 12:04:16.000000 blaze_double_bot-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:38.911675 blaze_double_bot-0.2.0/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.0/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0     9795 2024-05-24 00:48:20.000000 blaze_double_bot-0.2.0/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:38.963465 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3146 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-24 00:49:38.000000 blaze_double_bot-0.2.0/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 00:49:38.965253 blaze_double_bot-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-24 00:48:45.000000 blaze_double_bot-0.2.0/setup.py
```

### Comparing `blaze_double_bot-0.1.9/LICENSE` & `blaze_double_bot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.9/PKG-INFO` & `blaze_double_bot-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.9
+Version: 0.2.0
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-0.1.9/README.md` & `blaze_double_bot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.9/blaze_double_bot/bot.py` & `blaze_double_bot-0.2.0/blaze_double_bot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
         print('Entering password')
         sleep(5)
         self.driver.find_element(By.CLASS_NAME, "red.submit.shared-button-custom.css-12vlaew").click()
         print('Logging in')
         sleep(5)
 
     def close_driver(self):
-        self.driver.close()  # Fecha apenas a janela do navegador
-        self.driver.quit()   # Encerra completamente o driver
+        self.driver.close()  
+        self.driver.quit()   
 
     def is_time_to_bet(self):
         timer_text = self.driver.find_element(By.ID, "roulette-timer").text.lower()
         if 'rolling in' in timer_text:
             print(timer_text)
             return True
         return False
@@ -106,24 +106,21 @@
             if 'shared-button-custom css-1apb7jj' in b.get_attribute('class'):
                 actions = ActionChains(self.driver)
                 sleep(1)
                 actions.click(b).perform()
                 break
 
     def print_bet(self, color):
-        print(f'''
-{datetime.now().strftime("%m/%d/%Y %H:%M")}
-Bet on {"Red" if color == "red" else "Black"}
-Completed
+        print(f'''Bet on {"Red" if color == "red" else "Black"}
+Completed {datetime.now().strftime("%m/%d/%Y %H:%M")}
 Waiting for result ...
-
 ''')
 
     def print_bet_result(self, history, color):
-        print("Win" if history[-1] == self.color_dict[color] else "Loss")
+        print(f"Win -> {history}" if history[-1] == self.color_dict[color] else f"Loss -> {history}")
 
     def get_balance(self):
         return float(self.driver.find_element(By.CLASS_NAME, 'amount').text.replace(',', '.').split(' ')[-1])
 
     def strategy(self, history):
         for color, sequences in self.strategies.items():
             for sequence in sequences:
@@ -194,51 +191,47 @@
             strategy_size = self.get_strategy_size()
             while True:
                 if self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
                     if self.wait_for_next_round():
                         history = self.get_history_api(strategy_size)
                         color = self.strategy(history)
                         if color:
-                            
-                            print(history)
+                            print('Betting strategy -> ',history)
                             print()
                             self.choose_color(color)
                             self.place_bet(self.bet_amount)
                             self.print_bet(color)
                             self.wait_for_next_round()
                             sleep(1)
                             history = self.get_history_api(strategy_size)
                             self.current_balance = self.get_balance()
                             if history[-1] != self.color_dict[color] and self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
-                                print('Gale 1')
-                                print(history)
+                                print('Gale 1 -> ',history)
                                 self.place_bet(2 * self.bet_amount)
                                 self.wait_for_next_round()
                                 sleep(1)
                                 history = self.get_history_api(strategy_size)
                                 self.current_balance = self.get_balance()
                                 if history[-1] != self.color_dict[color] and self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
-                                    print('Gale 2')
-                                    print(history)
+                                    print('Gale 2 -> ',history)
                                     self.place_bet(4 * self.bet_amount)
                                     self.wait_for_next_round()
                                     sleep(1)
                                     history = self.get_history_api(strategy_size)
                             self.print_bet_result(history, color)
-                            print(history)
                             sleep(8)
                             self.current_balance = self.get_balance()
                             print('Balance: $ ',self.current_balance)
                             print(datetime.now().strftime("%m/%d/%Y %H:%M"))
                             if self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
-                                print('Waiting 150 seconds(5 rounds) to restart analysis ...')
+                                print('Waiting 150 seconds(5 rounds) to restart analysis ...\n')
                                 sleep(150)
                                 print(50*'*')
-                                print('Analyzes restarted!\n')
-                                print(datetime.now().strftime("%m/%d/%Y %H:%M"))
+                                print('Analyzes restarted! -> ',datetime.now().strftime("%m/%d/%Y %H:%M"))
+                    
                             
                 else:
                     self.print_final_text()
                     self.close_driver()
                     break
```

### Comparing `blaze_double_bot-0.1.9/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.2.0/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.9
+Version: 0.2.0
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-0.1.9/setup.py` & `blaze_double_bot-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
           readme =f.read()
 
 setup(
     name='blaze_double_bot',
     licence='MIT License',
-    version='0.1.9',
+    version='0.2.0',
     author='ror74559',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='ror74559@gmail.com',
     keywords='blaze double bot',
     description='This Python library automates the betting process on the Blaze Double',
     packages=['blaze_double_bot'],
```

