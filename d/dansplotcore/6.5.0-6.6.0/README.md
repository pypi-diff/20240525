# Comparing `tmp/dansplotcore-6.5.0.tar.gz` & `tmp/dansplotcore-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.5.0.tar", last modified: Thu May 16 21:56:10 2024, max compression
+gzip compressed data, was "dansplotcore-6.6.0.tar", last modified: Sat May 25 21:49:49 2024, max compression
```

## Comparing `dansplotcore-6.5.0.tar` & `dansplotcore-6.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.5.0/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     5030 2024-05-14 22:54:52.000000 dansplotcore-6.5.0/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9713 2024-05-13 23:40:36.000000 dansplotcore-6.5.0/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.5.0/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2234 2024-05-14 19:17:01.000000 dansplotcore-6.5.0/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)    10016 2024-05-16 21:54:43.000000 dansplotcore-6.5.0/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.5.0/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.5.0/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-05-16 21:56:10.000000 dansplotcore-6.5.0/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-05-16 21:56:10.312446 dansplotcore-6.5.0/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-05-16 21:55:43.000000 dansplotcore-6.5.0/setup.py
+drwxrwxr-x   0 dan       (1000) dan       (1000)        0 2024-05-25 21:49:49.824824 dansplotcore-6.6.0/
+-rw-rw-r--   0 dan       (1000) dan       (1000)      344 2024-05-25 21:49:49.824824 dansplotcore-6.6.0/PKG-INFO
+drwxrwxr-x   0 dan       (1000) dan       (1000)        0 2024-05-25 21:49:49.820824 dansplotcore-6.6.0/dansplotcore/
+-rw-rw-r--   0 dan       (1000) dan       (1000)      158 2024-05-22 03:07:47.000000 dansplotcore-6.6.0/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1000) dan       (1000)     6154 2024-05-25 21:35:49.000000 dansplotcore-6.6.0/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1000) dan       (1000)    10338 2024-05-25 21:47:53.000000 dansplotcore-6.6.0/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1000) dan       (1000)     2645 2024-05-22 03:07:47.000000 dansplotcore-6.6.0/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1000) dan       (1000)     2234 2024-05-22 03:07:47.000000 dansplotcore-6.6.0/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1000) dan       (1000)    11982 2024-05-25 21:48:19.000000 dansplotcore-6.6.0/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1000) dan       (1000)     2907 2024-05-22 03:07:47.000000 dansplotcore-6.6.0/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1000) dan       (1000)     7455 2024-05-22 03:07:47.000000 dansplotcore-6.6.0/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1000) dan       (1000)        0 2024-05-25 21:49:49.824824 dansplotcore-6.6.0/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1000) dan       (1000)      344 2024-05-25 21:49:49.000000 dansplotcore-6.6.0/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1000) dan       (1000)      382 2024-05-25 21:49:49.000000 dansplotcore-6.6.0/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1000) dan       (1000)        1 2024-05-25 21:49:49.000000 dansplotcore-6.6.0/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1000) dan       (1000)       15 2024-05-25 21:49:49.000000 dansplotcore-6.6.0/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1000) dan       (1000)       13 2024-05-25 21:49:49.000000 dansplotcore-6.6.0/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1000) dan       (1000)       38 2024-05-25 21:49:49.824824 dansplotcore-6.6.0/setup.cfg
+-rw-rw-r--   0 dan       (1000) dan       (1000)      492 2024-05-25 21:49:32.000000 dansplotcore-6.6.0/setup.py
```

### Comparing `dansplotcore-6.5.0/dansplotcore/media.py` & `dansplotcore-6.6.0/dansplotcore/media.py`

 * *Files 15% similar despite different names*

```diff
@@ -81,14 +81,17 @@
     def add_vertices(self, vertices):
         for v in self.vertices:
             self.add(v)
 
     def add_data(self, data):
         self.data.extend(data)
 
+    def clear(self):
+        self.data.clear()
+
     def prep(self, usage):
         gl.glBindBuffer(gl.GL_ARRAY_BUFFER, self.buffer)
         gl.glBufferData(
             gl.GL_ARRAY_BUFFER,
             len(self.data)*4,
             (gl.GLfloat * len(self.data))(*self.data),
             getattr(gl, f'GL_{usage.upper()}_DRAW'),
@@ -137,51 +140,77 @@
 def capture():
     pyglet.image.get_buffer_manager().get_color_buffer().save('plot.png')
 
 def clear():
     gl.glClear(gl.GL_COLOR_BUFFER_BIT)
 
 def set_callbacks(
-    mouse_drag,
-    mouse_scroll,
-    key_press,
-    draw,
-    resize,
+    mouse_press_left=None,
+    mouse_press_right=None,
+    mouse_release_left=None,
+    mouse_release_right=None,
+    mouse_drag_left=None,
+    mouse_drag_right=None,
+    mouse_scroll=None,
+    key_press=None,
+    draw=None,
+    resize=None,
 ):
     @F.window.event
+    def on_mouse_press(x, y, button, modifiers):
+        if button == pyglet.window.mouse.LEFT and mouse_press_left:
+            mouse_press_left(x, y)
+        if button == pyglet.window.mouse.RIGHT and mouse_press_right:
+            mouse_press_right(x, y)
+
+    @F.window.event
+    def on_mouse_release(x, y, button, modifiers):
+        if button == pyglet.window.mouse.LEFT and mouse_release_left:
+            mouse_release_left(x, y)
+        if button == pyglet.window.mouse.RIGHT and mouse_release_right:
+            mouse_release_right(x, y)
+
+    @F.window.event
     def on_mouse_drag(x, y, dx, dy, buttons, modifiers):
-        mouse_drag(dx, dy)
+        if buttons & pyglet.window.mouse.LEFT and mouse_drag_left:
+            mouse_drag_left(x, y, dx, dy)
+        if buttons & pyglet.window.mouse.RIGHT and mouse_drag_right:
+            mouse_drag_right(x, y, dx, dy)
 
     @F.window.event
     def on_mouse_scroll(x, y, scroll_x, scroll_y):
-        mouse_scroll(x, y, scroll_y)
+        if mouse_scroll:
+            mouse_scroll(x, y, scroll_y)
 
     @F.window.event
     def on_key_press(symbol, modifiers):
-        if 32 <= symbol < 127:
-            key = chr(symbol)
-        else:
-            key = {
-                pyglet.window.key.LEFT  : 'Left',
-                pyglet.window.key.RIGHT : 'Right',
-                pyglet.window.key.UP    : 'Up',
-                pyglet.window.key.DOWN  : 'Down',
-                pyglet.window.key.SPACE : 'Space',
-                pyglet.window.key.RETURN: 'Return',
-            }.get(symbol)
-        if key: key_press(key)
+        if key_press:
+            if 32 <= symbol < 127:
+                key = chr(symbol)
+            else:
+                key = {
+                    pyglet.window.key.LEFT  : 'Left',
+                    pyglet.window.key.RIGHT : 'Right',
+                    pyglet.window.key.UP    : 'Up',
+                    pyglet.window.key.DOWN  : 'Down',
+                    pyglet.window.key.SPACE : 'Space',
+                    pyglet.window.key.RETURN: 'Return',
+                }.get(symbol)
+            if key: key_press(key)
 
     @F.window.event
     def on_draw():
         gl.glUseProgram(F.program)
         gl.glUniform2f(F.locations['uOrigin'], *F.origin)
         gl.glUniform2f(F.locations['uZoom'  ], *F.zoom)
-        draw()
+        if draw:
+            draw()
 
     @F.window.event
     def on_resize(width, height):
-        resize(width, height)
+        if resize:
+            resize(width, height)
 
 def run():
     gl.glEnable(gl.GL_BLEND);
     gl.glBlendFunc(gl.GL_SRC_ALPHA, gl.GL_ONE_MINUS_SRC_ALPHA);
     pyglet.app.run()
```

### Comparing `dansplotcore-6.5.0/dansplotcore/plot.py` & `dansplotcore-6.6.0/dansplotcore/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 from . import primitives
 from . import transforms
 from . import vector_text
 
 import datetime
 import math
 
+class Variable:
+    def __init__(self, name, x, y, x_var, y_var, home=None):
+        self.name = name
+        self.x_var = x_var
+        self.y_var = y_var
+        self.x = x
+        self.y = y
+        self.home = home
+
+    def __call__(self):
+        if self.x_var and self.y_var:
+            return (self.x, self.y)
+        if self.x_var:
+            return self.x
+        if self.y_var:
+            return self.y
+
 class Plot:
     def __init__(
         self,
         title='plot',
         *,
         transform=None,
         hide_axes=False,
@@ -36,14 +53,15 @@
         self.hide_axes = hide_axes
         self.x_axis_transform = x_axis_transform
         self.y_axis_transform = y_axis_transform
         self.set_primitive(primitive or primitives.Point())
         self.datetime_unit = datetime_unit
         self.legend_displacement = legend_displacement
         self.legend_offset = legend_offset
+        self.variables = []
 
     def point(self, x, y, r=255, g=255, b=255, a=255):
         self.points.append([x, y, r, g, b, a])
         self._include(x, y)
 
     def line(self, xi, yi, xf, yf, r=255, g=255, b=255, a=255):
         self.lines.append([xi, yi, xf, yf, r, g, b, a])
@@ -67,14 +85,19 @@
     def text_static(self, s, x, y, w=1, h=1, r=255, g=255, b=255, a=255):
         '`w` and `h` are for a single character.'
         if not s: return
         self.static_texter.text(s, x, y, w, h, r, g, b, a)
         self._include(*self.static_texter.bounds[0:2])
         self._include(*self.static_texter.bounds[2:4])
 
+    def variable(self, name, x, y, dims='xy', home=None):
+        var = Variable(name, x, y, 'x' in dims, 'y' in dims, home)
+        self.variables.append(var)
+        return var
+
     def show(self, w=640, h=480):
         from .show import show
         show(self, w, h)
 
     def plot_list(self, l, **kwargs):
         for i, v in enumerate(l):
             self.primitive(**self.transform(i, v, i, self.series))
```

### Comparing `dansplotcore-6.5.0/dansplotcore/primitives.py` & `dansplotcore-6.6.0/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.5.0/dansplotcore/process.py` & `dansplotcore-6.6.0/dansplotcore/process.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.5.0/dansplotcore/show.py` & `dansplotcore-6.6.0/dansplotcore/show.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         translate_y_date(plot, plot.rects, 1)
         translate_y_date(plot, plot.rects, 3)
         plot.y_max = max(plot.y_max, (plot.epochs['y']['max'] - plot.epochs['y']['min']).total_seconds() / plot.datetime_unit)
         plot.y_min = min(plot.y_min, 0)
 
 def construct(plot, view, w, h):
     plot.buffer = media.Buffer()
-    plot.buffer_text = media.Buffer()
+    plot.buffer_dyn = media.Buffer()
     # late vertexors
     if plot.late_vertexors:
         if hasattr(plot, 'original_points'):
             plot.points = copy.copy(plot.original_points)
             plot.lines = copy.copy(plot.original_lines)
         else:
             plot.original_points = copy.copy(plot.points)
@@ -141,22 +141,38 @@
         if plot.late_vertexors:
             construct(plot, view, media.width(), media.height())
     def square(view):
         view.w = view.h * media.width() / media.height()
         media.view_set(*view.tuple())
         if plot.late_vertexors:
             construct(plot, view, media.width(), media.height())
+    class VarChanger:
+        var = None
     reset()
     construct(plot, view, w, h)
     def on_resize(w, h):
         zoom(view, w/media.width(), h/media.height(), w/2, h/2)
         if plot.late_vertexors:
             construct(plot, view, media.width(), media.height())
-    def on_mouse_drag(dx, dy):
+    def on_mouse_press_right(x, y):
+        for var in plot.variables:
+            if abs((var.x - view.x) / view.w * media.width() - x) > 5:
+                continue
+            if abs((var.y - view.y) / view.h * media.height() - y) > 5:
+                continue
+            VarChanger.var = var
+            break
+    def on_mouse_release_right(x, y):
+        VarChanger.var = None
+    def on_mouse_drag_left(x, y, dx, dy):
         move(view, dx, dy)
+    def on_mouse_drag_right(x, y, dx, dy):
+        if var := VarChanger.var:
+            var.x += dx * view.w / media.width()
+            var.y += dy * view.h / media.height()
     def on_mouse_scroll(x, y, delta):
         z = 1.25 if delta > 0 else 0.8
         zoom(view, z, z, x, y)
     def on_key_press(key):
         moves = {
             'Left' : ( 10,   0),
             'Right': (-10,   0),
@@ -185,16 +201,17 @@
             square(view)
             return
     def on_draw():
         media.clear()
         plot.buffer.draw()
         margin_x = 5.0 / media.width()  * view.w
         margin_y = 5.0 / media.height() * view.h
-        # draw texts
         texter = media.Texter()
+        plot.buffer_dyn.clear()
+        # draw texts
         for (s, x, y, r, g, b, a, max_w, max_h, scale) in plot.texts:
             text_w = scale / media.width()  * view.w
             text_h = scale * 3/2 / media.height() * view.h
             over = max(len(s) * text_w / max_w, text_h * 3 / 2 / max_h, 1)
             r, g, b, a = fcolor(r, g, b, a)
             texter.text(
                 s, x + margin_x / over, y + margin_y / over,
@@ -204,14 +221,37 @@
             )
             texter.text(
                 'L', x, y,
                 text_w / over,
                 text_h / 2 / over,
                 r, g, b, a,
             )
+        # draw variables
+        text_w = 10 / media.width()  * view.w
+        text_h = 15 / media.height() * view.h
+        for var in plot.variables:
+            texter.text(
+                var.name, var.x + margin_x, var.y + margin_y,
+                text_w,
+                text_h,
+            )
+            plot.buffer_dyn.add(var.x - margin_x, var.y, 1.0, 1.0, 1.0, 1.0)
+            plot.buffer_dyn.add(var.x + margin_x, var.y, 1.0, 1.0, 1.0, 1.0)
+            plot.buffer_dyn.add(var.x, var.y - margin_y, 1.0, 1.0, 1.0, 1.0)
+            plot.buffer_dyn.add(var.x, var.y + margin_y, 1.0, 1.0, 1.0, 1.0)
+            if var.x_var:
+                plot.buffer_dyn.add(var.x, view.y - view.h, 1.0, 1.0, 1.0, 0.2)
+                plot.buffer_dyn.add(var.x, view.y + view.h, 1.0, 1.0, 1.0, 0.2)
+            if var.y_var:
+                plot.buffer_dyn.add(view.x - view.w, var.y, 1.0, 1.0, 1.0, 0.2)
+                plot.buffer_dyn.add(view.x + view.w, var.y, 1.0, 1.0, 1.0, 0.2)
+            if var.home:
+                plot.buffer_dyn.add(var.x, var.y, 1.0, 1.0, 1.0, 0.2)
+                x, y = var.home
+                plot.buffer_dyn.add(x, y, 1.0, 1.0, 1.0, 0.2)
         if not plot.hide_axes:
             text_w = 10 / media.width()  * view.w
             text_h = 15 / media.height() * view.h
             # draw x axis
             increment = 10 ** math.floor(math.log10(view.w))
             if view.w / increment < 2:
                 increment /= 5
@@ -258,19 +298,22 @@
                         w=text_w * 0.66,
                         h=text_h * 0.66,
                     )
                 else:
                     texter.text(s, x=view.x+margin_x, y=i+margin_y, w=text_w, h=text_h)
                 texter.text('L', view.x, i, text_w * 2, text_h)
                 i += increment
-        plot.buffer_text.data = texter.data
-        plot.buffer_text.prep('dynamic')
-        plot.buffer_text.draws = [('lines', 0, len(plot.buffer_text.data))]
-        plot.buffer_text.draw()
+        plot.buffer_dyn.add_data(texter.data)
+        plot.buffer_dyn.prep('dynamic')
+        plot.buffer_dyn.draws = [('lines', 0, len(plot.buffer_dyn.data))]
+        plot.buffer_dyn.draw()
     media.set_callbacks(
-        mouse_drag=on_mouse_drag,
+        mouse_press_right=on_mouse_press_right,
+        mouse_release_right=on_mouse_release_right,
+        mouse_drag_left=on_mouse_drag_left,
+        mouse_drag_right=on_mouse_drag_right,
         mouse_scroll=on_mouse_scroll,
         key_press=on_key_press,
         draw=on_draw,
         resize=on_resize,
     )
     media.run()
```

### Comparing `dansplotcore-6.5.0/dansplotcore/transforms.py` & `dansplotcore-6.6.0/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.5.0/dansplotcore/vector_text.py` & `dansplotcore-6.6.0/dansplotcore/vector_text.py`

 * *Files identical despite different names*

