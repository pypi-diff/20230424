# Comparing `tmp/rt-option-menu-0.1.5.tar.gz` & `tmp/rt-option-menu-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rt-option-menu-0.1.5.tar", last modified: Tue Mar 28 18:42:00 2023, max compression
+gzip compressed data, was "rt-option-menu-0.1.6.tar", last modified: Mon Apr 24 20:41:41 2023, max compression
```

## Comparing `rt-option-menu-0.1.5.tar` & `rt-option-menu-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-03-28 18:42:00.894439 rt-option-menu-0.1.5/
--rw-r--r--   0 jared      (502) staff       (20)     1063 2023-03-09 22:22:22.000000 rt-option-menu-0.1.5/LICENSE
--rw-r--r--   0 jared      (502) staff       (20)       50 2023-03-10 17:15:58.000000 rt-option-menu-0.1.5/MANIFEST.in
--rw-r--r--   0 jared      (502) staff       (20)      209 2023-03-28 18:42:00.894269 rt-option-menu-0.1.5/PKG-INFO
-drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-03-28 18:42:00.881226 rt-option-menu-0.1.5/rt_option_menu/
--rw-r--r--   0 jared      (502) staff       (20)     4711 2023-03-28 18:38:37.000000 rt-option-menu-0.1.5/rt_option_menu/__init__.py
-drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-03-28 18:42:00.879935 rt-option-menu-0.1.5/rt_option_menu/frontend/
-drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-03-28 18:42:00.883905 rt-option-menu-0.1.5/rt_option_menu/frontend/build/
--rw-r--r--   0 jared      (502) staff       (20)      859 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/asset-manifest.json
--rw-r--r--   0 jared      (502) staff       (20)   197459 2023-03-28 18:37:53.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/bootstrap.min.css
--rw-r--r--   0 jared      (502) staff       (20)     2101 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/index.html
--rw-r--r--   0 jared      (502) staff       (20)      564 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/precache-manifest.a578b4c5e6f2a1d58f4fedbde90b383a.js
--rw-r--r--   0 jared      (502) staff       (20)     1183 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/service-worker.js
-drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-03-28 18:42:00.880131 rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/
-drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-03-28 18:42:00.893922 rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/
--rw-r--r--   0 jared      (502) staff       (20)  3695779 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js
--rw-r--r--   0 jared      (502) staff       (20)     1803 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.LICENSE.txt
--rw-r--r--   0 jared      (502) staff       (20)  9826830 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.map
--rw-r--r--   0 jared      (502) staff       (20)     3305 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/main.1e62fb47.chunk.js
--rw-r--r--   0 jared      (502) staff       (20)    10653 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/main.1e62fb47.chunk.js.map
--rw-r--r--   0 jared      (502) staff       (20)     1598 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js
--rw-r--r--   0 jared      (502) staff       (20)     8317 2023-03-28 18:38:09.000000 rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js.map
-drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-03-28 18:42:00.882041 rt-option-menu-0.1.5/rt_option_menu.egg-info/
--rw-r--r--   0 jared      (502) staff       (20)      209 2023-03-28 18:42:00.000000 rt-option-menu-0.1.5/rt_option_menu.egg-info/PKG-INFO
--rw-r--r--   0 jared      (502) staff       (20)      975 2023-03-28 18:42:00.000000 rt-option-menu-0.1.5/rt_option_menu.egg-info/SOURCES.txt
--rw-r--r--   0 jared      (502) staff       (20)        1 2023-03-28 18:42:00.000000 rt-option-menu-0.1.5/rt_option_menu.egg-info/dependency_links.txt
--rw-r--r--   0 jared      (502) staff       (20)       16 2023-03-28 18:42:00.000000 rt-option-menu-0.1.5/rt_option_menu.egg-info/requires.txt
--rw-r--r--   0 jared      (502) staff       (20)       15 2023-03-28 18:42:00.000000 rt-option-menu-0.1.5/rt_option_menu.egg-info/top_level.txt
--rw-r--r--   0 jared      (502) staff       (20)       38 2023-03-28 18:42:00.894501 rt-option-menu-0.1.5/setup.cfg
--rw-r--r--   0 jared      (502) staff       (20)      592 2023-03-28 18:38:04.000000 rt-option-menu-0.1.5/setup.py
+drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-04-24 20:41:41.918115 rt-option-menu-0.1.6/
+-rw-r--r--   0 jared      (502) staff       (20)     1063 2023-03-09 22:22:22.000000 rt-option-menu-0.1.6/LICENSE
+-rw-r--r--   0 jared      (502) staff       (20)       50 2023-03-10 17:15:58.000000 rt-option-menu-0.1.6/MANIFEST.in
+-rw-r--r--   0 jared      (502) staff       (20)      209 2023-04-24 20:41:41.917970 rt-option-menu-0.1.6/PKG-INFO
+drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-04-24 20:41:41.906302 rt-option-menu-0.1.6/rt_option_menu/
+-rw-r--r--   0 jared      (502) staff       (20)     4711 2023-04-24 20:40:18.000000 rt-option-menu-0.1.6/rt_option_menu/__init__.py
+drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-04-24 20:41:41.905315 rt-option-menu-0.1.6/rt_option_menu/frontend/
+drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-04-24 20:41:41.908495 rt-option-menu-0.1.6/rt_option_menu/frontend/build/
+-rw-r--r--   0 jared      (502) staff       (20)      859 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/asset-manifest.json
+-rw-r--r--   0 jared      (502) staff       (20)   197459 2023-04-24 20:40:11.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/bootstrap.min.css
+-rw-r--r--   0 jared      (502) staff       (20)     2101 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/index.html
+-rw-r--r--   0 jared      (502) staff       (20)      564 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/precache-manifest.71f79d5ea2999be28b3897d680cde1c7.js
+-rw-r--r--   0 jared      (502) staff       (20)     1183 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/service-worker.js
+drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-04-24 20:41:41.905583 rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/
+drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-04-24 20:41:41.917750 rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/
+-rw-r--r--   0 jared      (502) staff       (20)  3695779 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js
+-rw-r--r--   0 jared      (502) staff       (20)     1803 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.LICENSE.txt
+-rw-r--r--   0 jared      (502) staff       (20)  9826830 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.map
+-rw-r--r--   0 jared      (502) staff       (20)     3256 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/main.ec56508e.chunk.js
+-rw-r--r--   0 jared      (502) staff       (20)    10604 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/main.ec56508e.chunk.js.map
+-rw-r--r--   0 jared      (502) staff       (20)     1598 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js
+-rw-r--r--   0 jared      (502) staff       (20)     8317 2023-04-24 20:40:46.000000 rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js.map
+drwxr-xr-x   0 jared      (502) staff       (20)        0 2023-04-24 20:41:41.907383 rt-option-menu-0.1.6/rt_option_menu.egg-info/
+-rw-r--r--   0 jared      (502) staff       (20)      209 2023-04-24 20:41:41.000000 rt-option-menu-0.1.6/rt_option_menu.egg-info/PKG-INFO
+-rw-r--r--   0 jared      (502) staff       (20)      975 2023-04-24 20:41:41.000000 rt-option-menu-0.1.6/rt_option_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 jared      (502) staff       (20)        1 2023-04-24 20:41:41.000000 rt-option-menu-0.1.6/rt_option_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 jared      (502) staff       (20)       16 2023-04-24 20:41:41.000000 rt-option-menu-0.1.6/rt_option_menu.egg-info/requires.txt
+-rw-r--r--   0 jared      (502) staff       (20)       15 2023-04-24 20:41:41.000000 rt-option-menu-0.1.6/rt_option_menu.egg-info/top_level.txt
+-rw-r--r--   0 jared      (502) staff       (20)       38 2023-04-24 20:41:41.918167 rt-option-menu-0.1.6/setup.cfg
+-rw-r--r--   0 jared      (502) staff       (20)      592 2023-04-24 20:41:39.000000 rt-option-menu-0.1.6/setup.py
```

### Comparing `rt-option-menu-0.1.5/LICENSE` & `rt-option-menu-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rt-option-menu-0.1.5/rt_option_menu/__init__.py` & `rt-option-menu-0.1.6/rt_option_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/asset-manifest.json` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/asset-manifest.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068181818181819%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.ec56508e.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.ec56508e.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.ec56508e.chunk.js.map', "*

 * *            "'precache-manifest.71f79d5ea2999be28b3897d680cde1c7.js': "*

 * *            "'./precache-manifest.71f79d5ea2999be28b3897d680cde1c7.js', delete: "*

 * *            "['precache-manifest.a578b4c5e6f2a1d58f4fedbde90b383a.js']}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/js/runtime-main.44d30fc2.js",
         "static/js/2.6ff9f471.chunk.js",
-        "static/js/main.1e62fb47.chunk.js"
+        "static/js/main.ec56508e.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.1e62fb47.chunk.js",
-        "main.js.map": "./static/js/main.1e62fb47.chunk.js.map",
-        "precache-manifest.a578b4c5e6f2a1d58f4fedbde90b383a.js": "./precache-manifest.a578b4c5e6f2a1d58f4fedbde90b383a.js",
+        "main.js": "./static/js/main.ec56508e.chunk.js",
+        "main.js.map": "./static/js/main.ec56508e.chunk.js.map",
+        "precache-manifest.71f79d5ea2999be28b3897d680cde1c7.js": "./precache-manifest.71f79d5ea2999be28b3897d680cde1c7.js",
         "runtime-main.js": "./static/js/runtime-main.44d30fc2.js",
         "runtime-main.js.map": "./static/js/runtime-main.44d30fc2.js.map",
         "service-worker.js": "./service-worker.js",
         "static/js/2.6ff9f471.chunk.js": "./static/js/2.6ff9f471.chunk.js",
         "static/js/2.6ff9f471.chunk.js.LICENSE.txt": "./static/js/2.6ff9f471.chunk.js.LICENSE.txt",
         "static/js/2.6ff9f471.chunk.js.map": "./static/js/2.6ff9f471.chunk.js.map"
     }
```

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/bootstrap.min.css` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/index.html` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.6ff9f471.chunk.js"></script><script src="./static/js/main.1e62fb47.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.6ff9f471.chunk.js"></script><script src="./static/js/main.ec56508e.chunk.js"></script></body></html>
```

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/precache-manifest.a578b4c5e6f2a1d58f4fedbde90b383a.js` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/precache-manifest.71f79d5ea2999be28b3897d680cde1c7.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "b0e555ef97b8fb726dfb8209632cc85b",
+    "revision": "1effaa80610e223e2241129858d2be09",
     "url": "./index.html"
 }, {
     "revision": "730ae406e0f1224e9f4e",
     "url": "./static/js/2.6ff9f471.chunk.js"
 }, {
     "revision": "3dc2da520b7611f998bec3f8b32ee24e",
     "url": "./static/js/2.6ff9f471.chunk.js.LICENSE.txt"
 }, {
-    "revision": "30a069eaf418527d0ffb",
-    "url": "./static/js/main.1e62fb47.chunk.js"
+    "revision": "e8b631fd210f738913ec",
+    "url": "./static/js/main.ec56508e.chunk.js"
 }, {
     "revision": "7e9d84e346ce158d1e50",
     "url": "./static/js/runtime-main.44d30fc2.js"
 }]);
```

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/service-worker.js` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/service-worker.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.a578b4c5e6f2a1d58f4fedbde90b383a.js"
+    "./precache-manifest.71f79d5ea2999be28b3897d680cde1c7.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js`

 * *Files identical despite different names*

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.LICENSE.txt` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.map` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.map`

 * *Files identical despite different names*

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/main.1e62fb47.chunk.js` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/main.ec56508e.chunk.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -4,57 +4,57 @@
             e.exports = n(29)
         },
         29: function(e, t, n) {
             "use strict";
             n.r(t);
             var a = n(1),
                 i = n.n(a),
-                r = n(17),
-                c = n.n(r),
+                c = n(17),
+                r = n.n(c),
                 o = n(7),
                 l = n(2),
                 s = n(3),
                 m = n(4),
-                d = n(5),
-                u = n(12),
+                u = n(5),
+                d = n(12),
                 p = n(11),
                 f = n(19),
                 h = n(16),
-                g = ["iconName"],
-                y = function(e) {
+                y = ["iconName"],
+                C = function(e) {
                     var t = e.iconName,
-                        n = Object(p.a)(e, g),
+                        n = Object(p.a)(e, y),
                         a = f[t],
-                        r = Object(o.a)({}, n.style);
-                    return a || (r.visibility = "hidden", a = h.a), i.a.createElement(a, {
+                        c = Object(o.a)({}, n.style);
+                    return a || (c.visibility = "hidden", a = h.a), i.a.createElement(a, {
                         size: n.size,
-                        style: r
+                        style: c
                     })
                 },
-                C = function(e) {
+                b = function(e) {
                     Object(m.a)(n, e);
-                    var t = Object(d.a)(n);
+                    var t = Object(u.a)(n);
 
                     function n(e) {
                         var a;
                         Object(s.a)(this, n), (a = t.call(this, e)).render = function() {
                             var e = a.props.args.choices,
                                 t = a.props.args.options || {},
                                 n = a.state.selectedChoice;
                             if ("horizontal" === t.orientation) {
-                                var r = {
+                                var c = {
                                         padding: "0.25em",
                                         flex: 1,
                                         background: "rgb(237,240,244)",
                                         cursor: "pointer",
                                         textAlign: "center",
                                         userSelect: "none"
                                     },
-                                    c = Object(o.a)(Object(o.a)({}, r), {}, {
-                                        background: "rgb(151, 71, 255)",
+                                    r = Object(o.a)(Object(o.a)({}, c), {}, {
+                                        background: "rgba(107, 101, 255)",
                                         borderRadius: "10px",
                                         color: "white"
                                     });
                                 return i.a.createElement("div", {
                                     style: {
                                         display: "flex",
                                         flexDirection: "row",
@@ -64,15 +64,15 @@
                                         backgroundColor: "rgb(240,240,240)",
                                         padding: "0.5em",
                                         borderRadius: "10px"
                                     }
                                 }, e.map((function(e, t) {
                                     return i.a.createElement("div", {
                                         key: t,
-                                        style: n === e ? c : r,
+                                        style: n === e ? r : c,
                                         onClick: function() {
                                             return a.handleChoiceClick(e)
                                         }
                                     }, e)
                                 })))
                             }
                             var l = {
@@ -82,110 +82,110 @@
                                     marginTop: "1em",
                                     width: "100%",
                                     padding: "0.5em",
                                     userSelect: "none",
                                     cursor: "pointer"
                                 },
                                 s = Object(o.a)(Object(o.a)({}, l), {}, {
-                                    background: "linear-gradient(0deg, rgba(107, 101, 255, 0.12), rgba(107, 101, 255, 0.12))",
+                                    background: "rgba(107, 101, 255, 0.1)",
                                     fontWeight: 500
                                 }),
                                 m = {
                                     marginLeft: "0.5em",
                                     marginRight: "2em"
                                 },
-                                d = {
+                                u = {
                                     marginLeft: "auto"
                                 },
-                                u = {
+                                d = {
                                     fontSize: "15px"
                                 },
                                 p = t.icons || [],
                                 f = t.links || [];
                             return i.a.createElement("div", {
                                 style: {
                                     display: "flex",
                                     flexDirection: "column",
                                     justifyContent: "space-evenly",
                                     alignItems: "flex-start"
                                 }
                             }, e.map((function(e, t) {
-                                var r, c, o = f[t];
-                                return Array.isArray(p[t]) ? (r = p[t][0], c = p[t][1]) : (r = p[t], c = void 0), n === e ? i.a.createElement("div", {
+                                var c, r, o = f[t];
+                                return Array.isArray(p[t]) ? (c = p[t][0], r = p[t][1]) : (c = p[t], r = void 0), n === e ? i.a.createElement("div", {
                                     onClick: function() {
                                         return a.handleChoiceClick(e)
                                     },
                                     style: s
-                                }, i.a.createElement(y, {
-                                    iconName: r,
+                                }, i.a.createElement(C, {
+                                    iconName: c,
                                     size: 25,
                                     style: m
                                 }), i.a.createElement("span", {
-                                    style: u
-                                }, e), i.a.createElement(y, {
-                                    iconName: c,
-                                    size: 25,
                                     style: d
+                                }, e), i.a.createElement(C, {
+                                    iconName: r,
+                                    size: 25,
+                                    style: u
                                 })) : o ? i.a.createElement("div", {
                                     onClick: function() {
                                         return a.handleLinkClick(o)
                                     },
                                     style: l
-                                }, i.a.createElement(y, {
-                                    iconName: r,
+                                }, i.a.createElement(C, {
+                                    iconName: c,
                                     size: 25,
                                     style: m
                                 }), i.a.createElement("span", {
-                                    style: u
-                                }, e), i.a.createElement(y, {
-                                    iconName: c,
-                                    size: 25,
                                     style: d
+                                }, e), i.a.createElement(C, {
+                                    iconName: r,
+                                    size: 25,
+                                    style: u
                                 })) : i.a.createElement("div", {
                                     onClick: function() {
                                         return a.handleChoiceClick(e)
                                     },
                                     style: l
-                                }, i.a.createElement(y, {
-                                    iconName: r,
+                                }, i.a.createElement(C, {
+                                    iconName: c,
                                     size: 25,
                                     style: m
                                 }), i.a.createElement("span", {
-                                    style: u
-                                }, e), i.a.createElement(y, {
-                                    iconName: c,
-                                    size: 25,
                                     style: d
+                                }, e), i.a.createElement(C, {
+                                    iconName: r,
+                                    size: 25,
+                                    style: u
                                 }))
                             })))
                         }, a.handleLinkClick = function(e) {
                             window.open(e, "_blank")
                         }, a.handleChoiceClick = function(e) {
                             a.setState({
                                 selectedChoice: e
                             }), a.setState((function(t) {
                                 return {
                                     selectedChoice: e
                                 }
                             }), (function() {
-                                return u.a.setComponentValue(a.state.selectedChoice)
+                                return d.a.setComponentValue(a.state.selectedChoice)
                             }))
                         };
-                        var r = a.props.args.choices,
-                            c = a.props.args.options || {};
-                        return void 0 !== c.default_index ? (a.state = {
-                            selectedChoice: r[c.default_index]
-                        }, u.a.setComponentValue(a.state.selectedChoice)) : (a.state = {
+                        var c = a.props.args.choices,
+                            r = a.props.args.options || {};
+                        return void 0 !== r.default_index ? (a.state = {
+                            selectedChoice: c[r.default_index]
+                        }, d.a.setComponentValue(a.state.selectedChoice)) : (a.state = {
                             selectedChoice: ""
-                        }, u.a.setComponentValue(a.state.selectedChoice)), a
+                        }, d.a.setComponentValue(a.state.selectedChoice)), a
                     }
                     return Object(l.a)(n)
-                }(u.b),
-                b = Object(u.c)(C);
-            c.a.render(i.a.createElement(i.a.StrictMode, null, i.a.createElement(b, null)), document.getElementById("root"))
+                }(d.b),
+                g = Object(d.c)(b);
+            r.a.render(i.a.createElement(i.a.StrictMode, null, i.a.createElement(g, null)), document.getElementById("root"))
         }
     },
     [
         [20, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.1e62fb47.chunk.js.map
+//# sourceMappingURL=main.ec56508e.chunk.js.map
```

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/main.1e62fb47.chunk.js.map` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/main.ec56508e.chunk.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8214285714285714%*

 * *Differences: {"'file'": "'static/js/main.ec56508e.chunk.js'",*

 * * "'mappings'": "'+SAWaA,EAAO,SAAHC,GAA2C,IAArCC,EAAQD,EAARC,SAAaC,EAAKC,YAAAH,EAAAI,GACnCC,EAAgBC,EAAML,GACpBM,EAASC,YAAA,GAAQN,EAAMO,OAK7B,OAJKJ,IACHE,EAAUG,WAAa,SACvBL,EAAgBC,KAEXK,IAAAC,cAACP,EAAa,CAACQ,KAAMX,EAAMW,KAAMJ,MAAOF,KCM3CO,EAAY,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAChB,SAAAA,EAAYZ,GAAa,IAADiB,EAAAC,YAAA,KAAAN,IACtBK,EAAAF,EAAAI,KAAA,KAAMnB,IAeDoB,OAAS,WAGd,IAAMC,EAAoBJ,EAAKjB,MAAMsB,KAAc,QAC7CC,EAA4BN,EAAKjB,MAAMsB,KAAc,SAAK,GAE1DE,EA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.1e62fb47.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.ec56508e.chunk.js",
+    "mappings": "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",
     "names": [
         "Icon",
         "_ref",
         "iconName",
         "props",
         "_objectWithoutProperties",
         "_excluded",
@@ -91,12 +91,12 @@
     "sources": [
         "Icon.tsx",
         "RtOptionMenu.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "import React from 'react';\nimport * as icons from 'react-bootstrap-icons';\n\ninterface IconProps extends icons.IconProps {\n  // Cannot use \"name\" as it is a valid SVG attribute\n  // \"iconName\", \"filename\", \"icon\" will do it instead\n  iconName: keyof typeof icons;\n  size: number;\n  style: any;\n}\n\nexport const Icon = ({ iconName, ...props }: IconProps) => {\n  let BootstrapIcon = icons[iconName];\n  const iconStyle = { ...props.style };\n  if (!BootstrapIcon){\n    iconStyle.visibility = 'hidden';\n    BootstrapIcon = icons['XCircleFill']\n  }\n  return <BootstrapIcon size={props.size} style={iconStyle} />;\n}",
-        "// @ts-nocheck\nimport {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport { Icon } from \"./Icon\";\n\ninterface State {\n  selectedChoice: string\n}\n\ninterface ComponentOptions {\n  orientation?: string;\n  default_index?: number;\n  icons?: string[];\n  links?: string[];\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nclass RtOptionMenu extends StreamlitComponentBase<State> {\n  constructor(props: any) {\n    super(props);\n    const choices: string[] = this.props.args[\"choices\"];\n\n    const options: ComponentOptions= this.props.args[\"options\"] || {};\n    if (options.default_index !== undefined) {\n      this.state = { selectedChoice: choices[options.default_index] };\n      Streamlit.setComponentValue(this.state.selectedChoice)\n    }\n    else {\n      this.state = { selectedChoice: \"\"};\n      Streamlit.setComponentValue(this.state.selectedChoice)\n    }\n\n  }\n\n  public render = (): ReactNode => {\n    // Arguments that are passed to the plugin in Python are accessible\n    // via `this.props.args`. Here, we access the \"name\" arg.\n    const choices: string[] = this.props.args[\"choices\"];\n    const options: ComponentOptions = this.props.args[\"options\"] || {};\n\n    const selectedChoice = this.state.selectedChoice;\n\n    if (options.orientation === 'horizontal') {\n      const containerStyle = {\n        display: 'flex',\n        flexDirection: 'row' as 'row',\n        alignItems: 'center',\n        justifyContent: 'space-evenly',\n        columnGap: '0.5em',\n        backgroundColor: 'rgb(240,240,240)',\n        padding: '0.5em',\n        borderRadius: '10px'\n      }\n      const elementStyle = {\n        padding: '0.25em',\n        flex: 1,\n        background: 'rgb(237,240,244)',\n        cursor: 'pointer',\n        textAlign: 'center',\n        userSelect: 'none' as 'none',\n      }\n      const selectedElementStyle = {\n        ...elementStyle,\n        background: 'rgb(151, 71, 255)',\n        borderRadius: '10px',\n        color: 'white',\n      }\n      return (\n        <div style={containerStyle}>\n          {choices.map((choice, index) => {\n            return <div key={index} style={selectedChoice === choice ? selectedElementStyle : elementStyle} onClick={() => this.handleChoiceClick(choice)}>{choice}</div>\n          })}\n        </div>\n      )\n    }\n    // vertical style\n    else{\n      const containerStyle = {\n        display: 'flex',\n        flexDirection: 'column' as 'column',\n        justifyContent: 'space-evenly',\n        alignItems: 'flex-start',\n      }\n      const elementStyle = {\n        display: 'flex',\n        flexDirection: 'row' as 'row',\n        alignItems: 'flex-start',\n        marginTop: '1em',\n        width: '100%',\n        padding: '0.5em',\n        userSelect: 'none' as 'none',\n        cursor: 'pointer',\n      }\n      const selectedElementStyle = {\n        ...elementStyle,\n        background: 'linear-gradient(0deg, rgba(107, 101, 255, 0.12), rgba(107, 101, 255, 0.12))',\n        fontWeight: 500\n      }\n      const leftIconStyle = {\n        marginLeft: '0.5em',\n        marginRight: '2em',\n      }\n      const rightIconStyle = {\n        marginLeft: 'auto'\n      }\n      const textStyle = {\n        fontSize: '15px',\n      }\n      const icons = options.icons || [];\n      const links = options.links || [];\n      return (\n        <div style={containerStyle}>\n          {choices.map((choice, index) => {\n            let leftIcon, rightIcon;\n            let link = links[index];\n\n            if (Array.isArray(icons[index])){\n              leftIcon = icons[index][0];\n              rightIcon = icons[index][1];\n            }\n            else {\n              leftIcon = icons[index];\n              rightIcon = undefined;\n            }\n\n            if (selectedChoice === choice){\n              return <div onClick={() => this.handleChoiceClick(choice)} style={selectedElementStyle}><Icon iconName={leftIcon} size={25} style={leftIconStyle}/><span style={textStyle}>{choice}</span><Icon iconName={rightIcon} size={25} style={rightIconStyle}/></div>\n            }\n            else{\n              if (!(link)){\n                return <div onClick={() => this.handleChoiceClick(choice)} style={elementStyle}><Icon iconName={leftIcon} size={25} style={leftIconStyle}/><span style={textStyle}>{choice}</span><Icon iconName={rightIcon} size={25} style={rightIconStyle}/></div>\n              }\n              else{\n                return <div onClick={() => this.handleLinkClick(link)} style={elementStyle}><Icon iconName={leftIcon} size={25} style={leftIconStyle}/><span style={textStyle}>{choice}</span><Icon iconName={rightIcon} size={25} style={rightIconStyle}/></div>\n              }\n            }\n          })}\n        </div>\n      )\n    }\n  }\n\n  private handleLinkClick = (link: string): void => {\n    window.open(link, '_blank');\n  }\n\n  private handleChoiceClick = (clickedChoice: string): void => {\n    this.setState({ selectedChoice: clickedChoice })\n\n    this.setState(\n      prevState => ({selectedChoice: clickedChoice}),\n      () => Streamlit.setComponentValue(this.state.selectedChoice)\n    )\n  }\n\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RtOptionMenu)\n",
+        "// @ts-nocheck\nimport {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport { Icon } from \"./Icon\";\n\ninterface State {\n  selectedChoice: string\n}\n\ninterface ComponentOptions {\n  orientation?: string;\n  default_index?: number;\n  icons?: string[];\n  links?: string[];\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nclass RtOptionMenu extends StreamlitComponentBase<State> {\n  constructor(props: any) {\n    super(props);\n    const choices: string[] = this.props.args[\"choices\"];\n\n    const options: ComponentOptions= this.props.args[\"options\"] || {};\n    if (options.default_index !== undefined) {\n      this.state = { selectedChoice: choices[options.default_index] };\n      Streamlit.setComponentValue(this.state.selectedChoice)\n    }\n    else {\n      this.state = { selectedChoice: \"\"};\n      Streamlit.setComponentValue(this.state.selectedChoice)\n    }\n\n  }\n\n  public render = (): ReactNode => {\n    // Arguments that are passed to the plugin in Python are accessible\n    // via `this.props.args`. Here, we access the \"name\" arg.\n    const choices: string[] = this.props.args[\"choices\"];\n    const options: ComponentOptions = this.props.args[\"options\"] || {};\n\n    const selectedChoice = this.state.selectedChoice;\n\n    if (options.orientation === 'horizontal') {\n      const containerStyle = {\n        display: 'flex',\n        flexDirection: 'row' as 'row',\n        alignItems: 'center',\n        justifyContent: 'space-evenly',\n        columnGap: '0.5em',\n        backgroundColor: 'rgb(240,240,240)',\n        padding: '0.5em',\n        borderRadius: '10px'\n      }\n      const elementStyle = {\n        padding: '0.25em',\n        flex: 1,\n        background: 'rgb(237,240,244)',\n        cursor: 'pointer',\n        textAlign: 'center',\n        userSelect: 'none' as 'none',\n      }\n      const selectedElementStyle = {\n        ...elementStyle,\n        background: 'rgba(107, 101, 255)',\n        borderRadius: '10px',\n        color: 'white',\n      }\n      return (\n        <div style={containerStyle}>\n          {choices.map((choice, index) => {\n            return <div key={index} style={selectedChoice === choice ? selectedElementStyle : elementStyle} onClick={() => this.handleChoiceClick(choice)}>{choice}</div>\n          })}\n        </div>\n      )\n    }\n    // vertical style\n    else{\n      const containerStyle = {\n        display: 'flex',\n        flexDirection: 'column' as 'column',\n        justifyContent: 'space-evenly',\n        alignItems: 'flex-start',\n      }\n      const elementStyle = {\n        display: 'flex',\n        flexDirection: 'row' as 'row',\n        alignItems: 'flex-start',\n        marginTop: '1em',\n        width: '100%',\n        padding: '0.5em',\n        userSelect: 'none' as 'none',\n        cursor: 'pointer',\n      }\n      const selectedElementStyle = {\n        ...elementStyle,\n        background: 'rgba(107, 101, 255, 0.1)',\n        fontWeight: 500\n      }\n      const leftIconStyle = {\n        marginLeft: '0.5em',\n        marginRight: '2em',\n      }\n      const rightIconStyle = {\n        marginLeft: 'auto'\n      }\n      const textStyle = {\n        fontSize: '15px',\n      }\n      const icons = options.icons || [];\n      const links = options.links || [];\n      return (\n        <div style={containerStyle}>\n          {choices.map((choice, index) => {\n            let leftIcon, rightIcon;\n            let link = links[index];\n\n            if (Array.isArray(icons[index])){\n              leftIcon = icons[index][0];\n              rightIcon = icons[index][1];\n            }\n            else {\n              leftIcon = icons[index];\n              rightIcon = undefined;\n            }\n\n            if (selectedChoice === choice){\n              return <div onClick={() => this.handleChoiceClick(choice)} style={selectedElementStyle}><Icon iconName={leftIcon} size={25} style={leftIconStyle}/><span style={textStyle}>{choice}</span><Icon iconName={rightIcon} size={25} style={rightIconStyle}/></div>\n            }\n            else{\n              if (!(link)){\n                return <div onClick={() => this.handleChoiceClick(choice)} style={elementStyle}><Icon iconName={leftIcon} size={25} style={leftIconStyle}/><span style={textStyle}>{choice}</span><Icon iconName={rightIcon} size={25} style={rightIconStyle}/></div>\n              }\n              else{\n                return <div onClick={() => this.handleLinkClick(link)} style={elementStyle}><Icon iconName={leftIcon} size={25} style={leftIconStyle}/><span style={textStyle}>{choice}</span><Icon iconName={rightIcon} size={25} style={rightIconStyle}/></div>\n              }\n            }\n          })}\n        </div>\n      )\n    }\n  }\n\n  private handleLinkClick = (link: string): void => {\n    window.open(link, '_blank');\n  }\n\n  private handleChoiceClick = (clickedChoice: string): void => {\n    this.setState({ selectedChoice: clickedChoice })\n\n    this.setState(\n      prevState => ({selectedChoice: clickedChoice}),\n      () => Streamlit.setComponentValue(this.state.selectedChoice)\n    )\n  }\n\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RtOptionMenu)\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport RtOptionMenu from \"./RtOptionMenu\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <RtOptionMenu />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js`

 * *Files identical despite different names*

### Comparing `rt-option-menu-0.1.5/rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js.map` & `rt-option-menu-0.1.6/rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js.map`

 * *Files identical despite different names*

### Comparing `rt-option-menu-0.1.5/rt_option_menu.egg-info/SOURCES.txt` & `rt-option-menu-0.1.6/rt_option_menu.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 rt_option_menu.egg-info/SOURCES.txt
 rt_option_menu.egg-info/dependency_links.txt
 rt_option_menu.egg-info/requires.txt
 rt_option_menu.egg-info/top_level.txt
 rt_option_menu/frontend/build/asset-manifest.json
 rt_option_menu/frontend/build/bootstrap.min.css
 rt_option_menu/frontend/build/index.html
-rt_option_menu/frontend/build/precache-manifest.a578b4c5e6f2a1d58f4fedbde90b383a.js
+rt_option_menu/frontend/build/precache-manifest.71f79d5ea2999be28b3897d680cde1c7.js
 rt_option_menu/frontend/build/service-worker.js
 rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js
 rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.LICENSE.txt
 rt_option_menu/frontend/build/static/js/2.6ff9f471.chunk.js.map
-rt_option_menu/frontend/build/static/js/main.1e62fb47.chunk.js
-rt_option_menu/frontend/build/static/js/main.1e62fb47.chunk.js.map
+rt_option_menu/frontend/build/static/js/main.ec56508e.chunk.js
+rt_option_menu/frontend/build/static/js/main.ec56508e.chunk.js.map
 rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js
 rt_option_menu/frontend/build/static/js/runtime-main.44d30fc2.js.map
```

### Comparing `rt-option-menu-0.1.5/setup.py` & `rt-option-menu-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="rt-option-menu",
-    version="0.1.5",
+    version="0.1.6",
     author="Jared Foster",
     author_email="jfoster@cafemedia.com",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

