# Comparing `tmp/frascii-2.4.tar.gz` & `tmp/frascii-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-2.4.tar", last modified: Wed Apr 12 12:35:18 2023, max compression
+gzip compressed data, was "frascii-2.5.tar", last modified: Mon Apr 24 15:52:07 2023, max compression
```

## Comparing `frascii-2.4.tar` & `frascii-2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-12 12:35:18.960043 frascii-2.4/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-12 12:35:18.960043 frascii-2.4/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12240 2023-04-07 11:54:45.000000 frascii-2.4/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-12 12:35:18.956043 frascii-2.4/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1533 2023-04-12 12:35:12.000000 frascii-2.4/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     6323 2023-03-07 12:42:34.000000 frascii-2.4/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-12 12:35:18.960043 frascii-2.4/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.4/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.4/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.4/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.4/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.4/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      744 2023-02-28 13:56:01.000000 frascii-2.4/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.4/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-2.4/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      609 2023-02-24 15:05:19.000000 frascii-2.4/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.4/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.4/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.4/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.4/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-12 12:35:18.956043 frascii-2.4/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-12 12:35:18.000000 frascii-2.4/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-12 12:35:18.960043 frascii-2.4/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.4/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 15:52:07.484273 frascii-2.5/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-24 15:52:07.484273 frascii-2.5/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12240 2023-04-07 11:54:45.000000 frascii-2.5/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 15:52:07.484273 frascii-2.5/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1585 2023-04-24 15:51:32.000000 frascii-2.5/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7022 2023-04-24 15:51:06.000000 frascii-2.5/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 15:52:07.484273 frascii-2.5/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.5/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.5/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.5/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.5/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.5/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1602 2023-04-20 13:09:29.000000 frascii-2.5/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.5/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-2.5/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2381 2023-04-20 12:54:46.000000 frascii-2.5/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.5/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.5/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.5/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.5/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 15:52:07.484273 frascii-2.5/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-24 15:52:07.488273 frascii-2.5/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.5/setup.py
```

### Comparing `frascii-2.4/README.md` & `frascii-2.5/README.md`

 * *Files identical despite different names*

### Comparing `frascii-2.4/frascii/__init__.py` & `frascii-2.5/frascii/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string
 
-__version__ = '2.4'
+__version__ = '2.5'
 
-def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter):
-	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter)
+def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid):
+	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
-def julia(f, x, y, x_radius, y_radius, stepsize, max_iter):
-	return julia_string(f, x, y, x_radius, y_radius, stepsize, max_iter)
+def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid):
+	return julia_string(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
 def sierpinski_carpet(n):
 	return sierpinski_carpet_string(n)
 
 def cantor(n):
 	return cantor_string(n)
```

### Comparing `frascii-2.4/frascii/commands.py` & `frascii-2.5/frascii/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,29 +51,38 @@
 	fibonacci_parser.add_argument("-n", type=int, help="iterations", choices=range(0, 14), nargs="?", default=3)
 	fibonacci_parser.set_defaults(func=frascii.fibonacci)
 
 	# Mandelbrot sub-command
 	mandelbrot_parser = subparsers.add_parser("mandelbrot", description="Wikipedia: https://en.wikipedia.org/wiki/Mandelbrot_set", formatter_class=fc)
 	mandelbrot_parser.add_argument("-x", type=float, help="real part of the images center", nargs="?", default=-0.8)
 	mandelbrot_parser.add_argument("-y", type=float, help="imaginary part of the images center", nargs="?", default=0)
-	mandelbrot_parser.add_argument("-x_radius", type=int, help="pixels added on left and right of center", nargs="?", default=27)
-	mandelbrot_parser.add_argument("-y_radius", type=int, help="pixels added on top and bottom of center", nargs="?", default=12)
+	mandelbrot_parser.add_argument("-x_radius", type=int, help="pixels added on left and right of center", nargs="?", default=25)
+	mandelbrot_parser.add_argument("-y_radius", type=int, help="pixels added on top and bottom of center", nargs="?", default=14)
 	mandelbrot_parser.add_argument("-stepsize", type=float, help="size of a pixel", nargs="?", default=0.05)
 	mandelbrot_parser.add_argument("-max_iter", type=int, help="iterations after which z is assumed to be in the set", nargs="?", default=20)
+	mandelbrot_parser.add_argument("-style", type=str, help="style of the visualization",
+								   choices=["repeating", "non-repeating"], nargs="?", default="non-repeating")
+	mandelbrot_parser.add_argument("-grid", type=str, help="square (double-chars) or rectangle (single-char) grid.",
+								   choices=["square", "rect"], nargs="?", default="rect")
 	mandelbrot_parser.set_defaults(func=frascii.mandelbrot)
 
 	# Julia sub-command
 	julia_parser = subparsers.add_parser("julia", description="Wikipedia: https://en.wikipedia.org/wiki/Julia_set", formatter_class=fc)
 	julia_parser.add_argument("-f", type=str, help="complex function", nargs="?", default="z**2 - 0.4 + 0.6j")
 	julia_parser.add_argument("-x", type=float, help="real part of the images center", nargs="?", default=0)
 	julia_parser.add_argument("-y", type=float, help="imaginary part of the images center", nargs="?", default=0)
 	julia_parser.add_argument("-x_radius", type=int, help="pixels added on left and right of center", nargs="?", default=45)
 	julia_parser.add_argument("-y_radius", type=int, help="pixels added on top and bottom of center", nargs="?", default=18)
 	julia_parser.add_argument("-stepsize", type=float, help="size of a pixel", nargs="?", default=0.033)
 	julia_parser.add_argument("-max_iter", type=int, help="iterations after which z is assumed to be in the set", nargs="?", default=40)
+	julia_parser.add_argument("-style", type=str, help="style of the visualization",
+								   choices=["repeating", "non-repeating"], nargs="?", default="non-repeating")
+	julia_parser.add_argument("-grid", type=str, help="square (double-chars) or rectangle (single-char) grid.",
+								   choices=["square", "rect"], nargs="?", default="rect")
+
 	julia_parser.set_defaults(func=frascii.julia)
 
 	# L-system sub-command
 	l_system_parser = subparsers.add_parser("l_system", description="Wikipedia: https://en.wikipedia.org/wiki/L-system", formatter_class=fc)
 	l_system_parser.add_argument("-start", type=str, help="real part of the images center", nargs="?", default="F")
 	l_system_parser.add_argument("-rules", type=str, help="imaginary part of the images center", nargs="?", default="(F->F+F-F-F+F)")
 	l_system_parser.add_argument("-n", type=int, help="pixels added on left and right of center", nargs="?", default=3)
```

### Comparing `frascii-2.4/frascii/fractals/dragon_curve.py` & `frascii-2.5/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.4/frascii/fractals/fibonacci.py` & `frascii-2.5/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-2.4/frascii/fractals/hilbert_curve.py` & `frascii-2.5/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.4/frascii/fractals/koch.py` & `frascii-2.5/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-2.4/frascii/fractals/l_system.py` & `frascii-2.5/frascii/fractals/l_system.py`

 * *Files identical despite different names*

### Comparing `frascii-2.4/frascii/fractals/peano_curve.py` & `frascii-2.5/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.4/frascii/fractals/sierpinski_carpet.py` & `frascii-2.5/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-2.4/frascii.egg-info/SOURCES.txt` & `frascii-2.5/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

