# Comparing `tmp/dash_spread_grid-0.0.8.tar.gz` & `tmp/dash_spread_grid-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_spread_grid-0.0.8.tar", last modified: Sun Apr  7 17:49:21 2024, max compression
+gzip compressed data, was "dash_spread_grid-0.0.9.tar", last modified: Tue Apr  9 17:54:55 2024, max compression
```

## Comparing `dash_spread_grid-0.0.8.tar` & `dash_spread_grid-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-04-07 17:49:21.330875 dash_spread_grid-0.0.8/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.0.8/LICENSE
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.0.8/MANIFEST.in
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-04-07 17:49:21.330875 dash_spread_grid-0.0.8/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.0.8/README.md
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-04-07 17:49:21.330875 dash_spread_grid-0.0.8/dash_spread_grid/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3272 2024-04-07 17:49:21.000000 dash_spread_grid-0.0.8/dash_spread_grid/DashSpreadGrid.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.0.8/dash_spread_grid/__init__.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-04-07 17:49:21.000000 dash_spread_grid-0.0.8/dash_spread_grid/_imports_.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    51010 2024-04-07 17:49:20.000000 dash_spread_grid-0.0.8/dash_spread_grid/dash_spread_grid.min.js
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   196712 2024-04-07 17:49:20.000000 dash_spread_grid-0.0.8/dash_spread_grid/dash_spread_grid.min.js.map
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6042 2024-04-07 17:49:21.000000 dash_spread_grid-0.0.8/dash_spread_grid/metadata.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2332 2024-04-07 17:49:20.000000 dash_spread_grid-0.0.8/dash_spread_grid/package-info.json
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-04-07 17:49:21.330875 dash_spread_grid-0.0.8/dash_spread_grid.egg-info/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-04-07 17:49:21.000000 dash_spread_grid-0.0.8/dash_spread_grid.egg-info/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-04-07 17:49:21.000000 dash_spread_grid-0.0.8/dash_spread_grid.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-04-07 17:49:21.000000 dash_spread_grid-0.0.8/dash_spread_grid.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-04-07 17:49:21.000000 dash_spread_grid-0.0.8/dash_spread_grid.egg-info/top_level.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2332 2024-04-07 17:49:09.000000 dash_spread_grid-0.0.8/package.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-04-07 17:49:21.330875 dash_spread_grid-0.0.8/setup.cfg
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.0.8/setup.py
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.0.9/LICENSE
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.0.9/MANIFEST.in
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.0.9/README.md
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/dash_spread_grid/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3272 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid/DashSpreadGrid.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.0.9/dash_spread_grid/__init__.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid/_imports_.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    51727 2024-04-09 17:54:53.000000 dash_spread_grid-0.0.9/dash_spread_grid/dash_spread_grid.min.js
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   199999 2024-04-09 17:54:53.000000 dash_spread_grid-0.0.9/dash_spread_grid/dash_spread_grid.min.js.map
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6042 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid/metadata.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2332 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid/package-info.json
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/top_level.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2332 2024-04-09 17:54:43.000000 dash_spread_grid-0.0.9/package.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/setup.cfg
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.0.9/setup.py
```

### Comparing `dash_spread_grid-0.0.8/README.md` & `dash_spread_grid-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.0.8/dash_spread_grid/DashSpreadGrid.py` & `dash_spread_grid-0.0.9/dash_spread_grid/DashSpreadGrid.py`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.0.8/dash_spread_grid/__init__.py` & `dash_spread_grid-0.0.9/dash_spread_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.0.8/dash_spread_grid/dash_spread_grid.min.js` & `dash_spread_grid-0.0.9/dash_spread_grid/dash_spread_grid.min.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
                 __webpack_require__.d(__webpack_exports__, {
                     Z: () => __WEBPACK_DEFAULT_EXPORT__
                 });
                 var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(196),
                     react__WEBPACK_IMPORTED_MODULE_0___default = __webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__),
                     prop_types__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(64),
                     prop_types__WEBPACK_IMPORTED_MODULE_1___default = __webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_1__),
-                    js_spread_grid__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(462);
+                    js_spread_grid__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(713);
 
                 function _typeof(e) {
                     return _typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     }, _typeof(e)
@@ -280,15 +280,15 @@
             },
             64: e => {
                 e.exports = window.PropTypes
             },
             196: e => {
                 e.exports = window.React
             },
-            462: (e, t, o) => {
+            713: (e, t, o) => {
                 function n(e) {
                     return null === e ? "null" : Array.isArray(e) ? `[${e.map(n).join(",")}]` : "object" == typeof e ? (t = e, `{${Object.keys(t).sort().map((e=>`${e}:${n(t[e])}`)).join(",")}}`) : JSON.stringify(e);
                     var t
                 }
 
                 function r(e, t) {
                     return "FILTER" === e.type ^ "FILTER" === t.type ? "FILTER" : "DATA" === e.type && "DATA" === t.type ? "DATA" : "OTHER"
@@ -306,15 +306,15 @@
                             edit: t.resolve(c, a).edit,
                             cell: e,
                             type: r(a, c)
                         }
                     })).filter((e => e?.edit))
                 }
                 o.d(t, {
-                    Z: () => Ke
+                    Z: () => We
                 });
                 const l = "12px Calibri",
                     s = {
                         top: 2,
                         right: 5,
                         bottom: 2,
                         left: 5
@@ -345,30 +345,30 @@
                         y = s.showLeftBorder,
                         w = s.showRightBorder,
                         b = m / 2,
                         E = u.length - 1 + (_ ? 1 : 0) + (g ? 1 : 0),
                         v = c.length - 1 + (y ? 1 : 0) + (w ? 1 : 0),
                         x = u.map((e => e.height)),
                         R = c.map((e => e.width)),
-                        A = R.reduce(((e, t) => e + t), 0) + v * m,
-                        C = x.reduce(((e, t) => e + t), 0) + E * m,
+                        C = R.reduce(((e, t) => e + t), 0) + v * m,
+                        A = x.reduce(((e, t) => e + t), 0) + E * m,
                         k = "center" === o ? p.left : 0,
                         I = "middle" === t ? p.top : 0,
                         D = "center" === o ? p.width : s.width,
                         M = "middle" === t ? p.height : i.height,
-                        O = R.reduce(((e, t, o) => {
+                        T = R.reduce(((e, t, o) => {
                             const n = e[o] + t + m;
                             return e.push(n), e
                         }), [y ? m : 0]),
-                        T = x.reduce(((e, t, o) => {
+                        O = x.reduce(((e, t, o) => {
                             const n = e[o] + t + m;
                             return e.push(n), e
                         }), [_ ? m : 0]),
-                        L = O.slice(0, -1),
-                        P = T.slice(0, -1),
+                        L = T.slice(0, -1),
+                        P = O.slice(0, -1),
                         B = Math.max(L.findLastIndex((e => e <= k)), 0),
                         S = L.findLastIndex((e => e <= k + D)),
                         K = Math.max(P.findLastIndex((e => e <= I)), 0),
                         W = P.findLastIndex((e => e <= I + M)),
                         F = Math.max(B, y ? 0 : 1),
                         N = S + (w ? 1 : 0),
                         z = Math.max(K, _ ? 0 : 1),
@@ -381,28 +381,28 @@
                                 length: S - B + 1
                             }, ((e, t) => {
                                 const n = c[t + B];
                                 return f.resolve(o, n)
                             }))
                         })),
                         H = (e, t) => j[e - K][t - B];
-                    r.width = Math.round(D * devicePixelRatio), r.height = Math.round(M * devicePixelRatio), r.style.width = `${D}px`, r.style.height = `${M}px`, r.style.marginLeft = `${k}px`, r.style.marginTop = `${I}px`, r.style.marginRight = A - D - k + "px", r.style.marginBottom = C - M - I + "px", d.fillStyle = "#E9E9E9", d.fillRect(0, 0, r.width, r.height);
+                    r.width = Math.round(D * devicePixelRatio), r.height = Math.round(M * devicePixelRatio), r.style.width = `${D}px`, r.style.height = `${M}px`, r.style.marginLeft = `${k}px`, r.style.marginTop = `${I}px`, r.style.marginRight = C - D - k + "px", r.style.marginBottom = A - M - I + "px", d.fillStyle = "#E9E9E9", d.fillRect(0, 0, r.width, r.height);
                     const q = (e, t) => {
                             d.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (e - k) * devicePixelRatio, (t - I) * devicePixelRatio)
                         },
                         $ = (e, t, o, n) => {
                             d.beginPath(), d.rect(e, t, o, n), d.clip()
                         };
                     for (let e = B; e <= S; e++) {
-                        d.save(), q(O[e], 0), $(0, 0, R[e], C);
+                        d.save(), q(T[e], 0), $(0, 0, R[e], A);
                         for (let t = K; t <= W; t++) {
                             const o = H(t, e),
                                 n = o.style,
-                                r = T[t],
-                                i = O[e],
+                                r = O[t],
+                                i = T[e],
                                 s = R[e],
                                 c = x[t],
                                 u = o.text,
                                 p = n.textAlign || "left",
                                 f = n.textBaseline || "middle",
                                 _ = o.padding;
                             q(i, r), d.fillStyle = n.background || "white", d.fillRect(0, 0, s, c), "draw" in o && o.draw(d), n.highlight && (d.fillStyle = n.highlight, d.fillRect(0, 0, s, c)), n.corner && (d.fillStyle = n.corner, d.beginPath(), d.moveTo(s - 7, c), d.lineTo(s, c), d.lineTo(s, c - 7), d.fill()), d.fillStyle = n.foreground || "black", d.font = n.font || l, d.textAlign = p;
@@ -426,23 +426,23 @@
                         },
                         G = (e, t) => e ? t ? e.index > t.index ? e : t : e : t;
                     for (let e = z; e <= U; e++) {
                         const t = e - 1,
                             o = e;
                         for (let e = B; e <= S; e++) {
                             const n = G(t >= K ? H(t, e).style.borderBottom : null, o <= W ? H(o, e).style.borderTop : null);
-                            V(O[e] - b, T[o] - b, O[e + 1] - b, T[o] - b, n)
+                            V(T[e] - b, O[o] - b, T[e + 1] - b, O[o] - b, n)
                         }
                     }
                     for (let e = F; e <= N; e++) {
                         const t = e - 1,
                             o = e;
                         for (let e = K; e <= W; e++) {
                             const n = G(t >= B ? H(e, t).style.borderRight : null, o <= S ? H(e, o).style.borderLeft : null);
-                            V(O[o] - b, T[e] - b, O[o] - b, T[e + 1] - b, n)
+                            V(T[o] - b, O[e] - b, T[o] - b, O[e + 1] - b, n)
                         }
                     }
                 }
 
                 function u(e) {
                     if (!e.error) try {
                         ! function(e) {
@@ -950,26 +950,26 @@
                     }) => [n(e), t])));
                     return x(e, t, o).map((e => ({
                         ...e,
                         width: i.has(e.key) ? i.get(e.key) : e.width
                     })))
                 }
 
-                function A(e, t, o, r) {
+                function C(e, t, o, r) {
                     const i = new Map(r.map((({
                         rowId: e,
                         height: t
                     }) => [n(e), t])));
                     return x(e, t, o).map((e => ({
                         ...e,
                         height: i.has(e.key) ? i.get(e.key) : e.height
                     })))
                 }
 
-                function C(e, t, o) {
+                function A(e, t, o) {
                     let n = o;
                     return e.map(((e, r) => {
                         const i = a("width" in e ? e.width : 100, t),
                             l = {
                                 ...e,
                                 index: r,
                                 width: i,
@@ -1056,31 +1056,35 @@
                             for (const o of t.labels) e.byLabel.has(o) && n(e.byLabel.get(o))
                         }
                         this.lookup.byKey.has(e.key) && r(this.lookup.byKey.get(e.key)), this.lookup.byIndex.has(e.index) && r(this.lookup.byIndex.get(e.index)), this.lookup.byMatch.has(e.type) && r(this.lookup.byMatch.get(e.type));
                         for (const t of e.labels) this.lookup.byLabel.has(t) && r(this.lookup.byLabel.get(t));
                         return o
                     }
                 }
-                const O = ["borderTop", "borderRight", "borderBottom", "borderLeft"];
+                const T = ["borderTop", "borderRight", "borderBottom", "borderLeft"],
+                    O = {
+                        validate: () => !0,
+                        parse: e => e
+                    };
 
-                function T(e, t) {
+                function L(e, t) {
                     const o = {
                         ...e
                     };
                     if ("border" in o) {
-                        for (const e of O) o[e] = o.border;
+                        for (const e of T) o[e] = o.border;
                         delete o.border
                     }
-                    for (const e of O) e in o && (o[e] = {
+                    for (const e of T) e in o && (o[e] = {
                         ...o[e],
                         index: t
                     });
                     return o
                 }
-                class L {
+                class P {
                     constructor(e) {
                         this.rulesLookup = new M;
                         for (const [t, o] of e.entries()) {
                             const e = {
                                 index: t
                             };
                             "condition" in o && (e.condition = o.condition), "style" in o && (e.style = "function" == typeof o.style ? o.style : () => o.style), "value" in o && (e.value = "function" == typeof o.value ? o.value : () => o.value), "text" in o && (e.text = "function" == typeof o.text ? o.text : () => o.text), "padding" in o && (e.padding = "function" == typeof o.padding ? o.padding : () => o.padding), "edit" in o && (e.edit = o.edit), "draw" in o && (e.draw = o.draw), this.rulesLookup.addRule(o.column, o.row, e)
@@ -1103,113 +1107,119 @@
                         });
                         for (const e of l)
                             if ((!("condition" in e) || e.condition(c)) && ("value" in e && (c = {
                                     ...c,
                                     value: e.value(c)
                                 }), "style" in e && (u = {
                                     ...u,
-                                    ...T(e.style(c), e.index)
+                                    ...L(e.style(c), e.index)
                                 }), "text" in e && (c = {
                                     ...c,
                                     text: e.text(c)
                                 }), "padding" in e && (d = {
                                     ...d,
                                     ...e.padding(c)
                                 }), "edit" in e && (c = {
                                     ...c,
                                     edit: e.edit && "edit" in c ? {
                                         ...c.edit,
                                         ...e.edit
-                                    } : e.edit
+                                    } : {
+                                        ...O,
+                                        ...e.edit
+                                    }
                                 }), "draw" in e)) {
                                 const t = c;
                                 a = o => e.draw({
                                     ...t,
                                     ctx: o
                                 })
-                            } const p = {
-                            style: u,
-                            visible: !0,
-                            text: "text" in c ? c.text : `${c.value}`,
-                            padding: d
-                        };
-                        return "value" in c && (p.value = c.value), "edit" in c && (p.edit = c.edit), void 0 !== a && (p.draw = a), "text" in c && (p.text = c.text), p
+                            } const p = function(e) {
+                                return "text" in e ? e.text : void 0 !== e.value ? `${e.value}` : ""
+                            }(c),
+                            h = {
+                                style: u,
+                                visible: !0,
+                                text: p,
+                                padding: d
+                            };
+                        return "value" in c && (h.value = c.value), "edit" in c && (h.edit = c.edit), void 0 !== a && (h.draw = a), "text" in c && (h.text = c.text), h
                     }
                 }
 
-                function P(e) {
-                    return new L(e)
+                function B(e) {
+                    return new P(e)
                 }
-                class B {
+                class S {
                     constructor(e, t, o, n, r) {
                         this.formattingRules = e, this.data = t, this.rows = o, this.columns = n, this.edition = r
                     }
                     resolve(e, t) {
                         return this.formattingRules.resolve(this.data, this.rows, this.columns, e, t, this.edition)
                     }
                 }
 
-                function S(e, t, o, n, r) {
-                    return new B(e, t, o, n, r)
+                function K(e, t, o, n, r) {
+                    return new S(e, t, o, n, r)
                 }
 
-                function K(e, t, o) {
+                function W(e, t, o) {
                     const r = new Map;
                     for (const i of e) {
                         const e = n(i[t]),
                             l = n(i[o]);
                         r.has(e) || r.set(e, new Map), r.get(e).set(l, i.expression)
                     }
                     return r
                 }
 
-                function W(e, t, o, n, r, i, l) {
+                function F(e, t, o, n, r, i, l) {
                     if (0 === e.length) return r;
-                    const s = K(e, "columnId", "rowId"),
+                    const s = W(e, "columnId", "rowId"),
                         a = i.filter((e => "FILTER" !== e.type && s.has(e.key)));
                     return 0 === a.length ? r : r.filter((e => {
                         for (const c of a) {
                             const a = o.resolve(n, r, i, e, c, l),
                                 u = s.get(c.key);
                             if (!t.resolve(n, r, i, e, c, a.value, a.text, u)) return !1
                         }
                         return !0
                     }))
                 }
 
-                function F(e, t, o, n, r, i, l) {
+                function N(e, t, o, n, r, i, l) {
                     if (0 === e.length) return i;
-                    const s = K(e, "rowId", "columnId"),
+                    const s = W(e, "rowId", "columnId"),
                         a = r.filter((e => "FILTER" !== e.type && s.has(e.key)));
                     return 0 === a.length ? i : i.filter((e => {
                         for (const c of a) {
                             const a = o.resolve(n, r, i, c, e, l),
                                 u = s.get(c.key);
                             if (!t.resolve(n, r, i, c, e, a.value, a.text, u)) return !1
                         }
                         return !0
                     }))
                 }
 
-                function N(e, t, o, n) {
+                function z(e, t, o, n) {
                     return {
                         top: e,
                         bottom: t,
                         left: o,
                         right: n
                     }
                 }
 
-                function z(e, t) {
+                function U(e, t) {
                     return {
                         width: e.length ? e.at(-1).rightWithBorder : 0,
                         height: t.length ? t.at(-1).bottomWithBorder : 0
                     }
                 }
-                class U {
+                class j {
                     constructor() {
                         this.canvas = document.createElement("canvas"), this.context = this.canvas.getContext("2d"), this.fontMetrics = new Map
                     }
                     measureWidth(e, t) {
                         const o = this.context;
                         return o.font = t || l, o.measureText(e).width
                     }
@@ -1231,72 +1241,72 @@
                                 bottomOffset: n.fontBoundingBoxDescent - r,
                                 height: n.fontBoundingBoxAscent + n.fontBoundingBoxDescent
                             };
                         return this.fontMetrics.set(t, i), i
                     }
                 }
 
-                function j() {
-                    return new U
+                function H() {
+                    return new j
                 }
 
-                function H(e, t) {
+                function q(e, t) {
                     return t.top >= e.top && t.left >= e.left && t.top + t.height <= e.top + e.height && t.left + t.width <= e.left + e.width
                 }
 
-                function q(e, t) {
+                function $(e, t) {
                     const o = {
                         top: Math.max(e.top, t.top),
                         left: Math.max(e.left, t.left),
                         width: Math.min(e.left + e.width, t.left + t.width) - Math.max(e.left, t.left),
                         height: Math.min(e.top + e.height, t.top + t.height) - Math.max(e.top, t.top)
                     };
                     return o.width >= 0 && o.height >= 0 ? o : {
                         top: e.top,
                         left: e.left,
                         width: 0,
                         height: 0
                     }
                 }
 
-                function $(e, t) {
+                function V(e, t) {
                     return {
                         top: e.top - t,
                         left: e.left - t,
                         width: e.width + 2 * t,
                         height: e.height + 2 * t
                     }
                 }
 
-                function V(e) {
+                function G(e) {
                     return e.width * e.height
                 }
 
-                function G(e, t) {
+                function Y(e, t) {
                     return {
                         top: e.top,
                         left: e.left,
                         width: Math.max(0, e.width - t.left - t.right),
                         height: Math.max(0, e.height - t.top - t.bottom)
                     }
                 }
-                const Y = 200,
-                    X = 400,
-                    Z = {
+                const X = 200,
+                    Z = 400,
+                    J = {
                         left: 0,
                         top: 0,
                         width: 0,
                         height: 0
                     };
 
-                function J(e) {
+                function Q(e) {
                     return e.reduce(((e, t) => e.set(t.key, t)), new Map)
                 }
 
-                function Q(e, t, o, r, i, l, s, a) {
+                function ee(e, t, o, r, i, l, s, a) {
                     if (!e) return [];
                     if (t) return [];
                     if (!r) return [];
                     if (!o) return [];
                     const c = n(o.columnId),
                         u = n(o.rowId),
                         d = n(r.columnId),
@@ -1311,37 +1321,37 @@
                         _ = Math.max(a.get(u).index, a.get(p).index);
                     return i.slice(h, f + 1).flatMap((e => l.slice(m, _ + 1).map((t => ({
                         rowId: t.id,
                         columnId: e.id
                     })))))
                 }
 
-                function ee(e, t) {
+                function te(e, t) {
                     const o = function(e) {
                             return "BEGIN" === e.pinned ? "top" : "END" === e.pinned ? "bottom" : "middle"
                         }(t),
                         n = function(e) {
                             return "BEGIN" === e.pinned ? "left" : "END" === e.pinned ? "right" : "center"
                         }(e);
                     return `${o}-${n}`
                 }
 
-                function te(e, t, o, r, i) {
+                function oe(e, t, o, r, i) {
                     if (!t) return null;
                     const l = n(t.columnId),
                         s = n(t.rowId);
                     if (!o.has(l)) return null;
                     if (!r.has(s)) return null;
                     const a = o.get(l),
                         c = r.get(s);
                     if (0 === e.length) return null;
                     const u = {
                         width: a.width,
                         height: c.height,
-                        section: ee(a, c)
+                        section: te(a, c)
                     };
                     switch (c.pinned) {
                         case "BEGIN":
                             u.top = c.top;
                             break;
                         case "END":
                             u.bottom = i.top.height + i.middle.height + i.bottom.height - c.top - c.height;
@@ -1358,83 +1368,86 @@
                             break;
                         default:
                             u.marginLeft = a.left - i.left.width
                     }
                     return u
                 }
 
-                function oe(e, t) {
+                function ne(e, t) {
                     return t.every((t => t.edit.validate({
                         string: e
                     })))
                 }
 
-                function ne(e) {
+                function re(e) {
                     return Array.isArray(e) ? e.map(((e, t) => t)) : Object.keys(e)
                 }
 
-                function re(e) {
-                    return ne(e)
+                function ie(e) {
+                    return re(e)
                 }
 
-                function ie(e) {
-                    if (Array.isArray(e)) return e.length > 0 ? Object.keys(e[0]) : [];
-                    {
-                        const t = Object.keys(e);
-                        return t.length > 0 ? ne(e[t[0]]) : []
-                    }
+                function le(e) {
+                    const t = new Set;
+                    if (Array.isArray(e))
+                        for (const o of e)
+                            for (const e of re(o)) t.add(e);
+                    else
+                        for (const o in e)
+                            for (const n of re(e[o])) t.add(n);
+                    return [...t]
                 }
 
-                function le(e, t) {
+                function se(e, t) {
                     if (!e.some((e => "DATA-BLOCK" === e.type))) return e;
                     const o = [];
                     for (const n of e)
                         if ("DATA-BLOCK" === n.type) {
-                            const e = "selector" in n ? n.selector(t) : ie(t);
+                            const e = "selector" in n ? n.selector(t) : le(t);
                             for (const t of e) o.push({
                                 ...n,
                                 id: t,
                                 type: "DATA"
                             })
                         } else o.push(n);
                     return o
                 }
 
-                function se(e, t) {
+                function ae(e, t) {
                     if (!e.some((e => "DATA-BLOCK" === e.type))) return e;
                     const o = [];
                     for (const n of e)
                         if ("DATA-BLOCK" === n.type) {
-                            const e = "selector" in n ? n.selector(t) : re(t);
+                            const e = "selector" in n ? n.selector(t) : ie(t);
                             for (const t of e) o.push({
                                 ...n,
                                 id: t,
                                 type: "DATA"
                             })
                         } else o.push(n);
                     return o
                 }
-                const ae = ({
+                const ce = ({
                     text: e,
                     expression: t
                 }) => e.includes(t);
-                class ce {
+                class ue {
                     constructor(e) {
                         this.rulesLookup = new M;
                         for (const t of e) {
                             const e = {
                                 by: n("by" in t ? t.by : "FILTER"),
-                                condition: t.condition || ae
+                                condition: t.condition || ce
                             };
                             this.rulesLookup.addRule(t.column, t.row, e)
                         }
                     }
                     resolve(e, t, o, n, r, i, l, s) {
                         const a = this.rulesLookup.getRules(r, n);
-                        if (0 === a.length) return "DATA" !== n.type || "DATA" !== r.type || !s.has('"FILTER"') || ae({
+                        if (0 === a.length) return "DATA" !== n.type || "DATA" !== r.type || !s.has('"FILTER"') || ce({
                             text: l,
                             expression: s.get('"FILTER"')
                         });
                         let c = {
                             data: e,
                             rows: t,
                             columns: o,
@@ -1451,27 +1464,27 @@
                             };
                             if (!e.condition(t)) return !1
                         }
                         return !0
                     }
                 }
 
-                function ue(e) {
-                    return new ce(e)
+                function de(e) {
+                    return new ue(e)
                 }
 
-                function de(e) {
+                function pe(e) {
                     return e
                 }
 
-                function pe(e) {
+                function he(e) {
                     return e
                 }
 
-                function he(e, t, o, n, r, i) {
+                function fe(e, t, o, n, r, i) {
                     if (e.every((e => "number" == typeof e.width))) return e;
                     const l = e => {
                         const i = "width" in e ? e.width : "fit-once";
                         if ("number" == typeof i) return i;
                         if (r.has(e.key)) {
                             const t = r.get(e.key);
                             if ("fit-once" === i && !t.dataOnly) return t.width;
@@ -1496,15 +1509,15 @@
                     for (const e of r.keys()) i.has(e) || r.delete(e);
                     return e.map((e => ({
                         ...e,
                         width: l(e)
                     })))
                 }
 
-                function fe(e, t, o, n, r, i) {
+                function me(e, t, o, n, r, i) {
                     if (t.every((e => "number" == typeof e.height))) return t;
                     const l = t => {
                         const i = "height" in t ? t.height : "fit-once";
                         if ("number" == typeof i) return i;
                         if (r.has(t.key)) {
                             const e = r.get(t.key);
                             if ("fit-once" === i && !e.dataOnly) return e.height;
@@ -1529,153 +1542,159 @@
                     for (const e of r.keys()) i.has(e) || r.delete(e);
                     return t.map((e => ({
                         ...e,
                         height: l(e)
                     })))
                 }
 
-                function me(e) {
+                function _e(e) {
                     return new Set(e.map((e => e.key)))
                 }
 
-                function _e(e) {
+                function ge(e) {
                     return e
                 }
-                const ge = (e, t) => e.value < t.value,
-                    ye = (e, t) => e.value > t.value;
-                class we {
+
+                function ye(e, t) {
+                    return null != e.value && (null == t.value || e.value < t.value)
+                }
+
+                function we(e, t) {
+                    return null != e.value && (null == t.value || e.value > t.value)
+                }
+                class be {
                     constructor(e) {
                         this.rulesLookup = new M;
                         for (const t of e) {
                             const e = {
                                 by: stringifyId("by" in t ? t.by : "HEADER"),
-                                comparatorAsc: t.comparator || ge,
-                                comparatorDesc: (e, o) => -t.comparator(e, o) || ye
+                                comparatorAsc: t.comparator || ye,
+                                comparatorDesc: (e, o) => -t.comparator(e, o) || we
                             };
                             this.rulesLookup.addRule(t.column, t.row, e)
                         }
                     }
                     resolve(e, t, o) {
                         const n = this.rulesLookup.getRules(e, t);
-                        if (0 === n.length) return "DATA" !== t.type || "DATA" !== e.type ? null : o.has('"HEADER"') ? "ASC" === o.get('"HEADER"') ? ge : ye : null;
+                        if (0 === n.length) return "DATA" !== t.type || "DATA" !== e.type ? null : o.has('"HEADER"') ? "ASC" === o.get('"HEADER"') ? ye : we : null;
                         if (n.length > 1) throw new Error("Multiple sorting rules for the same cell");
                         const r = n[0];
                         return "ASC" === o.get(r.by) ? r.comparatorAsc : r.comparatorDesc
                     }
                 }
 
-                function be(e) {
-                    return new we(e)
+                function Ee(e) {
+                    return new be(e)
                 }
 
-                function Ee(e, t, o) {
+                function ve(e, t, o) {
                     const r = new Map;
                     for (const i of e) {
                         const e = n(i[t]),
                             l = n(i[o]);
                         r.has(e) || r.set(e, new Map), r.get(e).set(l, i.direction)
                     }
                     return r
                 }
 
-                function ve(e, t) {
+                function xe(e, t) {
                     e.sort(((e, t) => {
                         const o = e.comparator(e.cell, t.cell);
                         return "number" == typeof o ? o : o ? -1 : 1
                     })), t.push(...e.map((e => e.entity))), e.length = 0
                 }
 
-                function xe(e, t, o, r, i, l, s) {
+                function Re(e, t, o, r, i, l, s) {
                     if (0 === e.length) return i;
-                    const a = Ee(e, "columnId", "rowId"),
+                    const a = ve(e, "columnId", "rowId"),
                         c = new Map(l.map((e => [e.key, e]))),
                         u = e.map((e => n(e.columnId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
                     if (0 === u.length) return i;
                     for (const e of u) {
                         const n = [],
                             c = [];
                         for (const u of i) {
                             const d = t.resolve(e, u, a.get(e.key));
                             if (!d) {
-                                ve(c, n), n.push(u);
+                                xe(c, n), n.push(u);
                                 continue
                             }
                             const p = {
                                 entity: u,
                                 comparator: d,
                                 cell: o.resolve(r, i, l, u, e, s)
                             };
-                            0 !== c.length && c[0].comparator !== d ? (ve(c, n), c.push(p)) : c.push(p)
+                            0 !== c.length && c[0].comparator !== d ? (xe(c, n), c.push(p)) : c.push(p)
                         }
-                        ve(c, n), i = n
+                        xe(c, n), i = n
                     }
                     return i
                 }
 
-                function Re(e, t, o, r, i, l, s) {
+                function Ce(e, t, o, r, i, l, s) {
                     if (0 === e.length) return l;
-                    const a = Ee(e, "rowId", "columnId"),
+                    const a = ve(e, "rowId", "columnId"),
                         c = new Map(i.map((e => [e.key, e]))),
                         u = e.map((e => n(e.rowId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
                     if (0 === u.length) return l;
                     for (const e of u) {
                         const n = [],
                             c = [];
                         for (const u of l) {
                             const d = t.resolve(u, e, a.get(e.key));
                             if (!d) {
-                                ve(c, n), n.push(u);
+                                xe(c, n), n.push(u);
                                 continue
                             }
                             const p = {
                                 entity: u,
                                 comparator: d,
                                 cell: o.resolve(r, i, l, e, u, s)
                             };
-                            0 !== c.length && c[0].comparator !== d ? (ve(c, n), c.push(p)) : c.push(p)
+                            0 !== c.length && c[0].comparator !== d ? (xe(c, n), c.push(p)) : c.push(p)
                         }
-                        ve(c, n), l = n
+                        xe(c, n), l = n
                     }
                     return l
                 }
                 const Ae = 5;
 
-                function Ce(e, t, o, r, i) {
+                function ke(e, t, o, r, i) {
                     if (!r) return null;
                     const l = t.get(n(r.columnId)),
                         s = o.get(n(r.rowId)),
                         a = i.x;
                     return "HEADER" !== s.type ? null : a >= l.right - Ae && a <= l.right + Ae ? l.id : 0 === l.index || a < l.left - Ae || a > l.left + Ae ? null : e[l.index - 1].id
                 }
 
-                function ke(e, t, o, r, i) {
+                function Ie(e, t, o, r, i) {
                     if (!r) return null;
                     const l = t.get(n(r.columnId)),
                         s = o.get(n(r.rowId)),
                         a = i.y;
                     return "HEADER" !== l.type ? null : a >= s.bottom - Ae && a <= s.bottom + Ae ? s.id : 0 === s.index || a < s.top - Ae || a > s.top + Ae ? null : e[s.index - 1].id
                 }
 
-                function Ie(e) {
+                function De(e) {
                     return e.map((e => ({
                         columnId: "columnId" in e ? e.columnId : "HEADER",
                         rowId: "rowId" in e ? e.rowId : "HEADER",
                         direction: e.direction
                     })))
                 }
 
-                function De(e) {
+                function Me(e) {
                     return e.map((e => ({
                         columnId: "columnId" in e ? e.columnId : "FILTER",
                         rowId: "rowId" in e ? e.rowId : "FILTER",
                         expression: e.expression
                     })))
                 }
 
-                function Me(e, t) {
+                function Te(e, t) {
                     return function(e, t) {
                         const o = e.filter((e => "DATA" === e.type)).map((e => e.id));
                         return t(o), o
                     }(e, t)
                 }
 
                 function Oe(e) {
@@ -1694,54 +1713,54 @@
                             dependencies: n
                         }), o[e].value
                     }
                     const l = window.devicePixelRatio,
                         s = t.borderWidth / l,
                         a = t.data,
                         c = e.input.value,
-                        u = r("sortBy", Ie, [t.sortBy]),
-                        h = r("filters", De, [t.filters]),
-                        g = r("textResolver", j, []),
+                        u = r("sortBy", De, [t.sortBy]),
+                        h = r("filters", Me, [t.filters]),
+                        g = r("textResolver", H, []),
                         w = r("dataFormatting", d, [t.formatting, t.dataSelector, u]),
                         v = r("editedCellsAndFilters", _, [t.editedCells, h]),
                         x = r("edition", y, [v]),
                         I = r("invokedColumns", E, [t.columns, a]),
                         D = r("invokedRows", E, [t.rows, a]),
-                        M = r("unfoldedColumns", le, [I, a]),
-                        O = r("unfoldedRows", se, [D, a]),
-                        T = r("unfilteredColumns", R, [M, t.pinnedLeft, t.pinnedRight, t.columnWidths]),
-                        L = r("unfilteredRows", A, [O, t.pinnedTop, t.pinnedBottom, t.rowHeights]),
-                        B = r("unfilteredColumnKeys", me, [T]),
-                        K = r("unfilteredRowKeys", me, [L]),
-                        U = r("filterFormatting", de, [w]),
-                        ee = r("filterFormattingRules", P, [U]),
-                        ne = r("filteringRules", ue, [t.filtering]),
-                        re = r("filteredColumns", F, [h, ne, ee, a, L, T, x]),
-                        ie = r("filteredRows", W, [h, ne, ee, a, L, T, x]),
-                        ae = r("sortingFormatting", _e, [w]),
-                        ce = r("sortingFormattingRules", P, [ae]),
-                        ge = r("sortingRules", be, [t.sorting]),
-                        ye = r("sortedColumns", Re, [u, ge, ce, a, ie, re, x]),
-                        we = r("sortedRows", xe, [u, ge, ce, a, ie, re, x]),
-                        Ee = r("measureFormatting", pe, [w]),
-                        ve = r("measureFormattingRules", P, [Ee]),
-                        Ae = r("measureFormatResolver", S, [ve, a, we, ye, x]),
-                        Oe = e.columnWidthCache,
-                        Te = e.rowHeightCache,
-                        Le = r("measuredColumns", he, [ye, we, g, Ae, Oe, B]),
-                        Pe = r("measuredRows", fe, [ye, we, g, Ae, Te, K]),
-                        Be = r("columns", C, [Le, l, s]),
+                        M = r("unfoldedColumns", se, [I, a]),
+                        T = r("unfoldedRows", ae, [D, a]),
+                        O = r("unfilteredColumns", R, [M, t.pinnedLeft, t.pinnedRight, t.columnWidths]),
+                        L = r("unfilteredRows", C, [T, t.pinnedTop, t.pinnedBottom, t.rowHeights]),
+                        P = r("unfilteredColumnKeys", _e, [O]),
+                        S = r("unfilteredRowKeys", _e, [L]),
+                        W = r("filterFormatting", pe, [w]),
+                        j = r("filterFormattingRules", B, [W]),
+                        te = r("filteringRules", de, [t.filtering]),
+                        re = r("filteredColumns", N, [h, te, j, a, L, O, x]),
+                        ie = r("filteredRows", F, [h, te, j, a, L, O, x]),
+                        le = r("sortingFormatting", ge, [w]),
+                        ce = r("sortingFormattingRules", B, [le]),
+                        ue = r("sortingRules", Ee, [t.sorting]),
+                        ye = r("sortedColumns", Ce, [u, ue, ce, a, ie, re, x]),
+                        we = r("sortedRows", Re, [u, ue, ce, a, ie, re, x]),
+                        be = r("measureFormatting", he, [w]),
+                        ve = r("measureFormattingRules", B, [be]),
+                        xe = r("measureFormatResolver", K, [ve, a, we, ye, x]),
+                        Ae = e.columnWidthCache,
+                        Oe = e.rowHeightCache,
+                        Le = r("measuredColumns", fe, [ye, we, g, xe, Ae, P]),
+                        Pe = r("measuredRows", me, [ye, we, g, xe, Oe, S]),
+                        Be = r("columns", A, [Le, l, s]),
                         Se = r("rows", k, [Pe, l, s]),
-                        Ke = r("columnLookup", J, [Be]),
-                        We = r("rowLookup", J, [Se]),
+                        Ke = r("columnLookup", Q, [Be]),
+                        We = r("rowLookup", Q, [Se]),
                         Fe = t.focusedCell,
                         Ne = r("sections", m, [Be, Se]),
                         ze = t.selectedCells,
-                        Ue = r("fixedSize", N, [Ne.top.height, Ne.bottom.height, Ne.left.width, Ne.right.width]),
-                        je = r("totalSize", z, [Be, Se]),
+                        Ue = r("fixedSize", z, [Ne.top.height, Ne.bottom.height, Ne.left.width, Ne.right.width]),
+                        je = r("totalSize", U, [Be, Se]),
                         He = function(e, t, o, n, r, i) {
                             if (!t) return null;
                             if (t.x < 0 || t.y < 0 || t.x > i.width || t.y > i.height) return null;
                             const l = e.scrollLeft,
                                 s = e.scrollTop,
                                 a = e.clientWidth,
                                 c = e.clientHeight,
@@ -1779,52 +1798,52 @@
                                     return -1
                                 }(n, u);
                             return -1 === d || -1 === p ? null : {
                                 rowId: o[d].id,
                                 columnId: n[p].id
                             }
                         }(e.element, e.mousePosition, Se, Be, Ue, je),
-                        qe = e.resizingColumn || r("resizableColumn", Ce, [Be, Ke, We, He, e.mousePosition]),
-                        $e = e.resizingRow || r("resizableRow", ke, [Se, Ke, We, He, e.mousePosition]),
-                        Ve = r("highlightedCells", Q, [e.isMouseDown, !!qe || !!$e, Fe, He, Be, Se, Ke, We]),
+                        qe = e.resizingColumn || r("resizableColumn", ke, [Be, Ke, We, He, e.mousePosition]),
+                        $e = e.resizingRow || r("resizableRow", Ie, [Se, Ke, We, He, e.mousePosition]),
+                        Ve = r("highlightedCells", ee, [e.isMouseDown, !!qe || !!$e, Fe, He, Be, Se, Ke, We]),
                         Ge = r("selection", b, [ze]),
                         Ye = r("highlight", b, [Ve]),
                         Xe = r("renderFormatting", f, [w, He, Fe, Ge, Ye, x, qe, $e]),
-                        Ze = r("renderFormattingRules", P, [Xe]),
-                        Je = r("renderFormatResolver", S, [Ze, a, Se, Be, x]),
+                        Ze = r("renderFormattingRules", B, [Xe]),
+                        Je = r("renderFormatResolver", K, [Ze, a, Se, Be, x]),
                         Qe = r("inputFormatting", p, [w]),
-                        et = r("inputFormattingRules", P, [Qe]),
-                        tt = r("inputFormatResolver", S, [et, a, Se, Be, x]),
+                        et = r("inputFormattingRules", B, [Qe]),
+                        tt = r("inputFormatResolver", K, [et, a, Se, Be, x]),
                         ot = r("editableCells", i, [ze, tt, Ke, We]),
-                        nt = r("inputPlacement", te, [ot, Fe, Ke, We, Ne]),
-                        rt = r("isTextValid", oe, [c, ot]),
+                        nt = r("inputPlacement", oe, [ot, Fe, Ke, We, Ne]),
+                        rt = r("isTextValid", ne, [c, ot]),
                         it = function(e, t, o, n) {
                             const r = {
                                     width: n.getBoundingClientRect().width,
                                     height: n.getBoundingClientRect().height
                                 },
                                 i = {
                                     left: n.scrollLeft,
                                     top: n.scrollTop
                                 },
-                                l = e || Z,
-                                s = G({
+                                l = e || J,
+                                s = Y({
                                     left: 0,
                                     top: 0,
                                     ...t
                                 }, o),
-                                a = G({
+                                a = Y({
                                     ...i,
                                     ...r
                                 }, o),
-                                c = q(s, $(a, Y)),
-                                u = q(s, $(a, X));
-                            return H(s, l) && H(l, c) ? V(l) > 2 * V(u) ? u : l : u
+                                c = $(s, V(a, X)),
+                                u = $(s, V(a, Z));
+                            return q(s, l) && q(l, c) ? G(l) > 2 * G(u) ? u : l : u
                         }(n?.scrollRect, je, Ue, e.element);
-                    r("activeColumns", Me, [Be, t.onActiveColumnsChange]), r("activeRows", Me, [Se, t.onActiveRowsChange]), e.state = {
+                    r("activeColumns", Te, [Be, t.onActiveColumnsChange]), r("activeRows", Te, [Se, t.onActiveRowsChange]), e.state = {
                         options: t,
                         devicePixelRatio: l,
                         borderWidth: s,
                         data: a,
                         dataFormatting: w,
                         edition: x,
                         filteredColumns: re,
@@ -1852,41 +1871,41 @@
                         text: c,
                         isTextValid: rt,
                         resizableColumn: qe,
                         resizableRow: $e
                     }
                 }
 
-                function Te(e) {
+                function Le(e) {
                     if (!e.error) try {
                         Oe(e)
                     } catch (t) {
                         e.error = t
                     }
                 }
 
-                function Le(e, t) {
+                function Pe(e, t) {
                     const o = new w(t);
                     return [...t, ...e.filter((e => !o.isIdSelected(e.rowId, e.columnId)))]
                 }
 
-                function Pe(e, t) {
+                function Be(e, t) {
                     const o = new w(t);
                     return e.filter((e => !o.isIdSelected(e.rowId, e.columnId)))
                 }
 
-                function Be(e) {
+                function Se(e) {
                     const t = e.currentTarget.getBoundingClientRect();
                     return {
                         x: e.clientX - t.left,
                         y: e.clientY - t.top
                     }
                 }
 
-                function Se(e) {
+                function Ke(e) {
                     if ("spread-grid-context" in e) return;
                     console.log("initialize");
                     const t = {
                             "top-left": document.createElement("canvas"),
                             "top-center": document.createElement("canvas"),
                             "top-right": document.createElement("canvas"),
                             "middle-left": document.createElement("canvas"),
@@ -1894,42 +1913,42 @@
                             "middle-right": document.createElement("canvas"),
                             "bottom-left": document.createElement("canvas"),
                             "bottom-center": document.createElement("canvas"),
                             "bottom-right": document.createElement("canvas")
                         },
                         o = document.createElement("input");
                     e.setAttribute("tabindex", "0"), e.setAttribute("style", "max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;"), e.classList.add("spread-grid"), t["top-left"].setAttribute("style", "position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;"), t["top-center"].setAttribute("style", "position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;"), t["top-right"].setAttribute("style", "position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;"), t["middle-left"].setAttribute("style", "position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;"), t["middle-center"].setAttribute("style", "grid-row: 2; grid-column: 2; z-index: 0;"), t["middle-right"].setAttribute("style", "position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;"), t["bottom-left"].setAttribute("style", "position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;"), t["bottom-center"].setAttribute("style", "position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;"), t["bottom-right"].setAttribute("style", "position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;"), o.setAttribute("style", "position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;");
-                    const r = {
+                    const l = {
                         externalOptions: {},
                         state: null,
                         memory: {},
                         element: e,
                         canvases: t,
                         input: o,
                         renderRequested: !1,
                         mousePosition: null,
                         isMouseDown: !1,
                         columnWidthCache: new Map,
                         rowHeightCache: new Map,
                         requestNewRender: () => {
-                            r.renderRequested || (r.renderRequested = !0, requestAnimationFrame((() => {
-                                r.renderRequested = !1, Te(r), u(r)
+                            l.renderRequested || (l.renderRequested = !0, requestAnimationFrame((() => {
+                                l.renderRequested = !1, Le(l), u(l)
                             })))
                         },
                         addEventListener: (e, t, o) => {
                             e.addEventListener(t, (e => {
                                 try {
                                     o(e)
                                 } catch (e) {
-                                    e.message = `[${t} event]: ${e.message}`, r.error = e, r.requestNewRender()
+                                    e.message = `[${t} event]: ${e.message}`, l.error = e, l.requestNewRender()
                                 }
                             }))
                         }
                     };
-                    r.localOptions = {
+                    l.localOptions = {
                         data: [],
                         columns: [{
                             type: "DATA-BLOCK"
                         }],
                         rows: [{
                             type: "HEADER"
                         }, {
@@ -1946,204 +1965,222 @@
                         pinnedTop: 0,
                         pinnedBottom: 0,
                         pinnedLeft: 0,
                         pinnedRight: 0,
                         borderWidth: 1,
                         focusedCell: null,
                         onFocusedCellChange: e => {
-                            r.localOptions.focusedCell = e, r.requestNewRender()
+                            l.localOptions.focusedCell = e, l.requestNewRender()
                         },
                         selectedCells: [],
                         onSelectedCellsChange: e => {
-                            r.localOptions.selectedCells = e, r.requestNewRender()
+                            l.localOptions.selectedCells = e, l.requestNewRender()
                         },
                         highlightedCells: [],
                         editedCells: [],
                         onEditedCellsChange: e => {
-                            r.localOptions.editedCells = e, r.requestNewRender()
+                            l.localOptions.editedCells = e, l.requestNewRender()
                         },
                         filters: [],
                         onFiltersChange: e => {
-                            r.localOptions.filters = e, r.requestNewRender()
+                            l.localOptions.filters = e, l.requestNewRender()
                         },
                         sortBy: [],
                         onSortByChange: e => {
-                            r.localOptions.sortBy = e, r.requestNewRender()
+                            l.localOptions.sortBy = e, l.requestNewRender()
                         },
                         onCellClick: () => {},
                         onCustomCellClick: () => {},
                         columnWidths: [],
                         onColumnWidthsChange: e => {
-                            r.localOptions.columnWidths = e, r.requestNewRender()
+                            l.localOptions.columnWidths = e, l.requestNewRender()
                         },
                         rowHeights: [],
                         onRowHeightsChange: e => {
-                            r.localOptions.rowHeights = e, r.requestNewRender()
+                            l.localOptions.rowHeights = e, l.requestNewRender()
                         },
                         onActiveColumnsChange: () => {},
                         onActiveRowsChange: () => {}
-                    }, e["spread-grid-context"] = r;
-                    const l = e => {
+                    }, e["spread-grid-context"] = l;
+                    const s = e => {
                             o.value = e, o.dispatchEvent(new Event("input"))
                         },
-                        s = e => {
-                            const t = r.state.options.selectedCells,
-                                o = r.state.inputFormatResolver,
-                                n = r.state.columnLookup,
-                                s = r.state.rowLookup,
-                                a = r.state.text,
-                                c = r.state.isTextValid,
-                                u = r.state.options.onEditedCellsChange,
-                                d = r.state.options.onFiltersChange,
-                                p = i(t, o, n, s);
+                        a = e => {
+                            const t = l.state.options.selectedCells,
+                                o = l.state.inputFormatResolver,
+                                n = l.state.columnLookup,
+                                r = l.state.rowLookup,
+                                a = l.state.text,
+                                c = l.state.isTextValid,
+                                u = l.state.options.onEditedCellsChange,
+                                d = l.state.options.onFiltersChange,
+                                p = i(t, o, n, r);
                             if ("" === a) return;
                             if (!c) return;
                             if (e && !p.every((e => e.edit.autoCommit))) return;
                             const h = p.filter((e => "DATA" === e.type)),
                                 f = p.filter((e => "FILTER" === e.type));
                             var m;
                             m = h.map((e => ({
                                 ...e.cell,
                                 value: e.edit.parse({
                                     string: a
                                 })
-                            }))), u(Le(r.state.options.editedCells, m)), (e => {
-                                d(Le(r.state.options.filters, e))
+                            }))), u(Pe(l.state.options.editedCells, m)), (e => {
+                                d(Pe(l.state.options.filters, e))
                             })(f.map((e => ({
                                 ...e.cell,
                                 expression: e.edit.parse({
                                     string: a
                                 })
-                            })))), e || l("")
+                            })))), e || s("")
                         },
-                        a = e => {
-                            const t = r.state.options.selectedCells,
-                                o = r.state.options.onEditedCellsChange,
-                                n = r.state.options.onFiltersChange,
-                                l = i(t, r.state.inputFormatResolver, r.state.columnLookup, r.state.rowLookup);
+                        c = e => {
+                            const t = l.state.options.selectedCells,
+                                o = l.state.options.onEditedCellsChange,
+                                n = l.state.options.onFiltersChange,
+                                r = i(t, l.state.inputFormatResolver, l.state.columnLookup, l.state.rowLookup);
                             var s;
-                            e && !l.every((e => e.edit.autoCommit)) || (s = t, o(Pe(r.state.options.editedCells, s)), (e => {
-                                n(Pe(r.state.options.filters, e))
+                            e && !r.every((e => e.edit.autoCommit)) || (s = t, o(Be(l.state.options.editedCells, s)), (e => {
+                                n(Be(l.state.options.filters, e))
                             })(t))
                         };
-                    r.addEventListener(e, "scroll", (e => {
-                        r.requestNewRender()
-                    })), r.addEventListener(e, "mouseenter", (e => {
-                        r.mousePosition = Be(e), r.requestNewRender()
-                    })), r.addEventListener(e, "mousemove", (e => {
-                        if (r.mousePosition = Be(e), r.resizingColumn) {
-                            const e = r.state.columnLookup.get(n(r.resizingColumn)),
+                    l.addEventListener(e, "scroll", (e => {
+                        l.requestNewRender()
+                    })), l.addEventListener(e, "mouseenter", (e => {
+                        l.mousePosition = Se(e), l.requestNewRender()
+                    })), l.addEventListener(e, "mousemove", (e => {
+                        if (l.mousePosition = Se(e), l.resizingColumn) {
+                            const e = l.state.columnLookup.get(n(l.resizingColumn)),
                                 t = e.width,
                                 o = e.right,
-                                i = r.mousePosition.x,
-                                l = Math.max(10, i - o + t),
-                                s = r.state.options.columnWidths.filter((t => n(t.columnId) !== e.key)).concat([{
+                                r = l.mousePosition.x,
+                                i = Math.max(10, r - o + t),
+                                s = l.state.options.columnWidths.filter((t => n(t.columnId) !== e.key)).concat([{
                                     columnId: e.id,
-                                    width: l
+                                    width: i
                                 }]);
-                            r.state.options.onColumnWidthsChange(s)
+                            l.state.options.onColumnWidthsChange(s)
                         }
-                        if (r.resizingRow) {
-                            const e = r.state.rowLookup.get(n(r.resizingRow)),
+                        if (l.resizingRow) {
+                            const e = l.state.rowLookup.get(n(l.resizingRow)),
                                 t = e.height,
                                 o = e.bottom,
-                                i = r.mousePosition.y,
-                                l = Math.max(10, i - o + t),
-                                s = r.state.options.rowHeights.filter((t => n(t.rowId) !== e.key)).concat([{
+                                r = l.mousePosition.y,
+                                i = Math.max(10, r - o + t),
+                                s = l.state.options.rowHeights.filter((t => n(t.rowId) !== e.key)).concat([{
                                     rowId: e.id,
-                                    height: l
+                                    height: i
                                 }]);
-                            r.state.options.onRowHeightsChange(s)
+                            l.state.options.onRowHeightsChange(s)
                         }
-                        r.requestNewRender()
-                    })), r.addEventListener(e, "mouseleave", (() => {
-                        r.mousePosition = null, r.requestNewRender()
-                    })), r.addEventListener(e, "mousedown", (e => {
-                        Te(r), l(""), r.isMouseDown = !0, r.mouseDownPosition = r.mousePosition, r.mouseDownCell = r.state.hoveredCell, r.state.resizableColumn && (r.resizingColumn = r.state.resizableColumn), r.state.resizableRow && (r.resizingRow = r.state.resizableRow), r.state.resizableColumn || r.state.resizableRow || r.state.options.onFocusedCellChange(r.state.hoveredCell), e.ctrlKey || r.state.options.onSelectedCellsChange([]), r.requestNewRender()
-                    })), r.addEventListener(e, "mouseup", (e => {
-                        Te(r), r.isMouseDown = !1, r.resizingColumn = null, r.resizingRow = null, r.state.options.onSelectedCellsChange(Le(r.state.options.selectedCells, r.state.highlightedCells)), r.requestNewRender()
-                    })), r.addEventListener(e, "pointerdown", (e => {
-                        r.element.setPointerCapture(e.pointerId)
-                    })), r.addEventListener(e, "pointerup", (e => {
-                        r.element.releasePointerCapture(e.pointerId)
-                    })), r.addEventListener(e, "click", (e => {
-                        Te(r);
-                        const t = r.state.hoveredCell,
-                            o = r.mouseDownCell;
-                        if (r.state.resizableColumn || r.state.resizableRow) return;
+                        l.requestNewRender()
+                    })), l.addEventListener(e, "mouseleave", (() => {
+                        l.mousePosition = null, l.requestNewRender()
+                    })), l.addEventListener(e, "mousedown", (e => {
+                        Le(l), s(""), l.isMouseDown = !0, l.mouseDownPosition = l.mousePosition, l.mouseDownCell = l.state.hoveredCell, l.state.resizableColumn && (l.resizingColumn = l.state.resizableColumn), l.state.resizableRow && (l.resizingRow = l.state.resizableRow), l.state.resizableColumn || l.state.resizableRow || l.state.options.onFocusedCellChange(l.state.hoveredCell), e.ctrlKey || l.state.options.onSelectedCellsChange([]), l.requestNewRender()
+                    })), l.addEventListener(e, "mouseup", (e => {
+                        Le(l), l.isMouseDown = !1, l.resizingColumn = null, l.resizingRow = null, l.state.options.onSelectedCellsChange(Pe(l.state.options.selectedCells, l.state.highlightedCells)), l.requestNewRender()
+                    })), l.addEventListener(e, "pointerdown", (e => {
+                        l.element.setPointerCapture(e.pointerId)
+                    })), l.addEventListener(e, "pointerup", (e => {
+                        l.element.releasePointerCapture(e.pointerId)
+                    })), l.addEventListener(e, "click", (e => {
+                        Le(l);
+                        const t = l.state.hoveredCell,
+                            o = l.mouseDownCell;
+                        if (l.state.resizableColumn || l.state.resizableRow) return;
                         if (null === t) return;
                         if (n(t.columnId) !== n(o.columnId)) return;
                         if (n(t.rowId) !== n(o.rowId)) return;
-                        const i = r.state.columnLookup.get(n(t.columnId)),
-                            l = r.state.rowLookup.get(n(t.rowId)),
-                            s = r.state.options.sortBy;
-                        if ("DATA" === i.type && "DATA" === l.type) r.state.options.onCellClick(r.state.hoveredCell);
-                        else if ("CUSTOM" === i.type || "CUSTOM" === l.type) r.state.options.onCustomCellClick(r.state.hoveredCell);
-                        else if ("HEADER" === i.type || "HEADER" === l.type) {
+                        const i = l.state.columnLookup.get(n(t.columnId)),
+                            s = l.state.rowLookup.get(n(t.rowId)),
+                            a = l.state.options.sortBy,
+                            c = l.state.inputFormatResolver.resolve(s, i);
+                        if (c.edit?.toggle) {
+                            const e = function(e, t, o, n) {
+                                    const r = n.hasValueByKey(o.key, t.key) ? n.getValueByKey(o.key, t.key) : e.value,
+                                        i = e.edit.toggle;
+                                    return "function" == typeof i ? i({
+                                        value: r
+                                    }) : i[(i.indexOf(r) + 1) % i.length]
+                                }(c, i, s, l.state.edition),
+                                o = r(i, s);
+                            "DATA" === o && l.state.options.onEditedCellsChange(Pe(l.state.options.editedCells, [{
+                                ...t,
+                                value: e
+                            }])), "FILTER" === o && l.state.options.onFiltersChange(Pe(l.state.options.filters, [{
+                                ...t,
+                                expression: e
+                            }]))
+                        } else if ("DATA" === i.type && "DATA" === s.type) l.state.options.onCellClick(l.state.hoveredCell);
+                        else if ("CUSTOM" === i.type || "CUSTOM" === s.type) l.state.options.onCustomCellClick(l.state.hoveredCell);
+                        else if ("HEADER" === i.type || "HEADER" === s.type) {
                             const t = function(e, t, o, r) {
                                 function i(e) {
                                     return t.key === n(e.columnId || "HEADER") && o.key === n(e.rowId || "HEADER")
                                 }
                                 const l = ["ASC", "DESC", void 0],
                                     s = e.find(i),
                                     a = l.indexOf(s?.direction),
                                     c = l[(a + 1) % l.length],
                                     u = e.indexOf(s) === e.length - 1;
                                 return [...!r || !u && s ? [] : e.filter((e => !i(e))), ...c ? [{
                                     columnId: t.id,
                                     rowId: o.id,
                                     direction: c
                                 }] : []]
-                            }(s, i, l, e.ctrlKey);
-                            r.state.options.onSortByChange(t), r.state.options.onSelectedCellsChange([])
+                            }(a, i, s, e.ctrlKey);
+                            l.state.options.onSortByChange(t), l.state.options.onSelectedCellsChange([])
                         }
-                    })), r.addEventListener(e, "dblclick", (e => {
-                        if (Te(r), r.state.resizableColumn) {
-                            const e = n(r.state.resizableColumn),
-                                t = r.state.options.columnWidths.filter((t => n(t.columnId) !== e));
-                            r.state.options.onColumnWidthsChange(t), r.columnWidthCache.delete(e)
-                        }
-                        if (r.state.resizableRow) {
-                            const e = n(r.state.resizableRow),
-                                t = r.state.options.rowHeights.filter((t => n(t.rowId) !== e));
-                            r.state.options.onRowHeightsChange(t), r.rowHeightCache.delete(e)
+                    })), l.addEventListener(e, "dblclick", (e => {
+                        if (Le(l), l.state.resizableColumn) {
+                            const e = n(l.state.resizableColumn),
+                                t = l.state.options.columnWidths.filter((t => n(t.columnId) !== e));
+                            l.state.options.onColumnWidthsChange(t), l.columnWidthCache.delete(e)
+                        }
+                        if (l.state.resizableRow) {
+                            const e = n(l.state.resizableRow),
+                                t = l.state.options.rowHeights.filter((t => n(t.rowId) !== e));
+                            l.state.options.onRowHeightsChange(t), l.rowHeightCache.delete(e)
                         }
-                        const t = r.state.focusedCell;
+                        const t = l.state.focusedCell;
                         if (null === t) return;
-                        const i = n(t.columnId),
-                            s = n(t.rowId),
-                            a = r.state.columnLookup,
-                            c = r.state.rowLookup,
-                            u = r.state.inputFormatResolver;
-                        if (!a.has(i)) return;
-                        if (!c.has(s)) return;
-                        const d = a.get(i),
-                            p = c.get(s),
-                            h = u.resolve(p, d).text;
-                        l(h), o?.select()
-                    })), r.addEventListener(e, "focus", (() => {
+                        const r = n(t.columnId),
+                            i = n(t.rowId),
+                            a = l.state.columnLookup,
+                            c = l.state.rowLookup,
+                            u = l.state.inputFormatResolver;
+                        if (!a.has(r)) return;
+                        if (!c.has(i)) return;
+                        const d = a.get(r),
+                            p = c.get(i),
+                            h = u.resolve(p, d),
+                            f = h.text;
+                        h.edit && (h.edit.toggle || (s(f), o?.select()))
+                    })), l.addEventListener(e, "focus", (() => {
                         o.parentElement && o.focus({
                             preventScroll: !0
                         })
-                    })), r.addEventListener(e, "keydown", (e => {
-                        Te(r);
-                        const t = r.state.focusedCell,
-                            o = r.state.columnLookup,
-                            i = r.state.rowLookup,
-                            c = r.state.options.selectedCells,
-                            u = r.state.options.onSelectedCellsChange,
-                            d = r.state.options.onFocusedCellChange,
-                            p = r.state.options.editedCells,
-                            h = r.state.options.onEditedCellsChange,
-                            f = r.state.columns,
-                            m = r.state.rows,
-                            _ = r.state.text,
-                            g = r.state.inputFormatResolver,
+                    })), l.addEventListener(e, "keydown", (e => {
+                        Le(l);
+                        const t = l.state.focusedCell,
+                            o = l.state.columnLookup,
+                            r = l.state.rowLookup,
+                            i = l.state.options.selectedCells,
+                            u = l.state.options.onSelectedCellsChange,
+                            d = l.state.options.onFocusedCellChange,
+                            p = l.state.options.editedCells,
+                            h = l.state.options.onEditedCellsChange,
+                            f = l.state.columns,
+                            m = l.state.rows,
+                            _ = l.state.text,
+                            g = l.state.inputFormatResolver,
                             y = (e, t) => {
-                                d(e), t.shiftKey ? u(Le(c, [e])) : u([e])
+                                d(e), t.shiftKey ? u(Pe(i, [e])) : u([e])
                             },
                             b = (e, r) => {
                                 if (!t) return;
                                 const i = n(t.columnId);
                                 if (!o.has(i)) return;
                                 const l = o.get(i).index,
                                     s = Math.max(0, Math.min(f.length - 1, l + e));
@@ -2152,34 +2189,34 @@
                                     rowId: t.rowId,
                                     columnId: f[s].id
                                 };
                                 y(a, r)
                             },
                             E = (e, o) => {
                                 if (!t) return;
-                                const r = n(t.rowId);
-                                if (!i.has(r)) return;
-                                const l = i.get(r).index,
+                                const i = n(t.rowId);
+                                if (!r.has(i)) return;
+                                const l = r.get(i).index,
                                     s = Math.max(0, Math.min(m.length - 1, l + e));
                                 if (s === l) return;
                                 const a = {
                                     rowId: m[s].id,
                                     columnId: t.columnId
                                 };
                                 y(a, o)
                             },
                             v = () => {
                                 e.preventDefault(), e.stopPropagation()
                             };
                         switch (e.key) {
                             case "Escape":
-                                "" !== _ ? l("") : c.length > 1 ? u([t]) : p.length > 0 ? h([]) : (d(null), u([]));
+                                "" !== _ ? s("") : i.length > 1 ? u([t]) : p.length > 0 ? h([]) : (d(null), u([]));
                                 break;
                             case "Enter":
-                                s();
+                                a();
                                 break;
                             case "ArrowUp":
                                 v(), E(e.ctrlKey ? -m.length : -1, e);
                                 break;
                             case "ArrowDown":
                                 v(), E(e.ctrlKey ? m.length : 1, e);
                                 break;
@@ -2187,15 +2224,15 @@
                                 v(), b(e.ctrlKey ? -f.length : -1, e);
                                 break;
                             case "ArrowRight":
                                 v(), b(e.ctrlKey ? f.length : 1, e);
                                 break;
                             case "Delete":
                             case "Backspace":
-                                a();
+                                c();
                                 break;
                             case "c":
                                 (e => {
                                     if (!e.ctrlKey) return;
                                     const t = function(e, t, o, r) {
                                         const i = new Map(t.map((e => [e.key, e]))),
                                             l = new Map(o.map((e => [e.key, e]))),
@@ -2227,55 +2264,55 @@
                                                         e < p && m.push("\t")
                                                     }
                                                 }
                                                 e < f && m.push("\n")
                                             }
                                         }
                                         return m.join("")
-                                    }(c, f, m, g);
+                                    }(i, f, m, g);
                                     if (navigator.clipboard) navigator.clipboard.writeText(t);
                                     else {
                                         const e = document.createElement("textarea");
                                         e.value = t, document.body.appendChild(e), e.select(), document.execCommand("copy"), document.body.removeChild(e)
                                     }
                                 })(e)
                         }
                     })), new ResizeObserver((() => {
-                        r.requestNewRender()
-                    })).observe(e), r.addEventListener(o, "input", (e => {
-                        Te(r), e.target.value ? (s(!0), o.style.opacity = 1, o.style.pointerEvents = "auto") : (e.isTrusted && a(!0), o.style.opacity = 0, o.style.pointerEvents = "none")
-                    })), r.addEventListener(o, "click", (e => {
+                        l.requestNewRender()
+                    })).observe(e), l.addEventListener(o, "input", (e => {
+                        Le(l), e.target.value ? (a(!0), o.style.opacity = 1, o.style.pointerEvents = "auto") : (e.isTrusted && c(!0), o.style.opacity = 0, o.style.pointerEvents = "none")
+                    })), l.addEventListener(o, "click", (e => {
                         e.stopPropagation()
-                    })), r.addEventListener(o, "dblclick", (e => {
+                    })), l.addEventListener(o, "dblclick", (e => {
                         e.stopPropagation()
-                    })), r.addEventListener(o, "mousedown", (e => {
+                    })), l.addEventListener(o, "mousedown", (e => {
                         e.stopPropagation()
-                    })), r.addEventListener(o, "keydown", (e => {
+                    })), l.addEventListener(o, "keydown", (e => {
                         switch (e.key) {
                             case "Enter":
                             case "Escape":
                                 break;
                             case "Delete":
                             case "Backspace":
                             case "ArrowUp":
                             case "ArrowDown":
                             case "ArrowLeft":
                             case "ArrowRight":
-                                "" !== o.value && (e.stopPropagation(), r.requestNewRender());
+                                "" !== o.value && (e.stopPropagation(), l.requestNewRender());
                                 break;
                             default:
-                                e.stopPropagation(), r.requestNewRender()
+                                e.stopPropagation(), l.requestNewRender()
                         }
                     }))
                 }
 
-                function Ke(e, t) {
-                    console.log("createGrid"), Se(e);
+                function We(e, t) {
+                    console.log("createGrid"), Ke(e);
                     const o = e["spread-grid-context"];
-                    o.externalOptions = t, null === o.state ? (Te(o), u(o)) : o.requestNewRender()
+                    o.externalOptions = t, null === o.state ? (Le(o), u(o)) : o.requestNewRender()
                 }
             }
         },
         __webpack_module_cache__ = {};
 
     function __webpack_require__(e) {
         var t = __webpack_module_cache__[e];
@@ -2325,15 +2362,15 @@
         jsonpScriptSrc = function(e) {
             var t = getCurrentScript(),
                 o = isLocalScript(t),
                 n = __jsonpScriptSrc__(e);
             if (!o) return n;
             var r = n.split("/"),
                 i = r.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_0_8m1712512160"), r.splice(-1, 1, i.join(".")), r.join("/")
+            return i.splice(1, 0, "v0_0_9m1712685293"), r.splice(-1, 1, i.join(".")), r.join("/")
         }
     }
     var __webpack_exports__ = {};
     (() => {
         __webpack_require__.r(__webpack_exports__), __webpack_require__.d(__webpack_exports__, {
             DashSpreadGrid: () => e.Z
         });
```

### Comparing `dash_spread_grid-0.0.8/dash_spread_grid/dash_spread_grid.min.js.map` & `dash_spread_grid-0.0.9/dash_spread_grid/dash_spread_grid.min.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9163427863204711%*

 * *Differences: {"'mappings'": "'2rGAMA,SAASA,SAASC,GACd,MAAwB,iBAAVA,GAAsBA,aAAiBC,MACzD,CAEA,SAASC,sBAAsBC,YAC3B,OAAOC,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,oEAEhB,OAAOF,WAAWG,KAAI,SAAAC,MAClB,IAAMC,WAAa,CAAC,EAgBpB,GAdI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAC9D,UAAWJ,OACXC,WAAWR,MAAQY,KAAK,IAADC,OAAKR,QAAO,SAAAQ,OAAQN,KAAKP,MAAK,OACrD,SAAUO,OACVC,WAAWM,KAAOF,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKO,KAAI,OACpD,UAAWP,OACXC, […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "dash_spread_grid.min.js",
-    "mappings": "2rGAMA,SAASA,SAASC,GACd,MAAwB,iBAAVA,GAAsBA,aAAiBC,MACzD,CAEA,SAASC,sBAAsBC,YAC3B,OAAOC,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,oEAEhB,OAAOF,WAAWG,KAAI,SAAAC,MAClB,IAAMC,WAAa,CAAC,EAgBpB,GAdI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAC9D,UAAWJ,OACXC,WAAWR,MAAQY,KAAK,IAADC,OAAKR,QAAO,SAAAQ,OAAQN,KAAKP,MAAK,OACrD,SAAUO,OACVC,WAAWM,KAAOF,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKO,KAAI,OACpD,UAAWP,OACXC,WAAWO,MAAQhB,SAASQ,KAAKQ,OAASH,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKQ,MAAK,MAAOR,KAAKQ,OACzF,YAAaR,OACbC,WAAWQ,QAAUjB,SAASQ,KAAKS,SAAWJ,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKS,QAAO,MAAOT,KAAKS,SAC/F,SAAUT,KACV,GAAIA,KAAKU,KAAM,CACX,IAAMC,WAAa,CAAC,EAChB,aAAcX,KAAKU,OACnBC,WAAWC,SAAWP,KAAK,kBAADC,OAAmBN,KAAKU,KAAKE,SAAQ,OAC/D,UAAWZ,KAAKU,OAChBC,WAAWE,MAAQR,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKU,KAAKG,MAAK,OAC3D,gBAAiBb,KAAKU,OACtBC,WAAWG,WAAad,KAAKU,KAAKK,aACtCd,WAAWS,KAAOC,UACtB,MAEIV,WAAWS,KAAOV,KAAKU,KAG/B,OAAOT,UACX,GACJ,GAAG,CAACL,YACR,CAEA,SAASoB,qBAAqBC,WAC1B,OAAOpB,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,8DAEhB,OAAOmB,UAAUlB,KAAI,SAAAC,MACjB,IAAMC,WAAa,CAAC,EASpB,MAPI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAE3DH,UACX,GACJ,GAAG,CAACgB,WACR,CAIA,SAASC,eAAeC,GACpBC,QAAQC,MAAM,yBAEd,IAAMC,EAAWH,EAAMG,SACjBC,GAAUC,EAAAA,mCAAAA,QAAO,GAEjBC,EAAON,EAAMM,KACbC,EAAUP,EAAMO,QAChBC,EAAOR,EAAMQ,KACb/B,EAAaD,sBAAsBwB,EAAMvB,YACzCqB,EAAYD,qBAAqBG,EAAMF,WACvCW,EAAYT,EAAMU,WAClBC,EAAeX,EAAMY,cACrBC,EAAab,EAAMc,YACnBC,EAAcf,EAAMgB,aACpBC,EAAUjB,EAAMiB,QAChBC,GAAkBC,EAAAA,mCAAAA,cAAY,SAACF,GACjCd,EAAS,CAAEc,QAAAA,GACf,GAAG,CAACd,IACEiB,EAAcpB,EAAMqB,aACpBC,GAAcH,EAAAA,mCAAAA,cAAY,SAACI,GAC7BpB,EAAS,CAAEkB,aAAYG,cAAAA,cAAA,GAAOD,GAAI,IAAEE,EAAGrB,EAAQsB,aACnD,GAAG,CAACvB,IACEwB,EAAoB3B,EAAM4B,oBAC1BC,GAAoBV,EAAAA,mCAAAA,cAAY,SAACI,GACnCpB,EAAS,CAAEyB,oBAAmBJ,cAAAA,cAAA,GAAOD,GAAI,IAAEE,EAAGrB,EAAQsB,aAC1D,GAAG,CAACvB,IACE2B,GAAwBX,EAAAA,mCAAAA,cAAY,SAACY,GACvC5B,EAAS,CAAE6B,eAAgBD,GAC/B,GAAG,CAAC5B,IACE8B,GAAqBd,EAAAA,mCAAAA,cAAY,SAACe,GACpC/B,EAAS,CAAEgC,YAAaD,GAC5B,GAAG,CAAC/B,IAEwCiC,EAAAC,gBAAdC,EAAAA,mCAAAA,UAAS,MAAK,GAArCC,EAAOH,EAAA,GAAEI,EAAUJ,EAAA,GAuB1B,OArBIG,IACAE,EAAAA,4CAAAA,GAAWF,EAAS,CAChBjC,KAAAA,EACAC,QAAAA,EACAC,KAAAA,EACA/B,WAAAA,EACAqB,UAAAA,EACAW,UAAAA,EACAE,aAAAA,EACAE,WAAAA,EACAE,YAAAA,EACAE,QAAAA,EACAC,gBAAAA,EACAE,YAAAA,EACAE,YAAAA,EACAK,kBAAAA,EACAE,kBAAAA,EACAC,sBAAAA,EACAG,mBAAAA,IAGDS,6CAAAA,cAAoB,MAAO,CAAEC,IAAKH,GAC7C,CAIAzC,eAAe6C,UAAY,CAEvBzC,SAAU0C,kDAAAA,KAEVC,GAAID,kDAAAA,OAEJvC,KAAMuC,kDAAAA,IAENtC,QAASsC,kDAAAA,MAETrC,KAAMqC,kDAAAA,MAENpE,WAAYoE,kDAAAA,MAEZ/C,UAAW+C,kDAAAA,MAEXE,QAASF,kDAAAA,MAETG,aAAcH,kDAAAA,OAEdnC,WAAYmC,kDAAAA,OAEZjC,cAAeiC,kDAAAA,OAEf/B,YAAa+B,kDAAAA,OAEb7B,aAAc6B,kDAAAA,OAEdI,YAAaJ,kDAAAA,OAEbK,YAAaL,kDAAAA,OAEbM,cAAeN,kDAAAA,MAEfO,iBAAkBP,kDAAAA,MAElBQ,YAAaR,kDAAAA,MAEb5B,QAAS4B,kDAAAA,MAETS,OAAQT,kDAAAA,MAERU,aAAcV,kDAAAA,MAEdW,WAAYX,kDAAAA,MAEZxB,aAAcwB,kDAAAA,OAEdjB,oBAAqBiB,kDAAAA,OAErBb,eAAgBa,kDAAAA,MAEhBV,YAAaU,kDAAAA,OAGjB9C,eAAe0D,aAAe,CAC1BnD,KAAM,GACNC,QAAS,CAAC,CAAE,KAAQ,eACpBC,KAAM,CAAC,CAAE,KAAQ,UAAY,CAAE,KAAQ,eACvC/B,WAAY,GACZqB,UAAW,GACXiD,QAAS,GACTC,aAAc,0BACdtC,WAAY,EACZE,cAAe,EACfE,YAAa,EACbE,aAAc,EACdiC,YAAa,EACbC,YAAa,KACbC,cAAe,GACfC,iBAAkB,GAClBC,YAAa,GACbpC,QAAS,GACTqC,OAAQ,GACRC,aAAc,GACdC,WAAY,GACZnC,aAAc,KACdO,oBAAqB,KACrBI,eAAgB,GAChBG,YAAa,IAGjB,+C,SCxNAuB,EAAOC,QAAUC,OAAkB,S,UCAnCF,EAAOC,QAAUC,OAAc,K,gBCehB,SAAS,EAAYC,GAChC,OAAY,OAARA,EACO,OAEPC,MAAMC,QAAQF,GAPX,IAQmBA,EAVAjF,IAAI,GAEPoF,KAAK,QAUT,iBAARH,GAtBUI,EAuBMJ,EAjBpB,IALMK,OAAOC,KAAKF,GAAQG,OACRxF,KAAIiF,GAClB,GAAGA,KAAO,EAAYI,EAAOJ,QAGjBG,KAAK,SAmBrBK,KAAKC,UAAUT,GAhB1B,IATyBI,CA0BzB,CC1Be,SAASM,EAAYxF,EAAQC,GACxC,MAAoB,WAAhBD,EAAOyF,KAAiC,WAAbxF,EAAIwF,KACxB,SACS,SAAhBzF,EAAOyF,MAAgC,SAAbxF,EAAIwF,KACvB,OACJ,OACX,CCHe,SAASC,EAAiBtB,EAAeuB,EAAgBC,EAAcC,GAClF,OAAOzB,EAAcvE,KAAI2C,IACrB,MAAMsD,EAAY,EAAYtD,EAAKuD,UAC7BC,EAAS,EAAYxD,EAAKyD,OAEhC,IAAKL,EAAaM,IAAIJ,GAClB,OAAO,KACX,IAAKD,EAAUK,IAAIF,GACf,OAAO,KAEX,MAAMhG,EAAS4F,EAAaO,IAAIL,GAC1B7F,EAAM4F,EAAUM,IAAIH,GAE1B,MAAO,CACHxF,KAAMmF,EAAeS,QAAQnG,EAAKD,GAAQQ,KAC1CgC,KAAMA,EACNiD,KAAMD,EAAYxF,EAAQC,GAC9B,IACDoG,QAAO7D,GAAQA,GAAMhC,MAC5B,C,kBCtBA,MAAM8F,EAAc,eACdC,EAAiB,CAAEC,IAAK,EAAGC,MAAO,EAAGC,OAAQ,EAAGC,KAAM,GCD7C,SAASC,EAAcrH,EAAOsH,GACzC,OAAOC,KAAKC,MAAMxH,EAAQsH,GAAoBA,CAClD,CCCA,SAASG,EAAcpH,EAASqH,EAAUC,GACtC,MAAMC,EAAQvH,EAAQuH,MAChBC,EAASxH,EAAQyH,SAAS,GAAGJ,KAAYC,KACzCI,EAAkBH,EAAMI,SAASN,GACjCO,EAAoBL,EAAMI,SAASL,GACnC1F,EAAUgG,EAAkBhG,QAC5BC,EAAO6F,EAAgB7F,KAE7B,GAAoB,IAAhBA,EAAKgG,QAAmC,IAAnBjG,EAAQiG,OAG7B,YAFIL,EAAOM,eACPN,EAAOM,cAAcC,YAAYP,IAIpCA,EAAOM,eACR9H,EAAQ4D,QAAQoE,YAAYR,GAGhClG,QAAQ2G,IAAI,QAIZ,MAAMC,EAAMV,EAAOW,WAAW,KAAM,CAAEC,OAAO,IAEvCC,EAAad,EAAMc,WACnBC,EAAef,EAAMe,aAErBvC,EAAiBwB,EAAMgB,qBACvBjE,EAAciD,EAAMjD,YACpBkE,EACGd,EAAgBe,cADnBD,EAEMd,EAAgBgB,iBAFtBF,EAGIZ,EAAkBe,eAHtBH,EAIKZ,EAAkBgB,gBAEvBC,EAAevE,EAAc,EAG7BwE,EAFWjH,EAAKgG,OAEmB,GAAKW,EAAqB,EAAI,IAAMA,EAAwB,EAAI,GACnGO,EAFcnH,EAAQiG,OAEc,GAAKW,EAAsB,EAAI,IAAMA,EAAuB,EAAI,GACpG3D,EAAahD,EAAK5B,KAAII,GAAOA,EAAI2I,SACjCpE,EAAehD,EAAQ3B,KAAIG,GAAUA,EAAO6I,QAC5CC,EAAatE,EAAauE,QAAO,CAACC,EAAGC,IAAMD,EAAIC,GAAG,GAAKN,EAAsBzE,EAC7EgF,EAAczE,EAAWsE,QAAO,CAACC,EAAGC,IAAMD,EAAIC,GAAG,GAAKP,EAAwBxE,EAE9EyC,EAAsB,WAAfO,EACPe,EAAWtB,KACX,EACAH,EAAmB,WAAbS,EACNgB,EAAWzB,IACX,EACAqC,EAAuB,WAAf3B,EACRe,EAAWY,MACXrB,EAAkBqB,MAClBD,EAAsB,WAAb3B,EACTgB,EAAWW,OACXtB,EAAgBsB,OAGhBO,EAAoB3E,EAAauE,QAAO,CAACK,EAAKP,EAAOQ,KACvD,MACMC,EADaF,EAAIC,GACKR,EAAQ3E,EAEpC,OADAkF,EAAIG,KAAKD,GACFF,CAAG,GACX,CAAChB,EAAsBlE,EAAc,IAClCsF,EAAkB/E,EAAWsE,QAAO,CAACK,EAAKR,EAAQS,KACpD,MACMC,EADaF,EAAIC,GACKT,EAAS1E,EAErC,OADAkF,EAAIG,KAAKD,GACFF,CAAG,GACX,CAAChB,EAAqBlE,EAAc,IAEjCuF,EAAgBN,EAAkBO,MAAM,GAAI,GAC5CC,EAAaH,EAAgBE,MAAM,GAAI,GAEvCE,EAAwB9C,KAAK+C,IAAIJ,EAAcK,eAAcR,GAAUA,GAAU3C,IAAO,GACxFoD,EAAwBN,EAAcK,eAAcR,GAAUA,GAAU3C,EAAOkC,IAC/EmB,EAAqBlD,KAAK+C,IAAIF,EAAWG,eAAcR,GAAUA,GAAU9C,IAAM,GACjFyD,EAAqBN,EAAWG,eAAcR,GAAUA,GAAU9C,EAAMoC,IAExEsB,EAAgCpD,KAAK+C,IAAID,EAAuBxB,EAAsB,EAAI,GAC1F+B,EAAgCJ,GAAyB3B,EAAuB,EAAI,GACpFgC,EAAkCtD,KAAK+C,IAAIG,EAAoB5B,EAAqB,EAAI,GACxFiC,EAAkCJ,GAAsB7B,EAAwB,EAAI,GAEpFkC,EAAQvF,MAAMwF,KAAK,CAAE9C,OAAQwC,EAAqBD,EAAqB,IAAK,CAACQ,EAAGC,KAClF,MAAMxK,EAAMwB,EAAKgJ,EAAWT,GAC5B,OAAOjF,MAAMwF,KAAK,CAAE9C,OAAQsC,EAAwBH,EAAwB,IAAK,CAACY,EAAGE,KACjF,MAAM1K,EAASwB,EAAQkJ,EAAcd,GACrC,OAAOjE,EAAeS,QAAQnG,EAAKD,EAAO,GAC5C,IAEA2K,EAAU,CAACF,EAAUC,IAAgBJ,EAAMG,EAAWT,GAAoBU,EAAcd,GAE9FxC,EAAOyB,MAAQ/B,KAAKC,MAAM8B,EAAQhC,kBAClCO,EAAOwB,OAAS9B,KAAKC,MAAM6B,EAAS/B,kBACpCO,EAAO9G,MAAMuI,MAAQ,GAAGA,MACxBzB,EAAO9G,MAAMsI,OAAS,GAAGA,MACzBxB,EAAO9G,MAAMsK,WAAa,GAAGjE,MAC7BS,EAAO9G,MAAMuK,UAAY,GAAGrE,MAC5BY,EAAO9G,MAAMwK,YAAiBhC,EAAaD,EAAQlC,EAAxB,KAC3BS,EAAO9G,MAAMyK,aAAkB7B,EAAcN,EAASpC,EAA1B,KAE5BsB,EAAIkD,UAAY,UAChBlD,EAAImD,SAAS,EAAG,EAAG7D,EAAOyB,MAAOzB,EAAOwB,QAExC,MAAMsC,EAAe,CAACC,EAAGC,KACrBtD,EAAIoD,aAAarE,iBAAkB,EAAG,EAAGA,kBAAmBsE,EAAIxE,GAAQE,kBAAmBuE,EAAI5E,GAAOK,iBAAiB,EAErHwE,EAAU,CAACF,EAAGC,EAAGvC,EAAOD,KAC1Bd,EAAIwD,YACJxD,EAAIyD,KAAKJ,EAAGC,EAAGvC,EAAOD,GACtBd,EAAI0D,MAAM,EAId,IAAK,IAAId,EAAcd,EAAuBc,GAAeX,EAAuBW,IAAe,CAC/F5C,EAAI2D,OACJP,EAAa/B,EAAkBuB,GAAc,GAC7CW,EAAQ,EAAG,EAAG7G,EAAakG,GAAcxB,GAEzC,IAAK,IAAIuB,EAAWT,EAAoBS,GAAYR,EAAoBQ,IAAY,CAChF,MAAMjI,EAAOmI,EAAQF,EAAUC,GACzBpK,EAAQkC,EAAKlC,MACboL,EAAUlC,EAAgBiB,GAC1BkB,EAAWxC,EAAkBuB,GAC7BkB,EAAYpH,EAAakG,GACzBmB,EAAapH,EAAWgG,GACxBpK,EAAOmC,EAAKnC,KACZyL,EAAYxL,EAAMwL,WAAa,OAC/BC,EAAezL,EAAMyL,cAAgB,SACrCxL,EAAUiC,EAAKjC,QAErB2K,EAAaS,EAAUD,GAEvB5D,EAAIkD,UAAY1K,EAAM0L,YAAc,QACpClE,EAAImD,SAAS,EAAG,EAAGW,EAAWC,GAE1B,SAAUrJ,GACVA,EAAKyJ,KAAKnE,GAEVxH,EAAM4L,YACNpE,EAAIkD,UAAY1K,EAAM4L,UACtBpE,EAAImD,SAAS,EAAG,EAAGW,EAAWC,IAG9BvL,EAAM6L,SACNrE,EAAIkD,UAAY1K,EAAM6L,OACtBrE,EAAIwD,YACJxD,EAAIsE,OAAOR,EAAY,EAAGC,GAC1B/D,EAAIuE,OAAOT,EAAWC,GACtB/D,EAAIuE,OAAOT,EAAWC,EAAa,GACnC/D,EAAIwE,QAGRxE,EAAIkD,UAAY1K,EAAMiM,YAAc,QACpCzE,EAAI0E,KAAOlM,EAAMkM,MAAQlG,EACzBwB,EAAIgE,UAAYA,EAEhB,MAAMW,EAAcvE,EAAawE,eAAepM,EAAMkM,MAGhDG,EAAQ/F,EACI,SAAdkF,EAAuBvL,EAAQoG,KACb,WAAdmF,EAAyBF,EAAY,EACnB,UAAdE,EAAwBF,EAAYrL,EAAQkG,MACxC,EACZI,kBAGE+F,EAAQhG,EACO,QAAjBmF,EAAyBU,EAAYI,OAASJ,EAAYK,UAAYvM,EAAQiG,IACzD,WAAjBuF,EAA4BF,EAAa,EAAIY,EAAYI,OACpC,WAAjBd,EAA4BF,EAAaY,EAAYI,OAASJ,EAAYM,aAAexM,EAAQmG,OAC7F,EACZG,kBAGmB+F,EAAQH,EAAYI,OAASJ,EAAYK,WAAa,GAAKF,EAAQH,EAAYI,OAASJ,EAAYM,cAAgBlB,EAGvI/D,EAAIkF,SAAS3M,EAAMsM,EAAOC,IAI1B9E,EAAImF,YAAc,UAClBnF,EAAIoF,UAAYhJ,EAEhB4D,EAAIwD,YACJxD,EAAIsE,OAAO,EAAGlI,EAAcuE,GAC5BX,EAAIuE,OAAOT,EAAW1H,EAAcuE,GACpCX,EAAIsE,OAAO,EAAGP,EAAa3H,EAAcuE,GACzCX,EAAIuE,OAAOT,EAAWC,EAAa3H,EAAcuE,GACjDX,EAAIqF,SAEJrF,EAAI2D,OACJJ,EAAQ,EAAG,EAAInH,EAAa0H,EAAWC,EAAa,EAAI3H,GAExD4D,EAAIkF,SAAS3M,EAAMsM,EAAOC,GAE1B9E,EAAIsF,UAEZ,CAEAtF,EAAIsF,SACR,CAEAlC,EAAa,EAAG,GAMhB,MAAMmC,EAAa,CAACC,EAAIC,EAAIC,EAAIC,EAAInN,KAChC,IAAKA,EACD,OAEJ,MAAMuI,EAAQvI,EAAMuI,MAAQ3E,EAEtBwJ,EAAeH,IAAOE,EAGtBE,EAAKL,GAAMI,EAAe7E,EAAQ,EAAI,GACtC+E,EAAKL,GAAOG,EAA2B,EAAZ7E,EAAQ,GACnCgF,EAAKL,GAAME,EAAe7E,EAAQ,EAAI,GACtCiF,EAAKL,GAAOC,EAA2B,EAAZ7E,EAAQ,GAEzCf,EAAImF,YAAc3M,EAAMyN,OAAS,QACjCjG,EAAIoF,UAAYrE,EAEZvI,EAAM0N,MACNlG,EAAImG,YAAY3N,EAAM0N,KAAKnO,KAAIN,GAASA,EAAQsH,oBAChDiB,EAAIoG,eAAkBR,EAAeC,EAAKC,GAG1C9F,EAAImG,YAAY,IAGpBnG,EAAIwD,YACJxD,EAAIsE,OAAOuB,EAAIC,GACf9F,EAAIuE,OAAOwB,EAAIC,GACfhG,EAAIqF,QAAQ,EAGVgB,EAAe,CAACC,EAAcC,IAC3BD,EAGAC,EAGDD,EAAa/E,MAAQgF,EAAahF,MAC3B+E,EAEJC,EALID,EAHAC,EAYf,IAAK,IAAIC,EAAwBlE,EAAiCkE,GAAyBjE,EAAiCiE,IAAyB,CACjJ,MAAMC,EAAcD,EAAwB,EACtCE,EAAiBF,EAEvB,IAAK,IAAI5D,EAAcd,EAAuBc,GAAeX,EAAuBW,IAAe,CAC/F,MAGM+D,EAAcN,EAHGI,GAAevE,EAAqBW,EAAQ4D,EAAa7D,GAAapK,MAAMoO,aAAe,KACxFF,GAAkBvE,EAAqBU,EAAQ6D,EAAgB9D,GAAapK,MAAMqO,UAAY,MAIxHtB,EACIlE,EAAkBuB,GAAejC,EACjCe,EAAgBgF,GAAkB/F,EAClCU,EAAkBuB,EAAc,GAAKjC,EACrCe,EAAgBgF,GAAkB/F,EAClCgG,EACR,CACJ,CAEA,IAAK,IAAIG,EAAsB1E,EAA+B0E,GAAuBzE,EAA+ByE,IAAuB,CACvI,MAAMC,EAAkBD,EAAsB,EACxCE,EAAmBF,EAEzB,IAAK,IAAInE,EAAWT,EAAoBS,GAAYR,EAAoBQ,IAAY,CAChF,MAGMgE,EAAcN,EAHIU,GAAmBjF,EAAwBe,EAAQF,EAAUoE,GAAiBvO,MAAMyO,YAAc,KACjGD,GAAoB/E,EAAwBY,EAAQF,EAAUqE,GAAkBxO,MAAM0O,WAAa,MAI5H3B,EACIlE,EAAkB2F,GAAoBrG,EACtCe,EAAgBiB,GAAYhC,EAC5BU,EAAkB2F,GAAoBrG,EACtCe,EAAgBiB,EAAW,GAAKhC,EAChCgG,EACR,CACJ,CACJ,CAyFe,SAASQ,EAAOrP,GAC3B,IAAKA,EAAQsP,MACT,KArCR,SAAwBtP,GACpBoH,EAAcpH,EAAS,MAAO,QAC9BoH,EAAcpH,EAAS,MAAO,UAC9BoH,EAAcpH,EAAS,MAAO,SAC9BoH,EAAcpH,EAAS,SAAU,QACjCoH,EAAcpH,EAAS,SAAU,UACjCoH,EAAcpH,EAAS,SAAU,SACjCoH,EAAcpH,EAAS,SAAU,QACjCoH,EAAcpH,EAAS,SAAU,UACjCoH,EAAcpH,EAAS,SAAU,SA7DrC,SAAqBA,GACjB,MAAM4D,EAAU5D,EAAQ4D,QAClB2L,EAAQvP,EAAQuP,MAChBhI,EAAQvH,EAAQuH,MAChBiI,EAAiBjI,EAAMiI,eAE7B,IAAKA,EAAgB,CACjB,GAAID,EAAMzH,cAAe,CACrB,MAAM2H,EAAWC,SAASC,gBAAkBJ,EAC5CA,EAAMzH,cAAcC,YAAYwH,GAC5BE,GACA7L,EAAQgM,MAAM,CAAEC,eAAe,GACvC,CACA,MACJ,CAEA,MAAMrI,EAASxH,EAAQyH,SAAS+H,EAAeM,SAc/C,GAZAP,EAAM7O,MAAMqG,KAAO,SAAUyI,EAAiB,GAAGA,EAAezI,SAAW,IAC3EwI,EAAM7O,MAAMkG,IAAM,QAAS4I,EAAiB,GAAGA,EAAe5I,QAAU,IACxE2I,EAAM7O,MAAMmG,MAAQ,UAAW2I,EAAiB,GAAGA,EAAe3I,UAAY,IAC9E0I,EAAM7O,MAAMoG,OAAS,WAAY0I,EAAiB,GAAGA,EAAe1I,WAAa,IACjFyI,EAAM7O,MAAMsK,WAAa,eAAgBwE,EAAiB,GAAGA,EAAexE,eAAiB,IAC7FuE,EAAM7O,MAAMuK,UAAY,cAAeuE,EAAiB,GAAGA,EAAevE,cAAgB,IAC1FsE,EAAM7O,MAAMuI,MAAQ,GAAGuG,EAAevG,UACtCsG,EAAM7O,MAAMsI,OAAS,GAAGwG,EAAexG,WACvCuG,EAAM7O,MAAMqP,SAAWvI,EAAO9G,MAAMqP,SACpCR,EAAM7O,MAAMsP,OAASxI,EAAO9G,MAAMsP,OAClCT,EAAM7O,MAAMuP,gBAAkB1I,EAAM2I,YAAc,QAAU,WAEvDX,EAAMzH,cAAe,CACtB,MAAM2H,EAAWC,SAASC,gBAAkB/L,EAC5CA,EAAQoE,YAAYuH,GAChBE,GACAF,EAAMK,MAAM,CAAEC,eAAe,GACrC,CACJ,CA2BIM,CAAYnQ,GAzBhB,SAAsBA,GAClB,MAAM4D,EAAU5D,EAAQ4D,QAClB2D,EAAQvH,EAAQuH,MAElBA,EAAM6I,iBAAmB7I,EAAM8I,aAC/BzM,EAAQlD,MAAM4P,OAAS,cAClB/I,EAAM6I,gBACXxM,EAAQlD,MAAM4P,OAAS,aAClB/I,EAAM8I,aACXzM,EAAQlD,MAAM4P,OAAS,aAEvB1M,EAAQlD,MAAM4P,OAAS,SAC/B,CAcIC,CAAavQ,EACjB,CAyBYwQ,CAAexQ,EACnB,CACA,MAAOsP,GACHtP,EAAQsP,MAAQA,CACpB,CAGAtP,EAAQsP,OA9BhB,SAAqBtP,GACjB,MAAM4D,EAAU5D,EAAQ4D,QAClB0L,EAAQtP,EAAQsP,MAEtB1L,EAAQlD,MAAMuP,gBAAkB,UAChCrM,EAAQlD,MAAMyN,MAAQ,QACtBvK,EAAQlD,MAAMC,QAAU,OACxBiD,EAAQlD,MAAM+P,QAAU,OACxB7M,EAAQlD,MAAMgQ,cAAgB,SAC9B9M,EAAQ+M,UAAY,0OAKVrB,EAAMsB,yFAE2CtB,EAAMuB,mBAErE,CAaQC,CAAY9Q,EACpB,CC/Ye,SAAS+Q,EAAkBjR,EAAYuE,EAAcM,GAChE,MAAO,CACH,CACIvE,OAAQ,CAAE4Q,MAAO,QACjB3Q,IAAK,CAAE2Q,MAAO,UACdrR,MAAO,EAAGS,iBAA+B6Q,IAAlB7Q,EAAO8Q,OAAuB9Q,EAAO+D,GAAK/D,EAAO8Q,QAE5E,CACI9Q,OAAQ,CAAE4Q,MAAO,UACjB3Q,IAAK,CAAE2Q,MAAO,QACdrR,MAAO,EAAGU,cAAyB4Q,IAAf5Q,EAAI6Q,OAAuB7Q,EAAI8D,GAAK9D,EAAI6Q,QAEhE,CACI9Q,OAAQ,CAAE4Q,MAAO,UACjB3Q,IAAK,CAAE2Q,MAAO,WACdrR,MAAO,IAEX,CACIS,OAAQ,CAAE4Q,MAAO,WACjB3Q,IAAK,CAAE2Q,MAAO,UACdrR,MAAO,OAERgF,EAAO1E,KAAI,EAAGkG,WAAUE,QAAO8K,aAAa1H,KAAU,CACrDrJ,OAAQ,CAAE+D,GAAIgC,GACd9F,IAAK,CAAE8D,GAAIkC,GACX5F,KAAM,EAAGL,YAAa,GAAGuE,EAAOkD,OAAS,EAAI4B,EAAQ,EAAI,KAAmB,QAAd0H,EAAsB,IAAM,OAAO/Q,EAAO8Q,aAE5G,CACI9Q,OAAQ,CAAE4Q,MAAO,OACjB3Q,IAAK,CAAE2Q,MAAO,UACdrR,MAAO,EAAGyR,cAAeA,GAAY,GACrC3Q,KAAM,EAAG2Q,cAAeA,GAAY,YACpCxQ,KAAM,CACFE,SAAU,KAAM,EAChBC,MAAO,EAAGsQ,YAAaA,EACvBrQ,YAAY,IAGpB,CACIZ,OAAQ,CAAE4Q,MAAO,QACjB3Q,IAAK,CAAE2Q,MAAO,QACdrR,MAAO0E,MAERvE,EAEX,CC7Ce,SAASwR,EAAmBxR,GACvC,OAAOA,CACX,CCAA,SAASyR,EAAkBC,EAAWC,GAClC,OAAIA,EACOD,EAAY,KAEZA,EAAY,IAC3B,CAEe,SAASE,EAAoB5R,EAAY6R,EAAapN,EAAaqN,EAAWtF,EAAWuF,EAASzB,EAAiBC,GAC9H,MAAMyB,EAAmBvN,EAAc,EAAYA,EAAY4B,UAAY,KACrE4L,EAAgBxN,EAAc,EAAYA,EAAY8B,OAAS,KAE/D2L,EAAiC,OAAjB3B,EAChB4B,EAFuC,OAApB7B,GAEc4B,EAEjCE,EAAa,CAACrQ,EAAMD,EAASiJ,EAAUC,KACzC,GAAID,EAAW,GAAKA,GAAYhJ,EAAKgG,OACjC,OAAO,EACX,GAAIiD,EAAc,GAAKA,GAAelJ,EAAQiG,OAC1C,OAAO,EAEX,MAAMzB,EAASvE,EAAKgJ,GAAU3F,IACxBgB,EAAYtE,EAAQkJ,GAAa5F,IAEvC,OAAO0M,EAAUO,cAAc/L,EAAQF,EAAU,EAG/CkM,EAAW,CAAC9R,EAAWI,IACrBJ,EACO,CAACI,GAED,GAGf,MAAO,CACH,CACIN,OAAQ,CAAE4Q,MAAO,OACjB3Q,IAAK,CAAE2Q,MAAO,UACdtQ,MAAO,EAAG0Q,eAAe,CAAGhF,WAAY,UAAWO,WAAYyE,EAAW,QAAU,UAAWiB,OAAQ,CAAEpJ,MAAO,EAAGkF,MAAO,WAE9H,CACI/N,OAAQ,CAAE4Q,MAAO,OACjB3Q,IAAK,CAAE2Q,MAAO,UACdtQ,MAAO,CAAE0L,WAAY,UAAWiG,OAAQ,CAAEpJ,MAAO,EAAGkF,MAAO,UAE/D,CACI/N,OAAQ,CAAE4Q,MAAO,UACjB3Q,IAAK,CAAE2Q,MAAO,OACdtQ,MAAO,CAAE0L,WAAY,UAAWiG,OAAQ,CAAEpJ,MAAO,EAAGkF,MAAO,UAE/D,CACI/N,OAAQ,CAAE4Q,MAAO,UACjB3Q,IAAK,CAAE2Q,MAAO,UACdtQ,MAAO,CAAE0L,WAAY,eAEtBtM,KAOAsS,EAAST,IAAgBK,EAAe,CACvC5R,OAAQ,CAAE4Q,MAAO,OACjB3Q,IAAK,CAAE8D,GAAIwN,GAAatL,OACxB3F,MAAO,CAAE4L,UAAW,kBAErB8F,EAAST,IAAgBM,EAAY,CACpC7R,OAAQ,CAAE+D,GAAIwN,GAAaxL,UAC3B9F,IAAK,CAAE8D,GAAIwN,GAAatL,OACxB3F,MAAO,CAAE4L,UAAW,eAExB,CACIlM,OAAQ,CAAE4Q,MAAO,OACjB3Q,IAAK,CAAE2Q,MAAO,OACd1Q,UAAW,EAAGuB,OAAMD,UAASvB,MAAKD,YAAa8R,EAAWrQ,EAAMD,EAASvB,EAAIoJ,MAAOrJ,EAAOqJ,OAC3F/I,MAAO,EAAGmB,OAAMD,UAASvB,MAAKD,SAAQQ,WAAW,IACxCsR,EAAWrQ,EAAMD,EAASvB,EAAIoJ,MAAQ,EAAGrJ,EAAOqJ,OAAyF,CAAC,EAAjF,CAAEsF,UAAW,CAAE9F,MAAO,EAAGkF,MAAO,UAAW1E,MAAO6I,OAAOC,sBAClHL,EAAWrQ,EAAMD,EAASvB,EAAIoJ,MAAQ,EAAGrJ,EAAOqJ,OAA4F,CAAC,EAApF,CAAEqF,aAAc,CAAE7F,MAAO,EAAGkF,MAAO,UAAW1E,MAAO6I,OAAOC,sBACrHL,EAAWrQ,EAAMD,EAASvB,EAAIoJ,MAAOrJ,EAAOqJ,MAAQ,GAAsF,CAAC,EAAlF,CAAE2F,WAAY,CAAEnG,MAAO,EAAGkF,MAAO,UAAW1E,MAAO6I,OAAOC,sBACnHL,EAAWrQ,EAAMD,EAASvB,EAAIoJ,MAAOrJ,EAAOqJ,MAAQ,GAAuF,CAAC,EAAnF,CAAE0F,YAAa,CAAElG,MAAO,EAAGkF,MAAO,UAAW1E,MAAO6I,OAAOC,mBACzHjG,UAAWiF,EAAkB3Q,EAAO,UAAY,UAAWkR,IAAqB1R,EAAO8E,KAAO6M,IAAkB1R,EAAI6E,QAG5H,CACI9E,OAAQ,CAAE4Q,MAAO,OACjB3Q,IAAK,CAAE2Q,MAAO,OACd1Q,UAAW,EAAGD,MAAKD,YAAakM,EAAU6F,cAAc9R,EAAI6E,IAAK9E,EAAO8E,KACxExE,MAAO,EAAGL,MAAKD,aAAa,CACxBkM,UAAWiF,EAAkB,UAAWO,IAAqB1R,EAAO8E,KAAO6M,IAAkB1R,EAAI6E,WAGtGkN,EAAS7N,EAAa,CACrBnE,OAAQ,CAAE+D,GAAII,GAAa4B,UAC3B9F,IAAK,CAAE8D,GAAII,GAAa8B,OACxB3F,MAAO,CAAE4L,UAAW,eAExB,CACIlM,OAAQ,CAAE4Q,MAAO,OACjB3Q,IAAK,CAAE2Q,MAAO,OACd1Q,UAAW,EAAGM,UAAWA,EACzBF,MAAO,CAAE6L,OAAQ,cAErB,CACInM,OAAQ,CAAE4Q,MAAO,OACjB3Q,IAAK,CAAE2Q,MAAO,OACd1Q,UAAW,EAAGD,MAAKD,YAAayR,EAAQW,cAAcnS,EAAI6E,IAAK9E,EAAO8E,KACtExE,MAAO,CAAE6L,OAAQ,iBAElB6F,EAAShC,EAAiB,CACzBhQ,OAAQ,CAAE+D,GAAIiM,GACd/P,IAAK,CAAE2Q,MAAO,UACdtQ,MAAO,CAAEyO,YAAa,CAAElG,MAAO,EAAGkF,MAAO,wBAE1CiE,EAAS/B,EAAc,CACtBjQ,OAAQ,CAAE4Q,MAAO,UACjB3Q,IAAK,CAAE8D,GAAIkM,GACX3P,MAAO,CAAEoO,aAAc,CAAE7F,MAAO,EAAGkF,MAAO,qBAGtD,CCzHe,SAASsE,EAAY7Q,EAASC,GACzC,MAAM6Q,EAAY7Q,EAAK4E,QAAOpG,GAAsB,UAAfA,EAAIsS,SAAoB9K,OACvD+K,EAAe/Q,EAAK4E,QAAOpG,GAAsB,QAAfA,EAAIsS,SAAkB9K,OACxDgL,EAAehR,EAAKgG,OAAS6K,EAAYE,EACzCE,EAAalR,EAAQ6E,QAAOrG,GAA4B,UAAlBA,EAAOuS,SAAoB9K,OACjEkL,EAAcnR,EAAQ6E,QAAOrG,GAA4B,QAAlBA,EAAOuS,SAAkB9K,OAChEmL,EAAepR,EAAQiG,OAASiL,EAAaC,EAE7CE,EAAUpR,EAAKiI,MAAM,EAAG4I,GACxBQ,EAAarR,EAAKiI,MAAMjI,EAAKgG,OAAS+K,EAAc/Q,EAAKgG,QACzDsL,EAAatR,EAAKiI,MAAM4I,EAAW7Q,EAAKgG,OAAS+K,GACjDQ,EAAcxR,EAAQkI,MAAM,EAAGgJ,GAC/BO,EAAezR,EAAQkI,MAAMlI,EAAQiG,OAASkL,EAAanR,EAAQiG,QACnEyL,EAAgB1R,EAAQkI,MAAMgJ,EAAYlR,EAAQiG,OAASkL,GAE3DQ,EAAab,EAAY,EAGzBc,EAAiBV,EAAa,EAM9BW,EAPgBZ,EAAe,IAOSU,EAExCG,GAAuBH,EACvBI,IAXgBf,EAAe,GAc/BgB,EAVmBZ,EAAe,IAUSQ,EAE3CK,GAAwBL,EACxBM,IAdkBf,EAAc,GAgBhCgB,EAAY,CAAClS,EAAM4G,EAAeC,KACpC,GAAoB,IAAhB7G,EAAKgG,OACL,OAAO,EAEX,MAAMjB,EAAM6B,EAAgB5G,EAAKmS,GAAG,GAAGC,cAAgBpS,EAAKmS,GAAG,GAAGpN,IAGlE,OAFe8B,EAAmB7G,EAAKmS,IAAI,GAAGE,iBAAmBrS,EAAKmS,IAAI,GAAGlN,QAE7DF,CAAG,EAGjBuN,EAAW,CAACvS,EAAS+G,EAAgBC,KACvC,GAAuB,IAAnBhH,EAAQiG,OACR,OAAO,EAEX,MAAMd,EAAO4B,EAAiB/G,EAAQoS,GAAG,GAAGI,eAAiBxS,EAAQoS,GAAG,GAAGjN,KAG3E,OAFc6B,EAAkBhH,EAAQoS,IAAI,GAAGK,gBAAkBzS,EAAQoS,IAAI,GAAGnN,OAEjEE,CAAI,EAUvB,MAAO,CACHH,IAAK,CACD/E,KAAMoR,EACNxK,eA3CiB,EA4CjBC,kBA3CoB,EA4CpBM,OAZU+K,EAAUd,GAjCH,GACG,IA8CxBnM,OAAQ,CACJjF,KAAMqR,EACNzK,cAAegL,EACf/K,kBA/CuB,EAgDvBM,OAjBa+K,EAAUb,EAAYO,GA/BZ,IAkD3BxG,OAAQ,CACJpL,KAAMsR,EACN1K,cAAeiL,EACfhL,iBAAkBiL,EAClB3K,OAtBa+K,EAAUZ,EAAYO,EAAqBC,IAwB5D5M,KAAM,CACFnF,QAASwR,EACTzK,gBAvDmB,EAwDnBC,iBAvDoB,EAwDpBK,MA3BUkL,EAASf,GA9BA,GACC,IA0DxBvM,MAAO,CACHjF,QAASyR,EACT1K,eAAgBiL,EAChBhL,iBA3DqB,EA4DrBK,MAhCWkL,EAASd,EAAcO,GA5Bb,IA8DzBU,OAAQ,CACJ1S,QAAS0R,EACT3K,eAAgBkL,EAChBjL,gBAAiBkL,EACjB7K,MArCYkL,EAASb,EAAeO,EAAsBC,IAwCtE,CCnGe,SAASS,EAAyB7P,EAAapC,GAC1D,MAAO,IAAIoC,KAAgBpC,EAAQrC,KAAIwG,IAAU,CAAGN,SAAUM,EAAON,SAAUE,MAAOI,EAAOJ,MAAO1G,MAAO8G,EAAO+N,eACtH,CCAe,MAAMC,EACjB,WAAAC,CAAYhQ,GACRiQ,KAAKC,OAAS,IAAIC,IAElBnQ,EAAYoQ,SAAQlS,IAChB,MAAMwD,EAAS,EAAYxD,EAAKyD,OAC1BH,EAAY,EAAYtD,EAAKuD,UAE9BwO,KAAKC,OAAOtO,IAAIF,IACjBuO,KAAKC,OAAOG,IAAI3O,EAAQ,IAAIyO,KAEhCF,KAAKC,OAAOrO,IAAIH,GAAQ2O,IAAI7O,EAAWtD,EAAKjD,MAAM,GAE1D,CAEA,aAAA6S,CAAcpM,EAAQF,GAClB,OAAOyO,KAAKC,OAAOtO,IAAIF,IAAWuO,KAAKC,OAAOrO,IAAIH,GAAQE,IAAIJ,EAClE,CAEA,aAAA8O,CAAc5O,EAAQF,GAClB,GAAKyO,KAAKnC,cAAcpM,EAAQF,GAGhC,OAAOyO,KAAKC,OAAOrO,IAAIH,GAAQG,IAAIL,EACvC,CAEA,YAAA+O,CAAa5O,EAAOF,GAChB,OAAOwO,KAAKnC,cAAc,EAAYnM,GAAQ,EAAYF,GAC9D,CAEA,YAAA+O,CAAa7O,EAAOF,GAChB,OAAOwO,KAAKK,cAAc,EAAY3O,GAAQ,EAAYF,GAC9D,EChCW,SAASgP,EAAWC,GAC/B,OAAO,IAAIX,EAAQW,EACvB,CCHe,MAAMC,EACjB,WAAAX,CAAYlQ,GACRmQ,KAAKC,OAAS,IAAIC,IAElBrQ,EAAcsQ,SAAQlS,IAClB,MAAMwD,EAAS,EAAYxD,EAAKyD,OAC1BH,EAAY,EAAYtD,EAAKuD,UAE9BwO,KAAKC,OAAOtO,IAAIF,IACjBuO,KAAKC,OAAOG,IAAI3O,EAAQ,IAAIkP,KAEhCX,KAAKC,OAAOrO,IAAIH,GAAQmP,IAAIrP,EAAU,GAE9C,CAEA,aAAAiM,CAAc/L,EAAQF,GAClB,OAAOyO,KAAKC,OAAOtO,IAAIF,IAAWuO,KAAKC,OAAOrO,IAAIH,GAAQE,IAAIJ,EAClE,CAEA,YAAAsP,CAAanP,EAAOF,GAChB,OAAOwO,KAAKxC,cAAc,EAAY9L,GAAQ,EAAYF,GAC9D,ECrBW,SAASsP,EAAajR,GACjC,OAAO,IAAI6Q,EAAU7Q,EACzB,CCJe,SAASkR,EAAWC,EAAehU,GAC9C,MAAgC,mBAAlBgU,EACRA,EAAchU,GACdgU,CACV,CCHe,SAASC,EAAUnM,EAAO5B,EAAQgO,EAAaC,GAC1D,OAAIrM,EAAQoM,EACD,QACPpM,GAAS5B,EAASiO,EACX,WADX,CAGJ,CCJA,SAASC,EAAYC,EAAUH,EAAaC,GACxC,OAAOE,EAAS/V,KAAI,CAAC2D,EAAS6F,KAC1B,MAAMtF,EAAK,OAAQP,EAAUA,EAAQO,GAAKP,EAAQiC,KAClD,MAAO,IACAjC,EACHO,GAAIA,EACJ0B,KAAMjC,EAAQiC,MAAQ,OACtB4D,MAAOA,EACPvE,IAAK,EAAYf,GACjBwO,OAAQiD,EAAUnM,EAAOuM,EAASnO,OAAQgO,EAAaC,GACvD5E,OAAQ,WAAYtN,EAAUA,EAAQsN,OAAS/M,EAC/C8R,OAAQrS,EAAQqS,QAAU,GAC7B,GAET,CAEO,SAASC,EAAmBtU,EAASiU,EAAaC,EAAWlR,GAChE,MAAMuR,EAAe,IAAItB,IAAIjQ,EAAa3E,KAAI,EAAGkG,WAAU8C,WAAY,CAAC,EAAY9C,GAAW8C,MAG/F,OAFwB8M,EAAYnU,EAASiU,EAAaC,GAEnC7V,KAAIG,IAAU,IAC9BA,EACH6I,MAAOkN,EAAa7P,IAAIlG,EAAO8E,KACzBiR,EAAa5P,IAAInG,EAAO8E,KACxB9E,EAAO6I,SAErB,CAEO,SAASmN,EAAgBvU,EAAMgU,EAAaC,EAAWjR,GAC1D,MAAMwR,EAAgB,IAAIxB,IAAIhQ,EAAW5E,KAAI,EAAGoG,QAAO2C,YAAa,CAAC,EAAY3C,GAAQ2C,MAGzF,OAFqB+M,EAAYlU,EAAMgU,EAAaC,GAEhC7V,KAAII,IAAO,IACxBA,EACH2I,OAAQqN,EAAc/P,IAAIjG,EAAI6E,KACxBmR,EAAc9P,IAAIlG,EAAI6E,KACtB7E,EAAI2I,UAElB,CCvCO,SAASsN,EAAiB1U,EAASqF,EAAkB3C,GACxD,IAAIyC,EAAOzC,EAEX,OAAO1C,EAAQ3B,KAAI,CAACG,EAAQqJ,KACxB,MACMR,EAAQjC,EADQ,UAAW5G,EAASA,EAAO6I,MAAQ,IACdhC,GACrCsP,EAAY,IACXnW,EACHqJ,MAAOA,EACPR,MAAOA,EACPmL,eAAgBrN,EAAOzC,EACvByC,KAAMA,EACNF,MAAOE,EAAOkC,EACdoL,gBAAiBtN,EAAOkC,EAAQ3E,GAKpC,OAFAyC,GAAQwP,EAAUtN,MAAQ3E,EAEnBiS,CAAS,GAExB,CAEO,SAASC,EAAc3U,EAAMoF,EAAkB3C,GAClD,IAAIsC,EAAMtC,EAEV,OAAOzC,EAAK5B,KAAI,CAACI,EAAKoJ,KAClB,MACMT,EAAShC,EADQ,WAAY3G,EAAMA,EAAI2I,OAAS,GACT/B,GACvCwP,EAAS,IACRpW,EACHoJ,MAAOA,EACPT,OAAQA,EACRiL,cAAerN,EAAMtC,EACrBsC,IAAKA,EACLE,OAAQF,EAAMoC,EACdkL,iBAAkBtN,EAAMoC,EAAS1E,GAKrC,OAFAsC,GAAO6P,EAAOzN,OAAS1E,EAEhBmS,CAAM,GAErB,CC1CA,MAAMC,EAAe,CACjB,OAAU,CAAC,UACX,OAAU,CAAC,UACX,KAAQ,CAAC,QACT,OAAU,CAAC,UACX,IAAO,CAAC,SAAU,OAAQ,SAAU,UACpC,QAAW,CAAC,SAAU,SAAU,UAChCzF,UAAW,IAGf,MAAM0F,EACFC,MAAQ,IAAI/B,IACZgC,QAAU,IAAIhC,IACdiC,QAAU,IAAIjC,IACdkC,QAAU,IAAIlC,IAGH,MAAMmC,EACjBpC,OAAS,IAAI+B,EACbM,UAAW,EAEX,OAAAC,CAAQ9W,EAAQC,EAAKH,GAGjB,GAFAyU,KAAKsC,UAAW,EAEZ9R,MAAMC,QAAQhF,GACd,IAAK,MAAM+W,KAAK/W,EACZuU,KAAKuC,QAAQC,EAAG9W,EAAKH,QAI7B,GAAIiF,MAAMC,QAAQ/E,GACd,IAAK,MAAM+W,KAAK/W,EACZsU,KAAKuC,QAAQ9W,EAAQgX,EAAGlX,OAFhC,CAMAE,EAASA,EACH,OAAQA,EACJ,CAAE8E,IAAK,EAAY9E,EAAO+D,KAC1B/D,EACJ,CAAE4Q,MAAO,QACf3Q,EAAMA,EACA,OAAQA,EACJ,CAAE6E,IAAK,EAAY7E,EAAI8D,KACvB9D,EACJ,CAAE2Q,MAAO,QAuBX,QAAS5Q,GACTiX,EAAc1C,KAAKC,OAAOgC,MAAOxW,EAAO8E,KACxC,UAAW9E,GACXiX,EAAc1C,KAAKC,OAAOiC,QAASzW,EAAOqJ,OAC1C,UAAWrJ,GACXiX,EAAc1C,KAAKC,OAAOkC,QAAS1W,EAAOkX,OAC9C,IAAK,MAAMtG,KAAS0F,EAAatW,EAAO4Q,OACpCqG,EAAc1C,KAAKC,OAAOmC,QAAS/F,EAzCvC,CAaA,SAASuG,EAAW3C,EAAQ1P,GACnB0P,EAAOtO,IAAIpB,IACZ0P,EAAOG,IAAI7P,EAAK,IAEpB0P,EAAOrO,IAAIrB,GAAKyE,KAAKzJ,EACzB,CAEA,SAASmX,EAAczC,EAAQ1P,GACtB0P,EAAOtO,IAAIpB,IACZ0P,EAAOG,IAAI7P,EAAK,IAAIyR,GAEpB,QAAStW,GACTkX,EAAW3C,EAAOrO,IAAIrB,GAAK0R,MAAOvW,EAAI6E,KACtC,UAAW7E,GACXkX,EAAW3C,EAAOrO,IAAIrB,GAAK2R,QAASxW,EAAIoJ,OACxC,UAAWpJ,GACXkX,EAAW3C,EAAOrO,IAAIrB,GAAK4R,QAASzW,EAAIiX,OAC5C,IAAK,MAAMtG,KAAS0F,EAAarW,EAAI2Q,OACjCuG,EAAW3C,EAAOrO,IAAIrB,GAAK6R,QAAS/F,EAC5C,CAUJ,CAEA,QAAAwG,CAASpX,EAAQC,GACb,MAAMoX,EAAQ,GAEd,IAAK9C,KAAKsC,SACN,OAAOQ,EAEX,SAASC,EAAYC,GACjB,IAAK,MAAMzX,KAAQyX,EACfF,EAAM9N,KAAKzJ,EACnB,CAEA,SAAS0X,EAAehD,GAChBA,EAAOgC,MAAMtQ,IAAIjG,EAAI6E,MACrBwS,EAAY9C,EAAOgC,MAAMrQ,IAAIlG,EAAI6E,MACjC0P,EAAOiC,QAAQvQ,IAAIjG,EAAIoJ,QACvBiO,EAAY9C,EAAOiC,QAAQtQ,IAAIlG,EAAIoJ,QACnCmL,EAAOmC,QAAQzQ,IAAIjG,EAAIwF,OACvB6R,EAAY9C,EAAOmC,QAAQxQ,IAAIlG,EAAIwF,OACvC,IAAK,MAAMyR,KAASjX,EAAI4V,OAChBrB,EAAOkC,QAAQxQ,IAAIgR,IACnBI,EAAY9C,EAAOkC,QAAQvQ,IAAI+Q,GAE3C,CAEI3C,KAAKC,OAAOgC,MAAMtQ,IAAIlG,EAAO8E,MAC7B0S,EAAejD,KAAKC,OAAOgC,MAAMrQ,IAAInG,EAAO8E,MAC5CyP,KAAKC,OAAOiC,QAAQvQ,IAAIlG,EAAOqJ,QAC/BmO,EAAejD,KAAKC,OAAOiC,QAAQtQ,IAAInG,EAAOqJ,QAC9CkL,KAAKC,OAAOmC,QAAQzQ,IAAIlG,EAAOyF,OAC/B+R,EAAejD,KAAKC,OAAOmC,QAAQxQ,IAAInG,EAAOyF,OAClD,IAAK,MAAMyR,KAASlX,EAAO6V,OACnBtB,KAAKC,OAAOkC,QAAQxQ,IAAIgR,IACxBM,EAAejD,KAAKC,OAAOkC,QAAQvQ,IAAI+Q,IAG/C,OAAOG,CACX,ECjHJ,MAAMI,EAAc,CAAC,YAAa,cAAe,eAAgB,cAGjE,SAASC,EAAapX,EAAO+I,GACzB,MAAMsO,EAAW,IAAKrX,GAEtB,GAAI,WAAYqX,EAAU,CACtB,IAAK,MAAMC,KAAcH,EACrBE,EAASC,GAAcD,EAAS1F,cAC7B0F,EAAS1F,MACpB,CAEA,IAAK,MAAM2F,KAAcH,EACjBG,KAAcD,IACdA,EAASC,GAAc,IAAKD,EAASC,GAAavO,UAE1D,OAAOsO,CACX,CAMe,MAAME,EACjB,WAAAvD,CAAY+C,GACR9C,KAAKuD,YAAc,IAAIlB,EAEvB,IAAK,MAAOvN,EAAOvJ,KAASuX,EAAMU,UAAW,CACzC,MAAMC,EAAQ,CAAE3O,SAEZ,cAAevJ,IACfkY,EAAM9X,UAAYJ,EAAKI,WACvB,UAAWJ,IACXkY,EAAM1X,MAA8B,mBAAfR,EAAKQ,MAAuBR,EAAKQ,MAAQ,IAAMR,EAAKQ,OACzE,UAAWR,IACXkY,EAAMzY,MAA8B,mBAAfO,EAAKP,MAAuBO,EAAKP,MAAQ,IAAMO,EAAKP,OACzE,SAAUO,IACVkY,EAAM3X,KAA4B,mBAAdP,EAAKO,KAAsBP,EAAKO,KAAO,IAAMP,EAAKO,MACtE,YAAaP,IACbkY,EAAMzX,QAAkC,mBAAjBT,EAAKS,QAAyBT,EAAKS,QAAU,IAAMT,EAAKS,SAC/E,SAAUT,IACVkY,EAAMxX,KAAOV,EAAKU,MAClB,SAAUV,IACVkY,EAAM/L,KAAOnM,EAAKmM,MAEtBsI,KAAKuD,YAAYhB,QAAQhX,EAAKE,OAAQF,EAAKG,IAAK+X,EACpD,CACJ,CAEA,OAAA5R,CAAQ7E,EAAME,EAAMD,EAASvB,EAAKD,EAAQyR,GACtC,MAAM4F,EAAQ9C,KAAKuD,YACdV,SAASpX,EAAQC,GACjBoF,MAAK,CAAC2D,EAAGC,IAAMD,EAAEK,MAAQJ,EAAEI,QAC3BhD,QAAO,CAAC9G,EAAO8J,EAAO4O,IAAU1Y,EAAM8J,QAAU4O,EAAM5O,EAAQ,IAAIA,QAEvE,IAEI4C,EAFArM,EAAU,CAAE2B,OAAME,OAAMD,UAASvB,MAAKD,UACtCM,EAAQ,CAAC,EAGTC,EAAUgG,EAEVkL,EAAQW,cAAcnS,EAAI6E,IAAK9E,EAAO8E,OACtClF,EAAU,IAAKA,EAASoR,SAAUS,EAAQmD,cAAc3U,EAAI6E,IAAK9E,EAAO8E,OAE5E,IAAK,MAAMhF,KAAQuX,EACf,MAAI,cAAevX,IAASA,EAAKI,UAAUN,MAIvC,UAAWE,IACXF,EAAU,IAAKA,EAASL,MAAOO,EAAKP,MAAMK,KAC1C,UAAWE,IACXQ,EAAQ,IAAKA,KAAUoX,EAAa5X,EAAKQ,MAAMV,GAAUE,EAAKuJ,SAC9D,SAAUvJ,IACVF,EAAU,IAAKA,EAASS,KAAMP,EAAKO,KAAKT,KACxC,YAAaE,IACbS,EAAU,IAAKA,KAAYT,EAAKS,QAAQX,KACxC,SAAUE,IACVF,EAAU,IAAKA,EAASY,KAAMV,EAAKU,MAAQ,SAAUZ,EAAU,IAAKA,EAAQY,QAASV,EAAKU,MAASV,EAAKU,OACxG,SAAUV,GAAM,CAChB,MAAMoY,EAAiBtY,EACvBqM,EAAQnE,GAAQhI,EAAKmM,KAAK,IAAKiM,EAAgBpQ,OACnD,CAKJ,MACMqQ,EAAS,CACX7X,QACA8X,SAhCU,EAiCV/X,KAJS,SAAUT,EAAUA,EAAQS,KAAO,GAAGT,EAAQL,QAKvDgB,WAYJ,MATI,UAAWX,IACXuY,EAAO5Y,MAAQK,EAAQL,OACvB,SAAUK,IACVuY,EAAO3X,KAAOZ,EAAQY,WACbqQ,IAAT5E,IACAkM,EAAOlM,KAAOA,GACd,SAAUrM,IACVuY,EAAO9X,KAAOT,EAAQS,MAEnB8X,CACX,EC1GW,SAASE,EAAmBC,GACvC,OAAO,IAAIT,EAAgBS,EAC/B,CCJe,MAAMC,EACjB,WAAAjE,CAAYkE,EAAiBjX,EAAME,EAAMD,EAASiQ,GAC9C8C,KAAKiE,gBAAkBA,EACvBjE,KAAKhT,KAAOA,EACZgT,KAAK9S,KAAOA,EACZ8S,KAAK/S,QAAUA,EACf+S,KAAK9C,QAAUA,CACnB,CAEA,OAAArL,CAAQnG,EAAKD,GACT,OAAOuU,KAAKiE,gBAAgBpS,QACxBmO,KAAKhT,KACLgT,KAAK9S,KACL8S,KAAK/S,QACLvB,EACAD,EACAuU,KAAK9C,QACb,ECfW,SAASgH,EAAkBD,EAAiBjX,EAAME,EAAMD,EAASiQ,GAC5E,OAAO,IAAI8G,EAAeC,EAAiBjX,EAAME,EAAMD,EAASiQ,EACpE,CCFA,SAASiH,EAAgBxW,EAASyW,EAAYC,GAC1C,MAAMC,EAAe,IAAIpE,IACzB,IAAK,MAAMjS,KAAQN,EAAS,CACxB,MAAM4W,EAAU,EAAYtW,EAAKmW,IAC3BI,EAAY,EAAYvW,EAAKoW,IAE9BC,EAAa3S,IAAI4S,IAClBD,EAAalE,IAAImE,EAAS,IAAIrE,KAElCoE,EAAa1S,IAAI2S,GAASnE,IAAIoE,EAAWvW,EAAK4R,WAClD,CACA,OAAOyE,CACX,CAEO,SAASG,EAAgB9W,EAAS+W,EAAgBT,EAAiBjX,EAAME,EAAMD,EAASiQ,GAC3F,GAAuB,IAAnBvP,EAAQuF,OACR,OAAOhG,EAEX,MAAMoX,EAAeH,EAAgBxW,EAAS,WAAY,SACpDgX,EAAkB1X,EAAQ6E,QAAOrG,GAA0B,WAAhBA,EAAOyF,MAAqBoT,EAAa3S,IAAIlG,EAAO8E,OAErG,OAA+B,IAA3BoU,EAAgBzR,OACThG,EAEJA,EAAK4E,QAAOpG,IACf,IAAK,MAAMD,KAAUkZ,EAAiB,CAClC,MAAM1W,EAAOgW,EAAgBpS,QAAQ7E,EAAME,EAAMD,EAASvB,EAAKD,EAAQyR,GACjE0H,EAAgBN,EAAa1S,IAAInG,EAAO8E,KAG9C,IAFgBmU,EAAe7S,QAAQ7E,EAAME,EAAMD,EAASvB,EAAKD,EAAQwC,EAAKjD,MAAOiD,EAAKnC,KAAM8Y,GAG5F,OAAO,CACf,CACA,OAAO,CAAI,GAEnB,CAEO,SAASC,EAAmBlX,EAAS+W,EAAgBT,EAAiBjX,EAAME,EAAMD,EAASiQ,GAC9F,GAAuB,IAAnBvP,EAAQuF,OACR,OAAOjG,EAEX,MAAMqX,EAAeH,EAAgBxW,EAAS,QAAS,YACjDmX,EAAe5X,EAAK4E,QAAOpG,GAAoB,WAAbA,EAAIwF,MAAqBoT,EAAa3S,IAAIjG,EAAI6E,OAEtF,OAA4B,IAAxBuU,EAAa5R,OACNjG,EAEJA,EAAQ6E,QAAOrG,IAClB,IAAK,MAAMC,KAAOoZ,EAAc,CAC5B,MAAM7W,EAAOgW,EAAgBpS,QAAQ7E,EAAME,EAAMD,EAASvB,EAAKD,EAAQyR,GACjE6H,EAAaT,EAAa1S,IAAIlG,EAAI6E,KAGxC,IAFgBmU,EAAe7S,QAAQ7E,EAAME,EAAMD,EAASvB,EAAKD,EAAQwC,EAAKjD,MAAOiD,EAAKnC,KAAMiZ,GAG5F,OAAO,CACf,CACA,OAAO,CAAI,GAEnB,CC5De,SAASC,EAAa/S,EAAKE,EAAQC,EAAMF,GACpD,MAAO,CACHD,IAAKA,EACLE,OAAQA,EACRC,KAAMA,EACNF,MAAOA,EAEf,CCPe,SAAS+S,EAAahY,EAASC,GAC1C,MAAO,CACHoH,MAAOrH,EAAQiG,OAASjG,EAAQoS,IAAI,GAAGK,gBAAkB,EACzDrL,OAAQnH,EAAKgG,OAAShG,EAAKmS,IAAI,GAAGE,iBAAmB,EAE7D,CCHe,MAAM2F,EAEjB,WAAAnF,GACIC,KAAKnN,OAASkI,SAASoK,cAAc,UACrCnF,KAAK3U,QAAU2U,KAAKnN,OAAOW,WAAW,MACtCwM,KAAK9H,YAAc,IAAIgI,GAC3B,CAEA,YAAAkF,CAAatZ,EAAMmM,GACf,MAAM1E,EAAMyM,KAAK3U,QAMjB,OAJAkI,EAAI0E,KAAOA,GAAQlG,EAECwB,EAAI8R,YAAYvZ,GAEjBwI,KACvB,CAEA,aAAAgR,CAAcxZ,EAAMmM,GAChB,IAAIsN,EAAQ,EACZ,IAAK,MAAMC,KAAQ1Z,EACF,OAAT0Z,GACAD,IAGR,OAAOA,EAAQvF,KAAK7H,eAAeF,GAAM5D,MAC7C,CAEA,cAAA8D,CAAeF,GACX,MAAM1H,EAAM0H,EAEZ,GAAI+H,KAAK9H,YAAYvG,IAAIpB,GACrB,OAAOyP,KAAK9H,YAAYtG,IAAIrB,GAEhC,MAAMgD,EAAMyM,KAAK3U,QAGjBkI,EAAI0E,KAAOA,GAAQlG,EAEnB,MAAM0T,EAAclS,EAAI8R,YAAY,KAE9B/M,GAAUmN,EAAYC,yBAA2BD,EAAYE,yBAA2B,EAKxFzN,EAAc,CAChBK,UALcD,EAASmN,EAAYG,sBAMnCtN,QAASA,EACTE,aANiBiN,EAAYI,uBAAyBvN,EAOtDjE,OANWoR,EAAYG,sBAAwBH,EAAYI,wBAW/D,OAFA7F,KAAK9H,YAAYkI,IAAI7P,EAAK2H,GAEnBA,CACX,ECxDW,SAAS4N,IACpB,OAAO,IAAIZ,CACf,CCJO,SAASa,EAASC,EAAQhP,GAC7B,OACIA,EAAK/E,KAAO+T,EAAO/T,KACnB+E,EAAK5E,MAAQ4T,EAAO5T,MACpB4E,EAAK/E,IAAM+E,EAAK3C,QAAU2R,EAAO/T,IAAM+T,EAAO3R,QAC9C2C,EAAK5E,KAAO4E,EAAK1C,OAAS0R,EAAO5T,KAAO4T,EAAO1R,KAEvD,CAEO,SAAS2C,EAAK+O,EAAQhP,GACzB,MAAMiP,EAAU,CACZhU,IAAKM,KAAK+C,IAAI0Q,EAAO/T,IAAK+E,EAAK/E,KAC/BG,KAAMG,KAAK+C,IAAI0Q,EAAO5T,KAAM4E,EAAK5E,MACjCkC,MAAO/B,KAAK2T,IAAIF,EAAO5T,KAAO4T,EAAO1R,MAAO0C,EAAK5E,KAAO4E,EAAK1C,OAAS/B,KAAK+C,IAAI0Q,EAAO5T,KAAM4E,EAAK5E,MACjGiC,OAAQ9B,KAAK2T,IAAIF,EAAO/T,IAAM+T,EAAO3R,OAAQ2C,EAAK/E,IAAM+E,EAAK3C,QAAU9B,KAAK+C,IAAI0Q,EAAO/T,IAAK+E,EAAK/E,MAGrG,OAAIgU,EAAQ3R,OAAS,GAAK2R,EAAQ5R,QAAU,EACjC4R,EAEJ,CACHhU,IAAK+T,EAAO/T,IACZG,KAAM4T,EAAO5T,KACbkC,MAAO,EACPD,OAAQ,EAEhB,CAEO,SAAS8R,EAAOnP,EAAMoP,GACzB,MAAO,CACHnU,IAAK+E,EAAK/E,IAAMmU,EAChBhU,KAAM4E,EAAK5E,KAAOgU,EAClB9R,MAAO0C,EAAK1C,MAAiB,EAAT8R,EACpB/R,OAAQ2C,EAAK3C,OAAkB,EAAT+R,EAE9B,CAEO,SAAS,EAAKpP,GACjB,OAAOA,EAAK1C,MAAQ0C,EAAK3C,MAC7B,CAEO,SAASgS,EAASrP,EAAMoP,GAC3B,MAAO,CACHnU,IAAK+E,EAAK/E,IACVG,KAAM4E,EAAK5E,KACXkC,MAAO/B,KAAK+C,IAAI,EAAG0B,EAAK1C,MAAQ8R,EAAOhU,KAAOgU,EAAOlU,OACrDmC,OAAQ9B,KAAK+C,IAAI,EAAG0B,EAAK3C,OAAS+R,EAAOnU,IAAMmU,EAAOjU,QAE9D,CC9CA,MAAMmU,EAAiB,IACjBC,EAAkB,IAClBC,EAAY,CACdpU,KAAM,EACNH,IAAK,EACLqC,MAAO,EACPD,OAAQ,GCRG,SAASoS,EAAUpF,GAC9B,OAAOA,EAAS7M,QAAO,CAACyL,EAAQhR,IAAYgR,EAAOG,IAAInR,EAAQsB,IAAKtB,IAAU,IAAIiR,IACtF,CCAe,SAASwG,EAAoBC,EAAarJ,EAAY1N,EAAaoN,EAAa/P,EAASC,EAAMmE,EAAcC,GACxH,IAAKqV,EACD,MAAO,GACX,GAAIrJ,EACA,MAAO,GACX,IAAKN,EACD,MAAO,GACX,IAAKpN,EACD,MAAO,GAEX,MAAMuN,EAAmB,EAAYvN,EAAY4B,UAC3C4L,EAAgB,EAAYxN,EAAY8B,OACxCkV,EAAmB,EAAY5J,EAAYxL,UAC3CqV,EAAgB,EAAY7J,EAAYtL,OAE9C,IAAKL,EAAaM,IAAIwL,GAClB,MAAO,GACX,IAAK7L,EAAUK,IAAIyL,GACf,MAAO,GACX,IAAK/L,EAAaM,IAAIiV,GAClB,MAAO,GACX,IAAKtV,EAAUK,IAAIkV,GACf,MAAO,GAEX,MAAMC,EAAiBvU,KAAK2T,IAAI7U,EAAaO,IAAIuL,GAAkBrI,MAAOzD,EAAaO,IAAIgV,GAAkB9R,OACvGiS,EAAiBxU,KAAK+C,IAAIjE,EAAaO,IAAIuL,GAAkBrI,MAAOzD,EAAaO,IAAIgV,GAAkB9R,OACvGkS,EAAczU,KAAK2T,IAAI5U,EAAUM,IAAIwL,GAAetI,MAAOxD,EAAUM,IAAIiV,GAAe/R,OACxFmS,EAAc1U,KAAK+C,IAAIhE,EAAUM,IAAIwL,GAAetI,MAAOxD,EAAUM,IAAIiV,GAAe/R,OAE9F,OAAO7H,EAAQkI,MAAM2R,EAAgBC,EAAiB,GAAGG,SAAQzb,GACtDyB,EAAKiI,MAAM6R,EAAaC,EAAc,GAAG3b,KAAII,IACzC,CACHgG,MAAOhG,EAAI8D,GACXgC,SAAU/F,EAAO+D,QAIjC,CCvBe,SAAS2X,GAAe1b,EAAQC,GAC3C,MAAMqH,EAjBV,SAA4BrH,GACxB,MAAmB,UAAfA,EAAIsS,OACG,MACQ,QAAftS,EAAIsS,OACG,SACJ,QACX,CAW4BoJ,CAAmB1b,GACrCuH,EAVV,SAA8BxH,GAC1B,MAAsB,UAAlBA,EAAOuS,OACA,OACW,QAAlBvS,EAAOuS,OACA,QACJ,QACX,CAI8BqJ,CAAqB5b,GAE/C,MAAO,GAAGsH,KAAmBE,GACjC,CClBe,SAASqU,GAAkBC,EAAe3X,EAAayB,EAAcC,EAAW0B,GAC3F,IAAKpD,EACD,OAAO,KAEX,MAAMuN,EAAmB,EAAYvN,EAAY4B,UAC3C4L,EAAgB,EAAYxN,EAAY8B,OAE9C,IAAKL,EAAaM,IAAIwL,GAClB,OAAO,KACX,IAAK7L,EAAUK,IAAIyL,GACf,OAAO,KAEX,MAAM3R,EAAS4F,EAAaO,IAAIuL,GAC1BzR,EAAM4F,EAAUM,IAAIwL,GAE1B,GAA6B,IAAzBmK,EAAcrU,OACd,OAAO,KAEX,MAAMsU,EAAW,CACblT,MAAO7I,EAAO6I,MACdD,OAAQ3I,EAAI2I,OACZ8G,QAASgM,GAAe1b,EAAQC,IAGpC,OAAQA,EAAIsS,QACR,IAAK,QACDwJ,EAASvV,IAAMvG,EAAIuG,IACnB,MACJ,IAAK,MACDuV,EAASrV,OAASa,EAASf,IAAIoC,OAASrB,EAASsF,OAAOjE,OAASrB,EAASb,OAAOkC,OAAS3I,EAAIuG,IAAMvG,EAAI2I,OACxG,MACJ,QACImT,EAASlR,UAAY5K,EAAIuG,IAAMe,EAASf,IAAIoC,OAGpD,OAAQ5I,EAAOuS,QACX,IAAK,QACDwJ,EAASpV,KAAO3G,EAAO2G,KACvB,MACJ,IAAK,MACDoV,EAAStV,MAAQc,EAASZ,KAAKkC,MAAQtB,EAAS2M,OAAOrL,MAAQtB,EAASd,MAAMoC,MAAQ7I,EAAO2G,KAAO3G,EAAO6I,MAC3G,MACJ,QACIkT,EAASnR,WAAa5K,EAAO2G,KAAOY,EAASZ,KAAKkC,MAG1D,OAAOkT,CACX,CClDe,SAASC,GAAe3b,EAAMyb,GACzC,OAAOA,EAAcG,OAAMzZ,GAAQA,EAAKhC,KAAKE,SAAS,CAAEuQ,OAAQ5Q,KACpE,CCFA,SAAS6b,GAActG,GACnB,OAAK7Q,MAAMC,QAAQ4Q,GAGZA,EAAS/V,KAAI,CAAC2K,EAAGnB,IAAUA,IAFvBlE,OAAOC,KAAKwQ,EAG3B,CAEA,SAASuG,GAAiB5a,GACtB,OAAO2a,GAAc3a,EACzB,CAEA,SAAS6a,GAAoB7a,GACzB,GAAIwD,MAAMC,QAAQzD,GACd,OAAIA,EAAKkG,OAAS,EACPtC,OAAOC,KAAK7D,EAAK,IACrB,GACJ,CACH,MAAM6D,EAAOD,OAAOC,KAAK7D,GACzB,OAAI6D,EAAKqC,OAAS,EACPyU,GAAc3a,EAAK6D,EAAK,KAC5B,EACX,CACJ,CAEO,SAASiX,GAAmB7a,EAASD,GAGxC,IAFsBC,EAAQ8a,MAAKtc,GAA0B,eAAhBA,EAAOyF,OAGhD,OAAOjE,EAEX,MAAM+a,EAAkB,GAExB,IAAK,MAAMvc,KAAUwB,EACjB,GAAoB,eAAhBxB,EAAOyF,KAAuB,CAC9B,MAAM+W,EAAM,aAAcxc,EACpBA,EAAOyc,SAASlb,GAChB6a,GAAoB7a,GAE1B,IAAK,MAAMwC,KAAMyY,EACbD,EAAgBhT,KAAK,IACdvJ,EACH+D,KACA0B,KAAM,QAGlB,MACI8W,EAAgBhT,KAAKvJ,GAI7B,OAAOuc,CACX,CAEO,SAASG,GAAgBjb,EAAMF,GAGlC,IAFsBE,EAAK6a,MAAKrc,GAAoB,eAAbA,EAAIwF,OAGvC,OAAOhE,EAEX,MAAMkb,EAAe,GAErB,IAAK,MAAM1c,KAAOwB,EACd,GAAiB,eAAbxB,EAAIwF,KAAuB,CAC3B,MAAM+W,EAAM,aAAcvc,EACpBA,EAAIwc,SAASlb,GACb4a,GAAiB5a,GAEvB,IAAK,MAAMwC,KAAMyY,EACbG,EAAapT,KAAK,IACXtJ,EACH8D,KACA0B,KAAM,QAGlB,MACIkX,EAAapT,KAAKtJ,GAI1B,OAAO0c,CACX,CC7EA,MAAMC,GAAmB,EAAGvc,OAAM+T,gBAAiB/T,EAAKwc,SAASzI,GAElD,MAAM0I,GACjB,WAAAxI,CAAY+C,GACR9C,KAAKuD,YAAc,IAAIlB,EAEvB,IAAK,MAAM9W,KAAQuX,EAAO,CACtB,MAAMW,EAAQ,CACV+E,GAAI,EAAY,OAAQjd,EAAOA,EAAKid,GAAK,UACzC7c,UAAWJ,EAAKI,WAAa0c,IAGjCrI,KAAKuD,YAAYhB,QAAQhX,EAAKE,OAAQF,EAAKG,IAAK+X,EACpD,CACJ,CAEA,OAAA5R,CAAQ7E,EAAME,EAAMD,EAASvB,EAAKD,EAAQT,EAAOc,EAAMwY,GACnD,MAAMxB,EAAQ9C,KAAKuD,YAAYV,SAASpX,EAAQC,GAEhD,GAAqB,IAAjBoX,EAAM5P,OACN,MAAiB,SAAbxH,EAAIwF,MAEY,SAAhBzF,EAAOyF,OAENoT,EAAa3S,IAAI,aAGf0W,GAAiB,CAAEvc,OAAM+T,WAAYyE,EAAa1S,IAAI,cAGjE,IAAIvG,EAAU,CAAE2B,OAAME,OAAMD,UAASvB,MAAKD,SAAQT,QAAOc,QAEzD,IAAK,MAAMP,KAAQuX,EAAO,CACtB,IAAKwB,EAAa3S,IAAIpG,EAAKid,IACvB,SAEJ,MAAMC,EAAgB,IAAKpd,EAASwU,WAAYyE,EAAa1S,IAAIrG,EAAKid,KAEtE,IAAKjd,EAAKI,UAAU8c,GAChB,OAAO,CACf,CAEA,OAAO,CACX,EC5CW,SAASC,GAAkBlc,GACtC,OAAO,IAAI+b,GAAe/b,EAC9B,CCJe,SAASmc,GAAoBxd,GACxC,OAAOA,CACX,CCFe,SAASyd,GAAqBzd,GACzC,OAAOA,CACX,CCEO,SAAS0d,GAAmB5b,EAASC,EAAMyG,EAAcvC,EAAgB0X,EAAgBC,GAC5F,GAAI9b,EAAQya,OAAMjc,GAAkC,iBAAjBA,EAAO6I,QACtC,OAAOrH,EAEX,MAAM+b,EAAgBvd,IAClB,MAAMwd,EAAiB,UAAWxd,EAASA,EAAO6I,MAAQ,WAE1D,GAA8B,iBAAnB2U,EACP,OAAOA,EAEX,GAAIH,EAAenX,IAAIlG,EAAO8E,KAAM,CAChC,MAAM2Y,EAASJ,EAAelX,IAAInG,EAAO8E,KAEzC,GAAuB,aAAnB0Y,IAAkCC,EAAOC,SACzC,OAAOD,EAAO5U,MAClB,GAAuB,kBAAnB2U,GAAsCC,EAAOC,SAC7C,OAAOD,EAAO5U,KACtB,CAEA,IAAIA,EAAQ,EACZ,IAAK,MAAM5I,KAAOwB,EAAM,CACpB,GAAiB,SAAbxB,EAAIwF,MAAsC,kBAAnB+X,EACvB,SACJ,GAAiB,SAAbvd,EAAIwF,MAAsC,aAAnB+X,EACvB,SAEJ,MAAMhb,EAAOmD,EAAeS,QAAQnG,EAAKD,GACnCK,EAAOmC,EAAKnC,KACZmM,EAAOhK,EAAKgK,KACZjM,EAAUiC,EAAKjC,QAAQoG,KAAOnE,EAAKjC,QAAQkG,MAE3CmF,EAAY1D,EAAayR,aAAatZ,EAAMmM,GAAQjM,EAE1DsI,EAAQ/B,KAAK+C,IAAIhB,EAAO+C,EAC5B,CAOA,OALAyR,EAAe1I,IAAI3U,EAAO8E,IAAK,CAC3B+D,QACA6U,SAA6B,kBAAnBF,IAGP3U,CAAK,EAGhB,IAAK,MAAM/D,KAAOuY,EAAejY,OACxBkY,EAAYpX,IAAIpB,IACjBuY,EAAeM,OAAO7Y,GAG9B,OAAOtD,EAAQ3B,KAAIG,IAAU,IACtBA,EACH6I,MAAO0U,EAAcvd,MAE7B,CAEO,SAAS4d,GAAgBpc,EAASC,EAAMyG,EAAcvC,EAAgB0X,EAAgBC,GACzF,GAAI7b,EAAKwa,OAAMhc,GAA6B,iBAAfA,EAAI2I,SAC7B,OAAOnH,EAEX,MAAMoc,EAAa5d,IACf,MAAM6d,EAAkB,WAAY7d,EAAMA,EAAI2I,OAAS,WAEvD,GAA+B,iBAApBkV,EACP,OAAOA,EAEX,GAAIT,EAAenX,IAAIjG,EAAI6E,KAAM,CAC7B,MAAM2Y,EAASJ,EAAelX,IAAIlG,EAAI6E,KAEtC,GAAwB,aAApBgZ,IAAmCL,EAAOC,SAC1C,OAAOD,EAAO7U,OAClB,GAAwB,kBAApBkV,GAAuCL,EAAOC,SAC9C,OAAOD,EAAO7U,MACtB,CAEA,IAAIA,EAAS,EACb,IAAK,MAAM5I,KAAUwB,EAAS,CAC1B,GAAoB,SAAhBxB,EAAOyF,MAAuC,kBAApBqY,EAC1B,SACJ,GAAoB,SAAhB9d,EAAOyF,MAAuC,aAApBqY,EAC1B,SAEJ,MAAMtb,EAAOmD,EAAeS,QAAQnG,EAAKD,GACnCK,EAAOmC,EAAKnC,KACZmM,EAAOhK,EAAKgK,KACZjM,EAAUiC,EAAKjC,QAAQiG,IAAMhE,EAAKjC,QAAQmG,OAE1CmF,EAAa3D,EAAa2R,cAAcxZ,EAAMmM,GAAQjM,EAE5DqI,EAAS9B,KAAK+C,IAAIjB,EAAQiD,EAC9B,CAOA,OALAwR,EAAe1I,IAAI1U,EAAI6E,IAAK,CACxB8D,SACA8U,SAA8B,kBAApBI,IAGPlV,CAAM,EAGjB,IAAK,MAAM9D,KAAOuY,EAAejY,OACxBkY,EAAYpX,IAAIpB,IACjBuY,EAAeM,OAAO7Y,GAG9B,OAAOrD,EAAK5B,KAAII,IAAO,IAChBA,EACH2I,OAAQiV,EAAW5d,MAE3B,CChHe,SAAS8d,GAAQhG,GAC5B,OAAO,IAAI7C,IAAI6C,EAAQlY,KAAImY,GAASA,EAAMlT,MAC9C,CCFe,SAASkZ,GAAqBte,GACzC,OAAOA,CACX,CCAA,MAAMue,GAAuB,CAACC,EAAKC,IAAQD,EAAI3e,MAAQ4e,EAAI5e,MACrD6e,GAAwB,CAACF,EAAKC,IAAQD,EAAI3e,MAAQ4e,EAAI5e,MAE7C,MAAM8e,GACjB,WAAA/J,CAAY+C,GACR9C,KAAKuD,YAAc,IAAIlB,EAEvB,IAAK,MAAM9W,KAAQuX,EAAO,CACtB,MAAMW,EAAQ,CACV+E,GAAIuB,YAAY,OAAQxe,EAAOA,EAAKid,GAAK,UACzCwB,cAAeze,EAAK0e,YAAcP,GAClCQ,eAAgB,CAACP,EAAKC,KAASre,EAAK0e,WAAWN,EAAKC,IAAQC,IAGhE7J,KAAKuD,YAAYhB,QAAQhX,EAAKE,OAAQF,EAAKG,IAAK+X,EACpD,CACJ,CAEA,OAAA5R,CAAQpG,EAAQC,EAAKye,GACjB,MAAMrH,EAAQ9C,KAAKuD,YAAYV,SAASpX,EAAQC,GAEhD,GAAqB,IAAjBoX,EAAM5P,OACN,MAAiB,SAAbxH,EAAIwF,MAEY,SAAhBzF,EAAOyF,KADA,KAGNiZ,EAAaxY,IAAI,YAGkB,QAAjCwY,EAAavY,IAAI,YAClB8X,GACAG,GAJK,KAOf,GAAI/G,EAAM5P,OAAS,EACf,MAAM,IAAIkX,MAAM,4CAEpB,MAAM7e,EAAOuX,EAAM,GAEnB,MAAqC,QAA9BqH,EAAavY,IAAIrG,EAAKid,IACvBjd,EAAKye,cACLze,EAAK2e,cACf,EC1CW,SAASG,GAAgB5a,GACpC,OAAO,IAAIqa,GAAara,EAC5B,CCFA,SAAS6a,GAAgBta,EAAQoU,EAAYC,GACzC,MAAM8F,EAAe,IAAIjK,IACzB,IAAK,MAAMjS,KAAQ+B,EAAQ,CACvB,MAAMuU,EAAU,EAAYtW,EAAKmW,IAC3BI,EAAY,EAAYvW,EAAKoW,IAE9B8F,EAAaxY,IAAI4S,IAClB4F,EAAa/J,IAAImE,EAAS,IAAIrE,KAElCiK,EAAavY,IAAI2S,GAASnE,IAAIoE,EAAWvW,EAAKuO,UAClD,CACA,OAAO2N,CACX,CAEA,SAASI,GAAMC,EAAM5G,GACjB4G,EAAK1Z,MAAK,CAAC6Y,EAAKC,KACZ,MAAMhG,EAAS+F,EAAIM,WAAWN,EAAI1b,KAAM2b,EAAI3b,MAC5C,MAAsB,iBAAX2V,EACAA,EACJA,GAAU,EAAI,CAAC,IAE1BA,EAAO5O,QAAQwV,EAAKlf,KAAImY,GAASA,EAAMgH,UACvCD,EAAKtX,OAAS,CAClB,CAEO,SAASwX,GAAc1a,EAAQ2a,EAAc1G,EAAiBjX,EAAME,EAAMD,EAASiQ,GACtF,GAAsB,IAAlBlN,EAAOkD,OACP,OAAOhG,EAEX,MAAMid,EAAeG,GAAgBta,EAAQ,WAAY,SACnDqB,EAAe,IAAI6O,IAAIjT,EAAQ3B,KAAIG,GAAU,CAACA,EAAO8E,IAAK9E,MAC1Dmf,EAAgB5a,EACjB1E,KAAI2C,GAAQ,EAAYA,EAAKuD,YAC7BM,QAAOvB,GAAOc,EAAaM,IAAIpB,KAC/BjF,KAAIiF,GAAOc,EAAaO,IAAIrB,KAC5Bsa,UAEL,GAA6B,IAAzBD,EAAc1X,OACd,OAAOhG,EAEX,IAAK,MAAMzB,KAAUmf,EAAe,CAChC,MAAMhH,EAAS,GACT4G,EAAO,GAEb,IAAK,MAAM9e,KAAOwB,EAAM,CACpB,MAAM+c,EAAaU,EAAa9Y,QAAQpG,EAAQC,EAAKye,EAAavY,IAAInG,EAAO8E,MAE7E,IAAK0Z,EAAY,CACbM,GAAMC,EAAM5G,GACZA,EAAO5O,KAAKtJ,GACZ,QACJ,CAEA,MACM+X,EAAQ,CAAEgH,OAAQ/e,EAAKue,aAAYhc,KAD5BgW,EAAgBpS,QAAQ7E,EAAME,EAAMD,EAASvB,EAAKD,EAAQyR,IAGnD,IAAhBsN,EAAKtX,QAKLsX,EAAK,GAAGP,aAAeA,GAK3BM,GAAMC,EAAM5G,GACZ4G,EAAKxV,KAAKyO,IAVN+G,EAAKxV,KAAKyO,EAWlB,CAEA8G,GAAMC,EAAM5G,GACZ1W,EAAO0W,CACX,CAEA,OAAO1W,CACX,CAEO,SAAS4d,GAAiB9a,EAAQ2a,EAAc1G,EAAiBjX,EAAME,EAAMD,EAASiQ,GACzF,GAAsB,IAAlBlN,EAAOkD,OACP,OAAOjG,EAEX,MAAMkd,EAAeG,GAAgBta,EAAQ,QAAS,YAChDsB,EAAY,IAAI4O,IAAIhT,EAAK5B,KAAII,GAAO,CAACA,EAAI6E,IAAK7E,MAC9Cqf,EAAa/a,EACd1E,KAAI2C,GAAQ,EAAYA,EAAKyD,SAC7BI,QAAOvB,GAAOe,EAAUK,IAAIpB,KAC5BjF,KAAIiF,GAAOe,EAAUM,IAAIrB,KACzBsa,UAEL,GAA0B,IAAtBE,EAAW7X,OACX,OAAOjG,EAEX,IAAK,MAAMvB,KAAOqf,EAAY,CAC1B,MAAMnH,EAAS,GACT4G,EAAO,GAEb,IAAK,MAAM/e,KAAUwB,EAAS,CAC1B,MAAMgd,EAAaU,EAAa9Y,QAAQpG,EAAQC,EAAKye,EAAavY,IAAIlG,EAAI6E,MAE1E,IAAK0Z,EAAY,CACbM,GAAMC,EAAM5G,GACZA,EAAO5O,KAAKvJ,GACZ,QACJ,CAEA,MACMgY,EAAQ,CAAEgH,OAAQhf,EAAQwe,aAAYhc,KAD/BgW,EAAgBpS,QAAQ7E,EAAME,EAAMD,EAASvB,EAAKD,EAAQyR,IAGnD,IAAhBsN,EAAKtX,QAKLsX,EAAK,GAAGP,aAAeA,GAK3BM,GAAMC,EAAM5G,GACZ4G,EAAKxV,KAAKyO,IAVN+G,EAAKxV,KAAKyO,EAWlB,CAEA8G,GAAMC,EAAM5G,GACZ3W,EAAU2W,CACd,CAEA,OAAO3W,CACX,CC/HA,MAAM+d,GAAa,EAIZ,SAASC,GAAmBhe,EAASoE,EAAcC,EAAW0L,EAAakO,GAC9E,IAAKlO,EACD,OAAO,KAEX,MAAMvR,EAAS4F,EAAaO,IAAI,EAAYoL,EAAYxL,WAClD9F,EAAM4F,EAAUM,IAAI,EAAYoL,EAAYtL,QAC5CkF,EAAIsU,EAActU,EAExB,MAAiB,WAAblL,EAAIwF,KACG,KAEP0F,GAAKnL,EAAOyG,MAAQ8Y,IAAcpU,GAAKnL,EAAOyG,MAAQ8Y,GAC/Cvf,EAAO+D,GAEG,IAAjB/D,EAAOqJ,OAEP8B,EAAInL,EAAO2G,KAAO4Y,IAAcpU,EAAInL,EAAO2G,KAAO4Y,GAD3C,KAIJ/d,EAAQxB,EAAOqJ,MAAQ,GAAGtF,EACrC,CAEO,SAAS2b,GAAgBje,EAAMmE,EAAcC,EAAW0L,EAAakO,GACxE,IAAKlO,EACD,OAAO,KAEX,MAAMvR,EAAS4F,EAAaO,IAAI,EAAYoL,EAAYxL,WAClD9F,EAAM4F,EAAUM,IAAI,EAAYoL,EAAYtL,QAC5CmF,EAAIqU,EAAcrU,EAExB,MAAoB,WAAhBpL,EAAOyF,KACA,KAEP2F,GAAKnL,EAAIyG,OAAS6Y,IAAcnU,GAAKnL,EAAIyG,OAAS6Y,GAC3Ctf,EAAI8D,GAEG,IAAd9D,EAAIoJ,OAEJ+B,EAAInL,EAAIuG,IAAM+Y,IAAcnU,EAAInL,EAAIuG,IAAM+Y,GADnC,KAIJ9d,EAAKxB,EAAIoJ,MAAQ,GAAGtF,EAC/B,CChDe,SAAS4b,GAAkBpb,GACtC,OAAOA,EAAO1E,KAAIwF,IAAQ,CACtBU,SAAU,aAAcV,EAAOA,EAAKU,SAAW,SAC/CE,MAAO,UAAWZ,EAAOA,EAAKY,MAAQ,SACtC8K,UAAW1L,EAAK0L,aAExB,CCNe,SAAS6O,GAAmB1d,GACvC,OAAOA,EAAQrC,KAAIwG,IAAU,CACzBN,SAAU,aAAcM,EAASA,EAAON,SAAW,SACnDE,MAAO,UAAWI,EAASA,EAAOJ,MAAQ,SAC1CmO,WAAY/N,EAAO+N,cAE3B,CCIO,SAASyL,GAAiBre,EAASse,GACtC,OAXJ,SAAmB/H,EAAS+H,GACxB,MAAMtD,EAAMzE,EACP1R,QAAO2R,GAAwB,SAAfA,EAAMvS,OACtB5F,KAAImY,GAASA,EAAMjU,KAIxB,OAFA+b,EAAStD,GAEFA,CACX,CAGWuD,CAAUve,EAASse,EAC9B,CC0BA,SAASE,GAAoBpgB,GACzBsB,QAAQC,MAAM,eAEd,MAAM8e,EAAU,IAAKrgB,EAAQsgB,gBAAiBtgB,EAAQugB,iBAChDC,EAASxgB,EAAQwgB,OACjBC,EAAgBzgB,EAAQuH,MAG9B,SAASmZ,EAAMxb,EAAKyb,EAAMC,GACtB,MAAMC,EAAuBL,EAAOtb,IAAQsb,EAAOtb,GAAK0b,aAGxD,OAFKC,IAAwBD,EAAalE,MAAK,CAACoE,EAAYrX,IAAUqX,IAAeD,EAAqBpX,OACtG+W,EAAOtb,GAAO,CAAEvF,MAAOghB,KAAQC,GAAeA,iBAC3CJ,EAAOtb,GAAKvF,KACvB,CAEA,MAAMsH,EAAmBhC,OAAOgC,iBAC1B3C,EAAc+b,EAAQ/b,YAAc2C,EACpCtF,EAAO0e,EAAQ1e,KACflB,EAAOT,EAAQuP,MAAM5P,MACrBgF,EAAS+b,EAAM,SAAUX,GAAmB,CAACM,EAAQ1b,SACrDrC,EAAUoe,EAAM,UAAWV,GAAoB,CAACK,EAAQ/d,UACxDgG,EAAeoY,EAAM,eAAgBjG,EAAiB,IACtD/B,EAAiBgI,EAAM,iBAAkB3P,EAAmB,CAACsP,EAAQvgB,WAAYugB,EAAQhc,aAAcM,IACvGyQ,EAAwBsL,EAAM,wBAAyBnM,EAA0B,CAAC8L,EAAQ3b,YAAapC,IACvGuP,EAAU6O,EAAM,UAAWvL,EAAY,CAACC,IACxC2L,EAAiBL,EAAM,iBAAkBhL,EAAY,CAAC2K,EAAQze,QAASD,IACvEqf,EAAcN,EAAM,cAAehL,EAAY,CAAC2K,EAAQxe,KAAMF,IAG9Dgb,EAAkB+D,EAAM,kBAAmBjE,GAAoB,CAACsE,EAAgBpf,IAChFob,EAAe2D,EAAM,eAAgB5D,GAAiB,CAACkE,EAAarf,IACpEsf,EAAoBP,EAAM,oBAAqBxK,EAAoB,CAACyG,EAAiB0D,EAAQne,WAAYme,EAAQje,YAAaie,EAAQzb,eACtIsc,EAAiBR,EAAM,iBAAkBtK,EAAiB,CAAC2G,EAAcsD,EAAQve,UAAWue,EAAQre,aAAcqe,EAAQxb,aAC1Hsc,EAAuBT,EAAM,uBAAwBvC,GAAS,CAAC8C,IAC/DG,EAAoBV,EAAM,oBAAqBvC,GAAS,CAAC+C,IAGzDG,EAAmBX,EAAM,mBAAoBpD,GAAqB,CAAC5E,IACnE4I,GAAwBZ,EAAM,wBAAyBjI,EAAoB,CAAC4I,IAC5EhI,GAAiBqH,EAAM,iBAAkBrD,GAAmB,CAACgD,EAAQlf,YACrEmY,GAAkBoH,EAAM,kBAAmBlH,EAAoB,CAAClX,EAAS+W,GAAgBiI,GAAuB3f,EAAMuf,EAAgBD,EAAmBpP,IACzJ4H,GAAeiH,EAAM,eAAgBtH,EAAiB,CAAC9W,EAAS+W,GAAgBiI,GAAuB3f,EAAMuf,EAAgBD,EAAmBpP,IAGhJ0P,GAAoBb,EAAM,oBAAqBtC,GAAsB,CAAC1F,IACtE8I,GAAyBd,EAAM,yBAA0BjI,EAAoB,CAAC8I,KAC9EjC,GAAeoB,EAAM,eAAgB1B,GAAiB,CAACqB,EAAQjc,UAK/Dqd,GAJgBf,EAAM,gBAAiBjB,GAAkB,CAAC9a,EAAQ2a,GAAckC,GAAwB7f,EAAM8X,GAAcH,GAAiBzH,IAK7I6P,GAJahB,EAAM,aAAcrB,GAAe,CAAC1a,EAAQ2a,GAAckC,GAAwB7f,EAAM8X,GAAcH,GAAiBzH,IAOpI8P,GAAoBjB,EAAM,oBAAqBnD,GAAsB,CAAC7E,IACtEkJ,GAAyBlB,EAAM,yBAA0BjI,EAAoB,CAACkJ,KAC9EE,GAAwBnB,EAAM,wBAAyB7H,EAAmB,CAAC+I,GAAwBjgB,EAAM+f,GAAYD,GAAe5P,IACpIiQ,GAAmB9hB,EAAQ8hB,iBAC3BC,GAAiB/hB,EAAQ+hB,eACzBC,GAAkBtB,EAAM,kBAAmBlD,GAAoB,CAACiE,GAAeC,GAAYpZ,EAAcuZ,GAAuBC,GAAkBX,IAClJc,GAAevB,EAAM,eAAgB1C,GAAiB,CAACyD,GAAeC,GAAYpZ,EAAcuZ,GAAuBE,GAAgBX,IAGvIxf,GAAU8e,EAAM,UAAWpK,EAAkB,CAAC0L,GAAiB/a,EAAkB3C,IACjFzC,GAAO6e,EAAM,OAAQlK,EAAe,CAACyL,GAAchb,EAAkB3C,IACrE0B,GAAe0a,EAAM,eAAgBtF,EAAW,CAACxZ,KACjDqE,GAAYya,EAAM,YAAatF,EAAW,CAACvZ,KAC3C0C,GAAc8b,EAAQ9b,YACtBoD,GAAW+Y,EAAM,WAAYjO,EAAa,CAAC7Q,GAASC,KACpD2C,GAAgB6b,EAAQ7b,cACxB0d,GAAYxB,EAAM,YAAa/G,EAAc,CAAChS,GAASf,IAAIoC,OAAQrB,GAASb,OAAOkC,OAAQrB,GAASZ,KAAKkC,MAAOtB,GAASd,MAAMoC,QAC/HkZ,GAAYzB,EAAM,YAAa9G,EAAc,CAAChY,GAASC,KAEvD8P,GC7GK,SAAwB/N,EAASic,EAAehe,EAAMD,EAASsgB,EAAWC,GAGrF,IAAKtC,EACD,OAAO,KACX,GAAIA,EAActU,EAAI,GAAKsU,EAAcrU,EAAI,GAAKqU,EAActU,EAAI4W,EAAUlZ,OAAS4W,EAAcrU,EAAI2W,EAAUnZ,OAC/G,OAAO,KAEX,MAAMoZ,EACIxe,EAAQye,WADZD,EAEGxe,EAAQ0e,UAGXC,EACK3e,EAAQ4e,YADbD,EAEM3e,EAAQ6e,aAGdlX,EAAIsU,EAActU,GAAK2W,EAAUnb,KACjC8Y,EAActU,EACdsU,EAActU,GAAKgX,EAAmBL,EAAUrb,MAC5Csb,EAAUlZ,MAAQsZ,EAAmB1C,EAActU,EACnDsU,EAActU,EAAI6W,EAOtBM,EChCK,SAAqB7gB,EAAM2J,GACtC,GAAoB,IAAhB3J,EAAKgG,OACL,OAAQ,EACZ,GAAI2D,EAAI3J,EAAK,GAAGoS,cACZ,OAAQ,EACZ,GAAIzI,EAAI3J,EAAKA,EAAKgG,OAAS,GAAGqM,iBAC1B,OAAQ,EAEZ,IAAIyO,EAAQ,EACRC,EAAQ/gB,EAAKgG,OAAS,EAE1B,KAAO8a,GAASC,GAAO,CACnB,MAAMC,EAAQ3b,KAAK4b,OAAOH,EAAQC,GAAS,GAE3C,GAAIpX,EAAI3J,EAAKghB,GAAO5O,cAChB2O,EAAQC,EAAQ,MACf,MAAIrX,EAAI3J,EAAKghB,GAAO3O,kBAIrB,OAAO2O,EAHPF,EAAQE,EAAQ,CAGJ,CACpB,CAEA,OAAQ,CACZ,CDQ0BE,CAAYlhB,EANxBge,EAAcrU,GAAK0W,EAAUtb,IACjCiZ,EAAcrU,EACdqU,EAAcrU,GAAK+W,EAAoBL,EAAUpb,OAC7Cqb,EAAUnZ,OAASuZ,EAAoB1C,EAAcrU,EACrDqU,EAAcrU,EAAI4W,GAGtBY,EEjCK,SAAwBphB,EAAS2J,GAC5C,GAAuB,IAAnB3J,EAAQiG,OACR,OAAQ,EACZ,GAAI0D,EAAI3J,EAAQ,GAAGwS,eACf,OAAQ,EACZ,GAAI7I,EAAI3J,EAAQA,EAAQiG,OAAS,GAAGwM,gBAChC,OAAQ,EAEZ,IAAIsO,EAAQ,EACRC,EAAQhhB,EAAQiG,OAAS,EAE7B,KAAO8a,GAASC,GAAO,CACnB,MAAMC,EAAQ3b,KAAK4b,OAAOH,EAAQC,GAAS,GAE3C,GAAIrX,EAAI3J,EAAQihB,GAAOzO,eACnBwO,EAAQC,EAAQ,MACf,MAAItX,EAAI3J,EAAQihB,GAAOxO,iBAIxB,OAAOwO,EAHPF,EAAQE,EAAQ,CAGJ,CACpB,CAEA,OAAQ,CACZ,CFS6BI,CAAerhB,EAAS2J,GAEjD,OAAuB,IAAnBmX,IAA8C,IAAtBM,EACjB,KAEJ,CACH3c,MAAOxE,EAAK6gB,GAAeve,GAC3BgC,SAAUvE,EAAQohB,GAAkB7e,GAE5C,CDsEwB+e,CAAeljB,EAAQ4D,QAAS5D,EAAQ6f,cAAehe,GAAMD,GAASsgB,GAAWC,IAC/F/R,GAAkBpQ,EAAQmjB,gBAAkBzC,EAAM,kBAAmBd,GAAoB,CAAChe,GAASoE,GAAcC,GAAW0L,GAAa3R,EAAQ6f,gBACjJxP,GAAerQ,EAAQojB,aAAe1C,EAAM,eAAgBZ,GAAiB,CAACje,GAAMmE,GAAcC,GAAW0L,GAAa3R,EAAQ6f,gBAGlIpb,GAAmBic,EAAM,mBAAoBrF,EAAqB,CAFpDrb,EAAQsb,cACPlL,MAAqBC,GACwD9L,GAAaoN,GAAa/P,GAASC,GAAMmE,GAAcC,KACnJ2L,GAAY8O,EAAM,YAAajL,EAAc,CAACjR,KAC9C8H,GAAYoU,EAAM,YAAajL,EAAc,CAAChR,KAE9C4e,GAAmB3C,EAAM,mBAAoBhP,EAAqB,CAACgH,EAAgB/G,GAAapN,GAAaqN,GAAWtF,GAAWuF,EAASzB,GAAiBC,KAC7JiT,GAAwB5C,EAAM,wBAAyBjI,EAAoB,CAAC4K,KAC5E9a,GAAuBmY,EAAM,uBAAwB7H,EAAmB,CAACyK,GAAuB3hB,EAAME,GAAMD,GAASiQ,IACrH0R,GAAkB7C,EAAM,kBAAmBpP,EAAoB,CAACoH,IAChE8K,GAAuB9C,EAAM,uBAAwBjI,EAAoB,CAAC8K,KAC1EE,GAAsB/C,EAAM,sBAAuB7H,EAAmB,CAAC2K,GAAsB7hB,EAAME,GAAMD,GAASiQ,IAClHqK,GAAgBwE,EAAM,gBAAiB5a,EAAkB,CAACtB,GAAeif,GAAqBzd,GAAcC,KAC5GuJ,GAAiBkR,EAAM,iBAAkBzE,GAAmB,CAACC,GAAe3X,GAAayB,GAAcC,GAAW0B,KAClHuI,GAAcwQ,EAAM,cAAetE,GAAgB,CAAC3b,EAAMyb,KAG1D7T,GrBzHK,SAAuBqb,EAAUvB,EAAWD,EAAWte,GAElE,MAAM+f,EAAO,CACT1a,MAAOrF,EAAQggB,wBAAwB3a,MACvCD,OAAQpF,EAAQggB,wBAAwB5a,QAEtCoZ,EAAe,CACjBrb,KAAMnD,EAAQye,WACdzb,IAAKhD,EAAQ0e,WAGXuB,EAAiBH,GAAYvI,EAG7BR,EAASK,EADG,CAAEjU,KAAM,EAAGH,IAAK,KAAMub,GACLD,GAC7B7Z,EAAa2S,EAAS,IAAKoH,KAAiBuB,GAAQzB,GACpD4B,EAAqBlY,EAAK+O,EAAQG,EAAOzS,EAAY4S,IACrD8I,EAAsBnY,EAAK+O,EAAQG,EAAOzS,EAAY6S,IAE5D,OAAKR,EAASC,EAAQkJ,IAGjBnJ,EAASmJ,EAAgBC,GAG1B,EAAKD,GAAkB,EAAI,EAAKE,GACzBA,EAEJF,EARIE,CASf,CqB4FuBC,CAAcvD,GAAepY,WAAY8Z,GAAWD,GAAWliB,EAAQ4D,SAG1F8c,EAAM,gBAAiBT,GAAkB,CAACre,GAASye,EAAQld,wBAC3Dud,EAAM,aAAcT,GAAkB,CAACpe,GAAMwe,EAAQ/c,qBAErDtD,EAAQuH,MAAQ,CACZ8Y,UACApZ,mBACA3C,cACA3C,OACA+W,iBACA7G,UACAyH,mBACAG,gBACA7X,WACAC,QACA8F,YACAnD,iBACAoN,aACAtF,aACAqF,eACApN,eACA8e,oBACA9a,wBACAgb,mBACAE,uBACAvB,aACAC,aACA7Z,eACAD,cACA5D,oBACA+K,kBACAxJ,gBACAC,aACAxF,OACAyP,eACAE,mBACAC,gBAER,CAEe,SAAS4T,GAAYjkB,GAChC,IAAKA,EAAQsP,MACT,IACI8Q,GAAoBpgB,EACxB,CAAE,MAAOsP,GACLtP,EAAQsP,MAAQA,CACpB,CAER,CIpLe,SAAS4U,GAAiBC,EAAeC,GACpD,MAAMxS,EAAY,IAAIyD,EAAU+O,GAChC,MAAO,IAAIA,KAAaD,EAAc1d,QAAO7D,IAASgP,EAAU4D,aAAa5S,EAAKyD,MAAOzD,EAAKuD,YAClG,CCHe,SAASke,GAAgBF,EAAeG,GACnD,MAAM1S,EAAY,IAAIyD,EAAUiP,GAChC,OAAOH,EAAc1d,QAAO7D,IAASgP,EAAU4D,aAAa5S,EAAKyD,MAAOzD,EAAKuD,WACjF,CCLe,SAASoe,GAAiBC,GACrC,MACM7Y,EADU6Y,EAAMC,cACDb,wBACrB,MAAO,CACHrY,EAAGiZ,EAAME,QAAU/Y,EAAK5E,KACxByE,EAAGgZ,EAAMG,QAAUhZ,EAAK/E,IAEhC,CCGA,SAASge,GAAWhhB,GAChB,GAAI,wBAAyBA,EAAS,OAEtCtC,QAAQ2G,IAAI,cAEZ,MAAMR,EAAW,CACb,WAAYiI,SAASoK,cAAc,UACnC,aAAcpK,SAASoK,cAAc,UACrC,YAAapK,SAASoK,cAAc,UACpC,cAAepK,SAASoK,cAAc,UACtC,gBAAiBpK,SAASoK,cAAc,UACxC,eAAgBpK,SAASoK,cAAc,UACvC,cAAepK,SAASoK,cAAc,UACtC,gBAAiBpK,SAASoK,cAAc,UACxC,eAAgBpK,SAASoK,cAAc,WAErCvK,EAAQG,SAASoK,cAAc,SAErClW,EAAQihB,aAAa,WAAY,KACjCjhB,EAAQihB,aAAa,QAAS,oQAC9BjhB,EAAQkhB,UAAUvP,IAAI,eACtB9N,EAAS,YAAYod,aAAa,QAAS,+EAC3Cpd,EAAS,cAAcod,aAAa,QAAS,sEAC7Cpd,EAAS,aAAaod,aAAa,QAAS,gFAC5Cpd,EAAS,eAAeod,aAAa,QAAS,uEAC9Cpd,EAAS,iBAAiBod,aAAa,QAAS,4CAChDpd,EAAS,gBAAgBod,aAAa,QAAS,wEAC/Cpd,EAAS,eAAeod,aAAa,QAAS,kFAC9Cpd,EAAS,iBAAiBod,aAAa,QAAS,yEAChDpd,EAAS,gBAAgBod,aAAa,QAAS,mFAC/CtV,EAAMsV,aAAa,QAAS,0NAE5B,MAAM7kB,EAAU,CACZugB,gBAAiB,CAAC,EAClBhZ,MAAO,KACPiZ,OAAQ,CAAC,EACT5c,QAASA,EACT6D,SAAUA,EACV8H,MAAOA,EACPwV,iBAAiB,EACjBlF,cAAe,KACfvE,aAAa,EACbwG,iBAAkB,IAAIjN,IACtBkN,eAAgB,IAAIlN,IAGxB7U,iBAA2B,KACnBA,EAAQ+kB,kBACZ/kB,EAAQ+kB,iBAAkB,EAC1BC,uBAAsB,KAClBhlB,EAAQ+kB,iBAAkB,EAC1Bd,GAAYjkB,GACZqP,EAAOrP,EAAQ,IACjB,EAGNA,iBAA2B,CAAC4D,EAASiC,EAAMof,KACvCrhB,EAAQshB,iBAAiBrf,GAAO2e,IAC5B,IACIS,EAAST,EACb,CACA,MAAOlV,GACHA,EAAMsB,QAAU,IAAI/K,aAAgByJ,EAAMsB,UAC1C5Q,EAAQsP,MAAQA,EAChBtP,EAAQmlB,kBACZ,IACF,GAGNnlB,EAAQsgB,aAAe,CACnB3e,KAAM,GACNC,QAAS,CAAC,CAAEiE,KAAM,eAClBhE,KAAM,CAAC,CAAEgE,KAAM,UAAY,CAAEA,KAAM,eACnC/F,WAAY,GACZqB,UAAW,GACXiD,QAAS,GACTC,aAAc,EAAG1C,OAAMtB,MAAKD,YAAauB,EAAKtB,EAAI8D,IAAI/D,EAAO+D,IAC7DrC,UAAW,EACXE,aAAc,EACdE,WAAY,EACZE,YAAa,EACbkC,YAAa,EACbC,YAAa,KACb6gB,oBAAsB7gB,IAClBvE,EAAQsgB,aAAa/b,YAAcA,EACnCvE,EAAQmlB,kBAAkB,EAE9B3gB,cAAe,GACf6gB,sBAAwB7gB,IACpBxE,EAAQsgB,aAAa9b,cAAgBA,EACrCxE,EAAQmlB,kBAAkB,EAE9B1gB,iBAAkB,GAClBC,YAAa,GACb4gB,oBAAsB5gB,IAElB1E,EAAQsgB,aAAa5b,YAAcA,EACnC1E,EAAQmlB,kBAAkB,EAE9B7iB,QAAS,GACTC,gBAAkBD,IACdtC,EAAQsgB,aAAahe,QAAUA,EAC/BtC,EAAQmlB,kBAAkB,EAE9BxgB,OAAQ,GACR4gB,eAAiB5gB,IACb3E,EAAQsgB,aAAa3b,OAASA,EAC9B3E,EAAQmlB,kBAAkB,EAE9BxiB,YAAa,OACbO,kBAAmB,OACnB0B,aAAc,GACd4gB,qBAAuB5gB,IACnB5E,EAAQsgB,aAAa1b,aAAeA,EACpC5E,EAAQmlB,kBAAkB,EAE9BtgB,WAAY,GACZ4gB,mBAAqB5gB,IACjB7E,EAAQsgB,aAAazb,WAAaA,EAClC7E,EAAQmlB,kBAAkB,EAE9BhiB,sBAAuB,OACvBG,mBAAoB,QAGxBM,EAAQ,uBAAyB5D,EAEjC,MAAM0lB,EAAWjlB,IACb8O,EAAM5P,MAAQc,EACd8O,EAAMoW,cAAc,IAAIC,MAAM,SAAS,EAGrCC,EAAU7kB,IACZ,MAAMwD,EAAgBxE,EAAQuH,MAAM8Y,QAAQ7b,cACtCuB,EAAiB/F,EAAQuH,MAAMkc,oBAC/Bzd,EAAehG,EAAQuH,MAAMvB,aAC7BC,EAAYjG,EAAQuH,MAAMtB,UAC1BxF,EAAOT,EAAQuH,MAAM9G,KACrByP,EAAclQ,EAAQuH,MAAM2I,YAC5B4V,EAAiB9lB,EAAQuH,MAAM8Y,QAAQiF,oBACvCS,EAAa/lB,EAAQuH,MAAM8Y,QAAQ9d,gBAGnC2Z,EAAgBpW,EAAiBtB,EAAeuB,EAAgBC,EAAcC,GAEpF,GAAa,KAATxF,EACA,OACJ,IAAKyP,EACD,OACJ,GAAIlP,IAAekb,EAAcG,OAAMzZ,GAAQA,EAAKhC,KAAKI,aACrD,OAEJ,MAAMglB,EAAY9J,EAAczV,QAAO7D,GAAsB,SAAdA,EAAKiD,OAC9CogB,EAAc/J,EAAczV,QAAO7D,GAAsB,WAAdA,EAAKiD,OAZ/B,IAAC6E,IAcTsb,EAAU/lB,KAAI2C,IAAQ,IAAMA,EAAKA,KAAMjD,MAAOiD,EAAKhC,KAAKG,MAAM,CAAEsQ,OAAQ5Q,QAdrDqlB,EAAe5B,GAAiBlkB,EAAQuH,MAAM8Y,QAAQ3b,YAAagG,IAClF,CAACA,IAAUqb,EAAW7B,GAAiBlkB,EAAQuH,MAAM8Y,QAAQ/d,QAASoI,GAAO,EAchGwb,CAAWD,EAAYhmB,KAAI2C,IAAQ,IAAMA,EAAKA,KAAM4R,WAAY5R,EAAKhC,KAAKG,MAAM,CAAEsQ,OAAQ5Q,SAErFO,GACD0kB,EAAQ,GAAG,EAGbS,EAASnlB,IACX,MAAMwD,EAAgBxE,EAAQuH,MAAM8Y,QAAQ7b,cACtCshB,EAAiB9lB,EAAQuH,MAAM8Y,QAAQiF,oBACvCS,EAAa/lB,EAAQuH,MAAM8Y,QAAQ9d,gBAMnC2Z,EAAgBpW,EAAiBtB,EAHhBxE,EAAQuH,MAAMkc,oBAChBzjB,EAAQuH,MAAMvB,aACjBhG,EAAQuH,MAAMtB,WAJN,IAACyE,EAOvB1J,IAAekb,EAAcG,OAAMzZ,GAAQA,EAAKhC,KAAKI,eAP9B0J,EAUTlG,EAVmBshB,EAAezB,GAAgBrkB,EAAQuH,MAAM8Y,QAAQ3b,YAAagG,IACjF,CAACA,IAAUqb,EAAW1B,GAAgBrkB,EAAQuH,MAAM8Y,QAAQ/d,QAASoI,GAAO,EAUlG0b,CAAc5hB,GAAc,EAKhCxE,EAAQklB,iBAAiBthB,EAAS,UAAW4gB,IAKzCxkB,EAAQmlB,kBAAkB,IAG9BnlB,EAAQklB,iBAAiBthB,EAAS,cAAe4gB,IAC7CxkB,EAAQ6f,cAAgB0E,GAAiBC,GACzCxkB,EAAQmlB,kBAAkB,IAG9BnlB,EAAQklB,iBAAiBthB,EAAS,aAAc4gB,IAG5C,GAFAxkB,EAAQ6f,cAAgB0E,GAAiBC,GAErCxkB,EAAQmjB,eAAgB,CACxB,MAAM/iB,EAASJ,EAAQuH,MAAMvB,aAAaO,IAAI,EAAYvG,EAAQmjB,iBAC5DkD,EAAcjmB,EAAO6I,MACrBqd,EAAclmB,EAAOyG,MACrBgZ,EAAgB7f,EAAQ6f,cAActU,EACtCgb,EAAiBrf,KAAK+C,IAAI,GAAI4V,EAAgByG,EAAcD,GAE5DG,EADuBxmB,EAAQuH,MAAM8Y,QAAQzb,aAE9C6B,QAAO4f,GAAe,EAAYA,EAAYlgB,YAAc/F,EAAO8E,MACnE1E,OAAO,CAAC,CAAE2F,SAAU/F,EAAO+D,GAAI8E,MAAOsd,KAC3CvmB,EAAQuH,MAAM8Y,QAAQmF,qBAAqBgB,EAC/C,CACA,GAAIxmB,EAAQojB,YAAa,CACrB,MAAM/iB,EAAML,EAAQuH,MAAMtB,UAAUM,IAAI,EAAYvG,EAAQojB,cACtDqD,EAAYpmB,EAAI2I,OAChB0d,EAAYrmB,EAAIyG,OAChB+Y,EAAgB7f,EAAQ6f,cAAcrU,EACtCmb,EAAezf,KAAK+C,IAAI,GAAI4V,EAAgB6G,EAAYD,GAExDG,EADqB5mB,EAAQuH,MAAM8Y,QAAQxb,WAE5C4B,QAAOggB,GAAa,EAAYA,EAAUpgB,SAAWhG,EAAI6E,MACzD1E,OAAO,CAAC,CAAE6F,MAAOhG,EAAI8D,GAAI6E,OAAQ2d,KACtC3mB,EAAQuH,MAAM8Y,QAAQoF,mBAAmBmB,EAC7C,CAGA5mB,EAAQmlB,kBAAkB,IAG9BnlB,EAAQklB,iBAAiBthB,EAAS,cAAc,KAC5C5D,EAAQ6f,cAAgB,KACxB7f,EAAQmlB,kBAAkB,IAK9BnlB,EAAQklB,iBAAiBthB,EAAS,aAAc4gB,IAC5CP,GAAYjkB,GACZ0lB,EAAQ,IAER1lB,EAAQsb,aAAc,EACtBtb,EAAQ6mB,kBAAoB7mB,EAAQ6f,cACpC7f,EAAQ8mB,cAAgB9mB,EAAQuH,MAAMoK,YAElC3R,EAAQuH,MAAM6I,kBACdpQ,EAAQmjB,eAAiBnjB,EAAQuH,MAAM6I,iBAEvCpQ,EAAQuH,MAAM8I,eACdrQ,EAAQojB,YAAcpjB,EAAQuH,MAAM8I,cAEnCrQ,EAAQuH,MAAM6I,iBAAoBpQ,EAAQuH,MAAM8I,cACjDrQ,EAAQuH,MAAM8Y,QAAQ+E,oBAAoBplB,EAAQuH,MAAMoK,aAGvD6S,EAAMuC,SACP/mB,EAAQuH,MAAM8Y,QAAQgF,sBAAsB,IAEhDrlB,EAAQmlB,kBAAkB,IAG9BnlB,EAAQklB,iBAAiBthB,EAAS,WAAY4gB,IAC1CP,GAAYjkB,GAEZA,EAAQsb,aAAc,EACtBtb,EAAQmjB,eAAiB,KACzBnjB,EAAQojB,YAAc,KAEtBpjB,EAAQuH,MAAM8Y,QAAQgF,sBAAsBnB,GAAiBlkB,EAAQuH,MAAM8Y,QAAQ7b,cAAexE,EAAQuH,MAAM9C,mBAChHzE,EAAQmlB,kBAAkB,IAG9BnlB,EAAQklB,iBAAiBthB,EAAS,eAAgB4gB,IAC9CxkB,EAAQ4D,QAAQojB,kBAAkBxC,EAAMyC,UAAU,IAGtDjnB,EAAQklB,iBAAiBthB,EAAS,aAAc4gB,IAC5CxkB,EAAQ4D,QAAQsjB,sBAAsB1C,EAAMyC,UAAU,IAG1DjnB,EAAQklB,iBAAiBthB,EAAS,SAAU4gB,IACxCP,GAAYjkB,GAEZ,MAAM4C,EAAO5C,EAAQuH,MAAMoK,YACrBmV,EAAgB9mB,EAAQ8mB,cAE9B,GAAI9mB,EAAQuH,MAAM6I,iBAAmBpQ,EAAQuH,MAAM8I,aAC/C,OACJ,GAAa,OAATzN,EACA,OACJ,GAAI,EAAYA,EAAKuD,YAAc,EAAY2gB,EAAc3gB,UACzD,OACJ,GAAI,EAAYvD,EAAKyD,SAAW,EAAYygB,EAAczgB,OACtD,OAEJ,MAAMjG,EAASJ,EAAQuH,MAAMvB,aAAaO,IAAI,EAAY3D,EAAKuD,WACzD9F,EAAML,EAAQuH,MAAMtB,UAAUM,IAAI,EAAY3D,EAAKyD,QACnD1B,EAAS3E,EAAQuH,MAAM8Y,QAAQ1b,OAErC,GAAoB,SAAhBvE,EAAOyF,MAAgC,SAAbxF,EAAIwF,KAC9B7F,EAAQuH,MAAM8Y,QAAQ1d,YAAY3C,EAAQuH,MAAMoK,kBAC7C,GAAoB,WAAhBvR,EAAOyF,MAAkC,WAAbxF,EAAIwF,KACvC7F,EAAQuH,MAAM8Y,QAAQnd,kBAAkBlD,EAAQuH,MAAMoK,kBACnD,GAAoB,WAAhBvR,EAAOyF,MAAkC,WAAbxF,EAAIwF,KAAmB,CAC1D,MAAMshB,ECrTH,SAAsBxiB,EAAQvE,EAAQC,EAAK0mB,GAGtD,SAASK,EAAclnB,GACnB,OAAOE,EAAO8E,MAAQ,EAAYhF,EAAKiG,UAAY,WAAa9F,EAAI6E,MAAQ,EAAYhF,EAAKmG,OAAS,SAC1G,CAEA,MAAMghB,EAAgB,CAAC,MAAO,YAAQpW,GAChCqW,EAAc3iB,EAAO4iB,KAAKH,GAC1BI,EAAiBH,EAAcI,QAAQH,GAAanW,WACpDuW,EAAeL,GAAeG,EAAiB,GAAKH,EAAcxf,QAClE8f,EAAahjB,EAAO8iB,QAAQH,KAAiB3iB,EAAOkD,OAAS,EAKnE,MAAO,KAJekf,IAAYY,GAAeL,EACiC,GAA9C3iB,EAAO8B,QAAOvG,IAASknB,EAAclnB,QACxDwnB,EAAe,CAAC,CAAEvhB,SAAU/F,EAAO+D,GAAIkC,MAAOhG,EAAI8D,GAAIgN,UAAWuW,IAAkB,GAGxG,CDoS8BE,CAAajjB,EAAQvE,EAAQC,EAAKmkB,EAAMuC,SAC1D/mB,EAAQuH,MAAM8Y,QAAQkF,eAAe4B,GACrCnnB,EAAQuH,MAAM8Y,QAAQgF,sBAAsB,GAChD,KAGJrlB,EAAQklB,iBAAiBthB,EAAS,YAAa4gB,IAG3C,GAFAP,GAAYjkB,GAERA,EAAQuH,MAAM6I,gBAAiB,CAC/B,MAAMyX,EAAqB,EAAY7nB,EAAQuH,MAAM6I,iBAC/CoW,EAAkBxmB,EAAQuH,MAAM8Y,QAAQzb,aAAa6B,QAAO4f,GAAe,EAAYA,EAAYlgB,YAAc0hB,IACvH7nB,EAAQuH,MAAM8Y,QAAQmF,qBAAqBgB,GAC3CxmB,EAAQ8hB,iBAAiB/D,OAAO8J,EACpC,CACA,GAAI7nB,EAAQuH,MAAM8I,aAAc,CAC5B,MAAMyX,EAAkB,EAAY9nB,EAAQuH,MAAM8I,cAC5CuW,EAAgB5mB,EAAQuH,MAAM8Y,QAAQxb,WAAW4B,QAAOggB,GAAa,EAAYA,EAAUpgB,SAAWyhB,IAC5G9nB,EAAQuH,MAAM8Y,QAAQoF,mBAAmBmB,GACzC5mB,EAAQ+hB,eAAehE,OAAO+J,EAClC,CAEA,MAAMvjB,EAAcvE,EAAQuH,MAAMhD,YAClC,GAAoB,OAAhBA,EACA,OAEJ,MAAMuN,EAAmB,EAAYvN,EAAY4B,UAC3C4L,EAAgB,EAAYxN,EAAY8B,OACxCL,EAAehG,EAAQuH,MAAMvB,aAC7BC,EAAYjG,EAAQuH,MAAMtB,UAC1BF,EAAiB/F,EAAQuH,MAAMkc,oBAErC,IAAKzd,EAAaM,IAAIwL,GAClB,OACJ,IAAK7L,EAAUK,IAAIyL,GACf,OAEJ,MAAM3R,EAAS4F,EAAaO,IAAIuL,GAC1BzR,EAAM4F,EAAUM,IAAIwL,GAEpBtR,EADOsF,EAAeS,QAAQnG,EAAKD,GACvBK,KAElBilB,EAAQjlB,GACR8O,GAAOwY,QAAQ,IAGnB/nB,EAAQklB,iBAAiBthB,EAAS,SAAS,KACnC2L,EAAMzH,eACNyH,EAAMK,MAAM,CAAEC,eAAe,GAAO,IAG5C7P,EAAQklB,iBAAiBthB,EAAS,WAAY4gB,IAE1CP,GAAYjkB,GAEZ,MAAMuE,EAAcvE,EAAQuH,MAAMhD,YAC5ByB,EAAehG,EAAQuH,MAAMvB,aAC7BC,EAAYjG,EAAQuH,MAAMtB,UAC1BzB,EAAgBxE,EAAQuH,MAAM8Y,QAAQ7b,cACtCwjB,EAAmBhoB,EAAQuH,MAAM8Y,QAAQgF,sBAEzC4C,EAAiBjoB,EAAQuH,MAAM8Y,QAAQ+E,oBACvC1gB,EAAc1E,EAAQuH,MAAM8Y,QAAQ3b,YACpCohB,EAAiB9lB,EAAQuH,MAAM8Y,QAAQiF,oBACvC1jB,EAAU5B,EAAQuH,MAAM3F,QACxBC,EAAO7B,EAAQuH,MAAM1F,KACrBpB,EAAOT,EAAQuH,MAAM9G,KACrBgjB,EAAsBzjB,EAAQuH,MAAMkc,oBAEpCyE,EAAU,CAACtlB,EAAM4hB,KACnByD,EAAerlB,GAEX4hB,EAAM2D,SAZsBH,EAAiB9D,GAAiB1f,EAa7C,CAAC5B,KAElBolB,EAAiB,CAACplB,GAAM,EAG1BwlB,EAAoB,CAAC1e,EAAQ8a,KAC/B,IAAKjgB,EACD,OAEJ,MAAMuN,EAAmB,EAAYvN,EAAY4B,UACjD,IAAKH,EAAaM,IAAIwL,GAClB,OAEJ,MAAMuW,EAAqBriB,EAAaO,IAAIuL,GAAkBrI,MACxD6e,EAAiBphB,KAAK+C,IAAI,EAAG/C,KAAK2T,IAAIjZ,EAAQiG,OAAS,EAAGwgB,EAAqB3e,IACrF,GAAI4e,IAAmBD,EACnB,OAEJ,MAAME,EAAiB,CAAEliB,MAAO9B,EAAY8B,MAAOF,SAAUvE,EAAQ0mB,GAAgBnkB,IAErF+jB,EAAQK,EAAgB/D,EAAM,EAG5BgE,EAAkB,CAAC9e,EAAQ8a,KAC7B,IAAKjgB,EACD,OAEJ,MAAMwN,EAAgB,EAAYxN,EAAY8B,OAC9C,IAAKJ,EAAUK,IAAIyL,GACf,OAEJ,MAAM0W,EAAkBxiB,EAAUM,IAAIwL,GAAetI,MAC/Cif,EAAcxhB,KAAK+C,IAAI,EAAG/C,KAAK2T,IAAIhZ,EAAKgG,OAAS,EAAG4gB,EAAkB/e,IAC5E,GAAIgf,IAAgBD,EAChB,OAEJ,MAAMF,EAAiB,CAAEliB,MAAOxE,EAAK6mB,GAAavkB,GAAIgC,SAAU5B,EAAY4B,UAE5E+hB,EAAQK,EAAgB/D,EAAM,EAG5BmE,EAAiB,KACnBnE,EAAMmE,iBACNnE,EAAMoE,iBAAiB,EAqC3B,OAAQpE,EAAMtf,KACV,IAAK,SAlCQ,KAATzE,EACAilB,EAAQ,IAEHlhB,EAAcqD,OAAS,EAC5BmgB,EAAiB,CAACzjB,IAEbG,EAAYmD,OAAS,EAC1Bie,EAAe,KAGfmC,EAAe,MACfD,EAAiB,KAyBjB,MACJ,IAAK,QACDnC,IACA,MACJ,IAAK,UAGD8C,IACAH,EAAgBhE,EAAMuC,SAAWllB,EAAKgG,QAAU,EAAG2c,GACnD,MACJ,IAAK,YACDmE,IACAH,EAAgBhE,EAAMuC,QAAUllB,EAAKgG,OAAS,EAAG2c,GACjD,MACJ,IAAK,YACDmE,IACAP,EAAkB5D,EAAMuC,SAAWnlB,EAAQiG,QAAU,EAAG2c,GACxD,MACJ,IAAK,aACDmE,IACAP,EAAkB5D,EAAMuC,QAAUnlB,EAAQiG,OAAS,EAAG2c,GACtD,MACJ,IAAK,SACL,IAAK,YACD2B,IACA,MACJ,IAAK,IA/Ce,CAAC3B,IACrB,IAAKA,EAAMuC,QACP,OAEJ,MAAM8B,EE/bH,SAA0BrkB,EAAe5C,EAASC,EAAMkE,GACnE,MAAMC,EAAe,IAAI6O,IAAIjT,EAAQ3B,KAAIG,GAAU,CAACA,EAAO8E,IAAK9E,MAC1D6F,EAAY,IAAI4O,IAAIhT,EAAK5B,KAAII,GAAO,CAACA,EAAI6E,IAAK7E,MAC9CyoB,EAAmBtkB,EAAcvE,KAAI2C,IAAQ,CAC/CsD,UAAW,EAAYtD,EAAKuD,UAC5BC,OAAQ,EAAYxD,EAAKyD,WACzBI,QAAO7D,GAAQoD,EAAaM,IAAI1D,EAAKsD,YAAcD,EAAUK,IAAI1D,EAAKwD,UACpE2iB,EAAkB,IAAIzT,IAAIwT,EAAiB7oB,KAAI2C,GAAQA,EAAKsD,aAC5D8iB,EAAe,IAAI1T,IAAIwT,EAAiB7oB,KAAI2C,GAAQA,EAAKwD,UAE/D,GAAgC,IAA5B0iB,EAAiBjhB,OACjB,MAAO,GAEX,MAAM+J,EAAY,IAAIyD,EAAU7Q,GAC1BiX,EAAiBvU,KAAK2T,OAAOiO,EAAiB7oB,KAAI2C,GAAQoD,EAAaO,IAAI3D,EAAKsD,WAAWuD,SAC3FiS,EAAiBxU,KAAK+C,OAAO6e,EAAiB7oB,KAAI2C,GAAQoD,EAAaO,IAAI3D,EAAKsD,WAAWuD,SAC3FkS,EAAczU,KAAK2T,OAAOiO,EAAiB7oB,KAAI2C,GAAQqD,EAAUM,IAAI3D,EAAKwD,QAAQqD,SAClFmS,EAAc1U,KAAK+C,OAAO6e,EAAiB7oB,KAAI2C,GAAQqD,EAAUM,IAAI3D,EAAKwD,QAAQqD,SAElFwf,EAAgB,GAEtB,IAAK,IAAIpe,EAAW8Q,EAAa9Q,GAAY+Q,EAAa/Q,IAAY,CAClE,MAAMxK,EAAMwB,EAAKgJ,GACXzE,EAAS/F,EAAI6E,IAEnB,GAAK8jB,EAAa1iB,IAAIF,GAAtB,CAGA,IAAK,IAAI0E,EAAc2Q,EAAgB3Q,GAAe4Q,EAAgB5Q,IAAe,CACjF,MAAM1K,EAASwB,EAAQkJ,GACjB5E,EAAY9F,EAAO8E,IAEzB,GAAK6jB,EAAgBziB,IAAIJ,GAAzB,CAGA,GAAI0L,EAAUO,cAAc/L,EAAQF,GAAY,CAC5C,MAAMgjB,EAAWnjB,EAAeS,QAAQnG,EAAKD,GAAQK,KACrDwoB,EAActf,KAAKuf,EACvB,CAEIpe,EAAc4Q,GACduN,EAActf,KAAK,KARX,CAShB,CAEIkB,EAAW+Q,GACXqN,EAActf,KAAK,KAnBX,CAoBhB,CAEA,OAAOsf,EAAc5jB,KAAK,GAC9B,CF8YkC8jB,CAAiB3kB,EAAe5C,EAASC,EAAM4hB,GAErE,GAAI2F,UAAUC,UACVD,UAAUC,UAAUC,UAAUT,OAC3B,CACH,MAAMU,EAAW7Z,SAASoK,cAAc,YACxCyP,EAAS5pB,MAAQkpB,EACjBnZ,SAAS8Z,KAAKxhB,YAAYuhB,GAC1BA,EAASxB,SACTrY,SAAS+Z,YAAY,QACrB/Z,SAAS8Z,KAAKzhB,YAAYwhB,EAC9B,GAiCIG,CAAgBlF,GAIxB,IAGJ,IAAImF,gBAAe,KACf3pB,EAAQmlB,kBAAkB,IAC3ByE,QAAQhmB,GAEX5D,EAAQklB,iBAAiB3V,EAAO,SAAUiV,IAEtCP,GAAYjkB,GAERwkB,EAAMqF,OAAOlqB,OACbkmB,GAAO,GAEPtW,EAAM7O,MAAMopB,QAAU,EACtBva,EAAM7O,MAAMqpB,cAAgB,SAGxBvF,EAAMwF,WACN7D,GAAM,GAEV5W,EAAM7O,MAAMopB,QAAU,EACtBva,EAAM7O,MAAMqpB,cAAgB,OAChC,IAGJ/pB,EAAQklB,iBAAiB3V,EAAO,SAAUiV,IACtCA,EAAMoE,iBAAiB,IAG3B5oB,EAAQklB,iBAAiB3V,EAAO,YAAaiV,IACzCA,EAAMoE,iBAAiB,IAG3B5oB,EAAQklB,iBAAiB3V,EAAO,aAAciV,IAC1CA,EAAMoE,iBAAiB,IAG3B5oB,EAAQklB,iBAAiB3V,EAAO,WAAYiV,IACxC,OAAQA,EAAMtf,KACV,IAAK,QACL,IAAK,SACD,MACJ,IAAK,SACL,IAAK,YACL,IAAK,UACL,IAAK,YACL,IAAK,YACL,IAAK,aACmB,KAAhBqK,EAAM5P,QACN6kB,EAAMoE,kBACN5oB,EAAQmlB,oBAEZ,MACJ,QACIX,EAAMoE,kBAEN5oB,EAAQmlB,mBAEhB,GAER,CAEe,SAASrhB,GAAWF,EAASyc,GACxC/e,QAAQ2G,IAAI,cAEZ2c,GAAWhhB,GAEX,MAAM5D,EAAU4D,EAAQ,uBACxB5D,EAAQugB,gBAAkBF,EAEJ,OAAlBrgB,EAAQuH,OACR0c,GAAYjkB,GAEZqP,EAAOrP,IAGPA,EAAQmlB,kBAEhB,C,GGhkBI8E,yBAA2B,CAAC,EAGhC,SAASC,oBAAoBC,GAE5B,IAAIC,EAAeH,yBAAyBE,GAC5C,QAAqBlZ,IAAjBmZ,EACH,OAAOA,EAAaplB,QAGrB,IAAID,EAASklB,yBAAyBE,GAAY,CAGjDnlB,QAAS,CAAC,GAOX,OAHAqlB,oBAAoBF,GAAUplB,EAAQA,EAAOC,QAASklB,qBAG/CnlB,EAAOC,OACf,CCrBAklB,oBAAoBpnB,EAAKiC,IACxB,IAAIulB,EAASvlB,GAAUA,EAAOwlB,WAC7B,IAAOxlB,EAAiB,QACxB,IAAM,EAEP,OADAmlB,oBAAoBM,EAAEF,EAAQ,CAAElhB,EAAGkhB,IAC5BA,CAAM,ECLdJ,oBAAoBM,EAAI,CAACxlB,EAASylB,KACjC,IAAI,IAAIvlB,KAAOulB,EACXP,oBAAoBQ,EAAED,EAAYvlB,KAASglB,oBAAoBQ,EAAE1lB,EAASE,IAC5EK,OAAOolB,eAAe3lB,EAASE,EAAK,CAAE0lB,YAAY,EAAMrkB,IAAKkkB,EAAWvlB,IAE1E,ECNDglB,oBAAoBQ,EAAI,CAACG,EAAKC,IAAUvlB,OAAOwlB,UAAUC,eAAeC,KAAKJ,EAAKC,GCClFZ,oBAAoB9S,EAAKpS,IACH,oBAAXkmB,QAA0BA,OAAOC,aAC1C5lB,OAAOolB,eAAe3lB,EAASkmB,OAAOC,YAAa,CAAExrB,MAAO,WAE7D4F,OAAOolB,eAAe3lB,EAAS,aAAc,CAAErF,OAAO,GAAO,ECL9D,IAAIyrB,iBAAmB,WACnB,IAAIC,EAAS3b,SAAS4b,cACtB,IAAKD,EAAQ,CAOT,IAHA,IAAIE,EAAc7b,SAAS8b,qBAAqB,UAC5CC,EAAU,GAELC,EAAI,EAAGA,EAAIH,EAAY1jB,OAAQ6jB,IACpCD,EAAQ9hB,KAAK4hB,EAAYG,IAI7BL,GADAI,EAAUA,EAAQhlB,QAAO,SAASklB,GAAK,OAAQA,EAAEC,QAAUD,EAAElrB,OAASkrB,EAAEE,WAAa,KACpE/hB,OAAO,GAAG,EAC/B,CAEA,OAAOuhB,CACX,EAEIS,cAAgB,SAAST,GACzB,MAAO,6BAA6BU,KAAKV,EAAOW,IACpD,EAMYC,IAQZ,GAZA1mB,OAAOolB,eAAeT,oBAAqB,IAAK,CAC5C3jB,KAGQ0lB,IAFSb,mBAEIY,IAAIE,MAAM,KAAKpiB,MAAM,GAAI,GAAGzE,KAAK,KAAO,IAElD,WACH,OAAO4mB,GACX,KAIsB,oBAAnBE,eAAgC,CACvC,IAAIC,mBAAqBD,eACzBA,eAAiB,SAASE,GACtB,IAAIhB,EAASD,mBACTkB,EAAUR,cAAcT,GAExBW,EAAMI,mBAAmBC,GAE7B,IAAIC,EACA,OAAON,EAGX,IAAIO,EAAeP,EAAIE,MAAM,KACzBM,EAAgBD,EAAaziB,OAAO,GAAG,GAAGoiB,MAAM,KAKpD,OAHAM,EAAcC,OAAO,EAAG,EAAG,qBAC3BF,EAAaE,QAAQ,EAAG,EAAGD,EAAcnnB,KAAK,MAEvCknB,EAAalnB,KAAK,IAC7B,CACJ,C",
+    "mappings": "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",
     "names": [
         "isString",
         "value",
         "String",
         "useResolvedFormatting",
         "formatting",
         "useMemo",
@@ -386,23 +386,25 @@
         "addRowRule",
         "getRules",
         "rules",
         "gatherRules",
         "newRules",
         "gatherRowRules",
         "borderTypes",
+        "defaultEdit",
         "indexBorders",
         "newStyle",
         "borderType",
         "FormattingRules",
         "rulesLookup",
         "entries",
         "entry",
         "array",
         "currentContext",
+        "getText",
         "result",
         "visible",
         "getFormattingRules",
         "dataFormatting",
         "FormatResolver",
         "formattingRules",
         "getFormatResolver",
@@ -631,21 +633,25 @@
         "newRowHeights",
         "mouseDownPosition",
         "mouseDownCell",
         "ctrlKey",
         "setPointerCapture",
         "pointerId",
         "releasePointerCapture",
+        "cellData",
+        "toggle",
+        "indexOf",
+        "getToggledValue",
+        "cellType",
         "newSortBy",
         "isCurrentRule",
         "directionLoop",
         "currentRule",
         "find",
         "directionIndex",
-        "indexOf",
         "newDirection",
         "isLastRule",
         "getNewSortBy",
         "resizableColumnKey",
         "resizableRowKey",
         "select",
         "setSelectedCells",
@@ -662,15 +668,14 @@
         "preventDefault",
         "stopPropagation",
         "clipboardData",
         "selectedCellKeys",
         "selectedColumns",
         "selectedRows",
         "stringBuilder",
-        "cellData",
         "getClipboardData",
         "navigator",
         "clipboard",
         "writeText",
         "textArea",
         "body",
         "execCommand",
@@ -783,14 +788,15 @@
         "webpack:///../lib/src/state-utils/getHoveredCell.js",
         "webpack:///../lib/src/state-utils/getRowIndex.js",
         "webpack:///../lib/src/state-utils/getColumnIndex.js",
         "webpack:///../lib/src/state-utils/getCombinedCells.js",
         "webpack:///../lib/src/state-utils/getReducedCells.js",
         "webpack:///../lib/src/state-utils/getMousePosition.js",
         "webpack:///../lib/src/index.js",
+        "webpack:///../lib/src/state-utils/getToggledValue.js",
         "webpack:///../lib/src/state-utils/getNewSortBy.js",
         "webpack:///../lib/src/state-utils/getClipboardData.js",
         "webpack:///webpack/bootstrap",
         "webpack:///webpack/runtime/compat get default export",
         "webpack:///webpack/runtime/define property getters",
         "webpack:///webpack/runtime/hasOwnProperty shorthand",
         "webpack:///webpack/runtime/make namespace object",
@@ -816,15 +822,15 @@
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default class Selection {\n    constructor(selectedCells) {\n        this.lookup = new Map();\n\n        selectedCells.forEach(cell => {\n            const rowKey = stringifyId(cell.rowId);\n            const columnKey = stringifyId(cell.columnId);\n\n            if (!this.lookup.has(rowKey))\n                this.lookup.set(rowKey, new Set());\n\n            this.lookup.get(rowKey).add(columnKey);\n        });\n    }\n\n    isKeySelected(rowKey, columnKey) {\n        return this.lookup.has(rowKey) && this.lookup.get(rowKey).has(columnKey);\n    }\n\n    isIdSelected(rowId, columnId) {\n        return this.isKeySelected(stringifyId(rowId), stringifyId(columnId));\n    }\n}",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getSelection(selectedCells) {\n    return new Selection(selectedCells);\n}\n",
         "export default function getInvoked(columnsOrRows, data) {\n    return typeof columnsOrRows === 'function'\n        ? columnsOrRows(data)\n        : columnsOrRows;\n}\n",
         "// TODO: Move\nexport default function getPinned(index, length, pinnedBegin, pinnedEnd) {\n    if (index < pinnedBegin)\n        return \"BEGIN\";\n    if (index >= length - pinnedEnd)\n        return \"END\";\n    return undefined;\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getPinned from \"./getPinned.js\";\n\nfunction getResolved(elements, pinnedBegin, pinnedEnd) {\n    return elements.map((element, index) => {\n        const id = 'id' in element ? element.id : element.type;\n        return {\n            ...element,\n            id: id,\n            type: element.type || \"DATA\",\n            index: index,\n            key: stringifyId(id),\n            pinned: getPinned(index, elements.length, pinnedBegin, pinnedEnd),\n            header: 'header' in element ? element.header : id,\n            labels: element.labels || []\n        };\n    });\n}\n\nexport function getResolvedColumns(columns, pinnedBegin, pinnedEnd, columnWidths) {\n    const widthsLookup = new Map(columnWidths.map(({ columnId, width }) => [stringifyId(columnId), width]));\n    const resolvedColumns = getResolved(columns, pinnedBegin, pinnedEnd);\n\n    return resolvedColumns.map(column => ({\n        ...column,\n        width: widthsLookup.has(column.key)\n            ? widthsLookup.get(column.key)\n            : column.width\n    }));\n}\n\nexport function getResolvedRows(rows, pinnedBegin, pinnedEnd, rowHeights) {\n    const heightsLookup = new Map(rowHeights.map(({ rowId, height }) => [stringifyId(rowId), height]));\n    const resolvedRows = getResolved(rows, pinnedBegin, pinnedEnd);\n\n    return resolvedRows.map(row => ({\n        ...row,\n        height: heightsLookup.has(row.key)\n            ? heightsLookup.get(row.key)\n            : row.height\n    }));\n}\n",
         "import roundToPixels from \"../core-utils/roundToPixels.js\";\n\nexport function getPlacedColumns(columns, devicePixelRatio, borderWidth) {\n    let left = borderWidth;\n\n    return columns.map((column, index) => {\n        const assignedWidth = 'width' in column ? column.width : 100;\n        const width = roundToPixels(assignedWidth, devicePixelRatio);\n        const newColumn = {\n            ...column,\n            index: index,\n            width: width,\n            leftWithBorder: left - borderWidth,\n            left: left,\n            right: left + width,\n            rightWithBorder: left + width + borderWidth\n        };\n\n        left += newColumn.width + borderWidth;\n\n        return newColumn;\n    });\n}\n\nexport function getPlacedRows(rows, devicePixelRatio, borderWidth) {\n    let top = borderWidth;\n\n    return rows.map((row, index) => {\n        const assignedHeight = 'height' in row ? row.height : 20;\n        const height = roundToPixels(assignedHeight, devicePixelRatio);\n        const newRow = {\n            ...row,\n            index: index,\n            height: height,\n            topWithBorder: top - borderWidth,\n            top: top,\n            bottom: top + height,\n            bottomWithBorder: top + height + borderWidth\n        };\n\n        top += newRow.height + borderWidth;\n\n        return newRow;\n    });\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nconst matchMapping = {\n    'HEADER': ['HEADER'],\n    'FILTER': ['FILTER'],\n    'DATA': ['DATA'],\n    'CUSTOM': ['CUSTOM'],\n    'ANY': ['HEADER', 'DATA', 'FILTER', 'CUSTOM'],\n    'SPECIAL': ['HEADER', 'FILTER', 'CUSTOM'],\n    undefined: []\n};\n\nclass Lookup {\n    byKey = new Map();\n    byIndex = new Map(); // TODO: Should this be removed?\n    byLabel = new Map();\n    byMatch = new Map();\n}\n\nexport default class RulesLookup {\n    lookup = new Lookup();\n    hasRules = false;\n\n    addRule(column, row, rule) {\n        this.hasRules = true;\n\n        if (Array.isArray(column)) {\n            for (const c of column)\n                this.addRule(c, row, rule);\n            return;\n        }\n\n        if (Array.isArray(row)) {\n            for (const r of row)\n                this.addRule(column, r, rule);\n            return;\n        }\n\n        column = column\n            ? 'id' in column\n                ? { key: stringifyId(column.id) }\n                : column\n            : { match: 'DATA' };\n        row = row\n            ? 'id' in row\n                ? { key: stringifyId(row.id) }\n                : row\n            : { match: 'DATA' };\n\n        function addRowRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, []);\n\n            lookup.get(key).push(rule);\n        }\n\n        function addColumnRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, new Lookup());\n\n            if ('key' in row)\n                addRowRule(lookup.get(key).byKey, row.key);\n            if ('index' in row)\n                addRowRule(lookup.get(key).byIndex, row.index);\n            if ('label' in row)\n                addRowRule(lookup.get(key).byLabel, row.label);\n            for (const match of matchMapping[row.match])\n                addRowRule(lookup.get(key).byMatch, match);\n        }\n\n        if ('key' in column)\n            addColumnRule(this.lookup.byKey, column.key);\n        if ('index' in column)\n            addColumnRule(this.lookup.byIndex, column.index);\n        if ('label' in column)\n            addColumnRule(this.lookup.byLabel, column.label);\n        for (const match of matchMapping[column.match])\n            addColumnRule(this.lookup.byMatch, match);\n    }\n\n    getRules(column, row) {\n        const rules = [];\n\n        if (!this.hasRules)\n            return rules;\n\n        function gatherRules(newRules) {\n            for (const rule of newRules)\n                rules.push(rule);\n        }\n\n        function gatherRowRules(lookup) {\n            if (lookup.byKey.has(row.key))\n                gatherRules(lookup.byKey.get(row.key));\n            if (lookup.byIndex.has(row.index))\n                gatherRules(lookup.byIndex.get(row.index));\n            if (lookup.byMatch.has(row.type))\n                gatherRules(lookup.byMatch.get(row.type));\n            for (const label of row.labels) {\n                if (lookup.byLabel.has(label))\n                    gatherRules(lookup.byLabel.get(label));\n            }\n        }\n\n        if (this.lookup.byKey.has(column.key))\n            gatherRowRules(this.lookup.byKey.get(column.key));\n        if (this.lookup.byIndex.has(column.index))\n            gatherRowRules(this.lookup.byIndex.get(column.index));\n        if (this.lookup.byMatch.has(column.type))\n            gatherRowRules(this.lookup.byMatch.get(column.type));\n        for (const label of column.labels) {\n            if (this.lookup.byLabel.has(label))\n                gatherRowRules(this.lookup.byLabel.get(label));\n        }\n\n        return rules;\n    }\n};",
-        "import { defaultPadding } from \"../core-utils/defaults.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst borderTypes = ['borderTop', 'borderRight', 'borderBottom', 'borderLeft'];\n\n// TODO: Don't recreate styles if they haven't changed\nfunction indexBorders(style, index) {\n    const newStyle = { ...style };\n\n    if ('border' in newStyle) {\n        for (const borderType of borderTypes)\n            newStyle[borderType] = newStyle.border;\n        delete newStyle.border;\n    }\n\n    for (const borderType of borderTypes)\n        if (borderType in newStyle)\n            newStyle[borderType] = { ...newStyle[borderType], index };\n\n    return newStyle;\n}\n\n// TODO: Rename to FormatResolver\n// TODO: Optimize by not searching using keys that don't have correlated match rules\n// TODO: Accept both a function and an object as a style (where the object is a resolved style)\n// TODO: Consider removing index from the lookup\nexport default class FormattingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const [index, rule] of rules.entries()) {\n            const entry = { index };\n    \n            if ('condition' in rule)\n                entry.condition = rule.condition;\n            if ('style' in rule)\n                entry.style = typeof rule.style === 'function' ? rule.style : () => rule.style;\n            if ('value' in rule)\n                entry.value = typeof rule.value === 'function' ? rule.value : () => rule.value;\n            if ('text' in rule)\n                entry.text = typeof rule.text === 'function' ? rule.text : () => rule.text;\n            if ('padding' in rule)\n                entry.padding = typeof rule.padding === 'function' ? rule.padding : () => rule.padding;\n            if ('edit' in rule)\n                entry.edit = rule.edit;\n            if ('draw' in rule)\n                entry.draw = rule.draw;\n    \n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, edition) {\n        const rules = this.rulesLookup\n            .getRules(column, row)\n            .sort((a, b) => a.index - b.index)\n            .filter((value, index, array) => value.index !== array[index - 1]?.index);\n\n        let context = { data, rows, columns, row, column };\n        let style = {};\n        let draw = undefined;\n        let visible = true;\n        let padding = defaultPadding;\n\n        if (edition.hasValueByKey(row.key, column.key))\n            context = { ...context, newValue: edition.getValueByKey(row.key, column.key) };\n\n        for (const rule of rules) {\n            if ('condition' in rule && !rule.condition(context))\n                continue;\n\n            // TODO: Don't actually add things like `edit` to the context\n            if ('value' in rule)\n                context = { ...context, value: rule.value(context) };\n            if ('style' in rule)\n                style = { ...style, ...indexBorders(rule.style(context), rule.index) };\n            if ('text' in rule)\n                context = { ...context, text: rule.text(context) };\n            if ('padding' in rule)\n                padding = { ...padding, ...rule.padding(context) };\n            if ('edit' in rule)\n                context = { ...context, edit: rule.edit && 'edit' in context ? { ...context.edit, ...rule.edit } : rule.edit };\n            if ('draw' in rule) {\n                const currentContext = context;\n                draw = (ctx) => rule.draw({ ...currentContext, ctx });\n            }\n\n            // TODO: Add StopPropagation\n        }\n\n        const text = 'text' in context ? context.text : `${context.value}`;\n        const result = {\n            style,\n            visible,\n            text,\n            padding\n        };\n\n        if ('value' in context)\n            result.value = context.value;\n        if ('edit' in context)\n            result.edit = context.edit;\n        if (draw !== undefined)\n            result.draw = draw;\n        if ('text' in context)\n            result.text = context.text;\n\n        return result;\n    }\n}",
+        "import { defaultPadding } from \"../core-utils/defaults.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst borderTypes = ['borderTop', 'borderRight', 'borderBottom', 'borderLeft'];\n// TODO: better handle default validate for toggle edit\nconst defaultEdit = { validate: () => true, parse: string => string };\n\n// TODO: Don't recreate styles if they haven't changed\nfunction indexBorders(style, index) {\n    const newStyle = { ...style };\n\n    if ('border' in newStyle) {\n        for (const borderType of borderTypes)\n            newStyle[borderType] = newStyle.border;\n        delete newStyle.border;\n    }\n\n    for (const borderType of borderTypes)\n        if (borderType in newStyle)\n            newStyle[borderType] = { ...newStyle[borderType], index };\n\n    return newStyle;\n}\n\nfunction getText(context) {\n    if ('text' in context)\n        return context.text;\n    if (context.value !== undefined)\n        return `${context.value}`;\n    return '';\n}\n\n// TODO: Rename to FormatResolver\n// TODO: Optimize by not searching using keys that don't have correlated match rules\n// TODO: Accept both a function and an object as a style (where the object is a resolved style)\n// TODO: Consider removing index from the lookup\nexport default class FormattingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const [index, rule] of rules.entries()) {\n            const entry = { index };\n\n            if ('condition' in rule)\n                entry.condition = rule.condition;\n            if ('style' in rule)\n                entry.style = typeof rule.style === 'function' ? rule.style : () => rule.style;\n            if ('value' in rule)\n                entry.value = typeof rule.value === 'function' ? rule.value : () => rule.value;\n            if ('text' in rule)\n                entry.text = typeof rule.text === 'function' ? rule.text : () => rule.text;\n            if ('padding' in rule)\n                entry.padding = typeof rule.padding === 'function' ? rule.padding : () => rule.padding;\n            if ('edit' in rule)\n                entry.edit = rule.edit;\n            if ('draw' in rule)\n                entry.draw = rule.draw;\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, edition) {\n        const rules = this.rulesLookup\n            .getRules(column, row)\n            .sort((a, b) => a.index - b.index)\n            .filter((value, index, array) => value.index !== array[index - 1]?.index);\n\n        let context = { data, rows, columns, row, column };\n        let style = {};\n        let draw = undefined;\n        let visible = true;\n        let padding = defaultPadding;\n\n        if (edition.hasValueByKey(row.key, column.key))\n            context = { ...context, newValue: edition.getValueByKey(row.key, column.key) };\n\n        for (const rule of rules) {\n            if ('condition' in rule && !rule.condition(context))\n                continue;\n\n            // TODO: Don't actually add things like `edit` to the context\n            if ('value' in rule)\n                context = { ...context, value: rule.value(context) };\n            if ('style' in rule)\n                style = { ...style, ...indexBorders(rule.style(context), rule.index) };\n            if ('text' in rule)\n                context = { ...context, text: rule.text(context) };\n            if ('padding' in rule)\n                padding = { ...padding, ...rule.padding(context) };\n            if ('edit' in rule)\n                context = { ...context, edit: rule.edit && 'edit' in context ? { ...context.edit, ...rule.edit } : { ...defaultEdit, ...rule.edit } };\n            if ('draw' in rule) {\n                const currentContext = context;\n                draw = (ctx) => rule.draw({ ...currentContext, ctx });\n            }\n\n            // TODO: Add StopPropagation\n        }\n\n        const text = getText(context);\n        const result = {\n            style,\n            visible,\n            text,\n            padding\n        };\n\n        if ('value' in context)\n            result.value = context.value;\n        if ('edit' in context)\n            result.edit = context.edit;\n        if (draw !== undefined)\n            result.draw = draw;\n        if ('text' in context)\n            result.text = context.text;\n\n        return result;\n    }\n}",
         "import FormattingRules from \"../types/FormattingRules.js\";\n\nexport default function getFormattingRules(dataFormatting) {\n    return new FormattingRules(dataFormatting);\n}\n",
         "export default class FormatResolver {\n    constructor(formattingRules, data, rows, columns, edition) {\n        this.formattingRules = formattingRules;\n        this.data = data;\n        this.rows = rows;\n        this.columns = columns;\n        this.edition = edition;\n    }\n\n    resolve(row, column) {\n        return this.formattingRules.resolve(\n            this.data,\n            this.rows,\n            this.columns,\n            row,\n            column,\n            this.edition);\n    }\n}",
         "import FormatResolver from \"../types/FormatResolver.js\";\n\nexport default function getFormatResolver(formattingRules, data, rows, columns, edition) {\n    return new FormatResolver(formattingRules, data, rows, columns, edition);\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction getFilterLookup(filters, primaryKey, secondaryKey) {\n    const filterLookup = new Map();\n    for (const cell of filters) {\n        const primary = stringifyId(cell[primaryKey]);\n        const secondary = stringifyId(cell[secondaryKey]);\n\n        if (!filterLookup.has(primary))\n            filterLookup.set(primary, new Map());\n\n        filterLookup.get(primary).set(secondary, cell.expression);\n    }\n    return filterLookup;\n}\n\nexport function getFilteredRows(filters, filteringRules, formattingRules, data, rows, columns, edition) {\n    if (filters.length === 0)\n        return rows;\n\n    const filterLookup = getFilterLookup(filters, 'columnId', 'rowId');\n    const filteredColumns = columns.filter(column => column.type !== 'FILTER' && filterLookup.has(column.key));\n\n    if (filteredColumns.length === 0)\n        return rows;\n\n    return rows.filter(row => {\n        for (const column of filteredColumns) {\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const columnFilters = filterLookup.get(column.key);\n            const visible = filteringRules.resolve(data, rows, columns, row, column, cell.value, cell.text, columnFilters);\n\n            if (!visible)\n                return false;\n        }\n        return true;\n    });\n}\n\nexport function getFilteredColumns(filters, filteringRules, formattingRules, data, rows, columns, edition) {\n    if (filters.length === 0)\n        return columns;\n\n    const filterLookup = getFilterLookup(filters, 'rowId', 'columnId');\n    const filteredRows = rows.filter(row => row.type !== 'FILTER' && filterLookup.has(row.key));\n\n    if (filteredRows.length === 0)\n        return columns;\n\n    return columns.filter(column => {\n        for (const row of filteredRows) {\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const rowFilters = filterLookup.get(row.key);\n            const visible = filteringRules.resolve(data, rows, columns, row, column, cell.value, cell.text, rowFilters);\n\n            if (!visible)\n                return false;\n        }\n        return true;\n    });\n}",
         "export default function getFixedSize(top, bottom, left, right) {\n    return {\n        top: top,\n        bottom: bottom,\n        left: left,\n        right: right\n    };\n}\n",
         "export default function getTotalSize(columns, rows) {\n    return {\n        width: columns.length ? columns.at(-1).rightWithBorder : 0,\n        height: rows.length ? rows.at(-1).bottomWithBorder : 0\n    };\n}\n",
         "import { defaultFont } from \"../core-utils/defaults.js\";\n\nexport default class TextResolver\n{\n    constructor() {\n        this.canvas = document.createElement('canvas');\n        this.context = this.canvas.getContext('2d');\n        this.fontMetrics = new Map();\n    }\n\n    measureWidth(text, font) {\n        const ctx = this.context;\n\n        ctx.font = font || defaultFont;\n\n        const textMetrics = ctx.measureText(text);\n\n        return textMetrics.width;\n    }\n\n    measureHeight(text, font) {\n        let lines = 1;\n        for (const char of text) {\n            if (char === '\\n')\n                lines++;\n        }\n\n        return lines * this.getFontMetrics(font).height;\n    }\n\n    getFontMetrics(font) {\n        const key = font;\n\n        if (this.fontMetrics.has(key))\n            return this.fontMetrics.get(key);\n\n        const ctx = this.context;\n\n        // TODO: Set other font properties\n        ctx.font = font || defaultFont;\n\n        const textMetrics = ctx.measureText('X');\n\n        const middle = (textMetrics.actualBoundingBoxDescent - textMetrics.actualBoundingBoxAscent) / 2;\n        const topOffset = middle + textMetrics.fontBoundingBoxAscent;\n        const bottomOffset = textMetrics.fontBoundingBoxDescent - middle;\n        const height = textMetrics.fontBoundingBoxAscent + textMetrics.fontBoundingBoxDescent;\n\n        const fontMetrics = {\n            topOffset: topOffset,\n            middle: -middle,\n            bottomOffset: bottomOffset,\n            height: height\n        };\n\n        this.fontMetrics.set(key, fontMetrics);\n\n        return fontMetrics;\n    }\n}",
@@ -832,41 +838,42 @@
         "export function contains(bounds, rect) {\n    return (\n        rect.top >= bounds.top &&\n        rect.left >= bounds.left &&\n        rect.top + rect.height <= bounds.top + bounds.height &&\n        rect.left + rect.width <= bounds.left + bounds.width\n    );\n}\n\nexport function clip(bounds, rect) {\n    const newRect = {\n        top: Math.max(bounds.top, rect.top),\n        left: Math.max(bounds.left, rect.left),\n        width: Math.min(bounds.left + bounds.width, rect.left + rect.width) - Math.max(bounds.left, rect.left),\n        height: Math.min(bounds.top + bounds.height, rect.top + rect.height) - Math.max(bounds.top, rect.top)\n    };\n\n    if (newRect.width >= 0 && newRect.height >= 0)\n        return newRect;\n\n    return {\n        top: bounds.top,\n        left: bounds.left,\n        width: 0,\n        height: 0\n    }\n}\n\nexport function expand(rect, margin) {\n    return {\n        top: rect.top - margin,\n        left: rect.left - margin,\n        width: rect.width + margin * 2,\n        height: rect.height + margin * 2\n    };\n}\n\nexport function area(rect) {\n    return rect.width * rect.height;\n}\n\nexport function subtract(rect, margin) {\n    return {\n        top: rect.top,\n        left: rect.left,\n        width: Math.max(0, rect.width - margin.left - margin.right),\n        height: Math.max(0, rect.height - margin.top - margin.bottom)\n    };\n}",
         "import { area, clip, contains, expand, subtract } from \"../core-utils/rect.js\";\n\nconst requiredMargin = 200;\nconst preloadedMargin = 400;\nconst emptyRect = {\n    left: 0,\n    top: 0,\n    width: 0,\n    height: 0\n};\n\nexport default function getScrollRect(previous, totalSize, fixedSize, element) {\n    // TODO: Is it optimal to use getBoundingClientRect()?\n    const size = {\n        width: element.getBoundingClientRect().width,\n        height: element.getBoundingClientRect().height\n    };\n    const scrollOffset = {\n        left: element.scrollLeft,\n        top: element.scrollTop\n    };\n\n    const prevScrollRect = previous || emptyRect;\n\n    const totalRect = { left: 0, top: 0, ...totalSize };\n    const bounds = subtract(totalRect, fixedSize);\n    const scrollRect = subtract({ ...scrollOffset, ...size }, fixedSize);\n    const requiredScrollRect = clip(bounds, expand(scrollRect, requiredMargin));\n    const preloadedScrollRect = clip(bounds, expand(scrollRect, preloadedMargin));\n\n    if (!contains(bounds, prevScrollRect))\n        return preloadedScrollRect;\n\n    if (!contains(prevScrollRect, requiredScrollRect))\n        return preloadedScrollRect;\n\n    if (area(prevScrollRect) > 2 * area(preloadedScrollRect))\n        return preloadedScrollRect;\n\n    return prevScrollRect;\n}\n",
         "export default function getLookup(elements) {\n    return elements.reduce((lookup, element) => lookup.set(element.key, element), new Map());\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default function getHighlightedCells(isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup) {\n    if (!isMouseDown)\n        return [];\n    if (isResizing)\n        return [];\n    if (!hoveredCell)\n        return [];\n    if (!focusedCell)\n        return [];\n\n    const focusedColumnKey = stringifyId(focusedCell.columnId);\n    const focusedRowKey = stringifyId(focusedCell.rowId);\n    const hoveredColumnKey = stringifyId(hoveredCell.columnId);\n    const hoveredRowKey = stringifyId(hoveredCell.rowId);\n\n    if (!columnLookup.has(focusedColumnKey))\n        return [];\n    if (!rowLookup.has(focusedRowKey))\n        return [];\n    if (!columnLookup.has(hoveredColumnKey))\n        return [];\n    if (!rowLookup.has(hoveredRowKey))\n        return [];\n\n    const minColumnIndex = Math.min(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const maxColumnIndex = Math.max(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const minRowIndex = Math.min(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n    const maxRowIndex = Math.max(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n\n    return columns.slice(minColumnIndex, maxColumnIndex + 1).flatMap(column => {\n        return rows.slice(minRowIndex, maxRowIndex + 1).map(row => {\n            return {\n                rowId: row.id,\n                columnId: column.id\n            };\n        });\n    });\n}\n",
         "function getVerticalSection(row) {\n    if (row.pinned === \"BEGIN\")\n        return \"top\";\n    if (row.pinned === \"END\")\n        return \"bottom\";\n    return \"middle\";\n}\n\nfunction getHorizontalSection(column) {\n    if (column.pinned === \"BEGIN\")\n        return \"left\";\n    if (column.pinned === \"END\")\n        return \"right\";\n    return \"center\";\n}\n\nexport default function getCellSection(column, row) {\n    const verticalSection = getVerticalSection(row);\n    const horizontalSection = getHorizontalSection(column);\n\n    return `${verticalSection}-${horizontalSection}`;\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getCellSection from \"./getCellSection.js\";\n\nexport default function getInputPlacement(editableCells, focusedCell, columnLookup, rowLookup, sections) {\n    if (!focusedCell)\n        return null;\n\n    const focusedColumnKey = stringifyId(focusedCell.columnId);\n    const focusedRowKey = stringifyId(focusedCell.rowId);\n\n    if (!columnLookup.has(focusedColumnKey))\n        return null;\n    if (!rowLookup.has(focusedRowKey))\n        return null;\n\n    const column = columnLookup.get(focusedColumnKey);\n    const row = rowLookup.get(focusedRowKey);\n\n    if (editableCells.length === 0)\n        return null;\n\n    const position = {\n        width: column.width,\n        height: row.height,\n        section: getCellSection(column, row)\n    };\n\n    switch (row.pinned) {\n        case \"BEGIN\":\n            position.top = row.top;\n            break;\n        case \"END\":\n            position.bottom = sections.top.height + sections.middle.height + sections.bottom.height - row.top - row.height;\n            break;\n        default:\n            position.marginTop = row.top - sections.top.height;\n    }\n\n    switch (column.pinned) {\n        case \"BEGIN\":\n            position.left = column.left;\n            break;\n        case \"END\":\n            position.right = sections.left.width + sections.center.width + sections.right.width - column.left - column.width;\n            break;\n        default:\n            position.marginLeft = column.left - sections.left.width;\n    }\n\n    return position;\n}\n",
         "export default function getIsTextValid(text, editableCells) {\n    return editableCells.every(cell => cell.edit.validate({ string: text }));\n}\n",
-        "function getDefaultIds(elements) {\n    if (!Array.isArray(elements))\n        return Object.keys(elements);\n\n    return elements.map((_, index) => index);\n}\n\nfunction getDefaultRowIds(data) {\n    return getDefaultIds(data);\n}\n\nfunction getDefaultColumnIds(data) {\n    if (Array.isArray(data)) {\n        if (data.length > 0)\n            return Object.keys(data[0]);\n        return [];\n    } else {\n        const keys = Object.keys(data);\n        if (keys.length > 0)\n            return getDefaultIds(data[keys[0]]);\n        return [];\n    }\n}\n\nexport function getUnfoldedColumns(columns, data) {\n    const hasDataBlocks = columns.some(column => column.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return columns;\n\n    const unfoldedColumns = [];\n\n    for (const column of columns) {\n        if (column.type === 'DATA-BLOCK') {\n            const ids = 'selector' in column\n                ? column.selector(data)\n                : getDefaultColumnIds(data);\n\n            for (const id of ids) {\n                unfoldedColumns.push({\n                    ...column,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedColumns.push(column);\n        }\n    }\n\n    return unfoldedColumns;\n}\n\nexport function getUnfoldedRows(rows, data) {\n    const hasDataBlocks = rows.some(row => row.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return rows;\n\n    const unfoldedRows = [];\n\n    for (const row of rows) {\n        if (row.type === 'DATA-BLOCK') {\n            const ids = 'selector' in row\n                ? row.selector(data)\n                : getDefaultRowIds(data);\n\n            for (const id of ids) {\n                unfoldedRows.push({\n                    ...row,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedRows.push(row);\n        }\n    }\n\n    return unfoldedRows;\n}",
+        "function getDefaultIds(elements) {\n    if (!Array.isArray(elements))\n        return Object.keys(elements);\n\n    return elements.map((_, index) => index);\n}\n\nfunction getDefaultRowIds(data) {\n    return getDefaultIds(data);\n}\n\nfunction getDefaultColumnIds(data) {\n    const keys = new Set();\n\n    if (Array.isArray(data)) {\n        for (const element of data) {\n            for (const id of getDefaultIds(element))\n                keys.add(id);\n        }\n    } else {\n        for (const key in data) {\n            for (const id of getDefaultIds(data[key]))\n                keys.add(id);\n        }\n    }\n\n    return [...keys];\n}\n\nexport function getUnfoldedColumns(columns, data) {\n    const hasDataBlocks = columns.some(column => column.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return columns;\n\n    const unfoldedColumns = [];\n\n    for (const column of columns) {\n        if (column.type === 'DATA-BLOCK') {\n            const ids = 'selector' in column\n                ? column.selector(data)\n                : getDefaultColumnIds(data);\n\n            for (const id of ids) {\n                unfoldedColumns.push({\n                    ...column,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedColumns.push(column);\n        }\n    }\n\n    return unfoldedColumns;\n}\n\nexport function getUnfoldedRows(rows, data) {\n    const hasDataBlocks = rows.some(row => row.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return rows;\n\n    const unfoldedRows = [];\n\n    for (const row of rows) {\n        if (row.type === 'DATA-BLOCK') {\n            const ids = 'selector' in row\n                ? row.selector(data)\n                : getDefaultRowIds(data);\n\n            for (const id of ids) {\n                unfoldedRows.push({\n                    ...row,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedRows.push(row);\n        }\n    }\n\n    return unfoldedRows;\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst defaultCondition = ({ text, expression }) => text.includes(expression);\n\nexport default class FilteringRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'FILTER'),\n                condition: rule.condition || defaultCondition\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, value, text, filterLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return true;\n            if (column.type !== 'DATA')\n                return true;\n            if (!filterLookup.has('\"FILTER\"'))\n                return true;\n\n            return defaultCondition({ text, expression: filterLookup.get('\"FILTER\"') });\n        }\n\n        let context = { data, rows, columns, row, column, value, text };\n\n        for (const rule of rules) {\n            if (!filterLookup.has(rule.by))\n                continue;\n\n            const filterContext = { ...context, expression: filterLookup.get(rule.by) };\n\n            if (!rule.condition(filterContext))\n                return false;\n        }\n\n        return true;\n    }\n}",
         "import FilteringRules from \"../types/FilteringRules.js\";\n\nexport default function getFilteringRules(filtering) {\n    return new FilteringRules(filtering);\n}",
         "export default function getFilterFormatting(formatting) {\n    return formatting;\n}",
         "export default function getMeasureFormatting(formatting) {\n    return formatting;\n}",
         "import { defaultPadding } from \"../core-utils/defaults.js\";\n\n// TODO: add expand and expand-data\n\nexport function getMeasuredColumns(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (columns.every(column => typeof column.width === 'number'))\n        return columns;\n\n    const measureColumn = column => {\n        const requestedWidth = 'width' in column ? column.width : 'fit-once';\n\n        if (typeof requestedWidth === 'number')\n            return requestedWidth;\n\n        if (measuringCache.has(column.key)) {\n            const cached = measuringCache.get(column.key);\n\n            if (requestedWidth === 'fit-once' && !cached.dataOnly)\n                return cached.width;\n            if (requestedWidth === 'fit-data-once' && cached.dataOnly)\n                return cached.width;\n        }\n\n        let width = 0;\n        for (const row of rows) {\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data-once')\n                continue;\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.left + cell.padding.right;\n\n            const cellWidth = textResolver.measureWidth(text, font) + padding;\n\n            width = Math.max(width, cellWidth);\n        }\n\n        measuringCache.set(column.key, {\n            width,\n            dataOnly: requestedWidth === 'fit-data-once'\n        });\n\n        return width;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return columns.map(column => ({\n        ...column,\n        width: measureColumn(column)\n    }));\n}\n\nexport function getMeasuredRows(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (rows.every(row => typeof row.height === 'number'))\n        return rows;\n\n    const measureRow = row => {\n        const requestedHeight = 'height' in row ? row.height : 'fit-once';\n\n        if (typeof requestedHeight === 'number')\n            return requestedHeight;\n\n        if (measuringCache.has(row.key)) {\n            const cached = measuringCache.get(row.key);\n\n            if (requestedHeight === 'fit-once' && !cached.dataOnly)\n                return cached.height;\n            if (requestedHeight === 'fit-data-once' && cached.dataOnly)\n                return cached.height;\n        }\n\n        let height = 0;\n        for (const column of columns) {\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data-once')\n                continue;\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.top + cell.padding.bottom;\n\n            const cellHeight = textResolver.measureHeight(text, font) + padding;\n\n            height = Math.max(height, cellHeight);\n        }\n\n        measuringCache.set(row.key, {\n            height,\n            dataOnly: requestedHeight === 'fit-data-once'\n        });\n\n        return height;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return rows.map(row => ({\n        ...row,\n        height: measureRow(row)\n    }));\n}",
         "export default function getKeys(entries) {\n    return new Set(entries.map(entry => entry.key));\n}\n",
         "export default function getSortingFormatting(formatting) {\n    return formatting;\n}",
-        "import RulesLookup from \"./RulesLookup.js\";\n\nconst defaultComparatorAsc = (lhs, rhs) => lhs.value < rhs.value;\nconst defaultComparatorDesc = (lhs, rhs) => lhs.value > rhs.value;\n\nexport default class SortingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'HEADER'),\n                comparatorAsc: rule.comparator || defaultComparatorAsc,\n                comparatorDesc: (lhs, rhs) => -rule.comparator(lhs, rhs) || defaultComparatorDesc\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(column, row, sortByLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return null;\n            if (column.type !== 'DATA')\n                return null;\n            if (!sortByLookup.has('\"HEADER\"'))\n                return null;\n\n            return sortByLookup.get('\"HEADER\"') === 'ASC'\n                ? defaultComparatorAsc\n                : defaultComparatorDesc;\n        }\n\n        if (rules.length > 1)\n            throw new Error('Multiple sorting rules for the same cell'); // TODO: add more context\n\n        const rule = rules[0];\n\n        return sortByLookup.get(rule.by) === 'ASC'\n            ? rule.comparatorAsc\n            : rule.comparatorDesc;\n    }\n}",
+        "import RulesLookup from \"./RulesLookup.js\";\n\n// const defaultComparatorAsc = (lhs, rhs) => lhs.value < rhs.value;\n// const defaultComparatorDesc = (lhs, rhs) => lhs.value > rhs.value;\n\nfunction defaultComparatorAsc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value < rhs.value;\n}\n\nfunction defaultComparatorDesc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value > rhs.value;\n}\n\nexport default class SortingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'HEADER'),\n                comparatorAsc: rule.comparator || defaultComparatorAsc,\n                comparatorDesc: (lhs, rhs) => -rule.comparator(lhs, rhs) || defaultComparatorDesc\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(column, row, sortByLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return null;\n            if (column.type !== 'DATA')\n                return null;\n            if (!sortByLookup.has('\"HEADER\"'))\n                return null;\n\n            return sortByLookup.get('\"HEADER\"') === 'ASC'\n                ? defaultComparatorAsc\n                : defaultComparatorDesc;\n        }\n\n        if (rules.length > 1)\n            throw new Error('Multiple sorting rules for the same cell'); // TODO: add more context\n\n        const rule = rules[0];\n\n        return sortByLookup.get(rule.by) === 'ASC'\n            ? rule.comparatorAsc\n            : rule.comparatorDesc;\n    }\n}",
         "import SortingRules from \"../types/SortingRules.js\";\n\nexport default function getSortingRules(sorting) {\n    return new SortingRules(sorting);\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction getSortByLookup(sortBy, primaryKey, secondaryKey) {\n    const sortByLookup = new Map();\n    for (const cell of sortBy) {\n        const primary = stringifyId(cell[primaryKey]);\n        const secondary = stringifyId(cell[secondaryKey]);\n\n        if (!sortByLookup.has(primary))\n            sortByLookup.set(primary, new Map());\n\n        sortByLookup.get(primary).set(secondary, cell.direction);\n    }\n    return sortByLookup;\n}\n\nfunction flush(temp, result) {\n    temp.sort((lhs, rhs) => {\n        const result = lhs.comparator(lhs.cell, rhs.cell);\n        if (typeof result === 'number')\n            return result;\n        return result ? -1 : 1;\n    });\n    result.push(...temp.map(entry => entry.entity));\n    temp.length = 0;\n}\n\nexport function getSortedRows(sortBy, sortingRules, formattingRules, data, rows, columns, edition) {\n    if (sortBy.length === 0)\n        return rows;\n\n    const sortByLookup = getSortByLookup(sortBy, 'columnId', 'rowId');\n    const columnLookup = new Map(columns.map(column => [column.key, column]));\n    const sortedColumns = sortBy\n        .map(cell => stringifyId(cell.columnId))\n        .filter(key => columnLookup.has(key))\n        .map(key => columnLookup.get(key))\n        .reverse();\n\n    if (sortedColumns.length === 0)\n        return rows;\n\n    for (const column of sortedColumns) {\n        const result = [];\n        const temp = [];\n\n        for (const row of rows) {\n            const comparator = sortingRules.resolve(column, row, sortByLookup.get(column.key));\n\n            if (!comparator) {\n                flush(temp, result);\n                result.push(row);\n                continue;\n            }\n\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const entry = { entity: row, comparator, cell };\n\n            if (temp.length === 0) {\n                temp.push(entry);\n                continue;\n            }\n\n            if (temp[0].comparator === comparator) {\n                temp.push(entry);\n                continue;\n            }\n\n            flush(temp, result);\n            temp.push(entry);\n        }\n\n        flush(temp, result);\n        rows = result;\n    }\n\n    return rows;\n}\n\nexport function getSortedColumns(sortBy, sortingRules, formattingRules, data, rows, columns, edition) {\n    if (sortBy.length === 0)\n        return columns;\n\n    const sortByLookup = getSortByLookup(sortBy, 'rowId', 'columnId');\n    const rowLookup = new Map(rows.map(row => [row.key, row]));\n    const sortedRows = sortBy\n        .map(cell => stringifyId(cell.rowId))\n        .filter(key => rowLookup.has(key))\n        .map(key => rowLookup.get(key))\n        .reverse();\n\n    if (sortedRows.length === 0)\n        return columns;\n\n    for (const row of sortedRows) {\n        const result = [];\n        const temp = [];\n\n        for (const column of columns) {\n            const comparator = sortingRules.resolve(column, row, sortByLookup.get(row.key));\n\n            if (!comparator) {\n                flush(temp, result);\n                result.push(column);\n                continue;\n            }\n\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const entry = { entity: column, comparator, cell };\n\n            if (temp.length === 0) {\n                temp.push(entry);\n                continue;\n            }\n\n            if (temp[0].comparator === comparator) {\n                temp.push(entry);\n                continue;\n            }\n\n            flush(temp, result);\n            temp.push(entry);\n        }\n\n        flush(temp, result);\n        columns = result;\n    }\n\n    return columns;\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nconst grabOffset = 5;\n\n// TODO: not working when scrolled\n\nexport function getResizableColumn(columns, columnLookup, rowLookup, hoveredCell, mousePosition) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n    const x = mousePosition.x;\n\n    if (row.type !== 'HEADER')\n        return null;\n\n    if (x >= column.right - grabOffset && x <= column.right + grabOffset)\n        return column.id;\n\n    if (column.index === 0)\n        return null;\n    if (x < column.left - grabOffset || x > column.left + grabOffset)\n        return null;\n\n    return columns[column.index - 1].id;\n}\n\nexport function getResizableRow(rows, columnLookup, rowLookup, hoveredCell, mousePosition) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n    const y = mousePosition.y;\n\n    if (column.type !== 'HEADER')\n        return null;\n\n    if (y >= row.bottom - grabOffset && y <= row.bottom + grabOffset)\n        return row.id;\n\n    if (row.index === 0)\n        return null;\n    if (y < row.top - grabOffset || y > row.top + grabOffset)\n        return null;\n\n    return rows[row.index - 1].id;\n}",
         "export default function getResolvedSortBy(sortBy) {\n    return sortBy.map(sort => ({\n        columnId: 'columnId' in sort ? sort.columnId : 'HEADER',\n        rowId: 'rowId' in sort ? sort.rowId : 'HEADER',\n        direction: sort.direction\n    }));\n}",
         "export default function getResolvedFilters(filters) {\n    return filters.map(filter => ({\n        columnId: 'columnId' in filter ? filter.columnId : 'FILTER',\n        rowId: 'rowId' in filter ? filter.rowId : 'FILTER',\n        expression: filter.expression\n    }));\n}",
         "function getActive(entries, callback) {\n    const ids = entries\n        .filter(entry => entry.type === 'DATA')\n        .map(entry => entry.id);\n\n    callback(ids);\n\n    return ids;\n}\n\nexport function getActiveColumns(columns, callback) {\n    return getActive(columns, callback);\n}\n\nexport function getActiveRows(rows, callback) {\n    return getActive(rows, callback);\n}",
         "import getEditableCells from \"../state-utils/getEditableCells.js\";\nimport getDataFormatting from \"../state-utils/getDataFormatting.js\";\nimport getInputFormatting from \"../state-utils/getInputFormatting.js\";\nimport getRenderFormatting from \"../state-utils/getRenderFormatting.js\";\nimport getSections from \"../state-utils/getSections.js\";\nimport getEditedCellsAndFilters from \"../state-utils/getEditedCellsAndFilters.js\";\nimport getEdition from \"../state-utils/getEdition.js\";\nimport getSelection from \"../state-utils/getSelection.js\";\nimport getInvoked from \"../state-utils/getInvoked.js\";\nimport { getResolvedColumns, getResolvedRows } from \"../state-utils/getResolved.js\";\nimport { getPlacedColumns, getPlacedRows } from \"../state-utils/getPlaced.js\";\nimport getFormattingRules from \"../state-utils/getFormattingRules.js\";\nimport getFormatResolver from \"../state-utils/getFormatResolver.js\";\nimport { getFilteredColumns as getFilteredColumns, getFilteredRows as getFilteredRows } from \"../state-utils/getFiltered.js\";\nimport getFixedSize from \"../state-utils/getFixedSize.js\";\nimport getTotalSize from \"../state-utils/getTotalSize.js\";\nimport getTextResolver from \"../state-utils/getTextResolver.js\";\nimport getScrollRect from \"../state-utils/getScrollRect.js\";\nimport getHoveredCell from \"../state-utils/getHoveredCell.js\";\nimport getLookup from \"../state-utils/getLookup.js\";\nimport getHighlightedCells from \"../state-utils/getHighlightedCells.js\";\nimport getInputPlacement from \"../state-utils/getInputPlacement.js\";\nimport getIsTextValid from \"../state-utils/getIsTextValid.js\";\nimport { getUnfoldedColumns, getUnfoldedRows } from \"../state-utils/getUnfolded.js\";\nimport getFilteringRules from \"../state-utils/getFilteringRules.js\";\nimport getFilterFormatting from \"../state-utils/getFilterFormatting.js\";\nimport getMeasureFormatting from \"../state-utils/getMeasureFormatting.js\";\nimport { getMeasuredColumns, getMeasuredRows } from \"../state-utils/getMeasured.js\";\nimport getKeys from \"../state-utils/getKeys.js\";\nimport getSortingFormatting from \"../state-utils/getSortingFormatting.js\";\nimport getSortingRules from \"../state-utils/getSortingRules.js\";\nimport { getSortedColumns, getSortedRows } from \"../state-utils/getSorted.js\";\nimport { getResizableColumn, getResizableRow } from \"../state-utils/getResizable.js\";\nimport getResolvedSortBy from \"../state-utils/getResolvedSortBy.js\";\nimport getResolvedFilters from \"../state-utils/getResolvedFilters.js\";\nimport { getActiveColumns } from \"../state-utils/getActive.js\";\n\n// TODO: write some test to check if the cache is working properly\nfunction updateStateInternal(context) {\n    console.count('updateState');\n\n    const options = { ...context.localOptions, ...context.externalOptions };\n    const memory = context.memory;\n    const previousState = context.state;\n\n    // TODO: Move to utils\n    function cache(key, func, dependencies) {\n        const previousDependencies = memory[key] && memory[key].dependencies;\n        if (!previousDependencies || dependencies.some((dependency, index) => dependency !== previousDependencies[index]))\n            memory[key] = { value: func(...dependencies), dependencies };\n        return memory[key].value;\n    }\n\n    const devicePixelRatio = window.devicePixelRatio; // TODO: Trigger update on devicePixelRatio change\n    const borderWidth = options.borderWidth / devicePixelRatio;\n    const data = options.data;\n    const text = context.input.value;\n    const sortBy = cache('sortBy', getResolvedSortBy, [options.sortBy]);\n    const filters = cache('filters', getResolvedFilters, [options.filters]);\n    const textResolver = cache('textResolver', getTextResolver, []);\n    const dataFormatting = cache('dataFormatting', getDataFormatting, [options.formatting, options.dataSelector, sortBy]);\n    const editedCellsAndFilters = cache('editedCellsAndFilters', getEditedCellsAndFilters, [options.editedCells, filters]);\n    const edition = cache('edition', getEdition, [editedCellsAndFilters]);\n    const invokedColumns = cache('invokedColumns', getInvoked, [options.columns, data]);\n    const invokedRows = cache('invokedRows', getInvoked, [options.rows, data]);\n    // TODO: throw on duplicate ids\n    // TODO: throw on duplicate row/column filter ids\n    const unfoldedColumns = cache('unfoldedColumns', getUnfoldedColumns, [invokedColumns, data]);\n    const unfoldedRows = cache('unfoldedRows', getUnfoldedRows, [invokedRows, data]);\n    const unfilteredColumns = cache('unfilteredColumns', getResolvedColumns, [unfoldedColumns, options.pinnedLeft, options.pinnedRight, options.columnWidths]);\n    const unfilteredRows = cache('unfilteredRows', getResolvedRows, [unfoldedRows, options.pinnedTop, options.pinnedBottom, options.rowHeights]);\n    const unfilteredColumnKeys = cache('unfilteredColumnKeys', getKeys, [unfilteredColumns]);\n    const unfilteredRowKeys = cache('unfilteredRowKeys', getKeys, [unfilteredRows]);\n\n    // Filtering\n    const filterFormatting = cache('filterFormatting', getFilterFormatting, [dataFormatting]);\n    const filterFormattingRules = cache('filterFormattingRules', getFormattingRules, [filterFormatting]);\n    const filteringRules = cache('filteringRules', getFilteringRules, [options.filtering]);\n    const filteredColumns = cache('filteredColumns', getFilteredColumns, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n    const filteredRows = cache('filteredRows', getFilteredRows, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n\n    // Sorting\n    const sortingFormatting = cache('sortingFormatting', getSortingFormatting, [dataFormatting]);\n    const sortingFormattingRules = cache('sortingFormattingRules', getFormattingRules, [sortingFormatting]);\n    const sortingRules = cache('sortingRules', getSortingRules, [options.sorting]);\n    const sortedColumns = cache('sortedColumns', getSortedColumns, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n    const sortedRows = cache('sortedRows', getSortedRows, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n\n    // Shaping\n    const shapedColumns = sortedColumns;\n    const shapedRows = sortedRows;\n\n    // Measuring\n    const measureFormatting = cache('measureFormatting', getMeasureFormatting, [dataFormatting]);\n    const measureFormattingRules = cache('measureFormattingRules', getFormattingRules, [measureFormatting]);\n    const measureFormatResolver = cache('measureFormatResolver', getFormatResolver, [measureFormattingRules, data, shapedRows, shapedColumns, edition]);\n    const columnWidthCache = context.columnWidthCache;\n    const rowHeightCache = context.rowHeightCache;\n    const measuredColumns = cache('measuredColumns', getMeasuredColumns, [shapedColumns, shapedRows, textResolver, measureFormatResolver, columnWidthCache, unfilteredColumnKeys]);\n    const measuredRows = cache('measuredRows', getMeasuredRows, [shapedColumns, shapedRows, textResolver, measureFormatResolver, rowHeightCache, unfilteredRowKeys]);\n\n    // Placement\n    const columns = cache('columns', getPlacedColumns, [measuredColumns, devicePixelRatio, borderWidth]);\n    const rows = cache('rows', getPlacedRows, [measuredRows, devicePixelRatio, borderWidth]);\n    const columnLookup = cache('columnLookup', getLookup, [columns]);\n    const rowLookup = cache('rowLookup', getLookup, [rows]);\n    const focusedCell = options.focusedCell;\n    const sections = cache('sections', getSections, [columns, rows]);\n    const selectedCells = options.selectedCells;\n    const fixedSize = cache('fixedSize', getFixedSize, [sections.top.height, sections.bottom.height, sections.left.width, sections.right.width]);\n    const totalSize = cache('totalSize', getTotalSize, [columns, rows]);\n    // TODO: do some proper caching, so that if value is not changed, the old value is returned (currently not working because of scrolling)\n    const hoveredCell = getHoveredCell(context.element, context.mousePosition, rows, columns, fixedSize, totalSize);\n    const resizableColumn = context.resizingColumn || cache('resizableColumn', getResizableColumn, [columns, columnLookup, rowLookup, hoveredCell, context.mousePosition]);\n    const resizableRow = context.resizingRow || cache('resizableRow', getResizableRow, [rows, columnLookup, rowLookup, hoveredCell, context.mousePosition]);\n    const isMouseDown = context.isMouseDown;\n    const isResizing = !!resizableColumn || !!resizableRow;\n    const highlightedCells = cache('highlightedCells', getHighlightedCells, [isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup]);\n    const selection = cache('selection', getSelection, [selectedCells]);\n    const highlight = cache('highlight', getSelection, [highlightedCells]);\n    // TODO: addDataFormattingRules and addRenderFormattingRules should remove unnecessary rules\n    const renderFormatting = cache('renderFormatting', getRenderFormatting, [dataFormatting, hoveredCell, focusedCell, selection, highlight, edition, resizableColumn, resizableRow]);\n    const renderFormattingRules = cache('renderFormattingRules', getFormattingRules, [renderFormatting]);\n    const renderFormatResolver = cache('renderFormatResolver', getFormatResolver, [renderFormattingRules, data, rows, columns, edition]);\n    const inputFormatting = cache('inputFormatting', getInputFormatting, [dataFormatting]);\n    const inputFormattingRules = cache('inputFormattingRules', getFormattingRules, [inputFormatting]);\n    const inputFormatResolver = cache('inputFormatResolver', getFormatResolver, [inputFormattingRules, data, rows, columns, edition]);\n    const editableCells = cache('editableCells', getEditableCells, [selectedCells, inputFormatResolver, columnLookup, rowLookup]);\n    const inputPlacement = cache('inputPlacement', getInputPlacement, [editableCells, focusedCell, columnLookup, rowLookup, sections]);\n    const isTextValid = cache('isTextValid', getIsTextValid, [text, editableCells]);\n\n    // cache result, but not call\n    const scrollRect = getScrollRect(previousState?.scrollRect, totalSize, fixedSize, context.element);\n\n    // callbacks\n    cache('activeColumns', getActiveColumns, [columns, options.onActiveColumnsChange]);\n    cache('activeRows', getActiveColumns, [rows, options.onActiveRowsChange]);\n\n    context.state = {\n        options,\n        devicePixelRatio,\n        borderWidth,\n        data,\n        dataFormatting,\n        edition,\n        filteredColumns,\n        filteredRows,\n        columns,\n        rows,\n        sections,\n        selectedCells,\n        selection,\n        highlight,\n        hoveredCell,\n        focusedCell,\n        renderFormatting,\n        renderFormatResolver,\n        inputFormatting,\n        inputFormatResolver,\n        fixedSize,\n        totalSize,\n        textResolver,\n        scrollRect,\n        highlightedCells,\n        inputPlacement,\n        columnLookup,\n        rowLookup,\n        text,\n        isTextValid,\n        resizableColumn,\n        resizableRow,\n    };\n}\n\nexport default function updateState(context) {\n    if (!context.error) {\n        try {\n            updateStateInternal(context);\n        } catch (error) {\n            context.error = error;\n        }\n    }\n}",
         "import getColumnIndex from \"./getColumnIndex.js\";\nimport getRowIndex from \"./getRowIndex.js\";\n\nexport default function getHoveredCell(element, mousePosition, rows, columns, fixedSize, totalSize) {\n    // TODO: sometimes mousePosition is outside of bounds and it crashes the click events\n\n    if (!mousePosition)\n        return null;\n    if (mousePosition.x < 0 || mousePosition.y < 0 || mousePosition.x > totalSize.width || mousePosition.y > totalSize.height)\n        return null;\n\n    const scrollOffset = {\n        left: element.scrollLeft,\n        top: element.scrollTop\n    };\n\n    const clientSize = {\n        width: element.clientWidth,\n        height: element.clientHeight\n    };\n\n    const x = mousePosition.x <= fixedSize.left\n        ? mousePosition.x\n        : mousePosition.x >= clientSize.width - fixedSize.right\n            ? totalSize.width - clientSize.width + mousePosition.x\n            : mousePosition.x + scrollOffset.left;\n    const y = mousePosition.y <= fixedSize.top\n        ? mousePosition.y\n        : mousePosition.y >= clientSize.height - fixedSize.bottom\n            ? totalSize.height - clientSize.height + mousePosition.y\n            : mousePosition.y + scrollOffset.top;\n\n    const hoverRowIndex = getRowIndex(rows, y);\n    const hoverColumnIndex = getColumnIndex(columns, x);\n\n    if (hoverRowIndex === -1 || hoverColumnIndex === -1)\n        return null;\n\n    return {\n        rowId: rows[hoverRowIndex].id,\n        columnId: columns[hoverColumnIndex].id\n    };\n}\n",
         "export default function getRowIndex(rows, y) {\n    if (rows.length === 0)\n        return -1;\n    if (y < rows[0].topWithBorder)\n        return -1;\n    if (y > rows[rows.length - 1].bottomWithBorder)\n        return -1;\n\n    let iterA = 0;\n    let iterC = rows.length - 1;\n\n    while (iterA <= iterC) {\n        const iterB = Math.floor((iterA + iterC) / 2);\n\n        if (y < rows[iterB].topWithBorder)\n            iterC = iterB - 1;\n        else if (y > rows[iterB].bottomWithBorder)\n            iterA = iterB + 1;\n\n        else\n            return iterB;\n    }\n\n    return -1;\n}\n",
         "export default function getColumnIndex(columns, x) {\n    if (columns.length === 0)\n        return -1;\n    if (x < columns[0].leftWithBorder)\n        return -1;\n    if (x > columns[columns.length - 1].rightWithBorder)\n        return -1;\n\n    let iterA = 0;\n    let iterC = columns.length - 1;\n\n    while (iterA <= iterC) {\n        const iterB = Math.floor((iterA + iterC) / 2);\n\n        if (x < columns[iterB].leftWithBorder)\n            iterC = iterB - 1;\n        else if (x > columns[iterB].rightWithBorder)\n            iterA = iterB + 1;\n\n        else\n            return iterB;\n    }\n\n    return -1;\n}\n",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getCombinedCells(previousCells, newCells) {\n    const selection = new Selection(newCells);\n    return [...newCells, ...previousCells.filter(cell => !selection.isIdSelected(cell.rowId, cell.columnId))];\n}\n",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getReducedCells(previousCells, cellsToRemove) {\n    const selection = new Selection(cellsToRemove);\n    return previousCells.filter(cell => !selection.isIdSelected(cell.rowId, cell.columnId));\n}\n",
         "export default function getMousePosition(event) {\n    const element = event.currentTarget;\n    const rect = element.getBoundingClientRect();\n    return {\n        x: event.clientX - rect.left,\n        y: event.clientY - rect.top\n    };\n}",
-        "import getEditableCells from \"./state-utils/getEditableCells.js\";\nimport stringifyId from \"./core-utils/stringifyId.js\";\nimport render from \"./core/render.js\";\nimport updateState from \"./core/state.js\";\nimport getCombinedCells from \"./state-utils/getCombinedCells.js\";\nimport getReducedCells from \"./state-utils/getReducedCells.js\";\nimport getMousePosition from \"./state-utils/getMousePosition.js\";\nimport getNewSortBy from \"./state-utils/getNewSortBy.js\";\nimport getClipboardData from \"./state-utils/getClipboardData.js\";\n\nfunction initialize(element) {\n    if ('spread-grid-context' in element) return;\n\n    console.log('initialize');\n\n    const canvases = {\n        'top-left': document.createElement('canvas'),\n        'top-center': document.createElement('canvas'),\n        'top-right': document.createElement('canvas'),\n        'middle-left': document.createElement('canvas'),\n        'middle-center': document.createElement('canvas'),\n        'middle-right': document.createElement('canvas'),\n        'bottom-left': document.createElement('canvas'),\n        'bottom-center': document.createElement('canvas'),\n        'bottom-right': document.createElement('canvas')\n    };\n    const input = document.createElement('input');\n\n    element.setAttribute('tabindex', '0');\n    element.setAttribute('style', 'max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;');\n    element.classList.add('spread-grid');\n    canvases['top-left'].setAttribute('style', 'position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;');\n    canvases['top-center'].setAttribute('style', 'position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;');\n    canvases['top-right'].setAttribute('style', 'position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;');\n    canvases['middle-left'].setAttribute('style', 'position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;');\n    canvases['middle-center'].setAttribute('style', 'grid-row: 2; grid-column: 2; z-index: 0;');\n    canvases['middle-right'].setAttribute('style', 'position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;');\n    canvases['bottom-left'].setAttribute('style', 'position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;');\n    canvases['bottom-center'].setAttribute('style', 'position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;');\n    canvases['bottom-right'].setAttribute('style', 'position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;');\n    input.setAttribute('style', 'position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;');\n\n    const context = {\n        externalOptions: {},\n        state: null,\n        memory: {},\n        element: element,\n        canvases: canvases,\n        input: input,\n        renderRequested: false,\n        mousePosition: null,\n        isMouseDown: false,\n        columnWidthCache: new Map(),\n        rowHeightCache: new Map(),\n    };\n\n    context.requestNewRender = () => {\n        if (context.renderRequested) return;\n        context.renderRequested = true;\n        requestAnimationFrame(() => {\n            context.renderRequested = false;\n            updateState(context);\n            render(context);\n        });\n    };\n\n    context.addEventListener = (element, type, listener) => {\n        element.addEventListener(type, (event) => {\n            try {\n                listener(event);\n            }\n            catch (error) {\n                error.message = `[${type} event]: ${error.message}`;\n                context.error = error;\n                context.requestNewRender();\n            }\n        });\n    }\n\n    context.localOptions = {\n        data: [],\n        columns: [{ type: 'DATA-BLOCK' }],\n        rows: [{ type: 'HEADER' }, { type: 'DATA-BLOCK' }],\n        formatting: [],\n        filtering: [],\n        sorting: [],\n        dataSelector: ({ data, row, column }) => data[row.id][column.id],\n        pinnedTop: 0,\n        pinnedBottom: 0,\n        pinnedLeft: 0,\n        pinnedRight: 0,\n        borderWidth: 1,\n        focusedCell: null,\n        onFocusedCellChange: (focusedCell) => {\n            context.localOptions.focusedCell = focusedCell;\n            context.requestNewRender();\n        },\n        selectedCells: [],\n        onSelectedCellsChange: (selectedCells) => {\n            context.localOptions.selectedCells = selectedCells;\n            context.requestNewRender();\n        },\n        highlightedCells: [],\n        editedCells: [],\n        onEditedCellsChange: (editedCells) => {\n            // TODO: optimize by coalescing\n            context.localOptions.editedCells = editedCells;\n            context.requestNewRender();\n        },\n        filters: [],\n        onFiltersChange: (filters) => {\n            context.localOptions.filters = filters;\n            context.requestNewRender();\n        },\n        sortBy: [],\n        onSortByChange: (sortBy) => {\n            context.localOptions.sortBy = sortBy;\n            context.requestNewRender();\n        },\n        onCellClick: () => { },\n        onCustomCellClick: () => { },\n        columnWidths: [],\n        onColumnWidthsChange: (columnWidths) => {\n            context.localOptions.columnWidths = columnWidths;\n            context.requestNewRender();\n        },\n        rowHeights: [],\n        onRowHeightsChange: (rowHeights) => {\n            context.localOptions.rowHeights = rowHeights;\n            context.requestNewRender();\n        },\n        onActiveColumnsChange: () => { },\n        onActiveRowsChange: () => { },\n    };\n\n    element['spread-grid-context'] = context;\n\n    const setText = (text) => {\n        input.value = text;\n        input.dispatchEvent(new Event('input'));\n    }\n\n    const accept = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const text = context.state.text;\n        const isTextValid = context.state.isTextValid;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const addEditedCells = (cells) => setEditedCells(getCombinedCells(context.state.options.editedCells, cells));\n        const addFilters = (cells) => setFilters(getCombinedCells(context.state.options.filters, cells));\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (text === '')\n            return;\n        if (!isTextValid)\n            return;\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        const dataCells = editableCells.filter(cell => cell.type === 'DATA');\n        const filterCells = editableCells.filter(cell => cell.type === 'FILTER');\n\n        addEditedCells(dataCells.map(cell => ({ ...cell.cell, value: cell.edit.parse({ string: text }) })));\n        addFilters(filterCells.map(cell => ({ ...cell.cell, expression: cell.edit.parse({ string: text }) })));\n\n        if (!autoCommit)\n            setText('');\n    };\n\n    const clear = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const removeEditedCells = (cells) => setEditedCells(getReducedCells(context.state.options.editedCells, cells));\n        const removeFilters = (cells) => setFilters(getReducedCells(context.state.options.filters, cells));\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        removeEditedCells(selectedCells);\n        removeFilters(selectedCells);\n    }\n\n    // TODO: Move other input functions here as well\n\n    context.addEventListener(element, 'scroll', (event) => {\n        // TODO: only request new render if scroll position changed outside of the scope\n        // TODO: how to: calculate the new scrollRect here and compare it to the one in the state\n        // TODO: Also don't forget to check if the highlighted cell did change\n        // TODO: Consider forcing a new render when visible scrollRect changes (without waiting for the next render frame)\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseenter', (event) => {\n        context.mousePosition = getMousePosition(event);\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mousemove', (event) => {\n        context.mousePosition = getMousePosition(event);\n\n        if (context.resizingColumn) {\n            const column = context.state.columnLookup.get(stringifyId(context.resizingColumn));\n            const columnWidth = column.width;\n            const columnRight = column.right;\n            const mousePosition = context.mousePosition.x;\n            const newColumnWidth = Math.max(10, mousePosition - columnRight + columnWidth);\n            const previousColumnWidths = context.state.options.columnWidths;\n            const newColumnWidths = previousColumnWidths\n                .filter(columnWidth => stringifyId(columnWidth.columnId) !== column.key)\n                .concat([{ columnId: column.id, width: newColumnWidth }]);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n        }\n        if (context.resizingRow) {\n            const row = context.state.rowLookup.get(stringifyId(context.resizingRow));\n            const rowHeight = row.height;\n            const rowBottom = row.bottom;\n            const mousePosition = context.mousePosition.y;\n            const newRowHeight = Math.max(10, mousePosition - rowBottom + rowHeight);\n            const previousRowHeights = context.state.options.rowHeights;\n            const newRowHeights = previousRowHeights\n                .filter(rowHeight => stringifyId(rowHeight.rowId) !== row.key)\n                .concat([{ rowId: row.id, height: newRowHeight }]);\n            context.state.options.onRowHeightsChange(newRowHeights);\n        }\n\n        // TODO: only request new render if hovered cell changed\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseleave', () => {\n        context.mousePosition = null;\n        context.requestNewRender();\n    });\n\n    // TODO: update mouse position on resize\n\n    context.addEventListener(element, 'mousedown', (event) => {\n        updateState(context);\n        setText('');\n\n        context.isMouseDown = true;\n        context.mouseDownPosition = context.mousePosition;\n        context.mouseDownCell = context.state.hoveredCell;\n\n        if (context.state.resizableColumn) {\n            context.resizingColumn = context.state.resizableColumn;\n        }\n        if (context.state.resizableRow) {\n            context.resizingRow = context.state.resizableRow;\n        }\n        if (!context.state.resizableColumn && !context.state.resizableRow) {\n            context.state.options.onFocusedCellChange(context.state.hoveredCell);\n        }\n\n        if (!event.ctrlKey)\n            context.state.options.onSelectedCellsChange([]);\n\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseup', (event) => {\n        updateState(context);\n\n        context.isMouseDown = false;\n        context.resizingColumn = null;\n        context.resizingRow = null;\n\n        context.state.options.onSelectedCellsChange(getCombinedCells(context.state.options.selectedCells, context.state.highlightedCells));\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'pointerdown', (event) => {\n        context.element.setPointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'pointerup', (event) => {\n        context.element.releasePointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'click', (event) => {\n        updateState(context);\n\n        const cell = context.state.hoveredCell;\n        const mouseDownCell = context.mouseDownCell;\n\n        if (context.state.resizableColumn || context.state.resizableRow)\n            return;\n        if (cell === null)\n            return;\n        if (stringifyId(cell.columnId) !== stringifyId(mouseDownCell.columnId))\n            return;\n        if (stringifyId(cell.rowId) !== stringifyId(mouseDownCell.rowId))\n            return;\n\n        const column = context.state.columnLookup.get(stringifyId(cell.columnId));\n        const row = context.state.rowLookup.get(stringifyId(cell.rowId));\n        const sortBy = context.state.options.sortBy;\n\n        if (column.type === 'DATA' && row.type === 'DATA') {\n            context.state.options.onCellClick(context.state.hoveredCell);\n        } else if (column.type === 'CUSTOM' || row.type === 'CUSTOM') {\n            context.state.options.onCustomCellClick(context.state.hoveredCell);\n        } else if (column.type === 'HEADER' || row.type === 'HEADER') {\n            const newSortBy = getNewSortBy(sortBy, column, row, event.ctrlKey);\n            context.state.options.onSortByChange(newSortBy);\n            context.state.options.onSelectedCellsChange([]);\n        }\n    });\n\n    context.addEventListener(element, 'dblclick', (event) => {\n        updateState(context);\n\n        if (context.state.resizableColumn) {\n            const resizableColumnKey = stringifyId(context.state.resizableColumn);\n            const newColumnWidths = context.state.options.columnWidths.filter(columnWidth => stringifyId(columnWidth.columnId) !== resizableColumnKey);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n            context.columnWidthCache.delete(resizableColumnKey);\n        }\n        if (context.state.resizableRow) {\n            const resizableRowKey = stringifyId(context.state.resizableRow);\n            const newRowHeights = context.state.options.rowHeights.filter(rowHeight => stringifyId(rowHeight.rowId) !== resizableRowKey);\n            context.state.options.onRowHeightsChange(newRowHeights);\n            context.rowHeightCache.delete(resizableRowKey);\n        }\n\n        const focusedCell = context.state.focusedCell;\n        if (focusedCell === null)\n            return;\n\n        const focusedColumnKey = stringifyId(focusedCell.columnId);\n        const focusedRowKey = stringifyId(focusedCell.rowId);\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const formatResolver = context.state.inputFormatResolver;\n\n        if (!columnLookup.has(focusedColumnKey))\n            return;\n        if (!rowLookup.has(focusedRowKey))\n            return;\n\n        const column = columnLookup.get(focusedColumnKey);\n        const row = rowLookup.get(focusedRowKey);\n        const cell = formatResolver.resolve(row, column);\n        const text = cell.text; // TODO: Make it configurable\n\n        setText(text);\n        input?.select();\n    });\n\n    context.addEventListener(element, 'focus', () => {\n        if (input.parentElement)\n            input.focus({ preventScroll: true });\n    });\n\n    context.addEventListener(element, 'keydown', (event) => {\n        // TODO: make sure it's not invoked on keydown of the input\n        updateState(context);\n\n        const focusedCell = context.state.focusedCell;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const selectedCells = context.state.options.selectedCells;\n        const setSelectedCells = context.state.options.onSelectedCellsChange;\n        const addSelectedCells = (cells) => setSelectedCells(getCombinedCells(selectedCells, cells));\n        const setFocusedCell = context.state.options.onFocusedCellChange;\n        const editedCells = context.state.options.editedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const columns = context.state.columns;\n        const rows = context.state.rows;\n        const text = context.state.text;\n        const inputFormatResolver = context.state.inputFormatResolver;\n\n        const arrowTo = (cell, event) => {\n            setFocusedCell(cell);\n\n            if (event.shiftKey)\n                addSelectedCells([cell]);\n            else\n                setSelectedCells([cell]);\n        };\n\n        const arrowHorizontally = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedColumnKey = stringifyId(focusedCell.columnId);\n            if (!columnLookup.has(focusedColumnKey))\n                return;\n\n            const focusedColumnIndex = columnLookup.get(focusedColumnKey).index;\n            const newColumnIndex = Math.max(0, Math.min(columns.length - 1, focusedColumnIndex + offset));\n            if (newColumnIndex === focusedColumnIndex)\n                return;\n\n            const newFocusedCell = { rowId: focusedCell.rowId, columnId: columns[newColumnIndex].id };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const arrowVertically = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedRowKey = stringifyId(focusedCell.rowId);\n            if (!rowLookup.has(focusedRowKey))\n                return;\n\n            const focusedRowIndex = rowLookup.get(focusedRowKey).index;\n            const newRowIndex = Math.max(0, Math.min(rows.length - 1, focusedRowIndex + offset));\n            if (newRowIndex === focusedRowIndex)\n                return;\n\n            const newFocusedCell = { rowId: rows[newRowIndex].id, columnId: focusedCell.columnId };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const preventDefault = () => {\n            event.preventDefault();\n            event.stopPropagation();\n        };\n\n        const cancel = () => {\n            if (text !== '') {\n                setText('');\n            }\n            else if (selectedCells.length > 1) {\n                setSelectedCells([focusedCell]);\n            }\n            else if (editedCells.length > 0) {\n                setEditedCells([]);\n            }\n            else {\n                setFocusedCell(null);\n                setSelectedCells([]);\n            }\n        };\n\n        const copyToClipboard = (event) => {\n            if (!event.ctrlKey)\n                return;\n\n            const clipboardData = getClipboardData(selectedCells, columns, rows, inputFormatResolver);\n\n            if (navigator.clipboard) {\n                navigator.clipboard.writeText(clipboardData);\n            } else {\n                const textArea = document.createElement('textarea');\n                textArea.value = clipboardData;\n                document.body.appendChild(textArea);\n                textArea.select();\n                document.execCommand('copy');\n                document.body.removeChild(textArea);\n            }\n        }\n\n        switch (event.key) {\n            case 'Escape':\n                cancel();\n                break;\n            case 'Enter':\n                accept();\n                break;\n            case 'ArrowUp':\n                // TODO: When ctrl and shift are pressed together, select all cells between the focused cell and the new cell\n                // TODO: When shift is pressed, expand the current rect selection instead of moving the focused cell\n                preventDefault();\n                arrowVertically(event.ctrlKey ? -rows.length : -1, event);\n                break;\n            case 'ArrowDown':\n                preventDefault();\n                arrowVertically(event.ctrlKey ? rows.length : 1, event);\n                break;\n            case 'ArrowLeft':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? -columns.length : -1, event);\n                break;\n            case 'ArrowRight':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? columns.length : 1, event);\n                break;\n            case 'Delete':\n            case 'Backspace':\n                clear();\n                break;\n            case 'c':\n                copyToClipboard(event);\n                break;\n            default:\n                break;\n        }\n    });\n\n    new ResizeObserver(() => {\n        context.requestNewRender();\n    }).observe(element);\n\n    context.addEventListener(input, 'input', (event) => {\n        // TODO: check performance of this (if it's ok to update the state on every input event)\n        updateState(context);\n\n        if (event.target.value) {\n            accept(true);\n\n            input.style.opacity = 1;\n            input.style.pointerEvents = 'auto';\n        }\n        else {\n            if (event.isTrusted)\n                clear(true);\n\n            input.style.opacity = 0;\n            input.style.pointerEvents = 'none';\n        }\n    });\n\n    context.addEventListener(input, 'click', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'dblclick', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'mousedown', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'keydown', (event) => {\n        switch (event.key) {\n            case 'Enter':\n            case 'Escape':\n                break;\n            case 'Delete':\n            case 'Backspace':\n            case 'ArrowUp':\n            case 'ArrowDown':\n            case 'ArrowLeft':\n            case 'ArrowRight':\n                if (input.value !== '') {\n                    event.stopPropagation();\n                    context.requestNewRender();\n                }\n                break;\n            default:\n                event.stopPropagation();\n                // TODO: maybe only check if the new text is valid\n                context.requestNewRender();\n                break;\n        }\n    });\n}\n\nexport default function createGrid(element, options) {\n    console.log('createGrid');\n\n    initialize(element);\n\n    const context = element['spread-grid-context'];\n    context.externalOptions = options;\n\n    if (context.state === null) {\n        updateState(context);\n        // TODO: only render if the state has sufficiently changed\n        render(context);\n    }\n    else {\n        context.requestNewRender();\n    }\n}",
+        "import getEditableCells from \"./state-utils/getEditableCells.js\";\nimport stringifyId from \"./core-utils/stringifyId.js\";\nimport render from \"./core/render.js\";\nimport updateState from \"./core/state.js\";\nimport getCombinedCells from \"./state-utils/getCombinedCells.js\";\nimport getReducedCells from \"./state-utils/getReducedCells.js\";\nimport getMousePosition from \"./state-utils/getMousePosition.js\";\nimport getNewSortBy from \"./state-utils/getNewSortBy.js\";\nimport getClipboardData from \"./state-utils/getClipboardData.js\";\nimport getToggledValue from \"./state-utils/getToggledValue.js\";\nimport getCellType from \"./state-utils/getCellType.js\";\n\nfunction initialize(element) {\n    if ('spread-grid-context' in element) return;\n\n    console.log('initialize');\n\n    const canvases = {\n        'top-left': document.createElement('canvas'),\n        'top-center': document.createElement('canvas'),\n        'top-right': document.createElement('canvas'),\n        'middle-left': document.createElement('canvas'),\n        'middle-center': document.createElement('canvas'),\n        'middle-right': document.createElement('canvas'),\n        'bottom-left': document.createElement('canvas'),\n        'bottom-center': document.createElement('canvas'),\n        'bottom-right': document.createElement('canvas')\n    };\n    const input = document.createElement('input');\n\n    element.setAttribute('tabindex', '0');\n    element.setAttribute('style', 'max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;');\n    element.classList.add('spread-grid');\n    canvases['top-left'].setAttribute('style', 'position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;');\n    canvases['top-center'].setAttribute('style', 'position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;');\n    canvases['top-right'].setAttribute('style', 'position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;');\n    canvases['middle-left'].setAttribute('style', 'position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;');\n    canvases['middle-center'].setAttribute('style', 'grid-row: 2; grid-column: 2; z-index: 0;');\n    canvases['middle-right'].setAttribute('style', 'position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;');\n    canvases['bottom-left'].setAttribute('style', 'position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;');\n    canvases['bottom-center'].setAttribute('style', 'position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;');\n    canvases['bottom-right'].setAttribute('style', 'position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;');\n    input.setAttribute('style', 'position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;');\n\n    const context = {\n        externalOptions: {},\n        state: null,\n        memory: {},\n        element: element,\n        canvases: canvases,\n        input: input,\n        renderRequested: false,\n        mousePosition: null,\n        isMouseDown: false,\n        columnWidthCache: new Map(),\n        rowHeightCache: new Map(),\n    };\n\n    context.requestNewRender = () => {\n        if (context.renderRequested) return;\n        context.renderRequested = true;\n        requestAnimationFrame(() => {\n            context.renderRequested = false;\n            updateState(context);\n            render(context);\n        });\n    };\n\n    context.addEventListener = (element, type, listener) => {\n        element.addEventListener(type, (event) => {\n            try {\n                listener(event);\n            }\n            catch (error) {\n                error.message = `[${type} event]: ${error.message}`;\n                context.error = error;\n                context.requestNewRender();\n            }\n        });\n    }\n\n    context.localOptions = {\n        data: [],\n        columns: [{ type: 'DATA-BLOCK' }],\n        rows: [{ type: 'HEADER' }, { type: 'DATA-BLOCK' }],\n        formatting: [],\n        filtering: [],\n        sorting: [],\n        dataSelector: ({ data, row, column }) => data[row.id][column.id],\n        pinnedTop: 0,\n        pinnedBottom: 0,\n        pinnedLeft: 0,\n        pinnedRight: 0,\n        borderWidth: 1,\n        focusedCell: null,\n        onFocusedCellChange: (focusedCell) => {\n            context.localOptions.focusedCell = focusedCell;\n            context.requestNewRender();\n        },\n        selectedCells: [],\n        onSelectedCellsChange: (selectedCells) => {\n            context.localOptions.selectedCells = selectedCells;\n            context.requestNewRender();\n        },\n        highlightedCells: [],\n        editedCells: [],\n        onEditedCellsChange: (editedCells) => {\n            // TODO: optimize by coalescing\n            context.localOptions.editedCells = editedCells;\n            context.requestNewRender();\n        },\n        filters: [],\n        onFiltersChange: (filters) => {\n            context.localOptions.filters = filters;\n            context.requestNewRender();\n        },\n        sortBy: [],\n        onSortByChange: (sortBy) => {\n            context.localOptions.sortBy = sortBy;\n            context.requestNewRender();\n        },\n        onCellClick: () => { },\n        onCustomCellClick: () => { },\n        columnWidths: [],\n        onColumnWidthsChange: (columnWidths) => {\n            context.localOptions.columnWidths = columnWidths;\n            context.requestNewRender();\n        },\n        rowHeights: [],\n        onRowHeightsChange: (rowHeights) => {\n            context.localOptions.rowHeights = rowHeights;\n            context.requestNewRender();\n        },\n        onActiveColumnsChange: () => { },\n        onActiveRowsChange: () => { },\n    };\n\n    element['spread-grid-context'] = context;\n\n    const setText = (text) => {\n        input.value = text;\n        input.dispatchEvent(new Event('input'));\n    }\n\n    const accept = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const text = context.state.text;\n        const isTextValid = context.state.isTextValid;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const addEditedCells = (cells) => setEditedCells(getCombinedCells(context.state.options.editedCells, cells));\n        const addFilters = (cells) => setFilters(getCombinedCells(context.state.options.filters, cells));\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (text === '')\n            return;\n        if (!isTextValid)\n            return;\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        const dataCells = editableCells.filter(cell => cell.type === 'DATA');\n        const filterCells = editableCells.filter(cell => cell.type === 'FILTER');\n\n        addEditedCells(dataCells.map(cell => ({ ...cell.cell, value: cell.edit.parse({ string: text }) })));\n        addFilters(filterCells.map(cell => ({ ...cell.cell, expression: cell.edit.parse({ string: text }) })));\n\n        if (!autoCommit)\n            setText('');\n    };\n\n    const clear = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const removeEditedCells = (cells) => setEditedCells(getReducedCells(context.state.options.editedCells, cells));\n        const removeFilters = (cells) => setFilters(getReducedCells(context.state.options.filters, cells));\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        removeEditedCells(selectedCells);\n        removeFilters(selectedCells);\n    }\n\n    // TODO: Move other input functions here as well\n\n    context.addEventListener(element, 'scroll', (event) => {\n        // TODO: only request new render if scroll position changed outside of the scope\n        // TODO: how to: calculate the new scrollRect here and compare it to the one in the state\n        // TODO: Also don't forget to check if the highlighted cell did change\n        // TODO: Consider forcing a new render when visible scrollRect changes (without waiting for the next render frame)\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseenter', (event) => {\n        context.mousePosition = getMousePosition(event);\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mousemove', (event) => {\n        context.mousePosition = getMousePosition(event);\n\n        if (context.resizingColumn) {\n            const column = context.state.columnLookup.get(stringifyId(context.resizingColumn));\n            const columnWidth = column.width;\n            const columnRight = column.right;\n            const mousePosition = context.mousePosition.x;\n            const newColumnWidth = Math.max(10, mousePosition - columnRight + columnWidth);\n            const previousColumnWidths = context.state.options.columnWidths;\n            const newColumnWidths = previousColumnWidths\n                .filter(columnWidth => stringifyId(columnWidth.columnId) !== column.key)\n                .concat([{ columnId: column.id, width: newColumnWidth }]);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n        }\n        if (context.resizingRow) {\n            const row = context.state.rowLookup.get(stringifyId(context.resizingRow));\n            const rowHeight = row.height;\n            const rowBottom = row.bottom;\n            const mousePosition = context.mousePosition.y;\n            const newRowHeight = Math.max(10, mousePosition - rowBottom + rowHeight);\n            const previousRowHeights = context.state.options.rowHeights;\n            const newRowHeights = previousRowHeights\n                .filter(rowHeight => stringifyId(rowHeight.rowId) !== row.key)\n                .concat([{ rowId: row.id, height: newRowHeight }]);\n            context.state.options.onRowHeightsChange(newRowHeights);\n        }\n\n        // TODO: only request new render if hovered cell changed\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseleave', () => {\n        context.mousePosition = null;\n        context.requestNewRender();\n    });\n\n    // TODO: update mouse position on resize\n\n    context.addEventListener(element, 'mousedown', (event) => {\n        updateState(context);\n        setText('');\n\n        context.isMouseDown = true;\n        context.mouseDownPosition = context.mousePosition;\n        context.mouseDownCell = context.state.hoveredCell;\n\n        if (context.state.resizableColumn) {\n            context.resizingColumn = context.state.resizableColumn;\n        }\n        if (context.state.resizableRow) {\n            context.resizingRow = context.state.resizableRow;\n        }\n        if (!context.state.resizableColumn && !context.state.resizableRow) {\n            context.state.options.onFocusedCellChange(context.state.hoveredCell);\n        }\n\n        if (!event.ctrlKey)\n            context.state.options.onSelectedCellsChange([]);\n\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseup', (event) => {\n        updateState(context);\n\n        context.isMouseDown = false;\n        context.resizingColumn = null;\n        context.resizingRow = null;\n\n        context.state.options.onSelectedCellsChange(getCombinedCells(context.state.options.selectedCells, context.state.highlightedCells));\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'pointerdown', (event) => {\n        context.element.setPointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'pointerup', (event) => {\n        context.element.releasePointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'click', (event) => {\n        updateState(context);\n\n        const cell = context.state.hoveredCell;\n        const mouseDownCell = context.mouseDownCell;\n\n        if (context.state.resizableColumn || context.state.resizableRow)\n            return;\n        if (cell === null)\n            return;\n        if (stringifyId(cell.columnId) !== stringifyId(mouseDownCell.columnId))\n            return;\n        if (stringifyId(cell.rowId) !== stringifyId(mouseDownCell.rowId))\n            return;\n\n        const column = context.state.columnLookup.get(stringifyId(cell.columnId));\n        const row = context.state.rowLookup.get(stringifyId(cell.rowId));\n        const sortBy = context.state.options.sortBy;\n        const formatResolver = context.state.inputFormatResolver;\n        const cellData = formatResolver.resolve(row, column);\n\n        if (cellData.edit?.toggle) {\n            const edition = context.state.edition;\n            const newValue = getToggledValue(cellData, column, row, edition);\n            const cellType = getCellType(column, row);\n            if (cellType === 'DATA')\n                context.state.options.onEditedCellsChange(getCombinedCells(context.state.options.editedCells, [{ ...cell, value: newValue }]));\n            if (cellType === 'FILTER')\n                context.state.options.onFiltersChange(getCombinedCells(context.state.options.filters, [{ ...cell, expression: newValue }]));\n        } else if (column.type === 'DATA' && row.type === 'DATA') {\n            context.state.options.onCellClick(context.state.hoveredCell);\n        } else if (column.type === 'CUSTOM' || row.type === 'CUSTOM') {\n            context.state.options.onCustomCellClick(context.state.hoveredCell);\n        } else if (column.type === 'HEADER' || row.type === 'HEADER') {\n            const newSortBy = getNewSortBy(sortBy, column, row, event.ctrlKey);\n            context.state.options.onSortByChange(newSortBy);\n            context.state.options.onSelectedCellsChange([]);\n        }\n    });\n\n    context.addEventListener(element, 'dblclick', (event) => {\n        updateState(context);\n\n        if (context.state.resizableColumn) {\n            const resizableColumnKey = stringifyId(context.state.resizableColumn);\n            const newColumnWidths = context.state.options.columnWidths.filter(columnWidth => stringifyId(columnWidth.columnId) !== resizableColumnKey);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n            context.columnWidthCache.delete(resizableColumnKey);\n        }\n        if (context.state.resizableRow) {\n            const resizableRowKey = stringifyId(context.state.resizableRow);\n            const newRowHeights = context.state.options.rowHeights.filter(rowHeight => stringifyId(rowHeight.rowId) !== resizableRowKey);\n            context.state.options.onRowHeightsChange(newRowHeights);\n            context.rowHeightCache.delete(resizableRowKey);\n        }\n\n        const focusedCell = context.state.focusedCell;\n        if (focusedCell === null)\n            return;\n\n        const focusedColumnKey = stringifyId(focusedCell.columnId);\n        const focusedRowKey = stringifyId(focusedCell.rowId);\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const formatResolver = context.state.inputFormatResolver;\n\n        if (!columnLookup.has(focusedColumnKey))\n            return;\n        if (!rowLookup.has(focusedRowKey))\n            return;\n\n        const column = columnLookup.get(focusedColumnKey);\n        const row = rowLookup.get(focusedRowKey);\n        const cell = formatResolver.resolve(row, column);\n        const text = cell.text; // TODO: Make it configurable\n\n        if (!cell.edit)\n            return;\n        if (cell.edit.toggle)\n            return;\n\n        setText(text);\n        input?.select();\n    });\n\n    context.addEventListener(element, 'focus', () => {\n        if (input.parentElement)\n            input.focus({ preventScroll: true });\n    });\n\n    context.addEventListener(element, 'keydown', (event) => {\n        // TODO: make sure it's not invoked on keydown of the input\n        updateState(context);\n\n        const focusedCell = context.state.focusedCell;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const selectedCells = context.state.options.selectedCells;\n        const setSelectedCells = context.state.options.onSelectedCellsChange;\n        const addSelectedCells = (cells) => setSelectedCells(getCombinedCells(selectedCells, cells));\n        const setFocusedCell = context.state.options.onFocusedCellChange;\n        const editedCells = context.state.options.editedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const columns = context.state.columns;\n        const rows = context.state.rows;\n        const text = context.state.text;\n        const inputFormatResolver = context.state.inputFormatResolver;\n\n        const arrowTo = (cell, event) => {\n            setFocusedCell(cell);\n\n            if (event.shiftKey)\n                addSelectedCells([cell]);\n            else\n                setSelectedCells([cell]);\n        };\n\n        const arrowHorizontally = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedColumnKey = stringifyId(focusedCell.columnId);\n            if (!columnLookup.has(focusedColumnKey))\n                return;\n\n            const focusedColumnIndex = columnLookup.get(focusedColumnKey).index;\n            const newColumnIndex = Math.max(0, Math.min(columns.length - 1, focusedColumnIndex + offset));\n            if (newColumnIndex === focusedColumnIndex)\n                return;\n\n            const newFocusedCell = { rowId: focusedCell.rowId, columnId: columns[newColumnIndex].id };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const arrowVertically = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedRowKey = stringifyId(focusedCell.rowId);\n            if (!rowLookup.has(focusedRowKey))\n                return;\n\n            const focusedRowIndex = rowLookup.get(focusedRowKey).index;\n            const newRowIndex = Math.max(0, Math.min(rows.length - 1, focusedRowIndex + offset));\n            if (newRowIndex === focusedRowIndex)\n                return;\n\n            const newFocusedCell = { rowId: rows[newRowIndex].id, columnId: focusedCell.columnId };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const preventDefault = () => {\n            event.preventDefault();\n            event.stopPropagation();\n        };\n\n        const cancel = () => {\n            if (text !== '') {\n                setText('');\n            }\n            else if (selectedCells.length > 1) {\n                setSelectedCells([focusedCell]);\n            }\n            else if (editedCells.length > 0) {\n                setEditedCells([]);\n            }\n            else {\n                setFocusedCell(null);\n                setSelectedCells([]);\n            }\n        };\n\n        const copyToClipboard = (event) => {\n            if (!event.ctrlKey)\n                return;\n\n            const clipboardData = getClipboardData(selectedCells, columns, rows, inputFormatResolver);\n\n            if (navigator.clipboard) {\n                navigator.clipboard.writeText(clipboardData);\n            } else {\n                const textArea = document.createElement('textarea');\n                textArea.value = clipboardData;\n                document.body.appendChild(textArea);\n                textArea.select();\n                document.execCommand('copy');\n                document.body.removeChild(textArea);\n            }\n        }\n\n        switch (event.key) {\n            case 'Escape':\n                cancel();\n                break;\n            case 'Enter':\n                accept();\n                break;\n            case 'ArrowUp':\n                // TODO: When ctrl and shift are pressed together, select all cells between the focused cell and the new cell\n                // TODO: When shift is pressed, expand the current rect selection instead of moving the focused cell\n                preventDefault();\n                arrowVertically(event.ctrlKey ? -rows.length : -1, event);\n                break;\n            case 'ArrowDown':\n                preventDefault();\n                arrowVertically(event.ctrlKey ? rows.length : 1, event);\n                break;\n            case 'ArrowLeft':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? -columns.length : -1, event);\n                break;\n            case 'ArrowRight':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? columns.length : 1, event);\n                break;\n            case 'Delete':\n            case 'Backspace':\n                clear();\n                break;\n            case 'c':\n                copyToClipboard(event);\n                break;\n            default:\n                break;\n        }\n    });\n\n    new ResizeObserver(() => {\n        context.requestNewRender();\n    }).observe(element);\n\n    context.addEventListener(input, 'input', (event) => {\n        // TODO: check performance of this (if it's ok to update the state on every input event)\n        updateState(context);\n\n        if (event.target.value) {\n            accept(true);\n\n            input.style.opacity = 1;\n            input.style.pointerEvents = 'auto';\n        }\n        else {\n            if (event.isTrusted)\n                clear(true);\n\n            input.style.opacity = 0;\n            input.style.pointerEvents = 'none';\n        }\n    });\n\n    context.addEventListener(input, 'click', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'dblclick', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'mousedown', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'keydown', (event) => {\n        switch (event.key) {\n            case 'Enter':\n            case 'Escape':\n                break;\n            case 'Delete':\n            case 'Backspace':\n            case 'ArrowUp':\n            case 'ArrowDown':\n            case 'ArrowLeft':\n            case 'ArrowRight':\n                if (input.value !== '') {\n                    event.stopPropagation();\n                    context.requestNewRender();\n                }\n                break;\n            default:\n                event.stopPropagation();\n                // TODO: maybe only check if the new text is valid\n                context.requestNewRender();\n                break;\n        }\n    });\n}\n\nexport default function createGrid(element, options) {\n    console.log('createGrid');\n\n    initialize(element);\n\n    const context = element['spread-grid-context'];\n    context.externalOptions = options;\n\n    if (context.state === null) {\n        updateState(context);\n        // TODO: only render if the state has sufficiently changed\n        render(context);\n    }\n    else {\n        context.requestNewRender();\n    }\n}",
+        "export default function getToggledValue(cell, column, row, edition) {\n    const value = edition.hasValueByKey(row.key, column.key)\n        ? edition.getValueByKey(row.key, column.key)\n        : cell.value;\n    const toggle = cell.edit.toggle;\n\n    if (typeof toggle === 'function')\n        return toggle({value}); // TODO: expand by context\n\n    return toggle[(toggle.indexOf(value) + 1) % toggle.length];\n}",
         "import stringifyId from '../core-utils/stringifyId.js';\n\nexport default function getNewSortBy(sortBy, column, row, ctrlKey) {\n    // TODO: better support for multi-row sorting\n\n    function isCurrentRule(rule) {\n        return column.key === stringifyId(rule.columnId || 'HEADER') && row.key === stringifyId(rule.rowId || 'HEADER');\n    }\n\n    const directionLoop = ['ASC', 'DESC', undefined];\n    const currentRule = sortBy.find(isCurrentRule);\n    const directionIndex = directionLoop.indexOf(currentRule?.direction);\n    const newDirection = directionLoop[(directionIndex + 1) % directionLoop.length];\n    const isLastRule = sortBy.indexOf(currentRule) === sortBy.length - 1;\n    const shouldKeepOld = ctrlKey && (isLastRule || !currentRule);\n    const rulesToKeep = shouldKeepOld ? sortBy.filter(rule => !isCurrentRule(rule)) : [];\n    const newRules = newDirection ? [{ columnId: column.id, rowId: row.id, direction: newDirection }] : [];\n\n    return [...rulesToKeep, ...newRules];\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport Selection from \"../types/Selection.js\";\n\nexport default function getClipboardData(selectedCells, columns, rows, formatResolver) {\n    const columnLookup = new Map(columns.map(column => [column.key, column]));\n    const rowLookup = new Map(rows.map(row => [row.key, row]));\n    const selectedCellKeys = selectedCells.map(cell => ({\n        columnKey: stringifyId(cell.columnId),\n        rowKey: stringifyId(cell.rowId)\n    })).filter(cell => columnLookup.has(cell.columnKey) && rowLookup.has(cell.rowKey));\n    const selectedColumns = new Set(selectedCellKeys.map(cell => cell.columnKey));\n    const selectedRows = new Set(selectedCellKeys.map(cell => cell.rowKey));\n\n    if (selectedCellKeys.length === 0)\n        return '';\n\n    const selection = new Selection(selectedCells);\n    const minColumnIndex = Math.min(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const maxColumnIndex = Math.max(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const minRowIndex = Math.min(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n    const maxRowIndex = Math.max(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n\n    const stringBuilder = [];\n\n    for (let rowIndex = minRowIndex; rowIndex <= maxRowIndex; rowIndex++) {\n        const row = rows[rowIndex];\n        const rowKey = row.key;\n\n        if (!selectedRows.has(rowKey))\n            continue;\n\n        for (let columnIndex = minColumnIndex; columnIndex <= maxColumnIndex; columnIndex++) {\n            const column = columns[columnIndex];\n            const columnKey = column.key;\n\n            if (!selectedColumns.has(columnKey))\n                continue;\n\n            if (selection.isKeySelected(rowKey, columnKey)) {\n                const cellData = formatResolver.resolve(row, column).text;\n                stringBuilder.push(cellData);\n            }\n\n            if (columnIndex < maxColumnIndex)\n                stringBuilder.push('\\t');\n        }\n\n        if (rowIndex < maxRowIndex)\n            stringBuilder.push('\\n');\n    }\n\n    return stringBuilder.join('');\n}",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_8m1712512160\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_9m1712685293\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
     ],
     "version": 3
 }
```

### Comparing `dash_spread_grid-0.0.8/dash_spread_grid/metadata.json` & `dash_spread_grid-0.0.9/dash_spread_grid/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.0.8/dash_spread_grid/package-info.json` & `dash_spread_grid-0.0.9/dash_spread_grid/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.0.9'"}*

```diff
@@ -53,15 +53,15 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.0.8",
+    "version": "0.0.9",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

### Comparing `dash_spread_grid-0.0.8/package.json` & `dash_spread_grid-0.0.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.0.9'"}*

```diff
@@ -53,15 +53,15 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.0.8",
+    "version": "0.0.9",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

