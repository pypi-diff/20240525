# Comparing `tmp/tiktok_captcha_solver-0.0.5.tar.gz` & `tmp/tiktok_captcha_solver-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok_captcha_solver-0.0.5.tar", last modified: Wed May 15 13:09:38 2024, max compression
+gzip compressed data, was "tiktok_captcha_solver-0.0.6.tar", last modified: Sat May 25 21:24:00 2024, max compression
```

## Comparing `tiktok_captcha_solver-0.0.5.tar` & `tiktok_captcha_solver-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.966226 tiktok_captcha_solver-0.0.5/
--rw-r--r--   0 gregb     (1000) gregb     (1000)     3533 2024-05-15 13:09:38.966226 tiktok_captcha_solver-0.0.5/PKG-INFO
--rw-r--r--   0 gregb     (1000) gregb     (1000)     2529 2024-05-14 04:00:19.000000 tiktok_captcha_solver-0.0.5/README.md
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1087 2024-05-15 13:09:24.000000 tiktok_captcha_solver-0.0.5/pyproject.toml
--rw-r--r--   0 gregb     (1000) gregb     (1000)       38 2024-05-15 13:09:38.966226 tiktok_captcha_solver-0.0.5/setup.cfg
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.962226 tiktok_captcha_solver-0.0.5/src/
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.964226 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/
--rw-r--r--   0 gregb     (1000) gregb     (1000)      120 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/__init__.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1895 2024-05-12 21:58:21.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/api.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      350 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/downloader.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      335 2024-05-05 06:12:30.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/models.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     8164 2024-05-15 12:47:17.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/playwrightsolver.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     7977 2024-05-15 13:01:27.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/seleniumsolver.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     2196 2024-05-15 13:03:24.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/solver.py
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.965226 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/
--rw-r--r--   0 gregb     (1000) gregb     (1000)        0 2024-05-05 16:49:30.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/__init__.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1264 2024-05-05 17:22:04.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_api.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      189 2024-05-05 17:34:44.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_downloader.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1608 2024-05-15 13:09:16.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_playwrightsolver.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     2356 2024-05-15 13:09:26.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_seleniumsolver.py
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.966226 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/
--rw-r--r--   0 gregb     (1000) gregb     (1000)     3533 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/PKG-INFO
--rw-r--r--   0 gregb     (1000) gregb     (1000)      792 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/SOURCES.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)        1 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/dependency_links.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)      106 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/requires.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)       22 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/top_level.txt
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-25 21:24:00.532695 tiktok_captcha_solver-0.0.6/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     4448 2024-05-25 21:24:00.532695 tiktok_captcha_solver-0.0.6/PKG-INFO
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     3414 2024-05-25 21:22:36.000000 tiktok_captcha_solver-0.0.6/README.md
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1107 2024-05-25 21:23:51.000000 tiktok_captcha_solver-0.0.6/pyproject.toml
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       38 2024-05-25 21:24:00.532695 tiktok_captcha_solver-0.0.6/setup.cfg
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-25 21:24:00.526695 tiktok_captcha_solver-0.0.6/src/
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-25 21:24:00.529695 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      178 2024-05-25 21:20:21.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/__init__.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1895 2024-05-12 21:58:21.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/api.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     8772 2024-05-25 21:07:13.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/asyncplaywrightsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2272 2024-05-25 21:07:11.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/asyncsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      350 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/downloader.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      335 2024-05-05 06:12:30.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/models.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     8164 2024-05-15 12:47:17.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/playwrightsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     7977 2024-05-15 13:01:27.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/seleniumsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2195 2024-05-19 20:31:33.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/solver.py
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-25 21:24:00.531695 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)        0 2024-05-05 16:49:30.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/__init__.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1264 2024-05-05 17:22:04.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/test_api.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1849 2024-05-25 21:22:00.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/test_asyncplaywrightsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      189 2024-05-05 17:34:44.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/test_downloader.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1608 2024-05-25 21:08:16.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/test_playwrightsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2356 2024-05-25 21:08:10.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/test_seleniumsolver.py
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-25 21:24:00.531695 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver.egg-info/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     4448 2024-05-25 21:24:00.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver.egg-info/PKG-INFO
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      946 2024-05-25 21:24:00.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)        1 2024-05-25 21:24:00.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      121 2024-05-25 21:24:00.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver.egg-info/requires.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       22 2024-05-25 21:24:00.000000 tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver.egg-info/top_level.txt
```

### Comparing `tiktok_captcha_solver-0.0.5/PKG-INFO` & `tiktok_captcha_solver-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-captcha-solver
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package integrates with Selenium or Playwright to solve any TikTok captcha in one line of code.
 Author-email: Toughdata LLC <greg@toughdata.net>
 Project-URL: Homepage, https://www.sadcaptcha.com
 Project-URL: Source, https://github.com/gbiz123/tiktok-captcha-solver/
 Keywords: tiktok,captcha,solver,selenium,rotate,puzzle,3d
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -15,38 +15,39 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: selenium
 Requires-Dist: webdriver-manager
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: pytest
+Requires-Dist: pytest-asyncio
 Requires-Dist: playwright
 Requires-Dist: playwright-stealth
 Requires-Dist: undetected_chromedriver
 
 # TikTok Captcha Solver API
 This project is the [SadCaptcha TikTok Captcha Solver](https://www.sadcaptcha.com?ref=ghclientrepo) API client.
-The purpose is to make integrating SadCaptcha into your Selenium or Playwright app as simple as one line of code.
+The purpose is to make integrating SadCaptcha into your Selenium, Playwright, or Async Playwright app as simple as one line of code.
 
 
-Instructions for integrating with Selenium and Playwright are described below in their respective sections.
+Instructions for integrating with Selenium, Playwright, and Async Playwright are described below in their respective sections.
 
 ## Requirements
 - Python >= 3.10
 - **If using Selenium** - Selenium properly installed and in `PATH`
 - **If using Playwright** - Playwright must be properly installed with `playwright install`
 
 ## Installation
 This project can be installed with `pip`. Just run the following command:
 ```
 pip install tiktok-captcha-solver
 ```
 
 ## Selenium Client 
-Import the package, set up the SadCaptcha class, and call it whenever you need.
+Import the package, set up the `SeleniumSolver` class, and call it whenever you need.
 This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
 It is the recommended method if you are using Playwright.
 
 ```py
 from tiktok_captcha_solver import SeleniumSolver
 import undetected_chromedriver as uc
 
@@ -58,17 +59,17 @@
 
 sadcaptcha.solve_captcha_if_present()
 ```
 
 That's it!
 
 ## Playwright Client
-Import the package, set up the SadCaptcha class, and call it whenever you need.
+Import the package, set up the `PlaywrightSolver` class, and call it whenever you need.
 This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
-It is the recommended method if you are using Selenium.
+It is the recommended method if you are using playwright.
 
 ```py
 from tiktok_captcha_solver import PlaywrightSolver
 from playwright.sync_api import Page, sync_playwright
 
 api_key = "YOUR_API_KEY_HERE"
 
@@ -79,14 +80,40 @@
     # Playwright code that causes a TikTok captcha...
 
     sadcaptcha = PlaywrightSolver(page, api_key)
     sadcaptcha.solve_captcha_if_present()
 ```
 That's it!
 
+## Async Playwright Client
+Import the package, set up the `AsyncPlaywrightSolver` class, and call it whenever you need.
+This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
+It is the recommended method if you are using async playwright.
+
+```py
+import asyncio
+from tiktok_captcha_solver import AsyncPlaywrightSolver
+from playwright.async_api import Page, async_playwright
+
+api_key = "YOUR_API_KEY_HERE"
+
+async def main()
+    async with async_playwright() as p:
+        browser = await p.chromium.launch(headless=False)
+        page = await browser.new_page()
+        
+        # Playwright code that causes a TikTok captcha...
+
+        sadcaptcha = AsyncPlaywrightSolver(page, api_key)
+        await sadcaptcha.solve_captcha_if_present()
+
+asyncio.run(main())
+```
+That's it!
+
 ## API Client
 If you are not using Selenium or Playwright, you can still import and use the API client to help you make calls to SadCaptcha
 ```py
 from tiktok_captcha_solver import ApiClient
 
 api_key = "YOUR_API_KEY_HERE"
 client = ApiClient(api_key)
```

### Comparing `tiktok_captcha_solver-0.0.5/README.md` & `tiktok_captcha_solver-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # TikTok Captcha Solver API
 This project is the [SadCaptcha TikTok Captcha Solver](https://www.sadcaptcha.com?ref=ghclientrepo) API client.
-The purpose is to make integrating SadCaptcha into your Selenium or Playwright app as simple as one line of code.
+The purpose is to make integrating SadCaptcha into your Selenium, Playwright, or Async Playwright app as simple as one line of code.
 
 
-Instructions for integrating with Selenium and Playwright are described below in their respective sections.
+Instructions for integrating with Selenium, Playwright, and Async Playwright are described below in their respective sections.
 
 ## Requirements
 - Python >= 3.10
 - **If using Selenium** - Selenium properly installed and in `PATH`
 - **If using Playwright** - Playwright must be properly installed with `playwright install`
 
 ## Installation
 This project can be installed with `pip`. Just run the following command:
 ```
 pip install tiktok-captcha-solver
 ```
 
 ## Selenium Client 
-Import the package, set up the SadCaptcha class, and call it whenever you need.
+Import the package, set up the `SeleniumSolver` class, and call it whenever you need.
 This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
 It is the recommended method if you are using Playwright.
 
 ```py
 from tiktok_captcha_solver import SeleniumSolver
 import undetected_chromedriver as uc
 
@@ -33,17 +33,17 @@
 
 sadcaptcha.solve_captcha_if_present()
 ```
 
 That's it!
 
 ## Playwright Client
-Import the package, set up the SadCaptcha class, and call it whenever you need.
+Import the package, set up the `PlaywrightSolver` class, and call it whenever you need.
 This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
-It is the recommended method if you are using Selenium.
+It is the recommended method if you are using playwright.
 
 ```py
 from tiktok_captcha_solver import PlaywrightSolver
 from playwright.sync_api import Page, sync_playwright
 
 api_key = "YOUR_API_KEY_HERE"
 
@@ -54,14 +54,40 @@
     # Playwright code that causes a TikTok captcha...
 
     sadcaptcha = PlaywrightSolver(page, api_key)
     sadcaptcha.solve_captcha_if_present()
 ```
 That's it!
 
+## Async Playwright Client
+Import the package, set up the `AsyncPlaywrightSolver` class, and call it whenever you need.
+This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
+It is the recommended method if you are using async playwright.
+
+```py
+import asyncio
+from tiktok_captcha_solver import AsyncPlaywrightSolver
+from playwright.async_api import Page, async_playwright
+
+api_key = "YOUR_API_KEY_HERE"
+
+async def main()
+    async with async_playwright() as p:
+        browser = await p.chromium.launch(headless=False)
+        page = await browser.new_page()
+        
+        # Playwright code that causes a TikTok captcha...
+
+        sadcaptcha = AsyncPlaywrightSolver(page, api_key)
+        await sadcaptcha.solve_captcha_if_present()
+
+asyncio.run(main())
+```
+That's it!
+
 ## API Client
 If you are not using Selenium or Playwright, you can still import and use the API client to help you make calls to SadCaptcha
 ```py
 from tiktok_captcha_solver import ApiClient
 
 api_key = "YOUR_API_KEY_HERE"
 client = ApiClient(api_key)
```

### Comparing `tiktok_captcha_solver-0.0.5/pyproject.toml` & `tiktok_captcha_solver-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"  # If not defined, then legacy behavior can happen.
 
 [project]
 name = "tiktok-captcha-solver"
-version = "0.0.5"
+version = "0.0.6"
 
 description = "This package integrates with Selenium or Playwright to solve any TikTok captcha in one line of code."
 readme = "README.md"
 requires-python = ">=3.10"
 
 keywords = ["tiktok", "captcha", "solver", "selenium", "rotate", "puzzle", "3d"]
 
@@ -27,14 +27,15 @@
 
 dependencies = [
   "selenium",
   "webdriver-manager",
   "pydantic",
   "requests",
   "pytest",
+  "pytest-asyncio",
   "playwright",
   "playwright-stealth",
   "undetected_chromedriver"
 ]
 
 [project.urls]
 "Homepage" = "https://www.sadcaptcha.com"
```

### Comparing `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/api.py` & `tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/api.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/playwrightsolver.py` & `tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/playwrightsolver.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/seleniumsolver.py` & `tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/seleniumsolver.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/solver.py` & `tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     @property
     def captcha_wrappers(self) -> list[str]:
         return [
             "div#captcha_container",
             "div.captcha_verify_container",
             "#verify-points",
-            ".captcha_verify_action",
+            ".captcha_verify_action"
         ]
 
     @property
     def rotate_selectors(self) -> list[str]:
         return [
             "[data-testid=whirl-inner-img]",
             "[data-testid=whirl-outer-img]"
```

### Comparing `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_api.py` & `tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_playwrightsolver.py` & `tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/test_playwrightsolver.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_seleniumsolver.py` & `tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver/tests/test_seleniumsolver.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/PKG-INFO` & `tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-captcha-solver
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package integrates with Selenium or Playwright to solve any TikTok captcha in one line of code.
 Author-email: Toughdata LLC <greg@toughdata.net>
 Project-URL: Homepage, https://www.sadcaptcha.com
 Project-URL: Source, https://github.com/gbiz123/tiktok-captcha-solver/
 Keywords: tiktok,captcha,solver,selenium,rotate,puzzle,3d
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -15,38 +15,39 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: selenium
 Requires-Dist: webdriver-manager
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: pytest
+Requires-Dist: pytest-asyncio
 Requires-Dist: playwright
 Requires-Dist: playwright-stealth
 Requires-Dist: undetected_chromedriver
 
 # TikTok Captcha Solver API
 This project is the [SadCaptcha TikTok Captcha Solver](https://www.sadcaptcha.com?ref=ghclientrepo) API client.
-The purpose is to make integrating SadCaptcha into your Selenium or Playwright app as simple as one line of code.
+The purpose is to make integrating SadCaptcha into your Selenium, Playwright, or Async Playwright app as simple as one line of code.
 
 
-Instructions for integrating with Selenium and Playwright are described below in their respective sections.
+Instructions for integrating with Selenium, Playwright, and Async Playwright are described below in their respective sections.
 
 ## Requirements
 - Python >= 3.10
 - **If using Selenium** - Selenium properly installed and in `PATH`
 - **If using Playwright** - Playwright must be properly installed with `playwright install`
 
 ## Installation
 This project can be installed with `pip`. Just run the following command:
 ```
 pip install tiktok-captcha-solver
 ```
 
 ## Selenium Client 
-Import the package, set up the SadCaptcha class, and call it whenever you need.
+Import the package, set up the `SeleniumSolver` class, and call it whenever you need.
 This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
 It is the recommended method if you are using Playwright.
 
 ```py
 from tiktok_captcha_solver import SeleniumSolver
 import undetected_chromedriver as uc
 
@@ -58,17 +59,17 @@
 
 sadcaptcha.solve_captcha_if_present()
 ```
 
 That's it!
 
 ## Playwright Client
-Import the package, set up the SadCaptcha class, and call it whenever you need.
+Import the package, set up the `PlaywrightSolver` class, and call it whenever you need.
 This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
-It is the recommended method if you are using Selenium.
+It is the recommended method if you are using playwright.
 
 ```py
 from tiktok_captcha_solver import PlaywrightSolver
 from playwright.sync_api import Page, sync_playwright
 
 api_key = "YOUR_API_KEY_HERE"
 
@@ -79,14 +80,40 @@
     # Playwright code that causes a TikTok captcha...
 
     sadcaptcha = PlaywrightSolver(page, api_key)
     sadcaptcha.solve_captcha_if_present()
 ```
 That's it!
 
+## Async Playwright Client
+Import the package, set up the `AsyncPlaywrightSolver` class, and call it whenever you need.
+This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
+It is the recommended method if you are using async playwright.
+
+```py
+import asyncio
+from tiktok_captcha_solver import AsyncPlaywrightSolver
+from playwright.async_api import Page, async_playwright
+
+api_key = "YOUR_API_KEY_HERE"
+
+async def main()
+    async with async_playwright() as p:
+        browser = await p.chromium.launch(headless=False)
+        page = await browser.new_page()
+        
+        # Playwright code that causes a TikTok captcha...
+
+        sadcaptcha = AsyncPlaywrightSolver(page, api_key)
+        await sadcaptcha.solve_captcha_if_present()
+
+asyncio.run(main())
+```
+That's it!
+
 ## API Client
 If you are not using Selenium or Playwright, you can still import and use the API client to help you make calls to SadCaptcha
 ```py
 from tiktok_captcha_solver import ApiClient
 
 api_key = "YOUR_API_KEY_HERE"
 client = ApiClient(api_key)
```

### Comparing `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/SOURCES.txt` & `tiktok_captcha_solver-0.0.6/src/tiktok_captcha_solver.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 README.md
 pyproject.toml
 src/tiktok_captcha_solver/__init__.py
 src/tiktok_captcha_solver/api.py
+src/tiktok_captcha_solver/asyncplaywrightsolver.py
+src/tiktok_captcha_solver/asyncsolver.py
 src/tiktok_captcha_solver/downloader.py
 src/tiktok_captcha_solver/models.py
 src/tiktok_captcha_solver/playwrightsolver.py
 src/tiktok_captcha_solver/seleniumsolver.py
 src/tiktok_captcha_solver/solver.py
 src/tiktok_captcha_solver.egg-info/PKG-INFO
 src/tiktok_captcha_solver.egg-info/SOURCES.txt
 src/tiktok_captcha_solver.egg-info/dependency_links.txt
 src/tiktok_captcha_solver.egg-info/requires.txt
 src/tiktok_captcha_solver.egg-info/top_level.txt
 src/tiktok_captcha_solver/tests/__init__.py
 src/tiktok_captcha_solver/tests/test_api.py
+src/tiktok_captcha_solver/tests/test_asyncplaywrightsolver.py
 src/tiktok_captcha_solver/tests/test_downloader.py
 src/tiktok_captcha_solver/tests/test_playwrightsolver.py
 src/tiktok_captcha_solver/tests/test_seleniumsolver.py
```

