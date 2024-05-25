# Comparing `tmp/geo_track_analyzer-1.3.2.tar.gz` & `tmp/geo_track_analyzer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_track_analyzer-1.3.2.tar", max compression
+gzip compressed data, was "geo_track_analyzer-1.4.0.tar", max compression
```

## Comparing `geo_track_analyzer-1.3.2.tar` & `geo_track_analyzer-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1076 2024-04-09 19:22:31.650846 geo_track_analyzer-1.3.2/LICENSE
--rw-r--r--   0        0        0     3492 2024-04-09 19:22:31.650846 geo_track_analyzer-1.3.2/README.md
--rw-r--r--   0        0        0      593 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/__init__.py
--rw-r--r--   0        0        0      778 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/cli/__init__.py
--rw-r--r--   0        0        0      859 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/cli/_extract_track.py
--rw-r--r--   0        0        0     4500 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/cli/_update_elevation.py
--rw-r--r--   0        0        0    16054 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/compare.py
--rw-r--r--   0        0        0     7774 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/enhancer.py
--rw-r--r--   0        0        0      462 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/exceptions.py
--rw-r--r--   0        0        0     4994 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/model.py
--rw-r--r--   0        0        0    14046 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/processing.py
--rw-r--r--   0        0        0    39346 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/track.py
--rw-r--r--   0        0        0        0 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/utils/__init__.py
--rw-r--r--   0        0        0    22327 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/utils/base.py
--rw-r--r--   0        0        0     5449 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/utils/internal.py
--rw-r--r--   0        0        0     4034 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/utils/track.py
--rw-r--r--   0        0        0      433 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/__init__.py
--rw-r--r--   0        0        0      352 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/constants.py
--rw-r--r--   0        0        0      441 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/interactive.py
--rw-r--r--   0        0        0    13262 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/map.py
--rw-r--r--   0        0        0    13665 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/profiles.py
--rw-r--r--   0        0        0     2160 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/utils.py
--rw-r--r--   0        0        0     2775 2024-04-09 19:22:31.658846 geo_track_analyzer-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     4859 1970-01-01 00:00:00.000000 geo_track_analyzer-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3492 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/README.md
+-rw-r--r--   0        0        0      593 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/__init__.py
+-rw-r--r--   0        0        0      778 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/cli/__init__.py
+-rw-r--r--   0        0        0      859 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/cli/_extract_track.py
+-rw-r--r--   0        0        0     4500 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/cli/_update_elevation.py
+-rw-r--r--   0        0        0    16054 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/compare.py
+-rw-r--r--   0        0        0     7774 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/enhancer.py
+-rw-r--r--   0        0        0      462 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/exceptions.py
+-rw-r--r--   0        0        0     8162 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/model.py
+-rw-r--r--   0        0        0    15919 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/processing.py
+-rw-r--r--   0        0        0    45732 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/track.py
+-rw-r--r--   0        0        0        0 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/utils/__init__.py
+-rw-r--r--   0        0        0    22327 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/utils/base.py
+-rw-r--r--   0        0        0     5449 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/utils/internal.py
+-rw-r--r--   0        0        0     1156 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/utils/model.py
+-rw-r--r--   0        0        0     5740 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/utils/track.py
+-rw-r--r--   0        0        0      670 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/visualize/__init__.py
+-rw-r--r--   0        0        0      414 2024-05-25 14:24:57.514459 geo_track_analyzer-1.4.0/geo_track_analyzer/visualize/constants.py
+-rw-r--r--   0        0        0      441 2024-05-25 14:24:57.518459 geo_track_analyzer-1.4.0/geo_track_analyzer/visualize/interactive.py
+-rw-r--r--   0        0        0    14406 2024-05-25 14:24:57.518459 geo_track_analyzer-1.4.0/geo_track_analyzer/visualize/map.py
+-rw-r--r--   0        0        0    16860 2024-05-25 14:24:57.518459 geo_track_analyzer-1.4.0/geo_track_analyzer/visualize/profiles.py
+-rw-r--r--   0        0        0    14689 2024-05-25 14:24:57.518459 geo_track_analyzer-1.4.0/geo_track_analyzer/visualize/summary.py
+-rw-r--r--   0        0        0     4949 2024-05-25 14:24:57.518459 geo_track_analyzer-1.4.0/geo_track_analyzer/visualize/utils.py
+-rw-r--r--   0        0        0     2757 2024-05-25 14:24:57.518459 geo_track_analyzer-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 geo_track_analyzer-1.4.0/PKG-INFO
```

### Comparing `geo_track_analyzer-1.3.2/LICENSE` & `geo_track_analyzer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/README.md` & `geo_track_analyzer-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/__init__.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/cli/__init__.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/cli/_extract_track.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/cli/_extract_track.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/cli/_update_elevation.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/cli/_update_elevation.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/compare.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/compare.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/enhancer.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/enhancer.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/processing.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/processing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import logging
 from datetime import timedelta
 from typing import Any, Callable, Dict, Literal, Union
 
 import numpy as np
 import pandas as pd
+import plotly
 from gpxpy.gpx import GPXTrack, GPXTrackPoint, GPXTrackSegment
 
 from geo_track_analyzer.exceptions import GPXPointExtensionError
+from geo_track_analyzer.model import Zones
 from geo_track_analyzer.utils.internal import get_extension_value
+from geo_track_analyzer.utils.model import format_zones_for_digitize
 
 logger = logging.getLogger(__name__)
 
 
 def _recalc_cumulated_columns(data: pd.DataFrame) -> pd.DataFrame:
     data = data.copy()
     data.cum_time = data.time.cumsum()
@@ -51,14 +54,17 @@
     return data
 
 
 def get_processed_track_data(
     track: GPXTrack,
     stopped_speed_threshold: float = 1,
     connect_segments: Literal["full", "forward"] = "forward",
+    heartrate_zones: None | Zones = None,
+    power_zones: None | Zones = None,
+    cadence_zones: None | Zones = None,
 ) -> tuple[float, float, float, float, pd.DataFrame]:
     """
     Process GPX track data and return a tuple of calculated values. The connect_segmen
     argument determines connection between segments in the DataFrame will be handled. As
     default each segment in the Track will be processed individually and the returned.
     Choosing forward will add the first point form the next segment to the end of each
     segment. So that each segment ends with the first point of the next segment.
@@ -130,28 +136,38 @@
     # Not really possible but keeps linters happy
     if track_data is None:
         raise RuntimeError("Track has no segments")
 
     # Recalculate all cumulated columns over the segments
     track_data = _recalc_cumulated_columns(track_data)
 
+    if heartrate_zones is not None:
+        track_data = add_zones_to_dataframe(track_data, "heartrate", heartrate_zones)
+    if power_zones is not None:
+        track_data = add_zones_to_dataframe(track_data, "power", power_zones)
+    if cadence_zones is not None:
+        track_data = add_zones_to_dataframe(track_data, "cadence", cadence_zones)
+
     return (
         track_time,
         track_distance,
         track_stopped_time,
         track_stopped_distance,
         track_data,
     )
 
 
 def get_processed_segment_data(
     segment: GPXTrackSegment,
     stopped_speed_threshold: float = 1,
     extend_segment_start: None | list[GPXTrackPoint] = None,
     extend_segment_end: None | list[GPXTrackPoint] = None,
+    heartrate_zones: None | Zones = None,
+    power_zones: None | Zones = None,
+    cadence_zones: None | Zones = None,
 ) -> tuple[float, float, float, float, pd.DataFrame]:
     """
     Calculate the speed and distance from point to point for a segment. This follows
     the implementation of the get_moving_data method in the implementation of
     gpx.GPXTrackSegment
 
     :param segment: GPXTrackSegment to process
@@ -202,14 +218,21 @@
         ) = _get_processed_data_w_time(segment, data, threshold_ms)
     else:
         distance, data = _get_processed_data_wo_time(segment, data)
         time, stopped_distance, stopped_time = 0, 0, 0
 
     data_df = pd.DataFrame(data)
 
+    if heartrate_zones is not None:
+        data_df = add_zones_to_dataframe(data_df, "heartrate", heartrate_zones)
+    if power_zones is not None:
+        data_df = add_zones_to_dataframe(data_df, "power", power_zones)
+    if cadence_zones is not None:
+        data_df = add_zones_to_dataframe(data_df, "cadence", cadence_zones)
+
     return (time, distance, stopped_time, stopped_distance, data_df)
 
 
 def _get_processed_data_w_time(
     segment: GPXTrackSegment, data: Dict[str, list[Any]], threshold_ms: float
 ) -> tuple[float, float, float, float, Dict[str, list[Any]]]:
     time = 0.0
@@ -347,15 +370,15 @@
     split_by: Literal["distance", "time"],
     split_at: float,
     moving_only: bool = True,
     method: Literal["first", "closest", "interploation"] = "closest",
 ) -> pd.DataFrame:
     split_idx_finder: Callable[[pd.Series, float], int]
     if method == "closest":
-        split_idx_finder = lambda s, v: np.abs(s.to_numpy() - v).argmin()
+        split_idx_finder = lambda s, v: np.abs(s.to_numpy() - v).argmin()  # type: ignore
     # TODO: Implement method in which the plotting point is interpolat to the ecxat val
     elif method == "interploation":
         raise NotImplementedError("Interploation splitting method not implemented")
     else:
         split_idx_finder = lambda s, v: s[s < v].index.max()
 
     data = data.copy()
@@ -391,7 +414,26 @@
         last_split = split_idx + 1
         i_segement += 1
 
     if last_split != data.index.max() + 1:
         data.loc[last_split : data.index.max() + 1, "segment"] = i_segement
 
     return data
+
+
+def add_zones_to_dataframe(
+    data: pd.DataFrame, metric: Literal["heartrate", "power", "cadence"], zones: Zones
+) -> pd.DataFrame:
+    zone_bins, names, zone_colors = format_zones_for_digitize(zones)
+    if zone_colors is None:
+        zone_colors = plotly.colors.sample_colorscale("viridis", len(names))
+
+    metric_data = data[metric][~data[metric].isna()]
+    binned_metric = pd.Series(
+        np.digitize(metric_data, zone_bins), index=metric_data.index
+    )
+    data[f"{metric}_zones"] = binned_metric.apply(lambda v: names[v - 1])
+    data[f"{metric}_zone_colors"] = binned_metric.apply(lambda v: zone_colors[v - 1])
+    data.loc[data[data[metric].isna()].index, f"{metric}_zones"] = names[0]
+    data.loc[data[data[metric].isna()].index, f"{metric}_zone_colors"] = zone_colors[0]
+
+    return data
```

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/track.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/track.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,65 +15,77 @@
 
 from geo_track_analyzer.compare import get_segment_overlap
 from geo_track_analyzer.exceptions import (
     TrackInitializationError,
     TrackTransformationError,
     VisualizationSetupError,
 )
-from geo_track_analyzer.model import PointDistance, Position3D, SegmentOverview
+from geo_track_analyzer.model import PointDistance, Position3D, SegmentOverview, Zones
 from geo_track_analyzer.processing import (
     get_processed_segment_data,
     get_processed_track_data,
 )
 from geo_track_analyzer.utils.base import (
     calc_elevation_metrics,
     fill_list,
     get_point_distance,
     interpolate_segment,
 )
 from geo_track_analyzer.utils.internal import get_extended_track_point
 from geo_track_analyzer.visualize import (
+    plot_segment_box_summary,
+    plot_segment_summary,
+    plot_segment_zones,
     plot_segments_on_map,
     plot_track_2d,
     plot_track_enriched_on_map,
     plot_track_line_on_map,
     plot_track_with_slope,
+    plot_track_zones,
 )
 
 logger = logging.getLogger(__name__)
 
 process_data_tuple_type = tuple[float, float, float, float, pd.DataFrame]
 
 
 class Track(ABC):
     """
     Abstract base container for geospacial Tracks that defines all methods common to
     all Track types.
     """
 
     def __init__(
-        self, stopped_speed_threshold: float, max_speed_percentile: int
+        self,
+        stopped_speed_threshold: float,
+        max_speed_percentile: int,
+        heartrate_zones: None | Zones = None,
+        power_zones: None | Zones = None,
+        cadence_zones: None | Zones = None,
     ) -> None:
         logger.debug(
             "Using threshold for stopped speed: %s km/h", stopped_speed_threshold
         )
         logger.debug("Using %s percentile to calculate overview", max_speed_percentile)
 
         self.stopped_speed_threshold = stopped_speed_threshold
         self.max_speed_percentile = max_speed_percentile
 
         self._processed_segment_data: dict[int, process_data_tuple_type] = {}
         self._processed_track_data: dict[str, tuple[int, process_data_tuple_type]] = {}
 
         self.session_data: Dict[str, str | int | float] = {}
 
+        self.heartrate_zones = heartrate_zones
+        self.power_zones = power_zones
+        self.cadence_zones = cadence_zones
+
     @property
     @abstractmethod
-    def track(self) -> GPXTrack:
-        ...
+    def track(self) -> GPXTrack: ...
 
     @property
     def n_segments(self) -> int:
         return len(self.track.segments)
 
     def add_segmeent(self, segment: GPXTrackSegment) -> None:
         """Add a new segment ot the track
@@ -307,15 +319,19 @@
             (
                 time,
                 distance,
                 stopped_time,
                 stopped_distance,
                 data,
             ) = get_processed_segment_data(
-                self.track.segments[n_segment], self.stopped_speed_threshold
+                self.track.segments[n_segment],
+                self.stopped_speed_threshold,
+                heartrate_zones=self.heartrate_zones,
+                power_zones=self.power_zones,
+                cadence_zones=self.cadence_zones,
             )
 
             if data.time.notna().any():
                 data = self._apply_outlier_cleaning(data)
 
             self._processed_segment_data[n_segment] = (
                 time,
@@ -338,15 +354,20 @@
         (
             time,
             distance,
             stopped_time,
             stopped_distance,
             processed_data,
         ) = get_processed_track_data(
-            self.track, self.stopped_speed_threshold, connect_segments=connect_segments
+            self.track,
+            self.stopped_speed_threshold,
+            connect_segments=connect_segments,
+            heartrate_zones=self.heartrate_zones,
+            power_zones=self.power_zones,
+            cadence_zones=self.cadence_zones,
         )
 
         if processed_data.time.notna().any():
             processed_data = self._apply_outlier_cleaning(processed_data)
 
         return self._set_processed_track_data(
             (
@@ -416,15 +437,15 @@
         - Use value of start point for first half and last point for second half
           (meet-center)
         - Linear interpolation (linear)
 
 
         :param spacing: Minimum distance between points added by the interpolation
         :param n_segment: segment in the track to use, defaults to 0
-        :param copy_extension: How should the extenstion (if present) be defined in the
+        :param copy_extensions: How should the extenstion (if present) be defined in the
             interpolated points.
         """
         self.track.segments[n_segment] = interpolate_segment(
             self.track.segments[n_segment], spacing, copy_extensions=copy_extensions
         )
 
         # Reset saved processed data
@@ -573,65 +594,119 @@
                 )
             )
         return matched_tracks
 
     def plot(
         self,
         kind: Literal[
-            "profile", "profile-slope", "map-line", "map-line-enhanced", "map-segments"
+            "profile",
+            "profile-slope",
+            "map-line",
+            "map-line-enhanced",
+            "map-segments",
+            "zone_summary",
+            "segment_zone_summary",
+            "segment_box",
+            "segment_summary",
         ],
         *,
         segment: None | int | list[int] = None,
         reduce_pp_intervals: None | int = None,
+        use_distance_segments: None | float = None,
         **kwargs,
     ) -> Figure:
         """
         Visualize the full track or a single segment.
 
         :param kind: Kind of plot to be generated
 
             - profile: Elevation profile of the track. May be enhanced with additional
               information like Velocity, Heartrate, Cadence, and Power. Pass keyword
-              args for :func:`~geo_track_analyzer.visualize.plot_track_2d`
+              args for [`plot_track_2d`][geo_track_analyzer.visualize.plot_track_2d]
             - profile-slope: Elevation profile with slopes between points. Use the
               reduce_pp_intervals argument to reduce the number of slope intervals.
               Pass keyword args for
-              :func:`~geo_track_analyzer.visualize.plot_track_with_slope`
+              [`plot_track_with_slope`][geo_track_analyzer.visualize.plot_track_with_slope]
             - map-line: Visualize coordinates on the map. Pass keyword args for
-              :func:`~geo_track_analyzer.visualize.plot_track_line_on_map`
+              [`plot_track_line_on_map`][geo_track_analyzer.visualize.plot_track_line_on_map]
             - map-line-enhanced: Visualize coordinates on the map. Enhance with
               additional information like Elevation, Velocity, Heartrate, Cadence, and
-              Power. Pass keyword args for
-              :func:`~geo_track_analyzer.visualize.plot_track_enriched_on_map`
+              Power. Pass keyword args for [`plot_track_enriched_on_map`][geo_track_analyzer.visualize.plot_track_enriched_on_map]
             - map-segments: Visualize coordinates on the map split into segments.
               Pass keyword args for
-              :func:`~geo_track_analyzer.visualize.plot_segments_on_map`
+              [`plot_segments_on_map`][geo_track_analyzer.visualize.plot_segments_on_map]
+            - zone_summary : Visualize an aggregate (time, distance, speed) value for a
+                metric (heartrate, power, cadence) with defined zones. Pass keyword args
+                for [`plot_track_zones`][geo_track_analyzer.visualize.plot_track_zones],
+                `aggregate` and `metric` are required.
+            - segment_zone_summary : Same as "zone_summary" but split aggregate per
+                segment [`plot_segment_zones`][geo_track_analyzer.visualize.plot_segment_zones]
+            - segment_box : Box plot of a metric (heartrate, power, cadence, speed,
+                elevation) per segment. Pass keyword args for [`plot_segments_on_map`][geo_track_analyzer.visualize.plot_segments_on_map]
+                `metric` is required.
+            - segment_summary : Visualize a aggregate (total_time, total_distance,
+                avg_speed, max_speed) per segment. Pass keyword args for [`plot_segment_summary`][geo_track_analyzer.visualize.plot_segment_summary]
+                `aggregate` is required.
         :param segment: Select a specific segment, multiple segments or all segmenets,
             defaults to None
         :param reduce_pp_intervals: Optionally pass a distance in m which is used to
             reduce the points in a track, defaults to None
+        :param use_distance_segments: Ignore all segments in data and split full track
+            into segments with passed cummulated distance in meters. If passed, segment
+            arg must be None. Defaults to None.
         :raises VisualizationSetupError: If the plot prequisites are not met
 
         :return: Figure (plotly)
         """
+        from geo_track_analyzer.utils.track import generate_distance_segments
+
+        if use_distance_segments is not None and segment is not None:
+            raise VisualizationSetupError(
+                f"use_distance_segments {use_distance_segments} cannot be passed with "
+                f"segment {segment}."
+            )
+
         valid_kinds = [
             "profile",
             "profile-slope",
             "map-line",
             "map-line-enhanced",
             "map-segments",
+            "zone_summary",
+            "segment_zone_summary",
+            "segment_box",
+            "segment_summary",
         ]
 
         require_elevation = ["profile", "profile-slope"]
         connect_segment_full = ["map-segments"]
         if kind not in valid_kinds:
             raise VisualizationSetupError(
                 f"Kind {kind} is not valid. Pass on of {','.join(valid_kinds)}"
             )
 
+        if kind in ["zone_summary", "segment_zone_summary"] and not all(
+            key in kwargs.keys() for key in ["metric", "aggregate"]
+        ):
+            raise VisualizationSetupError(
+                f"If {kind} is passed, **metric** and **aggregate** need to be passed"
+            )
+        if kind in ["segment_box"] and not all(
+            key in kwargs.keys() for key in ["metric"]
+        ):
+            raise VisualizationSetupError(
+                f"If {kind} is passed, **metric** needs to be passed"
+            )
+        if kind in ["segment_summary"] and not all(
+            key in kwargs.keys() for key in ["aggregate"]
+        ):
+            raise VisualizationSetupError(
+                f"If {kind} is passed, **metric** needs to be passed"
+            )
+
         if segment is None:
             from geo_track_analyzer.utils.track import extract_track_data_for_plot
 
             data = extract_track_data_for_plot(
                 track=self,
                 kind=kind,
                 require_elevation=require_elevation,
@@ -657,25 +732,36 @@
                 track=self,
                 segments=segment,
                 kind=kind,
                 require_elevation=require_elevation,
                 intervals=reduce_pp_intervals,
             )
 
+        if use_distance_segments is not None:
+            data = generate_distance_segments(data, use_distance_segments)
+
         fig: Figure
         if kind == "profile":
             fig = plot_track_2d(data=data, **kwargs)
         elif kind == "profile-slope":
             fig = plot_track_with_slope(data=data, **kwargs)
         elif kind == "map-line":
             fig = plot_track_line_on_map(data=data, **kwargs)
         elif kind == "map-line-enhanced":
             fig = plot_track_enriched_on_map(data=data, **kwargs)
-        else:
+        elif kind == "map-segments":
             fig = plot_segments_on_map(data=data, **kwargs)
+        elif kind == "zone_summary":
+            fig = plot_track_zones(data=data, **kwargs)
+        elif kind == "segment_zone_summary":
+            fig = plot_segment_zones(data=data, **kwargs)
+        elif kind == "segment_summary":
+            fig = plot_segment_summary(data=data, **kwargs)
+        elif kind == "segment_box":
+            fig = plot_segment_box_summary(data=data, **kwargs)
 
         return fig
 
     def split(
         self, coords: tuple[float, float], distance_threshold: float = 20
     ) -> None:
         """
@@ -718,28 +804,37 @@
 
     def __init__(
         self,
         gpx_file: str,
         n_track: int = 0,
         stopped_speed_threshold: float = 1,
         max_speed_percentile: int = 95,
+        heartrate_zones: None | Zones = None,
+        power_zones: None | Zones = None,
+        cadence_zones: None | Zones = None,
     ) -> None:
         """Initialize a Track object from a gpx file
 
         :param gpx_file: Path to the gpx file.
         :param n_track: Index of track in the gpx file, defaults to 0
         :param stopped_speed_threshold: Minium speed required for a point to be count
             as moving, defaults to 1
         :param max_speed_percentile: Points with speed outside of the percentile are not
             counted when analyzing the track, defaults to 95
+        :param heartrate_zones: Optional heartrate Zones, defaults to None
+        :param power_zones: Optional power Zones, defaults to None
+        :param cadence_zones: Optional cadence Zones, defaults to None
         """
 
         super().__init__(
             stopped_speed_threshold=stopped_speed_threshold,
             max_speed_percentile=max_speed_percentile,
+            heartrate_zones=heartrate_zones,
+            power_zones=power_zones,
+            cadence_zones=cadence_zones,
         )
 
         logger.info("Loading gpx track from file %s", gpx_file)
 
         gpx = self._get_gpx(gpx_file)
 
         self._track = gpx.tracks[n_track]
@@ -760,27 +855,36 @@
 
     def __init__(
         self,
         bytefile: bytes,
         n_track: int = 0,
         stopped_speed_threshold: float = 1,
         max_speed_percentile: int = 95,
+        heartrate_zones: None | Zones = None,
+        power_zones: None | Zones = None,
+        cadence_zones: None | Zones = None,
     ) -> None:
         """Initialize a Track object from a gpx file
 
         :param bytefile: Bytestring of a gpx file
         :param n_track: Index of track in the gpx file, defaults to 0
         :param stopped_speed_threshold: Minium speed required for a point to be count
             as moving, defaults to 1
         :param max_speed_percentile: Points with speed outside of the percentile are not
             counted when analyzing the track, defaults to 95
+        :param heartrate_zones: Optional heartrate Zones, defaults to None
+        :param power_zones: Optional power Zones, defaults to None
+        :param cadence_zones: Optional cadence Zones, defaults to None
         """
         super().__init__(
             stopped_speed_threshold=stopped_speed_threshold,
             max_speed_percentile=max_speed_percentile,
+            heartrate_zones=heartrate_zones,
+            power_zones=power_zones,
+            cadence_zones=cadence_zones,
         )
 
         gpx = gpxpy.parse(bytefile)
 
         self._track = gpx.tracks[n_track]
 
     @property
@@ -798,33 +902,42 @@
         elevations: None | list[float],
         times: None | list[datetime],
         heartrate: None | list[int] = None,
         cadence: None | list[int] = None,
         power: None | list[int] = None,
         stopped_speed_threshold: float = 1,
         max_speed_percentile: int = 95,
+        heartrate_zones: None | Zones = None,
+        power_zones: None | Zones = None,
+        cadence_zones: None | Zones = None,
     ) -> None:
         """A geospacial data track initialized from python objects
 
         :param points: List of Latitude/Longitude tuples
         :param elevations: Optional list of elevation for each point
         :param times: Optional list of times for each point
         :param heartrate: Optional list of heartrate values for each point
         :param cadence: Optional list of cadence values for each point
         :param power: Optional list of power values for each point
         :param stopped_speed_threshold: Minium speed required for a point to be count
             as moving, defaults to 1
         :param max_speed_percentile: Points with speed outside of the percentile are not
             counted when analyzing the track, defaults to 95
+        :param heartrate_zones: Optional heartrate Zones, defaults to None
+        :param power_zones: Optional power Zones, defaults to None
+        :param cadence_zones: Optional cadence Zones, defaults to None
         :raises TrackInitializationError: Raised if number of elevation, time, heatrate,
             or cadence values do not match passed points
         """
         super().__init__(
             stopped_speed_threshold=stopped_speed_threshold,
             max_speed_percentile=max_speed_percentile,
+            heartrate_zones=heartrate_zones,
+            power_zones=power_zones,
+            cadence_zones=cadence_zones,
         )
 
         gpx = GPX()
 
         gpx_track = GPXTrack()
         gpx.tracks.append(gpx_track)
 
@@ -950,26 +1063,35 @@
     """
 
     def __init__(
         self,
         segment: GPXTrackSegment,
         stopped_speed_threshold: float = 1,
         max_speed_percentile: int = 95,
+        heartrate_zones: None | Zones = None,
+        power_zones: None | Zones = None,
+        cadence_zones: None | Zones = None,
     ) -> None:
         """Wrap a GPXTrackSegment into a Track object
 
         :param segment: GPXTrackSegment
         :param stopped_speed_threshold: Minium speed required for a point to be count
             as moving, defaults to 1
         :param max_speed_percentile: Points with speed outside of the percentile are not
             counted when analyzing the track, defaults to 95
+        :param heartrate_zones: Optional heartrate Zones, defaults to None
+        :param power_zones: Optional power Zones, defaults to None
+        :param cadence_zones: Optional cadence Zones, defaults to None
         """
         super().__init__(
             stopped_speed_threshold=stopped_speed_threshold,
             max_speed_percentile=max_speed_percentile,
+            heartrate_zones=heartrate_zones,
+            power_zones=power_zones,
+            cadence_zones=cadence_zones,
         )
         gpx = GPX()
 
         gpx_track = GPXTrack()
         gpx.tracks.append(gpx_track)
 
         gpx_track.segments.append(segment)
@@ -987,29 +1109,38 @@
 
     def __init__(
         self,
         source: str | bytes,
         stopped_speed_threshold: float = 1,
         max_speed_percentile: int = 95,
         strict_elevation_loading: bool = False,
+        heartrate_zones: None | Zones = None,
+        power_zones: None | Zones = None,
+        cadence_zones: None | Zones = None,
     ) -> None:
         """Load a .fit file and extract the data into a Track object.
         NOTE: Tested with Wahoo devices only
 
         :param source: Patch to fit file or byte representation of fit file
         :param stopped_speed_threshold: Minium speed required for a point to be count
             as moving, defaults to 1
         :param max_speed_percentile: Points with speed outside of the percentile are not
             counted when analyzing the track, defaults to 95
         :param strict_elevation_loading: If set, only points are added to the track that
             have a valid elevation,defaults to False
+        :param heartrate_zones: Optional heartrate Zones, defaults to None
+        :param power_zones: Optional power Zones, defaults to None
+        :param cadence_zones: Optional cadence Zones, defaults to None
         """
         super().__init__(
             stopped_speed_threshold=stopped_speed_threshold,
             max_speed_percentile=max_speed_percentile,
+            heartrate_zones=heartrate_zones,
+            power_zones=power_zones,
+            cadence_zones=cadence_zones,
         )
 
         if isinstance(source, str):
             logger.info("Loading fit track from file %s", source)
         else:
             logger.info("Using passed bytes data as fit track")
```

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/utils/base.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/utils/base.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/utils/internal.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/utils/internal.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/utils/track.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/utils/track.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from itertools import pairwise
 from typing import Literal
 
 import pandas as pd
 
 from geo_track_analyzer.exceptions import VisualizationSetupError
 from geo_track_analyzer.processing import (
     get_processed_segment_data,
@@ -35,15 +36,19 @@
         if track.get_avg_pp_distance() >= intervals:
             logger.debug("Average pp distance larget than interval. Skipping reduction")
         else:
             _track = _track.clone()
             _track.reduce_points(intervals)
 
     _, _, _, _, data = get_processed_track_data(
-        _track, connect_segments=connect_segments
+        _track,
+        connect_segments=connect_segments,
+        heartrate_zones=track.heartrate_zones,
+        power_zones=track.power_zones,
+        cadence_zones=track.cadence_zones,
     )
 
     return data
 
 
 def extract_multiple_segment_data_for_plot(
     track: Track,
@@ -113,9 +118,50 @@
     if intervals is not None:
         if track.get_avg_pp_distance_in_segment(segment) >= intervals:
             logger.debug("Average pp distance larget than interval. Skipping reduction")
         else:
             segement = track.track.segments[segment].clone()
             segement.reduce_points(intervals)
 
-    _, _, _, _, data = get_processed_segment_data(segement)
+    _, _, _, _, data = get_processed_segment_data(
+        segement,
+        heartrate_zones=track.heartrate_zones,
+        power_zones=track.power_zones,
+        cadence_zones=track.cadence_zones,
+    )
+
+    return data
+
+
+def generate_distance_segments(data: pd.DataFrame, distance: float) -> pd.DataFrame:
+    """Generate segments with the distance specified with the passed parameter. Segments
+    present in the passed data will be replaced. Splitting is done based on the
+    distance_moving value in the data. Segements are split closest to the passed
+    distance. So extact cummulated distance in a segment depends on the pp-distance in
+    the track. The last segmeent may be shorter than the passed distance.
+
+    :param data: Dataframe create with extract_track_data_for_plot,
+        extract_segment_data_for_plot, or extract_multiple_segment_data_for_plot
+        methods.
+    :param distance: Intended segmeent distance
+
+    :return: Dataframe with updated segments
+    """
+    key = "cum_distance_moving"
+    max_distance = data.iloc[-1][key]
+
+    if max_distance < distance:
+        data["segment"] = 0
+        return data
+
+    distances, segments_ids = [0.0], [0]
+    while distances[-1] < max_distance:
+        distances.append(distances[-1] + distance)
+        segments_ids.append(segments_ids[-1] + 1)
+
+    new_segments = data.segment.copy()
+    new_segments.loc[:] = max(segments_ids)
+    for (start, end), idx in zip(pairwise(distances), segments_ids):
+        new_segments.iloc[data[(data[key] >= start) & (data[key] < end)].index] = idx
+
+    data["segment"] = new_segments
     return data
```

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/map.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/visualize/map.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,43 +74,53 @@
 
 def plot_track_enriched_on_map(
     data: pd.DataFrame,
     *,
     enrich_with_column: Literal[
         "elevation", "speed", "heartrate", "cadence", "power"
     ] = "elevation",
+    color_by_zone: bool = False,
     zoom: int = 13,
     height: None | int = None,
     width: None | int = None,
     overwrite_color_gradient: None | tuple[str, str] = None,
     overwrite_unit_text: None | str = None,
     cbar_ticks: int = 5,
     map_style: str = "open-street-map",
     **kwargs,
 ) -> Figure:
     """
     Plot the track line enriched with additional information (as z-axis) on a map.
 
     :param data: DataFrame containing track data.
     :param enrich_with_column: Column to enrich the track with, defaults to "elevation"
+    :param color_by_zone: If True, track will be covered by Zones. Only available for
+        enrich_with_column heartrate, cadence and power.
     :param zoom: Zoom level for the map, defaults to 13
     :param height: Height of the plot, defaults to None
     :param width: Width of the plot, defaults to None
     :param overwrite_color_gradient: Custom color gradient for the plot. Check
         track_analyzer.visualize.constants for defaults, defaults to None
     :param overwrite_unit_text: Custom unit text for the enrichment. Check
         track_analyzer.visualize.constants for defaults, defaults to None
     :param cbar_ticks: Number of color bar ticks, defaults to 5
     :param map_style: Valid map_style for plotly mapbox_style, defaults to
         open-street-map
     :param kwargs: Additional keyword arguments.
     :raises VisualizationSetupError: If no data is in passed enrich_with_column column
-
+    :raises VisualizationSetupError: If color_by_zone is passed and enricht_with_column
+        is unsupported or Zones are not set for the supported values
     :return: Plotly Figure object.
     """
+    if color_by_zone and (
+        (enrich_with_column not in ["heartrate", "cadence", "power"])
+        or (f"{enrich_with_column}_zones" not in data.columns)
+    ):
+        raise VisualizationSetupError("Zone data is not provided in passed dataframe")
+
     mask = data.moving
 
     plot_data = data[mask]
 
     center_lat, center_lon = center_geolocation(
         [(r["latitude"], r["longitude"]) for r in data[mask].to_dict("records")]
     )
@@ -121,15 +131,15 @@
         if overwrite_unit_text is None
         else overwrite_unit_text
     )
     enrich_type = (
         int if enrich_with_column in ["heartrate", "cadence", "power"] else float
     )
 
-    # ~~~~~~~~~~~ Generator colors for passed column ~~~~~~~~~~~~~~~~~
+    # ~~~~~~~~~~~ Colors ~~~~~~~~~~~~~~~~~
     color_column_values = plot_data[enrich_with_column]
 
     if color_column_values.isna().all():
         raise VisualizationSetupError(
             f"Plotting not possible. No values for {enrich_with_column} in passed data."
         )
 
@@ -143,69 +153,77 @@
         color_column_values = color_column_values[~color_column_values.isna()]
 
     if enrich_with_column == "speed":
         color_column_values = color_column_values * 3.6
     diff_abs = color_column_values.max() - color_column_values.min()
     assert diff_abs > 0
 
-    if overwrite_color_gradient:
-        color_min, color_max = overwrite_color_gradient
+    colorbar_trace = None
+    # ~~~~~~~~~~~~~~~~ Color by Zone ~~~~~~~~~~~~~~~~~~~~~~~
+    if color_by_zone:
+        color_col = f"{enrich_with_column}_zone_colors"
+        colors = plot_data[color_col]
+        marker = go.scattermapbox.Marker(color=colors)
+    # ~~~~~~~~~~~~~~~~ Generate color gradient from value ~~~~~~~~~~~~~~~
     else:
-        if enrich_with_column in COLOR_GRADIENTS.keys():
-            color_min, color_max = COLOR_GRADIENTS[enrich_with_column]
-        else:
-            color_min, color_max = DEFAULT_COLOR_GRADIENT
-    color_map = pd.Series(
-        data=get_color_gradient(color_min, color_max, round(diff_abs) + 1),
-        index=range(
-            round(color_column_values.min()), round(color_column_values.max()) + 1
-        ),
-    )
-
-    def color_mapper(value: float) -> str:
-        if value < color_map.index.start:
-            return color_map.iloc[0]
-        elif value > color_map.index.stop:
-            return color_map.iloc[-1]
+        if overwrite_color_gradient:
+            color_min, color_max = overwrite_color_gradient
         else:
-            return color_map.loc[int(value)]
-
-    colors = color_column_values.apply(color_mapper).to_list()
-    marker = go.scattermapbox.Marker(color=colors)
+            if enrich_with_column in COLOR_GRADIENTS.keys():
+                color_min, color_max = COLOR_GRADIENTS[enrich_with_column]
+            else:
+                color_min, color_max = DEFAULT_COLOR_GRADIENT
+        color_map = pd.Series(
+            data=get_color_gradient(color_min, color_max, round(diff_abs) + 1),
+            index=range(
+                round(color_column_values.min()), round(color_column_values.max()) + 1
+            ),
+        )
 
-    # ~~~~~~~~~~~~~~~ Colorbar for the passed column ~~~~~~~~~~~~~~~~~~~~
-    splits = 1 / (cbar_ticks - 1)
-    factor = 0.0
-    tick_vals = []
-    tick_cols = []
-    while factor <= 1:
-        idx = int(diff_abs * factor)
-        tick_vals.append(color_map.index[idx])
-        tick_cols.append(color_map.iloc[idx])
-        factor += splits
-
-    colorbar_trace = go.Scatter(
-        x=[None],
-        y=[None],
-        mode="markers",
-        marker=dict(
-            colorscale=color_map.to_list(),
-            showscale=True,
-            cmin=color_column_values.min(),
-            cmax=color_column_values.max(),
-            colorbar=dict(
-                title=enrich_with_column.capitalize(),
-                thickness=10,
-                tickvals=tick_vals,
-                ticktext=tick_vals,
-                outlinewidth=0,
+        def color_mapper(value: float) -> str:
+            if value < color_map.index.start:
+                return color_map.iloc[0]
+            elif value > color_map.index.stop:
+                return color_map.iloc[-1]
+            else:
+                return color_map.loc[int(value)]
+
+        colors = color_column_values.apply(color_mapper).to_list()
+        marker = go.scattermapbox.Marker(color=colors)
+
+        # ~~~~~~~~~~~~~~~ Colorbar for the passed column ~~~~~~~~~~~~~~~~~~~~
+        splits = 1 / (cbar_ticks - 1)
+        factor = 0.0
+        tick_vals = []
+        tick_cols = []
+        while factor <= 1:
+            idx = int(diff_abs * factor)
+            tick_vals.append(color_map.index[idx])
+            tick_cols.append(color_map.iloc[idx])
+            factor += splits
+
+        colorbar_trace = go.Scatter(
+            x=[None],
+            y=[None],
+            mode="markers",
+            marker=dict(
+                colorscale=color_map.to_list(),
+                showscale=True,
+                cmin=color_column_values.min(),
+                cmax=color_column_values.max(),
+                colorbar=dict(
+                    title=enrich_with_column.capitalize(),
+                    thickness=10,
+                    tickvals=tick_vals,
+                    ticktext=tick_vals,
+                    outlinewidth=0,
+                ),
             ),
-        ),
-        hoverinfo="none",
-    )
+            hoverinfo="none",
+        )
 
     # ~~~~~~~~~~~~~~~ Build figure ~~~~~~~~~~~~~~~~~~~
     fig = go.Figure(
         go.Scattermapbox(
             lat=plot_data["latitude"],
             lon=plot_data["longitude"],
             mode="markers",
@@ -216,15 +234,16 @@
             + "<b>Lat</b>: %{lat:4.6f}°<br>"
             + "<b>Lon</b>: %{lon:4.6f}°<br>",
             text=[enrich_type(v) for v in color_column_values.to_list()],
             name="",
         )
     )
 
-    fig.add_trace(colorbar_trace)
+    if colorbar_trace is not None:
+        fig.add_trace(colorbar_trace)
 
     fig.update_layout(mapbox_style=map_style)
     fig.update_layout(
         margin={"r": 57, "t": 5, "l": 49, "b": 5},
         mapbox={
             "style": map_style,
             "zoom": zoom,
```

### Comparing `geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/profiles.py` & `geo_track_analyzer-1.4.0/geo_track_analyzer/visualize/profiles.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
+from typing import Callable, Literal
 
 import pandas as pd
 import plotly.graph_objects as go
 from plotly.graph_objs import Figure
 from plotly.subplots import make_subplots
 
 from geo_track_analyzer.exceptions import VisualizationSetupError
-from geo_track_analyzer.visualize.utils import get_slope_colors
+from geo_track_analyzer.visualize.utils import get_slope_colors, group_dataframe
 
 logger = logging.getLogger(__name__)
 
 
 def _check_segment_availability(data: pd.DataFrame) -> bool:
     if "segment" not in data.columns:
         logger.warning(
@@ -36,14 +37,157 @@
             line_dash="dash",
             line_color="darkslategray" if color is None else color,
             annotation_text=f"Segment {data.loc[segment_border_idx].segment}",
             annotation_borderpad=5,
         )
 
 
+def _add_secondary(
+    fig: Figure,
+    data: pd.DataFrame,
+    secondary: Literal["velocity", "heartrate", "cadence", "power"],
+    split_by_zone: bool,
+    min_zone_size: float,
+) -> None:
+    mode = "lines"
+    fill: None | str = "tozeroy"
+    y_range_max_factor = 1.2
+    y_converter: Callable[[pd.Series], pd.Series] = lambda s: s.fillna(0).astype(int)
+    if secondary == "velocity":
+        title = "Velocity [km/h]"
+        y_range_max_factor = 2.1
+        y_converter = lambda s: s * 3.6
+    elif secondary == "heartrate":
+        title = "Heart Rate [bpm]"
+    elif secondary == "power":
+        title = "Power [W]"
+    elif secondary == "cadence":
+        title = "Cadence [rpm]"
+        fill = None
+        mode = "markers"
+
+    else:
+        raise RuntimeError
+
+    if pd.isna(data[secondary]).all():
+        raise VisualizationSetupError(
+            "Requested to plot heart rate but no heart rate information available "
+            "in data"
+        )
+
+    if split_by_zone:
+        _add_secondary_disonct(
+            fig=fig,
+            data=data,
+            secondary=secondary,
+            y_converter=y_converter,
+            y_range_max_factor=y_range_max_factor,
+            title=title,
+            mode=mode,
+            fill=fill,
+            min_zone_size=min_zone_size,
+        )
+    else:
+        y_data = y_converter(data[secondary])
+        y_range = (0, y_data.max() * y_range_max_factor)
+
+        _add_secondary_cont(
+            fig=fig,
+            x=data.cum_distance_moving,
+            y=y_data,
+            y_range=y_range,
+            title=title,
+            mode=mode,
+            fill=fill,
+        )
+
+
+def _add_secondary_cont(
+    fig: Figure,
+    # data: pd.DataFrame,
+    x: pd.Series,
+    y: pd.Series,
+    y_range: None | tuple[float, float],
+    title: str,
+    mode: str,
+    fill: None | str,
+    color: None | str = None,
+    legend_group: None | str = None,
+    show_legend: bool = False,
+    y_title: None | str = None,
+) -> None:
+    scatter_kwargs = dict(
+        x=x,
+        y=y,
+        mode=mode,
+        name=title,
+        legendgroup=legend_group,
+        fill=fill,
+        showlegend=show_legend,
+    )
+    if color is not None:
+        scatter_kwargs["line_color"] = color
+    fig.add_trace(
+        go.Scatter(**scatter_kwargs),
+        secondary_y=True,
+    )
+    fig.update_yaxes(
+        title_text=title if y_title is None else y_title,
+        secondary_y=True,
+        range=y_range,
+    )
+
+
+def _add_secondary_disonct(
+    fig: Figure,
+    data: pd.DataFrame,
+    secondary: str,
+    y_converter: Callable[[pd.Series], pd.Series],
+    y_range_max_factor: float,
+    title: str,
+    mode: str,
+    fill: None | str,
+    min_zone_size: float,
+) -> None:
+    if f"{secondary}_zones" not in data.columns:
+        raise VisualizationSetupError("Zone data is not provided in passed dataframe")
+
+    zone_data = group_dataframe(
+        data, f"{secondary}_zones", int(len(data) * min_zone_size)
+    )
+    seen_group_names = []
+    y_max = -99
+    for data_ in zone_data[::-1]:
+        group_name = data_[f"{secondary}_zones"].iloc[-1]
+
+        y_data = y_converter(data_[secondary])
+        y_max = max(y_max, y_data.max() * y_range_max_factor)
+
+        _add_secondary_cont(
+            fig=fig,
+            x=data_.cum_distance_moving,
+            y=y_data,
+            y_range=None,
+            title=group_name,
+            mode=mode,
+            fill=fill,
+            color=data_[f"{secondary}_zone_colors"].iloc[-1],
+            legend_group=group_name,
+            show_legend=group_name not in seen_group_names,
+            y_title=title,
+        )
+        if group_name not in seen_group_names:
+            seen_group_names.append(group_name)
+
+    fig.update_yaxes(
+        range=(0, y_max),
+        secondary_y=True,
+    )
+
+
 def plot_track_2d(
     data: pd.DataFrame,
     *,
     include_velocity: bool = False,
     include_heartrate: bool = False,
     include_cadence: bool = False,
     include_power: bool = False,
@@ -53,14 +197,16 @@
     width: None | int = 1800,
     pois: None | list[tuple[float, float]] = None,
     color_elevation: None | str = None,
     color_additional_trace: None | str = None,
     color_poi: None | str = None,
     color_segment_border: None | str = None,
     slider: bool = False,
+    split_by_zone: bool = False,
+    min_zone_size: float = 0.0025,
     **kwargs,
 ) -> Figure:
     """Elevation profile of the track. May be enhanced with additional information like
     Velocity, Heartrate, Cadence, and Power.
 
     :param data: DataFrame containing track data
     :param include_velocity: Plot velocity as second y-axis, defaults to False
@@ -80,22 +226,30 @@
     :param color_additional_trace: Color of velocity/heartrate/cadence/power as str
         interpretable by plotly, defaults to None
     :param color_poi: Color of the pois as str interpretable by plotly, defaults to None
     :param color_segment_border: Color of the segment border lines as str interpretable
         by plotly, defaults to None
     :param slider: Should a slide be included in the plot to zoom into the x-axis,
         defaults to False
+    :param split_by_zone: If True, and one for included_* flags is passed and Zones are
+        set for the corresponding extension are set, the Zones will be colored
+        according to the zone colors.
+    :param min_zone_size: Minimum fraction of points required for a distinct zone, if
+        split_by_Zone is passed.
     :raises VisualizationSetupError: If more than one of include_velocity,
         include_heartrate, include_cadence, or include_power was set the True
     :raises VisualizationSetupError: If elevation data is missing in the data
     :raises VisualizationSetupError: If the data requried for the additional data is
        missing
+    :raises VisualizationSetupError: If split_by_zone is passed but Zones are not set
 
     :return: Plotly Figure object.
     """
+    if split_by_zone:
+        color_additional_trace = None
     if (
         sum(
             [
                 int(include_velocity),
                 int(include_heartrate),
                 int(include_cadence),
                 int(include_power),
@@ -107,15 +261,15 @@
             "Only one of include_velocity, include_heartrate, include_cadence, "
             "and include_power can be set to True"
         )
     mask = data.moving
     if strict_data_selection:
         mask = mask & data.in_speed_percentile
 
-    data_for_plot = data[mask]
+    data_for_plot: pd.DataFrame = data[mask].copy()  # type: ignore
 
     if show_segment_borders:
         show_segment_borders = _check_segment_availability(data_for_plot)
 
     if data_for_plot.elevation.isna().all():
         raise VisualizationSetupError("Can not plot profile w/o elevation information")
 
@@ -131,79 +285,45 @@
                 "<b>Lat</b>: {lat:4.6f}°<br><b>Lon</b>: {lon:4.6f}°<br>".format(
                     lon=rcrd["longitude"], lat=rcrd["latitude"]
                 )
                 for rcrd in data_for_plot.to_dict("records")
             ],
             hovertemplate="<b>Distance</b>: %{x:.1f} km <br><b>Elevation</b>: "
             + "%{y:.1f} m <br>%{text}<extra></extra>",
+            showlegend=False,
         ),
         secondary_y=False,
     )
     fig.update_yaxes(
         title_text="Elevation [m]",
         secondary_y=False,
         range=[
             data_for_plot.elevation.min() * 0.97,
             data_for_plot.elevation.max() * 1.05,
         ],
     )
     fig.update_xaxes(title_text="Distance [m]")
 
-    y_data = None
-    y_range = None
-    title = None
-    mode = "lines"
-    fill: None | str = "tozeroy"
+    secondary = None
     if include_velocity:
-        y_data = data_for_plot.apply(lambda c: c.speed * 3.6, axis=1)
-        title = "Velocity [km/h]"
-        y_range = [0, y_data.max() * 2.1]
+        secondary = "velocity"
     if include_heartrate:
-        if pd.isna(data_for_plot.heartrate).all():
-            raise VisualizationSetupError(
-                "Requested to plot heart rate but no heart rate information available "
-                "in data"
-            )
-        y_data = data_for_plot.heartrate.fillna(0).astype(int)
-        title = "Heart Rate [bpm]"
-        y_range = [0, y_data.max() * 1.2]
+        secondary = "heartrate"
     if include_cadence:
-        if pd.isna(data_for_plot.cadence).all():
-            raise VisualizationSetupError(
-                "Requested to plot cadence but no cadence information available in data"
-            )
-        y_data = data_for_plot.cadence.fillna(0).astype(int)
-        title = "Cadence [rpm]"
-        mode = "markers"
-        fill = None
-        y_range = [0, y_data.max() * 1.2]
+        secondary = "cadence"
     if include_power:
-        if pd.isna(data_for_plot.power).all():
-            raise VisualizationSetupError(
-                "Requested to plot power but no power information available in data"
-            )
-        y_data = data_for_plot.power.fillna(0).astype(int)
-        title = "Power [W]"
-        y_range = [0, y_data.max() * 1.2]
+        secondary = "power"
 
-    if y_data is not None:
-        fig.add_trace(
-            go.Scatter(
-                x=data_for_plot.cum_distance_moving,
-                y=y_data,
-                mode=mode,
-                name=title,
-                fill=fill,
-            ),
-            secondary_y=True,
-        )
-        fig.update_yaxes(
-            title_text=title,
-            secondary_y=True,
-            range=y_range,
+    if secondary is not None:
+        _add_secondary(
+            fig=fig,
+            data=data_for_plot,
+            secondary=secondary,
+            split_by_zone=split_by_zone,
+            min_zone_size=min_zone_size,
         )
 
     if pois is not None:
         for i_poi, poi in enumerate(pois):
             lat, lng = poi
             poi_data = data_for_plot[
                 (data_for_plot.latitude == lat) & (data_for_plot.longitude == lng)
@@ -222,21 +342,24 @@
                 marker=dict(
                     size=20,
                     color="MediumPurple" if color_poi is None else color_poi,
                     symbol="triangle-up",
                     standoff=10,
                     angle=180,
                 ),
+                showlegend=False,
             )
 
     if show_segment_borders:
         _add_segment_borders(data_for_plot, fig, color_segment_border)
 
     fig.update_layout(
-        showlegend=False, autosize=False, margin={"r": 0, "t": 0, "l": 0, "b": 0}
+        showlegend=split_by_zone,
+        autosize=False,
+        margin={"r": 0, "t": 0, "l": 0, "b": 0},
     )
     if height is not None:
         fig.update_layout(height=height)
     if width is not None:
         fig.update_layout(width=width)
 
     fig.update_xaxes(
@@ -297,15 +420,15 @@
 
     :return: Plotly Figure object
     """
     slope_color_map = get_slope_colors(
         *slope_gradient_color, max_slope=max_slope, min_slope=min_slope
     )
 
-    data = data[data.moving].copy()
+    data = data[data.moving].copy()  # type: ignore
 
     if data.elevation.isna().all():
         raise VisualizationSetupError("Can not plot profile w/o elevation information")
 
     if show_segment_borders:
         show_segment_borders = _check_segment_availability(data)
```

### Comparing `geo_track_analyzer-1.3.2/pyproject.toml` & `geo_track_analyzer-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geo-track-analyzer"
-version = "1.3.2"
+version = "1.4.0"
 description = "Analyze geospacial data tracks"
 authors = ["Korbinian Schweiger <korbinian.schweiger@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Visualization",
 ]
@@ -12,52 +12,53 @@
 readme = "README.md"
 packages = [{ include = "geo_track_analyzer" }]
 documentation = "https://kschweiger.github.io/track_analyzer/"
 repository = "https://github.com/kschweiger/track_analyzer"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
-numpy = "^1.26.4"
-gpxpy = "^1.6.2"
-coloredlogs = "^15.0.1"
-requests = "^2.31.0"
-plotly = "^5.19.0"
-pandas = "^2.2.1"
-fitparse = "^1.2.0"
-pydantic = "^2.6.2"
-pydantic-numpy = "^4.2.0"
-click = { version = "^8.1.7", optional = true }
-rich = { version = "^13.7.0", optional = true }
+numpy = "^1"
+gpxpy = "^1.6"
+coloredlogs = "^15"
+requests = "^2"
+plotly = "^5"
+pandas = "^2"
+fitparse = "^1.2"
+pydantic = "^2"
+pydantic-numpy = "^5"
+click = { version = "^8", optional = true }
+rich = { version = "^13", optional = true }
 
 [tool.poetry.extras]
 cli = ["click", "rich"]
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.6.2"
-black = "^23.12.1"
+pre-commit = "^3.7.0"
 flake8 = "^7.0.0"
-mypy = "^1.8.0"
-types-requests = "^2.31.0.20240218"
-ruff = "^0.2.2"
+mypy = "^1.10.0"
+types-requests = "^2.31.0.20240406"
+ruff = "~0.4.3"
 bpython = "^0.24"
-git-changelog = "^2.4.0"
+git-changelog = "^2.5.2"
+debugpy = "^1.8.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.4.4"
-pytest-cov = "^4.1.0"
-pytest-mock = "^3.12.0"
+pytest = "^8.2.0"
+pytest-cov = "^5.0.0"
+pytest-mock = "^3.14.0"
 pytest-dependency = "^0.6.0"
-pytest-sugar = "^0.9.7"
+pytest-sugar = "^1.0.0"
+pytest-retry = "^1.6.2"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.11"
```

### Comparing `geo_track_analyzer-1.3.2/PKG-INFO` & `geo_track_analyzer-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-track-analyzer
-Version: 1.3.2
+Version: 1.4.0
 Summary: Analyze geospacial data tracks
 Home-page: https://github.com/kschweiger/track_analyzer
 License: MIT
 Keywords: fit,gpx,visualization,analysis
 Author: Korbinian Schweiger
 Author-email: korbinian.schweiger@gmail.com
 Requires-Python: >=3.10,<3.13
@@ -12,25 +12,25 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Provides-Extra: cli
-Requires-Dist: click (>=8.1.7,<9.0.0) ; extra == "cli"
-Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
-Requires-Dist: fitparse (>=1.2.0,<2.0.0)
-Requires-Dist: gpxpy (>=1.6.2,<2.0.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pandas (>=2.2.1,<3.0.0)
-Requires-Dist: plotly (>=5.19.0,<6.0.0)
-Requires-Dist: pydantic (>=2.6.2,<3.0.0)
-Requires-Dist: pydantic-numpy (>=4.2.0,<5.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0) ; extra == "cli"
+Requires-Dist: click (>=8,<9) ; extra == "cli"
+Requires-Dist: coloredlogs (>=15,<16)
+Requires-Dist: fitparse (>=1.2,<2.0)
+Requires-Dist: gpxpy (>=1.6,<2.0)
+Requires-Dist: numpy (>=1,<2)
+Requires-Dist: pandas (>=2,<3)
+Requires-Dist: plotly (>=5,<6)
+Requires-Dist: pydantic (>=2,<3)
+Requires-Dist: pydantic-numpy (>=5,<6)
+Requires-Dist: requests (>=2,<3)
+Requires-Dist: rich (>=13,<14) ; extra == "cli"
 Project-URL: Documentation, https://kschweiger.github.io/track_analyzer/
 Project-URL: Repository, https://github.com/kschweiger/track_analyzer
 Description-Content-Type: text/markdown
 
 [![Testing](https://github.com/kschweiger/track_analyzer/actions/workflows/test.yml/badge.svg)](https://github.com/kschweiger/track_analyzer/actions/workflows/test.yml)
 [![Build Documentation](https://github.com/kschweiger/track_analyzer/actions/workflows/doc.yml/badge.svg)](https://github.com/kschweiger/track_analyzer/actions/workflows/doc.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/geo-track-analyzer)
```

