# Comparing `tmp/scrape_schema-0.0.7.tar.gz` & `tmp/scrape_schema-0.0.8.tar.gz`

## Comparing `scrape_schema-0.0.7.tar` & `scrape_schema-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/__init__.py
--rw-r--r--   0        0        0    19592 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/LICENSE
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/README.md
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/__init__.py
+-rw-r--r--   0        0        0    19469 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/README.md
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/PKG-INFO
```

### Comparing `scrape_schema-0.0.7/scrape_schema/base.py` & `scrape_schema-0.0.8/scrape_schema/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -510,27 +510,14 @@
         if parse_markup:
             self._parse_markup_to_fields(markup)
 
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     @classmethod
-    def init_list(cls, markups: Iterable[str]) -> list[Self]:
-        """Init list of schemas by markups sequence
-
-        :param markups: - iterable markups sequence
-        """
-        warnings.warn(
-            "This method deprecated, usage `from_list`",
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-        return cls.from_list(markups)
-
-    @classmethod
     def from_list(cls, markups: Iterable[str], **kwargs) -> list[Self]:
         """Init list of schemas by markups sequence
 
         :param markups: iterable markups sequence
         :param kwargs: any attrs
         """
         return [cls(markup, parse_markup=True, **kwargs) for markup in markups]
@@ -557,14 +544,24 @@
         """
         return cls(crop_rule(markup), parse_markup=True, **kwargs)
 
     @classmethod
     def from_markup(cls, markup: str, **kwargs) -> Self:
         return cls(markup, parse_markup=True, **kwargs)
 
+    @classmethod
+    def from_kwargs(cls, **kwargs) -> Self:
+        """Create new class without parse markup and fields
+
+        :param kwargs: any keyword arguments
+        """
+        kwargs.pop("parse_markup")
+
+        return cls("", parse_markup=False, **kwargs)
+
     @staticmethod
     def _to_dict(value: BaseSchema | list | dict):
         if isinstance(value, BaseSchema):
             return value.dict()
 
         elif isinstance(value, list):
             if all(isinstance(val, BaseSchema) for val in value):
```

### Comparing `scrape_schema-0.0.7/scrape_schema/callbacks/slax.py` & `scrape_schema-0.0.8/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/scrape_schema/callbacks/soup.py` & `scrape_schema-0.0.8/scrape_schema/callbacks/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/scrape_schema/fields/nested.py` & `scrape_schema-0.0.8/scrape_schema/fields/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/scrape_schema/fields/regex.py` & `scrape_schema-0.0.8/scrape_schema/fields/regex.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/scrape_schema/fields/slax.py` & `scrape_schema-0.0.8/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/scrape_schema/fields/soup.py` & `scrape_schema-0.0.8/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/.gitignore` & `scrape_schema-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/LICENSE` & `scrape_schema-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/README.md` & `scrape_schema-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/pyproject.toml` & `scrape_schema-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.7/PKG-INFO` & `scrape_schema-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
```

