# Comparing `tmp/mxio-2023.1.23.tar.gz` & `tmp/mxio-2023.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxio-2023.1.23.tar", last modified: Mon Apr 24 16:33:03 2023, max compression
+gzip compressed data, was "mxio-2023.1.4.tar", last modified: Mon Jan  9 14:53:34 2023, max compression
```

## Comparing `mxio-2023.1.23.tar` & `mxio-2023.1.4.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-04-24 16:33:03.096171 mxio-2023.1.23/
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-04-24 16:33:03.095172 mxio-2023.1.23/.github/
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-04-24 16:33:03.095172 mxio-2023.1.23/.github/workflows/
--rw-rw-r--   0 michel   (70005) michel   (70005)      865 2020-03-30 21:45:04.000000 mxio-2023.1.23/.github/workflows/pythonpublish.yml
--rw-rw-r--   0 michel   (70005) michel   (70005)     1083 2020-03-30 21:07:43.000000 mxio-2023.1.23/LICENSE
--rw-r--r--   0 michel   (70005) michel   (70005)       34 2023-01-03 13:42:37.000000 mxio-2023.1.23/MANIFEST.in
--rw-r--r--   0 michel   (70005) michel   (70005)      781 2023-04-24 16:33:03.096171 mxio-2023.1.23/PKG-INFO
--rw-rw-r--   0 michel   (70005) michel   (70005)      291 2021-12-13 19:32:22.000000 mxio-2023.1.23/README.md
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-04-24 16:33:03.095172 mxio-2023.1.23/mxio/
--rw-r--r--   0 michel   (70005) michel   (70005)    14620 2023-03-30 22:39:14.000000 mxio-2023.1.23/mxio/__init__.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-04-24 16:33:03.096171 mxio-2023.1.23/mxio/formats/
--rw-r--r--   0 michel   (70005) michel   (70005)        0 2023-01-03 13:42:37.000000 mxio-2023.1.23/mxio/formats/__init__.py
--rw-r--r--   0 michel   (70005) michel   (70005)    19491 2023-03-07 15:54:42.000000 mxio-2023.1.23/mxio/formats/cbf.py
--rw-r--r--   0 michel   (70005) michel   (70005)     6293 2023-02-07 18:27:33.000000 mxio-2023.1.23/mxio/formats/eiger.py
--rw-r--r--   0 michel   (70005) michel   (70005)     8739 2023-04-24 16:27:14.000000 mxio-2023.1.23/mxio/formats/hdf5.py
--rw-r--r--   0 michel   (70005) michel   (70005)     4588 2023-03-07 16:16:22.000000 mxio-2023.1.23/mxio/formats/mar345.py
--rw-r--r--   0 michel   (70005) michel   (70005)     2467 2023-03-07 16:32:14.000000 mxio-2023.1.23/mxio/formats/marccd.py
--rw-r--r--   0 michel   (70005) michel   (70005)     3464 2023-04-24 16:22:59.000000 mxio-2023.1.23/mxio/formats/nexus.py
--rw-r--r--   0 michel   (70005) michel   (70005)     4037 2023-03-08 19:35:33.000000 mxio-2023.1.23/mxio/formats/raxis.py
--rw-r--r--   0 michel   (70005) michel   (70005)     3550 2023-01-13 13:36:56.000000 mxio-2023.1.23/mxio/formats/smv.py
--rw-rw-r--   0 michel   (70005) michel   (70005)     2715 2021-12-13 19:32:22.000000 mxio-2023.1.23/mxio/log.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-04-24 16:33:03.096171 mxio-2023.1.23/mxio/misc/
--rw-rw-r--   0 michel   (70005) michel   (70005)        0 2022-01-28 15:58:04.000000 mxio-2023.1.23/mxio/misc/__init__.py
--rw-rw-r--   0 michel   (70005) michel   (70005)     4600 2022-01-28 15:58:04.000000 mxio-2023.1.23/mxio/misc/bshuf.py
--rw-r--r--   0 michel   (70005) michel   (70005)     8175 2023-01-11 14:07:36.000000 mxio-2023.1.23/mxio/parser.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-04-24 16:33:03.095172 mxio-2023.1.23/mxio.egg-info/
--rw-rw-r--   0 michel   (70005) michel   (70005)      781 2023-04-24 16:33:03.000000 mxio-2023.1.23/mxio.egg-info/PKG-INFO
--rw-rw-r--   0 michel   (70005) michel   (70005)      579 2023-04-24 16:33:03.000000 mxio-2023.1.23/mxio.egg-info/SOURCES.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)        1 2023-04-24 16:33:03.000000 mxio-2023.1.23/mxio.egg-info/dependency_links.txt
--rw-r--r--   0 michel   (70005) michel   (70005)      199 2023-04-24 16:33:03.000000 mxio-2023.1.23/mxio.egg-info/entry_points.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)      151 2023-04-24 16:33:03.000000 mxio-2023.1.23/mxio.egg-info/requires.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)       11 2023-04-24 16:33:03.000000 mxio-2023.1.23/mxio.egg-info/top_level.txt
--rw-r--r--   0 michel   (70005) michel   (70005)      144 2023-01-13 13:36:56.000000 mxio-2023.1.23/requirements.txt
--rw-r--r--   0 michel   (70005) michel   (70005)       38 2023-04-24 16:33:03.096171 mxio-2023.1.23/setup.cfg
--rw-r--r--   0 michel   (70005) michel   (70005)     1759 2023-01-12 17:53:06.000000 mxio-2023.1.23/setup.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-04-24 16:33:03.096171 mxio-2023.1.23/tests/
--rw-r--r--   0 michel   (70005) michel   (70005)        0 2022-12-21 15:26:38.000000 mxio-2023.1.23/tests/__init__.py
--rw-r--r--   0 michel   (70005) michel   (70005)     2776 2023-01-20 20:39:58.000000 mxio-2023.1.23/tests/formats.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-01-09 14:53:34.974144 mxio-2023.1.4/
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-01-09 14:53:34.973144 mxio-2023.1.4/.github/
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-01-09 14:53:34.973144 mxio-2023.1.4/.github/workflows/
+-rw-rw-r--   0 michel   (70005) michel   (70005)      865 2020-03-30 21:45:04.000000 mxio-2023.1.4/.github/workflows/pythonpublish.yml
+-rw-rw-r--   0 michel   (70005) michel   (70005)     1083 2020-03-30 21:07:43.000000 mxio-2023.1.4/LICENSE
+-rw-r--r--   0 michel   (70005) michel   (70005)       34 2023-01-03 13:42:37.000000 mxio-2023.1.4/MANIFEST.in
+-rw-r--r--   0 michel   (70005) michel   (70005)      780 2023-01-09 14:53:34.974144 mxio-2023.1.4/PKG-INFO
+-rw-rw-r--   0 michel   (70005) michel   (70005)      291 2021-12-13 19:32:22.000000 mxio-2023.1.4/README.md
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-01-09 14:53:34.974144 mxio-2023.1.4/mxio/
+-rw-r--r--   0 michel   (70005) michel   (70005)    11806 2023-01-05 20:49:56.000000 mxio-2023.1.4/mxio/__init__.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-01-09 14:53:34.974144 mxio-2023.1.4/mxio/formats/
+-rw-r--r--   0 michel   (70005) michel   (70005)        0 2023-01-03 13:42:37.000000 mxio-2023.1.4/mxio/formats/__init__.py
+-rw-r--r--   0 michel   (70005) michel   (70005)    18435 2023-01-03 13:42:37.000000 mxio-2023.1.4/mxio/formats/cbf.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     6254 2023-01-04 16:58:59.000000 mxio-2023.1.4/mxio/formats/eiger.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     7879 2023-01-05 21:28:19.000000 mxio-2023.1.4/mxio/formats/hdf5.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     2486 2023-01-06 21:48:54.000000 mxio-2023.1.4/mxio/formats/marccd.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     2962 2023-01-06 22:01:22.000000 mxio-2023.1.4/mxio/formats/nexus.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     3603 2023-01-03 13:42:37.000000 mxio-2023.1.4/mxio/formats/raxis.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     3544 2023-01-06 21:45:12.000000 mxio-2023.1.4/mxio/formats/smv.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)     2715 2021-12-13 19:32:22.000000 mxio-2023.1.4/mxio/log.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-01-09 14:53:34.974144 mxio-2023.1.4/mxio/misc/
+-rw-rw-r--   0 michel   (70005) michel   (70005)        0 2022-01-28 15:58:04.000000 mxio-2023.1.4/mxio/misc/__init__.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)     4600 2022-01-28 15:58:04.000000 mxio-2023.1.4/mxio/misc/bshuf.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     4827 2023-01-03 13:42:37.000000 mxio-2023.1.4/mxio/parser.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-01-09 14:53:34.974144 mxio-2023.1.4/mxio.egg-info/
+-rw-rw-r--   0 michel   (70005) michel   (70005)      780 2023-01-09 14:53:34.000000 mxio-2023.1.4/mxio.egg-info/PKG-INFO
+-rw-rw-r--   0 michel   (70005) michel   (70005)      556 2023-01-09 14:53:34.000000 mxio-2023.1.4/mxio.egg-info/SOURCES.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)        1 2023-01-09 14:53:34.000000 mxio-2023.1.4/mxio.egg-info/dependency_links.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)      170 2023-01-09 14:53:34.000000 mxio-2023.1.4/mxio.egg-info/entry_points.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)      145 2023-01-09 14:53:34.000000 mxio-2023.1.4/mxio.egg-info/requires.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)       11 2023-01-09 14:53:34.000000 mxio-2023.1.4/mxio.egg-info/top_level.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)      138 2023-01-03 13:42:37.000000 mxio-2023.1.4/requirements.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)       38 2023-01-09 14:53:34.974144 mxio-2023.1.4/setup.cfg
+-rw-r--r--   0 michel   (70005) michel   (70005)     1715 2023-01-03 13:42:37.000000 mxio-2023.1.4/setup.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-01-09 14:53:34.974144 mxio-2023.1.4/tests/
+-rw-r--r--   0 michel   (70005) michel   (70005)        0 2022-12-21 15:26:38.000000 mxio-2023.1.4/tests/__init__.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     1624 2023-01-03 13:42:37.000000 mxio-2023.1.4/tests/formats.py
```

### Comparing `mxio-2023.1.23/.github/workflows/pythonpublish.yml` & `mxio-2023.1.4/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `mxio-2023.1.23/LICENSE` & `mxio-2023.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mxio-2023.1.23/PKG-INFO` & `mxio-2023.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxio
-Version: 2023.1.23
+Version: 2023.1.4
 Summary: A Simple X-ray Area Detector Data IO Library
 Home-page: https://github.com/michel4j/mxio
 Author: Michel Fodje
 Author-email: michel4j@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mxio-2023.1.23/mxio/__init__.py` & `mxio-2023.1.4/mxio/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,35 +31,26 @@
     'read_image',
     'read_header',
     'XYPair',
     'HeaderAttrs',
     'ImageFrame',
     'DataSetAttrs',
     'DataSet',
-    'Geometry',
 ]
 
 class UnknownDataFormat(Exception):
     ...
 
 
 @dataclass
 class XYPair:
     x: Union[int, float]
     y: Union[int, float]
 
 
-@dataclass
-class Geometry:
-    detector: Tuple[Tuple[float, float, float], Tuple[float, float, float]] = ((1., 0., 0.), (0., 1., 0.))
-    goniometer: Tuple[float, float, float] = (1., 0., 0.)
-    beam: Tuple[float, float, float] = (0., 0., 1.)
-    polarization: Tuple[float, float, float] = (0., 1., 0.)
-
-
 class HeaderAttrs(TypedDict):
     detector: str
     serial_number: str
     format: str
     filename: str
     pixel_size: XYPair
     center: XYPair
@@ -67,15 +58,14 @@
     distance: float
     two_theta: float
     exposure: float
     wavelength: float
     start_angle: float
     delta_angle: float
     cutoff_value: float
-    geometry: Geometry
     maximum: float
     minimum: float
     sigma: float
     average: float
     overloads: int
     sensor_thickness: float
 
@@ -91,15 +81,14 @@
     distance: float
     two_theta: float
     exposure: float
     wavelength: float
     start_angle: float
     delta_angle: float
     cutoff_value: float = field(repr=False)
-    geometry: Geometry = field(repr=False)
     serial_number: str = field(repr=False, default='00-000')
     maximum: Optional[float] = field(repr=False, default=0.0)
     minimum: Optional[float] = field(repr=False, default=0.0)
     average: Optional[float] = field(repr=False, default=0.0)
     sigma: Optional[float] = field(repr=False, default=1.0)
     overloads: Optional[int] = field(repr=False, default=0)
     sensor_thickness: Optional[float] = field(repr=False, default=0.0)
@@ -120,15 +109,14 @@
     directory: Path
     series: ArrayLike
     identifier: str
     template: str
     reference: str
     glob: str
     index: int
-    geometry: Geometry
     size: int
     tags: Tuple[str, ...]
     frame: Union[ImageFrame, None]
 
     def __init__(
             self, file_path: Union[PathLike, str, None] = None,
             tags: Tuple[str, ...] = (),
@@ -138,15 +126,14 @@
         self.directory = Path()
         self.series = numpy.array([])
         self.template = ""
         self.reference = ""
         self.index = 0
         self.size = 0
         self.tags = tags
-        self.frame = None
 
         if file_path is not None:
             file_path = Path(file_path).absolute()
             self.reference = file_path.name
             self.directory = file_path.parent
             self.setup()
         elif attrs is not None:
@@ -169,47 +156,62 @@
 
     def setup(self):
         """
         Find dataset sweeps corresponding to this dataset on disk and update the attributes,
         'name', 'index', 'regex', 'template', 'frame' and 'sweeps'
         """
 
-        params = find_sweep(self.directory / self.reference)
-        pattern = params['pattern']
-        if pattern:
+        pattern = re.compile(
+            r'^(?P<name>[\w_-]+?)(?P<separator>[._-]?)'
+            r'(?P<field>\d{3,12})(?P<extension>(?:\.\D\w+)?)$'
+        )
+        matched = pattern.match(self.reference)
+        if matched:
+            params = matched.groupdict()
+            width = len(params['field'])
+            name = params['name']
+            index = int(params['field'])
+            template = '{name}{separator}{{field:>0{width}}}{extension}'.format(width=width, **params)
+            frame_pattern = re.compile(
+                r'^{name}{separator}(\d{{{width}}}){extension}$'.format(width=width, **params)
+            )
+            glob = '{name}{separator}{wildcard}{extension}'.format(width=width, wildcard='?'*width, **params)
             frames = numpy.array([
-                int(frame_match.group(1)) for file_path in self.directory.iterdir()
-                for frame_match in [pattern.match(file_path.name)]
-                if file_path.is_file() and frame_match
+                int(frame_match.group(1)) for file_name in self.directory.iterdir()
+                for frame_match in [frame_pattern.match(file_name.name)]
+                if file_name.is_file() and frame_match
             ], dtype=int)
             frames.sort()
+
         else:
+            name = ""
+            index = 0
+            template = ""
+            glob = ""
             frames = numpy.array([])
 
-        self.name = params['name']
-        self.glob = params['glob']
-        self.index = params['index']
-        self.template = params['template']
+        self.name = name
+        self.glob = glob
+        self.index = index
+        self.template = template
         self.series = frames
         self.size = len(frames)
-
-        header, data = self.read_file(self.directory / self.reference)
-        self.set_frame(header, data, self.index)
+        self.frame = self.get_frame(self.index)
 
     @classmethod
     def save_frame(cls, file_path: Union[PathLike, str], frame: ImageFrame):
         """Save the image frame to disk.
 
         :param frame: ImageFrame to save to file
         :param file_path: full path to file
         """
         raise RuntimeWarning("This format does not support exporting")
 
     @classmethod
-    def new_from_file(cls, filename: Union[str, Path]) -> "DataSet":
+    def new_from_file(cls, filename: str) -> "DataSet":
         """Create and return an instance of a DataSet subclass providing the appropriate format
 
         :param filename: str
         :return: DataSet instance
         """
 
         test_path = Path(filename)
@@ -254,72 +256,48 @@
     def get_frame(self, index: int) -> Union[ImageFrame, None]:
         """
         Fetch and return a frame given an index
 
         :param index: Frame number
         :return: ImageFrame or None if no frame of the given number exists
         """
-        if index == self.index and self.frame is not None:
-            return self.frame
-        elif index in self.series:
+
+        if index in self.series:
             file_name = self.directory.joinpath(self.template.format(field=index))
             header, data = self.read_file(file_name)
             self.set_frame(header, data, index)
             return self.frame
 
-    def frames(self) -> ImageFrame:
-        """
-        A generator which yields frames from the dataset, updates the index parameter of the dataset each iteration
-        """
-        for index in self.series:
-            yield self.get_frame(index=index)
-
     def next_frame(self) -> Union[ImageFrame, None]:
         """
         Load and return the next Frame in the dataset. Also updates the current frame and index to this
         frame.
 
         :return: ImageFrame | None if there is no next frame in the sequence
         """
-        next_pos = numpy.searchsorted(self.series, self.index) + 1
-        if next_pos < len(self.series):
-            return self.get_frame(self.series[next_pos])
+        return self.get_frame(self.index + 1)
 
     def prev_frame(self) -> Union[ImageFrame, None]:
         """
         Load and return the previous Frame in the dataset. Also updates the current frame and index to this
         frame.
 
         :return: ImageFrame | None if there is no previous frame in the sequence
         """
-
-        prev_pos = numpy.searchsorted(self.series, self.index) - 1
-        if prev_pos >= 0:
-            return self.get_frame(self.series[prev_pos])
+        return self.get_frame(self.index - 1)
 
     def set_frame(self, header: HeaderAttrs, data: NDArray, index: int = 1):
         """
         Set the current frame and frame index directly from a frame instance.
 
         :param header: dictionary of header meta data
         :param data: Image array
         :param index: int Frame index, defaults ot 1 if not provided
         """
 
-        if 'geometry' not in header:
-            two_theta_radians = numpy.radians(header['two_theta'])
-            header['geometry'] = Geometry(
-                detector=(
-                    (1.0, 0.0, 0.0),
-                    (0.0, numpy.cos(two_theta_radians), -1 * numpy.sin(two_theta_radians)),
-                ),
-                beam=(0.0, 0.0, 1.0),
-                goniometer=(1.0, 0.0, 0.0)
-            )
-
         # calculate statistics if missing in header
         if any(key not in header for key in ("average", "minimum", "maximum", "overloads", "sigma")):
             w, h = numpy.array(data.shape) // 2
             quadrant_data = data[:h, :w]
             mask = (quadrant_data > 0)
             stats_data = quadrant_data[mask] if mask.sum() > 0 else quadrant_data
 
@@ -330,19 +308,18 @@
             sigma = numpy.sqrt(numpy.dot(residuals, residuals)/stats_data.size)
 
             header.update({
                 "maximum": maximum,
                 "average": average,
                 "minimum": minimum,
                 "sigma": sigma,
-                "overloads": 4*(data >= header['cutoff_value']).sum()
+                "overloads": (data >= header['cutoff_value']).sum()
             })
 
         frame = ImageFrame(**header, data=data)
-        self.geometry = frame.geometry
         self.frame = frame
         self.index = index
 
     def get_sweeps(self) -> Sequence[Tuple[int, int]]:
         """
         Compress an the frame series which is a sequence of ints into a sequence of tuple pairs representing
         contiguous ranges of values.
@@ -368,15 +345,15 @@
         :return:  Tuple[str, ...]
         """
         ...
 
     @abstractmethod
     def read_file(self, filename: Union[str, Path]) -> Tuple[HeaderAttrs, NDArray]:
         """
-        Read the file and return a header dictionary and a 2D array representing the image
+        Read
         :param filename: file to read
         :return: Tuple[dict, NDArray]
         """
         ...
 
 
 def read_image(path: str) -> Union[DataSet, None]:
@@ -397,59 +374,7 @@
     :param path: str
     """
 
     dset = DataSet.new_from_file(path)
     return asdict(dset.frame)
 
 
-def find_sweep(path: Path, name=r'[\w_-]+?') -> dict:
-    """
-    Find the disk representation of a dataset from a single frame in a series
-    :param path: full path to one image
-    :param name: optional raw regex string representing the root name of the dataset
-    :return: dictionary containing the "name", "index", "template", "glob" and compiled regex "pattern"
-    """
-
-    pattern = re.compile(
-        rf'^(?P<name>{name})'
-        r'(?P<separator>[._-]?)'
-        r'(?P<field>\d{3,12})'
-        r'(?P<extension>(?:\.\D\w+)?)$'
-    )
-    directory = path.parent
-    file_name = path.name
-
-    matched = pattern.match(file_name)
-    if matched:
-        params = matched.groupdict()
-        width = len(params['field'])
-        index = int(params['field'])
-        template = '{name}{separator}{{field:>0{width}}}{extension}'.format(width=width, **params)
-        frame_pattern = re.compile(
-            r'^{name}{separator}(\d{{{width}}}){extension}$'.format(width=width, **params)
-        )
-        glob = '{name}{separator}{wildcard}{extension}'.format(width=width, wildcard='?' * width, **params)
-        name = params['name']
-
-        # unusual frame names without field separator
-        if width > 6:
-            names = [
-                file_path.name for file_path in directory.iterdir()
-                if file_path.is_file() and frame_pattern.match(file_path.name)
-            ]
-            common_name = os.path.commonprefix(names)
-            return find_sweep(path, name=common_name)
-        else:
-            return {
-                'name': name,
-                'index': index,
-                'template': template,
-                'glob': glob,
-                'pattern': frame_pattern
-            }
-    return {
-        'name': file_name,
-        'index': 0,
-        'template': file_name,
-        'glob': file_name,
-        'pattern': ''
-    }
```

### Comparing `mxio-2023.1.23/mxio/formats/cbf.py` & `mxio-2023.1.4/mxio/formats/cbf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import ctypes as ct
 import os
-import sys
 import re
 from pathlib import Path
 from typing import Tuple, Union, BinaryIO
 
 import numpy
 from numpy.typing import ArrayLike
 
 from mxio import parser
-from mxio import DataSet, ImageFrame, XYPair, Geometry
+from mxio import DataSet, ImageFrame, XYPair
 
 __all__ = [
     "CBFDataSet"
 ]
 
 
 # Define CBF constants
@@ -78,24 +77,18 @@
     "unsigned 16-bit integer": numpy.dtype('u2'),
     "unsigned 32-bit integer": numpy.dtype('u4'),
     "signed 16-bit integer": numpy.dtype('i2'),
     "signed 32-bit integer": numpy.dtype('i4'),
     "unsigned 64-bit integer": numpy.dtype("i8")
 }
 
-BYTE_ORDERING = {
-    '>': 'big',
-    '<': 'little',
-    '=': sys.byteorder,
-}
-
 HEADER_SPECS = {
     "SLS_1.0": {
         "fields": [
-            "# Detector: <str:detector> SN: <slug:serial_number>",
+            "# Detector: <str:detector>, SN <slug:serial_number>, <str:beamline>",
             "# Pixel_size <float:pixel_size> m x <float:pixel_size> m",
             "# Exposure_period <float:exposure> s",
             "# Count_cutoff <int:cutoff_value> counts",
             "# Wavelength <float:wavelength> A",
             "# Detector_distance <float:distance> m",
             "# Beam_xy (<float:center>, <float:center>) pixels",
             "# Start_angle <float:start_angle> deg",
@@ -117,15 +110,14 @@
             '# Angle_increment <float:delta_angle> deg.',
             '# Detector_2theta <float:two_theta> deg.',
             '# Silicon sensor, thickness <float:sensor_thickness> m'
         ]
     }
 }
 
-
 def unit_vector(vector):
     """ Returns the unit vector of the vector.  """
     return vector / numpy.linalg.norm(vector)
 
 
 cbflib = ct.cdll.LoadLibrary('libcbf.so.0')
 libc = ct.cdll.LoadLibrary('libc.so.6')
@@ -169,22 +161,14 @@
 ]
 cbflib.cbf_get_image_size.argtypes = [
     ct.c_void_p, ct.c_uint, ct.c_uint, ct.POINTER(ct.c_size_t), ct.POINTER(ct.c_size_t)
 ]
 cbflib.cbf_get_detector_normal.argtypes = [
     ct.c_void_p, ct.POINTER(ct.c_double), ct.POINTER(ct.c_double), ct.POINTER(ct.c_double)
 ]
-
-cbflib.cbf_get_detector_axis_slow.argtypes = [
-    ct.c_void_p,  ct.POINTER(ct.c_double), ct.POINTER(ct.c_double), ct.POINTER(ct.c_double),
-]
-cbflib.cbf_get_detector_axis_fast.argtypes =[
-    ct.c_void_p,  ct.POINTER(ct.c_double), ct.POINTER(ct.c_double), ct.POINTER(ct.c_double),
-]
-
 cbflib.cbf_get_rotation_axis.argtypes = [
     ct.c_void_p, ct.c_uint, ct.POINTER(ct.c_double), ct.POINTER(ct.c_double), ct.POINTER(ct.c_double)
 ]
 cbflib.cbf_get_image.argtypes = [
     ct.c_void_p, ct.c_uint, ct.c_uint, ct.c_void_p, ct.c_size_t, ct.c_int, ct.c_size_t, ct.c_size_t
 ]
 cbflib.cbf_parse_mimeheader.argtypes = [
@@ -202,15 +186,15 @@
 ]
 
 
 class CBFDataSet(DataSet):
 
     @classmethod
     def identify(cls, file: BinaryIO, extension: str) -> Tuple[str, ...]:
-        magic = b'###CBF: '
+        magic = b'###CBF: VERSION'
         if file.read(len(magic)) == magic:
             return "CBF Area Detector Image",
 
     @classmethod
     def save_frame(cls, file_path: Union[os.PathLike, str], frame: ImageFrame):
         header_text = (
             f"\n"
@@ -251,17 +235,17 @@
         data = ct.create_string_buffer(frame.data.tobytes())
         cbflib.cbf_set_integerarray_wdims(
             cbf_data,
             Flags.BYTE_OFFSET,
             1,  # binary id
             ct.byref(data),
             ct.c_size_t(frame.data.itemsize),
-            int(frame.data.dtype.kind == 'i'),  # signed
+            0,  # signed
             frame.size.x * frame.size.y,
-            "{}_endian".format(BYTE_ORDERING.get(frame.data.dtype.byteorder, 'little')).encode("utf-8"),
+            b"little_endian",
             ct.c_size_t(frame.size.x),
             ct.c_size_t(frame.size.y),
             0,
             0
         )
         cbflib.cbf_write_file(cbf_data, file_pointer, 1, 0, Flags.MSG_DIGEST | Flags.MIME_HEADERS | Flags.PAD_4K, 0)
         cbflib.cbf_free_handle(cbf_data)
@@ -325,19 +309,19 @@
         result = cbflib.cbf_get_wavelength(handle, ct.byref(wavelength))
         header['wavelength'] = wavelength.value
 
         x_size = ct.c_size_t(mime_header.get('X-Binary-Size-Fastest-Dimension', 0))
         y_size = ct.c_size_t(mime_header.get('X-Binary-Size-Second-Dimension', 0))
         header['size'] = XYPair(x_size.value, y_size.value)
 
-        pixel_size = ct.c_double(0.1)
+        pixel_size = ct.c_double(1.0)
         result |= cbflib.cbf_get_pixel_size(handle, 0, 1, ct.byref(pixel_size))
         header['pixel_size'] = XYPair(pixel_size.value, pixel_size.value)
 
-        distance = ct.c_double(250.0)
+        distance = ct.c_double(999.0)
         result |= cbflib.cbf_get_detector_distance(detector, ct.byref(distance))
         header['distance'] = distance.value
 
         x_center, y_center = ct.c_double(0.0), ct.c_double(0.0)
         ix, iy = ct.c_double(x_size.value / 2.0), ct.c_double(y_size.value / 2.0)
         result |= cbflib.cbf_get_beam_center(detector, ct.byref(ix), ct.byref(iy), ct.byref(x_center),
                                              ct.byref(y_center))
@@ -352,70 +336,55 @@
         header['start_angle'] = start_angle.value
         header['delta_angle'] = delta_angle.value
 
         ovl = ct.c_double()
         result |= cbflib.cbf_get_overload(handle, 0, ct.byref(ovl))
         header['cutoff_value'] = ovl.value
 
-        gonio_x, gonio_y, gonio_z = ct.c_double(1.0), ct.c_double(0.0), ct.c_double(0.0)
-        xaxis_x, xaxis_y, xaxis_z = ct.c_double(1.0), ct.c_double(0.0), ct.c_double(0.0)
-        yaxis_x, yaxis_y, yaxis_z = ct.c_double(0.0), ct.c_double(1.0), ct.c_double(0.0)
-        result |= cbflib.cbf_get_detector_axis_fast(detector, ct.byref(xaxis_x), ct.byref(xaxis_y), ct.byref(xaxis_z))
-        result |= cbflib.cbf_get_detector_axis_slow(detector, ct.byref(yaxis_x), ct.byref(yaxis_y), ct.byref(yaxis_z))
-        result |= cbflib.cbf_get_rotation_axis(goniometer, 0, ct.byref(gonio_x), ct.byref(gonio_y), ct.byref(gonio_x))
-
-        geometry = Geometry(
-            detector=(
-                (xaxis_x.value, xaxis_y.value, xaxis_z.value),
-                (yaxis_x.value, yaxis_y.value, yaxis_z.value)
-            ),
-            goniometer=(gonio_x.value, gonio_y.value, gonio_z.value),
-            beam=(0.0, 0.0, 1.0),
-        )
-
-        detector_norm = numpy.cross(geometry.detector[0], geometry.detector[1])
-        two_theta_radians = numpy.arccos(numpy.dot(detector_norm, geometry.beam))
-
-        header['geometry'] = geometry
-        header['two_theta'] = numpy.degrees(two_theta_radians)
+        # FIXME Calculate actual two_theta from the beam direction and detector normal
+        # vec_x, vec_y, vec_z = ct.c_double(0.0), ct.c_double(0.0), ct.c_double(0.0)
+        # result |= cbflib.cbf_get_detector_normal(detector, ct.byref(vec_x), ct.byref(vec_y), ct.byref(vec_x))
+        # detector_norm = numpy.array([vec_x.value, vec_y.value, vec_z.value])
+        #
+        # result |= cbflib.cbf_get_rotation_axis(goniometer, 0, ct.byref(vec_x), ct.byref(vec_y), ct.byref(vec_x))
+        # rot_axis = numpy.array([vec_x.value, vec_y.value, vec_z.value])
+        # header['two_theta'] = 0.0
 
         detector_name = ct.c_char_p()
         result |= cbflib.cbf_get_detector_id(handle, 0, ct.byref(detector_name))
-        header['detector'] = detector_name.value.decode('utf-8') if detector_name.value else "UNKNOWN"
+        header['detector'] = detector_name.value if detector_name.value else "UNKNOWN"
 
-        # handle mini-cbf files
-        if header['delta_angle'] == 0.0 and header['exposure'] == 0.0:
+        # handle XDS Special cbf files
+        if header['distance'] == 999.0 and header['delta_angle'] == 0.0 and header['exposure'] == 0.0:
             mini_cbf_type = ct.c_char_p()
             mini_cbf_header = ct.c_char_p()
 
             result = cbflib.cbf_select_datablock(handle, ct.c_uint(0))
             result |= cbflib.cbf_find_category(handle, b"array_data")
             result |= cbflib.cbf_find_column(handle, b"header_convention")
             result |= cbflib.cbf_get_value(handle, ct.byref(mini_cbf_type))
             result |= cbflib.cbf_find_column(handle, b"header_contents")
             result |= cbflib.cbf_get_value(handle, ct.byref(mini_cbf_header))
 
             if result == 0 and mini_cbf_type.value != b'XDS special':
                 specs = HEADER_SPECS[mini_cbf_type.value.decode('utf-8')]
-                info = parser.parse_text(specs, mini_cbf_header.value.decode('utf-8'))
+                info = parser.parse_section(specs, mini_cbf_header.value.decode('utf-8'))
                 pixel_size = list(map(lambda v: v * 1000, info['pixel_size']))
                 header['detector'] = info['detector'].strip()
+                header['two_theta'] = 0 if not info['two_theta'] else round(info['two_theta'], 2)
                 header['pixel_size'] = XYPair(*pixel_size)
                 header['exposure'] = info['exposure']
                 header['wavelength'] = info['wavelength']
                 header['distance'] = info['distance'] * 1000
                 header['center'] = XYPair(*info['center'])
                 header['start_angle'] = info['start_angle']
                 header['delta_angle'] = info['delta_angle']
                 header['cutoff_value'] = info['cutoff_value']
                 header['sensor_thickness'] = info['sensor_thickness'] * 1000
 
-                if 'two_theta' in info:
-                    header['two_theta'] = round(info['two_theta'], 2)
-
         data_type = DATA_TYPES[mime_header.get('X-Binary-Element-Type', 'signed 32-bit integer')]
         element_size = data_type.itemsize
         num_elements = header['size'].x * header['size'].y
         data = ct.create_string_buffer(num_elements * element_size)
         result = cbflib.cbf_get_image(handle, 0, 0, ct.byref(data), element_size, 1, header['size'].x, header['size'].y)
         if result != 0:
             # MiniCBF
```

### Comparing `mxio-2023.1.23/mxio/formats/eiger.py` & `mxio-2023.1.4/mxio/formats/eiger.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             'exposure': self.global_header['exposure'],
             'cutoff_value': 2.8e6, #self.global_header['count_cutoff'],
             'filename': self.name,
             'wavelength': self.global_header['wavelength'],
             'distance': self.global_header['distance'],
             'center': XYPair(*self.global_header['center']),
             'start_angle': self.global_header['start_angle'] + index * self.global_header['delta_angle'],
-            'delta_angle': self.global_header['delta_angle'],
+            'delta_angle': 0.0,
             'sensor_thickness': self.global_header['sensor_thickness'],
         }
 
 
         try:
             if metadata['encoding'].startswith('lz4'):
                 arr_bytes = lz4.block.decompress(img_data, uncompressed_size=size * data_type.itemsize)
@@ -158,19 +158,18 @@
     """
     Proxies the PUSH/PULL Stream from address and publishes it as a PUB/SUB Stream through port.
     This allows multiple ZMQ clients to access the same data.
     """
 
     context = zmq.Context()
     backend = context.socket(zmq.PULL)
+    backend.connect(address)
     frontend = context.socket(zmq.PUB)
+    frontend.bind(f"tcp://*:{port}")
 
     try:
-        backend.connect(address)
-        frontend.bind(f"tcp://*:{port}")
-
         print(f'Starting ZMQ PULL Multiplexer proxying messages from {address} to {port} ...')
         zmq.device(zmq.STREAMER, frontend, backend)
     finally:
         frontend.close()
         backend.close()
         context.term()
```

### Comparing `mxio-2023.1.23/mxio/formats/hdf5.py` & `mxio-2023.1.4/mxio/formats/hdf5.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from __future__ import annotations
 
 import re
 
 from pathlib import Path
-from typing import Tuple, Union, Dict, Any, BinaryIO
+from typing import Tuple, Union, Sequence, Any, BinaryIO
 
 import h5py
 import hdf5plugin
 import numpy
-from numpy.typing import NDArray, ArrayLike
+from numpy.typing import NDArray
 
-from mxio import DataSet, XYPair, Geometry
+from mxio import DataSet, XYPair
 
 __all__ = [
     "HDF5DataSet",
     "hdf5_file_parts",
     "CONVERTERS",
     "NUMBER_FORMATS"
 ]
@@ -65,18 +64,19 @@
     else:
         return 1, image_path.name, image_path.parent
 
 
 class HDF5DataSet(DataSet):
 
     file: h5py.File
-    data_sections: Dict[str, range]
+    data_sections: Sequence[str]
+    max_section_size: int
     format: str
     omega_field: str = '/entry/sample/goniometer/omega'
-    array_fields: tuple = ('two_theta', 'omega', 'chi', 'phi', 'kappa', 'geometry')
+    array_fields: tuple = ('two_theta', 'omega', 'chi', 'phi', 'kappa')
     header_fields: dict = {
         'detector': '/entry/instrument/detector/description',
         'serial_number': '/entry/instrument/detector/detector_number',
         'two_theta': '/entry/instrument/detector/goniometer/two_theta',
         'pixel_size': (
             '/entry/instrument/detector/x_pixel_size',
             '/entry/instrument/detector/y_pixel_size',
@@ -90,24 +90,21 @@
         ),
         'cutoff_value': '/entry/instrument/detector/detectorSpecific/countrate_correction_count_cutoff',
         'sensor_thickness': '/entry/instrument/detector/sensor_thickness',
         'size': (
             '/entry/instrument/detector/detectorSpecific/x_pixels_in_detector',
             '/entry/instrument/detector/detectorSpecific/y_pixels_in_detector'
         ),
-        # 'geometry': (
-        #     '/entry/instrument/detector/geometry/orientation/value',
-        # )
     }
     oscillation_fields: dict = {
         'start': '/entry/sample/goniometer/{}',
         'delta': '/entry/sample/goniometer/{}_range_average'
     }
     format: str = 'HDF5'
-    start_angles: ArrayLike
+
 
     @classmethod
     def identify(cls, file: BinaryIO, extension: str) -> Tuple[str, ...]:
         magic = b'\211HDF\r\n\032\n'
         if file.read(len(magic)) == magic:
             return "HDF5 Area Detector Data",
 
@@ -123,36 +120,28 @@
             self.name = params['name']
             self.reference = f'{self.name}{params["separator"]}master.{params["extension"]}'
             self.template = f'{self.reference}/{{field:>06}}'
             self.glob = self.reference.replace('master', '??????')
 
         self.file = h5py.File(self.directory.joinpath(self.reference), 'r')
         self.format = 'HDF5'
-
-        # count frames from actual data arrays
-        frame_count = 0
-        section_keys = list(self.file['/entry/data'].keys())
-        self.data_sections = {}
-        for section in section_keys:
-            attrs = self.file[f'/entry/data/{section}'].attrs
-            self.data_sections[section] = range(attrs['image_nr_low'], attrs['image_nr_high']+1)
-            frame_count += len(self.data_sections[section])
-
+        frame_count = self.extract_field(self.omega_field, array=True).size
         self.series = numpy.arange(frame_count) + 1
         self.size = frame_count
+        self.data_sections = list(self.file['/entry/data'].keys())
+        self.max_section_size = int(numpy.ceil(frame_count / len(self.data_sections)))
         self.get_frame(self.index)
 
-    def extract_field(self, field: str, array: bool = False, index: slice | int = ()) -> Any:
+    def extract_field(self, field: str, array: bool = False, index: slice = ()) -> Any:
         """
         Extract an HDF5 field from the archive
         :param field: field path
         :param array: bool
         :param index: slice to extract a subset of a larger array
         """
-
         field_value = self.file[field]
         raw_value = field_value[index]
         if field_value.shape == () and array:
             raw_value = numpy.array([raw_value])
         return raw_value
 
     def parse_header(self, header_fields: dict, oscillation_fields: dict):
@@ -172,61 +161,46 @@
                 pass
 
         for axis in ['omega', 'phi', 'chi', 'kappa']:
             try:
                 start_angles = self.extract_field(oscillation_fields['start'].format(axis), array=True)
                 value_varies = (start_angles.mean() != 0.0 and numpy.diff(start_angles).sum() != 0)
                 if len(start_angles) == 1 or value_varies:
-                    self.start_angles = start_angles
-
                     # found the right axis
                     for field, path in oscillation_fields.items():
                         header[f'{field}_angle'] = self.extract_field(path.format(axis), array=True)
 
-                    header['start_angle'] = float(start_angles[0])
+                    header['start_angle'] = float(header['start_angle'][0])
                     header['delta_angle'] = float(header['delta_angle'][0])
                     header['two_theta'] = 0.0
                     break
             except KeyError:
                 pass
 
         header['size'] = XYPair(*header["size"])
         header['pixel_size'] = XYPair(*header['pixel_size'])
         header['center'] = XYPair(*header["center"])
 
-        # detector_orientation = header['geometry'][0]
-        # header['geometry'] = Geometry(
-        #     detector=(tuple(detector_orientation[:3]), tuple(detector_orientation[3:])),
-        #     goniometer=(-1, 0, 0), beam=(0, 0, 1)
-        # )
-
         return header
 
     def read_file(self, filename: Union[str, Path]) -> Tuple[dict, NDArray]:
         index, reference, directory = hdf5_file_parts(filename)
         assert (reference, directory) == (self.reference, self.directory), "Invalid data archive"
         assert index in self.series, f"Frame {index} does not exist in this archive"
 
-        section_name, frame_index = "", -1
-        for name, frame_range in self.data_sections.items():
-            if index in frame_range:
-                section_name = name
-                frame_index = frame_range.index(index)
-                break
-
         header = self.parse_header(self.header_fields, self.oscillation_fields)
         header['format'] = self.format
-        header['start_angle'] = self.start_angles[index-1]
 
-        assert section_name in self.data_sections, f"Section not found"
+        section_index, frame_index = divmod(index, self.max_section_size)
+        assert section_index < len(self.data_sections), f"Section {section_index} does not exist"
+        section_name = self.data_sections[section_index]
 
         key = f'/entry/data/{section_name}'
         link = self.file.get(key, getlink=True)
         section_file = link.filename
         path = self.directory.joinpath(section_file)
 
         assert path.exists(), f"External data link file {section_file} could not be found"
-        raw_data = self.extract_field(key, array=True, index=frame_index)
-        data = raw_data.view(NUMBER_FORMATS[str(raw_data.dtype)])
+        data = self.extract_field(key, array=True, index=frame_index)
 
-        return header, data
+        return header, data.view(NUMBER_FORMATS[str(data.dtype)])
```

### Comparing `mxio-2023.1.23/mxio/formats/marccd.py` & `mxio-2023.1.4/mxio/formats/marccd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import os
 import cv2
 import math
 import struct
-import numpy
-
 from pathlib import Path
 from typing import Tuple, Union, BinaryIO
 from numpy.typing import NDArray
 
-from mxio import DataSet, XYPair, Geometry
+from mxio import DataSet, XYPair
 
 __all__ = [
     "MarCCDDataSet"
 ]
 
 
 class MarCCDDataSet(DataSet):
@@ -24,42 +22,42 @@
         if file.read(len(magic)) == magic:
             return "MAR Area Detector Image",
 
     def read_file(self, filename: Union[str, Path]) -> Tuple[dict, NDArray]:
         # Read MarCCD header
         header_format = 'I16s39I80x'  # 256 bytes
         statistics_format = '3Q7I9I40x128H'  # 128 + 256 bytes
-        gonio_format = '28i16x'  # 128 bytes
+        goniostat_format = '28i16x'  # 128 bytes
         detector_format = '5i9i9i9i'  # 128 bytes
         source_format = '10i16x10i32x'  # 128 bytes
 
         with open(Path(filename), 'rb') as file:
             file.seek(1024)
             header_fields = struct.unpack(header_format, file.read(256))
             statistics_fields = struct.unpack(statistics_format, file.read(128 + 256))
-            gonio_fields = struct.unpack(gonio_format, file.read(128))
+            goniostat_fields = struct.unpack(goniostat_format, file.read(128))
             detector_fields = struct.unpack(detector_format, file.read(128))
             source_fields = struct.unpack(source_format, file.read(128))
 
         header = {
             'pixel_size': XYPair(detector_fields[1] / 1e6, detector_fields[1] / 1e6),
-            'center': XYPair(gonio_fields[1] / 1e3, gonio_fields[2] / 1e3),
+            'center': XYPair(goniostat_fields[1] / 1e3, goniostat_fields[2] / 1e3),
             'size': XYPair(header_fields[17], header_fields[18]),
-            'distance': gonio_fields[0] / 1e3,
-            'two_theta': (gonio_fields[7] / 1e3) * math.pi / -180.0,
-            'exposure': gonio_fields[4] / 1e3,
+            'distance': goniostat_fields[0] / 1e3,
+            'two_theta': (goniostat_fields[7] / 1e3) * math.pi / -180.0,
+            'exposure': goniostat_fields[4] / 1e3,
             'wavelength': source_fields[3] / 1e5,
-            'start_angle': gonio_fields[(7 + gonio_fields[23])] / 1e3,
-            'delta_angle': gonio_fields[24] / 1e3,
+            'start_angle': goniostat_fields[(7 + goniostat_fields[23])] / 1e3,
+            'delta_angle': goniostat_fields[24] / 1e3,
             'minimum': statistics_fields[3],
             'maximum': statistics_fields[4],
             'average': statistics_fields[5] / 1e3,
             'overloads': statistics_fields[8],
             'cutoff_value': header_fields[23],
-            'filename': os.path.basename(filename),
+            'filename': os.path.basename(filename)
         }
 
         det_mm = int(round(header['pixel_size'].x * header['size'].x))
         header['detector'] = f'Rayonix MX{det_mm:d}'
         header['format'] = 'TIFF'
 
         data = cv2.imread(str(filename), -1)
```

### Comparing `mxio-2023.1.23/mxio/formats/raxis.py` & `mxio-2023.1.4/mxio/formats/raxis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy
 import struct
 from pathlib import Path
 from typing import Tuple, Union, BinaryIO
 from numpy.typing import NDArray
 
-from mxio import DataSet, XYPair, Geometry
+from mxio import DataSet, XYPair
 
 __all__ = [
     "RAXISDataSet"
 ]
 
 HEADER_SPECS = {
     "instrument": '10s',
@@ -81,22 +81,23 @@
 
     def read_file(self, filename: Union[str, Path]) -> Tuple[dict, NDArray]:
         # Read RAXIS header
         with open(Path(filename), 'rb') as file:
             # detect endianness
             file.seek(796)
             endian_test = struct.unpack('>l', file.read(struct.calcsize('>l')))[0]
-            endian = '>' if endian_test < 20 else '<'
+            endian = '>' if endian_test < 20 else '>'
             file.seek(0)
 
             info = {
                 key: struct.unpack(f"{endian}{format_str}", file.read(struct.calcsize(f"{endian}{format_str}")))
                 for key, format_str in HEADER_SPECS.items()
             }
-            data_type = numpy.dtype('u2')
+            data_type = numpy.dtype(f'{endian}u2')
+
             header = {
                 'format': 'RAXIS',
                 'filename': os.path.basename(filename),
                 'pixel_size': XYPair(*info['pixel_size']),
                 'center': XYPair(*info['center']),
                 'size': XYPair(*info['size']),
                 'distance': info['distance'][0],
@@ -105,26 +106,18 @@
                 'wavelength': info['wavelength'][0],
                 'start_angle': info['start_angle'][0],
                 'delta_angle': info['end_angle'][0] - info['start_angle'][0],
                 'detector': info['instrument'][0].decode('utf-8').strip(),
                 'cutoff_value': int(2 ** (8 * data_type.itemsize) - 1)
             }
 
-            gonio_axis = tuple(numpy.reshape(info['gonio_axes'], (-1, 3))[info['scan_axis']])
-            header['geometry'] = Geometry(
-                detector=(
-                    (0.0, -1.0, 0.0),
-                    (numpy.cos(numpy.radians(header['two_theta'])), 0.0, numpy.sin(numpy.radians(header['two_theta']))),
-                ),
-                goniometer=gonio_axis, beam=(0.0, 0.0, 1.0),  polarization=(1.0, 0.0, 0.0)
-            )
             num_elements = header['size'].x * header['size'].y
             data_size = num_elements * data_type.itemsize
             file.seek(-data_size, 2)
             raw_data = file.read(data_size)
 
         data = numpy.frombuffer(raw_data, dtype=data_type).reshape(header['size'].y, header['size'].x)
-        if endian == '>':
+        if data_type.byteorder == '>':
             data = data.byteswap()
 
         return header, data
```

### Comparing `mxio-2023.1.23/mxio/formats/smv.py` & `mxio-2023.1.4/mxio/formats/smv.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,16 +39,16 @@
             pattern = re.compile(r'\n(?P<key>\w+)=(?P<value>.+);')
             info = {
                 match.groupdict()['key'].lower(): match.groupdict()['value'].strip()
                 for match in pattern.finditer(header_text)
             }
 
             data_type_str = DATA_TYPES[info.get('type', "unsigned_short")]
-            endian = '>' if info.get("byte_order") == 'big_endian' else '<'
-            data_type = numpy.dtype(f'{data_type_str}')
+            endian_suffix = '>' if info.get("byte_order") == 'big_endian' else '<'
+            data_type = numpy.dtype(f'{endian_suffix}{data_type_str}')
             pixel_size = float(info['pixel_size'])
             x_center = float(info['beam_center_x']) / pixel_size
             y_center = float(info['beam_center_y']) / pixel_size
 
             header['delta_angle'] = float(info['osc_range'])
             header['distance'] = float(info['distance'])
             header['wavelength'] = float(info['wavelength'])
@@ -62,15 +62,14 @@
             header['cutoff_value'] = int(info.get('ccd_image_saturation', 2 ** (8 * data_type.itemsize) - 1))
 
             header['detector'] = {
                 (2048, 0.050): 'ADSC Q105',
                 (2048, 0.102): 'ADSC Q210',
                 (4096, 0.051): 'ADSC Q210',
                 (2304, 0.082): 'ADSC Q4',
-                (1152, 0.163): 'ADSC Q4',
                 (3072, 0.103): 'ADSC Q315',
                 (6144, 0.051): 'ADSC Q315',
                 (2048, 0.078): 'NOIR-1',
                 (1500, 0.200): 'RAXIS4',
                 (3000, 0.100): 'RAXIS4',
                 (6000, 0.050): 'RAXIS4',
                 (1024, 0.090): 'SATURN 92',
@@ -82,10 +81,11 @@
             num_elements = header['size'].x * header['size'].y
             data_size = num_elements * data_type.itemsize
             file.seek(0)
             file.read(header_size)
             raw_data = file.read(data_size)
 
         data = numpy.frombuffer(raw_data, dtype=data_type).reshape(header['size'].y, header['size'].x)
-        if endian == '>':
+        if data_type.byteorder == '>':
             data = data.byteswap()
+
         return header, data
```

### Comparing `mxio-2023.1.23/mxio/log.py` & `mxio-2023.1.4/mxio/log.py`

 * *Files identical despite different names*

### Comparing `mxio-2023.1.23/mxio/misc/bshuf.py` & `mxio-2023.1.4/mxio/misc/bshuf.py`

 * *Files identical despite different names*

### Comparing `mxio-2023.1.23/mxio.egg-info/PKG-INFO` & `mxio-2023.1.4/mxio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxio
-Version: 2023.1.23
+Version: 2023.1.4
 Summary: A Simple X-ray Area Detector Data IO Library
 Home-page: https://github.com/michel4j/mxio
 Author: Michel Fodje
 Author-email: michel4j@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mxio-2023.1.23/mxio.egg-info/SOURCES.txt` & `mxio-2023.1.4/mxio.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 mxio.egg-info/entry_points.txt
 mxio.egg-info/requires.txt
 mxio.egg-info/top_level.txt
 mxio/formats/__init__.py
 mxio/formats/cbf.py
 mxio/formats/eiger.py
 mxio/formats/hdf5.py
-mxio/formats/mar345.py
 mxio/formats/marccd.py
 mxio/formats/nexus.py
 mxio/formats/raxis.py
 mxio/formats/smv.py
 mxio/misc/__init__.py
 mxio/misc/bshuf.py
 tests/__init__.py
```

### Comparing `mxio-2023.1.23/setup.py` & `mxio-2023.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         'mxio.plugins': [
             'CBF = mxio.formats.cbf',
             'HDF5 = mxio.formats.hdf5',
             'MARCCD = mxio.formats.marccd',
             'RAXIS = mxio.formats.raxis',
             'SMV = mxio.formats.smv',
             'NEXUS = mxio.formats.nexus',
-            'MAR345 = mxio.formats.mar345',
         ]
     },
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

