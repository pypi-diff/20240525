# Comparing `tmp/fyers_token_manager_3-0.1.0.tar.gz` & `tmp/fyers_token_manager_3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_3-0.1.0.tar", max compression
+gzip compressed data, was "fyers_token_manager_3-0.1.1.tar", max compression
```

## Comparing `fyers_token_manager_3-0.1.0.tar` & `fyers_token_manager_3-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       11 2024-05-25 04:15:25.173150 fyers_token_manager_3-0.1.0/LICENSE
--rw-r--r--   0        0        0      842 2024-05-25 05:58:58.018732 fyers_token_manager_3-0.1.0/README.md
--rw-r--r--   0        0        0     6414 2024-05-25 05:17:52.035268 fyers_token_manager_3-0.1.0/fyers_token_manager_3/__init__.py
--rw-r--r--   0        0        0     1834 2024-05-25 05:17:31.307041 fyers_token_manager_3-0.1.0/fyers_token_manager_3/base_token_manager.py
--rw-r--r--   0        0        0      387 2024-05-25 05:59:27.451060 fyers_token_manager_3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1412 1970-01-01 00:00:00.000000 fyers_token_manager_3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-05-25 04:15:25.173150 fyers_token_manager_3-0.1.1/LICENSE
+-rw-r--r--   0        0        0      856 2024-05-25 06:07:22.848344 fyers_token_manager_3-0.1.1/README.md
+-rw-r--r--   0        0        0     6436 2024-05-25 06:09:42.753897 fyers_token_manager_3-0.1.1/fyers_token_manager_3/__init__.py
+-rw-r--r--   0        0        0     1834 2024-05-25 06:09:40.101868 fyers_token_manager_3-0.1.1/fyers_token_manager_3/base_token_manager.py
+-rw-r--r--   0        0        0      387 2024-05-25 06:09:50.261981 fyers_token_manager_3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1426 1970-01-01 00:00:00.000000 fyers_token_manager_3-0.1.1/PKG-INFO
```

### Comparing `fyers_token_manager_3-0.1.0/README.md` & `fyers_token_manager_3-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 00000000: 6060 600d 0a63 6f6e 6669 6720 3d20 7b0d  ```..config = {.
-00000010: 0a20 2022 7573 6572 6e61 6d65 223a 2022  .  "username": "
-00000020: 3c55 5345 524e 414d 453e 222c 0d0a 2020  <USERNAME>",..  
-00000030: 2274 6f74 705f 6b65 7922 3a20 223c 544f  "totp_key": "<TO
-00000040: 5450 5f4b 4559 3e22 2c0d 0a20 2022 7069  TP_KEY>",..  "pi
-00000050: 6e22 3a20 223c 5049 4e3e 222c 0d0a 2020  n": "<PIN>",..  
-00000060: 2263 6c69 656e 745f 6964 223a 2022 3c43  "client_id": "<C
-00000070: 4c49 454e 545f 4944 3e22 2c0d 0a20 2022  LIENT_ID>",..  "
-00000080: 7365 6372 6574 5f6b 6579 223a 2022 3c53  secret_key": "<S
-00000090: 4543 5245 545f 4b45 593e 222c 0d0a 2020  ECRET_KEY>",..  
-000000a0: 2272 6564 6972 6563 745f 7572 6922 3a20  "redirect_uri": 
-000000b0: 3c52 4544 4952 4543 545f 5552 4c3e 0d0a  <REDIRECT_URL>..
-000000c0: 7d0d 0a60 6060 0d0a 0d0a 2323 2049 6e73  }..```....## Ins
-000000d0: 7461 6c6c 0d0a 0d0a 6060 600d 0a70 6970  tall....```..pip
-000000e0: 2069 6e73 7461 6c6c 2066 7965 7273 2d74   install fyers-t
-000000f0: 6f6b 656e 2d6d 616e 6167 6572 2d33 0d0a  oken-manager-3..
-00000100: 6060 600d 0a0d 0a23 2320 4679 6572 7320  ```....## Fyers 
-00000110: 546f 6b65 6e20 4765 6e65 7261 746f 720d  Token Generator.
-00000120: 0a0d 0a60 6060 0d0a 6672 6f6d 2066 7965  ...```..from fye
-00000130: 7273 5f74 6f6b 656e 5f6d 616e 6167 6572  rs_token_manager
-00000140: 5f76 3320 696d 706f 7274 2046 7965 7273  _v3 import Fyers
-00000150: 546f 6b65 6e4d 616e 6167 6572 0d0a 0d0a  TokenManager....
-00000160: 6679 6572 7354 6f6b 656e 4d61 6e61 6765  fyersTokenManage
-00000170: 7220 3d20 4679 6572 7354 6f6b 656e 4d61  r = FyersTokenMa
-00000180: 6e61 6765 7228 0d0a 2020 2020 7573 6572  nager(..    user
-00000190: 6e61 6d65 3d63 6f6e 6669 675b 2275 7365  name=config["use
-000001a0: 726e 616d 6522 5d2c 0d0a 2020 2020 746f  rname"],..    to
-000001b0: 7470 5f6b 6579 3d63 6f6e 6669 675b 2274  tp_key=config["t
-000001c0: 6f74 705f 6b65 7922 5d2c 0d0a 2020 2020  otp_key"],..    
-000001d0: 7069 6e3d 636f 6e66 6967 5b22 7069 6e22  pin=config["pin"
-000001e0: 5d2c 0d0a 2020 2020 636c 6965 6e74 5f69  ],..    client_i
-000001f0: 643d 636f 6e66 6967 5b22 636c 6965 6e74  d=config["client
-00000200: 5f69 6422 5d2c 0d0a 2020 2020 7365 6372  _id"],..    secr
-00000210: 6574 5f6b 6579 3d63 6f6e 6669 675b 2273  et_key=config["s
-00000220: 6563 7265 745f 6b65 7922 5d2c 0d0a 2020  ecret_key"],..  
-00000230: 2020 7265 6469 7265 6374 5f75 726c 3d63    redirect_url=c
-00000240: 6f6e 6669 675b 2272 6564 6972 6563 745f  onfig["redirect_
-00000250: 7572 6c22 5d2c 0d0a 290d 0a0d 0a70 7269  url"],..)....pri
-00000260: 6e74 2866 7965 7273 546f 6b65 6e4d 616e  nt(fyersTokenMan
-00000270: 6167 6572 2e68 7474 705f 6163 6365 7373  ager.http_access
-00000280: 5f74 6f6b 656e 290d 0a70 7269 6e74 2866  _token)..print(f
-00000290: 7965 7273 546f 6b65 6e4d 616e 6167 6572  yersTokenManager
-000002a0: 2e77 735f 6163 6365 7373 5f74 6f6b 656e  .ws_access_token
-000002b0: 290d 0a60 6060 0d0a 0d0a 2323 2323 2048  )..```....#### H
-000002c0: 5454 5020 436c 6965 6e74 0d0a 0d0a 2d20  TTP Client....- 
-000002d0: 6679 6572 7354 6f6b 656e 4d61 6e61 6765  fyersTokenManage
-000002e0: 722e 6874 7470 5f63 6c69 656e 742e 6765  r.http_client.ge
-000002f0: 745f 7072 6f66 696c 6528 290d 0a0d 0a23  t_profile()....#
-00000300: 2323 2320 5765 6253 6f63 6b65 7420 436c  ### WebSocket Cl
-00000310: 6965 6e74 0d0a 0d0a 2d20 6679 6572 7354  ient....- fyersT
-00000320: 6f6b 656e 4d61 6e61 6765 722e 7773 5f63  okenManager.ws_c
-00000330: 6c69 656e 742e 7375 6273 6372 6962 6528  lient.subscribe(
-00000340: 7061 796c 6f61 6429 0d0a                 payload)..
+00000010: 0a20 2020 2022 7573 6572 6e61 6d65 223a  .    "username":
+00000020: 2022 3c55 5345 524e 414d 453e 222c 0d0a   "<USERNAME>",..
+00000030: 2020 2020 2274 6f74 705f 6b65 7922 3a20      "totp_key": 
+00000040: 223c 544f 5450 5f4b 4559 3e22 2c0d 0a20  "<TOTP_KEY>",.. 
+00000050: 2020 2022 7069 6e22 3a20 223c 5049 4e3e     "pin": "<PIN>
+00000060: 222c 0d0a 2020 2020 2263 6c69 656e 745f  ",..    "client_
+00000070: 6964 223a 2022 3c43 4c49 454e 545f 4944  id": "<CLIENT_ID
+00000080: 3e22 2c0d 0a20 2020 2022 7365 6372 6574  >",..    "secret
+00000090: 5f6b 6579 223a 2022 3c53 4543 5245 545f  _key": "<SECRET_
+000000a0: 4b45 593e 222c 0d0a 2020 2020 2272 6564  KEY>",..    "red
+000000b0: 6972 6563 745f 7572 6922 3a20 223c 5245  irect_uri": "<RE
+000000c0: 4449 5245 4354 5f55 524c 3e22 2c0d 0a7d  DIRECT_URL>",..}
+000000d0: 0d0a 6060 600d 0a0d 0a23 2320 496e 7374  ..```....## Inst
+000000e0: 616c 6c0d 0a0d 0a60 6060 0d0a 7069 7020  all....```..pip 
+000000f0: 696e 7374 616c 6c20 6679 6572 732d 746f  install fyers-to
+00000100: 6b65 6e2d 6d61 6e61 6765 722d 330d 0a60  ken-manager-3..`
+00000110: 6060 0d0a 0d0a 2323 2046 7965 7273 2054  ``....## Fyers T
+00000120: 6f6b 656e 2047 656e 6572 6174 6f72 0d0a  oken Generator..
+00000130: 0d0a 6060 600d 0a66 726f 6d20 6679 6572  ..```..from fyer
+00000140: 735f 746f 6b65 6e5f 6d61 6e61 6765 725f  s_token_manager_
+00000150: 3320 696d 706f 7274 2046 7965 7273 546f  3 import FyersTo
+00000160: 6b65 6e4d 616e 6167 6572 0d0a 0d0a 6679  kenManager....fy
+00000170: 6572 7354 6f6b 656e 4d61 6e61 6765 7220  ersTokenManager 
+00000180: 3d20 4679 6572 7354 6f6b 656e 4d61 6e61  = FyersTokenMana
+00000190: 6765 7228 0d0a 2020 2020 7573 6572 6e61  ger(..    userna
+000001a0: 6d65 3d63 6f6e 6669 675b 2275 7365 726e  me=config["usern
+000001b0: 616d 6522 5d2c 0d0a 2020 2020 746f 7470  ame"],..    totp
+000001c0: 5f6b 6579 3d63 6f6e 6669 675b 2274 6f74  _key=config["tot
+000001d0: 705f 6b65 7922 5d2c 0d0a 2020 2020 7069  p_key"],..    pi
+000001e0: 6e3d 636f 6e66 6967 5b22 7069 6e22 5d2c  n=config["pin"],
+000001f0: 0d0a 2020 2020 636c 6965 6e74 5f69 643d  ..    client_id=
+00000200: 636f 6e66 6967 5b22 636c 6965 6e74 5f69  config["client_i
+00000210: 6422 5d2c 0d0a 2020 2020 7365 6372 6574  d"],..    secret
+00000220: 5f6b 6579 3d63 6f6e 6669 675b 2273 6563  _key=config["sec
+00000230: 7265 745f 6b65 7922 5d2c 0d0a 2020 2020  ret_key"],..    
+00000240: 7265 6469 7265 6374 5f75 726c 3d63 6f6e  redirect_url=con
+00000250: 6669 675b 2272 6564 6972 6563 745f 7572  fig["redirect_ur
+00000260: 6c22 5d2c 0d0a 290d 0a0d 0a70 7269 6e74  l"],..)....print
+00000270: 2866 7965 7273 546f 6b65 6e4d 616e 6167  (fyersTokenManag
+00000280: 6572 2e68 7474 705f 6163 6365 7373 5f74  er.http_access_t
+00000290: 6f6b 656e 290d 0a70 7269 6e74 2866 7965  oken)..print(fye
+000002a0: 7273 546f 6b65 6e4d 616e 6167 6572 2e77  rsTokenManager.w
+000002b0: 735f 6163 6365 7373 5f74 6f6b 656e 290d  s_access_token).
+000002c0: 0a60 6060 0d0a 0d0a 2323 2323 2048 5454  .```....#### HTT
+000002d0: 5020 436c 6965 6e74 0d0a 0d0a 2d20 6679  P Client....- fy
+000002e0: 6572 7354 6f6b 656e 4d61 6e61 6765 722e  ersTokenManager.
+000002f0: 6874 7470 5f63 6c69 656e 742e 6765 745f  http_client.get_
+00000300: 7072 6f66 696c 6528 290d 0a0d 0a23 2323  profile()....###
+00000310: 2320 5765 6253 6f63 6b65 7420 436c 6965  # WebSocket Clie
+00000320: 6e74 0d0a 0d0a 2d20 6679 6572 7354 6f6b  nt....- fyersTok
+00000330: 656e 4d61 6e61 6765 722e 7773 5f63 6c69  enManager.ws_cli
+00000340: 656e 742e 7375 6273 6372 6962 6528 7061  ent.subscribe(pa
+00000350: 796c 6f61 6429 0d0a                      yload)..
```

### Comparing `fyers_token_manager_3-0.1.0/fyers_token_manager_3/__init__.py` & `fyers_token_manager_3-0.1.1/fyers_token_manager_3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any
 from urllib.parse import urlparse, parse_qs
 
 from fyers_apiv3 import fyersModel
 from fyers_apiv3.FyersWebsocket.data_ws import FyersDataSocket
 from fyers_apiv3.fyersModel import FyersModel
 
-from base_token_manager import BaseTokenManager
+from fyers_token_manager_3.base_token_manager import BaseTokenManager
 
 AUTH_URL = "https://api-t2.fyers.in/vagator/v2"
 API_URL = "https://api.fyers.in/api/v2"
 URL_SEND_LOGIN_OTP_V2 = AUTH_URL + "/send_login_otp_v2"
 URL_VERIFY_TOTP = AUTH_URL + "/verify_otp"
 URL_VERIFY_PIN_V2 = AUTH_URL + "/verify_pin_v2"
 URL_TOKEN = API_URL + "/token"
```

### Comparing `fyers_token_manager_3-0.1.0/fyers_token_manager_3/base_token_manager.py` & `fyers_token_manager_3-0.1.1/fyers_token_manager_3/base_token_manager.py`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_3-0.1.0/PKG-INFO` & `fyers_token_manager_3-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager-3
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,33 +14,33 @@
 Requires-Dist: pyotp (>=2.9.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
 
 ```
 config = {
-  "username": "<USERNAME>",
-  "totp_key": "<TOTP_KEY>",
-  "pin": "<PIN>",
-  "client_id": "<CLIENT_ID>",
-  "secret_key": "<SECRET_KEY>",
-  "redirect_uri": <REDIRECT_URL>
+    "username": "<USERNAME>",
+    "totp_key": "<TOTP_KEY>",
+    "pin": "<PIN>",
+    "client_id": "<CLIENT_ID>",
+    "secret_key": "<SECRET_KEY>",
+    "redirect_uri": "<REDIRECT_URL>",
 }
 ```
 
 ## Install
 
 ```
 pip install fyers-token-manager-3
 ```
 
 ## Fyers Token Generator
 
 ```
-from fyers_token_manager_v3 import FyersTokenManager
+from fyers_token_manager_3 import FyersTokenManager
 
 fyersTokenManager = FyersTokenManager(
     username=config["username"],
     totp_key=config["totp_key"],
     pin=config["pin"],
     client_id=config["client_id"],
     secret_key=config["secret_key"],
```

