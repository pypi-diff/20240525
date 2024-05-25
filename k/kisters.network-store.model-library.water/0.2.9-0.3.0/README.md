# Comparing `tmp/kisters.network_store.model_library.water-0.2.9.tar.gz` & `tmp/kisters.network_store.model_library.water-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kisters.network_store.model_library.water-0.2.9.tar", last modified: Thu Sep 10 12:03:44 2020, max compression
+gzip compressed data, was "kisters.network_store.model_library.water-0.3.0.tar", last modified: Thu Mar 21 11:13:59 2024, max compression
```

## Comparing `kisters.network_store.model_library.water-0.2.9.tar` & `kisters.network_store.model_library.water-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/
--rw-rw-rw-   0 root         (0) root         (0)       90 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1100 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       28 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)    26475 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      838 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      122 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters/network_store/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters/network_store/model_library/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters/network_store/model_library/water/
--rw-rw-rw-   0 root         (0) root         (0)       61 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/kisters/network_store/model_library/water/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/kisters/network_store/model_library/water/groups.py
--rw-rw-rw-   0 root         (0) root         (0)    12921 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/kisters/network_store/model_library/water/links.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/kisters/network_store/model_library/water/nodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters.network_store.model_library.water.egg-info/
--rw-r--r--   0 root         (0) root         (0)      838 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters.network_store.model_library.water.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      771 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters.network_store.model_library.water.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters.network_store.model_library.water.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters.network_store.model_library.water.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters.network_store.model_library.water.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       67 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters.network_store.model_library.water.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/kisters.network_store.model_library.water.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      408 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1380 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:03:44.000000 kisters.network_store.model_library.water-0.2.9/test/
--rw-rw-rw-   0 root         (0) root         (0)    22459 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/test/test_water_models.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2020-09-10 12:03:38.000000 kisters.network_store.model_library.water-0.2.9/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.989477 kisters.network_store.model_library.water-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)    26475 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1174 2024-03-21 11:13:59.989477 kisters.network_store.model_library.water-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.985477 kisters.network_store.model_library.water-0.3.0/kisters/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.985477 kisters.network_store.model_library.water-0.3.0/kisters/network_store/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.985477 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.989477 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)    15027 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/links.py
+-rw-rw-rw-   0 root         (0) root         (0)     5034 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/nodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.988477 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1174 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      771 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       67 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-03-21 11:13:59.990477 kisters.network_store.model_library.water-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.989477 kisters.network_store.model_library.water-0.3.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)    23054 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/test/test_water_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kisters.network_store.model_library.water-0.2.9/.gitlab-ci.yml` & `kisters.network_store.model_library.water-0.3.0/.gitlab-ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-image: python:3.7
+image: python:3.9
 
 before_script:
   - pip install tox
 
 stages:
   - style
   - build
@@ -34,35 +34,35 @@
 
 # test
 .job_template: &unittests
   stage: test
   script:
     - tox -- -vv
 
-py36:linux:
+py39:linux:
   <<: *unittests
-  image: python:3.6-jessie
+  image: python:3.9
   variables:
-    TOXENV: py36
+    TOXENV: py39
   tags:
     - docker
 
-py37:linux:
+py310:linux:
   <<: *unittests
-  image: python:3.7-stretch
+  image: python:3.10
   variables:
-    TOXENV: py37
+    TOXENV: py310
   tags:
     - docker
 
-py38:linux:
+py311:linux:
   <<: *unittests
-  image: python:3.8-buster
+  image: python:3.11
   variables:
-    TOXENV: py38
+    TOXENV: py311
   tags:
     - docker
 
 # coverage
 coverage:
   stage: coverage
   script:
```

### Comparing `kisters.network_store.model_library.water-0.2.9/LICENSE` & `kisters.network_store.model_library.water-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kisters.network_store.model_library.water-0.2.9/kisters/network_store/model_library/water/links.py` & `kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/links.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,55 @@
 import enum
 import math
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Literal, Optional, Union
 
-from kisters.network_store.model_library.base import BaseLink as _BaseLink
-from kisters.network_store.model_library.base import Model as _Model
-from pydantic import Field, validator
+from kisters.network_store.model_library.base import (
+    BaseLink as _BaseLink,
+    Location as _Location,
+    Model as _Model,
+)
+from pydantic import (
+    field_validator,
+    Field,
+    StrictFloat,
+    StrictStr,
+    validator,
+    model_validator,
+)
+from typing_extensions import Self
+
+
+class Polygon(_Model):
+    vertices: List[_Location] = Field(
+        None,
+        description="List of boundary vertices, that define the polygons",
+    )
 
 
 class _Link(_BaseLink):
-    domain: str = Field("water", const=True)
+    domain: Literal["water"] = "water"
 
 
 class Delay(_Link):
-    element_class: str = Field("Delay", const=True)
+    element_class: Literal["Delay"] = "Delay"
     transit_time: float = Field(
         0.0, ge=0.0, description="Time delay in seconds between source and target nodes"
     )
+    multiplier: Optional[Union[StrictFloat, StrictStr]] = Field(
+        None, description="Optional multiplier, outflow = multiplier * inflow"
+    )
 
 
 class PipeFrictionModel(str, enum.Enum):
     DARCY_WEISBACH = "darcy-weisbach"
     HAZEN_WILLIAMS = "hazen-williams"
 
 
 class Pipe(_Link):
-    element_class: str = Field("Pipe", const=True)
+    element_class: Literal["Pipe"] = "Pipe"
     diameter: float = Field(..., gt=0.0, description="Measured internal diameter")
     length: float = Field(..., gt=0.0, description="Longitudinal length of the pipe")
     roughness: float = Field(..., gt=0.0, description="Friction coefficient")
     model: PipeFrictionModel = Field(
         ..., description="Friction loss approximation method"
     )
     check_valve: Optional[bool] = Field(False, description="Disallow reverse flow")
@@ -55,36 +76,41 @@
         description="Local roughness correction (acts as multiplier on base roughness)",
     )
 
 
 class _HydraulicLongitudinalStation(_Model):
     roughness: float = Field(..., gt=0.0, description="Friction coefficient")
     cross_section: List[_HydraulicCrossSectionStation] = Field(
-        ..., min_items=3, description="List of points defining the channel bottom"
+        ..., min_length=3, description="List of points defining the channel bottom"
+    )
+    initial_level: Optional[float] = Field(
+        None, description="Initial level for simulation"
     )
 
-    @validator("cross_section")
+    @field_validator("cross_section")
+    @classmethod
     def check_cross_section_stations(cls, v: Any) -> Any:
         if sorted(v, key=lambda x: x.lr) != v:
             raise ValueError(
                 "Cross Section Stations must be specified in increasing order"
             )
         return v
 
-    @validator("cross_section")
+    @field_validator("cross_section")
+    @classmethod
     def check_non_empty(cls, v: Any) -> Any:
         z = [x.z for x in v]
         if min(z) >= max(z):
             raise ValueError("Empty cross section specified")
         return v
 
 
 class _LongitudinalDelimitedStation(_Model):
     distance: float = Field(
-        ..., ge=0.0, description="Distance along channel from source node"
+        ..., ge=0.0, description="Distance along channel from source node [m]"
     )
 
 
 class _HydraulicLongitudinalDelimitedStation(
     _HydraulicLongitudinalStation, _LongitudinalDelimitedStation
 ):
     pass
@@ -92,115 +118,132 @@
 
 class _HydraulicRouting(_Model):
     model: HydraulicRoutingModel = Field(
         ..., description="Hydraulics approximation equations"
     )
     stations: Union[
         _HydraulicLongitudinalStation, List[_HydraulicLongitudinalDelimitedStation]
-    ] = Field(
-        ..., min_items=1, description="Longitudinal stations defining channel geometry"
-    )
+    ] = Field(..., description="Longitudinal stations defining channel geometry")
     roughness_model: ChannelRoughnessModel = Field(
         ChannelRoughnessModel.CHEZY, description="Friction loss approximation method"
     )
+    initial_flow: Optional[float] = Field(
+        None, description="Initial volumetric flow rate for simulation in m3/s"
+    )
 
-    @validator("stations")
+    @field_validator("stations")
+    @classmethod
     def stations_sorted(cls, v: Any) -> Any:
         if isinstance(v, list):
             return sorted(v, key=lambda x: x.distance)
         return v
 
-    @validator("stations")
+    @field_validator("stations")
+    @classmethod
     def stations_unique(cls, v: Any) -> Any:
         if isinstance(v, list):
             distances = [s.distance for s in v]
             unique_distances = sorted(set(distances))
             if distances != unique_distances:
                 raise ValueError("Two stations may not be placed at the same distance")
         return v
 
 
-class _MuskingumCungeLongitudinalStation(_Model):
-    k: float = Field(..., description="Storage coefficient")
-    x: float = Field(..., description="Weighting factor")
-
-
-class _MuskingumCungeLongitudinalDelimitedStation(
-    _MuskingumCungeLongitudinalStation, _LongitudinalDelimitedStation
-):
-    pass
+class MuskingumLongitudinalStation(_Model):
+    model: Literal["muskingum"] = Field(
+        ..., description="To which models it can be applied"
+    )
+    k: float = Field(..., gt=0.0, description="Storage coefficient")
+    x: float = Field(..., ge=0.0, le=1.0, description="Weighting factor")
 
 
-class HydrologicRoutingModel(str, enum.Enum):
-    MUSKINGUM_CUNGE = "muskingum-cunge"
+class MuskingumCungeLongitudinalStation(_Model):
+    model: Literal["muskingum-cunge"] = Field(
+        ..., description="To which models it can be applied"
+    )
+    roughness: float = Field(..., gt=0.0, description="Friction coefficient")
+    roughness_model: ChannelRoughnessModel = Field(
+        ..., description="Friction loss approximation method"
+    )
+    cross_section: List[_HydraulicCrossSectionStation] = Field(
+        ..., min_length=3, description="List of points defining the channel bottom"
+    )
+    slope: float = Field(..., gt=0.0, description="Longitudinal slope [-]")
 
 
-class _HydrologicRouting(_Model):
-    model: HydrologicRoutingModel = Field(
-        ..., description="Hydrology flow routing scheme"
+class ReservoirLongitudinalStation(_Model):
+    model: Literal["reservoir"] = Field(
+        ..., description="To which models it can be applied"
     )
-    stations: Union[
-        _MuskingumCungeLongitudinalStation,
-        List[_MuskingumCungeLongitudinalDelimitedStation],
-    ] = Field(
-        ...,
-        min_items=1,
-        description="Longitudinal stations characterizing channel hydrology",
+    p: Union[StrictFloat, StrictStr] = Field(
+        ..., description="Reservoir equation multiplier"
+    )
+    m: Union[StrictFloat, StrictStr] = Field(
+        ..., description="Reservoir equation exponent"
     )
 
-    @validator("stations")
-    def stations_sorted(cls, v: Any) -> Any:
-        if isinstance(v, list):
-            return sorted(v, key=lambda x: x.distance)
-        return v
 
-    @validator("stations")
-    def stations_unique(cls, v: Any) -> Any:
-        if isinstance(v, list):
-            distances = [s.distance for s in v]
-            unique_distances = sorted(set(distances))
-            if distances != unique_distances:
-                raise ValueError("Two stations may not be placed at the same distance")
-        return v
+class HydrologicRoutingModel(str, enum.Enum):
+    MUSKINGUM = "muskingum"
+    MUSKINGUM_CUNGE = "muskingum-cunge"
+    RESERVOIR = "reservoir"
+
+
+class HydrologicRouting(_Model):
+    reservoir_station: Optional[ReservoirLongitudinalStation] = Field(None)
+    muskingum_station: Optional[MuskingumLongitudinalStation] = Field(None)
+    muskingum_cunge_station: Optional[MuskingumCungeLongitudinalStation] = Field(None)
 
 
 class Channel(_Link):
-    element_class: str = Field("Channel", const=True)
-    length: float = Field(..., gt=0.0, description="Longitudinal length of the channel")
+    element_class: Literal["Channel"] = "Channel"
+    length: float = Field(
+        ..., gt=0.0, description="Longitudinal length of the channel [m]"
+    )
     hydraulic_routing: _HydraulicRouting = Field(
         None, description="Hydraulic routing model"
     )
-    hydrologic_routing: _HydrologicRouting = Field(
+    hydrologic_routing: HydrologicRouting = Field(
         None, description="Hydrologic routing model"
     )
+    catchment: Optional[Polygon] = Field(
+        None,
+        description="Boundary polygon of the catchment area",
+    )
+    catchment_area: Optional[float] = Field(None, description="Catchment area [km^2]")
 
-    @validator("hydraulic_routing", "hydrologic_routing")
-    def check_distance_less_than_length(cls, v: Any, values: Dict[str, Any]) -> Any:
-        if isinstance(v.stations, list):
-            if v.stations[-1].distance > values["length"]:
-                raise ValueError(
-                    f"Station {v.stations[-1].distance} distance exceeds"
-                    f" length {values['length']}"
-                )
-        return v
+    @model_validator(mode="after")
+    def check_hydraulic_distance_less_than_length(self) -> Self:
+        if self.hydraulic_routing:
+            if isinstance(self.hydraulic_routing.stations, list):
+                if self.hydraulic_routing.stations[-1].distance > self.length:
+                    raise ValueError(
+                        f"Station {self.hydraulic_routing.stations[-1].distance} "
+                        f"distance exceeds length {self.length}"
+                    )
+        return self
 
 
 class FlowControlledStructure(_Link):
-    element_class: str = Field("FlowControlledStructure", const=True)
+    element_class: Literal["FlowControlledStructure"] = "FlowControlledStructure"
     min_flow: float = Field(..., description="Minimum volumetric flow rate in m^3/s")
     max_flow: float = Field(..., description="Maximum volumetric flow rate in m^3/s")
+    initial_flow: Optional[float] = Field(
+        None, description="Initial volumetric flow rate for simulation in m^3/s"
+    )
 
     @validator("max_flow")
     def min_flow_le_max_flow(cls, v: Any, values: Dict[str, Any]) -> Any:
         min_flow = values.get("min_flow")
         if min_flow is not None and v < min_flow:
             raise ValueError("max_flow must be greater than min_flow")
         return v
 
-    @validator("min_flow", "max_flow")
+    @field_validator("min_flow", "max_flow")
+    @classmethod
     def bounds_are_real_valued(cls, v: Any) -> Any:
         if v is not None and not math.isfinite(v):
             raise ValueError("Only real-valued bounds are allowed")
         return v
 
 
 class _PumpTurbineSpeedPoint(_Model):
@@ -209,40 +252,44 @@
     speed: float = Field(1.0, ge=0.0)
 
 
 class _PumpTurbineEfficiencyPoint(_Model):
     flow: float = Field(..., ge=0.0)
     head: float = Field(..., ge=0.0)
     efficiency: float = Field(..., gt=0.0, le=1.0)
+    standard_deviation: Optional[float] = Field(5e-3, ge=0.0, le=1.0)
 
 
 class _PumpTurbineHeadTWCorrection(_Model):
-    link_uid: str = Field(..., regex="^[a-zA-Z]\\w*$")
+    link_uid: str = Field(..., pattern="^[a-zA-Z]\\w*$")
     power: int = Field(..., ge=0.0)
     value: float
 
 
 class _PumpTurbineOtherConstraints(_Model):
     flow_power: int = Field(..., ge=0.0)
     head_power: int = Field(..., ge=0.0)
     value: float
 
 
 class _PumpTurbine(_Link):
     speed: Optional[List[_PumpTurbineSpeedPoint]] = Field(
-        None, min_items=1, description="Flow-head-speed curve of drive shaft"
+        None, min_length=1, description="Flow-head-speed curve of drive shaft"
     )
     efficiency: Optional[List[_PumpTurbineEfficiencyPoint]] = Field(
         None,
-        min_items=1,
+        min_length=1,
         description="Flow-head-efficiency energy conversion curve of assembly",
     )
     length: Optional[float] = Field(None, gt=0.0, description="Length of flow path")
     min_flow: float = Field(..., description="Minimum volumetric flow rate in m^3/s")
     max_flow: float = Field(..., description="Maximum volumetric flow rate in m^3/s")
+    initial_flow: Optional[float] = Field(
+        None, description="Initial volumetric flow rate for simulation in m^3/s"
+    )
     min_head: Optional[float] = Field(None, ge=0.0, description="Minimum head in m")
     max_head: Optional[float] = Field(None, ge=0.0, description="Maximum head in m")
     min_power: float = Field(..., description="Minimum power in W")
     max_power: float = Field(..., description="Maximum power in W")
     min_speed: Optional[float] = Field(None, ge=0.0, description="Minimum speed")
     max_speed: Optional[float] = Field(None, ge=0.0, description="Maximum speed")
     head_tailwater_correction: Optional[List[_PumpTurbineHeadTWCorrection]] = Field(
@@ -250,24 +297,25 @@
         description="This polynomial is added to the difference between"
         " up- and downstream levels",
     )
     other_constraints: Optional[List[_PumpTurbineOtherConstraints]] = Field(
         None, description="Every polynomial will be added a constraint <= 0"
     )
 
-    @validator(
+    @field_validator(
         "min_flow",
         "max_flow",
         "min_head",
         "max_head",
         "min_power",
         "max_power",
         "min_speed",
         "max_speed",
     )
+    @classmethod
     def bounds_are_real_valued(cls, v: Any) -> Any:
         if v is not None and not math.isfinite(v):
             raise ValueError("Only real-valued bounds are allowed")
         return v
 
     @validator("max_flow")
     def min_flow_le_max_flow(cls, v: Any, values: Dict[str, Any]) -> Any:
@@ -295,32 +343,32 @@
         min_speed = values.get("min_speed")
         if min_speed is not None and v < min_speed:
             raise ValueError("max_speed must be greater than min_speed")
         return v
 
 
 class Pump(_PumpTurbine):
-    element_class: str = Field("Pump", const=True)
+    element_class: Literal["Pump"] = "Pump"
 
 
 class Turbine(_PumpTurbine):
-    element_class: str = Field("Turbine", const=True)
+    element_class: Literal["Turbine"] = "Turbine"
 
 
 class ValveModel(str, enum.Enum):
     PRV = "prv"
     PSV = "psv"
     PBV = "pbv"
     FCV = "fcv"
     TCV = "tcv"
     GPV = "gpv"
 
 
 class Valve(_Link):
-    element_class: str = Field("Valve", const=True)
+    element_class: Literal["Valve"] = "Valve"
     model: ValveModel = Field(..., description="Specific type of valve")
     coefficient: float = Field(..., gt=0.0, description="Discharge coefficient")
     diameter: float = Field(
         ..., ge=0.0, description="Measured characteristic internal diameter"
     )
     setting: float = Field(
         ..., description="Valve setting, meaning varies with valve model"
@@ -335,40 +383,49 @@
 
 class _FlowRelation(_Link):
     coefficient: float = Field(..., gt=0.0, description="Discharge coefficient")
     flow_model: FlowModel = Field(..., description="Flow model")
 
 
 class Weir(_FlowRelation):
-    element_class: str = Field("Weir", const=True)
+    element_class: Literal["Weir"] = "Weir"
     min_crest_level: float = Field(..., description="Minimum crest level")
     max_crest_level: float = Field(..., description="Maximum crest level")
+    initial_crest_level: Optional[float] = Field(
+        None, description="Initial crest level value for simulation"
+    )
     crest_width: float = Field(..., gt=0.0)
 
     @validator("max_crest_level")
     def min_crest_level_le_max_crest_level(cls, v: Any, values: Dict[str, Any]) -> Any:
         min_crest_level = values.get("min_crest_level")
         if min_crest_level is not None and v < min_crest_level:
             raise ValueError("max_crest_level must be greater than min_crest_level")
         return v
 
 
 class _TopDownOrifice(_FlowRelation):
     bottom_level: float = Field(..., description="Bottom level")
     min_top_level: float = Field(..., description="Minimum top level")
     max_top_level: float = Field(..., description="Maximum top level")
+    initial_top_level: Optional[float] = Field(
+        None, description="Initial top level value for simulation"
+    )
     reference_width: float = Field(..., gt=0.0)
 
 
 class TopDownRectangularOrifice(_FlowRelation):
-    element_class: str = Field("TopDownRectangularOrifice", const=True)
+    element_class: Literal["TopDownRectangularOrifice"] = "TopDownRectangularOrifice"
 
 
 class TopDownSphericalOrifice(_FlowRelation):
-    element_class: str = Field("TopDownSphericalOrifice", const=True)
+    element_class: Literal["TopDownSphericalOrifice"] = "TopDownSphericalOrifice"
 
 
 class Drain(_FlowRelation):
-    element_class: str = Field("Drain", const=True)
+    element_class: Literal["Drain"] = "Drain"
     level: float = Field(..., description="Level at which drain is installed")
     min_area: float = Field(..., ge=0.0, description="Minimum aperture area")
     max_area: float = Field(..., gt=0.0, description="Maximum aperture area")
+    initial_area: Optional[float] = Field(
+        None, description="Initial area value for simulation"
+    )
```

### Comparing `kisters.network_store.model_library.water-0.2.9/kisters.network_store.model_library.water.egg-info/PKG-INFO` & `kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: kisters.network-store.model-library.water
-Version: 0.2.9
-Summary: Model library for the Kisters Network Store ecosystem
-Home-page: https://gitlab.com/kisters/network-store/model-library-water
-Author: Jesse VanderWees
-Author-email: jesse.vanderwees@kisters-bv.nl
-License: UNKNOWN
-Description: # kisters.network_store.model_library.water
-        
-        The models for the `water` domain of the kisters.network_store.model_library
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: test
+.gitignore
+.gitlab-ci.yml
+AUTHORS.md
+LICENSE
+README.md
+setup.cfg
+setup.py
+tox.ini
+kisters.network_store.model_library.water.egg-info/PKG-INFO
+kisters.network_store.model_library.water.egg-info/SOURCES.txt
+kisters.network_store.model_library.water.egg-info/dependency_links.txt
+kisters.network_store.model_library.water.egg-info/entry_points.txt
+kisters.network_store.model_library.water.egg-info/not-zip-safe
+kisters.network_store.model_library.water.egg-info/requires.txt
+kisters.network_store.model_library.water.egg-info/top_level.txt
+kisters/network_store/model_library/water/__init__.py
+kisters/network_store/model_library/water/groups.py
+kisters/network_store/model_library/water/links.py
+kisters/network_store/model_library/water/nodes.py
+test/test_water_models.py
```

### Comparing `kisters.network_store.model_library.water-0.2.9/setup.py` & `kisters.network_store.model_library.water-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,20 +15,20 @@
     author_email="jesse.vanderwees@kisters-bv.nl",
     description="Model library for the Kisters Network Store ecosystem",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/kisters/network-store/model-library-water",
     packages=find_namespace_packages(include=["kisters.*"]),
     zip_safe=False,
-    install_requires=["kisters.network_store.model_library>=0.2.9", "pydantic"],
+    install_requires=["kisters.network_store.model_library>=0.5.0", "pydantic"],
     extras_require={"test": ["pytest"]},
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "kisters.network_store.model_library.util": [
             "water = kisters.network_store.model_library.water"
         ],
```

### Comparing `kisters.network_store.model_library.water-0.2.9/test/test_water_models.py` & `kisters.network_store.model_library.water-0.3.0/test/test_water_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
+import json
 import math
 from typing import Any, Dict
 
 import pytest
-
-from kisters.network_store.model_library.util import (
+from kisters.network_store.model_library.util import (  # element_to_dict,
     all_links,
     all_nodes,
     element_from_dict,
-    element_to_dict,
     elements_mapping,
 )
 
 elements = [
     {
         "uid": "channel1",
         "source_uid": "junction",
@@ -72,43 +71,50 @@
         "domain": "water",
     },
     {
         "uid": "channel3",
         "source_uid": "junction",
         "target_uid": "storage",
         "hydrologic_routing": {
-            "model": "muskingum-cunge",
-            "stations": [
-                {"k": 100.0, "x": 100.0, "distance": 25.0},
-                {"k": 100.0, "x": 100.0, "distance": 75.0},
-            ],
+            "muskingum_station": {"model": "muskingum", "k": 100.0, "x": 0.4},
+            "reservoir_station": {"model": "reservoir", "p": 2.0, "m": 1.0},
         },
         "length": 100.0,
         "display_name": "channel",
         "element_class": "Channel",
+        "user_metadata": {
+            "ArbitraryKey": "1",
+            "ArbitraryKey2": 1.0,
+            "ArbitraryKey3": 1,
+            "ArbitraryKey4": True,
+            "ArbitraryKey5": 1.1,
+        },
         "collection": "links",
         "domain": "water",
     },
     {
         "uid": "channel4",
         "source_uid": "junction",
         "target_uid": "storage",
         "hydrologic_routing": {
-            "model": "muskingum-cunge",
-            "stations": {"k": 100.0, "x": 100.0},
+            "reservoir_station": {
+                "model": "reservoir",
+                "p": 2.0,
+                "m": 1.0,
+            }
         },
         "length": 100.0,
         "display_name": "channel",
         "element_class": "Channel",
         "collection": "links",
         "domain": "water",
     },
     {
         "uid": "delay",
-        "created": "2020-03-04T11:02:16.790000+00:00",
+        "created": "2020-03-04T11:02:16.790000Z",
         "source_uid": "junction",
         "target_uid": "storage",
         "transit_time": 10.0,
         "display_name": "delay",
         "element_class": "Delay",
         "collection": "links",
         "domain": "water",
@@ -280,18 +286,29 @@
     },
     {
         "uid": "storage",
         "location": {"x": 1.0, "y": 1.0, "z": 0.0},
         "level_volume": [
             {"level": 0.0, "volume": 0.0},
             {"level": 10.0, "volume": 10.0},
+            {"level": 20.0, "volume": 20.0},
+            {"level": 30.0, "volume": 30.0},
+        ],
+        "level_volume_interp": "bspline",
+        "level_capacity": [
+            {"level": 0.0, "capacity": 0.0},
+            {"level": 10.0, "capacity": 10.0},
+            {"level": 20.0, "capacity": 20.0},
+            {"level": 30.0, "capacity": 30.0},
         ],
+        "level_capacity_interp": "bspline",
         "display_name": "storage",
         "schematic_location": {"x": 1.0, "y": 1.0, "z": 0.0},
         "element_class": "Storage",
+        "flow_boundary": False,
         "collection": "nodes",
         "domain": "water",
     },
 ]
 
 bad_elements = [
     {
@@ -373,47 +390,46 @@
         "domain": "water",
     },
     {
         "uid": "channel3",
         "source_uid": "junction",
         "target_uid": "storage",
         "hydrologic_routing": {
-            "model": "muskingum-cunge",
-            "stations": {"k": 100.0, "x": 100.0, "distance": 25.0},
+            "model": "muskingum",
+            "stations": {"model": "muskingum", "k": 100.0, "x": 100.0},
         },
         "length": 100.0,
         "display_name": "channel",
         "element_class": "Channel",
         "collection": "links",
         "domain": "water",
     },
     {
         "uid": "channel4",
         "source_uid": "junction",
         "target_uid": "storage",
         "hydrologic_routing": {
             "model": "muskingum-cunge",
-            "stations": [{"k": 100.0, "x": 100.0}],
+            "stations": {
+                "muskingum-cunge": {"model": "muskingum-cunge", "k": 100.0, "x": 100.0}
+            },
         },
         "length": 100.0,
         "display_name": "channel",
         "element_class": "Channel",
         "collection": "links",
         "domain": "water",
     },
     {
         "uid": "channel5",
         "source_uid": "junction",
         "target_uid": "storage",
         "hydrologic_routing": {
-            "model": "muskingum-cunge",
-            "stations": [
-                {"k": 100.0, "x": 100.0, "distance": 50.0},
-                {"k": 100.0, "x": 100.0, "distance": 50.0},
-            ],
+            "model": "muskingum",
+            "stations": {"muskingum": {"model": "muskingum", "k": 100.0, "x": 100.0}},
         },
         "length": 100.0,
         "display_name": "channel",
         "element_class": "Channel",
         "collection": "links",
         "domain": "water",
     },
@@ -490,19 +506,16 @@
         "domain": "water",
     },
     {
         "uid": "channel8",
         "source_uid": "junction",
         "target_uid": "storage",
         "hydrologic_routing": {
-            "model": "muskingum-cunge",
-            "stations": [
-                {"k": 100.0, "x": 100.0, "distance": 25.0},
-                {"k": 100.0, "x": 100.0, "distance": 101.0},
-            ],
+            "model": "muskingum",
+            "stations": {"muskingum": {"model": "muskingum", "k": 100.0, "x": 100.0}},
         },
         "length": 100.0,
         "display_name": "channel",
         "element_class": "Channel",
         "collection": "links",
         "domain": "water",
     },
@@ -578,15 +591,14 @@
         "max_flow": 1.0,
         "min_power": 1.0,
         "max_power": 1.0,
         "display_name": "turbine",
         "element_class": "Turbine",
         "collection": "links",
         "domain": "water",
-        "collection": "links",
     },
     {
         "uid": "pump3",
         "source_uid": "junction",
         "target_uid": "storage",
         "min_flow": 1.0,
         "max_flow": 1.0,
@@ -760,15 +772,17 @@
     },
 ]
 
 
 @pytest.mark.parametrize("element", elements)
 def test_parse(element: Dict[str, Any]) -> None:
     instance = element_from_dict(element)
-    reserialised = element_to_dict(instance)
+    reserialised = json.loads(
+        instance.model_dump_json(exclude_none=True, exclude_unset=True)
+    )
     assert element == reserialised
 
 
 @pytest.mark.parametrize("element", bad_elements)
 def test_parse_bad(element: Dict[str, Any]) -> None:
     with pytest.raises(ValueError):
         element_from_dict(element)
```

