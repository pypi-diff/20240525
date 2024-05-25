# Comparing `tmp/sopel_twitter-1.3.7.tar.gz` & `tmp/sopel_twitter-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_twitter-1.3.7.tar", last modified: Thu Apr 25 21:51:05 2024, max compression
+gzip compressed data, was "sopel_twitter-1.3.8.tar", last modified: Sat May 25 02:36:45 2024, max compression
```

## Comparing `sopel_twitter-1.3.7.tar` & `sopel_twitter-1.3.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:51:05.820076 sopel_twitter-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-25 21:51:00.000000 sopel_twitter-1.3.7/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-25 21:51:00.000000 sopel_twitter-1.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-25 21:51:00.000000 sopel_twitter-1.3.7/NEWS
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-25 21:51:05.820076 sopel_twitter-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-25 21:51:00.000000 sopel_twitter-1.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-25 21:51:00.000000 sopel_twitter-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:51:05.820076 sopel_twitter-1.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:51:05.816076 sopel_twitter-1.3.7/sopel_twitter/
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-25 21:51:00.000000 sopel_twitter-1.3.7/sopel_twitter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:51:05.820076 sopel_twitter-1.3.7/sopel_twitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-25 21:51:05.000000 sopel_twitter-1.3.7/sopel_twitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-25 21:51:05.000000 sopel_twitter-1.3.7/sopel_twitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:51:05.000000 sopel_twitter-1.3.7/sopel_twitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 21:51:05.000000 sopel_twitter-1.3.7/sopel_twitter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 21:51:05.000000 sopel_twitter-1.3.7/sopel_twitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 21:51:05.000000 sopel_twitter-1.3.7/sopel_twitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:36:45.256705 sopel_twitter-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-25 02:36:41.000000 sopel_twitter-1.3.8/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-25 02:36:41.000000 sopel_twitter-1.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-25 02:36:41.000000 sopel_twitter-1.3.8/NEWS
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-25 02:36:45.256705 sopel_twitter-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-25 02:36:41.000000 sopel_twitter-1.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-25 02:36:41.000000 sopel_twitter-1.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 02:36:45.256705 sopel_twitter-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:36:45.256705 sopel_twitter-1.3.8/sopel_twitter/
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-05-25 02:36:41.000000 sopel_twitter-1.3.8/sopel_twitter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:36:45.256705 sopel_twitter-1.3.8/sopel_twitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-25 02:36:45.000000 sopel_twitter-1.3.8/sopel_twitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-25 02:36:45.000000 sopel_twitter-1.3.8/sopel_twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:36:45.000000 sopel_twitter-1.3.8/sopel_twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 02:36:45.000000 sopel_twitter-1.3.8/sopel_twitter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 02:36:45.000000 sopel_twitter-1.3.8/sopel_twitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-25 02:36:45.000000 sopel_twitter-1.3.8/sopel_twitter.egg-info/top_level.txt
```

### Comparing `sopel_twitter-1.3.7/COPYING` & `sopel_twitter-1.3.8/COPYING`

 * *Files identical despite different names*

### Comparing `sopel_twitter-1.3.7/NEWS` & `sopel_twitter-1.3.8/NEWS`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Changes between 1.3.7 and 1.3.8
+===============================
+
+Added:
+* Handle more exception types when fetching tweets (#66)
+
+Changed:
+* Upgrade minimum `tweety-ns` version to 1.1.4 (#65)
+* Check public session state property instead of internal value (#65)
+
+
 Changes between 1.3.6 and 1.3.7
 ===============================
 
 Added:
 * Gracefully truncate long tweet text (#61)
 
 Changed:
```

### Comparing `sopel_twitter-1.3.7/PKG-INFO` & `sopel_twitter-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.3.7
+Version: 1.3.8
 Summary: A Twitter plugin for Sopel
 Author-email: dgw <dgw@technobabbl.es>
 License: EFL-2.0
 Project-URL: Homepage, https://github.com/sopel-irc/sopel-twitter
 Project-URL: Bug Tracker, https://github.com/sopel-irc/sopel-twitter/issues
 Keywords: sopel,plugin,bot,irc
 Platform: Linux x86, x86-64
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Eiffel Forum License (EFL)
 Classifier: License :: OSI Approved :: Eiffel Forum License
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: sopel<9,>=7.1
-Requires-Dist: tweety-ns~=1.1.2
+Requires-Dist: tweety-ns~=1.1.4
 
 # sopel-twitter
 
 A Twitter plugin for [Sopel](https://sopel.chat/).
 
 ## Installation
 
@@ -105,14 +105,25 @@
 ```irc
 < Wiz> .twitinfo NASA
 < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
          | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
          | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
 ```
 
+Changes between 1.3.7 and 1.3.8
+===============================
+
+Added:
+* Handle more exception types when fetching tweets (#66)
+
+Changed:
+* Upgrade minimum `tweety-ns` version to 1.1.4 (#65)
+* Check public session state property instead of internal value (#65)
+
+
 Changes between 1.3.6 and 1.3.7
 ===============================
 
 Added:
 * Gracefully truncate long tweet text (#61)
 
 Changed:
```

### Comparing `sopel_twitter-1.3.7/README.md` & `sopel_twitter-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `sopel_twitter-1.3.7/pyproject.toml` & `sopel_twitter-1.3.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 namespaces = false
 
 [tool.setuptools.dynamic]
 readme = { file=["README.md", "NEWS"], content-type="text/markdown" }
 
 [project]
 name = "sopel-twitter"
-version = "1.3.7"
+version = "1.3.8"
 description = "A Twitter plugin for Sopel"
 
 authors = [
   { name="dgw", email="dgw@technobabbl.es" },
 ]
 
 license = { text="EFL-2.0" }
@@ -38,15 +38,15 @@
   "irc",
 ]
 
 # Python spec should be enabled along with bumping `sopel` to 8+
 # requires-python = ">=3.8, <4"
 dependencies = [
     "sopel>=7.1,<9",
-    "tweety-ns~=1.1.2",
+    "tweety-ns~=1.1.4",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sopel-irc/sopel-twitter"
 "Bug Tracker" = "https://github.com/sopel-irc/sopel-twitter/issues"
 
 [project.entry-points."sopel.plugins"]
```

### Comparing `sopel_twitter-1.3.7/sopel_twitter/__init__.py` & `sopel_twitter-1.3.8/sopel_twitter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
 def output_status(bot, trigger, id_):
     try:
         app = Twitter(_get_tweety_session_name(bot))
         # try to use saved session
         app.connect()
 
-        if not app.session.logged_in:
+        if not app.is_user_authorized:
             # existing session not present
             app.sign_in(bot.settings.twitter.username, bot.settings.twitter.password)
 
         tweet = app.tweet_detail(id_)
     except tweety_errors.DeniedLogin:
         bot.say("Twitter wouldn't let me log in. Please try again later. If this issue persists, contact my owner.")
         return
@@ -232,14 +232,20 @@
         return
     except tweety_errors.InvalidCredentials:
         bot.say("Can't authenticate with Twitter. Please ask my owner to check my credentials.")
         return
     except tweety_errors.AuthenticationRequired:
         bot.say("That content requires authentication; sorry!")
         return
+    except tweety_errors.UserProtected:
+        bot.say("User profile is protected.")
+        return
+    except tweety_errors.ProtectedTweet:
+        bot.say("Tweet is protected.")
+        return
     except tweety_errors.RateLimitReached:
         bot.say("Rate limit reached. Please try again later.")
         return
     except tweety_errors.InvalidTweetIdentifier:
         bot.say("Couldn't fetch that tweet. It's probably private, 18+ flagged, or deleted.")
         return
     except (
@@ -282,15 +288,15 @@
 
 def output_user(bot, trigger, sn):
     try:
         app = Twitter(_get_tweety_session_name(bot))
         # try to use saved session
         app.connect()
 
-        if not app.session.logged_in:
+        if not app.is_user_authorized:
             # existing session not present
             app.sign_in(bot.settings.twitter.username, bot.settings.twitter.password)
 
         user = app.get_user_info(sn)
     except tweety_errors.DeniedLogin:
         bot.say("Twitter wouldn't let me log in. Please try again later. If this issue persists, contact my owner.")
         return
```

### Comparing `sopel_twitter-1.3.7/sopel_twitter.egg-info/PKG-INFO` & `sopel_twitter-1.3.8/sopel_twitter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.3.7
+Version: 1.3.8
 Summary: A Twitter plugin for Sopel
 Author-email: dgw <dgw@technobabbl.es>
 License: EFL-2.0
 Project-URL: Homepage, https://github.com/sopel-irc/sopel-twitter
 Project-URL: Bug Tracker, https://github.com/sopel-irc/sopel-twitter/issues
 Keywords: sopel,plugin,bot,irc
 Platform: Linux x86, x86-64
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Eiffel Forum License (EFL)
 Classifier: License :: OSI Approved :: Eiffel Forum License
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: sopel<9,>=7.1
-Requires-Dist: tweety-ns~=1.1.2
+Requires-Dist: tweety-ns~=1.1.4
 
 # sopel-twitter
 
 A Twitter plugin for [Sopel](https://sopel.chat/).
 
 ## Installation
 
@@ -105,14 +105,25 @@
 ```irc
 < Wiz> .twitinfo NASA
 < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
          | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
          | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
 ```
 
+Changes between 1.3.7 and 1.3.8
+===============================
+
+Added:
+* Handle more exception types when fetching tweets (#66)
+
+Changed:
+* Upgrade minimum `tweety-ns` version to 1.1.4 (#65)
+* Check public session state property instead of internal value (#65)
+
+
 Changes between 1.3.6 and 1.3.7
 ===============================
 
 Added:
 * Gracefully truncate long tweet text (#61)
 
 Changed:
```

