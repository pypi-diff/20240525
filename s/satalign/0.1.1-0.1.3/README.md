# Comparing `tmp/satalign-0.1.1.tar.gz` & `tmp/satalign-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satalign-0.1.1.tar", max compression
+gzip compressed data, was "satalign-0.1.3.tar", max compression
```

## Comparing `satalign-0.1.1.tar` & `satalign-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satalign-0.1.1/LICENSE
--rw-r--r--   0        0        0     2506 2024-05-08 16:32:44.207454 satalign-0.1.1/README.md
--rw-r--r--   0        0        0     1999 2024-05-12 16:28:57.856068 satalign-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      114 2024-05-12 16:28:51.328251 satalign-0.1.1/satalign/__init__.py
--rw-r--r--   0        0        0     3008 2024-05-08 16:38:35.766819 satalign-0.1.1/satalign/ecc.py
--rw-r--r--   0        0        0     7614 2024-05-08 13:08:04.256526 satalign-0.1.1/satalign/lgm.py
--rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/__init__.py
--rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satalign-0.1.1/satalign/lightglue/aliked.py
--rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/disk.py
--rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/dog_hardnet.py
--rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satalign-0.1.1/satalign/lightglue/lightglue.py
--rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/sift.py
--rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/superpoint.py
--rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satalign-0.1.1/satalign/lightglue/utils.py
--rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satalign-0.1.1/satalign/lightglue/viz2d.py
--rw-r--r--   0        0        0    14351 2024-05-08 13:08:32.407756 satalign-0.1.1/satalign/main.py
--rw-r--r--   0        0        0     4114 2024-05-08 13:08:55.767118 satalign-0.1.1/satalign/pcc.py
--rw-r--r--   0        0        0    13642 2024-05-06 09:31:34.186154 satalign-0.1.1/satalign/utils.py
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 satalign-0.1.1/setup.py
--rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 satalign-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satalign-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2506 2024-05-08 16:32:44.207454 satalign-0.1.3/README.md
+-rw-r--r--   0        0        0     1999 2024-05-25 15:43:39.493461 satalign-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-05-25 15:34:39.264696 satalign-0.1.3/satalign/__init__.py
+-rw-r--r--   0        0        0     3047 2024-05-25 15:42:08.732018 satalign-0.1.3/satalign/ecc.py
+-rw-r--r--   0        0        0     7696 2024-05-25 15:41:07.697737 satalign-0.1.3/satalign/lgm.py
+-rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satalign-0.1.3/satalign/lightglue/__init__.py
+-rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satalign-0.1.3/satalign/lightglue/aliked.py
+-rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satalign-0.1.3/satalign/lightglue/disk.py
+-rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satalign-0.1.3/satalign/lightglue/dog_hardnet.py
+-rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satalign-0.1.3/satalign/lightglue/lightglue.py
+-rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satalign-0.1.3/satalign/lightglue/sift.py
+-rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satalign-0.1.3/satalign/lightglue/superpoint.py
+-rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satalign-0.1.3/satalign/lightglue/utils.py
+-rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satalign-0.1.3/satalign/lightglue/viz2d.py
+-rw-r--r--   0        0        0    15133 2024-05-25 15:43:00.478560 satalign-0.1.3/satalign/main.py
+-rw-r--r--   0        0        0     4153 2024-05-25 15:40:07.819425 satalign-0.1.3/satalign/pcc.py
+-rw-r--r--   0        0        0    13667 2024-05-25 15:34:39.180698 satalign-0.1.3/satalign/utils.py
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 satalign-0.1.3/setup.py
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 satalign-0.1.3/PKG-INFO
```

### Comparing `satalign-0.1.1/LICENSE` & `satalign-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/README.md` & `satalign-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/pyproject.toml` & `satalign-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "satalign"
-version = "0.1.1"
+version = "0.1.3"
 description = "Methods for spatial alignment of satellite imagery"
 authors = ["Cesar Aybar <cesar.aybar@uv.es>"]
 repository = "https://github.com/csaybar/satalign"
 documentation = "https://csaybar.github.io/satalign/"
 readme = "README.md"
 packages = [
   {include = "satalign"}
```

### Comparing `satalign-0.1.1/satalign/ecc.py` & `satalign-0.1.3/satalign/ecc.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,8 +77,9 @@
                 inputMask=None,
                 gaussFiltSize=self.gauss_kernel_size,
             )
 
         except cv2.error as cv2err:
             warnings.warn(f"Could not calculate the warp matrix: {cv2err}")
             warp_matrix = np.eye(*self.warp_matrix_size, dtype=np.float32)
+            self.warning_status = True
         return warp_matrix
```

### Comparing `satalign-0.1.1/satalign/lgm.py` & `satalign-0.1.3/satalign/lgm.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         )
 
         # Get the reference points from the moving image feature
         with torch.no_grad():
             feats0 = self.feature_model.extract(moving_image_torch, resize=None)
             if feats0["keypoints"].shape[1] == 0:
                 warnings.warn("No keypoints found in the moving image")
+                self.warning_status = True
                 return self.warp_matrix
 
         # Run the matcher model
         matches01 = self.matcher_model({"image0": feats0, "image1": feats1})
 
         # remove batch dimension
         feats0, feats1, matches01 = [rbd(x) for x in [feats0, feats1, matches01]]
@@ -105,14 +106,15 @@
         # if the distance between the points is higher than self.threshold_distance
         # it is considered a bad match
         dist = torch.sqrt(torch.sum((points0 - points1) ** 2, dim=1))
         thres = dist < self.max_translations
 
         if thres.sum().item() == 0:
             warnings.warn("No matching points found")
+            self.warning_status = True
             return self.warp_matrix
 
         p0 = points0[thres]
         p1 = points1[thres]
 
         # Get the warp matrix
         translation_x = p1[:, 0].mean() - p0[:, 0].mean()
```

### Comparing `satalign-0.1.1/satalign/lightglue/aliked.py` & `satalign-0.1.3/satalign/lightglue/aliked.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/satalign/lightglue/disk.py` & `satalign-0.1.3/satalign/lightglue/disk.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/satalign/lightglue/dog_hardnet.py` & `satalign-0.1.3/satalign/lightglue/dog_hardnet.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/satalign/lightglue/lightglue.py` & `satalign-0.1.3/satalign/lightglue/lightglue.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/satalign/lightglue/sift.py` & `satalign-0.1.3/satalign/lightglue/sift.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/satalign/lightglue/superpoint.py` & `satalign-0.1.3/satalign/lightglue/superpoint.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/satalign/lightglue/utils.py` & `satalign-0.1.3/satalign/lightglue/utils.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/satalign/lightglue/viz2d.py` & `satalign-0.1.3/satalign/lightglue/viz2d.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.1/satalign/main.py` & `satalign-0.1.3/satalign/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,30 +29,32 @@
         interpolation: int = cv2.INTER_LINEAR + cv2.WARP_FILL_OUTLIERS,
         crop_center: Optional[int] = None,
         rgb_bands: List[int] = [3, 2, 1],
         border_mode: int = cv2.BORDER_REPLICATE,
         num_threads: int = 4,
         max_translations: int = 5.0,
         border_value: int = 0,
+        warning_status: bool = False,
     ):
         """
 
         Args:
             datacube (xr.DataArray): The data cube to be aligned. The data cube
                 needs to have the following dimensions: (time, bands, height, width).
             reference (Optional[xr.DataArray], optional): The reference image.
                 The reference image needs to have the following dimensions:
                 (bands, height, width).
             channel (Union[int, str], optional): The channel or feature to be used for
                 alignment. Defaults to "gradients". The options are:
-                - "gradients": The gradients of the image. It uses the Sobel operator
-                    to calculate the gradients.
+                - "gradients": The gradients of the rgb channels of the image. 
+                    It uses the Sobel operator to calculate the gradients.
                 - "mean": The mean of all the bands.
-                - "luminance": The luminance of the image. It uses the following
+                - "luminance": The luminance of the rgb channels of the image. It uses the following
                     formula: 0.299 * R + 0.587 * G + 0.114 * B.
+                - "rgb_mean": The mean of the RGB bands.
                 - int: The index of the band to be used.
             interpolation (int, optional): Interpolation type used when transforming
                 the stack of images. Defaults to cv2.INTER_LINEAR + cv2.WARP_FILL_OUTLIERS.
             crop_center (Optional[int], optional): If this parameter is set, the
                 images will be cropped with respect to the center of the image to
                 calculate the warp matrix. The resulted warp matrix will be applied
                 to the original image size. This can be useful for large images
@@ -66,14 +68,19 @@
             num_threads (int, optional): Number of threads used to estimate the warp matrix.
                 Only used in run_multicore method. The only method that supports multiple
                 threads in a safe way is PCC. If ECC needs to be used, the cv2
                 package have to be compiled with the flag WITH_TBB. Defaults to 4.
             max_translations (int, optional): Estimated transformations are considered
                 incorrect when the norm of the translation component is larger than
                 this parameter. Defaults to 5.0.
+            border_value (int, optional): Value used to fill the border of the 
+                image when the warp matrix affects the border of the image. Defaults 
+                to 0.
+            warning_status (bool, optional): The warning status of the alignment
+                method. Defaults to False.
         """
 
         # Set the class attributes (REQUIRED)
         self.datacube = datacube
         self.reference = reference
 
         # Set the class attributes (OPTIONAL)
@@ -85,14 +92,15 @@
         self.num_threads = num_threads
         self.max_translations = max_translations
         self.border_value = border_value
 
         # We do no support homography for now (AUTOMATIC)
         self.warp_matrix_size = (2, 3)
         self.warp_matrix: np.ndarray = np.eye(*self.warp_matrix_size, dtype=np.float32)
+        self.warning_status = warning_status
 
     @abstractmethod
     def find_warp(
         self,
         reference_image: np.ndarray,
         moving_image: np.ndarray,
     ) -> np.ndarray:
@@ -160,43 +168,48 @@
         Returns:
             numpy.ndarray: The feature image
         """
 
         # If the image has more than 3 bands, select the RGB bands
         C, H, W = img.shape
 
-        if C > 3:
-            layer = img[self.rgb_bands]
-        else:
-            layer = img
-
         # Crop the image with respect to the centroid
         if self.crop_center is not None:
 
             if self.crop_center > H or self.crop_center > W:
                 raise ValueError("The crop_center should be less than the image size")
 
             radius_x = (img.shape[-1] - self.crop_center) // 2
             radius_y = (img.shape[-2] - self.crop_center) // 2
-            layer = layer[:, radius_y:-radius_y, radius_x:-radius_x]
+            img = img[:, radius_y:-radius_y, radius_x:-radius_x]
 
         # From RGB to grayscale (image feature)
         if isinstance(self.channel, str):
+            if C > 3:
+                layer = img[self.rgb_bands]
+            else:
+                layer = img
+            
             if self.channel == "gradients":
                 global_reference = cv2.Sobel(
                     layer.mean(0).astype(np.float32), cv2.CV_32F, 1, 1
                 )
             elif self.channel == "mean":
-                global_reference = layer.mean(0)
+                global_reference = img.mean(0)
             elif self.channel == "luminance":
                 global_reference = (
                     layer[0] * 0.299 + layer[1] * 0.587 + layer[2] * 0.114
                 )
+            elif self.channel == "rgb_mean":
+                global_reference = layer.mean(0)
+            else:
+                raise ValueError("The channel should be 'gradients', 'mean', 'luminance' or 'rgb_mean'")
+            
         elif isinstance(self.channel, int):
-            global_reference = layer[self.channel].copy()
+            global_reference = img[self.channel].copy()
         else:
             raise ValueError(
                 "The channel should be a string (a specific method) or an integer (a band index)"
             )
 
         return global_reference
 
@@ -222,14 +235,15 @@
             moving_image=self.create_layer(moving_image),
         )
 
         # Check if the translation is large
         if self.is_translation_large(warp_matrix):
             warnings.warn("Estimated translation is too large")
             warp_matrix = self.warp_matrix
+            self.warning_status = True
 
         # Warp the image using the estimated warp matrix
         warped_image = self.warp_feature(img=moving_image, warp_matrix=warp_matrix)
 
         return warped_image, warp_matrix
 
     def run_xarray(self) -> xr.Dataset:
```

### Comparing `satalign-0.1.1/satalign/pcc.py` & `satalign-0.1.3/satalign/pcc.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,9 +89,10 @@
             # Create the warp matrix with the shift
             warp_matrix = np.eye(*self.warp_matrix_size, dtype=np.float32)
             warp_matrix[:2, 2] = shift[::-1]
 
         except Exception as err:
             warnings.warn(f"Could not calculate the warp matrix: {err}")
             warp_matrix = np.eye(*self.warp_matrix_size, dtype=np.float32)
+            self.warning_status = True
 
         return warp_matrix
```

### Comparing `satalign-0.1.1/satalign/utils.py` & `satalign-0.1.3/satalign/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,16 +127,16 @@
 
     # x1, y1 are the points after the fix in spatial alignment
     # x2, y2 are the points before the fix in spatial alignment
     x1, y1 = warp_df[warp_df["after"]]["x"], warp_df[warp_df["after"]]["y"]
     x2, y2 = warp_df[~warp_df["after"]]["x"], warp_df[~warp_df["after"]]["y"]
     
     # Build the scatter plot
-    ax.scatter(x1, y1, label="After", color="blue", alpha=0.5)
-    ax.scatter(x2, y2, label="Before", color="red", alpha=0.5)
+    ax.scatter(x1, y1, label="After Cutoff date", color="blue", alpha=0.5)
+    ax.scatter(x2, y2, label="Before  Cutoff date", color="red", alpha=0.5)
     ax.legend()
 
     return fig, ax
 
 def plot_rgb(
     warped_cube: np.ndarray,
     raw_cube: np.ndarray,
```

### Comparing `satalign-0.1.1/setup.py` & `satalign-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'rasterio>=1.3.10',
  'scikit-image>=0.23.1',
  'torch>=2.0.0',
  'xarray>=2023.7.0']
 
 setup_kwargs = {
     'name': 'satalign',
-    'version': '0.1.1',
+    'version': '0.1.3',
     'description': 'Methods for spatial alignment of satellite imagery',
     'long_description': '# satalign\n\n[![Release](https://img.shields.io/github/v/release/csaybar/satalign)](https://img.shields.io/github/v/release/csaybar/satalign)\n[![Build status](https://img.shields.io/github/actions/workflow/status/csaybar/satalign/main.yml?branch=main)](https://github.com/csaybar/satalign/actions/workflows/main.yml?query=branch%3Amain)\n[![codecov](https://codecov.io/gh/csaybar/satalign/branch/main/graph/badge.svg)](https://codecov.io/gh/csaybar/satalign)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/csaybar/satalign)](https://img.shields.io/github/commit-activity/m/csaybar/satalign)\n[![License](https://img.shields.io/github/license/csaybar/satalign)](https://img.shields.io/github/license/csaybar/satalign)\n\nA python package to align satellite images.\n\n- **Github repository**: <https://github.com/csaybar/satalign/>\n- **Documentation** <https://csaybar.github.io/satalign/>\n\n## Getting started with your project\n\nFirst, create a repository on GitHub with the same name as this project, and then run the following commands:\n\n```bash\ngit init -b main\ngit add .\ngit commit -m "init commit"\ngit remote add origin git@github.com:csaybar/satalign.git\ngit push -u origin main\n```\n\nFinally, install the environment and the pre-commit hooks with\n\n```bash\nmake install\n```\n\nYou are now ready to start development on your project!\nThe CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.\n\nTo finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).\nFor activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).\nTo enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).\n\n## Releasing a new version\n\n- Create an API Token on [Pypi](https://pypi.org/).\n- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/csaybar/satalign/settings/secrets/actions/new).\n- Create a [new release](https://github.com/csaybar/satalign/releases/new) on Github.\n- Create a new tag in the form `*.*.*`.\n\nFor more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).\n\n---\n\nRepository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).\n',
     'author': 'Cesar Aybar',
     'author_email': 'cesar.aybar@uv.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csaybar/satalign',
```

### Comparing `satalign-0.1.1/PKG-INFO` & `satalign-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satalign
-Version: 0.1.1
+Version: 0.1.3
 Summary: Methods for spatial alignment of satellite imagery
 Home-page: https://github.com/csaybar/satalign
 Author: Cesar Aybar
 Author-email: cesar.aybar@uv.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

