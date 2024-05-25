# Comparing `tmp/django_postcodes-1.0.2.tar.gz` & `tmp/django_postcodes-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_postcodes-1.0.2.tar", last modified: Sat May 25 13:35:22 2024, max compression
+gzip compressed data, was "django_postcodes-1.0.3.tar", last modified: Sat May 25 17:22:33 2024, max compression
```

## Comparing `django_postcodes-1.0.2.tar` & `django_postcodes-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.100762 django_postcodes-1.0.2/
--rw-rw-rw-   0        0        0    18429 2024-05-24 22:58:35.000000 django_postcodes-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      237 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7979 2024-05-25 13:35:22.100762 django_postcodes-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6807 2024-05-25 13:34:25.000000 django_postcodes-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.098766 django_postcodes-1.0.2/django_postcodes.egg-info/
--rw-rw-rw-   0        0        0     7979 2024-05-25 13:35:21.000000 django_postcodes-1.0.2/django_postcodes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2024-05-25 13:35:22.000000 django_postcodes-1.0.2/django_postcodes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 13:35:21.000000 django_postcodes-1.0.2/django_postcodes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-25 13:35:21.000000 django_postcodes-1.0.2/django_postcodes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 13:35:21.000000 django_postcodes-1.0.2/django_postcodes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.086248 django_postcodes-1.0.2/postcodes/
--rw-rw-rw-   0        0        0        0 2024-05-24 13:07:54.000000 django_postcodes-1.0.2/postcodes/__init__.py
--rw-rw-rw-   0        0        0      156 2024-05-24 13:07:54.000000 django_postcodes-1.0.2/postcodes/apps.py
--rw-rw-rw-   0        0        0     7945 2024-05-24 22:23:16.000000 django_postcodes-1.0.2/postcodes/countries.py
--rw-rw-rw-   0        0        0     4791 2024-05-25 13:22:29.000000 django_postcodes-1.0.2/postcodes/postcode.py
--rw-rw-rw-   0        0        0      786 2024-05-24 22:33:00.000000 django_postcodes-1.0.2/postcodes/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.061875 django_postcodes-1.0.2/postcodes/static/
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.061875 django_postcodes-1.0.2/postcodes/static/postcodes/
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.086248 django_postcodes-1.0.2/postcodes/static/postcodes/css/
--rw-rw-rw-   0        0        0      305 2024-05-25 12:16:23.000000 django_postcodes-1.0.2/postcodes/static/postcodes/css/postcodes.css
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.087249 django_postcodes-1.0.2/postcodes/static/postcodes/js/
--rw-rw-rw-   0        0        0     4295 2024-05-25 12:32:27.000000 django_postcodes-1.0.2/postcodes/static/postcodes/js/postcodes.js
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.089248 django_postcodes-1.0.2/postcodes/test/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/__init__.py
--rw-rw-rw-   0        0        0      708 2024-05-24 22:41:12.000000 django_postcodes-1.0.2/postcodes/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.089248 django_postcodes-1.0.2/postcodes/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.090752 django_postcodes-1.0.2/postcodes/test/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.091758 django_postcodes-1.0.2/postcodes/test/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     1012 2024-05-24 23:29:16.000000 django_postcodes-1.0.2/postcodes/test/testapp/core/tests.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:35:22.097766 django_postcodes-1.0.2/postcodes/test/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3500 2024-05-24 22:41:51.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      509 2024-05-24 22:39:56.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/postcodes/test/testapp/testapp/wsgi.py
--rw-rw-rw-   0        0        0      173 2024-05-24 22:59:49.000000 django_postcodes-1.0.2/postcodes/urls.py
--rw-rw-rw-   0        0        0     2147 2024-05-25 13:09:08.000000 django_postcodes-1.0.2/postcodes/views.py
--rw-rw-rw-   0        0        0       90 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1137 2024-05-25 13:35:22.101910 django_postcodes-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-05-24 22:26:59.000000 django_postcodes-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.788300 django_postcodes-1.0.3/
+-rw-rw-rw-   0        0        0    18429 2024-05-24 22:58:35.000000 django_postcodes-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      237 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     8352 2024-05-25 17:22:33.787168 django_postcodes-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7180 2024-05-25 17:21:43.000000 django_postcodes-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.785874 django_postcodes-1.0.3/django_postcodes.egg-info/
+-rw-rw-rw-   0        0        0     8352 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 17:22:33.000000 django_postcodes-1.0.3/django_postcodes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.765479 django_postcodes-1.0.3/postcodes/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:07:54.000000 django_postcodes-1.0.3/postcodes/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-05-24 13:07:54.000000 django_postcodes-1.0.3/postcodes/apps.py
+-rw-rw-rw-   0        0        0     7945 2024-05-24 22:23:16.000000 django_postcodes-1.0.3/postcodes/countries.py
+-rw-rw-rw-   0        0        0     4850 2024-05-25 16:57:44.000000 django_postcodes-1.0.3/postcodes/postcode.py
+-rw-rw-rw-   0        0        0      786 2024-05-24 22:33:00.000000 django_postcodes-1.0.3/postcodes/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.740402 django_postcodes-1.0.3/postcodes/static/
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.741410 django_postcodes-1.0.3/postcodes/static/postcodes/
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.766481 django_postcodes-1.0.3/postcodes/static/postcodes/css/
+-rw-rw-rw-   0        0        0      305 2024-05-25 12:16:23.000000 django_postcodes-1.0.3/postcodes/static/postcodes/css/postcodes.css
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.767480 django_postcodes-1.0.3/postcodes/static/postcodes/js/
+-rw-rw-rw-   0        0        0     4420 2024-05-25 17:19:39.000000 django_postcodes-1.0.3/postcodes/static/postcodes/js/postcodes.js
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.768480 django_postcodes-1.0.3/postcodes/test/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/__init__.py
+-rw-rw-rw-   0        0        0      708 2024-05-24 22:41:12.000000 django_postcodes-1.0.3/postcodes/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.769429 django_postcodes-1.0.3/postcodes/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.771404 django_postcodes-1.0.3/postcodes/test/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.771404 django_postcodes-1.0.3/postcodes/test/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1012 2024-05-24 23:29:16.000000 django_postcodes-1.0.3/postcodes/test/testapp/core/tests.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:22:33.780385 django_postcodes-1.0.3/postcodes/test/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3500 2024-05-24 22:41:51.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      509 2024-05-24 22:39:56.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/postcodes/test/testapp/testapp/wsgi.py
+-rw-rw-rw-   0        0        0      173 2024-05-24 22:59:49.000000 django_postcodes-1.0.3/postcodes/urls.py
+-rw-rw-rw-   0        0        0     2159 2024-05-25 16:54:51.000000 django_postcodes-1.0.3/postcodes/views.py
+-rw-rw-rw-   0        0        0       90 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1137 2024-05-25 17:22:33.790841 django_postcodes-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-05-24 22:26:59.000000 django_postcodes-1.0.3/setup.py
```

### Comparing `django_postcodes-1.0.2/LICENSE` & `django_postcodes-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.2/PKG-INFO` & `django_postcodes-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postcodes
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Django app to manage postcode/home number address forms
 Home-page: https://github.com/Nigel2392/postcodes
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -34,14 +34,23 @@
 
 By default we use the free (but rate limited) API from [postcode.go-dev.nl](https://postcode.go-dev.nl/).
 
 You must create an account and get an API key to use this package (in the default configuration).
 
 This API key must be set in the [settings](#settings).
 
+**Features**
+
+* Lookup addresses by postcode and home number
+* Customizable form fields
+* Customizable API endpoint
+* Autofill form fields with the address data
+* Validation of form fields when the address is not found
+* Validation of form fields when user input was given (regex, min, max.)
+
 Quick start
 -----------
 
 1. Install the package via pip:
 
    ```bash
    pip install django-postcodes
@@ -113,25 +122,29 @@
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            lookupPostcode({
                bind: {
                    // These are required for the lookup
                     postcode: document.querySelector('#id_postcode'),
                     home_number: document.querySelector('#id_home_number'),
+
                     // Custom fields returned by the API
                     straat: document.querySelector("#id_street"),
                     woonplaats: document.querySelector("#id_city"),
                     gemeente: document.querySelector("#id_municipality"),
                     provincie: document.querySelector("#id_province"),
                     bouwjaar: document.querySelector("#id_build_year"),
                     vloeroppervlakte: document.querySelector("#id_floor_area"),
-                    latitude: document.querySelector("#id_geo_x"),
-                    longitude: document.querySelector("#id_geo_y"),
-                    rd_x: document.querySelector("#id_rd_x"),
-                    rd_y: document.querySelector("#id_rd_y"),
+
+                    // Or optionally as a queryselector
+                    // If everything is a string - it is safe to omit the DOMContentLoaded eventListener
+                    latitude: "#id_geo_x",
+                    longitude: "#id_geo_y",
+                    rd_x: "#id_rd_x",
+                    rd_y: "#id_rd_y",
                },
                success: function(addr) {
                    console.log(addr);
                },
                error: function(error) {
                    console.log(error);
                }
```

### Comparing `django_postcodes-1.0.2/README.md` & `django_postcodes-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 
 By default we use the free (but rate limited) API from [postcode.go-dev.nl](https://postcode.go-dev.nl/).
 
 You must create an account and get an API key to use this package (in the default configuration).
 
 This API key must be set in the [settings](#settings).
 
+**Features**
+
+* Lookup addresses by postcode and home number
+* Customizable form fields
+* Customizable API endpoint
+* Autofill form fields with the address data
+* Validation of form fields when the address is not found
+* Validation of form fields when user input was given (regex, min, max.)
+
 Quick start
 -----------
 
 1. Install the package via pip:
 
    ```bash
    pip install django-postcodes
@@ -84,25 +93,29 @@
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            lookupPostcode({
                bind: {
                    // These are required for the lookup
                     postcode: document.querySelector('#id_postcode'),
                     home_number: document.querySelector('#id_home_number'),
+
                     // Custom fields returned by the API
                     straat: document.querySelector("#id_street"),
                     woonplaats: document.querySelector("#id_city"),
                     gemeente: document.querySelector("#id_municipality"),
                     provincie: document.querySelector("#id_province"),
                     bouwjaar: document.querySelector("#id_build_year"),
                     vloeroppervlakte: document.querySelector("#id_floor_area"),
-                    latitude: document.querySelector("#id_geo_x"),
-                    longitude: document.querySelector("#id_geo_y"),
-                    rd_x: document.querySelector("#id_rd_x"),
-                    rd_y: document.querySelector("#id_rd_y"),
+
+                    // Or optionally as a queryselector
+                    // If everything is a string - it is safe to omit the DOMContentLoaded eventListener
+                    latitude: "#id_geo_x",
+                    longitude: "#id_geo_y",
+                    rd_x: "#id_rd_x",
+                    rd_y: "#id_rd_y",
                },
                success: function(addr) {
                    console.log(addr);
                },
                error: function(error) {
                    console.log(error);
                }
```

#### html2text {}

```diff
@@ -1,45 +1,49 @@
 postcodes ================ **A dutch postcode lookup app for Django.** By
 default we use the free (but rate limited) API from [postcode.go-dev.nl](https:
 //postcode.go-dev.nl/). You must create an account and get an API key to use
 this package (in the default configuration). This API key must be set in the
-[settings](#settings). Quick start ----------- 1. Install the package via pip:
-```bash pip install django-postcodes ``` 2. Add 'postcodes' to your
-INSTALLED_APPS setting like this: ``` INSTALLED_APPS = [ ..., 'postcodes', ]
-``` 3. Add the postcodes URL to your project's `urls.py`: ```python path
-('postcodes/', include('postcodes.urls', namespace='postcodes')), ``` ##
-Example usage First we must define the appropriate form. This is an example of
-a form that uses the default API endpoint (custom ones can be defined in the
-settings): Every attribute can be customized, except for the postcode and home
-number fields, which are required for the lookup. These are hard-coded. All
-other elements provided in the `bind` object will be filled in with the data
-from the API. ```python class AddressForm(forms.Form): # These are required for
-the lookup postcode = forms.CharField(max_length=10, widget=forms.TextInput
-(attrs={"placeholder": "1234 AB", "class": "postcode", "pattern": "^[0-9]{4}
-(\s+|)[A-Z]{2}$"})) home_number = forms.CharField(max_length=10,
-widget=forms.TextInput(attrs={"placeholder": "123", "class": "home_number"})) #
-Custom fields street = forms.CharField(max_length=255, widget=forms.TextInput
-(attrs={"placeholder": "Main street", "class": "street"})) city =
+[settings](#settings). **Features** * Lookup addresses by postcode and home
+number * Customizable form fields * Customizable API endpoint * Autofill form
+fields with the address data * Validation of form fields when the address is
+not found * Validation of form fields when user input was given (regex, min,
+max.) Quick start ----------- 1. Install the package via pip: ```bash pip
+install django-postcodes ``` 2. Add 'postcodes' to your INSTALLED_APPS setting
+like this: ``` INSTALLED_APPS = [ ..., 'postcodes', ] ``` 3. Add the postcodes
+URL to your project's `urls.py`: ```python path('postcodes/', include
+('postcodes.urls', namespace='postcodes')), ``` ## Example usage First we must
+define the appropriate form. This is an example of a form that uses the default
+API endpoint (custom ones can be defined in the settings): Every attribute can
+be customized, except for the postcode and home number fields, which are
+required for the lookup. These are hard-coded. All other elements provided in
+the `bind` object will be filled in with the data from the API. ```python class
+AddressForm(forms.Form): # These are required for the lookup postcode =
+forms.CharField(max_length=10, widget=forms.TextInput(attrs={"placeholder":
+"1234 AB", "class": "postcode", "pattern": "^[0-9]{4}(\s+|)[A-Z]{2}$"}))
+home_number = forms.CharField(max_length=10, widget=forms.TextInput(attrs=
+{"placeholder": "123", "class": "home_number"})) # Custom fields street =
 forms.CharField(max_length=255, widget=forms.TextInput(attrs={"placeholder":
-"Amsterdam", "class": "city"})) municipality = forms.CharField(max_length=255,
-widget=forms.TextInput(attrs={"placeholder": "Amsterdam", "class":
-"municipality"})) province = forms.CharField(max_length=255,
-widget=forms.TextInput(attrs={"placeholder": "Noord-Holland", "class":
-"province"})) build_year = forms.IntegerField(widget=forms.NumberInput(attrs=
-{"placeholder": "1990", "class": "build_year", "pattern": "^[0-9]{4}$", "min":
-"1900", "max": "2022"})) floor_area = forms.DecimalField
-(widget=forms.NumberInput(attrs={"placeholder": "100", "class": "floor_area",
-"pattern": "^[0-9]{1,3}$"})) # "pattern": "^[0-9]{1,3}$" geo_x =
-forms.DecimalField(widget=forms.NumberInput(attrs={"placeholder": "52.123456",
-"class": "geo_x"})) geo_y = forms.DecimalField(widget=forms.NumberInput(attrs=
-{"placeholder": "4.123456", "class": "geo_y"})) rd_x = forms.DecimalField
-(widget=forms.NumberInput(attrs={"placeholder": "123456", "class": "rd_x"})) #
-Rijksdriehoek rd_y = forms.DecimalField(widget=forms.NumberInput(attrs=
-{"placeholder": "123456", "class": "rd_y"})) # Rijksdriehoek ``` Then we can
-define our template ```html {% extends 'base.html' %} {% block content %}
+"Main street", "class": "street"})) city = forms.CharField(max_length=255,
+widget=forms.TextInput(attrs={"placeholder": "Amsterdam", "class": "city"}))
+municipality = forms.CharField(max_length=255, widget=forms.TextInput(attrs=
+{"placeholder": "Amsterdam", "class": "municipality"})) province =
+forms.CharField(max_length=255, widget=forms.TextInput(attrs={"placeholder":
+"Noord-Holland", "class": "province"})) build_year = forms.IntegerField
+(widget=forms.NumberInput(attrs={"placeholder": "1990", "class": "build_year",
+"pattern": "^[0-9]{4}$", "min": "1900", "max": "2022"})) floor_area =
+forms.DecimalField(widget=forms.NumberInput(attrs={"placeholder": "100",
+"class": "floor_area", "pattern": "^[0-9]{1,3}$"})) # "pattern": "^[0-9]{1,3}$"
+geo_x = forms.DecimalField(widget=forms.NumberInput(attrs={"placeholder":
+"52.123456", "class": "geo_x"})) geo_y = forms.DecimalField
+(widget=forms.NumberInput(attrs={"placeholder": "4.123456", "class": "geo_y"}))
+rd_x = forms.DecimalField(widget=forms.NumberInput(attrs={"placeholder":
+"123456", "class": "rd_x"})) # Rijksdriehoek rd_y = forms.DecimalField
+(widget=forms.NumberInput(attrs={"placeholder": "123456", "class": "rd_y"})) #
+Rijksdriehoek ``` Then we can define our template ```html {% extends
+'base.html' %} {% block content %}
 }">
 {% csrf_token %} {{ form.as_p }} Submit
 ...
 {% endblock %} ``` The form will now automatically fill in the address fields
 when a valid postcode and home number is entered. If it is invalid or not
 found, the error callback will be called. ## Settings ###
 `ADDR_VALIDATOR_API_KEY` The API key to use for the postcode lookup. This will
```

### Comparing `django_postcodes-1.0.2/django_postcodes.egg-info/PKG-INFO` & `django_postcodes-1.0.3/django_postcodes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postcodes
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Django app to manage postcode/home number address forms
 Home-page: https://github.com/Nigel2392/postcodes
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -34,14 +34,23 @@
 
 By default we use the free (but rate limited) API from [postcode.go-dev.nl](https://postcode.go-dev.nl/).
 
 You must create an account and get an API key to use this package (in the default configuration).
 
 This API key must be set in the [settings](#settings).
 
+**Features**
+
+* Lookup addresses by postcode and home number
+* Customizable form fields
+* Customizable API endpoint
+* Autofill form fields with the address data
+* Validation of form fields when the address is not found
+* Validation of form fields when user input was given (regex, min, max.)
+
 Quick start
 -----------
 
 1. Install the package via pip:
 
    ```bash
    pip install django-postcodes
@@ -113,25 +122,29 @@
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            lookupPostcode({
                bind: {
                    // These are required for the lookup
                     postcode: document.querySelector('#id_postcode'),
                     home_number: document.querySelector('#id_home_number'),
+
                     // Custom fields returned by the API
                     straat: document.querySelector("#id_street"),
                     woonplaats: document.querySelector("#id_city"),
                     gemeente: document.querySelector("#id_municipality"),
                     provincie: document.querySelector("#id_province"),
                     bouwjaar: document.querySelector("#id_build_year"),
                     vloeroppervlakte: document.querySelector("#id_floor_area"),
-                    latitude: document.querySelector("#id_geo_x"),
-                    longitude: document.querySelector("#id_geo_y"),
-                    rd_x: document.querySelector("#id_rd_x"),
-                    rd_y: document.querySelector("#id_rd_y"),
+
+                    // Or optionally as a queryselector
+                    // If everything is a string - it is safe to omit the DOMContentLoaded eventListener
+                    latitude: "#id_geo_x",
+                    longitude: "#id_geo_y",
+                    rd_x: "#id_rd_x",
+                    rd_y: "#id_rd_y",
                },
                success: function(addr) {
                    console.log(addr);
                },
                error: function(error) {
                    console.log(error);
                }
```

### Comparing `django_postcodes-1.0.2/django_postcodes.egg-info/SOURCES.txt` & `django_postcodes-1.0.3/django_postcodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.2/postcodes/countries.py` & `django_postcodes-1.0.3/postcodes/countries.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.2/postcodes/postcode.py` & `django_postcodes-1.0.3/postcodes/postcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,18 @@
     response = requests.get(url, headers=headers)
     try:
         data = response.json()
     except:
         raise AddressValidationError(_(f"Endpoint returned an invalid response: {response.text}"))
     
     if response.status_code != 200:
-        raise AddressValidationError(_("Invalid Response status %(status)s") % {"status": response.status_code}, getattr(data, ERROR_ATTRIBUTE, _("Endpoint returned an error response.")))
+        raise AddressValidationError(
+            _("Invalid Response status %(status)s / %(url)s") % {"status": response.status_code, "url": url},
+            getattr(data, ERROR_ATTRIBUTE, _("Endpoint returned an error response."))
+        )
 
     # Create a new address instance
     address = Address(
         postcode=postcode,
         home_number=number,
         data=data,
     )
```

### Comparing `django_postcodes-1.0.2/postcodes/settings.py` & `django_postcodes-1.0.3/postcodes/settings.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.2/postcodes/static/postcodes/js/postcodes.js` & `django_postcodes-1.0.3/postcodes/static/postcodes/js/postcodes.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -24,52 +24,56 @@
             }(t, e || t.value) ? (t.classList.remove(o.min || "is-invalid-min"), !0) : (t.classList.add(o.min || "is-invalid-min"), !1) : ! function(t) {
                 return t && t.hasAttribute("max")
             }(t) || (function(t, e) {
                 let n = t.getAttribute("max");
                 return !n || parseFloat(e) <= parseFloat(n)
             }(t, e || t.value) ? (t.classList.remove(o.max || "is-invalid-max"), !0) : (t.classList.add(o.max || "is-invalid-max"), !1))
     }
-    var i = function(t, e, n, o) {
+
+    function i(t) {
+        return "string" == typeof t ? document.querySelector(t) : t
+    }
+    var r = function(t, e, n, o) {
         return new(n || (n = Promise))((function(i, r) {
             function s(t) {
                 try {
-                    d(o.next(t))
+                    c(o.next(t))
                 } catch (t) {
                     r(t)
                 }
             }
 
             function a(t) {
                 try {
-                    d(o.throw(t))
+                    c(o.throw(t))
                 } catch (t) {
                     r(t)
                 }
             }
 
-            function d(t) {
+            function c(t) {
                 var e;
                 t.done ? i(t.value) : (e = t.value, e instanceof n ? e : new n((function(t) {
                     t(e)
                 }))).then(s, a)
             }
-            d((o = o.apply(t, e || [])).next())
+            c((o = o.apply(t, e || [])).next())
         }))
     };
-    const r = {
+    const s = {
             empty: "is-empty",
             invalid: "is-invalid",
             pattern: "is-invalid-pattern",
             min: "is-invalid-min",
             max: "is-invalid-max"
         },
-        s = Object.values(r);
+        a = Object.values(s);
 
-    function a(e, n, o) {
-        return i(this, void 0, void 0, (function*() {
+    function c(e, n, o) {
+        return r(this, void 0, void 0, (function*() {
             if (e = null == e ? void 0 : e.trim(), n = null == n ? void 0 : n.trim(), !e) throw new Error("No postcode provided");
             if (!n) throw new Error("No home number provided");
             let i = o.buildRequest || function(t, e) {
                 let n = function(t) {
                     return t.startsWith("http") || (t.startsWith("/") && (t = t.slice(1)), t = `${window.location.origin}/${t}`), new URL(t)
                 }(d);
                 return n.searchParams.append("postcode", t), n.searchParams.append("home_number", e.toString()), {
@@ -106,68 +110,69 @@
             const l = c.data;
             return o.success && o.success(l), l
         }))
     }
     const d = document.currentScript.dataset.apiUrl;
     if (!d) throw new Error("No API URL provided, cannot initialize postcode lookup module");
     console.log("Postcode lookup module initialized with API URL:", d), window.lookupPostcode = function(t) {
-        return i(this, void 0, void 0, (function*() {
+        return r(this, void 0, void 0, (function*() {
             let n = t.postcode,
-                i = t.home_number;
+                r = t.home_number;
             if (t && t.bind && t.bind.postcode && t.bind.home_number) {
-                const d = t.bind.postcode,
-                    c = t.bind.home_number;
-                delete t.bind.postcode, delete t.bind.home_number;
-                const l = Object.keys(t.bind);
-                if (0 == l.length) throw new Error("At least postcode, home_number and one other field must be bound");
-                const u = t.bind,
-                    m = () => {
-                        if (!n && !i) {
-                            for (let t = 0; t < s.length; t++) {
-                                const e = s[t];
-                                d.classList.remove(e), c.classList.remove(e)
+                let d, l, u;
+                const m = t.bind,
+                    p = () => {
+                        if (!n && !r) {
+                            for (let t = 0; t < a.length; t++) {
+                                const e = a[t];
+                                d.classList.remove(e), l.classList.remove(e)
                             }
-                            for (const t of l) {
-                                const e = u[t];
+                            for (const t of u) {
+                                const e = m[t];
                                 e && (e.value = "")
                             }
                             return !0
                         }
                         return !1
                     },
-                    p = t => {
-                        d.classList.remove(r.invalid), c.classList.remove(r.invalid);
-                        for (const o of l) {
-                            const a = u[o];
-                            if (a) {
-                                const d = t[o];
-                                for (const t of s) a.classList.remove(t);
-                                e(d) || !n && !i ? a.classList.add(r.empty) : (a.classList.remove(r.empty), a.value = d.toString())
+                    v = t => {
+                        d.classList.remove(s.invalid), l.classList.remove(s.invalid);
+                        for (const o of u) {
+                            const i = m[o];
+                            if (i) {
+                                const c = t[o];
+                                for (const t of a) i.classList.remove(t);
+                                e(c) || !n && !r ? i.classList.add(s.empty) : (i.classList.remove(s.empty), i.value = c.toString())
                             }
                         }
                     },
-                    v = e => {
-                        t && t.error && t.error(e), d.classList.add(r.invalid), c.classList.add(r.invalid)
+                    f = e => {
+                        t && t.error && t.error(e), d.classList.add(s.invalid), l.classList.add(s.invalid)
                     },
                     h = e => (e.classList.add("postcodes-input"), () => {
-                        n = d.value, i = c.value, m() || o(e, null, r) && a(n, i, t).then(p).catch(v)
+                        n = d.value, r = l.value, p() || o(e, null, s) && c(n, r, t).then(v).catch(f)
                     }),
-                    f = () => {
-                        for (let t = 0; t < l.length; t++) {
-                            const e = l[t],
-                                n = u[e];
-                            n && (n.classList.add("postcodes-input"), n.addEventListener("change", (() => o(n, null, r))))
+                    b = () => {
+                        if (d = i(t.bind.postcode), l = i(t.bind.home_number), delete t.bind.postcode, delete t.bind.home_number, u = Object.keys(t.bind), 0 == u.length) throw new Error("At least postcode, home_number and one other field must be bound");
+                        for (let t = 0; t < u.length; t++) {
+                            const e = u[t];
+                            m[e] = i(m[e])
+                        }
+                        for (let t = 0; t < u.length; t++) {
+                            const e = u[t],
+                                n = m[e];
+                            n && (n.classList.add("postcodes-input"), n.addEventListener("change", (() => o(n, null, s))))
                         }
-                        d.addEventListener("input", h(d)), c.addEventListener("input", h(c))
+                        d.addEventListener("input", h(d)), l.addEventListener("input", h(l))
                     };
-                "complete" === document.readyState || "interactive" === document.readyState ? f() : document.addEventListener("DOMContentLoaded", f)
+                "complete" === document.readyState || "interactive" === document.readyState ? b() : document.addEventListener("DOMContentLoaded", b)
             } else {
                 if (t && t.bind && (!t.bind.postcode || !t.bind.home_number)) throw new Error("Both postcode and home_number must be bound to use the bind option");
                 try {
-                    return yield a(n, i, t)
+                    return yield c(n, r, t)
                 } catch (e) {
                     throw t && t.error && t.error(e), e
                 }
             }
         }))
     }
 })();
```

### Comparing `django_postcodes-1.0.2/postcodes/test/manage.py` & `django_postcodes-1.0.3/postcodes/test/manage.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.2/postcodes/test/testapp/core/tests.py` & `django_postcodes-1.0.3/postcodes/test/testapp/core/tests.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.2/postcodes/test/testapp/testapp/settings.py` & `django_postcodes-1.0.3/postcodes/test/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django_postcodes-1.0.2/postcodes/views.py` & `django_postcodes-1.0.3/postcodes/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     # An unexpected error occurred
     except Exception as e:
         logger.error(f"An error occurred while checking the address: {e}")
         return JsonResponse({
             "success": False,
             "error": _("An error occurred while checking the address.")
-        })
+        }, status=200)
     
 
     # Return the address information
     return JsonResponse({
         "success": True,
         "data": {
             "home_number":  addr.home_number,
```

### Comparing `django_postcodes-1.0.2/setup.cfg` & `django_postcodes-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 706f 7374 636f   = django-postco
 00000020: 6465 730d 0a76 6572 7369 6f6e 203d 2031  des..version = 1
-00000030: 2e30 2e32 0d0a 6465 7363 7269 7074 696f  .0.2..descriptio
+00000030: 2e30 2e33 0d0a 6465 7363 7269 7074 696f  .0.3..descriptio
 00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
 00000050: 2074 6f20 6d61 6e61 6765 2070 6f73 7463   to manage postc
 00000060: 6f64 652f 686f 6d65 206e 756d 6265 7220  ode/home number 
 00000070: 6164 6472 6573 7320 666f 726d 730d 0a6c  address forms..l
 00000080: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000090: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
 000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
```

