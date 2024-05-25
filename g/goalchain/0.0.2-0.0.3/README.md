# Comparing `tmp/goalchain-0.0.2.tar.gz` & `tmp/goalchain-0.0.3.tar.gz`

## Comparing `goalchain-0.0.2.tar` & `goalchain-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 goalchain-0.0.2/src/goalchain/__init__.py
--rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 goalchain-0.0.2/src/goalchain/goalchain.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 goalchain-0.0.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 goalchain-0.0.2/LICENSE
--rw-r--r--   0        0        0    13340 2020-02-02 00:00:00.000000 goalchain-0.0.2/README.md
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 goalchain-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 goalchain-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 goalchain-0.0.3/src/goalchain/__init__.py
+-rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 goalchain-0.0.3/src/goalchain/goalchain.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 goalchain-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 goalchain-0.0.3/LICENSE
+-rw-r--r--   0        0        0    13340 2020-02-02 00:00:00.000000 goalchain-0.0.3/README.md
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 goalchain-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 goalchain-0.0.3/PKG-INFO
```

### Comparing `goalchain-0.0.2/src/goalchain/goalchain.py` & `goalchain-0.0.3/src/goalchain/goalchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,14 +280,16 @@
             else:
                 return self.simulate_response(response_text)
     
     def take_over(self, messages = [], hand_over = False):
         self.completed = False
         if messages:
             self.messages = messages
+        else:
+            self.messages = []
         if hand_over:
             self.hand_over = True
         return self
     
     def connect(self, goal, user_goal, hand_over = False, keep_messages = False):
         self.connected_goals.append(
             {
```

### Comparing `goalchain-0.0.2/.gitignore` & `goalchain-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `goalchain-0.0.2/LICENSE` & `goalchain-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goalchain-0.0.2/README.md` & `goalchain-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `goalchain-0.0.2/pyproject.toml` & `goalchain-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "goalchain"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   {name="Adrian Lucas Malec", email="dr.adrian@gmail.com"},
 ]
 description = "GoalChain is a simple but effective framework for enabling goal-orientated conversation flows for human-LLM and LLM-LLM interaction."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="MIT"}
```

### Comparing `goalchain-0.0.2/PKG-INFO` & `goalchain-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: goalchain
-Version: 0.0.2
+Version: 0.0.3
 Summary: GoalChain is a simple but effective framework for enabling goal-orientated conversation flows for human-LLM and LLM-LLM interaction.
 Project-URL: Homepage, https://github.com/adlumal/GoalChain
 Project-URL: Documentation, https://github.com/adlumal/GoalChain/blob/main/README.md
 Project-URL: Issues, https://github.com/adlumal/GoalChain/issues
 Project-URL: Source, https://github.com/adlumal/GoalChain
 Author-email: Adrian Lucas Malec <dr.adrian@gmail.com>
 License: MIT
```

