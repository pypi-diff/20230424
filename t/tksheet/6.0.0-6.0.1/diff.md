# Comparing `tmp/tksheet-6.0.0.tar.gz` & `tmp/tksheet-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.0.0.tar", last modified: Sat Apr 22 18:12:28 2023, max compression
+gzip compressed data, was "tksheet-6.0.1.tar", last modified: Mon Apr 24 17:39:04 2023, max compression
```

## Comparing `tksheet-6.0.0.tar` & `tksheet-6.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 18:12:28.041739 tksheet-6.0.0/
--rw-rw-rw-   0        0        0     1101 2023-04-13 09:47:22.000000 tksheet-6.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2882 2023-04-22 18:12:28.041739 tksheet-6.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2232 2023-04-18 08:24:22.000000 tksheet-6.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-04-22 18:12:28.041739 tksheet-6.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-04-06 11:16:22.000000 tksheet-6.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 18:12:28.026112 tksheet-6.0.0/tksheet/
--rw-rw-rw-   0        0        0      351 2023-04-13 08:55:45.000000 tksheet-6.0.0/tksheet/__init__.py
--rw-rw-rw-   0        0        0   154985 2023-04-22 17:48:29.000000 tksheet-6.0.0/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   100042 2023-04-22 17:24:51.000000 tksheet-6.0.0/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0    10066 2023-04-22 08:55:16.000000 tksheet-6.0.0/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   326370 2023-04-22 16:43:14.000000 tksheet-6.0.0/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12894 2023-04-21 17:11:16.000000 tksheet-6.0.0/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0    99701 2023-04-22 17:25:19.000000 tksheet-6.0.0/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5642 2023-04-20 08:50:10.000000 tksheet-6.0.0/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    52264 2023-04-22 08:42:39.000000 tksheet-6.0.0/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-04-22 18:12:28.041739 tksheet-6.0.0/tksheet.egg-info/
--rw-rw-rw-   0        0        0     2882 2023-04-22 18:12:28.000000 tksheet-6.0.0/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-22 18:12:28.000000 tksheet-6.0.0/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 18:12:28.000000 tksheet-6.0.0/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 18:12:28.000000 tksheet-6.0.0/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 17:39:04.375100 tksheet-6.0.1/
+-rw-rw-rw-   0        0        0     1101 2023-04-13 09:47:22.000000 tksheet-6.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2882 2023-04-24 17:39:04.375100 tksheet-6.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2232 2023-04-18 08:24:22.000000 tksheet-6.0.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 17:39:04.375100 tksheet-6.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-04-23 07:10:11.000000 tksheet-6.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:39:04.375100 tksheet-6.0.1/tksheet/
+-rw-rw-rw-   0        0        0      351 2023-04-13 08:55:45.000000 tksheet-6.0.1/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   164503 2023-04-24 17:34:13.000000 tksheet-6.0.1/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0    99275 2023-04-24 11:22:20.000000 tksheet-6.0.1/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0    10233 2023-04-24 07:09:26.000000 tksheet-6.0.1/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   328996 2023-04-24 16:00:43.000000 tksheet-6.0.1/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12952 2023-04-24 11:27:55.000000 tksheet-6.0.1/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0    99038 2023-04-24 11:22:38.000000 tksheet-6.0.1/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5642 2023-04-20 08:50:10.000000 tksheet-6.0.1/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    52264 2023-04-22 08:42:39.000000 tksheet-6.0.1/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:39:04.375100 tksheet-6.0.1/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     2882 2023-04-24 17:39:04.000000 tksheet-6.0.1/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-24 17:39:04.000000 tksheet-6.0.1/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:39:04.000000 tksheet-6.0.1/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 17:39:04.000000 tksheet-6.0.1/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.0.0/LICENSE.txt` & `tksheet-6.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.0/PKG-INFO` & `tksheet-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.0.0
+Version: 6.0.1
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.0.0.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.0.1.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.0.0/README.md` & `tksheet-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.0/setup.py` & `tksheet-6.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.0.0',
+  version = '6.0.1',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.0.0.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.0.1.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.0.0/tksheet/_tksheet.py` & `tksheet-6.0.1/tksheet/_tksheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,28 +51,30 @@
                  header_height: str = "1", #str or int
                  max_colwidth: str = "inf", #str or int
                  max_rh: str = "inf", #str or int
                  max_header_height: str = "inf", #str or int
                  max_row_width: str = "inf", #str or int
                  row_index: list = None,
                  index: list = None,
-                 after_redraw_time_ms: int = 100,
+                 after_redraw_time_ms: int = 50,
                  row_index_width: int = 100,
                  auto_resize_default_row_index: bool = True,
                  set_all_heights_and_widths: bool = False,
                  row_height: str = "1", #str or int
                  font: tuple = get_font(),
                  header_font: tuple = get_heading_font(),
                  index_font: tuple = get_index_font(), #currently has no effect
                  popup_menu_font: tuple = get_font(),
                  align: str = "w",
                  header_align: str = "center",
                  row_index_align: str = "center",
                  displayed_columns: list = [],
                  all_columns_displayed: bool = True,
+                 displayed_rows: list = [],
+                 all_rows_displayed: bool = True,
                  max_undos: int = 30,
                  outline_thickness: int = 0,
                  outline_color: str = theme_light_blue['outline_color'],
                  column_drag_and_drop_perform: bool = True,
                  row_drag_and_drop_perform: bool = True,
                  empty_horizontal: int = 150,
                  empty_vertical: int = 100,
@@ -234,14 +236,16 @@
                             table_selected_rows_bg = table_selected_rows_bg,
                             table_selected_rows_fg = table_selected_rows_fg,
                             table_selected_columns_border_fg = table_selected_columns_border_fg,
                             table_selected_columns_bg = table_selected_columns_bg,
                             table_selected_columns_fg = table_selected_columns_fg,
                             displayed_columns = displayed_columns,
                             all_columns_displayed = all_columns_displayed,
+                            displayed_rows = displayed_rows,
+                            all_rows_displayed = all_rows_displayed,
                             selected_rows_to_end_of_window = selected_rows_to_end_of_window,
                             horizontal_grid_to_end_of_window = horizontal_grid_to_end_of_window,
                             vertical_grid_to_end_of_window = vertical_grid_to_end_of_window,
                             empty_horizontal = empty_horizontal,
                             empty_vertical = empty_vertical,
                             max_undos = max_undos)
         self.TL = TopLeftRectangle(parentframe = self,
@@ -407,14 +411,20 @@
             self.MT.focus_set()
         elif canvas == "header":
             self.CH.focus_set()
         elif canvas == "index":
             self.RI.focus_set()
         elif canvas == "topleft":
             self.TL.focus_set()
+            
+    def displayed_column_to_data(self, c):
+        return c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+    
+    def displayed_row_to_data(self, r):
+        return r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
 
     def popup_menu_add_command(self, label, func, table_menu = True, index_menu = True, header_menu = True, empty_space_menu = True):
         if label not in self.MT.extra_table_rc_menu_funcs and table_menu:
             self.MT.extra_table_rc_menu_funcs[label] = func
         if label not in self.MT.extra_index_rc_menu_funcs and index_menu:
             self.MT.extra_index_rc_menu_funcs[label] = func
         if label not in self.MT.extra_header_rc_menu_funcs and header_menu:
@@ -755,22 +765,20 @@
     def get_row_heights(self, canvas_positions = False):
         if canvas_positions:
             return [int(n) for n in self.MT.row_positions]
         return [int(b - a) for a, b in zip(self.MT.row_positions, islice(self.MT.row_positions, 1, len(self.MT.row_positions)))]
 
     def set_all_cell_sizes_to_text(self, redraw = True):
         self.MT.set_all_cell_sizes_to_text()
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
         return self.MT.row_positions, self.MT.col_positions
 
     def set_all_column_widths(self, width = None, only_set_if_too_small = False, redraw = True, recreate_selection_boxes = True):
         self.CH.set_width_of_all_cols(width = width, only_set_if_too_small = only_set_if_too_small, recreate = recreate_selection_boxes)
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
 
     def column_width(self, column = None, width = None, only_set_if_too_small = False, redraw = True):
         if column == "all":
             if width == "default":
                 self.MT.reset_col_positions()
         elif column == "displayed":
             if width == "text":
@@ -779,16 +787,15 @@
                     self.CH.set_col_width(c)
         elif width == "text" and column is not None:
             self.CH.set_col_width(col = column, width = None, only_set_if_too_small = only_set_if_too_small)
         elif width is not None and column is not None:
             self.CH.set_col_width(col = column, width = width, only_set_if_too_small = only_set_if_too_small)
         elif column is not None:
             return int(self.MT.col_positions[column + 1] - self.MT.col_positions[column])
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
 
     def set_column_widths(self, column_widths = None, canvas_positions = False, reset = False, verify = False):
         cwx = None
         if reset:
             self.MT.reset_col_positions()
             return
         if verify:
@@ -798,21 +805,19 @@
                 self.MT.col_positions = column_widths
             else:
                 self.MT.col_positions = list(accumulate(chain([0], (width for width in column_widths))))
         return cwx
 
     def set_all_row_heights(self, height = None, only_set_if_too_small = False, redraw = True, recreate_selection_boxes = True):
         self.RI.set_height_of_all_rows(height = height, only_set_if_too_small = only_set_if_too_small, recreate = recreate_selection_boxes)
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
 
     def set_cell_size_to_text(self, row, column, only_set_if_too_small = False, redraw = True):
         self.MT.set_cell_size_to_text(r = row, c = column, only_set_if_too_small = only_set_if_too_small)
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
 
     def set_width_of_index_to_text(self, recreate = True):
         self.RI.set_width_of_index_to_text(recreate = recreate)
 
     def row_height(self, row = None, height = None, only_set_if_too_small = False, redraw = True):
         if row == "all":
             if height == "default":
@@ -824,16 +829,15 @@
                     self.RI.set_row_height(r)
         elif height == "text" and row is not None:
             self.RI.set_row_height(row = row, height = None, only_set_if_too_small = only_set_if_too_small)
         elif height is not None and row is not None:
             self.RI.set_row_height(row = row, height = height, only_set_if_too_small = only_set_if_too_small)
         elif row is not None:
             return int(self.MT.row_positions[row + 1] - self.MT.row_positions[row])
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
 
     def set_row_heights(self, row_heights = None, canvas_positions = False, reset = False, verify = False):
         if reset:
             self.MT.reset_row_positions()
             return
         if is_iterable(row_heights):
             qmin = self.MT.min_rh
@@ -913,15 +917,16 @@
         self.MT.edit_cell_(event = event, dropdown = dropdown)
 
     def delete_row_position(self, idx: int, deselect_all = False):
         self.MT.del_row_position(idx = idx,
                                  deselect_all = deselect_all)
 
     def delete_row(self, idx = 0, deselect_all = False, redraw = True):
-        self.delete_rows(rows = {idx}, deselect_all = deselect_all, redraw = redraw)
+        self.delete_rows(rows = {idx}, deselect_all = deselect_all, redraw = False)
+        self.set_refresh_timer(redraw)
 
     def delete_rows(self, rows: set = set(), deselect_all = False, redraw = True):
         if deselect_all:
             self.deselect("all", redraw = False)
         if isinstance(rows, set):
             to_del = rows
         else:
@@ -943,35 +948,35 @@
         self.RI.cell_options = {r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r): v for r, v in self.RI.cell_options.items() if r not in to_del}
         self.set_refresh_timer(redraw)
 
     def insert_row_position(self, idx = "end", height = None, deselect_all = False, redraw = False):
         self.MT.insert_row_position(idx = idx,
                                     height = height,
                                     deselect_all = deselect_all)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def insert_row_positions(self, idx = "end", heights = None, deselect_all = False, redraw = False):
         self.MT.insert_row_positions(idx = idx,
                                      heights = heights,
                                      deselect_all = deselect_all)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def total_rows(self, number = None, mod_positions = True, mod_data = True):
         if number is None:
             return int(self.MT.total_data_rows())
         if not isinstance(number, int) or number < 0:
             raise ValueError("number argument must be integer and > 0")
         if number > len(self.MT.data):
             if mod_positions:
                 height = self.MT.GetLinesHeight(int(self.MT.default_rh[0]))
                 for r in range(number - len(self.MT.data)):
                     self.MT.insert_row_position("end", height)
         elif number < len(self.MT.data):
+            if not self.MT.all_rows_displayed:
+                self.MT.display_rows(enable = False, reset_row_positions = False, deselect_all = True)
             self.MT.row_positions[number + 1:] = []
         if mod_data:
             self.MT.data_dimensions(total_rows = number)
 
     def total_columns(self, number = None, mod_positions = True, mod_data = True):
         total_cols = self.MT.total_data_cols()
         if number is None:
@@ -1006,28 +1011,21 @@
 
     def move_row_position(self, row: int, moveto: int):
         self.MT.move_row_position(row, moveto)
 
     def move_row(self, row: int, moveto: int):
         self.move_rows(moveto, row, 1)
 
-    def move_rows(self, moveto: int, to_move_min: int, number_of_rows: int, move_data: bool = True, index_type: str = "displayed", create_selections: bool = True, redraw = False):
-        if index_type.lower() == "displayed" or self.MT.all_rows_displayed:
-            new_selected, dispset = self.MT.move_rows_adjust_options_dict(moveto, to_move_min, number_of_rows, move_data, create_selections)
-        else:
-            new_selected, dispset = self.MT.move_rows_adjust_options_dict(moveto, to_move_min, number_of_rows, move_data, create_selections)
-        self.set_refresh_timer(redraw)
-        return new_selected, dispset
-
     def delete_column_position(self, idx: int, deselect_all = False):
         self.MT.del_col_position(idx,
                                  deselect_all = deselect_all)
 
     def delete_column(self, idx = 0, deselect_all = False, redraw = True):
-        self.delete_columns(columns = {idx}, deselect_all = deselect_all, redraw = redraw)
+        self.delete_columns(columns = {idx}, deselect_all = deselect_all, redraw = False)
+        self.set_refresh_timer(redraw)
         
     def delete_columns(self, columns: set = set(), deselect_all = False, redraw = True):
         if deselect_all:
             self.deselect("all", redraw = False)
         if isinstance(columns, set):
             to_del = columns
         else:
@@ -1050,36 +1048,33 @@
         self.CH.cell_options = {c if not bisect.bisect_left(to_bis, c) else c - bisect.bisect_left(to_bis, c): v for c, v in self.CH.cell_options.items() if c not in to_del}
         self.set_refresh_timer(redraw)
 
     def insert_column_position(self, idx = "end", width = None, deselect_all = False, redraw = False):
         self.MT.insert_col_position(idx = idx,
                                     width = width,
                                     deselect_all = deselect_all)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def insert_column_positions(self, idx = "end", widths = None, deselect_all = False, redraw = False):
         self.MT.insert_col_positions(idx = idx,
                                      widths = widths,
                                      deselect_all = deselect_all)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def move_column_position(self, column: int, moveto: int):
         self.MT.move_col_position(column, moveto)
 
     def move_column(self, column: int, moveto: int):
         self.move_columns(moveto, column, 1)
 
     def move_columns(self, moveto: int, to_move_min: int, number_of_columns: int, move_data: bool = True, index_type: str = "displayed", create_selections: bool = True, redraw = False):
         if index_type.lower() == "displayed" or self.MT.all_columns_displayed:
             new_selected, dispset = self.MT.move_columns_adjust_options_dict(moveto, to_move_min, number_of_columns, move_data, create_selections)
-            self.set_refresh_timer(redraw)
-            return new_selected, dispset
         else:
+            dispset = {}
             c = int(moveto)
             to_move_max = to_move_min + number_of_columns
             totalcols = int(number_of_columns)
             to_del = to_move_max + number_of_columns
             orig_selected = list(range(to_move_min, to_move_min + totalcols))
             num_data_cols = self.MT.total_data_cols()
             if c + totalcols > num_data_cols:
@@ -1142,16 +1137,92 @@
                 }
                 self.MT.col_options = {
                     int(newcolsdct[k]) if k in newcolsdct else
                     k - totalcols if k < c and k > to_move_min else
                     int(k): v for k, v in self.MT.col_options.items()
                 }
                 self.MT.displayed_columns = sorted(int(newcolsdct[k]) if k in newcolsdct else k - totalcols if k < c and k > to_move_min else int(k) for k in self.MT.displayed_columns)
-            self.set_refresh_timer(redraw)
-            return new_selected, {}
+        self.set_refresh_timer(redraw)
+        return new_selected, dispset
+        
+    def move_rows(self, moveto: int, to_move_min: int, number_of_rows: int, move_data: bool = True, index_type: str = "displayed", create_selections: bool = True, redraw = False):
+        if index_type.lower() == "displayed" or self.MT.all_rows_displayed:
+            new_selected, dispset = self.MT.move_rows_adjust_options_dict(moveto, to_move_min, number_of_rows, move_data, create_selections)
+        else:
+            dispset = {}
+            r = int(moveto)
+            to_move_max = to_move_min + number_of_rows
+            totalrows = int(number_of_rows)
+            to_del = to_move_max + number_of_rows
+            orig_selected = list(range(to_move_min, to_move_min + totalrows))
+            num_data_rows = self.MT.total_data_rows()
+            if r + totalrows > num_data_rows:
+                new_selected = tuple(range(num_data_rows - totalrows, num_data_rows))
+            else:
+                if to_move_min > r:
+                    new_selected = tuple(range(r, r + totalrows))
+                else:
+                    new_selected = tuple(range(r + 1 - totalrows, r + 1))
+            newrowsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
+            if to_move_min > r:
+                if len(self.MT.data) < to_move_max:
+                    self.MT.data.extend(list(repeat("", to_move_max - len(self.MT.data) + 1)))
+                self.MT.data[r:r] = self.MT.data[to_move_min:to_move_max]
+                self.MT.data[to_move_max:to_del] = []
+                if isinstance(self.MT._row_index, list) and self.MT._row_index:
+                    if len(self.MT._row_index) < to_move_max:
+                        self.MT._row_index.extend(list(repeat("", to_move_max - len(self.MT._row_index) + 1)))
+                    self.MT._row_index[r:r] = self.MT._row_index[to_move_min:to_move_max]
+                    self.MT._row_index[to_move_max:to_del] = []
+                self.RI.cell_options = {
+                    int(newrowsdct[k]) if k in newrowsdct else
+                    k + totalrows if k < to_move_min and k >= r else
+                    int(k): v for k, v in self.RI.cell_options.items()
+                }
+                self.MT.cell_options = {
+                    (int(newrowsdct[k[0]]), k[1]) if k[0] in newrowsdct else
+                    (k[0] + totalrows, k[1]) if k[0] < to_move_min and k[0] >= r else
+                    k: v for k, v in self.MT.cell_options.items()
+                }
+                self.MT.row_options = {
+                    int(newrowsdct[k]) if k in newrowsdct else
+                    k + totalrows if k < to_move_min and k >= r else
+                    int(k): v for k, v in self.MT.row_options.items()
+                }
+                self.MT.displayed_rows = sorted(int(newrowsdct[k]) if k in newrowsdct else k + totalrows if k < to_move_min and k >= r else int(k) for k in self.MT.displayed_rows)
+            else:
+                r += 1
+                if move_data:
+                    if len(self.MT.data) < r - 1:
+                        self.MT.data.extend(list(repeat("", r - len(self.MT.data))))
+                    self.MT.data[r:r] = self.MT.data[to_move_min:to_move_max]
+                    self.MT.data[to_move_min:to_move_max] = []
+                    if isinstance(self.MT._row_index, list) and self.MT._row_index:
+                        if len(self.MT._row_index) < r:
+                            self.MT._row_index.extend(list(repeat("", r - len(self.MT._row_index))))
+                        self.MT._row_index[r:r] = self.MT._row_index[to_move_min:to_move_max]
+                        self.MT._row_index[to_move_min:to_move_max] = []
+                self.RI.cell_options = {
+                    int(newrowsdct[k]) if k in newrowsdct else
+                    k - totalrows if k < r and k > to_move_min else
+                    int(k): v for k, v in self.RI.cell_options.items()
+                }
+                self.MT.cell_options = {
+                    (int(newrowsdct[k[0]]), k[1]) if k[0] in newrowsdct else
+                    (k[0] - totalrows, k[1]) if k[0] < r and k[0] > to_move_min else
+                    k: v for k, v in self.MT.cell_options.items()
+                }
+                self.MT.row_options = {
+                    int(newrowsdct[k]) if k in newrowsdct else
+                    k - totalrows if k < r and k > to_move_min else
+                    int(k): v for k, v in self.MT.row_options.items()
+                }
+                self.MT.displayed_rows = sorted(int(newrowsdct[k]) if k in newrowsdct else k - totalrows if k < r and k > to_move_min else int(k) for k in self.MT.displayed_rows)
+        self.set_refresh_timer(redraw)
+        return new_selected, dispset
 
     # works on currently selected box
     def open_cell(self, ignore_existing_editor = True):
         self.MT.open_cell(event = GeneratedMouseEvent(), ignore_existing_editor = ignore_existing_editor)
         
     def open_header_cell(self, ignore_existing_editor = True):
         self.CH.open_cell(event = GeneratedMouseEvent(), ignore_existing_editor = ignore_existing_editor)
@@ -1208,53 +1279,64 @@
     def set_yview(self, position, option = "moveto"):
         self.MT.set_yviews(option, position)
 
     def set_view(self, x_args, y_args):
         self.MT.set_view(x_args, y_args)
 
     def see(self, row = 0, column = 0, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = True):
-        self.MT.see(row, column, keep_yscroll, keep_xscroll, bottom_right_corner, check_cell_visibility = check_cell_visibility, redraw = redraw)
+        self.MT.see(row, column, keep_yscroll, keep_xscroll, bottom_right_corner, check_cell_visibility = check_cell_visibility, redraw = False)
+        self.set_refresh_timer(redraw)
 
     def select_row(self, row, redraw = True):
-        self.RI.select_row(int(row) if not isinstance(row, int) else row, redraw = redraw)
+        self.RI.select_row(int(row) if not isinstance(row, int) else row, redraw = False)
+        self.set_refresh_timer(redraw)
 
     def select_column(self, column, redraw = True):
-        self.CH.select_col(int(column) if not isinstance(column, int) else column, redraw = redraw)
+        self.CH.select_col(int(column) if not isinstance(column, int) else column, redraw = False)
+        self.set_refresh_timer(redraw)
 
     def select_cell(self, row, column, redraw = True):
         self.MT.select_cell(int(row) if not isinstance(row, int) else row,
                             int(column) if not isinstance(column, int) else column,
-                            redraw = redraw)
+                            redraw = False)
+        self.set_refresh_timer(redraw)
 
     def select_all(self, redraw = True, run_binding_func = True):
-        self.MT.select_all(redraw = redraw, run_binding_func = run_binding_func)
+        self.MT.select_all(redraw = False, run_binding_func = run_binding_func)
+        self.set_refresh_timer(redraw)
 
     def move_down(self):
         self.MT.move_down()
 
     def add_cell_selection(self, row, column, redraw = True, run_binding_func = True, set_as_current = True):
-        self.MT.add_selection(r = row, c = column, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.MT.add_selection(r = row, c = column, redraw = False, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.set_refresh_timer(redraw)
 
     def add_row_selection(self, row, redraw = True, run_binding_func = True, set_as_current = True):
-        self.RI.add_selection(r = row, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.RI.add_selection(r = row, redraw = False, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.set_refresh_timer(redraw)
 
     def add_column_selection(self, column, redraw = True, run_binding_func = True, set_as_current = True):
-        self.CH.add_selection(c = column, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.CH.add_selection(c = column, redraw = False, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.set_refresh_timer(redraw)
 
     def toggle_select_cell(self, row, column, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
-        self.MT.toggle_select_cell(row = row, column = column, add_selection = add_selection, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.MT.toggle_select_cell(row = row, column = column, add_selection = add_selection, redraw = False, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.set_refresh_timer(redraw)
 
     def toggle_select_row(self, row, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
-        self.RI.toggle_select_row(row = row, add_selection = add_selection, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.RI.toggle_select_row(row = row, add_selection = add_selection, redraw = False, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.set_refresh_timer(redraw)
 
     def toggle_select_column(self, column, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
-        self.CH.toggle_select_col(column = column, add_selection = add_selection, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.CH.toggle_select_col(column = column, add_selection = add_selection, redraw = False, run_binding_func = run_binding_func, set_as_current = set_as_current)
+        self.set_refresh_timer(redraw)
 
     def deselect(self, row = None, column = None, cell = None, redraw = True):
-        self.MT.deselect(r = row, c = column, cell = cell, redraw = redraw)
+        self.MT.deselect(r = row, c = column, cell = cell, redraw = False)
 
     # (row, column, type_) e.g. (0, 0, "column") as a named tuple
     def get_currently_selected(self):
         return self.MT.currently_selected()
 
     def set_currently_selected(self, row, column, type_ = "cell", selection_binding = True):
         self.MT.create_current(r = row,
@@ -1323,65 +1405,57 @@
 
     def all_selected(self):
         return self.MT.all_selected()
 
     def readonly_rows(self, rows = [], readonly = True, redraw = False):
         self.MT.readonly_rows(rows = rows,
                               readonly = readonly)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def readonly_columns(self, columns = [], readonly = True, redraw = False):
         self.MT.readonly_columns(columns = columns,
                                  readonly = readonly)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def readonly_cells(self, row = 0, column = 0, cells = [], readonly = True, redraw = False):
         self.MT.readonly_cells(row = row,
                                column = column,
                                cells = cells,
                                readonly = readonly)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
             
     def readonly_header(self, columns = [], readonly = True, redraw = False):
         self.CH.readonly_header(columns = columns,
                                 readonly = readonly)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
             
     def readonly_index(self, rows = [], readonly = True, redraw = False):
         self.RI.readonly_index(rows = rows,
                                readonly = readonly)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
-    def dehighlight_all(self):
+    def dehighlight_all(self, redraw = True):
         for k in self.MT.cell_options:
             if 'highlight' in self.MT.cell_options[k]:
                 del self.MT.cell_options[k]['highlight']
-                
         for k in self.MT.row_options:
             if 'highlight' in self.MT.row_options[k]:
                 del self.MT.row_options[k]['highlight']
-                
         for k in self.MT.col_options:
             if 'highlight' in self.MT.col_options[k]:
                 del self.MT.col_options[k]['highlight']
-                
         for k in self.RI.cell_options:
             if 'highlight' in self.RI.cell_options[k]:
                 del self.RI.cell_options[k]['highlight']
-                
         for k in self.CH.cell_options:
             if 'highlight' in self.CH.cell_options[k]:
                 del self.CH.cell_options[k]['highlight']
+        self.set_refresh_timer(redraw)
 
-    def dehighlight_rows(self, rows = [], redraw = False):
+    def dehighlight_rows(self, rows = [], redraw = True):
         if isinstance(rows, int):
             rows_ = [rows]
         else:
             rows_ = rows
         if not rows_ or rows_ == "all":
             for r in self.MT.row_options:
                 if 'highlight' in self.MT.row_options[r]:
@@ -1396,18 +1470,17 @@
                     del self.MT.row_options[r]['highlight']
                 except:
                     pass
                 try:
                     del self.RI.cell_options[r]['highlight']
                 except:
                     pass
-        if redraw:
-            self.refresh(True, True)
+        self.set_refresh_timer(redraw)
 
-    def dehighlight_columns(self, columns = [], redraw = False):
+    def dehighlight_columns(self, columns = [], redraw = True):
         if isinstance(columns, int):
             columns_ = [columns]
         else:
             columns_ = columns
         if not columns_ or columns_ == "all":
             for c in self.MT.col_options:
                 if 'highlight' in self.MT.col_options[c]:
@@ -1422,57 +1495,59 @@
                     del self.MT.col_options[c]['highlight']
                 except:
                     pass
                 try:
                     del self.CH.cell_options[c]['highlight']
                 except:
                     pass
-        if redraw:
-            self.refresh(True, True)
+        self.set_refresh_timer(redraw)
             
-    def highlight_rows(self, rows = [], bg = None, fg = None, highlight_index = True, redraw = False, end_of_screen = False, overwrite = True):
+    def highlight_rows(self, rows = [], bg = None, fg = None, highlight_index = True, redraw = True, end_of_screen = False, overwrite = True):
         self.MT.highlight_rows(rows = rows,
                                bg = bg,
                                fg = fg,
                                highlight_index = highlight_index,
-                               redraw = redraw,
+                               redraw = False,
                                end_of_screen = end_of_screen,
                                overwrite = overwrite)
+        self.set_refresh_timer(redraw)
 
-    def highlight_columns(self, columns = [], bg = None, fg = None, highlight_header = True, redraw = False, overwrite = True):
+    def highlight_columns(self, columns = [], bg = None, fg = None, highlight_header = True, redraw = True, overwrite = True):
         self.MT.highlight_cols(cols = columns,
                                bg = bg,
                                fg = fg,
                                highlight_header = highlight_header,
-                               redraw = redraw,
+                               redraw = False,
                                overwrite = overwrite)
+        self.set_refresh_timer(redraw)
 
-    def highlight_cells(self, row = 0, column = 0, cells = [], canvas = "table", bg = None, fg = None, redraw = False, overwrite = True):
+    def highlight_cells(self, row = 0, column = 0, cells = [], canvas = "table", bg = None, fg = None, redraw = True, overwrite = True):
         if canvas == "table":
             self.MT.highlight_cells(r = row,
                                     c = column,
                                     cells = cells,
                                     bg = bg,
                                     fg = fg,
-                                    redraw = redraw,
+                                    redraw = False,
                                     overwrite = overwrite)
         elif canvas in ("row_index", "index"):
             self.RI.highlight_cells(r = row,
                                     cells = cells,
                                     bg = bg,
                                     fg = fg,
-                                    redraw = redraw,
+                                    redraw = False,
                                     overwrite = overwrite)
         elif canvas == "header":
             self.CH.highlight_cells(c = column,
                                     cells = cells,
                                     bg = bg,
                                     fg = fg,
-                                    redraw = redraw,
+                                    redraw = False,
                                     overwrite = overwrite)
+        self.set_refresh_timer(redraw)
 
     def dehighlight_cells(self, row = 0, column = 0, cells = [], canvas = "table", all_ = False, redraw = True):
         if row == "all" and canvas == "table":
             for k, v in self.MT.cell_options.items():
                 if 'highlight' in v:
                     del self.MT.cell_options[k]['highlight']
         elif row == "all" and canvas == "row_index":
@@ -1521,16 +1596,15 @@
             elif not all_:
                 if column in self.CH.cell_options and 'highlight' in self.CH.cell_options[column]:
                     del self.CH.cell_options[column]['highlight']
             elif all_:
                 for c in self.CH.cell_options:
                     if 'highlight' in self.CH.cell_options[c]:
                         del self.CH.cell_options[c]['highlight']
-        if redraw:
-            self.refresh(True, True)
+        self.set_refresh_timer(redraw)
             
     def delete_out_of_bounds_options(self):
         maxc = self.total_columns()
         maxr = self.total_rows()
         self.MT.cell_options = {k: v for k, v in self.MT.cell_options.items() if k[0] < maxr and k[1] < maxc}
         self.RI.cell_options = {k: v for k, v in self.RI.cell_options.items() if k < maxr}
         self.CH.cell_options = {k: v for k, v in self.CH.cell_options.items() if k < maxc}
@@ -1593,100 +1667,92 @@
                     self.MT.align_rows(rows = k,
                                        align = v,
                                        align_index = align_index)
             else:
                 self.MT.align_rows(rows = rows,
                                    align = align if align == "global" else self.convert_align(align),
                                    align_index = align_index)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
         
     def align_columns(self, columns = [], align = "global", align_header = False, redraw = True): #"center", "w", "e" or "global"
         if align == "global" or self.convert_align(align):
             if isinstance(columns, dict):
                 for k, v in columns.items():
                     self.MT.align_columns(columns = k,
                                           align = v,
                                           align_header = align_header)
             else:
                 self.MT.align_columns(columns = columns,
                                       align = align if align == "global" else self.convert_align(align),
                                       align_header = align_header)
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def align_cells(self, row = 0, column = 0, cells = [], align = "global", redraw = True): #"center", "w", "e" or "global"
         if align == "global" or self.convert_align(align):
             if isinstance(cells, dict):
                 for (r, c), v in cells.items():
                     self.MT.align_cells(row = r,
                                         column = c,
                                         cells = [],
                                         align = v)
             else:
                 self.MT.align_cells(row = row,
                                     column = column,
                                     cells = cells,
                                     align = align if align == "global" else self.convert_align(align))
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def align_header(self, columns = [], align = "global", redraw = True):
         if align == "global" or self.convert_align(align):
             if isinstance(columns, dict):
                 for k, v in columns.items():
                     self.CH.align_cells(columns = k,
                                         align = v)
             else:
                 self.CH.align_cells(columns = columns,
                                     align = align if align == "global" else self.convert_align(align))
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def align_index(self, rows = [], align = "global", redraw = True):
         if align == "global" or self.convert_align(align):
             if isinstance(rows, dict):
                 for k, v in rows.items():
                     self.RI.align_cells(rows = rows,
                                         align = v)
             else:
                 self.RI.align_cells(rows = rows,
                                     align = align if align == "global" else self.convert_align(align))
-        if redraw:
-            self.redraw()
+        self.set_refresh_timer(redraw)
 
     def align(self, align: str = None, redraw = True):
         if align is None:
             return self.MT.align
         elif self.convert_align(align):
             self.MT.align = self.convert_align(align)
         else:
             raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
 
     def header_align(self, align: str = None, redraw = True):
         if align is None:
             return self.CH.align
         elif self.convert_align(align):
             self.CH.align = self.convert_align(align)
         else:
             raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
 
     def row_index_align(self, align: str = None, redraw = True):
         if align is None:
             return self.RI.align
         elif self.convert_align(align):
             self.RI.align = self.convert_align(align)
         else:
             raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
 
     def font(self, newfont = None, reset_row_positions = True):
         self.MT.font(newfont, reset_row_positions = reset_row_positions)
 
     def header_font(self, newfont = None):
         self.MT.header_font(newfont)
 
@@ -1859,43 +1925,43 @@
             self.CH.drag_and_drop_bg = kwargs['drag_and_drop_bg']
             self.RI.drag_and_drop_bg = kwargs['drag_and_drop_bg']
         if 'outline_thickness' in kwargs:
             self.config(highlightthickness = kwargs['outline_thickness'])
         if 'outline_color' in kwargs:
             self.config(highlightbackground = kwargs['outline_color'], highlightcolor = kwargs['outline_color'])
         self.MT.create_rc_menus()
-        if redraw:
-            self.refresh()
+        self.set_refresh_timer(redraw)
 
     def change_theme(self, theme = "light blue", redraw = True):
         if theme.lower() in ("light blue", "light_blue"):
             self.set_options(**theme_light_blue,
-                             redraw = redraw)
+                             redraw = False)
             self.config(bg = theme_light_blue['table_bg'])
         elif theme.lower() == "dark":
             self.set_options(**theme_dark,
-                             redraw = redraw)
+                             redraw = False)
             self.config(bg = theme_dark['table_bg'])
         elif theme.lower() in ("light green", "light_green"):
             self.set_options(**theme_light_green,
-                             redraw = redraw)
+                             redraw = False)
             self.config(bg = theme_light_green['table_bg'])
         elif theme.lower() in ("dark blue", "dark_blue"):
             self.set_options(**theme_dark_blue,
-                             redraw = redraw)
+                             redraw = False)
             self.config(bg = theme_dark_blue['table_bg'])
         elif theme.lower() in ("dark green", "dark_green"):
             self.set_options(**theme_dark_green,
-                             redraw = redraw)
+                             redraw = False)
             self.config(bg = theme_dark_green['table_bg'])
         elif theme.lower() == "black":
             self.set_options(**theme_black,
-                             redraw = redraw)
+                             redraw = False)
             self.config(bg = theme_black['table_bg'])
         self.MT.recreate_all_selection_boxes()
+        self.set_refresh_timer(redraw)
 
     def get_header_data(self, c, get_displayed = False):
         return self.CH.get_cell_data(datacn = c, get_displayed = get_displayed)
 
     def get_index_data(self, r, get_displayed = False):
         return self.RI.get_cell_data(datarn = r, get_displayed = get_displayed)
 
@@ -2058,15 +2124,15 @@
         maxidx = len(self.MT.data[r]) - 1
         if not values:
             self.MT.data[r][:] = list(repeat("", len(self.MT.data[r])))
         if add_columns:
             for c, v in enumerate(values):
                 if c > maxidx:
                     self.MT.data[r].append(v)
-                    if self.MT.all_columns_displayed and c >= len(self.MT.col_positions) - 1:
+                    if self.MT.all_columns_displayed:
                         self.MT.insert_col_position("end")
                 else:
                     self.set_cell_data(r = r, c = c, value = v, redraw = False, keep_formatting = keep_formatting)
         else:
             for c, v in enumerate(values):
                 if c > maxidx:
                     self.MT.data[r].append(v)
@@ -2082,104 +2148,100 @@
             total_cols = None
             height = self.MT.default_rh[1]
             for rn, v in enumerate(values):
                 if rn > maxidx:
                     if total_cols is None:
                         total_cols = self.MT.total_data_cols()
                     self.MT.data.append(list(repeat("", total_cols)))
-                    self.MT.insert_row_position("end", height = height)
+                    if self.MT.all_rows_displayed:
+                        self.MT.insert_row_position("end", height = height)
                     maxidx += 1
                 if c >= len(self.MT.data[rn]):
                     self.MT.data[rn].extend(list(repeat("", c - len(self.MT.data[rn]))))
                 self.set_cell_data(r = rn, c = c, value = v, redraw = False, keep_formatting = keep_formatting)
         else:
             for rn, v in enumerate(values):
                 if c >= len(self.MT.data[rn]):
                     self.MT.data[rn].extend(list(repeat("", c - len(self.MT.data[rn]))))
                 self.set_cell_data(r = rn, c = c, value = v, redraw = False, keep_formatting = keep_formatting)
         self.set_refresh_timer(redraw)
 
     def insert_column(self,
-                      values = None, 
-                      idx = "end", 
+                      values: Union[list, tuple, int, None] = None, 
+                      idx: Union[str, int] = "end", 
                       width = None, 
                       deselect_all = False, 
                       add_rows = True, 
                       equalize_data_row_lengths = True,
                       mod_column_positions = True,
-                      redraw = False):
-        if isinstance(values, (list, tuple)):
-            _values = (values, )
-        elif values is None:
-            _values = 1
-        else:
-            _values = values
-        if isinstance(width, int):
-            _width = (width, )
-        elif width is None:
-            _width = width
-        self.insert_columns(_values,
+                      redraw = True):
+        self.insert_columns((values, ) if isinstance(values, (list, tuple)) else 1 if values is None else values,
                             idx,
-                            _width,
+                            (width, ) if isinstance(width, int) else width,
                             deselect_all, 
                             add_rows, 
                             equalize_data_row_lengths,
                             mod_column_positions,
                             redraw)
 
     def insert_columns(self, 
-                       columns = 1, 
-                       idx = "end", 
+                       columns: Union[list, tuple, int, None] = 1, 
+                       idx: Union[str, int] = "end", 
                        widths = None, 
                        deselect_all = False, 
                        add_rows = True, 
                        equalize_data_row_lengths = True,
                        mod_column_positions = True,
-                       redraw = False):
-        if mod_column_positions:
-            self.MT.insert_col_positions(idx = idx,
-                                         widths = columns if isinstance(columns, int) and widths is None else widths,
-                                         deselect_all = deselect_all)
+                       redraw = True):
         if equalize_data_row_lengths:
             old_total = self.MT.equalize_data_row_lengths()
         else:
             old_total = self.MT.total_data_cols()
         if isinstance(columns, int):
+            if columns < 1:
+                raise ValueError(f"columns arg must be greater than 0, not {columns}")
             total_rows = self.MT.total_data_rows()
             data = [list(repeat("", total_rows)) for i in range(columns)]
             numcols = columns
         else:
             data = columns
             numcols = len(columns)
-        if not self.MT.all_columns_displayed:
+        if self.MT.all_columns_displayed:
+            if mod_column_positions:
+                self.MT.insert_col_positions(idx = idx,
+                                             widths = columns if isinstance(columns, int) and widths is None else widths,
+                                             deselect_all = deselect_all)
+        elif not self.MT.all_columns_displayed:
             if idx != "end":
                 self.MT.displayed_columns = [c if c < idx else c + numcols for c in self.MT.displayed_columns]
             if mod_column_positions:
-                try:
-                    disp_next = max(self.MT.displayed_columns) + 1
-                except:
-                    disp_next = 0
-                self.MT.displayed_columns.extend(list(range(disp_next, disp_next + numcols)))
+                inspos = bisect.bisect_left(self.MT.displayed_columns, idx)
+                self.MT.displayed_columns[inspos:inspos] = list(range(idx, idx + numcols))
+                self.MT.insert_col_positions(idx = inspos,
+                                             widths = columns if isinstance(columns, int) and widths is None else widths,
+                                             deselect_all = deselect_all)
         maxidx = len(self.MT.data) - 1
         if add_rows:
             height = self.MT.default_rh[1]
             if idx == "end":
                 for values in reversed(data):
                     for rn, v in enumerate(values):
                         if rn > maxidx:
                             self.MT.data.append(list(repeat("", old_total)))
-                            self.MT.insert_row_position("end", height = height)
+                            if self.MT.all_rows_displayed:
+                                self.MT.insert_row_position("end", height = height)
                             maxidx += 1
                         self.MT.data[rn].append(v)
             else:
                 for values in reversed(data):
                     for rn, v in enumerate(values):
                         if rn > maxidx:
                             self.MT.data.append(list(repeat("", old_total)))
-                            self.MT.insert_row_position("end", height = height)
+                            if self.MT.all_rows_displayed:
+                                self.MT.insert_row_position("end", height = height)
                             maxidx += 1
                         self.MT.data[rn].insert(idx, v)
         else:
             if idx == "end":
                 for values in reversed(data):
                     for rn, v in enumerate(values):
                         if rn > maxidx:
@@ -2194,78 +2256,107 @@
         if isinstance(idx, int):
             num_add = len(data)
             self.MT.cell_options = {(rn, cn if cn < idx else cn + num_add): t2 for (rn, cn), t2 in self.MT.cell_options.items()}
             self.MT.col_options = {cn if cn < idx else cn + num_add: t for cn, t in self.MT.col_options.items()}
             self.CH.cell_options = {cn if cn < idx else cn + num_add: t for cn, t in self.CH.cell_options.items()}
         self.set_refresh_timer(redraw)
 
-    def insert_row(self, values = None, idx = "end", height = None, deselect_all = False, add_columns = False,
-                   redraw = False):
-        self.MT.insert_row_position(idx = idx,
-                                    height = height,
-                                    deselect_all = deselect_all)
+    def insert_row(self, 
+                   values: Union[list, int, None] = None, 
+                   idx: Union[str, int] = "end", 
+                   height = None, 
+                   deselect_all = False, 
+                   add_columns = False,
+                   mod_row_positions = True,
+                   redraw = True):
         total_cols = None
         if values is None:
             total_cols = self.MT.total_data_cols()
             data = list(repeat("", total_cols))
-        elif isinstance(values, list):
-            data = values
-        else:
+        elif not isinstance(values, list):
             data = list(values)
+        else:
+            data = values
         if add_columns:
             if total_cols is None:
                 total_cols = self.MT.total_data_cols()
             if len(data) > total_cols:
                 self.MT.data[:] = [r + list(repeat("", len(data) - total_cols)) for r in self.MT.data]
             elif len(data) < total_cols:
                 data += list(repeat("", total_cols - len(data)))
             if self.MT.all_columns_displayed:
                 if not self.MT.col_positions:
                     self.MT.col_positions = [0]
                 if len(data) > len(self.MT.col_positions) - 1:
                     self.insert_column_positions("end", len(data) - (len(self.MT.col_positions) - 1))
+        if self.MT.all_rows_displayed and mod_row_positions:
+            inspos = idx
+        if not self.MT.all_rows_displayed:
+            if idx != "end":
+                self.MT.displayed_rows = [r if r < idx else r + 1 for r in self.MT.displayed_rows]
+            if mod_row_positions:
+                inspos = bisect.bisect_left(self.MT.displayed_rows, idx)
+                self.MT.displayed_rows[inspos:inspos] = list(range(idx, idx + 1))
+        if mod_row_positions:
+            self.MT.insert_row_position(idx = inspos, height = height, deselect_all = deselect_all)
         if isinstance(idx, str) and idx.lower() == "end":
             self.MT.data.append(data)
         else:
             self.MT.data.insert(idx, data)
             self.MT.cell_options = {(rn if rn < idx else rn + 1, cn): t2 for (rn, cn), t2 in self.MT.cell_options.items()}
             self.MT.row_options = {rn if rn < idx else rn + 1: t for rn, t in self.MT.row_options.items()}
             self.RI.cell_options = {rn if rn < idx else rn + 1: t for rn, t in self.RI.cell_options.items()}
         self.set_refresh_timer(redraw)
 
-    def insert_rows(self, rows = 1, idx = "end", heights = None, deselect_all = False, add_columns = True,
-                    redraw = False):
+    def insert_rows(self, 
+                    rows: Union[list, int] = 1, 
+                    idx: Union[str, int] = "end", 
+                    heights = None, 
+                    deselect_all = False, 
+                    add_columns = True,
+                    mod_row_positions = True, 
+                    redraw = True):
         total_cols = None
         if isinstance(rows, int):
+            if rows < 1:
+                raise ValueError(f"rows arg must be greater than 0, not {rows}")
             total_cols = self.MT.total_data_cols()
             data = [list(repeat("", total_cols)) for i in range(rows)]
-        elif isinstance(rows, list):
-            data = rows
-        else:
+        elif not isinstance(rows, list):
             data = list(rows)
-        if heights is None:
-            heights_ = len(data)
         else:
-            heights_ = heights
-        self.MT.insert_row_positions(idx = idx,
-                                     heights = heights_,
-                                     deselect_all = deselect_all)
+            data = rows
+        try:
+            data = [r if isinstance(r, list) else list(r) for r in data]
+        except Exception as msg:
+            raise ValueError(f"rows arg must be int or list of lists. {msg}")
         if add_columns:
             if total_cols is None:
                 total_cols = self.MT.total_data_cols()
             data_max_cols = len(max(data, key = len))
             if data_max_cols > total_cols:
                 self.MT.data[:] = [r + list(repeat("", data_max_cols - total_cols)) for r in self.MT.data]
             else:
                 data[:] = [r + list(repeat("", total_cols - data_max_cols)) for r in data]
             if self.MT.all_columns_displayed:
                 if not self.MT.col_positions:
                     self.MT.col_positions = [0]
                 if data_max_cols > len(self.MT.col_positions) - 1:
                     self.insert_column_positions("end", data_max_cols - (len(self.MT.col_positions) - 1))
+        if self.MT.all_rows_displayed and mod_row_positions:
+            inspos = idx
+        if not self.MT.all_rows_displayed:
+            numrows = len(data)
+            if idx != "end":
+                self.MT.displayed_rows = [r if r < idx else r + numrows for r in self.MT.displayed_rows]
+            if mod_row_positions:
+                inspos = bisect.bisect_left(self.MT.displayed_rows, idx)
+                self.MT.displayed_rows[inspos:inspos] = list(range(idx, idx + numrows))
+        if mod_row_positions:
+            self.MT.insert_row_positions(idx = inspos, heights = len(data) if heights is None else heights, deselect_all = deselect_all)
         if isinstance(idx, str) and idx.lower() == "end":
             self.MT.data.extend(data)
         else:
             self.MT.data[idx:idx] = data
             num_add = len(data)
             self.MT.cell_options = {(rn if rn < idx else rn + num_add, cn): t2 for (rn, cn), t2 in self.MT.cell_options.items()}
             self.MT.row_options = {rn if rn < idx else rn + num_add: t for rn, t in self.MT.row_options.items()}
@@ -2279,56 +2370,117 @@
         return self.MT.total_data_rows(include_index = include_index)
 
     def get_total_columns(self, include_header = False):
         return self.MT.total_data_cols(include_header = include_header)
 
     def equalize_data_row_lengths(self):
         return self.MT.equalize_data_row_lengths()
-
+        
+    def display_rows(self,
+                     rows = None,
+                     all_rows_displayed = None,
+                     reset_row_positions = True,
+                     refresh = False,
+                     redraw = False,
+                     deselect_all = True,
+                     **kwargs):
+        if 'all_displayed' in kwargs:
+            all_rows_displayed = kwargs['all_displayed']
+        res = self.MT.display_rows(rows = None if isinstance(rows, str) and rows.lower() == "all" else rows,
+                                   all_rows_displayed = True if isinstance(rows, str) and rows.lower() == "all" else all_rows_displayed,
+                                   reset_row_positions = reset_row_positions,
+                                   deselect_all = deselect_all)
+        if refresh or redraw:
+            self.set_refresh_timer(redraw if redraw else refresh)
+        return res
+    
     def display_columns(self,
                         columns = None,
                         all_columns_displayed = None,
                         reset_col_positions = True,
                         refresh = False,
                         redraw = False,
-                        deselect_all = True):
+                        deselect_all = True,
+                        **kwargs):
+        if 'all_displayed' in kwargs:
+            all_columns_displayed = kwargs['all_displayed']
         res = self.MT.display_columns(columns = None if isinstance(columns, str) and columns.lower() == "all" else columns,
                                       all_columns_displayed = True if isinstance(columns, str) and columns.lower() == "all" else all_columns_displayed,
                                       reset_col_positions = reset_col_positions,
                                       deselect_all = deselect_all)
         if refresh or redraw:
-            self.refresh()
+            self.set_refresh_timer(redraw if redraw else refresh)
         return res
+
+    def all_rows_displayed(self, a = None):
+        v = bool(self.MT.all_rows_displayed)
+        if type(a) == bool:
+            self.MT.all_rows_displayed = a
+        return v
+    
+    def all_columns_displayed(self, a = None):
+        v = bool(self.MT.all_columns_displayed)
+        if type(a) == bool:
+            self.MT.all_columns_displayed = a
+        return v
+    
+    # uses displayed indexes
+    def hide_rows(self, rows = set(), redraw = True, deselect_all = True):
+        if isinstance(rows, int):
+            _rows = {rows}
+        elif isinstance(rows, set):
+            _rows = rows
+        else:
+            _rows = set(rows)
+        if not _rows:
+            return
+        if self.MT.all_rows_displayed:
+            _rows = [r for r in range(self.MT.total_data_rows()) if r not in _rows]
+        else:
+            _rows = [e for r, e in enumerate(self.MT.displayed_rows) if r not in _rows]
+        self.display_rows(rows = _rows,
+                          all_rows_displayed = False,
+                          redraw = redraw, 
+                          deselect_all = deselect_all)
     
-    def hide_columns(self, columns = set(), refresh = True, deselect_all = True):
+    # uses displayed indexes
+    def hide_columns(self, columns = set(), redraw = True, deselect_all = True):
         if isinstance(columns, int):
             _columns = {columns}
         elif isinstance(columns, set):
             _columns = columns
         else:
             _columns = set(columns)
-        self.display_columns(columns = [c for c in range(self.MT.total_data_cols()) if c not in _columns] if self.MT.all_columns_displayed else [c for c in self.MT.displayed_columns if c not in _columns],
+        if not _columns:
+            return
+        if self.MT.all_columns_displayed:
+            _columns = [c for c in range(self.MT.total_data_cols()) if c not in _columns]
+        else:
+            _columns = [e for c, e in enumerate(self.MT.displayed_columns) if c not in _columns]
+        self.display_columns(columns = _columns,
                              all_columns_displayed = False,
-                             refresh = refresh, 
+                             redraw = redraw, 
                              deselect_all = deselect_all)
 
     def show_ctrl_outline(self, canvas = "table", start_cell = (0, 0), end_cell = (1, 1)):
         self.MT.show_ctrl_outline(canvas = canvas, start_cell = start_cell, end_cell = end_cell)
 
     def get_ctrl_x_c_boxes(self):
         return self.MT.get_ctrl_x_c_boxes()
 
     def get_selected_min_max(self): # returns (min_y, min_x, max_y, max_x) of any selections including rows/columns
         return self.MT.get_selected_min_max()
         
     def headers(self, newheaders = None, index = None, reset_col_positions = False, show_headers_if_not_sheet = True, redraw = False):
-        return self.MT.headers(newheaders, index, reset_col_positions = reset_col_positions, show_headers_if_not_sheet = show_headers_if_not_sheet, redraw = redraw)
-        
+        self.set_refresh_timer(redraw)
+        return self.MT.headers(newheaders, index, reset_col_positions = reset_col_positions, show_headers_if_not_sheet = show_headers_if_not_sheet, redraw = False)
+
     def row_index(self, newindex = None, index = None, reset_row_positions = False, show_index_if_not_sheet = True, redraw = False):
-        return self.MT.row_index(newindex, index, reset_row_positions = reset_row_positions, show_index_if_not_sheet = show_index_if_not_sheet, redraw = redraw)
+        self.set_refresh_timer(redraw)
+        return self.MT.row_index(newindex, index, reset_row_positions = reset_row_positions, show_index_if_not_sheet = show_index_if_not_sheet, redraw = False)
 
     def reset_undos(self):
         self.MT.undo_storage = deque(maxlen = self.MT.max_undos)
 
     def redraw(self, redraw_header = True, redraw_row_index = True):
         self.MT.main_table_redraw_grid_and_text(redraw_header = redraw_header, redraw_row_index = redraw_row_index)
```

### Comparing `tksheet-6.0.0/tksheet/_tksheet_column_headers.py` & `tksheet-6.0.1/tksheet/_tksheet_column_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,15 +554,15 @@
                                                                                 sorted(orig_selected),  #4
                                                                                 dispset))))                  #5
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ch_extra_end_drag_drop_func is not None:
                         self.ch_extra_end_drag_drop_func(EndDragDropEvent("end_column_header_drag_drop", tuple(orig_selected), new_selected, int(c)))
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             c = self.MT.identify_col(x = event.x)
-            if c is not None and c == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
+            if c is not None and c < len(self.MT.col_positions) - 1 and c == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
                 datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
                 canvasx = self.canvasx(event.x)
                 if (event.y < self.MT.hdr_txt_h + 5 and
                     (
                      (datacn in self.cell_options and 
                       'dropdown' in self.cell_options[datacn] and 
                       canvasx < self.MT.col_positions[c + 1] and 
@@ -663,70 +663,70 @@
                 r1, c1, r2, c2 = tuple(int(e) for e in current[1].split("_") if e)
                 self.MT.create_selected(r1, c1, r2, c2, current[2] + "s")
         self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(("select_column", int(c)))
+            
+    def get_cell_dimensions(self, datacn):
+        txt = self.get_valid_cell_data_as_str(datacn, fix = False)
+        if txt:
+            self.MT.txt_measure_canvas.itemconfig(self.MT.txt_measure_canvas_text, text = txt, font = self.MT._hdr_font)
+            b = self.MT.txt_measure_canvas.bbox(self.MT.txt_measure_canvas_text)
+            w = b[2] - b[0] + 7
+            h = b[3] - b[1] + 5
+        else:
+            w = self.MT.min_cw
+            h = self.MT.hdr_min_rh
+        if datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 'checkbox' in self.cell_options[datacn]):
+            return w + self.MT.hdr_txt_h, h
+        return w, h
 
     def set_col_width(self, col, width = None, only_set_if_too_small = False, displayed_only = False, recreate = True, return_new_width = False):
         if col < 0:
             return
         qconf = self.MT.txt_measure_canvas.itemconfig
         qbbox = self.MT.txt_measure_canvas.bbox
         qtxtm = self.MT.txt_measure_canvas_text
         qtxth = self.MT.txt_h
         qclop = self.MT.cell_options
         qfont = self.MT._font
+        self.fix_header()
         if width is None:
             w = self.MT.min_cw
             hw = self.MT.min_cw
-            if displayed_only:
-                x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-                start_row, end_row = self.MT.get_visible_rows(y1, y2)
+            if self.MT.all_rows_displayed:
+                if displayed_only:
+                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
+                    start_row, end_row = self.MT.get_visible_rows(y1, y2)
+                else:
+                    start_row, end_row = 0, len(self.MT.data)
+                iterable = range(start_row, end_row)
             else:
-                start_row, end_row = 0, None
+                if displayed_only:
+                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
+                    start_row, end_row = self.MT.get_visible_rows(y1, y2)
+                else:
+                    start_row, end_row = 0, len(self.MT.displayed_rows)
+                iterable = self.MT.displayed_rows[start_row:end_row]
             datacn = col if self.MT.all_columns_displayed else self.MT.displayed_columns[col]
             # header
-            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
-                qconf(qtxtm, text = self.cell_options[datacn]['checkbox']['text'], font = self.MT._hdr_font)
-                b = qbbox(qtxtm)
-                hw = b[2] - b[0] + 7 + self.MT.hdr_txt_h
-            else:
-                txt = ""
-                if isinstance(self.MT._headers, int) or len(self.MT._headers) > datacn:
-                    txt = self.get_valid_cell_data_as_str(datacn, fix = False)
-                    if txt or (datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]):
-                        qconf(qtxtm, text = txt, font = self.MT._hdr_font)
-                        b = qbbox(qtxtm)
-                        if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
-                            hw = b[2] - b[0] + 7 + self.MT.hdr_txt_h
-                        else:
-                            hw = b[2] - b[0] + 7
-                if not isinstance(self.MT._headers, int) and ((not txt and self.show_default_header_for_empty) or len(self.MT._headers) < datacn):
-                    if self.default_header == "letters":
-                        hw = self.MT.GetHdrTextWidth(num2alpha(datacn)) + 7
-                    elif self.default_header == "numbers":
-                        hw = self.MT.GetHdrTextWidth(f"{datacn + 1}") + 7
-                    else:
-                        hw = self.MT.GetHdrTextWidth(f"{datacn + 1} {num2alpha(datacn)}") + 7
+            hw, hh_ = self.get_cell_dimensions(datacn)
             # table
-            for rn, r in enumerate(islice(self.MT.data, start_row, end_row), start_row):
-                if (rn, datacn) in qclop and 'checkbox' in qclop[(rn, datacn)]:
-                    qconf(qtxtm, text = qclop[(rn, datacn)]['checkbox']['text'], font = qfont)
-                    b = qbbox(qtxtm)
-                    tw = qtxth + 7 + b[2] - b[0]
-                    if tw > w:
-                        w = tw
-                else:
-                    txt = self.MT.get_valid_cell_data_as_str(rn, datacn, get_displayed = True)
+            if self.MT.data:
+                for datarn in iterable:
+                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
                     if txt:
                         qconf(qtxtm, text = txt, font = qfont)
                         b = qbbox(qtxtm)
-                        tw = b[2] - b[0] + qtxth + 7 if (rn, datacn) in qclop and 'dropdown' in qclop[(rn, datacn)] else b[2] - b[0] + 7
+                        if (datarn, datacn) in qclop and ('dropdown' in qclop[(datarn, datacn)] or 'checkbox' in qclop[(datarn, datacn)]):
+                            tw = b[2] - b[0] + qtxth + 7
+                        else:
+                            tw = b[2] - b[0] + 7
                         if tw > w:
                             w = tw
             if w > hw:
                 new_width = w
             else:
                 new_width = hw
         else:
@@ -908,15 +908,15 @@
                 else:
                     self.itemconfig(t, fill = fill, tag = tag, state = "normal")
                 self.lift(t)
             else:
                 t = self.create_line(points, fill = fill, width = 2, capstyle = tk.ROUND, joinstyle = tk.ROUND, tag = tag)
             self.disp_dropdown[t] = True
             
-    def redraw_checkbox(self, datacn, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
+    def redraw_checkbox(self, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
         points = self.MT.get_checkbox_points(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill = outline, outline = fill)
             else:
@@ -998,18 +998,15 @@
         c_2 = self.header_selected_cells_bg if self.header_selected_cells_bg.startswith("#") else Color_Map_[self.header_selected_cells_bg]
         c_3 = self.header_selected_columns_bg if self.header_selected_columns_bg.startswith("#") else Color_Map_[self.header_selected_columns_bg]
         font = self.MT._hdr_font
         for c in range(start_col, end_col - 1):
             draw_y = self.MT.hdr_fl_ins
             cleftgridln = self.MT.col_positions[c]
             crightgridln = self.MT.col_positions[c + 1]
-            if self.MT.all_columns_displayed:
-                datacn = c
-            else:
-                datacn = self.MT.displayed_columns[c]
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             fill, dd_drawn = self.redraw_highlight_get_text_fg(cleftgridln, crightgridln, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, datacn)
 
             if datacn in self.cell_options and 'align' in self.cell_options[datacn]:
                 align = self.cell_options[datacn]['align']
             else:
                 align = self.align
                 
@@ -1057,27 +1054,23 @@
                         mw -= 1
                     else:
                         mw -= 3
                     try:
                         draw_check = self.MT._headers[datacn] if isinstance(self.MT._headers, (list, tuple)) else self.MT.data[self.MT._headers][datacn]
                     except:
                         draw_check = False
-                    self.redraw_checkbox(datacn,
-                                         cleftgridln + 2,
+                    self.redraw_checkbox(cleftgridln + 2,
                                          2,
                                          cleftgridln + self.MT.hdr_txt_h + 3,
                                          self.MT.hdr_txt_h + 3,
                                          fill = fill if self.cell_options[datacn]['checkbox']['state'] == "normal" else self.header_grid_fg,
                                          outline = "",
                                          tag = "cb", 
                                          draw_check = draw_check)
-            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
-                lns = self.cell_options[datacn]['checkbox']['text'].split("\n") if isinstance(self.cell_options[datacn]['checkbox']['text'], str) else f"{self.cell_options[datacn]['checkbox']['text']}".split("\n")
-            else:
-                lns = self.get_valid_cell_data_as_str(datacn, fix = False).split("\n")
+            lns = self.get_valid_cell_data_as_str(datacn, fix = False).split("\n")
             if lns == [""]:
                 if self.show_default_header_for_empty:
                     lns = (get_n2a(datacn, self.default_header), )
                 else:
                     continue
             if mw > self.MT.hdr_txt_w and not ((align == "w" and (draw_x > x_stop)) or
                                                (align == "e" and (draw_x > x_stop)) or
@@ -1268,15 +1261,15 @@
         self.text_editor_loc = c
         x = self.MT.col_positions[c] + 1
         y = 0
         w = self.MT.col_positions[c + 1] - x
         h = self.current_height + 1
         datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         if text is None:
-            text = self.get_valid_cell_data_as_str(datacn)
+            text = self.get_cell_data(datacn)
         bg, fg = self.header_bg, self.header_fg
         self.text_editor = TextEditor(self,
                                       text = text,
                                       font = self.MT._hdr_font,
                                       state = state,
                                       width = w,
                                       height = h,
@@ -1450,15 +1443,15 @@
     
     def set_cell_data(self, datacn = None, value = ""):
         if isinstance(self.MT._headers, int):
             self.MT.set_cell_data(datarn = self.MT._headers, datacn = datacn, value = value)
         else:
             self.fix_header(datacn)
             if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
-                self.MT._headers[datacn] = to_bool(value)
+                self.MT._headers[datacn] = try_to_bool(value)
             else:
                 self.MT._headers[datacn] = value
     
     def input_valid_for_cell(self, datacn, value):
         if datacn in self.cell_options:
             if 'readonly' in self.cell_options[datacn]:
                 return False
@@ -1472,44 +1465,45 @@
             value not in self.cell_options[datacn]['dropdown']['values']):
             return False
         return True
     
     def cell_equal_to(self, datacn, value):
         self.fix_header(datacn)
         if isinstance(self.MT._headers, list):
-            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
-                try:
-                    return to_bool(self.MT._headers[datacn]) == to_bool(value)
-                except:
-                    return False
             return self.MT._headers[datacn] == value
         elif isinstance(self.MT._headers, int):
             return self.MT.cell_equal_to(self.MT._headers, datacn, value)
             
     def get_cell_data(self, datacn, get_displayed = False, redirect_int = False):
-        if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn] and self.cell_options[datacn]['dropdown']['text'] is not None and get_displayed:
-            return self.cell_options[datacn]['dropdown']['text']
+        if get_displayed and datacn in self.cell_options:
+            if 'dropdown' in self.cell_options[datacn] and self.cell_options[datacn]['dropdown']['text'] is not None:
+                return self.cell_options[datacn]['dropdown']['text']
+            if 'checkbox' in self.cell_options[datacn]:
+                return self.cell_options[datacn]['checkbox']['text']
         if redirect_int and isinstance(self.MT._headers, int):
             return self.MT.get_cell_data(self.MT._headers, datacn, none_to_empty_str = True)
         if isinstance(self.MT._headers, int) or not self.MT._headers or datacn >= len(self.MT._headers) or not self.MT._headers[datacn]:
             if get_displayed and self.show_default_header_for_empty:
                 return get_n2a(datacn, self.default_header)
             else:
                 return ""
-        return self.MT._headers[datacn]
+        return "" if self.MT._headers[datacn] is None and get_displayed else self.MT._headers[datacn]
             
     def get_valid_cell_data_as_str(self, datacn, fix = True) -> str:
-        if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn] and self.cell_options[datacn]['dropdown']['text'] is not None:
-            return f"{self.cell_options[datacn]['dropdown']['text']}"
+        if datacn in self.cell_options:
+            if 'dropdown' in self.cell_options[datacn] and self.cell_options[datacn]['dropdown']['text'] is not None:
+                return f"{self.cell_options[datacn]['dropdown']['text']}"
+            if 'checkbox' in self.cell_options[datacn]:
+                return f"{self.cell_options[datacn]['checkbox']['text']}"
         if isinstance(self.MT._headers, int):
             return self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed = True)
         if fix:
             self.fix_header(datacn)
         try:
-            return f"{self.MT._headers[datacn]}"
+            return "" if self.MT._headers[datacn] is None else f"{self.MT._headers[datacn]}"
         except:
             return ""
             
     def fix_header(self, datacn = None):
         if isinstance(self.MT._headers, int):
             return
         if isinstance(self.MT._headers, float):
@@ -1558,46 +1552,45 @@
         if redraw:
             self.MT.refresh()
 
     def create_checkbox(self, datacn = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
         if datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 
                                             'checkbox' in self.cell_options[datacn]):
             self.delete_dropdown_and_checkbox(datacn)
-        self.set_cell_data(datacn = datacn,
-                            value = checked)
         if datacn not in self.cell_options:
             self.cell_options[datacn] = {}
         self.cell_options[datacn]['checkbox'] = {'check_function': check_function,
                                                  'state': state,
                                                  'text': text}
+        self.set_cell_data(datacn = datacn, value = checked)
         if redraw:
             self.MT.refresh()
 
     def create_dropdown(self, 
                         datacn = 0, 
                         values = [], set_value = None, 
                         state = "normal", redraw = True, 
                         selection_function = None, modified_function = None,
                         search_function = dropdown_search_function, validate_input = True, text = None):
         if datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 
                                             'checkbox' in self.cell_options[datacn]):
             self.delete_dropdown_and_checkbox(datacn)
-        self.set_cell_data(datacn = datacn, 
-                            value = set_value if set_value is not None else values[0] if values else "")
         if datacn not in self.cell_options:
             self.cell_options[datacn] = {}
         self.cell_options[datacn]['dropdown'] = {'values': values,
                                                  'window': "no dropdown open",
                                                  'canvas_id': "no dropdown open",
                                                  'select_function': selection_function,
                                                  'modified_function': modified_function,
                                                  'search_function': search_function,
                                                  'validate_input': validate_input,
                                                  'text': text,
                                                  'state': state}
+        self.set_cell_data(datacn = datacn, 
+                           value = set_value if set_value is not None else values[0] if values else "")
         if redraw:
             self.MT.refresh()
 
     def get_dropdown_height_anchor(self, datacn, text_editor_h = None):
         win_h = 5
         for i, v in enumerate(self.cell_options[datacn]['dropdown']['values']):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
```

### Comparing `tksheet-6.0.0/tksheet/_tksheet_formatters.py` & `tksheet-6.0.1/tksheet/_tksheet_formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,20 @@
         _falsy = falsy
     if v in _truthy:
         return True
     elif v in _falsy:
         return False
     raise ValueError(f'Cannot map "{val}" to bool.')
 
+def try_to_bool(val: Any, **kwargs):
+    try:
+        return to_bool(val)
+    except:
+        return val
+
 def is_bool_like(v: Any, **kwargs):
     try:
         to_bool(v)
         return True
     except:
         return False
 
@@ -60,22 +66,23 @@
         if 'decimals' in kwargs and isinstance(kwargs['decimals'], int):
             if kwargs['decimals']:
                 return f"{round(v, kwargs['decimals'])}"
             return f"{int(round(v, kwargs['decimals']))}"
     return f"{v}"
 
 def percentage_to_str(v: Union[int, float], **kwargs: dict) -> str:
-    x = v * 100
-    if isinstance(x, float):
-        if x.is_integer():
-            return f"{int(x)}%"
-        if 'decimals' in kwargs and isinstance(kwargs['decimals'], int):
-            if kwargs['decimals']:
-                return f"{round(x, kwargs['decimals'])}%"
-            return f"{int(round(x, kwargs['decimals']))}%"
+    if isinstance(v, (int, float)):
+        x = v * 100
+        if isinstance(x, float):
+            if x.is_integer():
+                return f"{int(x)}%"
+            if 'decimals' in kwargs and isinstance(kwargs['decimals'], int):
+                if kwargs['decimals']:
+                    return f"{round(x, kwargs['decimals'])}%"
+                return f"{int(round(x, kwargs['decimals']))}%"
     return f"{x}%"
 
 def bool_to_str(v: Any, **kwargs: dict) -> str:
     return f"{v}"
 
 def int_formatter(datatypes = int,
                   format_function = to_int,
@@ -158,15 +165,15 @@
         value = pre_format_function(value)
     if nullable and is_none_like(value):
         value = None
     else:
         try:
             value = format_function(value, **kwargs)
         except Exception as e:
-            value = f"{value}"
+            pass
     if post_format_function and isinstance(value, datatypes):
         value = post_format_function(value)
     return value
 
 def data_to_str(value = "",
                 datatypes = int,
                 nullable = True,
```

### Comparing `tksheet-6.0.0/tksheet/_tksheet_main_table.py` & `tksheet-6.0.1/tksheet/_tksheet_main_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,14 +236,18 @@
                 self._row_index = _row_index
             else:
                 self._row_index = []
         self.displayed_columns = []
         self.displayed_rows = []
         self.col_positions = [0]
         self.row_positions = [0]
+        self.display_rows(rows = kwargs['displayed_rows'],
+                          all_rows_displayed = kwargs['all_rows_displayed'],
+                          reset_row_positions = False,
+                          deselect_all = False)
         self.reset_row_positions()
         self.display_columns(columns = kwargs['displayed_columns'],
                              all_columns_displayed = kwargs['all_columns_displayed'],
                              reset_col_positions = False,
                              deselect_all = False)
         self.reset_col_positions()
         self.table_grid_fg = kwargs['table_grid_fg']
@@ -391,34 +395,34 @@
                     except:
                         return
                 for rn in range(maxrows):
                     row = []
                     for r1, c1, r2, c2 in boxes:
                         if r2 - r1 < maxrows:
                             continue
-                        data_ref_rn = r1 + rn
+                        datarn = (r1 if self.all_rows_displayed else self.displayed_rows[r1]) + rn
                         for c in range(c1, c2):
                             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                            row.append(self.get_cell_clipboard(data_ref_rn, datacn))
+                            row.append(self.get_cell_clipboard(datarn, datacn))
                     writer.writerow(row)
                     rows.append(row)
             else:
                 boxes = self.get_ctrl_x_c_boxes()
                 if self.extra_begin_ctrl_c_func is not None:
                     try:
                         self.extra_begin_ctrl_c_func(CtrlKeyEvent("begin_ctrl_c", boxes, currently_selected, tuple()))
                     except:
                         return
                 for r1, c1, r2, c2 in boxes:
                     for rn in range(r2 - r1):
                         row = []
-                        data_ref_rn = r1 + rn
+                        datarn = (r1 if self.all_rows_displayed else self.displayed_rows[r1]) + rn
                         for c in range(c1, c2):
                             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                            row.append(self.get_cell_clipboard(data_ref_rn, datacn))
+                            row.append(self.get_cell_clipboard(datarn, datacn))
                         writer.writerow(row)
                         rows.append(row)
             for r1, c1, r2, c2 in boxes:
                 self.show_ctrl_outline(canvas = "table", start_cell = (c1, r1), end_cell = (c2, r2))
             self.clipboard_clear()
             self.clipboard_append(s.getvalue())
             self.update_idletasks()
@@ -446,57 +450,57 @@
                 except:
                     return
             for rn in range(maxrows):
                 row = []
                 for r1, c1, r2, c2 in boxes:
                     if r2 - r1 < maxrows:
                         continue
-                    data_ref_rn = r1 + rn
+                    datarn = (r1 if self.all_rows_displayed else self.displayed_rows[r1]) + rn
                     for c in range(c1, c2):
                         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                        row.append(self.get_cell_clipboard(data_ref_rn, datacn))
+                        row.append(self.get_cell_clipboard(datarn, datacn))
                 writer.writerow(row)
                 rows.append(row)
             for rn in range(maxrows):
                 for r1, c1, r2, c2 in boxes:
                     if r2 - r1 < maxrows:
                         continue
-                    data_ref_rn = r1 + rn
+                    datarn = (r1 if self.all_rows_displayed else self.displayed_rows[r1]) + rn
                     for c in range(c1, c2):
                         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                        if self.input_valid_for_cell(data_ref_rn, datacn, ""):
+                        if self.input_valid_for_cell(datarn, datacn, ""):
                             if self.undo_enabled:
-                                undo_storage[(data_ref_rn, datacn)] = self.get_cell_data(data_ref_rn, datacn)
-                            self.set_cell_data(data_ref_rn, datacn, "")
+                                undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
+                            self.set_cell_data(datarn, datacn, "")
                             changes += 1
         else:
             boxes = self.get_ctrl_x_c_boxes()
             if self.extra_begin_ctrl_x_func is not None:
                 try:
                     self.extra_begin_ctrl_x_func(CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple()))
                 except:
                     return
             for r1, c1, r2, c2 in boxes:
                 for rn in range(r2 - r1):
                     row = []
-                    data_ref_rn = r1 + rn
+                    datarn = (r1 if self.all_rows_displayed else self.displayed_rows[r1]) + rn
                     for c in range(c1, c2):
                         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                        row.append(self.get_cell_data(data_ref_rn, datacn))
+                        row.append(self.get_cell_data(datarn, datacn))
                     writer.writerow(row)
                     rows.append(row)
             for r1, c1, r2, c2 in boxes:
                 for rn in range(r2 - r1):
-                    data_ref_rn = r1 + rn
+                    datarn = (r1 if self.all_rows_displayed else self.displayed_rows[r1]) + rn
                     for c in range(c1, c2):
                         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                        if self.input_valid_for_cell(data_ref_rn, datacn, ""):
+                        if self.input_valid_for_cell(datarn, datacn, ""):
                             if self.undo_enabled:
-                                undo_storage[(data_ref_rn, datacn)] = self.get_cell_data(data_ref_rn, datacn)
-                            self.set_cell_data(data_ref_rn, datacn, "")
+                                undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
+                            self.set_cell_data(datarn, datacn, "")
                             changes += 1
         if changes and self.undo_enabled:
             self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, tuple(boxes.items()), currently_selected))))
         self.clipboard_clear()
         self.clipboard_append(s.getvalue())
         self.update_idletasks()
         self.refresh()
@@ -586,14 +590,17 @@
                     self.displayed_columns.extend(list(range(total_data_cols, total_data_cols + added_cols)))
             if selected_r + numrows > len(self.row_positions) - 1:
                 added_rows = selected_r + numrows - len(self.row_positions) + 1
                 if isinstance(self.paste_insert_row_limit, int) and self.paste_insert_row_limit < len(self.row_positions) - 1 + added_rows:
                     added_rows = self.paste_insert_row_limit - len(self.row_positions) - 1
                 if added_rows > 0:
                     self.insert_row_positions(heights = int(added_rows))
+                if not self.all_rows_displayed:
+                    total_data_rows = self.total_data_rows()
+                    self.displayed_rows.extend(list(range(total_data_rows, total_data_rows + added_rows)))
             added_rows_cols = (added_rows, added_cols)
         else:
             added_rows_cols = (0, 0)
         if selected_c + numcols > len(self.col_positions) - 1:
             numcols = len(self.col_positions) - 1 - selected_c
         if selected_r + numrows > len(self.row_positions) - 1:
             numrows = len(self.row_positions) - 1 - selected_r
@@ -834,64 +841,118 @@
             else:
                 new_selected = tuple(range(r + 1 - num_rows, r + 1))
                 if create_selections:
                     self.create_selected(r + 1 - num_rows, 0, r + 1, len(self.col_positions) - 1, "rows")
         if create_selections:
             self.create_current(int(new_selected[0]), 0, type_ = "row", inside = True)
         newrowsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
-        if to_move_min > r:
-            if move_data:
-                self.data[r:r] = self.data[to_move_min:to_move_max]
-                self.data[to_move_max:to_del] = []
-                if isinstance(self._row_index, list) and self._row_index:
-                    if len(self._row_index) < to_move_max:
-                        self._row_index.extend(list(repeat("", to_move_max - len(self._row_index) + 1)))
-                    self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
-                    self._row_index[to_move_max:to_del] = []
-            self.RI.cell_options = {
-                newrowsdct[k] if k in newrowsdct else
-                k + num_rows if k < to_move_min and k >= r else
-                k: v for k, v in self.RI.cell_options.items()
-            }
-            self.cell_options = {
-                (newrowsdct[k[0]], k[1]) if k[0] in newrowsdct else
-                (k[0] + num_rows, k[1]) if k[0] < to_move_min and k[0] >= r else
-                k: v for k, v in self.cell_options.items()
-            }
-            self.row_options = {
-                newrowsdct[k] if k in newrowsdct else
-                k + num_rows if k < to_move_min and k >= r else
-                k: v for k, v in self.row_options.items()
-            }
+        if self.all_rows_displayed:
+            dispset = {}
+            if to_move_min > r:
+                if move_data:
+                    self.data[r:r] = self.data[to_move_min:to_move_max]
+                    self.data[to_move_max:to_del] = []
+                    if isinstance(self._row_index, list) and self._row_index:
+                        if len(self._row_index) < to_move_max:
+                            self._row_index.extend(list(repeat("", to_move_max - len(self._row_index) + 1)))
+                        self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
+                        self._row_index[to_move_max:to_del] = []
+                self.RI.cell_options = {
+                    newrowsdct[k] if k in newrowsdct else
+                    k + num_rows if k < to_move_min and k >= r else
+                    k: v for k, v in self.RI.cell_options.items()
+                }
+                self.cell_options = {
+                    (newrowsdct[k[0]], k[1]) if k[0] in newrowsdct else
+                    (k[0] + num_rows, k[1]) if k[0] < to_move_min and k[0] >= r else
+                    k: v for k, v in self.cell_options.items()
+                }
+                self.row_options = {
+                    newrowsdct[k] if k in newrowsdct else
+                    k + num_rows if k < to_move_min and k >= r else
+                    k: v for k, v in self.row_options.items()
+                }
+            else:
+                r += 1
+                if move_data:
+                    self.data[r:r] = self.data[to_move_min:to_move_max]
+                    self.data[to_move_min:to_move_max] = []
+                    if isinstance(self._row_index, list) and self._row_index:
+                        if len(self._row_index) < r:
+                            self._row_index.extend(list(repeat("", r - len(self._row_index))))
+                        self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
+                        self._row_index[to_move_min:to_move_max] = []
+                self.RI.cell_options = {
+                    newrowsdct[k] if k in newrowsdct else
+                    k - num_rows if k < r and k > to_move_min else
+                    k: v for k, v in self.RI.cell_options.items()
+                }
+                self.cell_options = {
+                    (newrowsdct[k[0]], k[1]) if k[0] in newrowsdct else 
+                    (k[0] - num_rows, k[1]) if k[0] < r and k[0] > to_move_min else 
+                    k: v for k, v in self.cell_options.items()
+                }
+                self.row_options = {
+                    newrowsdct[k] if k in newrowsdct else
+                    k - num_rows if k < r and k > to_move_min else
+                    k: v for k, v in self.row_options.items()
+                }
         else:
-            r += 1
+            # moves data around, not displayed rows indexes
+            # which remain sorted and the same after drop and drop
+            if to_move_min > r:
+                dispset = {a: b for a, b in zip(self.displayed_rows, (self.displayed_rows[:r] +
+                                                                      self.displayed_rows[to_move_min:to_move_min + num_rows] +
+                                                                      self.displayed_rows[r:to_move_min] +
+                                                                      self.displayed_rows[to_move_min + num_rows:]))}
+            else:
+                dispset = {a: b for a, b in zip(self.displayed_rows, (self.displayed_rows[:to_move_min] +
+                                                                      self.displayed_rows[to_move_min + num_rows:r + 1] +
+                                                                      self.displayed_rows[to_move_min:to_move_min + num_rows] +
+                                                                      self.displayed_rows[r + 1:]))}
+            # has to pick up rows from all over the place in the original sheet
+            # building an entirely new sheet is best due to permutations of hidden rows
             if move_data:
-                self.data[r:r] = self.data[to_move_min:to_move_max]
-                self.data[to_move_min:to_move_max] = []
+                max_idx = max(chain(dispset, dispset.values())) + 1
+                if len(self.data) < max_idx:
+                    self.data[:] = self.data + list(repeat("", max_idx - len(self.data)))
+                new = []
+                idx = 0
+                done = set()
+                while len(new) < len(self.data):
+                    if idx in dispset and idx not in done:
+                        new.append(self.data[dispset[idx]])
+                        done.add(idx)
+                    elif idx not in done:
+                        new.append(self.data[idx])
+                        idx += 1
+                    else:
+                        idx += 1
+                self.data = new
                 if isinstance(self._row_index, list) and self._row_index:
-                    if len(self._row_index) < r:
-                        self._row_index.extend(list(repeat("", r - len(self._row_index))))
-                    self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
-                    self._row_index[to_move_min:to_move_max] = []
-            self.RI.cell_options = {
-                newrowsdct[k] if k in newrowsdct else
-                k - num_rows if k < r and k > to_move_min else
-                k: v for k, v in self.RI.cell_options.items()
-            }
-            self.cell_options = {
-                (newrowsdct[k[0]], k[1]) if k[0] in newrowsdct else 
-                (k[0] - num_rows, k[1]) if k[0] < r and k[0] > to_move_min else 
-                k: v for k, v in self.cell_options.items()
-            }
-            self.row_options = {
-                newrowsdct[k] if k in newrowsdct else
-                k - num_rows if k < r and k > to_move_min else
-                k: v for k, v in self.row_options.items()
-            }
-        return new_selected, {}
+                    if len(self._row_index) < max_idx:
+                        self._row_index[:] = self._row_index + list(repeat("", max_idx - len(self._row_index)))
+                    new = []
+                    idx = 0
+                    done = set()
+                    while len(new) < len(self._row_index):
+                        if idx in dispset and idx not in done:
+                            new.append(self._row_index[dispset[idx]])
+                            done.add(idx)
+                        elif idx not in done:
+                            new.append(self._row_index[idx])
+                            idx += 1
+                        else:
+                            idx += 1
+                    self._row_index = new
+            dispset = {b: a for a, b in dispset.items()}
+            self.RI.cell_options = {dispset[k] if k in dispset else k: v for k, v in self.RI.cell_options.items()}
+            self.cell_options = {(dispset[k[0]], k[1]) if k[0] in dispset else k: v for k, v in self.cell_options.items()}
+            self.row_options = {dispset[k] if k in dispset else k: v for k, v in self.row_options.items()}
+        return new_selected, dispset
 
     def ctrl_z(self, event = None):
         if not self.undo_storage:
             return
         if not isinstance(self.undo_storage[-1], (tuple, dict)):
             undo_storage = pickle.loads(zlib.decompress(self.undo_storage[-1]))
         else:
@@ -971,14 +1032,15 @@
             to_move_min = undo_storage[2]
             totalrows = len(undo_storage[4])
             if to_move_min < r:
                 r += totalrows - 1
             self.move_rows_adjust_options_dict(r, to_move_min, totalrows)
                     
         elif undo_storage[0] == "insert_row":
+            self.displayed_rows = undo_storage[1]['displayed_rows']
             self.data[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
             try:
                 self._row_index[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
             except:
                 pass
             self.del_row_positions(undo_storage[1]['sheet_row_num'],
                                     undo_storage[1]['numrows'],
@@ -1025,16 +1087,18 @@
             self.CH.cell_options = {cn if cn < idx else cn - numcols: t for cn, t in self.CH.cell_options.items()}
             if len(self.col_positions) > 1:
                 start_col = undo_storage[1]['sheet_col_num'] if undo_storage[1]['sheet_col_num'] < len(self.col_positions) - 1 else undo_storage[1]['sheet_col_num'] - 1
                 self.CH.select_col(start_col)
                 self.see(r = 0, c = start_col, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
                 
         elif undo_storage[0] == "delete_rows":
-            for rn, r, h in reversed(undo_storage[1]['deleted_rows']):
+            self.displayed_rows = undo_storage[1]['displayed_rows']
+            for rn, r in reversed(undo_storage[1]['deleted_rows']):
                 self.data.insert(rn, r)
+            for rn, h in reversed(tuple(undo_storage[1]['rowheights'].items())):
                 self.insert_row_position(idx = rn, height = h)
             self.cell_options = undo_storage[1]['cell_options']
             self.row_options = undo_storage[1]['row_options']
             self.RI.cell_options = undo_storage[1]['RI_cell_options']
             for rn, r in reversed(undo_storage[1]['deleted_index_values']):
                 try:
                     self._row_index.insert(rn, r)
@@ -2621,24 +2685,25 @@
             self.b1_pressed_loc = None
         self.RI.rsz_w = None
         self.CH.rsz_h = None
         if self.b1_pressed_loc is not None:
             r = self.identify_row(y = event.y, allow_end = False)
             c = self.identify_col(x = event.x, allow_end = False)
             if r is not None and c is not None and (r, c) == self.b1_pressed_loc:
+                datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                 datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                if (r, datacn) in self.cell_options and ('dropdown' in self.cell_options[(r, datacn)] or 'checkbox' in self.cell_options[(r, datacn)]):
+                if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 'checkbox' in self.cell_options[(datarn, datacn)]):
                     canvasx = self.canvasx(event.x)
                     if (
                         (self.closed_dropdown != self.b1_pressed_loc and
-                         'dropdown' in self.cell_options[(r, datacn)] and
+                         'dropdown' in self.cell_options[(datarn, datacn)] and
                          canvasx > self.col_positions[c + 1] - self.txt_h - 5 and
                          canvasx < self.col_positions[c + 1] - 1) 
                         or
-                        ('checkbox' in self.cell_options[(r, datacn)] and 
+                        ('checkbox' in self.cell_options[(datarn, datacn)] and 
                          canvasx < self.col_positions[c] + self.txt_h + 5 and
                          self.canvasy(event.y) < self.row_positions[r] + self.txt_h + 5)
                         ):
                         self.open_cell(event)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.b1_pressed_loc = None
@@ -2930,52 +2995,38 @@
                 self.reset_row_positions()
             if redraw:
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if return_id:
             return id(self.data)
         else:
             return self.data
-
-    def set_cell_size_to_text(self, r, c, only_set_if_too_small = False, redraw = True, run_binding = False):
-        min_cw = self.min_cw
-        min_rh = self.min_rh
-        h = int(min_rh)
-        w = int(min_cw)
-        if self.all_columns_displayed:
-            cn = int(c)
-        else:
-            cn = self.displayed_columns[c]
-        rn = int(r)
-        if (rn, cn) in self.cell_options and 'checkbox' in self.cell_options[(rn, cn)]:
-            self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, 
-                                               text = self.cell_options[(rn, cn)]['checkbox']['text'],
-                                               font = self._hdr_font)
+        
+    def get_cell_dimensions(self, datarn, datacn):
+        txt = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
+        if txt:
+            self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self._font)
             b = self.txt_measure_canvas.bbox(self.txt_measure_canvas_text)
-            tw = b[2] - b[0] + 7 + self.txt_h
-            if b[3] - b[1] + 5 > h:
-                h = b[3] - b[1] + 5
+            w = b[2] - b[0] + 7
+            h = b[3] - b[1] + 5
         else:
-            try:
-                if isinstance(self.data[r][cn], str):
-                    txt = self.data[r][cn]
-                else:
-                    txt = f"{self.data[r][cn]}"
-            except:
-                txt = ""
-            if txt:
-                self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self._font)
-                b = self.txt_measure_canvas.bbox(self.txt_measure_canvas_text)
-                tw = b[2] - b[0] + self.txt_h + 7 if (rn, cn) in self.cell_options and 'dropdown' in self.cell_options[(rn, cn)] else b[2] - b[0] + 7
-                if b[3] - b[1] + 5 > h:
-                    h = b[3] - b[1] + 5
-            else:
-                if (rn, cn) in self.cell_options and 'dropdown' in self.cell_options[(rn, cn)]:
-                    tw = self.txt_h + 7
-                else:
-                    tw = min_cw
+            w = self.min_cw
+            h = self.min_rh
+        if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
+                                                      'checkbox' in self.cell_options[(datarn, datacn)]):
+            return w + self.txt_h, h
+        return w, h
+
+    def set_cell_size_to_text(self, r, c, only_set_if_too_small = False, redraw = True, run_binding = False):
+        min_cw = int(self.min_cw)
+        min_rh = int(self.min_rh)
+        w = min_cw
+        h = min_rh
+        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+        datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+        tw, h = self.get_cell_dimensions(datarn, datacn)
         if tw > w:
             w = tw
         if h < min_rh:
             h = int(min_rh)
         elif h > self.RI.max_rh:
             h = int(self.RI.max_rh)
         if w < min_cw:
@@ -3017,115 +3068,67 @@
             if redraw:
                 self.refresh()
                 return True
             else:
                 return False
 
     def set_all_cell_sizes_to_text(self, include_index = False):
-        min_cw = self.min_cw
-        min_rh = self.min_rh
+        min_cw = int(self.min_cw)
+        min_rh = int(self.min_rh)
+        w = min_cw
+        h = min_rh
         rhs = defaultdict(lambda: int(min_rh))
         cws = []
         x = self.txt_measure_canvas.create_text(0, 0, text = "", font = self._font)
         x2 = self.txt_measure_canvas.create_text(0, 0, text = "", font = self._hdr_font)
         itmcon = self.txt_measure_canvas.itemconfig
         itmbbx = self.txt_measure_canvas.bbox
         if self.all_columns_displayed:
-            iterable = range(self.total_data_cols())
+            itercols = range(self.total_data_cols())
         else:
-            iterable = self.displayed_columns
-        if isinstance(self._row_index, list):
-            for rn in range(self.total_data_rows()):
-                if rn in self.RI.cell_options and 'checkbox' in self.RI.cell_options[rn]:
-                    txt = self.RI.cell_options[rn]['checkbox']['text']
-                else:
-                    try:
-                        if isinstance(self._row_index[rn], str):
-                            txt = self._row_index[rn]
-                        else:
-                            txt = f"{self._row_index[rn]}"
-                    except:
-                        txt = ""
-                if txt:
-                    itmcon(x, text = txt)
-                    b = itmbbx(x)
-                    h = b[3] - b[1] + 7
-                else:
-                    h = min_rh
+            itercols = self.displayed_columns
+        if self.all_rows_displayed:
+            iterrows = range(self.total_data_rows())
+        else:
+            iterrows = self.displayed_rows
+        if is_iterable(self._row_index):
+            for datarn in iterrows:
+                w_, h = self.RI.get_cell_dimensions(datarn)
                 if h < min_rh:
                     h = int(min_rh)
                 elif h > self.RI.max_rh:
                     h = int(self.RI.max_rh)
-                if h > rhs[rn]:
-                    rhs[rn] = h
-        for cn in iterable:
-            if cn in self.CH.cell_options and 'checkbox' in self.CH.cell_options[cn]:
-                txt = self.CH.cell_options[cn]['checkbox']['text']
+                if h > rhs[datarn]:
+                    rhs[datarn] = h
+        for datacn in itercols:
+            w, h_ = self.CH.get_cell_dimensions(datacn)
+            if self.all_rows_displayed:
+                # refresh range generator if needed
+                iterrows = range(self.total_data_rows())
+            for datarn in iterrows:
+                txt = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
                 if txt:
-                    itmcon(x2, text = txt)
-                    b = itmbbx(x2)
-                    w = b[2] - b[0] + 7 + self.hdr_txt_h
-                else:
-                    w = self.min_cw
-            else:
-                try:
-                    if isinstance(self._headers, int):
-                        txt = self.data[self._headers][cn]
-                    else:
-                        txt = self._headers[cn]
-                    if txt:
-                        itmcon(x2, text = txt)
-                        b = itmbbx(x2)
-                        w = b[2] - b[0] + self.hdr_txt_h + 7 if cn in self.CH.cell_options and 'dropdown' in self.CH.cell_options[cn] else b[2] - b[0] + 7
-                    else:
-                        w = self.min_cw + self.hdr_txt_h + 7 if cn in self.CH.cell_options and 'dropdown' in self.CH.cell_options[cn] else self.min_cw
-                except:
-                    if self.CH.default_header == "letters":
-                        itmcon(x2, text = f"{num2alpha(cn)}")
-                    elif self.CH.default_header == "numbers":
-                        itmcon(x2, text = f"{cn + 1}")
-                    else:
-                        itmcon(x2, text = f"{cn + 1} {num2alpha(cn)}")
-                    b = itmbbx(x2)
-                    w = b[2] - b[0] + 7
-            for rn, r in enumerate(self.data):
-                if (rn, cn) in self.cell_options and 'checkbox' in self.cell_options[(rn, cn)]:
-                    txt = self.cell_options[(rn, cn)]['checkbox']['text']
-                    if txt:
-                        itmcon(x, text = txt)
-                        b = itmbbx(x)
-                        tw = b[2] - b[0] + 7
-                        h = b[3] - b[1] + 5
-                    else:
-                        tw = min_cw
-                        h = min_rh
+                    itmcon(x, text = txt)
+                    b = itmbbx(x)
+                    tw = b[2] - b[0] + 7
+                    h = b[3] - b[1] + 5
                 else:
-                    try:
-                        if isinstance(r[cn], str):
-                            txt = r[cn]
-                        else:
-                            txt = f"{r[cn]}"
-                    except:
-                        txt = ""
-                    if txt:
-                        itmcon(x, text = txt)
-                        b = itmbbx(x)
-                        tw = b[2] - b[0] + self.txt_h + 7 if (rn, cn) in self.cell_options and 'dropdown' in self.cell_options[(rn, cn)] else b[2] - b[0] + 7
-                        h = b[3] - b[1] + 5
-                    else:
-                        tw = self.txt_h + 7 if (rn, cn) in self.cell_options and 'dropdown' in self.cell_options[(rn, cn)] else min_cw
-                        h = min_rh
+                    tw = min_cw
+                    h = min_rh
+                if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
+                                                              'checkbox' in self.cell_options[(datarn, datacn)]):
+                    tw += self.txt_h
                 if tw > w:
                     w = tw
                 if h < min_rh:
                     h = int(min_rh)
                 elif h > self.RI.max_rh:
                     h = int(self.RI.max_rh)
-                if h > rhs[rn]:
-                    rhs[rn] = h
+                if h > rhs[datarn]:
+                    rhs[datarn] = h
             if w < min_cw:
                 w = int(min_cw)
             elif w > self.CH.max_cw:
                 w = int(self.CH.max_cw)
             cws.append(w)
         self.txt_measure_canvas.delete(x)
         self.txt_measure_canvas.delete(x2)
@@ -3136,50 +3139,93 @@
 
     def reset_col_positions(self, ncols = None):
         colpos = int(self.default_cw)
         if self.all_columns_displayed:
             self.col_positions = list(accumulate(chain([0], (colpos for c in range(ncols if ncols is not None else self.total_data_cols())))))
         else:
             self.col_positions = list(accumulate(chain([0], (colpos for c in range(ncols if ncols is not None else len(self.displayed_columns))))))
+            
+    def reset_row_positions(self, nrows = None):
+        rowpos = self.default_rh[1]
+        if self.all_rows_displayed:
+            self.row_positions = list(accumulate(chain([0], (rowpos for r in range(nrows if nrows is not None else self.total_data_rows())))))
+        else:
+            self.row_positions = list(accumulate(chain([0], (rowpos for r in range(nrows if nrows is not None else len(self.displayed_rows))))))
 
     def del_col_position(self, idx, deselect_all = False):
         if deselect_all:
             self.deselect("all", redraw = False)
         if idx == "end" or len(self.col_positions) <= idx + 1:
             del self.col_positions[-1]
         else:
             w = self.col_positions[idx + 1] - self.col_positions[idx]
             idx += 1
             del self.col_positions[idx]
             self.col_positions[idx:] = [e - w for e in islice(self.col_positions, idx, len(self.col_positions))]
+            
+    def del_row_position(self, idx, deselect_all = False):
+        if deselect_all:
+            self.deselect("all", redraw = False)
+        if idx == "end" or len(self.row_positions) <= idx + 1:
+            del self.row_positions[-1]
+        else:
+            w = self.row_positions[idx + 1] - self.row_positions[idx]
+            idx += 1
+            del self.row_positions[idx]
+            self.row_positions[idx:] = [e - w for e in islice(self.row_positions, idx, len(self.row_positions))]
 
     def del_col_positions(self, idx, num = 1, deselect_all = False):
         if deselect_all:
             self.deselect("all", redraw = False)
         if idx == "end" or len(self.col_positions) <= idx + 1:
             del self.col_positions[-1]
         else:
             cws = [int(b - a) for a, b in zip(self.col_positions, islice(self.col_positions, 1, len(self.col_positions)))]
             cws[idx:idx + num] = []
             self.col_positions = list(accumulate(chain([0], (width for width in cws))))
 
+    def del_row_positions(self, idx, numrows = 1, deselect_all = False):
+        if deselect_all:
+            self.deselect("all", redraw = False)
+        if idx == "end" or len(self.row_positions) <= idx + 1:
+            del self.row_positions[-1]
+        else:
+            rhs = [int(b - a) for a, b in zip(self.row_positions, islice(self.row_positions, 1, len(self.row_positions)))]
+            rhs[idx:idx + numrows] = []
+            self.row_positions = list(accumulate(chain([0], (height for height in rhs))))
+
     def insert_col_position(self, idx = "end", width = None, deselect_all = False):
         if deselect_all:
             self.deselect("all", redraw = False)
         if width is None:
             w = self.default_cw
         else:
             w = width
         if idx == "end" or len(self.col_positions) == idx + 1:
             self.col_positions.append(self.col_positions[-1] + w)
         else:
             idx += 1
             self.col_positions.insert(idx, self.col_positions[idx - 1] + w)
             idx += 1
             self.col_positions[idx:] = [e + w for e in islice(self.col_positions, idx, len(self.col_positions))]
+            
+    def insert_row_position(self, idx, height = None, deselect_all = False):
+        if deselect_all:
+            self.deselect("all", redraw = False)
+        if height is None:
+            h = self.default_rh[1]
+        else:
+            h = height
+        if idx == "end" or len(self.row_positions) == idx + 1:
+            self.row_positions.append(self.row_positions[-1] + h)
+        else:
+            idx += 1
+            self.row_positions.insert(idx, self.row_positions[idx - 1] + h)
+            idx += 1
+            self.row_positions[idx:] = [e + h for e in islice(self.row_positions, idx, len(self.row_positions))]
 
     def insert_col_positions(self, idx = "end", widths = None, deselect_all = False):
         if deselect_all:
             self.deselect("all", redraw = False)
         if widths is None:
             w = [self.default_cw]
         elif isinstance(widths, int):
@@ -3201,14 +3247,42 @@
             else:
                 w = w[0]
                 idx += 1
                 self.col_positions.insert(idx, self.col_positions[idx - 1] + w)
                 idx += 1
                 self.col_positions[idx:] = [e + w for e in islice(self.col_positions, idx, len(self.col_positions))]
 
+    def insert_row_positions(self, idx = "end", heights = None, deselect_all = False):
+        if deselect_all:
+            self.deselect("all", redraw = False)
+        if heights is None:
+            h = [self.default_rh[1]]
+        elif isinstance(heights, int):
+            h = list(repeat(self.default_rh[1], heights))
+        else:
+            h = heights
+        if idx == "end" or len(self.row_positions) == idx + 1:
+            if len(h) > 1:
+                self.row_positions += list(accumulate(chain([self.row_positions[-1] + h[0]], islice(h, 1, None))))
+            else:
+                self.row_positions.append(self.row_positions[-1] + h[0])
+        else:
+            if len(h) > 1:
+                idx += 1
+                self.row_positions[idx:idx] = list(accumulate(chain([self.row_positions[idx - 1] + h[0]], islice(h, 1, None))))
+                idx += len(h)
+                sumh = sum(h)
+                self.row_positions[idx:] = [e + sumh for e in islice(self.row_positions, idx, len(self.row_positions))]
+            else:
+                h = h[0]
+                idx += 1
+                self.row_positions.insert(idx, self.row_positions[idx - 1] + h)
+                idx += 1
+                self.row_positions[idx:] = [e + h for e in islice(self.row_positions, idx, len(self.row_positions))]
+
     def insert_col_rc(self, event = None):
         if self.anything_selected(exclude_rows = True, exclude_cells = True):
             selcols = self.get_selected_cols()
             numcols = len(selcols)
             displayed_ins_col = min(selcols) if event == "left" else max(selcols) + 1
             if self.all_columns_displayed:
                 data_ins_col = int(displayed_ins_col)
@@ -3339,72 +3413,41 @@
             seldset = set(seld_cols) if self.all_columns_displayed else set(self.displayed_columns[c] for c in seld_cols)
             list_of_coords = tuple((r, c) for (r, c) in self.cell_options if c in seldset)
             if self.undo_enabled:
                 undo_storage = {'deleted_cols': {},
                                 'colwidths': {},
                                 'deleted_hdr_values': {},
                                 'selection_boxes': self.get_boxes(),
-                                'displayed_columns': list(self.displayed_columns),
+                                'displayed_columns': list(self.displayed_columns) if not isinstance(self.displayed_columns, int) else int(self.displayed_columns),
                                 'cell_options': {k: v.copy() for k, v in self.cell_options.items()},
                                 'col_options': {k: v.copy() for k, v in self.col_options.items()},
                                 'CH_cell_options': {k: v.copy() for k, v in self.CH.cell_options.items()}}
-            if self.all_columns_displayed:
-                if self.undo_enabled:
-                    for c in reversed(seld_cols):
-                        undo_storage['colwidths'][c] = self.col_positions[c + 1] - self.col_positions[c]
-                        for rn in range(len(self.data)):
-                            if c not in undo_storage['deleted_cols']:
-                                undo_storage['deleted_cols'][c] = {}
-                            try:
-                                undo_storage['deleted_cols'][c][rn] = self.data[rn].pop(c)
-                            except:
-                                continue
-                    if self._headers and isinstance(self._headers, list):
-                        for c in reversed(seld_cols):
-                            try:
-                                undo_storage['deleted_hdr_values'][c] = self._headers.pop(c)
-                            except:
-                                continue
-                else:
+                for c in reversed(seld_cols):
+                    undo_storage['colwidths'][c] = self.col_positions[c + 1] - self.col_positions[c]
+                    datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                     for rn in range(len(self.data)):
-                        for c in reversed(seld_cols):
-                            del self.data[rn][c]
-                    if self._headers and isinstance(self._headers, list):
-                        for c in reversed(seld_cols):
-                            try:
-                                del self._headers[c]
-                            except:
-                                continue
+                        if datacn not in undo_storage['deleted_cols']:
+                            undo_storage['deleted_cols'][datacn] = {}
+                        try:
+                            undo_storage['deleted_cols'][datacn][rn] = self.data[rn].pop(datacn)
+                        except:
+                            continue
+                    try:
+                        undo_storage['deleted_hdr_values'][datacn] = self._headers.pop(datacn)
+                    except:
+                        continue
             else:
-                if self.undo_enabled:
-                    for c in reversed(seld_cols):
-                        undo_storage['colwidths'][c] = self.col_positions[c + 1] - self.col_positions[c]
-                        for rn in range(len(self.data)):
-                            if self.displayed_columns[c] not in undo_storage['deleted_cols']:
-                                undo_storage['deleted_cols'][self.displayed_columns[c]] = {}
-                            try:
-                                undo_storage['deleted_cols'][self.displayed_columns[c]][rn] = self.data[rn].pop(self.displayed_columns[c])
-                            except:
-                                continue
-                    if self._headers and isinstance(self._headers, list):
-                        for c in reversed(seld_cols):
-                            try:
-                                undo_storage['deleted_hdr_values'][self.displayed_columns[c]] = self._headers.pop(self.displayed_columns[c])
-                            except:
-                                continue
-                else:
+                for c in reversed(seld_cols):
+                    datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                     for rn in range(len(self.data)):
-                        for c in reversed(seld_cols):
-                            del self.data[rn][self.displayed_columns[c]]
-                    if self._headers and isinstance(self._headers, list):
-                        for c in reversed(seld_cols):
-                            try:
-                                del self._headers[self.displayed_columns[c]]
-                            except:
-                                continue
+                        del self.data[rn][datacn]
+                    try:
+                        del self._headers[datacn]
+                    except:
+                        continue
             if self.undo_enabled:
                 self.undo_storage.append(("delete_cols", undo_storage))
             self.del_cell_options(list_of_coords)
             for c in reversed(seld_cols):
                 datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                 self.del_col_position(c,
                                       deselect_all = False)
@@ -3423,144 +3466,71 @@
                 self.displayed_columns = [c for c in self.displayed_columns if c not in seldset]
                 for c in sorted(seldset):
                     self.displayed_columns = [dc if c > dc else dc - 1 for dc in self.displayed_columns]
             self.refresh()
             if self.extra_end_del_cols_rc_func is not None:
                 self.extra_end_del_cols_rc_func(DeleteRowColumnEvent("end_delete_columns", seld_cols))
 
-    def del_cell_options(self, list_of_coords):
-        for r, datacn in list_of_coords:
-            if (r, datacn) in self.cell_options and 'dropdown' in self.cell_options[(r, datacn)]:
-                self.delete_dropdown(r, datacn)
-            del self.cell_options[(r, datacn)]
-
     def del_rows_rc(self, event = None):
         seld_rows = sorted(self.get_selected_rows())
         if seld_rows:
             if self.extra_begin_del_rows_rc_func is not None:
                 try:
                     self.extra_begin_del_rows_rc_func(DeleteRowColumnEvent("begin_delete_rows", seld_rows))
                 except:
                     return
-            seldset = set(seld_rows)
+            seldset = set(seld_rows) if self.all_rows_displayed else set(self.displayed_rows[c] for r in seld_rows)
             list_of_coords = tuple((r, c) for (r, c) in self.cell_options if r in seldset)
             if self.undo_enabled:
                 undo_storage = {'deleted_rows': [],
+                                'rowheights': {},
                                 'deleted_index_values': [],
                                 'selection_boxes': self.get_boxes(),
+                                'displayed_rows': list(self.displayed_rows) if not isinstance(self.displayed_rows, int) else int(self.displayed_rows),
                                 'cell_options': {k: v.copy() for k, v in self.cell_options.items()},
                                 'row_options': {k: v.copy() for k, v in self.row_options.items()},
                                 'RI_cell_options': {k: v.copy() for k, v in self.RI.cell_options.items()}}
                 for r in reversed(seld_rows):
-                    undo_storage['deleted_rows'].append((r, self.data.pop(r), self.row_positions[r + 1] - self.row_positions[r]))
+                    undo_storage['rowheights'][r] = self.row_positions[r + 1] - self.row_positions[r]
+                    datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+                    undo_storage['deleted_rows'].append((datarn, self.data.pop(datarn)))
+                    try:
+                        undo_storage['deleted_index_values'].append((datarn, self._row_index.pop(datarn)))
+                    except:
+                        continue
             else:
                 for r in reversed(seld_rows):
-                    del self.data[r]
-            if self._row_index and isinstance(self._row_index, list):
-                if self.undo_enabled:
-                    for r in reversed(seld_rows):
-                        try:
-                            undo_storage['deleted_index_values'].append((r, self._row_index.pop(r)))
-                        except:
-                            continue
-                else:
-                    for r in reversed(seld_rows):
-                        try:
-                            del self._row_index[r]
-                        except:
-                            continue
+                    datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+                    del self.data[datarn]
+                    try:
+                        del self._row_index[datarn]
+                    except:
+                        continue
             if self.undo_enabled:
                 self.undo_storage.append(("delete_rows", undo_storage))
             self.del_cell_options(list_of_coords)
             for r in reversed(seld_rows):
+                datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                 self.del_row_position(r,
                                       deselect_all = False)
-                if r in self.row_options:
-                    del self.row_options[r]
-                if r in self.RI.cell_options:
-                    del self.RI.cell_options[r]
+                if datarn in self.row_options:
+                    del self.row_options[datarn]
+                if datarn in self.RI.cell_options:
+                    del self.RI.cell_options[datarn]
             numrows = len(seld_rows)
-            idx = seld_rows[-1]
+            idx = seld_rows[-1] if self.all_rows_displayed else self.displayed_rows[seld_rows[-1]]
             self.cell_options = {(rn if rn < idx else rn - numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items()}
             self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items()}
             self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items()}
             self.deselect("allrows", redraw = False)
             self.set_current_to_last()
             self.refresh()
             if self.extra_end_del_rows_rc_func is not None:
                 self.extra_end_del_rows_rc_func(DeleteRowColumnEvent("end_delete_rows", seld_rows))
 
-    def reset_row_positions(self):
-        rowpos = self.default_rh[1]
-        self.row_positions = list(accumulate(chain([0], (rowpos for r in range(self.total_data_rows())))))
-
-    def del_row_position(self, idx, deselect_all = False):
-        if deselect_all:
-            self.deselect("all", redraw = False)
-        if idx == "end" or len(self.row_positions) <= idx + 1:
-            del self.row_positions[-1]
-        else:
-            w = self.row_positions[idx + 1] - self.row_positions[idx]
-            idx += 1
-            del self.row_positions[idx]
-            self.row_positions[idx:] = [e - w for e in islice(self.row_positions, idx, len(self.row_positions))]
-
-    def del_row_positions(self, idx, numrows = 1, deselect_all = False):
-        if deselect_all:
-            self.deselect("all", redraw = False)
-        if idx == "end" or len(self.row_positions) <= idx + 1:
-            del self.row_positions[-1]
-        else:
-            rhs = [int(b - a) for a, b in zip(self.row_positions, islice(self.row_positions, 1, len(self.row_positions)))]
-            rhs[idx:idx + numrows] = []
-            self.row_positions = list(accumulate(chain([0], (height for height in rhs))))
-
-    def insert_row_position(self, idx, height = None, deselect_all = False):
-        if deselect_all:
-            self.deselect("all", redraw = False)
-        if height is None:
-            h = self.default_rh[1]
-        else:
-            h = height
-        if idx == "end" or len(self.row_positions) == idx + 1:
-            self.row_positions.append(self.row_positions[-1] + h)
-        else:
-            idx += 1
-            self.row_positions.insert(idx, self.row_positions[idx - 1] + h)
-            idx += 1
-            self.row_positions[idx:] = [e + h for e in islice(self.row_positions, idx, len(self.row_positions))]
-
-    def insert_row_positions(self, idx = "end", heights = None, deselect_all = False):
-        if deselect_all:
-            self.deselect("all", redraw = False)
-        if heights is None:
-            h = [self.default_rh[1]]
-        elif isinstance(heights, int):
-            h = list(repeat(self.default_rh[1], heights))
-        else:
-            h = heights
-        if idx == "end" or len(self.row_positions) == idx + 1:
-            if len(h) > 1:
-                self.row_positions += list(accumulate(chain([self.row_positions[-1] + h[0]], islice(h, 1, None))))
-            else:
-                self.row_positions.append(self.row_positions[-1] + h[0])
-        else:
-            if len(h) > 1:
-                idx += 1
-                self.row_positions[idx:idx] = list(accumulate(chain([self.row_positions[idx - 1] + h[0]], islice(h, 1, None))))
-                idx += len(h)
-                sumh = sum(h)
-                self.row_positions[idx:] = [e + sumh for e in islice(self.row_positions, idx, len(self.row_positions))]
-            else:
-                h = h[0]
-                idx += 1
-                self.row_positions.insert(idx, self.row_positions[idx - 1] + h)
-                idx += 1
-                self.row_positions[idx:] = [e + h for e in islice(self.row_positions, idx, len(self.row_positions))]
-
     def move_row_position(self, idx1, idx2):
         if not len(self.row_positions) <= 2:
             if idx1 < idx2:
                 height = self.row_positions[idx1 + 1] - self.row_positions[idx1]
                 self.row_positions.insert(idx2 + 1, self.row_positions.pop(idx1 + 1))
                 for i in range(idx1 + 1, idx2 + 1):
                     self.row_positions[i] -= height
@@ -3582,14 +3552,37 @@
                 self.col_positions[idx2 + 1] = self.col_positions[idx2] + width
             else:
                 width = self.col_positions[idx1 + 1] - self.col_positions[idx1]
                 self.col_positions.insert(idx2 + 1, self.col_positions.pop(idx1 + 1))
                 for i in range(idx2 + 2, idx1 + 2):
                     self.col_positions[i] += width
                 self.col_positions[idx2 + 1] = self.col_positions[idx2] + width
+                
+    def display_rows(self, rows = None, all_rows_displayed = None, reset_row_positions = True, deselect_all = True):
+        if rows is None and all_rows_displayed is None:
+            return list(range(self.total_data_rows())) if self.all_rows_displayed else self.displayed_rows
+        total_data_rows = None
+        if (
+            (rows is not None and rows != self.displayed_rows) or 
+            (all_rows_displayed and not self.all_rows_displayed)
+            ):
+            self.undo_storage = deque(maxlen = self.max_undos)
+        if rows is not None and rows != self.displayed_rows:
+            self.displayed_rows = sorted(rows)
+        if all_rows_displayed:
+            if not self.all_rows_displayed:
+                total_data_rows = self.total_data_rows()
+                self.displayed_rows = list(range(total_data_rows))
+            self.all_rows_displayed = True
+        elif all_rows_displayed is not None and not all_rows_displayed:
+            self.all_rows_displayed = False
+        if reset_row_positions:
+            self.reset_row_positions(nrows = total_data_rows)
+        if deselect_all:
+            self.deselect("all", redraw = False)
 
     def display_columns(self, columns = None, all_columns_displayed = None, reset_col_positions = True, deselect_all = True):
         if columns is None and all_columns_displayed is None:
             return list(range(self.total_data_cols())) if self.all_columns_displayed else self.displayed_columns
         total_data_cols = None
         if (
             (columns is not None and columns != self.displayed_columns) or 
@@ -3632,17 +3625,16 @@
                 if self.all_columns_displayed:
                     self.col_positions = list(accumulate(chain([0], (colpos for c in range(len(self._headers))))))
                 else:
                     self.col_positions = list(accumulate(chain([0], (colpos for c in range(len(self.displayed_columns))))))
             if redraw:
                 self.refresh()
         else:
-            if index is not None:
-                if isinstance(index, int):
-                    return self._headers[index]
+            if not isinstance(self._headers, int) and index is not None and isinstance(index, int):
+                return self._headers[index]
             else:
                 return self._headers
 
     def row_index(self, newindex = None, index = None, reset_row_positions = False, show_index_if_not_sheet = True, redraw = False):
         if newindex is not None:
             if not self._row_index and not isinstance(self._row_index, int):
                 self.RI.set_width(self.RI.default_width, set_TL = True)
@@ -3659,21 +3651,24 @@
                     self._row_index = list(newindex)
                 except:
                     raise ValueError("New index must be iterable or int (use int to use a column as the index")
             if reset_row_positions:
                 self.reset_row_positions()
             elif show_index_if_not_sheet and isinstance(self._row_index, list) and (self.row_positions == [0] or not self.row_positions):
                 rowpos = self.default_rh[1]
-                self.row_positions = list(accumulate(chain([0], (rowpos for c in range(len(self._row_index))))))
+                if self.all_rows_displayed:
+                    self.row_positions = list(accumulate(chain([0], (rowpos for r in range(len(self._row_index))))))
+                else:
+                    self.row_positions = list(accumulate(chain([0], (rowpos for r in range(len(self.displayed_rows))))))
+                
             if redraw:
                 self.refresh()
         else:
-            if index is not None:
-                if isinstance(index, int):
-                    return self._row_index[index]
+            if not isinstance(self._row_index, int) and index is not None and isinstance(index, int):
+                return self._row_index[index]
             else:
                 return self._row_index
 
     def total_data_cols(self, include_header = True):
         h_total = 0
         d_total = 0
         if include_header:
@@ -3738,15 +3733,15 @@
         # ________________________ CELL IS HIGHLIGHTED AND IN SELECTED CELLS ________________________
         if (datarn, datacn) in self.cell_options and 'highlight' in self.cell_options[(datarn, datacn)] and (r, c) in selected_cells:
             tf = self.table_selected_cells_fg if self.cell_options[(datarn, datacn)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(datarn, datacn)]['highlight'][1]
             if self.cell_options[(datarn, datacn)]['highlight'][0] is not None:
                 c_1 = self.cell_options[(datarn, datacn)]['highlight'][0] if self.cell_options[(datarn, datacn)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(datarn, datacn)]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_2_[0]) / 2):02X}" +
                                                                                 f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"),
+                                                                                f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"), 
                                                 outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
                                                 tag = "hi")
             
         elif datarn in self.row_options and 'highlight' in self.row_options[datarn] and (r, c) in selected_cells:
             tf = self.table_selected_cells_fg if self.row_options[datarn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[datarn]['highlight'][1]
             if self.row_options[datarn]['highlight'][0] is not None:
                 c_1 = self.row_options[datarn]['highlight'][0] if self.row_options[datarn]['highlight'][0].startswith("#") else Color_Map_[self.row_options[datarn]['highlight'][0]]
@@ -3863,21 +3858,26 @@
             tf = self.table_selected_columns_fg
 
         # ________________________ CELL IS NOT SELECTED ________________________
         else:
             tf = self.table_fg
         return tf, redrawn
 
-    def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag, can_width = None):
+    def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag, can_width = None, pc = None):
         config = (fill, outline)
-        coords = (x1 - 1 if outline else x1,
-                  y1 - 1 if outline else y1,
-                  x2 if can_width is None else x2 + can_width, 
-                  y2)
-
+        if type(pc) != int or pc >= 100 or pc <= 0:
+            coords = (x1 - 1 if outline else x1,
+                      y1 - 1 if outline else y1,
+                      x2 if can_width is None else x2 + can_width, 
+                      y2)
+        else:
+            coords = (x1,
+                      y1,
+                      (x2 - x1) * (pc / 100),
+                      y2)
         k = None
         if config in self.hidd_high:
             k = config
             iid, showing = self.hidd_high[k].pop()
             if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 0 if showing else 2
             else:
@@ -4155,16 +4155,16 @@
                     cleftgridln = self.col_positions[c]
                     crightgridln = self.col_positions[c + 1]
                     
                     datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                     datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                     
                     fill, dd_drawn = self.redraw_highlight_get_text_fg(r, c, cleftgridln, rtopgridln, crightgridln, rbotgridln,
-                                                                        c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, 
-                                                                        datarn, datacn, can_width)
+                                                                       c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, 
+                                                                       datarn, datacn, can_width)
                         
                     if (datarn, datacn) in self.cell_options and 'align' in self.cell_options[(datarn, datacn)]:
                         align = self.cell_options[(datarn, datacn)]['align']
                     elif datarn in self.row_options and 'align' in self.row_options[datarn]:
                         align = self.row_options[datarn]['align']
                     elif datacn in self.col_options and 'align' in self.col_options[datacn]:
                         align = self.col_options[datacn]['align']
@@ -4216,24 +4216,20 @@
                             else:
                                 mw -= 3
                             try:
                                 draw_check = self.data[datarn][datacn]
                             except:
                                 draw_check = False
                             self.redraw_checkbox(cleftgridln + 2,
-                                                    rtopgridln + 2,
-                                                    cleftgridln + self.txt_h + 3,
-                                                    rtopgridln + self.txt_h + 3,
-                                                    fill = fill if self.cell_options[(datarn, datacn)]['checkbox']['state'] == "normal" else self.table_grid_fg,
-                                                    outline = "", tag = "cb", draw_check = draw_check)
-
-                    if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
-                        lns = self.cell_options[(datarn, datacn)]['checkbox']['text'].split("\n") if isinstance(self.cell_options[(datarn, datacn)]['checkbox']['text'], str) else f"{self.cell_options[(datarn, datacn)]['checkbox']['text']}".split("\n")
-                    else:
-                        lns = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True).split("\n")
+                                                 rtopgridln + 2,
+                                                 cleftgridln + self.txt_h + 3,
+                                                 rtopgridln + self.txt_h + 3,
+                                                 fill = fill if self.cell_options[(datarn, datacn)]['checkbox']['state'] == "normal" else self.table_grid_fg,
+                                                 outline = "", tag = "cb", draw_check = draw_check)
+                    lns = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True).split("\n")
                     if lns != [''] and mw > self.txt_w and not ((align == "w" and draw_x > scrollpos_right) or
                                                                 (align == "e" and cleftgridln + 5 > scrollpos_right) or
                                                                 (align == "center" and stop > scrollpos_right)):
                         draw_y = rtopgridln + self.fl_ins
                         start_ln = int((scrollpos_top - rtopgridln) / self.xtra_lines_increment)
                         if start_ln < 0:
                             start_ln = 0
@@ -5332,25 +5328,26 @@
     def set_cell_data(self, datarn, datacn, value, kwargs = {}, expand_sheet = True):
         if expand_sheet:
             if datarn >= len(self.data):
                 self.data.extend([list(repeat("", datacn + 1)) for i in range((datarn + 1) - len(self.data))])
             elif datacn >= len(self.data[datarn]):
                 self.data[datarn].extend(list(repeat("", (datacn + 1) - len(self.data[datarn]))))
         if expand_sheet or (len(self.data) > datarn and len(self.data[datarn]) > datacn):
-            if not kwargs:
-                kwargs = self.get_format_kwargs(datarn, datacn)
-            if kwargs:
-                if kwargs['formatter'] is None:
-                    self.data[datarn][datacn] = format_data(value = value, **kwargs)
-                else:
-                    self.data[datarn][datacn] = kwargs['formatter'](value, **kwargs)
-            elif (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
-                self.data[datarn][datacn] = to_bool(value)
+            if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
+                self.data[datarn][datacn] = try_to_bool(value)
             else:
-                self.data[datarn][datacn] = value
+                if not kwargs:
+                    kwargs = self.get_format_kwargs(datarn, datacn)
+                if kwargs:
+                    if kwargs['formatter'] is None:
+                        self.data[datarn][datacn] = format_data(value = value, **kwargs)
+                    else:
+                        self.data[datarn][datacn] = kwargs['formatter'](value, **kwargs)
+                else:
+                    self.data[datarn][datacn] = value
 
     #internal event use
     def _click_checkbox(self, r, c, datarn = None, datacn = None, undo = True, redraw = True):
         if datarn is None:
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         if datacn is None:
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
@@ -5366,44 +5363,44 @@
             self.refresh()
 
     def create_checkbox(self, datarn = 0, datacn = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
         self.delete_cell_format(datarn, datacn, clear_values = True)
         if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
                                                       'checkbox' in self.cell_options[(datarn, datacn)]):
             self.delete_dropdown_and_checkbox(datarn, datacn)
-        self.set_cell_data(datarn, datacn, checked)
         if (datarn, datacn) not in self.cell_options:
             self.cell_options[(datarn, datacn)] = {}
         self.cell_options[(datarn, datacn)]['checkbox'] = {'check_function': check_function,
                                                            'state': state,
                                                            'text': text}
+        self.set_cell_data(datarn, datacn, checked)
         if redraw:
             self.refresh()
 
     def create_dropdown(self, 
                         datarn = 0, datacn = 0, 
                         values = [], set_value = None,
                         state = "normal", redraw = True, 
                         selection_function = None, modified_function = None,
                         search_function = dropdown_search_function, validate_input = True, text = None):
         if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
                                                       'checkbox' in self.cell_options[(datarn, datacn)]):
             self.delete_dropdown_and_checkbox(datarn, datacn)
-        self.set_cell_data(datarn, datacn, set_value if set_value is not None else values[0] if values else "")
         if (datarn, datacn) not in self.cell_options:
             self.cell_options[(datarn, datacn)] = {}
         self.cell_options[(datarn, datacn)]['dropdown'] = {'values': values,
                                                            'window': "no dropdown open",
                                                            'canvas_id': "no dropdown open",
                                                            'select_function': selection_function,
                                                            'modified_function': modified_function,
                                                            'search_function': search_function,
                                                            'validate_input': validate_input,
                                                            'text': text,
                                                            'state': state}
+        self.set_cell_data(datarn, datacn, set_value if set_value is not None else values[0] if values else "")
         if redraw:
             self.refresh()
 
     def format_cell(self,
                     datarn, 
                     datacn,
                     **kwargs):
@@ -5533,60 +5530,76 @@
     
     def delete_sheet_format(self, clear_values = False):
         if 'format' in self.sheet_options:
             del self.sheet_options['format']
             if clear_values:
                 total_cols = self.total_data_cols()
                 self.data = [list(repeat("", total_cols)) for i in range(len(self.data))]
+                
+    def del_cell_options(self, list_of_coords):
+        for r, datacn in list_of_coords:
+            if (r, datacn) in self.cell_options and 'dropdown' in self.cell_options[(r, datacn)]:
+                self.delete_dropdown(r, datacn)
+            del self.cell_options[(r, datacn)]
 
     # deals with possibility of formatter class being in self.data cell
     # if cell is formatted - possibly returns invalid_value kwarg if cell value is not in datatypes kwarg
     # if get displayed is true then Nones are replaced by ""
     def get_valid_cell_data_as_str(self, datarn, datacn, get_displayed = False, **kwargs) -> str:
+        if get_displayed and (datarn, datacn) in self.cell_options:
+            if 'dropdown' in self.cell_options[(datarn, datacn)] and self.cell_options[(datarn, datacn)]['dropdown']['text'] is not None:
+                return f"{self.cell_options[(datarn, datacn)]['dropdown']['text']}"
+            if 'checkbox' in self.cell_options[(datarn, datacn)]:
+                return f"{self.cell_options[(datarn, datacn)]['checkbox']['text']}"
         value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
         kwargs = self.get_format_kwargs(datarn, datacn)
         if kwargs:
             if kwargs['formatter'] is None:
                 if get_displayed:
                     return data_to_str(value, **kwargs)
                 else:
                     return f"{get_data_with_valid_check(value, **kwargs)}"
             else:
                 if get_displayed:
                     return f"{value}" # assumed given formatter class has __str__() function
                 else:
                     return f"{value.get_data_with_valid_check()}" # assumed given formatter class has get_data_with_valid_check() function
-        return f"{value}"
+        return "" if value is None else f"{value}"
 
     def get_cell_data(self, datarn, datacn, get_displayed = False, none_to_empty_str = False, **kwargs) -> Any:
+        if get_displayed and (datarn, datacn) in self.cell_options:
+            if 'dropdown' in self.cell_options[(datarn, datacn)] and self.cell_options[(datarn, datacn)]['dropdown']['text'] is not None:
+                return self.cell_options[(datarn, datacn)]['dropdown']['text']
+            if 'checkbox' in self.cell_options[(datarn, datacn)] and self.cell_options[(datarn, datacn)]['checkbox']['text'] is not None:
+                return self.cell_options[(datarn, datacn)]['checkbox']['text']
         value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
         kwargs = self.get_format_kwargs(datarn, datacn)
         if kwargs:
             if kwargs['formatter'] is None:
                 if get_displayed:
                     return data_to_str(value, **kwargs)
             else:
                 if get_displayed:
                     return f"{value}" # assumed given formatter class has __str__() function
                 else:
                     value = value.value # assumed given formatter class has value attribute
-        return "" if (value is None and none_to_empty_str) else value
+        return "" if (value is None and (none_to_empty_str or get_displayed)) else value
     
     def input_valid_for_cell(self, datarn, datacn, value):
         if (datarn, datacn) in self.cell_options and 'readonly' in self.cell_options[(datarn, datacn)]:
             return False
         if datarn in self.row_options and 'readonly' in self.row_options[datarn]:
             return False
         if datacn in self.col_options and 'readonly' in self.col_options[datacn]:
             return False
         if self.cell_equal_to(datarn, datacn, value):
             return False
         if self.get_format_kwargs(datarn, datacn):
             return True
-        if (datarn, datacn) in self.cell_options: 
+        if (datarn, datacn) in self.cell_options:
             if 'checkbox' in self.cell_options[(datarn, datacn)]:
                 return is_bool_like(value)
             if ('dropdown' in self.cell_options[(datarn, datacn)] and 
                 self.cell_options[(datarn, datacn)]['dropdown']['validate_input'] and 
                 value not in self.cell_options[(datarn, datacn)]['dropdown']['values']):
                 return False
         return True
@@ -5595,19 +5608,14 @@
         v = self.get_cell_data(datarn, datacn)
         kwargs = self.get_format_kwargs(datarn, datacn)
         if kwargs and kwargs['formatter'] is None:
             return v == format_data(value = value, **kwargs)
         # assumed if there is a formatter class in cell then it has a __eq__() function anyway
         # else if there is not a formatter class in cell and cell is not formatted
         # then compare value as is
-        if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
-            try:
-                return to_bool(v) == to_bool(value)
-            except:
-                return False
         return v == value
 
     def get_cell_clipboard(self, datarn, datacn) -> Union[str, int, float, bool]:
         value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
         kwargs = self.get_format_kwargs(datarn, datacn)
         if kwargs:
             if kwargs['formatter'] is None:
```

### Comparing `tksheet-6.0.0/tksheet/_tksheet_other_classes.py` & `tksheet-6.0.1/tksheet/_tksheet_other_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 EditIndexEvent = namedtuple("EditIndexEvent", "row key text eventname")
 BeginDragDropEvent = namedtuple("BeginDragDropEvent", "eventname columnstomove movedto")
 EndDragDropEvent = namedtuple("EndDragDropEvent", "eventname oldindexes newindexes movedto")
 ResizeEvent = namedtuple("ResizeEvent", "eventname index oldsize newsize")
 DropDownModifiedEvent = namedtuple("DropDownModifiedEvent", "eventname row column value")
 DrawnItem = namedtuple("DrawnItem", "iid showing")
 TextCfg = namedtuple("TextCfg", "txt tf font align")
+ProgressBar = namedtuple("ProgressBar", "bg fg pc name")
 
 
 class TextEditor_(tk.Text):
     def __init__(self,
                  parent,
                  font = get_font(),
                  text = None,
```

### Comparing `tksheet-6.0.0/tksheet/_tksheet_row_index.py` & `tksheet-6.0.1/tksheet/_tksheet_row_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,15 +543,15 @@
                                                                                 sorted(orig_selected)))))
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ri_extra_end_drag_drop_func is not None:
                         self.ri_extra_end_drag_drop_func(EndDragDropEvent("end_row_index_drag_drop", tuple(orig_selected), new_selected, int(r)))
                         
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             r = self.MT.identify_row(y = event.y)
-            if r is not None and r == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
+            if r is not None and r < len(self.MT.row_positions) - 1 and r == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
                 datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
                 if (self.canvasy(event.y) < self.MT.row_positions[r] + self.MT.txt_h and
                     (
                      (datarn in self.cell_options and 
                       'dropdown' in self.cell_options[datarn] and 
                       event.x < self.current_width and 
                       event.x > self.current_width - self.MT.txt_h - 4) 
@@ -651,14 +651,28 @@
                 r1, c1, r2, c2 = tuple(int(e) for e in current[1].split("_") if e)
                 self.MT.create_selected(r1, c1, r2, c2, current[2] + "s")
         self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(("select_row", int(r)))
+            
+    def get_cell_dimensions(self, datarn):
+        txt = self.get_valid_cell_data_as_str(datarn, fix = False)
+        if txt:
+            self.MT.txt_measure_canvas.itemconfig(self.MT.txt_measure_canvas_text, text = txt, font = self.MT._font)
+            b = self.MT.txt_measure_canvas.bbox(self.MT.txt_measure_canvas_text)
+            w = b[2] - b[0] + 7
+            h = b[3] - b[1] + 5
+        else:
+            w = self.default_width
+            h = self.MT.min_rh
+        if datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 'checkbox' in self.cell_options[datarn]):
+            return w + self.MT.txt_h, h
+        return w, h
 
     def set_row_height(self, row, height = None, only_set_if_too_small = False, recreate = True, return_new_height = False, displayed_only = False):
         r_norm = row + 1
         r_extra = row + 2
         min_rh = self.MT.min_rh
         datarn = row if self.MT.all_rows_displayed else self.MT.displayed_rows[row]
         if height is None:
@@ -673,34 +687,24 @@
                 if displayed_only:
                     x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
                     start_col, end_col = self.MT.get_visible_columns(x1, x2)
                 else:
                     start_col, end_col = 0, len(self.MT.displayed_columns)
                 iterable = self.MT.displayed_columns[start_col:end_col]
             new_height = int(min_rh)
-            if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
-                txt = self.cell_options[datarn]['checkbox']['text']
-            else:
-                txt = self.get_valid_cell_data_as_str(datarn, fix = False)
-            if txt:
-                h = self.MT.GetTextHeight(txt) + 5
-            else:
-                h = min_rh
+            w_, h = self.get_cell_dimensions(datarn)
             if h < min_rh:
                 h = int(min_rh)
             elif h > self.max_rh:
                 h = int(self.max_rh)
             if h > new_height:
                 new_height = h
             if self.MT.data:
-                for cn in iterable:
-                    if (datarn, cn) in self.MT.cell_options and 'checkbox' in self.MT.cell_options[(datarn, cn)]:
-                        txt = self.MT.cell_options[(datarn, cn)]['checkbox']['text']
-                    else:
-                        txt = self.MT.get_valid_cell_data_as_str(datarn, cn, get_displayed = True)
+                for datacn in iterable:
+                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
                     if txt:
                         h = self.MT.GetTextHeight(txt) + 5
                     else:
                         h = min_rh
                     if h < min_rh:
                         h = int(min_rh)
                     elif h > self.max_rh:
@@ -727,49 +731,39 @@
     def set_width_of_index_to_text(self, recreate = True):
         if not self.MT._row_index and isinstance(self.MT._row_index, list):
             return
         qconf = self.MT.txt_measure_canvas.itemconfig
         qbbox = self.MT.txt_measure_canvas.bbox
         qtxtm = self.MT.txt_measure_canvas_text
         new_width = int(self.MT.min_cw)
+        self.fix_index()
+        if self.MT.all_rows_displayed:
+            if isinstance(self.MT._row_index, list):
+                iterable = range(len(self.MT._row_index))
+            else:
+                iterable = range(len(self.MT.data))
+        else:
+            iterable = self.MT.displayed_rows
         if isinstance(self.MT._row_index, list):
-            for rn, row in enumerate(self.MT._row_index):
-                if rn in self.cell_options and 'checkbox' in self.cell_options[rn]:
-                    txt = self.cell_options[rn]['checkbox']['text']
-                else:
-                    try:
-                        if isinstance(row, str):
-                            txt = row
-                        else:
-                            txt = f"{row}"
-                    except:
-                        txt = ""
-                if txt:
-                    qconf(qtxtm, text = txt)
-                    b = qbbox(qtxtm)
-                    w = b[2] - b[0] + 10
-                else:
-                    w = self.default_width
+            for datarn in iterable:
+                w, h_ = self.get_cell_dimensions(datarn)
                 if w < self.MT.min_cw:
                     w = int(self.MT.min_cw)
                 elif w > self.max_row_width:
                     w = int(self.max_row_width)
-                if rn in self.cell_options and 'checkbox' in self.cell_options[rn]:
+                if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
                     w += self.MT.txt_h + 6
-                elif rn in self.cell_options and 'dropdown' in self.cell_options[rn]:
+                elif datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
                     w += self.MT.txt_h + 4
                 if w > new_width:
                     new_width = w
         elif isinstance(self.MT._row_index, int):
-            c = self.MT._row_index
-            for rn, row in enumerate(self.MT.data):
-                if (rn, c) in self.MT.cell_options and 'checkbox' in self.MT.cell_options[(rn, c)]:
-                    txt = self.MT.cell_options[(rn, c)]['checkbox']['text']
-                else:
-                    txt = self.MT.get_valid_cell_data_as_str(rn, c, get_displayed = True)
+            datacn = self.MT._row_index
+            for datarn in iterable:
+                txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
                 if txt:
                     qconf(qtxtm, text = txt)
                     b = qbbox(qtxtm)
                     w = b[2] - b[0] + 10
                 else:
                     w = self.default_width
                 if w < self.MT.min_cw:
@@ -955,15 +949,15 @@
                 else:
                     self.itemconfig(t, fill = fill, tag = tag, state = "normal")
                 self.lift(t)
             else:
                 t = self.create_line(points, fill = fill, width = 2, capstyle = tk.ROUND, joinstyle = tk.ROUND, tag = tag)
             self.disp_dropdown[t] = True
             
-    def redraw_checkbox(self, r, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
+    def redraw_checkbox(self, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
         points = self.MT.get_checkbox_points(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill = outline, outline = fill)
             else:
@@ -1037,96 +1031,86 @@
                                    self.current_width, self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y])
                 elif st_or_end == "end":
                     points.extend([self.current_width, draw_y,
                                    -1, draw_y,
                                    -1, self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y])
                 if points:
                     self.redraw_gridline(points = points, fill = self.index_grid_fg, width = 1, tag = "h")
-        scrollpos_bot_add2 = scrollpos_bot + 2
         c_2 = self.index_selected_cells_bg if self.index_selected_cells_bg.startswith("#") else Color_Map_[self.index_selected_cells_bg]
         c_3 = self.index_selected_rows_bg if self.index_selected_rows_bg.startswith("#") else Color_Map_[self.index_selected_rows_bg]
         font = self.MT._font
         for r in range(start_row, end_row - 1):
             rtopgridln = self.MT.row_positions[r]
             rbotgridln = self.MT.row_positions[r + 1]
             if rbotgridln - rtopgridln < self.MT.txt_h:
                 continue
-            if rbotgridln > scrollpos_bot_add2:
-                rbotgridln = scrollpos_bot_add2
-            if self.MT.all_rows_displayed:
-                datarn = r
-            else:
-                datarn = self.MT.displayed_rows[r]
+            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             fill, dd_drawn = self.redraw_highlight_get_text_fg(rtopgridln, rbotgridln, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, datarn)
             
-            if r in self.cell_options and 'align' in self.cell_options[r]:
-                align = self.cell_options[r]['align']
+            if datarn in self.cell_options and 'align' in self.cell_options[datarn]:
+                align = self.cell_options[datarn]['align']
             else:
                 align = self.align
                 
             if align == "w":
                 draw_x = 3
-                if r in self.cell_options and 'dropdown' in self.cell_options[r]:
+                if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
                     mw = self.current_width - self.MT.txt_h - 2
                     self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[r]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = self.cell_options[datarn]['dropdown']['window'] != "no dropdown open")
                 else:
                     mw = self.current_width - 2
 
             elif align == "e":
-                if r in self.cell_options and 'dropdown' in self.cell_options[r]:
+                if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
                     mw = self.current_width - self.MT.txt_h - 2
                     draw_x = self.current_width - 5 - self.MT.txt_h
                     self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[r]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = self.cell_options[datarn]['dropdown']['window'] != "no dropdown open")
                 else:
                     mw = self.current_width - 2
                     draw_x = self.current_width - 3
 
             elif align == "center":
-                if r in self.cell_options and 'dropdown' in self.cell_options[r]:
+                if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
                     mw = self.current_width - self.MT.txt_h - 2
                     draw_x = ceil((self.current_width - self.MT.txt_h) / 2)
                     self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[r]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = self.cell_options[datarn]['dropdown']['window'] != "no dropdown open")
                 else:
                     mw = self.current_width - 1
                     draw_x = floor(self.current_width / 2)
 
-            if r in self.cell_options and 'checkbox' in self.cell_options[r]:
+            if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
                 if mw > + 2:
                     box_w = self.MT.txt_h + 1
                     mw -= box_w
                     if align == "w":
                         draw_x += box_w + 1
                     elif align == "center":
                         draw_x += ceil(box_w / 2) + 1
                         mw -= 1
                     else:
                         mw -= 3
                     try:
-                        draw_check = self.MT._row_index[r] if isinstance(self.MT._row_index, (list, tuple)) else self.MT.data[r][self.MT._row_index]
+                        draw_check = self.MT._row_index[datarn] if isinstance(self.MT._row_index, (list, tuple)) else self.MT.data[datarn][self.MT._row_index]
                     except:
                         draw_check = False
-                    self.redraw_checkbox(r,
-                                         2,
+                    self.redraw_checkbox(2,
                                          rtopgridln + 2,
                                          self.MT.txt_h + 3,
                                          rtopgridln + self.MT.txt_h + 3,
-                                         fill = fill if self.cell_options[r]['checkbox']['state'] == "normal" else self.index_grid_fg,
+                                         fill = fill if self.cell_options[datarn]['checkbox']['state'] == "normal" else self.index_grid_fg,
                                          outline = "",
                                          tag = "cb",
                                          draw_check = draw_check)
-            if r in self.cell_options and 'checkbox' in self.cell_options[r]:
-                lns = self.cell_options[r]['checkbox']['text'].split("\n") if isinstance(self.cell_options[r]['checkbox']['text'], str) else f"{self.cell_options[r]['checkbox']['text']}".split("\n")
-            else:
-                lns = self.get_valid_cell_data_as_str(r, fix = False).split("\n")
+            lns = self.get_valid_cell_data_as_str(datarn, fix = False).split("\n")
             if lns == [""]:
                 if self.show_default_index_for_empty:
                     lns = (get_n2a(r, self.default_index), )
                 else:
                     continue
             draw_y = rtopgridln + self.MT.fl_ins
             if mw > 5:
@@ -1319,15 +1303,15 @@
         self.text_editor_loc = r
         x = 0
         y = self.MT.row_positions[r] + 1
         w = self.current_width + 1
         h = self.MT.row_positions[r + 1] - y
         datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         if text is None:
-            text = self.get_valid_cell_data_as_str(datarn)
+            text = self.get_cell_data(datarn)
         bg, fg = self.index_bg, self.index_fg
         self.text_editor = TextEditor(self,
                                       text = text,
                                       font = self.MT._font,
                                       state = state,
                                       width = w,
                                       height = h,
@@ -1490,15 +1474,15 @@
 
     def set_cell_data(self, datarn = None, value = ""):
         if isinstance(self.MT._row_index, int):
             self.MT.set_cell_data(datarn = datarn, datacn = self.MT._row_index, value = value)
         else:
             self.fix_index(datarn)
             if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
-                self.MT._row_index[datarn] = to_bool(value)
+                self.MT._row_index[datarn] = try_to_bool(value)
             else:
                 self.MT._row_index[datarn] = value
             
     def input_valid_for_cell(self, datarn, value):
         if datarn in self.cell_options:
             if 'readonly' in self.cell_options[datarn]:
                 return False
@@ -1512,44 +1496,45 @@
             value not in self.cell_options[datarn]['dropdown']['values']):
             return False
         return True
     
     def cell_equal_to(self, datarn, value):
         self.fix_index(datarn)
         if isinstance(self.MT._row_index, list):
-            if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
-                try:
-                    return to_bool(self.MT._row_index[datarn]) == to_bool(value)
-                except:
-                    return False
             return self.MT._row_index[datarn] == value
         elif isinstance(self.MT._row_index, int):
             return self.MT.cell_equal_to(datarn, self.MT._row_index, value)
             
     def get_cell_data(self, datarn, get_displayed = False, redirect_int = False):
-        if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn] and self.cell_options[datarn]['dropdown']['text'] is not None and get_displayed:
-            return self.cell_options[datarn]['dropdown']['text']
+        if get_displayed and datarn in self.cell_options:
+            if 'dropdown' in self.cell_options[datarn] and self.cell_options[datarn]['dropdown']['text'] is not None:
+                return self.cell_options[datarn]['dropdown']['text']
+            if 'checkbox' in self.cell_options[datarn]:
+                return self.cell_options[datarn]['checkbox']['text']
         if redirect_int and isinstance(self.MT._row_index, int):
             return self.MT.get_cell_data(datarn, self.MT._row_index, none_to_empty_str = True)
         if isinstance(self.MT._row_index, int) or not self.MT._row_index or datarn >= len(self.MT._row_index) or not self.MT._row_index[datarn]:
             if get_displayed and self.show_default_index_for_empty:
                 return get_n2a(datarn, self.default_index)
             else:
                 return ""
-        return self.MT._row_index[datarn]
+        return "" if self.MT._row_index[datarn] is None and get_displayed else self.MT._row_index[datarn]
             
     def get_valid_cell_data_as_str(self, datarn, fix = True) -> str:
-        if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn] and self.cell_options[datarn]['dropdown']['text'] is not None:
-            return f"{self.cell_options[datarn]['dropdown']['text']}"
+        if datarn in self.cell_options:
+            if 'dropdown' in self.cell_options[datarn] and self.cell_options[datarn]['dropdown']['text'] is not None:
+                return f"{self.cell_options[datarn]['dropdown']['text']}"
+            if 'checkbox' in self.cell_options[datarn]:
+                return f"{self.cell_options[datarn]['checkbox']['text']}"
         if isinstance(self.MT._row_index, int):
             return self.MT.get_valid_cell_data_as_str(datarn, self.MT._row_index, get_displayed = True)
         if fix:
             self.fix_index(datarn)
         try:
-            return f"{self.MT._row_index[datarn]}"
+            return "" if self.MT._row_index[datarn] is None else f"{self.MT._row_index[datarn]}"
         except:
             return ""
             
     def fix_index(self, datarn = None):
         if isinstance(self.MT._row_index, int):
             return
         if isinstance(self.MT._row_index, float):
@@ -1573,15 +1558,15 @@
     def _click_checkbox(self, r, datarn = None, undo = True, redraw = True):
         if datarn is None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         if self.cell_options[datarn]['checkbox']['state'] == "normal":
             if isinstance(self.MT._row_index, list):
                 value = not self.MT._row_index[datarn] if type(self.MT._row_index[datarn]) == bool else False
             elif isinstance(self.MT._row_index, int):
-                value = not self.MT.data[self.MT._row_index][datarn] if type(self.MT.data[self.MT._row_index][datarn]) == bool else False
+                value = not self.MT.data[datarn][self.MT._row_index] if type(self.MT.data[datarn][self.MT._row_index]) == bool else False
             else:
                 value = False
             self.set_cell_data_undo(r, 
                                     datarn = datarn, 
                                     value = value, 
                                     cell_resize = False)
             if self.cell_options[datarn]['checkbox']['check_function'] is not None:
@@ -1597,46 +1582,45 @@
         if redraw:
             self.MT.refresh()
 
     def create_checkbox(self, datarn = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
         if datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 
                                             'checkbox' in self.cell_options[datarn]):
             self.delete_dropdown_and_checkbox(datarn)
-        self.set_cell_data(datarn = datarn, 
-                            value = checked)
         if datarn not in self.cell_options:
             self.cell_options[datarn] = {}
         self.cell_options[datarn]['checkbox'] = {'check_function': check_function,
                                                  'state': state,
                                                  'text': text}
+        self.set_cell_data(datarn = datarn, value = checked)
         if redraw:
             self.MT.refresh()
 
     def create_dropdown(self, 
                         datarn = 0, 
                         values = [], set_value = None, 
                         state = "normal", redraw = True, 
                         selection_function = None, modified_function = None,
                         search_function = dropdown_search_function, validate_input = True, text = None):
         if datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 
                                             'checkbox' in self.cell_options[datarn]):
             self.delete_dropdown_and_checkbox(datarn)
-        self.set_cell_data(datarn = datarn, 
-                            value = set_value if set_value is not None else values[0] if values else "")
         if datarn not in self.cell_options:
             self.cell_options[datarn] = {}
         self.cell_options[datarn]['dropdown'] = {'values': values,
                                                  'window': "no dropdown open",
                                                  'canvas_id': "no dropdown open",
                                                  'select_function': selection_function,
                                                  'modified_function': modified_function,
                                                  'search_function': search_function,
                                                  'validate_input': validate_input,
                                                  'text': text,
                                                  'state': state}
+        self.set_cell_data(datarn = datarn, 
+                           value = set_value if set_value is not None else values[0] if values else "")
         if redraw:
             self.MT.refresh()
     
     def get_dropdown_height_anchor(self, datarn, text_editor_h = None):
         win_h = 5
         for i, v in enumerate(self.cell_options[datarn]['dropdown']['values']):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
```

### Comparing `tksheet-6.0.0/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.0.1/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.0/tksheet/_tksheet_vars.py` & `tksheet-6.0.1/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.0/tksheet.egg-info/PKG-INFO` & `tksheet-6.0.1/tksheet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.0.0
+Version: 6.0.1
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.0.0.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.0.1.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

