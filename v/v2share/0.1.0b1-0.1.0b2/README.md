# Comparing `tmp/v2share-0.1.0b1.tar.gz` & `tmp/v2share-0.1.0b2.tar.gz`

## Comparing `v2share-0.1.0b1.tar` & `v2share-0.1.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0b1/requirements.txt
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0b1/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0b1/tests/__init__.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 v2share-0.1.0b1/tests/test_links.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/_version.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/clash.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/clashmeta.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/data.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/links.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/singbox.py
--rw-r--r--   0        0        0    11033 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/xray.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/templates/clash.yml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/templates/singbox.json
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/templates/xray.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/templates/xray_mux.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 v2share-0.1.0b1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0b1/README.md
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0b2/requirements.txt
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0b2/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0b2/tests/__init__.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 v2share-0.1.0b2/tests/test_links.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/_version.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/clash.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/clashmeta.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/data.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/links.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/singbox.py
+-rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/xray.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/templates/clash.yml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/templates/singbox.json
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/templates/xray.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 v2share-0.1.0b2/v2share/templates/xray_mux.json
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 v2share-0.1.0b2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0b2/README.md
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0b2/PKG-INFO
```

### Comparing `v2share-0.1.0b1/.github/workflows/python-tests.yml` & `v2share-0.1.0b2/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b1/tests/test_links.py` & `v2share-0.1.0b2/tests/test_links.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 def test_shadowsocks_link():
     ss = V2Data(
         "shadowsocks",
         "remark",
         "127.0.0.1",
         1234,
-        uuid=uuid.UUID("bb34fc3a-529d-473a-a3d9-1749b2116f2a"),
+        password="1234",
     )
-    assert ss.to_link() == "ss://Tm9uZTpOb25lQDEyNy4wLjAuMToxMjM0#remark"
+    assert ss.to_link() == "ss://Tm9uZToxMjM0QDEyNy4wLjAuMToxMjM0#remark"
 
 
 def test_trojan_link():
     tj = V2Data("trojan", "remark", "127.0.0.1", 1234, password="1234")
     assert tj.to_link() == "trojan://1234@127.0.0.1:1234?security=none&type=tcp#remark"
```

### Comparing `v2share-0.1.0b1/v2share/clash.py` & `v2share-0.1.0b2/v2share/clash.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b1/v2share/clashmeta.py` & `v2share-0.1.0b2/v2share/clashmeta.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b1/v2share/data.py` & `v2share-0.1.0b2/v2share/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,123 +13,130 @@
     address: str
     port: int
     shadowsocks_method: Optional[str] = None
     uuid: Optional[UUID] = None
     vmess_security: str = "auto"
     password: Optional[str] = None
     host: Optional[str] = None
-    transport_type: Optional[str] = "tcp"
+    transport_type: str = "tcp"
     grpc_multi_mode: bool = False
     path: Optional[str] = None
-    kcp_header_type: Optional[str] = None
     header_type: Optional[str] = None
-    tls: Optional[str] = "none"
+    tls: str = "none"
     flow: Optional[str] = None
     sni: Optional[str] = None
     fingerprint: Optional[str] = None
     alpn: Optional[str] = None
     reality_pbk: Optional[str] = None
     reality_sid: Optional[str] = None
     reality_spx: Optional[str] = None
     fragment: bool = False
-    fragment_packets: Optional[str] = "tlshello"
-    fragment_length: Optional[str] = "100-200"
-    fragment_interval: Optional[str] = "10-20"
+    fragment_packets: str = "tlshello"
+    fragment_length: str = "100-200"
+    fragment_interval: str = "10-20"
     allow_insecure: bool = False
 
     def _apply_tls_settings(self, payload):
-        if self.tls == "tls" or self.tls == "reality":
+        if self.tls in ["tls", "reality"]:
             payload.update(
                 {
                     "sni": self.sni,
                     "fp": self.fingerprint,
                 }
             )
         if self.tls == "tls":
             payload.update(
                 {
                     "alpn": self.alpn,
                 }
             )
-        if self.tls == "reality":
+        elif self.tls == "reality":
             payload.update(
                 {
                     "pbk": self.reality_pbk,
                     "sid": self.reality_sid,
                     "spx": self.reality_spx,
                 }
             )
 
+    def _apply_trojan_vless_transport(self, payload):
+        if self.transport_type == "grpc":
+            transport_data = {
+                "serviceName": self.path,
+                "authority": self.host,
+                "mode": "multi" if self.grpc_multi_mode else "gun",
+            }
+        elif self.transport_type == "kcp":
+            transport_data = {"seed": self.path}
+        elif self.transport_type == "quic":
+            transport_data = {"key": self.path, "quicSecurity": self.host}
+        else:
+            transport_data = {"path": self.path, "host": self.host}
+
+        payload.update(transport_data)
+
     def to_link(self):
         if self.protocol == "shadowsocks":
             return (
                 "ss://"
                 + base64.b64encode(
                     (
                         f"{self.shadowsocks_method}:{self.password}"
                         + f"@{self.address}:{self.port}"
                     ).encode()
                 ).decode()
                 + f"#{urlparse.quote(self.remark)}"
             )
+
         elif self.protocol == "vmess":
             payload = {
                 "add": self.address,
                 "aid": "0",
                 "host": self.host,
                 "id": str(self.uuid),
                 "net": self.transport_type,
                 "path": self.path,
                 "port": self.port,
                 "ps": self.remark,
-                "scy": "auto",
+                "scy": self.vmess_security,
                 "tls": self.tls,
                 "type": self.header_type,
                 "v": "2",
             }
 
             self._apply_tls_settings(payload)
             payload = dict(filter(lambda p: p[1], payload.items()))
             return (
                 "vmess://"
                 + base64.b64encode(
-                    json.dumps(payload, sort_keys=True).encode("utf-8")
+                    json.dumps(payload, sort_keys=True).encode()
                 ).decode()
             )
-        elif self.protocol == "vless":
+
+        elif self.protocol in ["trojan", "vless"]:
             payload = {
                 "security": self.tls,
                 "type": self.transport_type,
-                "host": self.host,
                 "headerType": self.header_type,
             }
-            if self.flow:
+            if self.protocol == "vless" and self.flow:
                 payload.update({"flow": self.flow})
 
-            path_name = "serviceName" if self.transport_type == "grpc" else "path"
-            payload.update({path_name: self.path})
+            self._apply_trojan_vless_transport(payload)
 
             self._apply_tls_settings(payload)
+
             payload = dict(filter(lambda p: p[1], payload.items()))
-            return (
-                "vless://"
-                + f"{self.uuid}@{self.address}:{self.port}?"
-                + urlparse.urlencode(payload)
-                + f"#{(urlparse.quote(self.remark))}"
-            )
-        elif self.protocol == "trojan":
-            payload = {
-                "security": self.tls,
-                "type": self.transport_type,
-                "host": self.host,
-                "headerType": self.header_type,
-            }
-            path_name = "serviceName" if self.transport_type == "grpc" else "path"
-            payload.update({path_name: self.path})
-            self._apply_tls_settings(payload)
-            payload = dict(filter(lambda p: p[1], payload.items()))
-            return (
-                "trojan://"
-                + f"{urlparse.quote(self.password, safe=':')}@{self.address}:{self.port}?"
-                + urlparse.urlencode(payload)
-                + f"#{urlparse.quote(self.remark)}"
-            )
+            if self.protocol == "vless":
+                return (
+                    "vless://"
+                    + f"{self.uuid}@{self.address}:{self.port}?"
+                    + urlparse.urlencode(payload)
+                    + f"#{(urlparse.quote(self.remark))}"
+                )
+            else:
+                return (
+                    "trojan://"
+                    + f"{urlparse.quote(self.password, safe=':')}@{self.address}:{self.port}?"
+                    + urlparse.urlencode(payload)
+                    + f"#{urlparse.quote(self.remark)}"
+                )
```

### Comparing `v2share-0.1.0b1/v2share/singbox.py` & `v2share-0.1.0b2/v2share/singbox.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b1/v2share/xray.py` & `v2share-0.1.0b2/v2share/xray.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 host=data.host,
                 path=data.path,
                 alpn=data.alpn,
                 fp=data.fingerprint,
                 pbk=data.reality_pbk,
                 sid=data.reality_sid,
                 ais=data.allow_insecure,
-                kcp_header_type=data.kcp_header_type,
+                header_type=data.header_type,
                 grpc_multi_mode=data.grpc_multi_mode,
                 dialer_proxy=dialer_proxy,
             )
 
             mux_config = json.loads(self._mux_template)
 
             outbound["mux"] = mux_config
@@ -148,39 +148,23 @@
             "initial_windows_size": 0,
         }
         if service_name:
             grpc_settings["serviceName"] = service_name
         return grpc_settings
 
     @staticmethod
-    def tcp_http_config(path=None, host=None):
-        tcp_settings = {}
-
-        if any((path, host)):
-            tcp_settings = {
-                "header": {
-                    "type": "http",
-                    "request": {
-                        "version": "1.1",
-                        "method": "GET",
-                        "headers": {
-                            "User-Agent": [],
-                            "Accept-Encoding": ["gzip, deflate"],
-                            "Connection": ["keep-alive"],
-                            "Pragma": "no-cache",
-                        },
-                    },
-                }
+    def tcp_http_config(header_type=None):
+        if header_type is None:
+            header_type = "none"
+
+        tcp_settings = {
+            "header": {
+                "type": header_type,
             }
-
-            if path:
-                tcp_settings["header"]["request"]["path"] = [path]
-
-            if host:
-                tcp_settings["header"]["request"]["headers"]["Host"] = [host]
+        }
 
         return tcp_settings
 
     @staticmethod
     def h2_config(path=None, host=None):
         if host is None:
             host = []
@@ -221,16 +205,14 @@
             "writeBufferSize": 2,
         }
 
         if seed:
             kcp_settings["seed"] = seed
         if header_type:
             kcp_settings["header"]["type"] = header_type
-        else:
-            kcp_settings["header"]["type"] = "none"
 
         return kcp_settings
 
     @staticmethod
     def make_stream_settings(
         net="tcp",
         path=None,
@@ -238,38 +220,42 @@
         tls="none",
         sni="",
         fp=None,
         alpn="h2,http/1.1",
         pbk=None,
         sid=None,
         ais=False,
-        kcp_header_type=None,
+        header_type=None,
         grpc_multi_mode=False,
         dialer_proxy=None,
     ):
         stream_settings = {"network": net}
 
         if net == "ws":
             stream_settings["wsSettings"] = XrayConfig.ws_config(path=path, host=host)
         elif net == "grpc":
             stream_settings["grpcSettings"] = XrayConfig.grpc_config(
                 service_name=path, multi_mode=grpc_multi_mode
             )
         elif net == "h2":
-            stream_settings["httpSettings"] = XrayConfig.h2_config(path=path, host=host)
+            stream_settings["httpSettings"] = XrayConfig.h2_config(
+                path=path, host=[host]
+            )
         elif net == "kcp":
             stream_settings["kcpSettings"] = XrayConfig.kcp_config(
-                seed=path, header_type=kcp_header_type
+                seed=path, header_type=header_type
             )
         elif net == "tcp":
             stream_settings["tcpSettings"] = XrayConfig.tcp_http_config(
-                path=path, host=host
+                header_type=header_type
             )
         elif net == "quic":
-            stream_settings["quicSettings"] = XrayConfig.quic_config()
+            stream_settings["quicSettings"] = XrayConfig.quic_config(
+                security=host, key=path, header_type=header_type
+            )
         elif net == "httpupgrade":
             stream_settings["httpupgradeSettings"] = XrayConfig.httpupgrade_config(
                 path=path, host=host
             )
 
         if tls == "tls":
             stream_settings["security"] = "tls"
```

### Comparing `v2share-0.1.0b1/v2share/templates/singbox.json` & `v2share-0.1.0b2/v2share/templates/singbox.json`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b1/v2share/templates/xray.json` & `v2share-0.1.0b2/v2share/templates/xray.json`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b1/.gitignore` & `v2share-0.1.0b2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
+_version.py
```

### Comparing `v2share-0.1.0b1/pyproject.toml` & `v2share-0.1.0b2/pyproject.toml`

 * *Files identical despite different names*

