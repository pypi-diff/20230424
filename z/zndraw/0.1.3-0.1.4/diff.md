# Comparing `tmp/zndraw-0.1.3.tar.gz` & `tmp/zndraw-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zndraw-0.1.3.tar", max compression
+gzip compressed data, was "zndraw-0.1.4.tar", max compression
```

## Comparing `zndraw-0.1.3.tar` & `zndraw-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.3/LICENSE
--rw-r--r--   0        0        0     1734 2023-04-21 13:19:36.154627 zndraw-0.1.3/README.md
--rw-r--r--   0        0        0      797 2023-04-21 13:19:36.154627 zndraw-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      125 2023-04-15 20:56:00.080869 zndraw-0.1.3/zndraw/__init__.py
--rw-r--r--   0        0        0     3475 2023-04-21 13:19:36.154627 zndraw-0.1.3/zndraw/app.py
--rw-r--r--   0        0        0     2613 2023-04-19 19:55:37.727848 zndraw-0.1.3/zndraw/cli.py
--rw-r--r--   0        0        0     2356 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/examples/__init__.py
--rw-r--r--   0        0        0     3491 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/globals.py
--rw-r--r--   0        0        0     1208 2023-04-18 14:25:10.131721 zndraw-0.1.3/zndraw/io.py
--rw-r--r--   0        0        0     9533 2023-04-17 10:14:40.724969 zndraw-0.1.3/zndraw/static/favion-192x192.png
--rw-r--r--   0        0        0     4714 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/static/main.css
--rw-r--r--   0        0        0    24146 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/static/main.js
--rw-r--r--   0        0        0    12956 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/templates/index.html
--rw-r--r--   0        0        0     2626 1970-01-01 00:00:00.000000 zndraw-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2020 2023-04-24 08:50:45.092660 zndraw-0.1.4/README.md
+-rw-r--r--   0        0        0      797 2023-04-24 08:51:03.752461 zndraw-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-04-21 17:52:18.309756 zndraw-0.1.4/zndraw/__init__.py
+-rw-r--r--   0        0        0     3976 2023-04-24 08:50:45.102660 zndraw-0.1.4/zndraw/app.py
+-rw-r--r--   0        0        0     1659 2023-04-23 21:22:34.280010 zndraw-0.1.4/zndraw/cli.py
+-rw-r--r--   0        0        0     2695 2023-04-24 08:50:45.102660 zndraw-0.1.4/zndraw/examples/__init__.py
+-rw-r--r--   0        0        0     4278 2023-04-24 08:50:45.102660 zndraw-0.1.4/zndraw/globals.py
+-rw-r--r--   0        0        0     1208 2023-04-22 20:55:05.579300 zndraw-0.1.4/zndraw/io.py
+-rw-r--r--   0        0        0      880 2023-04-21 17:52:18.319756 zndraw-0.1.4/zndraw/main.py
+-rw-r--r--   0        0        0     9533 2023-04-17 10:14:40.724969 zndraw-0.1.4/zndraw/static/favion-192x192.png
+-rw-r--r--   0        0        0     3521 2023-04-23 21:22:34.290009 zndraw-0.1.4/zndraw/static/main.css
+-rw-r--r--   0        0        0    21070 2023-04-24 08:50:45.112660 zndraw-0.1.4/zndraw/static/main.js
+-rw-r--r--   0        0        0     2893 2023-04-24 08:50:45.112660 zndraw-0.1.4/zndraw/static/modules/draw.js
+-rw-r--r--   0        0        0      854 2023-04-24 06:27:16.592781 zndraw-0.1.4/zndraw/static/modules/keypress.js
+-rw-r--r--   0        0        0    10032 2023-04-24 08:50:45.112660 zndraw-0.1.4/zndraw/static/modules/particles.js
+-rw-r--r--   0        0        0    16455 2023-04-24 08:50:45.112660 zndraw-0.1.4/zndraw/templates/index.html
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 zndraw-0.1.4/PKG-INFO
```

### Comparing `zndraw-0.1.3/LICENSE` & `zndraw-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.3/README.md` & `zndraw-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 
 ```python
 import abc
 from pydantic import BaseModel
 
 class UpdateScene(BaseModel, abc.ABC):
     @abc.abstractmethod
-    def run(self, atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+    def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         pass
 ```
 
 The ``run`` method expects as inputs
 - atom_ids: list[int], the ids of the currently selected atoms
 - atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where selected.
+- kwargs: dict could be additional information from the scene
 
 and as an output:
 - list[ase.Atoms], a list of ase Atoms objects to display.
 
 
 You can define the parameters using `pydantic.Field` which will be displayed in the UI.
 
@@ -42,8 +43,12 @@
     symbol: str = Field("same")
 ```
 
 To add your method click on the `+` on the right side of the window.
 Your should be able to add your method from the working directory via `module.MyUpdateCls` as long
 as it can be imported via `from module import MyUpdateCls`.
 
-![Alt text](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
+![ZnDraw UI](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
+
+![ZnDraw UI2](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_protein.png "ZnDraw UI2")
+
+![ZnDraw UI3](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_draw.png "ZnDraw UI3")
```

### Comparing `zndraw-0.1.3/pyproject.toml` & `zndraw-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zndraw"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zndraw-0.1.3/zndraw/app.py` & `zndraw-0.1.4/zndraw/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,133 @@
-import dataclasses
 import uuid
 
-from flask import Flask, make_response, render_template, request, session
+import networkx as nx
+import numpy as np
+from flask import Flask, render_template, request, session
 
 from zndraw import globals, io
 
 app = Flask(__name__)
 app.secret_key = str(uuid.uuid4())
 
 
 @app.route("/")
 def index():
+    """Render the main ZnDraw page."""
     session["key"] = str(uuid.uuid4())  # TODO use session key e.g. for atoms cache
-    return render_template("index.html", config=dataclasses.asdict(globals.config))
+    return render_template("index.html", config=globals.config.dict())
 
 
-@app.route("/config")
+@app.route("/config", methods=["POST", "GET"])
 def config():
+    """Get the zndraw configuration."""
+    if request.method == "POST":
+        print(f"Updating config: {request.json}")
+        for key, value in request.json.items():
+            setattr(globals.config, key, value)
     return {
-        **dataclasses.asdict(globals.config),
-        "total_frames": len(globals._atoms_cache) - 1,
+        **globals.config.dict(),
+        "total_frames": len(globals.config._atoms_cache) - 1,
     }
 
 
-@app.route("/atoms", methods=["POST"])
-def atoms_step():
+@app.route("/graph", methods=["POST"])
+def get_graph():
     step = request.json
     try:
         atoms = globals.config.get_atoms(step=int(step))
         graph = io.get_graph(atoms)
-        return [{**graph.nodes[idx], "id": idx} for idx in graph.nodes]
-    except (KeyError, IndexError):
-        return []
+        return {
+            "nodes": [{**graph.nodes[idx], "id": idx} for idx in graph.nodes],
+            "edges": list(graph.edges),
+        }
+    except KeyError:
+        return {}
 
 
 @app.route("/positions", methods=["POST"])
 def positions_step():
     params = request.json
     result = []
     try:
         for step in range(params["start"], params["stop"]):
             atoms = globals.config.get_atoms(step=int(step))
             result.append(atoms.get_positions().tolist())
         return result
-    except (KeyError, IndexError):
+    except KeyError:
         return result
 
 
-@app.route("/bonds", methods=["POST"])
-def bonds_step():
-    step = request.json
-    atoms = globals.config.get_atoms(step=int(step))
-    graph = io.get_graph(atoms)
-    return list(graph.edges)
-
-
 @app.route("/select", methods=["POST"])
 def select() -> list[int]:
     """Update the selected atoms."""
     step = request.json["step"]
-    selected_ids = request.json["selected_ids"]
-    return {"selected_ids": selected_ids, "updated": False}
+    method = request.json["method"]
+    try:
+        selected_ids = [int(x) for x in request.json["selected_ids"]]
+    except TypeError:
+        selected_ids = []
+    if method in ["particles", "none"]:
+        return {"selected_ids": selected_ids, "updated": False}
+    elif method == "species":
+        atoms = globals.config.get_atoms(step)
+
+        for id in tuple(selected_ids):
+            selected_symbol = atoms[id].symbol
+            selected_ids += [
+                idx for idx, atom in enumerate(atoms) if atom.symbol == selected_symbol
+            ]
+        return {"selected_ids": list(set(selected_ids)), "updated": True}
+    elif method == "connected":
+        atoms = globals.config.get_atoms(step)
+        graph = io.get_graph(atoms)
+
+        total_ids = []
 
-    # atoms = globals.config.get_atoms(step)
+        for node_id in selected_ids:
+            total_ids += list(nx.node_connected_component(graph, node_id))
 
-    # for id in tuple(selected_ids):
-    #     selected_symbol = atoms[id].symbol
-    #     selected_ids += [
-    #         idx for idx, atom in enumerate(atoms) if atom.symbol == selected_symbol
-    #     ]
+        return {"selected_ids": list(set(total_ids)), "updated": True}
 
-    # return {"selected_ids": list(set(selected_ids)), "updated": True}
+    else:
+        raise ValueError(f"Unknown selection method: {method}")
 
 
 @app.route("/add_update_function", methods=["POST"])
 def add_update_function():
     """Add a function to the config."""
-    globals.config.update_function = request.json
     try:
-        signature = globals.config.get_update_signature()
+        signature = globals.config.add_update_function(request.json)
     except (ImportError, ValueError) as err:
         return {"error": str(err)}
     return signature
 
 
-@app.route("/update_function_values", methods=["POST"])
-def update_function_values():
+@app.route("/set_update_function_parameter", methods=["POST"])
+def set_update_function_parameter():
     """Update the values of the update function."""
-    globals.config.set_update_function_parameters(request.json)
+    globals.config.set_update_function_parameter(request.json)
     return {}
 
 
 @app.route("/select_update_function/<name>")
 def select_update_function(name):
     """Select a function from the config."""
-    globals.config.update_function_name = name
+    if name == "none":
+        name = None
+    globals.config.active_update_function = name
     return {}
 
 
 @app.route("/update", methods=["POST"])
 def update_scene():
     selected_ids = list(sorted(request.json["selected_ids"]))
     step = request.json["step"]
-
-    function = globals.config.get_update_function()
-    atoms = function(
-        [int(x) for x in selected_ids], globals.config.get_atoms(step=int(step))
-    )
-
-    offset = len(globals._atoms_cache)
-
-    for idx, atom in enumerate(atoms):
-        print(f"processing {idx}")
-        globals._atoms_cache[idx + offset] = atom
-
-    # this has to return before the scene is automatically updated
+    points = np.array([[x["x"], x["y"], x["z"]] for x in request.json["points"]])
+    globals.config.apply_update_function(selected_ids, step, points=points)
     return {}
 
 
 @app.route("/load")
 def load():
     """Function to call asynchronously to load atoms in the background."""
     globals.config.load_atoms()
```

### Comparing `zndraw-0.1.3/zndraw/examples/__init__.py` & `zndraw-0.1.4/zndraw/examples/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,72 +3,81 @@
 import ase
 import numpy as np
 from pydantic import BaseModel, Field
 
 
 class UpdateScene(BaseModel, abc.ABC):
     @abc.abstractmethod
-    def run(self, atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+    def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         pass
 
 
 class Explode(UpdateScene):
     steps: int = Field(100, le=1000, ge=1)
-    particles: int = Field(10, le=100, ge=1)
+    particles: int = Field(10, le=20, ge=1)
 
-    def run(self, atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+    def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         particles = []
         for _atom_id in atom_ids:
             for _ in range(self.particles):
                 particles.append(ase.Atoms("Na", positions=[atoms.positions[_atom_id]]))
 
         for _ in range(self.steps):
             struct = atoms.copy()
             for particle in particles:
                 particle.positions += np.random.normal(scale=0.1, size=(1, 3))
                 struct += particle
             yield struct
 
 
 class Delete(UpdateScene):
-    def run(self, atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+    def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         for idx, atom_id in enumerate(sorted(atom_ids)):
             atoms.pop(atom_id - idx)  # we remove the atom and shift the index
         return [atoms]
 
 
 class Move(UpdateScene):
     x: float = Field(0.5, le=5, ge=0)
     y: float = Field(0.5, le=5, ge=0)
     z: float = Field(0.5, le=5, ge=0)
 
-    def run(self, atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+    def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         for atom_id in atom_ids:
             atom = atoms[atom_id]
             atom.position += np.array([self.x, self.y, self.z])
             atoms += atom
         return [atoms]
 
 
 class Duplicate(UpdateScene):
     x: float = Field(0.5, le=5, ge=0)
     y: float = Field(0.5, le=5, ge=0)
     z: float = Field(0.5, le=5, ge=0)
     symbol: str = Field("same")
 
-    def run(self, atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+    def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         for atom_id in atom_ids:
             atom = ase.Atom(atoms[atom_id].symbol, atoms[atom_id].position)
             atom.position += np.array([self.x, self.y, self.z])
             atom.symbol = self.symbol if self.symbol != "same" else atom.symbol
             atoms += atom
         return [atoms]
 
 
 class ChangeType(UpdateScene):
     symbol: str = Field("")
 
-    def run(self, atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+    def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         for atom_id in atom_ids:
             atoms[atom_id].symbol = self.symbol
-        print(atoms)
+        return [atoms]
+
+
+class AddLineParticles(UpdateScene):
+    symbol: str = Field("H")
+
+    def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
+        points = kwargs["points"]
+        for point in points:
+            atoms += ase.Atom(self.symbol, position=point)
         return [atoms]
```

### Comparing `zndraw-0.1.3/zndraw/io.py` & `zndraw-0.1.4/zndraw/io.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.3/zndraw/static/favion-192x192.png` & `zndraw-0.1.4/zndraw/static/favion-192x192.png`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.3/zndraw/static/main.css` & `zndraw-0.1.4/zndraw/static/main.css`

 * *Files 20% similar despite different names*

```diff
@@ -13,57 +13,28 @@
     top: 0;
     left: 0;
     width: 100%;
     height: 100%;
     z-index: -100;
 }
 
-#info {
-    position: absolute;
-    bottom: 10px;
-    text-align: center;
-    width: 100%;
-    z-index: 100;
-    display: block;
-    opacity: 0.5;
-}
-
-#loading {
-    position: absolute;
-    bottom: 50%;
-    left: 50%;
-    z-index: 100;
-    display: block;
-}
-
-#right_btn_group {
-    position: absolute;
-    top: 5px;
-    right: 10px;
-    width: 30px;
-    z-index: 100;
-    display: block;
-    opacity: 0.5;
-}
-
-#add_class {
-    z-index: 2000;
-    display: none;
-
-}
-
 .atom-spinner,
 .atom-spinner * {
     box-sizing: border-box;
 }
 
 .atom-spinner {
     height: var(--spinner-size);
     width: var(--spinner-size);
     overflow: hidden;
+    position: absolute;
+    bottom: 50%;
+    left: 50%;
+    z-index: 100;
+    display: block;
 }
 
 .atom-spinner .spinner-inner {
     position: relative;
     display: block;
     height: 100%;
     width: 100%;
@@ -172,88 +143,41 @@
     height: 100%;
     background-color: black;
     opacity: 0.05;
     z-index: 1;
     text-align: center;
 }
 
-#hamburger-menu {
+#info {
     position: absolute;
-    display: block;
+    bottom: 10px;
+    text-align: center;
     width: 100%;
-    height: 100%;
-}
-
-#menu__toggle {
-    opacity: 0;
-}
-
-#menu__toggle:checked+.menu__btn>span {
-    transform: rotate(45deg);
-}
-
-#menu__toggle:checked+.menu__btn>span::before {
-    top: 0;
-    transform: rotate(0deg);
-}
-
-#menu__toggle:checked+.menu__btn>span::after {
-    top: 0;
-    transform: rotate(90deg);
-}
-
-#menu__toggle:checked~.menu__box {
-    left: 0 !important;
+    z-index: 100;
+    display: block;
+    opacity: 0.5;
 }
 
-.menu__btn {
+#infoBox {
     position: absolute;
-    top: 20px;
-    left: 20px;
-    width: 26px;
-    height: 26px;
-    cursor: pointer;
-    z-index: 1;
-}
-
-.menu__btn>span,
-.menu__btn>span::before,
-.menu__btn>span::after {
+    bottom: 1%;
+    left: 69%;
+    right: 1%;
+    width: 30%;
+    z-index: 100;
     display: block;
-    position: absolute;
-    width: 100%;
-    height: 2px;
-    background-color: #616161;
-    transition-duration: .25s;
-}
-
-.menu__btn>span::before {
-    content: '';
-    top: -8px;
-}
-
-.menu__btn>span::after {
-    content: '';
-    top: 8px;
+    background-color: rgb(235, 235, 235);
+    opacity: 0.8;
 }
 
-.menu__box {
+#helpBox {
+    position: absolute;
+    top: 20%;
     display: block;
-    position: fixed;
-    top: 0;
-    left: -100%;
-    width: 40%;
-    height: 100%;
-    margin: 0;
-    padding: 30px 0;
-    /* padding from the top */
-    list-style: none;
-    background-color: #ECEFF1;
-    opacity: 95%;
-    box-shadow: 2px 2px 6px rgba(0, 0, 0, .4);
-    transition-duration: .25s;
+    left: 10%;
+    right: 10%;
+    width: 80%;
 }
 
-.menu__header {
-    padding: 12px 24px;
-    text-align: center;
+.canvasControl {
+    opacity: 0.95;
 }
```

### Comparing `zndraw-0.1.3/zndraw/static/main.js` & `zndraw-0.1.4/zndraw/static/main.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,316 +1,159 @@
 import * as THREE from 'three';
 import {
     OrbitControls
 } from 'three/addons/controls/OrbitControls.js';
-
-
-THREE.Object3D.prototype.getObjectByUserDataProperty = function(name, value) {
-
-    if (this.userData[name] === value) return this;
-
-    for (var i = 0, l = this.children.length; i < l; i++) {
-
-        var child = this.children[i];
-        var object = child.getObjectByUserDataProperty(name, value);
-
-        if (object !== undefined) {
-
-            return object;
-
-        }
-
-    }
-
-    return undefined;
-
-}
-
+import * as PARTICLES from './modules/particles.js';
+import * as DRAW from './modules/draw.js';
+import {
+    keydown
+} from './modules/keypress.js';
 // THREE.Cache.enabled = true;
 
-/**
- * ThreeJS variables
- */
-
-const scene = new THREE.Scene();
-const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
-const renderer = new THREE.WebGLRenderer({
-    antialias: true,
-    alpha: true
-});
-
-const hemisphereLight = new THREE.HemisphereLight(0xffffff, 0x777777, 0.1);
-const spotLight = new THREE.SpotLight(0xffffff, 1, 0, Math.PI / 2);
-
-const atomsGroup = new THREE.Group();
-
-const bondsGroup = new THREE.Group();
-const bondsGroup_1 = new THREE.Group();
-const bondsGroup_2 = new THREE.Group();
-
-let node1 = new THREE.Vector3();
-let node2 = new THREE.Vector3();
-
-const materials = {
-    "MeshBasicMaterial": new THREE.MeshBasicMaterial({
-        color: "#ffa500"
-    }),
-    "MeshLambertMaterial": new THREE.MeshLambertMaterial({
-        color: "#ffa500"
-    }),
-    "MeshMatcapMaterial": new THREE.MeshMatcapMaterial({
-        color: "#ffa500"
-    }),
-    "MeshPhongMaterial": new THREE.MeshPhongMaterial({
-        color: "#ffa500"
-    }),
-    "MeshPhysicalMaterial": new THREE.MeshPhysicalMaterial({
-        color: "#ffa500"
-    }),
-    "MeshStandardMaterial": new THREE.MeshStandardMaterial({
-        color: "#ffa500"
-    }),
-    "MeshToonMaterial": new THREE.MeshToonMaterial({
-        color: "#ffa500"
-    }),
-
-};
 
 /**
  * Three JS Setup
  */
 
-renderer.setSize(window.innerWidth, window.innerHeight);
-document.body.appendChild(renderer.domElement);
-
-
-spotLight.position.set(0, 0, 100);
-scene.add(spotLight);
-
-scene.add(hemisphereLight);
+/**
+ * ThreeJS variables
+ */
 
 let config = {};
 
 
 // some global variables
 let frames = [];
 let selected_ids = [];
 let animation_frame = 0;
+let displayed_frame = 0;
 let scene_building = false;
 let animation_running = true;
 let data_loading = false;
 let fps = [];
 
-let keydown = {
-    "shift": false,
-    "ctrl": false,
-    "alt": false,
-    "c": false,
-    "l": false
-};
 
 /**
  * DOM variables
  */
 
 const div_info = document.getElementById('info');
-const div_loading = document.getElementById('loading');
+const div_loading = document.getElementById('atom-spinner');
 const div_progressBar = document.getElementById('progressBar');
 const div_bufferBar = document.getElementById('bufferBar');
 const div_greyOut = document.getElementById('greyOut');
 const div_lst_selected_ids = document.getElementById('lst_selected_ids');
 const div_FPS = document.getElementById('FPS');
 const div_n_particles = document.getElementById('n_particles');
 const div_n_bonds = document.getElementById('n_bonds');
-const div_help_container = document.getElementById('help_container');
-const div_python_class_control = document.getElementById('python_class_control');
 
-const o_selectAtoms = document.getElementById('selectAtoms');
 const o_autoRestart = document.getElementById('autoRestart');
 const o_animate = document.getElementById('animate');
 const o_reset_selection = document.getElementById('reset_selection');
-const o_hide_selection = document.getElementById('hide_selection');
 const o_reset = document.getElementById('reset');
 const o_max_fps = document.getElementById('max_fps');
 const o_frames_per_post = document.getElementById('frames_per_post');
-const o_sphere_plus = document.getElementById('sphere_plus');
-const o_sphere_minus = document.getElementById('sphere_minus');
-const o_bond_plus = document.getElementById('bond_plus');
-const o_bond_minus = document.getElementById('bond_minus');
-const o_resolution_plus = document.getElementById('resolution_plus');
-const o_resolution_minus = document.getElementById('resolution_minus');
 const o_materialSelect = document.getElementById('materialSelect');
 const o_wireframe = document.getElementById('wireframe');
 const o_spotLightIntensity = document.getElementById('spotLightIntensity');
 const o_hemisphereLightIntensity = document.getElementById('hemisphereLightIntensity');
-const o_help_btn = document.getElementById('help_btn');
-const o_add_btn = document.getElementById('add_btn');
-const o_newPythonClassBtn = document.getElementById('newPythonClassBtn');
+
+const addModifierModal = new bootstrap.Modal(document.getElementById("addModifierModal"));
+const addSceneModifier = document.getElementById("addSceneModifier");
 
 
 // Helper Functions
 
 async function load_config() {
     config = await (await fetch("config")).json();
     console.log(config)
 }
+await load_config();
+
+// THREE JS Setup
+const scene = new THREE.Scene();
+const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
+const renderer = new THREE.WebGLRenderer({
+    antialias: config["antialias"],
+    alpha: true
+});
+
+const hemisphereLight = new THREE.HemisphereLight(0xffffff, 0x777777, 0.1);
+const spotLight = new THREE.SpotLight(0xffffff, 1, 0, Math.PI / 2);
+
+renderer.setSize(window.innerWidth, window.innerHeight);
+document.body.appendChild(renderer.domElement);
+
+
+spotLight.position.set(0, 0, 100);
+scene.add(spotLight);
+
+scene.add(hemisphereLight);
 
 async function update_materials() {
-    for (const material in materials) {
+    for (const material in PARTICLES.materials) {
         const option = document.createElement("option");
         option.text = material;
         option.value = material;
         o_materialSelect.appendChild(option);
     }
-    o_materialSelect.value = "MeshPhongMaterial";
+    o_materialSelect.value = config["material"];
 }
 
 update_materials();
 
-function halfCylinderGeometry(pointX, pointY) {
-    // Make the geometry (of "direction" length)
-    var direction = new THREE.Vector3().subVectors(pointY, pointX);
-
-    var geometry = new THREE.CylinderGeometry(0.15 * config["bond_size"], 0.15 * config["bond_size"], direction.length() / 2, config["resolution"] * 2);
-    // // shift it so one end rests on the origin
-    geometry.applyMatrix4(new THREE.Matrix4().makeTranslation(0, direction.length() / 4, 0));
-    // // rotate it the right way for lookAt to work
-    geometry.applyMatrix4(new THREE.Matrix4().makeRotationX(THREE.MathUtils.degToRad(90)));
-
-    return geometry;
-
-}
 
-function halfCylinderMesh(pointX, pointY, material) {
-    // // Make a mesh with the geometry
-    var geometry = halfCylinderGeometry(pointX, pointY);
-    var mesh = new THREE.Mesh(geometry, material);
-    // alignBetweenVectors(pointX, pointY, mesh);
-    // // Position it where we want
-    mesh.position.copy(pointX);
-    // // And make it point to where we want
-    mesh.lookAt(pointY);
-
-    return mesh;
-}
 
 // Setup Scene
 
-function addAtom(item) {
-    const geometry = new THREE.SphereGeometry(item["radius"] * config["sphere_size"], config["resolution"] * 4, config["resolution"] * 2);
-
-    const particle = new THREE.Mesh(geometry, materials[o_materialSelect.value].clone());
-    atomsGroup.add(particle);
-    particle.material.color.set(item["color"]);
-    particle.material.wireframe = o_wireframe.checked;
-
-    particle.position.set(...item["position"]);
-    particle.userData["id"] = item["id"];
-    particle.userData["color"] = item["color"];
-    particle.userData["bond_ids"] = [];
-}
-
-function addBond(item) {
-    atomsGroup.children[item[0]].getWorldPosition(node1);
-    atomsGroup.children[item[1]].getWorldPosition(node2);
-
-    const bond_1 = halfCylinderMesh(node1, node2, atomsGroup.children[item[0]].material);
-    const bond_2 = halfCylinderMesh(node2, node1, atomsGroup.children[item[1]].material);
-
-    bond_1.userData["atom_id"] = item[0];
-    bond_2.userData["atom_id"] = item[1];
-
-    atomsGroup.children[item[0]].userData["bond_ids"].push(bond_1.id);
-    atomsGroup.children[item[0]].userData["bond_ids"].push(bond_2.id);
-    atomsGroup.children[item[1]].userData["bond_ids"].push(bond_1.id);
-    atomsGroup.children[item[1]].userData["bond_ids"].push(bond_2.id);
-
-
-    bondsGroup_1.add(bond_1);
-    bondsGroup_2.add(bond_2);
-
-}
-
-function cleanScene() {
-    while (atomsGroup.children.length > 0) {
-        scene.remove(atomsGroup.children.shift());
-    };
-    while (bondsGroup_1.children.length > 0) {
-        scene.remove(bondsGroup_1.children.shift());
-    };
-    while (bondsGroup_2.children.length > 0) {
-        scene.remove(bondsGroup_2.children.shift());
-    };
-}
-
-
-function drawAtoms(atoms, bonds) {
-    cleanScene();
-
-    atoms.forEach(function(item, index) {
-        // console.log("Adding item " + index + " to scene(" + item + ")");
-        addAtom(item);
-    });
-
-    scene.add(atomsGroup);
-    if (config["bond_size"] > 0) {
-
-        bonds.forEach(function(item, index) {
-            // console.log("Adding item " + index + " to scene(" + item + ")");
-            addBond(item);
-
-        });
-
-        bondsGroup.add(bondsGroup_1);
-        bondsGroup.add(bondsGroup_2);
-        scene.add(bondsGroup);
-
-    }
-
-
-}
+let build_scene_cache = {};
 
 async function build_scene(step) {
     if (scene_building) {
         return;
     }
-    const urls = ["atoms", "bonds"];
-    animation_frame = step;
     console.log("Updating scene");
 
     div_loading.style.visibility = 'visible';
     div_greyOut.style.visibility = 'visible';
 
-    // this is faster then doing it one by one
-    const arrayOfResponses = await Promise.all(
-        urls.map((url) =>
-            fetch(url, {
-                "method": "POST",
-                "headers": {
-                    "Content-Type": "application/json"
-                },
-                "body": JSON.stringify(step)
-            })
-            .then((res) => res.json())
-        )
-    );
+    animation_frame = step;
+
+    let arrayOfResponses = [];
+    if (build_scene_cache.hasOwnProperty(step)) {
+        console.log("Using cached scene");
+        arrayOfResponses = build_scene_cache[step];
+    } else {
+        // this is faster then doing it one by one
+
+        arrayOfResponses = await (await fetch("graph", {
+            "method": "POST",
+            "headers": {
+                "Content-Type": "application/json"
+            },
+            "body": JSON.stringify(step)
+        })).json();
+        console.log(arrayOfResponses);
+        build_scene_cache[step] = arrayOfResponses;
+    }
 
+    config = await (await fetch("config")).json();
 
-    drawAtoms(arrayOfResponses[0], arrayOfResponses[1]);
+    PARTICLES.drawAtoms(arrayOfResponses["nodes"], arrayOfResponses["edges"], config, scene);
     selected_ids = [];
     await update_selection();
     scene_building = false;
 
-    div_n_particles.innerHTML = atomsGroup.children.length;
-    div_n_bonds.innerHTML = bondsGroup_1.children.length;
+    div_n_particles.innerHTML = PARTICLES.particleGroup.children.length;
+
+    div_n_bonds.innerHTML = PARTICLES.countBonds();
 
     div_greyOut.style.visibility = 'hidden';
     div_loading.style.visibility = 'hidden';
 }
-await load_config();
 
 build_scene(0);
 
 // interactions
 
 camera.position.z = 50;
 const controls = new OrbitControls(camera, renderer.domElement);
@@ -337,28 +180,30 @@
     pointer.x = (event.clientX / window.innerWidth) * 2 - 1;
     pointer.y = -(event.clientY / window.innerHeight) * 2 + 1;
 
     // update the picking ray with the camera and pointer position
     raycaster.setFromCamera(pointer, camera);
 
     // calculate objects intersecting the picking ray
-    const intersects = raycaster.intersectObjects(atomsGroup.children);
+    const intersects = raycaster.intersectObjects(PARTICLES.particleGroup.children, true);
 
     if (intersects.length == 0) {
         return;
     }
 
     // for (let i = 0; i < intersects.length; i++) {
     let mesh = intersects[0].object;
     if (!keydown["shift"]) {
-        selected_ids = [mesh.userData["id"]];
-        mesh.material.color.set(0xffa500);
+        if (selected_ids.includes(mesh.userData["id"])) {
+            selected_ids = [];
+        } else {
+            selected_ids = [mesh.userData["id"]];
+        }
     } else {
         if (!selected_ids.includes(mesh.userData["id"])) {
-            mesh.material.color.set(0xffa500);
             selected_ids.push(mesh.userData["id"]);
         } else {
             mesh.material.color.set(mesh.userData["color"]);
             selected_ids.splice(selected_ids.indexOf(mesh.userData["id"]), 1);
         }
     }
     // update colors here for better performance
@@ -369,19 +214,26 @@
 /**
  * We update the color of every atom in the scene
  * @param {list[int]} ids, the selected ids
  * @returns 
  */
 
 async function update_color_of_ids(ids) {
-    atomsGroup.children.forEach(function(mesh) {
+    PARTICLES.particleGroup.children.forEach(function(atom_grp) {
+        let mesh = atom_grp.children[0];
         if (ids.includes(mesh.userData["id"])) {
-            mesh.material.color.set(0xffa500);
+            let material = PARTICLES.speciesMaterial(document.getElementById('materialSelect').value, 0xffa500, document.getElementById('wireframe').checked);
+            atom_grp.children.forEach(function(item) {
+                item.material = material;
+            });
         } else {
-            mesh.material.color.set(mesh.userData["color"]);
+            let material = PARTICLES.speciesMaterial(document.getElementById('materialSelect').value, mesh.userData["color"], document.getElementById('wireframe').checked);
+            atom_grp.children.forEach(function(item) {
+                item.material = material;
+            });
         }
     });
     return ids;
 }
 
 async function update_selection() {
     console.log("Updating selection");
@@ -389,15 +241,16 @@
     await fetch("select", {
         "method": "POST",
         "headers": {
             "Content-Type": "application/json"
         },
         "body": JSON.stringify({
             "selected_ids": selected_ids,
-            "step": animation_frame
+            "step": animation_frame,
+            "method": document.getElementById("selection-method").value
         }),
     }).then(response => response.json()).then(function(response_json) {
         if (response_json["updated"]) {
             update_color_of_ids(response_json["selected_ids"]);
             selected_ids = response_json["selected_ids"];
         }
         div_lst_selected_ids.innerHTML = response_json["selected_ids"].join(", ");
@@ -457,134 +310,139 @@
 /**
  * Event listeners
  */
 
 window.addEventListener('pointerdown', onPointerDown, false);
 window.addEventListener('resize', onWindowResize, false);
 
-o_selectAtoms.onclick = function() {
-    if (o_selectAtoms.checked) {
-        console.log("Selecting atoms");
-        window.addEventListener('pointerdown', onPointerDown, false);
-    } else {
+document.getElementById("selection-method").onclick = function() {
+    if (document.getElementById("selection-method").value == "none") {
         console.log("Deselecting atoms");
         window.removeEventListener('pointerdown', onPointerDown, false);
+    } else {
+        console.log("Selecting atoms");
+        window.addEventListener('pointerdown', onPointerDown, false);
     }
+
 }
+
 o_animate.onclick = function() {
     div_info.innerHTML = "Reading file...";
     getAnimationFrames();
 }
 
 
 o_reset_selection.onclick = function() {
     selected_ids = [];
+    update_color_of_ids(selected_ids);
     update_selection();
 }
 
 
-o_hide_selection.onclick = function() {
-    selected_ids.forEach(function(item, index) {
-        let mesh = atomsGroup.getObjectByUserDataProperty("id", item);
-        mesh.visible = false;
-
-        mesh.userData["bond_ids"].forEach(function(item, index) {
-            bondsGroup_1.getObjectById(item).visible = false;
-            bondsGroup_2.getObjectById(item).visible = false;
-        });
-    });
-}
-
 o_reset.onclick = function() {
     load_config();
     animation_frame = 0;
     build_scene(0);
     selected_ids = [];
     update_selection();
 }
 
-o_sphere_plus.onclick = function() {
-    config["sphere_size"] += 0.1;
-    build_scene(animation_frame);
-}
+document.getElementById("sphereRadius").onchange = function() {
+    let radius = parseFloat(document.getElementById("sphereRadius").value);
+    let particleGeometry = PARTICLES.particleGroup.children[0].children[0].geometry;
+    let scale = radius / particleGeometry.boundingSphere.radius;
+    particleGeometry.scale(scale, scale, scale);
+    fetch("config", {
+        "method": "POST",
+        "headers": {
+            "Content-Type": "application/json"
+        },
+        "body": JSON.stringify({
+            "sphere_size": radius
+        }),
+    });
 
-o_sphere_minus.onclick = function() {
-    config["sphere_size"] -= 0.1;
-    build_scene(animation_frame);
-}
+};
 
-o_bond_plus.onclick = function() {
-    config["bond_size"] += 0.1;
-    build_scene(animation_frame);
-}
+document.getElementById("sphereRadius").oninput = function() {
+    let radius = parseFloat(document.getElementById("sphereRadius").value);
+    document.getElementById("sphereRadiusLabel").innerHTML = "Sphere radius: " + radius;
+};
 
-o_bond_minus.onclick = function() {
-    config["bond_size"] -= 0.1;
-    build_scene(animation_frame);
-}
+document.getElementById("bondDiameter").oninput = function() {
+    let radius = parseFloat(document.getElementById("bondDiameter").value);
+    document.getElementById("bondDiameterLabel").innerHTML = "Bond diameter: " + radius;
+};
 
-o_resolution_plus.onclick = function() {
-    config["resolution"] += 1;
+document.getElementById("bondDiameter").onchange = function() {
+    let diameter = parseFloat(document.getElementById("bondDiameter").value);
+    fetch("config", {
+        "method": "POST",
+        "headers": {
+            "Content-Type": "application/json"
+        },
+        "body": JSON.stringify({
+            "bond_size": diameter
+        }),
+    });
+    // currently we can't scale correctly so we reset everything
     build_scene(animation_frame);
-}
+};
 
-o_resolution_minus.onclick = function() {
-    config["resolution"] -= 1;
+document.getElementById("resolution").onchange = function() {
+    let resolution = parseInt(document.getElementById("resolution").value);
+    fetch("config", {
+        "method": "POST",
+        "headers": {
+            "Content-Type": "application/json"
+        },
+        "body": JSON.stringify({
+            "resolution": resolution
+        }),
+    });
     build_scene(animation_frame);
-}
+};
+
+document.getElementById("resolution").oninput = function() {
+    let resolution = parseInt(document.getElementById("resolution").value);
+    document.getElementById("resolutionLabel").innerHTML = "Resolution: " + resolution;
+};
 
 o_materialSelect.onchange = function() {
     build_scene(animation_frame);
 }
 
 o_wireframe.onchange = function() {
     build_scene(animation_frame);
 }
 
 o_spotLightIntensity.oninput = function() {
-    document.getElementById("spotLightIntensity_output").value = o_spotLightIntensity.value;
     spotLight.intensity = o_spotLightIntensity.value;
+    document.getElementById("spotLightIntensityLabel").innerHTML = "Spot light intensity: " + o_spotLightIntensity.value;
 }
 
 o_hemisphereLightIntensity.oninput = function() {
-    document.getElementById("hemisphereLightIntensity_output").value = o_hemisphereLightIntensity.value;
     hemisphereLight.intensity = o_hemisphereLightIntensity.value;
-}
-
-o_help_btn.onmouseover = function() {
-    div_help_container.style.display = "block";
-}
-
-o_help_btn.onmouseout = function() {
-    div_help_container.style.display = "none";
-}
+    document.getElementById("hemisphereLightIntensityLabel").innerHTML = "Hemisphere light intensity: " + o_hemisphereLightIntensity.value;
 
-o_add_btn.onclick = function() {
-    document.getElementById("add_class").style.display = "block";
 }
 
 
 /**
  * Helper function, move later
  * @param {} name 
  * @param {*} checked 
  * @returns 
  */
-function createRadioElement(name, checked, id, properties) {
-    var radioHtml = '<input class="form-check-input" type="radio" name="' + name + '"  id="' + id + '"';
-    if (checked) {
-        radioHtml += ' checked="checked"';
-    }
-    radioHtml += '/>';
+function createRadioElement(id, properties) {
 
     var radioFragment = document.createElement('div');
-    radioFragment.classList.add("form-check");
-    radioFragment.innerHTML = radioHtml;
-
-
+    radioFragment.classList.add("mb-3");
+    radioFragment.classList.add("collapse", "show", "scene-modifier");
+    radioFragment.id = "sceneModifier_" + id;
 
     let function_container = document.createElement('div');
     function_container.classList.add("container-fluid", "bg-light", "rounded", "border", "border-primary");
 
     let function_container_label = document.createElement('h5');
     function_container_label.innerHTML = id;
 
@@ -655,15 +513,15 @@
 
         controller.oninput = function() {
             value.innerHTML = controller.value;
         }
 
         controller.onchange = function() {
             // fetch with post 
-            fetch("update_function_values", {
+            fetch("set_update_function_parameter", {
                 "method": "POST",
                 "headers": {
                     "Content-Type": "application/json"
                 },
                 "body": JSON.stringify({
                     "function_id": id,
                     "property": item["title"],
@@ -674,47 +532,79 @@
     });
     function_container.appendChild(function_container_col);
     radioFragment.appendChild(function_container);
 
     return radioFragment;
 }
 
-o_newPythonClassBtn.onclick = function() {
-    document.getElementById("add_class").style.display = "none";
+addSceneModifier.onchange = function() {
+    console.log(this.value);
+    if (this.value == "add") {
+        addModifierModal.show();
+    } else {
+        fetch("/select_update_function/" + this.value)
+    }
 
+    let domElements = document.getElementsByClassName("scene-modifier");
+
+    [...domElements].forEach(element => {
+        let bs_collapse = new bootstrap.Collapse(element, {
+            toggle: false
+        });
+        if (element.id == "sceneModifier_" + this.value) {
+            bs_collapse.show();
+        } else {
+            bs_collapse.hide();
+        }
+    });
+};
+
+document.getElementById("addSceneModifierImportBtn").onclick = function() {
+    let function_id = document.getElementById("addSceneModifierImport").value;
     fetch("add_update_function", {
         "method": "POST",
         "headers": {
             "Content-Type": "application/json"
         },
-        "body": JSON.stringify(document.getElementById("newPythonClass").value),
+        "body": JSON.stringify(function_id),
     }).then(response => response.json()).then(function(response_json) {
         // if not null alert
         if ("error" in response_json) {
+            // TODO check if method is already loaded
             alert(response_json["error"]);
             stepError(response_json["error"]);
         } else {
+            if (document.getElementById("sceneModifier_" + response_json["title"]) != null) {
+                alert("Function already loaded");
+                stepError("Function already loaded");
+            };
+
+            addModifierModal.hide();
+
             console.log(response_json);
             load_config();
         }
         return response_json;
     }).then(function(response_json) {
         console.log(response_json);
-        div_python_class_control.appendChild(createRadioElement("flexRadioUpdateFunction", true, response_json["title"], response_json["properties"]));
-
-        document.getElementById(response_json["title"]).onclick = function() {
-            console.log("clicked");
-            console.log(document.querySelector('input[name="flexRadioUpdateFunction"]:checked').id);
-            fetch("/select_update_function/" + document.querySelector('input[name="flexRadioUpdateFunction"]:checked').id)
-        };
-
+        let modifier = document.createElement("option");
+        modifier.value = response_json["title"];
+        modifier.innerHTML = response_json["title"];
+        addSceneModifier.appendChild(modifier);
+        addSceneModifier.value = response_json["title"];
+        return response_json;
+    }).then(function(response_json) {
+        let sceneModifierSettings = document.getElementById("sceneModifierSettings");
+        // sceneModifierSettings.innerHTML = "";
+        // TODO make them invisible and only the select one displayed / collapse / none ?
+        sceneModifierSettings.appendChild(createRadioElement(response_json["title"], response_json["properties"]));
     });
+}
 
 
-}
 
 window.addEventListener("keydown", (event) => {
     if (event.isComposing || event.key === " ") {
         event.preventDefault();
         if (animation_running && animation_frame == frames.length - 1) {
             animation_frame = 0;
         } else {
@@ -734,43 +624,24 @@
     }
     if (event.isComposing || event.key === "ArrowDown") {
         animation_frame = parseInt(Math.max(0, animation_frame - (frames.length / 10)));
     }
     if (event.isComposing || event.key === "q") {
         getAnimationFrames();
     }
-    if (event.isComposing || event.shiftKey) {
-        keydown["shift"] = true;
-    }
-    if (event.isComposing || event.ctrlKey) {
-        keydown["strg"] = true;
-    }
-    if (event.isComposing || event.altKey) {
-        keydown["alt"] = true;
-    }
-    for (let key in keydown) {
-        if (event.isComposing || event.key === key) {
-            keydown[key] = true;
-        }
-    }
+    if (event.isComposing || event.key === "i") {
+        PARTICLES.printIndices(camera);
+    };
 });
 
 window.addEventListener("keyup", (event) => {
-    if (event.isComposing || !event.shiftKey) {
-        keydown["shift"] = false;
-    }
-    if (event.isComposing || !event.ctrlKey) {
-        keydown["ctrl"] = false;
-    }
-    if (event.isComposing || !event.altKey) {
-        keydown["alt"] = false;
-    }
-    for (let key in keydown) {
-        if (event.isComposing || event.key === key) {
-            keydown[key] = false;
+    if (event.isComposing || event.key === "i") {
+        let ids = document.getElementsByClassName("particle-id")
+        while (ids.length > 0) {
+            ids[0].parentNode.removeChild(ids[0]);
         }
     }
 });
 
 window.addEventListener("keydown", (event) => {
     if (event.isComposing || event.key === "Enter") {
         div_info.innerHTML = "Processing...";
@@ -778,24 +649,41 @@
         fetch("update", {
             "method": "POST",
             "headers": {
                 "Content-Type": "application/json"
             },
             "body": JSON.stringify({
                 "selected_ids": selected_ids,
-                "step": animation_frame
+                "step": animation_frame,
+                "points": DRAW.positions
             }),
-        }).then((response) => getAnimationFrames());
-
-        if (!data_loading) {
+        }).then((response) => {
+            if (frames.length > 0) {
+                frames.length = animation_frame + 1;
+            }
             getAnimationFrames();
-        }
+        });
     }
 });
 
+// Drawing
+
+DRAW.init(camera, renderer, scene, controls)
+
+document.getElementById("drawAddAnchor").onclick = function() {
+    let {
+        position
+    } = PARTICLES.particleGroup.children[selected_ids[0]].children[0];
+    DRAW.createAnchorPoint(position);
+};
+
+document.getElementById("drawRemoveLine").onclick = function() {
+    DRAW.reset();
+};
+
 
 
 
 let move_atoms_clock = new THREE.Clock();
 
 
 function move_atoms() {
@@ -822,56 +710,26 @@
         return;
     }
     if (config["total_frames"] > 0) {
         div_progressBar.style.visibility = "visible";
         div_progressBar.style.width = ((animation_frame / config["total_frames"]) * 100).toFixed(2) + "%";
         div_bufferBar.style.width = (((frames.length - 1) / config["total_frames"]) * 100).toFixed(2) + "%";
     }
-
-    if (frames[animation_frame].length != atomsGroup.children.length) {
+    if (frames[animation_frame].length != PARTICLES.particleGroup.children.length) {
         // we need to update the scene
         build_scene(animation_frame);
         scene_building = true;
         return; // we need to wait for the scene to be updated
     }
 
-
-    frames[animation_frame].forEach(function(item, index) {
-        atomsGroup.getObjectByUserDataProperty("id", index).position.set(...item);
-    });
-
     div_info.innerHTML = "Frame (" + animation_frame + "/" + (frames.length - 1) + ")";
 
-    if (config["bond_size"] > 0) {
-        scene.updateMatrixWorld();
-
-        for (let i = 0; i < bondsGroup_1.children.length; i++) {
-            let bond_1 = bondsGroup_1.children[i];
-            let bond_2 = bondsGroup_2.children[i];
-
-            atomsGroup.getObjectByUserDataProperty("id", bond_1.userData["atom_id"]).getWorldPosition(node1);
-            atomsGroup.getObjectByUserDataProperty("id", bond_2.userData["atom_id"]).getWorldPosition(node2);
-
-            let direction = new THREE.Vector3().subVectors(node1, node2);
-
-            let scale = (direction.length() / 2) / bond_1.geometry.parameters.height;
-
-            if (scale > 1.5) {
-                scale = 0.0;
-            }
-
-            bond_1.scale.set(1, 1, scale);
-            bond_2.scale.set(1, 1, scale);
-
-            bond_1.position.copy(node1);
-            bond_2.position.copy(node2);
-
-            bond_1.lookAt(node2);
-            bond_2.lookAt(node1);
-        }
+    if (animation_frame != displayed_frame) {
+        displayed_frame = animation_frame;
+        PARTICLES.updateParticlePositions(frames[animation_frame]);
     }
 
     fps.push(move_atoms_clock.getElapsedTime());
 
     if (fps.length > 10) {
         fps.shift();
     }
@@ -881,20 +739,26 @@
 
     div_FPS.innerHTML = (1 / (fps.reduce((a, b) => a + b, 0) / fps.length)).toFixed(2);
     move_atoms_clock.start();
 }
 
 function centerCamera() {
     if (selected_ids.length === 0) {
-        controls.target = new THREE.Vector3(0, 0, 0);
+        controls.target = PARTICLES.getAtomsCenter([...Array(PARTICLES.particleGroup.children.length).keys()]);
     } else {
-        controls.target = atomsGroup.getObjectByUserDataProperty("id", selected_ids[0]).position.clone();
+        controls.target = PARTICLES.getAtomsCenter(selected_ids);
     }
 }
 
+/**
+ * Dynamic indices
+ * 
+ */
+
+
 function animate() {
 
     renderer.render(scene, camera);
     controls.update();
 
     if (frames.length > 0) {
         move_atoms();
```

### Comparing `zndraw-0.1.3/zndraw/templates/index.html` & `zndraw-0.1.4/zndraw/templates/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -10,236 +10,322 @@
     integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
   <link rel="stylesheet" href="{{ url_for('static', filename='main.css') }}">
   <script async src="https://unpkg.com/es-module-shims@1.6.3/dist/es-module-shims.js"></script>
   <script type="importmap">
   {
     "imports": {
       "three": "https://unpkg.com/three@0.151.3/build/three.module.js",
-      "three/addons/": "https://unpkg.com/three@0.151.3/examples/jsm/"
+      "three/addons/": "https://unpkg.com/three@0.151.3/examples/jsm/",
+      "./modules/": "{{ url_for('static', filename='/modules/') }}"
     }
   }
 </script>
 </head>
 
 <body>
   <script type="module" src="{{ url_for('static', filename='main.js') }}"></script>
 
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
     integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe"
     crossorigin="anonymous"></script>
 
-  <div class="hamburger-menu">
-    <input id="menu__toggle" type="checkbox" />
-    <label class="menu__btn" for="menu__toggle">
-      <span></span>
-    </label>
-
-    <ul class="menu__box">
-      <h1 class="menu__header">ZnDraw</h1>
-      <div class="accordion" id="accordionPanelsStayOpenExample">
-        <div class="accordion-item">
-          <h2 class="accordion-header" id="panelsStayOpen-headingOne">
-            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
-              data-bs-target="#panelsStayOpen-collapseOne" aria-expanded="false"
-              aria-controls="panelsStayOpen-collapseOne">
-              Settings
+  <!-- Loading Spinner -->
+  <div class="atom-spinner" , id="atom-spinner">
+    <div class="spinner-inner">
+      <div class="spinner-line"></div>
+      <div class="spinner-line"></div>
+      <div class="spinner-line"></div>
+      <!--Chrome renders little circles malformed :(-->
+      <div class="spinner-circle">
+        &#9679;
+      </div>
+    </div>
+  </div>
+  <div id="greyOut"></div>
+
+
+  <!-- Navigation -->
+
+  <nav class="navbar fixed-top navbar-expand-sm bg-light"> <!-- navbar-expand to use smaller breakpoint -->
+    <div class="container-fluid">
+      <a class="navbar-brand">
+        <!-- <img src="{{ url_for('static', filename='favion-192x192.png') }}" alt="ZnDraw Logo" width="30" height="24"> -->
+        ZnDraw
+      </a>
+      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown"
+        aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
+        <span class="navbar-toggler-icon"></span>
+      </button>
+      <div class="collapse navbar-collapse" id="navbarNavDropdown">
+        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
+          <li class="nav-item mx-1">
+            <button class="btn btn-outline-secondary" type="button" data-bs-toggle="offcanvas"
+              data-bs-target="#particleCanvas" aria-controls="particleCanvas">
+              Particles
             </button>
-          </h2>
-          <div id="panelsStayOpen-collapseOne" class="accordion-collapse collapse"
-            aria-labelledby="panelsStayOpen-headingOne">
-            <div class="container">
-              <div class="accordion-body">
-                <div class="row">
-                  <div class="col-sm">
-                    <div class="form-check form-switch">
-                      <input class="form-check-input" type="checkbox" value="" id="selectAtoms" checked>
-                      <label class="form-check-label" for="selectAtoms">
-                        Select Atoms
-                      </label>
-                    </div>
-                    <div class="form-check form-switch">
-                      <input class="form-check-input" type="checkbox" value="" id="autoRestart">
-                      <label class="form-check-label" for="autoRestart">
-                        Auto Restart
-                      </label>
-                    </div>
-
-                    <select class="form-select" aria-label="Default select example" id="materialSelect">
-                      <option selected>Select Material</option>
-                    </select>
-
-                    <div class="form-check form-switch">
-                      <input class="form-check-input" type="checkbox" value="" id="wireframe">
-                      <label class="form-check-label" for="wireframe">
-                        Wireframe
-                      </label>
-                    </div>
-                  </div>
-                  <div class="col-sm">
-                    <div class="row">
-                      <div class="col-sm-3">
-                        <div class="row">Max FPS</div>
-                        <div class="row">POST</div>
-
-                        <div class="row">1. Light</div>
-                        <div class="row">2. Light</div>
-                      </div>
-                      <div class="col-sm-2">
-                        <div class="row"><output id="max_fps_output">{{ config.max_fps }}</output></div>
-                        <div class="row"><output id="frames_per_post_output">{{ config.frames_per_post }}</output></div>
-
-                        <div class="row"><output id="spotLightIntensity_output">1</output></div>
-                        <div class="row"><output id="hemisphereLightIntensity_output">0.1</output></div>
-                      </div>
-                      <div class="col-sm">
-                        <div class="row"><input type="range" class="form-range" min="1" max="100" step="0.5"
-                            id="max_fps" value="{{ config.max_fps }}" , oninput="max_fps_output.value = this.value">
-                        </div>
-                        <div class="row"><input type="range" class="form-range" min="1" max="500" id="frames_per_post"
-                            value="{{ config.frames_per_post }}" , oninput="frames_per_post_output.value = this.value">
-                        </div>
-
-                        <div class="row"><input type="range" class="form-range" min="0" max="1" step="0.01"
-                            id="spotLightIntensity" value="1"></div>
-                        <div class="row"><input type="range" class="form-range" min="0" max="1" step="0.01"
-                            id="hemisphereLightIntensity" value="0.1"></div>
-                      </div>
-                      <div class="col-sm-1"><!-- Padding on the right --></div>
-
-                    </div>
-                  </div>
-                </div>
-              </div>
-            </div>
-          </div>
-        </div>
-        <div class="accordion-item">
-          <h2 class="accordion-header" id="panelsStayOpen-headingTwo">
-            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
-              data-bs-target="#panelsStayOpen-collapseTwo" aria-expanded="false"
-              aria-controls="panelsStayOpen-collapseTwo">
-              Controls
+          </li>
+          <li class="nav-item mx-1">
+            <button class="btn btn-outline-secondary" type="button" data-bs-toggle="offcanvas"
+              data-bs-target="#interactionCanvas" aria-controls="interactionCanvas">
+              Interaction
+            </button>
+          </li>
+          <li class="nav-item mx-1">
+            <button class="btn btn-outline-secondary" type="button" data-bs-toggle="offcanvas"
+              data-bs-target="#sceneCanvas" aria-controls="sceneCanvas">
+              Scene
+            </button>
+          </li>
+          <li class="nav-item mx-1">
+            <button class="btn btn-outline-secondary" type="button" data-bs-toggle="offcanvas"
+              data-bs-target="#drawCanvas" aria-controls="drawCanvas">
+              Draw
             </button>
-          </h2>
-          <div id="panelsStayOpen-collapseTwo" class="accordion-collapse collapse"
-            aria-labelledby="panelsStayOpen-headingTwo">
-            <div class="accordion-body">
-
-              <div class="container">
-                <div class="row">
-                  <div class="col-sm">
-
-                    <div class="btn-group-vertical" role="group" aria-label="Basic example">
-                      <button type="button" class="btn btn-secondary" id="animate" {% if config.update_function %}
-                        disabled {% endif %}>Load Animation</button>
-                      <button type="button" class="btn btn-secondary" id="reset_selection">Reset Selection</button>
-                      <button type="button" class="btn btn-secondary" id="hide_selection" disabled>Hide
-                        Selection</button>
-                      <button type="button" class="btn btn-secondary" id="reset">Reset Scene</button>
-                    </div>
-                  </div>
-                  <div class="col-sm">
-                    <div class="btn-group-vertical" role="group" aria-label="Basic example">
-                      <button type="button" class="btn btn-outline-dark" id="sphere_plus">+</button>
-                      <button type="button" class="btn btn-outline-dark" id="bond_plus">+</button>
-                      <button type="button" class="btn btn-outline-dark" id="resolution_plus">+</button>
-                    </div>
-                    <div class="btn-group-vertical" role="group" aria-label="Basic example">
-                      <button type="button" class="btn btn-outline-dark" disabled>Particles</button>
-                      <button type="button" class="btn btn-outline-dark" disabled>Bonds</button>
-                      <button type="button" class="btn btn-outline-dark" disabled>Resolution</button>
-                    </div>
-                    <div class="btn-group-vertical" role="group" aria-label="Basic example">
-                      <button type="button" class="btn btn-outline-dark" id="sphere_minus">-</button>
-                      <button type="button" class="btn btn-outline-dark" id="bond_minus">-</button>
-                      <button type="button" class="btn btn-outline-dark" id="resolution_minus">-</button>
-                    </div>
-                  </div>
-                </div>
-              </div>
+          </li>
+        </ul>
+        <form class="d-flex">
+          <button class="btn btn-outline-primary mx-1" type="button" data-bs-toggle="collapse"
+            data-bs-target="#helpBoxCollapse" aria-expanded="false" aria-controls="helpBoxCollapse">
+            Help
+          </button>
+          <button class="btn btn-outline-primary" type="button" data-bs-toggle="collapse"
+            data-bs-target="#infoBoxCollapse" aria-expanded="false" aria-controls="infoBoxCollapse">
+            Info
+          </button>
+        </form>
+      </div>
+    </div>
+  </nav>
+
+  <!-- Off Canvas -->
+  <!-- Particles -->
+  <div class="offcanvas offcanvas-start canvasControl" data-bs-scroll="true" data-bs-backdrop="false" tabindex="-1"
+    id="particleCanvas" aria-labelledby="particleCanvasLabel">
+    <div class="offcanvas-header">
+      <h5 class="offcanvas-title" id="particleCanvasLabel">Particles</h5>
+      <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
+    </div>
+    <div class="offcanvas-body">
+
+      <div class="mb-3">
+        <label for="materialSelect" class="form-label">Select particle material</label>
+        <select class="form-select" id="materialSelect">
+        </select>
+        <div id="materialSelectHelp" class="form-text">Change the material of the particles and bonds..</div>
+      </div>
+      <div class="mb-3">
+        <input class="form-check-input" type="checkbox" value="" id="wireframe">
+        <label for="wireframe" class="form-label">Wireframe material</label>
+      </div>
+      <div class="mb-3">
+        <label for="sphereRadius" class="form-label" id="sphereRadiusLabel">Sphere radius: {{ config['sphere_size']
+          }}</label>
+        <input type="range" class="form-range" id="sphereRadius" min="0.1" max="4" step="0.1"
+          value="{{ config['sphere_size'] }}">
+      </div>
+      <div class="mb-3">
+        <label for="bondDiameter" class="form-label" id="bondDiameterLabel">Bond diameter: {{ config['bond_size']
+          }}</label>
+        <input type="range" class="form-range" id="bondDiameter" min="0.1" max="2.0" step="0.1"
+          value="{{ config['bond_size'] }}">
+      </div>
+      <div class="mb-3">
+        <label for="resolution" class="form-label" id="resolutionLabel">Resolution: {{ config['resolution'] }}</label>
+        <input type="range" class="form-range" id="resolution" min="1" max="20" step="1"
+          value="{{ config['resolution'] }}">
+      </div>
+
+    </div>
+  </div>
+
+  <!-- Interaction -->
+  <div class="offcanvas offcanvas-start canvasControl" data-bs-scroll="true" data-bs-backdrop="false" tabindex="-1"
+    id="interactionCanvas" aria-labelledby="interactioneCanvasLabel">
+    <div class="offcanvas-header">
+      <h5 class="offcanvas-title" id="interactionCanvasLabel">Interaction</h5>
+      <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
+    </div>
+    <div class="offcanvas-body">
+
+      <div class="mb-3">
+        <label for="selection-method" class="form-label">Selection Method</label>
+        <select class="form-select" aria-label="Default select example" id="selection-method">
+          <option selected, value="particles">Particles</option>
+          <option value="species">Species</option>
+          <option value="connected">Connected Particles</option>
+          <option value="none">None</option>
+        </select>
+        <div id="selection-methodHelp" class="form-text">Select single particles, whole molecules or disable selection.
+        </div>
+      </div>
+      <div class="mb-3">
+        <button type="button" class="btn btn-secondary" id="reset_selection">Reset Selection</button>
+      </div>
+      <div class="mb-3">
+        <label for="addSceneModifier" class="form-label">Select scene modifier</label>
+        <select class="form-select" aria-label="Default select example" id="addSceneModifier">
+          <option selected, value="none"> </option>
+          <option value="add">Add New</option>
+        </select>
+        <div id="addSceneModifierHelp" class="form-text">Load a Python class to modify the scene
+        </div>
+      </div>
+      <div id="sceneModifierSettings"></div>
+    </div>
+  </div>
+
+  <!-- Scene -->
+  <div class="offcanvas offcanvas-start canvasControl" data-bs-scroll="true" data-bs-backdrop="false" tabindex="-1"
+    id="sceneCanvas" aria-labelledby="sceneCanvasLabel">
+    <div class="offcanvas-header">
+      <h5 class="offcanvas-title" id="sceneCanvasLabel">Scene</h5>
+      <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
+    </div>
+    <div class="offcanvas-body">
+
+      <div class="mb-3">
+        <label for="spotLightIntensity" class="form-label" id="spotLightIntensityLabel">Spot light intensity:
+          1.0</label>
+        <input type="range" class="form-range" min="0" max="1" step="0.01" id="spotLightIntensity" value="1">
+      </div>
+      <div class="mb-3">
+        <label for="hemisphereLightIntensity" class="form-label" id="hemisphereLightIntensityLabel">Hemisphere light
+          intensity: 1.0</label>
+        <input type="range" class="form-range" min="0" max="1" step="0.01" id="hemisphereLightIntensity" value="0.1">
+      </div>
+      <div class="mb-3">
+        <label for="max_fps" class="form-label" id="max_fpsLabel">Max FPS: {{ config.max_fps }}</label>
+        <input type="range" class="form-range" min="1" max="100" step="0.5" id="max_fps" value="{{ config.max_fps }}" ,
+          oninput="max_fpsLabel.innerHTML = 'Max FPS: ' + this.value">
+      </div>
+      <div class="mb-3">
+        <input class="form-check-input" type="checkbox" value="" id="autoRestart">
+        <label class="form-check-label" for="autoRestart">
+          Auto Restart
+        </label>
+      </div>
+      <div class="mb-3">
+        <button type="button" class="btn btn-secondary" id="reset">Reset Scene</button>
+        <button type="button" class="btn btn-secondary" id="animate" {% if config.update_function %} disabled {% endif
+          %}>Load Animation</button>
+      </div>
+    </div>
+  </div>
+
+  <!-- Draw -->
+  <div class="offcanvas offcanvas-start canvasControl" data-bs-scroll="true" data-bs-backdrop="false" tabindex="-1"
+    id="drawCanvas" aria-labelledby="drawCanvasLabel">
+    <div class="offcanvas-header">
+      <h5 class="offcanvas-title" id="drawCanvasLabel">Draw</h5>
+      <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
+    </div>
+    <div class="offcanvas-body">
+
+      <div class="mb-3">
+        <button type="button" class="btn btn-secondary" id="drawAddAnchor">Add anchor point</button>
+        <button type="button" class="btn btn-secondary" id="drawRemoveLine">Remove Line</button>
+      </div>
+    </div>
+  </div>
+
+
+  <!-- TODOs -->
+  <div style="display: none;">
+    <div class="row">
+      <div class="col-sm">
+        <div class="form-check form-switch">
+        </div>
+
+
+      </div>
+      <div class="col-sm">
+        <div class="row">
+          <div class="col-sm-3">
+            <div class="row">Max FPS</div>
+            <div class="row">POST</div>
+
+            <div class="row">1. Light</div>
+            <div class="row">2. Light</div>
+          </div>
+          <div class="col-sm-2">
+            <div class="row"><output id="frames_per_post_output">{{ config.frames_per_post }}</output></div>
+
+          </div>
+          <div class="col-sm">
+            <div class="row">
+            </div>
+            <div class="row"><input type="range" class="form-range" min="1" max="500" id="frames_per_post"
+                value="{{ config.frames_per_post }}" , oninput="frames_per_post_output.value = this.value">
             </div>
+
+            <div class="row"></div>
+            <div class="row"></div>
           </div>
+          <div class="col-sm-1"><!-- Padding on the right --></div>
+
         </div>
-        <div class="accordion-item">
-          <h2 class="accordion-header" id="panelsStayOpen-headingThree">
-            <button class="accordion-button" type="button" data-bs-toggle="collapse"
-              data-bs-target="#panelsStayOpen-collapseThree" aria-expanded="true"
-              aria-controls="panelsStayOpen-collapseThree">
-              Info
-            </button>
-          </h2>
-          <div id="panelsStayOpen-collapseThree" class="accordion-collapse collapse show"
-            aria-labelledby="panelsStayOpen-headingThree">
-            <div class="accordion-body">
-              <dl class="row">
-                <dt class="col-sm-3">File</dt>
-                <dd class="col-sm-9"><code>{{ config.file }}</code></dd>
-                <dt class="col-sm-3">FPS</dt>
-                <dd class="col-sm-9" id="FPS">-</dd>
-                <dt class="col-sm-3">Particles</dt>
-                <dd class="col-sm-9" id="n_particles">-</dd>
-                <dt class="col-sm-3">Bonds</dt>
-                <dd class="col-sm-9" id="n_bonds">-</dd>
-                <dt class="col-sm-3">Selected IDs</dt>
-                <dd class="col-sm-9" id="lst_selected_ids"></dd>
-                {% if config.update_function %}
-                <dt class="col-sm-3">Function</dt>
-                <dd class="col-sm-9" id="lst_selected_ids"><code>{{ config.update_function }}</code></dd>
-                {% endif %}
-              </dl>
-            </div>
+      </div>
+    </div>
+    <div class="container">
+      <div class="row">
+        <div class="col-sm">
+
+          <div class="btn-group-vertical" role="group" aria-label="Basic example">
+            <button type="button" class="btn btn-secondary" id="hide_selection" disabled>Hide
+              Selection</button>
           </div>
         </div>
-        <div class="accordion-item">
-          <h2 class="accordion-header" id="panelsStayOpen-headingFour">
-            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
-              data-bs-target="#panelsStayOpen-collapseFour" aria-expanded="false"
-              aria-controls="panelsStayOpen-collapseFour">
-              Manipulate Particles
-            </button>
-          </h2>
-          <div id="panelsStayOpen-collapseFour" class="accordion-collapse collapse"
-            aria-labelledby="panelsStayOpen-headingFour">
-            <div class="accordion-body">
-              <div id="python_class_control"></div>
-            </div>
+        <div class="col-sm">
+          <div class="btn-group-vertical" role="group" aria-label="Basic example">
+            <button type="button" class="btn btn-outline-dark" id="sphere_plus">+</button>
+            <button type="button" class="btn btn-outline-dark" id="bond_plus">+</button>
+            <button type="button" class="btn btn-outline-dark" id="resolution_plus">+</button>
+          </div>
+          <div class="btn-group-vertical" role="group" aria-label="Basic example">
+            <button type="button" class="btn btn-outline-dark" disabled>Particles</button>
+            <button type="button" class="btn btn-outline-dark" disabled>Bonds</button>
+            <button type="button" class="btn btn-outline-dark" disabled>Resolution</button>
+          </div>
+          <div class="btn-group-vertical" role="group" aria-label="Basic example">
+            <button type="button" class="btn btn-outline-dark" id="sphere_minus">-</button>
+            <button type="button" class="btn btn-outline-dark" id="bond_minus">-</button>
+            <button type="button" class="btn btn-outline-dark" id="resolution_minus">-</button>
           </div>
         </div>
       </div>
-    </ul>
+    </div>
   </div>
 
-  <div id="loading">
-    <div class="atom-spinner">
-      <div class="spinner-inner">
-        <div class="spinner-line"></div>
-        <div class="spinner-line"></div>
-        <div class="spinner-line"></div>
-        <!--Chrome renders little circles malformed :(-->
-        <div class="spinner-circle">
-          &#9679;
-        </div>
-      </div>
+  <!-- Info Box -->
+  <div class="collapse" id="infoBoxCollapse">
+    <div class="container-fluid rounded border border-dark" id="infoBox">
+      <dl class="row">
+        <dt class="col-sm-3">File</dt>
+        <dd class="col-sm-9"><code>{{ config.file }}</code></dd>
+        <dt class="col-sm-3">FPS</dt>
+        <dd class="col-sm-9" id="FPS">-</dd>
+        <dt class="col-sm-3">Particles</dt>
+        <dd class="col-sm-9" id="n_particles">-</dd>
+        <dt class="col-sm-3">Bonds</dt>
+        <dd class="col-sm-9" id="n_bonds">-</dd>
+        <dt class="col-sm-3">Selected IDs</dt>
+        <dd class="col-sm-9" id="lst_selected_ids"></dd>
+        {% if config.update_function %}
+        <dt class="col-sm-3">Function</dt>
+        <dd class="col-sm-9" id="lst_selected_ids"><code>{{ config.update_function }}</code></dd>
+        {% endif %}
+      </dl>
     </div>
   </div>
-  <div id="info"></div>
-  <div id="progressBar"></div>
-  <div id="bufferBar"></div>
-  <div id="greyOut"></div>
-  <div id="right_btn_group">
-    <img id="help_btn" src="https://openmoji.org/data/color/svg/2139.svg" />
-    <img id="add_btn" src="https://openmoji.org/data/color/svg/2795.svg" />
-  </div>
-
 
-  <div class="container py-4" id="help_container" style="display: none; opacity: 0.9;">
-    <div class="h-100 p-5 bg-light rounded-3 border border-primary">
+  <!-- Help Box -->
+  <div class="collapse" id="helpBoxCollapse">
+    <div class="container-fluid bg-light rounded border border-primary pt-2" id="helpBox">
       <h2>ZnDraw Help</h2>
-      <br>
-      <div class="rounded-3 bg-white" , style="padding-left: 10px;">
+      <div class="rounded-3 bg-white px-2 pt-2">
         <dl class="row">
           <dt class="col-sm-3">move light to camera position</dt>
           <dd class="col-sm-9"><code>keypress L</code></dd>
           <dt class="col-sm-3">play / pause</dt>
           <dd class="col-sm-9"><code>keypress space</code></dd>
           <dt class="col-sm-3">frame forwards / backwards</dt>
           <dd class="col-sm-9"><code>keypress &#9654;\&#9664; </code></dd>
@@ -249,31 +335,48 @@
           <dd class="col-sm-9"><code>keypress enter</code></dd>
           <dt class="col-sm-3">center camera around selected particle</dt>
           <dd class="col-sm-9"><code>keypress C</code></dd>
           <dt class="col-sm-3">reload animation</dt>
           <dd class="col-sm-9"><code>keypress Q</code></dd>
           <dt class="col-sm-3">select multiple particles</dt>
           <dd class="col-sm-9"><code>keydown shift</code></dd>
-
+          <dt class="col-sm-3">show particle index</dt>
+          <dd class="col-sm-9"><code>keydown I</code></dd>
         </dl>
       </div>
     </div>
   </div>
 
-  <div id="add_class">
-    <div class="container py-4" id="help_container">
-      <div class="h-100 p-5 bg-light rounded-3 border border-primary">
-        <div class="form-group">
-          <label for="newPythonClass">Add path to python module</label>
-          <input class="form-control" id="newPythonClass" placeholder="zndraw.examples.Duplicate">
-          <br>
-          <button id="newPythonClassBtn" class="btn btn-primary">Add to Scene</button>
+  <!-- Add Scene Modifer -->
+  <div class="modal" tabindex="-1" id="addModifierModal">
+    <div class="modal-dialog">
+      <div class="modal-content">
+        <div class="modal-header">
+          <h5 class="modal-title">Add Scene Modifier</h5>
+          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
+        </div>
+        <div class="modal-body">
+          <div class="mb-3">
+            <label for="addSceneModifierImport" class="form-label">Path to modifier <code>class</code></label>
+            <input type="email" class="form-control" id="addSceneModifierImport"
+              aria-describedby="addSceneModifierImportHelp">
+            <div id="addSceneModifierImportHelp" class="form-text">The input should be <code>module.cls</code> such that
+              <code> from module import cls</code> works.
+            </div>
+          </div>
+        </div>
+        <div class="modal-footer">
+          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
+          <button type="button" class="btn btn-primary" id="addSceneModifierImportBtn">Load</button>
         </div>
       </div>
     </div>
   </div>
 
-
+  <!-- Progress Bar -->
+  <div id="info"></div>
+  <div id="progressBar"></div>
+  <div id="bufferBar"></div>
 
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,42 +1,57 @@
 
 
-⁰
-****** ZnDraw ******
-*****  Settings  *****
-*  Select Atoms
+
+ id="atom-spinner">
+●
+
+ ZnDraw
+    *  Particles
+    *  Interaction
+    *  Scene
+    *  Draw
+ Help   Info
+
+** Particles **
+Change the material of the particles and bonds..
+⁰ Wireframe material
+Sphere radius: {{ config['sphere_size'] }} [Unknown INPUT type]
+Bond diameter: {{ config['bond_size'] }} [Unknown INPUT type]
+Resolution: {{ config['resolution'] }} [Unknown INPUT type]
+** Interaction **
+ value="particles">Particles
+Species
+Connected Particles
+None
+Select single particles, whole molecules or disable selection.
+Reset Selection
+ value="none">
+Add New
+Load a Python class to modify the scene
+** Scene **
+Spot light intensity: 1.0 [Unknown INPUT type]
+Hemisphere light intensity: 1.0 [Unknown INPUT type]
+Max FPS: {{ config.max_fps }}
+ oninput="max_fpsLabel.innerHTML = 'Max FPS: ' + this.value">
 ⁰  Auto Restart
-[One of: Select Material]
-⁰  Wireframe
+Reset Scene
+% if config.update_function %} disabled {% endif %}>Load Animation
+** Draw **
+Add anchor point Remove Line
 Max FPS
 POST
 1. Light
 2. Light
-{{ config.max_fps }}
 {{ config.frames_per_post }}
-1
-0.1
- oninput="max_fps_output.value = this.value">
  oninput="frames_per_post_output.value = this.value">
-[Unknown INPUT type]
-[Unknown INPUT type]
-*****  Controls  *****
-% if config.update_function %} disabled {% endif %}>Load Animation Reset
-Selection Hide Selection Reset Scene
+Hide Selection
 + + +
 Particles Bonds Resolution
 - - -
-*****  Info  *****
-*****  Manipulate Particles  *****
-●
-[https://openmoji.org/data/color/svg/2139.svg] [https://openmoji.org/data/
-color/svg/2795.svg]
 ***** ZnDraw Help *****
-
- style="padding-left: 10px;">
   move light to camera position
       keypress L
   play / pause
       keypress space
   frame forwards / backwards
       keypress ▶\◀
   jump forwards / backwards
@@ -45,9 +60,13 @@
       keypress enter
   center camera around selected particle
       keypress C
   reload animation
       keypress Q
   select multiple particles
       keydown shift
-Add path to python module [                    ]
-Add to Scene
+  show particle index
+      keydown I
+** Add Scene Modifier **
+Path to modifier class [Unknown INPUT type]
+The input should be module.cls such that from module import cls works.
+Close Load
```

### Comparing `zndraw-0.1.3/PKG-INFO` & `zndraw-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zndraw
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -42,21 +42,22 @@
 
 ```python
 import abc
 from pydantic import BaseModel
 
 class UpdateScene(BaseModel, abc.ABC):
     @abc.abstractmethod
-    def run(self, atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
+    def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         pass
 ```
 
 The ``run`` method expects as inputs
 - atom_ids: list[int], the ids of the currently selected atoms
 - atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where selected.
+- kwargs: dict could be additional information from the scene
 
 and as an output:
 - list[ase.Atoms], a list of ase Atoms objects to display.
 
 
 You can define the parameters using `pydantic.Field` which will be displayed in the UI.
 
@@ -67,9 +68,13 @@
     symbol: str = Field("same")
 ```
 
 To add your method click on the `+` on the right side of the window.
 Your should be able to add your method from the working directory via `module.MyUpdateCls` as long
 as it can be imported via `from module import MyUpdateCls`.
 
-![Alt text](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
+![ZnDraw UI](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
+
+![ZnDraw UI2](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_protein.png "ZnDraw UI2")
+
+![ZnDraw UI3](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_draw.png "ZnDraw UI3")
```

