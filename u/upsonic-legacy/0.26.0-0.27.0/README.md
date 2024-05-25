# Comparing `tmp/upsonic_legacy-0.26.0.tar.gz` & `tmp/upsonic_legacy-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsonic_legacy-0.26.0.tar", last modified: Wed May 22 15:39:02 2024, max compression
+gzip compressed data, was "upsonic_legacy-0.27.0.tar", last modified: Sat May 25 12:59:29 2024, max compression
```

## Comparing `upsonic_legacy-0.26.0.tar` & `upsonic_legacy-0.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/upsonic/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/upsonic/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25476 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/upsonic/remote/localimport/
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/localimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17647 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/ollama_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    52869 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/on_prem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:59:29.624613 upsonic_legacy-0.27.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-25 12:59:29.624613 upsonic_legacy-0.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:59:29.624613 upsonic_legacy-0.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:59:29.620613 upsonic_legacy-0.27.0/upsonic/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/upsonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:59:29.624613 upsonic_legacy-0.27.0/upsonic/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/upsonic/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25476 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/upsonic/remote/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/upsonic/remote/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/upsonic/remote/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:59:29.624613 upsonic_legacy-0.27.0/upsonic/remote/localimport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/upsonic/remote/localimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17647 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/upsonic/remote/ollama_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54817 2024-05-25 12:59:17.000000 upsonic_legacy-0.27.0/upsonic/remote/on_prem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:59:29.624613 upsonic_legacy-0.27.0/upsonic_legacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-25 12:59:29.000000 upsonic_legacy-0.27.0/upsonic_legacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-25 12:59:29.000000 upsonic_legacy-0.27.0/upsonic_legacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:59:29.000000 upsonic_legacy-0.27.0/upsonic_legacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 12:59:29.000000 upsonic_legacy-0.27.0/upsonic_legacy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:59:29.000000 upsonic_legacy-0.27.0/upsonic_legacy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-25 12:59:29.000000 upsonic_legacy-0.27.0/upsonic_legacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 12:59:29.000000 upsonic_legacy-0.27.0/upsonic_legacy.egg-info/top_level.txt
```

### Comparing `upsonic_legacy-0.26.0/LICENSE` & `upsonic_legacy-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.26.0/PKG-INFO` & `upsonic_legacy-0.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic_legacy
-Version: 0.26.0
+Version: 0.27.0
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | Self-Driven Autonomous Python Libraries
         
@@ -52,16 +52,16 @@
         
         
         ## Usage
         
         Here's an updated quickstart guide to get you up and running with your container:
         
         ```python
-        from upsonic import Upsonic_On_Prem
-        upsonic = Upsonic_On_Prem('https://your-server-address:5000', 'ACK_****************')
+        from upsonic import UpsonicOnPrem
+        upsonic = UpsonicOnPrem('https://your-server-address:5000', 'ACK_****************')
         
         
         
         def sum(a, b):
             return a + b
         
         upsonic.dump("math.basics.sum", sum)
```

### Comparing `upsonic_legacy-0.26.0/README.md` & `upsonic_legacy-0.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
 
 ## Usage
 
 Here's an updated quickstart guide to get you up and running with your container:
 
 ```python
-from upsonic import Upsonic_On_Prem
-upsonic = Upsonic_On_Prem('https://your-server-address:5000', 'ACK_****************')
+from upsonic import UpsonicOnPrem
+upsonic = UpsonicOnPrem('https://your-server-address:5000', 'ACK_****************')
 
 
 
 def sum(a, b):
     return a + b
 
 upsonic.dump("math.basics.sum", sum)
```

### Comparing `upsonic_legacy-0.26.0/setup.py` & `upsonic_legacy-0.27.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="upsonic_legacy",
-    version="0.26.0",
+    version="0.27.0",
     description="""Magic Cloud Layer""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/Upsonic/Upsonic",
     author="Upsonic",
     author_email="onur.atakan.ulusoy@upsonic.co",
     license="MIT",
```

### Comparing `upsonic_legacy-0.26.0/upsonic/__init__.py` & `upsonic_legacy-0.27.0/upsonic/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from .core import Upsonic_Serial
 
 except:
     pass
 
 from .remote import localimport
 
-from .remote import Upsonic_On_Prem, Tiger, Tiger_Admin
+from .remote import Upsonic_On_Prem, Tiger, Tiger_Admin, UpsonicOnPrem
 from .remote import Upsonic_Cloud_Free
 from .remote import Upsonic_Cloud_Pro
 from .remote import Upsonic_Cloud_Premium
 from .remote import Upsonic_Cloud_Startup
 from .remote import Upsonic_Cloud_Readonly
 from .remote import Upsonic_Cloud_Generic
 from .remote import no_exception
@@ -24,12 +24,12 @@
 from .remote import decrypt
 from .remote import upsonic_serializer
 from .remote import interface
 
 
 open_databases = {}
 
-__version__ = '0.26.0'
+__version__ = '0.27.0'
```

### Comparing `upsonic_legacy-0.26.0/upsonic/remote/__init__.py` & `upsonic_legacy-0.27.0/upsonic/remote/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from .on_prem import Upsonic_On_Prem, Tiger, Tiger_Admin
+from .on_prem import Upsonic_On_Prem, Tiger, Tiger_Admin, UpsonicOnPrem
 from .interface import Upsonic_Cloud_Free
 from .interface import Upsonic_Cloud_Pro
 from .interface import Upsonic_Cloud_Premium
 from .interface import Upsonic_Cloud_Startup
 from .interface import Upsonic_Cloud_Readonly
 from .interface import Upsonic_Cloud_Generic
 from .helper import no_exception
```

### Comparing `upsonic_legacy-0.26.0/upsonic/remote/controller.py` & `upsonic_legacy-0.27.0/upsonic/remote/controller.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.26.0/upsonic/remote/helper.py` & `upsonic_legacy-0.27.0/upsonic/remote/helper.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.26.0/upsonic/remote/interface.py` & `upsonic_legacy-0.27.0/upsonic/remote/interface.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.26.0/upsonic/remote/localimport/__init__.py` & `upsonic_legacy-0.27.0/upsonic/remote/localimport/__init__.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.26.0/upsonic/remote/ollama_langchain.py` & `upsonic_legacy-0.27.0/upsonic/remote/ollama_langchain.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.26.0/upsonic/remote/on_prem.py` & `upsonic_legacy-0.27.0/upsonic/remote/on_prem.py`

 * *Files 3% similar despite different names*

```diff
@@ -693,34 +693,28 @@
             if the_lock and the_lock != [None]:
                 self._log("This scope is locked now! Someone dumping.")
                 return False
         except:
             pass
 
 
+
+
         the_type = type(value).__name__
         if the_type == "type":
             the_type = "class"
 
         encryption_key = "u"
 
-        data = {
-            "scope": key,
-            "code": textwrap.dedent(self.extract_source(value)),
-        }
-
-        self._send_request("POST", "/dump_code", data)
+        the_code = textwrap.dedent(self.extract_source(value))
 
 
 
 
 
-        data = {"scope": key, "type": the_type}
-
-        self._send_request("POST", "/dump_type", data)
 
 
         the_requirements = Upsonic_On_Prem.export_requirement()
         the_original_requirements = ""
         if self.tester:
             self._log(f"The first original requirements {the_original_requirements}")
         elements = []
@@ -753,29 +747,19 @@
                 self._log(f"Error on extract_needed_libraries while dumping {key}")
                 traceback.print_exc()
 
 
 
         if self.tester:
             self._log(f"the_original_requirements {the_original_requirements}")
-        data = {
-            "scope": key,
-            "requirements": the_original_requirements,
-        }
-
-        self._send_request("POST", "/dump_requirements", data)
 
 
+        the_version = f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
 
-        data = {
-            "scope": key,
-            "python_version": f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}",
-        }
 
-        self._send_request("POST", "/dump_python_version", data)
 
         fernet_key = base64.urlsafe_b64encode(hashlib.sha256(encryption_key.encode()).digest())
         fernet = Fernet(fernet_key)
 
 
         engine_reports_exceptions = []
         the_engine_reports = {}
@@ -805,36 +789,44 @@
         try:
             the_engine_reports["extract_source"] = fernet.encrypt(pickle.dumps(extract_source(value, self.tester), protocol=1))
         except:
             if self.tester:
                 self._log(f"Error on extract_source while dumping {key}")
                 traceback.print_exc()
 
+
+
         if extracted_needed_libraries != None:
             the_engine_reports["extract_needed_libraries"] = fernet.encrypt(pickle.dumps(extracted_needed_libraries, protocol=1))
 
 
         if self.tester:
             self._log(f"the_engine_reports {the_engine_reports}")
         dumped = pickle.dumps(the_engine_reports, protocol=1)
 
 
         data = {
             "scope": key,
+            "code": the_code,
+            "type": the_type,
+            "requirements": the_original_requirements,
+            "python_version": the_version,
             "data": fernet.encrypt(dumped),
             "commit_message": message
         }
 
-        response = self._send_request("POST", "/dump", data)
+        response = self._send_request("POST", "/dump_together", data)
 
         if response != [None]:
             return True
         else:
             return False
 
+
+
     def print_code(self, key, version=None):
         print(self.get(key, version=version, extract_source=True))
 
     def get(
             self,
             key,
             version=None,
@@ -1120,18 +1112,25 @@
         result = ""
         try:
             result = inspect.getsource(value)
         except:
             result = dill.source.getsource(value)
         return result
 
+    def auto_dump(self, value, ask=True, check_function=True, print_prompts=False, model=None):
+
+        
+        if model == None:
+            model = self.get_default_ai_model()
+
+        if model == "llama3-8b":
+            check_function = False
 
-    def auto_dump(self, value, ask=True, check_idea=True, print_prompts=False, model=None):
-        if check_idea:
-            check = self.check_idea(value, print_prompts=print_prompts, model=model)
+        if check_function:
+            check = self.check_function(value, print_prompts=print_prompts, model=model)
             if check != True:
                 print("Check:", check)
                 return
 
         code = textwrap.dedent(self.extract_source(value))
         all_scopes = self.get_all_scopes_user()
         all_scopes = "\n".join(all_scopes)
@@ -1146,14 +1145,17 @@
 ```
 
 Currenlty Index of Library:
 ```
 {all_scopes}
 ```
 
+Your answer should be just the suggested position. Dont say any other think.
+
+
 Suggested Position:
 
 """
 
         ai_answer = self.ai_completion(prompt, model=model)
         ai_answer = ai_answer.replace("`", "").replace("\n", "")
         ai_answer = '.'.join(ai_answer.split('.')[:-1])
@@ -1184,26 +1186,28 @@
                     break
 
         else:
             self.set(ai_answer, value)
             print("\nDumped")
 
 
+
+
     def get_code(self, scope):
         data = {"scope": scope}
         return self._send_request("POST", "/get_code_of_scope", data)
 
     def get_document(self, scope, version=None):
         data = {"scope": scope}
         if version != None:
             data["version"] = version
         return self._send_request("POST", "/get_document_of_scope", data)
 
 
-    def check_idea(self, value, print_prompts=False, model=None):
+    def check_function(self, value, print_prompts=False, model=None):
         code = textwrap.dedent(self.extract_source(value))
 
 
         all_scopes_ = self.get_all_scopes_user()
         all_scopes = ""
         for i in all_scopes_:
             all_scopes += i + "\n"
@@ -1525,13 +1529,79 @@
 
         from .ollama_langchain import Ollama
 
         llm = Ollama(model=f"{model}**{self.password}", base_url = self.api_url+'/ollama')
         return llm
 
 
+
+    def check_idea(self, idea):
+        search_result = self.search(idea)
+        if len(search_result) == 0:
+            return True
+        
+        # Get the first result of check and as ai to check the similarity
+        first_result = search_result[0]
+
+        # Get the document of the first result
+        first_result_document = self.get_document(first_result) 
+
+        # get the code of the first result
+        first_result_code = self.get_code(first_result)
+
+        # Ask to AI to check the similarity
+        prompt = f"""
+        The user planning to write a function about this: {idea}
+
+        Currently function: {first_result}
+        Currently function Document: {first_result_document}
+        Currently function Code: {first_result_code}
+
+        Is the idea making same thing with the first result (Y/N)?
+        """
+
+
+        ai_answer = self.ai_completion(prompt)
+        ai_answer = ai_answer.replace("`", "").replace("\n", "")
+        ai_answer = ai_answer.split(",")[0]
+        ai_answer = ai_answer.replace("ASSISTANT: ", "")
+
+        is_not_similar = False
+
+
+        if ai_answer == "N" or ai_answer == "NO" or ai_answer == "No":
+            is_not_similar = True
+
+        if not is_not_similar:
+            #Ask ai to explain similarity in one sentence
+            prompt = f"""
+            Current Idea: {idea}
+            First Result: {first_result}
+            First Result Document: {first_result_document}
+            First Result Code: {first_result_code}
+
+            Explain the similarity in one sentence. If you need to refer to First Result please use {first_result}.
+            """
+
+            ai_answer = self.ai_completion(prompt)
+            ai_answer = ai_answer.replace("`", "").replace("\n", "")
+            ai_answer = ai_answer.split(",")[0]
+            ai_answer = ai_answer.replace("ASSISTANT: ", "")
+
+            return "Fail: "+ ai_answer
+        else:
+            return "Pass: There is no same functionality in the library"
+
+
+
+
+class UpsonicOnPrem(Upsonic_On_Prem):
+    pass
+
+
+
 def Tiger():
     return Upsonic_On_Prem("https://api_tiger.upsonic.co", 'ACK_xmxIiqsgGySvBPPd55M0Ldm5AcR2kt6r3kmL52Ptqo', engine="upsonic_serializer", pass_python_version_check=True)
 
 
 def Tiger_Admin(api_url, access_key):
     return Upsonic_On_Prem(api_url, access_key, engine="upsonic_serializer", pass_python_version_check=True)
```

### Comparing `upsonic_legacy-0.26.0/upsonic_legacy.egg-info/PKG-INFO` & `upsonic_legacy-0.27.0/upsonic_legacy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic-legacy
-Version: 0.26.0
+Version: 0.27.0
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | Self-Driven Autonomous Python Libraries
         
@@ -52,16 +52,16 @@
         
         
         ## Usage
         
         Here's an updated quickstart guide to get you up and running with your container:
         
         ```python
-        from upsonic import Upsonic_On_Prem
-        upsonic = Upsonic_On_Prem('https://your-server-address:5000', 'ACK_****************')
+        from upsonic import UpsonicOnPrem
+        upsonic = UpsonicOnPrem('https://your-server-address:5000', 'ACK_****************')
         
         
         
         def sum(a, b):
             return a + b
         
         upsonic.dump("math.basics.sum", sum)
```

### Comparing `upsonic_legacy-0.26.0/upsonic_legacy.egg-info/SOURCES.txt` & `upsonic_legacy-0.27.0/upsonic_legacy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

