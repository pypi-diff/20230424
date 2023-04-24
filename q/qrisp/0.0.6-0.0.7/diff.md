# Comparing `tmp/qrisp-0.0.6.tar.gz` & `tmp/qrisp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrisp-0.0.6.tar", last modified: Tue Sep  6 09:11:15 2022, max compression
+gzip compressed data, was "C:\Users\sea\Desktop\GITLAB\qompiler\qrisp\dist\.tmp-hgypjn36\qrisp-0.0.7.tar", last modified: Mon Apr 24 15:14:45 2023, max compression
```

## Comparing `qrisp-0.0.6.tar` & `qrisp-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,164 @@
-drwxrwxrwx   0        0        0        0 2022-09-06 09:11:15.892315 qrisp-0.0.6/
--rw-rw-rw-   0        0        0     1091 2022-01-29 14:12:08.000000 qrisp-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      697 2022-09-06 09:11:15.893359 qrisp-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      174 2022-01-29 14:11:17.000000 qrisp-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2022-01-29 14:05:17.000000 qrisp-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      633 2022-09-06 09:11:15.894373 qrisp-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1017 2022-09-06 09:11:01.000000 qrisp-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-06 09:11:15.864175 qrisp-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2022-09-06 09:11:15.884269 qrisp-0.0.6/src/qrisp/
--rw-rw-rw-   0        0        0       29 2022-09-06 09:09:32.000000 qrisp-0.0.6/src/qrisp/__init__.py
--rw-rw-rw-   0        0        0       43 2022-04-06 09:43:24.000000 qrisp-0.0.6/src/qrisp/add_one.py
-drwxrwxrwx   0        0        0        0 2022-09-06 09:11:15.890235 qrisp-0.0.6/src/qrisp.egg-info/
--rw-rw-rw-   0        0        0      697 2022-09-06 09:11:15.000000 qrisp-0.0.6/src/qrisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2022-09-06 09:11:15.000000 qrisp-0.0.6/src/qrisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-06 09:11:15.000000 qrisp-0.0.6/src/qrisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-09-06 09:11:15.000000 qrisp-0.0.6/src/qrisp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/
+-rw-rw-rw-   0        0        0    14474 2023-04-24 14:39:30.000000 qrisp-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      640 2023-04-24 15:14:45.000000 qrisp-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2022-05-11 14:39:01.000000 qrisp-0.0.7/README.md
+-rw-rw-rw-   0        0        0      387 2023-04-24 15:14:24.000000 qrisp-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      713 2023-04-24 15:14:45.000000 qrisp-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1477 2023-04-24 15:00:34.000000 qrisp-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/
+-rw-rw-rw-   0        0        0      705 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/arithmetic/
+-rw-rw-rw-   0        0        0    32545 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/SBP_arithmetic.py
+-rw-rw-rw-   0        0        0      703 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/__init__.py
+-rw-rw-rw-   0        0        0     7316 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/comparisons.py
+-rw-rw-rw-   0        0        0     5362 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/incrementation.py
+-rw-rw-rw-   0        0        0    26506 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/matrix_multiplication.py
+-rw-rw-rw-   0        0        0     3293 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/poly_tools.py
+-rw-rw-rw-   0        0        0    11029 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/ripple_carry_adder.py
+-rw-rw-rw-   0        0        0    16515 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/ripple_division.py
+-rw-rw-rw-   0        0        0     1154 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/ripple_mult.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/circuit/
+-rw-rw-rw-   0        0        0      745 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/clbit.py
+-rw-rw-rw-   0        0        0     5927 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/controlled_operations.py
+-rw-rw-rw-   0        0        0     3764 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/instruction.py
+-rw-rw-rw-   0        0        0      504 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/library.py
+-rw-rw-rw-   0        0        0    20068 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/multi_cx.py
+-rw-rw-rw-   0        0        0    28034 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/operation.py
+-rw-rw-rw-   0        0        0    68556 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/quantum_circuit.py
+-rw-rw-rw-   0        0        0     1463 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/qubit.py
+-rw-rw-rw-   0        0        0     5362 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/standard_operations.py
+-rw-rw-rw-   0        0        0     5445 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/transpiler.py
+-rw-rw-rw-   0        0        0     4163 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/transpiler_old.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/core/
+-rw-rw-rw-   0        0        0      774 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/__init__.py
+-rw-rw-rw-   0        0        0    34327 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/compilation.py
+-rw-rw-rw-   0        0        0    38436 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/library.py
+-rw-rw-rw-   0        0        0    33412 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/quantum_array.py
+-rw-rw-rw-   0        0        0     9283 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/quantum_dictionary.py
+-rw-rw-rw-   0        0        0    41602 2023-04-24 14:38:09.000000 qrisp-0.0.7/src/qrisp/core/quantum_session.py
+-rw-rw-rw-   0        0        0    48724 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/quantum_variable.py
+-rw-rw-rw-   0        0        0    13770 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/session_merging_tools.py
+-rw-rw-rw-   0        0        0      641 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/default_backend.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/environments/
+-rw-rw-rw-   0        0        0     6672 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/GMS_environment.py
+-rw-rw-rw-   0        0        0      791 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/__init__.py
+-rw-rw-rw-   0        0        0    11053 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/control_environment.py
+-rw-rw-rw-   0        0        0     5685 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/gate_wrap_environment.py
+-rw-rw-rw-   0        0        0    26529 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/quantum_conditionals.py
+-rw-rw-rw-   0        0        0    15427 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/quantum_environments.py
+-rw-rw-rw-   0        0        0    20105 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/quantum_inversion.py
+-rw-rw-rw-   0        0        0     3996 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/temp_var_environment.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/grover/
+-rw-rw-rw-   0        0        0      451 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/grover/__init__.py
+-rw-rw-rw-   0        0        0    12647 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/grover/grover_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/interface/
+-rw-rw-rw-   0        0        0      672 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/__init__.py
+-rw-rw-rw-   0        0        0     8119 2023-04-24 14:42:14.000000 qrisp-0.0.7/src/qrisp/interface/backends.py
+-rw-rw-rw-   0        0        0    13257 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/circuit_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/
+-rw-rw-rw-   0        0        0      857 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/backend_client.py
+-rw-rw-rw-   0        0        0     3921 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/backend_server.py
+-rw-rw-rw-   0        0        0     1099 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/interface_types.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/
+-rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/__init__.py
+-rw-rw-rw-   0        0        0     3394 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/backend_client.py
+-rw-rw-rw-   0        0        0     5835 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/backend_server.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/
+-rw-rw-rw-   0        0        0    15394 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/BackendService.py
+-rw-rw-rw-   0        0        0      463 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    26149 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0      963 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/interface_types.py
+-rw-rw-rw-   0        0        0     1692 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/iterators/
+-rw-rw-rw-   0        0        0      479 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/iterators/__init__.py
+-rw-rw-rw-   0        0        0     3967 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/iterators/qrange.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/
+-rw-rw-rw-   0        0        0      592 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/__init__.py
+-rw-rw-rw-   0        0        0    19768 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/gray_synthesis.py
+-rw-rw-rw-   0        0        0     2768 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/pprm_synthesis.py
+-rw-rw-rw-   0        0        0    15620 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/truth_tables.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/misc/
+-rw-rw-rw-   0        0        0    17646 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/misc/GMS_tools.py
+-rw-rw-rw-   0        0        0      488 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/misc/__init__.py
+-rw-rw-rw-   0        0        0     4076 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/misc/depth_reduction.py
+-rw-rw-rw-   0        0        0    60365 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/misc/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/qtypes/
+-rw-rw-rw-   0        0        0      607 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/__init__.py
+-rw-rw-rw-   0        0        0     6385 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/quantum_bool.py
+-rw-rw-rw-   0        0        0     2239 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/quantum_char.py
+-rw-rw-rw-   0        0        0    31986 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/quantum_float.py
+-rw-rw-rw-   0        0        0     4976 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/quantum_string.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/quantum_network/
+-rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/
+-rw-rw-rw-   0        0        0      410 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/
+-rw-rw-rw-   0        0        0    52890 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
+-rw-rw-rw-   0        0        0      470 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    21148 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0     1360 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface_connection_example.py
+-rw-rw-rw-   0        0        0    13558 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/qn_client.py
+-rw-rw-rw-   0        0        0     5590 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/qn_server.py
+-rw-rw-rw-   0        0        0     5722 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/qn_simulator_server.py
+-rw-rw-rw-   0        0        0     6907 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/quantum_network_session.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/simulator/
+-rw-rw-rw-   0        0        0      786 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/__init__.py
+-rw-rw-rw-   0        0        0     8518 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/bi_array_helper.py
+-rw-rw-rw-   0        0        0    49714 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/bi_arrays.py
+-rw-rw-rw-   0        0        0    49650 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/bi_arrays_new.py
+-rw-rw-rw-   0        0        0    26922 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/circuit_preprocessing.py
+-rw-rw-rw-   0        0        0    13881 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/circuit_reordering.py
+-rw-rw-rw-   0        0        0     7995 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/impure_quantum_state.py
+-rw-rw-rw-   0        0        0      493 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/numerics_config.py
+-rw-rw-rw-   0        0        0     6077 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/quantum_state.py
+-rw-rw-rw-   0        0        0    13850 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/simulator.py
+-rw-rw-rw-   0        0        0     7462 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/tensor_factor.py
+-rw-rw-rw-   0        0        0    11761 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/unitary_management.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/uncomputation/
+-rw-rw-rw-   0        0        0      549 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/uncomputation/__init__.py
+-rw-rw-rw-   0        0        0     6180 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/uncomputation/type_checker.py
+-rw-rw-rw-   0        0        0     4430 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/uncomputation/uncomputation.py
+-rw-rw-rw-   0        0        0    11617 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/uncomputation/unqomp.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/
+-rw-rw-rw-   0        0        0      640 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5228 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/tests/
+-rw-rw-rw-   0        0        0     1121 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_GMS_environment_example.py
+-rw-rw-rw-   0        0        0     1475 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_GXX_converter_example.py
+-rw-rw-rw-   0        0        0     2190 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_GXX_gates_example.py
+-rw-rw-rw-   0        0        0     3035 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_GZZ_gates_example.py
+-rw-rw-rw-   0        0        0     2476 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_abstract_parameters.py
+-rw-rw-rw-   0        0        0      940 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_array_entry_manipulation.py
+-rw-rw-rw-   0        0        0     4149 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_comparisons.py
+-rw-rw-rw-   0        0        0     3442 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_conditional_environments_example.py
+-rw-rw-rw-   0        0        0     3037 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_controlled_gates.py
+-rw-rw-rw-   0        0        0     4231 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_diagonal_hamiltonian_application.py
+-rw-rw-rw-   0        0        0     1603 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_gray_synthesis_example.py
+-rw-rw-rw-   0        0        0     3848 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_grovers_algorithm.py
+-rw-rw-rw-   0        0        0      675 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_hello_world.py
+-rw-rw-rw-   0        0        0     1693 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_inpl_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     1569 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_interface.py
+-rw-rw-rw-   0        0        0      973 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_loops.py
+-rw-rw-rw-   0        0        0     2058 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     2420 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_mcx.py
+-rw-rw-rw-   0        0        0      670 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_measurement_reduction.py
+-rw-rw-rw-   0        0        0      663 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_outcome_array.py
+-rw-rw-rw-   0        0        0     1894 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_qiskit_backend_client.py
+-rw-rw-rw-   0        0        0      806 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_qompiler.py
+-rw-rw-rw-   0        0        0     3087 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_quantum_arithmetic.py
+-rw-rw-rw-   0        0        0     2912 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_quantum_dictionary.py
+-rw-rw-rw-   0        0        0     1047 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_quantum_division.py
+-rw-rw-rw-   0        0        0     4896 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_quantum_teleportation.py
+-rw-rw-rw-   0        0        0     1236 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_state_preparation.py
+-rw-rw-rw-   0        0        0      958 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_string_test.py
+-rw-rw-rw-   0        0        0     5218 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_uncomputation_example.py
+-rw-rw-rw-   0        0        0     1600 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_unitary_calculation.py
+-rw-rw-rw-   0        0        0     4023 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/tests_doc_examples.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `qrisp-0.0.6/PKG-INFO` & `qrisp-0.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.0.6
-Summary: A small example package
+Version: 0.0.7
+Summary: Qrisp - A high-level programming language for gate-based quantum computers
 Home-page: https://github.com/pypa/sampleproject
 Author: Raphael Seidel
-Author-email: raphael.seidel@fokus.fraunhofer.de
+Author-email: Raphael Seidel <raphael.seidel@fokus.fraunhofer.de>
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Example Package
+# Qrisp
 
-This is a simple example package. You can use
-[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+High-Level quantum programming language
```

### Comparing `qrisp-0.0.6/src/qrisp.egg-info/PKG-INFO` & `qrisp-0.0.7/src/qrisp.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.0.6
-Summary: A small example package
+Version: 0.0.7
+Summary: Qrisp - A high-level programming language for gate-based quantum computers
 Home-page: https://github.com/pypa/sampleproject
 Author: Raphael Seidel
-Author-email: raphael.seidel@fokus.fraunhofer.de
+Author-email: Raphael Seidel <raphael.seidel@fokus.fraunhofer.de>
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Example Package
+# Qrisp
 
-This is a simple example package. You can use
-[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+High-Level quantum programming language
```

