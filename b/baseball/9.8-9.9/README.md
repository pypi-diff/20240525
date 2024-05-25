# Comparing `tmp/baseball-9.8.tar.gz` & `tmp/baseball-9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baseball-9.8.tar", last modified: Tue Apr 13 02:22:12 2021, max compression
+gzip compressed data, was "dist/baseball-9.9.tar", last modified: Tue Apr 13 03:46:25 2021, max compression
```

## Comparing `baseball-9.8.tar` & `baseball-9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 bcrom     (1000) bcrom     (1000)        0 2021-04-13 02:22:12.148294 baseball-9.8/
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)      309 2021-04-13 02:22:12.148294 baseball-9.8/PKG-INFO
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)    16970 2021-04-13 01:58:17.000000 baseball-9.8/README.md
-drwxrwxr-x   0 bcrom     (1000) bcrom     (1000)        0 2021-04-13 02:22:12.144294 baseball-9.8/baseball/
--rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)     1135 2021-04-12 23:03:46.000000 baseball-9.8/baseball/__init__.py
--rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    33998 2021-04-13 01:43:07.000000 baseball-9.8/baseball/baseball.py
--rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)     5950 2021-04-11 19:09:09.000000 baseball-9.8/baseball/baseball_events.py
--rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    37292 2021-04-13 02:21:48.000000 baseball-9.8/baseball/fetch_game.py
--rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    84897 2021-04-13 00:58:15.000000 baseball-9.8/baseball/generate_svg.py
--rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    19096 2021-04-11 19:17:02.000000 baseball-9.8/baseball/process_game_json.py
--rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    35668 2021-04-11 18:47:46.000000 baseball-9.8/baseball/process_game_xml.py
--rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    31264 2021-04-10 17:55:45.000000 baseball-9.8/baseball/stats.py
-drwxrwxr-x   0 bcrom     (1000) bcrom     (1000)        0 2021-04-13 02:22:12.148294 baseball-9.8/baseball.egg-info/
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)      309 2021-04-13 02:22:12.000000 baseball-9.8/baseball.egg-info/PKG-INFO
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)      403 2021-04-13 02:22:12.000000 baseball-9.8/baseball.egg-info/SOURCES.txt
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)        1 2021-04-13 02:22:12.000000 baseball-9.8/baseball.egg-info/dependency_links.txt
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)        1 2021-04-13 02:22:12.000000 baseball-9.8/baseball.egg-info/not-zip-safe
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)       30 2021-04-13 02:22:12.000000 baseball-9.8/baseball.egg-info/requires.txt
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)        9 2021-04-13 02:22:12.000000 baseball-9.8/baseball.egg-info/top_level.txt
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)       38 2021-04-13 02:22:12.148294 baseball-9.8/setup.cfg
--rw-rw-r--   0 bcrom     (1000) bcrom     (1000)      480 2021-04-13 02:22:01.000000 baseball-9.8/setup.py
+drwxrwxr-x   0 bcrom     (1000) bcrom     (1000)        0 2021-04-13 03:46:25.511778 baseball-9.9/
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)      309 2021-04-13 03:46:25.511778 baseball-9.9/PKG-INFO
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)    16970 2021-04-13 01:58:17.000000 baseball-9.9/README.md
+drwxrwxr-x   0 bcrom     (1000) bcrom     (1000)        0 2021-04-13 03:46:25.507778 baseball-9.9/baseball/
+-rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)     1135 2021-04-12 23:03:46.000000 baseball-9.9/baseball/__init__.py
+-rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    33998 2021-04-13 01:43:07.000000 baseball-9.9/baseball/baseball.py
+-rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)     5950 2021-04-11 19:09:09.000000 baseball-9.9/baseball/baseball_events.py
+-rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    37584 2021-04-13 03:45:47.000000 baseball-9.9/baseball/fetch_game.py
+-rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    84897 2021-04-13 00:58:15.000000 baseball-9.9/baseball/generate_svg.py
+-rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    19265 2021-04-13 03:29:58.000000 baseball-9.9/baseball/process_game_json.py
+-rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    35668 2021-04-11 18:47:46.000000 baseball-9.9/baseball/process_game_xml.py
+-rwxrwxr-x   0 bcrom     (1000) bcrom     (1000)    31264 2021-04-10 17:55:45.000000 baseball-9.9/baseball/stats.py
+drwxrwxr-x   0 bcrom     (1000) bcrom     (1000)        0 2021-04-13 03:46:25.507778 baseball-9.9/baseball.egg-info/
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)      309 2021-04-13 03:46:25.000000 baseball-9.9/baseball.egg-info/PKG-INFO
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)      403 2021-04-13 03:46:25.000000 baseball-9.9/baseball.egg-info/SOURCES.txt
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)        1 2021-04-13 03:46:25.000000 baseball-9.9/baseball.egg-info/dependency_links.txt
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)        1 2021-04-13 03:46:25.000000 baseball-9.9/baseball.egg-info/not-zip-safe
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)       30 2021-04-13 03:46:25.000000 baseball-9.9/baseball.egg-info/requires.txt
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)        9 2021-04-13 03:46:25.000000 baseball-9.9/baseball.egg-info/top_level.txt
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)       38 2021-04-13 03:46:25.511778 baseball-9.9/setup.cfg
+-rw-rw-r--   0 bcrom     (1000) bcrom     (1000)      480 2021-04-13 03:46:21.000000 baseball-9.9/setup.py
```

### Comparing `baseball-9.8/README.md` & `baseball-9.9/README.md`

 * *Files identical despite different names*

### Comparing `baseball-9.8/baseball/__init__.py` & `baseball-9.9/baseball/__init__.py`

 * *Files identical despite different names*

### Comparing `baseball-9.8/baseball/baseball.py` & `baseball-9.9/baseball/baseball.py`

 * *Files identical despite different names*

### Comparing `baseball-9.8/baseball/baseball_events.py` & `baseball-9.9/baseball/baseball_events.py`

 * *Files identical despite different names*

### Comparing `baseball-9.8/baseball/fetch_game.py` & `baseball-9.9/baseball/fetch_game.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,27 +413,34 @@
 
 def get_object_html_str(game_html_id_tuple_list):
     object_html_str = ''
     for i, (game_html_id, game) in enumerate(game_html_id_tuple_list):
         start_datetime = (game.start_datetime if game.start_datetime
                           else game.expected_start_datetime)
 
-        start_datetime_str = start_datetime.astimezone(
-            timezone(game.timezone_str)
-        ).strftime('%-I:%M %p %Z')
 
         game_id_element_list = game_html_id.split('-')
-        title_str = '{} @ {} <br />{}'.format(
-            game.away_team.name,
-            game.home_team.name,
-            start_datetime_str
-        )
+        title_str = '{} @ {}<br />'.format(game.away_team.name,
+                                           game.home_team.name)
 
-        if game_id_element_list[5] != '1':
-            title_str += ' (Game {})'.format(game_id_element_list[5])
+        if game_id_element_list[5] == '0':
+            title_str += 'Postponed'
+        elif game_id_element_list[5] != '1':
+            title_str += '{} (Game {})'.format(
+                start_datetime.astimezone(
+                    timezone(game.timezone_str)
+                ).strftime('%-I:%M %p %Z'),
+                game_id_element_list[5]
+            )
+        else:
+            title_str += '{}'.format(
+                start_datetime.astimezone(
+                    timezone(game.timezone_str)
+                ).strftime('%-I:%M %p %Z')
+            )
 
         if i % 2 == 0:
             object_html_str += '<tr>'
 
         object_html_str += OBJECT_ENTRY_TEMPLATE.format(
             title_str=title_str,
             game_id_str=game_html_id
```

### Comparing `baseball-9.8/baseball/generate_svg.py` & `baseball-9.9/baseball/generate_svg.py`

 * *Files identical despite different names*

### Comparing `baseball-9.8/baseball/process_game_json.py` & `baseball-9.9/baseball/process_game_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,8 +505,12 @@
         game.away_team.batting_order_list_list = [[]] * 9
 
     game.set_batting_box_score_dict()
     game.set_pitching_box_score_dict()
     game.set_team_stats()
     game.set_gametimes()
 
+    if 'Postponed' in game_dict.get(
+            'gameData', {}).get('status', {}).get('detailedState', {}):
+        game.game_date_str = game.game_date_str[:-1] + '0'
+
     return game
```

### Comparing `baseball-9.8/baseball/process_game_xml.py` & `baseball-9.9/baseball/process_game_xml.py`

 * *Files identical despite different names*

### Comparing `baseball-9.8/baseball/stats.py` & `baseball-9.9/baseball/stats.py`

 * *Files identical despite different names*

