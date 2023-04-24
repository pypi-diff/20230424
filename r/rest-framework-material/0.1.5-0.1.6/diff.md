# Comparing `tmp/rest_framework_material-0.1.5.tar.gz` & `tmp/rest_framework_material-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_material-0.1.5.tar", max compression
+gzip compressed data, was "rest_framework_material-0.1.6.tar", max compression
```

## Comparing `rest_framework_material-0.1.5.tar` & `rest_framework_material-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-21 17:36:10.988103 rest_framework_material-0.1.5/LICENSE
--rw-r--r--   0        0        0      637 2023-04-23 05:23:35.369583 rest_framework_material-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      749 2023-04-21 17:40:45.269789 rest_framework_material-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_material-0.1.5/rest_framework_material/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_material-0.1.5/rest_framework_material/admin.py
--rw-r--r--   0        0        0      248 2023-04-21 17:38:09.789518 rest_framework_material-0.1.5/rest_framework_material/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_material-0.1.5/rest_framework_material/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_material-0.1.5/rest_framework_material/models.py
--rw-r--r--   0        0        0    23726 2023-04-22 17:24:36.643761 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1181 2023-04-21 17:25:31.881402 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      682 2023-04-22 06:32:18.842409 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4252 2023-04-21 17:33:58.678317 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_material-0.1.5/rest_framework_material/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_material-0.1.5/rest_framework_material/views.py
--rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 rest_framework_material-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-21 17:36:10.988103 rest_framework_material-0.1.6/LICENSE
+-rw-r--r--   0        0        0      637 2023-04-24 10:12:02.626405 rest_framework_material-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      749 2023-04-21 17:40:45.269789 rest_framework_material-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_material-0.1.6/rest_framework_material/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_material-0.1.6/rest_framework_material/admin.py
+-rw-r--r--   0        0        0      248 2023-04-21 17:38:09.789518 rest_framework_material-0.1.6/rest_framework_material/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_material-0.1.6/rest_framework_material/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_material-0.1.6/rest_framework_material/models.py
+-rw-r--r--   0        0        0    23092 2023-04-24 06:09:06.750990 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1181 2023-04-21 17:25:31.881402 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      682 2023-04-22 06:32:18.842409 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     3618 2023-04-24 06:09:24.194418 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_material-0.1.6/rest_framework_material/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_material-0.1.6/rest_framework_material/views.py
+-rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 rest_framework_material-0.1.6/PKG-INFO
```

### Comparing `rest_framework_material-0.1.5/LICENSE` & `rest_framework_material-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/pyproject.toml` & `rest_framework_material-0.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-material"
-version = "0.1.5"
+version = "0.1.6"
 description = "Redesign of the browsable api of Django REST Framework using MD Bootstrap"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_material"}]
 homepage = "https://github.com/youzarsiph/rest-framework-material/"
 repository = "https://github.com/youzarsiph/rest-framework-material/"
```

### Comparing `rest_framework_material-0.1.5/README.md` & `rest_framework_material-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/api.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/api.html`

 * *Files 3% similar despite different names*

```diff
@@ -479,27 +479,12 @@
 {% endblock %}
 
 {% if filter_form %}
   {{ filter_form }}
 {% endif %}
 
 {% block script %}
-  <script>
-    window.drf = {
-      csrfHeaderName: "{{ csrf_header_name|default:'X-CSRFToken' }}",
-      csrfToken: "{% if request %}{{ csrf_token }}{% endif %}"
-    };
-  </script>
-  <script src="{% static "rest_framework/js/jquery-3.5.1.min.js" %}"></script>
-  <script src="{% static "rest_framework/js/ajax-form.js" %}"></script>
-  <script src="{% static "rest_framework/js/csrf.js" %}"></script>
-  <script src="{% static "rest_framework/js/prettify-min.js" %}"></script>
-  <script src="{% static "rest_framework/js/default.js" %}"></script>
-  <script>
-    $(document).ready(function() {
-      $('form').ajaxForm();
-    });
-  </script>
+  {{ block.super }}
   <script type="text/javascript"src="https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.2.0/mdb.min.js"></script>
   <script src="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/highlight.min.js"></script>
   <script>hljs.highlightAll()</script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -121,15 +121,9 @@
 {% if raw_data_put_form %}
  {% translate "PUT" %}
   {% endif %} {% if raw_data_patch_form %}
  {% translate "PATCH" %}
   {% endif %}
 {% endwith %}
 {% endif %} {% endif %}   {% endblock %} {% if filter_form %} {{ filter_form }}
-{% endif %} {% block script %}
-
-s/jquery-3.5.1.min.js" %}">
-s/ajax-form.js" %}">
-s/csrf.js" %}">
-s/prettify-min.js" %}">
-s/default.js" %}">
+{% endif %} {% block script %} {{ block.super }}
  {% endblock %}
```

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/filters/base.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/filters/ordering.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/filters/search.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/input.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/radio.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/select.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/horizontal/textarea.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/login.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/login.html`

 * *Files 18% similar despite different names*

```diff
@@ -210,57 +210,18 @@
 00000d10: 6765 7220 726f 756e 6465 642d 626f 7474  ger rounded-bott
 00000d20: 6f6d 2d34 223e 3c2f 6469 763e 0d0a 2020  om-4"></div>..  
 00000d30: 2020 2020 2020 3c2f 6469 763e 0d0a 2020        </div>..  
 00000d40: 2020 2020 3c2f 6469 763e 0d0a 2020 2020      </div>..    
 00000d50: 3c2f 6469 763e 0d0a 2020 3c2f 626f 6479  </div>..  </body
 00000d60: 3e0d 0a7b 2520 656e 6462 6c6f 636b 2025  >..{% endblock %
 00000d70: 7d0d 0a0d 0a0d 0a7b 2520 626c 6f63 6b20  }......{% block 
-00000d80: 7363 7269 7074 2025 7d0d 0a20 203c 7363  script %}..  <sc
-00000d90: 7269 7074 3e0d 0a20 2020 2077 696e 646f  ript>..    windo
-00000da0: 772e 6472 6620 3d20 7b0d 0a20 2020 2020  w.drf = {..     
-00000db0: 2063 7372 6648 6561 6465 724e 616d 653a   csrfHeaderName:
-00000dc0: 2022 7b7b 2063 7372 665f 6865 6164 6572   "{{ csrf_header
-00000dd0: 5f6e 616d 657c 6465 6661 756c 743a 2758  _name|default:'X
-00000de0: 2d43 5352 4654 6f6b 656e 2720 7d7d 222c  -CSRFToken' }}",
-00000df0: 0d0a 2020 2020 2020 6373 7266 546f 6b65  ..      csrfToke
-00000e00: 6e3a 2022 7b25 2069 6620 7265 7175 6573  n: "{% if reques
-00000e10: 7420 257d 7b7b 2063 7372 665f 746f 6b65  t %}{{ csrf_toke
-00000e20: 6e20 7d7d 7b25 2065 6e64 6966 2025 7d22  n }}{% endif %}"
-00000e30: 0d0a 2020 2020 7d3b 0d0a 2020 3c2f 7363  ..    };..  </sc
-00000e40: 7269 7074 3e0d 0a20 203c 7363 7269 7074  ript>..  <script
-00000e50: 2073 7263 3d22 7b25 2073 7461 7469 6320   src="{% static 
-00000e60: 2272 6573 745f 6672 616d 6577 6f72 6b2f  "rest_framework/
-00000e70: 6a73 2f6a 7175 6572 792d 332e 352e 312e  js/jquery-3.5.1.
-00000e80: 6d69 6e2e 6a73 2220 257d 223e 3c2f 7363  min.js" %}"></sc
-00000e90: 7269 7074 3e0d 0a20 203c 7363 7269 7074  ript>..  <script
-00000ea0: 2073 7263 3d22 7b25 2073 7461 7469 6320   src="{% static 
-00000eb0: 2272 6573 745f 6672 616d 6577 6f72 6b2f  "rest_framework/
-00000ec0: 6a73 2f61 6a61 782d 666f 726d 2e6a 7322  js/ajax-form.js"
-00000ed0: 2025 7d22 3e3c 2f73 6372 6970 743e 0d0a   %}"></script>..
-00000ee0: 2020 3c73 6372 6970 7420 7372 633d 227b    <script src="{
-00000ef0: 2520 7374 6174 6963 2022 7265 7374 5f66  % static "rest_f
-00000f00: 7261 6d65 776f 726b 2f6a 732f 6373 7266  ramework/js/csrf
-00000f10: 2e6a 7322 2025 7d22 3e3c 2f73 6372 6970  .js" %}"></scrip
-00000f20: 743e 0d0a 2020 3c73 6372 6970 7420 7372  t>..  <script sr
-00000f30: 633d 227b 2520 7374 6174 6963 2022 7265  c="{% static "re
-00000f40: 7374 5f66 7261 6d65 776f 726b 2f6a 732f  st_framework/js/
-00000f50: 7072 6574 7469 6679 2d6d 696e 2e6a 7322  prettify-min.js"
-00000f60: 2025 7d22 3e3c 2f73 6372 6970 743e 0d0a   %}"></script>..
-00000f70: 2020 3c73 6372 6970 7420 7372 633d 227b    <script src="{
-00000f80: 2520 7374 6174 6963 2022 7265 7374 5f66  % static "rest_f
-00000f90: 7261 6d65 776f 726b 2f6a 732f 6465 6661  ramework/js/defa
-00000fa0: 756c 742e 6a73 2220 257d 223e 3c2f 7363  ult.js" %}"></sc
-00000fb0: 7269 7074 3e0d 0a20 203c 7363 7269 7074  ript>..  <script
-00000fc0: 3e0d 0a20 2020 2024 2864 6f63 756d 656e  >..    $(documen
-00000fd0: 7429 2e72 6561 6479 2866 756e 6374 696f  t).ready(functio
-00000fe0: 6e28 2920 7b0d 0a20 2020 2020 2024 2827  n() {..      $('
-00000ff0: 666f 726d 2729 2e61 6a61 7846 6f72 6d28  form').ajaxForm(
-00001000: 293b 0d0a 2020 2020 7d29 3b0d 0a20 203c  );..    });..  <
-00001010: 2f73 6372 6970 743e 0d0a 2020 3c73 6372  /script>..  <scr
-00001020: 6970 7420 7479 7065 3d22 7465 7874 2f6a  ipt type="text/j
-00001030: 6176 6173 6372 6970 7422 7372 633d 2268  avascript"src="h
-00001040: 7474 7073 3a2f 2f63 646e 6a73 2e63 6c6f  ttps://cdnjs.clo
-00001050: 7564 666c 6172 652e 636f 6d2f 616a 6178  udflare.com/ajax
-00001060: 2f6c 6962 732f 6d64 622d 7569 2d6b 6974  /libs/mdb-ui-kit
-00001070: 2f36 2e32 2e30 2f6d 6462 2e6d 696e 2e6a  /6.2.0/mdb.min.j
-00001080: 7322 3e3c 2f73 6372 6970 743e 0d0a 7b25  s"></script>..{%
-00001090: 2065 6e64 626c 6f63 6b20 257d             endblock %}
+00000d80: 7363 7269 7074 2025 7d0d 0a20 207b 7b20  script %}..  {{ 
+00000d90: 626c 6f63 6b2e 7375 7065 7220 7d7d 0d0a  block.super }}..
+00000da0: 2020 3c73 6372 6970 7420 7479 7065 3d22    <script type="
+00000db0: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
+00000dc0: 7372 633d 2268 7474 7073 3a2f 2f63 646e  src="https://cdn
+00000dd0: 6a73 2e63 6c6f 7564 666c 6172 652e 636f  js.cloudflare.co
+00000de0: 6d2f 616a 6178 2f6c 6962 732f 6d64 622d  m/ajax/libs/mdb-
+00000df0: 7569 2d6b 6974 2f36 2e32 2e30 2f6d 6462  ui-kit/6.2.0/mdb
+00000e00: 2e6d 696e 2e6a 7322 3e3c 2f73 6372 6970  .min.js"></scrip
+00000e10: 743e 0d0a 7b25 2065 6e64 626c 6f63 6b20  t>..{% endblock 
+00000e20: 257d                                     %}
```

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/pagination/numbers.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_material-0.1.6/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.5/PKG-INFO` & `rest_framework_material-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-material
-Version: 0.1.5
+Version: 0.1.6
 Summary: Redesign of the browsable api of Django REST Framework using MD Bootstrap
 Home-page: https://github.com/youzarsiph/rest-framework-material/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

