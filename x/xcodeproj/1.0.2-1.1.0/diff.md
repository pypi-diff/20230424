# Comparing `tmp/xcodeproj-1.0.2.tar.gz` & `tmp/xcodeproj-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcodeproj-1.0.2.tar", max compression
+gzip compressed data, was "xcodeproj-1.1.0.tar", max compression
```

## Comparing `xcodeproj-1.0.2.tar` & `xcodeproj-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1141 2023-03-22 05:31:26.588313 xcodeproj-1.0.2/LICENSE
--rw-r--r--   0        0        0     3638 2023-03-22 05:31:26.588614 xcodeproj-1.0.2/README.md
--rw-r--r--   0        0        0     1065 2023-03-22 08:37:45.128415 xcodeproj-1.0.2/pyproject.toml
--rwxr-xr-x   0        0        0     9660 2023-03-22 05:39:30.354581 xcodeproj-1.0.2/xcodeproj/__init__.py
--rwxr-xr-x   0        0        0     3670 2023-03-22 05:31:26.599876 xcodeproj-1.0.2/xcodeproj/buildphases.py
--rwxr-xr-x   0        0        0      466 2023-03-22 05:31:26.600149 xcodeproj-1.0.2/xcodeproj/buildrules.py
--rwxr-xr-x   0        0        0      941 2023-03-22 05:31:26.600363 xcodeproj-1.0.2/xcodeproj/files.py
--rwxr-xr-x   0        0        0     1470 2023-03-22 05:31:26.600583 xcodeproj-1.0.2/xcodeproj/other.py
--rwxr-xr-x   0        0        0     6908 2023-03-22 05:31:26.600841 xcodeproj-1.0.2/xcodeproj/pathobjects.py
--rwxr-xr-x   0        0        0     1783 2023-03-22 05:31:26.601078 xcodeproj-1.0.2/xcodeproj/pbxobject.py
--rwxr-xr-x   0        0        0     1888 2023-03-22 05:31:26.601477 xcodeproj-1.0.2/xcodeproj/pbxproject.py
--rwxr-xr-x   0        0        0    23926 2023-03-22 05:31:26.601951 xcodeproj-1.0.2/xcodeproj/schemes.py
--rwxr-xr-x   0        0        0     3602 2023-03-22 05:31:26.602239 xcodeproj-1.0.2/xcodeproj/targets.py
--rwxr-xr-x   0        0        0     2731 2023-03-22 08:37:07.901946 xcodeproj-1.0.2/xcodeproj/xcobjects.py
--rw-r--r--   0        0        0     4436 1970-01-01 00:00:00.000000 xcodeproj-1.0.2/setup.py
--rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 xcodeproj-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-03-22 05:31:26.588313 xcodeproj-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3638 2023-03-22 05:31:26.588614 xcodeproj-1.1.0/README.md
+-rw-r--r--   0        0        0     1205 2023-04-24 05:12:35.593601 xcodeproj-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0     9675 2023-04-24 02:42:41.641003 xcodeproj-1.1.0/xcodeproj/__init__.py
+-rwxr-xr-x   0        0        0     3670 2023-03-22 05:31:26.599876 xcodeproj-1.1.0/xcodeproj/buildphases.py
+-rwxr-xr-x   0        0        0      466 2023-03-22 05:31:26.600149 xcodeproj-1.1.0/xcodeproj/buildrules.py
+-rwxr-xr-x   0        0        0     1082 2023-04-24 02:30:59.751221 xcodeproj-1.1.0/xcodeproj/files.py
+-rwxr-xr-x   0        0        0     1470 2023-03-22 05:31:26.600583 xcodeproj-1.1.0/xcodeproj/other.py
+-rwxr-xr-x   0        0        0     6908 2023-03-22 05:31:26.600841 xcodeproj-1.1.0/xcodeproj/pathobjects.py
+-rwxr-xr-x   0        0        0     1783 2023-03-22 05:31:26.601078 xcodeproj-1.1.0/xcodeproj/pbxobject.py
+-rwxr-xr-x   0        0        0     1888 2023-03-22 05:31:26.601477 xcodeproj-1.1.0/xcodeproj/pbxproject.py
+-rwxr-xr-x   0        0        0    23926 2023-03-22 05:31:26.601951 xcodeproj-1.1.0/xcodeproj/schemes.py
+-rwxr-xr-x   0        0        0     3602 2023-03-22 05:31:26.602239 xcodeproj-1.1.0/xcodeproj/targets.py
+-rwxr-xr-x   0        0        0     2731 2023-03-22 08:37:07.901946 xcodeproj-1.1.0/xcodeproj/xcobjects.py
+-rw-r--r--   0        0        0     4851 1970-01-01 00:00:00.000000 xcodeproj-1.1.0/PKG-INFO
```

### Comparing `xcodeproj-1.0.2/LICENSE` & `xcodeproj-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/README.md` & `xcodeproj-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/xcodeproj/__init__.py` & `xcodeproj-1.1.0/xcodeproj/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Xcode project file management."""
 
 try:
-    import _pickle as pickle
+    import _pickle as pickle  # type: ignore
 except ImportError:
     import pickle  # type: ignore
 
 import hashlib
 import json
 import os
 import pathlib
@@ -106,15 +106,15 @@
             value["object_key"] = key
 
         self.objects = Objects(
             **deserialize.deserialize(
                 Dict[str, PBXObject],
                 tree["objects"],
                 throw_on_unhandled=not ignore_deserialization_errors,
-                raw_storage_mode=deserialize.RawStorageMode.all,
+                raw_storage_mode=deserialize.RawStorageMode.ALL,
             )
         )
 
         self.project = self.objects[tree["rootObject"]]
         self._cached_items = {}
         self._schemes = None
         self._is_populated = False
@@ -183,15 +183,14 @@
 
         if object_type.__name__ in self._cached_items:
             return
 
         cached_items: Dict[str, PBXObject] = {}
 
         for object_key, project_object in self.objects.items():
-
             if not isinstance(project_object, object_type):
                 continue
 
             cached_items[object_key] = project_object
 
         self._cached_items[object_type.__name__] = cached_items
```

### Comparing `xcodeproj-1.0.2/xcodeproj/buildphases.py` & `xcodeproj-1.1.0/xcodeproj/buildphases.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/xcodeproj/files.py` & `xcodeproj-1.1.0/xcodeproj/files.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,10 +24,14 @@
     platform_filter: Optional[str]
     settings: Optional[Dict[str, Any]]
 
     @property
     def file_ref(self) -> PBXFileReference:
         """Get the file reference.
 
+        :raises ValueError: If file_ref_id is None
+
         :returns: The file reference
         """
+        if self.file_ref_id is None:
+            raise ValueError("file_ref_id is None")
         return cast(PBXFileReference, self.objects()[self.file_ref_id])
```

### Comparing `xcodeproj-1.0.2/xcodeproj/other.py` & `xcodeproj-1.1.0/xcodeproj/other.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/xcodeproj/pathobjects.py` & `xcodeproj-1.1.0/xcodeproj/pathobjects.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/xcodeproj/pbxobject.py` & `xcodeproj-1.1.0/xcodeproj/pbxobject.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/xcodeproj/pbxproject.py` & `xcodeproj-1.1.0/xcodeproj/pbxproject.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/xcodeproj/schemes.py` & `xcodeproj-1.1.0/xcodeproj/schemes.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/xcodeproj/targets.py` & `xcodeproj-1.1.0/xcodeproj/targets.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/xcodeproj/xcobjects.py` & `xcodeproj-1.1.0/xcodeproj/xcobjects.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.0.2/setup.py` & `xcodeproj-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,106 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: xcodeproj
+Version: 1.1.0
+Summary: A utility for interacting with Xcode's xcodeproj bundle format.
+Home-page: https://github.com/Microsoft/xcodeproj
+License: MIT
+Keywords: xcode,xcodeproj,pbxproj,apple
+Author: Dale Myers
+Author-email: dalemy@microsoft.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development
+Classifier: Topic :: Utilities
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: deserialize (>=2.0.1,<3.0.0)
+Project-URL: Repository, https://github.com/Microsoft/xcodeproj
+Description-Content-Type: text/markdown
+
+# xcodeproj
+
+`xcodeproj` is a utility for interacting with Xcode's xcodeproj bundle format.
+
+It expects some level of understanding of the internals of the pbxproj format and schemes. Note that this tool only reads projects. It does not write out any changes. If you are looking for more advanced functionality like this, I recommend looking at the Ruby gem of the same name (which is unaffiliated in anyway). 
+
+To learn more about the format, you can look at any of these locations:
+
+* <http://www.monobjc.net/xcode-project-file-format.html>
+* <https://www.rubydoc.info/gems/xcodeproj/Xcodeproj/Project>
+
+## Getting Started
+
+Loading a project is very simple:
+
+```python
+project = xcodeproj.XcodeProject("/path/to/project.xcodeproj")
+```
+
+From here you can explore the project in different ways:
+
+```python
+
+# Get all targets
+for target in project.targets:
+    print(target.name)
+
+# Print from the root level, 2 levels deep (.project is a property on the root 
+# project as other properties such as .schemes are also available)
+for item1 in project.project.main_group.children:
+    print(item1)
+    if not isinstance(item1, xcodeproj.PBXGroup):
+        continue
+
+    for item2 in item1.children:
+        print("\t", item2)
+
+# Check that all files referenced in the project exist on disk
+for item in project.fetch_type(xcodeproj.PBXFileReference).values():
+    assert os.path.exists(item.absolute_path())
+
+# You can access the raw objects map directly:
+obj = project.objects["key here"]
+
+# For any object you have, you can access its key/identifier via the 
+# `.object_key` property
+key = obj.object_key
+```
+
+Note: This library is "lazy". Many things aren't calculated until they are used. This time will be inconsequential on smaller projects, but on larger ones, it can save quite a bit of time due to not parsing the entire project on load. These properties are usually stored though so that subsequent accesses are instant.
+
+## Note on Scheme Support
+There's no DTD for xcscheme files, so the implementation has been guessed. There will definitely be holes that still need to be patched in it though. Please open an issue if you find any, along with a sample xcscheme file.
+
+## Contributing
+
+This project welcomes contributions and suggestions.  Most contributions require you to agree to a
+Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
+the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
+
+When you submit a pull request, a CLA bot will automatically determine whether you need to provide
+a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
+provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
+For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
+contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
+
+## Trademarks
+
+This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
+trademarks or logos is subject to and must follow 
+[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
+Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
+Any use of third-party trademarks or logos are subject to those third-party's policies.
 
-packages = \
-['xcodeproj']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['appdirs>=1.0,<2.0', 'deserialize>=1.8.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'xcodeproj',
-    'version': '1.0.2',
-    'description': "A utility for interacting with Xcode's xcodeproj bundle format.",
-    'long_description': '# xcodeproj\n\n`xcodeproj` is a utility for interacting with Xcode\'s xcodeproj bundle format.\n\nIt expects some level of understanding of the internals of the pbxproj format and schemes. Note that this tool only reads projects. It does not write out any changes. If you are looking for more advanced functionality like this, I recommend looking at the Ruby gem of the same name (which is unaffiliated in anyway). \n\nTo learn more about the format, you can look at any of these locations:\n\n* <http://www.monobjc.net/xcode-project-file-format.html>\n* <https://www.rubydoc.info/gems/xcodeproj/Xcodeproj/Project>\n\n## Getting Started\n\nLoading a project is very simple:\n\n```python\nproject = xcodeproj.XcodeProject("/path/to/project.xcodeproj")\n```\n\nFrom here you can explore the project in different ways:\n\n```python\n\n# Get all targets\nfor target in project.targets:\n    print(target.name)\n\n# Print from the root level, 2 levels deep (.project is a property on the root \n# project as other properties such as .schemes are also available)\nfor item1 in project.project.main_group.children:\n    print(item1)\n    if not isinstance(item1, xcodeproj.PBXGroup):\n        continue\n\n    for item2 in item1.children:\n        print("\\t", item2)\n\n# Check that all files referenced in the project exist on disk\nfor item in project.fetch_type(xcodeproj.PBXFileReference).values():\n    assert os.path.exists(item.absolute_path())\n\n# You can access the raw objects map directly:\nobj = project.objects["key here"]\n\n# For any object you have, you can access its key/identifier via the \n# `.object_key` property\nkey = obj.object_key\n```\n\nNote: This library is "lazy". Many things aren\'t calculated until they are used. This time will be inconsequential on smaller projects, but on larger ones, it can save quite a bit of time due to not parsing the entire project on load. These properties are usually stored though so that subsequent accesses are instant.\n\n## Note on Scheme Support\nThere\'s no DTD for xcscheme files, so the implementation has been guessed. There will definitely be holes that still need to be patched in it though. Please open an issue if you find any, along with a sample xcscheme file.\n\n## Contributing\n\nThis project welcomes contributions and suggestions.  Most contributions require you to agree to a\nContributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us\nthe rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.\n\nWhen you submit a pull request, a CLA bot will automatically determine whether you need to provide\na CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions\nprovided by the bot. You will only need to do this once across all repos using our CLA.\n\nThis project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).\nFor more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or\ncontact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.\n\n## Trademarks\n\nThis project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft \ntrademarks or logos is subject to and must follow \n[Microsoft\'s Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).\nUse of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.\nAny use of third-party trademarks or logos are subject to those third-party\'s policies.\n',
-    'author': 'Dale Myers',
-    'author_email': 'dalemy@microsoft.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Microsoft/xcodeproj',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

