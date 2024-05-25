# Comparing `tmp/pyrasp-0.6.2.tar.gz` & `tmp/pyrasp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrasp-0.6.2.tar", last modified: Sat Apr 27 12:55:33 2024, max compression
+gzip compressed data, was "pyrasp-0.7.0.tar", last modified: Sat May 25 08:31:08 2024, max compression
```

## Comparing `pyrasp-0.6.2.tar` & `pyrasp-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 12:55:33.347148 pyrasp-0.6.2/
--rw-rw-rw-   0        0        0    35823 2024-04-27 12:55:27.000000 pyrasp-0.6.2/LICENSE
--rw-rw-rw-   0        0        0    43555 2024-04-27 12:55:33.345703 pyrasp-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2024-04-27 12:55:27.000000 pyrasp-0.6.2/README.md
--rw-rw-rw-   0        0        0      777 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-27 12:55:33.328569 pyrasp-0.6.2/pyrasp/
--rw-rw-rw-   0        0        0        0 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 12:55:33.340597 pyrasp-0.6.2/pyrasp/data/
--rw-rw-rw-   0        0        0   483629 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/data/sqli_model-1.1.0
--rw-rw-rw-   0        0        0  1116155 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/data/xss_model-1.2.0
--rw-rw-rw-   0        0        0    96789 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/pyrasp.py
--rw-rw-rw-   0        0        0     6631 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/pyrasp_data.py
-drwxrwxrwx   0        0        0        0 2024-04-27 12:55:33.343144 pyrasp-0.6.2/pyrasp.egg-info/
--rw-rw-rw-   0        0        0    43555 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 12:55:33.347148 pyrasp-0.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:08.688018 pyrasp-0.7.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-25 08:31:02.000000 pyrasp-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0    43662 2024-05-25 08:31:08.686021 pyrasp-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1668 2024-05-25 08:31:02.000000 pyrasp-0.7.0/README.md
+-rw-rw-rw-   0        0        0      823 2024-05-25 08:31:02.000000 pyrasp-0.7.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:08.668275 pyrasp-0.7.0/pyrasp/
+-rw-rw-rw-   0        0        0        0 2024-05-25 08:31:02.000000 pyrasp-0.7.0/pyrasp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:08.679506 pyrasp-0.7.0/pyrasp/data/
+-rw-rw-rw-   0        0        0  1307935 2024-05-25 08:31:02.000000 pyrasp-0.7.0/pyrasp/data/sqli_model-2.0.0
+-rw-rw-rw-   0        0        0  3938017 2024-05-25 08:31:02.000000 pyrasp-0.7.0/pyrasp/data/xss_model-2.0.0
+-rw-rw-rw-   0        0        0    98436 2024-05-25 08:31:02.000000 pyrasp-0.7.0/pyrasp/pyrasp.py
+-rw-rw-rw-   0        0        0     6630 2024-05-25 08:31:02.000000 pyrasp-0.7.0/pyrasp/pyrasp_data.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:31:08.685019 pyrasp-0.7.0/pyrasp.egg-info/
+-rw-rw-rw-   0        0        0    43662 2024-05-25 08:31:08.000000 pyrasp-0.7.0/pyrasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-05-25 08:31:08.000000 pyrasp-0.7.0/pyrasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 08:31:08.000000 pyrasp-0.7.0/pyrasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-25 08:31:08.000000 pyrasp-0.7.0/pyrasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-25 08:31:08.000000 pyrasp-0.7.0/pyrasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 08:31:08.688018 pyrasp-0.7.0/setup.cfg
```

### Comparing `pyrasp-0.6.2/LICENSE` & `pyrasp-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.2/PKG-INFO` & `pyrasp-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasp
-Version: 0.6.2
+Version: 0.7.0
 Summary: Python RASP
 Author-email: Renaud Bidou <renaud@paracyberbellum.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,16 +674,17 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/rbidou/pyrasp
+Project-URL: Homepage, https://pyrasp.paracyberbellum.io
 Project-URL: Documentation, https://paracyberbellum.gitbook.io/pyrasp
+Project-URL: GitHub, https://github.com/rbidou/pyrasp
 Keywords: rasp,web application,security,xss,sql injection,waf,dlp
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Flask
 Classifier: Framework :: Django
 Classifier: Framework :: FastAPI
 Requires-Python: >=3.7
@@ -693,15 +694,15 @@
 Requires-Dist: scikit-learn==1.3.0
 Requires-Dist: requests
 Requires-Dist: psutil
 
 ![](pyrasp.png)
 
 <p>
-    <img src="https://img.shields.io/badge/Version-0.6.2-green?style=for-the-badge" alt="version 0.6.2"/>
+    <img src="https://img.shields.io/badge/Version-0.7.0-green?style=for-the-badge" alt="version 0.7.0"/>
     <a href="https://www.paracyberbellum.io">
         <img src="https://img.shields.io/badge/A%20project%20by-ParaCyberBellum-blue?style=for-the-badge" alt="A project by ParaCyberBellum"/>
     </a>
     <a href="https://twitter.com/ParaCyberBellum">
         <img src="https://img.shields.io/badge/Twitter-@ParaCyberBellum-yellow?style=for-the-badge&color=666666" alt="@ParaCyberBellum on Twitter"/>
     </a>
 </p>
@@ -712,14 +713,15 @@
 It can operate using a local configuration file or get it from a remote/cloud server. Logs and telemetry (optional) can be sent to remote servers as well, and threats information can be shared across agents.
 
 One specificity of `pyrasp` relies on the fact that it does not use signatures. Instead it will leverage decoys, thresholds, system and application internals, machine learning and grammatical analysis.
 
 # Documentation
 [Full documentation](https://paracyberbellum.gitbook.io/pyrasp)
 <br>[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.md)
+<br>[Web Site](https://pyrasp.paracyberbellum.io)
 
 # Contacts
 Renaud Bidou - renaud@paracyberbellum.io
```

### Comparing `pyrasp-0.6.2/README.md` & `pyrasp-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![](pyrasp.png)
 
 <p>
-    <img src="https://img.shields.io/badge/Version-0.6.2-green?style=for-the-badge" alt="version 0.6.2"/>
+    <img src="https://img.shields.io/badge/Version-0.7.0-green?style=for-the-badge" alt="version 0.7.0"/>
     <a href="https://www.paracyberbellum.io">
         <img src="https://img.shields.io/badge/A%20project%20by-ParaCyberBellum-blue?style=for-the-badge" alt="A project by ParaCyberBellum"/>
     </a>
     <a href="https://twitter.com/ParaCyberBellum">
         <img src="https://img.shields.io/badge/Twitter-@ParaCyberBellum-yellow?style=for-the-badge&color=666666" alt="@ParaCyberBellum on Twitter"/>
     </a>
 </p>
@@ -16,14 +16,15 @@
 It can operate using a local configuration file or get it from a remote/cloud server. Logs and telemetry (optional) can be sent to remote servers as well, and threats information can be shared across agents.
 
 One specificity of `pyrasp` relies on the fact that it does not use signatures. Instead it will leverage decoys, thresholds, system and application internals, machine learning and grammatical analysis.
 
 # Documentation
 [Full documentation](https://paracyberbellum.gitbook.io/pyrasp)
 <br>[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.md)
+<br>[Web Site](https://pyrasp.paracyberbellum.io)
 
 # Contacts
 Renaud Bidou - renaud@paracyberbellum.io
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 ![](pyrasp.png)
-[version 0.6.2]_[_A_ _p_r_o_j_e_c_t_ _b_y_ _P_a_r_a_C_y_b_e_r_B_e_l_l_u_m_]_[_@_P_a_r_a_C_y_b_e_r_B_e_l_l_u_m_ _o_n_ _T_w_i_t_t_e_r_]
+[version 0.7.0]_[_A_ _p_r_o_j_e_c_t_ _b_y_ _P_a_r_a_C_y_b_e_r_B_e_l_l_u_m_]_[_@_P_a_r_a_C_y_b_e_r_B_e_l_l_u_m_ _o_n_ _T_w_i_t_t_e_r_]
 # What is PyRASP ? `pyrasp` is a **Runtime Application Self Protection**
 package for Python-based Web Servers (Flask, FastAPI and Django) and Serverless
 Functions (AWS Lambda, Google Cloud Functions). It protects against the main
 attacks web applications are exposed to, from within the application. It is
 also capable of providing basic telemetry such as cpu and memory usage, as well
 as requests count. It can operate using a local configuration file or get it
 from a remote/cloud server. Logs and telemetry (optional) can be sent to remote
 servers as well, and threats information can be shared across agents. One
 specificity of `pyrasp` relies on the fact that it does not use signatures.
 Instead it will leverage decoys, thresholds, system and application internals,
 machine learning and grammatical analysis. # Documentation [Full documentation]
 (https://paracyberbellum.gitbook.io/pyrasp)
-[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.md) #
-Contacts Renaud Bidou - renaud@paracyberbellum.io
+[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.md)
+[Web Site](https://pyrasp.paracyberbellum.io) # Contacts Renaud Bidou -
+renaud@paracyberbellum.io
```

### Comparing `pyrasp-0.6.2/pyproject.toml` & `pyrasp-0.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrasp"
-version = "0.6.2"
+version = "0.7.0"
 authors = [
     { name = "Renaud Bidou", email = "renaud@paracyberbellum.io" }
 ]
 description = "Python RASP"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
@@ -20,13 +20,14 @@
   "sqlparse", 
   "scikit-learn==1.3.0",
   "requests",
   "psutil"
 ]
 
 [project.urls]
-Homepage = "https://github.com/rbidou/pyrasp"
+Homepage = "https://pyrasp.paracyberbellum.io"
 Documentation = "https://paracyberbellum.gitbook.io/pyrasp"
+GitHub = "https://github.com/rbidou/pyrasp"
 
 [tool.setuptools.package-data]
 pyrasp = ["data/*"]
```

### Comparing `pyrasp-0.6.2/pyrasp/pyrasp.py` & `pyrasp-0.7.0/pyrasp/pyrasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.6.2'
+VERSION = '0.7.0'
 
 from pprint import pprint
 import time
 import re
 import sqlparse
 import sqlite3
 import pickle
@@ -18,15 +18,15 @@
 from functools import partial
 import psutil
 import os
 from functools import wraps
 
 # Flask
 try:
-    from flask import request
+    from flask import request, redirect, url_for
     from flask import Response as FlaskResponse
     from flask.wrappers import Response as FlaskResponseType
     from werkzeug.utils import import_string
 except:
     pass
 
 # FastAPI
@@ -304,14 +304,25 @@
 
     # REQUESTS
     REQUESTS = {
         'success': 0,
         'errors': 0,
         'attacks': 0
     }
+
+    # API DATA
+    API_CONFIG = {}
+    API_BLACKLIST = []
+    API_STATUS = {
+        'version': '',
+        'blacklist': 0,
+        'xss_loaded': False,
+        'sqli_loaded': False,
+        'config': 'Default'
+    }
     
     ####################################################
     # CONSTRUCTOR & DESTRUCTOR
     ####################################################
 
     def __init__(self, app = None, app_name = None, hosts = [], conf = None, key = None, cloud_url = None, verbose_level = 10, dev = False):
 
@@ -358,23 +369,26 @@
                 self.KEY = os.environ.get('PYRASP_KEY')
 
             if self.KEY is None:
                 self.print_screen('[!] Agent key could not be found. Running default configuration.', init=True, new_line_up = True)
             
             if not self.load_cloud_config():
                 self.print_screen('[!] Could not load configuration from cloud server. Running default configuration.', init=True, new_line_up = True)
+            else:
+                self.API_STATUS['config'] = 'Cloud'
 
         # Load configuration file
         if not conf is None:
             self.CONF_FILE = conf
         else:
             self.CONF_FILE = os.environ.get('PYRASP_CONF')
 
         if not self.CONF_FILE is None:
-            self.load_file_config(self.CONF_FILE)
+            if self.load_file_config(self.CONF_FILE):
+                self.API_STATUS['config'] = 'Local'
 
         # Default config customization from 
         if all([
             self.CONF_FILE == None,
             self.KEY == None,
             not verbose_level == None
         ]):
@@ -458,14 +472,18 @@
                     sqli_model_loaded = True
 
             if not sqli_model_loaded:
                 self.print_screen('[!] SQLI model not loaded', init=False, new_line_up = False)
             else:
                 self.print_screen('[+] SQLI model loaded', init=True, new_line_up = False)
 
+        # Agent status
+        self.API_STATUS['version'] = VERSION
+        self.API_STATUS['xss_loaded'] = xss_model_loaded
+        self.API_STATUS['sqli_loaded'] = sqli_model_loaded
 
         # AWS, GCP & Azure
         if self.PLATFORM in CLOUD_FUNCTIONS:
             pass
 
         # Other environments
         else:   
@@ -603,16 +621,15 @@
                     if not new_entry in self.BLACKLIST:
                         self.BLACKLIST[new_entry] = time_now
             
                 # Force remove blacklist entries
                 remove_blacklist_entries = blacklist_update.get('remove') or []
                 for remove_entry in remove_blacklist_entries:
                     if remove_entry in self.BLACKLIST:
-                        del self.BLACKLIST[remove_entry]
-            
+                        del self.BLACKLIST[remove_entry]           
 
         # Set configuration
         if not error and server_data.get('config'):
             self.print_screen('[PyRASP] Loading new configuration')
             new_config = { 'config': server_data['config'] }
             config_changes = self.check_config_change(server_data['config'])
             self.load_config(new_config)
@@ -746,28 +763,34 @@
         if not error:
             result = self.load_config(config)
 
         return result
             
     def load_file_config(self, conf_file):
 
+        result = True
+
         self.print_screen(f'[+] Loading configuration from {conf_file}', init = True, new_line_up = False)
 
         try:
             with open(conf_file) as f:
                 config = json.load(f)
         except Exception as e:
             self.print_screen(f'[!] Error reading {conf_file}: {str(e)}', init = True, new_line_up = False)
+            result = False
         else:
             self.load_config(config)
+
+        return result
    
     def load_config(self, config):
 
         # Load parameters
         config_params = config.get('config') or config
+        self.API_CONFIG = config_params
 
         for key in config_params:
             setattr(self, key, config_params[key])
 
         # Setting defautl security checks
         for security_check in DEFAULT_SECURITY_CHECKS:
             if config_params['SECURITY_CHECKS'].get(security_check) == None:
@@ -776,49 +799,63 @@
         for key in config_params:
             self.print_screen(f'[+] {key} => {config_params[key]}', 100, init=False)    
 
         # Load blacklist
         config_blacklist = config.get('blacklist')
 
         if config_blacklist:
+
             self.BLACKLIST = config_blacklist
 
         return True
 
     ####################################################
     # ATTACK HANDLING
     ####################################################
 
     def handle_attack(self, attack, host, request_path, source_ip, timestamp):
 
         attack_id = attack['type']
         attack_check = ATTACKS_CHECKS[attack_id]
         attack_details = attack.get('details') or {}
+        attack_payload = None
+        if attack_details and attack_details.get('payload'):
+            attack_payload = attack_details['payload']
+            try:
+                attack_payload_b64 = base64.b64encode(attack_details['payload'].encode()).decode()
+                attack_details['payload'] = attack_payload_b64
+            except:
+                pass
+
         action = None
 
-        # Generic case
+        # Action
+        ## Generic case
         if not attack_id == 0:
             action = self.SECURITY_CHECKS[attack_check] 
-        # Blacklist
+        ## Blacklist
         else:
             action = 2
 
         attack_details['action'] = action
+
+        # Attack type
         if ATTACKS_CODES.get(attack_id):
             attack_details['codes'] = ATTACKS_CODES[attack_id]
 
         if not self.BLACKLIST_OVERRIDE and action == 2:
             self.blacklist_ip(source_ip, timestamp, attack_check)
 
-
+        # Print screen
         try:
-            self.print_screen(f'[!] {ATTACKS[attack_id]}: {attack["details"]["location"]} -> {attack["details"]["payload"]}')
+            self.print_screen(f'[!] {ATTACKS[attack_id]}: {attack["details"]["location"]} -> {attack_payload}')
         except:
             self.print_screen(f'[!] Attack - No details')
     
+        # Log
         if self.LOG_ENABLED:
             self.log_security_event(attack_check, source_ip, None, attack_details)
 
     ####################################################
     # CHECKS CONTROL
     ####################################################
 
@@ -1731,14 +1768,34 @@
                 match = text == pattern
                 
         except Exception as e:
             pass
 
         return match
 
+    ####################################################
+    # API
+    ####################################################
+
+    def get_config(self):
+
+        return self.API_CONFIG
+    
+    def get_blacklist(self):
+
+        self.API_BLACKLIST = [ i for i in self.BLACKLIST ]
+
+        return self.API_BLACKLIST
+    
+    def get_status(self):
+
+        self.API_STATUS['blacklist'] = len(self.BLACKLIST)
+
+        return self.API_STATUS
+
 class FlaskRASP(PyRASP):
 
     CURRENT_ATTACKS = {}
 
     def __init__(self, app, app_name=None, hosts=[], conf=None, key=None, cloud_url=None,verbose_level=10, dev=False):
         self.PLATFORM = 'Flask'
         super().__init__(app, app_name, hosts, conf, key, cloud_url, verbose_level, dev)
@@ -1764,16 +1821,17 @@
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
             
             attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
 
             # Send attack status in status code for handling by @after_request
             if not attack == None:
                 attack_id = '::'.join([host, request_method, request_path, source_ip])
-                self.CURRENT_ATTACKS[attack_id] = attack
-
+                self.CURRENT_ATTACKS[attack_id] = attack                
+                return FlaskResponse()
+        
     # Outgoing responses
     def set_after_security_checks(self, app):
         @app.after_request
         def after_request_callback(response):
 
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
```

### Comparing `pyrasp-0.6.2/pyrasp/pyrasp_data.py` & `pyrasp-0.7.0/pyrasp/pyrasp_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # VERSION
 #
 
 DATA_VERSION = '1.1.0'
-XSS_MODEL_VERSION = '1.2.0'
-SQLI_MODEL_VERSION = '1.1.0'
+XSS_MODEL_VERSION = '2.0.0'
+SQLI_MODEL_VERSION = '2.0.0'
 
 #
 # PLATFORMS
 #
 
 CLOUD_FUNCTIONS = ['AWS Lambda', 'Google Cloud Function', 'Azure Function' ]
 
@@ -206,18 +206,18 @@
         "/autodiscover", "/Autodiscover",           
         "/.git/",                                   
         "/.aws/ "                                 
     ],
 
     "EXCEPTIONS" : [],
 
-    "XSS_PROBA" : 0.60,
+    "XSS_PROBA" : 0.70,
     "MIN_XSS_LEN": 16,
 
-    "SQLI_PROBA" : 0.725,
+    "SQLI_PROBA" : 0.85,
     "MIN_SQLI_LEN": 8,
 
     "DLP_PHONE_NUMBERS": False,
     "DLP_CC_NUMBERS": False,
     "DLP_PRIVATE_KEYS": False,
     "DLP_HASHES": False,
     "DLP_WINDOWS_CREDS": False,
```

### Comparing `pyrasp-0.6.2/pyrasp.egg-info/PKG-INFO` & `pyrasp-0.7.0/pyrasp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasp
-Version: 0.6.2
+Version: 0.7.0
 Summary: Python RASP
 Author-email: Renaud Bidou <renaud@paracyberbellum.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,16 +674,17 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/rbidou/pyrasp
+Project-URL: Homepage, https://pyrasp.paracyberbellum.io
 Project-URL: Documentation, https://paracyberbellum.gitbook.io/pyrasp
+Project-URL: GitHub, https://github.com/rbidou/pyrasp
 Keywords: rasp,web application,security,xss,sql injection,waf,dlp
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Flask
 Classifier: Framework :: Django
 Classifier: Framework :: FastAPI
 Requires-Python: >=3.7
@@ -693,15 +694,15 @@
 Requires-Dist: scikit-learn==1.3.0
 Requires-Dist: requests
 Requires-Dist: psutil
 
 ![](pyrasp.png)
 
 <p>
-    <img src="https://img.shields.io/badge/Version-0.6.2-green?style=for-the-badge" alt="version 0.6.2"/>
+    <img src="https://img.shields.io/badge/Version-0.7.0-green?style=for-the-badge" alt="version 0.7.0"/>
     <a href="https://www.paracyberbellum.io">
         <img src="https://img.shields.io/badge/A%20project%20by-ParaCyberBellum-blue?style=for-the-badge" alt="A project by ParaCyberBellum"/>
     </a>
     <a href="https://twitter.com/ParaCyberBellum">
         <img src="https://img.shields.io/badge/Twitter-@ParaCyberBellum-yellow?style=for-the-badge&color=666666" alt="@ParaCyberBellum on Twitter"/>
     </a>
 </p>
@@ -712,14 +713,15 @@
 It can operate using a local configuration file or get it from a remote/cloud server. Logs and telemetry (optional) can be sent to remote servers as well, and threats information can be shared across agents.
 
 One specificity of `pyrasp` relies on the fact that it does not use signatures. Instead it will leverage decoys, thresholds, system and application internals, machine learning and grammatical analysis.
 
 # Documentation
 [Full documentation](https://paracyberbellum.gitbook.io/pyrasp)
 <br>[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.md)
+<br>[Web Site](https://pyrasp.paracyberbellum.io)
 
 # Contacts
 Renaud Bidou - renaud@paracyberbellum.io
```

