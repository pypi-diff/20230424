# Comparing `tmp/frascii-2.5.tar.gz` & `tmp/frascii-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-2.5.tar", last modified: Mon Apr 24 15:52:07 2023, max compression
+gzip compressed data, was "frascii-2.6.tar", last modified: Mon Apr 24 20:43:12 2023, max compression
```

## Comparing `frascii-2.5.tar` & `frascii-2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 15:52:07.484273 frascii-2.5/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-24 15:52:07.484273 frascii-2.5/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12240 2023-04-07 11:54:45.000000 frascii-2.5/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 15:52:07.484273 frascii-2.5/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1585 2023-04-24 15:51:32.000000 frascii-2.5/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7022 2023-04-24 15:51:06.000000 frascii-2.5/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 15:52:07.484273 frascii-2.5/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.5/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.5/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.5/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.5/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.5/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1602 2023-04-20 13:09:29.000000 frascii-2.5/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.5/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-2.5/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2381 2023-04-20 12:54:46.000000 frascii-2.5/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.5/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.5/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.5/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.5/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 15:52:07.484273 frascii-2.5/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-24 15:52:07.000000 frascii-2.5/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-24 15:52:07.488273 frascii-2.5/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.5/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 20:43:12.907507 frascii-2.6/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-24 20:43:12.907507 frascii-2.6/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12666 2023-04-24 20:42:46.000000 frascii-2.6/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 20:43:12.903508 frascii-2.6/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1942 2023-04-24 20:43:05.000000 frascii-2.6/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7766 2023-04-24 20:38:11.000000 frascii-2.6/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 20:43:12.907507 frascii-2.6/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.6/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.6/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.6/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.6/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.6/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3135 2023-04-24 20:36:12.000000 frascii-2.6/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.6/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-2.6/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2996 2023-04-24 20:34:17.000000 frascii-2.6/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.6/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.6/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.6/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.6/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-24 20:43:12.907507 frascii-2.6/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-24 20:43:12.000000 frascii-2.6/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-24 20:43:12.907507 frascii-2.6/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.6/setup.py
```

### Comparing `frascii-2.5/README.md` & `frascii-2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,30 +19,34 @@
 
 `frascii peano_curve <n>`: Displays the n-th iteration of the [Peano Curve](https://en.wikipedia.org/wiki/Peano_curve).
 
 `frascii dragon_curve <n>`: Displays the n-th iteration of the [Dragon Curve](https://en.wikipedia.org/wiki/Dragon_curve).
 
 `frascii fibonacci <n>`: Displays the [Fibonacci Sequence](https://en.wikipedia.org/wiki/Fibonacci_sequence) up to n as squares.
 
-`frascii mandelbrot <x, y, x_radius, y_radius, stepsize, max_iter>`: Displays a specified part of the [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set).
+`frascii mandelbrot <x, y, x_radius, y_radius, stepsize, max_iter, grid, style>`: Displays a specified part of the [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set).
 
-`frascii julia <f, x, y, x_radius, y_radius, stepsize, max_iter>`: Displays a specified part of the [Julia Set](https://en.wikipedia.org/wiki/Julia_set) for a given f(z).
+`frascii julia <f, x, y, x_radius, y_radius, stepsize, max_iter, grid, style>`: Displays a specified part of the [Julia Set](https://en.wikipedia.org/wiki/Julia_set) for a given f(z).
 
 `frascii l_system <start, rules, n>`: Displays a curve generated by a [L-System](https://en.wikipedia.org/wiki/L-system). Angles will be fixed to 90°.
 
 
 more to come ...
 
 # Examples
 
 ## Mandelbrot set
-`frascii mandelbrot -x_radius 400 -y_radius 180 -stepsize 0.0033`
+`frascii mandelbrot -x_radius 400 -y_radius 180 -stepsize 0.0033 -style non-repeating`
 
 ![Mandelbrot set in terminal by frascii](readme_images/mandelbrot.png)
 
+`frascii mandelbrot -x_radius 400 -y_radius 180 -stepsize 0.0033 -style repeating`
+
+![Mandelbrot set in terminal by frascii](readme_images/repeating.png)
+
 `frascii mandelbrot -x -1.15 -y 0.26 -x_radius 200 -y_radius 70 -stepsize 3.7e-4 -max_iter 60`
 
 ![Mandelbrot set in terminal by frascii](readme_images/mandelbrot2.png)
 
 `frascii mandelbrot`
 
 ```
@@ -140,20 +144,26 @@
 
 ```
 
 ## L-systems
 
 ### Rules
 
-**F** will draw a forward line.
+**F** will step forward and draw a line.
+
+**f** will step forward and not draw a line.
 
 **+** will turn right.
 
 **-** will turn left.
 
+**\[** will put current position and orientation on the stack.
+
+**\]** will set current position and orientation based on topmost entry on stack which is then removed.
+
 Any other character can be used in the rules but will be ignored when drawing.
 
 `frascii l_system -start "F" -rules "(F->F+F-F-F+F)" -n 2 -direction R`
 
 ```
           ┌─┐           
         ┌─┘ └─┐
```

### Comparing `frascii-2.5/frascii/__init__.py` & `frascii-2.6/frascii/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-from frascii.fractals.mandelbrot import mandelbrot_string
-from frascii.fractals.julia import julia_string
+from frascii.fractals.mandelbrot import mandelbrot_string, mandelbrot_explore
+from frascii.fractals.julia import julia_string, julia_explore
 from frascii.fractals.sierpinski_carpet import sierpinski_carpet_string
 from frascii.fractals.sierpinski_triangle import sierpinski_triangle_string
 from frascii.fractals.cantor import cantor_string
 from frascii.fractals.koch import koch_string
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string
 
-__version__ = '2.5'
+__version__ = '2.6'
 
-def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid):
+def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
+	if explore:
+		x, y, x_radius, y_radius, stepsize, max_iter, style, grid = mandelbrot_explore(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
-def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid):
+def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
+	if explore:
+		x, y, x_radius, y_radius, stepsize, max_iter, style, grid = julia_explore(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 	return julia_string(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
 def sierpinski_carpet(n):
 	return sierpinski_carpet_string(n)
 
 def cantor(n):
 	return cantor_string(n)
```

### Comparing `frascii-2.5/frascii/commands.py` & `frascii-2.6/frascii/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,19 @@
 	mandelbrot_parser.add_argument("-y_radius", type=int, help="pixels added on top and bottom of center", nargs="?", default=14)
 	mandelbrot_parser.add_argument("-stepsize", type=float, help="size of a pixel", nargs="?", default=0.05)
 	mandelbrot_parser.add_argument("-max_iter", type=int, help="iterations after which z is assumed to be in the set", nargs="?", default=20)
 	mandelbrot_parser.add_argument("-style", type=str, help="style of the visualization",
 								   choices=["repeating", "non-repeating"], nargs="?", default="non-repeating")
 	mandelbrot_parser.add_argument("-grid", type=str, help="square (double-chars) or rectangle (single-char) grid.",
 								   choices=["square", "rect"], nargs="?", default="rect")
+	mandelbrot_parser.add_argument("-explore", help=("explore the mandelbrot set using mouse and keyboard. Use mouse or arrow keys to navigate."
+																 "Use page-up and page-down to zoom in and out."
+																 "Use ',' and '.' to change the amount of iteratios. Use '-' to change style."
+																 "Exit with ESC or 'x'."),
+									action="store_true")
 	mandelbrot_parser.set_defaults(func=frascii.mandelbrot)
 
 	# Julia sub-command
 	julia_parser = subparsers.add_parser("julia", description="Wikipedia: https://en.wikipedia.org/wiki/Julia_set", formatter_class=fc)
 	julia_parser.add_argument("-f", type=str, help="complex function", nargs="?", default="z**2 - 0.4 + 0.6j")
 	julia_parser.add_argument("-x", type=float, help="real part of the images center", nargs="?", default=0)
 	julia_parser.add_argument("-y", type=float, help="imaginary part of the images center", nargs="?", default=0)
@@ -74,15 +79,19 @@
 	julia_parser.add_argument("-y_radius", type=int, help="pixels added on top and bottom of center", nargs="?", default=18)
 	julia_parser.add_argument("-stepsize", type=float, help="size of a pixel", nargs="?", default=0.033)
 	julia_parser.add_argument("-max_iter", type=int, help="iterations after which z is assumed to be in the set", nargs="?", default=40)
 	julia_parser.add_argument("-style", type=str, help="style of the visualization",
 								   choices=["repeating", "non-repeating"], nargs="?", default="non-repeating")
 	julia_parser.add_argument("-grid", type=str, help="square (double-chars) or rectangle (single-char) grid.",
 								   choices=["square", "rect"], nargs="?", default="rect")
-
+	julia_parser.add_argument("-explore", help=("explore the mandelbrot set using mouse and keyboard. Use mouse or arrow keys to navigate."
+																 "Use page-up and page-down to zoom in and out."
+																 "Use ',' and '.' to change the amount of iteratios. Use '-' to change style."
+																 "Exit with ESC or 'x'."),
+									action="store_true")
 	julia_parser.set_defaults(func=frascii.julia)
 
 	# L-system sub-command
 	l_system_parser = subparsers.add_parser("l_system", description="Wikipedia: https://en.wikipedia.org/wiki/L-system", formatter_class=fc)
 	l_system_parser.add_argument("-start", type=str, help="real part of the images center", nargs="?", default="F")
 	l_system_parser.add_argument("-rules", type=str, help="imaginary part of the images center", nargs="?", default="(F->F+F-F-F+F)")
 	l_system_parser.add_argument("-n", type=int, help="pixels added on left and right of center", nargs="?", default=3)
```

### Comparing `frascii-2.5/frascii/fractals/dragon_curve.py` & `frascii-2.6/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.5/frascii/fractals/fibonacci.py` & `frascii-2.6/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-2.5/frascii/fractals/hilbert_curve.py` & `frascii-2.6/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.5/frascii/fractals/koch.py` & `frascii-2.6/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-2.5/frascii/fractals/l_system.py` & `frascii-2.6/frascii/fractals/l_system.py`

 * *Files identical despite different names*

### Comparing `frascii-2.5/frascii/fractals/mandelbrot.py` & `frascii-2.6/frascii/fractals/mandelbrot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 def in_mandelbrot(c, max_iter):
 	z = 0
 	for i in range(max_iter):
 		z = z**2 + c
 		if abs(z) >= 2:
 			return i
 	return max_iter
@@ -29,57 +28,74 @@
 			m = len(shades)
 			return '\n'.join(''.join("  " if d == 0 else shades[d%m]*2 if d < max_iter else "██" for d in l) for l in mset)
 
 		elif style == "non-repeating":
 			shades = [' ', '░', '▒', '▓', '█']
 			return '\n'.join(''.join(shades[int(4*d/max_iter)]*2 for d in l) for l in mset)
 
-if __name__ == '__main__':
+def mandelbrot_explore(x, y, x_radius, y_radius, stepsize, max_iter, style="repeating", grid="rect"):
+	
 	import curses
 	from curses import wrapper
 	stdscr = curses.initscr()
-	#curses.use_default_colors()	
 	curses.mousemask(1)
 	curses.noecho()
 	curses.cbreak()
 	stdscr.keypad(True)
+	s = stepsize
+	i = max_iter
 
 	def main(stdscr):
-		x = -0.8
-		y = 0
-		s = 0.05
-		i = 20
-
-		# Clear screen
+		nonlocal x
+		nonlocal y
+		nonlocal x_radius
+		nonlocal y_radius
+		nonlocal s
+		nonlocal style
+		nonlocal grid
+		nonlocal i
+		styles = ["non-repeating", "repeating"]
+		si = 0 if style == "non-repeating" else 1
+ 	
 		while True:
 			stdscr.clear()
 			rows, cols = stdscr.getmaxyx()
-			y_radius = rows//2-1
-			x_radius = cols//2-1
-			stdscr.addstr(0, 0, mandelbrot_string(x, y, x_radius, y_radius, s, i, "repeating"))
+			y_rad = min(y_radius, rows//2-1)
+			x_rad = min(x_radius, cols//(2 if grid == "rect" else 4)-1)
+			stdscr.addstr(0, 0, mandelbrot_string(x, y, x_rad, y_rad, s, i, styles[si], grid))
 			stdscr.refresh()
 			key = stdscr.getch()
 			curses.flushinp()
 			if key == curses.KEY_RIGHT:
 				x += 5*s
-			if key == curses.KEY_LEFT:
+			elif key == curses.KEY_LEFT:
 				x -= 5*s
-			if key == curses.KEY_UP:
+			elif key == curses.KEY_UP:
 				y += 5*s
-			if key == curses.KEY_DOWN:
+			elif key == curses.KEY_DOWN:
 				y -= 5*s
-			if key == curses.KEY_NPAGE:
+			elif key == curses.KEY_NPAGE:
 				s /= 2
-			if key == curses.KEY_PPAGE:
+			elif key == curses.KEY_PPAGE:
 				s *= 2
-			if key == ord(','):
+			elif key == ord(','):
 				i -= 1
 				i = max(i,1)
-			if key == ord('.'):
+			elif key == ord('.'):
 				i += 1
-			if key == curses.KEY_MOUSE:
+			elif key == ord('-'):
+				si = 1 - si
+			elif key == curses.KEY_MOUSE:
 				_, mx, my, _, _ = curses.getmouse()
-				x += (mx - x_radius)*s
-				y += (-my + y_radius)*s
-			
-	wrapper(main)
+				x += ((mx if grid == "rect" else mx//2) - x_rad)*s
+				y += (-my + y_rad)*s
+			elif key == 27 or key == ord('x'):
+				break
+
+		return x, y, x_rad, y_rad, s, i, styles[si], grid
+
+	args = wrapper(main)
+	curses.endwin()
+	return args
 
+if __name__ == '__main__':
+	mandelbrot_explore(x=-0.8, y=0, x_radius=4000, y_radius=4000, stepsize=0.05, max_iter=20)
```

### Comparing `frascii-2.5/frascii/fractals/peano_curve.py` & `frascii-2.6/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.5/frascii/fractals/sierpinski_carpet.py` & `frascii-2.6/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-2.5/frascii.egg-info/SOURCES.txt` & `frascii-2.6/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

