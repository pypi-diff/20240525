# Comparing `tmp/timelineomat-0.6.0.tar.gz` & `tmp/timelineomat-0.7.0.tar.gz`

## Comparing `timelineomat-0.6.0.tar` & `timelineomat-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    16715 2020-02-02 00:00:00.000000 timelineomat-0.6.0/timelineomat.py
--rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 timelineomat-0.6.0/tests/test_basics.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.6.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.6.0/LICENSE
--rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 timelineomat-0.6.0/README.md
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 timelineomat-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     9510 2020-02-02 00:00:00.000000 timelineomat-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    16715 2020-02-02 00:00:00.000000 timelineomat-0.7.0/timelineomat.py
+-rw-r--r--   0        0        0    13611 2020-02-02 00:00:00.000000 timelineomat-0.7.0/tests/test_basics.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.7.0/LICENSE
+-rw-r--r--   0        0        0     8965 2020-02-02 00:00:00.000000 timelineomat-0.7.0/README.md
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 timelineomat-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9846 2020-02-02 00:00:00.000000 timelineomat-0.7.0/PKG-INFO
```

### Comparing `timelineomat-0.6.0/timelineomat.py` & `timelineomat-0.7.0/timelineomat.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,29 +230,28 @@
 def transform_events_to_times(
     *timelines,
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
     filter_fn: Optional[FilterFunction] = None,
     fallback_timezone: Optional[tz] = None,
     **kwargs,
-) -> list[TimeRangeTuple]:
+) -> Iterable[tuple[TimeRangeTuple, Event]]:
     assert "occlusions" not in kwargs, "occlusions not supported for this function"
     start_extractor = create_extractor(start_extractor)
     stop_extractor = create_extractor(stop_extractor)
-    transformed = []
     if not timelines:
-        return transformed
+        return
     for ev in chain.from_iterable(timelines):
         if filter_fn and not filter_fn(ev):
             continue
         try:
-            transformed.append(extract_tuple_from_event(ev, start_extractor, stop_extractor, fallback_timezone))
+            retval = (extract_tuple_from_event(ev, start_extractor, stop_extractor, fallback_timezone), ev)
+            yield retval
         except SkipEvent:
             continue
-    return transformed
 
 
 def _ordered_insert(
     event: Event,
     timeline: MutableSequence[Event],
     *,
     offset: Offset = 0,
@@ -422,15 +421,15 @@
             filter_fn=kwargs.get("filter_fn", self.filter_fn),
             fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
             start_setter=kwargs.get("start_setter", self.start_setter),
             stop_setter=kwargs.get("stop_setter", self.stop_setter),
             occlusions=kwargs.get("occlusions", None),
         )
 
-    def transform_events_to_times(self, *timelines, **kwargs) -> list[TimeRangeTuple]:
+    def transform_events_to_times(self, *timelines, **kwargs) -> Iterable[tuple[TimeRangeTuple, Event]]:
         assert "occlusions" not in kwargs, "occlusions not supported for this function"
         if not timelines:
             return []
         return transform_events_to_times(
             chain.from_iterable(timelines),
             start_extractor=kwargs.get("start_extractor", self.start_extractor),
             stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
```

### Comparing `timelineomat-0.6.0/tests/test_basics.py` & `timelineomat-0.7.0/tests/test_basics.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,23 +241,25 @@
     assert timeline[-1].start == dt(2024, 1, 3)
     timeline.append(
         Event1(**tm.streamline_event_times(new_event2, timeline, stop_extractor=one_time_overwrite_end)._asdict())
     )
     assert timeline[-1].stop == dt(2024, 1, 5)
     assert timeline[-1].start == dt(2024, 1, 4)
     # test conversion in TimeRangeTuple array
-    assert tm.transform_events_to_times(timeline) == [
+    assert [t for t, ev in tm.transform_events_to_times(timeline)] == [
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 2), stop=dt(2024, 1, 3)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5)),
     ]
     # test sorting
 
-    assert tm.transform_events_to_times(sorted(timeline, key=tm.streamline_event_times, reverse=True)) == [
+    assert [
+        t for t, ev in tm.transform_events_to_times(sorted(timeline, key=tm.streamline_event_times, reverse=True))
+    ] == [
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 2), stop=dt(2024, 1, 3)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
     ]
```

### Comparing `timelineomat-0.6.0/.gitignore` & `timelineomat-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timelineomat-0.6.0/LICENSE` & `timelineomat-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timelineomat-0.6.0/README.md` & `timelineomat-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 tm.streamline_event_times(Event(start=dt(2024, 1, 1), stop=dt(2024, 1, )), timeline) == TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5))
 
 # now integrate in django or whatever
 from django.db.models import Q
 
 q = Q()
 # this is not optimized
-for timetuple in tm.transform_events_to_times(timeline):
+for timetuple, ev in tm.transform_events_to_times(timeline):
     # timetuple is actually a 2 element tuple
-    q |= Q(timepoint__range=timetuple)
+    q |= Q(timepoint__range=timetuple) & ~Q(id=ev.id)
 
 ```
 
 
 ## Tricks to integrate in different datastructures
 
 TimelineOMat supports out of the box all kind of dicts as well as objects. It determinates
@@ -219,18 +219,22 @@
 position, offset = tm.ordered_insert(tm.streamline_event(new_event4, ordered_timeline[-1:]), ordered_timeline, offset=offset, direction="asc")
 
 ```
 
 
 ## How to integrate in db systems
 
-DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple)
+DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple) with transform_events_to_times.
+
+The result is an iterator which returns tuples of (TimeRangeTuple, Event)
 
 An example is in Usage
 
+Note: since 0.7.0 the Event from which the TimeRangeTuple is extracted is provided as second element
+
 
 ## How to use for sorting
 
 simple use the streamline_event_times(...) method of TimelineOMat without any timelines as key function. By using the TimelineOMat class parameters can be preinitialized
 
 The resulting tuple can be sorted
 
@@ -250,11 +254,12 @@
 
 ```
 
 Another usage of the key function would be together with heapq to implement some kind of merge sort
 
 ## Changes
 
+0.7.0 Breaking Change: transform_events_to_times is now an iterator and returns the event as second element
 0.6.0 add streamlined_ordered_insert
 0.5.0 add occlusions argument
 0.4.0 rename NoCallAllowed to NoCallAllowedError
 0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

### Comparing `timelineomat-0.6.0/pyproject.toml` & `timelineomat-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timelineomat"
-version = "0.6.0"
+version = "0.7.0"
 description = "Squeeze events into timelines and other timeline manipulations"
 authors = [{name = "Alexander Kaftan", email="devkral@web.de"}]
 license = "MIT"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
     "event",
```

### Comparing `timelineomat-0.6.0/PKG-INFO` & `timelineomat-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: timelineomat
-Version: 0.6.0
+Version: 0.7.0
 Summary: Squeeze events into timelines and other timeline manipulations
 Author-email: Alexander Kaftan <devkral@web.de>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: database,event,time,timelines
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -78,17 +78,17 @@
 tm.streamline_event_times(Event(start=dt(2024, 1, 1), stop=dt(2024, 1, )), timeline) == TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5))
 
 # now integrate in django or whatever
 from django.db.models import Q
 
 q = Q()
 # this is not optimized
-for timetuple in tm.transform_events_to_times(timeline):
+for timetuple, ev in tm.transform_events_to_times(timeline):
     # timetuple is actually a 2 element tuple
-    q |= Q(timepoint__range=timetuple)
+    q |= Q(timepoint__range=timetuple) & ~Q(id=ev.id)
 
 ```
 
 
 ## Tricks to integrate in different datastructures
 
 TimelineOMat supports out of the box all kind of dicts as well as objects. It determinates
@@ -241,18 +241,22 @@
 position, offset = tm.ordered_insert(tm.streamline_event(new_event4, ordered_timeline[-1:]), ordered_timeline, offset=offset, direction="asc")
 
 ```
 
 
 ## How to integrate in db systems
 
-DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple)
+DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple) with transform_events_to_times.
+
+The result is an iterator which returns tuples of (TimeRangeTuple, Event)
 
 An example is in Usage
 
+Note: since 0.7.0 the Event from which the TimeRangeTuple is extracted is provided as second element
+
 
 ## How to use for sorting
 
 simple use the streamline_event_times(...) method of TimelineOMat without any timelines as key function. By using the TimelineOMat class parameters can be preinitialized
 
 The resulting tuple can be sorted
 
@@ -272,11 +276,12 @@
 
 ```
 
 Another usage of the key function would be together with heapq to implement some kind of merge sort
 
 ## Changes
 
+0.7.0 Breaking Change: transform_events_to_times is now an iterator and returns the event as second element
 0.6.0 add streamlined_ordered_insert
 0.5.0 add occlusions argument
 0.4.0 rename NoCallAllowed to NoCallAllowedError
 0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

