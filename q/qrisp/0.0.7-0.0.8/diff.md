# Comparing `tmp/qrisp-0.0.7.tar.gz` & `tmp/qrisp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\sea\Desktop\GITLAB\qompiler\qrisp\dist\.tmp-hgypjn36\qrisp-0.0.7.tar", last modified: Mon Apr 24 15:14:45 2023, max compression
+gzip compressed data, was "C:\Users\sea\Desktop\GITLAB\qompiler\qrisp\dist\.tmp-368ve71z\qrisp-0.0.8.tar", last modified: Mon Apr 24 15:19:31 2023, max compression
```

## Comparing `qrisp-0.0.7.tar` & `qrisp-0.0.8.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/
--rw-rw-rw-   0        0        0    14474 2023-04-24 14:39:30.000000 qrisp-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      640 2023-04-24 15:14:45.000000 qrisp-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       48 2022-05-11 14:39:01.000000 qrisp-0.0.7/README.md
--rw-rw-rw-   0        0        0      387 2023-04-24 15:14:24.000000 qrisp-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      713 2023-04-24 15:14:45.000000 qrisp-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1477 2023-04-24 15:00:34.000000 qrisp-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/
--rw-rw-rw-   0        0        0      705 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/arithmetic/
--rw-rw-rw-   0        0        0    32545 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/SBP_arithmetic.py
--rw-rw-rw-   0        0        0      703 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/__init__.py
--rw-rw-rw-   0        0        0     7316 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/comparisons.py
--rw-rw-rw-   0        0        0     5362 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/incrementation.py
--rw-rw-rw-   0        0        0    26506 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/matrix_multiplication.py
--rw-rw-rw-   0        0        0     3293 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/poly_tools.py
--rw-rw-rw-   0        0        0    11029 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/ripple_carry_adder.py
--rw-rw-rw-   0        0        0    16515 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/ripple_division.py
--rw-rw-rw-   0        0        0     1154 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/arithmetic/ripple_mult.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/circuit/
--rw-rw-rw-   0        0        0      745 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/__init__.py
--rw-rw-rw-   0        0        0     1227 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/clbit.py
--rw-rw-rw-   0        0        0     5927 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/controlled_operations.py
--rw-rw-rw-   0        0        0     3764 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/instruction.py
--rw-rw-rw-   0        0        0      504 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/library.py
--rw-rw-rw-   0        0        0    20068 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/multi_cx.py
--rw-rw-rw-   0        0        0    28034 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/operation.py
--rw-rw-rw-   0        0        0    68556 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/quantum_circuit.py
--rw-rw-rw-   0        0        0     1463 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/qubit.py
--rw-rw-rw-   0        0        0     5362 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/standard_operations.py
--rw-rw-rw-   0        0        0     5445 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/transpiler.py
--rw-rw-rw-   0        0        0     4163 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/circuit/transpiler_old.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/core/
--rw-rw-rw-   0        0        0      774 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/__init__.py
--rw-rw-rw-   0        0        0    34327 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/compilation.py
--rw-rw-rw-   0        0        0    38436 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/library.py
--rw-rw-rw-   0        0        0    33412 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/quantum_array.py
--rw-rw-rw-   0        0        0     9283 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/quantum_dictionary.py
--rw-rw-rw-   0        0        0    41602 2023-04-24 14:38:09.000000 qrisp-0.0.7/src/qrisp/core/quantum_session.py
--rw-rw-rw-   0        0        0    48724 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/quantum_variable.py
--rw-rw-rw-   0        0        0    13770 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/core/session_merging_tools.py
--rw-rw-rw-   0        0        0      641 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/default_backend.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/environments/
--rw-rw-rw-   0        0        0     6672 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/GMS_environment.py
--rw-rw-rw-   0        0        0      791 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/__init__.py
--rw-rw-rw-   0        0        0    11053 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/control_environment.py
--rw-rw-rw-   0        0        0     5685 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/gate_wrap_environment.py
--rw-rw-rw-   0        0        0    26529 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/quantum_conditionals.py
--rw-rw-rw-   0        0        0    15427 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/quantum_environments.py
--rw-rw-rw-   0        0        0    20105 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/quantum_inversion.py
--rw-rw-rw-   0        0        0     3996 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/environments/temp_var_environment.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/grover/
--rw-rw-rw-   0        0        0      451 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/grover/__init__.py
--rw-rw-rw-   0        0        0    12647 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/grover/grover_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/interface/
--rw-rw-rw-   0        0        0      672 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/__init__.py
--rw-rw-rw-   0        0        0     8119 2023-04-24 14:42:14.000000 qrisp-0.0.7/src/qrisp/interface/backends.py
--rw-rw-rw-   0        0        0    13257 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/circuit_converter.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/
--rw-rw-rw-   0        0        0      857 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/backend_client.py
--rw-rw-rw-   0        0        0     3921 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/backend_server.py
--rw-rw-rw-   0        0        0     1099 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/openapi_interface/interface_types.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/
--rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/__init__.py
--rw-rw-rw-   0        0        0     3394 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/backend_client.py
--rw-rw-rw-   0        0        0     5835 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/backend_server.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/
--rw-rw-rw-   0        0        0    15394 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/BackendService.py
--rw-rw-rw-   0        0        0      463 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/__init__.py
--rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/constants.py
--rw-rw-rw-   0        0        0    26149 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/ttypes.py
--rw-rw-rw-   0        0        0      963 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/interface_types.py
--rw-rw-rw-   0        0        0     1692 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/iterators/
--rw-rw-rw-   0        0        0      479 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/iterators/__init__.py
--rw-rw-rw-   0        0        0     3967 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/iterators/qrange.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/
--rw-rw-rw-   0        0        0      592 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/__init__.py
--rw-rw-rw-   0        0        0    19768 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/gray_synthesis.py
--rw-rw-rw-   0        0        0     2768 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/pprm_synthesis.py
--rw-rw-rw-   0        0        0    15620 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/logic_synthesis/truth_tables.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/misc/
--rw-rw-rw-   0        0        0    17646 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/misc/GMS_tools.py
--rw-rw-rw-   0        0        0      488 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/misc/__init__.py
--rw-rw-rw-   0        0        0     4076 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/misc/depth_reduction.py
--rw-rw-rw-   0        0        0    60365 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/misc/utility.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/qtypes/
--rw-rw-rw-   0        0        0      607 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/__init__.py
--rw-rw-rw-   0        0        0     6385 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/quantum_bool.py
--rw-rw-rw-   0        0        0     2239 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/quantum_char.py
--rw-rw-rw-   0        0        0    31986 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/quantum_float.py
--rw-rw-rw-   0        0        0     4976 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/qtypes/quantum_string.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/quantum_network/
--rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/
--rw-rw-rw-   0        0        0      410 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/
--rw-rw-rw-   0        0        0    52890 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
--rw-rw-rw-   0        0        0      470 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/__init__.py
--rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/constants.py
--rw-rw-rw-   0        0        0    21148 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/ttypes.py
--rw-rw-rw-   0        0        0     1360 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/interface_connection_example.py
--rw-rw-rw-   0        0        0    13558 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/qn_client.py
--rw-rw-rw-   0        0        0     5590 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/qn_server.py
--rw-rw-rw-   0        0        0     5722 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/qn_simulator_server.py
--rw-rw-rw-   0        0        0     6907 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/quantum_network/quantum_network_session.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/simulator/
--rw-rw-rw-   0        0        0      786 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/__init__.py
--rw-rw-rw-   0        0        0     8518 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/bi_array_helper.py
--rw-rw-rw-   0        0        0    49714 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/bi_arrays.py
--rw-rw-rw-   0        0        0    49650 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/bi_arrays_new.py
--rw-rw-rw-   0        0        0    26922 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/circuit_preprocessing.py
--rw-rw-rw-   0        0        0    13881 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/circuit_reordering.py
--rw-rw-rw-   0        0        0     7995 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/impure_quantum_state.py
--rw-rw-rw-   0        0        0      493 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/numerics_config.py
--rw-rw-rw-   0        0        0     6077 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/quantum_state.py
--rw-rw-rw-   0        0        0    13850 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/simulator.py
--rw-rw-rw-   0        0        0     7462 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/tensor_factor.py
--rw-rw-rw-   0        0        0    11761 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/simulator/unitary_management.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp/uncomputation/
--rw-rw-rw-   0        0        0      549 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/uncomputation/__init__.py
--rw-rw-rw-   0        0        0     6180 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/uncomputation/type_checker.py
--rw-rw-rw-   0        0        0     4430 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/uncomputation/uncomputation.py
--rw-rw-rw-   0        0        0    11617 2023-04-24 14:36:50.000000 qrisp-0.0.7/src/qrisp/uncomputation/unqomp.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/
--rw-rw-rw-   0        0        0      640 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5228 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 15:14:45.000000 qrisp-0.0.7/src/qrisp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 15:14:45.000000 qrisp-0.0.7/tests/
--rw-rw-rw-   0        0        0     1121 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_GMS_environment_example.py
--rw-rw-rw-   0        0        0     1475 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_GXX_converter_example.py
--rw-rw-rw-   0        0        0     2190 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_GXX_gates_example.py
--rw-rw-rw-   0        0        0     3035 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_GZZ_gates_example.py
--rw-rw-rw-   0        0        0     2476 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_abstract_parameters.py
--rw-rw-rw-   0        0        0      940 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_array_entry_manipulation.py
--rw-rw-rw-   0        0        0     4149 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_comparisons.py
--rw-rw-rw-   0        0        0     3442 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_conditional_environments_example.py
--rw-rw-rw-   0        0        0     3037 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_controlled_gates.py
--rw-rw-rw-   0        0        0     4231 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_diagonal_hamiltonian_application.py
--rw-rw-rw-   0        0        0     1603 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_gray_synthesis_example.py
--rw-rw-rw-   0        0        0     3848 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_grovers_algorithm.py
--rw-rw-rw-   0        0        0      675 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_hello_world.py
--rw-rw-rw-   0        0        0     1693 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_inpl_matrix_multiplication_example.py
--rw-rw-rw-   0        0        0     1569 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_interface.py
--rw-rw-rw-   0        0        0      973 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_loops.py
--rw-rw-rw-   0        0        0     2058 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_matrix_multiplication_example.py
--rw-rw-rw-   0        0        0     2420 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_mcx.py
--rw-rw-rw-   0        0        0      670 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_measurement_reduction.py
--rw-rw-rw-   0        0        0      663 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_outcome_array.py
--rw-rw-rw-   0        0        0     1894 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_qiskit_backend_client.py
--rw-rw-rw-   0        0        0      806 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_qompiler.py
--rw-rw-rw-   0        0        0     3087 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_quantum_arithmetic.py
--rw-rw-rw-   0        0        0     2912 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_quantum_dictionary.py
--rw-rw-rw-   0        0        0     1047 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_quantum_division.py
--rw-rw-rw-   0        0        0     4896 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_quantum_teleportation.py
--rw-rw-rw-   0        0        0     1236 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_state_preparation.py
--rw-rw-rw-   0        0        0      958 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_string_test.py
--rw-rw-rw-   0        0        0     5218 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_uncomputation_example.py
--rw-rw-rw-   0        0        0     1600 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/test_unitary_calculation.py
--rw-rw-rw-   0        0        0     4023 2023-04-24 14:36:50.000000 qrisp-0.0.7/tests/tests_doc_examples.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/
+-rw-rw-rw-   0        0        0    14474 2023-04-24 14:39:30.000000 qrisp-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      640 2023-04-24 15:19:31.000000 qrisp-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2022-05-11 14:39:01.000000 qrisp-0.0.8/README.md
+-rw-rw-rw-   0        0        0      388 2023-04-24 15:18:58.000000 qrisp-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      713 2023-04-24 15:19:31.000000 qrisp-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1477 2023-04-24 15:00:34.000000 qrisp-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp/
+-rw-rw-rw-   0        0        0      705 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp/arithmetic/
+-rw-rw-rw-   0        0        0    32545 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/arithmetic/SBP_arithmetic.py
+-rw-rw-rw-   0        0        0      703 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/arithmetic/__init__.py
+-rw-rw-rw-   0        0        0     7316 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/arithmetic/comparisons.py
+-rw-rw-rw-   0        0        0     5362 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/arithmetic/incrementation.py
+-rw-rw-rw-   0        0        0    26506 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/arithmetic/matrix_multiplication.py
+-rw-rw-rw-   0        0        0     3293 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/arithmetic/poly_tools.py
+-rw-rw-rw-   0        0        0    11029 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/arithmetic/ripple_carry_adder.py
+-rw-rw-rw-   0        0        0    16515 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/arithmetic/ripple_division.py
+-rw-rw-rw-   0        0        0     1154 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/arithmetic/ripple_mult.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp/circuit/
+-rw-rw-rw-   0        0        0      745 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/clbit.py
+-rw-rw-rw-   0        0        0     5927 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/controlled_operations.py
+-rw-rw-rw-   0        0        0     3764 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/instruction.py
+-rw-rw-rw-   0        0        0      504 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/library.py
+-rw-rw-rw-   0        0        0    20068 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/multi_cx.py
+-rw-rw-rw-   0        0        0    28034 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/operation.py
+-rw-rw-rw-   0        0        0    68556 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/quantum_circuit.py
+-rw-rw-rw-   0        0        0     1463 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/qubit.py
+-rw-rw-rw-   0        0        0     5362 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/standard_operations.py
+-rw-rw-rw-   0        0        0     5445 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/transpiler.py
+-rw-rw-rw-   0        0        0     4163 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/circuit/transpiler_old.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp/core/
+-rw-rw-rw-   0        0        0      774 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/core/__init__.py
+-rw-rw-rw-   0        0        0    34327 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/core/compilation.py
+-rw-rw-rw-   0        0        0    38436 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/core/library.py
+-rw-rw-rw-   0        0        0    33412 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/core/quantum_array.py
+-rw-rw-rw-   0        0        0     9283 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/core/quantum_dictionary.py
+-rw-rw-rw-   0        0        0    41602 2023-04-24 14:38:09.000000 qrisp-0.0.8/src/qrisp/core/quantum_session.py
+-rw-rw-rw-   0        0        0    48724 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/core/quantum_variable.py
+-rw-rw-rw-   0        0        0    13770 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/core/session_merging_tools.py
+-rw-rw-rw-   0        0        0      641 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/default_backend.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp/environments/
+-rw-rw-rw-   0        0        0     6672 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/environments/GMS_environment.py
+-rw-rw-rw-   0        0        0      791 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/environments/__init__.py
+-rw-rw-rw-   0        0        0    11053 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/environments/control_environment.py
+-rw-rw-rw-   0        0        0     5685 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/environments/gate_wrap_environment.py
+-rw-rw-rw-   0        0        0    26529 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/environments/quantum_conditionals.py
+-rw-rw-rw-   0        0        0    15427 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/environments/quantum_environments.py
+-rw-rw-rw-   0        0        0    20105 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/environments/quantum_inversion.py
+-rw-rw-rw-   0        0        0     3996 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/environments/temp_var_environment.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp/grover/
+-rw-rw-rw-   0        0        0      451 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/grover/__init__.py
+-rw-rw-rw-   0        0        0    12647 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/grover/grover_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp/interface/
+-rw-rw-rw-   0        0        0      672 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/__init__.py
+-rw-rw-rw-   0        0        0     8119 2023-04-24 14:42:14.000000 qrisp-0.0.8/src/qrisp/interface/backends.py
+-rw-rw-rw-   0        0        0    13257 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/circuit_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp/interface/openapi_interface/
+-rw-rw-rw-   0        0        0      857 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/openapi_interface/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/openapi_interface/backend_client.py
+-rw-rw-rw-   0        0        0     3921 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/openapi_interface/backend_server.py
+-rw-rw-rw-   0        0        0     1099 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/openapi_interface/interface_types.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/
+-rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/__init__.py
+-rw-rw-rw-   0        0        0     3394 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/backend_client.py
+-rw-rw-rw-   0        0        0     5835 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/backend_server.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/codegen/
+-rw-rw-rw-   0        0        0    15394 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/codegen/BackendService.py
+-rw-rw-rw-   0        0        0      463 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    26149 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0      963 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/interface_types.py
+-rw-rw-rw-   0        0        0     1692 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/iterators/
+-rw-rw-rw-   0        0        0      479 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/iterators/__init__.py
+-rw-rw-rw-   0        0        0     3967 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/iterators/qrange.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/logic_synthesis/
+-rw-rw-rw-   0        0        0      592 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/logic_synthesis/__init__.py
+-rw-rw-rw-   0        0        0    19768 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/logic_synthesis/gray_synthesis.py
+-rw-rw-rw-   0        0        0     2768 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/logic_synthesis/pprm_synthesis.py
+-rw-rw-rw-   0        0        0    15620 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/logic_synthesis/truth_tables.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/misc/
+-rw-rw-rw-   0        0        0    17646 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/misc/GMS_tools.py
+-rw-rw-rw-   0        0        0      488 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/misc/__init__.py
+-rw-rw-rw-   0        0        0     4076 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/misc/depth_reduction.py
+-rw-rw-rw-   0        0        0    60365 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/misc/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/qtypes/
+-rw-rw-rw-   0        0        0      607 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/qtypes/__init__.py
+-rw-rw-rw-   0        0        0     6385 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/qtypes/quantum_bool.py
+-rw-rw-rw-   0        0        0     2239 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/qtypes/quantum_char.py
+-rw-rw-rw-   0        0        0    31986 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/qtypes/quantum_float.py
+-rw-rw-rw-   0        0        0     4976 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/qtypes/quantum_string.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/quantum_network/
+-rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/quantum_network/interface/
+-rw-rw-rw-   0        0        0      410 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/quantum_network/interface/codegen/
+-rw-rw-rw-   0        0        0    52890 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
+-rw-rw-rw-   0        0        0      470 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    21148 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0     1360 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/interface_connection_example.py
+-rw-rw-rw-   0        0        0    13558 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/qn_client.py
+-rw-rw-rw-   0        0        0     5590 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/qn_server.py
+-rw-rw-rw-   0        0        0     5722 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/qn_simulator_server.py
+-rw-rw-rw-   0        0        0     6907 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/quantum_network/quantum_network_session.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/simulator/
+-rw-rw-rw-   0        0        0      786 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/__init__.py
+-rw-rw-rw-   0        0        0     8518 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/bi_array_helper.py
+-rw-rw-rw-   0        0        0    49714 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/bi_arrays.py
+-rw-rw-rw-   0        0        0    49650 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/bi_arrays_new.py
+-rw-rw-rw-   0        0        0    26922 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/circuit_preprocessing.py
+-rw-rw-rw-   0        0        0    13881 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/circuit_reordering.py
+-rw-rw-rw-   0        0        0     7995 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/impure_quantum_state.py
+-rw-rw-rw-   0        0        0      493 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/numerics_config.py
+-rw-rw-rw-   0        0        0     6077 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/quantum_state.py
+-rw-rw-rw-   0        0        0    13850 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/simulator.py
+-rw-rw-rw-   0        0        0     7462 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/tensor_factor.py
+-rw-rw-rw-   0        0        0    11761 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/simulator/unitary_management.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/src/qrisp/uncomputation/
+-rw-rw-rw-   0        0        0      549 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/uncomputation/__init__.py
+-rw-rw-rw-   0        0        0     6180 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/uncomputation/type_checker.py
+-rw-rw-rw-   0        0        0     4430 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/uncomputation/uncomputation.py
+-rw-rw-rw-   0        0        0    11617 2023-04-24 14:36:50.000000 qrisp-0.0.8/src/qrisp/uncomputation/unqomp.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp.egg-info/
+-rw-rw-rw-   0        0        0      640 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5228 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 15:19:30.000000 qrisp-0.0.8/src/qrisp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 15:19:31.000000 qrisp-0.0.8/tests/
+-rw-rw-rw-   0        0        0     1121 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_GMS_environment_example.py
+-rw-rw-rw-   0        0        0     1475 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_GXX_converter_example.py
+-rw-rw-rw-   0        0        0     2190 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_GXX_gates_example.py
+-rw-rw-rw-   0        0        0     3035 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_GZZ_gates_example.py
+-rw-rw-rw-   0        0        0     2476 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_abstract_parameters.py
+-rw-rw-rw-   0        0        0      940 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_array_entry_manipulation.py
+-rw-rw-rw-   0        0        0     4149 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_comparisons.py
+-rw-rw-rw-   0        0        0     3442 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_conditional_environments_example.py
+-rw-rw-rw-   0        0        0     3037 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_controlled_gates.py
+-rw-rw-rw-   0        0        0     4231 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_diagonal_hamiltonian_application.py
+-rw-rw-rw-   0        0        0     1603 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_gray_synthesis_example.py
+-rw-rw-rw-   0        0        0     3848 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_grovers_algorithm.py
+-rw-rw-rw-   0        0        0      675 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_hello_world.py
+-rw-rw-rw-   0        0        0     1693 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_inpl_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     1569 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_interface.py
+-rw-rw-rw-   0        0        0      973 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_loops.py
+-rw-rw-rw-   0        0        0     2058 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     2420 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_mcx.py
+-rw-rw-rw-   0        0        0      670 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_measurement_reduction.py
+-rw-rw-rw-   0        0        0      663 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_outcome_array.py
+-rw-rw-rw-   0        0        0     1894 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_qiskit_backend_client.py
+-rw-rw-rw-   0        0        0      806 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_qompiler.py
+-rw-rw-rw-   0        0        0     3087 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_quantum_arithmetic.py
+-rw-rw-rw-   0        0        0     2912 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_quantum_dictionary.py
+-rw-rw-rw-   0        0        0     1047 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_quantum_division.py
+-rw-rw-rw-   0        0        0     4896 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_quantum_teleportation.py
+-rw-rw-rw-   0        0        0     1236 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_state_preparation.py
+-rw-rw-rw-   0        0        0      958 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_string_test.py
+-rw-rw-rw-   0        0        0     5218 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_uncomputation_example.py
+-rw-rw-rw-   0        0        0     1600 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/test_unitary_calculation.py
+-rw-rw-rw-   0        0        0     4023 2023-04-24 14:36:50.000000 qrisp-0.0.8/tests/tests_doc_examples.py
```

### Comparing `qrisp-0.0.7/LICENSE` & `qrisp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/PKG-INFO` & `qrisp-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Qrisp - A high-level programming language for gate-based quantum computers
 Home-page: https://github.com/pypa/sampleproject
 Author: Raphael Seidel
 Author-email: Raphael Seidel <raphael.seidel@fokus.fraunhofer.de>
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qrisp-0.0.7/setup.cfg` & `qrisp-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/setup.py` & `qrisp-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/__init__.py` & `qrisp-0.0.8/src/qrisp/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/arithmetic/SBP_arithmetic.py` & `qrisp-0.0.8/src/qrisp/arithmetic/SBP_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/arithmetic/__init__.py` & `qrisp-0.0.8/src/qrisp/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/arithmetic/comparisons.py` & `qrisp-0.0.8/src/qrisp/arithmetic/comparisons.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/arithmetic/incrementation.py` & `qrisp-0.0.8/src/qrisp/arithmetic/incrementation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/arithmetic/matrix_multiplication.py` & `qrisp-0.0.8/src/qrisp/arithmetic/matrix_multiplication.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/arithmetic/poly_tools.py` & `qrisp-0.0.8/src/qrisp/arithmetic/poly_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/arithmetic/ripple_carry_adder.py` & `qrisp-0.0.8/src/qrisp/arithmetic/ripple_carry_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/arithmetic/ripple_division.py` & `qrisp-0.0.8/src/qrisp/arithmetic/ripple_division.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/arithmetic/ripple_mult.py` & `qrisp-0.0.8/src/qrisp/arithmetic/ripple_mult.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/__init__.py` & `qrisp-0.0.8/src/qrisp/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/clbit.py` & `qrisp-0.0.8/src/qrisp/circuit/clbit.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/controlled_operations.py` & `qrisp-0.0.8/src/qrisp/circuit/controlled_operations.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/instruction.py` & `qrisp-0.0.8/src/qrisp/circuit/instruction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/multi_cx.py` & `qrisp-0.0.8/src/qrisp/circuit/multi_cx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/operation.py` & `qrisp-0.0.8/src/qrisp/circuit/operation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/quantum_circuit.py` & `qrisp-0.0.8/src/qrisp/circuit/quantum_circuit.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/qubit.py` & `qrisp-0.0.8/src/qrisp/circuit/qubit.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/standard_operations.py` & `qrisp-0.0.8/src/qrisp/circuit/standard_operations.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/transpiler.py` & `qrisp-0.0.8/src/qrisp/circuit/transpiler.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/circuit/transpiler_old.py` & `qrisp-0.0.8/src/qrisp/circuit/transpiler_old.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/core/__init__.py` & `qrisp-0.0.8/src/qrisp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/core/compilation.py` & `qrisp-0.0.8/src/qrisp/core/compilation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/core/library.py` & `qrisp-0.0.8/src/qrisp/core/library.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/core/quantum_array.py` & `qrisp-0.0.8/src/qrisp/core/quantum_array.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/core/quantum_dictionary.py` & `qrisp-0.0.8/src/qrisp/core/quantum_dictionary.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/core/quantum_session.py` & `qrisp-0.0.8/src/qrisp/core/quantum_session.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/core/quantum_variable.py` & `qrisp-0.0.8/src/qrisp/core/quantum_variable.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/core/session_merging_tools.py` & `qrisp-0.0.8/src/qrisp/core/session_merging_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/default_backend.py` & `qrisp-0.0.8/src/qrisp/default_backend.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/environments/GMS_environment.py` & `qrisp-0.0.8/src/qrisp/environments/GMS_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/environments/__init__.py` & `qrisp-0.0.8/src/qrisp/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/environments/control_environment.py` & `qrisp-0.0.8/src/qrisp/environments/control_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/environments/gate_wrap_environment.py` & `qrisp-0.0.8/src/qrisp/environments/gate_wrap_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/environments/quantum_conditionals.py` & `qrisp-0.0.8/src/qrisp/environments/quantum_conditionals.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/environments/quantum_environments.py` & `qrisp-0.0.8/src/qrisp/environments/quantum_environments.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/environments/quantum_inversion.py` & `qrisp-0.0.8/src/qrisp/environments/quantum_inversion.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/environments/temp_var_environment.py` & `qrisp-0.0.8/src/qrisp/environments/temp_var_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/grover/grover_tools.py` & `qrisp-0.0.8/src/qrisp/grover/grover_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/__init__.py` & `qrisp-0.0.8/src/qrisp/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/backends.py` & `qrisp-0.0.8/src/qrisp/interface/backends.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/circuit_converter.py` & `qrisp-0.0.8/src/qrisp/interface/circuit_converter.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/openapi_interface/__init__.py` & `qrisp-0.0.8/src/qrisp/interface/openapi_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/openapi_interface/backend_client.py` & `qrisp-0.0.8/src/qrisp/interface/openapi_interface/backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/openapi_interface/backend_server.py` & `qrisp-0.0.8/src/qrisp/interface/openapi_interface/backend_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/openapi_interface/interface_types.py` & `qrisp-0.0.8/src/qrisp/interface/openapi_interface/interface_types.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/thrift_interface/__init__.py` & `qrisp-0.0.8/src/qrisp/interface/thrift_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/thrift_interface/backend_client.py` & `qrisp-0.0.8/src/qrisp/interface/thrift_interface/backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/thrift_interface/backend_server.py` & `qrisp-0.0.8/src/qrisp/interface/thrift_interface/backend_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/BackendService.py` & `qrisp-0.0.8/src/qrisp/interface/thrift_interface/codegen/BackendService.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/constants.py` & `qrisp-0.0.8/src/qrisp/interface/thrift_interface/codegen/constants.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/thrift_interface/codegen/ttypes.py` & `qrisp-0.0.8/src/qrisp/interface/thrift_interface/codegen/ttypes.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/thrift_interface/interface_types.py` & `qrisp-0.0.8/src/qrisp/interface/thrift_interface/interface_types.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py` & `qrisp-0.0.8/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/iterators/qrange.py` & `qrisp-0.0.8/src/qrisp/iterators/qrange.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/logic_synthesis/__init__.py` & `qrisp-0.0.8/src/qrisp/logic_synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/logic_synthesis/gray_synthesis.py` & `qrisp-0.0.8/src/qrisp/logic_synthesis/gray_synthesis.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/logic_synthesis/pprm_synthesis.py` & `qrisp-0.0.8/src/qrisp/logic_synthesis/pprm_synthesis.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/logic_synthesis/truth_tables.py` & `qrisp-0.0.8/src/qrisp/logic_synthesis/truth_tables.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/misc/GMS_tools.py` & `qrisp-0.0.8/src/qrisp/misc/GMS_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/misc/depth_reduction.py` & `qrisp-0.0.8/src/qrisp/misc/depth_reduction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/misc/utility.py` & `qrisp-0.0.8/src/qrisp/misc/utility.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/qtypes/__init__.py` & `qrisp-0.0.8/src/qrisp/qtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/qtypes/quantum_bool.py` & `qrisp-0.0.8/src/qrisp/qtypes/quantum_bool.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/qtypes/quantum_char.py` & `qrisp-0.0.8/src/qrisp/qtypes/quantum_char.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/qtypes/quantum_float.py` & `qrisp-0.0.8/src/qrisp/qtypes/quantum_float.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/qtypes/quantum_string.py` & `qrisp-0.0.8/src/qrisp/qtypes/quantum_string.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/quantum_network/__init__.py` & `qrisp-0.0.8/src/qrisp/quantum_network/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py` & `qrisp-0.0.8/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/constants.py` & `qrisp-0.0.8/src/qrisp/quantum_network/interface/codegen/constants.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/quantum_network/interface/codegen/ttypes.py` & `qrisp-0.0.8/src/qrisp/quantum_network/interface/codegen/ttypes.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/quantum_network/interface_connection_example.py` & `qrisp-0.0.8/src/qrisp/quantum_network/interface_connection_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/quantum_network/qn_client.py` & `qrisp-0.0.8/src/qrisp/quantum_network/qn_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/quantum_network/qn_server.py` & `qrisp-0.0.8/src/qrisp/quantum_network/qn_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/quantum_network/qn_simulator_server.py` & `qrisp-0.0.8/src/qrisp/quantum_network/qn_simulator_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/quantum_network/quantum_network_session.py` & `qrisp-0.0.8/src/qrisp/quantum_network/quantum_network_session.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/__init__.py` & `qrisp-0.0.8/src/qrisp/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/bi_array_helper.py` & `qrisp-0.0.8/src/qrisp/simulator/bi_array_helper.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/bi_arrays.py` & `qrisp-0.0.8/src/qrisp/simulator/bi_arrays.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/bi_arrays_new.py` & `qrisp-0.0.8/src/qrisp/simulator/bi_arrays_new.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/circuit_preprocessing.py` & `qrisp-0.0.8/src/qrisp/simulator/circuit_preprocessing.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/circuit_reordering.py` & `qrisp-0.0.8/src/qrisp/simulator/circuit_reordering.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/impure_quantum_state.py` & `qrisp-0.0.8/src/qrisp/simulator/impure_quantum_state.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/quantum_state.py` & `qrisp-0.0.8/src/qrisp/simulator/quantum_state.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/simulator.py` & `qrisp-0.0.8/src/qrisp/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/tensor_factor.py` & `qrisp-0.0.8/src/qrisp/simulator/tensor_factor.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/simulator/unitary_management.py` & `qrisp-0.0.8/src/qrisp/simulator/unitary_management.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/uncomputation/__init__.py` & `qrisp-0.0.8/src/qrisp/uncomputation/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/uncomputation/type_checker.py` & `qrisp-0.0.8/src/qrisp/uncomputation/type_checker.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/uncomputation/uncomputation.py` & `qrisp-0.0.8/src/qrisp/uncomputation/uncomputation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp/uncomputation/unqomp.py` & `qrisp-0.0.8/src/qrisp/uncomputation/unqomp.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/src/qrisp.egg-info/PKG-INFO` & `qrisp-0.0.8/src/qrisp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Qrisp - A high-level programming language for gate-based quantum computers
 Home-page: https://github.com/pypa/sampleproject
 Author: Raphael Seidel
 Author-email: Raphael Seidel <raphael.seidel@fokus.fraunhofer.de>
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qrisp-0.0.7/src/qrisp.egg-info/SOURCES.txt` & `qrisp-0.0.8/src/qrisp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_GMS_environment_example.py` & `qrisp-0.0.8/tests/test_GMS_environment_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_GXX_converter_example.py` & `qrisp-0.0.8/tests/test_GXX_converter_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_GXX_gates_example.py` & `qrisp-0.0.8/tests/test_GXX_gates_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_GZZ_gates_example.py` & `qrisp-0.0.8/tests/test_GZZ_gates_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_abstract_parameters.py` & `qrisp-0.0.8/tests/test_abstract_parameters.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_array_entry_manipulation.py` & `qrisp-0.0.8/tests/test_array_entry_manipulation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_comparisons.py` & `qrisp-0.0.8/tests/test_comparisons.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_conditional_environments_example.py` & `qrisp-0.0.8/tests/test_conditional_environments_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_controlled_gates.py` & `qrisp-0.0.8/tests/test_controlled_gates.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_diagonal_hamiltonian_application.py` & `qrisp-0.0.8/tests/test_diagonal_hamiltonian_application.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_gray_synthesis_example.py` & `qrisp-0.0.8/tests/test_gray_synthesis_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_grovers_algorithm.py` & `qrisp-0.0.8/tests/test_grovers_algorithm.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_hello_world.py` & `qrisp-0.0.8/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_inpl_matrix_multiplication_example.py` & `qrisp-0.0.8/tests/test_inpl_matrix_multiplication_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_interface.py` & `qrisp-0.0.8/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_loops.py` & `qrisp-0.0.8/tests/test_loops.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_matrix_multiplication_example.py` & `qrisp-0.0.8/tests/test_matrix_multiplication_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_mcx.py` & `qrisp-0.0.8/tests/test_mcx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_measurement_reduction.py` & `qrisp-0.0.8/tests/test_measurement_reduction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_outcome_array.py` & `qrisp-0.0.8/tests/test_outcome_array.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_qiskit_backend_client.py` & `qrisp-0.0.8/tests/test_qiskit_backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_qompiler.py` & `qrisp-0.0.8/tests/test_qompiler.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_quantum_arithmetic.py` & `qrisp-0.0.8/tests/test_quantum_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_quantum_dictionary.py` & `qrisp-0.0.8/tests/test_quantum_dictionary.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_quantum_division.py` & `qrisp-0.0.8/tests/test_quantum_division.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_quantum_teleportation.py` & `qrisp-0.0.8/tests/test_quantum_teleportation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_state_preparation.py` & `qrisp-0.0.8/tests/test_state_preparation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_string_test.py` & `qrisp-0.0.8/tests/test_string_test.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_uncomputation_example.py` & `qrisp-0.0.8/tests/test_uncomputation_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/test_unitary_calculation.py` & `qrisp-0.0.8/tests/test_unitary_calculation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.7/tests/tests_doc_examples.py` & `qrisp-0.0.8/tests/tests_doc_examples.py`

 * *Files identical despite different names*

