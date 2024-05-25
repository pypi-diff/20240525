# Comparing `tmp/validators-0.8.tar.gz` & `tmp/validators-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/validators-0.8.tar", last modified: Wed Jun 24 07:31:51 2015, max compression
+gzip compressed data, was "dist/validators-0.9.tar", last modified: Sat Oct 10 06:58:48 2015, max compression
```

## Comparing `validators-0.8.tar` & `validators-0.9.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-06-24 07:31:51.000000 validators-0.8/
--rw-r--r--   0 konsta     (501) staff       (20)     1068 2015-06-24 07:29:26.000000 validators-0.8/CHANGES.rst
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-06-24 07:31:51.000000 validators-0.8/docs/
--rw-r--r--   0 konsta     (501) staff       (20)     8613 2014-09-07 13:24:00.000000 validators-0.8/docs/conf.py
--rw-r--r--   0 konsta     (501) staff       (20)     2638 2014-09-07 13:26:38.000000 validators-0.8/docs/index.rst
--rw-r--r--   0 konsta     (501) staff       (20)     6709 2013-11-28 13:15:23.000000 validators-0.8/docs/make.bat
--rw-r--r--   0 konsta     (501) staff       (20)     6778 2013-11-28 13:15:23.000000 validators-0.8/docs/Makefile
--rw-r--r--   0 konsta     (501) staff       (20)     1089 2014-09-07 13:24:00.000000 validators-0.8/LICENSE
--rw-r--r--   0 konsta     (501) staff       (20)      193 2014-06-25 15:39:24.000000 validators-0.8/MANIFEST.in
--rw-r--r--   0 konsta     (501) staff       (20)     1154 2015-06-24 07:31:51.000000 validators-0.8/PKG-INFO
--rw-r--r--   0 konsta     (501) staff       (20)      602 2014-09-07 13:24:00.000000 validators-0.8/README.rst
--rw-r--r--   0 konsta     (501) staff       (20)       59 2015-06-24 07:31:51.000000 validators-0.8/setup.cfg
--rw-r--r--   0 konsta     (501) staff       (20)     2118 2014-09-07 13:26:38.000000 validators-0.8/setup.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-06-24 07:31:51.000000 validators-0.8/tests/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2013-11-28 13:15:23.000000 validators-0.8/tests/__init__.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-06-24 07:31:51.000000 validators-0.8/tests/i18n/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2013-11-28 13:15:23.000000 validators-0.8/tests/i18n/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     1032 2013-11-28 13:15:23.000000 validators-0.8/tests/i18n/test_fi.py
--rw-r--r--   0 konsta     (501) staff       (20)      862 2013-11-28 13:15:23.000000 validators-0.8/tests/test_between.py
--rw-r--r--   0 konsta     (501) staff       (20)     1201 2013-11-28 13:15:23.000000 validators-0.8/tests/test_email.py
--rw-r--r--   0 konsta     (501) staff       (20)      813 2013-11-28 13:15:23.000000 validators-0.8/tests/test_extremes.py
--rw-r--r--   0 konsta     (501) staff       (20)      443 2015-06-24 07:29:26.000000 validators-0.8/tests/test_iban.py
--rw-r--r--   0 konsta     (501) staff       (20)      533 2013-11-28 13:15:23.000000 validators-0.8/tests/test_ipv4.py
--rw-r--r--   0 konsta     (501) staff       (20)      550 2013-11-28 13:15:23.000000 validators-0.8/tests/test_ipv6.py
--rw-r--r--   0 konsta     (501) staff       (20)      987 2013-11-28 13:15:23.000000 validators-0.8/tests/test_length.py
--rw-r--r--   0 konsta     (501) staff       (20)      536 2013-11-28 13:15:23.000000 validators-0.8/tests/test_mac_address.py
--rw-r--r--   0 konsta     (501) staff       (20)      477 2014-06-25 12:19:52.000000 validators-0.8/tests/test_slug.py
--rw-r--r--   0 konsta     (501) staff       (20)      830 2013-11-28 13:15:23.000000 validators-0.8/tests/test_url.py
--rw-r--r--   0 konsta     (501) staff       (20)      600 2013-11-28 13:15:23.000000 validators-0.8/tests/test_uuid.py
--rw-r--r--   0 konsta     (501) staff       (20)      605 2013-11-28 13:15:23.000000 validators-0.8/tests/test_validation_failure.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-06-24 07:31:51.000000 validators-0.8/validators/
--rw-r--r--   0 konsta     (501) staff       (20)      411 2015-06-24 07:31:20.000000 validators-0.8/validators/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     1576 2014-09-07 13:24:00.000000 validators-0.8/validators/between.py
--rw-r--r--   0 konsta     (501) staff       (20)     1913 2014-09-07 13:24:00.000000 validators-0.8/validators/email.py
--rw-r--r--   0 konsta     (501) staff       (20)     1092 2014-09-07 13:24:00.000000 validators-0.8/validators/extremes.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-06-24 07:31:51.000000 validators-0.8/validators/i18n/
--rw-r--r--   0 konsta     (501) staff       (20)       39 2014-09-07 13:24:00.000000 validators-0.8/validators/i18n/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     2214 2014-09-07 13:24:00.000000 validators-0.8/validators/i18n/fi.py
--rw-r--r--   0 konsta     (501) staff       (20)     1166 2015-06-24 07:29:26.000000 validators-0.8/validators/iban.py
--rw-r--r--   0 konsta     (501) staff       (20)     1838 2014-09-07 13:24:00.000000 validators-0.8/validators/ip_address.py
--rw-r--r--   0 konsta     (501) staff       (20)      970 2014-09-07 13:24:00.000000 validators-0.8/validators/length.py
--rw-r--r--   0 konsta     (501) staff       (20)      836 2014-09-07 13:24:00.000000 validators-0.8/validators/mac_address.py
--rw-r--r--   0 konsta     (501) staff       (20)      529 2014-09-07 13:24:00.000000 validators-0.8/validators/slug.py
--rw-r--r--   0 konsta     (501) staff       (20)      900 2014-09-07 13:24:00.000000 validators-0.8/validators/truthy.py
--rw-r--r--   0 konsta     (501) staff       (20)     1078 2014-09-07 13:24:00.000000 validators-0.8/validators/url.py
--rw-r--r--   0 konsta     (501) staff       (20)     2073 2014-09-07 13:24:00.000000 validators-0.8/validators/utils.py
--rw-r--r--   0 konsta     (501) staff       (20)      801 2014-09-07 13:24:00.000000 validators-0.8/validators/uuid.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-06-24 07:31:51.000000 validators-0.8/validators.egg-info/
--rw-r--r--   0 konsta     (501) staff       (20)        1 2015-06-24 07:31:51.000000 validators-0.8/validators.egg-info/dependency_links.txt
--rw-r--r--   0 konsta     (501) staff       (20)        1 2013-11-28 13:20:37.000000 validators-0.8/validators.egg-info/not-zip-safe
--rw-r--r--   0 konsta     (501) staff       (20)     1154 2015-06-24 07:31:51.000000 validators-0.8/validators.egg-info/PKG-INFO
--rw-r--r--   0 konsta     (501) staff       (20)       50 2015-06-24 07:31:51.000000 validators-0.8/validators.egg-info/requires.txt
--rw-r--r--   0 konsta     (501) staff       (20)      956 2015-06-24 07:31:51.000000 validators-0.8/validators.egg-info/SOURCES.txt
--rw-r--r--   0 konsta     (501) staff       (20)       11 2015-06-24 07:31:51.000000 validators-0.8/validators.egg-info/top_level.txt
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-10-10 06:58:48.000000 validators-0.9/
+-rw-r--r--   0 konsta     (501) staff       (20)     1193 2015-10-10 06:45:05.000000 validators-0.9/CHANGES.rst
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-10-10 06:58:48.000000 validators-0.9/docs/
+-rw-r--r--   0 konsta     (501) staff       (20)     8613 2014-09-07 13:24:00.000000 validators-0.9/docs/conf.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2775 2015-10-10 06:42:20.000000 validators-0.9/docs/index.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     6709 2013-11-28 13:15:23.000000 validators-0.9/docs/make.bat
+-rw-r--r--   0 konsta     (501) staff       (20)     6778 2013-11-28 13:15:23.000000 validators-0.9/docs/Makefile
+-rw-r--r--   0 konsta     (501) staff       (20)     1089 2014-09-07 13:24:00.000000 validators-0.9/LICENSE
+-rw-r--r--   0 konsta     (501) staff       (20)      193 2014-06-25 15:39:24.000000 validators-0.9/MANIFEST.in
+-rw-r--r--   0 konsta     (501) staff       (20)     1154 2015-10-10 06:58:48.000000 validators-0.9/PKG-INFO
+-rw-r--r--   0 konsta     (501) staff       (20)      602 2014-09-07 13:24:00.000000 validators-0.9/README.rst
+-rw-r--r--   0 konsta     (501) staff       (20)       59 2015-10-10 06:58:48.000000 validators-0.9/setup.cfg
+-rw-r--r--   0 konsta     (501) staff       (20)     2166 2015-10-10 06:54:02.000000 validators-0.9/setup.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-10-10 06:58:48.000000 validators-0.9/tests/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2015-10-10 06:47:39.000000 validators-0.9/tests/__init__.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-10-10 06:58:48.000000 validators-0.9/tests/i18n/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2015-10-10 06:47:39.000000 validators-0.9/tests/i18n/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1033 2015-10-10 06:47:39.000000 validators-0.9/tests/i18n/test_fi.py
+-rw-r--r--   0 konsta     (501) staff       (20)      863 2015-10-10 06:47:39.000000 validators-0.9/tests/test_between.py
+-rw-r--r--   0 konsta     (501) staff       (20)      496 2015-10-10 06:47:39.000000 validators-0.9/tests/test_domain.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1202 2015-10-10 06:47:39.000000 validators-0.9/tests/test_email.py
+-rw-r--r--   0 konsta     (501) staff       (20)      814 2015-10-10 06:47:39.000000 validators-0.9/tests/test_extremes.py
+-rw-r--r--   0 konsta     (501) staff       (20)      444 2015-10-10 06:47:39.000000 validators-0.9/tests/test_iban.py
+-rw-r--r--   0 konsta     (501) staff       (20)      534 2015-10-10 06:47:39.000000 validators-0.9/tests/test_ipv4.py
+-rw-r--r--   0 konsta     (501) staff       (20)      551 2015-10-10 06:47:39.000000 validators-0.9/tests/test_ipv6.py
+-rw-r--r--   0 konsta     (501) staff       (20)      988 2015-10-10 06:47:39.000000 validators-0.9/tests/test_length.py
+-rw-r--r--   0 konsta     (501) staff       (20)      537 2015-10-10 06:47:39.000000 validators-0.9/tests/test_mac_address.py
+-rw-r--r--   0 konsta     (501) staff       (20)      478 2015-10-10 06:47:39.000000 validators-0.9/tests/test_slug.py
+-rw-r--r--   0 konsta     (501) staff       (20)      831 2015-10-10 06:47:39.000000 validators-0.9/tests/test_url.py
+-rw-r--r--   0 konsta     (501) staff       (20)      601 2015-10-10 06:47:39.000000 validators-0.9/tests/test_uuid.py
+-rw-r--r--   0 konsta     (501) staff       (20)      605 2015-10-10 06:47:39.000000 validators-0.9/tests/test_validation_failure.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-10-10 06:58:48.000000 validators-0.9/validators/
+-rw-r--r--   0 konsta     (501) staff       (20)      550 2015-10-10 06:58:08.000000 validators-0.9/validators/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1576 2015-10-10 06:47:54.000000 validators-0.9/validators/between.py
+-rw-r--r--   0 konsta     (501) staff       (20)      610 2015-10-10 06:47:54.000000 validators-0.9/validators/domain.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1913 2015-10-10 06:47:54.000000 validators-0.9/validators/email.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1092 2015-10-10 06:47:54.000000 validators-0.9/validators/extremes.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-10-10 06:58:48.000000 validators-0.9/validators/i18n/
+-rw-r--r--   0 konsta     (501) staff       (20)       47 2015-10-10 06:47:54.000000 validators-0.9/validators/i18n/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2214 2015-10-10 06:47:54.000000 validators-0.9/validators/i18n/fi.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1167 2015-10-10 06:47:54.000000 validators-0.9/validators/iban.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1838 2015-10-10 06:47:54.000000 validators-0.9/validators/ip_address.py
+-rw-r--r--   0 konsta     (501) staff       (20)      970 2015-10-10 06:47:54.000000 validators-0.9/validators/length.py
+-rw-r--r--   0 konsta     (501) staff       (20)      836 2015-10-10 06:47:54.000000 validators-0.9/validators/mac_address.py
+-rw-r--r--   0 konsta     (501) staff       (20)      529 2015-10-10 06:47:54.000000 validators-0.9/validators/slug.py
+-rw-r--r--   0 konsta     (501) staff       (20)      901 2015-10-10 06:47:54.000000 validators-0.9/validators/truthy.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1078 2015-10-10 06:47:54.000000 validators-0.9/validators/url.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2074 2015-10-10 06:47:54.000000 validators-0.9/validators/utils.py
+-rw-r--r--   0 konsta     (501) staff       (20)      801 2015-10-10 06:47:54.000000 validators-0.9/validators/uuid.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2015-10-10 06:58:48.000000 validators-0.9/validators.egg-info/
+-rw-r--r--   0 konsta     (501) staff       (20)        1 2015-10-10 06:58:48.000000 validators-0.9/validators.egg-info/dependency_links.txt
+-rw-r--r--   0 konsta     (501) staff       (20)        1 2013-11-28 13:20:37.000000 validators-0.9/validators.egg-info/not-zip-safe
+-rw-r--r--   0 konsta     (501) staff       (20)     1154 2015-10-10 06:58:48.000000 validators-0.9/validators.egg-info/PKG-INFO
+-rw-r--r--   0 konsta     (501) staff       (20)       77 2015-10-10 06:58:48.000000 validators-0.9/validators.egg-info/requires.txt
+-rw-r--r--   0 konsta     (501) staff       (20)      998 2015-10-10 06:58:48.000000 validators-0.9/validators.egg-info/SOURCES.txt
+-rw-r--r--   0 konsta     (501) staff       (20)       11 2015-10-10 06:58:48.000000 validators-0.9/validators.egg-info/top_level.txt
```

### Comparing `validators-0.8/CHANGES.rst` & `validators-0.9/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Changelog
 ---------
 
-0.8.0 (unreleased)
+
+0.9.0 (2015-10-10)
+^^^^^^^^^^^^^^^^^^
+
+- Added new validator: ``domain``
+- Added flake8 and isort checks in travis config
+
+
+0.8.0 (2015-06-24)
 ^^^^^^^^^^^^^^^^^^
 
 - Added new validator: ``iban``
 
 
 0.7.0 (2014-09-07)
 ^^^^^^^^^^^^^^^^^^
```

### Comparing `validators-0.8/docs/conf.py` & `validators-0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `validators-0.8/docs/index.rst` & `validators-0.9/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -64,22 +64,37 @@
 -------
 
 .. module:: validators.between
 
 .. autofunction:: between
 
 
+domain
+------
+
+.. module:: validators.domain
+
+.. autofunction:: domain
+
+
 email
 -----
 
 .. module:: validators.email
 
 .. autofunction:: email
 
 
+iban
+----
+
+.. module:: validators.iban
+
+.. autofunction:: iban
+
 ipv4
 ----
 
 .. module:: validators.ip_address
 
 .. autofunction:: ipv4
```

### Comparing `validators-0.8/docs/make.bat` & `validators-0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `validators-0.8/docs/Makefile` & `validators-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `validators-0.8/LICENSE` & `validators-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `validators-0.8/PKG-INFO` & `validators-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: validators
-Version: 0.8
+Version: 0.9
 Summary: Python Data Validation for Humans™.
 Home-page: https://github.com/kvesteri/validators
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Description: 
         validators
```

### Comparing `validators-0.8/README.rst` & `validators-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `validators-0.8/setup.py` & `validators-0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     pattern = r"^__version__ = '(.*?)'$"
     return re.search(pattern, contents, re.MULTILINE).group(1)
 
 
 extras_require = {
     'test': [
         'pytest>=2.2.3',
+        'flake8>=2.4.0',
+        'isort>=4.2.2'
     ],
 }
 
 
 setup(
     name='validators',
     version=get_version(),
```

### Comparing `validators-0.8/tests/i18n/test_fi.py` & `validators-0.9/tests/i18n/test_fi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 from validators import fi_business_id, fi_ssn, ValidationFailure
 
 
 @pytest.mark.parametrize(('value',), [
     ('2336509-6',),  # Supercell
     ('0112038-9',),  # Fast Monkeys
     ('2417581-7',),  # Nokia
```

### Comparing `validators-0.8/tests/test_between.py` & `validators-0.9/tests/test_between.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 import validators
 
 
 @pytest.mark.parametrize(('value', 'min', 'max'), [
     (12, 11, 13),
     (12, None, 14),
     (12, 11, None),
```

### Comparing `validators-0.8/tests/test_email.py` & `validators-0.9/tests/test_email.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 from validators import email, ValidationFailure
 
 
 @pytest.mark.parametrize(('value', 'whitelist'), [
     ('email@here.com', None),
     ('weirder-email@here.and.there.com', None),
     ('email@[127.0.0.1]', None),
```

### Comparing `validators-0.8/tests/test_extremes.py` & `validators-0.9/tests/test_extremes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 from validators import Max, Min
 
 
 @pytest.mark.parametrize(('value',), [
     (None,),
     ('',),
     (12,),
```

### Comparing `validators-0.8/tests/test_ipv4.py` & `validators-0.9/tests/test_ipv4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 from validators import ipv4, ValidationFailure
 
 
 @pytest.mark.parametrize(('address',), [
     ('127.0.0.1',),
     ('123.5.77.88',),
     ('12.12.12.12',),
```

### Comparing `validators-0.8/tests/test_ipv6.py` & `validators-0.9/tests/test_ipv6.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 from validators import ipv6, ValidationFailure
 
 
 @pytest.mark.parametrize(('address',), [
     ('::1',),
     ('dead:beef:0:0:0:0:42:1',),
     ('abcd:ef::42:1',),
```

### Comparing `validators-0.8/tests/test_length.py` & `validators-0.9/tests/test_length.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 import validators
 
 
 @pytest.mark.parametrize(('value', 'min', 'max'), [
     ('password', 2, 10),
     ('password', None, 10),
     ('password', 2, None),
```

### Comparing `validators-0.8/tests/test_mac_address.py` & `validators-0.9/tests/test_mac_address.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 from validators import mac_address, ValidationFailure
 
 
 @pytest.mark.parametrize(('address',), [
     ('01:23:45:67:ab:CD',),
 ])
 def test_returns_true_on_valid_mac_address(address):
```

### Comparing `validators-0.8/tests/test_url.py` & `validators-0.9/tests/test_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 from validators import url, ValidationFailure
 
 
 @pytest.mark.parametrize(('address', 'require_tld'), [
     ('http://foobar.dk', True),
     ('http://foobar.dk', True),
     ('http://foobar.museum/foobar', True),
```

### Comparing `validators-0.8/tests/test_uuid.py` & `validators-0.9/tests/test_uuid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pytest
+
 from validators import uuid, ValidationFailure
 
 
 @pytest.mark.parametrize(('value',), [
     ('2bc1c94f-0deb-43e9-92a1-4775189ec9f8',),
 ])
 def test_returns_true_on_valid_mac_address(value):
```

### Comparing `validators-0.8/tests/test_validation_failure.py` & `validators-0.9/tests/test_validation_failure.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import validators
 import six
 
+import validators
 
 obj_repr = (
     "ValidationFailure(func=between"
 )
 
 
 class TestValidationFailure(object):
```

### Comparing `validators-0.8/validators/between.py` & `validators-0.9/validators/between.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .extremes import Min, Max
+from .extremes import Max, Min
 from .utils import validator
 
 
 @validator
 def between(value, min=None, max=None):
     """
     Validate that a number is between minimum and/or maximum value.
```

### Comparing `validators-0.8/validators/email.py` & `validators-0.9/validators/email.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
-from .utils import validator
 
+from .utils import validator
 
 user_regex = re.compile(
     # dot-atom
     r"(^[-!#$%&'*+/=?^_`{}|~0-9A-Z]+"
     r"(\.[-!#$%&'*+/=?^_`{}|~0-9A-Z]+)*$"
     # quoted-string
     r'|^"([\001-\010\013\014\016-\037!#-\[\]-\177]|'
```

### Comparing `validators-0.8/validators/extremes.py` & `validators-0.9/validators/extremes.py`

 * *Files identical despite different names*

### Comparing `validators-0.8/validators/i18n/fi.py` & `validators-0.9/validators/i18n/fi.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
-from validators.utils import validator
 
+from validators.utils import validator
 
 business_id_pattern = re.compile(r'^[0-9]{7}-[0-9]$')
 ssn_checkmarks = '0123456789ABCDEFHJKLMNPRSTUVWXY'
 ssn_pattern = re.compile(
     r"""^
     (?P<date>([0-2]\d|3[01])
     (0\d|1[012])
```

### Comparing `validators-0.8/validators/iban.py` & `validators-0.9/validators/iban.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+
 from .utils import validator
 
 regex = (
     r'^[A-Z]{2}[0-9]{2}[A-Z0-9]{13,30}$'
 )
 pattern = re.compile(regex)
```

### Comparing `validators-0.8/validators/ip_address.py` & `validators-0.9/validators/ip_address.py`

 * *Files identical despite different names*

### Comparing `validators-0.8/validators/length.py` & `validators-0.9/validators/length.py`

 * *Files identical despite different names*

### Comparing `validators-0.8/validators/mac_address.py` & `validators-0.9/validators/mac_address.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
-from .utils import validator
 
+from .utils import validator
 
 pattern = re.compile(r'^(?:[0-9a-fA-F]{2}:){5}[0-9a-fA-F]{2}$')
 
 
 @validator
 def mac_address(value):
     """
```

### Comparing `validators-0.8/validators/slug.py` & `validators-0.9/validators/slug.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
-from .utils import validator
 
+from .utils import validator
 
 slug_regex = re.compile(r'^[-a-zA-Z0-9_]+$')
 
 
 @validator
 def slug(value):
     """
```

### Comparing `validators-0.8/validators/truthy.py` & `validators-0.9/validators/truthy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import six
+
 from .utils import validator
 
 
 @validator
 def truthy(value):
     """
     Validate that given value is not a falsey value.
```

### Comparing `validators-0.8/validators/url.py` & `validators-0.9/validators/url.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
-from .utils import validator
 
+from .utils import validator
 
 regex = (
     r'^[a-z]+://([^/:]+{tld}|([0-9]{{1,3}}\.)'
     r'{{3}}[0-9]{{1,3}})(:[0-9]+)?(\/.*)?$'
 )
 
 pattern_with_tld = re.compile(regex.format(tld=r'\.[a-z]{2,10}'))
```

### Comparing `validators-0.8/validators/utils.py` & `validators-0.9/validators/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 try:
     from collections import OrderedDict
 except ImportError:
     from ordereddict import OrderedDict
-from decorator import decorator
 import inspect
 import itertools
+
 import six
+from decorator import decorator
 
 
 class ValidationFailure(object):
     def __init__(self, func, args):
         self.func = func
         self.__dict__.update(args)
```

### Comparing `validators-0.8/validators/uuid.py` & `validators-0.9/validators/uuid.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
-from .utils import validator
 
+from .utils import validator
 
 pattern = re.compile(r'^[0-9a-fA-F]{8}-([0-9a-fA-F]{4}-){3}[0-9a-fA-F]{12}$')
 
 
 @validator
 def uuid(value):
     """
```

### Comparing `validators-0.8/validators.egg-info/PKG-INFO` & `validators-0.9/validators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: validators
-Version: 0.8
+Version: 0.9
 Summary: Python Data Validation for Humans™.
 Home-page: https://github.com/kvesteri/validators
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Description: 
         validators
```

### Comparing `validators-0.8/validators.egg-info/SOURCES.txt` & `validators-0.9/validators.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 tests/__init__.py
 tests/test_between.py
+tests/test_domain.py
 tests/test_email.py
 tests/test_extremes.py
 tests/test_iban.py
 tests/test_ipv4.py
 tests/test_ipv6.py
 tests/test_length.py
 tests/test_mac_address.py
@@ -20,14 +21,15 @@
 tests/test_url.py
 tests/test_uuid.py
 tests/test_validation_failure.py
 tests/i18n/__init__.py
 tests/i18n/test_fi.py
 validators/__init__.py
 validators/between.py
+validators/domain.py
 validators/email.py
 validators/extremes.py
 validators/iban.py
 validators/ip_address.py
 validators/length.py
 validators/mac_address.py
 validators/slug.py
```

