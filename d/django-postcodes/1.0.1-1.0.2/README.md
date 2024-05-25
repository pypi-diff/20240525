# Comparing `tmp/django_postcodes-1.0.1.tar.gz` & `tmp/django_postcodes-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_postcodes-1.0.1.tar", last modified: Sat May 25 13:30:34 2024, max compression
+gzip compressed data, was "django_postcodes-1.0.2.tar", last modified: Sat May 25 13:35:22 2024, max compression
```

## Comparing `django_postcodes-1.0.1.tar` & `django_postcodes-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.514135 django_postcodes-1.0.1/
--rw-rw-rw-   0        0        0    18429 2024-05-24 22:58:35.000000 django_postcodes-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      237 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7660 2024-05-25 13:30:34.514135 django_postcodes-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6488 2024-05-25 13:28:13.000000 django_postcodes-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.512082 django_postcodes-1.0.1/django_postcodes.egg-info/
--rw-rw-rw-   0        0        0     7660 2024-05-25 13:30:34.000000 django_postcodes-1.0.1/django_postcodes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2024-05-25 13:30:34.000000 django_postcodes-1.0.1/django_postcodes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 13:30:34.000000 django_postcodes-1.0.1/django_postcodes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-25 13:30:34.000000 django_postcodes-1.0.1/django_postcodes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 13:30:34.000000 django_postcodes-1.0.1/django_postcodes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.496873 django_postcodes-1.0.1/postcodes/
--rw-rw-rw-   0        0        0        0 2024-05-24 13:07:54.000000 django_postcodes-1.0.1/postcodes/__init__.py
--rw-rw-rw-   0        0        0      156 2024-05-24 13:07:54.000000 django_postcodes-1.0.1/postcodes/apps.py
--rw-rw-rw-   0        0        0     7945 2024-05-24 22:23:16.000000 django_postcodes-1.0.1/postcodes/countries.py
--rw-rw-rw-   0        0        0     4791 2024-05-25 13:22:29.000000 django_postcodes-1.0.1/postcodes/postcode.py
--rw-rw-rw-   0        0        0      786 2024-05-24 22:33:00.000000 django_postcodes-1.0.1/postcodes/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.469217 django_postcodes-1.0.1/postcodes/static/
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.469217 django_postcodes-1.0.1/postcodes/static/postcodes/
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.497869 django_postcodes-1.0.1/postcodes/static/postcodes/css/
--rw-rw-rw-   0        0        0      305 2024-05-25 12:16:23.000000 django_postcodes-1.0.1/postcodes/static/postcodes/css/postcodes.css
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.498868 django_postcodes-1.0.1/postcodes/static/postcodes/js/
--rw-rw-rw-   0        0        0     4295 2024-05-25 12:32:27.000000 django_postcodes-1.0.1/postcodes/static/postcodes/js/postcodes.js
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.500754 django_postcodes-1.0.1/postcodes/test/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/postcodes/test/__init__.py
--rw-rw-rw-   0        0        0      708 2024-05-24 22:41:12.000000 django_postcodes-1.0.1/postcodes/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.502772 django_postcodes-1.0.1/postcodes/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/postcodes/test/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.504899 django_postcodes-1.0.1/postcodes/test/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/postcodes/test/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.505902 django_postcodes-1.0.1/postcodes/test/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/postcodes/test/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     1012 2024-05-24 23:29:16.000000 django_postcodes-1.0.1/postcodes/test/testapp/core/tests.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:30:34.510409 django_postcodes-1.0.1/postcodes/test/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/postcodes/test/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/postcodes/test/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3500 2024-05-24 22:41:51.000000 django_postcodes-1.0.1/postcodes/test/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      509 2024-05-24 22:39:56.000000 django_postcodes-1.0.1/postcodes/test/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/postcodes/test/testapp/testapp/wsgi.py
--rw-rw-rw-   0        0        0      173 2024-05-24 22:59:49.000000 django_postcodes-1.0.1/postcodes/urls.py
--rw-rw-rw-   0        0        0     2147 2024-05-25 13:09:08.000000 django_postcodes-1.0.1/postcodes/views.py
--rw-rw-rw-   0        0        0       90 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1137 2024-05-25 13:30:34.516567 django_postcodes-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-05-24 22:26:59.000000 django_postcodes-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.100762 django_postcodes-1.0.2/
+-rw-rw-rw-   0        0        0    18429 2024-05-24 22:58:35.000000 django_postcodes-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      237 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7979 2024-05-25 13:35:22.100762 django_postcodes-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6807 2024-05-25 13:34:25.000000 django_postcodes-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.098766 django_postcodes-1.0.2/django_postcodes.egg-info/
+-rw-rw-rw-   0        0        0     7979 2024-05-25 13:35:21.000000 django_postcodes-1.0.2/django_postcodes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2024-05-25 13:35:22.000000 django_postcodes-1.0.2/django_postcodes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 13:35:21.000000 django_postcodes-1.0.2/django_postcodes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-25 13:35:21.000000 django_postcodes-1.0.2/django_postcodes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 13:35:21.000000 django_postcodes-1.0.2/django_postcodes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.086248 django_postcodes-1.0.2/postcodes/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:07:54.000000 django_postcodes-1.0.2/postcodes/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-05-24 13:07:54.000000 django_postcodes-1.0.2/postcodes/apps.py
+-rw-rw-rw-   0        0        0     7945 2024-05-24 22:23:16.000000 django_postcodes-1.0.2/postcodes/countries.py
+-rw-rw-rw-   0        0        0     4791 2024-05-25 13:22:29.000000 django_postcodes-1.0.2/postcodes/postcode.py
+-rw-rw-rw-   0        0        0      786 2024-05-24 22:33:00.000000 django_postcodes-1.0.2/postcodes/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.061875 django_postcodes-1.0.2/postcodes/static/
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.061875 django_postcodes-1.0.2/postcodes/static/postcodes/
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.086248 django_postcodes-1.0.2/postcodes/static/postcodes/css/
+-rw-rw-rw-   0        0        0      305 2024-05-25 12:16:23.000000 django_postcodes-1.0.2/postcodes/static/postcodes/css/postcodes.css
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.087249 django_postcodes-1.0.2/postcodes/static/postcodes/js/
+-rw-rw-rw-   0        0        0     4295 2024-05-25 12:32:27.000000 django_postcodes-1.0.2/postcodes/static/postcodes/js/postcodes.js
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.089248 django_postcodes-1.0.2/postcodes/test/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/__init__.py
+-rw-rw-rw-   0        0        0      708 2024-05-24 22:41:12.000000 django_postcodes-1.0.2/postcodes/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.089248 django_postcodes-1.0.2/postcodes/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.090752 django_postcodes-1.0.2/postcodes/test/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.091758 django_postcodes-1.0.2/postcodes/test/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1012 2024-05-24 23:29:16.000000 django_postcodes-1.0.2/postcodes/test/testapp/core/tests.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.097766 django_postcodes-1.0.2/postcodes/test/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3500 2024-05-24 22:41:51.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      509 2024-05-24 22:39:56.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/wsgi.py
+-rw-rw-rw-   0        0        0      173 2024-05-24 22:59:49.000000 django_postcodes-1.0.2/postcodes/urls.py
+-rw-rw-rw-   0        0        0     2147 2024-05-25 13:09:08.000000 django_postcodes-1.0.2/postcodes/views.py
+-rw-rw-rw-   0        0        0       90 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1137 2024-05-25 13:35:22.101910 django_postcodes-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/setup.py
```

### Comparing `django_postcodes-1.0.1/LICENSE` & `django_postcodes-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/PKG-INFO` & `django_postcodes-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2064 6a61  : 2.1..Name: dja
 00000020: 6e67 6f2d 706f 7374 636f 6465 730d 0a56  ngo-postcodes..V
-00000030: 6572 7369 6f6e 3a20 312e 302e 310d 0a53  ersion: 1.0.1..S
+00000030: 6572 7369 6f6e 3a20 312e 302e 320d 0a53  ersion: 1.0.2..S
 00000040: 756d 6d61 7279 3a20 4120 446a 616e 676f  ummary: A Django
 00000050: 2061 7070 2074 6f20 6d61 6e61 6765 2070   app to manage p
 00000060: 6f73 7463 6f64 652f 686f 6d65 206e 756d  ostcode/home num
 00000070: 6265 7220 6164 6472 6573 7320 666f 726d  ber address form
 00000080: 730d 0a48 6f6d 652d 7061 6765 3a20 6874  s..Home-page: ht
 00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000a0: 2f4e 6967 656c 3233 3932 2f70 6f73 7463  /Nigel2392/postc
@@ -78,402 +78,422 @@
 000004d0: 2066 6f72 2044 6a61 6e67 6f2e 2a2a 0d0a   for Django.**..
 000004e0: 0d0a 4279 2064 6566 6175 6c74 2077 6520  ..By default we 
 000004f0: 7573 6520 7468 6520 6672 6565 2028 6275  use the free (bu
 00000500: 7420 7261 7465 206c 696d 6974 6564 2920  t rate limited) 
 00000510: 4150 4920 6672 6f6d 205b 706f 7374 636f  API from [postco
 00000520: 6465 2e67 6f2d 6465 762e 6e6c 5d28 6874  de.go-dev.nl](ht
 00000530: 7470 733a 2f2f 706f 7374 636f 6465 2e67  tps://postcode.g
-00000540: 6f2d 6465 762e 6e6c 2f29 2e0d 0a0d 0a51  o-dev.nl/).....Q
-00000550: 7569 636b 2073 7461 7274 0d0a 2d2d 2d2d  uick start..----
-00000560: 2d2d 2d2d 2d2d 2d0d 0a0d 0a31 2e20 496e  -------....1. In
-00000570: 7374 616c 6c20 7468 6520 7061 636b 6167  stall the packag
-00000580: 6520 7669 6120 7069 703a 0d0a 0d0a 2020  e via pip:....  
-00000590: 2060 6060 6261 7368 0d0a 2020 2070 6970   ```bash..   pip
-000005a0: 2069 6e73 7461 6c6c 2070 6f73 7463 6f64   install postcod
-000005b0: 6573 0d0a 2020 2060 6060 0d0a 0d0a 322e  es..   ```....2.
-000005c0: 2041 6464 2027 706f 7374 636f 6465 7327   Add 'postcodes'
-000005d0: 2074 6f20 796f 7572 2049 4e53 5441 4c4c   to your INSTALL
-000005e0: 4544 5f41 5050 5320 7365 7474 696e 6720  ED_APPS setting 
-000005f0: 6c69 6b65 2074 6869 733a 0d0a 0d0a 2020  like this:....  
-00000600: 2060 6060 0d0a 2020 2049 4e53 5441 4c4c   ```..   INSTALL
-00000610: 4544 5f41 5050 5320 3d20 5b0d 0a20 2020  ED_APPS = [..   
-00000620: 2e2e 2e2c 0d0a 2020 2020 2020 2770 6f73  ...,..      'pos
-00000630: 7463 6f64 6573 272c 0d0a 2020 205d 0d0a  tcodes',..   ]..
-00000640: 2020 2060 6060 0d0a 0d0a 0d0a 2323 2045     ```......## E
-00000650: 7861 6d70 6c65 2075 7361 6765 0d0a 0d0a  xample usage....
-00000660: 4669 7273 7420 7765 206d 7573 7420 6465  First we must de
-00000670: 6669 6e65 2074 6865 2061 7070 726f 7072  fine the appropr
-00000680: 6961 7465 2066 6f72 6d2e 0d0a 0d0a 5468  iate form.....Th
-00000690: 6973 2069 7320 616e 2065 7861 6d70 6c65  is is an example
-000006a0: 206f 6620 6120 666f 726d 2074 6861 7420   of a form that 
-000006b0: 7573 6573 2074 6865 2064 6566 6175 6c74  uses the default
-000006c0: 2041 5049 2065 6e64 706f 696e 7420 2863   API endpoint (c
-000006d0: 7573 746f 6d20 6f6e 6573 2063 616e 2062  ustom ones can b
-000006e0: 6520 6465 6669 6e65 6420 696e 2074 6865  e defined in the
-000006f0: 2073 6574 7469 6e67 7329 3a0d 0a0d 0a45   settings):....E
-00000700: 7665 7279 2061 7474 7269 6275 7465 2063  very attribute c
-00000710: 616e 2062 6520 6375 7374 6f6d 697a 6564  an be customized
-00000720: 2c20 6578 6365 7074 2066 6f72 2074 6865  , except for the
-00000730: 2070 6f73 7463 6f64 6520 616e 6420 686f   postcode and ho
-00000740: 6d65 206e 756d 6265 7220 6669 656c 6473  me number fields
-00000750: 2c20 7768 6963 6820 6172 6520 7265 7175  , which are requ
-00000760: 6972 6564 2066 6f72 2074 6865 206c 6f6f  ired for the loo
-00000770: 6b75 702e 0d0a 0d0a 5468 6573 6520 6172  kup.....These ar
-00000780: 6520 6861 7264 2d63 6f64 6564 2e0d 0a0d  e hard-coded....
-00000790: 0a41 6c6c 206f 7468 6572 2065 6c65 6d65  .All other eleme
-000007a0: 6e74 7320 7072 6f76 6964 6564 2069 6e20  nts provided in 
-000007b0: 7468 6520 6062 696e 6460 206f 626a 6563  the `bind` objec
-000007c0: 7420 7769 6c6c 2062 6520 6669 6c6c 6564  t will be filled
-000007d0: 2069 6e20 7769 7468 2074 6865 2064 6174   in with the dat
-000007e0: 6120 6672 6f6d 2074 6865 2041 5049 2e0d  a from the API..
-000007f0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 636c  ...```python..cl
-00000800: 6173 7320 4164 6472 6573 7346 6f72 6d28  ass AddressForm(
-00000810: 666f 726d 732e 466f 726d 293a 0d0a 2020  forms.Form):..  
-00000820: 2020 2320 5468 6573 6520 6172 6520 7265    # These are re
-00000830: 7175 6972 6564 2066 6f72 2074 6865 206c  quired for the l
-00000840: 6f6f 6b75 700d 0a20 2020 2070 6f73 7463  ookup..    postc
-00000850: 6f64 6520 3d20 666f 726d 732e 4368 6172  ode = forms.Char
-00000860: 4669 656c 6428 6d61 785f 6c65 6e67 7468  Field(max_length
-00000870: 3d31 302c 2077 6964 6765 743d 666f 726d  =10, widget=form
-00000880: 732e 5465 7874 496e 7075 7428 6174 7472  s.TextInput(attr
-00000890: 733d 7b22 706c 6163 6568 6f6c 6465 7222  s={"placeholder"
-000008a0: 3a20 2231 3233 3420 4142 222c 2022 636c  : "1234 AB", "cl
-000008b0: 6173 7322 3a20 2270 6f73 7463 6f64 6522  ass": "postcode"
-000008c0: 2c20 2270 6174 7465 726e 223a 2022 5e5b  , "pattern": "^[
-000008d0: 302d 395d 7b34 7d28 5c73 2b7c 295b 412d  0-9]{4}(\s+|)[A-
-000008e0: 5a5d 7b32 7d24 227d 2929 0d0a 2020 2020  Z]{2}$"}))..    
-000008f0: 686f 6d65 5f6e 756d 6265 7220 3d20 666f  home_number = fo
-00000900: 726d 732e 4368 6172 4669 656c 6428 6d61  rms.CharField(ma
-00000910: 785f 6c65 6e67 7468 3d31 302c 2077 6964  x_length=10, wid
-00000920: 6765 743d 666f 726d 732e 5465 7874 496e  get=forms.TextIn
-00000930: 7075 7428 6174 7472 733d 7b22 706c 6163  put(attrs={"plac
-00000940: 6568 6f6c 6465 7222 3a20 2231 3233 222c  eholder": "123",
-00000950: 2022 636c 6173 7322 3a20 2268 6f6d 655f   "class": "home_
-00000960: 6e75 6d62 6572 227d 2929 0d0a 2020 2020  number"}))..    
-00000970: 0d0a 2020 2020 2320 4375 7374 6f6d 2066  ..    # Custom f
-00000980: 6965 6c64 730d 0a20 2020 2073 7472 6565  ields..    stree
-00000990: 7420 3d20 666f 726d 732e 4368 6172 4669  t = forms.CharFi
-000009a0: 656c 6428 6d61 785f 6c65 6e67 7468 3d32  eld(max_length=2
-000009b0: 3535 2c20 7769 6467 6574 3d66 6f72 6d73  55, widget=forms
+00000540: 6f2d 6465 762e 6e6c 2f29 2e0d 0a0d 0a59  o-dev.nl/).....Y
+00000550: 6f75 206d 7573 7420 6372 6561 7465 2061  ou must create a
+00000560: 6e20 6163 636f 756e 7420 616e 6420 6765  n account and ge
+00000570: 7420 616e 2041 5049 206b 6579 2074 6f20  t an API key to 
+00000580: 7573 6520 7468 6973 2070 6163 6b61 6765  use this package
+00000590: 2028 696e 2074 6865 2064 6566 6175 6c74   (in the default
+000005a0: 2063 6f6e 6669 6775 7261 7469 6f6e 292e   configuration).
+000005b0: 0d0a 0d0a 5468 6973 2041 5049 206b 6579  ....This API key
+000005c0: 206d 7573 7420 6265 2073 6574 2069 6e20   must be set in 
+000005d0: 7468 6520 5b73 6574 7469 6e67 735d 2823  the [settings](#
+000005e0: 7365 7474 696e 6773 292e 0d0a 0d0a 5175  settings).....Qu
+000005f0: 6963 6b20 7374 6172 740d 0a2d 2d2d 2d2d  ick start..-----
+00000600: 2d2d 2d2d 2d2d 0d0a 0d0a 312e 2049 6e73  ------....1. Ins
+00000610: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
+00000620: 2076 6961 2070 6970 3a0d 0a0d 0a20 2020   via pip:....   
+00000630: 6060 6062 6173 680d 0a20 2020 7069 7020  ```bash..   pip 
+00000640: 696e 7374 616c 6c20 646a 616e 676f 2d70  install django-p
+00000650: 6f73 7463 6f64 6573 0d0a 2020 2060 6060  ostcodes..   ```
+00000660: 0d0a 0d0a 322e 2041 6464 2027 706f 7374  ....2. Add 'post
+00000670: 636f 6465 7327 2074 6f20 796f 7572 2049  codes' to your I
+00000680: 4e53 5441 4c4c 4544 5f41 5050 5320 7365  NSTALLED_APPS se
+00000690: 7474 696e 6720 6c69 6b65 2074 6869 733a  tting like this:
+000006a0: 0d0a 0d0a 2020 2060 6060 0d0a 2020 2049  ....   ```..   I
+000006b0: 4e53 5441 4c4c 4544 5f41 5050 5320 3d20  NSTALLED_APPS = 
+000006c0: 5b0d 0a20 2020 2e2e 2e2c 0d0a 2020 2020  [..   ...,..    
+000006d0: 2020 2770 6f73 7463 6f64 6573 272c 0d0a    'postcodes',..
+000006e0: 2020 205d 0d0a 2020 2060 6060 0d0a 332e     ]..   ```..3.
+000006f0: 2041 6464 2074 6865 2070 6f73 7463 6f64   Add the postcod
+00000700: 6573 2055 524c 2074 6f20 796f 7572 2070  es URL to your p
+00000710: 726f 6a65 6374 2773 2060 7572 6c73 2e70  roject's `urls.p
+00000720: 7960 3a0d 0a0d 0a20 2020 6060 6070 7974  y`:....   ```pyt
+00000730: 686f 6e0d 0a20 2020 7061 7468 2827 706f  hon..   path('po
+00000740: 7374 636f 6465 732f 272c 2069 6e63 6c75  stcodes/', inclu
+00000750: 6465 2827 706f 7374 636f 6465 732e 7572  de('postcodes.ur
+00000760: 6c73 272c 206e 616d 6573 7061 6365 3d27  ls', namespace='
+00000770: 706f 7374 636f 6465 7327 2929 2c0d 0a20  postcodes')),.. 
+00000780: 2020 6060 600d 0a0d 0a0d 0a23 2320 4578    ```......## Ex
+00000790: 616d 706c 6520 7573 6167 650d 0a0d 0a46  ample usage....F
+000007a0: 6972 7374 2077 6520 6d75 7374 2064 6566  irst we must def
+000007b0: 696e 6520 7468 6520 6170 7072 6f70 7269  ine the appropri
+000007c0: 6174 6520 666f 726d 2e0d 0a0d 0a54 6869  ate form.....Thi
+000007d0: 7320 6973 2061 6e20 6578 616d 706c 6520  s is an example 
+000007e0: 6f66 2061 2066 6f72 6d20 7468 6174 2075  of a form that u
+000007f0: 7365 7320 7468 6520 6465 6661 756c 7420  ses the default 
+00000800: 4150 4920 656e 6470 6f69 6e74 2028 6375  API endpoint (cu
+00000810: 7374 6f6d 206f 6e65 7320 6361 6e20 6265  stom ones can be
+00000820: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
+00000830: 7365 7474 696e 6773 293a 0d0a 0d0a 4576  settings):....Ev
+00000840: 6572 7920 6174 7472 6962 7574 6520 6361  ery attribute ca
+00000850: 6e20 6265 2063 7573 746f 6d69 7a65 642c  n be customized,
+00000860: 2065 7863 6570 7420 666f 7220 7468 6520   except for the 
+00000870: 706f 7374 636f 6465 2061 6e64 2068 6f6d  postcode and hom
+00000880: 6520 6e75 6d62 6572 2066 6965 6c64 732c  e number fields,
+00000890: 2077 6869 6368 2061 7265 2072 6571 7569   which are requi
+000008a0: 7265 6420 666f 7220 7468 6520 6c6f 6f6b  red for the look
+000008b0: 7570 2e0d 0a0d 0a54 6865 7365 2061 7265  up.....These are
+000008c0: 2068 6172 642d 636f 6465 642e 0d0a 0d0a   hard-coded.....
+000008d0: 416c 6c20 6f74 6865 7220 656c 656d 656e  All other elemen
+000008e0: 7473 2070 726f 7669 6465 6420 696e 2074  ts provided in t
+000008f0: 6865 2060 6269 6e64 6020 6f62 6a65 6374  he `bind` object
+00000900: 2077 696c 6c20 6265 2066 696c 6c65 6420   will be filled 
+00000910: 696e 2077 6974 6820 7468 6520 6461 7461  in with the data
+00000920: 2066 726f 6d20 7468 6520 4150 492e 0d0a   from the API...
+00000930: 0d0a 6060 6070 7974 686f 6e0d 0a63 6c61  ..```python..cla
+00000940: 7373 2041 6464 7265 7373 466f 726d 2866  ss AddressForm(f
+00000950: 6f72 6d73 2e46 6f72 6d29 3a0d 0a20 2020  orms.Form):..   
+00000960: 2023 2054 6865 7365 2061 7265 2072 6571   # These are req
+00000970: 7569 7265 6420 666f 7220 7468 6520 6c6f  uired for the lo
+00000980: 6f6b 7570 0d0a 2020 2020 706f 7374 636f  okup..    postco
+00000990: 6465 203d 2066 6f72 6d73 2e43 6861 7246  de = forms.CharF
+000009a0: 6965 6c64 286d 6178 5f6c 656e 6774 683d  ield(max_length=
+000009b0: 3130 2c20 7769 6467 6574 3d66 6f72 6d73  10, widget=forms
 000009c0: 2e54 6578 7449 6e70 7574 2861 7474 7273  .TextInput(attrs
 000009d0: 3d7b 2270 6c61 6365 686f 6c64 6572 223a  ={"placeholder":
-000009e0: 2022 4d61 696e 2073 7472 6565 7422 2c20   "Main street", 
-000009f0: 2263 6c61 7373 223a 2022 7374 7265 6574  "class": "street
-00000a00: 227d 2929 0d0a 2020 2020 6369 7479 203d  "}))..    city =
-00000a10: 2066 6f72 6d73 2e43 6861 7246 6965 6c64   forms.CharField
-00000a20: 286d 6178 5f6c 656e 6774 683d 3235 352c  (max_length=255,
-00000a30: 2077 6964 6765 743d 666f 726d 732e 5465   widget=forms.Te
-00000a40: 7874 496e 7075 7428 6174 7472 733d 7b22  xtInput(attrs={"
-00000a50: 706c 6163 6568 6f6c 6465 7222 3a20 2241  placeholder": "A
-00000a60: 6d73 7465 7264 616d 222c 2022 636c 6173  msterdam", "clas
-00000a70: 7322 3a20 2263 6974 7922 7d29 290d 0a20  s": "city"})).. 
-00000a80: 2020 206d 756e 6963 6970 616c 6974 7920     municipality 
-00000a90: 3d20 666f 726d 732e 4368 6172 4669 656c  = forms.CharFiel
-00000aa0: 6428 6d61 785f 6c65 6e67 7468 3d32 3535  d(max_length=255
-00000ab0: 2c20 7769 6467 6574 3d66 6f72 6d73 2e54  , widget=forms.T
-00000ac0: 6578 7449 6e70 7574 2861 7474 7273 3d7b  extInput(attrs={
-00000ad0: 2270 6c61 6365 686f 6c64 6572 223a 2022  "placeholder": "
-00000ae0: 416d 7374 6572 6461 6d22 2c20 2263 6c61  Amsterdam", "cla
-00000af0: 7373 223a 2022 6d75 6e69 6369 7061 6c69  ss": "municipali
-00000b00: 7479 227d 2929 0d0a 2020 2020 7072 6f76  ty"}))..    prov
-00000b10: 696e 6365 203d 2066 6f72 6d73 2e43 6861  ince = forms.Cha
-00000b20: 7246 6965 6c64 286d 6178 5f6c 656e 6774  rField(max_lengt
-00000b30: 683d 3235 352c 2077 6964 6765 743d 666f  h=255, widget=fo
-00000b40: 726d 732e 5465 7874 496e 7075 7428 6174  rms.TextInput(at
-00000b50: 7472 733d 7b22 706c 6163 6568 6f6c 6465  trs={"placeholde
-00000b60: 7222 3a20 224e 6f6f 7264 2d48 6f6c 6c61  r": "Noord-Holla
-00000b70: 6e64 222c 2022 636c 6173 7322 3a20 2270  nd", "class": "p
-00000b80: 726f 7669 6e63 6522 7d29 290d 0a20 2020  rovince"}))..   
-00000b90: 2062 7569 6c64 5f79 6561 7220 3d20 666f   build_year = fo
-00000ba0: 726d 732e 496e 7465 6765 7246 6965 6c64  rms.IntegerField
-00000bb0: 2877 6964 6765 743d 666f 726d 732e 4e75  (widget=forms.Nu
-00000bc0: 6d62 6572 496e 7075 7428 6174 7472 733d  mberInput(attrs=
-00000bd0: 7b22 706c 6163 6568 6f6c 6465 7222 3a20  {"placeholder": 
-00000be0: 2231 3939 3022 2c20 2263 6c61 7373 223a  "1990", "class":
-00000bf0: 2022 6275 696c 645f 7965 6172 222c 2022   "build_year", "
-00000c00: 7061 7474 6572 6e22 3a20 225e 5b30 2d39  pattern": "^[0-9
-00000c10: 5d7b 347d 2422 2c20 226d 696e 223a 2022  ]{4}$", "min": "
-00000c20: 3139 3030 222c 2022 6d61 7822 3a20 2232  1900", "max": "2
-00000c30: 3032 3222 7d29 290d 0a20 2020 2066 6c6f  022"}))..    flo
-00000c40: 6f72 5f61 7265 6120 3d20 666f 726d 732e  or_area = forms.
-00000c50: 4465 6369 6d61 6c46 6965 6c64 2877 6964  DecimalField(wid
-00000c60: 6765 743d 666f 726d 732e 4e75 6d62 6572  get=forms.Number
-00000c70: 496e 7075 7428 6174 7472 733d 7b22 706c  Input(attrs={"pl
-00000c80: 6163 6568 6f6c 6465 7222 3a20 2231 3030  aceholder": "100
-00000c90: 222c 2022 636c 6173 7322 3a20 2266 6c6f  ", "class": "flo
-00000ca0: 6f72 5f61 7265 6122 2c20 2270 6174 7465  or_area", "patte
-00000cb0: 726e 223a 2022 5e5b 302d 395d 7b31 2c33  rn": "^[0-9]{1,3
-00000cc0: 7d24 227d 2929 2023 2022 7061 7474 6572  }$"})) # "patter
-00000cd0: 6e22 3a20 225e 5b30 2d39 5d7b 312c 337d  n": "^[0-9]{1,3}
-00000ce0: 2422 0d0a 2020 2020 6765 6f5f 7820 3d20  $"..    geo_x = 
-00000cf0: 666f 726d 732e 4465 6369 6d61 6c46 6965  forms.DecimalFie
-00000d00: 6c64 2877 6964 6765 743d 666f 726d 732e  ld(widget=forms.
-00000d10: 4e75 6d62 6572 496e 7075 7428 6174 7472  NumberInput(attr
-00000d20: 733d 7b22 706c 6163 6568 6f6c 6465 7222  s={"placeholder"
-00000d30: 3a20 2235 322e 3132 3334 3536 222c 2022  : "52.123456", "
-00000d40: 636c 6173 7322 3a20 2267 656f 5f78 227d  class": "geo_x"}
-00000d50: 2929 0d0a 2020 2020 6765 6f5f 7920 3d20  ))..    geo_y = 
-00000d60: 666f 726d 732e 4465 6369 6d61 6c46 6965  forms.DecimalFie
-00000d70: 6c64 2877 6964 6765 743d 666f 726d 732e  ld(widget=forms.
-00000d80: 4e75 6d62 6572 496e 7075 7428 6174 7472  NumberInput(attr
-00000d90: 733d 7b22 706c 6163 6568 6f6c 6465 7222  s={"placeholder"
-00000da0: 3a20 2234 2e31 3233 3435 3622 2c20 2263  : "4.123456", "c
-00000db0: 6c61 7373 223a 2022 6765 6f5f 7922 7d29  lass": "geo_y"})
-00000dc0: 290d 0a20 2020 2072 645f 7820 3d20 666f  )..    rd_x = fo
-00000dd0: 726d 732e 4465 6369 6d61 6c46 6965 6c64  rms.DecimalField
-00000de0: 2877 6964 6765 743d 666f 726d 732e 4e75  (widget=forms.Nu
-00000df0: 6d62 6572 496e 7075 7428 6174 7472 733d  mberInput(attrs=
-00000e00: 7b22 706c 6163 6568 6f6c 6465 7222 3a20  {"placeholder": 
-00000e10: 2231 3233 3435 3622 2c20 2263 6c61 7373  "123456", "class
-00000e20: 223a 2022 7264 5f78 227d 2929 2023 2052  ": "rd_x"})) # R
-00000e30: 696a 6b73 6472 6965 686f 656b 0d0a 2020  ijksdriehoek..  
-00000e40: 2020 7264 5f79 203d 2066 6f72 6d73 2e44    rd_y = forms.D
-00000e50: 6563 696d 616c 4669 656c 6428 7769 6467  ecimalField(widg
-00000e60: 6574 3d66 6f72 6d73 2e4e 756d 6265 7249  et=forms.NumberI
-00000e70: 6e70 7574 2861 7474 7273 3d7b 2270 6c61  nput(attrs={"pla
-00000e80: 6365 686f 6c64 6572 223a 2022 3132 3334  ceholder": "1234
-00000e90: 3536 222c 2022 636c 6173 7322 3a20 2272  56", "class": "r
-00000ea0: 645f 7922 7d29 2920 2320 5269 6a6b 7364  d_y"})) # Rijksd
-00000eb0: 7269 6568 6f65 6b0d 0a60 6060 0d0a 0d0a  riehoek..```....
-00000ec0: 5468 656e 2077 6520 6361 6e20 6465 6669  Then we can defi
-00000ed0: 6e65 206f 7572 2074 656d 706c 6174 650d  ne our template.
-00000ee0: 0a0d 0a60 6060 6874 6d6c 0d0a 7b25 2065  ...```html..{% e
-00000ef0: 7874 656e 6473 2027 6261 7365 2e68 746d  xtends 'base.htm
-00000f00: 6c27 2025 7d0d 0a0d 0a7b 2520 626c 6f63  l' %}....{% bloc
-00000f10: 6b20 636f 6e74 656e 7420 257d 0d0a 2020  k content %}..  
-00000f20: 203c 6c69 6e6b 2072 656c 3d22 7374 796c   <link rel="styl
-00000f30: 6573 6865 6574 2220 6872 6566 3d22 7b25  esheet" href="{%
-00000f40: 2073 7461 7469 6320 2770 6f73 7463 6f64   static 'postcod
-00000f50: 6573 2f63 7373 2f70 6f73 7463 6f64 6573  es/css/postcodes
-00000f60: 2e63 7373 2720 257d 223e 0d0a 2020 203c  .css' %}">..   <
-00000f70: 7363 7269 7074 2073 7263 3d22 7b25 2073  script src="{% s
-00000f80: 7461 7469 6320 2770 6f73 7463 6f64 6573  tatic 'postcodes
-00000f90: 2f6a 732f 706f 7374 636f 6465 732e 6a73  /js/postcodes.js
-00000fa0: 2720 257d 2220 6461 7461 2d61 7069 2d75  ' %}" data-api-u
-00000fb0: 726c 3d22 7b25 2075 726c 2022 706f 7374  rl="{% url "post
-00000fc0: 636f 6465 733a 6170 6922 2025 7d22 3e3c  codes:api" %}"><
-00000fd0: 2f73 6372 6970 743e 0d0a 0d0a 2020 203c  /script>....   <
-00000fe0: 666f 726d 206d 6574 686f 643d 2270 6f73  form method="pos
-00000ff0: 7422 3e0d 0a20 2020 2020 2020 7b25 2063  t">..       {% c
-00001000: 7372 665f 746f 6b65 6e20 257d 0d0a 2020  srf_token %}..  
-00001010: 2020 2020 207b 7b20 666f 726d 2e61 735f       {{ form.as_
-00001020: 7020 7d7d 0d0a 2020 2020 2020 203c 6275  p }}..       <bu
-00001030: 7474 6f6e 2074 7970 653d 2273 7562 6d69  tton type="submi
-00001040: 7422 3e53 7562 6d69 743c 2f62 7574 746f  t">Submit</butto
-00001050: 6e3e 0d0a 2020 203c 2f66 6f72 6d3e 0d0a  n>..   </form>..
-00001060: 0d0a 2020 202e 2e2e 0d0a 0d0a 2020 203c  ..   .......   <
-00001070: 7363 7269 7074 3e0d 0a20 2020 2020 2020  script>..       
-00001080: 646f 6375 6d65 6e74 2e61 6464 4576 656e  document.addEven
-00001090: 744c 6973 7465 6e65 7228 2744 4f4d 436f  tListener('DOMCo
-000010a0: 6e74 656e 744c 6f61 6465 6427 2c20 6675  ntentLoaded', fu
-000010b0: 6e63 7469 6f6e 2829 207b 0d0a 2020 2020  nction() {..    
-000010c0: 2020 2020 2020 206c 6f6f 6b75 7050 6f73         lookupPos
-000010d0: 7463 6f64 6528 7b0d 0a20 2020 2020 2020  tcode({..       
-000010e0: 2020 2020 2020 2020 6269 6e64 3a20 7b0d          bind: {.
-000010f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001100: 2020 2020 2f2f 2054 6865 7365 2061 7265      // These are
-00001110: 2072 6571 7569 7265 6420 666f 7220 7468   required for th
-00001120: 6520 6c6f 6f6b 7570 0d0a 2020 2020 2020  e lookup..      
-00001130: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00001140: 7374 636f 6465 3a20 646f 6375 6d65 6e74  stcode: document
-00001150: 2e71 7565 7279 5365 6c65 6374 6f72 2827  .querySelector('
-00001160: 2369 645f 706f 7374 636f 6465 2729 2c0d  #id_postcode'),.
-00001170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001180: 2020 2020 2068 6f6d 655f 6e75 6d62 6572       home_number
-00001190: 3a20 646f 6375 6d65 6e74 2e71 7565 7279  : document.query
-000011a0: 5365 6c65 6374 6f72 2827 2369 645f 686f  Selector('#id_ho
-000011b0: 6d65 5f6e 756d 6265 7227 292c 0d0a 2020  me_number'),..  
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 2020 2f2f 2043 7573 746f 6d20 6669 656c    // Custom fiel
-000011e0: 6473 2072 6574 7572 6e65 6420 6279 2074  ds returned by t
-000011f0: 6865 2041 5049 0d0a 2020 2020 2020 2020  he API..        
-00001200: 2020 2020 2020 2020 2020 2020 7374 7261              stra
-00001210: 6174 3a20 646f 6375 6d65 6e74 2e71 7565  at: document.que
-00001220: 7279 5365 6c65 6374 6f72 2822 2369 645f  rySelector("#id_
-00001230: 7374 7265 6574 2229 2c0d 0a20 2020 2020  street"),..     
-00001240: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00001250: 6f6f 6e70 6c61 6174 733a 2064 6f63 756d  oonplaats: docum
-00001260: 656e 742e 7175 6572 7953 656c 6563 746f  ent.querySelecto
-00001270: 7228 2223 6964 5f63 6974 7922 292c 0d0a  r("#id_city"),..
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 6765 6d65 656e 7465 3a20 646f      gemeente: do
-000012a0: 6375 6d65 6e74 2e71 7565 7279 5365 6c65  cument.querySele
-000012b0: 6374 6f72 2822 2369 645f 6d75 6e69 6369  ctor("#id_munici
-000012c0: 7061 6c69 7479 2229 2c0d 0a20 2020 2020  pality"),..     
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000012e0: 726f 7669 6e63 6965 3a20 646f 6375 6d65  rovincie: docume
-000012f0: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
-00001300: 2822 2369 645f 7072 6f76 696e 6365 2229  ("#id_province")
-00001310: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001320: 2020 2020 2020 2062 6f75 776a 6161 723a         bouwjaar:
-00001330: 2064 6f63 756d 656e 742e 7175 6572 7953   document.queryS
-00001340: 656c 6563 746f 7228 2223 6964 5f62 7569  elector("#id_bui
-00001350: 6c64 5f79 6561 7222 292c 0d0a 2020 2020  ld_year"),..    
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 766c 6f65 726f 7070 6572 766c 616b 7465  vloeroppervlakte
-00001380: 3a20 646f 6375 6d65 6e74 2e71 7565 7279  : document.query
-00001390: 5365 6c65 6374 6f72 2822 2369 645f 666c  Selector("#id_fl
-000013a0: 6f6f 725f 6172 6561 2229 2c0d 0a20 2020  oor_area"),..   
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013c0: 206c 6174 6974 7564 653a 2064 6f63 756d   latitude: docum
-000013d0: 656e 742e 7175 6572 7953 656c 6563 746f  ent.querySelecto
-000013e0: 7228 2223 6964 5f67 656f 5f78 2229 2c0d  r("#id_geo_x"),.
-000013f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001400: 2020 2020 206c 6f6e 6769 7475 6465 3a20       longitude: 
-00001410: 646f 6375 6d65 6e74 2e71 7565 7279 5365  document.querySe
-00001420: 6c65 6374 6f72 2822 2369 645f 6765 6f5f  lector("#id_geo_
-00001430: 7922 292c 0d0a 2020 2020 2020 2020 2020  y"),..          
-00001440: 2020 2020 2020 2020 2020 7264 5f78 3a20            rd_x: 
-00001450: 646f 6375 6d65 6e74 2e71 7565 7279 5365  document.querySe
-00001460: 6c65 6374 6f72 2822 2369 645f 7264 5f78  lector("#id_rd_x
-00001470: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
-00001480: 2020 2020 2020 2020 2072 645f 793a 2064           rd_y: d
-00001490: 6f63 756d 656e 742e 7175 6572 7953 656c  ocument.querySel
-000014a0: 6563 746f 7228 2223 6964 5f72 645f 7922  ector("#id_rd_y"
-000014b0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000014c0: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
-000014d0: 2020 2020 2020 7375 6363 6573 733a 2066        success: f
-000014e0: 756e 6374 696f 6e28 6164 6472 2920 7b0d  unction(addr) {.
-000014f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001500: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
-00001510: 6164 6472 293b 0d0a 2020 2020 2020 2020  addr);..        
-00001520: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00001530: 2020 2020 2020 2020 2020 6572 726f 723a            error:
-00001540: 2066 756e 6374 696f 6e28 6572 726f 7229   function(error)
-00001550: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00001560: 2020 2020 2020 2063 6f6e 736f 6c65 2e6c         console.l
-00001570: 6f67 2865 7272 6f72 293b 0d0a 2020 2020  og(error);..    
-00001580: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00001590: 2020 2020 2020 2020 207d 290d 0a20 2020           })..   
-000015a0: 2020 2020 7d29 3b0d 0a20 2020 3c2f 7363      });..   </sc
-000015b0: 7269 7074 3e0d 0a0d 0a7b 2520 656e 6462  ript>....{% endb
-000015c0: 6c6f 636b 2025 7d0d 0a60 6060 0d0a 0d0a  lock %}..```....
-000015d0: 5468 6520 666f 726d 2077 696c 6c20 6e6f  The form will no
-000015e0: 7720 6175 746f 6d61 7469 6361 6c6c 7920  w automatically 
-000015f0: 6669 6c6c 2069 6e20 7468 6520 6164 6472  fill in the addr
-00001600: 6573 7320 6669 656c 6473 2077 6865 6e20  ess fields when 
-00001610: 6120 7661 6c69 6420 706f 7374 636f 6465  a valid postcode
-00001620: 2061 6e64 2068 6f6d 6520 6e75 6d62 6572   and home number
-00001630: 2069 7320 656e 7465 7265 642e 0d0a 0d0a   is entered.....
-00001640: 4966 2069 7420 6973 2069 6e76 616c 6964  If it is invalid
-00001650: 206f 7220 6e6f 7420 666f 756e 642c 2074   or not found, t
-00001660: 6865 2065 7272 6f72 2063 616c 6c62 6163  he error callbac
-00001670: 6b20 7769 6c6c 2062 6520 6361 6c6c 6564  k will be called
-00001680: 2e0d 0a0d 0a23 2320 5365 7474 696e 6773  .....## Settings
-00001690: 0d0a 0d0a 2323 2320 6041 4444 525f 5641  ....### `ADDR_VA
-000016a0: 4c49 4441 544f 525f 4150 495f 4b45 5960  LIDATOR_API_KEY`
-000016b0: 0d0a 0d0a 5468 6520 4150 4920 6b65 7920  ....The API key 
-000016c0: 746f 2075 7365 2066 6f72 2074 6865 2070  to use for the p
-000016d0: 6f73 7463 6f64 6520 6c6f 6f6b 7570 2e0d  ostcode lookup..
-000016e0: 0a0d 0a54 6869 7320 7769 6c6c 2062 6520  ...This will be 
-000016f0: 7573 6564 2062 7920 7468 6520 6070 6f73  used by the `pos
-00001700: 7463 6f64 6573 2e70 6f73 7463 6f64 652e  tcodes.postcode.
-00001710: 6164 6472 6573 735f 6368 6563 6b60 2066  address_check` f
-00001720: 756e 6374 696f 6e2e 0d0a 0d0a 0d0a 2323  unction.......##
-00001730: 2320 6041 4444 525f 5641 4c49 4441 544f  # `ADDR_VALIDATO
-00001740: 525f 4150 495f 5552 4c60 0d0a 0d0a 5468  R_API_URL`....Th
-00001750: 6520 4150 4920 5552 4c20 746f 2075 7365  e API URL to use
-00001760: 2066 6f72 2074 6865 2070 6f73 7463 6f64   for the postcod
-00001770: 6520 6c6f 6f6b 7570 2e0d 0a0d 0a54 6869  e lookup.....Thi
-00001780: 7320 7769 6c6c 2062 6520 7573 6564 2062  s will be used b
-00001790: 7920 7468 6520 6070 6f73 7463 6f64 6573  y the `postcodes
-000017a0: 2e70 6f73 7463 6f64 652e 6164 6472 6573  .postcode.addres
-000017b0: 735f 6368 6563 6b60 2066 756e 6374 696f  s_check` functio
-000017c0: 6e2e 0d0a 0d0a 4974 2073 686f 756c 6420  n.....It should 
-000017d0: 636f 6e74 6169 6e20 7468 6520 607b 706f  contain the `{po
-000017e0: 7374 636f 6465 7d60 2061 6e64 2060 7b68  stcode}` and `{h
-000017f0: 6f6d 655f 6e75 6d62 6572 7d60 2070 6c61  ome_number}` pla
-00001800: 6365 686f 6c64 6572 732e 0d0a 0d0a 0d0a  ceholders.......
-00001810: 2323 2320 6041 4444 525f 5641 4c49 4441  ### `ADDR_VALIDA
-00001820: 544f 525f 5041 5241 4d45 5445 525f 464f  TOR_PARAMETER_FO
-00001830: 524d 4154 600d 0a0d 0a41 6e20 6163 7475  RMAT`....An actu
-00001840: 616c 2066 756e 6374 696f 6e20 7468 6174  al function that
-00001850: 2066 6f72 6d61 7473 2074 6865 2070 6172   formats the par
-00001860: 616d 6574 6572 7320 666f 7220 7468 6520  ameters for the 
-00001870: 4150 4920 5552 4c2e 0d0a 0d0a 5468 6973  API URL.....This
-00001880: 206d 6179 206e 6f74 2062 6520 6120 7061   may not be a pa
-00001890: 7468 2074 6f20 6120 6675 6e63 7469 6f6e  th to a function
-000018a0: 2c20 6275 7420 7468 6520 6675 6e63 7469  , but the functi
-000018b0: 6f6e 2069 7473 656c 662e 0d0a 0d0a 4578  on itself.....Ex
-000018c0: 616d 706c 653a 0d0a 0d0a 6060 6070 7974  ample:....```pyt
-000018d0: 686f 6e0d 0a64 6566 2064 6566 6175 6c74  hon..def default
-000018e0: 5f70 6172 616d 6574 6572 5f66 6f72 6d61  _parameter_forma
-000018f0: 7474 6572 282a 2a6b 7761 7267 7329 3a0d  tter(**kwargs):.
-00001900: 0a20 2020 2072 6574 7572 6e20 2226 222e  .    return "&".
-00001910: 6a6f 696e 285b 6622 7b6b 6579 7d3d 7b76  join([f"{key}={v
-00001920: 616c 7565 7d22 2066 6f72 206b 6579 2c20  alue}" for key, 
-00001930: 7661 6c75 6520 696e 206b 7761 7267 732e  value in kwargs.
-00001940: 6974 656d 7328 295d 290d 0a60 6060 0d0a  items()])..```..
-00001950: 0d0a 0d0a 2323 2320 6041 4444 525f 5641  ....### `ADDR_VA
-00001960: 4c49 4441 544f 525f 4552 524f 525f 4154  LIDATOR_ERROR_AT
-00001970: 5452 4942 5554 4560 0d0a 0d0a 5468 6520  TRIBUTE`....The 
-00001980: 6174 7472 6962 7574 6520 696e 2074 6865  attribute in the
-00001990: 2072 6573 706f 6e73 6520 7468 6174 2063   response that c
-000019a0: 6f6e 7461 696e 7320 7468 6520 6572 726f  ontains the erro
-000019b0: 7220 6d65 7373 6167 652e 0d0a 0d0a 5468  r message.....Th
-000019c0: 6973 2077 696c 6c20 6265 2075 7365 6420  is will be used 
-000019d0: 6279 2074 6865 2060 706f 7374 636f 6465  by the `postcode
-000019e0: 732e 706f 7374 636f 6465 2e61 6464 7265  s.postcode.addre
-000019f0: 7373 5f63 6865 636b 6020 6675 6e63 7469  ss_check` functi
-00001a00: 6f6e 2e0d 0a0d 0a41 6464 7265 7373 5661  on.....AddressVa
-00001a10: 6c69 6461 7469 6f6e 4572 726f 7220 6578  lidationError ex
-00001a20: 6365 7074 696f 6e73 2077 696c 6c20 7265  ceptions will re
-00001a30: 7475 726e 2074 6865 2061 7070 726f 7072  turn the appropr
-00001a40: 6961 7465 2065 7272 6f72 206d 6573 7361  iate error messa
-00001a50: 6765 2069 6620 7468 6520 6174 7472 6962  ge if the attrib
-00001a60: 7574 6520 6973 2066 6f75 6e64 2e0d 0a0d  ute is found....
-00001a70: 0a0d 0a23 2323 2060 4144 4452 5f56 414c  ...### `ADDR_VAL
-00001a80: 4944 4154 4f52 5f43 4143 4845 5f54 494d  IDATOR_CACHE_TIM
-00001a90: 454f 5554 600d 0a0d 0a54 6865 2074 696d  EOUT`....The tim
-00001aa0: 656f 7574 2066 6f72 2074 6865 2063 6163  eout for the cac
-00001ab0: 6865 2069 6e20 7365 636f 6e64 732e 0d0a  he in seconds...
-00001ac0: 0d0a 5468 6973 2077 696c 6c20 6265 2075  ..This will be u
-00001ad0: 7365 6420 6279 2074 6865 2060 706f 7374  sed by the `post
-00001ae0: 636f 6465 732e 706f 7374 636f 6465 2e61  codes.postcode.a
-00001af0: 6464 7265 7373 5f63 6865 636b 6020 6675  ddress_check` fu
-00001b00: 6e63 7469 6f6e 2e0d 0a0d 0a49 7420 6973  nction.....It is
-00001b10: 2068 6967 686c 7920 7265 636f 6d6d 656e   highly recommen
-00001b20: 6465 6420 746f 2073 6574 2074 6869 7320  ded to set this 
-00001b30: 746f 2061 2068 6967 6820 6e75 6d62 6572  to a high number
-00001b40: 3b20 6279 2064 6566 6175 6c74 2069 7420  ; by default it 
-00001b50: 6361 6368 6573 2066 6f72 2061 2077 6565  caches for a wee
-00001b60: 6b2e 0d0a 0d0a 5468 6520 6465 6661 756c  k.....The defaul
-00001b70: 7420 656e 6470 6f69 6e74 2069 7320 6672  t endpoint is fr
-00001b80: 6565 2074 6f20 7573 652c 2062 7574 2068  ee to use, but h
-00001b90: 6173 2061 2072 6174 6520 6c69 6d69 742e  as a rate limit.
-00001ba0: 0d0a 0d0a 0d0a 2323 2320 6041 4444 525f  ......### `ADDR_
-00001bb0: 5641 4c49 4441 544f 525f 4150 495f 4b45  VALIDATOR_API_KE
-00001bc0: 595f 4154 5452 4942 5554 4560 0d0a 0d0a  Y_ATTRIBUTE`....
-00001bd0: 5468 6520 6174 7472 6962 7574 6520 696e  The attribute in
-00001be0: 2074 6865 2072 6573 706f 6e73 6520 7468   the response th
-00001bf0: 6174 2063 6f6e 7461 696e 7320 7468 6520  at contains the 
-00001c00: 4150 4920 6b65 792e 0d0a 0d0a 5468 6973  API key.....This
-00001c10: 2077 696c 6c20 6265 2075 7365 6420 6279   will be used by
-00001c20: 2074 6865 2060 706f 7374 636f 6465 732e   the `postcodes.
-00001c30: 706f 7374 636f 6465 2e61 6464 7265 7373  postcode.address
-00001c40: 5f63 6865 636b 6020 6675 6e63 7469 6f6e  _check` function
-00001c50: 2e0d 0a0d 0a49 7420 6973 2074 6865 2068  .....It is the h
-00001c60: 6561 6465 7220 7468 6174 2073 686f 756c  eader that shoul
-00001c70: 6420 6265 2073 656e 7420 7769 7468 2074  d be sent with t
-00001c80: 6865 2072 6571 7565 7374 2e0d 0a0d 0a44  he request.....D
-00001c90: 6566 6175 6c74 7320 746f 2060 582d 4150  efaults to `X-AP
-00001ca0: 492d 546f 6b65 6e60 2e0d 0a0d 0a0d 0a23  I-Token`.......#
-00001cb0: 2323 2060 4144 4452 5f56 414c 4944 4154  ## `ADDR_VALIDAT
-00001cc0: 4f52 5f52 4551 5549 5245 535f 4155 5448  OR_REQUIRES_AUTH
-00001cd0: 600d 0a0d 0a57 6865 7468 6572 2074 6865  `....Whether the
-00001ce0: 2041 5049 2072 6571 7569 7265 7320 6175   API requires au
-00001cf0: 7468 656e 7469 6361 7469 6f6e 2e0d 0a0d  thentication....
-00001d00: 0a54 6869 7320 7769 6c6c 2062 6520 7573  .This will be us
-00001d10: 6564 2062 7920 7468 6520 696e 7465 726e  ed by the intern
-00001d20: 616c 2076 6965 7720 746f 2063 6865 636b  al view to check
-00001d30: 2069 6620 7468 6520 7573 6572 2069 7320   if the user is 
-00001d40: 6175 7468 656e 7469 6361 7465 642e 0d0a  authenticated...
-00001d50: 0d0a 4966 2074 6865 2075 7365 7220 6973  ..If the user is
-00001d60: 2061 7574 6865 6e74 6963 6174 6564 3b20   authenticated; 
-00001d70: 7468 6520 7669 6577 2077 696c 6c20 7265  the view will re
-00001d80: 7475 726e 2074 6865 2061 6464 7265 7373  turn the address
-00001d90: 2064 6174 612e 0d0a 0d0a 5468 6973 2064   data.....This d
-00001da0: 6f65 7320 6e6f 7420 6d61 7474 6572 2069  oes not matter i
-00001db0: 6620 796f 7520 7573 6520 7468 6520 6070  f you use the `p
-00001dc0: 6f73 7463 6f64 6573 2e70 6f73 7463 6f64  ostcodes.postcod
-00001dd0: 652e 6164 6472 6573 735f 6368 6563 6b60  e.address_check`
-00001de0: 2066 756e 6374 696f 6e2e 0d0a             function...
+000009e0: 2022 3132 3334 2041 4222 2c20 2263 6c61   "1234 AB", "cla
+000009f0: 7373 223a 2022 706f 7374 636f 6465 222c  ss": "postcode",
+00000a00: 2022 7061 7474 6572 6e22 3a20 225e 5b30   "pattern": "^[0
+00000a10: 2d39 5d7b 347d 285c 732b 7c29 5b41 2d5a  -9]{4}(\s+|)[A-Z
+00000a20: 5d7b 327d 2422 7d29 290d 0a20 2020 2068  ]{2}$"}))..    h
+00000a30: 6f6d 655f 6e75 6d62 6572 203d 2066 6f72  ome_number = for
+00000a40: 6d73 2e43 6861 7246 6965 6c64 286d 6178  ms.CharField(max
+00000a50: 5f6c 656e 6774 683d 3130 2c20 7769 6467  _length=10, widg
+00000a60: 6574 3d66 6f72 6d73 2e54 6578 7449 6e70  et=forms.TextInp
+00000a70: 7574 2861 7474 7273 3d7b 2270 6c61 6365  ut(attrs={"place
+00000a80: 686f 6c64 6572 223a 2022 3132 3322 2c20  holder": "123", 
+00000a90: 2263 6c61 7373 223a 2022 686f 6d65 5f6e  "class": "home_n
+00000aa0: 756d 6265 7222 7d29 290d 0a20 2020 200d  umber"}))..    .
+00000ab0: 0a20 2020 2023 2043 7573 746f 6d20 6669  .    # Custom fi
+00000ac0: 656c 6473 0d0a 2020 2020 7374 7265 6574  elds..    street
+00000ad0: 203d 2066 6f72 6d73 2e43 6861 7246 6965   = forms.CharFie
+00000ae0: 6c64 286d 6178 5f6c 656e 6774 683d 3235  ld(max_length=25
+00000af0: 352c 2077 6964 6765 743d 666f 726d 732e  5, widget=forms.
+00000b00: 5465 7874 496e 7075 7428 6174 7472 733d  TextInput(attrs=
+00000b10: 7b22 706c 6163 6568 6f6c 6465 7222 3a20  {"placeholder": 
+00000b20: 224d 6169 6e20 7374 7265 6574 222c 2022  "Main street", "
+00000b30: 636c 6173 7322 3a20 2273 7472 6565 7422  class": "street"
+00000b40: 7d29 290d 0a20 2020 2063 6974 7920 3d20  }))..    city = 
+00000b50: 666f 726d 732e 4368 6172 4669 656c 6428  forms.CharField(
+00000b60: 6d61 785f 6c65 6e67 7468 3d32 3535 2c20  max_length=255, 
+00000b70: 7769 6467 6574 3d66 6f72 6d73 2e54 6578  widget=forms.Tex
+00000b80: 7449 6e70 7574 2861 7474 7273 3d7b 2270  tInput(attrs={"p
+00000b90: 6c61 6365 686f 6c64 6572 223a 2022 416d  laceholder": "Am
+00000ba0: 7374 6572 6461 6d22 2c20 2263 6c61 7373  sterdam", "class
+00000bb0: 223a 2022 6369 7479 227d 2929 0d0a 2020  ": "city"}))..  
+00000bc0: 2020 6d75 6e69 6369 7061 6c69 7479 203d    municipality =
+00000bd0: 2066 6f72 6d73 2e43 6861 7246 6965 6c64   forms.CharField
+00000be0: 286d 6178 5f6c 656e 6774 683d 3235 352c  (max_length=255,
+00000bf0: 2077 6964 6765 743d 666f 726d 732e 5465   widget=forms.Te
+00000c00: 7874 496e 7075 7428 6174 7472 733d 7b22  xtInput(attrs={"
+00000c10: 706c 6163 6568 6f6c 6465 7222 3a20 2241  placeholder": "A
+00000c20: 6d73 7465 7264 616d 222c 2022 636c 6173  msterdam", "clas
+00000c30: 7322 3a20 226d 756e 6963 6970 616c 6974  s": "municipalit
+00000c40: 7922 7d29 290d 0a20 2020 2070 726f 7669  y"}))..    provi
+00000c50: 6e63 6520 3d20 666f 726d 732e 4368 6172  nce = forms.Char
+00000c60: 4669 656c 6428 6d61 785f 6c65 6e67 7468  Field(max_length
+00000c70: 3d32 3535 2c20 7769 6467 6574 3d66 6f72  =255, widget=for
+00000c80: 6d73 2e54 6578 7449 6e70 7574 2861 7474  ms.TextInput(att
+00000c90: 7273 3d7b 2270 6c61 6365 686f 6c64 6572  rs={"placeholder
+00000ca0: 223a 2022 4e6f 6f72 642d 486f 6c6c 616e  ": "Noord-Hollan
+00000cb0: 6422 2c20 2263 6c61 7373 223a 2022 7072  d", "class": "pr
+00000cc0: 6f76 696e 6365 227d 2929 0d0a 2020 2020  ovince"}))..    
+00000cd0: 6275 696c 645f 7965 6172 203d 2066 6f72  build_year = for
+00000ce0: 6d73 2e49 6e74 6567 6572 4669 656c 6428  ms.IntegerField(
+00000cf0: 7769 6467 6574 3d66 6f72 6d73 2e4e 756d  widget=forms.Num
+00000d00: 6265 7249 6e70 7574 2861 7474 7273 3d7b  berInput(attrs={
+00000d10: 2270 6c61 6365 686f 6c64 6572 223a 2022  "placeholder": "
+00000d20: 3139 3930 222c 2022 636c 6173 7322 3a20  1990", "class": 
+00000d30: 2262 7569 6c64 5f79 6561 7222 2c20 2270  "build_year", "p
+00000d40: 6174 7465 726e 223a 2022 5e5b 302d 395d  attern": "^[0-9]
+00000d50: 7b34 7d24 222c 2022 6d69 6e22 3a20 2231  {4}$", "min": "1
+00000d60: 3930 3022 2c20 226d 6178 223a 2022 3230  900", "max": "20
+00000d70: 3232 227d 2929 0d0a 2020 2020 666c 6f6f  22"}))..    floo
+00000d80: 725f 6172 6561 203d 2066 6f72 6d73 2e44  r_area = forms.D
+00000d90: 6563 696d 616c 4669 656c 6428 7769 6467  ecimalField(widg
+00000da0: 6574 3d66 6f72 6d73 2e4e 756d 6265 7249  et=forms.NumberI
+00000db0: 6e70 7574 2861 7474 7273 3d7b 2270 6c61  nput(attrs={"pla
+00000dc0: 6365 686f 6c64 6572 223a 2022 3130 3022  ceholder": "100"
+00000dd0: 2c20 2263 6c61 7373 223a 2022 666c 6f6f  , "class": "floo
+00000de0: 725f 6172 6561 222c 2022 7061 7474 6572  r_area", "patter
+00000df0: 6e22 3a20 225e 5b30 2d39 5d7b 312c 337d  n": "^[0-9]{1,3}
+00000e00: 2422 7d29 2920 2320 2270 6174 7465 726e  $"})) # "pattern
+00000e10: 223a 2022 5e5b 302d 395d 7b31 2c33 7d24  ": "^[0-9]{1,3}$
+00000e20: 220d 0a20 2020 2067 656f 5f78 203d 2066  "..    geo_x = f
+00000e30: 6f72 6d73 2e44 6563 696d 616c 4669 656c  orms.DecimalFiel
+00000e40: 6428 7769 6467 6574 3d66 6f72 6d73 2e4e  d(widget=forms.N
+00000e50: 756d 6265 7249 6e70 7574 2861 7474 7273  umberInput(attrs
+00000e60: 3d7b 2270 6c61 6365 686f 6c64 6572 223a  ={"placeholder":
+00000e70: 2022 3532 2e31 3233 3435 3622 2c20 2263   "52.123456", "c
+00000e80: 6c61 7373 223a 2022 6765 6f5f 7822 7d29  lass": "geo_x"})
+00000e90: 290d 0a20 2020 2067 656f 5f79 203d 2066  )..    geo_y = f
+00000ea0: 6f72 6d73 2e44 6563 696d 616c 4669 656c  orms.DecimalFiel
+00000eb0: 6428 7769 6467 6574 3d66 6f72 6d73 2e4e  d(widget=forms.N
+00000ec0: 756d 6265 7249 6e70 7574 2861 7474 7273  umberInput(attrs
+00000ed0: 3d7b 2270 6c61 6365 686f 6c64 6572 223a  ={"placeholder":
+00000ee0: 2022 342e 3132 3334 3536 222c 2022 636c   "4.123456", "cl
+00000ef0: 6173 7322 3a20 2267 656f 5f79 227d 2929  ass": "geo_y"}))
+00000f00: 0d0a 2020 2020 7264 5f78 203d 2066 6f72  ..    rd_x = for
+00000f10: 6d73 2e44 6563 696d 616c 4669 656c 6428  ms.DecimalField(
+00000f20: 7769 6467 6574 3d66 6f72 6d73 2e4e 756d  widget=forms.Num
+00000f30: 6265 7249 6e70 7574 2861 7474 7273 3d7b  berInput(attrs={
+00000f40: 2270 6c61 6365 686f 6c64 6572 223a 2022  "placeholder": "
+00000f50: 3132 3334 3536 222c 2022 636c 6173 7322  123456", "class"
+00000f60: 3a20 2272 645f 7822 7d29 2920 2320 5269  : "rd_x"})) # Ri
+00000f70: 6a6b 7364 7269 6568 6f65 6b0d 0a20 2020  jksdriehoek..   
+00000f80: 2072 645f 7920 3d20 666f 726d 732e 4465   rd_y = forms.De
+00000f90: 6369 6d61 6c46 6965 6c64 2877 6964 6765  cimalField(widge
+00000fa0: 743d 666f 726d 732e 4e75 6d62 6572 496e  t=forms.NumberIn
+00000fb0: 7075 7428 6174 7472 733d 7b22 706c 6163  put(attrs={"plac
+00000fc0: 6568 6f6c 6465 7222 3a20 2231 3233 3435  eholder": "12345
+00000fd0: 3622 2c20 2263 6c61 7373 223a 2022 7264  6", "class": "rd
+00000fe0: 5f79 227d 2929 2023 2052 696a 6b73 6472  _y"})) # Rijksdr
+00000ff0: 6965 686f 656b 0d0a 6060 600d 0a0d 0a54  iehoek..```....T
+00001000: 6865 6e20 7765 2063 616e 2064 6566 696e  hen we can defin
+00001010: 6520 6f75 7220 7465 6d70 6c61 7465 0d0a  e our template..
+00001020: 0d0a 6060 6068 746d 6c0d 0a7b 2520 6578  ..```html..{% ex
+00001030: 7465 6e64 7320 2762 6173 652e 6874 6d6c  tends 'base.html
+00001040: 2720 257d 0d0a 0d0a 7b25 2062 6c6f 636b  ' %}....{% block
+00001050: 2063 6f6e 7465 6e74 2025 7d0d 0a20 2020   content %}..   
+00001060: 3c6c 696e 6b20 7265 6c3d 2273 7479 6c65  <link rel="style
+00001070: 7368 6565 7422 2068 7265 663d 227b 2520  sheet" href="{% 
+00001080: 7374 6174 6963 2027 706f 7374 636f 6465  static 'postcode
+00001090: 732f 6373 732f 706f 7374 636f 6465 732e  s/css/postcodes.
+000010a0: 6373 7327 2025 7d22 3e0d 0a20 2020 3c73  css' %}">..   <s
+000010b0: 6372 6970 7420 7372 633d 227b 2520 7374  cript src="{% st
+000010c0: 6174 6963 2027 706f 7374 636f 6465 732f  atic 'postcodes/
+000010d0: 6a73 2f70 6f73 7463 6f64 6573 2e6a 7327  js/postcodes.js'
+000010e0: 2025 7d22 2064 6174 612d 6170 692d 7572   %}" data-api-ur
+000010f0: 6c3d 227b 2520 7572 6c20 2270 6f73 7463  l="{% url "postc
+00001100: 6f64 6573 3a61 7069 2220 257d 223e 3c2f  odes:api" %}"></
+00001110: 7363 7269 7074 3e0d 0a0d 0a20 2020 3c66  script>....   <f
+00001120: 6f72 6d20 6d65 7468 6f64 3d22 706f 7374  orm method="post
+00001130: 223e 0d0a 2020 2020 2020 207b 2520 6373  ">..       {% cs
+00001140: 7266 5f74 6f6b 656e 2025 7d0d 0a20 2020  rf_token %}..   
+00001150: 2020 2020 7b7b 2066 6f72 6d2e 6173 5f70      {{ form.as_p
+00001160: 207d 7d0d 0a20 2020 2020 2020 3c62 7574   }}..       <but
+00001170: 746f 6e20 7479 7065 3d22 7375 626d 6974  ton type="submit
+00001180: 223e 5375 626d 6974 3c2f 6275 7474 6f6e  ">Submit</button
+00001190: 3e0d 0a20 2020 3c2f 666f 726d 3e0d 0a0d  >..   </form>...
+000011a0: 0a20 2020 2e2e 2e0d 0a0d 0a20 2020 3c73  .   .......   <s
+000011b0: 6372 6970 743e 0d0a 2020 2020 2020 2064  cript>..       d
+000011c0: 6f63 756d 656e 742e 6164 6445 7665 6e74  ocument.addEvent
+000011d0: 4c69 7374 656e 6572 2827 444f 4d43 6f6e  Listener('DOMCon
+000011e0: 7465 6e74 4c6f 6164 6564 272c 2066 756e  tentLoaded', fun
+000011f0: 6374 696f 6e28 2920 7b0d 0a20 2020 2020  ction() {..     
+00001200: 2020 2020 2020 6c6f 6f6b 7570 506f 7374        lookupPost
+00001210: 636f 6465 287b 0d0a 2020 2020 2020 2020  code({..        
+00001220: 2020 2020 2020 2062 696e 643a 207b 0d0a         bind: {..
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 2020 202f 2f20 5468 6573 6520 6172 6520     // These are 
+00001250: 7265 7175 6972 6564 2066 6f72 2074 6865  required for the
+00001260: 206c 6f6f 6b75 700d 0a20 2020 2020 2020   lookup..       
+00001270: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
+00001280: 7463 6f64 653a 2064 6f63 756d 656e 742e  tcode: document.
+00001290: 7175 6572 7953 656c 6563 746f 7228 2723  querySelector('#
+000012a0: 6964 5f70 6f73 7463 6f64 6527 292c 0d0a  id_postcode'),..
+000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012c0: 2020 2020 686f 6d65 5f6e 756d 6265 723a      home_number:
+000012d0: 2064 6f63 756d 656e 742e 7175 6572 7953   document.queryS
+000012e0: 656c 6563 746f 7228 2723 6964 5f68 6f6d  elector('#id_hom
+000012f0: 655f 6e75 6d62 6572 2729 2c0d 0a20 2020  e_number'),..   
+00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001310: 202f 2f20 4375 7374 6f6d 2066 6965 6c64   // Custom field
+00001320: 7320 7265 7475 726e 6564 2062 7920 7468  s returned by th
+00001330: 6520 4150 490d 0a20 2020 2020 2020 2020  e API..         
+00001340: 2020 2020 2020 2020 2020 2073 7472 6161             straa
+00001350: 743a 2064 6f63 756d 656e 742e 7175 6572  t: document.quer
+00001360: 7953 656c 6563 746f 7228 2223 6964 5f73  ySelector("#id_s
+00001370: 7472 6565 7422 292c 0d0a 2020 2020 2020  treet"),..      
+00001380: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+00001390: 6f6e 706c 6161 7473 3a20 646f 6375 6d65  onplaats: docume
+000013a0: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
+000013b0: 2822 2369 645f 6369 7479 2229 2c0d 0a20  ("#id_city"),.. 
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013d0: 2020 2067 656d 6565 6e74 653a 2064 6f63     gemeente: doc
+000013e0: 756d 656e 742e 7175 6572 7953 656c 6563  ument.querySelec
+000013f0: 746f 7228 2223 6964 5f6d 756e 6963 6970  tor("#id_municip
+00001400: 616c 6974 7922 292c 0d0a 2020 2020 2020  ality"),..      
+00001410: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001420: 6f76 696e 6369 653a 2064 6f63 756d 656e  ovincie: documen
+00001430: 742e 7175 6572 7953 656c 6563 746f 7228  t.querySelector(
+00001440: 2223 6964 5f70 726f 7669 6e63 6522 292c  "#id_province"),
+00001450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001460: 2020 2020 2020 626f 7577 6a61 6172 3a20        bouwjaar: 
+00001470: 646f 6375 6d65 6e74 2e71 7565 7279 5365  document.querySe
+00001480: 6c65 6374 6f72 2822 2369 645f 6275 696c  lector("#id_buil
+00001490: 645f 7965 6172 2229 2c0d 0a20 2020 2020  d_year"),..     
+000014a0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000014b0: 6c6f 6572 6f70 7065 7276 6c61 6b74 653a  loeroppervlakte:
+000014c0: 2064 6f63 756d 656e 742e 7175 6572 7953   document.queryS
+000014d0: 656c 6563 746f 7228 2223 6964 5f66 6c6f  elector("#id_flo
+000014e0: 6f72 5f61 7265 6122 292c 0d0a 2020 2020  or_area"),..    
+000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001500: 6c61 7469 7475 6465 3a20 646f 6375 6d65  latitude: docume
+00001510: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
+00001520: 2822 2369 645f 6765 6f5f 7822 292c 0d0a  ("#id_geo_x"),..
+00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001540: 2020 2020 6c6f 6e67 6974 7564 653a 2064      longitude: d
+00001550: 6f63 756d 656e 742e 7175 6572 7953 656c  ocument.querySel
+00001560: 6563 746f 7228 2223 6964 5f67 656f 5f79  ector("#id_geo_y
+00001570: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
+00001580: 2020 2020 2020 2020 2072 645f 783a 2064           rd_x: d
+00001590: 6f63 756d 656e 742e 7175 6572 7953 656c  ocument.querySel
+000015a0: 6563 746f 7228 2223 6964 5f72 645f 7822  ector("#id_rd_x"
+000015b0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+000015c0: 2020 2020 2020 2020 7264 5f79 3a20 646f          rd_y: do
+000015d0: 6375 6d65 6e74 2e71 7565 7279 5365 6c65  cument.querySele
+000015e0: 6374 6f72 2822 2369 645f 7264 5f79 2229  ctor("#id_rd_y")
+000015f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001600: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
+00001610: 2020 2020 2073 7563 6365 7373 3a20 6675       success: fu
+00001620: 6e63 7469 6f6e 2861 6464 7229 207b 0d0a  nction(addr) {..
+00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001640: 2020 2063 6f6e 736f 6c65 2e6c 6f67 2861     console.log(a
+00001650: 6464 7229 3b0d 0a20 2020 2020 2020 2020  ddr);..         
+00001660: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+00001670: 2020 2020 2020 2020 2065 7272 6f72 3a20           error: 
+00001680: 6675 6e63 7469 6f6e 2865 7272 6f72 2920  function(error) 
+00001690: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+000016a0: 2020 2020 2020 636f 6e73 6f6c 652e 6c6f        console.lo
+000016b0: 6728 6572 726f 7229 3b0d 0a20 2020 2020  g(error);..     
+000016c0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+000016d0: 2020 2020 2020 2020 7d29 0d0a 2020 2020          })..    
+000016e0: 2020 207d 293b 0d0a 2020 203c 2f73 6372     });..   </scr
+000016f0: 6970 743e 0d0a 0d0a 7b25 2065 6e64 626c  ipt>....{% endbl
+00001700: 6f63 6b20 257d 0d0a 6060 600d 0a0d 0a54  ock %}..```....T
+00001710: 6865 2066 6f72 6d20 7769 6c6c 206e 6f77  he form will now
+00001720: 2061 7574 6f6d 6174 6963 616c 6c79 2066   automatically f
+00001730: 696c 6c20 696e 2074 6865 2061 6464 7265  ill in the addre
+00001740: 7373 2066 6965 6c64 7320 7768 656e 2061  ss fields when a
+00001750: 2076 616c 6964 2070 6f73 7463 6f64 6520   valid postcode 
+00001760: 616e 6420 686f 6d65 206e 756d 6265 7220  and home number 
+00001770: 6973 2065 6e74 6572 6564 2e0d 0a0d 0a49  is entered.....I
+00001780: 6620 6974 2069 7320 696e 7661 6c69 6420  f it is invalid 
+00001790: 6f72 206e 6f74 2066 6f75 6e64 2c20 7468  or not found, th
+000017a0: 6520 6572 726f 7220 6361 6c6c 6261 636b  e error callback
+000017b0: 2077 696c 6c20 6265 2063 616c 6c65 642e   will be called.
+000017c0: 0d0a 0d0a 2323 2053 6574 7469 6e67 730d  ....## Settings.
+000017d0: 0a0d 0a23 2323 2060 4144 4452 5f56 414c  ...### `ADDR_VAL
+000017e0: 4944 4154 4f52 5f41 5049 5f4b 4559 600d  IDATOR_API_KEY`.
+000017f0: 0a0d 0a54 6865 2041 5049 206b 6579 2074  ...The API key t
+00001800: 6f20 7573 6520 666f 7220 7468 6520 706f  o use for the po
+00001810: 7374 636f 6465 206c 6f6f 6b75 702e 0d0a  stcode lookup...
+00001820: 0d0a 5468 6973 2077 696c 6c20 6265 2075  ..This will be u
+00001830: 7365 6420 6279 2074 6865 2060 706f 7374  sed by the `post
+00001840: 636f 6465 732e 706f 7374 636f 6465 2e61  codes.postcode.a
+00001850: 6464 7265 7373 5f63 6865 636b 6020 6675  ddress_check` fu
+00001860: 6e63 7469 6f6e 2e0d 0a0d 0a0d 0a23 2323  nction.......###
+00001870: 2060 4144 4452 5f56 414c 4944 4154 4f52   `ADDR_VALIDATOR
+00001880: 5f41 5049 5f55 524c 600d 0a0d 0a54 6865  _API_URL`....The
+00001890: 2041 5049 2055 524c 2074 6f20 7573 6520   API URL to use 
+000018a0: 666f 7220 7468 6520 706f 7374 636f 6465  for the postcode
+000018b0: 206c 6f6f 6b75 702e 0d0a 0d0a 5468 6973   lookup.....This
+000018c0: 2077 696c 6c20 6265 2075 7365 6420 6279   will be used by
+000018d0: 2074 6865 2060 706f 7374 636f 6465 732e   the `postcodes.
+000018e0: 706f 7374 636f 6465 2e61 6464 7265 7373  postcode.address
+000018f0: 5f63 6865 636b 6020 6675 6e63 7469 6f6e  _check` function
+00001900: 2e0d 0a0d 0a49 7420 7368 6f75 6c64 2063  .....It should c
+00001910: 6f6e 7461 696e 2074 6865 2060 7b70 6f73  ontain the `{pos
+00001920: 7463 6f64 657d 6020 616e 6420 607b 686f  tcode}` and `{ho
+00001930: 6d65 5f6e 756d 6265 727d 6020 706c 6163  me_number}` plac
+00001940: 6568 6f6c 6465 7273 2e0d 0a0d 0a0d 0a23  eholders.......#
+00001950: 2323 2060 4144 4452 5f56 414c 4944 4154  ## `ADDR_VALIDAT
+00001960: 4f52 5f50 4152 414d 4554 4552 5f46 4f52  OR_PARAMETER_FOR
+00001970: 4d41 5460 0d0a 0d0a 416e 2061 6374 7561  MAT`....An actua
+00001980: 6c20 6675 6e63 7469 6f6e 2074 6861 7420  l function that 
+00001990: 666f 726d 6174 7320 7468 6520 7061 7261  formats the para
+000019a0: 6d65 7465 7273 2066 6f72 2074 6865 2041  meters for the A
+000019b0: 5049 2055 524c 2e0d 0a0d 0a54 6869 7320  PI URL.....This 
+000019c0: 6d61 7920 6e6f 7420 6265 2061 2070 6174  may not be a pat
+000019d0: 6820 746f 2061 2066 756e 6374 696f 6e2c  h to a function,
+000019e0: 2062 7574 2074 6865 2066 756e 6374 696f   but the functio
+000019f0: 6e20 6974 7365 6c66 2e0d 0a0d 0a45 7861  n itself.....Exa
+00001a00: 6d70 6c65 3a0d 0a0d 0a60 6060 7079 7468  mple:....```pyth
+00001a10: 6f6e 0d0a 6465 6620 6465 6661 756c 745f  on..def default_
+00001a20: 7061 7261 6d65 7465 725f 666f 726d 6174  parameter_format
+00001a30: 7465 7228 2a2a 6b77 6172 6773 293a 0d0a  ter(**kwargs):..
+00001a40: 2020 2020 7265 7475 726e 2022 2622 2e6a      return "&".j
+00001a50: 6f69 6e28 5b66 227b 6b65 797d 3d7b 7661  oin([f"{key}={va
+00001a60: 6c75 657d 2220 666f 7220 6b65 792c 2076  lue}" for key, v
+00001a70: 616c 7565 2069 6e20 6b77 6172 6773 2e69  alue in kwargs.i
+00001a80: 7465 6d73 2829 5d29 0d0a 6060 600d 0a0d  tems()])..```...
+00001a90: 0a0d 0a23 2323 2060 4144 4452 5f56 414c  ...### `ADDR_VAL
+00001aa0: 4944 4154 4f52 5f45 5252 4f52 5f41 5454  IDATOR_ERROR_ATT
+00001ab0: 5249 4255 5445 600d 0a0d 0a54 6865 2061  RIBUTE`....The a
+00001ac0: 7474 7269 6275 7465 2069 6e20 7468 6520  ttribute in the 
+00001ad0: 7265 7370 6f6e 7365 2074 6861 7420 636f  response that co
+00001ae0: 6e74 6169 6e73 2074 6865 2065 7272 6f72  ntains the error
+00001af0: 206d 6573 7361 6765 2e0d 0a0d 0a54 6869   message.....Thi
+00001b00: 7320 7769 6c6c 2062 6520 7573 6564 2062  s will be used b
+00001b10: 7920 7468 6520 6070 6f73 7463 6f64 6573  y the `postcodes
+00001b20: 2e70 6f73 7463 6f64 652e 6164 6472 6573  .postcode.addres
+00001b30: 735f 6368 6563 6b60 2066 756e 6374 696f  s_check` functio
+00001b40: 6e2e 0d0a 0d0a 4164 6472 6573 7356 616c  n.....AddressVal
+00001b50: 6964 6174 696f 6e45 7272 6f72 2065 7863  idationError exc
+00001b60: 6570 7469 6f6e 7320 7769 6c6c 2072 6574  eptions will ret
+00001b70: 7572 6e20 7468 6520 6170 7072 6f70 7269  urn the appropri
+00001b80: 6174 6520 6572 726f 7220 6d65 7373 6167  ate error messag
+00001b90: 6520 6966 2074 6865 2061 7474 7269 6275  e if the attribu
+00001ba0: 7465 2069 7320 666f 756e 642e 0d0a 0d0a  te is found.....
+00001bb0: 0d0a 2323 2320 6041 4444 525f 5641 4c49  ..### `ADDR_VALI
+00001bc0: 4441 544f 525f 4341 4348 455f 5449 4d45  DATOR_CACHE_TIME
+00001bd0: 4f55 5460 0d0a 0d0a 5468 6520 7469 6d65  OUT`....The time
+00001be0: 6f75 7420 666f 7220 7468 6520 6361 6368  out for the cach
+00001bf0: 6520 696e 2073 6563 6f6e 6473 2e0d 0a0d  e in seconds....
+00001c00: 0a54 6869 7320 7769 6c6c 2062 6520 7573  .This will be us
+00001c10: 6564 2062 7920 7468 6520 6070 6f73 7463  ed by the `postc
+00001c20: 6f64 6573 2e70 6f73 7463 6f64 652e 6164  odes.postcode.ad
+00001c30: 6472 6573 735f 6368 6563 6b60 2066 756e  dress_check` fun
+00001c40: 6374 696f 6e2e 0d0a 0d0a 4974 2069 7320  ction.....It is 
+00001c50: 6869 6768 6c79 2072 6563 6f6d 6d65 6e64  highly recommend
+00001c60: 6564 2074 6f20 7365 7420 7468 6973 2074  ed to set this t
+00001c70: 6f20 6120 6869 6768 206e 756d 6265 723b  o a high number;
+00001c80: 2062 7920 6465 6661 756c 7420 6974 2063   by default it c
+00001c90: 6163 6865 7320 666f 7220 6120 7765 656b  aches for a week
+00001ca0: 2e0d 0a0d 0a54 6865 2064 6566 6175 6c74  .....The default
+00001cb0: 2065 6e64 706f 696e 7420 6973 2066 7265   endpoint is fre
+00001cc0: 6520 746f 2075 7365 2c20 6275 7420 6861  e to use, but ha
+00001cd0: 7320 6120 7261 7465 206c 696d 6974 2e0d  s a rate limit..
+00001ce0: 0a0d 0a0d 0a23 2323 2060 4144 4452 5f56  .....### `ADDR_V
+00001cf0: 414c 4944 4154 4f52 5f41 5049 5f4b 4559  ALIDATOR_API_KEY
+00001d00: 5f41 5454 5249 4255 5445 600d 0a0d 0a54  _ATTRIBUTE`....T
+00001d10: 6865 2061 7474 7269 6275 7465 2069 6e20  he attribute in 
+00001d20: 7468 6520 7265 7370 6f6e 7365 2074 6861  the response tha
+00001d30: 7420 636f 6e74 6169 6e73 2074 6865 2041  t contains the A
+00001d40: 5049 206b 6579 2e0d 0a0d 0a54 6869 7320  PI key.....This 
+00001d50: 7769 6c6c 2062 6520 7573 6564 2062 7920  will be used by 
+00001d60: 7468 6520 6070 6f73 7463 6f64 6573 2e70  the `postcodes.p
+00001d70: 6f73 7463 6f64 652e 6164 6472 6573 735f  ostcode.address_
+00001d80: 6368 6563 6b60 2066 756e 6374 696f 6e2e  check` function.
+00001d90: 0d0a 0d0a 4974 2069 7320 7468 6520 6865  ....It is the he
+00001da0: 6164 6572 2074 6861 7420 7368 6f75 6c64  ader that should
+00001db0: 2062 6520 7365 6e74 2077 6974 6820 7468   be sent with th
+00001dc0: 6520 7265 7175 6573 742e 0d0a 0d0a 4465  e request.....De
+00001dd0: 6661 756c 7473 2074 6f20 6058 2d41 5049  faults to `X-API
+00001de0: 2d54 6f6b 656e 602e 0d0a 0d0a 0d0a 2323  -Token`.......##
+00001df0: 2320 6041 4444 525f 5641 4c49 4441 544f  # `ADDR_VALIDATO
+00001e00: 525f 5245 5155 4952 4553 5f41 5554 4860  R_REQUIRES_AUTH`
+00001e10: 0d0a 0d0a 5768 6574 6865 7220 7468 6520  ....Whether the 
+00001e20: 4150 4920 7265 7175 6972 6573 2061 7574  API requires aut
+00001e30: 6865 6e74 6963 6174 696f 6e2e 0d0a 0d0a  hentication.....
+00001e40: 5468 6973 2077 696c 6c20 6265 2075 7365  This will be use
+00001e50: 6420 6279 2074 6865 2069 6e74 6572 6e61  d by the interna
+00001e60: 6c20 7669 6577 2074 6f20 6368 6563 6b20  l view to check 
+00001e70: 6966 2074 6865 2075 7365 7220 6973 2061  if the user is a
+00001e80: 7574 6865 6e74 6963 6174 6564 2e0d 0a0d  uthenticated....
+00001e90: 0a49 6620 7468 6520 7573 6572 2069 7320  .If the user is 
+00001ea0: 6175 7468 656e 7469 6361 7465 643b 2074  authenticated; t
+00001eb0: 6865 2076 6965 7720 7769 6c6c 2072 6574  he view will ret
+00001ec0: 7572 6e20 7468 6520 6164 6472 6573 7320  urn the address 
+00001ed0: 6461 7461 2e0d 0a0d 0a54 6869 7320 646f  data.....This do
+00001ee0: 6573 206e 6f74 206d 6174 7465 7220 6966  es not matter if
+00001ef0: 2079 6f75 2075 7365 2074 6865 2060 706f   you use the `po
+00001f00: 7374 636f 6465 732e 706f 7374 636f 6465  stcodes.postcode
+00001f10: 2e61 6464 7265 7373 5f63 6865 636b 6020  .address_check` 
+00001f20: 6675 6e63 7469 6f6e 2e0d 0a              function...
```

### Comparing `django_postcodes-1.0.1/README.md` & `django_postcodes-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 postcodes
 ================
 
 **A dutch postcode lookup app for Django.**
 
 By default we use the free (but rate limited) API from [postcode.go-dev.nl](https://postcode.go-dev.nl/).
 
+You must create an account and get an API key to use this package (in the default configuration).
+
+This API key must be set in the [settings](#settings).
+
 Quick start
 -----------
 
 1. Install the package via pip:
 
    ```bash
-   pip install postcodes
+   pip install django-postcodes
    ```
 
 2. Add 'postcodes' to your INSTALLED_APPS setting like this:
 
    ```
    INSTALLED_APPS = [
    ...,
       'postcodes',
    ]
    ```
+3. Add the postcodes URL to your project's `urls.py`:
+
+   ```python
+   path('postcodes/', include('postcodes.urls', namespace='postcodes')),
+   ```
 
 
 ## Example usage
 
 First we must define the appropriate form.
 
 This is an example of a form that uses the default API endpoint (custom ones can be defined in the settings):
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
 postcodes ================ **A dutch postcode lookup app for Django.** By
 default we use the free (but rate limited) API from [postcode.go-dev.nl](https:
-//postcode.go-dev.nl/). Quick start ----------- 1. Install the package via pip:
-```bash pip install postcodes ``` 2. Add 'postcodes' to your INSTALLED_APPS
-setting like this: ``` INSTALLED_APPS = [ ..., 'postcodes', ] ``` ## Example
-usage First we must define the appropriate form. This is an example of a form
-that uses the default API endpoint (custom ones can be defined in the
+//postcode.go-dev.nl/). You must create an account and get an API key to use
+this package (in the default configuration). This API key must be set in the
+[settings](#settings). Quick start ----------- 1. Install the package via pip:
+```bash pip install django-postcodes ``` 2. Add 'postcodes' to your
+INSTALLED_APPS setting like this: ``` INSTALLED_APPS = [ ..., 'postcodes', ]
+``` 3. Add the postcodes URL to your project's `urls.py`: ```python path
+('postcodes/', include('postcodes.urls', namespace='postcodes')), ``` ##
+Example usage First we must define the appropriate form. This is an example of
+a form that uses the default API endpoint (custom ones can be defined in the
 settings): Every attribute can be customized, except for the postcode and home
 number fields, which are required for the lookup. These are hard-coded. All
 other elements provided in the `bind` object will be filled in with the data
 from the API. ```python class AddressForm(forms.Form): # These are required for
 the lookup postcode = forms.CharField(max_length=10, widget=forms.TextInput
 (attrs={"placeholder": "1234 AB", "class": "postcode", "pattern": "^[0-9]{4}
 (\s+|)[A-Z]{2}$"})) home_number = forms.CharField(max_length=10,
```

### Comparing `django_postcodes-1.0.1/django_postcodes.egg-info/PKG-INFO` & `django_postcodes-1.0.2/django_postcodes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2064 6a61  : 2.1..Name: dja
 00000020: 6e67 6f2d 706f 7374 636f 6465 730d 0a56  ngo-postcodes..V
-00000030: 6572 7369 6f6e 3a20 312e 302e 310d 0a53  ersion: 1.0.1..S
+00000030: 6572 7369 6f6e 3a20 312e 302e 320d 0a53  ersion: 1.0.2..S
 00000040: 756d 6d61 7279 3a20 4120 446a 616e 676f  ummary: A Django
 00000050: 2061 7070 2074 6f20 6d61 6e61 6765 2070   app to manage p
 00000060: 6f73 7463 6f64 652f 686f 6d65 206e 756d  ostcode/home num
 00000070: 6265 7220 6164 6472 6573 7320 666f 726d  ber address form
 00000080: 730d 0a48 6f6d 652d 7061 6765 3a20 6874  s..Home-page: ht
 00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000a0: 2f4e 6967 656c 3233 3932 2f70 6f73 7463  /Nigel2392/postc
@@ -78,402 +78,422 @@
 000004d0: 2066 6f72 2044 6a61 6e67 6f2e 2a2a 0d0a   for Django.**..
 000004e0: 0d0a 4279 2064 6566 6175 6c74 2077 6520  ..By default we 
 000004f0: 7573 6520 7468 6520 6672 6565 2028 6275  use the free (bu
 00000500: 7420 7261 7465 206c 696d 6974 6564 2920  t rate limited) 
 00000510: 4150 4920 6672 6f6d 205b 706f 7374 636f  API from [postco
 00000520: 6465 2e67 6f2d 6465 762e 6e6c 5d28 6874  de.go-dev.nl](ht
 00000530: 7470 733a 2f2f 706f 7374 636f 6465 2e67  tps://postcode.g
-00000540: 6f2d 6465 762e 6e6c 2f29 2e0d 0a0d 0a51  o-dev.nl/).....Q
-00000550: 7569 636b 2073 7461 7274 0d0a 2d2d 2d2d  uick start..----
-00000560: 2d2d 2d2d 2d2d 2d0d 0a0d 0a31 2e20 496e  -------....1. In
-00000570: 7374 616c 6c20 7468 6520 7061 636b 6167  stall the packag
-00000580: 6520 7669 6120 7069 703a 0d0a 0d0a 2020  e via pip:....  
-00000590: 2060 6060 6261 7368 0d0a 2020 2070 6970   ```bash..   pip
-000005a0: 2069 6e73 7461 6c6c 2070 6f73 7463 6f64   install postcod
-000005b0: 6573 0d0a 2020 2060 6060 0d0a 0d0a 322e  es..   ```....2.
-000005c0: 2041 6464 2027 706f 7374 636f 6465 7327   Add 'postcodes'
-000005d0: 2074 6f20 796f 7572 2049 4e53 5441 4c4c   to your INSTALL
-000005e0: 4544 5f41 5050 5320 7365 7474 696e 6720  ED_APPS setting 
-000005f0: 6c69 6b65 2074 6869 733a 0d0a 0d0a 2020  like this:....  
-00000600: 2060 6060 0d0a 2020 2049 4e53 5441 4c4c   ```..   INSTALL
-00000610: 4544 5f41 5050 5320 3d20 5b0d 0a20 2020  ED_APPS = [..   
-00000620: 2e2e 2e2c 0d0a 2020 2020 2020 2770 6f73  ...,..      'pos
-00000630: 7463 6f64 6573 272c 0d0a 2020 205d 0d0a  tcodes',..   ]..
-00000640: 2020 2060 6060 0d0a 0d0a 0d0a 2323 2045     ```......## E
-00000650: 7861 6d70 6c65 2075 7361 6765 0d0a 0d0a  xample usage....
-00000660: 4669 7273 7420 7765 206d 7573 7420 6465  First we must de
-00000670: 6669 6e65 2074 6865 2061 7070 726f 7072  fine the appropr
-00000680: 6961 7465 2066 6f72 6d2e 0d0a 0d0a 5468  iate form.....Th
-00000690: 6973 2069 7320 616e 2065 7861 6d70 6c65  is is an example
-000006a0: 206f 6620 6120 666f 726d 2074 6861 7420   of a form that 
-000006b0: 7573 6573 2074 6865 2064 6566 6175 6c74  uses the default
-000006c0: 2041 5049 2065 6e64 706f 696e 7420 2863   API endpoint (c
-000006d0: 7573 746f 6d20 6f6e 6573 2063 616e 2062  ustom ones can b
-000006e0: 6520 6465 6669 6e65 6420 696e 2074 6865  e defined in the
-000006f0: 2073 6574 7469 6e67 7329 3a0d 0a0d 0a45   settings):....E
-00000700: 7665 7279 2061 7474 7269 6275 7465 2063  very attribute c
-00000710: 616e 2062 6520 6375 7374 6f6d 697a 6564  an be customized
-00000720: 2c20 6578 6365 7074 2066 6f72 2074 6865  , except for the
-00000730: 2070 6f73 7463 6f64 6520 616e 6420 686f   postcode and ho
-00000740: 6d65 206e 756d 6265 7220 6669 656c 6473  me number fields
-00000750: 2c20 7768 6963 6820 6172 6520 7265 7175  , which are requ
-00000760: 6972 6564 2066 6f72 2074 6865 206c 6f6f  ired for the loo
-00000770: 6b75 702e 0d0a 0d0a 5468 6573 6520 6172  kup.....These ar
-00000780: 6520 6861 7264 2d63 6f64 6564 2e0d 0a0d  e hard-coded....
-00000790: 0a41 6c6c 206f 7468 6572 2065 6c65 6d65  .All other eleme
-000007a0: 6e74 7320 7072 6f76 6964 6564 2069 6e20  nts provided in 
-000007b0: 7468 6520 6062 696e 6460 206f 626a 6563  the `bind` objec
-000007c0: 7420 7769 6c6c 2062 6520 6669 6c6c 6564  t will be filled
-000007d0: 2069 6e20 7769 7468 2074 6865 2064 6174   in with the dat
-000007e0: 6120 6672 6f6d 2074 6865 2041 5049 2e0d  a from the API..
-000007f0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 636c  ...```python..cl
-00000800: 6173 7320 4164 6472 6573 7346 6f72 6d28  ass AddressForm(
-00000810: 666f 726d 732e 466f 726d 293a 0d0a 2020  forms.Form):..  
-00000820: 2020 2320 5468 6573 6520 6172 6520 7265    # These are re
-00000830: 7175 6972 6564 2066 6f72 2074 6865 206c  quired for the l
-00000840: 6f6f 6b75 700d 0a20 2020 2070 6f73 7463  ookup..    postc
-00000850: 6f64 6520 3d20 666f 726d 732e 4368 6172  ode = forms.Char
-00000860: 4669 656c 6428 6d61 785f 6c65 6e67 7468  Field(max_length
-00000870: 3d31 302c 2077 6964 6765 743d 666f 726d  =10, widget=form
-00000880: 732e 5465 7874 496e 7075 7428 6174 7472  s.TextInput(attr
-00000890: 733d 7b22 706c 6163 6568 6f6c 6465 7222  s={"placeholder"
-000008a0: 3a20 2231 3233 3420 4142 222c 2022 636c  : "1234 AB", "cl
-000008b0: 6173 7322 3a20 2270 6f73 7463 6f64 6522  ass": "postcode"
-000008c0: 2c20 2270 6174 7465 726e 223a 2022 5e5b  , "pattern": "^[
-000008d0: 302d 395d 7b34 7d28 5c73 2b7c 295b 412d  0-9]{4}(\s+|)[A-
-000008e0: 5a5d 7b32 7d24 227d 2929 0d0a 2020 2020  Z]{2}$"}))..    
-000008f0: 686f 6d65 5f6e 756d 6265 7220 3d20 666f  home_number = fo
-00000900: 726d 732e 4368 6172 4669 656c 6428 6d61  rms.CharField(ma
-00000910: 785f 6c65 6e67 7468 3d31 302c 2077 6964  x_length=10, wid
-00000920: 6765 743d 666f 726d 732e 5465 7874 496e  get=forms.TextIn
-00000930: 7075 7428 6174 7472 733d 7b22 706c 6163  put(attrs={"plac
-00000940: 6568 6f6c 6465 7222 3a20 2231 3233 222c  eholder": "123",
-00000950: 2022 636c 6173 7322 3a20 2268 6f6d 655f   "class": "home_
-00000960: 6e75 6d62 6572 227d 2929 0d0a 2020 2020  number"}))..    
-00000970: 0d0a 2020 2020 2320 4375 7374 6f6d 2066  ..    # Custom f
-00000980: 6965 6c64 730d 0a20 2020 2073 7472 6565  ields..    stree
-00000990: 7420 3d20 666f 726d 732e 4368 6172 4669  t = forms.CharFi
-000009a0: 656c 6428 6d61 785f 6c65 6e67 7468 3d32  eld(max_length=2
-000009b0: 3535 2c20 7769 6467 6574 3d66 6f72 6d73  55, widget=forms
+00000540: 6f2d 6465 762e 6e6c 2f29 2e0d 0a0d 0a59  o-dev.nl/).....Y
+00000550: 6f75 206d 7573 7420 6372 6561 7465 2061  ou must create a
+00000560: 6e20 6163 636f 756e 7420 616e 6420 6765  n account and ge
+00000570: 7420 616e 2041 5049 206b 6579 2074 6f20  t an API key to 
+00000580: 7573 6520 7468 6973 2070 6163 6b61 6765  use this package
+00000590: 2028 696e 2074 6865 2064 6566 6175 6c74   (in the default
+000005a0: 2063 6f6e 6669 6775 7261 7469 6f6e 292e   configuration).
+000005b0: 0d0a 0d0a 5468 6973 2041 5049 206b 6579  ....This API key
+000005c0: 206d 7573 7420 6265 2073 6574 2069 6e20   must be set in 
+000005d0: 7468 6520 5b73 6574 7469 6e67 735d 2823  the [settings](#
+000005e0: 7365 7474 696e 6773 292e 0d0a 0d0a 5175  settings).....Qu
+000005f0: 6963 6b20 7374 6172 740d 0a2d 2d2d 2d2d  ick start..-----
+00000600: 2d2d 2d2d 2d2d 0d0a 0d0a 312e 2049 6e73  ------....1. Ins
+00000610: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
+00000620: 2076 6961 2070 6970 3a0d 0a0d 0a20 2020   via pip:....   
+00000630: 6060 6062 6173 680d 0a20 2020 7069 7020  ```bash..   pip 
+00000640: 696e 7374 616c 6c20 646a 616e 676f 2d70  install django-p
+00000650: 6f73 7463 6f64 6573 0d0a 2020 2060 6060  ostcodes..   ```
+00000660: 0d0a 0d0a 322e 2041 6464 2027 706f 7374  ....2. Add 'post
+00000670: 636f 6465 7327 2074 6f20 796f 7572 2049  codes' to your I
+00000680: 4e53 5441 4c4c 4544 5f41 5050 5320 7365  NSTALLED_APPS se
+00000690: 7474 696e 6720 6c69 6b65 2074 6869 733a  tting like this:
+000006a0: 0d0a 0d0a 2020 2060 6060 0d0a 2020 2049  ....   ```..   I
+000006b0: 4e53 5441 4c4c 4544 5f41 5050 5320 3d20  NSTALLED_APPS = 
+000006c0: 5b0d 0a20 2020 2e2e 2e2c 0d0a 2020 2020  [..   ...,..    
+000006d0: 2020 2770 6f73 7463 6f64 6573 272c 0d0a    'postcodes',..
+000006e0: 2020 205d 0d0a 2020 2060 6060 0d0a 332e     ]..   ```..3.
+000006f0: 2041 6464 2074 6865 2070 6f73 7463 6f64   Add the postcod
+00000700: 6573 2055 524c 2074 6f20 796f 7572 2070  es URL to your p
+00000710: 726f 6a65 6374 2773 2060 7572 6c73 2e70  roject's `urls.p
+00000720: 7960 3a0d 0a0d 0a20 2020 6060 6070 7974  y`:....   ```pyt
+00000730: 686f 6e0d 0a20 2020 7061 7468 2827 706f  hon..   path('po
+00000740: 7374 636f 6465 732f 272c 2069 6e63 6c75  stcodes/', inclu
+00000750: 6465 2827 706f 7374 636f 6465 732e 7572  de('postcodes.ur
+00000760: 6c73 272c 206e 616d 6573 7061 6365 3d27  ls', namespace='
+00000770: 706f 7374 636f 6465 7327 2929 2c0d 0a20  postcodes')),.. 
+00000780: 2020 6060 600d 0a0d 0a0d 0a23 2320 4578    ```......## Ex
+00000790: 616d 706c 6520 7573 6167 650d 0a0d 0a46  ample usage....F
+000007a0: 6972 7374 2077 6520 6d75 7374 2064 6566  irst we must def
+000007b0: 696e 6520 7468 6520 6170 7072 6f70 7269  ine the appropri
+000007c0: 6174 6520 666f 726d 2e0d 0a0d 0a54 6869  ate form.....Thi
+000007d0: 7320 6973 2061 6e20 6578 616d 706c 6520  s is an example 
+000007e0: 6f66 2061 2066 6f72 6d20 7468 6174 2075  of a form that u
+000007f0: 7365 7320 7468 6520 6465 6661 756c 7420  ses the default 
+00000800: 4150 4920 656e 6470 6f69 6e74 2028 6375  API endpoint (cu
+00000810: 7374 6f6d 206f 6e65 7320 6361 6e20 6265  stom ones can be
+00000820: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
+00000830: 7365 7474 696e 6773 293a 0d0a 0d0a 4576  settings):....Ev
+00000840: 6572 7920 6174 7472 6962 7574 6520 6361  ery attribute ca
+00000850: 6e20 6265 2063 7573 746f 6d69 7a65 642c  n be customized,
+00000860: 2065 7863 6570 7420 666f 7220 7468 6520   except for the 
+00000870: 706f 7374 636f 6465 2061 6e64 2068 6f6d  postcode and hom
+00000880: 6520 6e75 6d62 6572 2066 6965 6c64 732c  e number fields,
+00000890: 2077 6869 6368 2061 7265 2072 6571 7569   which are requi
+000008a0: 7265 6420 666f 7220 7468 6520 6c6f 6f6b  red for the look
+000008b0: 7570 2e0d 0a0d 0a54 6865 7365 2061 7265  up.....These are
+000008c0: 2068 6172 642d 636f 6465 642e 0d0a 0d0a   hard-coded.....
+000008d0: 416c 6c20 6f74 6865 7220 656c 656d 656e  All other elemen
+000008e0: 7473 2070 726f 7669 6465 6420 696e 2074  ts provided in t
+000008f0: 6865 2060 6269 6e64 6020 6f62 6a65 6374  he `bind` object
+00000900: 2077 696c 6c20 6265 2066 696c 6c65 6420   will be filled 
+00000910: 696e 2077 6974 6820 7468 6520 6461 7461  in with the data
+00000920: 2066 726f 6d20 7468 6520 4150 492e 0d0a   from the API...
+00000930: 0d0a 6060 6070 7974 686f 6e0d 0a63 6c61  ..```python..cla
+00000940: 7373 2041 6464 7265 7373 466f 726d 2866  ss AddressForm(f
+00000950: 6f72 6d73 2e46 6f72 6d29 3a0d 0a20 2020  orms.Form):..   
+00000960: 2023 2054 6865 7365 2061 7265 2072 6571   # These are req
+00000970: 7569 7265 6420 666f 7220 7468 6520 6c6f  uired for the lo
+00000980: 6f6b 7570 0d0a 2020 2020 706f 7374 636f  okup..    postco
+00000990: 6465 203d 2066 6f72 6d73 2e43 6861 7246  de = forms.CharF
+000009a0: 6965 6c64 286d 6178 5f6c 656e 6774 683d  ield(max_length=
+000009b0: 3130 2c20 7769 6467 6574 3d66 6f72 6d73  10, widget=forms
 000009c0: 2e54 6578 7449 6e70 7574 2861 7474 7273  .TextInput(attrs
 000009d0: 3d7b 2270 6c61 6365 686f 6c64 6572 223a  ={"placeholder":
-000009e0: 2022 4d61 696e 2073 7472 6565 7422 2c20   "Main street", 
-000009f0: 2263 6c61 7373 223a 2022 7374 7265 6574  "class": "street
-00000a00: 227d 2929 0d0a 2020 2020 6369 7479 203d  "}))..    city =
-00000a10: 2066 6f72 6d73 2e43 6861 7246 6965 6c64   forms.CharField
-00000a20: 286d 6178 5f6c 656e 6774 683d 3235 352c  (max_length=255,
-00000a30: 2077 6964 6765 743d 666f 726d 732e 5465   widget=forms.Te
-00000a40: 7874 496e 7075 7428 6174 7472 733d 7b22  xtInput(attrs={"
-00000a50: 706c 6163 6568 6f6c 6465 7222 3a20 2241  placeholder": "A
-00000a60: 6d73 7465 7264 616d 222c 2022 636c 6173  msterdam", "clas
-00000a70: 7322 3a20 2263 6974 7922 7d29 290d 0a20  s": "city"})).. 
-00000a80: 2020 206d 756e 6963 6970 616c 6974 7920     municipality 
-00000a90: 3d20 666f 726d 732e 4368 6172 4669 656c  = forms.CharFiel
-00000aa0: 6428 6d61 785f 6c65 6e67 7468 3d32 3535  d(max_length=255
-00000ab0: 2c20 7769 6467 6574 3d66 6f72 6d73 2e54  , widget=forms.T
-00000ac0: 6578 7449 6e70 7574 2861 7474 7273 3d7b  extInput(attrs={
-00000ad0: 2270 6c61 6365 686f 6c64 6572 223a 2022  "placeholder": "
-00000ae0: 416d 7374 6572 6461 6d22 2c20 2263 6c61  Amsterdam", "cla
-00000af0: 7373 223a 2022 6d75 6e69 6369 7061 6c69  ss": "municipali
-00000b00: 7479 227d 2929 0d0a 2020 2020 7072 6f76  ty"}))..    prov
-00000b10: 696e 6365 203d 2066 6f72 6d73 2e43 6861  ince = forms.Cha
-00000b20: 7246 6965 6c64 286d 6178 5f6c 656e 6774  rField(max_lengt
-00000b30: 683d 3235 352c 2077 6964 6765 743d 666f  h=255, widget=fo
-00000b40: 726d 732e 5465 7874 496e 7075 7428 6174  rms.TextInput(at
-00000b50: 7472 733d 7b22 706c 6163 6568 6f6c 6465  trs={"placeholde
-00000b60: 7222 3a20 224e 6f6f 7264 2d48 6f6c 6c61  r": "Noord-Holla
-00000b70: 6e64 222c 2022 636c 6173 7322 3a20 2270  nd", "class": "p
-00000b80: 726f 7669 6e63 6522 7d29 290d 0a20 2020  rovince"}))..   
-00000b90: 2062 7569 6c64 5f79 6561 7220 3d20 666f   build_year = fo
-00000ba0: 726d 732e 496e 7465 6765 7246 6965 6c64  rms.IntegerField
-00000bb0: 2877 6964 6765 743d 666f 726d 732e 4e75  (widget=forms.Nu
-00000bc0: 6d62 6572 496e 7075 7428 6174 7472 733d  mberInput(attrs=
-00000bd0: 7b22 706c 6163 6568 6f6c 6465 7222 3a20  {"placeholder": 
-00000be0: 2231 3939 3022 2c20 2263 6c61 7373 223a  "1990", "class":
-00000bf0: 2022 6275 696c 645f 7965 6172 222c 2022   "build_year", "
-00000c00: 7061 7474 6572 6e22 3a20 225e 5b30 2d39  pattern": "^[0-9
-00000c10: 5d7b 347d 2422 2c20 226d 696e 223a 2022  ]{4}$", "min": "
-00000c20: 3139 3030 222c 2022 6d61 7822 3a20 2232  1900", "max": "2
-00000c30: 3032 3222 7d29 290d 0a20 2020 2066 6c6f  022"}))..    flo
-00000c40: 6f72 5f61 7265 6120 3d20 666f 726d 732e  or_area = forms.
-00000c50: 4465 6369 6d61 6c46 6965 6c64 2877 6964  DecimalField(wid
-00000c60: 6765 743d 666f 726d 732e 4e75 6d62 6572  get=forms.Number
-00000c70: 496e 7075 7428 6174 7472 733d 7b22 706c  Input(attrs={"pl
-00000c80: 6163 6568 6f6c 6465 7222 3a20 2231 3030  aceholder": "100
-00000c90: 222c 2022 636c 6173 7322 3a20 2266 6c6f  ", "class": "flo
-00000ca0: 6f72 5f61 7265 6122 2c20 2270 6174 7465  or_area", "patte
-00000cb0: 726e 223a 2022 5e5b 302d 395d 7b31 2c33  rn": "^[0-9]{1,3
-00000cc0: 7d24 227d 2929 2023 2022 7061 7474 6572  }$"})) # "patter
-00000cd0: 6e22 3a20 225e 5b30 2d39 5d7b 312c 337d  n": "^[0-9]{1,3}
-00000ce0: 2422 0d0a 2020 2020 6765 6f5f 7820 3d20  $"..    geo_x = 
-00000cf0: 666f 726d 732e 4465 6369 6d61 6c46 6965  forms.DecimalFie
-00000d00: 6c64 2877 6964 6765 743d 666f 726d 732e  ld(widget=forms.
-00000d10: 4e75 6d62 6572 496e 7075 7428 6174 7472  NumberInput(attr
-00000d20: 733d 7b22 706c 6163 6568 6f6c 6465 7222  s={"placeholder"
-00000d30: 3a20 2235 322e 3132 3334 3536 222c 2022  : "52.123456", "
-00000d40: 636c 6173 7322 3a20 2267 656f 5f78 227d  class": "geo_x"}
-00000d50: 2929 0d0a 2020 2020 6765 6f5f 7920 3d20  ))..    geo_y = 
-00000d60: 666f 726d 732e 4465 6369 6d61 6c46 6965  forms.DecimalFie
-00000d70: 6c64 2877 6964 6765 743d 666f 726d 732e  ld(widget=forms.
-00000d80: 4e75 6d62 6572 496e 7075 7428 6174 7472  NumberInput(attr
-00000d90: 733d 7b22 706c 6163 6568 6f6c 6465 7222  s={"placeholder"
-00000da0: 3a20 2234 2e31 3233 3435 3622 2c20 2263  : "4.123456", "c
-00000db0: 6c61 7373 223a 2022 6765 6f5f 7922 7d29  lass": "geo_y"})
-00000dc0: 290d 0a20 2020 2072 645f 7820 3d20 666f  )..    rd_x = fo
-00000dd0: 726d 732e 4465 6369 6d61 6c46 6965 6c64  rms.DecimalField
-00000de0: 2877 6964 6765 743d 666f 726d 732e 4e75  (widget=forms.Nu
-00000df0: 6d62 6572 496e 7075 7428 6174 7472 733d  mberInput(attrs=
-00000e00: 7b22 706c 6163 6568 6f6c 6465 7222 3a20  {"placeholder": 
-00000e10: 2231 3233 3435 3622 2c20 2263 6c61 7373  "123456", "class
-00000e20: 223a 2022 7264 5f78 227d 2929 2023 2052  ": "rd_x"})) # R
-00000e30: 696a 6b73 6472 6965 686f 656b 0d0a 2020  ijksdriehoek..  
-00000e40: 2020 7264 5f79 203d 2066 6f72 6d73 2e44    rd_y = forms.D
-00000e50: 6563 696d 616c 4669 656c 6428 7769 6467  ecimalField(widg
-00000e60: 6574 3d66 6f72 6d73 2e4e 756d 6265 7249  et=forms.NumberI
-00000e70: 6e70 7574 2861 7474 7273 3d7b 2270 6c61  nput(attrs={"pla
-00000e80: 6365 686f 6c64 6572 223a 2022 3132 3334  ceholder": "1234
-00000e90: 3536 222c 2022 636c 6173 7322 3a20 2272  56", "class": "r
-00000ea0: 645f 7922 7d29 2920 2320 5269 6a6b 7364  d_y"})) # Rijksd
-00000eb0: 7269 6568 6f65 6b0d 0a60 6060 0d0a 0d0a  riehoek..```....
-00000ec0: 5468 656e 2077 6520 6361 6e20 6465 6669  Then we can defi
-00000ed0: 6e65 206f 7572 2074 656d 706c 6174 650d  ne our template.
-00000ee0: 0a0d 0a60 6060 6874 6d6c 0d0a 7b25 2065  ...```html..{% e
-00000ef0: 7874 656e 6473 2027 6261 7365 2e68 746d  xtends 'base.htm
-00000f00: 6c27 2025 7d0d 0a0d 0a7b 2520 626c 6f63  l' %}....{% bloc
-00000f10: 6b20 636f 6e74 656e 7420 257d 0d0a 2020  k content %}..  
-00000f20: 203c 6c69 6e6b 2072 656c 3d22 7374 796c   <link rel="styl
-00000f30: 6573 6865 6574 2220 6872 6566 3d22 7b25  esheet" href="{%
-00000f40: 2073 7461 7469 6320 2770 6f73 7463 6f64   static 'postcod
-00000f50: 6573 2f63 7373 2f70 6f73 7463 6f64 6573  es/css/postcodes
-00000f60: 2e63 7373 2720 257d 223e 0d0a 2020 203c  .css' %}">..   <
-00000f70: 7363 7269 7074 2073 7263 3d22 7b25 2073  script src="{% s
-00000f80: 7461 7469 6320 2770 6f73 7463 6f64 6573  tatic 'postcodes
-00000f90: 2f6a 732f 706f 7374 636f 6465 732e 6a73  /js/postcodes.js
-00000fa0: 2720 257d 2220 6461 7461 2d61 7069 2d75  ' %}" data-api-u
-00000fb0: 726c 3d22 7b25 2075 726c 2022 706f 7374  rl="{% url "post
-00000fc0: 636f 6465 733a 6170 6922 2025 7d22 3e3c  codes:api" %}"><
-00000fd0: 2f73 6372 6970 743e 0d0a 0d0a 2020 203c  /script>....   <
-00000fe0: 666f 726d 206d 6574 686f 643d 2270 6f73  form method="pos
-00000ff0: 7422 3e0d 0a20 2020 2020 2020 7b25 2063  t">..       {% c
-00001000: 7372 665f 746f 6b65 6e20 257d 0d0a 2020  srf_token %}..  
-00001010: 2020 2020 207b 7b20 666f 726d 2e61 735f       {{ form.as_
-00001020: 7020 7d7d 0d0a 2020 2020 2020 203c 6275  p }}..       <bu
-00001030: 7474 6f6e 2074 7970 653d 2273 7562 6d69  tton type="submi
-00001040: 7422 3e53 7562 6d69 743c 2f62 7574 746f  t">Submit</butto
-00001050: 6e3e 0d0a 2020 203c 2f66 6f72 6d3e 0d0a  n>..   </form>..
-00001060: 0d0a 2020 202e 2e2e 0d0a 0d0a 2020 203c  ..   .......   <
-00001070: 7363 7269 7074 3e0d 0a20 2020 2020 2020  script>..       
-00001080: 646f 6375 6d65 6e74 2e61 6464 4576 656e  document.addEven
-00001090: 744c 6973 7465 6e65 7228 2744 4f4d 436f  tListener('DOMCo
-000010a0: 6e74 656e 744c 6f61 6465 6427 2c20 6675  ntentLoaded', fu
-000010b0: 6e63 7469 6f6e 2829 207b 0d0a 2020 2020  nction() {..    
-000010c0: 2020 2020 2020 206c 6f6f 6b75 7050 6f73         lookupPos
-000010d0: 7463 6f64 6528 7b0d 0a20 2020 2020 2020  tcode({..       
-000010e0: 2020 2020 2020 2020 6269 6e64 3a20 7b0d          bind: {.
-000010f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001100: 2020 2020 2f2f 2054 6865 7365 2061 7265      // These are
-00001110: 2072 6571 7569 7265 6420 666f 7220 7468   required for th
-00001120: 6520 6c6f 6f6b 7570 0d0a 2020 2020 2020  e lookup..      
-00001130: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00001140: 7374 636f 6465 3a20 646f 6375 6d65 6e74  stcode: document
-00001150: 2e71 7565 7279 5365 6c65 6374 6f72 2827  .querySelector('
-00001160: 2369 645f 706f 7374 636f 6465 2729 2c0d  #id_postcode'),.
-00001170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001180: 2020 2020 2068 6f6d 655f 6e75 6d62 6572       home_number
-00001190: 3a20 646f 6375 6d65 6e74 2e71 7565 7279  : document.query
-000011a0: 5365 6c65 6374 6f72 2827 2369 645f 686f  Selector('#id_ho
-000011b0: 6d65 5f6e 756d 6265 7227 292c 0d0a 2020  me_number'),..  
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 2020 2f2f 2043 7573 746f 6d20 6669 656c    // Custom fiel
-000011e0: 6473 2072 6574 7572 6e65 6420 6279 2074  ds returned by t
-000011f0: 6865 2041 5049 0d0a 2020 2020 2020 2020  he API..        
-00001200: 2020 2020 2020 2020 2020 2020 7374 7261              stra
-00001210: 6174 3a20 646f 6375 6d65 6e74 2e71 7565  at: document.que
-00001220: 7279 5365 6c65 6374 6f72 2822 2369 645f  rySelector("#id_
-00001230: 7374 7265 6574 2229 2c0d 0a20 2020 2020  street"),..     
-00001240: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00001250: 6f6f 6e70 6c61 6174 733a 2064 6f63 756d  oonplaats: docum
-00001260: 656e 742e 7175 6572 7953 656c 6563 746f  ent.querySelecto
-00001270: 7228 2223 6964 5f63 6974 7922 292c 0d0a  r("#id_city"),..
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 6765 6d65 656e 7465 3a20 646f      gemeente: do
-000012a0: 6375 6d65 6e74 2e71 7565 7279 5365 6c65  cument.querySele
-000012b0: 6374 6f72 2822 2369 645f 6d75 6e69 6369  ctor("#id_munici
-000012c0: 7061 6c69 7479 2229 2c0d 0a20 2020 2020  pality"),..     
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000012e0: 726f 7669 6e63 6965 3a20 646f 6375 6d65  rovincie: docume
-000012f0: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
-00001300: 2822 2369 645f 7072 6f76 696e 6365 2229  ("#id_province")
-00001310: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001320: 2020 2020 2020 2062 6f75 776a 6161 723a         bouwjaar:
-00001330: 2064 6f63 756d 656e 742e 7175 6572 7953   document.queryS
-00001340: 656c 6563 746f 7228 2223 6964 5f62 7569  elector("#id_bui
-00001350: 6c64 5f79 6561 7222 292c 0d0a 2020 2020  ld_year"),..    
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 766c 6f65 726f 7070 6572 766c 616b 7465  vloeroppervlakte
-00001380: 3a20 646f 6375 6d65 6e74 2e71 7565 7279  : document.query
-00001390: 5365 6c65 6374 6f72 2822 2369 645f 666c  Selector("#id_fl
-000013a0: 6f6f 725f 6172 6561 2229 2c0d 0a20 2020  oor_area"),..   
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013c0: 206c 6174 6974 7564 653a 2064 6f63 756d   latitude: docum
-000013d0: 656e 742e 7175 6572 7953 656c 6563 746f  ent.querySelecto
-000013e0: 7228 2223 6964 5f67 656f 5f78 2229 2c0d  r("#id_geo_x"),.
-000013f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001400: 2020 2020 206c 6f6e 6769 7475 6465 3a20       longitude: 
-00001410: 646f 6375 6d65 6e74 2e71 7565 7279 5365  document.querySe
-00001420: 6c65 6374 6f72 2822 2369 645f 6765 6f5f  lector("#id_geo_
-00001430: 7922 292c 0d0a 2020 2020 2020 2020 2020  y"),..          
-00001440: 2020 2020 2020 2020 2020 7264 5f78 3a20            rd_x: 
-00001450: 646f 6375 6d65 6e74 2e71 7565 7279 5365  document.querySe
-00001460: 6c65 6374 6f72 2822 2369 645f 7264 5f78  lector("#id_rd_x
-00001470: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
-00001480: 2020 2020 2020 2020 2072 645f 793a 2064           rd_y: d
-00001490: 6f63 756d 656e 742e 7175 6572 7953 656c  ocument.querySel
-000014a0: 6563 746f 7228 2223 6964 5f72 645f 7922  ector("#id_rd_y"
-000014b0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000014c0: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
-000014d0: 2020 2020 2020 7375 6363 6573 733a 2066        success: f
-000014e0: 756e 6374 696f 6e28 6164 6472 2920 7b0d  unction(addr) {.
-000014f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001500: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
-00001510: 6164 6472 293b 0d0a 2020 2020 2020 2020  addr);..        
-00001520: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00001530: 2020 2020 2020 2020 2020 6572 726f 723a            error:
-00001540: 2066 756e 6374 696f 6e28 6572 726f 7229   function(error)
-00001550: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00001560: 2020 2020 2020 2063 6f6e 736f 6c65 2e6c         console.l
-00001570: 6f67 2865 7272 6f72 293b 0d0a 2020 2020  og(error);..    
-00001580: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00001590: 2020 2020 2020 2020 207d 290d 0a20 2020           })..   
-000015a0: 2020 2020 7d29 3b0d 0a20 2020 3c2f 7363      });..   </sc
-000015b0: 7269 7074 3e0d 0a0d 0a7b 2520 656e 6462  ript>....{% endb
-000015c0: 6c6f 636b 2025 7d0d 0a60 6060 0d0a 0d0a  lock %}..```....
-000015d0: 5468 6520 666f 726d 2077 696c 6c20 6e6f  The form will no
-000015e0: 7720 6175 746f 6d61 7469 6361 6c6c 7920  w automatically 
-000015f0: 6669 6c6c 2069 6e20 7468 6520 6164 6472  fill in the addr
-00001600: 6573 7320 6669 656c 6473 2077 6865 6e20  ess fields when 
-00001610: 6120 7661 6c69 6420 706f 7374 636f 6465  a valid postcode
-00001620: 2061 6e64 2068 6f6d 6520 6e75 6d62 6572   and home number
-00001630: 2069 7320 656e 7465 7265 642e 0d0a 0d0a   is entered.....
-00001640: 4966 2069 7420 6973 2069 6e76 616c 6964  If it is invalid
-00001650: 206f 7220 6e6f 7420 666f 756e 642c 2074   or not found, t
-00001660: 6865 2065 7272 6f72 2063 616c 6c62 6163  he error callbac
-00001670: 6b20 7769 6c6c 2062 6520 6361 6c6c 6564  k will be called
-00001680: 2e0d 0a0d 0a23 2320 5365 7474 696e 6773  .....## Settings
-00001690: 0d0a 0d0a 2323 2320 6041 4444 525f 5641  ....### `ADDR_VA
-000016a0: 4c49 4441 544f 525f 4150 495f 4b45 5960  LIDATOR_API_KEY`
-000016b0: 0d0a 0d0a 5468 6520 4150 4920 6b65 7920  ....The API key 
-000016c0: 746f 2075 7365 2066 6f72 2074 6865 2070  to use for the p
-000016d0: 6f73 7463 6f64 6520 6c6f 6f6b 7570 2e0d  ostcode lookup..
-000016e0: 0a0d 0a54 6869 7320 7769 6c6c 2062 6520  ...This will be 
-000016f0: 7573 6564 2062 7920 7468 6520 6070 6f73  used by the `pos
-00001700: 7463 6f64 6573 2e70 6f73 7463 6f64 652e  tcodes.postcode.
-00001710: 6164 6472 6573 735f 6368 6563 6b60 2066  address_check` f
-00001720: 756e 6374 696f 6e2e 0d0a 0d0a 0d0a 2323  unction.......##
-00001730: 2320 6041 4444 525f 5641 4c49 4441 544f  # `ADDR_VALIDATO
-00001740: 525f 4150 495f 5552 4c60 0d0a 0d0a 5468  R_API_URL`....Th
-00001750: 6520 4150 4920 5552 4c20 746f 2075 7365  e API URL to use
-00001760: 2066 6f72 2074 6865 2070 6f73 7463 6f64   for the postcod
-00001770: 6520 6c6f 6f6b 7570 2e0d 0a0d 0a54 6869  e lookup.....Thi
-00001780: 7320 7769 6c6c 2062 6520 7573 6564 2062  s will be used b
-00001790: 7920 7468 6520 6070 6f73 7463 6f64 6573  y the `postcodes
-000017a0: 2e70 6f73 7463 6f64 652e 6164 6472 6573  .postcode.addres
-000017b0: 735f 6368 6563 6b60 2066 756e 6374 696f  s_check` functio
-000017c0: 6e2e 0d0a 0d0a 4974 2073 686f 756c 6420  n.....It should 
-000017d0: 636f 6e74 6169 6e20 7468 6520 607b 706f  contain the `{po
-000017e0: 7374 636f 6465 7d60 2061 6e64 2060 7b68  stcode}` and `{h
-000017f0: 6f6d 655f 6e75 6d62 6572 7d60 2070 6c61  ome_number}` pla
-00001800: 6365 686f 6c64 6572 732e 0d0a 0d0a 0d0a  ceholders.......
-00001810: 2323 2320 6041 4444 525f 5641 4c49 4441  ### `ADDR_VALIDA
-00001820: 544f 525f 5041 5241 4d45 5445 525f 464f  TOR_PARAMETER_FO
-00001830: 524d 4154 600d 0a0d 0a41 6e20 6163 7475  RMAT`....An actu
-00001840: 616c 2066 756e 6374 696f 6e20 7468 6174  al function that
-00001850: 2066 6f72 6d61 7473 2074 6865 2070 6172   formats the par
-00001860: 616d 6574 6572 7320 666f 7220 7468 6520  ameters for the 
-00001870: 4150 4920 5552 4c2e 0d0a 0d0a 5468 6973  API URL.....This
-00001880: 206d 6179 206e 6f74 2062 6520 6120 7061   may not be a pa
-00001890: 7468 2074 6f20 6120 6675 6e63 7469 6f6e  th to a function
-000018a0: 2c20 6275 7420 7468 6520 6675 6e63 7469  , but the functi
-000018b0: 6f6e 2069 7473 656c 662e 0d0a 0d0a 4578  on itself.....Ex
-000018c0: 616d 706c 653a 0d0a 0d0a 6060 6070 7974  ample:....```pyt
-000018d0: 686f 6e0d 0a64 6566 2064 6566 6175 6c74  hon..def default
-000018e0: 5f70 6172 616d 6574 6572 5f66 6f72 6d61  _parameter_forma
-000018f0: 7474 6572 282a 2a6b 7761 7267 7329 3a0d  tter(**kwargs):.
-00001900: 0a20 2020 2072 6574 7572 6e20 2226 222e  .    return "&".
-00001910: 6a6f 696e 285b 6622 7b6b 6579 7d3d 7b76  join([f"{key}={v
-00001920: 616c 7565 7d22 2066 6f72 206b 6579 2c20  alue}" for key, 
-00001930: 7661 6c75 6520 696e 206b 7761 7267 732e  value in kwargs.
-00001940: 6974 656d 7328 295d 290d 0a60 6060 0d0a  items()])..```..
-00001950: 0d0a 0d0a 2323 2320 6041 4444 525f 5641  ....### `ADDR_VA
-00001960: 4c49 4441 544f 525f 4552 524f 525f 4154  LIDATOR_ERROR_AT
-00001970: 5452 4942 5554 4560 0d0a 0d0a 5468 6520  TRIBUTE`....The 
-00001980: 6174 7472 6962 7574 6520 696e 2074 6865  attribute in the
-00001990: 2072 6573 706f 6e73 6520 7468 6174 2063   response that c
-000019a0: 6f6e 7461 696e 7320 7468 6520 6572 726f  ontains the erro
-000019b0: 7220 6d65 7373 6167 652e 0d0a 0d0a 5468  r message.....Th
-000019c0: 6973 2077 696c 6c20 6265 2075 7365 6420  is will be used 
-000019d0: 6279 2074 6865 2060 706f 7374 636f 6465  by the `postcode
-000019e0: 732e 706f 7374 636f 6465 2e61 6464 7265  s.postcode.addre
-000019f0: 7373 5f63 6865 636b 6020 6675 6e63 7469  ss_check` functi
-00001a00: 6f6e 2e0d 0a0d 0a41 6464 7265 7373 5661  on.....AddressVa
-00001a10: 6c69 6461 7469 6f6e 4572 726f 7220 6578  lidationError ex
-00001a20: 6365 7074 696f 6e73 2077 696c 6c20 7265  ceptions will re
-00001a30: 7475 726e 2074 6865 2061 7070 726f 7072  turn the appropr
-00001a40: 6961 7465 2065 7272 6f72 206d 6573 7361  iate error messa
-00001a50: 6765 2069 6620 7468 6520 6174 7472 6962  ge if the attrib
-00001a60: 7574 6520 6973 2066 6f75 6e64 2e0d 0a0d  ute is found....
-00001a70: 0a0d 0a23 2323 2060 4144 4452 5f56 414c  ...### `ADDR_VAL
-00001a80: 4944 4154 4f52 5f43 4143 4845 5f54 494d  IDATOR_CACHE_TIM
-00001a90: 454f 5554 600d 0a0d 0a54 6865 2074 696d  EOUT`....The tim
-00001aa0: 656f 7574 2066 6f72 2074 6865 2063 6163  eout for the cac
-00001ab0: 6865 2069 6e20 7365 636f 6e64 732e 0d0a  he in seconds...
-00001ac0: 0d0a 5468 6973 2077 696c 6c20 6265 2075  ..This will be u
-00001ad0: 7365 6420 6279 2074 6865 2060 706f 7374  sed by the `post
-00001ae0: 636f 6465 732e 706f 7374 636f 6465 2e61  codes.postcode.a
-00001af0: 6464 7265 7373 5f63 6865 636b 6020 6675  ddress_check` fu
-00001b00: 6e63 7469 6f6e 2e0d 0a0d 0a49 7420 6973  nction.....It is
-00001b10: 2068 6967 686c 7920 7265 636f 6d6d 656e   highly recommen
-00001b20: 6465 6420 746f 2073 6574 2074 6869 7320  ded to set this 
-00001b30: 746f 2061 2068 6967 6820 6e75 6d62 6572  to a high number
-00001b40: 3b20 6279 2064 6566 6175 6c74 2069 7420  ; by default it 
-00001b50: 6361 6368 6573 2066 6f72 2061 2077 6565  caches for a wee
-00001b60: 6b2e 0d0a 0d0a 5468 6520 6465 6661 756c  k.....The defaul
-00001b70: 7420 656e 6470 6f69 6e74 2069 7320 6672  t endpoint is fr
-00001b80: 6565 2074 6f20 7573 652c 2062 7574 2068  ee to use, but h
-00001b90: 6173 2061 2072 6174 6520 6c69 6d69 742e  as a rate limit.
-00001ba0: 0d0a 0d0a 0d0a 2323 2320 6041 4444 525f  ......### `ADDR_
-00001bb0: 5641 4c49 4441 544f 525f 4150 495f 4b45  VALIDATOR_API_KE
-00001bc0: 595f 4154 5452 4942 5554 4560 0d0a 0d0a  Y_ATTRIBUTE`....
-00001bd0: 5468 6520 6174 7472 6962 7574 6520 696e  The attribute in
-00001be0: 2074 6865 2072 6573 706f 6e73 6520 7468   the response th
-00001bf0: 6174 2063 6f6e 7461 696e 7320 7468 6520  at contains the 
-00001c00: 4150 4920 6b65 792e 0d0a 0d0a 5468 6973  API key.....This
-00001c10: 2077 696c 6c20 6265 2075 7365 6420 6279   will be used by
-00001c20: 2074 6865 2060 706f 7374 636f 6465 732e   the `postcodes.
-00001c30: 706f 7374 636f 6465 2e61 6464 7265 7373  postcode.address
-00001c40: 5f63 6865 636b 6020 6675 6e63 7469 6f6e  _check` function
-00001c50: 2e0d 0a0d 0a49 7420 6973 2074 6865 2068  .....It is the h
-00001c60: 6561 6465 7220 7468 6174 2073 686f 756c  eader that shoul
-00001c70: 6420 6265 2073 656e 7420 7769 7468 2074  d be sent with t
-00001c80: 6865 2072 6571 7565 7374 2e0d 0a0d 0a44  he request.....D
-00001c90: 6566 6175 6c74 7320 746f 2060 582d 4150  efaults to `X-AP
-00001ca0: 492d 546f 6b65 6e60 2e0d 0a0d 0a0d 0a23  I-Token`.......#
-00001cb0: 2323 2060 4144 4452 5f56 414c 4944 4154  ## `ADDR_VALIDAT
-00001cc0: 4f52 5f52 4551 5549 5245 535f 4155 5448  OR_REQUIRES_AUTH
-00001cd0: 600d 0a0d 0a57 6865 7468 6572 2074 6865  `....Whether the
-00001ce0: 2041 5049 2072 6571 7569 7265 7320 6175   API requires au
-00001cf0: 7468 656e 7469 6361 7469 6f6e 2e0d 0a0d  thentication....
-00001d00: 0a54 6869 7320 7769 6c6c 2062 6520 7573  .This will be us
-00001d10: 6564 2062 7920 7468 6520 696e 7465 726e  ed by the intern
-00001d20: 616c 2076 6965 7720 746f 2063 6865 636b  al view to check
-00001d30: 2069 6620 7468 6520 7573 6572 2069 7320   if the user is 
-00001d40: 6175 7468 656e 7469 6361 7465 642e 0d0a  authenticated...
-00001d50: 0d0a 4966 2074 6865 2075 7365 7220 6973  ..If the user is
-00001d60: 2061 7574 6865 6e74 6963 6174 6564 3b20   authenticated; 
-00001d70: 7468 6520 7669 6577 2077 696c 6c20 7265  the view will re
-00001d80: 7475 726e 2074 6865 2061 6464 7265 7373  turn the address
-00001d90: 2064 6174 612e 0d0a 0d0a 5468 6973 2064   data.....This d
-00001da0: 6f65 7320 6e6f 7420 6d61 7474 6572 2069  oes not matter i
-00001db0: 6620 796f 7520 7573 6520 7468 6520 6070  f you use the `p
-00001dc0: 6f73 7463 6f64 6573 2e70 6f73 7463 6f64  ostcodes.postcod
-00001dd0: 652e 6164 6472 6573 735f 6368 6563 6b60  e.address_check`
-00001de0: 2066 756e 6374 696f 6e2e 0d0a             function...
+000009e0: 2022 3132 3334 2041 4222 2c20 2263 6c61   "1234 AB", "cla
+000009f0: 7373 223a 2022 706f 7374 636f 6465 222c  ss": "postcode",
+00000a00: 2022 7061 7474 6572 6e22 3a20 225e 5b30   "pattern": "^[0
+00000a10: 2d39 5d7b 347d 285c 732b 7c29 5b41 2d5a  -9]{4}(\s+|)[A-Z
+00000a20: 5d7b 327d 2422 7d29 290d 0a20 2020 2068  ]{2}$"}))..    h
+00000a30: 6f6d 655f 6e75 6d62 6572 203d 2066 6f72  ome_number = for
+00000a40: 6d73 2e43 6861 7246 6965 6c64 286d 6178  ms.CharField(max
+00000a50: 5f6c 656e 6774 683d 3130 2c20 7769 6467  _length=10, widg
+00000a60: 6574 3d66 6f72 6d73 2e54 6578 7449 6e70  et=forms.TextInp
+00000a70: 7574 2861 7474 7273 3d7b 2270 6c61 6365  ut(attrs={"place
+00000a80: 686f 6c64 6572 223a 2022 3132 3322 2c20  holder": "123", 
+00000a90: 2263 6c61 7373 223a 2022 686f 6d65 5f6e  "class": "home_n
+00000aa0: 756d 6265 7222 7d29 290d 0a20 2020 200d  umber"}))..    .
+00000ab0: 0a20 2020 2023 2043 7573 746f 6d20 6669  .    # Custom fi
+00000ac0: 656c 6473 0d0a 2020 2020 7374 7265 6574  elds..    street
+00000ad0: 203d 2066 6f72 6d73 2e43 6861 7246 6965   = forms.CharFie
+00000ae0: 6c64 286d 6178 5f6c 656e 6774 683d 3235  ld(max_length=25
+00000af0: 352c 2077 6964 6765 743d 666f 726d 732e  5, widget=forms.
+00000b00: 5465 7874 496e 7075 7428 6174 7472 733d  TextInput(attrs=
+00000b10: 7b22 706c 6163 6568 6f6c 6465 7222 3a20  {"placeholder": 
+00000b20: 224d 6169 6e20 7374 7265 6574 222c 2022  "Main street", "
+00000b30: 636c 6173 7322 3a20 2273 7472 6565 7422  class": "street"
+00000b40: 7d29 290d 0a20 2020 2063 6974 7920 3d20  }))..    city = 
+00000b50: 666f 726d 732e 4368 6172 4669 656c 6428  forms.CharField(
+00000b60: 6d61 785f 6c65 6e67 7468 3d32 3535 2c20  max_length=255, 
+00000b70: 7769 6467 6574 3d66 6f72 6d73 2e54 6578  widget=forms.Tex
+00000b80: 7449 6e70 7574 2861 7474 7273 3d7b 2270  tInput(attrs={"p
+00000b90: 6c61 6365 686f 6c64 6572 223a 2022 416d  laceholder": "Am
+00000ba0: 7374 6572 6461 6d22 2c20 2263 6c61 7373  sterdam", "class
+00000bb0: 223a 2022 6369 7479 227d 2929 0d0a 2020  ": "city"}))..  
+00000bc0: 2020 6d75 6e69 6369 7061 6c69 7479 203d    municipality =
+00000bd0: 2066 6f72 6d73 2e43 6861 7246 6965 6c64   forms.CharField
+00000be0: 286d 6178 5f6c 656e 6774 683d 3235 352c  (max_length=255,
+00000bf0: 2077 6964 6765 743d 666f 726d 732e 5465   widget=forms.Te
+00000c00: 7874 496e 7075 7428 6174 7472 733d 7b22  xtInput(attrs={"
+00000c10: 706c 6163 6568 6f6c 6465 7222 3a20 2241  placeholder": "A
+00000c20: 6d73 7465 7264 616d 222c 2022 636c 6173  msterdam", "clas
+00000c30: 7322 3a20 226d 756e 6963 6970 616c 6974  s": "municipalit
+00000c40: 7922 7d29 290d 0a20 2020 2070 726f 7669  y"}))..    provi
+00000c50: 6e63 6520 3d20 666f 726d 732e 4368 6172  nce = forms.Char
+00000c60: 4669 656c 6428 6d61 785f 6c65 6e67 7468  Field(max_length
+00000c70: 3d32 3535 2c20 7769 6467 6574 3d66 6f72  =255, widget=for
+00000c80: 6d73 2e54 6578 7449 6e70 7574 2861 7474  ms.TextInput(att
+00000c90: 7273 3d7b 2270 6c61 6365 686f 6c64 6572  rs={"placeholder
+00000ca0: 223a 2022 4e6f 6f72 642d 486f 6c6c 616e  ": "Noord-Hollan
+00000cb0: 6422 2c20 2263 6c61 7373 223a 2022 7072  d", "class": "pr
+00000cc0: 6f76 696e 6365 227d 2929 0d0a 2020 2020  ovince"}))..    
+00000cd0: 6275 696c 645f 7965 6172 203d 2066 6f72  build_year = for
+00000ce0: 6d73 2e49 6e74 6567 6572 4669 656c 6428  ms.IntegerField(
+00000cf0: 7769 6467 6574 3d66 6f72 6d73 2e4e 756d  widget=forms.Num
+00000d00: 6265 7249 6e70 7574 2861 7474 7273 3d7b  berInput(attrs={
+00000d10: 2270 6c61 6365 686f 6c64 6572 223a 2022  "placeholder": "
+00000d20: 3139 3930 222c 2022 636c 6173 7322 3a20  1990", "class": 
+00000d30: 2262 7569 6c64 5f79 6561 7222 2c20 2270  "build_year", "p
+00000d40: 6174 7465 726e 223a 2022 5e5b 302d 395d  attern": "^[0-9]
+00000d50: 7b34 7d24 222c 2022 6d69 6e22 3a20 2231  {4}$", "min": "1
+00000d60: 3930 3022 2c20 226d 6178 223a 2022 3230  900", "max": "20
+00000d70: 3232 227d 2929 0d0a 2020 2020 666c 6f6f  22"}))..    floo
+00000d80: 725f 6172 6561 203d 2066 6f72 6d73 2e44  r_area = forms.D
+00000d90: 6563 696d 616c 4669 656c 6428 7769 6467  ecimalField(widg
+00000da0: 6574 3d66 6f72 6d73 2e4e 756d 6265 7249  et=forms.NumberI
+00000db0: 6e70 7574 2861 7474 7273 3d7b 2270 6c61  nput(attrs={"pla
+00000dc0: 6365 686f 6c64 6572 223a 2022 3130 3022  ceholder": "100"
+00000dd0: 2c20 2263 6c61 7373 223a 2022 666c 6f6f  , "class": "floo
+00000de0: 725f 6172 6561 222c 2022 7061 7474 6572  r_area", "patter
+00000df0: 6e22 3a20 225e 5b30 2d39 5d7b 312c 337d  n": "^[0-9]{1,3}
+00000e00: 2422 7d29 2920 2320 2270 6174 7465 726e  $"})) # "pattern
+00000e10: 223a 2022 5e5b 302d 395d 7b31 2c33 7d24  ": "^[0-9]{1,3}$
+00000e20: 220d 0a20 2020 2067 656f 5f78 203d 2066  "..    geo_x = f
+00000e30: 6f72 6d73 2e44 6563 696d 616c 4669 656c  orms.DecimalFiel
+00000e40: 6428 7769 6467 6574 3d66 6f72 6d73 2e4e  d(widget=forms.N
+00000e50: 756d 6265 7249 6e70 7574 2861 7474 7273  umberInput(attrs
+00000e60: 3d7b 2270 6c61 6365 686f 6c64 6572 223a  ={"placeholder":
+00000e70: 2022 3532 2e31 3233 3435 3622 2c20 2263   "52.123456", "c
+00000e80: 6c61 7373 223a 2022 6765 6f5f 7822 7d29  lass": "geo_x"})
+00000e90: 290d 0a20 2020 2067 656f 5f79 203d 2066  )..    geo_y = f
+00000ea0: 6f72 6d73 2e44 6563 696d 616c 4669 656c  orms.DecimalFiel
+00000eb0: 6428 7769 6467 6574 3d66 6f72 6d73 2e4e  d(widget=forms.N
+00000ec0: 756d 6265 7249 6e70 7574 2861 7474 7273  umberInput(attrs
+00000ed0: 3d7b 2270 6c61 6365 686f 6c64 6572 223a  ={"placeholder":
+00000ee0: 2022 342e 3132 3334 3536 222c 2022 636c   "4.123456", "cl
+00000ef0: 6173 7322 3a20 2267 656f 5f79 227d 2929  ass": "geo_y"}))
+00000f00: 0d0a 2020 2020 7264 5f78 203d 2066 6f72  ..    rd_x = for
+00000f10: 6d73 2e44 6563 696d 616c 4669 656c 6428  ms.DecimalField(
+00000f20: 7769 6467 6574 3d66 6f72 6d73 2e4e 756d  widget=forms.Num
+00000f30: 6265 7249 6e70 7574 2861 7474 7273 3d7b  berInput(attrs={
+00000f40: 2270 6c61 6365 686f 6c64 6572 223a 2022  "placeholder": "
+00000f50: 3132 3334 3536 222c 2022 636c 6173 7322  123456", "class"
+00000f60: 3a20 2272 645f 7822 7d29 2920 2320 5269  : "rd_x"})) # Ri
+00000f70: 6a6b 7364 7269 6568 6f65 6b0d 0a20 2020  jksdriehoek..   
+00000f80: 2072 645f 7920 3d20 666f 726d 732e 4465   rd_y = forms.De
+00000f90: 6369 6d61 6c46 6965 6c64 2877 6964 6765  cimalField(widge
+00000fa0: 743d 666f 726d 732e 4e75 6d62 6572 496e  t=forms.NumberIn
+00000fb0: 7075 7428 6174 7472 733d 7b22 706c 6163  put(attrs={"plac
+00000fc0: 6568 6f6c 6465 7222 3a20 2231 3233 3435  eholder": "12345
+00000fd0: 3622 2c20 2263 6c61 7373 223a 2022 7264  6", "class": "rd
+00000fe0: 5f79 227d 2929 2023 2052 696a 6b73 6472  _y"})) # Rijksdr
+00000ff0: 6965 686f 656b 0d0a 6060 600d 0a0d 0a54  iehoek..```....T
+00001000: 6865 6e20 7765 2063 616e 2064 6566 696e  hen we can defin
+00001010: 6520 6f75 7220 7465 6d70 6c61 7465 0d0a  e our template..
+00001020: 0d0a 6060 6068 746d 6c0d 0a7b 2520 6578  ..```html..{% ex
+00001030: 7465 6e64 7320 2762 6173 652e 6874 6d6c  tends 'base.html
+00001040: 2720 257d 0d0a 0d0a 7b25 2062 6c6f 636b  ' %}....{% block
+00001050: 2063 6f6e 7465 6e74 2025 7d0d 0a20 2020   content %}..   
+00001060: 3c6c 696e 6b20 7265 6c3d 2273 7479 6c65  <link rel="style
+00001070: 7368 6565 7422 2068 7265 663d 227b 2520  sheet" href="{% 
+00001080: 7374 6174 6963 2027 706f 7374 636f 6465  static 'postcode
+00001090: 732f 6373 732f 706f 7374 636f 6465 732e  s/css/postcodes.
+000010a0: 6373 7327 2025 7d22 3e0d 0a20 2020 3c73  css' %}">..   <s
+000010b0: 6372 6970 7420 7372 633d 227b 2520 7374  cript src="{% st
+000010c0: 6174 6963 2027 706f 7374 636f 6465 732f  atic 'postcodes/
+000010d0: 6a73 2f70 6f73 7463 6f64 6573 2e6a 7327  js/postcodes.js'
+000010e0: 2025 7d22 2064 6174 612d 6170 692d 7572   %}" data-api-ur
+000010f0: 6c3d 227b 2520 7572 6c20 2270 6f73 7463  l="{% url "postc
+00001100: 6f64 6573 3a61 7069 2220 257d 223e 3c2f  odes:api" %}"></
+00001110: 7363 7269 7074 3e0d 0a0d 0a20 2020 3c66  script>....   <f
+00001120: 6f72 6d20 6d65 7468 6f64 3d22 706f 7374  orm method="post
+00001130: 223e 0d0a 2020 2020 2020 207b 2520 6373  ">..       {% cs
+00001140: 7266 5f74 6f6b 656e 2025 7d0d 0a20 2020  rf_token %}..   
+00001150: 2020 2020 7b7b 2066 6f72 6d2e 6173 5f70      {{ form.as_p
+00001160: 207d 7d0d 0a20 2020 2020 2020 3c62 7574   }}..       <but
+00001170: 746f 6e20 7479 7065 3d22 7375 626d 6974  ton type="submit
+00001180: 223e 5375 626d 6974 3c2f 6275 7474 6f6e  ">Submit</button
+00001190: 3e0d 0a20 2020 3c2f 666f 726d 3e0d 0a0d  >..   </form>...
+000011a0: 0a20 2020 2e2e 2e0d 0a0d 0a20 2020 3c73  .   .......   <s
+000011b0: 6372 6970 743e 0d0a 2020 2020 2020 2064  cript>..       d
+000011c0: 6f63 756d 656e 742e 6164 6445 7665 6e74  ocument.addEvent
+000011d0: 4c69 7374 656e 6572 2827 444f 4d43 6f6e  Listener('DOMCon
+000011e0: 7465 6e74 4c6f 6164 6564 272c 2066 756e  tentLoaded', fun
+000011f0: 6374 696f 6e28 2920 7b0d 0a20 2020 2020  ction() {..     
+00001200: 2020 2020 2020 6c6f 6f6b 7570 506f 7374        lookupPost
+00001210: 636f 6465 287b 0d0a 2020 2020 2020 2020  code({..        
+00001220: 2020 2020 2020 2062 696e 643a 207b 0d0a         bind: {..
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 2020 202f 2f20 5468 6573 6520 6172 6520     // These are 
+00001250: 7265 7175 6972 6564 2066 6f72 2074 6865  required for the
+00001260: 206c 6f6f 6b75 700d 0a20 2020 2020 2020   lookup..       
+00001270: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
+00001280: 7463 6f64 653a 2064 6f63 756d 656e 742e  tcode: document.
+00001290: 7175 6572 7953 656c 6563 746f 7228 2723  querySelector('#
+000012a0: 6964 5f70 6f73 7463 6f64 6527 292c 0d0a  id_postcode'),..
+000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012c0: 2020 2020 686f 6d65 5f6e 756d 6265 723a      home_number:
+000012d0: 2064 6f63 756d 656e 742e 7175 6572 7953   document.queryS
+000012e0: 656c 6563 746f 7228 2723 6964 5f68 6f6d  elector('#id_hom
+000012f0: 655f 6e75 6d62 6572 2729 2c0d 0a20 2020  e_number'),..   
+00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001310: 202f 2f20 4375 7374 6f6d 2066 6965 6c64   // Custom field
+00001320: 7320 7265 7475 726e 6564 2062 7920 7468  s returned by th
+00001330: 6520 4150 490d 0a20 2020 2020 2020 2020  e API..         
+00001340: 2020 2020 2020 2020 2020 2073 7472 6161             straa
+00001350: 743a 2064 6f63 756d 656e 742e 7175 6572  t: document.quer
+00001360: 7953 656c 6563 746f 7228 2223 6964 5f73  ySelector("#id_s
+00001370: 7472 6565 7422 292c 0d0a 2020 2020 2020  treet"),..      
+00001380: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+00001390: 6f6e 706c 6161 7473 3a20 646f 6375 6d65  onplaats: docume
+000013a0: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
+000013b0: 2822 2369 645f 6369 7479 2229 2c0d 0a20  ("#id_city"),.. 
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013d0: 2020 2067 656d 6565 6e74 653a 2064 6f63     gemeente: doc
+000013e0: 756d 656e 742e 7175 6572 7953 656c 6563  ument.querySelec
+000013f0: 746f 7228 2223 6964 5f6d 756e 6963 6970  tor("#id_municip
+00001400: 616c 6974 7922 292c 0d0a 2020 2020 2020  ality"),..      
+00001410: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001420: 6f76 696e 6369 653a 2064 6f63 756d 656e  ovincie: documen
+00001430: 742e 7175 6572 7953 656c 6563 746f 7228  t.querySelector(
+00001440: 2223 6964 5f70 726f 7669 6e63 6522 292c  "#id_province"),
+00001450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001460: 2020 2020 2020 626f 7577 6a61 6172 3a20        bouwjaar: 
+00001470: 646f 6375 6d65 6e74 2e71 7565 7279 5365  document.querySe
+00001480: 6c65 6374 6f72 2822 2369 645f 6275 696c  lector("#id_buil
+00001490: 645f 7965 6172 2229 2c0d 0a20 2020 2020  d_year"),..     
+000014a0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000014b0: 6c6f 6572 6f70 7065 7276 6c61 6b74 653a  loeroppervlakte:
+000014c0: 2064 6f63 756d 656e 742e 7175 6572 7953   document.queryS
+000014d0: 656c 6563 746f 7228 2223 6964 5f66 6c6f  elector("#id_flo
+000014e0: 6f72 5f61 7265 6122 292c 0d0a 2020 2020  or_area"),..    
+000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001500: 6c61 7469 7475 6465 3a20 646f 6375 6d65  latitude: docume
+00001510: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
+00001520: 2822 2369 645f 6765 6f5f 7822 292c 0d0a  ("#id_geo_x"),..
+00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001540: 2020 2020 6c6f 6e67 6974 7564 653a 2064      longitude: d
+00001550: 6f63 756d 656e 742e 7175 6572 7953 656c  ocument.querySel
+00001560: 6563 746f 7228 2223 6964 5f67 656f 5f79  ector("#id_geo_y
+00001570: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
+00001580: 2020 2020 2020 2020 2072 645f 783a 2064           rd_x: d
+00001590: 6f63 756d 656e 742e 7175 6572 7953 656c  ocument.querySel
+000015a0: 6563 746f 7228 2223 6964 5f72 645f 7822  ector("#id_rd_x"
+000015b0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+000015c0: 2020 2020 2020 2020 7264 5f79 3a20 646f          rd_y: do
+000015d0: 6375 6d65 6e74 2e71 7565 7279 5365 6c65  cument.querySele
+000015e0: 6374 6f72 2822 2369 645f 7264 5f79 2229  ctor("#id_rd_y")
+000015f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001600: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
+00001610: 2020 2020 2073 7563 6365 7373 3a20 6675       success: fu
+00001620: 6e63 7469 6f6e 2861 6464 7229 207b 0d0a  nction(addr) {..
+00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001640: 2020 2063 6f6e 736f 6c65 2e6c 6f67 2861     console.log(a
+00001650: 6464 7229 3b0d 0a20 2020 2020 2020 2020  ddr);..         
+00001660: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+00001670: 2020 2020 2020 2020 2065 7272 6f72 3a20           error: 
+00001680: 6675 6e63 7469 6f6e 2865 7272 6f72 2920  function(error) 
+00001690: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+000016a0: 2020 2020 2020 636f 6e73 6f6c 652e 6c6f        console.lo
+000016b0: 6728 6572 726f 7229 3b0d 0a20 2020 2020  g(error);..     
+000016c0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+000016d0: 2020 2020 2020 2020 7d29 0d0a 2020 2020          })..    
+000016e0: 2020 207d 293b 0d0a 2020 203c 2f73 6372     });..   </scr
+000016f0: 6970 743e 0d0a 0d0a 7b25 2065 6e64 626c  ipt>....{% endbl
+00001700: 6f63 6b20 257d 0d0a 6060 600d 0a0d 0a54  ock %}..```....T
+00001710: 6865 2066 6f72 6d20 7769 6c6c 206e 6f77  he form will now
+00001720: 2061 7574 6f6d 6174 6963 616c 6c79 2066   automatically f
+00001730: 696c 6c20 696e 2074 6865 2061 6464 7265  ill in the addre
+00001740: 7373 2066 6965 6c64 7320 7768 656e 2061  ss fields when a
+00001750: 2076 616c 6964 2070 6f73 7463 6f64 6520   valid postcode 
+00001760: 616e 6420 686f 6d65 206e 756d 6265 7220  and home number 
+00001770: 6973 2065 6e74 6572 6564 2e0d 0a0d 0a49  is entered.....I
+00001780: 6620 6974 2069 7320 696e 7661 6c69 6420  f it is invalid 
+00001790: 6f72 206e 6f74 2066 6f75 6e64 2c20 7468  or not found, th
+000017a0: 6520 6572 726f 7220 6361 6c6c 6261 636b  e error callback
+000017b0: 2077 696c 6c20 6265 2063 616c 6c65 642e   will be called.
+000017c0: 0d0a 0d0a 2323 2053 6574 7469 6e67 730d  ....## Settings.
+000017d0: 0a0d 0a23 2323 2060 4144 4452 5f56 414c  ...### `ADDR_VAL
+000017e0: 4944 4154 4f52 5f41 5049 5f4b 4559 600d  IDATOR_API_KEY`.
+000017f0: 0a0d 0a54 6865 2041 5049 206b 6579 2074  ...The API key t
+00001800: 6f20 7573 6520 666f 7220 7468 6520 706f  o use for the po
+00001810: 7374 636f 6465 206c 6f6f 6b75 702e 0d0a  stcode lookup...
+00001820: 0d0a 5468 6973 2077 696c 6c20 6265 2075  ..This will be u
+00001830: 7365 6420 6279 2074 6865 2060 706f 7374  sed by the `post
+00001840: 636f 6465 732e 706f 7374 636f 6465 2e61  codes.postcode.a
+00001850: 6464 7265 7373 5f63 6865 636b 6020 6675  ddress_check` fu
+00001860: 6e63 7469 6f6e 2e0d 0a0d 0a0d 0a23 2323  nction.......###
+00001870: 2060 4144 4452 5f56 414c 4944 4154 4f52   `ADDR_VALIDATOR
+00001880: 5f41 5049 5f55 524c 600d 0a0d 0a54 6865  _API_URL`....The
+00001890: 2041 5049 2055 524c 2074 6f20 7573 6520   API URL to use 
+000018a0: 666f 7220 7468 6520 706f 7374 636f 6465  for the postcode
+000018b0: 206c 6f6f 6b75 702e 0d0a 0d0a 5468 6973   lookup.....This
+000018c0: 2077 696c 6c20 6265 2075 7365 6420 6279   will be used by
+000018d0: 2074 6865 2060 706f 7374 636f 6465 732e   the `postcodes.
+000018e0: 706f 7374 636f 6465 2e61 6464 7265 7373  postcode.address
+000018f0: 5f63 6865 636b 6020 6675 6e63 7469 6f6e  _check` function
+00001900: 2e0d 0a0d 0a49 7420 7368 6f75 6c64 2063  .....It should c
+00001910: 6f6e 7461 696e 2074 6865 2060 7b70 6f73  ontain the `{pos
+00001920: 7463 6f64 657d 6020 616e 6420 607b 686f  tcode}` and `{ho
+00001930: 6d65 5f6e 756d 6265 727d 6020 706c 6163  me_number}` plac
+00001940: 6568 6f6c 6465 7273 2e0d 0a0d 0a0d 0a23  eholders.......#
+00001950: 2323 2060 4144 4452 5f56 414c 4944 4154  ## `ADDR_VALIDAT
+00001960: 4f52 5f50 4152 414d 4554 4552 5f46 4f52  OR_PARAMETER_FOR
+00001970: 4d41 5460 0d0a 0d0a 416e 2061 6374 7561  MAT`....An actua
+00001980: 6c20 6675 6e63 7469 6f6e 2074 6861 7420  l function that 
+00001990: 666f 726d 6174 7320 7468 6520 7061 7261  formats the para
+000019a0: 6d65 7465 7273 2066 6f72 2074 6865 2041  meters for the A
+000019b0: 5049 2055 524c 2e0d 0a0d 0a54 6869 7320  PI URL.....This 
+000019c0: 6d61 7920 6e6f 7420 6265 2061 2070 6174  may not be a pat
+000019d0: 6820 746f 2061 2066 756e 6374 696f 6e2c  h to a function,
+000019e0: 2062 7574 2074 6865 2066 756e 6374 696f   but the functio
+000019f0: 6e20 6974 7365 6c66 2e0d 0a0d 0a45 7861  n itself.....Exa
+00001a00: 6d70 6c65 3a0d 0a0d 0a60 6060 7079 7468  mple:....```pyth
+00001a10: 6f6e 0d0a 6465 6620 6465 6661 756c 745f  on..def default_
+00001a20: 7061 7261 6d65 7465 725f 666f 726d 6174  parameter_format
+00001a30: 7465 7228 2a2a 6b77 6172 6773 293a 0d0a  ter(**kwargs):..
+00001a40: 2020 2020 7265 7475 726e 2022 2622 2e6a      return "&".j
+00001a50: 6f69 6e28 5b66 227b 6b65 797d 3d7b 7661  oin([f"{key}={va
+00001a60: 6c75 657d 2220 666f 7220 6b65 792c 2076  lue}" for key, v
+00001a70: 616c 7565 2069 6e20 6b77 6172 6773 2e69  alue in kwargs.i
+00001a80: 7465 6d73 2829 5d29 0d0a 6060 600d 0a0d  tems()])..```...
+00001a90: 0a0d 0a23 2323 2060 4144 4452 5f56 414c  ...### `ADDR_VAL
+00001aa0: 4944 4154 4f52 5f45 5252 4f52 5f41 5454  IDATOR_ERROR_ATT
+00001ab0: 5249 4255 5445 600d 0a0d 0a54 6865 2061  RIBUTE`....The a
+00001ac0: 7474 7269 6275 7465 2069 6e20 7468 6520  ttribute in the 
+00001ad0: 7265 7370 6f6e 7365 2074 6861 7420 636f  response that co
+00001ae0: 6e74 6169 6e73 2074 6865 2065 7272 6f72  ntains the error
+00001af0: 206d 6573 7361 6765 2e0d 0a0d 0a54 6869   message.....Thi
+00001b00: 7320 7769 6c6c 2062 6520 7573 6564 2062  s will be used b
+00001b10: 7920 7468 6520 6070 6f73 7463 6f64 6573  y the `postcodes
+00001b20: 2e70 6f73 7463 6f64 652e 6164 6472 6573  .postcode.addres
+00001b30: 735f 6368 6563 6b60 2066 756e 6374 696f  s_check` functio
+00001b40: 6e2e 0d0a 0d0a 4164 6472 6573 7356 616c  n.....AddressVal
+00001b50: 6964 6174 696f 6e45 7272 6f72 2065 7863  idationError exc
+00001b60: 6570 7469 6f6e 7320 7769 6c6c 2072 6574  eptions will ret
+00001b70: 7572 6e20 7468 6520 6170 7072 6f70 7269  urn the appropri
+00001b80: 6174 6520 6572 726f 7220 6d65 7373 6167  ate error messag
+00001b90: 6520 6966 2074 6865 2061 7474 7269 6275  e if the attribu
+00001ba0: 7465 2069 7320 666f 756e 642e 0d0a 0d0a  te is found.....
+00001bb0: 0d0a 2323 2320 6041 4444 525f 5641 4c49  ..### `ADDR_VALI
+00001bc0: 4441 544f 525f 4341 4348 455f 5449 4d45  DATOR_CACHE_TIME
+00001bd0: 4f55 5460 0d0a 0d0a 5468 6520 7469 6d65  OUT`....The time
+00001be0: 6f75 7420 666f 7220 7468 6520 6361 6368  out for the cach
+00001bf0: 6520 696e 2073 6563 6f6e 6473 2e0d 0a0d  e in seconds....
+00001c00: 0a54 6869 7320 7769 6c6c 2062 6520 7573  .This will be us
+00001c10: 6564 2062 7920 7468 6520 6070 6f73 7463  ed by the `postc
+00001c20: 6f64 6573 2e70 6f73 7463 6f64 652e 6164  odes.postcode.ad
+00001c30: 6472 6573 735f 6368 6563 6b60 2066 756e  dress_check` fun
+00001c40: 6374 696f 6e2e 0d0a 0d0a 4974 2069 7320  ction.....It is 
+00001c50: 6869 6768 6c79 2072 6563 6f6d 6d65 6e64  highly recommend
+00001c60: 6564 2074 6f20 7365 7420 7468 6973 2074  ed to set this t
+00001c70: 6f20 6120 6869 6768 206e 756d 6265 723b  o a high number;
+00001c80: 2062 7920 6465 6661 756c 7420 6974 2063   by default it c
+00001c90: 6163 6865 7320 666f 7220 6120 7765 656b  aches for a week
+00001ca0: 2e0d 0a0d 0a54 6865 2064 6566 6175 6c74  .....The default
+00001cb0: 2065 6e64 706f 696e 7420 6973 2066 7265   endpoint is fre
+00001cc0: 6520 746f 2075 7365 2c20 6275 7420 6861  e to use, but ha
+00001cd0: 7320 6120 7261 7465 206c 696d 6974 2e0d  s a rate limit..
+00001ce0: 0a0d 0a0d 0a23 2323 2060 4144 4452 5f56  .....### `ADDR_V
+00001cf0: 414c 4944 4154 4f52 5f41 5049 5f4b 4559  ALIDATOR_API_KEY
+00001d00: 5f41 5454 5249 4255 5445 600d 0a0d 0a54  _ATTRIBUTE`....T
+00001d10: 6865 2061 7474 7269 6275 7465 2069 6e20  he attribute in 
+00001d20: 7468 6520 7265 7370 6f6e 7365 2074 6861  the response tha
+00001d30: 7420 636f 6e74 6169 6e73 2074 6865 2041  t contains the A
+00001d40: 5049 206b 6579 2e0d 0a0d 0a54 6869 7320  PI key.....This 
+00001d50: 7769 6c6c 2062 6520 7573 6564 2062 7920  will be used by 
+00001d60: 7468 6520 6070 6f73 7463 6f64 6573 2e70  the `postcodes.p
+00001d70: 6f73 7463 6f64 652e 6164 6472 6573 735f  ostcode.address_
+00001d80: 6368 6563 6b60 2066 756e 6374 696f 6e2e  check` function.
+00001d90: 0d0a 0d0a 4974 2069 7320 7468 6520 6865  ....It is the he
+00001da0: 6164 6572 2074 6861 7420 7368 6f75 6c64  ader that should
+00001db0: 2062 6520 7365 6e74 2077 6974 6820 7468   be sent with th
+00001dc0: 6520 7265 7175 6573 742e 0d0a 0d0a 4465  e request.....De
+00001dd0: 6661 756c 7473 2074 6f20 6058 2d41 5049  faults to `X-API
+00001de0: 2d54 6f6b 656e 602e 0d0a 0d0a 0d0a 2323  -Token`.......##
+00001df0: 2320 6041 4444 525f 5641 4c49 4441 544f  # `ADDR_VALIDATO
+00001e00: 525f 5245 5155 4952 4553 5f41 5554 4860  R_REQUIRES_AUTH`
+00001e10: 0d0a 0d0a 5768 6574 6865 7220 7468 6520  ....Whether the 
+00001e20: 4150 4920 7265 7175 6972 6573 2061 7574  API requires aut
+00001e30: 6865 6e74 6963 6174 696f 6e2e 0d0a 0d0a  hentication.....
+00001e40: 5468 6973 2077 696c 6c20 6265 2075 7365  This will be use
+00001e50: 6420 6279 2074 6865 2069 6e74 6572 6e61  d by the interna
+00001e60: 6c20 7669 6577 2074 6f20 6368 6563 6b20  l view to check 
+00001e70: 6966 2074 6865 2075 7365 7220 6973 2061  if the user is a
+00001e80: 7574 6865 6e74 6963 6174 6564 2e0d 0a0d  uthenticated....
+00001e90: 0a49 6620 7468 6520 7573 6572 2069 7320  .If the user is 
+00001ea0: 6175 7468 656e 7469 6361 7465 643b 2074  authenticated; t
+00001eb0: 6865 2076 6965 7720 7769 6c6c 2072 6574  he view will ret
+00001ec0: 7572 6e20 7468 6520 6164 6472 6573 7320  urn the address 
+00001ed0: 6461 7461 2e0d 0a0d 0a54 6869 7320 646f  data.....This do
+00001ee0: 6573 206e 6f74 206d 6174 7465 7220 6966  es not matter if
+00001ef0: 2079 6f75 2075 7365 2074 6865 2060 706f   you use the `po
+00001f00: 7374 636f 6465 732e 706f 7374 636f 6465  stcodes.postcode
+00001f10: 2e61 6464 7265 7373 5f63 6865 636b 6020  .address_check` 
+00001f20: 6675 6e63 7469 6f6e 2e0d 0a              function...
```

### Comparing `django_postcodes-1.0.1/django_postcodes.egg-info/SOURCES.txt` & `django_postcodes-1.0.2/django_postcodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/postcodes/countries.py` & `django_postcodes-1.0.2/postcodes/countries.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/postcodes/postcode.py` & `django_postcodes-1.0.2/postcodes/postcode.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/postcodes/settings.py` & `django_postcodes-1.0.2/postcodes/settings.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/postcodes/static/postcodes/js/postcodes.js` & `django_postcodes-1.0.2/postcodes/static/postcodes/js/postcodes.js`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/postcodes/test/manage.py` & `django_postcodes-1.0.2/postcodes/test/manage.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/postcodes/test/testapp/core/tests.py` & `django_postcodes-1.0.2/postcodes/test/testapp/core/tests.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/postcodes/test/testapp/testapp/settings.py` & `django_postcodes-1.0.2/postcodes/test/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/postcodes/views.py` & `django_postcodes-1.0.2/postcodes/views.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.1/setup.cfg` & `django_postcodes-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 706f 7374 636f   = django-postco
 00000020: 6465 730d 0a76 6572 7369 6f6e 203d 2031  des..version = 1
-00000030: 2e30 2e31 0d0a 6465 7363 7269 7074 696f  .0.1..descriptio
+00000030: 2e30 2e32 0d0a 6465 7363 7269 7074 696f  .0.2..descriptio
 00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
 00000050: 2074 6f20 6d61 6e61 6765 2070 6f73 7463   to manage postc
 00000060: 6f64 652f 686f 6d65 206e 756d 6265 7220  ode/home number 
 00000070: 6164 6472 6573 7320 666f 726d 730d 0a6c  address forms..l
 00000080: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000090: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
 000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
```

