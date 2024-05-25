# Comparing `tmp/lconrg-2023.12.11.tar.gz` & `tmp/lconrg-2024.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lconrg-2023.12.11.tar", max compression
+gzip compressed data, was "lconrg-2024.5.25.tar", max compression
```

## Comparing `lconrg-2023.12.11.tar` & `lconrg-2024.5.25.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1082 2023-12-11 08:05:01.624845 lconrg-2023.12.11/LICENSE
--rw-r--r--   0        0        0     1086 2023-12-11 08:05:01.628845 lconrg-2023.12.11/pyproject.toml
--rw-r--r--   0        0        0        7 2023-12-11 08:05:01.628845 lconrg-2023.12.11/src/lconrg/.python-version
--rw-r--r--   0        0        0      395 2023-12-11 08:05:01.628845 lconrg-2023.12.11/src/lconrg/__init__.py
--rw-r--r--   0        0        0    33433 2023-12-11 08:05:01.628845 lconrg-2023.12.11/src/lconrg/lconrg.py
--rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 lconrg-2023.12.11/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-25 10:43:51.288151 lconrg-2024.5.25/LICENSE
+-rw-r--r--   0        0        0     1086 2024-05-25 10:43:51.288151 lconrg-2024.5.25/pyproject.toml
+-rw-r--r--   0        0        0        7 2024-05-25 10:43:51.288151 lconrg-2024.5.25/src/lconrg/.python-version
+-rw-r--r--   0        0        0      395 2024-05-25 10:43:51.288151 lconrg-2024.5.25/src/lconrg/__init__.py
+-rw-r--r--   0        0        0    34884 2024-05-25 10:43:51.288151 lconrg-2024.5.25/src/lconrg/lconrg.py
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 lconrg-2024.5.25/PKG-INFO
```

### Comparing `lconrg-2023.12.11/LICENSE` & `lconrg-2024.5.25/LICENSE`

 * *Files identical despite different names*

### Comparing `lconrg-2023.12.11/pyproject.toml` & `lconrg-2024.5.25/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lconrg"
-version = "2023.12.11"
+version = "2024.05.25"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 numpy = "^1.22"
 pandas = "^1.4.1"
```

### Comparing `lconrg-2023.12.11/src/lconrg/lconrg.py` & `lconrg-2024.5.25/src/lconrg/lconrg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Levelised Cost of eNeRGy."""
+
 from collections import namedtuple
 from datetime import date
 from typing import Any, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
@@ -608,16 +609,20 @@
         var = ("variable_opex_kgbp", self.variable_cost_profile(load_factors))
         fuel = ("fuel_kgbp", self.fuel_costs_profile(fuel_prices, load_factors))
         carbon_costs = self.carbon_cost_profile(
             carbon_prices, load_factors, co2_transport_storage_cost
         )
         co2emit = ("carbon_emissions_kgbp", (carbon_costs[0], carbon_costs[1]))
         co2_store = ("carbon_storage_kgbp", (carbon_costs[0], carbon_costs[2]))
+        capacity = (
+            "capacity_mw",
+            self.build_profile(self.net_capacity_mw, self.date_range[0], self.lifetime),
+        )
 
-        source = [production, capital, fixed, var, fuel, co2emit, co2_store]
+        source = [capacity, production, capital, fixed, var, fuel, co2emit, co2_store]
 
         return pd.DataFrame(
             {name: (pd.Series(data[1], index=data[0])) for name, data in source},
         )
 
     def build_pv_cashflows(
         self,
@@ -722,44 +727,81 @@
                 "carbon_storage_kgbp",
             ]
         ]
         lrmc_df = pv_cf[["capital_kgbp", "fixed_opex_kgbp"]]
         srmc = sum(srmc_df.stack().values) / sum(  # type: ignore
             pv_cf.production_GWth.values
         )
+        srmc_cap = (  # type: ignore
+            sum(srmc_df.stack().values)  # type: ignore
+            / sum(pv_cf.capacity_mw.values)  # type: ignore
+            / 1000
+        )
         lrmc = sum(lrmc_df.stack().values) / sum(  # type: ignore
             pv_cf.production_GWth.values
         )
+        lrmc_cap = (  # type: ignore
+            sum(lrmc_df.stack().values)  # type: ignore
+            / sum(pv_cf.capacity_mw.values)  # type: ignore
+            / 1000
+        )
         lcoe = srmc + lrmc
-        full = pv_cf.drop("production_GWth", axis=1).sum() / pv_cf.production_GWth.sum()
+        lcoe_cap = srmc_cap + lrmc_cap
+        full = (
+            pv_cf.drop(["production_GWth", "capacity_mw"], axis=1).sum()
+            / pv_cf.production_GWth.sum()
+        )
+        full_cap = (
+            pv_cf.drop(["production_GWth", "capacity_mw"], axis=1).sum()
+            / pv_cf.capacity_mw.sum()
+            / 1000
+        )
 
         LCONRG = namedtuple(
             "LCONRG",
             [
-                "lcoe",
-                "srmc",
-                "lrmc",
-                "capital_kgbp",
-                "fixed_opex_kgbp",
-                "variable_opex_kgbp",
-                "fuel_kgbp",
-                "carbon_emissions_kgbp",
-                "carbon_storage_kgbp",
+                "lcoe_gbp_mwh",
+                "srmc_gbp_mwh",
+                "lrmc_gbp_mwh",
+                "capital_gbp_mwh",
+                "fixed_opex_gbp_mwh",
+                "variable_opex_gbp_mwh",
+                "fuel_gbp_mwh",
+                "carbon_emissions_gbp_mwh",
+                "carbon_storage_gbp_mwh",
+                "lcoe_gbp_kw",
+                "srmc_gbp_kw",
+                "lrmc_gbp_kw",
+                "capital_gbp_kw",
+                "fixed_opex_gbp_kw",
+                "variable_opex_gbp_kw",
+                "fuel_gbp_kw",
+                "carbon_emissions_gbp_kw",
+                "carbon_storage_gbp_kw",
             ],
         )
         return LCONRG(
             lcoe,
             srmc,
             lrmc,
             full.capital_kgbp,
             full.fixed_opex_kgbp,
             full.variable_opex_kgbp,
             full.fuel_kgbp,
             full.carbon_emissions_kgbp,
             full.carbon_storage_kgbp,
+            lcoe_cap,
+            srmc_cap,
+            lrmc_cap,
+            full_cap.capital_kgbp,
+            full_cap.fixed_opex_kgbp,
+            full_cap.variable_opex_kgbp,
+            full_cap.fuel_kgbp,
+            full_cap.carbon_emissions_kgbp,
+            full_cap.carbon_storage_kgbp,
         )
 
     def calculate_annual_lcoe(
         self,
         load_factors: Union[float, tuple[NDArrayDate, NDArrayFloat], pd.Series],
         fuel_prices: Union[float, tuple[NDArrayDate, NDArrayFloat], pd.Series],
         carbon_prices: Union[float, tuple[NDArrayDate, NDArrayFloat], pd.Series],
@@ -800,15 +842,15 @@
             load_factors, fuel_prices, carbon_prices, co2_transport_storage_cost
         )
         pv_cf["capital_annuity_kgbp"] = (
             sum(pv_cf.capital_kgbp) / sum(pv_cf.production_GWth)
         ) * pv_cf.production_GWth
         pv_cf.drop("capital_kgbp", axis=1, inplace=True)
         pv_profile = (
-            pv_cf.drop("production_GWth", axis=1)
+            pv_cf.drop(["production_GWth", "capacity_mw"], axis=1)
             .divide(pv_cf.production_GWth, axis=0)  # type: ignore
             .sum(axis=1)
         )
         return pv_profile
 
     def calculate_kw_cost(
         self,
```

