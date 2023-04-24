# Comparing `tmp/rest_framework_redesign-0.1.8.tar.gz` & `tmp/rest_framework_redesign-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_redesign-0.1.8.tar", max compression
+gzip compressed data, was "rest_framework_redesign-0.1.9.tar", max compression
```

## Comparing `rest_framework_redesign-0.1.8.tar` & `rest_framework_redesign-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.8/LICENSE
--rw-r--r--   0        0        0      618 2023-04-23 05:25:09.177260 rest_framework_redesign-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.8/rest_framework_redesign/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.8/rest_framework_redesign/admin.py
--rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.8/rest_framework_redesign/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.8/rest_framework_redesign/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.8/rest_framework_redesign/models.py
--rw-r--r--   0        0        0    23750 2023-04-20 09:09:17.444650 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1085 2023-04-20 09:11:06.989223 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4375 2023-04-18 08:11:26.812363 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.8/rest_framework_redesign/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.8/rest_framework_redesign/views.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.9/LICENSE
+-rw-r--r--   0        0        0      618 2023-04-24 10:13:18.845427 rest_framework_redesign-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.9/rest_framework_redesign/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.9/rest_framework_redesign/admin.py
+-rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.9/rest_framework_redesign/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.9/rest_framework_redesign/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.9/rest_framework_redesign/models.py
+-rw-r--r--   0        0        0    23116 2023-04-24 06:12:40.271460 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1085 2023-04-20 09:11:06.989223 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     3741 2023-04-24 06:13:07.927873 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.9/rest_framework_redesign/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.9/rest_framework_redesign/views.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.9/PKG-INFO
```

### Comparing `rest_framework_redesign-0.1.8/LICENSE` & `rest_framework_redesign-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/pyproject.toml` & `rest_framework_redesign-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-redesign"
-version = "0.1.8"
+version = "0.1.9"
 description = "Redesign of the browsable api of Django REST Framework"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_redesign"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
```

### Comparing `rest_framework_redesign-0.1.8/README.md` & `rest_framework_redesign-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/api.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/api.html`

 * *Files 3% similar despite different names*

```diff
@@ -471,29 +471,14 @@
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
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
     integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe"
     crossorigin="anonymous"></script>
   <script src="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/highlight.min.js"></script>
   <script>hljs.highlightAll()</script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -119,15 +119,9 @@
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

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/base.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/ordering.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/search.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/input.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/radio.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/select.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/login.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/login.html`

 * *Files 20% similar despite different names*

```diff
@@ -211,64 +211,24 @@
 00000d20: 756e 6465 642d 626f 7474 6f6d 2d34 223e  unded-bottom-4">
 00000d30: 3c2f 6469 763e 0d0a 2020 2020 2020 2020  </div>..        
 00000d40: 3c2f 6469 763e 0d0a 2020 2020 2020 3c2f  </div>..      </
 00000d50: 6469 763e 0d0a 2020 2020 3c2f 6469 763e  div>..    </div>
 00000d60: 0d0a 2020 3c2f 626f 6479 3e0d 0a7b 2520  ..  </body>..{% 
 00000d70: 656e 6462 6c6f 636b 2025 7d0d 0a0d 0a0d  endblock %}.....
 00000d80: 0a7b 2520 626c 6f63 6b20 7363 7269 7074  .{% block script
-00000d90: 2025 7d0d 0a20 203c 7363 7269 7074 3e0d   %}..  <script>.
-00000da0: 0a20 2020 2077 696e 646f 772e 6472 6620  .    window.drf 
-00000db0: 3d20 7b0d 0a20 2020 2020 2063 7372 6648  = {..      csrfH
-00000dc0: 6561 6465 724e 616d 653a 2022 7b7b 2063  eaderName: "{{ c
-00000dd0: 7372 665f 6865 6164 6572 5f6e 616d 657c  srf_header_name|
-00000de0: 6465 6661 756c 743a 2758 2d43 5352 4654  default:'X-CSRFT
-00000df0: 6f6b 656e 2720 7d7d 222c 0d0a 2020 2020  oken' }}",..    
-00000e00: 2020 6373 7266 546f 6b65 6e3a 2022 7b25    csrfToken: "{%
-00000e10: 2069 6620 7265 7175 6573 7420 257d 7b7b   if request %}{{
-00000e20: 2063 7372 665f 746f 6b65 6e20 7d7d 7b25   csrf_token }}{%
-00000e30: 2065 6e64 6966 2025 7d22 0d0a 2020 2020   endif %}"..    
-00000e40: 7d3b 0d0a 2020 3c2f 7363 7269 7074 3e0d  };..  </script>.
-00000e50: 0a20 203c 7363 7269 7074 2073 7263 3d22  .  <script src="
-00000e60: 7b25 2073 7461 7469 6320 2272 6573 745f  {% static "rest_
-00000e70: 6672 616d 6577 6f72 6b2f 6a73 2f6a 7175  framework/js/jqu
-00000e80: 6572 792d 332e 352e 312e 6d69 6e2e 6a73  ery-3.5.1.min.js
-00000e90: 2220 257d 223e 3c2f 7363 7269 7074 3e0d  " %}"></script>.
-00000ea0: 0a20 203c 7363 7269 7074 2073 7263 3d22  .  <script src="
-00000eb0: 7b25 2073 7461 7469 6320 2272 6573 745f  {% static "rest_
-00000ec0: 6672 616d 6577 6f72 6b2f 6a73 2f61 6a61  framework/js/aja
-00000ed0: 782d 666f 726d 2e6a 7322 2025 7d22 3e3c  x-form.js" %}"><
-00000ee0: 2f73 6372 6970 743e 0d0a 2020 3c73 6372  /script>..  <scr
-00000ef0: 6970 7420 7372 633d 227b 2520 7374 6174  ipt src="{% stat
-00000f00: 6963 2022 7265 7374 5f66 7261 6d65 776f  ic "rest_framewo
-00000f10: 726b 2f6a 732f 6373 7266 2e6a 7322 2025  rk/js/csrf.js" %
-00000f20: 7d22 3e3c 2f73 6372 6970 743e 0d0a 2020  }"></script>..  
-00000f30: 3c73 6372 6970 7420 7372 633d 227b 2520  <script src="{% 
-00000f40: 7374 6174 6963 2022 7265 7374 5f66 7261  static "rest_fra
-00000f50: 6d65 776f 726b 2f6a 732f 7072 6574 7469  mework/js/pretti
-00000f60: 6679 2d6d 696e 2e6a 7322 2025 7d22 3e3c  fy-min.js" %}"><
-00000f70: 2f73 6372 6970 743e 0d0a 2020 3c73 6372  /script>..  <scr
-00000f80: 6970 7420 7372 633d 227b 2520 7374 6174  ipt src="{% stat
-00000f90: 6963 2022 7265 7374 5f66 7261 6d65 776f  ic "rest_framewo
-00000fa0: 726b 2f6a 732f 6465 6661 756c 742e 6a73  rk/js/default.js
-00000fb0: 2220 257d 223e 3c2f 7363 7269 7074 3e0d  " %}"></script>.
-00000fc0: 0a20 203c 7363 7269 7074 3e0d 0a20 2020  .  <script>..   
-00000fd0: 2024 2864 6f63 756d 656e 7429 2e72 6561   $(document).rea
-00000fe0: 6479 2866 756e 6374 696f 6e28 2920 7b0d  dy(function() {.
-00000ff0: 0a20 2020 2020 2024 2827 666f 726d 2729  .      $('form')
-00001000: 2e61 6a61 7846 6f72 6d28 293b 0d0a 2020  .ajaxForm();..  
-00001010: 2020 7d29 3b0d 0a20 203c 2f73 6372 6970    });..  </scrip
-00001020: 743e 0d0a 2020 3c73 6372 6970 7420 7372  t>..  <script sr
-00001030: 633d 2268 7474 7073 3a2f 2f63 646e 2e6a  c="https://cdn.j
-00001040: 7364 656c 6976 722e 6e65 742f 6e70 6d2f  sdelivr.net/npm/
-00001050: 626f 6f74 7374 7261 7040 352e 332e 302d  bootstrap@5.3.0-
-00001060: 616c 7068 6133 2f64 6973 742f 6a73 2f62  alpha3/dist/js/b
-00001070: 6f6f 7473 7472 6170 2e62 756e 646c 652e  ootstrap.bundle.
-00001080: 6d69 6e2e 6a73 220d 0a20 2020 2069 6e74  min.js"..    int
-00001090: 6567 7269 7479 3d22 7368 6133 3834 2d45  egrity="sha384-E
-000010a0: 4e6a 644f 3444 7232 626b 4249 4678 5170  NjdO4Dr2bkBIFxQp
-000010b0: 656f 547a 3148 4963 6a65 3339 576d 346a  eoTz1HIcje39Wm4j
-000010c0: 444b 6466 3139 5538 6749 3464 6451 3347  DKdf19U8gI4ddQ3G
-000010d0: 594e 5337 4e54 4b66 4164 5651 535a 6522  YNS7NTKfAdVQSZe"
-000010e0: 0d0a 2020 2020 6372 6f73 736f 7269 6769  ..    crossorigi
-000010f0: 6e3d 2261 6e6f 6e79 6d6f 7573 223e 3c2f  n="anonymous"></
-00001100: 7363 7269 7074 3e0d 0a7b 2520 656e 6462  script>..{% endb
-00001110: 6c6f 636b 2025 7d                        lock %}
+00000d90: 2025 7d0d 0a20 207b 7b20 626c 6f63 6b2e   %}..  {{ block.
+00000da0: 7375 7065 7220 7d7d 0d0a 2020 3c73 6372  super }}..  <scr
+00000db0: 6970 7420 7372 633d 2268 7474 7073 3a2f  ipt src="https:/
+00000dc0: 2f63 646e 2e6a 7364 656c 6976 722e 6e65  /cdn.jsdelivr.ne
+00000dd0: 742f 6e70 6d2f 626f 6f74 7374 7261 7040  t/npm/bootstrap@
+00000de0: 352e 332e 302d 616c 7068 6133 2f64 6973  5.3.0-alpha3/dis
+00000df0: 742f 6a73 2f62 6f6f 7473 7472 6170 2e62  t/js/bootstrap.b
+00000e00: 756e 646c 652e 6d69 6e2e 6a73 220d 0a20  undle.min.js".. 
+00000e10: 2020 2069 6e74 6567 7269 7479 3d22 7368     integrity="sh
+00000e20: 6133 3834 2d45 4e6a 644f 3444 7232 626b  a384-ENjdO4Dr2bk
+00000e30: 4249 4678 5170 656f 547a 3148 4963 6a65  BIFxQpeoTz1HIcje
+00000e40: 3339 576d 346a 444b 6466 3139 5538 6749  39Wm4jDKdf19U8gI
+00000e50: 3464 6451 3347 594e 5337 4e54 4b66 4164  4ddQ3GYNS7NTKfAd
+00000e60: 5651 535a 6522 0d0a 2020 2020 6372 6f73  VQSZe"..    cros
+00000e70: 736f 7269 6769 6e3d 2261 6e6f 6e79 6d6f  sorigin="anonymo
+00000e80: 7573 223e 3c2f 7363 7269 7074 3e0d 0a7b  us"></script>..{
+00000e90: 2520 656e 6462 6c6f 636b 2025 7d         % endblock %}
```

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/pagination/numbers.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.8/PKG-INFO` & `rest_framework_redesign-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-redesign
-Version: 0.1.8
+Version: 0.1.9
 Summary: Redesign of the browsable api of Django REST Framework
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

