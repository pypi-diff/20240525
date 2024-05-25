# Comparing `tmp/tweeterpy-1.1.2.tar.gz` & `tmp/tweeterpy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-1.1.2.tar", last modified: Sat May 18 10:23:32 2024, max compression
+gzip compressed data, was "tweeterpy-1.1.3.tar", last modified: Fri May 24 14:07:57 2024, max compression
```

## Comparing `tweeterpy-1.1.2.tar` & `tweeterpy-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 10:23:32.616063 tweeterpy-1.1.2/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.1.2/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3967 2024-05-18 10:23:32.616063 tweeterpy-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2530 2023-10-11 13:44:39.000000 tweeterpy-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-18 10:23:32.616063 tweeterpy-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1499 2024-05-18 10:22:13.000000 tweeterpy-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 10:23:32.537946 tweeterpy-1.1.2/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.1.2/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     8241 2024-01-02 14:26:34.000000 tweeterpy-1.1.2/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0     2505 2023-10-11 13:49:03.000000 tweeterpy-1.1.2/tweeterpy/config.py
--rw-rw-rw-   0        0        0     3855 2024-05-17 15:23:46.000000 tweeterpy-1.1.2/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.1.2/tweeterpy/logging_util.py
--rw-rw-rw-   0        0        0     9024 2023-10-10 14:44:59.000000 tweeterpy-1.1.2/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1984 2024-01-04 12:34:59.000000 tweeterpy-1.1.2/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0     2481 2023-09-07 09:39:56.000000 tweeterpy-1.1.2/tweeterpy/session_util.py
--rw-rw-rw-   0        0        0    32367 2024-05-18 07:41:57.000000 tweeterpy-1.1.2/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0    16546 2024-05-18 07:23:11.000000 tweeterpy-1.1.2/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2024-05-18 10:23:32.600455 tweeterpy-1.1.2/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3967 2024-05-18 10:23:32.000000 tweeterpy-1.1.2/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-05-18 10:23:32.000000 tweeterpy-1.1.2/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 10:23:32.000000 tweeterpy-1.1.2/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2024-05-18 10:23:32.000000 tweeterpy-1.1.2/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 10:23:32.000000 tweeterpy-1.1.2/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 14:07:57.820560 tweeterpy-1.1.3/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3967 2024-05-24 14:07:57.820560 tweeterpy-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2023-10-11 13:44:39.000000 tweeterpy-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 14:07:57.820560 tweeterpy-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2024-05-24 13:39:18.000000 tweeterpy-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:07:57.758036 tweeterpy-1.1.3/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.1.3/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     8361 2024-05-24 13:19:12.000000 tweeterpy-1.1.3/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0     2428 2024-05-24 13:19:24.000000 tweeterpy-1.1.3/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     3855 2024-05-17 15:23:46.000000 tweeterpy-1.1.3/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.1.3/tweeterpy/logging_util.py
+-rw-rw-rw-   0        0        0     9250 2024-05-24 13:21:29.000000 tweeterpy-1.1.3/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     2126 2024-05-24 13:38:49.000000 tweeterpy-1.1.3/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0     2462 2024-05-24 13:32:11.000000 tweeterpy-1.1.3/tweeterpy/session_util.py
+-rw-rw-rw-   0        0        0    32742 2024-05-24 13:58:17.000000 tweeterpy-1.1.3/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0    16546 2024-05-18 07:23:11.000000 tweeterpy-1.1.3/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:07:57.820560 tweeterpy-1.1.3/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3967 2024-05-24 14:07:57.000000 tweeterpy-1.1.3/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-05-24 14:07:57.000000 tweeterpy-1.1.3/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 14:07:57.000000 tweeterpy-1.1.3/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2024-05-24 14:07:57.000000 tweeterpy-1.1.3/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 14:07:57.000000 tweeterpy-1.1.3/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-1.1.2/LICENSE` & `tweeterpy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.2/PKG-INFO` & `tweeterpy-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.1.2
+Version: 1.1.3
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.2 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.3 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tweeterpy-1.1.2/README.md` & `tweeterpy-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.2/setup.py` & `tweeterpy-1.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-1.1.2/tweeterpy/api_util.py` & `tweeterpy-1.1.3/tweeterpy/api_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 
 class ApiUpdater:
     """
         Twitter updates its API quite frequently. Therefore, ApiUpdater checks for the latest updates and modifies the api_endpoints, feature_switches, path etc in constants.py
     """
 
-    def __init__(self, update_api=True):
+    def __init__(self, update_api=True, session=None):
+        self.__session = session
         try:
             logger.debug('Updating API...')
             # fmt: off - Turns off formatting for this block of code.
             try:
                 if not update_api:
                     raise Exception("Skipping API Updates.")
                 api_files_data = []
@@ -55,15 +56,15 @@
             logger.info("API Updated Successfully.")
         except Exception as error:
             logger.exception(f"API Couldn't be Updated.\n{error}")
             raise
             # fmt: on 
 
     def _get_home_page_source(self):
-        return str(make_request(Path.BASE_URL))
+        return str(make_request(Path.BASE_URL, session=self.__session))
 
     def _get_api_file_url(self, page_source=None):
         if page_source is None:
             page_source = self._get_home_page_source
         try:
             api_file_name = re.search(api_file_regex, page_source).group(1)
             api_file_url = f"{Path.TWITTER_CDN}/api.{eval(api_file_name)}a.js"
@@ -84,20 +85,20 @@
             logger.exception(f"Couldn't get the main file Url.\n{error}")
             return None
         return main_file_url
 
     def _get_api_file_content(self, file_url=None):
         if file_url is None:
             file_url = self._get_api_file_url()
-        return str(make_request(file_url))
+        return str(make_request(file_url, session=self.__session))
 
     def _get_main_file_content(self, file_url=None):
         if file_url is None:
             file_url = self._get_main_file_url()
-        return str(make_request(file_url))
+        return str(make_request(file_url, session=self.__session))
 
     def _js_to_py_dict(sel, page_source):
         if isinstance(page_source, list):
             page_source = "\n".join([str(item) for item in page_source])
         else:
             page_source = str(page_source)
         matches = []
```

### Comparing `tweeterpy-1.1.2/tweeterpy/config.py` & `tweeterpy-1.1.3/tweeterpy/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Configuration File
-_DEFAULT_SESSION = None  # Used to reuse generated session. DON'T CHANGE IT
 _RATE_LIMIT_STATS = None  # Used to keep a track of api limits. DON'T CHANGE IT
 
 _USER_AGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36'
 
 # Maximun number of retries for each request
 MAX_RETRIES = 3
```

### Comparing `tweeterpy-1.1.2/tweeterpy/constants.py` & `tweeterpy-1.1.3/tweeterpy/constants.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.2/tweeterpy/logging_util.py` & `tweeterpy-1.1.3/tweeterpy/logging_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.2/tweeterpy/login_util.py` & `tweeterpy-1.1.3/tweeterpy/login_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .constants import Path
 from .request_util import make_request
 from .util import find_nested_key
 from .logging_util import disable_logger
 
 
 class TaskHandler:
-    def __init__(self):
-        pass
+    def __init__(self, session=None):
+        self.__session = session
 
     def _create_task_mapper(self, username, password, verification_input_data):
         # fmt: off  - Turns off formatting for this block of code. Just for the readability purpose.
         task_flow_mapper = {"LoginJsInstrumentationSubtask":{"task_executor": self._get_user_flow_token,"task_parameter":None},
                             "LoginEnterUserIdentifierSSO":{"task_executor": self._get_password_flow_token,"task_parameter":username},
                             "LoginEnterAlternateIdentifierSubtask":{"task_executor": self._handle_suspicious_login,"task_parameter":verification_input_data},
                             "LoginEnterPassword":{"task_executor": self._get_account_duplication_flow_token,"task_parameter":password},
@@ -28,60 +28,60 @@
                                  'choice_selection': 3, 'contacts_live_sync_permission_prompt': 0, 'cta': 7, 'email_verification': 2, 'end_flow': 1,
                                  'enter_date': 1, 'enter_email': 2, 'enter_password': 5, 'enter_phone': 2, 'enter_recaptcha': 1, 'enter_text': 5,
                                  'enter_username': 2, 'generic_urt': 3, 'in_app_notification': 1, 'interest_picker': 3, 'js_instrumentation': 1,
                                  'menu_dialog': 1, 'notifications_permission_prompt': 2, 'open_account': 2, 'open_home_timeline': 1, 'open_link': 1,
                                  'phone_verification': 4, 'privacy_options': 1, 'security_key': 3, 'select_avatar': 4, 'select_banner': 2,
                                  'settings_list': 7, 'show_code': 1, 'sign_up': 2, 'sign_up_review': 4, 'tweet_selection_urt': 1, 'update_users': 1,
                                  'upload_media': 1, 'user_recommendations_list': 4, 'user_recommendations_urt': 1, 'wait_spinner': 3, 'web_modal': 1}}
-        return make_request(Path.TASK_URL, method="POST", params=params, json=payload)
+        return make_request(Path.TASK_URL, method="POST", params=params, json=payload, session=self.__session)
 
     def _get_javscript_instrumentation_subtask(self):
         params = {'c_name': 'ui_metrics'}
-        return make_request(Path.JAVSCRIPT_INSTRUMENTATION_URL, params=params)
+        return make_request(Path.JAVSCRIPT_INSTRUMENTATION_URL, params=params, session=self.__session)
 
     def _get_user_flow_token(self, flow_token, subtask_id="LoginJsInstrumentationSubtask"):
         payload = {'flow_token': flow_token,
                    'subtask_inputs': [{'subtask_id': subtask_id,
                                       'js_instrumentation': {
                                           'response': '',
                                           'link': 'next_link'}}]}
-        return make_request(Path.TASK_URL, method="POST", json=payload)
+        return make_request(Path.TASK_URL, method="POST", json=payload, session=self.__session)
 
     @disable_logger
     def _get_password_flow_token(self, flow_token, subtask_id="LoginEnterUserIdentifierSSO", username=None):
         payload = {'flow_token': flow_token,
                    'subtask_inputs': [{'subtask_id': subtask_id,
                                       'settings_list': {
                                           'setting_responses': [{'key': 'user_identifier', 'response_data': {'text_data': {'result': username}}}],
                                           'link': 'next_link'}}]}
-        return make_request(Path.TASK_URL, method="POST", json=payload)
+        return make_request(Path.TASK_URL, method="POST", json=payload, session=self.__session)
 
     @disable_logger
     def _get_account_duplication_flow_token(self, flow_token, subtask_id="LoginEnterPassword", password=None):
         payload = {'flow_token': flow_token,
                    'subtask_inputs': [{'subtask_id': subtask_id,
                                       'enter_password': {'password': password, 'link': 'next_link'}}]}
-        return make_request(Path.TASK_URL, method="POST", json=payload)
+        return make_request(Path.TASK_URL, method="POST", json=payload, session=self.__session)
 
     def _check_suspicious_login(self, flow_token, subtask_id="DenyLoginSubtask"):
         payload = {"flow_token": flow_token,
                    "subtask_inputs": [{"subtask_id": subtask_id, "cta": {"link": "next_link"}}]}
-        return make_request(Path.TASK_URL, method="POST", json=payload)
+        return make_request(Path.TASK_URL, method="POST", json=payload, session=self.__session)
 
     def _check_account_duplication(self, flow_token, subtask_id="AccountDuplicationCheck"):
         payload = {'flow_token': flow_token,
                    'subtask_inputs': [{'subtask_id': subtask_id, 'check_logged_in_account': {'link': 'AccountDuplicationCheck_false'}}]}
-        return make_request(Path.TASK_URL, method="POST", json=payload)
+        return make_request(Path.TASK_URL, method="POST", json=payload, session=self.__session)
 
     def _handle_suspicious_login(self, flow_token, subtask_id="LoginAcid",verification_input_data=None):
         payload = {"flow_token": flow_token,
                    "subtask_inputs": [{"subtask_id": subtask_id, "enter_text": {"text": verification_input_data,"link":"next_link"}}]}
         handle_incorrect_input = True
         while handle_incorrect_input:
-            response = make_request(Path.TASK_URL, method="POST", json=payload, skip_error_checking=True)
+            response = make_request(Path.TASK_URL, method="POST", json=payload, skip_error_checking=True, session=self.__session)
             if isinstance(response, dict) and "errors" in response.keys():
                 error_message = "\n".join([error['message'] for error in response['errors']])
                 payload['subtask_inputs'][0]['enter_text']['text'] = str(input(f"{error_message} - Type again ==> "))
             else:
                 handle_incorrect_input = False
         return response
```

### Comparing `tweeterpy-1.1.2/tweeterpy/request_util.py` & `tweeterpy-1.1.3/tweeterpy/request_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from . import config
 
 logging.config.dictConfig(config.LOGGING_CONFIG)
 logger = logging.getLogger(__name__)
 
 
 def make_request(url, session=None, method=None, max_retries=None, timeout=None, skip_error_checking=False, **kwargs):
+    if session is None:
+        raise NameError("name 'session' is not defined.")
+    if not isinstance(session, requests.Session):
+        raise TypeError(f"Invalid session type. {session} is not a requests.Session Object...")
     if method is None:
         method = "GET"
     if max_retries is None:
         max_retries = config.MAX_RETRIES or 3
-    if session is None:
-        session = config._DEFAULT_SESSION or requests.Session()
     if timeout is None:
         timeout = config.TIMEOUT or 30
     logger.debug(f"{locals()}")
     for retry_count, _ in enumerate(range(max_retries), start=1):
         response_text, api_limit_stats = "", {}
         try:
             response = session.request(method, url, timeout=timeout, **kwargs)
```

### Comparing `tweeterpy-1.1.2/tweeterpy/session_util.py` & `tweeterpy-1.1.3/tweeterpy/session_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,41 +30,39 @@
         file_number = int(input("\nChoose a vaild Number : ").strip())
     else:
         file_path = os.path.join(directory_path, all_files[file_number-1])
     return file_path
 
 
 def save_session(filename=None, path=None, session=None):
-    if session is None or not isinstance(session, requests.Session):
-        logger.warn(
-            "No Session object given. Trying to save existing/default Session...")
-        if config._DEFAULT_SESSION:
-            session = config._DEFAULT_SESSION
-        else:
-            raise TypeError(f'{session} is not a requests Session Object...')
+    if session is None:
+        raise NameError("name 'session' is not defined.")
+    if not isinstance(session, requests.Session):
+        raise TypeError(f"Invalid session type. {session} is not a requests.Session Object...")
     if filename is None:
         filename = str(
             input("Enter Username/Account Name to Save the Session : ")).strip()
     if path is None:
         path = _create_session_directory()
     filename = f"{filename}.pkl"
     file_path = os.path.join(path, filename)
     with open(file_path, "wb") as file:
         pickle.dump([session.headers, session.cookies], file)
     return file_path
 
 
 def load_session(file_path=None, session=None):
+    if session is None:
+        raise NameError("name 'session' is not defined.")
+    if not isinstance(session, requests.Session):
+        raise TypeError(f"Invalid session type. {session} is not a requests.Session Object...")
     if file_path is None:
         file_path = _show_saved_sessions()
     with open(file_path, "rb") as file:
         headers, cookies = pickle.load(file)
-    if session is None:
-        session = config._DEFAULT_SESSION or requests.Session()
     session.headers = headers
     session.cookies = cookies
-    config._DEFAULT_SESSION = session
     return session
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `tweeterpy-1.1.2/tweeterpy/tweeterpy.py` & `tweeterpy-1.1.3/tweeterpy/tweeterpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,36 +24,36 @@
         if config.DISABLE_LOGS or config.DISABLE_EXTERNAL_LOGS:
             logger.debug("Disabling logs...")
             config.LOG_LEVEL = "ERROR" if config.DISABLE_LOGS else config.LOG_LEVEL
             disable_external_only = config.DISABLE_EXTERNAL_LOGS if not config.DISABLE_LOGS else False
             set_log_level(logging.ERROR, external_only=disable_external_only)
         self.generate_session()
         # update api endpoints
-        self.__token = self.session.headers.pop("Authorization")
+        self.__token = self.__session.headers.pop("Authorization")
         try:
-            ApiUpdater(update_api=config.UPDATE_API)
+            ApiUpdater(update_api=config.UPDATE_API, session=self.__session)
         except Exception as error:
             logger.warn(error)
-        self.session.headers.update({"Authorization":self.__token})
+        self.__session.headers.update({"Authorization":self.__token})
 
     def _generate_request_data(self, endpoint, variables=None, **kwargs):
         # fmt: off - Turns off formatting for this block of code. Just for the readability purpose.
         url = util.generate_url(domain=Path.API_URL, url_path=endpoint)
         query_params = {}
         if variables:
             query_params["variables"] = json.dumps(variables)
         if kwargs:
             features = FeatureSwitch().get_query_features(endpoint) or util.generate_features(**kwargs)
             query_params["features"] = json.dumps(features)
         # fmt: on   
-        request_payload = {"url": url, "params": query_params}
+        request_payload = {"url": url, "params": query_params, "session":self.__session}
         logger.debug(f"Request Payload => {request_payload}")
         return request_payload
 
-    def _handle_pagination(self, url, params, end_cursor=None, data_path=None, total=None, pagination=True):
+    def _handle_pagination(self, url, params, end_cursor=None, data_path=None, total=None, pagination=True, **kwargs):
         # fmt: off  - Turns off formatting for this block of code. Just for the readability purpose.
         def filter_data(response):
             filtered_data = []
             for each_entry in response:
                 if each_entry['entryId'].startswith('cursor-top') or each_entry['entryId'].startswith('cursor-bottom'):
                     continue
                 filtered_data.append(each_entry)
@@ -61,21 +61,22 @@
                     return filtered_data
             return filtered_data
 
         if not pagination and total:
             logger.warn("Either enable the pagination or disable total number of results.")
             raise Exception("pagination cannot be disabled while the total number of results are specified.")
         data_container = {"data": [],"cursor_endpoint": None, "has_next_page": True, "api_rate_limit":config._RATE_LIMIT_STATS}
+        session = kwargs.get("session", self.__session)
         while data_container["has_next_page"]:
             try:
                 if end_cursor:
                     variables = json.loads(params['variables'])
                     variables['cursor'] = end_cursor
                     params['variables'] = json.dumps(variables)
-                response = make_request(url, params=params)
+                response = make_request(url, params=params, session=session)
                 data = [item for item in reduce(
                     dict.get, data_path, response) if item['type'] == 'TimelineAddEntries'][0]['entries']
                 top_cursor = [
                     entry for entry in data if entry['entryId'].startswith('cursor-top')]
                 if top_cursor:
                     top_cursor = reduce(dict.get, ('content','value'),top_cursor[0]) or reduce(dict.get, ('content','itemContent','value'),end_cursor[0])
                 end_cursor = [
@@ -103,35 +104,36 @@
 
             except Exception as error:
                 logger.exception(error)
                 return data_container
 
     @property
     def session(self):
-        return self._session
+        return self.__session
 
     @session.setter
     def session(self, session):
-        self._session = session
-        config._DEFAULT_SESSION = session
+        self.__session = session
 
     @property
     def me(self):
         """Returns logged in user information.
 
         Returns:
             dict: Currently logged in user's data.
         """
         variables = {"withCommunitiesMemberships": True,
                      "withSubscribedTab": True, "withCommunitiesCreation": True}
         request_payload = self._generate_request_data(
             Path.VIEWER_ENDPOINT, variables, user_data_features=True)
-        response = self.session.get(**request_payload)
         try:
-            return response.json()
+            response = make_request(**request_payload)
+            if not isinstance(response, dict):
+                raise Exception(response)
+            return response
         except:
             logger.info("Guest Session")
             return
 
     def login_decorator(original_function):
         def wrapper(self, *args, **kwargs):
             if not self.logged_in():
@@ -147,90 +149,96 @@
             auth_token (str, optional): Generate session with an auth-token. If auth_token is None (Default Behaviour), generates a guest session without login. Defaults to None.
 
         Returns:
             requests.Session: requests.Session Object.
         """
         try:
             logger.debug("Trying to generate a new session.")
-            self.session = requests.Session()
+            session = requests.Session()
             if config.PROXY is not None:
-                self.session.proxies = config.PROXY
-                self.session.verify = False
-            self.session.headers.update(util.generate_headers())
-            # home_page = make_request(Path.BASE_URL, session=self.session)
-            home_page = util.handle_x_migration(session=self.session)
-            guest_token = make_request(
-                Path.GUEST_TOKEN_URL, method="POST", session=self.session).get('guest_token', util.find_guest_token(home_page))
-            self.session.headers.update({'X-Guest-Token': guest_token})
-            self.session.cookies.update({'gt': guest_token})
+                session.proxies = config.PROXY
+                session.verify = False
+            session.headers.update(util.generate_headers())
+            # home_page = make_request(Path.BASE_URL, session=session)
+            home_page = util.handle_x_migration(session=session)
+            try:
+                guest_token = make_request(
+                    Path.GUEST_TOKEN_URL, method="POST", session=session).get('guest_token', util.find_guest_token(home_page))
+            except Exception as error:
+                logger.error(error)
+            session.headers.update({'X-Guest-Token': guest_token})
+            session.cookies.update({'gt': guest_token})
             if auth_token:
-                self.session.cookies.update({'auth_token': auth_token})
-                util.generate_headers(self.session)
+                session.cookies.update({'auth_token': auth_token})
+                util.generate_headers(session)
         except Exception as error:
             logger.exception(f"Couldn't generate a new session.\n{error}\n")
             raise
         logger.debug("Session has been generated.")
-        return self.session
+        self.__session = session
+        return self.__session
 
     def save_session(self, session=None, session_name=None):
         """Save a logged in session to avoid frequent logins in future.
 
         Args:
             session (requests.Session, optional): requests.Session object you want to save. If None, saves current session by default. Defaults to None. 
             session_name (str, optional): Session name. If None, uses currently logged in username. Defaults to None.
 
         Returns:
             path: Saved session file path.
         """
         if session is None:
-            session = self.session
+            session = self.__session
         if session_name is None:
             session_name = self.me['data']['viewer']['user_results']['result']['legacy']['screen_name']
         return save_session(filename=session_name, session=session)
 
     def load_session(self, session_file_path=None, session=None):
         """Load a saved session.
 
         Args:
             session_file_path (path, optional): File path to load session from. If None, shows a list of all saved session to choose from. Defaults to None.
             session (request.Session, optional): requests.Session object to load a saved session into. Defaults to None.
 
         Returns:
             requests.Session: Restored session.
         """
-        self.session = load_session(
+        if session is None:
+            session = self.generate_session()
+        self.__session = load_session(
             file_path=session_file_path, session=session)
-        return self.session
+        return self.__session
 
     def logged_in(self):
         """Check if the user is logged in.
 
         Returns:
             bool: Returns True if the user is logged in.
         """
-        if "auth_token" in self.session.cookies.keys():
+        if "auth_token" in self.__session.cookies.keys():
             # logger.info('User is authenticated.')
             return True
         return False
 
     def login(self, username=None, password=None):
         """Log into an account.
 
         Args:
             username (str, optional): Twitter username or email. Defaults to None.
             password (str, optional): Password. Defaults to None.
         """
-        if "auth_token" in self.session.cookies.keys():
+        if "auth_token" in self.__session.cookies.keys():
             self.generate_session()
         if username is None:
             username = str(input("Enter Your Username or Email : ")).strip()
         if password is None:
             password = getpass.getpass()
-        TaskHandler().login(username, password)
-        util.generate_headers(session=self.session)
+        TaskHandler(session=self.__session).login(username, password)
+        util.generate_headers(session=self.__session)
         try:
             user = self.me
             username = util.find_nested_key(user, 'screen_name')
             account_locked = util.find_nested_key(user, 'bounce_location')
             if account_locked and not username:
                 raise Exception(
                     "Account logged in but couldn't get the user's details ! Make sure, the given account is working. (Ignore if its working)")
```

### Comparing `tweeterpy-1.1.2/tweeterpy/util.py` & `tweeterpy-1.1.3/tweeterpy/util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.2/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-1.1.3/tweeterpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.1.2
+Version: 1.1.3
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.2 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.3 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

