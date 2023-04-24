# Comparing `tmp/SfMLearner_installable-1.0.0.tar.gz` & `tmp/SfMLearner_installable-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SfMLearner_installable-1.0.0.tar", last modified: Sun Apr 23 23:05:37 2023, max compression
+gzip compressed data, was "SfMLearner_installable-1.0.1.tar", last modified: Mon Apr 24 01:00:22 2023, max compression
```

## Comparing `SfMLearner_installable-1.0.0.tar` & `SfMLearner_installable-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 23:05:37.002357 SfMLearner_installable-1.0.0/
--rw-rw-rw-   0        0        0     1090 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     8268 2023-04-23 23:05:37.000355 SfMLearner_installable-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7533 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.900357 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/
--rw-rw-rw-   0        0        0     8268 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.906356 SfMLearner_installable-1.0.0/data/
--rw-rw-rw-   0        0        0        0 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.959355 SfMLearner_installable-1.0.0/data/cityscapes/
--rw-rw-rw-   0        0        0        0 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/cityscapes/__init__.py
--rw-rw-rw-   0        0        0     5220 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/cityscapes/cityscapes_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.981358 SfMLearner_installable-1.0.0/data/kitti/
--rw-rw-rw-   0        0        0        0 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/kitti/__init__.py
--rw-rw-rw-   0        0        0     6338 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/kitti/kitti_odom_loader.py
--rw-rw-rw-   0        0        0     6338 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/kitti/kitti_raw_loader.py
--rw-rw-rw-   0        0        0     4693 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/data/prepare_train_data.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.997360 SfMLearner_installable-1.0.0/kitti_eval/
--rw-rw-rw-   0        0        0        0 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/__init__.py
--rw-rw-rw-   0        0        0     7651 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/depth_evaluation_utils.py
--rw-rw-rw-   0        0        0     3585 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/eval_depth.py
--rw-rw-rw-   0        0        0      989 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/eval_pose.py
--rw-rw-rw-   0        0        0    13974 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/pose_evaluation_utils.py
--rw-rw-rw-   0        0        0       42 2023-04-23 23:05:37.002357 SfMLearner_installable-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3944 2023-04-23 23:05:31.000000 SfMLearner_installable-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:00:22.992520 SfMLearner_installable-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     8213 2023-04-24 01:00:22.989521 SfMLearner_installable-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7478 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 01:00:22.941520 SfMLearner_installable-1.0.1/SfMLearner_installable.egg-info/
+-rw-rw-rw-   0        0        0     8213 2023-04-24 01:00:22.000000 SfMLearner_installable-1.0.1/SfMLearner_installable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-04-24 01:00:22.000000 SfMLearner_installable-1.0.1/SfMLearner_installable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:00:22.000000 SfMLearner_installable-1.0.1/SfMLearner_installable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-24 01:00:22.000000 SfMLearner_installable-1.0.1/SfMLearner_installable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-24 01:00:22.000000 SfMLearner_installable-1.0.1/SfMLearner_installable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 01:00:22.947520 SfMLearner_installable-1.0.1/data/
+-rw-rw-rw-   0        0        0        0 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:00:22.955521 SfMLearner_installable-1.0.1/data/cityscapes/
+-rw-rw-rw-   0        0        0        0 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/data/cityscapes/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/data/cityscapes/cityscapes_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:00:22.966522 SfMLearner_installable-1.0.1/data/kitti/
+-rw-rw-rw-   0        0        0        0 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/data/kitti/__init__.py
+-rw-rw-rw-   0        0        0     6338 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/data/kitti/kitti_odom_loader.py
+-rw-rw-rw-   0        0        0     6338 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/data/kitti/kitti_raw_loader.py
+-rw-rw-rw-   0        0        0     4693 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/data/prepare_train_data.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:00:22.985523 SfMLearner_installable-1.0.1/kitti_eval/
+-rw-rw-rw-   0        0        0        0 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/kitti_eval/__init__.py
+-rw-rw-rw-   0        0        0     7651 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/kitti_eval/depth_evaluation_utils.py
+-rw-rw-rw-   0        0        0     3585 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/kitti_eval/eval_depth.py
+-rw-rw-rw-   0        0        0      989 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/kitti_eval/eval_pose.py
+-rw-rw-rw-   0        0        0    13974 2023-04-24 00:58:29.000000 SfMLearner_installable-1.0.1/kitti_eval/pose_evaluation_utils.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:00:22.992520 SfMLearner_installable-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     4068 2023-04-24 00:59:47.000000 SfMLearner_installable-1.0.1/setup.py
```

### Comparing `SfMLearner_installable-1.0.0/LICENSE` & `SfMLearner_installable-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/PKG-INFO` & `SfMLearner_installable-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SfMLearner_installable
-Version: 1.0.0
+Version: 1.0.1
 Summary: Fork of the original SfMLearner with a setup.py file for installation with pip.
 Home-page: https://github.com/topher097/SfMLearner_installable
 Author: Christopher Endres
 Author-email: cmendres400@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Fork of SfMLearner
 This fork is of SfMLearner, nothing changed with it but includes a `setup.py` file so the repo can be installed via pip using the command:
 ```
-pip install -e git+https://github.com/topher097/SfMLearner_installable.git#egg=SfMLearner
+pip install SfMLearner-installable
 ```
 
 # SfMLearner
 This codebase implements the system described in the paper:
 
 Unsupervised Learning of Depth and Ego-Motion from Video
```

### Comparing `SfMLearner_installable-1.0.0/README.md` & `SfMLearner_installable-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Fork of SfMLearner
 This fork is of SfMLearner, nothing changed with it but includes a `setup.py` file so the repo can be installed via pip using the command:
 ```
-pip install -e git+https://github.com/topher097/SfMLearner_installable.git#egg=SfMLearner
+pip install SfMLearner-installable
 ```
 
 # SfMLearner
 This codebase implements the system described in the paper:
 
 Unsupervised Learning of Depth and Ego-Motion from Video
```

### Comparing `SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/PKG-INFO` & `SfMLearner_installable-1.0.1/SfMLearner_installable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SfMLearner-installable
-Version: 1.0.0
+Version: 1.0.1
 Summary: Fork of the original SfMLearner with a setup.py file for installation with pip.
 Home-page: https://github.com/topher097/SfMLearner_installable
 Author: Christopher Endres
 Author-email: cmendres400@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Fork of SfMLearner
 This fork is of SfMLearner, nothing changed with it but includes a `setup.py` file so the repo can be installed via pip using the command:
 ```
-pip install -e git+https://github.com/topher097/SfMLearner_installable.git#egg=SfMLearner
+pip install SfMLearner-installable
 ```
 
 # SfMLearner
 This codebase implements the system described in the paper:
 
 Unsupervised Learning of Depth and Ego-Motion from Video
```

### Comparing `SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/SOURCES.txt` & `SfMLearner_installable-1.0.1/SfMLearner_installable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/data/cityscapes/cityscapes_loader.py` & `SfMLearner_installable-1.0.1/data/cityscapes/cityscapes_loader.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/data/kitti/kitti_odom_loader.py` & `SfMLearner_installable-1.0.1/data/kitti/kitti_odom_loader.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/data/kitti/kitti_raw_loader.py` & `SfMLearner_installable-1.0.1/data/kitti/kitti_raw_loader.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/data/prepare_train_data.py` & `SfMLearner_installable-1.0.1/data/prepare_train_data.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/kitti_eval/depth_evaluation_utils.py` & `SfMLearner_installable-1.0.1/kitti_eval/depth_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/kitti_eval/eval_depth.py` & `SfMLearner_installable-1.0.1/kitti_eval/eval_depth.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/kitti_eval/eval_pose.py` & `SfMLearner_installable-1.0.1/kitti_eval/eval_pose.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/kitti_eval/pose_evaluation_utils.py` & `SfMLearner_installable-1.0.1/kitti_eval/pose_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-1.0.0/setup.py` & `SfMLearner_installable-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pipenv install twine --dev
-
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = 'SfMLearner_installable'
-DESCRIPTION = 'Fork of the original SfMLearner with a setup.py file for installation with pip.'
-URL = 'https://github.com/topher097/SfMLearner_installable'
-EMAIL = 'cmendres400@gmail.com'
-AUTHOR = 'Christopher Endres'
-REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.0'
-
-# What packages are required for this module to be executed?
-REQUIRED = [
-    'joblib == 1.2.0', 
-    'matplotlib == 3.7.1', 
-    'numpy == 1.24.3' , 
-    'Pillow == 9.5.0',
-    'scipy == 1.10.1',
-    'setuptools == 65.5.0',
-    'tensorflow == 2.12.0'
-]
-
-EXTRAS = {}
-
-# The rest you shouldn't have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    # If your package is a single module, use this instead of 'packages':
-    # py_modules=['mypackage'],
-
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    license='MIT',
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    },
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Note: To use the 'upload' functionality of this file, you must:
+#   $ pipenv install twine --dev
+
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = 'SfMLearner_installable'
+DESCRIPTION = 'Fork of the original SfMLearner with a setup.py file for installation with pip.'
+URL = 'https://github.com/topher097/SfMLearner_installable'
+EMAIL = 'cmendres400@gmail.com'
+AUTHOR = 'Christopher Endres'
+REQUIRES_PYTHON = '>=3.6.0'
+VERSION = '1.0.1'
+
+# What packages are required for this module to be executed?
+REQUIRED = [
+    'joblib >= 1.2.0', 
+    'matplotlib >= 3.7.1', 
+    'numpy' , 
+    'Pillow >= 9.5.0',
+    'scipy >= 1.10.1',
+    'setuptools >= 65.5.0',
+    'tensorflow >= 1.12.0'
+]
+
+EXTRAS = {}
+
+# The rest you shouldn't have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+        exec(f.read(), about)
+else:
+    about['__version__'] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    # If your package is a single module, use this instead of 'packages':
+    # py_modules=['mypackage'],
+
+    # entry_points={
+    #     'console_scripts': ['mycli=mymodule:cli'],
+    # },
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    license='MIT',
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy'
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        'upload': UploadCommand,
+    },
+)
```

