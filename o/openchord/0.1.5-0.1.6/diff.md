# Comparing `tmp/openchord-0.1.5.tar.gz` & `tmp/openchord-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openchord-0.1.5.tar", last modified: Sun Apr 23 21:40:45 2023, max compression
+gzip compressed data, was "openchord-0.1.6.tar", last modified: Mon Apr 24 10:50:38 2023, max compression
```

## Comparing `openchord-0.1.5.tar` & `openchord-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 21:40:45.436657 openchord-0.1.5/
--rw-rw-rw-   0        0        0    35823 2023-04-20 10:08:25.000000 openchord-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2313 2023-04-23 21:40:45.434689 openchord-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1782 2023-04-23 21:37:55.000000 openchord-0.1.5/README.md
--rw-rw-rw-   0        0        0      786 2023-04-23 09:31:26.000000 openchord-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 21:40:45.436657 openchord-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 21:40:45.402621 openchord-0.1.5/src/
--rw-rw-rw-   0        0        0        0 2023-04-23 09:15:38.000000 openchord-0.1.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:40:45.432557 openchord-0.1.5/src/openchord.egg-info/
--rw-rw-rw-   0        0        0     2313 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-23 21:40:45.000000 openchord-0.1.5/src/openchord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7362 2023-04-23 21:16:00.000000 openchord-0.1.5/src/openchord.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:50:38.795442 openchord-0.1.6/
+-rw-rw-rw-   0        0        0    35823 2023-04-20 10:08:25.000000 openchord-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2827 2023-04-24 10:50:38.794443 openchord-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2296 2023-04-24 10:39:17.000000 openchord-0.1.6/README.md
+-rw-rw-rw-   0        0        0      786 2023-04-23 09:31:26.000000 openchord-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 10:50:38.795442 openchord-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 10:50:38.766886 openchord-0.1.6/src/
+-rw-rw-rw-   0        0        0        0 2023-04-23 09:15:38.000000 openchord-0.1.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:50:38.792301 openchord-0.1.6/src/openchord.egg-info/
+-rw-rw-rw-   0        0        0     2827 2023-04-24 10:50:38.000000 openchord-0.1.6/src/openchord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-24 10:50:38.000000 openchord-0.1.6/src/openchord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 10:50:38.000000 openchord-0.1.6/src/openchord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-24 10:50:38.000000 openchord-0.1.6/src/openchord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-24 10:50:38.000000 openchord-0.1.6/src/openchord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10211 2023-04-24 09:33:39.000000 openchord-0.1.6/src/openchord.py
```

### Comparing `openchord-0.1.5/LICENSE` & `openchord-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openchord-0.1.5/PKG-INFO` & `openchord-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OpenChord
 
+<img src="https://raw.githubusercontent.com/pke1029/open-chord/main/media/logo.svg" width="360" height="100">
+
 OpenChord is a Python library I am developing to plot beautiful chord diagrams for visualising networks and graphs. OpenChord uses the `drawsvg` library and can display figures in a Jupyter notebook or Jupyter lab. Other libraries for drawing chord diagram includes [PlotAPI](https://plotapi.com/) (paid), [Bokeh](https://holoviews.org/reference/elements/bokeh/Chord.html) (visible moire artifact), and [Plotly](https://plotly.com/python/v3/filled-chord-diagram/) (tedious). 
 
 ## Installation
 
 OpenChord is now on PyPI.org! Install using the command
 ```
 pip install openchord
@@ -48,8 +50,29 @@
 ```python
 fig.save_svg("figure.svg")
 ```
 ![Chord diagram using OpenChord](https://raw.githubusercontent.com/pke1029/open-chord/main/media/figure.png)
 
 ## More tutorials and examples
 I wrote a few more tutorials available via the link below and in the `/example` directory
+
+
+
+
 1. [Quick Start](https://github.com/pke1029/open-chord/blob/main/examples/01_quick_start.ipynb)
+   * First chord diagram
+   * Radius
+   * Padding
+   * Font size and font family
+   * Colormap
+   * Gap size
+   * Background color and 
+
+2. [The Logo](https://github.com/pke1029/open-chord/blob/main/examples/02_the_logo.ipynb)
+   * Rotation
+   * Custom plot area
+   * Gradient style
+   * Arc thickness
+   * Text position
+   * Ribbon gap
+   * Ribbon stiffness
+   * Save as SVG
```

### Comparing `openchord-0.1.5/README.md` & `openchord-0.1.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # OpenChord
 
+<img src="https://raw.githubusercontent.com/pke1029/open-chord/main/media/logo.svg" width="360" height="100">
+
 OpenChord is a Python library I am developing to plot beautiful chord diagrams for visualising networks and graphs. OpenChord uses the `drawsvg` library and can display figures in a Jupyter notebook or Jupyter lab. Other libraries for drawing chord diagram includes [PlotAPI](https://plotapi.com/) (paid), [Bokeh](https://holoviews.org/reference/elements/bokeh/Chord.html) (visible moire artifact), and [Plotly](https://plotly.com/python/v3/filled-chord-diagram/) (tedious). 
 
 ## Installation
 
 OpenChord is now on PyPI.org! Install using the command
 ```
 pip install openchord
@@ -34,8 +36,29 @@
 ```python
 fig.save_svg("figure.svg")
 ```
 ![Chord diagram using OpenChord](https://raw.githubusercontent.com/pke1029/open-chord/main/media/figure.png)
 
 ## More tutorials and examples
 I wrote a few more tutorials available via the link below and in the `/example` directory
+
+
+
+
 1. [Quick Start](https://github.com/pke1029/open-chord/blob/main/examples/01_quick_start.ipynb)
+   * First chord diagram
+   * Radius
+   * Padding
+   * Font size and font family
+   * Colormap
+   * Gap size
+   * Background color and 
+
+2. [The Logo](https://github.com/pke1029/open-chord/blob/main/examples/02_the_logo.ipynb)
+   * Rotation
+   * Custom plot area
+   * Gradient style
+   * Arc thickness
+   * Text position
+   * Ribbon gap
+   * Ribbon stiffness
+   * Save as SVG
```

### Comparing `openchord-0.1.5/pyproject.toml` & `openchord-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openchord-0.1.5/src/openchord.egg-info/PKG-INFO` & `openchord-0.1.6/src/openchord.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OpenChord
 
+<img src="https://raw.githubusercontent.com/pke1029/open-chord/main/media/logo.svg" width="360" height="100">
+
 OpenChord is a Python library I am developing to plot beautiful chord diagrams for visualising networks and graphs. OpenChord uses the `drawsvg` library and can display figures in a Jupyter notebook or Jupyter lab. Other libraries for drawing chord diagram includes [PlotAPI](https://plotapi.com/) (paid), [Bokeh](https://holoviews.org/reference/elements/bokeh/Chord.html) (visible moire artifact), and [Plotly](https://plotly.com/python/v3/filled-chord-diagram/) (tedious). 
 
 ## Installation
 
 OpenChord is now on PyPI.org! Install using the command
 ```
 pip install openchord
@@ -48,8 +50,29 @@
 ```python
 fig.save_svg("figure.svg")
 ```
 ![Chord diagram using OpenChord](https://raw.githubusercontent.com/pke1029/open-chord/main/media/figure.png)
 
 ## More tutorials and examples
 I wrote a few more tutorials available via the link below and in the `/example` directory
+
+
+
+
 1. [Quick Start](https://github.com/pke1029/open-chord/blob/main/examples/01_quick_start.ipynb)
+   * First chord diagram
+   * Radius
+   * Padding
+   * Font size and font family
+   * Colormap
+   * Gap size
+   * Background color and 
+
+2. [The Logo](https://github.com/pke1029/open-chord/blob/main/examples/02_the_logo.ipynb)
+   * Rotation
+   * Custom plot area
+   * Gradient style
+   * Arc thickness
+   * Text position
+   * Ribbon gap
+   * Ribbon stiffness
+   * Save as SVG
```

### Comparing `openchord-0.1.5/src/openchord.py` & `openchord-0.1.6/src/openchord.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import drawsvg as dw
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 def pol2cart(rho, phi):
     x = rho * np.cos(phi)
     y = rho * np.sin(phi)
     return x, -y
 
 def get_arc(radius, start_angle, end_angle):
@@ -15,33 +15,38 @@
     return x1, y1, x2, y2
 
 def arc(radius, start_angle, end_angle, color="black", opacity=0.9, thickness=0.07):
     # coordinates
     k = 1.0 + thickness
     x1, y1, x2, y2 = get_arc(radius, start_angle, end_angle)
     x3, y3, x4, y4 = k*x2, k*y2, k*x1, k*y1
+    # arc direction
+    large_arc = 1 if end_angle-start_angle > np.pi else 0
     # create path 
     p = dw.Path(fill=color, fill_opacity=opacity)
     p.M(x1, y1)
-    p.A(radius, radius, rot=0, large_arc=0, sweep=0, ex=x2, ey=y2)
+    p.A(radius, radius, rot=0, large_arc=large_arc, sweep=0, ex=x2, ey=y2)
     p.L(x3, y3)
-    p.A(k*radius, k*radius, rot=0, large_arc=0, sweep=1, ex=x4, ey=y4).Z()
+    p.A(k*radius, k*radius, rot=0, large_arc=large_arc, sweep=1, ex=x4, ey=y4).Z()
     return p
 
 def ribbon(radius, source_a1, source_a2, target_a1, target_a2, color="black", opacity=0.6, control_strength=0.6):
     x1, y1, x2, y2 = get_arc(radius, source_a1, source_a2)
     x3, y3, x4, y4 = get_arc(radius, target_a1, target_a2)
     k = 1.0 - control_strength
     xctr1, yctr1, xctr2, yctr2, xctr3, yctr3, xctr4, yctr4 = k*x1, k*y1, k*x2, k*y2, k*x3, k*y3, k*x4, k*y4
+    # arc direction
+    source_large_arc = 1 if source_a2 - source_a1 > np.pi else 0
+    target_large_arc = 1 if target_a2 - target_a1 > np.pi else 0
     # define path
     p = dw.Path(fill=color, fill_opacity=opacity)
     p.M(x1, y1)
-    p.A(radius, radius, rot=0, large_arc=0, sweep=0, ex=x2, ey=y2)
+    p.A(radius, radius, rot=0, large_arc=source_large_arc, sweep=0, ex=x2, ey=y2)
     p.C(xctr2, yctr2, xctr3, yctr3, x3, y3)
-    p.A(radius, radius, rot=0, large_arc=0, sweep=0, ex=x4, ey=y4)
+    p.A(radius, radius, rot=0, large_arc=target_large_arc, sweep=0, ex=x4, ey=y4)
     p.C(xctr4, yctr4, xctr1, yctr1, x1, y1)
     p.Z()
     return p
 
 def is_symmetric(A):
         A = np.array(A)
         m, n = A.shape
@@ -51,31 +56,38 @@
 
 class Chord:
 
     colormap_default = ["#FFB6C1", "#FFD700", "#FFA07A", "#90EE90", "#87CEFA", "#DA70D6", "#FF69B4", "#20B2AA"]
     colormap_vibrant = ["#FF6B6B", "#F9844A", "#F9C74F", "#90BE6D", "#43AA8B", "#4D908E", "#577590", "#277DA1"]
     
     def __init__(self, data, labels=[], radius=200, gap_size=0.01):
-        self.data = np.array(data)
+        self.matrix = np.array(data)
         self.labels = labels
-        self.radius = radius
-        self.padding = 50
+        self._radius = radius
+        self._padding = 50
+        self.plot_area = self.get_plot_area()
         self.font_size = 10
         self.font_family = "Arial"
         self._gap_size = gap_size
+        self.ribbon_gap = 0.01
+        self.ribbon_stiffness = 0.6
+        self._rotation = 0
+        self.arc_thickness = 0.07
+        self.text_position = 0.1
         self.bg_color = "#ffffff"
         self.bg_transparancy = 1.0
-        self.shape = self.data.shape[0]
-        self.row_sum = np.sum(self.data, axis=0)
-        self.total = np.sum(self.data)
+        self.shape = self.matrix.shape[0]
+        self.row_sum = np.sum(self.matrix, axis=1)
+        self.total = np.sum(self.matrix)
         self.conversion_rate = (2*np.pi-self.gap_size*self.shape)/self.total
-        self.is_symmetric = is_symmetric(self.data)
+        self.is_symmetric = is_symmetric(self.matrix)
         self.ideogram_ends = self.get_ideogram_ends()
         self.ribbon_ends = self.get_ribbon_ends()
         self._colormap = self.colormap_default
+        self._gradient_style = "default"
         self.gradients = self.get_gradients()
 
     @property
     def colormap(self):
         return self._colormap
 
     @colormap.setter
@@ -89,54 +101,109 @@
 
     @gap_size.setter
     def gap_size(self, value):
         self._gap_size = value
         self.conversion_rate = (2*np.pi-self.gap_size*self.shape)/self.total
         self.ideogram_ends = self.get_ideogram_ends()
         self.ribbon_ends = self.get_ribbon_ends()
+        self.gradients = self.get_gradients()
+
+    @property
+    def rotation(self):
+        return self._rotation
+
+    @rotation.setter
+    def rotation(self, value):
+        self._rotation = value
+        self.ideogram_ends = self.get_ideogram_ends()
+        self.ribbon_ends = self.get_ribbon_ends()
+        self.gradients = self.get_gradients()
+
+    @property
+    def gradient_style(self):
+        return self._gradient_style
+
+    @gradient_style.setter
+    def gradient_style(self, value):
+        self._gradient_style = value
+        self.gradients = self.get_gradients()
+
+    @property
+    def radius(self):
+        return self._radius
+    
+    @radius.setter
+    def radius(self, value):
+        self._radius = value
+        self.plot_area = self.get_plot_area()
+
+    @property
+    def padding(self):
+        return self._padding
+
+    @padding.setter
+    def padding(self, value):
+        self._padding = value
+        self.plot_area = self.get_plot_area()
+    
+    def get_plot_area(self):
+        x = -self.radius-self.padding
+        y = x
+        w = 2.0*(self.radius+self.padding)
+        h = w
+        return {"x":x, "y":y, "w":w, "h":h}
         
     def show(self):
-        fig_size = 2*(self.radius + self.padding)
-        fig = dw.Drawing(fig_size, fig_size, origin='center')
+        fig = dw.Drawing(self.plot_area["w"], self.plot_area["h"], origin=(self.plot_area["x"], self.plot_area["y"]))
         # background
-        fig.append(dw.Rectangle(-0.5*fig_size, -0.5*fig_size, fig_size, fig_size, fill=self.bg_color, fill_opacity=self.bg_transparancy))
+        fig.append(dw.Rectangle(self.plot_area["x"], self.plot_area["y"], self.plot_area["w"], self.plot_area["h"], fill=self.bg_color, fill_opacity=self.bg_transparancy))
         # make ideogram
         for i,v in enumerate(self.ideogram_ends):
-            fig.append(arc(self.radius, v[0], v[1], color=self.get_color(i)))
+            fig.append(arc(self.radius, v[0], v[1], color=self.get_color(i), thickness=self.arc_thickness))
         # make ribbon
         for i,v in enumerate(self.ribbon_ends):
-            fig.append(ribbon(self.radius*0.99, v[0], v[1], v[2], v[3], color=self.gradients[i]))
+            fig.append(ribbon(self.radius*(1.0-self.ribbon_gap), v[0], v[1], v[2], v[3], color=self.gradients[i], control_strength=self.ribbon_stiffness))
         # draw labels
         for i,v in enumerate(self.labels):
             midpoint = np.mean(self.ideogram_ends[i,:])
             x, y = pol2cart(self.radius, midpoint)
-            r = np.sqrt(x*x+y*y) * 1.1
+            r = np.sqrt(x*x+y*y) * (1.0+self.text_position)
             angle = midpoint * 180.0/np.pi
             if midpoint > 0.5*np.pi and midpoint < 1.5*np.pi:
                 r *= -1
                 angle = -(180.0-angle)
                 anchor = "end"
             else:
                 anchor = "start"
             fig.append(dw.Text(v, font_size=self.font_size, x=r, y=0, text_anchor=anchor, dominant_baseline='middle', transform=f"rotate(%f)"%(-angle), font_family=self.font_family))
         return fig
     
     def get_ideogram_ends(self):
         arc_lens = self.row_sum * self.conversion_rate
         ideogram_ends = []
-        left = 0 
+        left = self.rotation
         for arc_len in arc_lens:
             right = left + arc_len
             ideogram_ends.append([left, right])
             left = right + self.gap_size
         return np.array(ideogram_ends)
+
+    def get_pairs(self):
+        n = self.shape
+        upper = []
+        for i in range(n):
+            for j in range(i+1, n):
+                if self.matrix[i,j] != 0:
+                    upper.append([i,j])
+        pairs = {"upper": upper}
+        return pairs
     
     def get_ribbon_ends(self):
         n = self.shape
-        arc_lens = self.data * self.conversion_rate
+        arc_lens = self.matrix * self.conversion_rate
         regions = np.zeros((n, n+1))
         for i in range(n):
             regions[i,0] = self.ideogram_ends[i,0]
             regions[i,1:n+1] = self.ideogram_ends[i,0] + np.cumsum(np.roll(arc_lens[i,::-1], i+1))
         ribbon_ends = []
         for i in range(n):
             ribbon_ends.append([regions[i,0], regions[i,1], regions[i,0], regions[i,1]]) # diagonal terms
@@ -151,32 +218,45 @@
         gradients = []
         idx = 0
         # diagonal terms
         n = self.shape
         for i in range(n):
             gradients.append(self.get_color(i))
             idx += 1
-        for i in range(n):
-            for j in range(i+1, n):
-                a0, a1, a2, a3 = self.ribbon_ends[idx]
-                if i == 0 and j == n-1:
-                    x0, y0 = pol2cart(self.radius, a1)
-                    x1, y1 = pol2cart(self.radius, a2)
-                elif np.abs(a3-a0) > np.abs(a2-a1):
-                    x0, y0 = pol2cart(self.radius, a0)
-                    x1, y1 = pol2cart(self.radius, a3)
-                else:
-                    x0, y0 = pol2cart(self.radius, a1)
-                    x1, y1 = pol2cart(self.radius, a2)
-                # create gradient
-                g = dw.LinearGradient(x0, y0, x1, y1)
-                g.add_stop(0, self.get_color(i))
-                g.add_stop(1, self.get_color(j))
-                gradients.append(g)
-                idx += 1
+        if self.gradient_style == "midpoint":
+            for i in range(n):
+                for j in range(i+1, n):
+                    a0, a1, a2, a3 = self.ribbon_ends[idx]
+                    x0, y0 = pol2cart(self.radius, 0.5*(a0+a1))
+                    x1, y1 = pol2cart(self.radius, 0.5*(a2+a3))
+                    g = dw.LinearGradient(x0, y0, x1, y1)
+                    g.add_stop(0, self.get_color(i))
+                    g.add_stop(1, self.get_color(j))
+                    gradients.append(g)
+                    idx += 1
+        else:
+            # default gradient 
+            for i in range(n):
+                for j in range(i+1, n):
+                    a0, a1, a2, a3 = self.ribbon_ends[idx]
+                    if i == 0 and j == n-1:
+                        x0, y0 = pol2cart(self.radius, a1)
+                        x1, y1 = pol2cart(self.radius, a2)
+                    elif np.abs(a3-a0) > np.abs(a2-a1):
+                        x0, y0 = pol2cart(self.radius, a0)
+                        x1, y1 = pol2cart(self.radius, a3)
+                    else:
+                        x0, y0 = pol2cart(self.radius, a1)
+                        x1, y1 = pol2cart(self.radius, a2)
+                    # create gradient
+                    g = dw.LinearGradient(x0, y0, x1, y1)
+                    g.add_stop(0, self.get_color(i))
+                    g.add_stop(1, self.get_color(j))
+                    gradients.append(g)
+                    idx += 1
         return gradients
     
     def save_svg(self, filename):
         fig = self.show()
         fig.save_svg(filename)
 
     def save_png(self, filename):
```

