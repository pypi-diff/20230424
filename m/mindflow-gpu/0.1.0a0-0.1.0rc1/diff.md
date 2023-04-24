# Comparing `tmp/mindflow_gpu-0.1.0a0-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/mindflow_gpu-0.1.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,104 +1,98 @@
-Zip file size: 153827 bytes, number of entries: 102
--rw-r--r--  2.0 unx     2960 b- defN 23-Jan-31 12:26 mindflow/__init__.py
--rw-r--r--  2.0 unx     2239 b- defN 23-Jan-31 12:26 mindflow/setup.py
--rw-r--r--  2.0 unx     1009 b- defN 23-Jan-31 12:26 mindflow/cell/__init__.py
--rw-r--r--  2.0 unx     3492 b- defN 23-Jan-31 12:26 mindflow/cell/activation.py
--rw-r--r--  2.0 unx    21410 b- defN 23-Jan-31 12:26 mindflow/cell/basic_block.py
--rw-r--r--  2.0 unx     5040 b- defN 23-Jan-31 12:26 mindflow/cell/utils.py
--rw-r--r--  2.0 unx      811 b- defN 23-Jan-31 12:26 mindflow/cell/neural_operators/__init__.py
--rw-r--r--  2.0 unx    14413 b- defN 23-Jan-31 12:26 mindflow/cell/neural_operators/dft.py
--rw-r--r--  2.0 unx     7621 b- defN 23-Jan-31 12:26 mindflow/cell/neural_operators/fno1d.py
--rw-r--r--  2.0 unx     9511 b- defN 23-Jan-31 12:26 mindflow/cell/neural_operators/fno2d.py
--rw-r--r--  2.0 unx     2357 b- defN 23-Jan-31 12:26 mindflow/cell/neural_operators/m2k.py
--rw-r--r--  2.0 unx    10030 b- defN 23-Jan-31 12:26 mindflow/cell/neural_operators/pdenet.py
--rw-r--r--  2.0 unx      699 b- defN 23-Jan-31 12:26 mindflow/cell/transformer/__init__.py
--rw-r--r--  2.0 unx    14042 b- defN 23-Jan-31 12:26 mindflow/cell/transformer/layer.py
--rw-r--r--  2.0 unx     6350 b- defN 23-Jan-31 12:26 mindflow/cell/transformer/vit.py
--rw-r--r--  2.0 unx      971 b- defN 23-Jan-31 12:26 mindflow/cfd/__init__.py
--rw-r--r--  2.0 unx     2531 b- defN 23-Jan-31 12:26 mindflow/cfd/mesh_info.py
--rw-r--r--  2.0 unx     4168 b- defN 23-Jan-31 12:26 mindflow/cfd/runtime.py
--rw-r--r--  2.0 unx     3298 b- defN 23-Jan-31 12:26 mindflow/cfd/simulator.py
--rw-r--r--  2.0 unx     4714 b- defN 23-Jan-31 12:26 mindflow/cfd/utils.py
--rw-r--r--  2.0 unx     2956 b- defN 23-Jan-31 12:26 mindflow/cfd/visualization.py
--rw-r--r--  2.0 unx      749 b- defN 23-Jan-31 12:26 mindflow/cfd/boundary_conditions/__init__.py
--rw-r--r--  2.0 unx     1165 b- defN 23-Jan-31 12:26 mindflow/cfd/boundary_conditions/base.py
--rw-r--r--  2.0 unx     2752 b- defN 23-Jan-31 12:26 mindflow/cfd/boundary_conditions/boundary_manager.py
--rw-r--r--  2.0 unx     1247 b- defN 23-Jan-31 12:26 mindflow/cfd/boundary_conditions/neumann.py
--rw-r--r--  2.0 unx     1173 b- defN 23-Jan-31 12:26 mindflow/cfd/boundary_conditions/periodic.py
--rw-r--r--  2.0 unx     1319 b- defN 23-Jan-31 12:26 mindflow/cfd/boundary_conditions/symmetry.py
--rw-r--r--  2.0 unx     1836 b- defN 23-Jan-31 12:26 mindflow/cfd/boundary_conditions/wall.py
--rw-r--r--  2.0 unx     1119 b- defN 23-Jan-31 12:26 mindflow/cfd/integrator/__init__.py
--rw-r--r--  2.0 unx      935 b- defN 23-Jan-31 12:26 mindflow/cfd/integrator/base.py
--rw-r--r--  2.0 unx     1056 b- defN 23-Jan-31 12:26 mindflow/cfd/integrator/euler.py
--rw-r--r--  2.0 unx     1307 b- defN 23-Jan-31 12:26 mindflow/cfd/integrator/runge_kutta3.py
--rw-r--r--  2.0 unx     1054 b- defN 23-Jan-31 12:26 mindflow/cfd/material/__init__.py
--rw-r--r--  2.0 unx     2685 b- defN 23-Jan-31 12:26 mindflow/cfd/material/base.py
--rw-r--r--  2.0 unx     1897 b- defN 23-Jan-31 12:26 mindflow/cfd/material/ideal_gas.py
--rw-r--r--  2.0 unx      735 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/__init__.py
--rw-r--r--  2.0 unx     1812 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/godunov_flux.py
--rw-r--r--  2.0 unx     2982 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/space_solver.py
--rw-r--r--  2.0 unx     6133 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/viscous_flux.py
--rw-r--r--  2.0 unx     1348 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/derivative_computer/__init__.py
--rw-r--r--  2.0 unx     1090 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/derivative_computer/base.py
--rw-r--r--  2.0 unx     2675 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/derivative_computer/forth_order_central_derivative_computer.py
--rw-r--r--  2.0 unx     2624 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/derivative_computer/forth_order_face_derivative_computer.py
--rw-r--r--  2.0 unx     1142 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/interpolator/__init__.py
--rw-r--r--  2.0 unx     1031 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/interpolator/base.py
--rw-r--r--  2.0 unx     2576 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/interpolator/central_forth_order_interpolator.py
--rw-r--r--  2.0 unx     1045 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/reconstructor/__init__.py
--rw-r--r--  2.0 unx     2064 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/reconstructor/base.py
--rw-r--r--  2.0 unx     6315 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/reconstructor/weno5.py
--rw-r--r--  2.0 unx     1114 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/riemann_computer/__init__.py
--rw-r--r--  2.0 unx     1021 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/riemann_computer/base.py
--rw-r--r--  2.0 unx     2374 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/riemann_computer/rusanov.py
--rw-r--r--  2.0 unx     3636 b- defN 23-Jan-31 12:26 mindflow/cfd/space_solver/riemann_computer/rusanov_net.py
--rw-r--r--  2.0 unx     1040 b- defN 23-Jan-31 12:26 mindflow/common/__init__.py
--rw-r--r--  2.0 unx     6210 b- defN 23-Jan-31 12:26 mindflow/common/callback.py
--rw-r--r--  2.0 unx     9966 b- defN 23-Jan-31 12:26 mindflow/common/lr_scheduler.py
--rw-r--r--  2.0 unx     2014 b- defN 23-Jan-31 12:26 mindflow/common/math.py
--rw-r--r--  2.0 unx     3345 b- defN 23-Jan-31 12:26 mindflow/common/metrics.py
--rw-r--r--  2.0 unx     1145 b- defN 23-Jan-31 12:26 mindflow/data/__init__.py
--rw-r--r--  2.0 unx     8430 b- defN 23-Jan-31 12:26 mindflow/data/boundary.py
--rw-r--r--  2.0 unx     5624 b- defN 23-Jan-31 12:26 mindflow/data/data_base.py
--rw-r--r--  2.0 unx    18758 b- defN 23-Jan-31 12:26 mindflow/data/dataset.py
--rw-r--r--  2.0 unx     5436 b- defN 23-Jan-31 12:26 mindflow/data/equation.py
--rw-r--r--  2.0 unx     6960 b- defN 23-Jan-31 12:26 mindflow/data/existed_data.py
--rw-r--r--  2.0 unx    12557 b- defN 23-Jan-31 12:26 mindflow/data/mind_dataset.py
--rw-r--r--  2.0 unx     1542 b- defN 23-Jan-31 12:26 mindflow/geometry/__init__.py
--rw-r--r--  2.0 unx    29673 b- defN 23-Jan-31 12:26 mindflow/geometry/csg.py
--rw-r--r--  2.0 unx     5593 b- defN 23-Jan-31 12:26 mindflow/geometry/geom_utils.py
--rw-r--r--  2.0 unx     2355 b- defN 23-Jan-31 12:26 mindflow/geometry/geometry_1d.py
--rw-r--r--  2.0 unx    15747 b- defN 23-Jan-31 12:26 mindflow/geometry/geometry_2d.py
--rw-r--r--  2.0 unx     9383 b- defN 23-Jan-31 12:26 mindflow/geometry/geometry_3d.py
--rw-r--r--  2.0 unx    11152 b- defN 23-Jan-31 12:26 mindflow/geometry/geometry_base.py
--rw-r--r--  2.0 unx    15730 b- defN 23-Jan-31 12:26 mindflow/geometry/geometry_nd.py
--rw-r--r--  2.0 unx    13857 b- defN 23-Jan-31 12:26 mindflow/geometry/geometry_td.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 12:26 mindflow/geometry/shapes/__init__.py
--rw-r--r--  2.0 unx     2337 b- defN 23-Jan-31 12:26 mindflow/geometry/shapes/adapter.py
--rw-r--r--  2.0 unx     2708 b- defN 23-Jan-31 12:26 mindflow/geometry/shapes/pentagon.py
--rw-r--r--  2.0 unx     7023 b- defN 23-Jan-31 12:26 mindflow/geometry/shapes/rotating.py
--rw-r--r--  2.0 unx     3146 b- defN 23-Jan-31 12:26 mindflow/geometry/shapes/shapes.py
--rw-r--r--  2.0 unx     6579 b- defN 23-Jan-31 12:26 mindflow/geometry/shapes/simplex.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-31 12:26 mindflow/loss/__init__.py
--rw-r--r--  2.0 unx    14254 b- defN 23-Jan-31 12:26 mindflow/loss/losses.py
--rw-r--r--  2.0 unx      804 b- defN 23-Jan-31 12:26 mindflow/operators/__init__.py
--rw-r--r--  2.0 unx     4635 b- defN 23-Jan-31 12:26 mindflow/operators/derivatives.py
--rw-r--r--  2.0 unx      962 b- defN 23-Jan-31 12:26 mindflow/pde/__init__.py
--rw-r--r--  2.0 unx     3049 b- defN 23-Jan-31 12:26 mindflow/pde/burgers.py
--rw-r--r--  2.0 unx     4908 b- defN 23-Jan-31 12:26 mindflow/pde/navier_stokes.py
--rw-r--r--  2.0 unx     2898 b- defN 23-Jan-31 12:26 mindflow/pde/poisson.py
--rw-r--r--  2.0 unx     7208 b- defN 23-Jan-31 12:26 mindflow/pde/sympy_pde.py
--rw-r--r--  2.0 unx      788 b- defN 23-Jan-31 12:26 mindflow/pde/sympy2mindspore/__init__.py
--rw-r--r--  2.0 unx     3087 b- defN 23-Jan-31 12:26 mindflow/pde/sympy2mindspore/parse_sympy.py
--rw-r--r--  2.0 unx     6055 b- defN 23-Jan-31 12:26 mindflow/pde/sympy2mindspore/pde_node.py
--rw-r--r--  2.0 unx     7047 b- defN 23-Jan-31 12:26 mindflow/pde/sympy2mindspore/sympy_translation.py
--rw-r--r--  2.0 unx      727 b- defN 23-Jan-31 12:26 mindflow/solver/__init__.py
--rw-r--r--  2.0 unx    13909 b- defN 23-Jan-31 12:26 mindflow/solver/solver.py
--rw-r--r--  2.0 unx      773 b- defN 23-Jan-31 12:26 mindflow/utils/__init__.py
--rw-r--r--  2.0 unx     5419 b- defN 23-Jan-31 12:26 mindflow/utils/check_func.py
--rw-r--r--  2.0 unx     1927 b- defN 23-Jan-31 12:26 mindflow/utils/load_config.py
--rw-r--r--  2.0 unx      690 b- defN 23-Jan-31 12:27 mindflow_gpu-0.1.0a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-31 12:27 mindflow_gpu-0.1.0a0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jan-31 12:27 mindflow_gpu-0.1.0a0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     9393 b- defN 23-Jan-31 12:27 mindflow_gpu-0.1.0a0.dist-info/RECORD
-102 files, 480511 bytes uncompressed, 138771 bytes compressed:  71.1%
+Zip file size: 144569 bytes, number of entries: 96
+-rw-r--r--  2.0 unx     2948 b- defN 23-Apr-04 12:21 mindflow/__init__.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Apr-04 12:21 mindflow/setup.py
+-rw-r--r--  2.0 unx     1012 b- defN 23-Apr-04 12:21 mindflow/cell/__init__.py
+-rw-r--r--  2.0 unx     3492 b- defN 23-Apr-04 12:21 mindflow/cell/activation.py
+-rw-r--r--  2.0 unx    21416 b- defN 23-Apr-04 12:21 mindflow/cell/basic_block.py
+-rw-r--r--  2.0 unx     5040 b- defN 23-Apr-04 12:21 mindflow/cell/utils.py
+-rw-r--r--  2.0 unx      811 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/__init__.py
+-rw-r--r--  2.0 unx    14413 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/dft.py
+-rw-r--r--  2.0 unx     7688 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/fno1d.py
+-rw-r--r--  2.0 unx     9511 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/fno2d.py
+-rw-r--r--  2.0 unx     2357 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/m2k.py
+-rw-r--r--  2.0 unx     9671 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/pdenet.py
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-04 12:21 mindflow/cell/transformer/__init__.py
+-rw-r--r--  2.0 unx    14042 b- defN 23-Apr-04 12:21 mindflow/cell/transformer/layer.py
+-rw-r--r--  2.0 unx     6350 b- defN 23-Apr-04 12:21 mindflow/cell/transformer/vit.py
+-rw-r--r--  2.0 unx      971 b- defN 23-Apr-04 12:21 mindflow/cfd/__init__.py
+-rw-r--r--  2.0 unx     2531 b- defN 23-Apr-04 12:21 mindflow/cfd/mesh_info.py
+-rw-r--r--  2.0 unx     4168 b- defN 23-Apr-04 12:21 mindflow/cfd/runtime.py
+-rw-r--r--  2.0 unx     3298 b- defN 23-Apr-04 12:21 mindflow/cfd/simulator.py
+-rw-r--r--  2.0 unx     4714 b- defN 23-Apr-04 12:21 mindflow/cfd/utils.py
+-rw-r--r--  2.0 unx     2956 b- defN 23-Apr-04 12:21 mindflow/cfd/visualization.py
+-rw-r--r--  2.0 unx      749 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/__init__.py
+-rw-r--r--  2.0 unx     1165 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/base.py
+-rw-r--r--  2.0 unx     2752 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/boundary_manager.py
+-rw-r--r--  2.0 unx     1247 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/neumann.py
+-rw-r--r--  2.0 unx     1173 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/periodic.py
+-rw-r--r--  2.0 unx     1319 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/symmetry.py
+-rw-r--r--  2.0 unx     1836 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/wall.py
+-rw-r--r--  2.0 unx     1119 b- defN 23-Apr-04 12:21 mindflow/cfd/integrator/__init__.py
+-rw-r--r--  2.0 unx      935 b- defN 23-Apr-04 12:21 mindflow/cfd/integrator/base.py
+-rw-r--r--  2.0 unx     1056 b- defN 23-Apr-04 12:21 mindflow/cfd/integrator/euler.py
+-rw-r--r--  2.0 unx     1307 b- defN 23-Apr-04 12:21 mindflow/cfd/integrator/runge_kutta3.py
+-rw-r--r--  2.0 unx     1054 b- defN 23-Apr-04 12:21 mindflow/cfd/material/__init__.py
+-rw-r--r--  2.0 unx     2685 b- defN 23-Apr-04 12:21 mindflow/cfd/material/base.py
+-rw-r--r--  2.0 unx     1897 b- defN 23-Apr-04 12:21 mindflow/cfd/material/ideal_gas.py
+-rw-r--r--  2.0 unx      735 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/__init__.py
+-rw-r--r--  2.0 unx     1812 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/godunov_flux.py
+-rw-r--r--  2.0 unx     2982 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/space_solver.py
+-rw-r--r--  2.0 unx     6133 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/viscous_flux.py
+-rw-r--r--  2.0 unx     1348 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/derivative_computer/__init__.py
+-rw-r--r--  2.0 unx     1090 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/derivative_computer/base.py
+-rw-r--r--  2.0 unx     2675 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/derivative_computer/forth_order_central_derivative_computer.py
+-rw-r--r--  2.0 unx     2624 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/derivative_computer/forth_order_face_derivative_computer.py
+-rw-r--r--  2.0 unx     1142 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/interpolator/__init__.py
+-rw-r--r--  2.0 unx     1031 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/interpolator/base.py
+-rw-r--r--  2.0 unx     2576 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/interpolator/central_forth_order_interpolator.py
+-rw-r--r--  2.0 unx     1045 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/reconstructor/__init__.py
+-rw-r--r--  2.0 unx     2064 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/reconstructor/base.py
+-rw-r--r--  2.0 unx     6315 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/reconstructor/weno5.py
+-rw-r--r--  2.0 unx     1114 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/riemann_computer/__init__.py
+-rw-r--r--  2.0 unx     1021 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/riemann_computer/base.py
+-rw-r--r--  2.0 unx     2374 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/riemann_computer/rusanov.py
+-rw-r--r--  2.0 unx     3636 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/riemann_computer/rusanov_net.py
+-rw-r--r--  2.0 unx      884 b- defN 23-Apr-04 12:21 mindflow/common/__init__.py
+-rw-r--r--  2.0 unx     9966 b- defN 23-Apr-04 12:21 mindflow/common/lr_scheduler.py
+-rw-r--r--  2.0 unx     2014 b- defN 23-Apr-04 12:21 mindflow/common/math.py
+-rw-r--r--  2.0 unx     1145 b- defN 23-Apr-04 12:21 mindflow/data/__init__.py
+-rw-r--r--  2.0 unx     8430 b- defN 23-Apr-04 12:21 mindflow/data/boundary.py
+-rw-r--r--  2.0 unx     5624 b- defN 23-Apr-04 12:21 mindflow/data/data_base.py
+-rw-r--r--  2.0 unx    18758 b- defN 23-Apr-04 12:21 mindflow/data/dataset.py
+-rw-r--r--  2.0 unx     5436 b- defN 23-Apr-04 12:21 mindflow/data/equation.py
+-rw-r--r--  2.0 unx     6960 b- defN 23-Apr-04 12:21 mindflow/data/existed_data.py
+-rw-r--r--  2.0 unx    12556 b- defN 23-Apr-04 12:21 mindflow/data/mind_dataset.py
+-rw-r--r--  2.0 unx     1542 b- defN 23-Apr-04 12:21 mindflow/geometry/__init__.py
+-rw-r--r--  2.0 unx    29673 b- defN 23-Apr-04 12:21 mindflow/geometry/csg.py
+-rw-r--r--  2.0 unx     5593 b- defN 23-Apr-04 12:21 mindflow/geometry/geom_utils.py
+-rw-r--r--  2.0 unx     2355 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_1d.py
+-rw-r--r--  2.0 unx    15747 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_2d.py
+-rw-r--r--  2.0 unx     9383 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_3d.py
+-rw-r--r--  2.0 unx    11153 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_base.py
+-rw-r--r--  2.0 unx    15732 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_nd.py
+-rw-r--r--  2.0 unx    13857 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_td.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/__init__.py
+-rw-r--r--  2.0 unx     2337 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/adapter.py
+-rw-r--r--  2.0 unx     2708 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/pentagon.py
+-rw-r--r--  2.0 unx     7023 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/rotating.py
+-rw-r--r--  2.0 unx     3146 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/shapes.py
+-rw-r--r--  2.0 unx     6579 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/simplex.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Apr-04 12:21 mindflow/loss/__init__.py
+-rw-r--r--  2.0 unx    14215 b- defN 23-Apr-04 12:21 mindflow/loss/losses.py
+-rw-r--r--  2.0 unx      804 b- defN 23-Apr-04 12:21 mindflow/operators/__init__.py
+-rw-r--r--  2.0 unx     4635 b- defN 23-Apr-04 12:21 mindflow/operators/derivatives.py
+-rw-r--r--  2.0 unx     1056 b- defN 23-Apr-04 12:21 mindflow/pde/__init__.py
+-rw-r--r--  2.0 unx     8517 b- defN 23-Apr-04 12:21 mindflow/pde/flow_with_loss.py
+-rw-r--r--  2.0 unx    15750 b- defN 23-Apr-04 12:21 mindflow/pde/pde_with_loss.py
+-rw-r--r--  2.0 unx      788 b- defN 23-Apr-04 12:21 mindflow/pde/sympy2mindspore/__init__.py
+-rw-r--r--  2.0 unx     3087 b- defN 23-Apr-04 12:21 mindflow/pde/sympy2mindspore/parse_sympy.py
+-rw-r--r--  2.0 unx     6012 b- defN 23-Apr-04 12:21 mindflow/pde/sympy2mindspore/pde_node.py
+-rw-r--r--  2.0 unx     7047 b- defN 23-Apr-04 12:21 mindflow/pde/sympy2mindspore/sympy_translation.py
+-rw-r--r--  2.0 unx      773 b- defN 23-Apr-04 12:21 mindflow/utils/__init__.py
+-rw-r--r--  2.0 unx     5419 b- defN 23-Apr-04 12:21 mindflow/utils/check_func.py
+-rw-r--r--  2.0 unx     1898 b- defN 23-Apr-04 12:21 mindflow/utils/load_config.py
+-rw-r--r--  2.0 unx      691 b- defN 23-Apr-04 12:21 mindflow_gpu-0.1.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-04 12:21 mindflow_gpu-0.1.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-04 12:21 mindflow_gpu-0.1.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     8909 b- defN 23-Apr-04 12:21 mindflow_gpu-0.1.0rc1.dist-info/RECORD
+96 files, 461567 bytes uncompressed, 130253 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -156,26 +156,20 @@
 
 Filename: mindflow/cfd/space_solver/riemann_computer/rusanov_net.py
 Comment: 
 
 Filename: mindflow/common/__init__.py
 Comment: 
 
-Filename: mindflow/common/callback.py
-Comment: 
-
 Filename: mindflow/common/lr_scheduler.py
 Comment: 
 
 Filename: mindflow/common/math.py
 Comment: 
 
-Filename: mindflow/common/metrics.py
-Comment: 
-
 Filename: mindflow/data/__init__.py
 Comment: 
 
 Filename: mindflow/data/boundary.py
 Comment: 
 
 Filename: mindflow/data/data_base.py
@@ -249,59 +243,47 @@
 
 Filename: mindflow/operators/derivatives.py
 Comment: 
 
 Filename: mindflow/pde/__init__.py
 Comment: 
 
-Filename: mindflow/pde/burgers.py
-Comment: 
-
-Filename: mindflow/pde/navier_stokes.py
+Filename: mindflow/pde/flow_with_loss.py
 Comment: 
 
-Filename: mindflow/pde/poisson.py
-Comment: 
-
-Filename: mindflow/pde/sympy_pde.py
+Filename: mindflow/pde/pde_with_loss.py
 Comment: 
 
 Filename: mindflow/pde/sympy2mindspore/__init__.py
 Comment: 
 
 Filename: mindflow/pde/sympy2mindspore/parse_sympy.py
 Comment: 
 
 Filename: mindflow/pde/sympy2mindspore/pde_node.py
 Comment: 
 
 Filename: mindflow/pde/sympy2mindspore/sympy_translation.py
 Comment: 
 
-Filename: mindflow/solver/__init__.py
-Comment: 
-
-Filename: mindflow/solver/solver.py
-Comment: 
-
 Filename: mindflow/utils/__init__.py
 Comment: 
 
 Filename: mindflow/utils/check_func.py
 Comment: 
 
 Filename: mindflow/utils/load_config.py
 Comment: 
 
-Filename: mindflow_gpu-0.1.0a0.dist-info/METADATA
+Filename: mindflow_gpu-0.1.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: mindflow_gpu-0.1.0a0.dist-info/WHEEL
+Filename: mindflow_gpu-0.1.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: mindflow_gpu-0.1.0a0.dist-info/top_level.txt
+Filename: mindflow_gpu-0.1.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: mindflow_gpu-0.1.0a0.dist-info/RECORD
+Filename: mindflow_gpu-0.1.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mindflow/__init__.py

```diff
@@ -13,34 +13,14 @@
 # limitations under the License.
 # ============================================================================
 """
 init
 """
 import re
 import time
-from .data import *
-from .geometry import *
-from .common import *
-from .operators import *
-from .pde import *
-from .loss import *
-from .solver import *
-from .cell import *
-from .utils import *
-
-__all__ = []
-__all__.extend(data.__all__)
-__all__.extend(geometry.__all__)
-__all__.extend(common.__all__)
-__all__.extend(operators.__all__)
-__all__.extend(pde.__all__)
-__all__.extend(loss.__all__)
-__all__.extend(solver.__all__)
-__all__.extend(cell.__all__)
-__all__.extend(utils.__all__)
 
 
 def _mindspore_version_check():
     """
        Do the MindSpore version check for MindFlow. If the
        MindSpore can not be imported, it will raise ImportError. If its
        version is not compatibale with current MindFlow verision,
@@ -54,17 +34,17 @@
         import mindspore as ms
         from mindspore import log as logger
     except ImportError:
         raise ImportError("Can not find MindSpore in current environment. Please install "
                           "MindSpore before using MindFlow, by following "
                           "the instruction at https://www.mindspore.cn/install")
 
-    pattern = r'\d+\.\d+\.\d+\w\d+'
+    pattern = r'\d+\.\d+\.\d+'
     ms_version = re.match(pattern, ms.__version__)
-    required_mindspore_version = '2.0.0a0'
+    required_mindspore_version = '2.0.0'
 
     logger.info("Current Mindspore version is {}.".format(ms_version))
 
     if not ms_version or ms_version.group() < required_mindspore_version:
         logger.warning("Current version of MindSpore is not compatible with MindFlow. "
                        "Some functions might not work or even raise error. Please install MindSpore "
                        "version >= {} For more details about dependency setting, please check "
@@ -75,7 +55,28 @@
         for i in range(warning_countdown, 0, -1):
             logger.warning(
                 f"Please pay attention to the above warning, countdown: {i}")
             time.sleep(1)
 
 
 _mindspore_version_check()
+
+from .data import *
+from .geometry import *
+from .common import *
+from .operators import *
+from .pde import *
+from .loss import *
+from .cell import *
+from .cfd import *
+from .utils import *
+
+__all__ = []
+__all__.extend(data.__all__)
+__all__.extend(geometry.__all__)
+__all__.extend(common.__all__)
+__all__.extend(operators.__all__)
+__all__.extend(pde.__all__)
+__all__.extend(loss.__all__)
+__all__.extend(cell.__all__)
+__all__.extend(cfd.__all__)
+__all__.extend(utils.__all__)
```

## mindflow/cell/__init__.py

```diff
@@ -10,14 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """init"""
 from .activation import get_activation
-from .basic_block import LinearBlock, ResBlock, InputScaleNet, FCSequential, MultiScaleFCCell
+from .basic_block import LinearBlock, ResBlock, InputScale, FCSequential, MultiScaleFCSequential
 from .neural_operators import FNO1D, FNO2D, PDENet
 from .transformer import ViT
 
 __all__ = ['FNO1D', 'FNO2D', 'ViT', 'PDENet']
 __all__.extend(activation.__all__)
 __all__.extend(basic_block.__all__)
```

## mindflow/cell/basic_block.py

```diff
@@ -23,16 +23,16 @@
 import mindspore.common.dtype as mstype
 from mindspore import Tensor, Parameter
 from mindspore.ops.primitive import constexpr
 
 from .activation import get_activation
 from ..utils.check_func import check_param_type
 
-__all__ = ['LinearBlock', 'ResBlock', 'InputScaleNet',
-           'FCSequential', 'MultiScaleFCCell']
+__all__ = ['LinearBlock', 'ResBlock', 'InputScale',
+           'FCSequential', 'MultiScaleFCSequential']
 
 
 @constexpr
 def _check_dense_input_shape(x, prim_name=None):
     msg_prefix = f"For '{prim_name}', the" if prim_name else "The"
     if len(x) < 2:
         raise ValueError(
@@ -61,15 +61,15 @@
         Tensor of shape :math:`(*, out\_channels)`.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
-        >>> from mindelec.architecture import LinearBlock
+        >>> from mindflow.cell import LinearBlock
         >>> from mindspore import Tensor
         >>> input = Tensor(np.array([[180, 234, 154], [244, 48, 247]], np.float32))
         >>> net = LinearBlock(3, 4)
         >>> output = net(input)
         >>> print(output.shape)
         (2, 4)
 
@@ -156,16 +156,15 @@
                              "out_channels: {}".format(in_channels, out_channels))
         self.dense = LinearBlock(in_channels,
                                  out_channels,
                                  weight_init=weight_init,
                                  bias_init=bias_init,
                                  has_bias=has_bias,
                                  activation=None)
-        self.activation = get_activation(activation) if isinstance(
-            activation, str) else activation
+        self.activation = get_activation(activation) if isinstance(activation, str) else activation
         if activation is not None and not isinstance(self.activation, (nn.Cell, ops.Primitive)):
             raise TypeError(
                 "The activation must be str or Cell or Primitive,"" but got {}.".format(type(activation)))
         if not activation:
             self.activation = ops.Identity()
 
     def construct(self, x):
@@ -176,15 +175,15 @@
 def _bias_init(fan_in, fan_out):
     """initializer function for bias"""
     bound = 1 / math.sqrt(fan_in) if fan_in > 0 else 0
     out = np.random.uniform(-bound, bound, fan_out)
     return Tensor(out, mstype.float32)
 
 
-class InputScaleNet(nn.Cell):
+class InputScale(nn.Cell):
     r"""
     Scale the input value to specified region.
 
     Args:
         input_scale (list): The scale factor of input x/y/t.
         input_center (Union[list, None]): Center position of coordinate translation. Default: None.
 
@@ -199,29 +198,29 @@
         TypeError: If `input_center` is not a list or None.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
-        >>> from mindflow.cell import InputScaleNet
+        >>> from mindflow.cell import InputScale
         >>> from mindspore import Tensor
         >>> inputs = np.random.uniform(size=(16, 3)) + 3.0
         >>> inputs = Tensor(inputs.astype(np.float32))
         >>> input_scale = [1.0, 2.0, 4.0]
         >>> input_center = [3.5, 3.5, 3.5]
-        >>> net = InputScaleNet(input_scale, input_center)
+        >>> net = InputScale(input_scale, input_center)
         >>> output = net(inputs).asnumpy()
         >>> assert np.all(output[:, 0] <= 0.5) and np.all(output[:, 0] >= -0.5)
         >>> assert np.all(output[:, 1] <= 1.0) and np.all(output[:, 0] >= -1.0)
         >>> assert np.all(output[:, 2] <= 2.0) and np.all(output[:, 0] >= -2.0)
     """
 
     def __init__(self, input_scale, input_center=None):
-        super(InputScaleNet, self).__init__()
+        super(InputScale, self).__init__()
         check_param_type(input_scale, "input_scale", data_type=list)
         check_param_type(input_center, "input_center",
                          data_type=(type(None), list))
         input_scale = np.array(input_scale)
         self.input_scale = Tensor(input_scale, mstype.float32)
         if input_center is None:
             self.input_center = Tensor(
@@ -358,17 +357,17 @@
         for _ in range(self.layers - 2):
             if self.residual:
                 self._add_res_block(in_channels, out_channels, weight_init)
             else:
                 self._add_linear_block(in_channels, out_channels, weight_init)
 
 
-class MultiScaleFCCell(nn.Cell):
+class MultiScaleFCSequential(nn.Cell):
     r"""
-    The multi-scale network.
+    The multi-scale fully conneted network.
 
     Args:
         in_channels (int): The number of channels in the input space.
         out_channels (int): The number of channels in the output space.
         layers (int): The total number of layers, include input/hidden/output layers.
         neurons (int): The number of neurons of hidden layers.
         residual (bool): full-connected of residual block for the hidden layers. Default: True.
@@ -403,25 +402,25 @@
         TypeError: If `latent_vector` is neither a Parameter nor None.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
-        >>> from mindflow.cell import MultiScaleFCCell
+        >>> from mindflow.cell import MultiScaleFCSequential
         >>> from mindspore import Tensor, Parameter
         >>> inputs = np.ones((64,3)) + 3.0
         >>> inputs = Tensor(inputs.astype(np.float32))
         >>> num_scenarios = 4
         >>> latent_size = 16
         >>> latent_init = np.ones((num_scenarios, latent_size)).astype(np.float32)
         >>> latent_vector = Parameter(Tensor(latent_init), requires_grad=True)
         >>> input_scale = [1.0, 2.0, 4.0]
         >>> input_center = [3.5, 3.5, 3.5]
-        >>> net = MultiScaleFCCell(3, 3, 5, 32,
+        >>> net = MultiScaleFCSequential(3, 3, 5, 32,
         ...                        weight_init="ones", bias_init="zeros",
         ...                        input_scale=input_scale, input_center=input_center, latent_vector=latent_vector)
         >>> output = net(inputs).asnumpy()
         >>> print(output.shape)
         (64, 3)
     """
 
@@ -439,15 +438,15 @@
                  num_scales=4,
                  amp_factor=1.0,
                  scale_factor=2.0,
                  input_scale=None,
                  input_center=None,
                  latent_vector=None
                  ):
-        super(MultiScaleFCCell, self).__init__()
+        super(MultiScaleFCSequential, self).__init__()
         check_param_type(num_scales, "num_scales",
                          data_type=int, exclude_type=bool)
         check_param_type(amp_factor, "amp_factor",
                          data_type=(int, float), exclude_type=bool)
         check_param_type(scale_factor, "scale_factor",
                          data_type=(int, float), exclude_type=bool)
 
@@ -475,15 +474,15 @@
                                                residual=residual,
                                                act=act,
                                                weight_init=weight_init,
                                                has_bias=has_bias,
                                                bias_init=bias_init,
                                                ))
         if input_scale is not None:
-            self.input_scale = InputScaleNet(input_scale, input_center)
+            self.input_scale = InputScale(input_scale, input_center)
         else:
             self.input_scale = ops.Identity()
 
         self.cast = ops.Cast()
         self.concat = ops.Concat(axis=1)
 
     def construct(self, x):
```

## mindflow/cell/neural_operators/fno1d.py

```diff
@@ -57,27 +57,27 @@
 
         w_re = P.Cast()(self.w_re, self.compute_dtype)
         w_im = P.Cast()(self.w_im, self.compute_dtype)
         out_ft_re = \
             self.mul1d(x_ft_re[:, :, :self.modes1], w_re) \
             - self.mul1d(x_ft_im[:, :, :self.modes1], w_im)
         out_ft_im = \
-            self.mul1d(x_ft_re[:, :, :self.modes1], w_re) \
-            + self.mul1d(x_ft_im[:, :, :self.modes1], w_im)
+            self.mul1d(x_ft_re[:, :, :self.modes1], w_im) \
+            + self.mul1d(x_ft_im[:, :, :self.modes1], w_re)
 
         x, _ = self.idft1_cell((out_ft_re, out_ft_im))
         return x
 
 
 class FNOBlock(nn.Cell):
     def __init__(self, in_channels, out_channels, modes1, resolution=1024, gelu=True, compute_dtype=mstype.float32):
         super().__init__()
         self.conv = SpectralConv1dDft(in_channels, out_channels, modes1, resolution, compute_dtype=compute_dtype)
         self.w = nn.Conv1d(in_channels, out_channels, 1).to_float(compute_dtype)
-
+        self.act = None
         if gelu:
             self.act = ops.GeLU()
         else:
             self.act = ops.Identity()
 
     def construct(self, x):
         return self.act(self.conv(x) + self.w(x)) + x
@@ -161,15 +161,16 @@
         self.layers = depths
 
         self.fno_seq = nn.SequentialCell()
         for _ in range(self.layers - 1):
             self.fno_seq.append(FNOBlock(self.channels, self.channels, modes1=self.modes1, resolution=resolution,
                                          compute_dtype=compute_dtype))
         self.fno_seq.append(
-            FNOBlock(self.channels, self.channels, self.modes1, gelu=False, compute_dtype=compute_dtype))
+            FNOBlock(self.channels, self.channels, self.modes1, resolution=resolution,
+                     gelu=False, compute_dtype=compute_dtype))
 
         self.fc1 = nn.Dense(
             self.channels, self.fc_channel).to_float(compute_dtype)
         self.fc2 = nn.Dense(
             self.fc_channel, out_channels).to_float(compute_dtype)
 
         self.grid = Tensor(get_grid_1d(resolution), dtype=mstype.float32)
```

## mindflow/cell/neural_operators/pdenet.py

```diff
@@ -50,30 +50,29 @@
 
     Args:
         height (int): The height number of the input and output tensor of the PDE-Net.
         width (int): The width number of the input and output tensor of the PDE-Net.
         channels (int): The channel number of the input and output tensor of the PDE-Net.
         kernel_size (int): Specifies the height and width of the 2D convolution kernel.
         max_order (int): The max order of the PDE models.
-        step (int): The number of the delta-T blocks used in PDE-Net.
         dx (float): The spatial resolution of x dimension. Default: 0.01.
         dy (float): The spatial resolution of y dimension. Default: 0.01.
         dt (float): The time step of the PDE-Net. Default: 0.01.
         periodic (bool): Specifies whether periodic pad is used with convolution kernels. Default: True.
         enable_moment (bool): Specifies whether the convolution kernels are constrained by moments. Default: True.
         if_fronzen (bool): Specifies whether the moment is frozen. Default: False.
 
     Inputs:
         - **input** (Tensor) - Tensor of shape :math:`(batch\_size, channels, height, width)`.
 
     Outputs:
         Tensor, has the same shape as `input` with data type of float32.
 
     Raises:
-        TypeError: If `height`, `width`, `channels`, `kernel_size`, `max_order` or `step` is not an int.
+        TypeError: If `height`, `width`, `channels`, `kernel_size` or `max_order` is not an int.
         TypeError: If `periodic`, `enable_moment`, `if_fronzen` is not a bool.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
@@ -89,29 +88,27 @@
 
     def __init__(self,
                  height,
                  width,
                  channels,
                  kernel_size,
                  max_order,
-                 step,
                  dx=0.01,
                  dy=0.01,
                  dt=0.01,
                  periodic=True,
                  enable_moment=True,
                  if_fronzen=False):
         """Initialize PDE-Net."""
         super().__init__()
         check_param_type(height, "height", data_type=int)
         check_param_type(width, "width", data_type=int)
         check_param_type(channels, "channels", data_type=int)
         check_param_type(kernel_size, "kernel_size", data_type=int)
         check_param_type(max_order, "max_order", data_type=int)
-        check_param_type(step, "step", data_type=int)
         check_param_type(periodic, "periodic", data_type=bool)
         check_param_type(enable_moment, "enable_moment", data_type=bool)
         check_param_type(if_fronzen, "if_fronzen", data_type=bool)
         self.in_c = channels
         self.out_c = channels
         self.periodic = periodic
         self.kernel_size = kernel_size
@@ -120,15 +117,14 @@
         self.h = height
         self.w = width
         self.dtype = mstype.float32
         self.num_filter = _count_num_filter(max_order)
         self.dx = dx
         self.dy = dy
         self.enable_moment = enable_moment
-        self.step = step
         self.if_fronzen = if_fronzen
         self.padding = int((self.kernel_size - 1) / 2)
         if self.enable_moment:
             self._init_moment()
         else:
             self.id_conv = nn.Conv2d(self.in_c, self.out_c, kernel_size=self.kernel_size, pad_mode='valid')
             self.fd_conv = nn.Conv2d(self.in_c, self.num_filter - 1, kernel_size=self.kernel_size, pad_mode='valid')
@@ -136,45 +132,39 @@
         self.idx2ij = {}
         if self.periodic:
             self.pad = [self.padding, self.padding, self.padding, self.padding]
             self.padding = 0
         self.coe_param = Parameter(ops.UniformReal(seed=2)((self.num_filter - 1, self.h, self.w)))
 
     def construct(self, x):
-        id_kernel = None
-        fd_kernel = None
-        if self.enable_moment:
-            if self.if_fronzen:
-                cur_moment = self.raw_moment
-            else:
-                cur_moment = self.moment * self.mask + self.raw_moment
-            kernel = []
-            for idx in range(cur_moment.shape[0]):
-                kernel.append(self.m2k(cur_moment[idx]))
-            kernel = ops.Stack()(kernel).astype(self.dtype)
-            kernel = self.scale * kernel
-            id_kernel = kernel[0].reshape((1, 1, self.kernel_size, self.kernel_size))
-            fd_kernel = kernel[1:].reshape((self.num_filter - 1, 1, self.kernel_size, self.kernel_size))
-
-        for _ in range(self.step):
-            x = self._one_step_forward(x, id_kernel, fd_kernel)
-        return x
+        return self._one_step_forward(x)
 
     @property
     def coe(self):
         return self.coe_param
 
-    def _one_step_forward(self, x, id_kernel, fd_kernel):
+    def _one_step_forward(self, x):
         if self.periodic:
             x = self._periodicpad(x)
 
         cast = ops.Cast()
         x = cast(x, self.dtype)
 
         if self.enable_moment:
+            if self.if_fronzen:
+                cur_moment = self.raw_moment
+            else:
+                cur_moment = self.moment * self.mask + self.raw_moment
+            kernel = []
+            for idx in range(cur_moment.shape[0]):
+                kernel.append(self.m2k(cur_moment[idx]))
+            kernel = ops.Stack()(kernel).astype(self.dtype)
+            kernel = self.scale * kernel
+            id_kernel = kernel[0].reshape((1, 1, self.kernel_size, self.kernel_size))
+            fd_kernel = kernel[1:].reshape((self.num_filter - 1, 1, self.kernel_size, self.kernel_size))
             id_conv2d = ops.Conv2D(out_channel=id_kernel.shape[0], kernel_size=self.kernel_size, pad=self.padding)
             fd_conv2d = ops.Conv2D(out_channel=fd_kernel.shape[0], kernel_size=self.kernel_size, pad=self.padding)
             id_out = id_conv2d(x, id_kernel)
             fd_out = fd_conv2d(x, fd_kernel)
         else:
             id_out = self.id_conv(x)
             fd_out = self.fd_conv(x)
@@ -197,15 +187,15 @@
         self.idx2ij = {}
         idx = 0
         for o1 in range(self.max_order + 1):
             for o2 in range(o1 + 1):
                 i = o1 - o2
                 j = o2
                 self.idx2ij[str(idx)] = (i, j,)
-                raw_moment[idx, i, j] = 1
+                raw_moment[idx, j, i] = 1
                 scale[idx] = 1.0 / (self.dx ** i * self.dy ** j)
                 for p in range(i + j + 1):
                     for q in range(i + j + 1):
                         if p + q <= (i + j):
                             mask[idx, p, q] = 0
                 idx += 1
```

## mindflow/common/__init__.py

```diff
@@ -9,18 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """init"""
-from .metrics import L2
 from .lr_scheduler import get_poly_lr, get_multi_step_lr, get_warmup_cosine_annealing_lr
-from .callback import EvalCallback, LossAndTimeMonitor
 
-__all__ = ["L2",
-           "EvalCallback",
-           "LossAndTimeMonitor",
-           "get_poly_lr",
+__all__ = ["get_poly_lr",
            "get_multi_step_lr",
            "get_warmup_cosine_annealing_lr",
            ]
```

## mindflow/data/mind_dataset.py

```diff
@@ -58,15 +58,15 @@
         num_samples (int, optional): The number of samples to be included in the dataset
             (default=None, all samples).
         num_parallel_workers (int, optional): The number of readers (default=None).
 
     Raises:
         ValueError: If dataset_files are not valid or do not exist.
         TypeError: If dataset_name is not string.
-        ValueError: If constraint)_type.lower() not in ["equation", "bc", "ic", "label", "function", "custom"].
+        ValueError: If constraint_type.lower() not in ["equation", "bc", "ic", "label", "function", "custom"].
         RuntimeError: If `num_shards` is specified but `shard_id` is None.
         RuntimeError: If `shard_id` is specified but `num_shards` is None.
         ValueError: If `shard_id` is invalid (< 0 or >= `num_shards`).
 
     Supported Platforms:
         ``Ascend`` ``GPU``
```

## mindflow/geometry/geometry_base.py

```diff
@@ -27,15 +27,15 @@
 
 
 class PartSamplingConfig:
     """
     Definition of partial sampling configuration.
 
     Args:
-        size (Union[int, tuple[int], list[int]): number of sampling points.
+        size (Union[int, tuple[int], list[int]]): number of sampling points.
         random_sampling (bool): Whether randomly sampling points. Default: True.
         sampler (str): method for random sampling. Default: uniform.
         random_merge (bool): Specifies whether randomly merge coordinates of different dimensions. Default: True.
         with_normal (bool): Specifies whether generating the normal vectors of the boundary. Default: False.
         with_sdf (bool): Specifies whether return the sign-distance-function result of the inner domain points.
                          Default: False.
```

## mindflow/geometry/geometry_nd.py

```diff
@@ -24,15 +24,15 @@
 from ..utils.check_func import check_param_type, check_param_type_value
 
 _SPACE = " "
 
 
 class FixedPoint(Geometry):
     r"""
-    Definition of HyperCube object.
+    Definition of fixed point object.
 
     Args:
         name (str): name of the fixed point.
         coord (Union[int, float, tuple, list, numpy.ndarray]): coordinate of the fixed point. if the parameter type is
             tuple or list, the element support tuple[int, int], tuple[float, float], list[int, int], list[float, float].
         dtype (numpy.dtype): Data type of sampled point data type. Default: numpy.float32.
         sampling_config (SamplingConfig): sampling configuration. Default: None.
```

## mindflow/loss/__init__.py

```diff
@@ -9,16 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """init"""
-from .losses import get_loss_metric, WaveletTransformLoss, MTLWeightedLossCell, RelativeRMSELoss
+from .losses import get_loss_metric, WaveletTransformLoss, MTLWeightedLoss, RelativeRMSELoss
 
 __all__ = ['get_loss_metric',
            'WaveletTransformLoss',
-           'MTLWeightedLossCell',
+           'MTLWeightedLoss',
            'RelativeRMSELoss'
            ]
 
 __all__.sort()
```

## mindflow/loss/losses.py

```diff
@@ -148,15 +148,15 @@
 
         Returns:
             Tensor, returns the computed result.
         """
         return losses
 
 
-class MTLWeightedLossCell(WeightedLossCell):
+class MTLWeightedLoss(WeightedLossCell):
     r"""
     Compute the MTL strategy weighted multi-task losses automatically.
     For more information, please refer to `MTL weighted losses <https://arxiv.org/pdf/1805.06334.pdf>`_ .
 
     Args:
         num_losses (int): The number of multi-task losses, should be positive integer.
         bound_param (float): The square addition to weight and regularization when the mere bound
@@ -169,27 +169,27 @@
         Tensor. losses for MTL weighted strategy.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
-        >>> from mindflow.loss import MTLWeightedLossCell
+        >>> from mindflow.loss import MTLWeightedLoss
         >>> import mindspore
         >>> from mindspore import Tensor
-        >>> net = MTLWeightedLossCell(num_losses=2)
+        >>> net = MTLWeightedLoss(num_losses=2)
         >>> input1 = Tensor(1.0, mindspore.float32)
         >>> input2 = Tensor(0.8, mindspore.float32)
         >>> output = net((input1, input2))
         >>> print(output)
         2.2862945
     """
 
     def __init__(self, num_losses, bound_param=0.0):
-        super(MTLWeightedLossCell, self).__init__()
+        super(MTLWeightedLoss, self).__init__()
         check_param_type(num_losses, "num_losses", data_type=int, exclude_type=bool)
         if num_losses <= 0:
             raise ValueError("the value of num_losses should be positive, but got {}".format(num_losses))
         self.num_losses = num_losses
         check_param_type(bound_param, "bound_param", data_type=float)
         self.bounded = bound_param > 1.0e-6
         self.bound_param = bound_param ** 2
@@ -255,20 +255,20 @@
         check_param_type(param=regroup, param_name="regroup", data_type=bool)
         super(WaveletTransformLoss, self).__init__()
         self.abs = P.Abs()
         self.wave_level = wave_level
         self.regroup = regroup
         self.print = P.Print()
         if self.regroup:
-            self.mtl = MTLWeightedLossCell(num_losses=3)
+            self.mtl = MTLWeightedLoss(num_losses=3)
         else:
             if self.wave_level == 1:
-                self.mtl = MTLWeightedLossCell(num_losses=4)
+                self.mtl = MTLWeightedLoss(num_losses=4)
             else:
-                self.mtl = MTLWeightedLossCell(num_losses=self.wave_level + 1)
+                self.mtl = MTLWeightedLoss(num_losses=self.wave_level + 1)
 
     def construct(self, logit, label):
         l1_loss = P.ReduceMean()(self.abs(logit - label))
         logit = unpatchify(logit)
         label = unpatchify(label)
 
         if self.wave_level == 1:
@@ -335,15 +335,15 @@
     root-mean-square error between :math:`x` and :math:`y` element-wise,
     where :math:`x` is the prediction and :math:`y` is the labels.
 
     For simplicity, let :math:`x` and :math:`y` be 1-dimensional Tensor with length :math:`N`,
     the loss of :math:`x` and :math:`y` is given as:
 
     .. math::
-        loss = \sqrt{\frac{\frac{1}{N}\sum_{i=1}^{N}{(x_i-y_i)^2}}{sum_{i=1}^{N}{(y_i)^2}}}
+        loss = \sqrt{\frac{\sum_{i=1}^{N}{(x_i-y_i)^2}}{sum_{i=1}^{N}{(y_i)^2}}}
 
     Args:
         reduction (str): Type of reduction to be applied to loss. The optional values are "mean", "sum", and "none".
             Default: "sum".
 
     Inputs:
         - **prediction** (Tensor) - The prediction value of the network. Tensor of shape :math:`(N, *)` where :math:`*`
```

## mindflow/operators/derivatives.py

```diff
@@ -41,15 +41,15 @@
     Calculate Jacobian matrix of network model.
 
     Args:
         model (mindspore.nn.Cell): a network with the input dimension is in_channels and output dimension is
             out_channels.
 
     Returns:
-        jacobian(Tensor): jacobi of the model. With the input dimension is [batch_size, in_channels], output dimension
+        jacobian(Tensor), jacobi of the model. With the input dimension is [batch_size, in_channels], output dimension
         is [out_channels, batch_size, in_channels].
 
     Note:
         The version of MindSpore should be >= 2.0.0 for using `mindspore.jacrev`.
 
     Supported Platforms:
         ``Ascend`` ``GPU`` ``CPU``
@@ -89,15 +89,15 @@
     Calculate Hessian matrix of network model.
 
     Args:
         model (mindspore.nn.Cell): a network with the input dimension is in_channels and output dimension is
             out_channels.
 
     Returns:
-        hessian(Tensor): hessian of the model. With the input dimension is [batch_size, in_channels], output dimension
+        hessian(Tensor), hessian of the model. With the input dimension is [batch_size, in_channels], output dimension
         is [out_channels, in_channels, batch_size, in_channels].
 
     Note:
         The version of MindSpore should be >= 2.0.0 for using `mindspore.jacrev`.
 
     Supported Platforms:
         ``Ascend`` ``GPU`` ``CPU``
```

## mindflow/pde/__init__.py

```diff
@@ -9,16 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """init"""
-from .burgers import Burgers
-from .navier_stokes import NavierStokes
-from .poisson import Poisson
 from .sympy2mindspore import sympy_to_mindspore
-from .sympy_pde import PDEWithLoss
+from .pde_with_loss import PDEWithLoss, Burgers, NavierStokes, Poisson
+from .flow_with_loss import FlowWithLoss, SteadyFlowWithLoss, UnsteadyFlowWithLoss
 
-__all__ = ["Burgers", "NavierStokes", "Poisson", "sympy_to_mindspore", "PDEWithLoss"]
+__all__ = ["Burgers", "NavierStokes", "Poisson", "sympy_to_mindspore", "PDEWithLoss",
+           "FlowWithLoss", "SteadyFlowWithLoss", "UnsteadyFlowWithLoss"]
 
 __all__.sort()
```

## mindflow/pde/sympy2mindspore/pde_node.py

```diff
@@ -71,15 +71,14 @@
     "And": mnp.logical_and,
     "Or": mnp.logical_or,
     "Not": mnp.logical_not,
     "Xor": mnp.logical_xor,
     "Max": _reduce(mnp.maximum),
     "Min": _reduce(mnp.minimum),
     "Trace": mnp.trace,
-    "Determinant": ops.matrix_determinant,
 }
 
 
 @jit_class
 class AddNode:
     """Compute add terms in sympy expression"""
     def __init__(self, nodes=None):
```

## mindflow/utils/load_config.py

```diff
@@ -56,10 +56,9 @@
 
     Supported Platforms:
         ``Ascend`` ``CPU`` ``GPU``
     """
     # Read YAML experiment definition file
     with open(file_path, 'r') as stream:
         config = yaml.safe_load(stream)
-    config = _make_paths_absolute(os.path.join(
-        os.path.dirname(file_path), ".."), config)
+    config = _make_paths_absolute(os.path.dirname(file_path), config)
     return config
```

## Comparing `mindflow_gpu-0.1.0a0.dist-info/METADATA` & `mindflow_gpu-0.1.0rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow-gpu
-Version: 0.1.0a0
+Version: 0.1.0rc1
 Summary: An AI framework for simulations of fluid dynamics
 Home-page: https://www.mindspore.cn/
 Author: The MindSpore Authors
 Author-email: contact@mindspore.cn
 License: Apache 2.0
 Download-URL: https://gitee.com/mindspore/mindscience/tags
 Project-URL: Sources, https://gitee.com/mindspore/mindscience
```

## Comparing `mindflow_gpu-0.1.0a0.dist-info/RECORD` & `mindflow_gpu-0.1.0rc1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-mindflow/__init__.py,sha256=x9UNVJXoMPUQ9NleRTa1KCEE7hUg7x6DRXGzlAQO8-0,2960
+mindflow/__init__.py,sha256=TXo-tv-1C3XBsTj_5ECkn0dAYkQy6G1w7meEwIfcTyk,2948
 mindflow/setup.py,sha256=gIgiwITWji7gZZ6V-tdkhFOHtRPWM_gUnfNL_C7WHzI,2239
-mindflow/cell/__init__.py,sha256=YFvOOF6wy4PAv-VaOxqydgd1t3j9v_qGHbM7ShMbHos,1009
+mindflow/cell/__init__.py,sha256=BrKWKG3gDg4SN0Ngc5FMTJlaqJ8o_o59eSs0i7HZaS0,1012
 mindflow/cell/activation.py,sha256=6jWLECYhPj5B4bdjjOjJlY-gmEeva8Kwq-XOUS9Hnpw,3492
-mindflow/cell/basic_block.py,sha256=IEi4iUYGTQSwPQoj8t9ptrMCAD_-UqKcsnkJvVLtpQA,21410
+mindflow/cell/basic_block.py,sha256=dJImfLsrQLDsyDCMKhunep7zyqXCi256M7FMSnBRgd0,21416
 mindflow/cell/utils.py,sha256=8oBQoPeE2hr4N9KVFgcsAC4o7Fd1EWwwBAvnqY2YyME,5040
 mindflow/cell/neural_operators/__init__.py,sha256=nIx7bANZjxy4w5fkz04FvA367wG0thcpM6dWDHxpqaU,811
 mindflow/cell/neural_operators/dft.py,sha256=fxTzkpq1NK7vnVSzXGRuLTRsKGD7XZDfZXXPYtnl64o,14413
-mindflow/cell/neural_operators/fno1d.py,sha256=nTmPx-7kGF66iWTwyrq3PU5P5Y1l9Hg68xIesMJH2QE,7621
+mindflow/cell/neural_operators/fno1d.py,sha256=i7CERdnou7ly7YhNNqE-VjWUxTbvNBkZ0B_dPsnxMMs,7688
 mindflow/cell/neural_operators/fno2d.py,sha256=jwaPsCPG_0NlhjMF6o7ro4k4mI1dw7U77JQ6LDZUPHM,9511
 mindflow/cell/neural_operators/m2k.py,sha256=xSGAtK8Ug7FaENq2fzVLEcjPFOP3bSL5kkizDboy7qI,2357
-mindflow/cell/neural_operators/pdenet.py,sha256=8RRqaYa98sKHZ_lxJKUvcPI7mAeMI62RLUNxf2s8ycY,10030
+mindflow/cell/neural_operators/pdenet.py,sha256=ByH1VDTRUyF4e-Y2Jd1QceVS-IDqitTPVsM4p5y7OW8,9671
 mindflow/cell/transformer/__init__.py,sha256=LGRSUi4bn1v8mLdF4_BUIOHo7xAXxybwRw68TFdLoHk,699
 mindflow/cell/transformer/layer.py,sha256=TNjH59BvOI9ZGli8fPWPKxob9HJeC6_9fCqZPrg0xPs,14042
 mindflow/cell/transformer/vit.py,sha256=7kUmbbrv2MXyUO-l2w9PgjFFUb3qjhymc7YkvTcXmz8,6350
 mindflow/cfd/__init__.py,sha256=1axgHkUrFAm9ZaBA-eeKbrSzRuI2JlTcQM8r4OHG1sI,971
 mindflow/cfd/mesh_info.py,sha256=cXkXSY9R53ljIcVLDQI2RyFoYIc7EQlIeMm4G_sdihM,2531
 mindflow/cfd/runtime.py,sha256=XMmg8yuYKed0_TD8BexTn3ndRG5w1sJP2-EqpePIFaw,4168
 mindflow/cfd/simulator.py,sha256=wYvZ3DylFho_839ih1JjuTP1In2yQoWIFM7uifF6F20,3298
@@ -47,56 +47,50 @@
 mindflow/cfd/space_solver/reconstructor/__init__.py,sha256=rsPuoU46unBG2n69tbNNaE6euTOqYFVsh8VybtkQyqE,1045
 mindflow/cfd/space_solver/reconstructor/base.py,sha256=kAjWtFLBfNU6i3flcSSYK-oUm1q3or7aPk4CKTxu72Q,2064
 mindflow/cfd/space_solver/reconstructor/weno5.py,sha256=vb4zG1jkSnURXP0YO8zPOIjsFkelFpWHPwS33sZKPzw,6315
 mindflow/cfd/space_solver/riemann_computer/__init__.py,sha256=YpZX6jeg3QS-lANhtBfH-V62qGkeDPi4wflZlvyyuGc,1114
 mindflow/cfd/space_solver/riemann_computer/base.py,sha256=ECb6fegQdaTWiMmGUctkH-A4E70lY-sWTS2DneSwd-U,1021
 mindflow/cfd/space_solver/riemann_computer/rusanov.py,sha256=iXeSRFDCLUM2ZQugFIwtGsWmOHu4YHfmIYPuiVMoK60,2374
 mindflow/cfd/space_solver/riemann_computer/rusanov_net.py,sha256=1iySNWVTLdeejvsbaVwrkCk4OZuRcM-Zr9Sz91jx_cY,3636
-mindflow/common/__init__.py,sha256=2G5Tpda9_UpP15udViaC_NNF03bL8CN9SmXH1u6txTc,1040
-mindflow/common/callback.py,sha256=N03KrGGGeVwLnxFw_in2e8Lpyw3PSnpfh5Zd34R4AGQ,6210
+mindflow/common/__init__.py,sha256=upo0ynjSiiHktNRoUbU7NZWiqsssowphuGpXGphYWsg,884
 mindflow/common/lr_scheduler.py,sha256=an2oztoguFZGUaWjWCma9K5PqQRlU-k3Lj0Hit9Hvkg,9966
 mindflow/common/math.py,sha256=V1S2Wr-VKsrCgD3FAp9Szax7Yovztd51WHkNNCQFEsw,2014
-mindflow/common/metrics.py,sha256=_U07NJVf4t-X0UbMHnZgirZARysRpR6bwesSjVa2-HI,3345
 mindflow/data/__init__.py,sha256=izQBltxrsBnCWLiRehjnDcbGt4CgtRRe3B3ZH1HCjNk,1145
 mindflow/data/boundary.py,sha256=hOId7ryYGia77FEImGE0FQwcGO-yrLjtZ6dmx_BoEho,8430
 mindflow/data/data_base.py,sha256=jdmNts0djeL2rCf9LhPKxKdvEBrFVf44hE8HXJusZEg,5624
 mindflow/data/dataset.py,sha256=61_FCtrBZck4lWS2RD5d-2qY2h7I1ky4NR_MT_7UnoI,18758
 mindflow/data/equation.py,sha256=PJY3F-mlFowUFf2vB0ETQby7YO5BEOHoYkYhfiUfzq0,5436
 mindflow/data/existed_data.py,sha256=hf34-RugoI6_CT8w1wqAkITz2c2TBGrjofBzF1Ty-LI,6960
-mindflow/data/mind_dataset.py,sha256=nuvHlCts3O6XPPixRV7nyJwmxEWKrmh_0p7gaF_nzn8,12557
+mindflow/data/mind_dataset.py,sha256=R0z0g7SqN2DLgoAiqutrt2SZn0vfaaRQ5EoPBCUEASk,12556
 mindflow/geometry/__init__.py,sha256=TE9Tbh8ZgMqVJXZh_Koy3seBResF_R-S8r_QOIy-s6Q,1542
 mindflow/geometry/csg.py,sha256=k8aP7Q6Vrv2itpkHTXWIAAEHrejNwJI3qjRFPoK_3Uk,29673
 mindflow/geometry/geom_utils.py,sha256=5yjXUC_OZyb1t73W7SuGdJoHRsnShOsqOwD-uT64AVc,5593
 mindflow/geometry/geometry_1d.py,sha256=LD_sKnO8kEYZPKlN7pgSDBR--prwUkjJNWchzJcp7X8,2355
 mindflow/geometry/geometry_2d.py,sha256=SgNw4-gExOT2rifjjRShQzzilXIxbQ5vJzEZek6_QQA,15747
 mindflow/geometry/geometry_3d.py,sha256=TAQorKspveIJLvOC_SNYBTvGhtEbSToqsDyixh7QZdg,9383
-mindflow/geometry/geometry_base.py,sha256=yYMCj0OpUOmsZ-klRGHrbDYQoFx_Ungkf9FIqa44acs,11152
-mindflow/geometry/geometry_nd.py,sha256=D5nBRo92h4OqEWZXxHx3FzyLEtUeIWyKzFnMSb3OXeY,15730
+mindflow/geometry/geometry_base.py,sha256=KrOFoUjT87fGICu2TIJo9kD1VqMgQKyqwBRF48yNer4,11153
+mindflow/geometry/geometry_nd.py,sha256=ESTDzrzAySqrDAVMT1AEqC90bpImq9t8eaqyWm42Zss,15732
 mindflow/geometry/geometry_td.py,sha256=FVsMI0l82r751h1vEEYn_Zxf-INrnJkglYFhCMS1rNU,13857
 mindflow/geometry/shapes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mindflow/geometry/shapes/adapter.py,sha256=mTvKsSX5LEne6NlNN7S-niwagok8sT7l4iAL05f4xtc,2337
 mindflow/geometry/shapes/pentagon.py,sha256=gJPQYiLgFZG3gIMLvC7x1DMAMX5Adpw-KpaDxuMla2s,2708
 mindflow/geometry/shapes/rotating.py,sha256=FGvyxb1zWB-rU5wX5AY89PZ9zGtKzdZvNNH7laFATQc,7023
 mindflow/geometry/shapes/shapes.py,sha256=MW9zwntlaXL1WO9FTzXwm4vVM5Zkvnc1Rrw03z_hQJE,3146
 mindflow/geometry/shapes/simplex.py,sha256=yOz2oV_I3w2K3vxeOSffSWl81DAl07t3WaNit6BtejQ,6579
-mindflow/loss/__init__.py,sha256=wO7zKdWXPTbO4hueqVdI-0Ke9tzvPlP6vYlrExjMGJ0,934
-mindflow/loss/losses.py,sha256=6iTvl_0iDRTPoDdek3JGd5701Kp41SR3yF8lJC569Ec,14254
+mindflow/loss/__init__.py,sha256=Idwts_ZyyrfnW-fO4dKi5OB0tBZwY--eNa6eeCCiwic,926
+mindflow/loss/losses.py,sha256=U46koRQhdssYssWJssR5UxEScrIE84omafg-lew-ips,14215
 mindflow/operators/__init__.py,sha256=hy7KSjr2lYOphcDKWFsRC_dorg-hg1pN0rUU_Sry-P8,804
-mindflow/operators/derivatives.py,sha256=g920Rg3YKGQcX3mbFgRxYWhVFu3lgST4TBEpP7dIhG0,4635
-mindflow/pde/__init__.py,sha256=ohgufMay10feoIGiF6V92wUJlc9rEvmSJJwWTMtMhvI,962
-mindflow/pde/burgers.py,sha256=RXQd5Mz2JvdlpVuCUMVZ4IAwFDJEegpA7MlBjn1edoM,3049
-mindflow/pde/navier_stokes.py,sha256=CdFWpsW2Vm5X1BUoTrozR-sZEW4MqALdNVWOS_foqN4,4908
-mindflow/pde/poisson.py,sha256=AKV1dOkalHiNH5PGxFOK5n9gAeSmPw72LTV31_imU6w,2898
-mindflow/pde/sympy_pde.py,sha256=N0jg0y3Qnap8tkm6oKDwddFGF01KApZ_OM8YKPKJYy0,7208
+mindflow/operators/derivatives.py,sha256=YIdY_7ATiu-yo4AVZEn_V-_-SO_XdO8stxLvqBVOq-8,4635
+mindflow/pde/__init__.py,sha256=YM8P1nzOg0iXeqrzwUO-xNS1xtY9HH2X-X8pEOreKns,1056
+mindflow/pde/flow_with_loss.py,sha256=APeJJ1LuubzU-kFsFuw4cc50mb7MQHKkXjkk7e6daKE,8517
+mindflow/pde/pde_with_loss.py,sha256=ZvqB4DpxbcJMcmYsg3oBBxERFBjMkdG5VjpzR8dQvS8,15750
 mindflow/pde/sympy2mindspore/__init__.py,sha256=5RLE_PvndYTEVJuIlTW1ZTJx3WQt9xqZ5U3RYOtDj2A,788
 mindflow/pde/sympy2mindspore/parse_sympy.py,sha256=fseIp_54XDmuiHbZBAyWiSU0ZbZO_HzhEf6ArLVlkBU,3087
-mindflow/pde/sympy2mindspore/pde_node.py,sha256=PiuG_2jslWtcNlLb8OGHZVoZk6uJzg-m9FLvU0-f0Cc,6055
+mindflow/pde/sympy2mindspore/pde_node.py,sha256=bLhUZDoIPKLq-N6MsxOS0lWEI-xm4PZEecrExeMTsXI,6012
 mindflow/pde/sympy2mindspore/sympy_translation.py,sha256=wihRFY3sCxNbNRukcY22CPkE0W5bjgdv6bfhQZ_IRhc,7047
-mindflow/solver/__init__.py,sha256=zOncrneVbXzpNmCPPnB2Tw8usiTr6dkbCiflm1WQTVw,727
-mindflow/solver/solver.py,sha256=LQnyBmsxwAWvOryGajEVihdrRCi31cmQyRoG0lZAGQM,13909
 mindflow/utils/__init__.py,sha256=wQ4qkN7hAGT7s40JNpARrtnvoUp8EKiDdIgQQBd4uW0,773
 mindflow/utils/check_func.py,sha256=gBOmFPc4hck4HrInrm66pun7PV7F5fSJ0nUgX9DFr88,5419
-mindflow/utils/load_config.py,sha256=rSsnvb8pbGSTuzgliPu-uPyYfJ1I15urSSX1Q8ASnJQ,1927
-mindflow_gpu-0.1.0a0.dist-info/METADATA,sha256=R0d2um3NHm7sb5d_r1tFUxAU21lw3sVle_Os5d5zFP0,690
-mindflow_gpu-0.1.0a0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mindflow_gpu-0.1.0a0.dist-info/top_level.txt,sha256=8LhUMCPy-q-NkiERuIGgzn7NBIZloxP4HLIvF8LZ48E,9
-mindflow_gpu-0.1.0a0.dist-info/RECORD,,
+mindflow/utils/load_config.py,sha256=QYXMkwBv3OJfx5ad3dmrXA91CWDyN6D45zqIBAhJpEc,1898
+mindflow_gpu-0.1.0rc1.dist-info/METADATA,sha256=_x4OycYXTGQSkYcv_6Amj8Ea7DVho9o2vSJigtF_n4s,691
+mindflow_gpu-0.1.0rc1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mindflow_gpu-0.1.0rc1.dist-info/top_level.txt,sha256=8LhUMCPy-q-NkiERuIGgzn7NBIZloxP4HLIvF8LZ48E,9
+mindflow_gpu-0.1.0rc1.dist-info/RECORD,,
```

