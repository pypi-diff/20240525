# Comparing `tmp/sopa-1.0.8.tar.gz` & `tmp/sopa-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopa-1.0.8.tar", max compression
+gzip compressed data, was "sopa-1.0.9.tar", max compression
```

## Comparing `sopa-1.0.8.tar` & `sopa-1.0.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1523 2024-04-02 21:44:23.275434 sopa-1.0.8/LICENSE
--rw-r--r--   0        0        0     5407 2024-04-02 21:44:23.275434 sopa-1.0.8/README.md
--rw-r--r--   0        0        0     2749 2024-04-02 21:44:23.303434 sopa-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      185 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/__init__.py
--rw-r--r--   0        0        0     1258 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/_constants.py
--rw-r--r--   0        0        0     1075 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/_logging.py
--rw-r--r--   0        0        0     7259 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/_sdata.py
--rw-r--r--   0        0        0       58 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/annotation/__init__.py
--rw-r--r--   0        0        0     1683 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/annotation/fluorescence.py
--rw-r--r--   0        0        0       34 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/annotation/tangram/__init__.py
--rw-r--r--   0        0        0     9736 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/annotation/tangram/run.py
--rw-r--r--   0        0        0     2640 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/annotate.py
--rw-r--r--   0        0        0     7640 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/app.py
--rw-r--r--   0        0        0     4436 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/check.py
--rw-r--r--   0        0        0     4833 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/explorer.py
--rw-r--r--   0        0        0     3926 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/patchify.py
--rw-r--r--   0        0        0     3572 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/resolve.py
--rw-r--r--   0        0        0     6812 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/segmentation.py
--rw-r--r--   0        0        0      562 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/utils.py
--rw-r--r--   0        0        0       79 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/cluster.py
--rw-r--r--   0        0        0      182 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/models/__init__.py
--rw-r--r--   0        0        0      374 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/models/dinov2.py
--rw-r--r--   0        0        0      496 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/models/histo_ssl.py
--rw-r--r--   0        0        0      876 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/models/resnet.py
--rw-r--r--   0        0        0     8381 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/patches.py
--rw-r--r--   0        0        0      314 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/__init__.py
--rw-r--r--   0        0        0      278 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/__init__.py
--rw-r--r--   0        0        0     3919 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/_constants.py
--rw-r--r--   0        0        0     7882 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/converter.py
--rw-r--r--   0        0        0     8851 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/images.py
--rw-r--r--   0        0        0     7213 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/points.py
--rw-r--r--   0        0        0     3779 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/shapes.py
--rw-r--r--   0        0        0     5112 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/table.py
--rw-r--r--   0        0        0      906 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/utils.py
--rw-r--r--   0        0        0     3972 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/histopathology.py
--rw-r--r--   0        0        0    10199 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/imaging.py
--rw-r--r--   0        0        0       35 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/report/__init__.py
--rw-r--r--   0        0        0   207321 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/report/css.py
--rw-r--r--   0        0        0     8116 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/io/report/engine.py
--rw-r--r--   0        0        0     6735 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/io/report/generate.py
--rw-r--r--   0        0        0     2987 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/io/standardize.py
--rw-r--r--   0        0        0     9291 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/io/transcriptomics.py
--rw-r--r--   0        0        0       25 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/main.py
--rw-r--r--   0        0        0      187 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/__init__.py
--rw-r--r--   0        0        0    12678 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/aggregate.py
--rw-r--r--   0        0        0        0 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/baysor/__init__.py
--rw-r--r--   0        0        0      549 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/baysor/prepare.py
--rw-r--r--   0        0        0     6615 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/baysor/resolve.py
--rw-r--r--   0        0        0     2518 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/methods.py
--rw-r--r--   0        0        0    13418 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/patching.py
--rw-r--r--   0        0        0     6795 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/shapes.py
--rw-r--r--   0        0        0     7390 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/stainings.py
--rw-r--r--   0        0        0     4590 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/tissue.py
--rw-r--r--   0        0        0      194 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/__init__.py
--rw-r--r--   0        0        0     4840 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/_build.py
--rw-r--r--   0        0        0     4154 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/_graph.py
--rw-r--r--   0        0        0     5628 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/distance.py
--rw-r--r--   0        0        0     6409 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/morpho.py
--rw-r--r--   0        0        0     1933 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/utils.py
--rw-r--r--   0        0        0        0 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/utils/__init__.py
--rw-r--r--   0        0        0     7128 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/utils/data.py
--rw-r--r--   0        0        0     2346 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/utils/image.py
--rw-r--r--   0        0        0     5109 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/utils/polygon_crop.py
--rw-r--r--   0        0        0     7737 1970-01-01 00:00:00.000000 sopa-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1523 2024-04-03 09:16:27.985777 sopa-1.0.9/LICENSE
+-rw-r--r--   0        0        0     5407 2024-04-03 09:16:27.985777 sopa-1.0.9/README.md
+-rw-r--r--   0        0        0     2749 2024-04-03 09:16:28.013777 sopa-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/__init__.py
+-rw-r--r--   0        0        0     1278 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/_constants.py
+-rw-r--r--   0        0        0     1075 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/_logging.py
+-rw-r--r--   0        0        0     7482 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/_sdata.py
+-rw-r--r--   0        0        0       58 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/annotation/__init__.py
+-rw-r--r--   0        0        0     1683 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/annotation/fluorescence.py
+-rw-r--r--   0        0        0       34 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/annotation/tangram/__init__.py
+-rw-r--r--   0        0        0     9844 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/annotation/tangram/run.py
+-rw-r--r--   0        0        0     2706 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/cli/annotate.py
+-rw-r--r--   0        0        0     7640 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/cli/app.py
+-rw-r--r--   0        0        0     4436 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/cli/check.py
+-rw-r--r--   0        0        0     4833 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/cli/explorer.py
+-rw-r--r--   0        0        0     3926 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/cli/patchify.py
+-rw-r--r--   0        0        0     3572 2024-04-03 09:16:28.013777 sopa-1.0.9/sopa/cli/resolve.py
+-rw-r--r--   0        0        0     6812 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/cli/segmentation.py
+-rw-r--r--   0        0        0      562 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/cli/utils.py
+-rw-r--r--   0        0        0       79 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/embedding/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/embedding/cluster.py
+-rw-r--r--   0        0        0      182 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/embedding/models/__init__.py
+-rw-r--r--   0        0        0      374 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/embedding/models/dinov2.py
+-rw-r--r--   0        0        0      496 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/embedding/models/histo_ssl.py
+-rw-r--r--   0        0        0      876 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/embedding/models/resnet.py
+-rw-r--r--   0        0        0     8381 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/embedding/patches.py
+-rw-r--r--   0        0        0      314 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/__init__.py
+-rw-r--r--   0        0        0      278 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/explorer/__init__.py
+-rw-r--r--   0        0        0     3919 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/explorer/_constants.py
+-rw-r--r--   0        0        0     8022 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/explorer/converter.py
+-rw-r--r--   0        0        0     8851 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/explorer/images.py
+-rw-r--r--   0        0        0     7213 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/explorer/points.py
+-rw-r--r--   0        0        0     3779 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/explorer/shapes.py
+-rw-r--r--   0        0        0     5112 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/explorer/table.py
+-rw-r--r--   0        0        0      906 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/explorer/utils.py
+-rw-r--r--   0        0        0     3972 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/histopathology.py
+-rw-r--r--   0        0        0    10199 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/imaging.py
+-rw-r--r--   0        0        0       35 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/report/__init__.py
+-rw-r--r--   0        0        0   207321 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/report/css.py
+-rw-r--r--   0        0        0     8116 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/report/engine.py
+-rw-r--r--   0        0        0     6763 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/report/generate.py
+-rw-r--r--   0        0        0     3073 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/standardize.py
+-rw-r--r--   0        0        0     9291 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/io/transcriptomics.py
+-rw-r--r--   0        0        0       25 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/main.py
+-rw-r--r--   0        0        0      187 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/__init__.py
+-rw-r--r--   0        0        0    12616 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/aggregate.py
+-rw-r--r--   0        0        0        0 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/baysor/__init__.py
+-rw-r--r--   0        0        0      549 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/baysor/prepare.py
+-rw-r--r--   0        0        0     6566 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/baysor/resolve.py
+-rw-r--r--   0        0        0     2518 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/methods.py
+-rw-r--r--   0        0        0    13418 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/patching.py
+-rw-r--r--   0        0        0     6795 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/shapes.py
+-rw-r--r--   0        0        0     7390 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/stainings.py
+-rw-r--r--   0        0        0     4590 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/segmentation/tissue.py
+-rw-r--r--   0        0        0      194 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/spatial/__init__.py
+-rw-r--r--   0        0        0     4892 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/spatial/_build.py
+-rw-r--r--   0        0        0     4154 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/spatial/_graph.py
+-rw-r--r--   0        0        0     5696 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/spatial/distance.py
+-rw-r--r--   0        0        0     6443 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/spatial/morpho.py
+-rw-r--r--   0        0        0     1933 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/spatial/utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/utils/__init__.py
+-rw-r--r--   0        0        0     7128 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/utils/data.py
+-rw-r--r--   0        0        0     2346 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/utils/image.py
+-rw-r--r--   0        0        0     5109 2024-04-03 09:16:28.017777 sopa-1.0.9/sopa/utils/polygon_crop.py
+-rw-r--r--   0        0        0     7737 1970-01-01 00:00:00.000000 sopa-1.0.9/PKG-INFO
```

### Comparing `sopa-1.0.8/LICENSE` & `sopa-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/README.md` & `sopa-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/pyproject.toml` & `sopa-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sopa"
-version = "1.0.8"
+version = "1.0.9"
 description = "Spatial-omics pipeline and analysis"
 documentation = "https://gustaveroussy.github.io/sopa"
 homepage = "https://gustaveroussy.github.io/sopa"
 repository = "https://github.com/gustaveroussy/sopa"
 authors = ["Quentin Blampey <quentin.blampey@gmail.com>"]
 packages = [{ include = "sopa" }]
 license = "BSD-3-Clause"
```

### Comparing `sopa-1.0.8/sopa/_constants.py` & `sopa-1.0.9/sopa/_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 class SopaKeys:
     CELLPOSE_BOUNDARIES = "cellpose_boundaries"
     BAYSOR_BOUNDARIES = "baysor_boundaries"
     PATCHES = "sopa_patches"
+    TABLE = "table"
 
     BOUNDS = "bboxes"
     PATCHES_ILOCS = "ilocs"
     EMBEDDINGS_PATCHES_KEY = "sopa_embedding_patches"
 
     UNS_KEY = "sopa_attrs"
     UNS_HAS_TRANSCRIPTS = "transcripts"
```

### Comparing `sopa-1.0.8/sopa/_logging.py` & `sopa-1.0.9/sopa/_logging.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/_sdata.py` & `sopa-1.0.9/sopa/_sdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,21 +126,25 @@
 def get_item(sdata: SpatialData, attr: str, key: str | None = None):
     key = get_key(sdata, attr, key)
     return key, sdata[key] if key is not None else None
 
 
 def get_intensities(sdata: SpatialData) -> pd.DataFrame | None:
     """Gets the intensity dataframe of shape `n_obs x n_channels`"""
-    if not sdata.table.uns[SopaKeys.UNS_KEY][SopaKeys.UNS_HAS_INTENSITIES]:
+    assert SopaKeys.TABLE in sdata.tables, f"No '{SopaKeys.TABLE}' found in sdata.tables"
+
+    adata = sdata.tables[SopaKeys.TABLE]
+
+    if not adata.uns[SopaKeys.UNS_KEY][SopaKeys.UNS_HAS_INTENSITIES]:
         return None
 
-    if sdata.table.uns[SopaKeys.UNS_KEY][SopaKeys.UNS_HAS_TRANSCRIPTS]:
-        return sdata.table.obsm[SopaKeys.INTENSITIES_OBSM]
+    if adata.uns[SopaKeys.UNS_KEY][SopaKeys.UNS_HAS_TRANSCRIPTS]:
+        return adata.obsm[SopaKeys.INTENSITIES_OBSM]
 
-    return sdata.table.to_df()
+    return adata.to_df()
 
 
 def iter_scales(image: MultiscaleSpatialImage) -> Iterator[xr.DataArray]:
     """Iterates through all the scales of a `MultiscaleSpatialImage`
 
     Args:
         image: a `MultiscaleSpatialImage`
@@ -183,41 +187,50 @@
 
 
 def save_shapes(
     sdata: SpatialData,
     name: str,
     overwrite: bool = False,
 ) -> None:
+    if not sdata.is_backed():
+        return
+
     elem_group = sdata._init_add_element(name=name, element_type="shapes", overwrite=overwrite)
     write_shapes(
         shapes=sdata.shapes[name],
         group=elem_group,
         name=name,
     )
 
 
 def save_image(
     sdata: SpatialData,
     name: str,
     overwrite: bool = False,
 ) -> None:
+    if not sdata.is_backed():
+        return
+
     elem_group = sdata._init_add_element(name=name, element_type="images", overwrite=overwrite)
     write_image(
         image=sdata.images[name],
         group=elem_group,
         name=name,
     )
     from spatialdata._io.io_raster import _read_multiscale
 
     # reload the image from the Zarr storage so that now the element is lazy loaded, and most importantly,
     # from the correct storage
     assert elem_group.path == "images"
     path = Path(elem_group.store.path) / "images" / name
     image = _read_multiscale(path, raster_type="image")
-    sdata._add_image_in_memory(name=name, image=image, overwrite=True)
+    sdata.images[name] = image
+
 
+def save_table(sdata: SpatialData, name: str):
+    if not sdata.is_backed():
+        return
 
-def save_table(sdata: SpatialData):
     store = parse_url(sdata.path, mode="r+").store
     root = zarr.group(store=store)
-    elem_group = root.require_group(name="table")
-    write_table(table=sdata.table, group=elem_group, name="table")
+    elem_group = root.require_group(name="tables")
+    write_table(table=sdata.tables[name], group=elem_group, name=name)
```

### Comparing `sopa-1.0.8/sopa/annotation/fluorescence.py` & `sopa-1.0.9/sopa/annotation/fluorescence.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/annotation/tangram/run.py` & `sopa-1.0.9/sopa/annotation/tangram/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
         sdata: A `SpatialData` object
         adata_sc: A scRNAseq annotated reference
         cell_type_key: Key of `adata_sc.obs` containing the cell types. For multi-level annotation, provide other levels like such: if `cell_type_key = "ct"`, then `"ct_level1"` and `"ct_level2"` are the two next levels
         reference_preprocessing: Preprocessing method used on the reference. Can be `"log1p"` (normalize_total + log1p) or `"normalized"` (just normalize_total). By default, consider that no processing was applied (raw counts)
         bag_size: Size of each bag on which tangram will be run. Use smaller bags to lower the RAM usage
         max_obs_reference: Maximum number of cells used in `adata_sc` at each level. Decrease it to lower the RAM usage.
     """
-    ad_sp = sdata.table
+    assert SopaKeys.TABLE in sdata.tables, f"No '{SopaKeys.TABLE}' found in sdata.tables"
+
+    ad_sp = sdata.tables[SopaKeys.TABLE]
 
     MultiLevelAnnotation(
         ad_sp,
         adata_sc,
         cell_type_key,
         reference_preprocessing,
         bag_size,
```

### Comparing `sopa-1.0.8/sopa/cli/annotate.py` & `sopa-1.0.9/sopa/cli/annotate.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,25 +17,25 @@
         "cell_type", help="Key added in `adata.obs` corresponding to the cell type"
     ),
 ):
     """Simple annotation based on fluorescence, where each provided channel corresponds to one cell type.
 
     For each cell, one z-score statistic is computed and the population with the highest z-score is attributed.
     """
-    from pathlib import Path
-
+    from sopa._constants import SopaKeys
+    from sopa._sdata import save_table
     from sopa.annotation.fluorescence import higher_z_score
     from sopa.io.standardize import read_zarr_standardized
 
     sdata = read_zarr_standardized(sdata_path)
 
-    assert sdata.table is not None, "Annotation requires `sdata.table` to be not None"
+    assert SopaKeys.TABLE in sdata.tables, f"No '{SopaKeys.TABLE}' found in sdata.tables"
 
-    higher_z_score(sdata.table, marker_cell_dict, cell_type_key)
-    sdata.table.write_zarr(Path(sdata_path) / "table" / "table")
+    higher_z_score(sdata.tables[SopaKeys.TABLE], marker_cell_dict, cell_type_key)
+    save_table(sdata, SopaKeys.TABLE)
 
 
 @app_annotate.command()
 def tangram(
     sdata_path: str = typer.Argument(help=SDATA_HELPER),
     sc_reference_path: str = typer.Option(
         help="Path to the scRNAseq annotated reference, as a `.h5ad` file"
@@ -51,26 +51,26 @@
     ),
     max_obs_reference: int = typer.Option(
         10_000,
         help="Maximum samples to be considered in the reference for tangram. Low values will decrease the memory usage",
     ),
 ):
     """Tangram segmentation (i.e., uses an annotated scRNAseq reference to transfer cell-types)"""
-    from pathlib import Path
-
     import anndata
 
+    from sopa._constants import SopaKeys
+    from sopa._sdata import save_table
     from sopa.annotation.tangram.run import tangram_annotate
     from sopa.io.standardize import read_zarr_standardized
 
     sdata = read_zarr_standardized(sdata_path)
     adata_sc = anndata.read_h5ad(sc_reference_path)
 
     tangram_annotate(
         sdata,
         adata_sc,
         cell_type_key,
         reference_preprocessing=reference_preprocessing,
         bag_size=bag_size,
         max_obs_reference=max_obs_reference,
     )
-    sdata.table.write_zarr(Path(sdata_path) / "table" / "table")
+    save_table(sdata, SopaKeys.TABLE)
```

### Comparing `sopa-1.0.8/sopa/cli/app.py` & `sopa-1.0.9/sopa/cli/app.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/cli/check.py` & `sopa-1.0.9/sopa/cli/check.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/cli/explorer.py` & `sopa-1.0.9/sopa/cli/explorer.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/cli/patchify.py` & `sopa-1.0.9/sopa/cli/patchify.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/cli/resolve.py` & `sopa-1.0.9/sopa/cli/resolve.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/cli/segmentation.py` & `sopa-1.0.9/sopa/cli/segmentation.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/cli/utils.py` & `sopa-1.0.9/sopa/cli/utils.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/embedding/cluster.py` & `sopa-1.0.9/sopa/embedding/cluster.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/embedding/models/resnet.py` & `sopa-1.0.9/sopa/embedding/models/resnet.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/embedding/patches.py` & `sopa-1.0.9/sopa/embedding/patches.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/explorer/_constants.py` & `sopa-1.0.9/sopa/io/explorer/_constants.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/explorer/converter.py` & `sopa-1.0.9/sopa/io/explorer/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import logging
 from pathlib import Path
 
 import geopandas as gpd
 from spatialdata import SpatialData
 
+from ..._constants import SopaKeys
 from ..._sdata import get_boundaries, get_element, get_spatial_image, to_intrinsic
 from . import (
     write_cell_categories,
     write_gene_counts,
     write_image,
     write_polygons,
     write_transcripts,
@@ -83,29 +84,29 @@
         path: Path to the directory where files will be saved.
         sdata: SpatialData object.
         image_key: Name of the image of interest (key of `sdata.images`).
         shapes_key: Name of the cell shapes (key of `sdata.shapes`).
         points_key: Name of the transcripts (key of `sdata.points`).
         gene_column: Column name of the points dataframe containing the gene names.
         pixel_size: Number of microns in a pixel. Invalid value can lead to inconsistent scales in the Explorer.
-        layer: Layer of `sdata.table` where the gene counts are saved. If `None`, uses `sdata.table.X`.
+        layer: Layer of the AnnData table where the gene counts are saved. If `None`, uses `table.X`.
         polygon_max_vertices: Maximum number of vertices for the cell polygons.
         lazy: If `True`, will not load the full images in memory (except if the image memory is below `ram_threshold_gb`).
         ram_threshold_gb: Threshold (in gygabytes) from which image can be loaded in memory. If `None`, the image is never loaded in memory.
         mode: string that indicated which files should be created. "-ib" means everything except images and boundaries, while "+tocm" means only transcripts/observations/counts/metadata (each letter corresponds to one explorer file). By default, keeps everything.
         save_h5ad: Whether to save the adata as h5ad in the explorer directory (for convenience only, since h5ad is faster to open than the original .zarr table)
     """
     path: Path = Path(path)
     _check_explorer_directory(path)
 
     image_key, image = get_spatial_image(sdata, image_key, return_key=True)
 
     ### Saving cell categories and gene counts
-    if sdata.table is not None:
-        adata = sdata.table
+    if SopaKeys.TABLE in sdata.tables:
+        adata = sdata.tables[SopaKeys.TABLE]
 
         shapes_key = adata.uns["spatialdata_attrs"]["region"]
         geo_df = sdata[shapes_key]
 
         if _should_save(mode, "c"):
             write_gene_counts(path, adata, layer=layer)
         if _should_save(mode, "o"):
@@ -116,15 +117,15 @@
         shapes_key, geo_df = get_boundaries(sdata, return_key=True, warn=True)
     else:
         geo_df = sdata[shapes_key]
 
     if _should_save(mode, "b") and geo_df is not None:
         geo_df = to_intrinsic(sdata, geo_df, image_key)
 
-        if sdata.table is not None:
+        if SopaKeys.TABLE in sdata.tables:
             geo_df = geo_df.loc[adata.obs[adata.uns["spatialdata_attrs"]["instance_key"]]]
 
         write_polygons(path, geo_df.geometry, polygon_max_vertices, pixel_size=pixel_size)
 
     ### Saving transcripts
     df = get_element(sdata, "points", points_key)
 
@@ -141,24 +142,24 @@
             path, image, lazy=lazy, ram_threshold_gb=ram_threshold_gb, pixel_size=pixel_size
         )
 
     ### Saving experiment.xenium file
     if _should_save(mode, "m"):
         write_metadata(path, image_key, shapes_key, _get_n_obs(sdata, geo_df), pixel_size)
 
-    if save_h5ad:
-        sdata.table.write_h5ad(path / FileNames.H5AD)
+    if save_h5ad and SopaKeys.TABLE in sdata.tables:
+        sdata.tables[SopaKeys.TABLE].write_h5ad(path / FileNames.H5AD)
 
     log.info(f"Saved files in the following directory: {path}")
     log.info(f"You can open the experiment with 'open {path / FileNames.METADATA}'")
 
 
 def _get_n_obs(sdata: SpatialData, geo_df: gpd.GeoDataFrame) -> int:
-    if sdata.table is not None:
-        return sdata.table.n_obs
+    if SopaKeys.TABLE in sdata.tables:
+        return sdata.tables[SopaKeys.TABLE].n_obs
     return len(geo_df) if geo_df is not None else 0
 
 
 def write_metadata(
     path: str,
     image_key: str = "NA",
     shapes_key: str = "NA",
```

### Comparing `sopa-1.0.8/sopa/io/explorer/images.py` & `sopa-1.0.9/sopa/io/explorer/images.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/explorer/points.py` & `sopa-1.0.9/sopa/io/explorer/points.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/explorer/shapes.py` & `sopa-1.0.9/sopa/io/explorer/shapes.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/explorer/table.py` & `sopa-1.0.9/sopa/io/explorer/table.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/explorer/utils.py` & `sopa-1.0.9/sopa/io/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/histopathology.py` & `sopa-1.0.9/sopa/io/histopathology.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/imaging.py` & `sopa-1.0.9/sopa/io/imaging.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/report/css.py` & `sopa-1.0.9/sopa/io/report/css.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/report/engine.py` & `sopa-1.0.9/sopa/io/report/engine.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/io/report/generate.py` & `sopa-1.0.9/sopa/io/report/generate.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,19 +52,20 @@
     sns.kdeplot(values)
     plt.xlim(0, threshold)
 
 
 class SectionBuilder:
     def __init__(self, sdata: SpatialData):
         self.sdata = sdata
+        self.adata = self.sdata.tables.get(SopaKeys.TABLE)
 
     def _table_has(self, key, default=False):
-        if SopaKeys.UNS_KEY not in self.sdata.table.uns:
+        if SopaKeys.UNS_KEY not in self.adata.uns:
             return default
-        return self.sdata.table.uns[SopaKeys.UNS_KEY].get(key, default)
+        return self.adata.uns[SopaKeys.UNS_KEY].get(key, default)
 
     def general_section(self):
         log.info("Writing general section")
 
         return Section(
             "General",
             [
@@ -83,23 +84,23 @@
     def cell_section(self):
         log.info("Writing cell section")
 
         shapes_key, _ = get_boundaries(self.sdata, return_key=True)
         coord_system = get_intrinsic_cs(self.sdata, shapes_key)
 
         fig = plt.figure()
-        _kdeplot_vmax_quantile(self.sdata.table.obs[SopaKeys.AREA_OBS])
+        _kdeplot_vmax_quantile(self.adata.obs[SopaKeys.AREA_OBS])
         plt.xlabel("Area (coordinate_system_unit ^ 2)")
 
         return Section(
             "Cells",
             [
                 SubSection(
                     "Number",
-                    Paragraph(f"Number of cells:<br>{Message(f'{self.sdata.table.n_obs} cells')}"),
+                    Paragraph(f"Number of cells:<br>{Message(f'{self.adata.n_obs} cells')}"),
                 ),
                 SubSection(
                     "Areas",
                     [
                         Paragraph(
                             f"The cells areas are obtained based on the coordinate system '{coord_system}' for the '{shapes_key}' boundaries"
                         ),
@@ -151,60 +152,58 @@
 
     def transcripts_section(self):
         if not self._table_has(SopaKeys.UNS_HAS_TRANSCRIPTS):
             return None
 
         log.info("Writing transcript section")
 
-        mean_transcript_count = self.sdata.table.X.mean(0).A1
+        mean_transcript_count = self.adata.X.mean(0).A1
         low_average = mean_transcript_count < LOW_AVERAGE_COUNT
 
         QC_subsubsections = []
         if low_average.sum():
             QC_subsubsections.append(
                 Paragraph(
                     f"{low_average.sum()} genes have a low count (less than {LOW_AVERAGE_COUNT} per cell, on average):"
                 )
             )
             QC_subsubsections.append(
-                Message(", ".join(self.sdata.table.var_names[low_average]), color="danger")
+                Message(", ".join(self.adata.var_names[low_average]), color="danger")
             )
 
         fig1 = plt.figure()
         _kdeplot_vmax_quantile(mean_transcript_count)
         plt.xlabel("Count per transcript (average / cells)")
 
         fig2 = plt.figure()
-        _kdeplot_vmax_quantile(self.sdata.table.X.sum(1).A1)
+        _kdeplot_vmax_quantile(self.adata.X.sum(1).A1)
         plt.xlabel("Transcript count per cell")
 
         QC_subsubsections.append(Columns([Image(fig1), Image(fig2)]))
 
         return Section("Transcripts", [SubSection("Quality controls", QC_subsubsections)])
 
     def representation_section(self, max_obs: int = 400_000):
         log.info("Writing representation section")
 
-        adata = self.sdata.table
-
         if self._table_has(SopaKeys.UNS_HAS_TRANSCRIPTS):
-            sc.pp.normalize_total(adata)
-            sc.pp.log1p(adata)
+            sc.pp.normalize_total(self.adata)
+            sc.pp.log1p(self.adata)
 
-        if adata.n_obs > max_obs:
-            sc.pp.subsample(adata, n_obs=max_obs)
+        if self.adata.n_obs > max_obs:
+            sc.pp.subsample(self.adata, n_obs=max_obs)
 
-        log.info(f"Computing UMAP on {adata.n_obs} cells")
+        log.info(f"Computing UMAP on {self.adata.n_obs} cells")
 
-        sc.pp.pca(adata)
-        sc.pp.neighbors(adata)
-        sc.tl.umap(adata)
+        sc.pp.pca(self.adata)
+        sc.pp.neighbors(self.adata)
+        sc.tl.umap(self.adata)
 
         colors = self._table_has(SopaKeys.UNS_CELL_TYPES, None)
-        sc.pl.umap(adata, color=colors, show=False)
+        sc.pl.umap(self.adata, color=colors, show=False)
 
         return Section(
             "Representation",
             [
                 SubSection("UMAP", Columns([Image(plt.gcf(), pretty_legend=False)])),
             ],
         )
```

### Comparing `sopa-1.0.8/sopa/io/standardize.py` & `sopa-1.0.9/sopa/io/standardize.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from pathlib import Path
 
 import spatialdata
 from spatialdata import SpatialData
 
-from .._constants import VALID_DIMENSIONS
+from .._constants import VALID_DIMENSIONS, SopaKeys
 from .._sdata import get_spatial_image
 from ..utils.image import _check_integer_dtype
 
 log = logging.getLogger(__name__)
 
 
 def sanity_check(sdata: SpatialData, delete_table: bool = False, warn: bool = False):
@@ -38,20 +38,20 @@
 
     # TODO: see https://github.com/scverse/spatialdata/issues/402
     # image_channels: np.ndarray = image.coords["c"].values
     # if image_channels.dtype.type is not np.str_:
     #     log.warn(f"Channel names are not strings. Converting {image_channels} to string values.")
     #     sdata[image_key].data = sdata[image_key].assign_coords(c=image_channels.astype(str))
 
-    if sdata.table is not None:
+    if SopaKeys.TABLE in sdata.tables:
         if delete_table:
             log.info(
-                "The table (i.e. `sdata.table`) will not be saved, since it will be created later by sopa"
+                f"The table `sdata.tables['{SopaKeys.TABLE}']` will not be saved, since it will be created later by sopa"
             )
-            del sdata.table
+            del sdata.tables[SopaKeys.TABLE]
 
 
 def read_zarr_standardized(path: str, warn: bool = False) -> SpatialData:
     sdata = spatialdata.read_zarr(path)
     sanity_check(sdata, warn=warn)
     return sdata
 
@@ -69,16 +69,16 @@
     sdata_path.rmdir()
 
 
 def write_standardized(sdata: SpatialData, sdata_path: str, delete_table: bool = False):
     sanity_check(sdata, delete_table)
 
     assert (
-        sdata.table is None
-    ), "sdata.table exists. Delete it you want to use sopa, to avoid conflicts with future table generation"
+        SopaKeys.TABLE not in sdata.tables
+    ), f"sdata.tables['{SopaKeys.TABLE}'] exists. Delete it you want to use sopa, to avoid conflicts with future table generation"
 
     if len(sdata.points) == 0:
         log.warn("No transcripts found. Some tools from sopa will not be available.")
 
     log.info(f"Writing the following spatialdata object to {sdata_path}:\n{sdata}")
 
     sdata_path: Path = Path(sdata_path)
```

### Comparing `sopa-1.0.8/sopa/io/transcriptomics.py` & `sopa-1.0.9/sopa/io/transcriptomics.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/segmentation/aggregate.py` & `sopa-1.0.9/sopa/segmentation/aggregate.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,21 +59,21 @@
 
         if shapes_key is None:
             self.shapes_key, self.geo_df = get_boundaries(sdata, return_key=True)
         else:
             self.shapes_key = shapes_key
             self.geo_df = self.sdata[shapes_key]
 
-        if sdata.table is not None and len(self.geo_df) != sdata.table.n_obs:
-            log.warn(
-                f"Table already existing with {sdata.table.n_obs} obs, but aggregating on {len(self.geo_df)} cells. Deleting table."
-            )
-            del sdata.table
-
-        self.table = sdata.table
+        self.table = None
+        if SopaKeys.TABLE in sdata.tables:
+            table = sdata.tables[SopaKeys.TABLE]
+            if len(self.geo_df) != table.n_obs:
+                log.warn("Not using existing table (aggregating on a different number of cells)")
+            else:
+                self.table = table
 
     def standardize_table(self):
         self.table.obs_names = list(map(str_cell_id, range(self.table.n_obs)))
 
         self.geo_df.index = list(self.table.obs_names)
         self.sdata.shapes[self.shapes_key] = self.geo_df
         save_shapes(self.sdata, self.shapes_key, overwrite=True)
@@ -97,18 +97,16 @@
         self.table = TableModel.parse(
             self.table,
             region_key=SopaKeys.REGION_KEY,
             region=self.shapes_key,
             instance_key=SopaKeys.INSTANCE_KEY,
         )
 
-        if self.sdata.table is not None and self.overwrite:
-            del self.sdata.table
-        self.sdata.tables["table"] = self.table
-        save_table(self.sdata)
+        self.sdata.tables[SopaKeys.TABLE] = self.table
+        save_table(self.sdata, SopaKeys.TABLE)
 
     def filter_cells(self, where_filter: np.ndarray):
         log.info(f"Filtering {where_filter.sum()} cells")
 
         self.geo_df = self.geo_df[~where_filter]
 
         if self.table is not None:
```

### Comparing `sopa-1.0.8/sopa/segmentation/baysor/prepare.py` & `sopa-1.0.9/sopa/segmentation/baysor/prepare.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/segmentation/baysor/resolve.py` & `sopa-1.0.9/sopa/segmentation/baysor/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from shapely.geometry import Polygon, shape
 from spatialdata import SpatialData
 from spatialdata.models import ShapesModel, TableModel
 from spatialdata.transformations import get_transformation
 from tqdm import tqdm
 
 from ..._constants import SopaKeys
-from ..._sdata import get_element, get_key, save_shapes
+from ..._sdata import get_element, get_key, save_shapes, save_table
 from .. import aggregate, shapes
 
 log = logging.getLogger(__name__)
 
 
 def read_baysor(
     directory: str, min_area: float = 0, min_vertices: int = 4
@@ -170,16 +170,13 @@
         region=SopaKeys.BAYSOR_BOUNDARIES,
         instance_key=SopaKeys.INSTANCE_KEY,
     )
 
     sdata.shapes[SopaKeys.BAYSOR_BOUNDARIES] = geo_df
     save_shapes(sdata, SopaKeys.BAYSOR_BOUNDARIES, overwrite=True)
 
-    if sdata.table is not None:
-        log.warn("Table already existing. It will be replaced by the new one.")
-        del sdata.table
-
-    sdata.table = table
+    sdata.tables[SopaKeys.TABLE] = table
+    save_table(sdata, SopaKeys.TABLE)
 
     log.info(
-        f"Added sdata.table, and {len(geo_df)} cell boundaries to sdata['{SopaKeys.BAYSOR_BOUNDARIES}']"
+        f"Added sdata.tables['{SopaKeys.TABLE}'], and {len(geo_df)} cell boundaries to sdata['{SopaKeys.BAYSOR_BOUNDARIES}']"
     )
```

### Comparing `sopa-1.0.8/sopa/segmentation/methods.py` & `sopa-1.0.9/sopa/segmentation/methods.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/segmentation/patching.py` & `sopa-1.0.9/sopa/segmentation/patching.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/segmentation/shapes.py` & `sopa-1.0.9/sopa/segmentation/shapes.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/segmentation/stainings.py` & `sopa-1.0.9/sopa/segmentation/stainings.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/segmentation/tissue.py` & `sopa-1.0.9/sopa/segmentation/tissue.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/spatial/_build.py` & `sopa-1.0.9/sopa/spatial/_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from anndata import AnnData
 from anndata.utils import make_index_unique
 from scipy.sparse import SparseEfficiencyWarning, block_diag, csr_matrix, spmatrix
 from scipy.spatial import Delaunay
 from sklearn.metrics.pairwise import euclidean_distances
 from spatialdata import SpatialData
 
+from .._constants import SopaKeys
+
 log = logging.getLogger(__name__)
 __all__ = ["spatial_neighbors"]
 
 
 def spatial_neighbors(
     adata: AnnData | SpatialData,
     radius: tuple[float, float] | None,
@@ -36,15 +38,15 @@
         adata: AnnData object
         radius: tuple that prunes the final graph to only contain edges in interval `[min(radius), max(radius)]`. If `None`, all edges are kept.
         library_key: Optional batch key in adata.obs
         percentile: Percentile of the distances to use as threshold.
         set_diag: Whether to set the diagonal of the spatial connectivities to `1.0`.
     """
     if isinstance(adata, SpatialData):
-        adata = adata.table
+        adata = adata.tables[SopaKeys.TABLE]
 
     assert (
         radius is None or len(radius) == 2
     ), "Radius is expected to be a tuple (min_radius, max_radius)"
 
     log.info("Computing delaunay graph")
```

### Comparing `sopa-1.0.8/sopa/spatial/_graph.py` & `sopa-1.0.9/sopa/spatial/_graph.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/spatial/distance.py` & `sopa-1.0.9/sopa/spatial/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from spatialdata import SpatialData
 from tqdm import tqdm
 
+from .._constants import SopaKeys
 from ._build import _check_has_delaunay
 
 log = logging.getLogger(__name__)
 
 
 def cells_to_groups(
     adata: AnnData,
@@ -27,15 +28,15 @@
         key_added_prefix: Prefix to the key added in `adata.obsm`. If `None`, will return the `DataFrame` instead of saving it.
         ignore_zeros: If `True`, a cell distance to its own group is 0.
 
     Returns:
         A `Dataframe` of shape `n_obs * n_groups`, or `None` if `key_added_prefix` was provided (in this case, the dataframe is saved in `"{key_added_prefix}{group_key}"`)
     """
     if isinstance(adata, SpatialData):
-        adata = adata.table
+        adata = adata.tables[SopaKeys.TABLE]
 
     _check_has_delaunay(adata)
 
     distances_to_groups = {}
 
     if not adata.obs[group_key].dtype.name == "category":
         log.info(f"Converting adata.obs['{group_key}'] to category")
@@ -87,15 +88,15 @@
         target_group_key: Key of `adata.obs` containing the target groups (by default, uses `group_key`)
         ignore_zeros: If `True`, a cell distance to its own group is 0.
 
     Returns:
         `DataFrame` of shape `n_groups * n_groups_target` of mean hop-distances
     """
     if isinstance(adata, SpatialData):
-        adata = adata.table
+        adata = adata.tables[SopaKeys.TABLE]
 
     target_group_key = group_key if target_group_key is None else target_group_key
 
     df_distances = cells_to_groups(adata, target_group_key, None, ignore_zeros=ignore_zeros)
 
     if ignore_zeros:
         df_distances.replace(0, np.nan, inplace=True)
```

### Comparing `sopa-1.0.8/sopa/spatial/morpho.py` & `sopa-1.0.9/sopa/spatial/morpho.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         buffer: Expansion radius applied on components. By default, `3 * mean_distance_neighbors`
         perc_area_th: For each niche, components whose area is less than `perc_area_th * max_component_area` will be removed
 
     Returns:
         A `GeoDataFrame` with geometries for each niche component. We also compute the area/perimeter/roundness of each component.
     """
     if isinstance(adata, SpatialData):
-        adata = adata.table
+        adata = adata.tables[SopaKeys.TABLE]
 
     _check_has_delaunay(adata)
     data = {"geometry": [], niche_key: []}
 
     delaunay = Delaunay(adata.obsm["spatial"])
     connectivities = adata.obsp["spatial_connectivities"]
     values = adata.obs[niche_key].values
@@ -134,15 +134,15 @@
         key_added_suffix: Suffix added in the DataFrame columns. Defaults to "_distance_to_niche_".
         geometrize_niches_kwargs: Kwargs to the `sopa.spatial.geometrize_niches` function
 
     Returns:
         A `DataFrame` of shape `n_niches * n_statistics`
     """
     if isinstance(adata, SpatialData):
-        adata = adata.table
+        adata = adata.tables[SopaKeys.TABLE]
 
     gdf = geometrize_niches(adata, niche_key, **geometrize_niches_kwargs)
     value_counts = gdf[niche_key].value_counts()
 
     assert len(gdf), "No niche geometry found, stats can't be computed"
 
     log.info(f"Computing pairwise distances between {len(gdf)} components")
```

### Comparing `sopa-1.0.8/sopa/spatial/utils.py` & `sopa-1.0.9/sopa/spatial/utils.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/utils/data.py` & `sopa-1.0.9/sopa/utils/data.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/utils/image.py` & `sopa-1.0.9/sopa/utils/image.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/sopa/utils/polygon_crop.py` & `sopa-1.0.9/sopa/utils/polygon_crop.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.8/PKG-INFO` & `sopa-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopa
-Version: 1.0.8
+Version: 1.0.9
 Summary: Spatial-omics pipeline and analysis
 Home-page: https://gustaveroussy.github.io/sopa
 License: BSD-3-Clause
 Author: Quentin Blampey
 Author-email: quentin.blampey@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: BSD License
```

