# Comparing `tmp/nokey-0.6.0.tar.gz` & `tmp/nokey-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.6.0.tar", max compression
+gzip compressed data, was "nokey-0.7.0.tar", max compression
```

## Comparing `nokey-0.6.0.tar` & `nokey-0.7.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
--rw-r--r--   0        0        0     1068 2024-04-10 23:28:41.225586 nokey-0.6.0/LICENSE
--rw-r--r--   0        0        0     3269 2024-05-18 19:50:31.691711 nokey-0.6.0/README.md
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.771711 nokey-0.6.0/nokey/__init__.py
--rw-r--r--   0        0        0     5116 2024-05-18 19:53:41.879711 nokey-0.6.0/nokey/activities/bored_api.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.775711 nokey-0.6.0/nokey/animals/__init__.py
--rw-r--r--   0        0        0     2754 2024-05-18 19:53:41.779711 nokey-0.6.0/nokey/animals/dog_api.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:42.019711 nokey-0.6.0/nokey/art_and_images/__init__.py
--rw-r--r--   0        0        0    92946 2024-05-18 19:53:42.027711 nokey-0.6.0/nokey/art_and_images/artic.py
--rw-r--r--   0        0        0     7770 2024-05-18 19:53:42.023711 nokey-0.6.0/nokey/art_and_images/lorem_picsum.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.931711 nokey-0.6.0/nokey/books_and_literature/__init__.py
--rw-r--r--   0        0        0     6079 2024-05-18 19:53:41.931711 nokey-0.6.0/nokey/books_and_literature/gutendex.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.891711 nokey-0.6.0/nokey/calendar/__init__.py
--rw-r--r--   0        0        0     4848 2024-05-18 19:53:41.895711 nokey-0.6.0/nokey/calendar/nager_date.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.783711 nokey-0.6.0/nokey/country_info/__init__.py
--rw-r--r--   0        0        0     4740 2024-05-18 19:53:41.787711 nokey-0.6.0/nokey/country_info/rest_country.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.939711 nokey-0.6.0/nokey/developer_tools/__init__.py
--rw-r--r--   0        0        0     3945 2024-05-18 19:53:41.951711 nokey-0.6.0/nokey/developer_tools/apis_guru.py
--rw-r--r--   0        0        0     3564 2024-05-18 19:53:41.955711 nokey-0.6.0/nokey/developer_tools/filter_lists.py
--rw-r--r--   0        0        0     2578 2024-05-18 19:53:41.955711 nokey-0.6.0/nokey/developer_tools/microlink.py
--rw-r--r--   0        0        0     7314 2024-05-18 19:53:41.943711 nokey-0.6.0/nokey/developer_tools/url_haus.py
--rw-r--r--   0        0        0     1621 2024-05-18 19:53:41.947711 nokey-0.6.0/nokey/developer_tools/url_shortener.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.871711 nokey-0.6.0/nokey/education/__init__.py
--rw-r--r--   0        0        0     2348 2024-05-18 19:53:41.875711 nokey-0.6.0/nokey/education/university_domains_and_names.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.963711 nokey-0.6.0/nokey/finance_and_crypto/__init__.py
--rw-r--r--   0        0        0     5877 2024-05-18 19:53:41.975711 nokey-0.6.0/nokey/finance_and_crypto/coinmap.py
--rw-r--r--   0        0        0     2513 2024-05-18 19:53:41.971711 nokey-0.6.0/nokey/finance_and_crypto/exchange_api.py
--rw-r--r--   0        0        0     1127 2024-05-18 19:53:41.967711 nokey-0.6.0/nokey/finance_and_crypto/wall_street_bets.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.795711 nokey-0.6.0/nokey/food/__init__.py
--rw-r--r--   0        0        0     3198 2024-05-18 19:53:41.799711 nokey-0.6.0/nokey/food/fruityvice.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.903711 nokey-0.6.0/nokey/games/__init__.py
--rw-r--r--   0        0        0     6542 2024-05-18 19:53:41.907711 nokey-0.6.0/nokey/games/free_to_game.py
--rw-r--r--   0        0        0     5382 2024-05-18 19:53:41.911711 nokey-0.6.0/nokey/games/open_trivia_db.py
--rw-r--r--   0        0        0    30240 2024-05-18 19:53:41.915711 nokey-0.6.0/nokey/games/shadify.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.859711 nokey-0.6.0/nokey/geolocation/__init__.py
--rw-r--r--   0        0        0     1045 2024-05-18 19:53:41.859711 nokey-0.6.0/nokey/geolocation/ip_api.py
--rw-r--r--   0        0        0     1874 2024-05-18 19:53:41.863711 nokey-0.6.0/nokey/geolocation/zippopotamus.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.991711 nokey-0.6.0/nokey/government/__init__.py
--rw-r--r--   0        0        0    10654 2024-05-18 19:53:41.995711 nokey-0.6.0/nokey/government/federal_register.py
--rw-r--r--   0        0        0   157333 2024-05-18 19:53:41.999711 nokey-0.6.0/nokey/government/usa_spending.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:42.035711 nokey-0.6.0/nokey/health/__init__.py
--rw-r--r--   0        0        0    32028 2024-05-18 19:53:42.031711 nokey-0.6.0/nokey/health/open_disease.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:42.007711 nokey-0.6.0/nokey/helperFuncs/__init__.py
--rw-r--r--   0        0        0      822 2024-05-18 19:53:42.011711 nokey-0.6.0/nokey/helperFuncs/get_api_list.py
--rw-r--r--   0        0        0     5461 2024-05-18 19:53:42.011711 nokey-0.6.0/nokey/helperFuncs/make_request.py
--rw-r--r--   0        0        0     1041 2024-05-18 19:53:42.015711 nokey-0.6.0/nokey/helperFuncs/nokey_apis.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.839711 nokey-0.6.0/nokey/inspiration/__init__.py
--rw-r--r--   0        0        0     5925 2024-05-18 19:53:41.843711 nokey-0.6.0/nokey/inspiration/dictum.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.803711 nokey-0.6.0/nokey/jokes/__init__.py
--rw-r--r--   0        0        0     3004 2024-05-18 19:53:41.807711 nokey-0.6.0/nokey/jokes/joke_api.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.847711 nokey-0.6.0/nokey/language/__init__.py
--rw-r--r--   0        0        0     1185 2024-05-18 19:53:41.851711 nokey-0.6.0/nokey/language/free_dictionary.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.811711 nokey-0.6.0/nokey/random/__init__.py
--rw-r--r--   0        0        0     1119 2024-05-18 19:53:41.815711 nokey-0.6.0/nokey/random/random_user.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.979711 nokey-0.6.0/nokey/science_and_nature/__init__.py
--rw-r--r--   0        0        0    50596 2024-05-18 19:53:41.987711 nokey-0.6.0/nokey/science_and_nature/integrated_taxonomic_information_system.py
--rw-r--r--   0        0        0     2948 2024-05-18 19:53:41.983711 nokey-0.6.0/nokey/science_and_nature/nobel_prize.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.823711 nokey-0.6.0/nokey/spaceflight/__init__.py
--rw-r--r--   0        0        0     8784 2024-05-18 19:53:41.823711 nokey-0.6.0/nokey/spaceflight/spaceflight_news.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.919711 nokey-0.6.0/nokey/tv_and_film/__init__.py
--rw-r--r--   0        0        0    43523 2024-05-18 19:53:41.923711 nokey-0.6.0/nokey/tv_and_film/star_trek_api.py
--rw-r--r--   0        0        0        0 2024-05-18 19:53:41.831711 nokey-0.6.0/nokey/weather/__init__.py
--rw-r--r--   0        0        0    26115 2024-05-18 19:53:41.835711 nokey-0.6.0/nokey/weather/national_weather_service.py
--rw-r--r--   0        0        0      684 2024-05-18 19:52:25.415711 nokey-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4145 1970-01-01 00:00:00.000000 nokey-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-10 23:28:41.225586 nokey-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3407 2024-05-25 13:37:22.426835 nokey-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.990835 nokey-0.7.0/nokey/__init__.py
+-rw-r--r--   0        0        0     5358 2024-05-25 13:32:20.882835 nokey-0.7.0/nokey/activities/bored_api.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.010835 nokey-0.7.0/nokey/animals/__init__.py
+-rw-r--r--   0        0        0     2991 2024-05-25 13:32:21.014835 nokey-0.7.0/nokey/animals/dog_api.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.130835 nokey-0.7.0/nokey/art_and_images/__init__.py
+-rw-r--r--   0        0        0    93276 2024-05-25 13:32:21.126835 nokey-0.7.0/nokey/art_and_images/artic.py
+-rw-r--r--   0        0        0     8014 2024-05-25 13:32:21.134835 nokey-0.7.0/nokey/art_and_images/lorem_picsum.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.118835 nokey-0.7.0/nokey/books_and_literature/__init__.py
+-rw-r--r--   0        0        0     6320 2024-05-25 13:32:21.122835 nokey-0.7.0/nokey/books_and_literature/gutendex.py
+-rw-r--r--   0        0        0     3495 2024-05-25 13:32:21.106835 nokey-0.7.0/nokey/books_and_literature/stephen_king.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.898835 nokey-0.7.0/nokey/calendar/__init__.py
+-rw-r--r--   0        0        0     5090 2024-05-25 13:32:20.894835 nokey-0.7.0/nokey/calendar/nager_date.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.978835 nokey-0.7.0/nokey/country_info/__init__.py
+-rw-r--r--   0        0        0     4985 2024-05-25 13:32:20.978835 nokey-0.7.0/nokey/country_info/rest_country.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.162835 nokey-0.7.0/nokey/developer_tools/__init__.py
+-rw-r--r--   0        0        0     4187 2024-05-25 13:32:21.158835 nokey-0.7.0/nokey/developer_tools/apis_guru.py
+-rw-r--r--   0        0        0     3809 2024-05-25 13:32:21.150835 nokey-0.7.0/nokey/developer_tools/filter_lists.py
+-rw-r--r--   0        0        0     2862 2024-05-25 13:32:21.154835 nokey-0.7.0/nokey/developer_tools/microlink.py
+-rw-r--r--   0        0        0     7552 2024-05-25 13:32:21.166835 nokey-0.7.0/nokey/developer_tools/url_haus.py
+-rw-r--r--   0        0        0     1964 2024-05-25 13:32:21.162835 nokey-0.7.0/nokey/developer_tools/url_shortener.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.966835 nokey-0.7.0/nokey/education/__init__.py
+-rw-r--r--   0        0        0     2591 2024-05-25 13:32:20.970835 nokey-0.7.0/nokey/education/university_domains_and_names.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.042835 nokey-0.7.0/nokey/finance_and_crypto/__init__.py
+-rw-r--r--   0        0        0     6117 2024-05-25 13:32:21.050835 nokey-0.7.0/nokey/finance_and_crypto/coinmap.py
+-rw-r--r--   0        0        0     2758 2024-05-25 13:32:21.046835 nokey-0.7.0/nokey/finance_and_crypto/exchange_api.py
+-rw-r--r--   0        0        0     1382 2024-05-25 13:32:21.054835 nokey-0.7.0/nokey/finance_and_crypto/wallstreet_bets.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.090835 nokey-0.7.0/nokey/food/__init__.py
+-rw-r--r--   0        0        0     3441 2024-05-25 13:32:21.094835 nokey-0.7.0/nokey/food/fruityvice.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.082835 nokey-0.7.0/nokey/games/__init__.py
+-rw-r--r--   0        0        0     6785 2024-05-25 13:32:21.082835 nokey-0.7.0/nokey/games/free_to_game.py
+-rw-r--r--   0        0        0     5626 2024-05-25 13:32:21.074835 nokey-0.7.0/nokey/games/open_trivia_db.py
+-rw-r--r--   0        0        0    30480 2024-05-25 13:32:21.078835 nokey-0.7.0/nokey/games/shadify.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.866835 nokey-0.7.0/nokey/geolocation/__init__.py
+-rw-r--r--   0        0        0     1377 2024-05-25 13:32:20.862835 nokey-0.7.0/nokey/geolocation/ip_api.py
+-rw-r--r--   0        0        0     2119 2024-05-25 13:32:20.866835 nokey-0.7.0/nokey/geolocation/zippopotamus.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.062835 nokey-0.7.0/nokey/government/__init__.py
+-rw-r--r--   0        0        0    10908 2024-05-25 13:32:21.062835 nokey-0.7.0/nokey/government/federal_register.py
+-rw-r--r--   0        0        0   157578 2024-05-25 13:32:21.066835 nokey-0.7.0/nokey/government/usa_spending.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.906835 nokey-0.7.0/nokey/health/__init__.py
+-rw-r--r--   0        0        0    32273 2024-05-25 13:32:20.906835 nokey-0.7.0/nokey/health/open_disease.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.926835 nokey-0.7.0/nokey/helperFuncs/__init__.py
+-rw-r--r--   0        0        0      822 2024-05-25 13:32:20.930835 nokey-0.7.0/nokey/helperFuncs/get_api_list.py
+-rw-r--r--   0        0        0     6851 2024-05-25 13:32:20.926835 nokey-0.7.0/nokey/helperFuncs/make_request.py
+-rw-r--r--   0        0        0     1076 2024-05-25 13:32:20.934835 nokey-0.7.0/nokey/helperFuncs/nokey_apis.py
+-rw-r--r--   0        0        0     1514 2024-05-25 13:32:20.962835 nokey-0.7.0/nokey/helperFuncs/throttler.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.838835 nokey-0.7.0/nokey/inspiration/__init__.py
+-rw-r--r--   0        0        0     6164 2024-05-25 13:32:20.834835 nokey-0.7.0/nokey/inspiration/dictum.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.038835 nokey-0.7.0/nokey/jokes/__init__.py
+-rw-r--r--   0        0        0     3342 2024-05-25 13:32:21.034835 nokey-0.7.0/nokey/jokes/joke_api.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.006835 nokey-0.7.0/nokey/language/__init__.py
+-rw-r--r--   0        0        0     1433 2024-05-25 13:32:21.006835 nokey-0.7.0/nokey/language/free_dictionary.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.998835 nokey-0.7.0/nokey/random/__init__.py
+-rw-r--r--   0        0        0     1363 2024-05-25 13:32:20.998835 nokey-0.7.0/nokey/random/random_user.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.182835 nokey-0.7.0/nokey/science_and_nature/__init__.py
+-rw-r--r--   0        0        0    50832 2024-05-25 13:32:21.174835 nokey-0.7.0/nokey/science_and_nature/integrated_taxonomic_information_system.py
+-rw-r--r--   0        0        0     3192 2024-05-25 13:32:21.178835 nokey-0.7.0/nokey/science_and_nature/nobel_prize.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.990835 nokey-0.7.0/nokey/spaceflight/__init__.py
+-rw-r--r--   0        0        0     9033 2024-05-25 13:32:20.986835 nokey-0.7.0/nokey/spaceflight/spaceflight_news.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.874835 nokey-0.7.0/nokey/tv_and_film/__init__.py
+-rw-r--r--   0        0        0    43761 2024-05-25 13:32:20.878835 nokey-0.7.0/nokey/tv_and_film/star_trek_api.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.846835 nokey-0.7.0/nokey/weather/__init__.py
+-rw-r--r--   0        0        0    26351 2024-05-25 13:32:20.842835 nokey-0.7.0/nokey/weather/national_weather_service.py
+-rw-r--r--   0        0        0      711 2024-05-25 13:39:44.190835 nokey-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 nokey-0.7.0/PKG-INFO
```

### Comparing `nokey-0.6.0/LICENSE` & `nokey-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.6.0/README.md` & `nokey-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 from nokey.helperFuncs.get_api_list import get_api_list
 
 api_list = get_api_list()
 
 print(api_list)
 ```
 
+Each API class has optional caching with requests_cache. To enable caching, set the use_caching argument when calling the class to True.
+
 Each API class has an "about" attribute that returns a short description of the API. To get the URL for the API documentation of any API, simply call the get_docs_url() method for the API class.
 
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
 # Supported APIs
 ## country_info
```

### Comparing `nokey-0.6.0/nokey/activities/bored_api.py` & `nokey-0.7.0/nokey/activities/bored_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class BoredAPI:
     """
     A class to interact with Bored API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="bored_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://www.boredapi.com/api/"
         self.about = "The Bored API helps you find things to do when you're bored. There are fields like the number of participants, activity type, and more that help you narrow down your results."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Bored API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/animals/dog_api.py` & `nokey-0.7.0/nokey/animals/dog_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class DogAPI:
     """
     A class to interact with the Dog API.
     
     Attributes:
     - base_url: The base URL for the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="dog_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://dog.ceo/api/"
         self.about = "The Dog API returns URLs for dog images, either at random or by breed."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, baackend=backend, expire_after=expire_after)
+        
     def get_docs_url(self):
         """
         Returns the URL for the Dog API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/art_and_images/artic.py` & `nokey-0.7.0/nokey/art_and_images/artic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
+from .. helperFuncs.throttler import throttle_class
 
+@throttle_class(rate_limit=1, period=1)
 class Artic:
     """
     A class for interacting with the Art Institute of Chicago API.
     
     Attributes:
     - base_url: The base URL of the API.
     - image_api_url: The base URL for accessing the images in this API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="artic_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.artic.edu/api/v1/"
         self.image_api_url ="https://www.artic.edu/iiif/2/"
         self.about = "The Art Institute of Chicago's API provides JSON-formatted data as a REST-style service that allows developers to explore and integrate the museum’s public data into their projects. This API is the same tool that powers our website, our mobile app, and many other technologies in the museum."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Art Institute of Chicago API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/art_and_images/lorem_picsum.py` & `nokey-0.7.0/nokey/art_and_images/lorem_picsum.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import requests
-
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class LoremPicsum:
     """
     A class for interacting with the Lorem Picsum API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="lorem_picsum_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://picsum.photos/"
         self.about = "This is an API for getting placeholder images, a Lorem Ipsum for images."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Lorem Picsum API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/books_and_literature/gutendex.py` & `nokey-0.7.0/nokey/books_and_literature/gutendex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class Gutendex:
     """
     A class for interacting with the Gutendex API.
     
     Attributes:
     base_url: The base URL for the API.
     about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="gutendex_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://gutendex.com/books/"
         self.about = "Gutendex is a JSON web API for Project Gutenberg ebook metadata."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Gutendex API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/calendar/nager_date.py` & `nokey-0.7.0/nokey/calendar/nager_date.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import requests
-
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class NagerDate:
     """
     A class to interact with the Nager.Date API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="nager_date_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://date.nager.at/api/v3/"
         self.about = "The Nager.Date API provides a simple way to query the holidays of over 100 countries. It is also possible to query long weekends."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Nager.Date API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/country_info/rest_country.py` & `nokey-0.7.0/nokey/country_info/rest_country.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 
 class RestCountries:
     """
     A class to interact with the RestCountries API.
     
     Attributes:
     - base_url: The base URL of the RestCountries API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="rest_country_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://restcountries.com/v3.1/"
         self.about = "REST Countries API is a simple REST API from RapidAPI that provides information about countries in the world In JSON format."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns url for API docs.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/developer_tools/apis_guru.py` & `nokey-0.7.0/nokey/developer_tools/apis_guru.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class APIsGuru:
     """
     A class to interact with the APIs.guru API.
     
     Attributes:
     - base_url: The base url for the APIs.guru API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="api_gurus_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.apis.guru/v2/"
         self.about = "The APIs.guru API is a self-proclaimed Wikipedia for APIs, maintaining an Open API directory."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the APIs.guru API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/developer_tools/filter_lists.py` & `nokey-0.7.0/nokey/developer_tools/filter_lists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class FilterLists:
     """
     A class for interacting with the FilterLists API.
     
     Attributes:
     - base_url: The base URL of the FilterLists API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="filter_lists_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://filterlists.com/api/directory/"
         self.about = "The FilterLists Directory API provides lists of filters used by AD blockers."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the FilterLists API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/developer_tools/microlink.py` & `nokey-0.7.0/nokey/developer_tools/microlink.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class Microlink:
     """
     A class for interacting with the Microlink API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
     
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="microlink_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.microlink.io"
-        self.about = "Microlink API provides a powerful API for automating any browser action."
+        self.about = "Microlink API provides a powerful API for automating any browser action. Free use is limited to 50 requests a day."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Microlink API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/developer_tools/url_haus.py` & `nokey-0.7.0/nokey/developer_tools/url_haus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
-
 import requests
-
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 
 class URLHaus:
     """
     A class to interact with the URLHaus API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="urlhaus_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://urlhaus-api.abuse.ch/v1/"
         self.about = "URLhaus is a project operated by abuse.ch. The purpose of the project is to collect, track and share malware URLs, helping network administrators and security analysts to protect their network and customers from cyber threats."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the URLHaus API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/developer_tools/url_shortener.py` & `nokey-0.7.0/nokey/random/random_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,42 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
-class UrlShortener:
+class RandomUserGenerator:
     """
-    A class for interacting with the URL Shortener API.
+    A class to interact with the Random User Generator API.
     
     Attributes:
-    - base_url: The base URL of the URL Shortener API.
+    - base_url: The base url of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
-        self.base_url = "https://is.gd/create.php?"
-        self.about = "This URL Shortener API (from is.gd) is a URL shortener service."
-        
+    def __init__(self, use_caching=False, cache_name="random_user_cache", backend="sqlite", expire_after=3600):
+        self.base_url = "https://randomuser.me/api/"
+        self.about = "The Random User Generator API is a free, open-source API for generating random user data, like Lorem Ipsum for people."
+        
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
-        Returns the URL for the URL Shortener API documentation.
+        Returns the url for the Random User Generator API documentation.
         
         Args:
         - None
         
         Returns:
-        - string: The URL for the API docs
+        - string: URL for API documentation.
         """
-        return "https://is.gd/apishorteningreference.php?"
+        return "https://randomuser.me/"
         
-    def shorten_url(self, url, shorturl=None):
+    def generate_random_user(self):
         """
-        Returns the shortened URL for the given parameters.
+        Returns randomly generated data for a random user.
         
         Args:
-        - url (str): The original URL to be shortened.
-        - shorturl (str): Optional parameter for a desired short URL if available (case sensitive). Must be between 5 and 30 characters. Defaults to None.
+        - None
         
         Returns:
-        - dict: Dictionary containing the shortened URL.
+        -dict: Dictionary containing random information (such as name, DOB, SSN, address, etc) for a random user.
         """
-        if shorturl is not None:
-            if len(shorturl) < 31 and len(shorturl) > 4:
-                endpoint = f"format=json&url={url}&shorturl={shorturl}"
-            else:
-                print("Chosen shortened URL must be between 5 and 30 characters")
-                return ""
-        else:
-            endpoint = f"format=json&url={url}"
-            return mr.make_request(self.base_url+endpoint)
-                    
-                    
+        return mr.make_request(self.base_url)
+
```

### Comparing `nokey-0.6.0/nokey/education/university_domains_and_names.py` & `nokey-0.7.0/nokey/education/university_domains_and_names.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class UniversityDomainsAndNames:
     """
     A class to interact with the University Domains and Names API.
     
     Attributes:
     - base_url: The base url for the University Domains and Names API.
     - about: A short description of the API.
     """
     
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="university_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://universities.hipolabs.com/search?"
         self.about = "This API accesses a list of universities and their domain names."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the url for the University Domains and Names API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/finance_and_crypto/coinmap.py` & `nokey-0.7.0/nokey/finance_and_crypto/coinmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from datetime import date
 from typing import Optional
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class Coinmap:
     """
     A class for interacting with the Coinmap API.
     
     Attributes:
     - base_url: The base URL of the Coinmap API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="coinmap_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://coinmap.org/api/v1/"
         self.about = "The CoinMap API is a free resource to access data about thousands of crypto merchants, ATMs, grocery stores, shops, cafes, and other venues. This API is really simple to use since it has a flat data structure, doesn't require authorization, and a well-described data format."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Coinmap API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/finance_and_crypto/exchange_api.py` & `nokey-0.7.0/nokey/finance_and_crypto/exchange_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class ExchangeAPI:
     """
     A class for interacting with Exchange API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="exchange_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@"
         self.about = "ExchangeAPI is a free currency exchange rates API with 150+ currencies and no rate limits."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the ExchangeAPI documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/finance_and_crypto/wall_street_bets.py` & `nokey-0.7.0/nokey/finance_and_crypto/wallstreet_bets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 
 class WallstreetBets:
     """
     A class to interact with the Wallstreet Bets API.
     
     Attributes:
     - base_url: The base URL of the Wallstreet Bets API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="wallstree_bets_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://tradestie.com/api/v1/apps/reddit"
         self.about = "This API gets the top 50 stocks discussed on the Reddit subreddit, Wallstreetbets"
-
+        
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Wallstreet Bets API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/food/fruityvice.py` & `nokey-0.7.0/nokey/food/fruityvice.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class Fruityvice:
     """
     A class to interact with the Fruityvice API.
     
     Attributes:
     - base_url: The base url of the Fruityvice API.
     - about: A short description of the API.
     """
     
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="fruityvice_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://www.fruityvice.com/api/fruit/"
         self.about = "Fruityvice is an API that provides information on fruits and their nutritional value."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the url for the Fruityvice API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/games/free_to_game.py` & `nokey-0.7.0/nokey/games/free_to_game.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class FreeToGame:
     """
     Class to interact with the Free To Game API.
     
     Attributes:
     - base_url: The base URL of the Free To Game API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="freetogame_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://www.freetogame.com/api/"
         self.about = "The Free To Game API is a way to access programmatically the best free-to-play games and free MMO games."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Free To Game API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/games/open_trivia_db.py` & `nokey-0.7.0/nokey/games/open_trivia_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class OpenTriviaDB:
     """
     A class for interacting with the Open Trivia Database API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="open_trivia_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://opentdb.com/api.php?"
         self.about = "The Open Trivia Database provides a completely free JSON API to retrieve trivia questions for use in programming projects."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Open Trivia Database API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/games/shadify.py` & `nokey-0.7.0/nokey/games/shadify.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class Shadify:
     """
     A class for interacting with the Shadify API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="shadify_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://shadify.dev/api/"
         self.about = "Shadify is a powerful REST API service provides a collection of different puzzle types, like crosswords, Sudoku, word search and so on. The API allows users to generate data for puzzles, check the correctness of solutions, and configure various parameters to change the difficulty of the puzzles."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Shadify API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/geolocation/ip_api.py` & `nokey-0.7.0/nokey/geolocation/ip_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
+from .. helperFuncs.throttler import throttle_class
 
-
+@throttle_class(rate_limit=45, period=60)
 class IP_API:
     """
     A class to interact with the IP API.
     
     Attributes:
     - base_url: The base URL of IP API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="ip_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://ip-api.com/json/" 
         self.about = "The IP API is a fast, reliable, and free IP geolocation API."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns URL for API docs.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/geolocation/zippopotamus.py` & `nokey-0.7.0/nokey/geolocation/zippopotamus.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class Zippopotomus:
     """
     A class to interact with the Zippopotomus API.
     
     Attributes:
     - base_url: The basee URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="zippopotomus_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://api.zippopotam.us/"
         self.about = "Zippopotamus is an open source project that is focused on converting zip codes into valid geographical locations."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Zippopotomus API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/government/federal_register.py` & `nokey-0.7.0/nokey/government/federal_register.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class FederalRegister:
     """
     A class for interacting with the Federal Register API.
     
     Attributes:
     base_url: The base URL of the API.
     about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="federal_register_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://www.federalregister.gov/api/v1/"
         self.about = "FederalRegister.gov provides multiple public API endpoints. These can be used to access information in the Federal Register, the daily journal of the US government."
-   
+        
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Federal Register API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/government/usa_spending.py` & `nokey-0.7.0/nokey/government/usa_spending.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import requests_cache
 import datetime as dt
 from .. helperFuncs import make_request as mr 
 
 current = dt.datetime.now().year
 
 class USAspending:
     """
     A class for interacting with the USA Spending API.
     
     Attributes:
     - base_url: The base URL for the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="usa_spending_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.usaspending.gov/api/v2/"
         self.about = "USAspending is the official open data source of federal spending information, including information about federal awards such as contracts, grants, and loans."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the USAspending API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/health/open_disease.py` & `nokey-0.7.0/nokey/health/open_disease.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class OpenDisease:
     """
     A class for interacting with the Open Disease API.
     
     Attributes:
     - base_url: The base URL for the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="open_disease_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://disease.sh/v3/"
         self.about = "Open Disease is a Third Party API for reliable global disease information, serving COVID and influenza data (Note: None of the data in this API seems to be up to date)"
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Open Disease API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/helperFuncs/get_api_list.py` & `nokey-0.7.0/nokey/helperFuncs/get_api_list.py`

 * *Files identical despite different names*

### Comparing `nokey-0.6.0/nokey/helperFuncs/make_request.py` & `nokey-0.7.0/nokey/helperFuncs/make_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
         # Handle any other unexpected errors
         return {"error": f"An unexpected error occurred: {err}"}
 
+
 def make_request_with_params(url, params):
     """
     Make a request to an API if the API call requires params.
     
     Args:
     - url (str): The url of the API.
     - params (dict): The params to be included in the request.
@@ -83,14 +84,41 @@
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
         # Handle any other unexpected errors
         return {"error": f"An unexpected error occurred: {err}"}
         
+def make_request_for_content_with_params(url, params):
+    """
+    Make a request to an API if the API call returns content other than in JSON format.
+    
+    Args:
+    - url (str): The url of the API.
+    
+    Returns:
+    - string: Text in any format containing either the response data or an error message.
+    """
+    try:
+        response = requests.get(url, params)
+        return response.content
+    except HTTPError as http_err:
+        # Handle HTTP error
+        return {"error": f"HTTP error occurred: {http_err}"}
+    except Timeout:
+        # Handle timeout error
+        return {"error": "Request timed out."}
+    except RequestException as req_err:
+        # Handle other request exceptions
+        return {"error": f"Request exception occurred: {req_err}"}
+    except Exception as err:
+        # Handle any other unexpected errors
+        return {"error": f"An unexpected error occurred: {err}"}
+        
+        
 def make_request_with_post_and_data(url, data):
     """
     Make a request to an API if the API using the POST method.
     
     Args:
     - url (str): The url of the API.
     - data (dict): The data to be included in the request.
@@ -136,11 +164,22 @@
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
         # Handle any other unexpected errors
         return {"error": f"An unexpected error occurred: {err}"}
-   
+        
+def add_params(params, params_list):
+    """
+    Adds parameters to the params dictionary if their values are not None.
+
+    Args:
+        params (dict): The dictionary to add parameters to.
+        params_list (list of tuples): Each tuple contains (original_param_name, new_param_name).
+    """
+    for original_param_name, new_param_name in params_list:
+        if new_param_name is not None:
+            params[original_param_name] = new_param_name
```

### Comparing `nokey-0.6.0/nokey/helperFuncs/nokey_apis.py` & `nokey-0.7.0/nokey/helperFuncs/nokey_apis.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,10 +15,10 @@
     "language": ["Free Dictionary"],
     "games": ["Free To Game", "Open Trivia Database", "Shadify"],
     "activities": ["Bored API"],
     "calendar": ["Nager.Date"],
     "government": ["Federal Register", "USA Spending"],
     "art_and_images": ["Lorem Picsum", "Art Institute of Chicago"],
     "tv_and_film": ["Star Trek API"],
-    "books": ["Gutendex"],
+    "books_and_literature": ["Gutendex", "Stephen King API"],
     "health": ["Open Disease"]
 }
```

### Comparing `nokey-0.6.0/nokey/inspiration/dictum.py` & `nokey-0.7.0/nokey/inspiration/dictum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class Dictum:
     """
     A class for interacting with the Dictum API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="dictum_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.fisenko.net/v1/"
         self.about = "Dictum API provides a programmatic way to access the most inspiring expressions of humanity."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Dictum API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/jokes/joke_api.py` & `nokey-0.7.0/nokey/jokes/joke_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
+from .. helperFuncs.throttler import throttle_class
 
+@throttle_class(rate_limit=120, period=60)
 class JokeAPI:
     """
     A class to interact with the JokeAPI API.
     
     Attributes:
     - base_url: Base URL for interacting with the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching="False", cache_name="joke_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://v2.jokeapi.dev/joke/"
         self.about = "JokeAPI is a REST API that serves uniformly and well formatted jokes. It can be used without any API token, membership, registration or payment. It supports a variety of filters that can be applied to get just the right jokes you need."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the JokeAPI documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/language/free_dictionary.py` & `nokey-0.7.0/nokey/language/free_dictionary.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class FreeDictionary:
     """
     A class to interact with the Free Dictionary API.
     
     Attributes:
     - base_url: The base URL of the Free Dictionary API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="free_dictionary_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.dictionaryapi.dev/api/v2/entries/en/"
         self.about = "The Free Dictionary API is a powerful tool that allows you to access the vast array of dictionary data."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Free Dictionary API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/science_and_nature/integrated_taxonomic_information_system.py` & `nokey-0.7.0/nokey/science_and_nature/integrated_taxonomic_information_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import requests_cache
 import xmltodict
-
 from .. helperFuncs import make_request as mr
 
 class ITIS:
     """ 
     A class for interacting with the Integrated Taxonomic Integration System API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="itis_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://www.itis.gov/ITISWebService/services/ITISService/"
         self.about = "The ITIS program is driven by a mission: communicate a comprehensive taxonomy of global species that enables biodiversity information to be discovered, indexed, and connected across all human endeavors."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the ITIS API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/science_and_nature/nobel_prize.py` & `nokey-0.7.0/nokey/science_and_nature/nobel_prize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class NobelPrizeAPI:
     """
     A class to interact with the Nobel Prize API.
     
     Attributes:
     - base_url: The base url for the Nobel Prize API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="nobel_prize_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.nobelprize.org/2.1/"
         self.about = "The Nobel Prize API returns all information about Laureates and Nobel Prizes."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Nobel Prize API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/spaceflight/spaceflight_news.py` & `nokey-0.7.0/nokey/spaceflight/spaceflight_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class SpaceflightNews:
     
     """
     A class to interact with the Spaceflight News API.
     
     Attributes:
     - base_url: The base URL of the Spaceflight News API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="spaceflight_news_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.spaceflightnewsapi.net/v4/"
         self.about = "The Spaceflight News API (SNAPI) is a product by The Space Devs (TSD). It's the most complete and up-to-date spaceflight news API currently available."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the url for the Spaceflight News API documentation.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/tv_and_film/star_trek_api.py` & `nokey-0.7.0/nokey/tv_and_film/star_trek_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 class STAPI:
     """
     A class for interacting with the Star Trek API.
     
     Attributes:
     - base_url: The base URL of the API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="stapi_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://stapi.co/api/"
         self.about = "STAPI (Star Trek API) is an API for accessing information about all things Star Trek."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns the URL for the Star Trek API.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/nokey/weather/national_weather_service.py` & `nokey-0.7.0/nokey/weather/national_weather_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import requests_cache
 from .. helperFuncs import make_request as mr
 
 
 class NationalWeatherService:
     """
     A class to interact with the National Weather Service API.
     
     Attributes:
     - base_url: The base URL of the National Weather Service API.
     - about: A short description of the API.
     """
-    def __init__(self):
+    def __init__(self, use_caching=False, cache_name="nws_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.weather.gov/"
         self.about = "The National Weather Service (NWS) API allows developers access to critical forecasts, alerts, and observations, along with other weather data."
         
+        if use_caching:
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
+            
     def get_docs_url(self):
         """
         Returns URL for API docs.
         
         Args:
         - None
```

### Comparing `nokey-0.6.0/pyproject.toml` & `nokey-0.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nokey"
-version = "0.6.0"
+version = "0.7.0"
 description = "A python package for accessing APIs that require no key."
 authors = ["Spyder Rex <billyjohnsonauthor@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/SpyderRex/nokey"
 repository = "https://github.com/SpyderRex/nokey"
 license = "MIT"
 keywords = ["API", "requests", "xmltodict"]
@@ -14,12 +14,13 @@
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26.0"
 xmltodict = "==0.13.0"
+requests-cache = "==1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nokey-0.6.0/PKG-INFO` & `nokey-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.6.0
+Version: 0.7.0
 Summary: A python package for accessing APIs that require no key.
 Home-page: https://github.com/SpyderRex/nokey
 License: MIT
 Keywords: API,requests,xmltodict
 Author: Spyder Rex
 Author-email: billyjohnsonauthor@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: requests-cache (==1.2.0)
 Requires-Dist: xmltodict (==0.13.0)
 Project-URL: Repository, https://github.com/SpyderRex/nokey
 Description-Content-Type: text/markdown
 
 # nokey - Access APIs without a Key
 
 nokey is a Python package designed to provide easy access to various APIs that do not require an API key for authentication. This project aims to simplify the process of interacting with different APIs by offering a unified interface for accessing them, all within a single Python package.
@@ -62,14 +63,16 @@
 from nokey.helperFuncs.get_api_list import get_api_list
 
 api_list = get_api_list()
 
 print(api_list)
 ```
 
+Each API class has optional caching with requests_cache. To enable caching, set the use_caching argument when calling the class to True.
+
 Each API class has an "about" attribute that returns a short description of the API. To get the URL for the API documentation of any API, simply call the get_docs_url() method for the API class.
 
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
 # Supported APIs
 ## country_info
```

