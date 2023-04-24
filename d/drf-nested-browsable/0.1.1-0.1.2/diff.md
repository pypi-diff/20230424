# Comparing `tmp/drf_nested_browsable-0.1.1.tar.gz` & `tmp/drf_nested_browsable-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_nested_browsable-0.1.1.tar", max compression
+gzip compressed data, was "drf_nested_browsable-0.1.2.tar", max compression
```

## Comparing `drf_nested_browsable-0.1.1.tar` & `drf_nested_browsable-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1332 2023-04-23 11:15:15.887977 drf_nested_browsable-0.1.1/README.md
--rw-r--r--   0        0        0      213 2023-04-23 08:13:02.976124 drf_nested_browsable-0.1.1/drf_nested_browsable/__init__.py
--rw-r--r--   0        0        0     4385 2023-04-23 08:23:30.043605 drf_nested_browsable-0.1.1/drf_nested_browsable/serializers.py
--rw-r--r--   0        0        0     3107 2023-04-23 08:30:02.544106 drf_nested_browsable-0.1.1/drf_nested_browsable/templates/writable_list.html
--rw-r--r--   0        0        0        0 2023-04-21 13:53:21.631214 drf_nested_browsable-0.1.1/drf_nested_browsable/templatetags/__init__.py
--rw-r--r--   0        0        0     1338 2023-04-23 11:12:11.747713 drf_nested_browsable-0.1.1/drf_nested_browsable/templatetags/drf_nested_browsable.py
--rw-r--r--   0        0        0     1099 2023-04-23 11:50:03.947558 drf_nested_browsable-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.1/setup.py
--rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1361 2023-04-24 15:12:49.325818 drf_nested_browsable-0.1.2/README.md
+-rw-r--r--   0        0        0      213 2023-04-23 08:13:02.976124 drf_nested_browsable-0.1.2/drf_nested_browsable/__init__.py
+-rw-r--r--   0        0        0     4385 2023-04-23 08:23:30.043605 drf_nested_browsable-0.1.2/drf_nested_browsable/serializers.py
+-rw-r--r--   0        0        0     3463 2023-04-24 15:10:03.715669 drf_nested_browsable-0.1.2/drf_nested_browsable/templates/writable_list.html
+-rw-r--r--   0        0        0        0 2023-04-21 13:53:21.631214 drf_nested_browsable-0.1.2/drf_nested_browsable/templatetags/__init__.py
+-rw-r--r--   0        0        0     1809 2023-04-24 14:57:46.511666 drf_nested_browsable-0.1.2/drf_nested_browsable/templatetags/drf_nested_browsable.py
+-rw-r--r--   0        0        0     1099 2023-04-24 15:13:47.335870 drf_nested_browsable-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2240 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.2/setup.py
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.2/PKG-INFO
```

### Comparing `drf_nested_browsable-0.1.1/README.md` & `drf_nested_browsable-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -26,11 +26,11 @@
 * Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class
 * Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API
 * Basic example
 
 ### To do
 
 * Make the current example work :
-  * Fix backend and form for multiple levels of nesting
   * Do not show `parent` select list when showing forms as children of another form
+  * Show `details` (`HyperlinkedIdentityField`) when displayed as a child Serializer
 * Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)
 * Write tests/specs
```

### Comparing `drf_nested_browsable-0.1.1/drf_nested_browsable/serializers.py` & `drf_nested_browsable-0.1.2/drf_nested_browsable/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.1.1/drf_nested_browsable/templates/writable_list.html` & `drf_nested_browsable-0.1.2/drf_nested_browsable/templates/writable_list.html`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,22 @@
       </legend>
     </div>
   {% endif %}
 
   {% with templateId=field.name|addstr:"-form-template" %}
     <div class="inner-form-list">
       {% if field.tree_root is None or field.tree_root %}
+      {% with placeholder=field.name|fieldname_to_placeholder %}
       <div class="inner-form-template" id="{{templateId}}">
-        <div class="inner-form-entry" data-index="{i}">
-          {% render_nested field.child prefix=field.name|addstr:"[{i}]" %}
+          <div class="inner-form-entry" data-index="{{ placeholder }}">
+          {% render_nested field.child prefix=field.name|addstr:"["|addstr:placeholder|addstr:"]" %}
           <button class="del-entry" data-field="{{field.name}}">-</button>
         </div>
       </div>
+      {% endwith %}
       {% endif %}
 
       <pre>
 {{ field.child }}
       </pre>
 
       {% for entry in field.value %}
@@ -39,38 +41,42 @@
         </div>
       {% endfor %}
     </div>
     <div class="inner-form-new">
       <button class="add-entry" data-field="{{field.name}}">+</button>
     </div>
     <script>
-      window.onload = function () {
-              function addDelEvents() {
+        window.onload = function () {
+            function addDelEvents() {
                 $('.inner-form-entry > button.del-entry').on('click', function(e){
-                        e.preventDefault();
-                        $(this).parent().remove();
+                    e.preventDefault();
+                    $(this).parent().remove();
                 })
-              }
-              $('.inner-form-new > button.add-entry').on('click', function(e){
-                      e.preventDefault();
-                      let id = $(this).data("field")+"-form-template";
-                      let templateElem = $("#"+id);
-                      let n = templateElem.parent().children(".inner-form-entry").last().data("index") + 1;
-                      n = n?n:0;
-                      let newHtml = templateElem.html().replaceAll("{i}",n);
-                      templateElem.parent().append(newHtml);
-                      addDelEvents();
-              })
-              addDelEvents();
-              $('form').on('submit', function() {
-                      console.log($('.inner-form-template'));
-                      $(".inner-form-template").remove();
-                      console.log($('.inner-form-template'));
-              })
-      };
+            }
+            function addButtonHandler(e){
+                e.preventDefault();
+                let id = $(this).data("field")+"-form-template";
+                let templateElem = $(document.getElementById(id));
+                let n = templateElem.parent().children(".inner-form-entry").last().data("index") + 1;
+                n = n?n:0;
+                let newHtml = templateElem.html().replaceAll("{i}",n);
+                newHtml = newHtml.replaceAll("{ii","{i");
+                templateElem.parent().append(newHtml);
+                addDelEvents();
+                let newElem = templateElem.parent().children(".inner-form-entry").last();
+                newElem.find('.inner-form-new > button.add-entry').on('click', addButtonHandler);
+            }
+            $('.inner-form-new > button.add-entry').on('click', addButtonHandler)
+            addDelEvents();
+            $('form').on('submit', function() {
+                console.log($('.inner-form-template'));
+                $(".inner-form-template").remove();
+                console.log($('.inner-form-template'));
+            })
+        };
     </script>
   {% endwith %}
 <style>
 .inner-form-template {
   display: none;
 }
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 {% load rest_framework %} {% load drf_nested_browsable %}  {% if field.label %}
  {{ field.label }}
 {% endif %} {% with templateId=field.name|addstr:"-form-template" %}
-{% if field.tree_root is None or field.tree_root %}
-{% render_nested field.child prefix=field.name|addstr:"[{i}]" %} -
-{% endif %}
+{% if field.tree_root is None or field.tree_root %} {% with
+placeholder=field.name|fieldname_to_placeholder %}
+{% render_nested field.child prefix=field.name|addstr:"["|addstr:
+placeholder|addstr:"]" %} -
+{% endwith %} {% endif %}
 {{ field.child }}
 {% for entry in field.value %}
 {% if field.proxied is None %} {% render_nested field.child data=entry
 prefix=field.name|addstr:"["|addstr:forloop.counter0|addstr:"]" %} Not proxied
 {% else %} {% render_nested field.proxied.child data=entry
 prefix=field.name|addstr:"["|addstr:forloop.counter0|addstr:"]" %} Proxied {%
 endif %} -
```

### Comparing `drf_nested_browsable-0.1.1/pyproject.toml` & `drf_nested_browsable-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-nested-browsable"
-version = "0.1.1"
+version = "0.1.2"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Framework :: Django",
     "Intended Audience :: Developers"
 ]
 description = "Writable nested serializers with forms for the Browsable API"
 keywords = ["django", "rest framework", "drf", "browsable api", "nested serializers"]
```

### Comparing `drf_nested_browsable-0.1.1/setup.py` & `drf_nested_browsable-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'drf_nested_browsable': ['templates/*']}
 
 install_requires = \
 ['django>=4.2,<5.0', 'djangorestframework>=3.14.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'drf-nested-browsable',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Writable nested serializers with forms for the Browsable API',
-    'long_description': ":warning: Work In Progress :warning:\n\n# Writable Nested Serializers with Browsable API Forms\n\nThis plugin is intended to provide writable nested serializers (similar to [the recommended plugin from DRF documentation](https://github.com/beda-software/drf-nested-browsable.git)) that bring their own forms for the Browsable API renderer.\n\n## Try it out\n\nThis project's dependencies are managed using [`poetry`](https://python-poetry.org/)\n\n```bash\ngit clone https://github.com/pcouy/drf-nested-browsable\ncd drf-nested-browsable\npoetry install\ncd example\npython manage.py migrate\npython manage.py runserver\n```\n\nThe above commands will install the dependencies, run the DB migrations, and launch a development server of the example project that uses the provided serializers.\n\n## Current state of the project\n\n### Done\n\n* Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class\n* Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API\n* Basic example\n\n### To do\n\n* Make the current example work :\n  * Fix backend and form for multiple levels of nesting\n  * Do not show `parent` select list when showing forms as children of another form\n* Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)\n* Write tests/specs\n",
+    'long_description': ":warning: Work In Progress :warning:\n\n# Writable Nested Serializers with Browsable API Forms\n\nThis plugin is intended to provide writable nested serializers (similar to [the recommended plugin from DRF documentation](https://github.com/beda-software/drf-nested-browsable.git)) that bring their own forms for the Browsable API renderer.\n\n## Try it out\n\nThis project's dependencies are managed using [`poetry`](https://python-poetry.org/)\n\n```bash\ngit clone https://github.com/pcouy/drf-nested-browsable\ncd drf-nested-browsable\npoetry install\ncd example\npython manage.py migrate\npython manage.py runserver\n```\n\nThe above commands will install the dependencies, run the DB migrations, and launch a development server of the example project that uses the provided serializers.\n\n## Current state of the project\n\n### Done\n\n* Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class\n* Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API\n* Basic example\n\n### To do\n\n* Make the current example work :\n  * Do not show `parent` select list when showing forms as children of another form\n  * Show `details` (`HyperlinkedIdentityField`) when displayed as a child Serializer\n* Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)\n* Write tests/specs\n",
     'author': 'Pierre Couy',
     'author_email': 'contact@pierre-couy.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pierre-couy.dev/projects/drf-nested-browsable.html',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `drf_nested_browsable-0.1.1/PKG-INFO` & `drf_nested_browsable-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-nested-browsable
-Version: 0.1.1
+Version: 0.1.2
 Summary: Writable nested serializers with forms for the Browsable API
 Home-page: https://pierre-couy.dev/projects/drf-nested-browsable.html
 License: MIT
 Keywords: django,rest framework,drf,browsable api,nested serializers
 Author: Pierre Couy
 Author-email: contact@pierre-couy.dev
 Requires-Python: >=3.10,<4.0
@@ -48,12 +48,12 @@
 * Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class
 * Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API
 * Basic example
 
 ### To do
 
 * Make the current example work :
-  * Fix backend and form for multiple levels of nesting
   * Do not show `parent` select list when showing forms as children of another form
+  * Show `details` (`HyperlinkedIdentityField`) when displayed as a child Serializer
 * Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)
 * Write tests/specs
```

