# Comparing `tmp/django_breeze-0.1.6.tar.gz` & `tmp/django_breeze-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_breeze-0.1.6.tar", max compression
+gzip compressed data, was "django_breeze-0.2.0.tar", max compression
```

## Comparing `django_breeze-0.1.6.tar` & `django_breeze-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
--rw-r--r--   0        0        0     1066 2023-04-20 12:19:20.337512 django_breeze-0.1.6/LICENSE.md
--rw-r--r--   0        0        0     3434 2023-04-20 12:19:20.337512 django_breeze-0.1.6/README.md
--rw-r--r--   0        0        0       61 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/__init__.py
--rw-r--r--   0        0        0      222 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/__main__.py
--rw-r--r--   0        0        0      814 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/apps.py
--rw-r--r--   0        0        0        0 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/core/__init__.py
--rw-r--r--   0        0        0     4100 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/core/management/__init__.py
--rw-r--r--   0        0        0      719 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/middleware.py
--rw-r--r--   0        0        0      232 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/scripts/django_breeze.py
--rw-r--r--   0        0        0     3057 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/settings.py
--rw-r--r--   0        0        0   129342 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/static/django_breeze/django-breeze-logo.jpg
--rw-r--r--   0        0        0   211529 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/static/django_breeze/django-breeze-logo.png
--rw-r--r--   0        0        0      322 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/.gitignore
--rw-r--r--   0        0        0      561 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/package.json
--rw-r--r--   0        0        0       80 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/postcss.config.js
--rw-r--r--   0        0        0      115 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/Layout/SiteLayout.jsx
--rw-r--r--   0        0        0     4126 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/assets/react.svg
--rw-r--r--   0        0        0       58 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/index.css
--rw-r--r--   0        0        0      416 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/index.html
--rw-r--r--   0        0        0      544 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/main.jsx
--rw-r--r--   0        0        0      983 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/pages/index.jsx
--rw-r--r--   0        0        0      174 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/tailwind.config.js
--rw-r--r--   0        0        0      814 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/vite.config.js
--rw-r--r--   0        0        0      322 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/.gitignore
--rw-r--r--   0        0        0      577 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/package.json
--rw-r--r--   0        0        0       80 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/postcss.config.js
--rw-r--r--   0        0        0     1497 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/public/vite.svg
--rw-r--r--   0        0        0      115 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/Layout/SiteLayout.tsx
--rw-r--r--   0        0        0     4126 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/assets/react.svg
--rw-r--r--   0        0        0       59 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/index.css
--rw-r--r--   0        0        0      417 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/index.html
--rw-r--r--   0        0        0      544 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/main.tsx
--rw-r--r--   0        0        0     1024 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/pages/index.tsx
--rw-r--r--   0        0        0       38 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/vite-env.d.ts
--rw-r--r--   0        0        0      174 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/tailwind.config.js
--rw-r--r--   0        0        0      559 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/tsconfig.json
--rw-r--r--   0        0        0      184 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/tsconfig.node.json
--rw-r--r--   0        0        0      814 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/vite.config.ts
--rw-r--r--   0        0        0      130 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/urls.py
--rw-r--r--   0        0        0      354 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/views.py
--rw-r--r--   0        0        0      804 2023-04-20 12:19:20.341512 django_breeze-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 django_breeze-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-24 03:45:06.677082 django_breeze-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     3402 2023-04-24 03:45:06.677082 django_breeze-0.2.0/README.md
+-rw-r--r--   0        0        0       61 2023-04-24 03:45:06.677082 django_breeze-0.2.0/django_breeze/__init__.py
+-rw-r--r--   0        0        0      222 2023-04-24 03:45:06.677082 django_breeze-0.2.0/django_breeze/__main__.py
+-rw-r--r--   0        0        0      814 2023-04-24 03:45:06.677082 django_breeze-0.2.0/django_breeze/apps.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:45:06.677082 django_breeze-0.2.0/django_breeze/core/__init__.py
+-rw-r--r--   0        0        0     4100 2023-04-24 03:45:06.677082 django_breeze-0.2.0/django_breeze/core/management/__init__.py
+-rw-r--r--   0        0        0      719 2023-04-24 03:45:06.677082 django_breeze-0.2.0/django_breeze/middleware.py
+-rw-r--r--   0        0        0      232 2023-04-24 03:45:06.677082 django_breeze-0.2.0/django_breeze/scripts/django_breeze.py
+-rw-r--r--   0        0        0     3145 2023-04-24 03:45:06.677082 django_breeze-0.2.0/django_breeze/settings.py
+-rw-r--r--   0        0        0   129342 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/static/django_breeze/django-breeze-logo.jpg
+-rw-r--r--   0        0        0   211529 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/static/django_breeze/django-breeze-logo.png
+-rw-r--r--   0        0        0      322 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/.gitignore
+-rw-r--r--   0        0        0      561 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/package.json
+-rw-r--r--   0        0        0       80 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/postcss.config.js
+-rw-r--r--   0        0        0      115 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/src/Layout/SiteLayout.jsx
+-rw-r--r--   0        0        0     4126 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/src/assets/react.svg
+-rw-r--r--   0        0        0       58 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/src/index.css
+-rw-r--r--   0        0        0      416 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/src/index.html
+-rw-r--r--   0        0        0      544 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/src/main.jsx
+-rw-r--r--   0        0        0      983 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/src/pages/index.jsx
+-rw-r--r--   0        0        0      174 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/tailwind.config.js
+-rw-r--r--   0        0        0      814 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react/vite.config.js
+-rw-r--r--   0        0        0      322 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/.gitignore
+-rw-r--r--   0        0        0      577 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/package.json
+-rw-r--r--   0        0        0       80 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/postcss.config.js
+-rw-r--r--   0        0        0     1497 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/public/vite.svg
+-rw-r--r--   0        0        0      115 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/src/Layout/SiteLayout.tsx
+-rw-r--r--   0        0        0     4126 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/src/assets/react.svg
+-rw-r--r--   0        0        0       59 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/src/index.css
+-rw-r--r--   0        0        0      417 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/src/index.html
+-rw-r--r--   0        0        0      544 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/src/main.tsx
+-rw-r--r--   0        0        0     1024 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/src/pages/index.tsx
+-rw-r--r--   0        0        0       38 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/src/vite-env.d.ts
+-rw-r--r--   0        0        0      174 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/tailwind.config.js
+-rw-r--r--   0        0        0      559 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/tsconfig.json
+-rw-r--r--   0        0        0      184 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/tsconfig.node.json
+-rw-r--r--   0        0        0      814 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templates/react_typescript/vite.config.ts
+-rw-r--r--   0        0        0        0 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templatetags/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/templatetags/django_vite.py
+-rw-r--r--   0        0        0      130 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/urls.py
+-rw-r--r--   0        0        0      354 2023-04-24 03:45:06.681082 django_breeze-0.2.0/django_breeze/views.py
+-rw-r--r--   0        0        0      804 2023-04-24 03:45:06.685082 django_breeze-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4235 1970-01-01 00:00:00.000000 django_breeze-0.2.0/PKG-INFO
```

### Comparing `django_breeze-0.1.6/LICENSE.md` & `django_breeze-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/README.md` & `django_breeze-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
 Add the following apps to your `INSTALLED_APPS` in `settings.py`
 
 ```python
 INSTALLED_APPS = [
   # installed apps,
   'django_breeze',
-  'django_vite',
-  'inertia',
   #...............
 ]
 ```
 
 <!-- Add the Inertia middleware to your `MIDDLEWARE` in `settings.py`
 
 ```python
@@ -74,21 +72,21 @@
 yarn
 ```
 
 ## Start Servers
 
 Run the following commands to start your development servers.
 
-### Vite server
+1. Vite server
 
 ```bash
 npm run dev
 ```
 
-### Django server
+2. Django server
 
 ```bash
 python manage.py runserver
 ```
 
 Now you're all set!
```

### Comparing `django_breeze-0.1.6/django_breeze/apps.py` & `django_breeze-0.2.0/django_breeze/apps.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/core/management/__init__.py` & `django_breeze-0.2.0/django_breeze/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/middleware.py` & `django_breeze-0.2.0/django_breeze/middleware.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/settings.py` & `django_breeze-0.2.0/django_breeze/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.conf import settings as django_settings
 from inertia.settings import settings as inertia_settings
 from pathlib import Path
+import inertia
 
 
 def initialize() -> None:
     """Initialize all neccessary django, inertia and django-vite settings"""
     BASE_DIR = getattr(django_settings, "BASE_DIR")
 
     MIDDLEWARES = [
@@ -74,15 +75,18 @@
                 settings[key] = value
 
     for key, value in settings.items():
         setattr(django_settings, key, value)
 
     TEMPLATE_DIR = Path(getattr(django_settings, "TEMPLATE_DIR_PATH"))
 
-    django_settings.TEMPLATES[0]["DIRS"].append(TEMPLATE_DIR)
+    django_settings.TEMPLATES[0]["DIRS"].extend(
+        [TEMPLATE_DIR, Path(inertia.__file__).resolve().parent / "templates/"]
+    )
+
     django_settings.STATICFILES_DIRS.extend(
         [
             django_settings.DJANGO_VITE_ASSETS_PATH,
             TEMPLATE_DIR / "assets",
             TEMPLATE_DIR / "public",
         ]
     )
```

### Comparing `django_breeze-0.1.6/django_breeze/static/django_breeze/django-breeze-logo.jpg` & `django_breeze-0.2.0/django_breeze/static/django_breeze/django-breeze-logo.jpg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/static/django_breeze/django-breeze-logo.png` & `django_breeze-0.2.0/django_breeze/static/django_breeze/django-breeze-logo.png`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react/package.json` & `django_breeze-0.2.0/django_breeze/templates/react/package.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react/src/assets/react.svg` & `django_breeze-0.2.0/django_breeze/templates/react/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react/src/main.jsx` & `django_breeze-0.2.0/django_breeze/templates/react/src/main.jsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react/src/pages/index.jsx` & `django_breeze-0.2.0/django_breeze/templates/react/src/pages/index.jsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react/vite.config.js` & `django_breeze-0.2.0/django_breeze/templates/react/vite.config.js`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react_typescript/package.json` & `django_breeze-0.2.0/django_breeze/templates/react_typescript/package.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react_typescript/public/vite.svg` & `django_breeze-0.2.0/django_breeze/templates/react_typescript/public/vite.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react_typescript/src/assets/react.svg` & `django_breeze-0.2.0/django_breeze/templates/react_typescript/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react_typescript/src/main.tsx` & `django_breeze-0.2.0/django_breeze/templates/react_typescript/src/main.tsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react_typescript/src/pages/index.tsx` & `django_breeze-0.2.0/django_breeze/templates/react_typescript/src/pages/index.tsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react_typescript/tsconfig.json` & `django_breeze-0.2.0/django_breeze/templates/react_typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/django_breeze/templates/react_typescript/vite.config.ts` & `django_breeze-0.2.0/django_breeze/templates/react_typescript/vite.config.ts`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.6/pyproject.toml` & `django_breeze-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-breeze"
-version =  "0.1.6"
+version =  "0.2.0"
 description = "Django Breeze provides a minimal and simple starting point for building a Django application with Inertia and Vite with minimal or no configuration. Styled with Tailwind CSS."
 keywords = ["react", "django", "vue", "inertia", "vite"]
 authors = ["louxsdon <louisayivi.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Louxsdon/django-breeze"
 packages = [{include = "django_breeze"}]
```

### Comparing `django_breeze-0.1.6/PKG-INFO` & `django_breeze-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-breeze
-Version: 0.1.6
+Version: 0.2.0
 Summary: Django Breeze provides a minimal and simple starting point for building a Django application with Inertia and Vite with minimal or no configuration. Styled with Tailwind CSS.
 Home-page: https://github.com/Louxsdon/django-breeze
 License: MIT
 Keywords: react,django,vue,inertia,vite
 Author: louxsdon
 Author-email: louisayivi.dev@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -37,16 +37,14 @@
 
 Add the following apps to your `INSTALLED_APPS` in `settings.py`
 
 ```python
 INSTALLED_APPS = [
   # installed apps,
   'django_breeze',
-  'django_vite',
-  'inertia',
   #...............
 ]
 ```
 
 <!-- Add the Inertia middleware to your `MIDDLEWARE` in `settings.py`
 
 ```python
@@ -93,21 +91,21 @@
 yarn
 ```
 
 ## Start Servers
 
 Run the following commands to start your development servers.
 
-### Vite server
+1. Vite server
 
 ```bash
 npm run dev
 ```
 
-### Django server
+2. Django server
 
 ```bash
 python manage.py runserver
 ```
 
 Now you're all set!
```

