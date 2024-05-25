# Comparing `tmp/aproxyrelay-1.90.1rc7688073331.tar.gz` & `tmp/aproxyrelay-1.97.1rc7688272509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aproxyrelay-1.90.1rc7688073331.tar", last modified: Sun Jan 28 20:01:52 2024, max compression
+gzip compressed data, was "aproxyrelay-1.97.1rc7688272509.tar", last modified: Sun Jan 28 20:36:43 2024, max compression
```

## Comparing `aproxyrelay-1.90.1rc7688073331.tar` & `aproxyrelay-1.97.1rc7688272509.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:01:52.987570 aproxyrelay-1.90.1rc7688073331/
--rw-rw-r--   0 root         (0) root         (0)    34523 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       34 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6858 2024-01-28 20:01:52.987570 aproxyrelay-1.90.1rc7688073331/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6015 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:01:52.983570 aproxyrelay-1.90.1rc7688073331/aproxyrelay/
--rw-rw-r--   0 root         (0) root         (0)     3888 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   141072 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/agents.py
--rw-rw-r--   0 root         (0) root         (0)     6900 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/core.py
--rw-rw-r--   0 root         (0) root         (0)     4462 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:01:52.987570 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/
--rw-rw-r--   0 root         (0) root         (0)     2716 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2889 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/core.py
--rw-rw-r--   0 root         (0) root         (0)     2002 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser.py
--rw-rw-r--   0 root         (0) root         (0)     3203 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_freeproxylist.py
--rw-rw-r--   0 root         (0) root         (0)     2054 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_gg_my_dev_app.py
--rw-rw-r--   0 root         (0) root         (0)     2770 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_lumiproxy.py
--rw-rw-r--   0 root         (0) root         (0)     2542 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_proxyscrape.py
--rw-rw-r--   0 root         (0) root         (0)     3174 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_socks_proxy.py
--rw-rw-r--   0 root         (0) root         (0)     4517 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_spys_de.py
--rw-rw-r--   0 root         (0) root         (0)     4521 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_spys_nl.py
--rw-rw-r--   0 root         (0) root         (0)     4523 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_spys_us.py
--rw-rw-r--   0 root         (0) root         (0)     3142 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_ssl_proxies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:01:52.987570 aproxyrelay-1.90.1rc7688073331/aproxyrelay.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6858 2024-01-28 20:01:52.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      859 2024-01-28 20:01:52.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-28 20:01:52.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-01-28 20:01:52.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      142 2024-01-28 20:01:52.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-01-28 20:01:52.000000 aproxyrelay-1.90.1rc7688073331/aproxyrelay.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     3110 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-28 20:01:52.991570 aproxyrelay-1.90.1rc7688073331/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1177 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:01:52.987570 aproxyrelay-1.90.1rc7688073331/tests/
--rw-rw-r--   0 root         (0) root         (0)      259 2024-01-28 20:01:27.000000 aproxyrelay-1.90.1rc7688073331/tests/test_class_initialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:36:43.910564 aproxyrelay-1.97.1rc7688272509/
+-rw-rw-r--   0 root         (0) root         (0)    34523 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       34 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7237 2024-01-28 20:36:43.910564 aproxyrelay-1.97.1rc7688272509/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6393 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:36:43.906564 aproxyrelay-1.97.1rc7688272509/aproxyrelay/
+-rw-rw-r--   0 root         (0) root         (0)     3888 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)   141072 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/agents.py
+-rw-rw-r--   0 root         (0) root         (0)     6900 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/core.py
+-rw-rw-r--   0 root         (0) root         (0)     4462 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:36:43.910564 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/
+-rw-rw-r--   0 root         (0) root         (0)     2716 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2889 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/core.py
+-rw-rw-r--   0 root         (0) root         (0)     2002 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser.py
+-rw-rw-r--   0 root         (0) root         (0)     3203 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_freeproxylist.py
+-rw-rw-r--   0 root         (0) root         (0)     2054 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_gg_my_dev_app.py
+-rw-rw-r--   0 root         (0) root         (0)     2770 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_lumiproxy.py
+-rw-rw-r--   0 root         (0) root         (0)     2542 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_proxyscrape.py
+-rw-rw-r--   0 root         (0) root         (0)     3174 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_socks_proxy.py
+-rw-rw-r--   0 root         (0) root         (0)     4517 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_spys_de.py
+-rw-rw-r--   0 root         (0) root         (0)     4521 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_spys_nl.py
+-rw-rw-r--   0 root         (0) root         (0)     4523 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_spys_us.py
+-rw-rw-r--   0 root         (0) root         (0)     3142 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_ssl_proxies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:36:43.910564 aproxyrelay-1.97.1rc7688272509/aproxyrelay.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7237 2024-01-28 20:36:43.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      859 2024-01-28 20:36:43.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-28 20:36:43.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-01-28 20:36:43.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      142 2024-01-28 20:36:43.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-01-28 20:36:43.000000 aproxyrelay-1.97.1rc7688272509/aproxyrelay.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     3110 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-28 20:36:43.910564 aproxyrelay-1.97.1rc7688272509/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1177 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 20:36:43.910564 aproxyrelay-1.97.1rc7688272509/tests/
+-rw-rw-r--   0 root         (0) root         (0)      259 2024-01-28 20:36:16.000000 aproxyrelay-1.97.1rc7688272509/tests/test_class_initialization.py
```

### Comparing `aproxyrelay-1.90.1rc7688073331/LICENSE` & `aproxyrelay-1.97.1rc7688272509/LICENSE`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/PKG-INFO` & `aproxyrelay-1.97.1rc7688272509/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aproxyrelay
-Version: 1.90.1rc7688073331
+Version: 1.97.1rc7688272509
 Summary: A Proxy Relay, forwarding requests through different IP.
 Home-page: https://github.com/my-dev-app/proxy-relay
 Author: undeƒined
 Author-email: my-dev.app@domainsbyproxy.com
 License: GNU AGPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,32 +31,25 @@
  #######    #       #####  #    #   ##     #      #   #   #      #      ######   #   
  #     #    #       #   #  #    #  #  #    #      #    #  #      #      #    #   #   
  #     #    #       #    #  ####  #    #   #      #     # ###### ###### #    #   #   
                                                                                      
 By undeƒined
 -------------------------------------
 ```
+[![PyPI version](https://badge.fury.io/py/aproxyrelay.svg)](https://badge.fury.io/py/aproxyrelay)
+[![A Proxy Relay build](https://github.com/my-dev-app/proxy-relay/actions/workflows/entrypoint.yaml/badge.svg?branch=development)](https://github.com/my-dev-app/proxy-relay/actions/workflows/entrypoint.yaml)
+
 # AProxyRelay: An Async Request Library with Proxy Rotation
 
 AProxyRelay is an asynchronous request library designed for easy data retrieval using various proxy servers. It seamlessly handles proxy rotation, preserves data that fails to be requested, and simplifies API scraping. The library is written in `Python 3.12.1` but is compatible with projects utilizing `Python 3.11.2`.
 
 In addition, tested proxies will be shared with other people using this library. The more this library is utilized, the bigger the pool of available proxies.
 
 Our scraper, used to obtain proxies, is highly modular and plug-and-play, making it easy to contribute to.
 
-## Compiling to package
-To compile the library into a package, use the following command after installing `requirements.txt`:
-
-```sh
-python setup.py sdist bdist_wheel
-```
-
-This will generate the package in the `dist` folder.
-Note: A version can be set with the environment variable `CUSTOM_VERSION`
-
 ## Usage
 AProxyRelay streamlines the process of making asynchronous requests with proxy servers. It offers the following features:
 - Asynchronously fetches lists of free proxies from various sources based on the provided zone
 - Tests and shares proxies with other users of the library
 - Identifies and discards bad proxies, preserving data for failed target requests
 - Bypasses API limiters in an asynchronous manner (for educational purpose)
 
@@ -84,14 +77,19 @@
 # Fetch data
 data = proxy_relay.start()
 
 # Result Queue
 print(data.qsize())
 ```
 
+## A Proxy Relay: Installation
+Simply run
+
+    pip install aproxyrelay
+
 ## A Proxy Relay: Local Development
 To install all library dependencies for local development, excluding the core code available locally, use the following command within a virtual environment:
 
     pip install -e .[dev]
 
 This command installs dependencies and removes the core code of AProxyRelay from the virtual environment.
 
@@ -157,7 +155,17 @@
         queue.put(data)
         ```
 4. ### Congratulations
     - If done correctly, congratulations! You've successfully created a new proxy parser for this library.
     - Add the targeted link and your scraper to `scrapers/__init__.py`.
 
 Feel free to contribute, share your improvements, and expand the library's capabilities. Your efforts contribute to a growing pool of available proxies for the AProxyRelay community.
+
+## Compiling to package
+To compile the library into a package, use the following command after installing `requirements.txt`:
+
+```sh
+python setup.py sdist bdist_wheel
+```
+
+This will generate the package in the `dist` folder.
+Note: A version can be set with the environment variable `CUSTOM_VERSION`
```

### Comparing `aproxyrelay-1.90.1rc7688073331/README.md` & `aproxyrelay-1.97.1rc7688272509/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,336 +41,360 @@
 00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000290: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000002a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000002b0: 2020 2020 2020 2020 200a 4279 2075 6e64           .By und
 000002c0: 65c6 9269 6e65 640a 2d2d 2d2d 2d2d 2d2d  e..ined.--------
 000002d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000002e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 6060  -------------.``
-000002f0: 600a 2320 4150 726f 7879 5265 6c61 793a  `.# AProxyRelay:
-00000300: 2041 6e20 4173 796e 6320 5265 7175 6573   An Async Reques
-00000310: 7420 4c69 6272 6172 7920 7769 7468 2050  t Library with P
-00000320: 726f 7879 2052 6f74 6174 696f 6e0a 0a41  roxy Rotation..A
-00000330: 5072 6f78 7952 656c 6179 2069 7320 616e  ProxyRelay is an
-00000340: 2061 7379 6e63 6872 6f6e 6f75 7320 7265   asynchronous re
-00000350: 7175 6573 7420 6c69 6272 6172 7920 6465  quest library de
-00000360: 7369 676e 6564 2066 6f72 2065 6173 7920  signed for easy 
-00000370: 6461 7461 2072 6574 7269 6576 616c 2075  data retrieval u
-00000380: 7369 6e67 2076 6172 696f 7573 2070 726f  sing various pro
-00000390: 7879 2073 6572 7665 7273 2e20 4974 2073  xy servers. It s
-000003a0: 6561 6d6c 6573 736c 7920 6861 6e64 6c65  eamlessly handle
-000003b0: 7320 7072 6f78 7920 726f 7461 7469 6f6e  s proxy rotation
-000003c0: 2c20 7072 6573 6572 7665 7320 6461 7461  , preserves data
-000003d0: 2074 6861 7420 6661 696c 7320 746f 2062   that fails to b
-000003e0: 6520 7265 7175 6573 7465 642c 2061 6e64  e requested, and
-000003f0: 2073 696d 706c 6966 6965 7320 4150 4920   simplifies API 
-00000400: 7363 7261 7069 6e67 2e20 5468 6520 6c69  scraping. The li
-00000410: 6272 6172 7920 6973 2077 7269 7474 656e  brary is written
-00000420: 2069 6e20 6050 7974 686f 6e20 332e 3132   in `Python 3.12
-00000430: 2e31 6020 6275 7420 6973 2063 6f6d 7061  .1` but is compa
-00000440: 7469 626c 6520 7769 7468 2070 726f 6a65  tible with proje
-00000450: 6374 7320 7574 696c 697a 696e 6720 6050  cts utilizing `P
-00000460: 7974 686f 6e20 332e 3131 2e32 602e 0a0a  ython 3.11.2`...
-00000470: 496e 2061 6464 6974 696f 6e2c 2074 6573  In addition, tes
-00000480: 7465 6420 7072 6f78 6965 7320 7769 6c6c  ted proxies will
-00000490: 2062 6520 7368 6172 6564 2077 6974 6820   be shared with 
-000004a0: 6f74 6865 7220 7065 6f70 6c65 2075 7369  other people usi
-000004b0: 6e67 2074 6869 7320 6c69 6272 6172 792e  ng this library.
-000004c0: 2054 6865 206d 6f72 6520 7468 6973 206c   The more this l
-000004d0: 6962 7261 7279 2069 7320 7574 696c 697a  ibrary is utiliz
-000004e0: 6564 2c20 7468 6520 6269 6767 6572 2074  ed, the bigger t
-000004f0: 6865 2070 6f6f 6c20 6f66 2061 7661 696c  he pool of avail
-00000500: 6162 6c65 2070 726f 7869 6573 2e0a 0a4f  able proxies...O
-00000510: 7572 2073 6372 6170 6572 2c20 7573 6564  ur scraper, used
-00000520: 2074 6f20 6f62 7461 696e 2070 726f 7869   to obtain proxi
-00000530: 6573 2c20 6973 2068 6967 686c 7920 6d6f  es, is highly mo
-00000540: 6475 6c61 7220 616e 6420 706c 7567 2d61  dular and plug-a
-00000550: 6e64 2d70 6c61 792c 206d 616b 696e 6720  nd-play, making 
-00000560: 6974 2065 6173 7920 746f 2063 6f6e 7472  it easy to contr
-00000570: 6962 7574 6520 746f 2e0a 0a23 2320 436f  ibute to...## Co
-00000580: 6d70 696c 696e 6720 746f 2070 6163 6b61  mpiling to packa
-00000590: 6765 0a54 6f20 636f 6d70 696c 6520 7468  ge.To compile th
-000005a0: 6520 6c69 6272 6172 7920 696e 746f 2061  e library into a
-000005b0: 2070 6163 6b61 6765 2c20 7573 6520 7468   package, use th
-000005c0: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
-000005d0: 616e 6420 6166 7465 7220 696e 7374 616c  and after instal
-000005e0: 6c69 6e67 2060 7265 7175 6972 656d 656e  ling `requiremen
-000005f0: 7473 2e74 7874 603a 0a0a 6060 6073 680a  ts.txt`:..```sh.
-00000600: 7079 7468 6f6e 2073 6574 7570 2e70 7920  python setup.py 
-00000610: 7364 6973 7420 6264 6973 745f 7768 6565  sdist bdist_whee
-00000620: 6c0a 6060 600a 0a54 6869 7320 7769 6c6c  l.```..This will
-00000630: 2067 656e 6572 6174 6520 7468 6520 7061   generate the pa
-00000640: 636b 6167 6520 696e 2074 6865 2060 6469  ckage in the `di
-00000650: 7374 6020 666f 6c64 6572 2e0a 4e6f 7465  st` folder..Note
-00000660: 3a20 4120 7665 7273 696f 6e20 6361 6e20  : A version can 
-00000670: 6265 2073 6574 2077 6974 6820 7468 6520  be set with the 
-00000680: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00000690: 6162 6c65 2060 4355 5354 4f4d 5f56 4552  able `CUSTOM_VER
-000006a0: 5349 4f4e 600a 0a23 2320 5573 6167 650a  SION`..## Usage.
-000006b0: 4150 726f 7879 5265 6c61 7920 7374 7265  AProxyRelay stre
-000006c0: 616d 6c69 6e65 7320 7468 6520 7072 6f63  amlines the proc
-000006d0: 6573 7320 6f66 206d 616b 696e 6720 6173  ess of making as
-000006e0: 796e 6368 726f 6e6f 7573 2072 6571 7565  ynchronous reque
-000006f0: 7374 7320 7769 7468 2070 726f 7879 2073  sts with proxy s
-00000700: 6572 7665 7273 2e20 4974 206f 6666 6572  ervers. It offer
-00000710: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
-00000720: 6665 6174 7572 6573 3a0a 2d20 4173 796e  features:.- Asyn
-00000730: 6368 726f 6e6f 7573 6c79 2066 6574 6368  chronously fetch
-00000740: 6573 206c 6973 7473 206f 6620 6672 6565  es lists of free
-00000750: 2070 726f 7869 6573 2066 726f 6d20 7661   proxies from va
-00000760: 7269 6f75 7320 736f 7572 6365 7320 6261  rious sources ba
-00000770: 7365 6420 6f6e 2074 6865 2070 726f 7669  sed on the provi
-00000780: 6465 6420 7a6f 6e65 0a2d 2054 6573 7473  ded zone.- Tests
-00000790: 2061 6e64 2073 6861 7265 7320 7072 6f78   and shares prox
-000007a0: 6965 7320 7769 7468 206f 7468 6572 2075  ies with other u
-000007b0: 7365 7273 206f 6620 7468 6520 6c69 6272  sers of the libr
-000007c0: 6172 790a 2d20 4964 656e 7469 6669 6573  ary.- Identifies
-000007d0: 2061 6e64 2064 6973 6361 7264 7320 6261   and discards ba
-000007e0: 6420 7072 6f78 6965 732c 2070 7265 7365  d proxies, prese
-000007f0: 7276 696e 6720 6461 7461 2066 6f72 2066  rving data for f
-00000800: 6169 6c65 6420 7461 7267 6574 2072 6571  ailed target req
-00000810: 7565 7374 730a 2d20 4279 7061 7373 6573  uests.- Bypasses
-00000820: 2041 5049 206c 696d 6974 6572 7320 696e   API limiters in
-00000830: 2061 6e20 6173 796e 6368 726f 6e6f 7573   an asynchronous
-00000840: 206d 616e 6e65 7220 2866 6f72 2065 6475   manner (for edu
-00000850: 6361 7469 6f6e 616c 2070 7572 706f 7365  cational purpose
-00000860: 290a 0a23 2323 2045 7861 6d70 6c65 0a60  )..### Example.`
-00000870: 6060 7079 0a66 726f 6d20 6170 726f 7879  ``py.from aproxy
-00000880: 7265 6c61 7920 696d 706f 7274 2041 5072  relay import APr
-00000890: 6f78 7952 656c 6179 0a0a 7461 7267 6574  oxyRelay..target
-000008a0: 7320 3d20 5b0a 2020 2020 2768 7474 7073  s = [.    'https
-000008b0: 3a2f 2f73 6f6d 652d 7765 6273 6974 652e  ://some-website.
-000008c0: 636f 6d2f 6170 692f 6170 703f 6964 3d31  com/api/app?id=1
-000008d0: 3535 3133 3630 272c 0a20 2020 2027 6874  551360',.    'ht
-000008e0: 7470 733a 2f2f 736f 6d65 2d77 6562 7369  tps://some-websi
-000008f0: 7465 2e63 6f6d 2f61 7069 2f61 7070 3f69  te.com/api/app?i
-00000900: 643d 3230 3732 3435 3027 2c0a 2020 2020  d=2072450',.    
-00000910: 2768 7474 7073 3a2f 2f73 6f6d 652d 7765  'https://some-we
-00000920: 6273 6974 652e 636f 6d2f 6170 692f 6170  bsite.com/api/ap
-00000930: 703f 6964 3d31 3932 3433 3630 272c 0a20  p?id=1924360',. 
-00000940: 2020 2027 6874 7470 733a 2f2f 736f 6d65     'https://some
-00000950: 2d77 6562 7369 7465 2e63 6f6d 2f61 7069  -website.com/api
-00000960: 2f61 7070 3f69 643d 3137 3037 3837 3027  /app?id=1707870'
-00000970: 2c0a 2020 2020 2768 7474 7073 3a2f 2f73  ,.    'https://s
-00000980: 6f6d 652d 7765 6273 6974 652e 636f 6d2f  ome-website.com/
-00000990: 6170 692f 6170 703f 6964 3d31 3833 3938  api/app?id=18398
-000009a0: 3830 272c 0a5d 0a0a 2320 496e 6974 6961  80',.]..# Initia
-000009b0: 6c69 7a65 2070 726f 7879 2072 656c 6179  lize proxy relay
-000009c0: 0a70 726f 7879 5f72 656c 6179 203d 2041  .proxy_relay = A
-000009d0: 5072 6f78 7952 656c 6179 280a 2020 2020  ProxyRelay(.    
-000009e0: 7461 7267 6574 733d 7461 7267 6574 732c  targets=targets,
-000009f0: 0a20 2020 2074 696d 656f 7574 3d35 2c0a  .    timeout=5,.
-00000a00: 2020 2020 7465 7374 5f70 726f 7879 3d54      test_proxy=T
-00000a10: 7275 652c 0a20 2020 2074 6573 745f 7469  rue,.    test_ti
-00000a20: 6d65 6f75 743d 3130 2c0a 2020 2020 7a6f  meout=10,.    zo
-00000a30: 6e65 3d27 7573 272c 0a29 0a0a 2320 4665  ne='us',.)..# Fe
-00000a40: 7463 6820 6461 7461 0a64 6174 6120 3d20  tch data.data = 
-00000a50: 7072 6f78 795f 7265 6c61 792e 7374 6172  proxy_relay.star
-00000a60: 7428 290a 0a23 2052 6573 756c 7420 5175  t()..# Result Qu
-00000a70: 6575 650a 7072 696e 7428 6461 7461 2e71  eue.print(data.q
-00000a80: 7369 7a65 2829 290a 6060 600a 0a23 2320  size()).```..## 
-00000a90: 4120 5072 6f78 7920 5265 6c61 793a 204c  A Proxy Relay: L
-00000aa0: 6f63 616c 2044 6576 656c 6f70 6d65 6e74  ocal Development
-00000ab0: 0a54 6f20 696e 7374 616c 6c20 616c 6c20  .To install all 
-00000ac0: 6c69 6272 6172 7920 6465 7065 6e64 656e  library dependen
-00000ad0: 6369 6573 2066 6f72 206c 6f63 616c 2064  cies for local d
-00000ae0: 6576 656c 6f70 6d65 6e74 2c20 6578 636c  evelopment, excl
-00000af0: 7564 696e 6720 7468 6520 636f 7265 2063  uding the core c
-00000b00: 6f64 6520 6176 6169 6c61 626c 6520 6c6f  ode available lo
-00000b10: 6361 6c6c 792c 2075 7365 2074 6865 2066  cally, use the f
-00000b20: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00000b30: 2077 6974 6869 6e20 6120 7669 7274 7561   within a virtua
-00000b40: 6c20 656e 7669 726f 6e6d 656e 743a 0a0a  l environment:..
-00000b50: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
-00000b60: 2d65 202e 5b64 6576 5d0a 0a54 6869 7320  -e .[dev]..This 
-00000b70: 636f 6d6d 616e 6420 696e 7374 616c 6c73  command installs
-00000b80: 2064 6570 656e 6465 6e63 6965 7320 616e   dependencies an
-00000b90: 6420 7265 6d6f 7665 7320 7468 6520 636f  d removes the co
-00000ba0: 7265 2063 6f64 6520 6f66 2041 5072 6f78  re code of AProx
-00000bb0: 7952 656c 6179 2066 726f 6d20 7468 6520  yRelay from the 
-00000bc0: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
-00000bd0: 656e 742e 0a0a 0a23 2043 6f6e 7472 6962  ent....# Contrib
-00000be0: 7574 6520 746f 2041 5072 6f78 7952 656c  ute to AProxyRel
-00000bf0: 6179 0a0a 4150 726f 7879 5265 6c61 7920  ay..AProxyRelay 
-00000c00: 656e 636f 7572 6167 6573 2063 6f6e 7472  encourages contr
-00000c10: 6962 7574 696f 6e73 2074 6f20 656e 6861  ibutions to enha
-00000c20: 6e63 6520 6974 7320 6361 7061 6269 6c69  nce its capabili
-00000c30: 7469 6573 2062 7920 616c 6c6f 7769 6e67  ties by allowing
-00000c40: 2075 7365 7273 2074 6f20 6372 6561 7465   users to create
-00000c50: 2063 7573 746f 6d20 7363 7261 7065 7273   custom scrapers
-00000c60: 2e20 5468 6573 6520 7363 7261 7065 7273  . These scrapers
-00000c70: 2061 7265 2064 6573 6967 6e65 6420 746f   are designed to
-00000c80: 2066 6574 6368 2070 726f 7879 2064 6174   fetch proxy dat
-00000c90: 6120 6672 6f6d 2064 6966 6665 7265 6e74  a from different
-00000ca0: 2073 6f75 7263 6573 2e20 5468 6520 7072   sources. The pr
-00000cb0: 6f63 6573 7320 6973 2073 7472 6169 6768  ocess is straigh
-00000cc0: 7466 6f72 7761 7264 2c20 616e 6420 6865  tforward, and he
-00000cd0: 7265 2773 2061 2067 7569 6465 2074 6f20  re's a guide to 
-00000ce0: 6865 6c70 2079 6f75 2067 6574 2073 7461  help you get sta
-00000cf0: 7274 6564 3a0a 0a23 2320 5363 7261 7065  rted:..## Scrape
-00000d00: 7220 5374 7275 6374 7572 650a 0a41 5072  r Structure..APr
-00000d10: 6f78 7952 656c 6179 2069 6e63 6c75 6465  oxyRelay include
-00000d20: 7320 6120 6465 6469 6361 7465 6420 666f  s a dedicated fo
-00000d30: 6c64 6572 206e 616d 6564 2060 7363 7261  lder named `scra
-00000d40: 7065 7273 602e 2057 6974 6869 6e20 7468  pers`. Within th
-00000d50: 6973 2066 6f6c 6465 722c 2065 6163 6820  is folder, each 
-00000d60: 7363 7261 7065 722c 2070 7265 6669 7865  scraper, prefixe
-00000d70: 6420 7769 7468 2060 7061 7273 6572 5f60  d with `parser_`
-00000d80: 2c20 696e 6865 7269 7473 2066 726f 6d20  , inherits from 
-00000d90: 7468 6520 6070 6172 7365 722e 7079 6020  the `parser.py` 
-00000da0: 6669 6c65 2e20 546f 2070 726f 7669 6465  file. To provide
-00000db0: 2079 6f75 2077 6974 6820 6120 6765 6e65   you with a gene
-00000dc0: 7261 6c20 756e 6465 7273 7461 6e64 696e  ral understandin
-00000dd0: 672c 2068 6572 6527 7320 616e 2065 7861  g, here's an exa
-00000de0: 6d70 6c65 206f 6620 7468 6520 604d 6169  mple of the `Mai
-00000df0: 6e53 6372 6170 6572 6020 636c 6173 733a  nScraper` class:
-00000e00: 0a0a 6060 6070 790a 6672 6f6d 2071 7565  ..```py.from que
-00000e10: 7565 2069 6d70 6f72 7420 5175 6575 650a  ue import Queue.
-00000e20: 0a66 726f 6d20 2e63 6f72 6520 696d 706f  .from .core impo
-00000e30: 7274 2053 6372 6170 6572 436f 7265 0a0a  rt ScraperCore..
-00000e40: 0a63 6c61 7373 204d 6169 6e53 6372 6170  .class MainScrap
-00000e50: 6572 2853 6372 6170 6572 436f 7265 293a  er(ScraperCore):
-00000e60: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00000e70: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
-00000e80: 0a20 2020 2020 2020 2053 6372 6170 6572  .        Scraper
-00000e90: 436f 7265 2e5f 5f69 6e69 745f 5f28 7365  Core.__init__(se
-00000ea0: 6c66 290a 0a20 2020 2040 636c 6173 736d  lf)..    @classm
-00000eb0: 6574 686f 640a 2020 2020 6173 796e 6320  ethod.    async 
-00000ec0: 6465 6620 666f 726d 6174 5f75 726c 2863  def format_url(c
-00000ed0: 6c73 2c20 7572 6c2c 202a 6172 6773 2c20  ls, url, *args, 
-00000ee0: 2a2a 6b77 6172 6773 2920 2d3e 2073 7472  **kwargs) -> str
-00000ef0: 3a0a 2020 2020 2020 2020 2222 2246 6f72  :.        """For
-00000f00: 6d61 7473 2055 524c 2062 6566 6f72 6520  mats URL before 
-00000f10: 7363 7261 7069 6e67 2c20 6c65 7420 7573  scraping, let us
-00000f20: 2061 646a 7573 7420 7175 6572 7920 7061   adjust query pa
-00000f30: 7261 6d65 7465 7273 2066 6f72 2065 6163  rameters for eac
-00000f40: 6820 7061 7273 6572 2222 220a 2020 2020  h parser""".    
-00000f50: 2020 2020 6e65 775f 7572 6c20 3d20 6627      new_url = f'
-00000f60: 7b75 726c 7d27 0a20 2020 2020 2020 2072  {url}'.        r
-00000f70: 6574 7572 6e20 6e65 775f 7572 6c0a 0a20  eturn new_url.. 
-00000f80: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00000f90: 2020 2020 6173 796e 6320 6465 6620 666f      async def fo
-00000fa0: 726d 6174 5f72 6177 2863 6c73 2c20 6874  rmat_raw(cls, ht
-00000fb0: 6d6c 3a20 7374 7229 3a0a 2020 2020 2020  ml: str):.      
-00000fc0: 2020 2222 2250 6172 7365 2074 6578 742f    """Parse text/
-00000fd0: 6874 6d6c 2070 6167 6573 2c20 6375 7374  html pages, cust
-00000fe0: 6f6d 697a 6564 206d 6574 686f 6420 666f  omized method fo
-00000ff0: 7220 7468 6520 7061 7273 6572 206f 6620  r the parser of 
-00001000: 7468 6973 2077 6562 7369 7465 2222 220a  this website""".
-00001010: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-00001020: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-00001030: 7228 2746 6f72 6d61 7420 7261 7720 7061  r('Format raw pa
-00001040: 7273 6572 2068 6173 206e 6f74 2062 6565  rser has not bee
-00001050: 6e20 696d 706c 656d 656e 7465 6420 7965  n implemented ye
-00001060: 7427 290a 0a20 2020 2040 636c 6173 736d  t')..    @classm
-00001070: 6574 686f 640a 2020 2020 6173 796e 6320  ethod.    async 
-00001080: 6465 6620 666f 726d 6174 5f64 6174 6128  def format_data(
-00001090: 636c 732c 2064 6174 613a 2064 6963 742c  cls, data: dict,
-000010a0: 2071 7565 7565 3a20 5175 6575 6529 3a0a   queue: Queue):.
-000010b0: 2020 2020 2020 2020 2222 2244 6174 6120          """Data 
-000010c0: 666f 726d 6174 7465 722c 2066 6f72 6d61  formatter, forma
-000010d0: 7473 2064 6174 6120 616e 6420 7265 7475  ts data and retu
-000010e0: 726e 7320 6973 2062 6163 6b20 696e 2074  rns is back in t
-000010f0: 6865 2070 726f 6365 7373 2051 7565 7565  he process Queue
-00001100: 2222 220a 2020 2020 2020 2020 7261 6973  """.        rais
-00001110: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
-00001120: 4572 726f 7228 2746 6f72 6d20 6461 7461  Error('Form data
-00001130: 2070 6172 7365 7220 6861 7320 6e6f 7420   parser has not 
-00001140: 6265 656e 2069 6d70 6c65 6d65 6e74 6564  been implemented
-00001150: 2079 6574 2729 0a60 6060 0a0a 2323 2043   yet').```..## C
-00001160: 7265 6174 696e 6720 796f 7572 206f 776e  reating your own
-00001170: 2050 726f 7879 2053 6372 6170 6572 0a0a   Proxy Scraper..
-00001180: 546f 2063 6f6e 7472 6962 7574 6520 796f  To contribute yo
-00001190: 7572 206f 776e 2070 726f 7879 2073 6372  ur own proxy scr
-000011a0: 6170 6572 2c20 666f 6c6c 6f77 2074 6865  aper, follow the
-000011b0: 7365 2073 7465 7073 3a0a 0a31 2e20 2323  se steps:..1. ##
-000011c0: 2320 4372 6561 7465 2061 206e 6577 2070  # Create a new p
-000011d0: 6172 7365 7220 636c 6173 7320 696e 7369  arser class insi
-000011e0: 6465 2074 6865 2073 6372 6170 6572 7320  de the scrapers 
-000011f0: 666f 6c64 6572 0a20 2020 202d 2049 6e68  folder.    - Inh
-00001200: 6572 6974 2066 726f 6d20 7468 6520 604d  erit from the `M
-00001210: 6169 6e53 6372 6170 6572 602e 0a20 2020  ainScraper`..   
-00001220: 202d 204f 7665 7277 7269 7465 2074 6865   - Overwrite the
-00001230: 206e 6563 6573 7361 7279 206d 6574 686f   necessary metho
-00001240: 6473 2072 6571 7569 7265 6420 666f 7220  ds required for 
-00001250: 7363 7261 7069 6e67 2061 6464 6974 696f  scraping additio
-00001260: 6e61 6c20 7072 6f78 7920 7365 7276 6572  nal proxy server
-00001270: 732e 0a32 2e20 2323 2320 4d65 7468 6f64  s..2. ### Method
-00001280: 7320 746f 204f 7665 7277 7269 7465 3a0a  s to Overwrite:.
-00001290: 2020 2020 2d20 6066 6f72 6d61 745f 7572      - `format_ur
-000012a0: 6c60 3a20 4d61 6e69 7075 6c61 7465 2074  l`: Manipulate t
-000012b0: 6865 2070 726f 7879 206c 6973 7420 7265  he proxy list re
-000012c0: 7175 6573 7420 5552 4c20 6265 666f 7265  quest URL before
-000012d0: 206d 616b 696e 6720 6120 7265 7175 6573   making a reques
-000012e0: 742c 2065 6e61 626c 696e 6720 6164 6a75  t, enabling adju
-000012f0: 7374 6d65 6e74 206f 6620 7661 7269 6f75  stment of variou
-00001300: 7320 7175 6572 7920 7061 7261 6d65 7465  s query paramete
-00001310: 7273 2e0a 2020 2020 2d20 6066 6f72 6d61  rs..    - `forma
-00001320: 745f 7261 7760 3a20 5768 656e 2074 6865  t_raw`: When the
-00001330: 2064 6174 6120 6f62 7461 696e 6564 2066   data obtained f
-00001340: 726f 6d20 7468 6520 6c69 6e6b 2069 7320  rom the link is 
-00001350: 6074 7874 2f68 746d 6c60 2c20 7468 6973  `txt/html`, this
-00001360: 206d 6574 686f 6420 7368 6f75 6c64 2073   method should s
-00001370: 6372 6170 6520 7468 6520 6461 7461 2061  crape the data a
-00001380: 6e64 2066 6f72 6d61 7420 6974 2069 6e74  nd format it int
-00001390: 6f20 776f 726b 6162 6c65 2064 6174 612e  o workable data.
-000013a0: 0a20 2020 202d 2060 666f 726d 6174 5f64  .    - `format_d
-000013b0: 6174 6160 3a20 5468 6973 206d 6574 686f  ata`: This metho
-000013c0: 6420 6973 2074 7269 6767 6572 6564 2077  d is triggered w
-000013d0: 6865 6e20 7468 6520 6361 6c6c 2074 6f20  hen the call to 
-000013e0: 7468 6520 7072 6f78 7920 6c69 7374 2072  the proxy list r
-000013f0: 6574 7572 6e73 2061 2064 6963 7469 6f6e  eturns a diction
-00001400: 6172 792c 206f 7220 7768 656e 2066 6f72  ary, or when for
-00001410: 6d61 745f 7261 7720 6861 7320 6265 656e  mat_raw has been
-00001420: 2063 6f6d 706c 6574 6564 2e0a 332e 2023   completed..3. #
-00001430: 2323 2046 6f72 6d61 7474 696e 6720 4461  ## Formatting Da
-00001440: 7461 3a0a 2020 2020 2d20 596f 7572 2067  ta:.    - Your g
-00001450: 6f61 6c20 6973 2074 6f20 666f 726d 6174  oal is to format
-00001460: 2074 6865 2064 6174 6120 696e 2074 6865   the data in the
-00001470: 2060 666f 726d 6174 5f64 6174 6160 206d   `format_data` m
-00001480: 6574 686f 6420 616e 6420 706c 6163 6520  ethod and place 
-00001490: 6974 2069 6e74 6f20 7468 6520 7072 6f76  it into the prov
-000014a0: 6964 6564 2051 7565 7565 2e20 5468 6520  ided Queue. The 
-000014b0: 6461 7461 2073 686f 756c 6420 6265 2073  data should be s
-000014c0: 7472 7563 7475 7265 6420 6173 2066 6f6c  tructured as fol
-000014d0: 6c6f 7773 3a0a 2020 2020 2020 2020 6060  lows:.        ``
-000014e0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-000014f0: 6461 7461 203d 207b 0a20 2020 2020 2020  data = {.       
-00001500: 2020 2020 2022 636f 756e 7472 7922 3a20       "country": 
-00001510: 2255 5322 2c0a 2020 2020 2020 2020 2020  "US",.          
-00001520: 2020 227a 6f6e 6522 3a20 2255 5322 2c0a    "zone": "US",.
-00001530: 2020 2020 2020 2020 2020 2020 226d 6574              "met
-00001540: 686f 6422 3a20 2268 7474 7022 2c0a 2020  hod": "http",.  
-00001550: 2020 2020 2020 2020 2020 2261 6e6f 6e79            "anony
-00001560: 6d69 7479 223a 2022 616e 6f6e 796d 6f75  mity": "anonymou
-00001570: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00001580: 2270 726f 746f 636f 6c22 3a20 2268 7474  "protocol": "htt
-00001590: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-000015a0: 2270 6f72 7422 3a20 2238 3038 3022 2c0a  "port": "8080",.
-000015b0: 2020 2020 2020 2020 2020 2020 2269 7022              "ip"
-000015c0: 3a20 2231 3237 2e30 2e30 2e31 222c 0a20  : "127.0.0.1",. 
-000015d0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000015e0: 2071 7565 7565 2e70 7574 2864 6174 6129   queue.put(data)
-000015f0: 0a20 2020 2020 2020 2060 6060 0a34 2e20  .        ```.4. 
-00001600: 2323 2320 436f 6e67 7261 7475 6c61 7469  ### Congratulati
-00001610: 6f6e 730a 2020 2020 2d20 4966 2064 6f6e  ons.    - If don
-00001620: 6520 636f 7272 6563 746c 792c 2063 6f6e  e correctly, con
-00001630: 6772 6174 756c 6174 696f 6e73 2120 596f  gratulations! Yo
-00001640: 7527 7665 2073 7563 6365 7373 6675 6c6c  u've successfull
-00001650: 7920 6372 6561 7465 6420 6120 6e65 7720  y created a new 
-00001660: 7072 6f78 7920 7061 7273 6572 2066 6f72  proxy parser for
-00001670: 2074 6869 7320 6c69 6272 6172 792e 0a20   this library.. 
-00001680: 2020 202d 2041 6464 2074 6865 2074 6172     - Add the tar
-00001690: 6765 7465 6420 6c69 6e6b 2061 6e64 2079  geted link and y
-000016a0: 6f75 7220 7363 7261 7065 7220 746f 2060  our scraper to `
-000016b0: 7363 7261 7065 7273 2f5f 5f69 6e69 745f  scrapers/__init_
-000016c0: 5f2e 7079 602e 0a0a 4665 656c 2066 7265  _.py`...Feel fre
-000016d0: 6520 746f 2063 6f6e 7472 6962 7574 652c  e to contribute,
-000016e0: 2073 6861 7265 2079 6f75 7220 696d 7072   share your impr
-000016f0: 6f76 656d 656e 7473 2c20 616e 6420 6578  ovements, and ex
-00001700: 7061 6e64 2074 6865 206c 6962 7261 7279  pand the library
-00001710: 2773 2063 6170 6162 696c 6974 6965 732e  's capabilities.
-00001720: 2059 6f75 7220 6566 666f 7274 7320 636f   Your efforts co
-00001730: 6e74 7269 6275 7465 2074 6f20 6120 6772  ntribute to a gr
-00001740: 6f77 696e 6720 706f 6f6c 206f 6620 6176  owing pool of av
-00001750: 6169 6c61 626c 6520 7072 6f78 6965 7320  ailable proxies 
-00001760: 666f 7220 7468 6520 4150 726f 7879 5265  for the AProxyRe
-00001770: 6c61 7920 636f 6d6d 756e 6974 792e 0a    lay community..
+000002f0: 600a 5b21 5b50 7950 4920 7665 7273 696f  `.[![PyPI versio
+00000300: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
+00000310: 2e66 7572 792e 696f 2f70 792f 6170 726f  .fury.io/py/apro
+00000320: 7879 7265 6c61 792e 7376 6729 5d28 6874  xyrelay.svg)](ht
+00000330: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
+00000340: 2e69 6f2f 7079 2f61 7072 6f78 7972 656c  .io/py/aproxyrel
+00000350: 6179 290a 5b21 5b41 2050 726f 7879 2052  ay).[![A Proxy R
+00000360: 656c 6179 2062 7569 6c64 5d28 6874 7470  elay build](http
+00000370: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00000380: 792d 6465 762d 6170 702f 7072 6f78 792d  y-dev-app/proxy-
+00000390: 7265 6c61 792f 6163 7469 6f6e 732f 776f  relay/actions/wo
+000003a0: 726b 666c 6f77 732f 656e 7472 7970 6f69  rkflows/entrypoi
+000003b0: 6e74 2e79 616d 6c2f 6261 6467 652e 7376  nt.yaml/badge.sv
+000003c0: 673f 6272 616e 6368 3d64 6576 656c 6f70  g?branch=develop
+000003d0: 6d65 6e74 295d 2868 7474 7073 3a2f 2f67  ment)](https://g
+000003e0: 6974 6875 622e 636f 6d2f 6d79 2d64 6576  ithub.com/my-dev
+000003f0: 2d61 7070 2f70 726f 7879 2d72 656c 6179  -app/proxy-relay
+00000400: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000410: 7773 2f65 6e74 7279 706f 696e 742e 7961  ws/entrypoint.ya
+00000420: 6d6c 290a 0a23 2041 5072 6f78 7952 656c  ml)..# AProxyRel
+00000430: 6179 3a20 416e 2041 7379 6e63 2052 6571  ay: An Async Req
+00000440: 7565 7374 204c 6962 7261 7279 2077 6974  uest Library wit
+00000450: 6820 5072 6f78 7920 526f 7461 7469 6f6e  h Proxy Rotation
+00000460: 0a0a 4150 726f 7879 5265 6c61 7920 6973  ..AProxyRelay is
+00000470: 2061 6e20 6173 796e 6368 726f 6e6f 7573   an asynchronous
+00000480: 2072 6571 7565 7374 206c 6962 7261 7279   request library
+00000490: 2064 6573 6967 6e65 6420 666f 7220 6561   designed for ea
+000004a0: 7379 2064 6174 6120 7265 7472 6965 7661  sy data retrieva
+000004b0: 6c20 7573 696e 6720 7661 7269 6f75 7320  l using various 
+000004c0: 7072 6f78 7920 7365 7276 6572 732e 2049  proxy servers. I
+000004d0: 7420 7365 616d 6c65 7373 6c79 2068 616e  t seamlessly han
+000004e0: 646c 6573 2070 726f 7879 2072 6f74 6174  dles proxy rotat
+000004f0: 696f 6e2c 2070 7265 7365 7276 6573 2064  ion, preserves d
+00000500: 6174 6120 7468 6174 2066 6169 6c73 2074  ata that fails t
+00000510: 6f20 6265 2072 6571 7565 7374 6564 2c20  o be requested, 
+00000520: 616e 6420 7369 6d70 6c69 6669 6573 2041  and simplifies A
+00000530: 5049 2073 6372 6170 696e 672e 2054 6865  PI scraping. The
+00000540: 206c 6962 7261 7279 2069 7320 7772 6974   library is writ
+00000550: 7465 6e20 696e 2060 5079 7468 6f6e 2033  ten in `Python 3
+00000560: 2e31 322e 3160 2062 7574 2069 7320 636f  .12.1` but is co
+00000570: 6d70 6174 6962 6c65 2077 6974 6820 7072  mpatible with pr
+00000580: 6f6a 6563 7473 2075 7469 6c69 7a69 6e67  ojects utilizing
+00000590: 2060 5079 7468 6f6e 2033 2e31 312e 3260   `Python 3.11.2`
+000005a0: 2e0a 0a49 6e20 6164 6469 7469 6f6e 2c20  ...In addition, 
+000005b0: 7465 7374 6564 2070 726f 7869 6573 2077  tested proxies w
+000005c0: 696c 6c20 6265 2073 6861 7265 6420 7769  ill be shared wi
+000005d0: 7468 206f 7468 6572 2070 656f 706c 6520  th other people 
+000005e0: 7573 696e 6720 7468 6973 206c 6962 7261  using this libra
+000005f0: 7279 2e20 5468 6520 6d6f 7265 2074 6869  ry. The more thi
+00000600: 7320 6c69 6272 6172 7920 6973 2075 7469  s library is uti
+00000610: 6c69 7a65 642c 2074 6865 2062 6967 6765  lized, the bigge
+00000620: 7220 7468 6520 706f 6f6c 206f 6620 6176  r the pool of av
+00000630: 6169 6c61 626c 6520 7072 6f78 6965 732e  ailable proxies.
+00000640: 0a0a 4f75 7220 7363 7261 7065 722c 2075  ..Our scraper, u
+00000650: 7365 6420 746f 206f 6274 6169 6e20 7072  sed to obtain pr
+00000660: 6f78 6965 732c 2069 7320 6869 6768 6c79  oxies, is highly
+00000670: 206d 6f64 756c 6172 2061 6e64 2070 6c75   modular and plu
+00000680: 672d 616e 642d 706c 6179 2c20 6d61 6b69  g-and-play, maki
+00000690: 6e67 2069 7420 6561 7379 2074 6f20 636f  ng it easy to co
+000006a0: 6e74 7269 6275 7465 2074 6f2e 0a0a 2323  ntribute to...##
+000006b0: 2055 7361 6765 0a41 5072 6f78 7952 656c   Usage.AProxyRel
+000006c0: 6179 2073 7472 6561 6d6c 696e 6573 2074  ay streamlines t
+000006d0: 6865 2070 726f 6365 7373 206f 6620 6d61  he process of ma
+000006e0: 6b69 6e67 2061 7379 6e63 6872 6f6e 6f75  king asynchronou
+000006f0: 7320 7265 7175 6573 7473 2077 6974 6820  s requests with 
+00000700: 7072 6f78 7920 7365 7276 6572 732e 2049  proxy servers. I
+00000710: 7420 6f66 6665 7273 2074 6865 2066 6f6c  t offers the fol
+00000720: 6c6f 7769 6e67 2066 6561 7475 7265 733a  lowing features:
+00000730: 0a2d 2041 7379 6e63 6872 6f6e 6f75 736c  .- Asynchronousl
+00000740: 7920 6665 7463 6865 7320 6c69 7374 7320  y fetches lists 
+00000750: 6f66 2066 7265 6520 7072 6f78 6965 7320  of free proxies 
+00000760: 6672 6f6d 2076 6172 696f 7573 2073 6f75  from various sou
+00000770: 7263 6573 2062 6173 6564 206f 6e20 7468  rces based on th
+00000780: 6520 7072 6f76 6964 6564 207a 6f6e 650a  e provided zone.
+00000790: 2d20 5465 7374 7320 616e 6420 7368 6172  - Tests and shar
+000007a0: 6573 2070 726f 7869 6573 2077 6974 6820  es proxies with 
+000007b0: 6f74 6865 7220 7573 6572 7320 6f66 2074  other users of t
+000007c0: 6865 206c 6962 7261 7279 0a2d 2049 6465  he library.- Ide
+000007d0: 6e74 6966 6965 7320 616e 6420 6469 7363  ntifies and disc
+000007e0: 6172 6473 2062 6164 2070 726f 7869 6573  ards bad proxies
+000007f0: 2c20 7072 6573 6572 7669 6e67 2064 6174  , preserving dat
+00000800: 6120 666f 7220 6661 696c 6564 2074 6172  a for failed tar
+00000810: 6765 7420 7265 7175 6573 7473 0a2d 2042  get requests.- B
+00000820: 7970 6173 7365 7320 4150 4920 6c69 6d69  ypasses API limi
+00000830: 7465 7273 2069 6e20 616e 2061 7379 6e63  ters in an async
+00000840: 6872 6f6e 6f75 7320 6d61 6e6e 6572 2028  hronous manner (
+00000850: 666f 7220 6564 7563 6174 696f 6e61 6c20  for educational 
+00000860: 7075 7270 6f73 6529 0a0a 2323 2320 4578  purpose)..### Ex
+00000870: 616d 706c 650a 6060 6070 790a 6672 6f6d  ample.```py.from
+00000880: 2061 7072 6f78 7972 656c 6179 2069 6d70   aproxyrelay imp
+00000890: 6f72 7420 4150 726f 7879 5265 6c61 790a  ort AProxyRelay.
+000008a0: 0a74 6172 6765 7473 203d 205b 0a20 2020  .targets = [.   
+000008b0: 2027 6874 7470 733a 2f2f 736f 6d65 2d77   'https://some-w
+000008c0: 6562 7369 7465 2e63 6f6d 2f61 7069 2f61  ebsite.com/api/a
+000008d0: 7070 3f69 643d 3135 3531 3336 3027 2c0a  pp?id=1551360',.
+000008e0: 2020 2020 2768 7474 7073 3a2f 2f73 6f6d      'https://som
+000008f0: 652d 7765 6273 6974 652e 636f 6d2f 6170  e-website.com/ap
+00000900: 692f 6170 703f 6964 3d32 3037 3234 3530  i/app?id=2072450
+00000910: 272c 0a20 2020 2027 6874 7470 733a 2f2f  ',.    'https://
+00000920: 736f 6d65 2d77 6562 7369 7465 2e63 6f6d  some-website.com
+00000930: 2f61 7069 2f61 7070 3f69 643d 3139 3234  /api/app?id=1924
+00000940: 3336 3027 2c0a 2020 2020 2768 7474 7073  360',.    'https
+00000950: 3a2f 2f73 6f6d 652d 7765 6273 6974 652e  ://some-website.
+00000960: 636f 6d2f 6170 692f 6170 703f 6964 3d31  com/api/app?id=1
+00000970: 3730 3738 3730 272c 0a20 2020 2027 6874  707870',.    'ht
+00000980: 7470 733a 2f2f 736f 6d65 2d77 6562 7369  tps://some-websi
+00000990: 7465 2e63 6f6d 2f61 7069 2f61 7070 3f69  te.com/api/app?i
+000009a0: 643d 3138 3339 3838 3027 2c0a 5d0a 0a23  d=1839880',.]..#
+000009b0: 2049 6e69 7469 616c 697a 6520 7072 6f78   Initialize prox
+000009c0: 7920 7265 6c61 790a 7072 6f78 795f 7265  y relay.proxy_re
+000009d0: 6c61 7920 3d20 4150 726f 7879 5265 6c61  lay = AProxyRela
+000009e0: 7928 0a20 2020 2074 6172 6765 7473 3d74  y(.    targets=t
+000009f0: 6172 6765 7473 2c0a 2020 2020 7469 6d65  argets,.    time
+00000a00: 6f75 743d 352c 0a20 2020 2074 6573 745f  out=5,.    test_
+00000a10: 7072 6f78 793d 5472 7565 2c0a 2020 2020  proxy=True,.    
+00000a20: 7465 7374 5f74 696d 656f 7574 3d31 302c  test_timeout=10,
+00000a30: 0a20 2020 207a 6f6e 653d 2775 7327 2c0a  .    zone='us',.
+00000a40: 290a 0a23 2046 6574 6368 2064 6174 610a  )..# Fetch data.
+00000a50: 6461 7461 203d 2070 726f 7879 5f72 656c  data = proxy_rel
+00000a60: 6179 2e73 7461 7274 2829 0a0a 2320 5265  ay.start()..# Re
+00000a70: 7375 6c74 2051 7565 7565 0a70 7269 6e74  sult Queue.print
+00000a80: 2864 6174 612e 7173 697a 6528 2929 0a60  (data.qsize()).`
+00000a90: 6060 0a0a 2323 2041 2050 726f 7879 2052  ``..## A Proxy R
+00000aa0: 656c 6179 3a20 496e 7374 616c 6c61 7469  elay: Installati
+00000ab0: 6f6e 0a53 696d 706c 7920 7275 6e0a 0a20  on.Simply run.. 
+00000ac0: 2020 2070 6970 2069 6e73 7461 6c6c 2061     pip install a
+00000ad0: 7072 6f78 7972 656c 6179 0a0a 2323 2041  proxyrelay..## A
+00000ae0: 2050 726f 7879 2052 656c 6179 3a20 4c6f   Proxy Relay: Lo
+00000af0: 6361 6c20 4465 7665 6c6f 706d 656e 740a  cal Development.
+00000b00: 546f 2069 6e73 7461 6c6c 2061 6c6c 206c  To install all l
+00000b10: 6962 7261 7279 2064 6570 656e 6465 6e63  ibrary dependenc
+00000b20: 6965 7320 666f 7220 6c6f 6361 6c20 6465  ies for local de
+00000b30: 7665 6c6f 706d 656e 742c 2065 7863 6c75  velopment, exclu
+00000b40: 6469 6e67 2074 6865 2063 6f72 6520 636f  ding the core co
+00000b50: 6465 2061 7661 696c 6162 6c65 206c 6f63  de available loc
+00000b60: 616c 6c79 2c20 7573 6520 7468 6520 666f  ally, use the fo
+00000b70: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
+00000b80: 7769 7468 696e 2061 2076 6972 7475 616c  within a virtual
+00000b90: 2065 6e76 6972 6f6e 6d65 6e74 3a0a 0a20   environment:.. 
+00000ba0: 2020 2070 6970 2069 6e73 7461 6c6c 202d     pip install -
+00000bb0: 6520 2e5b 6465 765d 0a0a 5468 6973 2063  e .[dev]..This c
+00000bc0: 6f6d 6d61 6e64 2069 6e73 7461 6c6c 7320  ommand installs 
+00000bd0: 6465 7065 6e64 656e 6369 6573 2061 6e64  dependencies and
+00000be0: 2072 656d 6f76 6573 2074 6865 2063 6f72   removes the cor
+00000bf0: 6520 636f 6465 206f 6620 4150 726f 7879  e code of AProxy
+00000c00: 5265 6c61 7920 6672 6f6d 2074 6865 2076  Relay from the v
+00000c10: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
+00000c20: 6e74 2e0a 0a0a 2320 436f 6e74 7269 6275  nt....# Contribu
+00000c30: 7465 2074 6f20 4150 726f 7879 5265 6c61  te to AProxyRela
+00000c40: 790a 0a41 5072 6f78 7952 656c 6179 2065  y..AProxyRelay e
+00000c50: 6e63 6f75 7261 6765 7320 636f 6e74 7269  ncourages contri
+00000c60: 6275 7469 6f6e 7320 746f 2065 6e68 616e  butions to enhan
+00000c70: 6365 2069 7473 2063 6170 6162 696c 6974  ce its capabilit
+00000c80: 6965 7320 6279 2061 6c6c 6f77 696e 6720  ies by allowing 
+00000c90: 7573 6572 7320 746f 2063 7265 6174 6520  users to create 
+00000ca0: 6375 7374 6f6d 2073 6372 6170 6572 732e  custom scrapers.
+00000cb0: 2054 6865 7365 2073 6372 6170 6572 7320   These scrapers 
+00000cc0: 6172 6520 6465 7369 676e 6564 2074 6f20  are designed to 
+00000cd0: 6665 7463 6820 7072 6f78 7920 6461 7461  fetch proxy data
+00000ce0: 2066 726f 6d20 6469 6666 6572 656e 7420   from different 
+00000cf0: 736f 7572 6365 732e 2054 6865 2070 726f  sources. The pro
+00000d00: 6365 7373 2069 7320 7374 7261 6967 6874  cess is straight
+00000d10: 666f 7277 6172 642c 2061 6e64 2068 6572  forward, and her
+00000d20: 6527 7320 6120 6775 6964 6520 746f 2068  e's a guide to h
+00000d30: 656c 7020 796f 7520 6765 7420 7374 6172  elp you get star
+00000d40: 7465 643a 0a0a 2323 2053 6372 6170 6572  ted:..## Scraper
+00000d50: 2053 7472 7563 7475 7265 0a0a 4150 726f   Structure..APro
+00000d60: 7879 5265 6c61 7920 696e 636c 7564 6573  xyRelay includes
+00000d70: 2061 2064 6564 6963 6174 6564 2066 6f6c   a dedicated fol
+00000d80: 6465 7220 6e61 6d65 6420 6073 6372 6170  der named `scrap
+00000d90: 6572 7360 2e20 5769 7468 696e 2074 6869  ers`. Within thi
+00000da0: 7320 666f 6c64 6572 2c20 6561 6368 2073  s folder, each s
+00000db0: 6372 6170 6572 2c20 7072 6566 6978 6564  craper, prefixed
+00000dc0: 2077 6974 6820 6070 6172 7365 725f 602c   with `parser_`,
+00000dd0: 2069 6e68 6572 6974 7320 6672 6f6d 2074   inherits from t
+00000de0: 6865 2060 7061 7273 6572 2e70 7960 2066  he `parser.py` f
+00000df0: 696c 652e 2054 6f20 7072 6f76 6964 6520  ile. To provide 
+00000e00: 796f 7520 7769 7468 2061 2067 656e 6572  you with a gener
+00000e10: 616c 2075 6e64 6572 7374 616e 6469 6e67  al understanding
+00000e20: 2c20 6865 7265 2773 2061 6e20 6578 616d  , here's an exam
+00000e30: 706c 6520 6f66 2074 6865 2060 4d61 696e  ple of the `Main
+00000e40: 5363 7261 7065 7260 2063 6c61 7373 3a0a  Scraper` class:.
+00000e50: 0a60 6060 7079 0a66 726f 6d20 7175 6575  .```py.from queu
+00000e60: 6520 696d 706f 7274 2051 7565 7565 0a0a  e import Queue..
+00000e70: 6672 6f6d 202e 636f 7265 2069 6d70 6f72  from .core impor
+00000e80: 7420 5363 7261 7065 7243 6f72 650a 0a0a  t ScraperCore...
+00000e90: 636c 6173 7320 4d61 696e 5363 7261 7065  class MainScrape
+00000ea0: 7228 5363 7261 7065 7243 6f72 6529 3a0a  r(ScraperCore):.
+00000eb0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00000ec0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00000ed0: 2020 2020 2020 2020 5363 7261 7065 7243          ScraperC
+00000ee0: 6f72 652e 5f5f 696e 6974 5f5f 2873 656c  ore.__init__(sel
+00000ef0: 6629 0a0a 2020 2020 4063 6c61 7373 6d65  f)..    @classme
+00000f00: 7468 6f64 0a20 2020 2061 7379 6e63 2064  thod.    async d
+00000f10: 6566 2066 6f72 6d61 745f 7572 6c28 636c  ef format_url(cl
+00000f20: 732c 2075 726c 2c20 2a61 7267 732c 202a  s, url, *args, *
+00000f30: 2a6b 7761 7267 7329 202d 3e20 7374 723a  *kwargs) -> str:
+00000f40: 0a20 2020 2020 2020 2022 2222 466f 726d  .        """Form
+00000f50: 6174 7320 5552 4c20 6265 666f 7265 2073  ats URL before s
+00000f60: 6372 6170 696e 672c 206c 6574 2075 7320  craping, let us 
+00000f70: 6164 6a75 7374 2071 7565 7279 2070 6172  adjust query par
+00000f80: 616d 6574 6572 7320 666f 7220 6561 6368  ameters for each
+00000f90: 2070 6172 7365 7222 2222 0a20 2020 2020   parser""".     
+00000fa0: 2020 206e 6577 5f75 726c 203d 2066 277b     new_url = f'{
+00000fb0: 7572 6c7d 270a 2020 2020 2020 2020 7265  url}'.        re
+00000fc0: 7475 726e 206e 6577 5f75 726c 0a0a 2020  turn new_url..  
+00000fd0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00000fe0: 2020 2061 7379 6e63 2064 6566 2066 6f72     async def for
+00000ff0: 6d61 745f 7261 7728 636c 732c 2068 746d  mat_raw(cls, htm
+00001000: 6c3a 2073 7472 293a 0a20 2020 2020 2020  l: str):.       
+00001010: 2022 2222 5061 7273 6520 7465 7874 2f68   """Parse text/h
+00001020: 746d 6c20 7061 6765 732c 2063 7573 746f  tml pages, custo
+00001030: 6d69 7a65 6420 6d65 7468 6f64 2066 6f72  mized method for
+00001040: 2074 6865 2070 6172 7365 7220 6f66 2074   the parser of t
+00001050: 6869 7320 7765 6273 6974 6522 2222 0a20  his website""". 
+00001060: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00001070: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00001080: 2827 466f 726d 6174 2072 6177 2070 6172  ('Format raw par
+00001090: 7365 7220 6861 7320 6e6f 7420 6265 656e  ser has not been
+000010a0: 2069 6d70 6c65 6d65 6e74 6564 2079 6574   implemented yet
+000010b0: 2729 0a0a 2020 2020 4063 6c61 7373 6d65  ')..    @classme
+000010c0: 7468 6f64 0a20 2020 2061 7379 6e63 2064  thod.    async d
+000010d0: 6566 2066 6f72 6d61 745f 6461 7461 2863  ef format_data(c
+000010e0: 6c73 2c20 6461 7461 3a20 6469 6374 2c20  ls, data: dict, 
+000010f0: 7175 6575 653a 2051 7565 7565 293a 0a20  queue: Queue):. 
+00001100: 2020 2020 2020 2022 2222 4461 7461 2066         """Data f
+00001110: 6f72 6d61 7474 6572 2c20 666f 726d 6174  ormatter, format
+00001120: 7320 6461 7461 2061 6e64 2072 6574 7572  s data and retur
+00001130: 6e73 2069 7320 6261 636b 2069 6e20 7468  ns is back in th
+00001140: 6520 7072 6f63 6573 7320 5175 6575 6522  e process Queue"
+00001150: 2222 0a20 2020 2020 2020 2072 6169 7365  "".        raise
+00001160: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+00001170: 7272 6f72 2827 466f 726d 2064 6174 6120  rror('Form data 
+00001180: 7061 7273 6572 2068 6173 206e 6f74 2062  parser has not b
+00001190: 6565 6e20 696d 706c 656d 656e 7465 6420  een implemented 
+000011a0: 7965 7427 290a 6060 600a 0a23 2320 4372  yet').```..## Cr
+000011b0: 6561 7469 6e67 2079 6f75 7220 6f77 6e20  eating your own 
+000011c0: 5072 6f78 7920 5363 7261 7065 720a 0a54  Proxy Scraper..T
+000011d0: 6f20 636f 6e74 7269 6275 7465 2079 6f75  o contribute you
+000011e0: 7220 6f77 6e20 7072 6f78 7920 7363 7261  r own proxy scra
+000011f0: 7065 722c 2066 6f6c 6c6f 7720 7468 6573  per, follow thes
+00001200: 6520 7374 6570 733a 0a0a 312e 2023 2323  e steps:..1. ###
+00001210: 2043 7265 6174 6520 6120 6e65 7720 7061   Create a new pa
+00001220: 7273 6572 2063 6c61 7373 2069 6e73 6964  rser class insid
+00001230: 6520 7468 6520 7363 7261 7065 7273 2066  e the scrapers f
+00001240: 6f6c 6465 720a 2020 2020 2d20 496e 6865  older.    - Inhe
+00001250: 7269 7420 6672 6f6d 2074 6865 2060 4d61  rit from the `Ma
+00001260: 696e 5363 7261 7065 7260 2e0a 2020 2020  inScraper`..    
+00001270: 2d20 4f76 6572 7772 6974 6520 7468 6520  - Overwrite the 
+00001280: 6e65 6365 7373 6172 7920 6d65 7468 6f64  necessary method
+00001290: 7320 7265 7175 6972 6564 2066 6f72 2073  s required for s
+000012a0: 6372 6170 696e 6720 6164 6469 7469 6f6e  craping addition
+000012b0: 616c 2070 726f 7879 2073 6572 7665 7273  al proxy servers
+000012c0: 2e0a 322e 2023 2323 204d 6574 686f 6473  ..2. ### Methods
+000012d0: 2074 6f20 4f76 6572 7772 6974 653a 0a20   to Overwrite:. 
+000012e0: 2020 202d 2060 666f 726d 6174 5f75 726c     - `format_url
+000012f0: 603a 204d 616e 6970 756c 6174 6520 7468  `: Manipulate th
+00001300: 6520 7072 6f78 7920 6c69 7374 2072 6571  e proxy list req
+00001310: 7565 7374 2055 524c 2062 6566 6f72 6520  uest URL before 
+00001320: 6d61 6b69 6e67 2061 2072 6571 7565 7374  making a request
+00001330: 2c20 656e 6162 6c69 6e67 2061 646a 7573  , enabling adjus
+00001340: 746d 656e 7420 6f66 2076 6172 696f 7573  tment of various
+00001350: 2071 7565 7279 2070 6172 616d 6574 6572   query parameter
+00001360: 732e 0a20 2020 202d 2060 666f 726d 6174  s..    - `format
+00001370: 5f72 6177 603a 2057 6865 6e20 7468 6520  _raw`: When the 
+00001380: 6461 7461 206f 6274 6169 6e65 6420 6672  data obtained fr
+00001390: 6f6d 2074 6865 206c 696e 6b20 6973 2060  om the link is `
+000013a0: 7478 742f 6874 6d6c 602c 2074 6869 7320  txt/html`, this 
+000013b0: 6d65 7468 6f64 2073 686f 756c 6420 7363  method should sc
+000013c0: 7261 7065 2074 6865 2064 6174 6120 616e  rape the data an
+000013d0: 6420 666f 726d 6174 2069 7420 696e 746f  d format it into
+000013e0: 2077 6f72 6b61 626c 6520 6461 7461 2e0a   workable data..
+000013f0: 2020 2020 2d20 6066 6f72 6d61 745f 6461      - `format_da
+00001400: 7461 603a 2054 6869 7320 6d65 7468 6f64  ta`: This method
+00001410: 2069 7320 7472 6967 6765 7265 6420 7768   is triggered wh
+00001420: 656e 2074 6865 2063 616c 6c20 746f 2074  en the call to t
+00001430: 6865 2070 726f 7879 206c 6973 7420 7265  he proxy list re
+00001440: 7475 726e 7320 6120 6469 6374 696f 6e61  turns a dictiona
+00001450: 7279 2c20 6f72 2077 6865 6e20 666f 726d  ry, or when form
+00001460: 6174 5f72 6177 2068 6173 2062 6565 6e20  at_raw has been 
+00001470: 636f 6d70 6c65 7465 642e 0a33 2e20 2323  completed..3. ##
+00001480: 2320 466f 726d 6174 7469 6e67 2044 6174  # Formatting Dat
+00001490: 613a 0a20 2020 202d 2059 6f75 7220 676f  a:.    - Your go
+000014a0: 616c 2069 7320 746f 2066 6f72 6d61 7420  al is to format 
+000014b0: 7468 6520 6461 7461 2069 6e20 7468 6520  the data in the 
+000014c0: 6066 6f72 6d61 745f 6461 7461 6020 6d65  `format_data` me
+000014d0: 7468 6f64 2061 6e64 2070 6c61 6365 2069  thod and place i
+000014e0: 7420 696e 746f 2074 6865 2070 726f 7669  t into the provi
+000014f0: 6465 6420 5175 6575 652e 2054 6865 2064  ded Queue. The d
+00001500: 6174 6120 7368 6f75 6c64 2062 6520 7374  ata should be st
+00001510: 7275 6374 7572 6564 2061 7320 666f 6c6c  ructured as foll
+00001520: 6f77 733a 0a20 2020 2020 2020 2060 6060  ows:.        ```
+00001530: 7079 7468 6f6e 0a20 2020 2020 2020 2064  python.        d
+00001540: 6174 6120 3d20 7b0a 2020 2020 2020 2020  ata = {.        
+00001550: 2020 2020 2263 6f75 6e74 7279 223a 2022      "country": "
+00001560: 5553 222c 0a20 2020 2020 2020 2020 2020  US",.           
+00001570: 2022 7a6f 6e65 223a 2022 5553 222c 0a20   "zone": "US",. 
+00001580: 2020 2020 2020 2020 2020 2022 6d65 7468             "meth
+00001590: 6f64 223a 2022 6874 7470 222c 0a20 2020  od": "http",.   
+000015a0: 2020 2020 2020 2020 2022 616e 6f6e 796d           "anonym
+000015b0: 6974 7922 3a20 2261 6e6f 6e79 6d6f 7573  ity": "anonymous
+000015c0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000015d0: 7072 6f74 6f63 6f6c 223a 2022 6874 7470  protocol": "http
+000015e0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000015f0: 706f 7274 223a 2022 3830 3830 222c 0a20  port": "8080",. 
+00001600: 2020 2020 2020 2020 2020 2022 6970 223a             "ip":
+00001610: 2022 3132 372e 302e 302e 3122 2c0a 2020   "127.0.0.1",.  
+00001620: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00001630: 7175 6575 652e 7075 7428 6461 7461 290a  queue.put(data).
+00001640: 2020 2020 2020 2020 6060 600a 342e 2023          ```.4. #
+00001650: 2323 2043 6f6e 6772 6174 756c 6174 696f  ## Congratulatio
+00001660: 6e73 0a20 2020 202d 2049 6620 646f 6e65  ns.    - If done
+00001670: 2063 6f72 7265 6374 6c79 2c20 636f 6e67   correctly, cong
+00001680: 7261 7475 6c61 7469 6f6e 7321 2059 6f75  ratulations! You
+00001690: 2776 6520 7375 6363 6573 7366 756c 6c79  've successfully
+000016a0: 2063 7265 6174 6564 2061 206e 6577 2070   created a new p
+000016b0: 726f 7879 2070 6172 7365 7220 666f 7220  roxy parser for 
+000016c0: 7468 6973 206c 6962 7261 7279 2e0a 2020  this library..  
+000016d0: 2020 2d20 4164 6420 7468 6520 7461 7267    - Add the targ
+000016e0: 6574 6564 206c 696e 6b20 616e 6420 796f  eted link and yo
+000016f0: 7572 2073 6372 6170 6572 2074 6f20 6073  ur scraper to `s
+00001700: 6372 6170 6572 732f 5f5f 696e 6974 5f5f  crapers/__init__
+00001710: 2e70 7960 2e0a 0a46 6565 6c20 6672 6565  .py`...Feel free
+00001720: 2074 6f20 636f 6e74 7269 6275 7465 2c20   to contribute, 
+00001730: 7368 6172 6520 796f 7572 2069 6d70 726f  share your impro
+00001740: 7665 6d65 6e74 732c 2061 6e64 2065 7870  vements, and exp
+00001750: 616e 6420 7468 6520 6c69 6272 6172 7927  and the library'
+00001760: 7320 6361 7061 6269 6c69 7469 6573 2e20  s capabilities. 
+00001770: 596f 7572 2065 6666 6f72 7473 2063 6f6e  Your efforts con
+00001780: 7472 6962 7574 6520 746f 2061 2067 726f  tribute to a gro
+00001790: 7769 6e67 2070 6f6f 6c20 6f66 2061 7661  wing pool of ava
+000017a0: 696c 6162 6c65 2070 726f 7869 6573 2066  ilable proxies f
+000017b0: 6f72 2074 6865 2041 5072 6f78 7952 656c  or the AProxyRel
+000017c0: 6179 2063 6f6d 6d75 6e69 7479 2e0a 0a23  ay community...#
+000017d0: 2320 436f 6d70 696c 696e 6720 746f 2070  # Compiling to p
+000017e0: 6163 6b61 6765 0a54 6f20 636f 6d70 696c  ackage.To compil
+000017f0: 6520 7468 6520 6c69 6272 6172 7920 696e  e the library in
+00001800: 746f 2061 2070 6163 6b61 6765 2c20 7573  to a package, us
+00001810: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00001820: 636f 6d6d 616e 6420 6166 7465 7220 696e  command after in
+00001830: 7374 616c 6c69 6e67 2060 7265 7175 6972  stalling `requir
+00001840: 656d 656e 7473 2e74 7874 603a 0a0a 6060  ements.txt`:..``
+00001850: 6073 680a 7079 7468 6f6e 2073 6574 7570  `sh.python setup
+00001860: 2e70 7920 7364 6973 7420 6264 6973 745f  .py sdist bdist_
+00001870: 7768 6565 6c0a 6060 600a 0a54 6869 7320  wheel.```..This 
+00001880: 7769 6c6c 2067 656e 6572 6174 6520 7468  will generate th
+00001890: 6520 7061 636b 6167 6520 696e 2074 6865  e package in the
+000018a0: 2060 6469 7374 6020 666f 6c64 6572 2e0a   `dist` folder..
+000018b0: 4e6f 7465 3a20 4120 7665 7273 696f 6e20  Note: A version 
+000018c0: 6361 6e20 6265 2073 6574 2077 6974 6820  can be set with 
+000018d0: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
+000018e0: 7661 7269 6162 6c65 2060 4355 5354 4f4d  variable `CUSTOM
+000018f0: 5f56 4552 5349 4f4e 60                   _VERSION`
```

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/__init__.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/__init__.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/agents.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/agents.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/core.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/core.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/process.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/process.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/__init__.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/__init__.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/core.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/core.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_freeproxylist.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_freeproxylist.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_gg_my_dev_app.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_gg_my_dev_app.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_lumiproxy.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_lumiproxy.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_proxyscrape.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_proxyscrape.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_socks_proxy.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_socks_proxy.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_spys_de.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_spys_de.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_spys_nl.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_spys_nl.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_spys_us.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_spys_us.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay/scrapers/parser_ssl_proxies.py` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay/scrapers/parser_ssl_proxies.py`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay.egg-info/PKG-INFO` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aproxyrelay
-Version: 1.90.1rc7688073331
+Version: 1.97.1rc7688272509
 Summary: A Proxy Relay, forwarding requests through different IP.
 Home-page: https://github.com/my-dev-app/proxy-relay
 Author: undeƒined
 Author-email: my-dev.app@domainsbyproxy.com
 License: GNU AGPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,32 +31,25 @@
  #######    #       #####  #    #   ##     #      #   #   #      #      ######   #   
  #     #    #       #   #  #    #  #  #    #      #    #  #      #      #    #   #   
  #     #    #       #    #  ####  #    #   #      #     # ###### ###### #    #   #   
                                                                                      
 By undeƒined
 -------------------------------------
 ```
+[![PyPI version](https://badge.fury.io/py/aproxyrelay.svg)](https://badge.fury.io/py/aproxyrelay)
+[![A Proxy Relay build](https://github.com/my-dev-app/proxy-relay/actions/workflows/entrypoint.yaml/badge.svg?branch=development)](https://github.com/my-dev-app/proxy-relay/actions/workflows/entrypoint.yaml)
+
 # AProxyRelay: An Async Request Library with Proxy Rotation
 
 AProxyRelay is an asynchronous request library designed for easy data retrieval using various proxy servers. It seamlessly handles proxy rotation, preserves data that fails to be requested, and simplifies API scraping. The library is written in `Python 3.12.1` but is compatible with projects utilizing `Python 3.11.2`.
 
 In addition, tested proxies will be shared with other people using this library. The more this library is utilized, the bigger the pool of available proxies.
 
 Our scraper, used to obtain proxies, is highly modular and plug-and-play, making it easy to contribute to.
 
-## Compiling to package
-To compile the library into a package, use the following command after installing `requirements.txt`:
-
-```sh
-python setup.py sdist bdist_wheel
-```
-
-This will generate the package in the `dist` folder.
-Note: A version can be set with the environment variable `CUSTOM_VERSION`
-
 ## Usage
 AProxyRelay streamlines the process of making asynchronous requests with proxy servers. It offers the following features:
 - Asynchronously fetches lists of free proxies from various sources based on the provided zone
 - Tests and shares proxies with other users of the library
 - Identifies and discards bad proxies, preserving data for failed target requests
 - Bypasses API limiters in an asynchronous manner (for educational purpose)
 
@@ -84,14 +77,19 @@
 # Fetch data
 data = proxy_relay.start()
 
 # Result Queue
 print(data.qsize())
 ```
 
+## A Proxy Relay: Installation
+Simply run
+
+    pip install aproxyrelay
+
 ## A Proxy Relay: Local Development
 To install all library dependencies for local development, excluding the core code available locally, use the following command within a virtual environment:
 
     pip install -e .[dev]
 
 This command installs dependencies and removes the core code of AProxyRelay from the virtual environment.
 
@@ -157,7 +155,17 @@
         queue.put(data)
         ```
 4. ### Congratulations
     - If done correctly, congratulations! You've successfully created a new proxy parser for this library.
     - Add the targeted link and your scraper to `scrapers/__init__.py`.
 
 Feel free to contribute, share your improvements, and expand the library's capabilities. Your efforts contribute to a growing pool of available proxies for the AProxyRelay community.
+
+## Compiling to package
+To compile the library into a package, use the following command after installing `requirements.txt`:
+
+```sh
+python setup.py sdist bdist_wheel
+```
+
+This will generate the package in the `dist` folder.
+Note: A version can be set with the environment variable `CUSTOM_VERSION`
```

### Comparing `aproxyrelay-1.90.1rc7688073331/aproxyrelay.egg-info/SOURCES.txt` & `aproxyrelay-1.97.1rc7688272509/aproxyrelay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/pyproject.toml` & `aproxyrelay-1.97.1rc7688272509/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aproxyrelay-1.90.1rc7688073331/setup.py` & `aproxyrelay-1.97.1rc7688272509/setup.py`

 * *Files identical despite different names*

