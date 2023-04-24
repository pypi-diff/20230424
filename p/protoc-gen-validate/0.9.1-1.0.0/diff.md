# Comparing `tmp/protoc-gen-validate-0.9.1.tar.gz` & `tmp/protoc-gen-validate-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protoc-gen-validate-0.9.1.tar", last modified: Mon Dec  5 16:57:57 2022, max compression
+gzip compressed data, was "protoc-gen-validate-1.0.0.tar", last modified: Mon Apr 24 17:11:05 2023, max compression
```

## Comparing `protoc-gen-validate-0.9.1.tar` & `protoc-gen-validate-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 16:57:57.627814 protoc-gen-validate-0.9.1/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-12-05 16:57:56.000000 protoc-gen-validate-0.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1730 2022-12-05 16:57:57.627814 protoc-gen-validate-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1170 2022-12-05 16:54:08.000000 protoc-gen-validate-0.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 16:57:57.627814 protoc-gen-validate-0.9.1/protoc_gen_validate/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-05 16:54:08.000000 protoc-gen-validate-0.9.1/protoc_gen_validate/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49214 2022-12-05 16:54:08.000000 protoc-gen-validate-0.9.1/protoc_gen_validate/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 16:57:57.627814 protoc-gen-validate-0.9.1/protoc_gen_validate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1730 2022-12-05 16:57:57.000000 protoc-gen-validate-0.9.1/protoc_gen_validate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      336 2022-12-05 16:57:57.000000 protoc-gen-validate-0.9.1/protoc_gen_validate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 16:57:57.000000 protoc-gen-validate-0.9.1/protoc_gen_validate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2022-12-05 16:57:57.000000 protoc-gen-validate-0.9.1/protoc_gen_validate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-12-05 16:57:57.000000 protoc-gen-validate-0.9.1/protoc_gen_validate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      159 2022-12-05 16:54:08.000000 protoc-gen-validate-0.9.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      855 2022-12-05 16:57:57.631814 protoc-gen-validate-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    31250 2022-12-05 16:57:56.000000 protoc-gen-validate-0.9.1/validate.proto
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 17:11:05.051478 protoc-gen-validate-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-04-24 17:11:04.000000 protoc-gen-validate-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-04-24 17:11:05.051478 protoc-gen-validate-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-24 17:07:21.000000 protoc-gen-validate-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 17:11:05.051478 protoc-gen-validate-1.0.0/protoc_gen_validate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 17:07:21.000000 protoc-gen-validate-1.0.0/protoc_gen_validate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50287 2023-04-24 17:07:21.000000 protoc-gen-validate-1.0.0/protoc_gen_validate/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 17:11:05.051478 protoc-gen-validate-1.0.0/protoc_gen_validate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-04-24 17:11:04.000000 protoc-gen-validate-1.0.0/protoc_gen_validate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2023-04-24 17:11:05.000000 protoc-gen-validate-1.0.0/protoc_gen_validate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 17:11:04.000000 protoc-gen-validate-1.0.0/protoc_gen_validate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-24 17:11:04.000000 protoc-gen-validate-1.0.0/protoc_gen_validate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-24 17:11:04.000000 protoc-gen-validate-1.0.0/protoc_gen_validate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-24 17:07:21.000000 protoc-gen-validate-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-24 17:11:05.055477 protoc-gen-validate-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    31250 2023-04-24 17:11:04.000000 protoc-gen-validate-1.0.0/validate.proto
```

### Comparing `protoc-gen-validate-0.9.1/LICENSE` & `protoc-gen-validate-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protoc-gen-validate-0.9.1/PKG-INFO` & `protoc-gen-validate-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protoc-gen-validate
-Version: 0.9.1
+Version: 1.0.0
 Summary: PGV for python via just-in-time code generation
 Home-page: https://github.com/bufbuild/protoc-gen-validate
 Author: Buf
 Author-email: dev@buf.build
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `protoc-gen-validate-0.9.1/README.md` & `protoc-gen-validate-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `protoc-gen-validate-0.9.1/protoc_gen_validate/validator.py` & `protoc-gen-validate-1.0.0/protoc_gen_validate/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -304,17 +304,14 @@
 def const_template(option_value, name):
     const_tmpl = """{%- if str(o.string) and o.string.HasField('const') -%}
     if {{ name }} != \"{{ o.string['const'] }}\":
         raise ValidationFailed(\"{{ name }} not equal to {{ o.string['const'] }}\")
     {%- elif str(o.bool) and o.bool['const'] != "" -%}
     if {{ name }} != {{ o.bool['const'] }}:
         raise ValidationFailed(\"{{ name }} not equal to {{ o.bool['const'] }}\")
-    {%- elif str(o.enum) and o.enum['const'] -%}
-    if {{ name }} != {{ o.enum['const'] }}:
-        raise ValidationFailed(\"{{ name }} not equal to {{ o.enum['const'] }}\")
     {%- elif str(o.bytes) and o.bytes.HasField('const') -%}
         {% if sys.version_info[0] >= 3 %}
     if {{ name }} != {{ o.bytes['const'] }}:
         raise ValidationFailed(\"{{ name }} not equal to {{ o.bytes['const'] }}\")
         {% else %}
     if {{ name }} != b\"{{ o.bytes['const'].encode('string_escape') }}\":
         raise ValidationFailed(\"{{ name }} not equal to {{ o.bytes['const'].encode('string_escape') }}\")
@@ -824,25 +821,60 @@
                                          bytes_template=bytes_template, repeated=repeated)
 
 
 def enum_values(field):
     return [x.number for x in field.enum_type.values]
 
 
+def enum_name(field, number):
+    for x in field.enum_type.values:
+        if x.number == number:
+            return x.name
+    return ""
+
+
+def enum_names(field, numbers):
+    m = {x.number: x.name for x in field.enum_type.values}
+    return "[" + "".join([m[n] for n in numbers]) + "]"
+
+
+def enum_const_template(value, name, field):
+    const_tmpl = """{%- if str(value) and value['const'] -%}
+    if {{ name }} != {{ value['const'] }}:
+        raise ValidationFailed(\"{{ name }} not equal to {{ enum_name(field, value['const']) }}\")
+    {%- endif -%}
+    """
+    return Template(const_tmpl).render(value=value, name=name, field=field, enum_name=enum_name, str=str)
+
+
+def enum_in_template(value, name, field):
+    in_tmpl = """
+    {%- if value['in'] %}
+    if {{ name }} not in {{ value['in'] }}:
+        raise ValidationFailed(\"{{ name }} not in {{ enum_names(field, value['in']) }}\")
+    {%- endif -%}
+    {%- if value['not_in'] %}
+    if {{ name }} in {{ value['not_in'] }}:
+        raise ValidationFailed(\"{{ name }} in {{ enum_names(field, value['not_in']) }}\")
+    {%- endif -%}
+    """
+    return Template(in_tmpl).render(value=value, name=name, field=field, enum_names=enum_names)
+
+
 def enum_template(option_value, name, field):
     enum_tmpl = """
-    {{ const_template(option_value, name) -}}
-    {{ in_template(option_value.enum, name) -}}
+    {{ enum_const_template(option_value.enum, name, field) -}}
+    {{ enum_in_template(option_value.enum, name, field) -}}
     {% if option_value.enum['defined_only'] %}
     if {{ name }} not in {{ enum_values(field) }}:
         raise ValidationFailed(\"{{ name }} is not defined\")
     {% endif %}
     """
-    return Template(enum_tmpl).render(option_value=option_value, name=name, const_template=const_template,
-                                      in_template=in_template, field=field, enum_values=enum_values)
+    return Template(enum_tmpl).render(option_value=option_value, name=name, enum_const_template=enum_const_template,
+                                      enum_in_template=enum_in_template, field=field, enum_values=enum_values)
 
 
 def any_template(option_value, name, repeated=False):
     any_tmpl = """
     {{- required_template(o, name) }}
     {%- if o['in'] %}
     {% if repeated %}
```

### Comparing `protoc-gen-validate-0.9.1/protoc_gen_validate.egg-info/PKG-INFO` & `protoc-gen-validate-1.0.0/protoc_gen_validate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protoc-gen-validate
-Version: 0.9.1
+Version: 1.0.0
 Summary: PGV for python via just-in-time code generation
 Home-page: https://github.com/bufbuild/protoc-gen-validate
 Author: Buf
 Author-email: dev@buf.build
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `protoc-gen-validate-0.9.1/setup.cfg` & `protoc-gen-validate-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `protoc-gen-validate-0.9.1/validate.proto` & `protoc-gen-validate-1.0.0/validate.proto`

 * *Files identical despite different names*

