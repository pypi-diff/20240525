# Comparing `tmp/Cryptem-0.1.1.tar.gz` & `tmp/cryptem-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cryptem-0.1.1.tar", last modified: Mon Jul  3 11:11:55 2023, max compression
+gzip compressed data, was "cryptem-0.1.3.tar", last modified: Sat May 25 17:43:06 2024, max compression
```

## Comparing `Cryptem-0.1.1.tar` & `cryptem-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-07-03 11:11:55.082133 Cryptem-0.1.1/
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-07-03 11:11:55.082133 Cryptem-0.1.1/Cryptem.egg-info/
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6641 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/PKG-INFO
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      199 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/SOURCES.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)        1 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/dependency_links.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       31 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/requires.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       16 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/top_level.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     4437 2023-05-21 10:00:39.000000 Cryptem-0.1.1/Cryptem.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6641 2023-07-03 11:11:55.082133 Cryptem-0.1.1/PKG-INFO
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7940 2023-07-03 11:09:54.000000 Cryptem-0.1.1/cryptem.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:09:46.000000 Cryptem-0.1.1/pyproject.toml
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-07-03 11:11:55.082133 Cryptem-0.1.1/setup.cfg
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1245 2023-05-21 10:24:10.000000 Cryptem-0.1.1/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-25 17:43:06.529060 cryptem-0.1.3/
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-25 17:43:06.525060 cryptem-0.1.3/Cryptem.egg-info/
+-rw-r--r--   0 llearuin  (1000) llearuin  (1000)     6681 2024-05-25 17:43:06.000000 cryptem-0.1.3/Cryptem.egg-info/PKG-INFO
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      199 2024-05-25 17:43:06.000000 cryptem-0.1.3/Cryptem.egg-info/SOURCES.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)        1 2024-05-25 17:43:06.000000 cryptem-0.1.3/Cryptem.egg-info/dependency_links.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       31 2024-05-25 17:43:06.000000 cryptem-0.1.3/Cryptem.egg-info/requires.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       16 2024-05-25 17:43:06.000000 cryptem-0.1.3/Cryptem.egg-info/top_level.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     4437 2023-05-21 10:00:39.000000 cryptem-0.1.3/Cryptem.py
+-rw-r--r--   0 llearuin  (1000) llearuin  (1000)     6681 2024-05-25 17:43:06.529060 cryptem-0.1.3/PKG-INFO
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     8735 2023-12-23 17:54:33.000000 cryptem-0.1.3/cryptem.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:09:46.000000 cryptem-0.1.3/pyproject.toml
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2024-05-25 17:43:06.529060 cryptem-0.1.3/setup.cfg
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1245 2023-05-21 10:24:10.000000 cryptem-0.1.3/setup.py
```

### Comparing `Cryptem-0.1.1/Cryptem.egg-info/PKG-INFO` & `cryptem-0.1.3/Cryptem.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: Cryptem
-Version: 0.1.1
+Version: 0.1.3
 Summary: Cryptographic applications library based on elliptic curve cryptography
 Home-page: https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Author: emendir
-License: UNKNOWN
 Project-URL: Source Code on IPFS, https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Project-URL: Github, https://github.com/emendir/Cryptem-Python
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: eciespy
+Requires-Dist: coincurve
+Requires-Dist: cryptography
 
 An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.  
 Can be used for asymmetric and symmetric cryptography, signature verification, and supports password-like private keys.
 Cryptem uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
 Built on the eciespy, cryptography, coincurve and hashlib modules.
 
 ## Classes `Crypt` and `Encryptor`:
@@ -132,8 +133,7 @@
   Receiver/Verifier:
   
     encryptor = Encryptor(public_key)
     assert(encryptor.verify_signature(data, signature)) # checking the validity of data's signature using the signer's public key
     
     
     
-
```

### Comparing `Cryptem-0.1.1/Cryptem.py` & `cryptem-0.1.3/Cryptem.py`

 * *Files identical despite different names*

### Comparing `Cryptem-0.1.1/PKG-INFO` & `cryptem-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: Cryptem
-Version: 0.1.1
+Version: 0.1.3
 Summary: Cryptographic applications library based on elliptic curve cryptography
 Home-page: https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Author: emendir
-License: UNKNOWN
 Project-URL: Source Code on IPFS, https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Project-URL: Github, https://github.com/emendir/Cryptem-Python
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: eciespy
+Requires-Dist: coincurve
+Requires-Dist: cryptography
 
 An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.  
 Can be used for asymmetric and symmetric cryptography, signature verification, and supports password-like private keys.
 Cryptem uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
 Built on the eciespy, cryptography, coincurve and hashlib modules.
 
 ## Classes `Crypt` and `Encryptor`:
@@ -132,8 +133,7 @@
   Receiver/Verifier:
   
     encryptor = Encryptor(public_key)
     assert(encryptor.verify_signature(data, signature)) # checking the validity of data's signature using the signer's public key
     
     
     
-
```

### Comparing `Cryptem-0.1.1/cryptem.py` & `cryptem-0.1.3/cryptem.py`

 * *Files 21% similar despite different names*

```diff
@@ -87,50 +87,24 @@
         self.__private_key = key
         self.public_key = key.public_key.format(False).hex()
 
     def encrypt(self, data_to_encrypt: bytearray):
         return encrypt(data_to_encrypt, self.public_key)
 
     def decrypt(self, encrypted_data: bytearray):
-        try:
-            if(type(encrypted_data) == bytearray):
-                encrypted_data = bytes(encrypted_data)
-            decrypted_data = ecies.decrypt(
-                self.__private_key.to_hex(), encrypted_data)
-            return decrypted_data
-        except Exception as e:
-            print("Failed at decryption.")
-            print(e)
-            print("----------------------------------------------------")
-            traceback.print_exc()  # printing stack trace
-            print("----------------------------------------------------")
-            print("")
-            # print(encrypted_data)
-            return None
+        return decrypt(encrypted_data, self.__private_key)
 
     def encrypt_file(self, plain_file, encrypted_file):
         return encrypt_file(plain_file, encrypted_file, self.public_key)
 
     def decrypt_file(self, encrypted_file, decrypted_file):
-
-        with open(encrypted_file, 'rb') as file:
-            encrypted_data = file.read()
-        key = encrypted_data[:141]   # extract encrypted key from file
-        encrypted_data = encrypted_data[141:]    # remove encrypted key from file
-
-        # decrypt encrypted key and create file-decrypting Fernet object from it
-        f = Fernet(self.decrypt(key))
-
-        decrypted_data = f.decrypt(encrypted_data)  # decrypt file
-
-        with open(decrypted_file, 'wb') as file:
-            file.write(decrypted_data)
+        return decrypt_file(encrypted_file, decrypted_file, self.__private_key)
 
     def sign(self, data: bytes):
-        return self.__private_key.sign(data)
+        return sign(data, self.__private_key)
 
     def verify_signature(self, data: bytes, signature: bytes):
         return verify_signature(data, self.public_key, signature)
 
     def get_private_key(self):
         """Returns the private key in hexadecimal format."""
         return self.__private_key.to_hex()
@@ -186,14 +160,61 @@
         print("----------------------------------------------------")
         print("")
         print("public key: " + public_key)
         print("")
         return None
 
 
+def decrypt(encrypted_data: bytearray, private_key: bytearray):
+    try:
+        if isinstance(private_key, coincurve.keys.PrivateKey):
+            key = private_key.to_hex()
+        elif isinstance(private_key, bytearray):
+            key = private_key.hex()
+        elif isinstance(private_key, str):
+            key = private_key
+
+        if(type(encrypted_data) == bytearray):
+            encrypted_data = bytes(encrypted_data)
+        decrypted_data = ecies.decrypt(
+            key, encrypted_data)
+        return decrypted_data
+    except Exception as e:
+        print("Failed at decryption.")
+        print(e)
+        print("----------------------------------------------------")
+        traceback.print_exc()  # printing stack trace
+        print("----------------------------------------------------")
+        print("")
+        # print(encrypted_data)
+        return None
+
+
+def sign(data: bytes, private_key: bytearray):
+    if isinstance(private_key, coincurve.keys.PrivateKey):
+        key = private_key
+    elif isinstance(private_key, bytearray):
+        key = coincurve.PrivateKey.from_hex(private_key.hex())
+    elif isinstance(private_key, str):
+        key = coincurve.PrivateKey.from_hex(private_key)
+    return key.sign(data)
+
+
+def verify_signature(data: bytes, public_key: bytes, signature: bytes):
+    if isinstance(public_key, str):
+        public_key = bytes(bytearray.fromhex(public_key))
+    elif isinstance(data, bytearray):
+        public_key = bytes(public_key)
+    if isinstance(data, bytearray):
+        data = bytes(data)
+    if isinstance(signature, bytearray):
+        signature = bytes(signature)
+    return coincurve.verify_signature(signature, data, public_key)
+
+
 def encrypt_file(plain_file, encrypted_file, public_key):
     """
     encrypt a file.
     Parameters:
         plain_file: the path of the file to encrypt
         encrypted_file: where the encrypted file should be saved
     """
@@ -207,17 +228,21 @@
     key_encrypted = encrypt(key, public_key)
 
     encrypted_data = key_encrypted + encrypted_data
     with open(encrypted_file, 'wb') as file:
         file.write(encrypted_data)
 
 
-def verify_signature(data: bytes, public_key: bytes, signature: bytes):
-    if isinstance(public_key, str):
-        public_key = bytes(bytearray.fromhex(public_key))
-    elif isinstance(data, bytearray):
-        public_key = bytes(public_key)
-    if isinstance(data, bytearray):
-        data = bytes(data)
-    if isinstance(signature, bytearray):
-        signature = bytes(signature)
-    return coincurve.verify_signature(signature, data, public_key)
+def decrypt_file(encrypted_file, decrypted_file, private_key: bytearray):
+
+    with open(encrypted_file, 'rb') as file:
+        encrypted_data = file.read()
+    key = encrypted_data[:141]   # extract encrypted key from file
+    encrypted_data = encrypted_data[141:]    # remove encrypted key from file
+
+    # decrypt encrypted key and create file-decrypting Fernet object from it
+    f = Fernet(decrypt(key, private_key))
+
+    decrypted_data = f.decrypt(encrypted_data)  # decrypt file
+
+    with open(decrypted_file, 'wb') as file:
+        file.write(decrypted_data)
```

### Comparing `Cryptem-0.1.1/setup.py` & `cryptem-0.1.3/setup.py`

 * *Files identical despite different names*

