# Comparing `tmp/sdkfabric_starwars-0.1.4.tar.gz` & `tmp/sdkfabric_starwars-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_starwars-0.1.4.tar", last modified: Thu May 23 21:17:08 2024, max compression
+gzip compressed data, was "sdkfabric_starwars-0.1.5.tar", last modified: Sat May 25 07:45:30 2024, max compression
```

## Comparing `sdkfabric_starwars-0.1.4.tar` & `sdkfabric_starwars-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:08.155511 sdkfabric_starwars-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/film.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/film_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/film_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/people.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/people_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/people_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/planet.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/planet_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/planet_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/species.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/species_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/species_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/starship.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/starship_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/starship_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/vehicle_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/vehicle_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:45:30.444854 sdkfabric_starwars-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-25 07:45:30.444854 sdkfabric_starwars-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-25 07:45:26.000000 sdkfabric_starwars-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 07:45:30.444854 sdkfabric_starwars-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:45:30.436854 sdkfabric_starwars-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:45:30.440854 sdkfabric_starwars-0.1.5/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/film.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/film_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/film_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/people.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/people_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/people_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/planet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/planet_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/planet_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/species_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/species_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/starship.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/starship_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/starship_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/vehicle_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-25 07:45:25.000000 sdkfabric_starwars-0.1.5/src/sdk/vehicle_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:45:30.444854 sdkfabric_starwars-0.1.5/src/sdkfabric_starwars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-25 07:45:30.000000 sdkfabric_starwars-0.1.5/src/sdkfabric_starwars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-25 07:45:30.000000 sdkfabric_starwars-0.1.5/src/sdkfabric_starwars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:45:30.000000 sdkfabric_starwars-0.1.5/src/sdkfabric_starwars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-25 07:45:30.000000 sdkfabric_starwars-0.1.5/src/sdkfabric_starwars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-25 07:45:30.000000 sdkfabric_starwars-0.1.5/src/sdkfabric_starwars.egg-info/top_level.txt
```

### Comparing `sdkfabric_starwars-0.1.4/LICENSE` & `sdkfabric_starwars-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/PKG-INFO` & `sdkfabric_starwars-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-starwars
-Version: 0.1.4
+Version: 0.1.5
 Summary: Starwars Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/starwars-python
 Project-URL: Issues, https://github.com/sdk-fabric/starwars-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_starwars-0.1.4/README.md` & `sdkfabric_starwars-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/pyproject.toml` & `sdkfabric_starwars-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-starwars"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Starwars Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/client.py` & `sdkfabric_starwars-0.1.5/src/sdk/client.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/collection.py` & `sdkfabric_starwars-0.1.5/src/sdk/collection.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/film.py` & `sdkfabric_starwars-0.1.5/src/sdk/film.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Film is a single film.
+# A Film is a single film
 class Film(BaseModel):
     title: Optional[str] = Field(default=None, alias="title")
     episode_id: Optional[int] = Field(default=None, alias="episode_id")
     opening_crawl: Optional[str] = Field(default=None, alias="opening_crawl")
     director: Optional[str] = Field(default=None, alias="director")
     producer: Optional[str] = Field(default=None, alias="producer")
     release_date: Optional[datetime.date] = Field(default=None, alias="release_date")
```

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/film_tag.py` & `sdkfabric_starwars-0.1.5/src/sdk/film_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/people.py` & `sdkfabric_starwars-0.1.5/src/sdk/people.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A People is an individual person or character within the Star Wars universe.
+# A People is an individual person or character within the Star Wars universe
 class People(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     birth_year: Optional[str] = Field(default=None, alias="birth_year")
     eye_color: Optional[str] = Field(default=None, alias="eye_color")
     gender: Optional[str] = Field(default=None, alias="gender")
     hair_color: Optional[str] = Field(default=None, alias="hair_color")
     height: Optional[str] = Field(default=None, alias="height")
```

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/people_tag.py` & `sdkfabric_starwars-0.1.5/src/sdk/people_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/planet.py` & `sdkfabric_starwars-0.1.5/src/sdk/planet.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Planet is a large mass, planet or planetoid in the Star Wars Universe, at the time of 0 ABY.
+# A Planet is a large mass, planet or planetoid in the Star Wars Universe, at the time of 0 ABY
 class Planet(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     diameter: Optional[str] = Field(default=None, alias="diameter")
     rotation_period: Optional[str] = Field(default=None, alias="rotation_period")
     orbital_period: Optional[str] = Field(default=None, alias="orbital_period")
     gravity: Optional[str] = Field(default=None, alias="gravity")
     population: Optional[str] = Field(default=None, alias="population")
```

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/planet_tag.py` & `sdkfabric_starwars-0.1.5/src/sdk/planet_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/root.py` & `sdkfabric_starwars-0.1.5/src/sdk/root.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/species.py` & `sdkfabric_starwars-0.1.5/src/sdk/species.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Species is a type of person or character within the Star Wars Universe.
+# A Species is a type of person or character within the Star Wars Universe
 class Species(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     classification: Optional[str] = Field(default=None, alias="classification")
     designation: Optional[str] = Field(default=None, alias="designation")
     average_height: Optional[str] = Field(default=None, alias="average_height")
     average_lifespan: Optional[str] = Field(default=None, alias="average_lifespan")
     eye_colors: Optional[str] = Field(default=None, alias="eye_colors")
```

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/species_tag.py` & `sdkfabric_starwars-0.1.5/src/sdk/species_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/starship.py` & `sdkfabric_starwars-0.1.5/src/sdk/starship.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Starship is a single transport craft that has hyperdrive capability.
+# A Starship is a single transport craft that has hyperdrive capability
 class Starship(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     model: Optional[str] = Field(default=None, alias="model")
     starship_class: Optional[str] = Field(default=None, alias="starship_class")
     manufacturer: Optional[str] = Field(default=None, alias="manufacturer")
     cost_in_credits: Optional[str] = Field(default=None, alias="cost_in_credits")
     length: Optional[str] = Field(default=None, alias="length")
```

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/starship_tag.py` & `sdkfabric_starwars-0.1.5/src/sdk/starship_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/vehicle.py` & `sdkfabric_starwars-0.1.5/src/sdk/vehicle.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Vehicle is a single transport craft that does not have hyperdrive capability.
+# A Vehicle is a single transport craft that does not have hyperdrive capability
 class Vehicle(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     model: Optional[str] = Field(default=None, alias="model")
     vehicle_class: Optional[str] = Field(default=None, alias="vehicle_class")
     manufacturer: Optional[str] = Field(default=None, alias="manufacturer")
     length: Optional[str] = Field(default=None, alias="length")
     cost_in_credits: Optional[str] = Field(default=None, alias="cost_in_credits")
```

### Comparing `sdkfabric_starwars-0.1.4/src/sdk/vehicle_tag.py` & `sdkfabric_starwars-0.1.5/src/sdk/vehicle_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/PKG-INFO` & `sdkfabric_starwars-0.1.5/src/sdkfabric_starwars.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-starwars
-Version: 0.1.4
+Version: 0.1.5
 Summary: Starwars Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/starwars-python
 Project-URL: Issues, https://github.com/sdk-fabric/starwars-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/SOURCES.txt` & `sdkfabric_starwars-0.1.5/src/sdkfabric_starwars.egg-info/SOURCES.txt`

 * *Files identical despite different names*

