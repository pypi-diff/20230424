# Comparing `tmp/ghhops_server-1.5.4.tar.gz` & `tmp/ghhops_server-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghhops_server-1.5.4.tar", last modified: Wed Jan  4 19:10:02 2023, max compression
+gzip compressed data, was "ghhops_server-1.5.5.tar", last modified: Mon Apr 24 09:28:54 2023, max compression
```

## Comparing `ghhops_server-1.5.4.tar` & `ghhops_server-1.5.5.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     2249 2023-01-04 19:02:44.388750 ghhops_server-1.5.4/ghhops_server/__init__.py
--rw-r--r--   0        0        0    12664 2023-01-04 16:44:50.914248 ghhops_server-1.5.4/ghhops_server/base.py
--rw-r--r--   0        0        0     1499 2022-05-16 02:54:39.687606 ghhops_server-1.5.4/ghhops_server/component.py
--rw-r--r--   0        0        0      135 2022-05-16 02:54:39.687606 ghhops_server-1.5.4/ghhops_server/logger.py
--rw-r--r--   0        0        0      177 2022-05-16 02:54:39.688506 ghhops_server-1.5.4/ghhops_server/middlewares/__init__.py
--rw-r--r--   0        0        0     2736 2023-01-04 16:38:23.585472 ghhops_server-1.5.4/ghhops_server/middlewares/hopsdefault.py
--rw-r--r--   0        0        0     1606 2023-01-04 16:38:23.585472 ghhops_server-1.5.4/ghhops_server/middlewares/hopsflask.py
--rw-r--r--   0        0        0    10787 2023-01-04 19:07:37.088922 ghhops_server-1.5.4/ghhops_server/params.py
--rw-r--r--   0        0        0      491 2022-05-16 02:54:39.689507 ghhops_server-1.5.4/pyproject.toml
--rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 ghhops_server-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     2187 2023-04-24 09:28:03.841744 ghhops_server-1.5.5/ghhops_server/__init__.py
+-rw-r--r--   0        0        0    12321 2023-02-01 22:51:17.090917 ghhops_server-1.5.5/ghhops_server/base.py
+-rw-r--r--   0        0        0     1443 2022-03-26 16:34:49.692776 ghhops_server-1.5.5/ghhops_server/component.py
+-rw-r--r--   0        0        0      131 2021-09-01 23:43:23.254664 ghhops_server-1.5.5/ghhops_server/logger.py
+-rw-r--r--   0        0        0      173 2021-03-13 02:05:04.573177 ghhops_server-1.5.5/ghhops_server/middlewares/__init__.py
+-rw-r--r--   0        0        0     2659 2022-08-25 23:39:27.476529 ghhops_server-1.5.5/ghhops_server/middlewares/hopsdefault.py
+-rw-r--r--   0        0        0     1555 2022-08-25 23:39:27.477058 ghhops_server-1.5.5/ghhops_server/middlewares/hopsflask.py
+-rw-r--r--   0        0        0    10426 2023-04-24 09:27:34.479088 ghhops_server-1.5.5/ghhops_server/params.py
+-rw-r--r--   0        0        0      477 2021-03-13 02:09:44.338269 ghhops_server-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 ghhops_server-1.5.5/setup.py
+-rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 ghhops_server-1.5.5/PKG-INFO
```

### Comparing `ghhops_server-1.5.4/ghhops_server/__init__.py` & `ghhops_server-1.5.5/ghhops_server/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-"""Grasshopper Hops Server"""
-import importlib
-import ghhops_server.base as base
-import ghhops_server.middlewares as hmw
-from ghhops_server import params
-from ghhops_server.logger import logging, hlogger
-
-# import all supported servers for easy typehinting
-from ghhops_server.middlewares import *  # noqa
-
-# import all supported parameter types for easy access
-from ghhops_server.params import *  # noqa
-
-
-# main module version for pypi build
-__version__ = "1.5.4"
-
-
-class Hops(base.HopsBase):
-    """Hops Middleware"""
-
-    def __new__(cls, app=None, debug=False, *args, **kwargs) -> base.HopsBase:
-        # set logger level
-        hlogger.setLevel(logging.DEBUG if debug else logging.INFO)
-
-        # determine the correct middleware base on the source app being wrapped
-        # when running standalone with no source apps
-        if app is None:
-            hlogger.debug("Using Hops default http server")
-            params._init_rhino3dm()
-            return hmw.HopsDefault()
-
-        # if wrapping another app
-        app_type = repr(app)
-        # if app is Flask
-        if app_type.startswith("<Flask"):
-            hlogger.debug("Using Hops Flask middleware")
-            params._init_rhino3dm()
-            return hmw.HopsFlask(app, *args, **kwargs)
-
-        # if wrapping rhinoinside
-        # paractically this is not necessary. it is implemented this way
-        # mostly to provide a level of consistency on how Hops is used
-        elif app_type.startswith("<module 'rhinoinside'"):
-            # detemine if running with rhino.inside.cpython
-            # and init the param module accordingly
-            if not Hops.is_inside():
-                raise Exception("rhinoinside is not loaded yet")
-            hlogger.debug("Using Hops default http server with rhinoinside")
-            params._init_rhinoinside()
-            return hmw.HopsDefault(*args, **kwargs)
-
-        raise Exception("Unsupported app")
-
-    @classmethod
-    def is_inside(cls):
-        try:
-            ri = importlib.import_module("rhinoinside")
-            ri_core = getattr(ri, "__rhino_core", None)
-            return ri_core is not None
-        except Exception:
-            return False
+"""Grasshopper Hops Server"""
+import importlib
+import ghhops_server.base as base
+import ghhops_server.middlewares as hmw
+from ghhops_server import params
+from ghhops_server.logger import logging, hlogger
+
+# import all supported servers for easy typehinting
+from ghhops_server.middlewares import *  # noqa
+
+# import all supported parameter types for easy access
+from ghhops_server.params import *  # noqa
+
+
+# main module version for pypi build
+__version__ = "1.5.5"
+
+
+class Hops(base.HopsBase):
+    """Hops Middleware"""
+
+    def __new__(cls, app=None, debug=False, *args, **kwargs) -> base.HopsBase:
+        # set logger level
+        hlogger.setLevel(logging.DEBUG if debug else logging.INFO)
+
+        # determine the correct middleware base on the source app being wrapped
+        # when running standalone with no source apps
+        if app is None:
+            hlogger.debug("Using Hops default http server")
+            params._init_rhino3dm()
+            return hmw.HopsDefault()
+
+        # if wrapping another app
+        app_type = repr(app)
+        # if app is Flask
+        if app_type.startswith("<Flask"):
+            hlogger.debug("Using Hops Flask middleware")
+            params._init_rhino3dm()
+            return hmw.HopsFlask(app, *args, **kwargs)
+
+        # if wrapping rhinoinside
+        # paractically this is not necessary. it is implemented this way
+        # mostly to provide a level of consistency on how Hops is used
+        elif app_type.startswith("<module 'rhinoinside'"):
+            # detemine if running with rhino.inside.cpython
+            # and init the param module accordingly
+            if not Hops.is_inside():
+                raise Exception("rhinoinside is not loaded yet")
+            hlogger.debug("Using Hops default http server with rhinoinside")
+            params._init_rhinoinside()
+            return hmw.HopsDefault(*args, **kwargs)
+
+        raise Exception("Unsupported app")
+
+    @classmethod
+    def is_inside(cls):
+        try:
+            ri = importlib.import_module("rhinoinside")
+            ri_core = getattr(ri, "__rhino_core", None)
+            return ri_core is not None
+        except Exception:
+            return False
```

### Comparing `ghhops_server-1.5.4/ghhops_server/base.py` & `ghhops_server-1.5.5/ghhops_server/base.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,343 +1,343 @@
-"""Base types for Hops middleware"""
-import sys
-import traceback
-import os
-import os.path as op
-import inspect
-import json
-import base64
-from typing import Tuple
-
-from ghhops_server.logger import hlogger
-from ghhops_server.component import HopsComponent
-
-
-DEFAULT_CATEGORY = "Hops"
-DEFAULT_SUBCATEGORY = "Hops Python"
-
-
-class HopsBase:
-    """Base class for all Hops middleware implementations"""
-
-    ROOT_ROUTE = "/"
-    SOLVE_ROUTE = "/solve"
-
-    BUILTIN_ROUTES = [ROOT_ROUTE, SOLVE_ROUTE]
-
-    ERROR_PAGE_405 = """<!doctype html>
-<html lang=en>
-<title>405 Method Not Allowed</title>
-<h1>Method Not Allowed</h1>
-<p>The method is not allowed for the requested URL.</p>"""
-
-    def __init__(self, app):
-        self.app = app
-        # components dict store each components two times under
-        # two keys get uri and solve uri, for faster lookups in query and solve
-        # it is assumed that uri and solve uri and both unique to the component
-        self._components: dict[str, HopsComponent] = {}
-
-    def handles(self, request):
-        uri = request.path
-        return uri in HopsBase.BUILTIN_ROUTES or uri in self._components
-
-    def handle_HEAD(self, _):
-        return self._prep_response(200, "Success")
-
-    def handle_GET(self, request):
-        uri = request.path
-
-        # if calling GET /solve, respond 405
-        if self._is_solve_uri(uri):
-            return self._return_method_not_allowed()
-
-        # if component exists, return component data
-        res, results = self.query(uri=uri)
-        if res:
-            response = self._prep_response()
-            response.data = results
-
-        # otherwise return 404
-        else:
-            response = self._prep_response(404, "Unknown URI")
-
-        return response
-
-    def handle_POST(self, request):
-        uri = request.path
-
-        # if POST on component uri, return 405
-        if self._is_comp_uri(uri):
-            return self._return_method_not_allowed()
-
-        # otherwise try to solve with payload
-        data = request.data
-        res, results = self.solve(uri=uri, payload=data)
-        if res:
-            response = self._prep_response()
-            response.data = results.encode(encoding="utf_8")
-
-        # otherwise return 404
-        else:
-            response = self._prep_response(404, "Execution Error")
-            response.data = results.encode(encoding="utf_8")
-
-        return response
-
-    def _is_solve_uri(self, uri):
-        return uri == HopsBase.SOLVE_ROUTE
-
-    def _is_comp_uri(self, uri):
-        return uri in self._components
-
-    def query(self, uri) -> Tuple[bool, str]:
-        """Get information on given uri"""
-        # try to find a component registered for this uri
-        # returns one object {}
-        comp = self._components.get(uri, None)
-        if comp:
-            hlogger.debug("Getting component metadata: %s", comp)
-            return True, self._get_comp_data(comp)
-
-        # try to find a collection of components in this uri
-        # returns list of objects [{},{},...]
-        comps = [c for c in self._components.values() if c.uri.startswith(uri)]
-        if comps:
-            hlogger.debug("Getting a list of all registered components")
-            return True, self._get_comps_data(comps)
-
-        return False, self._return_with_err("Unknown Hops url")
-
-    def solve(self, uri, payload) -> Tuple[bool, str]:
-        """Perform Solve on given uri"""
-        if uri == HopsBase.ROOT_ROUTE:
-            hlogger.debug("Nothing to solve on root")
-            return False, self._return_with_err("Nothing to solve on root")
-
-        # FIXME: remove support for legacy solve behaviour
-        elif uri == HopsBase.SOLVE_ROUTE:
-            data = json.loads(payload)
-            comp_uri = data["pointer"]
-            if not comp_uri.startswith(HopsBase.ROOT_ROUTE):
-                comp_uri = HopsBase.ROOT_ROUTE + comp_uri
-            for comp in self._components.values():
-                if comp_uri == comp.uri:
-                    hlogger.info("Solving using legacy API: %s", comp)
-                    return self._process_solve_request(comp, payload)
-
-        # FIXME: test this new api
-        else:
-            comp = self._components.get(uri, None)
-            if comp:
-                hlogger.info("Solving: %s", comp)
-                return self._process_solve_request(comp, payload)
-        return False, self._return_with_err("Unknown Hops component url")
-
-    def _return_with_err(self, err_msg, res_dict=None):
-        err_res = res_dict
-        if err_res:
-            err = err_res.get("errors", None)
-            if isinstance(err, list):
-                err.append(err_msg)
-            else:
-                err_res["errors"] = [err_msg]
-        else:
-            err_res = {"values": [], "errors": [err_msg]}
-
-        return json.dumps(err_res, cls=_HopsEncoder)
-
-    def _return_method_not_allowed(self):
-        response = self._prep_response(405, "Method Not Allowed")
-        response.data = HopsBase.ERROR_PAGE_405.encode(encoding="utf_8")
-        return response
-
-    def _get_all_comps_data(self):
-        # return json formatted string of all components metadata
-        return json.dumps(list(self._components.values()), cls=_HopsEncoder)
-
-    def _get_comps_data(self, comps):
-        # return json formatted string of all components metadata
-        return json.dumps(comps, cls=_HopsEncoder)
-
-    def _get_comp_data(self, comp):
-        # return json formatted string of component metadata
-        return json.dumps(comp, cls=_HopsEncoder)
-
-    def _prepare_icon(self, resource_path, icon_file_path):
-        # return icon data in base64 for embedding in http results
-        # determine possible icon paths
-        possible_icon_paths = []
-        if op.isabs(icon_file_path):
-            possible_icon_paths.append(icon_file_path)
-        else:
-            process_icon_file_path = op.join(os.getcwd(), icon_file_path)
-            possible_icon_paths.append(process_icon_file_path)
-            if resource_path:
-                sidecar_icon_file_path = op.join(resource_path, icon_file_path)
-                possible_icon_paths.append(sidecar_icon_file_path)
-
-        for icon_path in possible_icon_paths:
-            if op.exists(icon_path):
-                with open(icon_path, "rb") as image_file:
-                    base64_bytes = base64.b64encode(image_file.read())
-                    return base64_bytes.decode("ascii")
-
-        hlogger.error(
-            "Can not find icon file at %s",
-            ", ".join(possible_icon_paths)
-        )
-
-    def _process_solve_request(self, comp, payload) -> Tuple[bool, str]:
-        # parse payload for inputs
-        res, inputs = self._prepare_inputs(comp, payload)
-        if not res:
-            hlogger.debug("Bad inputs: %s", inputs)
-            return res, self._return_with_err("Bad inputs")
-
-        # run
-        try:
-            solve_returned = self._solve(comp, inputs)
-            hlogger.debug("Return data: %s", solve_returned)
-            res, outputs = self._prepare_outputs(comp, solve_returned)
-            return (
-                res,
-                outputs if res else self._return_with_err("Bad outputs"),
-            )
-        except Exception as solve_ex:
-            # try to grab traceback data and create err msg
-            _, _, exc_traceback = sys.exc_info()
-            try:
-                fmt_tb = traceback.format_tb(exc_traceback)
-                # FIXME: can we safely assume we are only 2 levels in stack?
-                ex_msg = "\n".join(fmt_tb[2:])
-                ex_msg = str(solve_ex) + f"\n{ex_msg}"
-            except Exception:
-                # otherwise use exception str as msg
-                ex_msg = str(solve_ex)
-
-            hlogger.debug("Exception occured in handler: %s", ex_msg)
-            return False, self._return_with_err(
-                "Exception occured in handler:\n%s" % ex_msg
-            )
-
-    def _prepare_inputs(self, comp, payload) -> Tuple[bool, list]:
-        # parse input payload
-        data = json.loads(payload)
-
-        # grab input param data and value items
-        # FIXME: this works on a single branch only? ["0"][0]
-        param_values = {}
-        for item in data["values"]:
-            param_values[item["ParamName"]] = item
-
-        inputs = []
-        for in_param in comp.inputs:
-            if in_param.name not in param_values and not in_param.optional:
-                return (
-                    False,
-                    f"Missing value for required input {in_param.name}",
-                )
-            in_param_data = param_values[in_param.name]
-            value = in_param.from_input(in_param_data)
-            inputs.append(value)
-
-        if len(comp.inputs) != len(param_values):
-            return (
-                False,
-                "Input count does not match number of inputs for component",
-            )
-
-        return True, inputs
-
-    def _solve(self, comp, inputs):
-        return comp.handler(*inputs)
-
-    def _prepare_outputs(self, comp, returns) -> Tuple[bool, str]:
-        outputs = []
-        if not isinstance(returns, tuple):
-            returns = (returns,)
-        for out_param, out_result in zip(comp.outputs, returns):
-            output_data = out_param.from_result(out_result)
-            outputs.append(output_data)
-        payload = {"values": outputs}
-        hlogger.debug("Return payload: %s", payload)
-        return True, json.dumps(payload, cls=_HopsEncoder)
-
-    def component(
-        self,
-        rule=None,
-        name=None,
-        nickname=None,
-        description=None,
-        category=None,
-        subcategory=None,
-        icon=None,
-        inputs=None,
-        outputs=None,
-    ):
-        """Decorator for Hops middleware"""
-
-        def __func_wrapper__(comp_func):
-            # determine path of the caller file
-            # this is used for resource resolution
-            frame = inspect.stack()[1]
-            module = inspect.getmodule(frame[0])
-            resource_path = None
-            if module and module.__file__:
-                resource_path = op.dirname(module.__file__)
-
-            # register python func as Hops component
-            if inputs:
-                # inspect default parameters in function signature
-                f_sig = inspect.signature(comp_func)
-                f_params = f_sig.parameters.values()
-                if len(inputs) != len(f_params):
-                    raise Exception(
-                        "Number of function parameters is "
-                        "different from defined Hops inputs"
-                    )
-                # apply function param default values in order
-                # to defined Hops inputs. this will override any
-                # previously defined default values
-                for hinput, fparam in zip(inputs, f_params):
-                    if fparam.default != inspect.Parameter.empty:
-                        hinput.default = fparam.default
-
-            # determine name, and uri
-            comp_name = name or comp_func.__qualname__
-            uri = rule or f"/{comp_name}"
-            # grab icon data
-            icon_data = None
-            if icon:
-                icon_data = self._prepare_icon(resource_path, icon)
-            # create component instance
-            comp = HopsComponent(
-                uri=uri,
-                name=comp_name,
-                nickname=nickname,
-                desc=description or comp_func.__doc__,
-                cat=category or DEFAULT_CATEGORY,
-                subcat=subcategory or DEFAULT_SUBCATEGORY,
-                icon=icon_data,
-                inputs=inputs or [],
-                outputs=outputs or [],
-                handler=comp_func,
-            )
-            hlogger.debug("Component registered: %s", comp)
-            # register by uri and solve uri, for fast lookup on query and solve
-            self._components[uri] = comp
-            self._components[comp.solve_uri] = comp
-            return comp_func
-
-        return __func_wrapper__
-
-
-class _HopsEncoder(json.JSONEncoder):
-    """Custom json encoder to properly encode RhinoCommon and Hops types"""
-
-    def default(self, o):
-        if hasattr(o, "Encode"):
-            return o.Encode()
-        elif hasattr(o, "encode"):
-            return o.encode()
-        return json.JSONEncoder.default(self, o)
+"""Base types for Hops middleware"""
+import sys
+import traceback
+import os
+import os.path as op
+import inspect
+import json
+import base64
+from typing import Tuple
+
+from ghhops_server.logger import hlogger
+from ghhops_server.component import HopsComponent
+
+
+DEFAULT_CATEGORY = "Hops"
+DEFAULT_SUBCATEGORY = "Hops Python"
+
+
+class HopsBase:
+    """Base class for all Hops middleware implementations"""
+
+    ROOT_ROUTE = "/"
+    SOLVE_ROUTE = "/solve"
+
+    BUILTIN_ROUTES = [ROOT_ROUTE, SOLVE_ROUTE]
+
+    ERROR_PAGE_405 = """<!doctype html>
+<html lang=en>
+<title>405 Method Not Allowed</title>
+<h1>Method Not Allowed</h1>
+<p>The method is not allowed for the requested URL.</p>"""
+
+    def __init__(self, app):
+        self.app = app
+        # components dict store each components two times under
+        # two keys get uri and solve uri, for faster lookups in query and solve
+        # it is assumed that uri and solve uri and both unique to the component
+        self._components: dict[str, HopsComponent] = {}
+
+    def handles(self, request):
+        uri = request.path
+        return uri in HopsBase.BUILTIN_ROUTES or uri in self._components
+
+    def handle_HEAD(self, _):
+        return self._prep_response(200, "Success")
+
+    def handle_GET(self, request):
+        uri = request.path
+
+        # if calling GET /solve, respond 405
+        if self._is_solve_uri(uri):
+            return self._return_method_not_allowed()
+
+        # if component exists, return component data
+        res, results = self.query(uri=uri)
+        if res:
+            response = self._prep_response()
+            response.data = results
+
+        # otherwise return 404
+        else:
+            response = self._prep_response(404, "Unknown URI")
+
+        return response
+
+    def handle_POST(self, request):
+        uri = request.path
+
+        # if POST on component uri, return 405
+        if self._is_comp_uri(uri):
+            return self._return_method_not_allowed()
+
+        # otherwise try to solve with payload
+        data = request.data
+        res, results = self.solve(uri=uri, payload=data)
+        if res:
+            response = self._prep_response()
+            response.data = results.encode(encoding="utf_8")
+
+        # otherwise return 404
+        else:
+            response = self._prep_response(404, "Execution Error")
+            response.data = results.encode(encoding="utf_8")
+
+        return response
+
+    def _is_solve_uri(self, uri):
+        return uri == HopsBase.SOLVE_ROUTE
+
+    def _is_comp_uri(self, uri):
+        return uri in self._components
+
+    def query(self, uri) -> Tuple[bool, str]:
+        """Get information on given uri"""
+        # try to find a component registered for this uri
+        # returns one object {}
+        comp = self._components.get(uri, None)
+        if comp:
+            hlogger.debug("Getting component metadata: %s", comp)
+            return True, self._get_comp_data(comp)
+
+        # try to find a collection of components in this uri
+        # returns list of objects [{},{},...]
+        comps = [c for c in self._components.values() if c.uri.startswith(uri)]
+        if comps:
+            hlogger.debug("Getting a list of all registered components")
+            return True, self._get_comps_data(comps)
+
+        return False, self._return_with_err("Unknown Hops url")
+
+    def solve(self, uri, payload) -> Tuple[bool, str]:
+        """Perform Solve on given uri"""
+        if uri == HopsBase.ROOT_ROUTE:
+            hlogger.debug("Nothing to solve on root")
+            return False, self._return_with_err("Nothing to solve on root")
+
+        # FIXME: remove support for legacy solve behaviour
+        elif uri == HopsBase.SOLVE_ROUTE:
+            data = json.loads(payload)
+            comp_uri = data["pointer"]
+            if not comp_uri.startswith(HopsBase.ROOT_ROUTE):
+                comp_uri = HopsBase.ROOT_ROUTE + comp_uri
+            for comp in self._components.values():
+                if comp_uri == comp.uri:
+                    hlogger.info("Solving using legacy API: %s", comp)
+                    return self._process_solve_request(comp, payload)
+
+        # FIXME: test this new api
+        else:
+            comp = self._components.get(uri, None)
+            if comp:
+                hlogger.info("Solving: %s", comp)
+                return self._process_solve_request(comp, payload)
+        return False, self._return_with_err("Unknown Hops component url")
+
+    def _return_with_err(self, err_msg, res_dict=None):
+        err_res = res_dict
+        if err_res:
+            err = err_res.get("errors", None)
+            if isinstance(err, list):
+                err.append(err_msg)
+            else:
+                err_res["errors"] = [err_msg]
+        else:
+            err_res = {"values": [], "errors": [err_msg]}
+
+        return json.dumps(err_res, cls=_HopsEncoder)
+
+    def _return_method_not_allowed(self):
+        response = self._prep_response(405, "Method Not Allowed")
+        response.data = HopsBase.ERROR_PAGE_405.encode(encoding="utf_8")
+        return response
+
+    def _get_all_comps_data(self):
+        # return json formatted string of all components metadata
+        return json.dumps(list(self._components.values()), cls=_HopsEncoder)
+
+    def _get_comps_data(self, comps):
+        # return json formatted string of all components metadata
+        return json.dumps(comps, cls=_HopsEncoder)
+
+    def _get_comp_data(self, comp):
+        # return json formatted string of component metadata
+        return json.dumps(comp, cls=_HopsEncoder)
+
+    def _prepare_icon(self, resource_path, icon_file_path):
+        # return icon data in base64 for embedding in http results
+        # determine possible icon paths
+        possible_icon_paths = []
+        if op.isabs(icon_file_path):
+            possible_icon_paths.append(icon_file_path)
+        else:
+            process_icon_file_path = op.join(os.getcwd(), icon_file_path)
+            possible_icon_paths.append(process_icon_file_path)
+            if resource_path:
+                sidecar_icon_file_path = op.join(resource_path, icon_file_path)
+                possible_icon_paths.append(sidecar_icon_file_path)
+
+        for icon_path in possible_icon_paths:
+            if op.exists(icon_path):
+                with open(icon_path, "rb") as image_file:
+                    base64_bytes = base64.b64encode(image_file.read())
+                    return base64_bytes.decode("ascii")
+
+        hlogger.error(
+            "Can not find icon file at %s",
+            ", ".join(possible_icon_paths)
+        )
+
+    def _process_solve_request(self, comp, payload) -> Tuple[bool, str]:
+        # parse payload for inputs
+        res, inputs = self._prepare_inputs(comp, payload)
+        if not res:
+            hlogger.debug("Bad inputs: %s", inputs)
+            return res, self._return_with_err("Bad inputs")
+
+        # run
+        try:
+            solve_returned = self._solve(comp, inputs)
+            hlogger.debug("Return data: %s", solve_returned)
+            res, outputs = self._prepare_outputs(comp, solve_returned)
+            return (
+                res,
+                outputs if res else self._return_with_err("Bad outputs"),
+            )
+        except Exception as solve_ex:
+            # try to grab traceback data and create err msg
+            _, _, exc_traceback = sys.exc_info()
+            try:
+                fmt_tb = traceback.format_tb(exc_traceback)
+                # FIXME: can we safely assume we are only 2 levels in stack?
+                ex_msg = "\n".join(fmt_tb[2:])
+                ex_msg = str(solve_ex) + f"\n{ex_msg}"
+            except Exception:
+                # otherwise use exception str as msg
+                ex_msg = str(solve_ex)
+
+            hlogger.debug("Exception occured in handler: %s", ex_msg)
+            return False, self._return_with_err(
+                "Exception occured in handler:\n%s" % ex_msg
+            )
+
+    def _prepare_inputs(self, comp, payload) -> Tuple[bool, list]:
+        # parse input payload
+        data = json.loads(payload)
+
+        # grab input param data and value items
+        # FIXME: this works on a single branch only? ["0"][0]
+        param_values = {}
+        for item in data["values"]:
+            param_values[item["ParamName"]] = item
+
+        inputs = []
+        for in_param in comp.inputs:
+            if in_param.name not in param_values and not in_param.optional:
+                return (
+                    False,
+                    f"Missing value for required input {in_param.name}",
+                )
+            in_param_data = param_values[in_param.name]
+            value = in_param.from_input(in_param_data)
+            inputs.append(value)
+
+        if len(comp.inputs) != len(param_values):
+            return (
+                False,
+                "Input count does not match number of inputs for component",
+            )
+
+        return True, inputs
+
+    def _solve(self, comp, inputs):
+        return comp.handler(*inputs)
+
+    def _prepare_outputs(self, comp, returns) -> Tuple[bool, str]:
+        outputs = []
+        if not isinstance(returns, tuple):
+            returns = (returns,)
+        for out_param, out_result in zip(comp.outputs, returns):
+            output_data = out_param.from_result(out_result)
+            outputs.append(output_data)
+        payload = {"values": outputs}
+        hlogger.debug("Return payload: %s", payload)
+        return True, json.dumps(payload, cls=_HopsEncoder)
+
+    def component(
+        self,
+        rule=None,
+        name=None,
+        nickname=None,
+        description=None,
+        category=None,
+        subcategory=None,
+        icon=None,
+        inputs=None,
+        outputs=None,
+    ):
+        """Decorator for Hops middleware"""
+
+        def __func_wrapper__(comp_func):
+            # determine path of the caller file
+            # this is used for resource resolution
+            frame = inspect.stack()[1]
+            module = inspect.getmodule(frame[0])
+            resource_path = None
+            if module and module.__file__:
+                resource_path = op.dirname(module.__file__)
+
+            # register python func as Hops component
+            if inputs:
+                # inspect default parameters in function signature
+                f_sig = inspect.signature(comp_func)
+                f_params = f_sig.parameters.values()
+                if len(inputs) != len(f_params):
+                    raise Exception(
+                        "Number of function parameters is "
+                        "different from defined Hops inputs"
+                    )
+                # apply function param default values in order
+                # to defined Hops inputs. this will override any
+                # previously defined default values
+                for hinput, fparam in zip(inputs, f_params):
+                    if fparam.default != inspect.Parameter.empty:
+                        hinput.default = fparam.default
+
+            # determine name, and uri
+            comp_name = name or comp_func.__qualname__
+            uri = rule or f"/{comp_name}"
+            # grab icon data
+            icon_data = None
+            if icon:
+                icon_data = self._prepare_icon(resource_path, icon)
+            # create component instance
+            comp = HopsComponent(
+                uri=uri,
+                name=comp_name,
+                nickname=nickname,
+                desc=description or comp_func.__doc__,
+                cat=category or DEFAULT_CATEGORY,
+                subcat=subcategory or DEFAULT_SUBCATEGORY,
+                icon=icon_data,
+                inputs=inputs or [],
+                outputs=outputs or [],
+                handler=comp_func,
+            )
+            hlogger.debug("Component registered: %s", comp)
+            # register by uri and solve uri, for fast lookup on query and solve
+            self._components[uri] = comp
+            self._components[comp.solve_uri] = comp
+            return comp_func
+
+        return __func_wrapper__
+
+
+class _HopsEncoder(json.JSONEncoder):
+    """Custom json encoder to properly encode RhinoCommon and Hops types"""
+
+    def default(self, o):
+        if hasattr(o, "Encode"):
+            return o.Encode()
+        elif hasattr(o, "encode"):
+            return o.encode()
+        return json.JSONEncoder.default(self, o)
```

### Comparing `ghhops_server-1.5.4/ghhops_server/middlewares/hopsdefault.py` & `ghhops_server-1.5.5/ghhops_server/middlewares/hopsdefault.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-"""Hops builtin HTTP server"""
-import ghhops_server.base as base
-from ghhops_server.logger import logging, hlogger
-
-from http.server import ThreadingHTTPServer, BaseHTTPRequestHandler
-
-
-class HopsDefault(base.HopsBase):
-    """Hops builtin HTTP server implementation"""
-
-    def __init__(self):
-        super(HopsDefault, self).__init__(None)
-
-    def start(self, address="localhost", port=5000, debug=False):
-        """Start hops builtin http server on given address:port"""
-        # setup logging
-        hlogger.setLevel(logging.DEBUG if debug else logging.INFO)
-        # start ther server
-        _HopsHTTPHandler.hops = self
-        httpd = ThreadingHTTPServer((address, port), _HopsHTTPHandler)
-        hlogger.info("Starting hops python server on %s:%s", address, port)
-        httpd.serve_forever()
-
-
-class _HopsHTTPHandler(BaseHTTPRequestHandler):
-    hops: HopsDefault = None
-
-    def __init__(self, request, client_address, server):
-        super(_HopsHTTPHandler, self).__init__(request, client_address, server)
-
-    def log_message(self, format, *args):
-        """Overriding BaseHTTPRequestHandler.log_message"""
-        hlogger.info(
-            "%s - - [%s] %s"
-            % (
-                self.address_string(),
-                self.log_date_time_string(),
-                format % args,
-            )
-        )
-
-    def _get_comp_uri(self):
-        return self.path.split("?")[0]
-
-    def _prep_response(self, status=200, msg=None):
-        self.send_response(status, msg if msg else "Success")
-        self.send_header("Content-type", "application/json")
-        self.end_headers()
-
-    def do_HEAD(self):
-        self._prep_response()
-
-    def do_GET(self):
-        # grab the path before url params
-        comp_uri = self._get_comp_uri()
-        res, results = self.hops.query(uri=comp_uri)
-        hlogger.debug(f"{res} : {results}")
-        if res:
-            self._prep_response()
-            self.wfile.write(results.encode(encoding="utf_8"))
-        else:
-            self._prep_response(status=404)
-
-    def do_POST(self):
-        # read the message and convert it into a python dictionary
-        comp_uri = self._get_comp_uri()
-        length = int(self.headers.get("Content-Length"))
-        data = self.rfile.read(length)
-        res, results = self.hops.solve(uri=comp_uri, payload=data)
-        hlogger.debug(f"{res} : {results}")
-        if res:
-            self._prep_response()
-            self.wfile.write(results.encode(encoding="utf_8"))
-        else:
-            # TODO: write proper errors
-            self._prep_response(500, "Execution Error")
-            self.wfile.write(results.encode(encoding="utf_8"))
+"""Hops builtin HTTP server"""
+import ghhops_server.base as base
+from ghhops_server.logger import logging, hlogger
+
+from http.server import ThreadingHTTPServer, BaseHTTPRequestHandler
+
+
+class HopsDefault(base.HopsBase):
+    """Hops builtin HTTP server implementation"""
+
+    def __init__(self):
+        super(HopsDefault, self).__init__(None)
+
+    def start(self, address="localhost", port=5000, debug=False):
+        """Start hops builtin http server on given address:port"""
+        # setup logging
+        hlogger.setLevel(logging.DEBUG if debug else logging.INFO)
+        # start ther server
+        _HopsHTTPHandler.hops = self
+        httpd = ThreadingHTTPServer((address, port), _HopsHTTPHandler)
+        hlogger.info("Starting hops python server on %s:%s", address, port)
+        httpd.serve_forever()
+
+
+class _HopsHTTPHandler(BaseHTTPRequestHandler):
+    hops: HopsDefault = None
+
+    def __init__(self, request, client_address, server):
+        super(_HopsHTTPHandler, self).__init__(request, client_address, server)
+
+    def log_message(self, format, *args):
+        """Overriding BaseHTTPRequestHandler.log_message"""
+        hlogger.info(
+            "%s - - [%s] %s"
+            % (
+                self.address_string(),
+                self.log_date_time_string(),
+                format % args,
+            )
+        )
+
+    def _get_comp_uri(self):
+        return self.path.split("?")[0]
+
+    def _prep_response(self, status=200, msg=None):
+        self.send_response(status, msg if msg else "Success")
+        self.send_header("Content-type", "application/json")
+        self.end_headers()
+
+    def do_HEAD(self):
+        self._prep_response()
+
+    def do_GET(self):
+        # grab the path before url params
+        comp_uri = self._get_comp_uri()
+        res, results = self.hops.query(uri=comp_uri)
+        hlogger.debug(f"{res} : {results}")
+        if res:
+            self._prep_response()
+            self.wfile.write(results.encode(encoding="utf_8"))
+        else:
+            self._prep_response(status=404)
+
+    def do_POST(self):
+        # read the message and convert it into a python dictionary
+        comp_uri = self._get_comp_uri()
+        length = int(self.headers.get("Content-Length"))
+        data = self.rfile.read(length)
+        res, results = self.hops.solve(uri=comp_uri, payload=data)
+        hlogger.debug(f"{res} : {results}")
+        if res:
+            self._prep_response()
+            self.wfile.write(results.encode(encoding="utf_8"))
+        else:
+            # TODO: write proper errors
+            self._prep_response(500, "Execution Error")
+            self.wfile.write(results.encode(encoding="utf_8"))
```

### Comparing `ghhops_server-1.5.4/ghhops_server/middlewares/hopsflask.py` & `ghhops_server-1.5.5/ghhops_server/middlewares/hopsflask.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""Hops flask middleware implementation"""
-import ghhops_server.base as base
-
-from werkzeug.wrappers import Request, Response
-
-
-class HopsFlask(base.HopsBase):
-    """Hops Middleware for Flask"""
-
-    def __init__(self, flask_app):
-        # keep a ref to original flask app
-        super(HopsFlask, self).__init__(flask_app)
-        # and and wsgi_app
-        self.wsgi_app = flask_app.wsgi_app
-        # replace wsgi_app with self, this instance will call the bubble up
-        # the unknown/unhandled messages to the original wsgi_app
-        flask_app.wsgi_app = self
-
-    def _prep_response(self, status=200, msg=None):
-        return Response(
-            msg if msg else "Success",
-            mimetype="application/json",
-            status=status,
-        )
-
-    def __call__(self, environ, start_response):
-        request = Request(environ)
-
-        method = request.method
-
-        # if hops app handled this request
-        if self.handles(request):
-            response = None
-
-            if method == "HEAD":
-                response = self.handle_HEAD(request)
-
-            elif method == "GET":
-                response = self.handle_GET(request)
-
-            elif method == "POST":
-                response = self.handle_POST(request)
-
-            if response:
-                return response(environ, start_response)
-
-            # respond with 405 if method is not valid
-            return self._return_method_not_allowed()
-
-        # otherwise ask wapped app to process the call
-        return self.wsgi_app(environ, start_response)
+"""Hops flask middleware implementation"""
+import ghhops_server.base as base
+
+from werkzeug.wrappers import Request, Response
+
+
+class HopsFlask(base.HopsBase):
+    """Hops Middleware for Flask"""
+
+    def __init__(self, flask_app):
+        # keep a ref to original flask app
+        super(HopsFlask, self).__init__(flask_app)
+        # and and wsgi_app
+        self.wsgi_app = flask_app.wsgi_app
+        # replace wsgi_app with self, this instance will call the bubble up
+        # the unknown/unhandled messages to the original wsgi_app
+        flask_app.wsgi_app = self
+
+    def _prep_response(self, status=200, msg=None):
+        return Response(
+            msg if msg else "Success",
+            mimetype="application/json",
+            status=status,
+        )
+
+    def __call__(self, environ, start_response):
+        request = Request(environ)
+
+        method = request.method
+
+        # if hops app handled this request
+        if self.handles(request):
+            response = None
+
+            if method == "HEAD":
+                response = self.handle_HEAD(request)
+
+            elif method == "GET":
+                response = self.handle_GET(request)
+
+            elif method == "POST":
+                response = self.handle_POST(request)
+
+            if response:
+                return response(environ, start_response)
+
+            # respond with 405 if method is not valid
+            return self._return_method_not_allowed()
+
+        # otherwise ask wapped app to process the call
+        return self.wsgi_app(environ, start_response)
```

### Comparing `ghhops_server-1.5.4/ghhops_server/params.py` & `ghhops_server-1.5.5/ghhops_server/params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,415 +1,416 @@
-"""Hops Component Parameter wrappers"""
-import json
-from enum import Enum
-import inspect
-from ghhops_server.base import _HopsEncoder
-from ghhops_server.logger import hlogger
-
-
-__all__ = (
-    "HopsParamAccess",
-    # "HopsArc",
-    "HopsBoolean",
-    # "HopsBox",
-    "HopsBrep",
-    "HopsCircle",
-    # "HopsColour",
-    # "HopsComplex"
-    # "HopsCulture",
-    "HopsCurve",
-    # "HopsField",
-    # "HopsFilePath",
-    # "HopsGeometry",
-    "HopsInteger",
-    # "HopsInterval",
-    # "HopsInterval2D"
-    "HopsLine",
-    # "HopsMatrix",
-    "HopsMesh",
-    # "HopsMeshFace",
-    "HopsNumber",
-    "HopsPlane",
-    "HopsPoint",
-    # "HopsRectangle",
-    "HopsString",
-    # "HopsStructurePath",
-    "HopsSubD",
-    "HopsSurface",
-    # "HopsTime",
-    # "HopsTransform",
-    "HopsVector",
-)
-
-
-RHINO = None
-RHINO_FROMJSON = None
-RHINO_TOJSON = None
-RHINO_GEOM = None
-CONVERT_VALUE = None
-
-
-def _init_rhinoinside():
-    global RHINO
-    global RHINO_FROMJSON
-    global RHINO_TOJSON
-    global RHINO_GEOM
-    global CONVERT_VALUE
-
-    # initialize with Rhino.Inside Cpython ==========
-    import clr
-
-    clr.AddReference("System.Collections")
-    clr.AddReference("Newtonsoft.Json.Rhino")
-    import System
-    import Newtonsoft.Json as NJ
-    from System.Collections.Generic import Dictionary
-
-    def from_json(json_obj):
-        """Convert to RhinoCommon from json"""
-        data_dict = Dictionary[str, str]()
-        for k, v in json_obj.items():
-            data_dict[k] = str(v)
-        return RHINO.Runtime.CommonObject.FromJSON(data_dict)
-
-    def to_json(value):
-        """Convert RhinoCommon object to json"""
-        return NJ.JsonConvert.SerializeObject(value)
-
-    def convert_value(value):
-        # FIXME: more value types probably need to be handled
-        if isinstance(value, bool):
-            return System.Boolean(value)
-        elif isinstance(value, int):
-            return System.Int32(value)
-        elif isinstance(value, float):
-            return System.Double(value)
-        elif isinstance(value, str):
-            return System.String(value)
-        return value
-
-    RHINO_FROMJSON = from_json
-    RHINO_TOJSON = to_json
-
-    import Rhino
-
-    RHINO = Rhino
-    RHINO_GEOM = Rhino.Geometry
-
-    CONVERT_VALUE = convert_value
-
-
-def _init_rhino3dm():
-    global RHINO
-    global RHINO_FROMJSON
-    global RHINO_TOJSON
-    global RHINO_GEOM
-    global CONVERT_VALUE
-
-    import rhino3dm
-
-    def from_json(json_obj):
-        """Convert to rhino3dm from json"""
-        return rhino3dm.CommonObject.Decode(json_obj)
-
-    def to_json(value):
-        """Convert rhino3dm object to json"""
-        return json.dumps(value, cls=_HopsEncoder)
-
-    def convert_value(value):
-        return value
-
-    RHINO_FROMJSON = from_json
-    RHINO_TOJSON = to_json
-
-    RHINO_GEOM = rhino3dm
-
-    CONVERT_VALUE = convert_value
-
-
-class HopsParamAccess(Enum):
-    """GH Item Access"""
-
-    ITEM = 0
-    LIST = 1
-    TREE = 2
-
-
-# TODO:
-# - params can have icons too
-# cast methods
-class _GHParam:
-    coercers = []
-    param_type = None
-    result_type = None
-
-    def __init__(
-        self,
-        name,
-        nickname=None,
-        desc=None,
-        access: HopsParamAccess = HopsParamAccess.ITEM,
-        optional=False,
-        default=None,
-    ):
-        self.name = name
-        self.nickname = nickname
-        self.description = desc
-        self.access: HopsParamAccess = access or HopsParamAccess.ITEM
-        self.optional = optional
-        self.default = default or inspect.Parameter.empty
-
-    def _coerce_value(self, param_type, param_data):
-        # get data as dict
-        data = json.loads(param_data)
-        # parse data
-        if isinstance(self.coercers, dict):
-            coercer = self.coercers.get(param_type, None)
-            if coercer:
-                return coercer(data)
-        elif param_type.startswith("Rhino.Geometry."):
-            return RHINO_FROMJSON(data)
-        return param_data
-
-    def encode(self):
-        """Parameter serializer"""
-        param_def = {
-            "Name": self.name,
-            "Nickname": self.nickname,
-            "Description": self.description,
-            "ParamType": self.param_type,
-            "ResultType": self.result_type,
-            "AtLeast": 1,
-        }
-        if HopsParamAccess.ITEM == self.access:
-            param_def["AtMost"] = 1
-        if HopsParamAccess.LIST == self.access:
-            param_def["AtMost"] = 2147483647  # Max 32 bit integer value
-        if HopsParamAccess.TREE == self.access:
-            param_def["AtLeast"] = -1
-            param_def["AtMost"] = -1
-        if self.default != inspect.Parameter.empty:
-            param_def["Default"] = self.default
-        return param_def
-
-    def from_input(self, input_data):
-        """Extract parameter data from serialized input"""
-        if self.access == HopsParamAccess.TREE:
-            paths = input_data["InnerTree"]
-            tree = {}
-            for k, v in paths.items():
-                data = []
-                for param_value_item in v:
-                    param_type = param_value_item["type"]
-                    param_value = param_value_item["data"]
-                    data.append(self._coerce_value(param_type, param_value))
-                tree[k] = data
-            return tree
-
-        data = []
-        for param_value_item in input_data["InnerTree"]["0"]:
-            param_type = param_value_item["type"]
-            param_value = param_value_item["data"]
-            data.append(self._coerce_value(param_type, param_value))
-        if self.access == HopsParamAccess.ITEM:
-            return data[0]
-        return data
-
-    def from_result(self, value):
-        """Serialize parameter with given value for output"""
-        if self.access == HopsParamAccess.TREE and isinstance(value, dict):
-            tree = {}
-            for key in value.keys():
-                branch_data = [
-                    {
-                        "type": self.result_type,
-                        "data": RHINO_TOJSON(CONVERT_VALUE(v)),
-                    }
-                    for v in value[key]
-                ]
-                tree[key] = branch_data
-            output = {
-                "ParamName": self.name,
-                "InnerTree": tree,
-            }
-            return output
-
-        if not isinstance(value, tuple) and not isinstance(value, list):
-            value = (value,)
-
-        output_list = [
-            {"type": self.result_type, "data": RHINO_TOJSON(CONVERT_VALUE(v))}
-            for v in value
-        ]
-
-        output = {
-            "ParamName": self.name,
-            "InnerTree": {"0": output_list},
-        }
-        return output
-
-
-class HopsBoolean(_GHParam):
-    """Wrapper for GH_Boolean"""
-
-    param_type = "Boolean"
-    result_type = "System.Boolean"
-
-    coercers = {"System.Boolean": lambda b: bool(b)}
-
-
-class HopsBrep(_GHParam):
-    """Wrapper for GH Brep"""
-
-    param_type = "Brep"
-    result_type = "Rhino.Geometry.Brep"
-
-
-class HopsCircle(_GHParam):
-    """Wrapper for GH_Circle"""
-
-    param_type = "Circle"
-    result_type = "Rhino.Geometry.Circle"
-
-    coercers = {
-        "Rhino.Geometry.Circle": lambda d: HopsCircle._make_circle(
-            HopsPlane._make_plane(
-                d["Plane"]["Origin"], d["Plane"]["XAxis"], d["Plane"]["YAxis"]
-            ),
-            d["Radius"],
-        )
-    }
-
-    @staticmethod
-    def _make_circle(p, r):
-        circle = RHINO_GEOM.Circle(r)
-        circle.Plane = p
-        return circle
-
-
-class HopsCurve(_GHParam):
-    """Wrapper for GH Curve"""
-
-    param_type = "Curve"
-    result_type = "Rhino.Geometry.Curve"
-
-
-class HopsInteger(_GHParam):
-    """Wrapper for GH_Integer"""
-
-    param_type = "Integer"
-    result_type = "System.Int32"
-
-    coercers = {"System.Int32": lambda i: int(i)}
-
-
-class HopsLine(_GHParam):
-    """Wrapper for GH_Line"""
-
-    param_type = "Line"
-    result_type = "Rhino.Geometry.Line"
-
-    coercers = {
-        "Rhino.Geometry.Line": lambda l: RHINO_GEOM.Line(
-            HopsLine._make_point(l["From"]), HopsLine._make_point(l["To"])
-        )
-    }
-
-    @staticmethod
-    def _make_point(a):
-        return RHINO_GEOM.Point3d(a["X"], a["Y"], a["Z"])
-
-
-class HopsMesh(_GHParam):
-    """Wrapper for GH Mesh"""
-
-    param_type = "Mesh"
-    result_type = "Rhino.Geometry.Mesh"
-
-
-class HopsNumber(_GHParam):
-    """Wrapper for GH Number"""
-
-    param_type = "Number"
-    result_type = "System.Double"
-
-    coercers = {
-        "System.Double": lambda d: float(d),
-    }
-
-
-class HopsPlane(_GHParam):
-    """Wrapper for GH_Plane"""
-
-    param_type = "Plane"
-    result_type = "Rhino.Geometry.Plane"
-
-    coercers = {
-        "Rhino.Geometry.Plane": lambda p: HopsPlane._make_plane(
-            p["Origin"], p["XAxis"], p["YAxis"]
-        )
-    }
-
-    @staticmethod
-    def _make_plane(o, x, y):
-        return RHINO_GEOM.Plane(
-            RHINO_GEOM.Point3d(o["X"], o["Y"], o["Z"]),
-            RHINO_GEOM.Vector3d(x["X"], x["Y"], x["Z"]),
-            RHINO_GEOM.Vector3d(y["X"], y["Y"], y["Z"]),
-        )
-
-
-class HopsPoint(_GHParam):
-    """Wrapper for GH Point"""
-
-    param_type = "Point"
-    result_type = "Rhino.Geometry.Point3d"
-
-    coercers = {
-        "Rhino.Geometry.Point2d": lambda d: RHINO_GEOM.Point2d(d["X"], d["Y"]),
-        "Rhino.Geometry.Point3d": lambda d: RHINO_GEOM.Point3d(
-            d["X"], d["Y"], d["Z"]
-        ),
-        "Rhino.Geometry.Vector3d": lambda d: RHINO_GEOM.Vector3d(
-            d["X"], d["Y"], d["Z"]
-        ),
-    }
-
-
-class HopsString(_GHParam):
-    """Wrapper for GH_String"""
-
-    param_type = "Text"
-    result_type = "System.String"
-
-    coercers = {"System.String": lambda s: s}
-
-
-class HopsSubD(_GHParam):
-    """Wrapper for GH SubD"""
-
-    param_type = "SubD"
-    result_type = "Rhino.Geometry.SubD"
-
-
-class HopsSurface(_GHParam):
-    """Wrapper for GH Surface"""
-
-    param_type = "Surface"
-    result_type = "Rhino.Geometry.Brep"
-
-
-class HopsVector(_GHParam):
-    """Wrapper for GH Vector"""
-
-    param_type = "Vector"
-    result_type = "Rhino.Geometry.Vector3d"
-
-    coercers = {
-        "Rhino.Geometry.Point2d": lambda d: RHINO_GEOM.Point2d(d["X"], d["Y"]),
-        "Rhino.Geometry.Point3d": lambda d: RHINO_GEOM.Point3d(
-            d["X"], d["Y"], d["Z"]
-        ),
-        "Rhino.Geometry.Vector3d": lambda d: RHINO_GEOM.Vector3d(
-            d["X"], d["Y"], d["Z"]
-        ),
-    }
+"""Hops Component Parameter wrappers"""
+import json
+from enum import Enum
+import inspect
+from ghhops_server.base import _HopsEncoder
+from ghhops_server.logger import hlogger
+from pprint import pprint
+
+__all__ = (
+    "HopsParamAccess",
+    # "HopsArc",
+    "HopsBoolean",
+    # "HopsBox",
+    "HopsBrep",
+    "HopsCircle",
+    # "HopsColour",
+    # "HopsComplex"
+    # "HopsCulture",
+    "HopsCurve",
+    # "HopsField",
+    # "HopsFilePath",
+    # "HopsGeometry",
+    "HopsInteger",
+    # "HopsInterval",
+    # "HopsInterval2D"
+    "HopsLine",
+    # "HopsMatrix",
+    "HopsMesh",
+    # "HopsMeshFace",
+    "HopsNumber",
+    "HopsPlane",
+    "HopsPoint",
+    # "HopsRectangle",
+    "HopsString",
+    # "HopsStructurePath",
+    "HopsSubD",
+    "HopsSurface",
+    # "HopsTime",
+    # "HopsTransform",
+    "HopsVector",
+)
+
+
+RHINO = None
+RHINO_FROMJSON = None
+RHINO_TOJSON = None
+RHINO_GEOM = None
+CONVERT_VALUE = None
+
+
+def _init_rhinoinside():
+    global RHINO
+    global RHINO_FROMJSON
+    global RHINO_TOJSON
+    global RHINO_GEOM
+    global CONVERT_VALUE
+
+    # initialize with Rhino.Inside Cpython ==========
+    import clr
+
+    clr.AddReference("System.Collections")
+    clr.AddReference("Newtonsoft.Json.Rhino")
+    import System
+    import Newtonsoft.Json as NJ
+    from System.Collections.Generic import Dictionary
+
+    def from_json(json_obj):
+        """Convert to RhinoCommon from json"""
+        data_dict = Dictionary[str, str]()
+        for k, v in json_obj.items():
+            data_dict[k] = str(v)
+        return RHINO.Runtime.CommonObject.FromJSON(data_dict)
+
+    def to_json(value):
+        """Convert RhinoCommon object to json"""
+        return NJ.JsonConvert.SerializeObject(value)
+
+    def convert_value(value):
+        # FIXME: more value types probably need to be handled
+        if isinstance(value, bool):
+            return System.Boolean(value)
+        elif isinstance(value, int):
+            return System.Int32(value)
+        elif isinstance(value, float):
+            return System.Double(value)
+        elif isinstance(value, str):
+            return System.String(value)
+        return value
+
+    RHINO_FROMJSON = from_json
+    RHINO_TOJSON = to_json
+
+    import Rhino
+
+    RHINO = Rhino
+    RHINO_GEOM = Rhino.Geometry
+
+    CONVERT_VALUE = convert_value
+
+
+def _init_rhino3dm():
+    global RHINO
+    global RHINO_FROMJSON
+    global RHINO_TOJSON
+    global RHINO_GEOM
+    global CONVERT_VALUE
+
+    import rhino3dm
+
+    def from_json(json_obj):
+        """Convert to rhino3dm from json"""
+        return rhino3dm.CommonObject.Decode(json_obj)
+
+    def to_json(value):
+        """Convert rhino3dm object to json"""
+        return json.dumps(value, cls=_HopsEncoder)
+
+    def convert_value(value):
+        return value
+
+    RHINO_FROMJSON = from_json
+    RHINO_TOJSON = to_json
+
+    RHINO_GEOM = rhino3dm
+
+    CONVERT_VALUE = convert_value
+
+
+class HopsParamAccess(Enum):
+    """GH Item Access"""
+
+    ITEM = 0
+    LIST = 1
+    TREE = 2
+
+
+# TODO:
+# - params can have icons too
+# cast methods
+class _GHParam:
+    coercers = []
+    param_type = None
+    result_type = None
+
+    def __init__(
+        self,
+        name,
+        nickname=None,
+        desc=None,
+        access: HopsParamAccess = HopsParamAccess.ITEM,
+        optional=False,
+        default=None,
+    ):
+        self.name = name
+        self.nickname = nickname
+        self.description = desc
+        self.access: HopsParamAccess = access or HopsParamAccess.ITEM
+        self.optional = optional
+        self.default = default or inspect.Parameter.empty
+
+    def _coerce_value(self, param_type, param_data):
+        # get data as dict
+        data = json.loads(param_data)
+        # parse data
+        if isinstance(self.coercers, dict):
+            coercer = self.coercers.get(param_type, None)
+            if coercer:
+                return coercer(data)
+        elif param_type.startswith("Rhino.Geometry."):
+            return RHINO_FROMJSON(data)
+        return param_data
+
+    def encode(self):
+        """Parameter serializer"""
+        param_def = {
+            "Name": self.name,
+            "Nickname": self.nickname,
+            "Description": self.description,
+            "ParamType": self.param_type,
+            "ResultType": self.result_type,
+            "AtLeast": 1,
+        }
+        if HopsParamAccess.ITEM == self.access:
+            param_def["AtMost"] = 1
+        if HopsParamAccess.LIST == self.access:
+            param_def["AtMost"] = 2147483647  # Max 32 bit integer value
+        if HopsParamAccess.TREE == self.access:
+            param_def["AtLeast"] = -1
+            param_def["AtMost"] = -1
+        if self.default != inspect.Parameter.empty:
+            param_def["Default"] = self.default
+        return param_def
+
+    def from_input(self, input_data):
+        """Extract parameter data from serialized input"""
+        pprint(input_data)
+        if self.access == HopsParamAccess.TREE:
+            paths = input_data["InnerTree"]
+            tree = {}
+            for k, v in paths.items():
+                data = []
+                for param_value_item in v:
+                    param_type = param_value_item["type"]
+                    param_value = param_value_item["data"]
+                    data.append(self._coerce_value(param_type, param_value))
+                tree[k] = data
+            return tree
+
+        data = []
+        for param_value_item in input_data["InnerTree"]["{0}"]:
+            param_type = param_value_item["type"]
+            param_value = param_value_item["data"]
+            data.append(self._coerce_value(param_type, param_value))
+        if self.access == HopsParamAccess.ITEM:
+            return data[0]
+        return data
+
+    def from_result(self, value):
+        """Serialize parameter with given value for output"""
+        if self.access == HopsParamAccess.TREE and isinstance(value, dict):
+            tree = {}
+            for key in value.keys():
+                branch_data = [
+                    {
+                        "type": self.result_type,
+                        "data": RHINO_TOJSON(CONVERT_VALUE(v)),
+                    }
+                    for v in value[key]
+                ]
+                tree[key] = branch_data
+            output = {
+                "ParamName": self.name,
+                "InnerTree": tree,
+            }
+            return output
+
+        if not isinstance(value, tuple) and not isinstance(value, list):
+            value = (value,)
+
+        output_list = [
+            {"type": self.result_type, "data": RHINO_TOJSON(CONVERT_VALUE(v))}
+            for v in value
+        ]
+
+        output = {
+            "ParamName": self.name,
+            "InnerTree": {"0": output_list},
+        }
+        return output
+
+
+class HopsBoolean(_GHParam):
+    """Wrapper for GH_Boolean"""
+
+    param_type = "Boolean"
+    result_type = "System.Boolean"
+
+    coercers = {"System.Boolean": lambda b: bool(b)}
+
+
+class HopsBrep(_GHParam):
+    """Wrapper for GH Brep"""
+
+    param_type = "Brep"
+    result_type = "Rhino.Geometry.Brep"
+
+
+class HopsCircle(_GHParam):
+    """Wrapper for GH_Circle"""
+
+    param_type = "Circle"
+    result_type = "Rhino.Geometry.Circle"
+
+    coercers = {
+        "Rhino.Geometry.Circle": lambda d: HopsCircle._make_circle(
+            HopsPlane._make_plane(
+                d["Plane"]["Origin"], d["Plane"]["XAxis"], d["Plane"]["YAxis"]
+            ),
+            d["Radius"],
+        )
+    }
+
+    @staticmethod
+    def _make_circle(p, r):
+        circle = RHINO_GEOM.Circle(r)
+        circle.Plane = p
+        return circle
+
+
+class HopsCurve(_GHParam):
+    """Wrapper for GH Curve"""
+
+    param_type = "Curve"
+    result_type = "Rhino.Geometry.Curve"
+
+
+class HopsInteger(_GHParam):
+    """Wrapper for GH_Integer"""
+
+    param_type = "Integer"
+    result_type = "System.Int32"
+
+    coercers = {"System.Int32": lambda i: int(i)}
+
+
+class HopsLine(_GHParam):
+    """Wrapper for GH_Line"""
+
+    param_type = "Line"
+    result_type = "Rhino.Geometry.Line"
+
+    coercers = {
+        "Rhino.Geometry.Line": lambda l: RHINO_GEOM.Line(
+            HopsLine._make_point(l["From"]), HopsLine._make_point(l["To"])
+        )
+    }
+
+    @staticmethod
+    def _make_point(a):
+        return RHINO_GEOM.Point3d(a["X"], a["Y"], a["Z"])
+
+
+class HopsMesh(_GHParam):
+    """Wrapper for GH Mesh"""
+
+    param_type = "Mesh"
+    result_type = "Rhino.Geometry.Mesh"
+
+
+class HopsNumber(_GHParam):
+    """Wrapper for GH Number"""
+
+    param_type = "Number"
+    result_type = "System.Double"
+
+    coercers = {
+        "System.Double": lambda d: float(d),
+    }
+
+
+class HopsPlane(_GHParam):
+    """Wrapper for GH_Plane"""
+
+    param_type = "Plane"
+    result_type = "Rhino.Geometry.Plane"
+
+    coercers = {
+        "Rhino.Geometry.Plane": lambda p: HopsPlane._make_plane(
+            p["Origin"], p["XAxis"], p["YAxis"]
+        )
+    }
+
+    @staticmethod
+    def _make_plane(o, x, y):
+        return RHINO_GEOM.Plane(
+            RHINO_GEOM.Point3d(o["X"], o["Y"], o["Z"]),
+            RHINO_GEOM.Vector3d(x["X"], x["Y"], x["Z"]),
+            RHINO_GEOM.Vector3d(y["X"], y["Y"], y["Z"]),
+        )
+
+
+class HopsPoint(_GHParam):
+    """Wrapper for GH Point"""
+
+    param_type = "Point"
+    result_type = "Rhino.Geometry.Point3d"
+
+    coercers = {
+        "Rhino.Geometry.Point2d": lambda d: RHINO_GEOM.Point2d(d["X"], d["Y"]),
+        "Rhino.Geometry.Point3d": lambda d: RHINO_GEOM.Point3d(
+            d["X"], d["Y"], d["Z"]
+        ),
+        "Rhino.Geometry.Vector3d": lambda d: RHINO_GEOM.Vector3d(
+            d["X"], d["Y"], d["Z"]
+        ),
+    }
+
+
+class HopsString(_GHParam):
+    """Wrapper for GH_String"""
+
+    param_type = "Text"
+    result_type = "System.String"
+
+    coercers = {"System.String": lambda s: s}
+
+
+class HopsSubD(_GHParam):
+    """Wrapper for GH SubD"""
+
+    param_type = "SubD"
+    result_type = "Rhino.Geometry.SubD"
+
+
+class HopsSurface(_GHParam):
+    """Wrapper for GH Surface"""
+
+    param_type = "Surface"
+    result_type = "Rhino.Geometry.Brep"
+
+
+class HopsVector(_GHParam):
+    """Wrapper for GH Vector"""
+
+    param_type = "Vector"
+    result_type = "Rhino.Geometry.Vector3d"
+
+    coercers = {
+        "Rhino.Geometry.Point2d": lambda d: RHINO_GEOM.Point2d(d["X"], d["Y"]),
+        "Rhino.Geometry.Point3d": lambda d: RHINO_GEOM.Point3d(
+            d["X"], d["Y"], d["Z"]
+        ),
+        "Rhino.Geometry.Vector3d": lambda d: RHINO_GEOM.Vector3d(
+            d["X"], d["Y"], d["Z"]
+        ),
+    }
```

