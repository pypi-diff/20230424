# Comparing `tmp/paddle-quantum-2.3.0.tar.gz` & `tmp/paddle-quantum-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddle-quantum-2.3.0.tar", last modified: Fri Jan  6 11:42:28 2023, max compression
+gzip compressed data, was "paddle-quantum-2.4.0.tar", last modified: Mon Apr 24 13:14:53 2023, max compression
```

## Comparing `paddle-quantum-2.3.0.tar` & `paddle-quantum-2.4.0.tar`

### file list

```diff
@@ -1,237 +1,240 @@
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.112498 paddle-quantum-2.3.0/
--rw-r--r--   0 wangzihe   (501) staff       (20)      617 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/LICENSE
--rw-r--r--   0 wangzihe   (501) staff       (20)    19490 2023-01-06 11:42:28.111778 paddle-quantum-2.3.0/PKG-INFO
--rw-r--r--   0 wangzihe   (501) staff       (20)    18762 2023-01-06 11:40:26.000000 paddle-quantum-2.3.0/README.md
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.952727 paddle-quantum-2.3.0/paddle_quantum/
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.959743 paddle-quantum-2.3.0/paddle_quantum/GIBBS/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1577 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/GIBBS/HGenerator.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3590 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/GIBBS/Paddle_GIBBS.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.960997 paddle-quantum-2.3.0/paddle_quantum/GIBBS/example/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1593 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/GIBBS/example/main.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.963728 paddle-quantum-2.3.0/paddle_quantum/QAOA/
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.964747 paddle-quantum-2.3.0/paddle_quantum/QAOA/example/
--rw-r--r--   0 wangzihe   (501) staff       (20)     2181 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/QAOA/example/main.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3294 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/QAOA/maxcut.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     6092 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/QAOA/tsp.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.966343 paddle-quantum-2.3.0/paddle_quantum/SSVQE/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1274 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/SSVQE/HGenerator.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4148 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/SSVQE/Paddle_SSVQE.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.967540 paddle-quantum-2.3.0/paddle_quantum/SSVQE/example/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1574 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/SSVQE/example/main.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.972048 paddle-quantum-2.3.0/paddle_quantum/VQE/
--rw-r--r--   0 wangzihe   (501) staff       (20)     3592 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQE/Paddle_VQE.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     2565 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQE/benchmark.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4128 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQE/chemistrygen.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4161 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQE/chemistrysub.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.974141 paddle-quantum-2.3.0/paddle_quantum/VQE/example/
--rw-r--r--   0 wangzihe   (501) staff       (20)      112 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQE/example/h2.xyz
--rw-r--r--   0 wangzihe   (501) staff       (20)     1772 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQE/example/main.py
--rw-r--r--   0 wangzihe   (501) staff       (20)      112 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQE/h2.xyz
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.975631 paddle-quantum-2.3.0/paddle_quantum/VQSD/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1361 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQSD/HGenerator.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3224 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQSD/Paddle_VQSD.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.976385 paddle-quantum-2.3.0/paddle_quantum/VQSD/example/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1092 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/VQSD/example/main.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     1469 2023-01-06 07:33:25.000000 paddle-quantum-2.3.0/paddle_quantum/__init__.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.979212 paddle-quantum-2.3.0/paddle_quantum/ansatz/
--rw-r--r--   0 wangzihe   (501) staff       (20)      800 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/ansatz/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    73094 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/ansatz/circuit.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     6687 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/ansatz/container.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    35749 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/ansatz/vans.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.982156 paddle-quantum-2.3.0/paddle_quantum/backend/
--rw-r--r--   0 wangzihe   (501) staff       (20)      985 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/backend/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     5067 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/backend/density_matrix.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    12883 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/backend/quleaf.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3507 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/backend/state_vector.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3569 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/backend/unitary_matrix.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4040 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/base.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.985342 paddle-quantum-2.3.0/paddle_quantum/biocomputing/
--rw-r--r--   0 wangzihe   (501) staff       (20)      816 2023-01-06 11:35:55.000000 paddle-quantum-2.3.0/paddle_quantum/biocomputing/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     6064 2023-01-06 11:35:59.000000 paddle-quantum-2.3.0/paddle_quantum/biocomputing/algorithm.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     2020 2023-01-06 11:36:02.000000 paddle-quantum-2.3.0/paddle_quantum/biocomputing/data_loader.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3969 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/biocomputing/mj_matrix.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3597 2023-01-06 11:36:05.000000 paddle-quantum-2.3.0/paddle_quantum/biocomputing/operators.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     8635 2023-01-06 11:36:08.000000 paddle-quantum-2.3.0/paddle_quantum/biocomputing/protein.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     2325 2023-01-06 11:36:10.000000 paddle-quantum-2.3.0/paddle_quantum/biocomputing/visualize.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.988236 paddle-quantum-2.3.0/paddle_quantum/channel/
--rw-r--r--   0 wangzihe   (501) staff       (20)      838 2023-01-05 03:00:12.000000 paddle-quantum-2.3.0/paddle_quantum/channel/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4249 2023-01-05 13:48:07.000000 paddle-quantum-2.3.0/paddle_quantum/channel/base.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    12485 2023-01-05 13:48:07.000000 paddle-quantum-2.3.0/paddle_quantum/channel/common.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    12497 2023-01-05 13:48:07.000000 paddle-quantum-2.3.0/paddle_quantum/channel/custom.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.989281 paddle-quantum-2.3.0/paddle_quantum/channel/functional/
--rw-r--r--   0 wangzihe   (501) staff       (20)      833 2023-01-05 03:00:12.000000 paddle-quantum-2.3.0/paddle_quantum/channel/functional/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    14987 2023-01-05 13:48:07.000000 paddle-quantum-2.3.0/paddle_quantum/channel/functional/common.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    16232 2023-01-05 13:31:39.000000 paddle-quantum-2.3.0/paddle_quantum/channel/representation.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.990349 paddle-quantum-2.3.0/paddle_quantum/data_analysis/
--rw-r--r--   0 wangzihe   (501) staff       (20)    13063 2023-01-05 17:33:47.000000 paddle-quantum-2.3.0/paddle_quantum/data_analysis/vqls.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    26432 2023-01-05 17:21:04.000000 paddle-quantum-2.3.0/paddle_quantum/data_analysis/vqr.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    42530 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/dataset.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.992450 paddle-quantum-2.3.0/paddle_quantum/finance/
--rw-r--r--   0 wangzihe   (501) staff       (20)      932 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/finance/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    14013 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/finance/finance.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     9359 2023-01-06 11:35:40.000000 paddle-quantum-2.3.0/paddle_quantum/finance/pricing.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4774 2023-01-06 11:35:37.000000 paddle-quantum-2.3.0/paddle_quantum/finance/qpo.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    15690 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/fisher.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.000866 paddle-quantum-2.3.0/paddle_quantum/gate/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1548 2022-11-23 15:45:48.000000 paddle-quantum-2.3.0/paddle_quantum/gate/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     6486 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/gate/base.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    10811 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/gate/clifford.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4754 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/gate/custom.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    12639 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/gate/encoding.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.005113 paddle-quantum-2.3.0/paddle_quantum/gate/functional/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1856 2022-11-23 15:45:48.000000 paddle-quantum-2.3.0/paddle_quantum/gate/functional/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     1987 2022-11-23 15:45:48.000000 paddle-quantum-2.3.0/paddle_quantum/gate/functional/base.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    20948 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/gate/functional/multi_qubit_gate.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    11695 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/gate/functional/single_qubit_gate.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    31046 2022-12-07 07:24:12.000000 paddle-quantum-2.3.0/paddle_quantum/gate/functional/visual.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    28228 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/gate/layer.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    42989 2022-11-23 15:45:48.000000 paddle-quantum-2.3.0/paddle_quantum/gate/multi_qubit_gate.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    25949 2022-11-23 15:45:48.000000 paddle-quantum-2.3.0/paddle_quantum/gate/single_qubit_gate.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    13979 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/gradtool.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    15806 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/hamiltonian.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3593 2023-01-05 03:00:12.000000 paddle-quantum-2.3.0/paddle_quantum/intrinsic.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    19439 2023-01-05 13:48:07.000000 paddle-quantum-2.3.0/paddle_quantum/linalg.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.008770 paddle-quantum-2.3.0/paddle_quantum/locc/
--rw-r--r--   0 wangzihe   (501) staff       (20)      840 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/locc/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    28962 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/locc/locc_ansatz.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    22013 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/locc/locc_net.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     1169 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/locc/locc_party.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3932 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/locc/locc_state.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.011569 paddle-quantum-2.3.0/paddle_quantum/loss/
--rw-r--r--   0 wangzihe   (501) staff       (20)      794 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/loss/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4813 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/loss/distance.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     9712 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/loss/measure.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.018970 paddle-quantum-2.3.0/paddle_quantum/mbqc/
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.019898 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.022238 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/
--rw-r--r--   0 wangzihe   (501) staff       (20)      909 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/main.py
--rw-r--r--   0 wangzihe   (501) staff       (20)      477 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/record_time.txt
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.935238 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.075129 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_0.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_1.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_2.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_3.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_4.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_5.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_6.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_7.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_8.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1598 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_9.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_0.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_1.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_2.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_3.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_4.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_5.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_6.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_7.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_8.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     1935 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_9.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_0.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_1.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_2.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_3.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_4.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_5.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_6.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_7.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_8.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2352 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_9.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_0.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_1.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_2.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_3.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_4.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_5.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_6.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_7.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_8.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     2774 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_9.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_0.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_1.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_2.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_3.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_4.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_5.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_6.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_7.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_8.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     3275 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_9.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     7210 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/supremacy.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.078347 paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.081718 paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/example/
--rw-r--r--   0 wangzihe   (501) staff       (20)     2486 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/example/maxcut_main.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     2147 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/example/pubo_main.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    11666 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/maxcut.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    12400 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/pubo.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    23553 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/qaoa.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.083004 paddle-quantum-2.3.0/paddle_quantum/mbqc/QKernel/
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.084964 paddle-quantum-2.3.0/paddle_quantum/mbqc/QKernel/example/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1086 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/QKernel/example/main.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3107 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/QKernel/example/record_time.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     8348 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/QKernel/qkernel.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.086189 paddle-quantum-2.3.0/paddle_quantum/mbqc/VQSVD/
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.089038 paddle-quantum-2.3.0/paddle_quantum/mbqc/VQSVD/example/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1077 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/VQSVD/example/main.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     1163 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/VQSVD/example/record_time.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)     7924 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/VQSVD/vqsvd.py
--rw-r--r--   0 wangzihe   (501) staff       (20)        0 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/__init__.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.937370 paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.092300 paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/mcalculus_tests/
--rw-r--r--   0 wangzihe   (501) staff       (20)     2353 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/mcalculus_tests/cnot_test.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     2041 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/mcalculus_tests/random_test.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     2923 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/mcalculus_tests/single_qubit_unitary_test.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.095275 paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/simulator_tests/
--rw-r--r--   0 wangzihe   (501) staff       (20)     2779 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/simulator_tests/cnot_test.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3169 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/simulator_tests/single_qubit_unitary_test.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    42712 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/mcalculus.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    35184 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/qobject.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    35787 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/simulator.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     1510 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/transpiler.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    33795 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/mbqc/utils.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    33817 2023-01-05 17:27:24.000000 paddle-quantum-2.3.0/paddle_quantum/model.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.096649 paddle-quantum-2.3.0/paddle_quantum/operator/
--rw-r--r--   0 wangzihe   (501) staff       (20)      767 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/operator/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     6756 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/operator/operator.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.102235 paddle-quantum-2.3.0/paddle_quantum/qchem/
--rw-r--r--   0 wangzihe   (501) staff       (20)      990 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/qchem/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4698 2023-01-06 11:36:39.000000 paddle-quantum-2.3.0/paddle_quantum/qchem/algorithm.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     8440 2023-01-06 11:36:43.000000 paddle-quantum-2.3.0/paddle_quantum/qchem/ansatz.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     5198 2023-01-06 11:36:47.000000 paddle-quantum-2.3.0/paddle_quantum/qchem/drivers.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    10202 2023-01-06 11:36:50.000000 paddle-quantum-2.3.0/paddle_quantum/qchem/fermionic_state.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     6727 2023-01-06 11:36:55.000000 paddle-quantum-2.3.0/paddle_quantum/qchem/molecule.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     4827 2023-01-06 11:37:00.000000 paddle-quantum-2.3.0/paddle_quantum/qchem/properties.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3987 2023-01-06 11:37:03.000000 paddle-quantum-2.3.0/paddle_quantum/qchem/utils.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    37146 2023-01-05 13:48:07.000000 paddle-quantum-2.3.0/paddle_quantum/qinfo.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.105560 paddle-quantum-2.3.0/paddle_quantum/qml/
--rw-r--r--   0 wangzihe   (501) staff       (20)      703 2022-11-25 12:35:04.000000 paddle-quantum-2.3.0/paddle_quantum/qml/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    17377 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/qml/qnnmic.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    16550 2023-01-05 17:36:37.000000 paddle-quantum-2.3.0/paddle_quantum/qml/qnnqd.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    21089 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/qml/qsann.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    18080 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/qml/vsql.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.107494 paddle-quantum-2.3.0/paddle_quantum/qpp/
--rw-r--r--   0 wangzihe   (501) staff       (20)      773 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/qpp/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     9721 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/qpp/angles.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    23320 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/qpp/laurent.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    11061 2022-12-01 14:52:57.000000 paddle-quantum-2.3.0/paddle_quantum/qpp/utils.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.109570 paddle-quantum-2.3.0/paddle_quantum/qsvt/
--rw-r--r--   0 wangzihe   (501) staff       (20)      867 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/qsvt/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    16138 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/qsvt/qsp.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     3808 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/qsvt/qsp_utils.py
--rw-r--r--   0 wangzihe   (501) staff       (20)     5617 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/qsvt/qsvt.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    11515 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/shadow.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:28.111112 paddle-quantum-2.3.0/paddle_quantum/state/
--rw-r--r--   0 wangzihe   (501) staff       (20)     1214 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/state/__init__.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    18690 2022-11-17 14:59:46.000000 paddle-quantum-2.3.0/paddle_quantum/state/common.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    24998 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/state/state.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    29353 2023-01-05 09:53:58.000000 paddle-quantum-2.3.0/paddle_quantum/trotter.py
--rw-r--r--   0 wangzihe   (501) staff       (20)    30799 2022-11-23 08:22:51.000000 paddle-quantum-2.3.0/paddle_quantum/visual.py
-drwxr-xr-x   0 wangzihe   (501) staff       (20)        0 2023-01-06 11:42:27.956210 paddle-quantum-2.3.0/paddle_quantum.egg-info/
--rw-r--r--   0 wangzihe   (501) staff       (20)    19490 2023-01-06 11:42:27.000000 paddle-quantum-2.3.0/paddle_quantum.egg-info/PKG-INFO
--rw-r--r--   0 wangzihe   (501) staff       (20)     8476 2023-01-06 11:42:27.000000 paddle-quantum-2.3.0/paddle_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)        1 2023-01-06 11:42:27.000000 paddle-quantum-2.3.0/paddle_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)      248 2023-01-06 11:42:27.000000 paddle-quantum-2.3.0/paddle_quantum.egg-info/requires.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)       15 2023-01-06 11:42:27.000000 paddle-quantum-2.3.0/paddle_quantum.egg-info/top_level.txt
--rw-r--r--   0 wangzihe   (501) staff       (20)       38 2023-01-06 11:42:28.112634 paddle-quantum-2.3.0/setup.cfg
--rw-r--r--   0 wangzihe   (501) staff       (20)     4103 2023-01-06 07:38:03.000000 paddle-quantum-2.3.0/setup.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.567585 paddle-quantum-2.4.0/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      617 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/LICENSE
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    19531 2023-04-24 13:14:53.567149 paddle-quantum-2.4.0/PKG-INFO
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    18803 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/README.md
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.379066 paddle-quantum-2.4.0/paddle_quantum/
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.388925 paddle-quantum-2.4.0/paddle_quantum/GIBBS/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1577 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/GIBBS/HGenerator.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3590 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/GIBBS/Paddle_GIBBS.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.390669 paddle-quantum-2.4.0/paddle_quantum/GIBBS/example/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1593 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/GIBBS/example/main.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.394015 paddle-quantum-2.4.0/paddle_quantum/QAOA/
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.394585 paddle-quantum-2.4.0/paddle_quantum/QAOA/example/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2211 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/QAOA/example/main.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3294 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/QAOA/maxcut.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     6092 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/QAOA/tsp.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.397522 paddle-quantum-2.4.0/paddle_quantum/SSVQE/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1274 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/SSVQE/HGenerator.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4148 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/SSVQE/Paddle_SSVQE.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.398965 paddle-quantum-2.4.0/paddle_quantum/SSVQE/example/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1574 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/SSVQE/example/main.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.406148 paddle-quantum-2.4.0/paddle_quantum/VQE/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3592 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQE/Paddle_VQE.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2565 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQE/benchmark.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4128 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQE/chemistrygen.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4161 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQE/chemistrysub.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.408830 paddle-quantum-2.4.0/paddle_quantum/VQE/example/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      112 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQE/example/h2.xyz
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1772 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQE/example/main.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      112 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQE/h2.xyz
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.411555 paddle-quantum-2.4.0/paddle_quantum/VQSD/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1361 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQSD/HGenerator.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3224 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQSD/Paddle_VQSD.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.412482 paddle-quantum-2.4.0/paddle_quantum/VQSD/example/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1092 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/VQSD/example/main.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1885 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/__init__.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.414959 paddle-quantum-2.4.0/paddle_quantum/ansatz/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      825 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/ansatz/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    68869 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/ansatz/circuit.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     7774 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/ansatz/container.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    13340 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/ansatz/layer.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    35755 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/ansatz/vans.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.418266 paddle-quantum-2.4.0/paddle_quantum/backend/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      985 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/backend/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     6889 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/backend/density_matrix.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    13865 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/backend/quleaf.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     5000 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/backend/state_vector.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3612 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/backend/unitary_matrix.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4239 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/base.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.434419 paddle-quantum-2.4.0/paddle_quantum/biocomputing/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      816 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/biocomputing/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     6018 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/biocomputing/algorithm.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2020 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/biocomputing/data_loader.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3969 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/biocomputing/mj_matrix.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3597 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/biocomputing/operators.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     8635 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/biocomputing/protein.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2325 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/biocomputing/visualize.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.437497 paddle-quantum-2.4.0/paddle_quantum/channel/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      803 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/channel/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    14631 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/channel/base.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    13857 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/channel/common.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2732 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/channel/custom.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.440829 paddle-quantum-2.4.0/paddle_quantum/channel/functional/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      833 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/channel/functional/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    14987 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/channel/functional/common.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    16840 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/channel/representation.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.443366 paddle-quantum-2.4.0/paddle_quantum/data_analysis/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    24047 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/data_analysis/power_flow.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     5083 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/data_analysis/rand_num.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    12963 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/data_analysis/vqls.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    26429 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/data_analysis/vqr.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    42530 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/dataset.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.448236 paddle-quantum-2.4.0/paddle_quantum/finance/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      952 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/finance/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    14013 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/finance/finance.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    22649 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/finance/pricing.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4774 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/finance/qpo.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    15690 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/fisher.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.453498 paddle-quantum-2.4.0/paddle_quantum/gate/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1361 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    16312 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/base.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    10811 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/gate/clifford.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4375 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/custom.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    12837 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/encoding.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.456136 paddle-quantum-2.4.0/paddle_quantum/gate/functional/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      761 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/functional/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4023 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/functional/base.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    21075 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/functional/visual.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    31369 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/matrix.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    30035 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/multi_qubit_gate.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    16498 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/gate/single_qubit_gate.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    13979 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/gradtool.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    16094 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/hamiltonian.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    16655 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/intrinsic.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    21674 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/linalg.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.460694 paddle-quantum-2.4.0/paddle_quantum/locc/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      840 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/locc/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    28954 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/locc/locc_ansatz.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    22013 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/locc/locc_net.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1169 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/locc/locc_party.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4385 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/locc/locc_state.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.463283 paddle-quantum-2.4.0/paddle_quantum/loss/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      794 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/loss/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4813 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/loss/distance.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     9261 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/loss/measure.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.466670 paddle-quantum-2.4.0/paddle_quantum/mbqc/
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.467499 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.469119 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      909 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/main.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      477 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/record_time.txt
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.361132 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.525610 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_0.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_1.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_2.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_3.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_4.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_5.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_6.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_7.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_8.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1598 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_9.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_0.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_1.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_2.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_3.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_4.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_5.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_6.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_7.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_8.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1935 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_9.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_0.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_1.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_2.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_3.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_4.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_5.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_6.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_7.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_8.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2352 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_9.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_0.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_1.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_2.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_3.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_4.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_5.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_6.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_7.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_8.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2774 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_9.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_0.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_1.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_2.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_3.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_4.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_5.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_6.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_7.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_8.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3275 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_9.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     7210 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/supremacy.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.529094 paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.531360 paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/example/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2486 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/example/maxcut_main.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2147 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/example/pubo_main.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    11666 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/maxcut.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    12400 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/pubo.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    23553 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/qaoa.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.532147 paddle-quantum-2.4.0/paddle_quantum/mbqc/QKernel/
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.534238 paddle-quantum-2.4.0/paddle_quantum/mbqc/QKernel/example/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1086 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/QKernel/example/main.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3107 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/QKernel/example/record_time.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     8348 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/QKernel/qkernel.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.535163 paddle-quantum-2.4.0/paddle_quantum/mbqc/VQSVD/
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.537149 paddle-quantum-2.4.0/paddle_quantum/mbqc/VQSVD/example/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1077 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/VQSVD/example/main.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1163 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/VQSVD/example/record_time.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     7924 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/VQSVD/vqsvd.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)        0 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/__init__.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.363066 paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.538901 paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/mcalculus_tests/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2393 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/mcalculus_tests/cnot_test.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2278 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/mcalculus_tests/random_test.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2923 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/mcalculus_tests/single_qubit_unitary_test.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.540821 paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/simulator_tests/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     2779 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/simulator_tests/cnot_test.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3169 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/simulator_tests/single_qubit_unitary_test.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    44234 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/mcalculus.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    37165 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/qobject.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    36559 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/simulator.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1577 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/transpiler.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    34105 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/mbqc/utils.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    34156 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/model.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.542203 paddle-quantum-2.4.0/paddle_quantum/operator/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      767 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/operator/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     7105 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/operator/operator.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.550673 paddle-quantum-2.4.0/paddle_quantum/qchem/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      990 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qchem/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     5483 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/qchem/algorithm.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     8440 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/qchem/ansatz.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     5198 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/qchem/drivers.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    10202 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/qchem/fermionic_state.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     6727 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/qchem/molecule.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4827 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/qchem/properties.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3987 2023-03-30 11:52:44.000000 paddle-quantum-2.4.0/paddle_quantum/qchem/utils.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    37574 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/qinfo.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.555357 paddle-quantum-2.4.0/paddle_quantum/qml/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      703 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qml/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    19573 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/qml/bert_qtc.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    19784 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/qml/qcaan.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    17418 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/qml/qnnmic.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    16531 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/qml/qnnqd.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    19979 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/qml/qsann.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    18080 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qml/vsql.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.560080 paddle-quantum-2.4.0/paddle_quantum/qpp/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      773 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qpp/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     9721 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qpp/angles.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    23320 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qpp/laurent.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    11061 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/qpp/utils.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.565051 paddle-quantum-2.4.0/paddle_quantum/qsvt/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      867 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qsvt/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    16138 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qsvt/qsp.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     3808 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qsvt/qsp_utils.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     5617 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/qsvt/qsvt.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    11253 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/shadow.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.566676 paddle-quantum-2.4.0/paddle_quantum/state/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     1130 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/state/__init__.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    17442 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/state/common.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    22602 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/paddle_quantum/state/state.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    29353 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/trotter.py
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    30799 2023-03-13 02:40:36.000000 paddle-quantum-2.4.0/paddle_quantum/visual.py
+drwxr-xr-x   0 liguangxi02   (501) staff       (20)        0 2023-04-24 13:14:53.385440 paddle-quantum-2.4.0/paddle_quantum.egg-info/
+-rw-r--r--   0 liguangxi02   (501) staff       (20)    19531 2023-04-24 13:14:53.000000 paddle-quantum-2.4.0/paddle_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     8548 2023-04-24 13:14:53.000000 paddle-quantum-2.4.0/paddle_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)        1 2023-04-24 13:14:53.000000 paddle-quantum-2.4.0/paddle_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)      258 2023-04-24 13:14:53.000000 paddle-quantum-2.4.0/paddle_quantum.egg-info/requires.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)       15 2023-04-24 13:14:53.000000 paddle-quantum-2.4.0/paddle_quantum.egg-info/top_level.txt
+-rw-r--r--   0 liguangxi02   (501) staff       (20)       38 2023-04-24 13:14:53.567664 paddle-quantum-2.4.0/setup.cfg
+-rw-r--r--   0 liguangxi02   (501) staff       (20)     4124 2023-04-24 13:13:55.000000 paddle-quantum-2.4.0/setup.py
```

### Comparing `paddle-quantum-2.3.0/LICENSE` & `paddle-quantum-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/PKG-INFO` & `paddle-quantum-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: paddle-quantum
-Version: 2.3.0
+Version: 2.4.0
 Summary: Paddle Quantum is a quantum machine learning (QML) toolkit developed based on Baidu PaddlePaddle.
 Home-page: http://qml.baidu.com
 Author: Institute for Quantum Computing, Baidu INC.
 Author-email: qml@baidu.com
 Project-URL: Documentation, https://qml.baidu.com/api/introduction.html
 Project-URL: Source, https://github.com/PaddlePaddle/Quantum/
 Project-URL: Tracker, https://github.com/PaddlePaddle/Quantum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+English | [简体中文](README_CN.md)
+
 # Paddle Quantum (量桨)
 
 - [Features](#features)
 - [Install](#install)
    - [Install PaddlePaddle](#install-paddlepaddle)
    - [Install Paddle Quantum](#install-paddle-quantum)
    - [Environment setup for Quantum Chemistry module](#environment_setup_for_quantum_chemistry_module)
@@ -44,15 +46,15 @@
 <p align="center">
   <!-- docs -->
   <a href="https://qml.baidu.com/api/paddle_quantum.circuit.html">
     <img src="https://img.shields.io/badge/docs-link-green.svg?style=flat-square&logo=read-the-docs"/>
   </a>
   <!-- PyPI -->
   <a href="https://pypi.org/project/paddle-quantum/">
-    <img src="https://img.shields.io/badge/pypi-v2.3.0-orange.svg?style=flat-square&logo=pypi"/>
+    <img src="https://img.shields.io/badge/pypi-v2.4.0-orange.svg?style=flat-square&logo=pypi"/>
   </a>
   <!-- Python -->
   <a href="https://www.python.org/">
     <img src="https://img.shields.io/badge/Python-3.6+-blue.svg?style=flat-square&logo=python"/>
   </a>
   <!-- License -->
   <a href="./LICENSE">
@@ -94,15 +96,15 @@
 
 ```bash
 pip install paddle-quantum
 ```
 or download all the files and finish the installation locally,
 
 ```bash
-git clone http://github.com/PaddlePaddle/quantum
+git clone https://github.com/PaddlePaddle/quantum
 cd quantum
 pip install -e .
 ```
 
 ### Environment setup for Quantum Chemistry module
 
 Currently, our `qchem` module uses `PySCF` as its backend to compute molecular integrals, so before executing quantum chemistry, we have to install this Python package.
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: paddle-quantum Version: 2.3.0 Summary: Paddle
+Metadata-Version: 2.1 Name: paddle-quantum Version: 2.4.0 Summary: Paddle
 Quantum is a quantum machine learning (QML) toolkit developed based on Baidu
 PaddlePaddle. Home-page: http://qml.baidu.com Author: Institute for Quantum
 Computing, Baidu INC. Author-email: qml@baidu.com Project-URL: Documentation,
 https://qml.baidu.com/api/introduction.html Project-URL: Source, https://
 github.com/PaddlePaddle/Quantum/ Project-URL: Tracker, https://github.com/
 PaddlePaddle/Quantum/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6, <4 Description-
-Content-Type: text/markdown License-File: LICENSE # Paddle Quantum (éæ¡¨) -
-[Features](#features) - [Install](#install) - [Install PaddlePaddle](#install-
-paddlepaddle) - [Install Paddle Quantum](#install-paddle-quantum) -
-[Environment setup for Quantum Chemistry module]
-(#environment_setup_for_quantum_chemistry_module) - [Run Example](#run-example)
-- [Introduction and developments](#introduction-and-developments) - [Quick
-start](#quick-start) - [Tutorials](#tutorials) - [API documentation](#api-
-documentation) - [Feedbacks](#feedbacks) - [Research with Paddle Quantum]
+Content-Type: text/markdown License-File: LICENSE English | [ç®ä½ä¸­æ]
+(README_CN.md) # Paddle Quantum (éæ¡¨) - [Features](#features) - [Install]
+(#install) - [Install PaddlePaddle](#install-paddlepaddle) - [Install Paddle
+Quantum](#install-paddle-quantum) - [Environment setup for Quantum Chemistry
+module](#environment_setup_for_quantum_chemistry_module) - [Run Example](#run-
+example) - [Introduction and developments](#introduction-and-developments) -
+[Quick start](#quick-start) - [Tutorials](#tutorials) - [API documentation]
+(#api-documentation) - [Feedbacks](#feedbacks) - [Research with Paddle Quantum]
 (#research-based-on-paddle-quantum) - [Frequently Asked Questions](#frequently-
 asked-questions) - [Copyright and License](#copyright-and-license) -
 [References](#references) [Paddle Quantum (éæ¡¨)](https://qml.baidu.com/) is
 the world's first cloud-integrated quantum machine learning platform based on
 Baidu PaddlePaddle. It supports the building and training of quantum neural
 networks, making PaddlePaddle the first deep learning framework in China.
 Paddle Quantum is feature-rich and easy to use. It provides comprehensive API
 documentation and tutorials help users get started right away.
           [https://release-data.cdn.bcebos.com/Paddle%20Quantum.png]
  [https://img.shields.io/badge/docs-link-green.svg?style=flat-square&logo=read-
-  the-docs]  [https://img.shields.io/badge/pypi-v2.3.0-orange.svg?style=flat-
+  the-docs]  [https://img.shields.io/badge/pypi-v2.4.0-orange.svg?style=flat-
          square&logo=pypi]  [https://img.shields.io/badge/Python-3.6+-
 blue.svg?style=flat-square&logo=python]  [https://img.shields.io/badge/license-
 Apache%202.0-blue.svg?style=flat-square&logo=apache]  [https://img.shields.io/
    badge/OS-MacOS%20|%20Windows%20|%20Linux-lightgrey.svg?style=flat-square]
 Paddle Quantum aims at establishing a bridge between artificial intelligence
 (AI) and quantum computing (QC). It has been utilized for developing several
 quantum machine learning applications. With the PaddlePaddle deep learning
@@ -44,15 +44,15 @@
 information processing - Self-developed QML algorithms ## Install ### Install
 PaddlePaddle This dependency will be automatically satisfied when users install
 Paddle Quantum. Please refer to [PaddlePaddle](https://www.paddlepaddle.org.cn/
 install/quick)'s official installation and configuration page. This project
 requires PaddlePaddle 2.2.0 to 2.3.0. ### Install Paddle Quantum We recommend
 the following way of installing Paddle Quantum with `pip`, ```bash pip install
 paddle-quantum ``` or download all the files and finish the installation
-locally, ```bash git clone http://github.com/PaddlePaddle/quantum cd quantum
+locally, ```bash git clone https://github.com/PaddlePaddle/quantum cd quantum
 pip install -e . ``` ### Environment setup for Quantum Chemistry module
 Currently, our `qchem` module uses `PySCF` as its backend to compute molecular
 integrals, so before executing quantum chemistry, we have to install this
 Python package. > It is recommended that `PySCF` is installed in a Python
 environment whose Python version >=3.6. We highly recommend you to install
 `PySCF` via conda. **MacOS/Linux** user can use the command: ```bash conda
 install -c pyscf pyscf ``` > NOTE: For **Windows** user, if your operating
```

### Comparing `paddle-quantum-2.3.0/README.md` & `paddle-quantum-2.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+English | [简体中文](README_CN.md)
+
 # Paddle Quantum (量桨)
 
 - [Features](#features)
 - [Install](#install)
    - [Install PaddlePaddle](#install-paddlepaddle)
    - [Install Paddle Quantum](#install-paddle-quantum)
    - [Environment setup for Quantum Chemistry module](#environment_setup_for_quantum_chemistry_module)
@@ -27,15 +29,15 @@
 <p align="center">
   <!-- docs -->
   <a href="https://qml.baidu.com/api/paddle_quantum.circuit.html">
     <img src="https://img.shields.io/badge/docs-link-green.svg?style=flat-square&logo=read-the-docs"/>
   </a>
   <!-- PyPI -->
   <a href="https://pypi.org/project/paddle-quantum/">
-    <img src="https://img.shields.io/badge/pypi-v2.3.0-orange.svg?style=flat-square&logo=pypi"/>
+    <img src="https://img.shields.io/badge/pypi-v2.4.0-orange.svg?style=flat-square&logo=pypi"/>
   </a>
   <!-- Python -->
   <a href="https://www.python.org/">
     <img src="https://img.shields.io/badge/Python-3.6+-blue.svg?style=flat-square&logo=python"/>
   </a>
   <!-- License -->
   <a href="./LICENSE">
@@ -77,15 +79,15 @@
 
 ```bash
 pip install paddle-quantum
 ```
 or download all the files and finish the installation locally,
 
 ```bash
-git clone http://github.com/PaddlePaddle/quantum
+git clone https://github.com/PaddlePaddle/quantum
 cd quantum
 pip install -e .
 ```
 
 ### Environment setup for Quantum Chemistry module
 
 Currently, our `qchem` module uses `PySCF` as its backend to compute molecular integrals, so before executing quantum chemistry, we have to install this Python package.
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-# Paddle Quantum (éæ¡¨) - [Features](#features) - [Install](#install) -
-[Install PaddlePaddle](#install-paddlepaddle) - [Install Paddle Quantum]
-(#install-paddle-quantum) - [Environment setup for Quantum Chemistry module]
+English | [ç®ä½ä¸­æ](README_CN.md) # Paddle Quantum (éæ¡¨) - [Features]
+(#features) - [Install](#install) - [Install PaddlePaddle](#install-
+paddlepaddle) - [Install Paddle Quantum](#install-paddle-quantum) -
+[Environment setup for Quantum Chemistry module]
 (#environment_setup_for_quantum_chemistry_module) - [Run Example](#run-example)
 - [Introduction and developments](#introduction-and-developments) - [Quick
 start](#quick-start) - [Tutorials](#tutorials) - [API documentation](#api-
 documentation) - [Feedbacks](#feedbacks) - [Research with Paddle Quantum]
 (#research-based-on-paddle-quantum) - [Frequently Asked Questions](#frequently-
 asked-questions) - [Copyright and License](#copyright-and-license) -
 [References](#references) [Paddle Quantum (éæ¡¨)](https://qml.baidu.com/) is
 the world's first cloud-integrated quantum machine learning platform based on
 Baidu PaddlePaddle. It supports the building and training of quantum neural
 networks, making PaddlePaddle the first deep learning framework in China.
 Paddle Quantum is feature-rich and easy to use. It provides comprehensive API
 documentation and tutorials help users get started right away.
           [https://release-data.cdn.bcebos.com/Paddle%20Quantum.png]
  [https://img.shields.io/badge/docs-link-green.svg?style=flat-square&logo=read-
-  the-docs]  [https://img.shields.io/badge/pypi-v2.3.0-orange.svg?style=flat-
+  the-docs]  [https://img.shields.io/badge/pypi-v2.4.0-orange.svg?style=flat-
          square&logo=pypi]  [https://img.shields.io/badge/Python-3.6+-
 blue.svg?style=flat-square&logo=python]  [https://img.shields.io/badge/license-
 Apache%202.0-blue.svg?style=flat-square&logo=apache]  [https://img.shields.io/
    badge/OS-MacOS%20|%20Windows%20|%20Linux-lightgrey.svg?style=flat-square]
 Paddle Quantum aims at establishing a bridge between artificial intelligence
 (AI) and quantum computing (QC). It has been utilized for developing several
 quantum machine learning applications. With the PaddlePaddle deep learning
@@ -34,15 +35,15 @@
 information processing - Self-developed QML algorithms ## Install ### Install
 PaddlePaddle This dependency will be automatically satisfied when users install
 Paddle Quantum. Please refer to [PaddlePaddle](https://www.paddlepaddle.org.cn/
 install/quick)'s official installation and configuration page. This project
 requires PaddlePaddle 2.2.0 to 2.3.0. ### Install Paddle Quantum We recommend
 the following way of installing Paddle Quantum with `pip`, ```bash pip install
 paddle-quantum ``` or download all the files and finish the installation
-locally, ```bash git clone http://github.com/PaddlePaddle/quantum cd quantum
+locally, ```bash git clone https://github.com/PaddlePaddle/quantum cd quantum
 pip install -e . ``` ### Environment setup for Quantum Chemistry module
 Currently, our `qchem` module uses `PySCF` as its backend to compute molecular
 integrals, so before executing quantum chemistry, we have to install this
 Python package. > It is recommended that `PySCF` is installed in a Python
 environment whose Python version >=3.6. We highly recommend you to install
 `PySCF` via conda. **MacOS/Linux** user can use the command: ```bash conda
 install -c pyscf pyscf ``` > NOTE: For **Windows** user, if your operating
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/GIBBS/HGenerator.py` & `paddle-quantum-2.4.0/paddle_quantum/GIBBS/HGenerator.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/GIBBS/Paddle_GIBBS.py` & `paddle-quantum-2.4.0/paddle_quantum/GIBBS/Paddle_GIBBS.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/GIBBS/example/main.py` & `paddle-quantum-2.4.0/paddle_quantum/GIBBS/example/main.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/QAOA/example/main.py` & `paddle-quantum-2.4.0/paddle_quantum/QAOA/example/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "font_color": "white",
     "node_size": 2000,
     "width": 2
 }
 
 
 if __name__ == "__main__":
-    n = 4
+    num_acted_qubits = 4
     paddle.seed(SEED)
     
     p = 4  # number of layers in the circuit
     ITR = 120  # number of iterations
     LR = 0.1    # learning rate
 
     G = nx.cycle_graph(4)
@@ -52,15 +52,15 @@
     ax = plt.gca()
     ax.margins(0.20)
     plt.axis("off")
     plt.show()
 
     # construct the Hamiltonian
     H_D_list = maxcut_hamiltonian(E)
-    H_D_matrix = pauli_str_to_matrix(H_D_list, n)
+    H_D_matrix = pauli_str_to_matrix(H_D_list, num_acted_qubits)
     H_D_diag = np.diag(H_D_matrix).real
     H_max = np.max(H_D_diag)
 
     print(H_D_diag)
     print('H_max:', H_max)   
 
     cut_bitstring, _ = find_cut(G, p, ITR, LR, print_loss=True, plot=True)
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/QAOA/maxcut.py` & `paddle-quantum-2.4.0/paddle_quantum/QAOA/maxcut.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/QAOA/tsp.py` & `paddle-quantum-2.4.0/paddle_quantum/QAOA/tsp.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/SSVQE/HGenerator.py` & `paddle-quantum-2.4.0/paddle_quantum/SSVQE/HGenerator.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/SSVQE/Paddle_SSVQE.py` & `paddle-quantum-2.4.0/paddle_quantum/SSVQE/Paddle_SSVQE.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/SSVQE/example/main.py` & `paddle-quantum-2.4.0/paddle_quantum/SSVQE/example/main.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/VQE/Paddle_VQE.py` & `paddle-quantum-2.4.0/paddle_quantum/VQE/Paddle_VQE.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/VQE/benchmark.py` & `paddle-quantum-2.4.0/paddle_quantum/VQE/benchmark.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/VQE/chemistrygen.py` & `paddle-quantum-2.4.0/paddle_quantum/VQE/chemistrygen.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/VQE/chemistrysub.py` & `paddle-quantum-2.4.0/paddle_quantum/VQE/chemistrysub.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/VQE/example/main.py` & `paddle-quantum-2.4.0/paddle_quantum/VQE/example/main.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/VQSD/HGenerator.py` & `paddle-quantum-2.4.0/paddle_quantum/VQSD/HGenerator.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/VQSD/Paddle_VQSD.py` & `paddle-quantum-2.4.0/paddle_quantum/VQSD/Paddle_VQSD.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/VQSD/example/main.py` & `paddle-quantum-2.4.0/paddle_quantum/VQSD/example/main.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,41 +10,51 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
-Paddle Quantum Library.
+Paddle Quantum
+==============
+
+[Paddle Quantum](https://qml.baidu.com) is a quantum machine learning (QML) toolkit 
+developed based on Baidu PaddlePaddle. It supports easy-to-use quantum neural 
+networks (QNN) construction and training, provides combinatorial optimization, 
+quantum chemistry and other cutting-edge quantum applications. 
+
+See [online API](https://qml.baidu.com/api) for complete documentation.
 """
+
 import os
 os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"]="python"
 from .backend import Backend
 from .state import State
 from .base import Operator
 from .base import set_device, get_device
 from .base import set_dtype, get_dtype
 from .base import set_backend, get_backend
 from .hamiltonian import Hamiltonian
+from .ansatz import Circuit
 from . import ansatz
 from . import channel
 from . import gate
 from . import locc
 from . import loss
 from . import mbqc
 from . import operator
 from . import base
 from . import dataset
-#from . import finance
+from . import finance
 from . import fisher
 from . import gradtool
 from . import hamiltonian
 from . import linalg
 from . import qinfo
 from . import qml
 from . import shadow
 from . import trotter
 from . import visual
 from . import qchem
 
 name = 'paddle_quantum'
-__version__ = '2.3.0'
+__version__ = '2.4.0'
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/ansatz/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/qml/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,13 +10,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
-The module that contains the various ansatzes.
+The quantum machine learning module.
 """
-
-from .container import Sequential
-from .circuit import Circuit
-from .vans import VAns
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/ansatz/circuit.py` & `paddle-quantum-2.4.0/paddle_quantum/ansatz/circuit.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,31 +16,30 @@
 r"""
 The source file of the Circuit class.
 """
 
 import warnings
 import paddle
 from .container import Sequential
+from .layer import Layer, SuperpositionLayer, WeakSuperpositionLayer, LinearEntangledLayer
+from .layer import RealBlockLayer, RealEntangledLayer, ComplexBlockLayer, ComplexEntangledLayer, QAOALayer
 from ..gate import Gate, H, S, Sdg, T, Tdg, X, Y, Z, P, RX, RY, RZ, U3
 from ..gate import CNOT, CX, CY, CZ, SWAP
 from ..gate import CP, CRX, CRY, CRZ, CU, RXX, RYY, RZZ
-from ..gate import MS, CSWAP, Toffoli
+from ..gate import MS, CSWAP, CCX
 from ..gate import UniversalTwoQubits, UniversalThreeQubits
 from ..gate import Oracle, ControlOracle
-from ..gate import SuperpositionLayer, WeakSuperpositionLayer, LinearEntangledLayer
-from ..gate import RealBlockLayer, RealEntangledLayer, ComplexBlockLayer, ComplexEntangledLayer
-from ..gate import QAOALayer
-from ..gate import AmplitudeEncoding
 from ..channel import BitFlip, PhaseFlip, BitPhaseFlip, AmplitudeDamping, GeneralizedAmplitudeDamping, PhaseDamping
 from ..channel import Depolarizing, GeneralizedDepolarizing, PauliChannel, ResetChannel, ThermalRelaxation
-from ..channel import MixedUnitaryChannel, KrausRepr
-from ..intrinsic import _get_float_dtype
+from ..channel import MixedUnitaryChannel, Channel, ChoiRepr, KrausRepr, StinespringRepr
+from ..intrinsic import _get_float_dtype, _format_qubits_idx, _cnot_idx_fetch
 from ..state import zero_state
 from ..operator import Collapse
 from typing import Union, Iterable, Optional, Dict, List, Tuple
+import paddle_quantum as pq
 from paddle_quantum import State, get_backend, get_dtype, Backend
 from math import pi
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 from ..gate.functional.visual import _circuit_plot
 
@@ -55,16 +54,23 @@
     def __init__(self, num_qubits: Optional[int] = None):
         super().__init__()
         self.__num_qubits = num_qubits
 
         # whether the circuit is a dynamic quantum circuit
         self.__isdynamic = num_qubits is None
 
-        # alias for ccx
+        # alias
         self.toffoli = self.ccx
+        self.cx = self.cnot
+
+        # preparing cnot index in 'cycle' case
+        if num_qubits is not None and num_qubits > 1:
+            cnot_qubits_idx = _format_qubits_idx("cycle", num_qubits, num_acted_qubits=2)
+            self.__cnot_cycle_idx = _cnot_idx_fetch(num_qubits=num_qubits, qubits_idx=cnot_qubits_idx)
+
 
     @property
     def num_qubits(self) -> int:
         r"""Number of qubits.
         """
         return self.__num_qubits
 
@@ -89,18 +95,19 @@
 
     @property
     def grad(self) -> np.ndarray:
         r"""Gradients with respect to the flattened parameters.
         """
         grad_list = []
         for param in self.parameters():
-            assert param.grad is not None, 'the gradient is None, run the backward first before calling this property,' + \
-                ' otherwise check where the gradient chain is broken'
-            grad_list.append(paddle.flatten(param.grad))
-        return paddle.concat(grad_list).numpy()
+            assert param.grad is not None, (
+                'The gradient is None, run the backward first before calling this property, '
+                'otherwise check where the gradient chain is broken.')
+            grad_list.append(param.grad.numpy().flatten())
+        return np.concatenate(grad_list)
 
     def update_param(self, theta: Union[paddle.Tensor, np.ndarray, float], idx: int = None) -> None:
         r"""Replace parameters of all/one layer(s) by ``theta``.
 
         Args:
             theta: New parameters
             idx: Index of replacement. Defaults to None, referring to all layers.
@@ -121,36 +128,39 @@
                 for name, _ in layer.named_parameters():
                     param = getattr(layer, name)
                     num_param = int(paddle.numel(param))
 
                     param = paddle.create_parameter(
                         shape=param.shape,
                         dtype='float32',
-                        default_initializer=paddle.nn.initializer.Assign(theta[:num_param].reshape(param.shape)),
+                        default_initializer=paddle.nn.initializer.Assign(
+                            theta[:num_param].reshape(param.shape)),
                     )
 
                     setattr(layer, 'theta', param)
                     if num_param == theta.shape[0]:
                         return
                     theta = theta[num_param:]
         elif isinstance(idx, int):
-            assert idx < len(self.sublayers()), f"the index is out of range, expect below {len(self.sublayers())}"
+            assert idx < len(self.sublayers(
+            )), f"the index is out of range, expect below {len(self.sublayers())}"
 
             layer = self.sublayers()[idx]
-            assert theta.shape == paddle.concat([paddle.flatten(param) for param in layer.parameters()]).shape, \
-                    "the shape of input parameters is not correct,"
+            assert theta.shape == paddle.concat([paddle.flatten(param) for param in layer.parameters()]).shape, (
+                "The shape of input parameters is not correct.")
 
             for name, _ in layer.named_parameters():
                 param = getattr(layer, name)
                 num_param = int(paddle.numel(param))
 
                 param = paddle.create_parameter(
                     shape=param.shape,
                     dtype='float32',
-                    default_initializer=paddle.nn.initializer.Assign(theta[:num_param].reshape(param.shape)),
+                    default_initializer=paddle.nn.initializer.Assign(
+                        theta[:num_param].reshape(param.shape)),
                 )
 
                 setattr(layer, 'theta', param)
                 if num_param == theta.shape[0]:
                     return
                 theta = theta[num_param:]
         else:
@@ -159,61 +169,80 @@
     def transfer_static(self) -> None:
         r"""
         set ``stop_gradient`` of all parameters of the circuit as ``True``
         """
         for layer in self.sublayers():
             for name, _ in layer.named_parameters():
                 param = getattr(layer, name)
-                param.stop_gradient = True 
+                param.stop_gradient = True
                 setattr(layer, 'theta', param)
 
-    def randomize_param(self, low: float = 0, high: Optional[float] = 2 * pi) -> None:
-        r"""Randomize parameters of the circuit in a range from low to high.
+    def randomize_param(self, arg0: float = 0, arg1: float = 2 * pi, initializer_type: str= 'Uniform') -> None:
+        r"""Randomize parameters of the circuit based on the initializer.  Current we only support Uniform and Normal initializer. 
+
+        A detail introduction can be found in https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/nn/initializer/Uniform_en.html
 
         Args:
-            low: Lower bound.
-            high: Upper bound.
+            arg0: first argument of the initializer. Defaults to 0.
+            arg1: first argument of the initializer. Defaults to 2 * pi.
+            initializer_type: The type of the initializer. Defaults to 'Uniform'.
         """
+        assert initializer_type in ["Uniform", "Normal"], (
+            "The initializer should be Uniform or Normal."
+        )
+
         for layer in self.sublayers():
             for name, _ in layer.named_parameters():
                 param = getattr(layer, name)
 
-                param = paddle.create_parameter(
-                    shape=param.shape,
-                    dtype=param.dtype,
-                    default_initializer=paddle.nn.initializer.Uniform(low=low, high=high),
-                )
-                setattr(layer, 'theta', param)
+                if initializer_type == 'Uniform':
+                    param = paddle.create_parameter(
+                        shape=param.shape,
+                        dtype=param.dtype,
+                        default_initializer=paddle.nn.initializer.Uniform(
+                            low=arg0, high=arg1),
+                    )
+                    setattr(layer, 'theta', param)      
+                elif initializer_type == 'Normal':
+                    param = paddle.create_parameter(
+                        shape=param.shape,
+                        dtype=param.dtype,
+                        default_initializer=paddle.nn.initializer.Normal(
+                            mean=arg0, std=arg1),
+                    )
+                    setattr(layer, 'theta', param)
 
     def __num_qubits_update(self, qubits_idx: Union[Iterable[int], int, str]) -> None:
         r"""Update ``self.num_qubits`` according to ``qubits_idx``, or report error.
 
         Args:
             qubits_idx: Input qubit indices of a quantum gate.
         """
         num_qubits = self.__num_qubits
-        if isinstance(qubits_idx, str):
-            assert num_qubits is not None, "The qubit idx cannot be full when the number of qubits is unknown"
+        if isinstance(qubits_idx, str) or qubits_idx is None:
+            assert num_qubits is not None, \
+                f"The qubit idx cannot be a string or None when the number of qubits is unknown: received {qubits_idx}"
             return
 
         if isinstance(qubits_idx, Iterable):
             max_idx = np.max(qubits_idx)
         else:
             max_idx = qubits_idx
 
         if num_qubits is None:
             self.__num_qubits = max_idx + 1
             return
 
-        assert max_idx + 1 <= num_qubits or self.__isdynamic, \
-            f"The circuit is not a dynamic quantum circuit. Invalid input qubit idx: {max_idx} num_qubit: {self.__num_qubits}"
+        assert max_idx + 1 <= num_qubits or self.__isdynamic, (
+            "The circuit is not a dynamic quantum circuit. "
+            f"Invalid input qubit idx: {max_idx} num_qubit: {self.__num_qubits}")
         self.__num_qubits = int(max(max_idx + 1, num_qubits))
 
     def h(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1
     ) -> None:
         r"""Add single-qubit Hadamard gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
@@ -221,22 +250,21 @@
                 \begin{bmatrix}
                     1&1\\
                     1&-1
                 \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(H(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(H(qubits_idx, self.num_qubits, depth))
 
     def s(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1
     ) -> None:
         r"""Add single-qubit S gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
@@ -244,23 +272,21 @@
                 \begin{bmatrix}
                     1&0\\
                     0&i
                 \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            S(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(S(qubits_idx, self.num_qubits, depth))
 
     def sdg(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1
     ) -> None:
         r"""Add single-qubit S dagger (S inverse) gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
@@ -268,46 +294,42 @@
                 \begin{bmatrix}
                     1&0\\
                     0&-i
                 \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``'full'``.
-            num_qubits: Total number of qubits. Defaults to ``None``.
             depth: Number of layers. Defaults to ``1``.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            Sdg(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(Sdg(qubits_idx, self.num_qubits, depth))
 
     def t(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1
     ) -> None:
         r"""Add single-qubit T gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
             T = \begin{bmatrix}
                     1&0\\
                     0&e^\frac{i\pi}{4}
                 \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            T(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(T(qubits_idx, self.num_qubits, depth))
 
     def tdg(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1
     ) -> None:
         r"""Add single-qubit T dagger (T inverse) gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
@@ -315,91 +337,83 @@
                 \begin{bmatrix}
                     1&0\\
                     0&e^{-\frac{i\pi}{4}}
                 \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``'full'``.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            Tdg(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
-        
+        self.append(Tdg(qubits_idx, self.num_qubits, depth))
+
     def x(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1
     ) -> None:
         r"""Add single-qubit X gates.
 
         The matrix form of such a gate is:
 
         .. math::
            X = \begin{bmatrix}
                 0 & 1 \\
                 1 & 0
             \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            X(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(X(qubits_idx, self.num_qubits, depth))
 
     def y(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1
     ) -> None:
         r"""Add single-qubit Y gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
             Y = \begin{bmatrix}
                 0 & -i \\
                 i & 0
             \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            Y(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(Y(qubits_idx, self.num_qubits, depth))
 
     def z(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1
     ) -> None:
         r"""Add single-qubit Z gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
             Z = \begin{bmatrix}
                 1 & 0 \\
                 0 & -1
             \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            Z(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(Z(qubits_idx, self.num_qubits, depth))
 
     def p(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add single-qubit P gates.
 
         The matrix form of such a gate is:
 
         .. math::
@@ -407,25 +421,23 @@
             P(\theta) = \begin{bmatrix}
                 1 & 0 \\
                 0 & e^{i\theta}
             \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            P(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth, param, param_sharing))
+        self.append(P(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def rx(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add single-qubit rotation gates about the x-axis.
 
         The matrix form of such a gate is:
 
         .. math::
@@ -433,25 +445,23 @@
             R_X(\theta) = \begin{bmatrix}
                 \cos\frac{\theta}{2} & -i\sin\frac{\theta}{2} \\
                 -i\sin\frac{\theta}{2} & \cos\frac{\theta}{2}
             \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(RX(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                       depth, param, param_sharing))
+        self.append(RX(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def ry(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add single-qubit rotation gates about the y-axis.
 
         The matrix form of such a gate is:
 
         .. math::
@@ -459,25 +469,23 @@
             R_Y(\theta) = \begin{bmatrix}
                 \cos\frac{\theta}{2} & -\sin\frac{\theta}{2} \\
                 \sin\frac{\theta}{2} & \cos\frac{\theta}{2}
             \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(RY(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                       depth, param, param_sharing))
+        self.append(RY(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def rz(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: Optional[int] = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add single-qubit rotation gates about the z-axis.
 
         The matrix form of such a gate is:
 
         .. math::
@@ -485,25 +493,23 @@
             R_Z(\theta) = \begin{bmatrix}
                 e^{-i\frac{\theta}{2}} & 0 \\
                 0 & e^{i\frac{\theta}{2}}
             \end{bmatrix}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(RZ(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                       depth, param, param_sharing))
+        self.append(RZ(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def u3(
-            self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], int, str] = 'full', depth: int = 1,
             param: Union[paddle.Tensor, Iterable[float]] = None, param_sharing: bool = False
     ) -> None:
         r"""Add single-qubit rotation gates.
 
         The matrix form of such a gate is:
 
         .. math::
@@ -514,25 +520,23 @@
                         \cos\frac\theta2&-e^{i\lambda}\sin\frac\theta2\\
                         e^{i\phi}\sin\frac\theta2&e^{i(\phi+\lambda)}\cos\frac\theta2
                     \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(U3(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                       depth, param, param_sharing))
+        self.append(U3(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def cnot(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1
     ) -> None:
         r"""Add CNOT gates.
 
         For a 2-qubit quantum circuit, when `qubits_idx` is `[0, 1]`, the matrix form of such a gate is:
 
         .. math::
 
@@ -545,37 +549,24 @@
                     0 & 0 & 0 & 1 \\
                     0 & 0 & 1 & 0
                 \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            CNOT(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
-
-    def cx(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1
-    ) -> None:
-        r"""Same as cnot.
-
-        Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
-            depth: Number of layers. Defaults to 1.
-        """
-        self.__num_qubits_update(qubits_idx)
-        self.append(
-            CX(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        if qubits_idx == "cycle" and not self.__isdynamic:
+            self.append(CNOT(qubits_idx, self.num_qubits, depth, self.__cnot_cycle_idx))
+        else:
+            self.append(CNOT(qubits_idx, self.num_qubits, depth))
 
     def cy(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1
     ) -> None:
         r"""Add controlled Y gates.
 
         For a 2-qubit quantum circuit, when `qubits_idx` is `[0, 1]`, the matrix form of such a gate is:
 
         .. math::
 
@@ -588,23 +579,21 @@
                     0 & 0 & 0 & -1j \\
                     0 & 0 & 1j & 0
                 \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            CY(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(CY(qubits_idx, self.num_qubits, depth))
 
     def cz(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], str] = 'linear', depth: int = 1
     ) -> None:
         r"""Add controlled Z gates.
 
         For a 2-qubit quantum circuit, when `qubits_idx` is `[0, 1]`, the matrix form of such a gate is:
 
         .. math::
 
@@ -616,24 +605,22 @@
                     0 & 1 & 0 & 0 \\
                     0 & 0 & 1 & 0 \\
                     0 & 0 & 0 & -1
                 \end{bmatrix}
             \end{align}
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'linear'.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            CZ(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(CZ(qubits_idx, self.num_qubits, depth))
 
     def swap(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], str] = 'linear', depth: int = 1
     ) -> None:
         r"""Add SWAP gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
@@ -644,24 +631,22 @@
                     0 & 0 & 1 & 0 \\
                     0 & 1 & 0 & 0 \\
                     0 & 0 & 0 & 1
                 \end{bmatrix}
             \end{align}
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'linear'.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            SWAP(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(SWAP(qubits_idx, self.num_qubits, depth))
 
     def cp(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add controlled P gates.
 
         For a 2-qubit quantum circuit, when `qubits_idx` is `[0, 1]`, the matrix form of such a gate is:
 
         .. math::
@@ -674,25 +659,23 @@
                     0 & 0 & 1 & 0 \\
                     0 & 0 & 0 & e^{i\theta}
                 \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(CP(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                       depth, param, param_sharing))
+        self.append(CP(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def crx(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add controlled rotation gates about the x-axis.
 
         For a 2-qubit quantum circuit, when `qubits_idx` is `[0, 1]`, the matrix form of such a gate is:
 
         .. math::
@@ -706,25 +689,23 @@
                     0 & 0 & \cos\frac{\theta}{2} & -i\sin\frac{\theta}{2} \\
                     0 & 0 & -i\sin\frac{\theta}{2} & \cos\frac{\theta}{2}
                 \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(CRX(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                        depth, param, param_sharing))
+        self.append(CRX(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def cry(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add controlled rotation gates about the y-axis.
 
         For a 2-qubit quantum circuit, when `qubits_idx` is `[0, 1]`, the matrix form of such a gate is:
 
         .. math::
@@ -738,25 +719,23 @@
                     0 & 0 & \cos\frac{\theta}{2} & -\sin\frac{\theta}{2} \\
                     0 & 0 & \sin\frac{\theta}{2} & \cos\frac{\theta}{2}
                 \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(CRY(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                        depth, param, param_sharing))
+        self.append(CRY(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def crz(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add controlled rotation gates about the z-axis.
 
         For a 2-qubit quantum circuit, when `qubits_idx` is `[0, 1]`, the matrix form of such a gate is:
 
         .. math::
@@ -770,25 +749,23 @@
                     0 & 0 & e^{-i\frac{\theta}{2}} & 0 \\
                     0 & 0 & 0 & e^{i\frac{\theta}{2}}
                 \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(CRZ(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                        depth, param, param_sharing))
+        self.append(CRZ(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def cu(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add controlled single-qubit rotation gates.
 
         For a 2-qubit quantum circuit, when `qubits_idx` is `[0, 1]`, the matrix form of such a gate is:
 
         .. math::
@@ -802,25 +779,23 @@
                     0 & 0 & \cos\frac\theta2 &-e^{i\lambda}\sin\frac\theta2 \\
                     0 & 0 & e^{i\phi}\sin\frac\theta2&e^{i(\phi+\lambda)}\cos\frac\theta2
                 \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(CU(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                       depth, param, param_sharing))
+        self.append(CU(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def rxx(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'linear', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add RXX gates.
 
         The matrix form of such a gate is:
 
         .. math::
@@ -832,26 +807,24 @@
                         0 & \cos\frac{\theta}{2} & -i\sin\frac{\theta}{2} & 0 \\
                         0 & -i\sin\frac{\theta}{2} & \cos\frac{\theta}{2} & 0 \\
                         -i\sin\frac{\theta}{2} & 0 & 0 & \cos\frac{\theta}{2}
                     \end{bmatrix}
             \end{align}
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'linear'.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(RXX(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                        depth, param, param_sharing))
+        self.append(RXX(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def ryy(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'linear', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add RYY gates.
 
         The matrix form of such a gate is:
 
         .. math::
@@ -863,26 +836,24 @@
                         0 & \cos\frac{\theta}{2} & -i\sin\frac{\theta}{2} & 0 \\
                         0 & -i\sin\frac{\theta}{2} & \cos\frac{\theta}{2} & 0 \\
                         i\sin\frac{\theta}{2} & 0 & 0 & cos\frac{\theta}{2}
                     \end{bmatrix}
             \end{align}
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'linear'.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(RYY(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                        depth, param, param_sharing))
+        self.append(RYY(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def rzz(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'linear', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add RZZ gates.
 
         The matrix form of such a gate is:
 
         .. math::
@@ -894,26 +865,24 @@
                         0 & e^{i\frac{\theta}{2}} & 0 & 0 \\
                         0 & 0 & e^{i\frac{\theta}{2}} & 0 \\
                         0 & 0 & 0 & e^{-i\frac{\theta}{2}}
                     \end{bmatrix}
             \end{align}
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'linear'.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(RZZ(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                        depth, param, param_sharing))
+        self.append(RZZ(qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def ms(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1
     ) -> None:
         r"""Add Mølmer-Sørensen (MS) gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
@@ -925,23 +894,21 @@
                         0 & i & 1 & 0 \\
                         i & 0 & 0 & 1
                     \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            MS(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(MS(qubits_idx, self.num_qubits, depth))
 
     def cswap(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1
     ) -> None:
         r"""Add CSWAP (Fredkin) gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
@@ -957,25 +924,23 @@
                     0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \\
                     0 & 0 & 0 & 0 & 0 & 0 & 0 & 1
                 \end{bmatrix}
             \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            CSWAP(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(CSWAP(qubits_idx, self.num_qubits, depth))
 
     def ccx(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1
     ) -> None:
-        r"""Add CCX gates.
+        r"""Add CCX (Toffoli) gates.
 
         The matrix form of such a gate is:
 
         .. math::
 
             \begin{align}
                     \mathit{CCX} = \begin{bmatrix}
@@ -988,477 +953,476 @@
                         0 & 0 & 0 & 0 & 0 & 0 & 0 & 1 \\
                         0 & 0 & 0 & 0 & 0 & 0 & 1 & 0
                     \end{bmatrix}
                 \end{align}
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            Toffoli(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.append(CCX(qubits_idx, self.num_qubits, depth))
 
     def universal_two_qubits(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add universal two-qubit gates. One of such a gate requires 15 parameters.
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(UniversalTwoQubits(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                                       depth, param, param_sharing))
+        self.append(UniversalTwoQubits(
+            qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def universal_three_qubits(
-            self, qubits_idx: Union[Iterable[int], str] = 'cycle', num_qubits: int = None, depth: int = 1,
+            self, qubits_idx: Union[Iterable[int], str] = 'cycle', depth: int = 1,
             param: Union[paddle.Tensor, float] = None, param_sharing: bool = False
     ) -> None:
         r"""Add universal three-qubit gates. One of such a gate requires 81 parameters.
 
         Args:
             qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'cycle'.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             param: Parameters of the gates. Defaults to None.
             param_sharing: Whether gates in the same layer share a parameter. Defaults to False.
 
         Raises:
             ValueError: The ``param`` must be paddle.Tensor or float.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(UniversalThreeQubits(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, 
-                                         depth, param, param_sharing))
+        self.append(UniversalThreeQubits(
+            qubits_idx, self.num_qubits, depth, param, param_sharing))
 
     def oracle(
-            self, oracle: paddle.tensor, qubits_idx: Union[Iterable[Iterable[int]], Iterable[int], int],
-            num_qubits: int = None, depth: int = 1,
+            self, oracle: paddle.tensor, qubits_idx: Union[Iterable[Iterable[int]], Iterable[int], int], depth: int = 1,
             gate_name: Optional[str] = 'O', latex_name: Optional[str] = None, plot_width: Optional[float] = None
     ) -> None:
         """Add an oracle gate.
 
         Args:
             oracle: Unitary oracle to be implemented.
             qubits_idx: Indices of the qubits on which the gates are applied.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             gate_name: name of this oracle.
             latex_name: latex name of this oracle, default to be the gate name.
             plot_width: width of this gate in circuit plot, default to be proportional with the gate name.
         """
         self.__num_qubits_update(qubits_idx)
-        gate_info = {'gatename': gate_name, 
-                     'texname': f"${gate_name}$" if latex_name is None else latex_name, 
-                     'plot_width': 0.6 * len(gate_name) if plot_width is None else plot_width}
-        self.append(Oracle(oracle, qubits_idx, 
-                           self.num_qubits if num_qubits is None else num_qubits, depth, gate_info))
+        gate_info = {
+            'gatename': gate_name,
+            'texname': f"${gate_name}$" if latex_name is None else latex_name,
+            'plot_width': 0.6 * len(gate_name) if plot_width is None else plot_width}
+        self.append(Oracle(
+            oracle, qubits_idx, self.num_qubits, depth, gate_info))
 
     def control_oracle(
-            self, oracle: paddle.Tensor, qubits_idx: Union[Iterable[Iterable[int]], Iterable[int]],
-            num_qubits: int = None, depth: int = 1, 
+            self, oracle: paddle.Tensor, qubits_idx: Union[Iterable[Iterable[int]], Iterable[int]], depth: int = 1,
             gate_name: Optional[str] = 'O', latex_name: Optional[str] = None, plot_width: Optional[float] = None
     ) -> None:
         """Add a controlled oracle gate.
 
         Args:
             oracle: Unitary oracle to be implemented.
             qubits_idx: Indices of the qubits on which the gates are applied.
-            num_qubits: Total number of qubits. Defaults to None.
             depth: Number of layers. Defaults to 1.
             gate_name: name of this oracle.
             latex_name: latex name of this oracle, default to be the gate name.
             plot_width: width of this gate in circuit plot, default to be proportional with the gate name.
         """
         self.__num_qubits_update(qubits_idx)
-        gate_info = {'gatename': f"c{gate_name}", 
-                     'texname': f"${gate_name}$" if latex_name is None else latex_name, 
-                     'plot_width': 0.6 * len(gate_name) if plot_width is None else plot_width}
-        self.append(ControlOracle(oracle, qubits_idx, 
-                                  self.num_qubits if num_qubits is None else num_qubits, depth, gate_info))
-        
-    def collapse(self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None,
+        gate_info = {
+            'gatename': f"c{gate_name}",
+            'texname': f"${gate_name}$" if latex_name is None else latex_name,
+            'plot_width': 0.6 * len(gate_name) if plot_width is None else plot_width}
+        self.append(ControlOracle(
+            oracle, qubits_idx, self.num_qubits, depth, gate_info))
+
+    def collapse(self, qubits_idx: Union[Iterable[int], int, str] = 'full',
                  desired_result: Union[int, str] = None, if_print: bool = False,
                  measure_basis: Union[Iterable[paddle.Tensor], str] = 'z') -> None:
         r"""
         Args:
             qubits_idx: list of qubits to be collapsed. Defaults to ``'full'``.
-            num_qubits: Total number of qubits. Defaults to ``None``.
             desired_result: The desired result you want to collapse. Defaults to ``None`` meaning randomly choose one.
             if_print: whether print the information about the collapsed state. Defaults to ``False``.
             measure_basis: The basis of the measurement. The quantum state will collapse to the corresponding eigenstate.
 
         Raises:
             NotImplementedError: If the basis of measurement is not z. Other bases will be implemented in future.
             TypeError: cannot get probability of state when the backend is unitary_matrix.
 
         Note:
             When desired_result is `None`, Collapse does not support gradient calculation
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(Collapse(qubits_idx, self.num_qubits if num_qubits is None else num_qubits,
-                             desired_result, if_print, measure_basis))
+        self.append(Collapse(
+            qubits_idx, self.num_qubits, desired_result, if_print, measure_basis))
 
     def superposition_layer(
-            self, qubits_idx: Iterable[int] = 'full', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Iterable[int] = None, depth: int = 1
     ) -> None:
         r"""Add layers of Hadamard gates.
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``None``.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            SuperpositionLayer(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
-        
+        self.extend(
+            SuperpositionLayer(qubits_idx, self.num_qubits, depth))
+
     def weak_superposition_layer(
-            self, qubits_idx: Iterable[int] = 'full', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Iterable[int] = None, depth: int = 1
     ) -> None:
         r"""Add layers of Ry gates with a rotation angle :math:`\pi/4`.
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``None``.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            WeakSuperpositionLayer(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
-        
+        self.extend(
+            WeakSuperpositionLayer(qubits_idx, self.num_qubits, depth))
+
     def linear_entangled_layer(
-            self, qubits_idx: Iterable[int] = 'full', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Iterable[int] = None, depth: int = 1
     ) -> None:
         r"""Add linear entangled layers consisting of Ry gates, Rz gates, and CNOT gates.
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``None``.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            LinearEntangledLayer(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.extend(
+            LinearEntangledLayer(qubits_idx, self.num_qubits, depth))
 
     def real_entangled_layer(
-            self, qubits_idx: Iterable[int] = 'full', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Iterable[int] = None, depth: int = 1
     ) -> None:
         r"""Add strongly entangled layers consisting of Ry gates and CNOT gates.
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``None``.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            RealEntangledLayer(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.extend(
+            RealEntangledLayer(qubits_idx, self.num_qubits, depth))
 
     def complex_entangled_layer(
-            self, qubits_idx: Iterable[int] = 'full', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Iterable[int] = None, depth: int = 1
     ) -> None:
         r"""Add strongly entangled layers consisting of single-qubit rotation gates and CNOT gates.
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``None``.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            ComplexEntangledLayer(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.extend(
+            ComplexEntangledLayer(qubits_idx, self.num_qubits, depth))
 
     def real_block_layer(
-            self, qubits_idx: Iterable[int] = 'full', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Iterable[int] = None, depth: int = 1
     ) -> None:
         r"""Add weakly entangled layers consisting of Ry gates and CNOT gates.
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``None``.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            RealBlockLayer(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
-    
+        self.extend(
+            RealBlockLayer(qubits_idx, self.num_qubits, depth))
+
     def complex_block_layer(
-            self, qubits_idx: Iterable[int] = 'full', num_qubits: int = None, depth: int = 1
+            self, qubits_idx: Iterable[int] = None, depth: int = 1
     ) -> None:
         r"""Add weakly entangled layers consisting of single-qubit rotation gates and CNOT gates.
 
         Args:
-            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
+            qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``None``.
             depth: Number of layers. Defaults to 1.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(
-            ComplexBlockLayer(qubits_idx, self.num_qubits if num_qubits is None else num_qubits, depth))
+        self.extend(
+            ComplexBlockLayer(qubits_idx, self.num_qubits, depth))
+
+    def qaoa_layer(self, edges: Iterable, nodes: Iterable, depth: Optional[int] = 1) -> None:
+        # TODO: see qaoa layer in layer.py
+        self.__num_qubits_update(edges)
+        self.__num_qubits_update(nodes)
+        self.extend(QAOALayer(edges, nodes, depth))
 
     def bit_flip(
-            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
+            self, prob: Union[paddle.Tensor, float],
+            qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add bit flip channels.
 
         Args:
             prob: Probability of a bit flip.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(BitFlip(prob, qubits_idx,
-                            self.num_qubits if num_qubits is None else num_qubits))
+        self.append(BitFlip(prob, qubits_idx, self.num_qubits))
 
     def phase_flip(
-        self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full',
-        num_qubits: int = None
+            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add phase flip channels.
 
         Args:
             prob: Probability of a phase flip.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
         self.append(PhaseFlip(prob, qubits_idx,
-                              self.num_qubits if num_qubits is None else num_qubits))
+                    self.num_qubits))
 
     def bit_phase_flip(
-            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full',
-            num_qubits: int = None
+            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add bit phase flip channels.
 
         Args:
             prob: Probability of a bit phase flip.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(BitPhaseFlip(prob, qubits_idx, 
-                                 self.num_qubits if num_qubits is None else num_qubits)) 
+        self.append(BitPhaseFlip(prob, qubits_idx, self.num_qubits))
 
     def amplitude_damping(
-            self, gamma: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
+            self, gamma: Union[paddle.Tensor, float],
+            qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add amplitude damping channels.
 
         Args:
             gamma: Damping probability.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(AmplitudeDamping(gamma, qubits_idx, 
-                                     self.num_qubits if num_qubits is None else num_qubits)) 
+        self.append(AmplitudeDamping(gamma, qubits_idx, self.num_qubits))
 
     def generalized_amplitude_damping(
             self, gamma: Union[paddle.Tensor, float], prob: Union[paddle.Tensor, float],
-            qubits_idx: Union[Iterable[int], int, str] = 'full',
-            num_qubits: int = None
+            qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add generalized amplitude damping channels.
 
         Args:
             gamma: Damping probability. Its value should be in the range :math:`[0, 1]`.
             prob: Excitation probability. Its value should be in the range :math:`[0, 1]`.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(GeneralizedAmplitudeDamping(gamma, prob, qubits_idx, 
-                                                self.num_qubits if num_qubits is None else num_qubits)) 
-        
+        self.append(GeneralizedAmplitudeDamping(
+            gamma, prob, qubits_idx, self.num_qubits))
+
     def phase_damping(
-            self, gamma: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full',
-            num_qubits: int = None
+            self, gamma: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add phase damping channels.
 
         Args:
             gamma: Parameter of the phase damping channel.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(PhaseDamping(gamma, qubits_idx, 
-                                 self.num_qubits if num_qubits is None else num_qubits)) 
+        self.append(PhaseDamping(gamma, qubits_idx, self.num_qubits))
 
     def depolarizing(
-            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full',
-            num_qubits: int = None
+            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add depolarizing channels.
 
         Args:
             prob: Parameter of the depolarizing channel.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(Depolarizing(prob, qubits_idx, 
-                                 self.num_qubits if num_qubits is None else num_qubits))
-        
+        self.append(Depolarizing(prob, qubits_idx, self.num_qubits))
+
     def generalized_depolarizing(
-            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str], 
-            num_qubits: int = None
+            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str]
     ) -> None:
         r"""Add a general depolarizing channel.
 
         Args:
             prob: Probabilities corresponding to the Pauli basis.
             qubits_idx: Indices of the qubits on which the channel is applied.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(PauliChannel(prob, qubits_idx, 
-                                 self.num_qubits if num_qubits is None else num_qubits))
+        self.append(GeneralizedDepolarizing(prob, qubits_idx, self.num_qubits))
 
     def pauli_channel(
-            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full',
-            num_qubits: int = None
+            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add Pauli channels.
 
         Args:
             prob: Probabilities corresponding to the Pauli X, Y, and Z operators.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(PauliChannel(prob, qubits_idx, 
-                                 self.num_qubits if num_qubits is None else num_qubits)) 
-        
+        self.append(PauliChannel(prob, qubits_idx, self.num_qubits))
+
     def reset_channel(
-            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full',
-            num_qubits: int = None
+            self, prob: Union[paddle.Tensor, float], qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add reset channels.
 
         Args:
             prob: Probabilities of resetting to :math:`|0\rangle` and to :math:`|1\rangle`.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(ResetChannel(prob, qubits_idx, 
-                                 self.num_qubits if num_qubits is None else num_qubits)) 
+        self.append(ResetChannel(prob, qubits_idx, self.num_qubits))
 
     def thermal_relaxation(
-            self, const_t: Union[paddle.Tensor, Iterable[float]], exec_time: Union[paddle.Tensor, float], 
-            qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
+            self, const_t: Union[paddle.Tensor, Iterable[float]], exec_time: Union[paddle.Tensor, float],
+            qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add thermal relaxation channels.
 
         Args:
             const_t: :math:`T_1` and :math:`T_2` relaxation time in microseconds.
             exec_time: Quantum gate execution time in the process of relaxation in nanoseconds.
             qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(ThermalRelaxation(const_t, exec_time, qubits_idx, 
-                                      self.num_qubits if num_qubits is None else num_qubits))
+        self.append(
+            ThermalRelaxation(const_t, exec_time, qubits_idx, self.num_qubits))
 
     def mixed_unitary_channel(
-            self, num_unitary: Union[paddle.Tensor, int], qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
+            self, num_unitary: Union[paddle.Tensor, int],
+            qubits_idx: Union[Iterable[int], int, str] = 'full'
     ) -> None:
         r"""Add mixed random unitary channels
 
         Args:
             num_unitary: The amount of random unitaries to be generated.
             qubits_idx: Indices of the qubits on which the channels act. Defaults to ``'full'``.
-            num_qubits: Total number of qubits. Defaults to ``None``.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(MixedUnitaryChannel(num_unitary, qubits_idx,
-                                        self.num_qubits if num_qubits is None else num_qubits))
+        self.append(MixedUnitaryChannel(num_unitary, qubits_idx, self.num_qubits))
+
+    def choi_channel(
+            self, choi_repr: Iterable[paddle.Tensor],
+            qubits_idx: Union[Iterable[Iterable[int]], Iterable[int], int]
+    ) -> None:
+        r"""Add custom channels in the Choi representation.
+
+        Args:
+            choi_repr: Choi representation of this channel.
+            qubits_idx: Indices of the qubits on which the channels are applied.
+        """
+        self.__num_qubits_update(qubits_idx)
+        self.append(ChoiRepr(choi_repr, qubits_idx, self.num_qubits))
 
-    def kraus_repr(
+    def kraus_channel(
             self, kraus_oper: Iterable[paddle.Tensor],
-            qubits_idx: Union[Iterable[Iterable[int]], Iterable[int], int],
-            num_qubits: int = None
+            qubits_idx: Union[Iterable[Iterable[int]], Iterable[int], int]
     ) -> None:
         r"""Add custom channels in the Kraus representation.
 
         Args:
-            kraus_oper: Kraus operators of this channel.
-            qubits_idx: Indices of the qubits on which the channels are applied. Defaults to 'full'.
-            num_qubits: Total number of qubits. Defaults to None.
+            kraus_oper: Kraus representation of this channel.
+            qubits_idx: Indices of the qubits on which the channels are applied.
         """
         self.__num_qubits_update(qubits_idx)
-        self.append(KrausRepr(kraus_oper, qubits_idx, 
-                              self.num_qubits if num_qubits is None else num_qubits))
+        self.append(KrausRepr(kraus_oper, qubits_idx, self.num_qubits))
 
-    def qaoa_layer(self, edges: Iterable, nodes: Iterable, depth: Optional[int] = 1) -> None:
-        # TODO: see qaoa layer in layer.py
-        self.__num_qubits_update(edges)
-        self.__num_qubits_update(nodes)
-        self.append(QAOALayer(edges, nodes, depth))
-
-    def unitary_matrix(self, num_qubits: Optional[int] = None) -> paddle.Tensor:
-        r"""Get the unitary matrix form of the circuit.
+    def stinespring_channel(
+            self, stinespring_repr: Iterable[paddle.Tensor],
+            qubits_idx: Union[Iterable[Iterable[int]], Iterable[int], int]
+    ) -> None:
+        r"""Add custom channels in the Stinespring representation.
 
         Args:
-            num_qubits: Total number of qubits. Defaults to None.
+            stinespring_repr: Stinespring representation of this channel.
+            qubits_idx: Indices of the qubits on which the channels are applied.
+        """
+        self.__num_qubits_update(qubits_idx)
+        self.append(
+            StinespringRepr(stinespring_repr, qubits_idx, self.num_qubits))
+
+    def unitary_matrix(self) -> paddle.Tensor:
+        r"""Get the unitary matrix form of the circuit.
 
         Returns:
             Unitary matrix form of the circuit.
         """
-        if num_qubits is None:
-            num_qubits = self.__num_qubits
-        else:
-            assert num_qubits >= self.__num_qubits
-
         backend = get_backend()
         self.to(backend=Backend.UnitaryMatrix)
-        unitary = State(paddle.eye(2 ** num_qubits).cast(get_dtype()), 
-                        backend=Backend.UnitaryMatrix)
+        unitary = State(paddle.eye(
+            2 ** self.num_qubits).cast(get_dtype()), backend=Backend.UnitaryMatrix)
         for layer in self._sub_layers.values():
             unitary = layer(unitary)
         self.to(backend=backend)
         return unitary.data
 
     @property
     def gate_history(self) -> List[Dict[str, Union[str, List[int], paddle.Tensor]]]:
-        r""" list of gates information of circuit
+        r"""List of gates information of circuit
 
         Returns:
             history of quantum gates of circuit
 
         """
         gate_history = []
-        for gate in self.sublayers():
-            if gate.gate_info['gatename'] is None:
-                raise NotImplementedError(f"Gate {type(gate)} has no gate name and hence cannot be recorded into history.")
+        for op in self.sublayers():
+            if isinstance(op, Layer):
+                gate_history.extend(op.gate_history)
             else:
-                gate.gate_history_generation()
-                gate_history.extend(gate.gate_history)
+                if op.gate_info['gatename'] is None:
+                    raise NotImplementedError(
+                        f"{type(op)} has no gate name and hence cannot be recorded into history.")
+                op.gate_history_generation()
+                gate_history.extend(op.gate_history)
         return gate_history
 
+    @property
+    def depth(self) -> int:
+        r"""Depth of gate sequences.
+        
+        Returns:
+            depth of this circuit
+        
+        Note:
+            The measurement is omitted, and all gates are assumed to have depth 1. 
+            See Niel's answer in the [StackExchange](https://quantumcomputing.stackexchange.com/a/5772).
+        
+        """
+        qubit_depth = np.array([0] * self.num_qubits)
+        for gate_info in self.gate_history:
+            qubits_idx = gate_info['which_qubits']
+            if isinstance(qubits_idx, int):
+                qubit_depth[qubits_idx] += 1
+            else:
+                qubit_depth[qubits_idx] = np.max(qubit_depth[qubits_idx]) + 1
+        return int(np.max(qubit_depth))
+
     def __count_history(self, history):
         # Record length of each section
         length = [5]
         n = self.__num_qubits
         # Record current section number for every qubit
         qubit = [0] * n
         # Number of sections
         qubit_max = max(qubit)
         # Record section number for each gate
         gate = []
-
         for current_gate in history:
             # Single-qubit gates with no params to print
             if current_gate['gate'] in {'h', 's', 't', 'x', 'y', 'z', 'u', 'sdg', 'tdg'}:
                 curr_qubit = current_gate['which_qubits']
                 gate.append(qubit[curr_qubit])
                 qubit[curr_qubit] = qubit[curr_qubit] + 1
                 # A new section is added
@@ -1470,23 +1434,25 @@
                 gate.append(qubit[curr_qubit])
                 if length[qubit[curr_qubit]] == 5:
                     length[qubit[curr_qubit]] = 13
                 qubit[curr_qubit] = qubit[curr_qubit] + 1
                 if qubit[curr_qubit] > qubit_max:
                     length.append(5)
                     qubit_max = qubit[curr_qubit]
-            elif current_gate['gate'] in {'cnot', 'swap', 'rxx', 'ryy', 'rzz', 'ms', 
-                                          'cy', 'cz', 'cu', 'cp', 'crx', 'cry', 'crz', 
-                                          'cswap', 'ccx'}:
+            elif current_gate['gate'] in {
+                'cnot', 'swap', 'rxx', 'ryy', 'rzz', 'ms',
+                'cy', 'cz', 'cu', 'cp', 'crx', 'cry', 'crz', 'cswap', 'ccx'
+            }:
                 a = max(current_gate['which_qubits'])
                 b = min(current_gate['which_qubits'])
                 ind = max(qubit[b: a + 1])
                 gate.append(ind)
-                if length[ind] < 13 and current_gate['gate'] in {'rxx', 'ryy', 'rzz',
-                                                                 'cp', 'crx', 'cry', 'crz'}:
+                if length[ind] < 13 and current_gate['gate'] in {
+                    'rxx', 'ryy', 'rzz', 'cp', 'crx', 'cry', 'crz'
+                }:
                     length[ind] = 13
                 for j in range(b, a + 1):
                     qubit[j] = ind + 1
                 if ind + 1 > qubit_max:
                     length.append(5)
                     qubit_max = ind + 1
 
@@ -1494,45 +1460,44 @@
 
     @property
     def qubit_history(self) -> List[List[Tuple[Dict[str, Union[str, List[int], paddle.Tensor]], int]]]:
         r""" gate information on each qubit
 
         Returns:
             list of gate history on each qubit
-        
+
         Note:
             The entry ``qubit_history[i][j][0/1]`` returns the gate information / gate index of the j-th gate
             applied on the i-th qubit.
         """
         history_qubit = [[] for _ in range(self.num_qubits)]
         for idx, i in enumerate(self.gate_history):
             qubits = i["which_qubits"]
             if not isinstance(qubits, Iterable):
                 history_qubit[qubits].append([i, idx])
             else:
                 for j in qubits:
                     history_qubit[j].append([i, idx])
         return history_qubit
 
-    def __str__(self) -> str:
+    def __str__(self):
         history = self.gate_history
         num_qubits = self.__num_qubits
         length, gate = self.__count_history(history)
         # Ignore the unused section
         total_length = sum(length) - 5
-
-        print_list = [['-' if i % 2 == 0 else ' '] * 
+        print_list = [['-' if i % 2 == 0 else ' '] *
                       total_length for i in range(num_qubits * 2)]
-
         for i, current_gate in enumerate(history):
             if current_gate['gate'] in {'h', 's', 't', 'x', 'y', 'z', 'u'}:
                 # Calculate starting position ind of current gate
                 sec = gate[i]
                 ind = sum(length[:sec])
-                print_list[current_gate['which_qubits'] * 2][ind + length[sec] // 2] = current_gate['gate'].upper()
+                print_list[current_gate['which_qubits'] * 2][ind +
+                                                             length[sec] // 2] = current_gate['gate'].upper()
             elif current_gate['gate'] in {'sdg'}:
                 sec = gate[i]
                 ind = sum(length[:sec])
                 print_list[current_gate['which_qubits'] * 2][
                     ind + length[sec] // 2 - 1: ind + length[sec] // 2 + 2] = current_gate['gate'].upper()
             elif current_gate['gate'] in {'tdg'}:
                 sec = gate[i]
@@ -1548,51 +1513,66 @@
                 if current_gate['gate'] == 'p':
                     print_list[line][ind + 2] = 'P'
                     print_list[line][ind + 3] = ' '
                 else:
                     print_list[line][ind + 2] = 'R'
                     print_list[line][ind + 3] = current_gate['gate'][1]
                 print_list[line][ind + 4] = '('
-                print_list[line][ind + 5: ind + 10] = format(float(param.numpy()), '.3f')[:5]
+                print_list[line][ind + 5: ind +
+                                 10] = format(float(param.numpy()), '.3f')[:5]
                 print_list[line][ind + 10] = ')'
             # Two-qubit gates
             elif current_gate['gate'] in {'cnot', 'swap', 'rxx', 'ryy', 'rzz', 'ms', 'cz', 'cy',
-                                          'cu', 'crx', 'cry', 'crz'}:
+                                          'cu', 'cp', 'crx', 'cry', 'crz'}:
                 sec = gate[i]
                 ind = sum(length[:sec])
                 cqubit = current_gate['which_qubits'][0]
                 tqubit = current_gate['which_qubits'][1]
                 if current_gate['gate'] in {'cnot', 'swap', 'cy', 'cz', 'cu'}:
                     print_list[cqubit * 2][ind + length[sec] // 2] = \
-                        '*' if current_gate['gate'] in {'cnot', 'cy', 'cz', 'cu'} else 'x'
+                        '*' if current_gate['gate'] in {'cnot',
+                                                        'cy', 'cz', 'cu'} else 'x'
                     print_list[tqubit * 2][ind + length[sec] // 2] = \
-                        'x' if current_gate['gate'] in {'swap', 'cnot'} else current_gate['gate'][1]
+                        'x' if current_gate['gate'] in {
+                            'swap', 'cnot'} else current_gate['gate'][1]
                 elif current_gate['gate'] == 'ms':
                     for qubit in {cqubit, tqubit}:
                         print_list[qubit * 2][ind + length[sec] // 2 - 1] = 'M'
                         print_list[qubit * 2][ind + length[sec] // 2] = '_'
                         print_list[qubit * 2][ind + length[sec] // 2 + 1] = 'S'
                 elif current_gate['gate'] in {'rxx', 'ryy', 'rzz'}:
                     # param = self.__param[current_gate['theta'][0]]
                     param = current_gate['theta']
                     for line in {cqubit * 2, tqubit * 2}:
                         print_list[line][ind + 2] = 'R'
-                        print_list[line][ind + 3: ind + 5] = current_gate['gate'][1:3].lower()
+                        print_list[line][ind + 3: ind +
+                                         5] = current_gate['gate'][1:3].lower()
                         print_list[line][ind + 5] = '('
-                        print_list[line][ind + 6: ind + 10] = format(float(param.numpy()), '.2f')[:4]
+                        print_list[line][ind + 6: ind +
+                                         10] = format(float(param.numpy()), '.2f')[:4]
                         print_list[line][ind + 10] = ')'
                 elif current_gate['gate'] in {'crx', 'cry', 'crz'}:
-                    # param = self.__param[current_gate['theta'][2 if current_gate['gate'] == 'crz' else 0]]
                     param = current_gate['theta']
                     print_list[cqubit * 2][ind + length[sec] // 2] = '*'
                     print_list[tqubit * 2][ind + 2] = 'R'
                     print_list[tqubit * 2][ind + 3] = current_gate['gate'][2]
                     print_list[tqubit * 2][ind + 4] = '('
-                    print_list[tqubit * 2][ind + 5: ind + 10] = format(float(param.numpy()), '.3f')[:5]
+                    print_list[tqubit * 2][ind + 5: ind +
+                                           10] = format(float(param.numpy()), '.3f')[:5]
+                    print_list[tqubit * 2][ind + 10] = ')'
+                elif current_gate['gate'] == 'cp':
+                    param = current_gate['theta']
+                    print_list[cqubit * 2][ind + length[sec] // 2] = '*'
+                    print_list[tqubit * 2][ind + 2] = ' '
+                    print_list[tqubit * 2][ind + 3] = 'P'
+                    print_list[tqubit * 2][ind + 4] = '('
+                    print_list[tqubit * 2][ind + 5: ind +
+                                           10] = format(float(param.numpy()), '.3f')[:5]
                     print_list[tqubit * 2][ind + 10] = ')'
+                    
                 start_line = min(cqubit, tqubit)
                 end_line = max(cqubit, tqubit)
                 for k in range(start_line * 2 + 1, end_line * 2):
                     print_list[k][ind + length[sec] // 2] = '|'
             # Three-qubit gates
             elif current_gate['gate'] in {'cswap'}:
                 sec = gate[i]
@@ -1619,96 +1599,103 @@
                 for k in range(start_line * 2 + 1, end_line * 2):
                     print_list[k][ind + length[sec] // 2] = '|'
                 if current_gate['gate'] in {'ccx'}:
                     print_list[cqubit1 * 2][ind + length[sec] // 2] = '*'
                     print_list[cqubit2 * 2][ind + length[sec] // 2] = '*'
                     print_list[tqubit * 2][ind + length[sec] // 2] = 'X'
             else:
-                raise NotImplementedError(f"Not support to print the gate {current_gate['gate']}.")
+                raise NotImplementedError(
+                    f"Not support to print the gate {current_gate['gate']}.")
 
         print_list = list(map(''.join, print_list))
         return_str = '\n'.join(print_list)
 
         return return_str
-    
-    def plot(self, 
-             save_path: Optional[str] = None, 
-             dpi: Optional[int] = 100, 
-             show: Optional[bool] = True, 
-             output: Optional[bool] = False,
-             scale: Optional[float] = 1.0,
-             tex: Optional[bool] = False,
-             ) -> Union[None, matplotlib.figure.Figure]:
+
+    def plot(
+            self,
+            save_path: Optional[str] = None,
+            dpi: Optional[int] = 100,
+            show: Optional[bool] = True,
+            output: Optional[bool] = False,
+            scale: Optional[float] = 1.0,
+            tex: Optional[bool] = False,
+    ) -> Union[None, matplotlib.figure.Figure]:
         r'''display the circuit using matplotlib
 
         Args:
             save_path: the save path of image
             dpi: dots per inches, here is resolution ratio
             show: whether execute ``plt.show()``
             output: whether return the ``matplotlib.figure.Figure`` instance
             scale: scale coefficient of figure, default to 1.0
-            tex: a bool flag which controls latex fonts of gate display, default to ``False``. 
+            tex: a bool flag which controls latex fonts of gate display, default to ``False``.
 
         Returns:
             a ``matplotlib.figure.Figure`` instance or ``None`` depends on ``output``
-        
+
         Note:
             Using ``plt.show()`` may cause a distortion, but it will not happen in the figure saved.
             If the depth is too long, there will be some patches unable to display.
             Setting ``tex = True`` requires that you have TeX and the other dependencies properly 
             installed on your system. See 
             https://matplotlib.org/stable/gallery/text_labels_and_annotations/tex_demo.html
             for more details.
         '''
-        _fig = _circuit_plot(self, dpi=dpi, scale=scale, tex = tex)
-
-        if save_path:  
-            plt.savefig(save_path, dpi=dpi,) 
-
-        if show:    # whether display in window
+        _fig = _circuit_plot(self, dpi=dpi, scale=scale, tex=tex)
+        if save_path:
+            plt.savefig(save_path, dpi=dpi, )
+        if show:  # whether display in window
             plt.show()
+        if output:
+            return _fig  # return the ``matplotlib.pyplot.figure`` instance
 
-        if output:  
-            return _fig    # return the ``matplotlib.pyplot.figure`` instance
-    
     def extend(self, cir):
         r""" extend for quantum circuit
-        
+
         Args:
             cir: a Circuit or a Sequential
-            
+
         Returns:
             concatenation of two quantum circuits
-        
         """
         if isinstance(cir, Circuit):
             if self.__num_qubits is None:
                 self.__num_qubits = cir.num_qubits
             else:
-                self.__num_qubits = self.__num_qubits if cir.num_qubits is None else max(self.__num_qubits, cir.num_qubits)
+                self.__num_qubits = self.__num_qubits if cir.num_qubits is None else max(self.__num_qubits,
+                                                                                         cir.num_qubits)
             super().extend(cir)
         elif isinstance(cir, Sequential):
             super().extend(cir)
         else:
             raise TypeError("the input type must be Circuit or Sequential")
-    
+
     def forward(self, state: Optional[State] = None) -> State:
         r""" forward the input
-        
+
         Args:
             state: initial state
-            
+
         Returns:
             output quantum state
-        
         """
         assert self.__num_qubits is not None, "Information about num_qubits is required before running the circuit"
-        
+
         if state is None:
             state = zero_state(self.__num_qubits, self.backend, self.dtype)
         else:
             assert self.__num_qubits == state.num_qubits, \
                 f"num_qubits does not agree: expected {self.__num_qubits}, received {state.num_qubits}"
-            
-        return super().forward(state)
-    
-    
+
+        if self.backend == Backend.QuLeaf and state.backend == Backend.QuLeaf:
+            state.oper_history = self.oper_history
+            return state
+
+        state = state.clone()
+        state.is_swap_back = False
+        state = super().forward(state)
+
+        # reset state in the original qubit sequence
+        state.reset_sequence()
+        state.is_swap_back = True
+        return state
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/ansatz/container.py` & `paddle-quantum-2.4.0/paddle_quantum/ansatz/container.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,146 +14,169 @@
 # limitations under the License.
 
 r"""
 The source file of the Sequential class.
 """
 
 import collections
-from paddle_quantum import Operator
-from typing import Optional, Union, Iterable, Any, List
+import warnings
+import paddle
+import paddle_quantum as pq
+from typing import Optional, Union, Iterable, Any, List, Dict
 
 
-class Sequential(Operator):
+class Sequential(pq.Operator):
     r"""Sequential container.
 
     Args:
         *operators: initial operators ready to be a sequential
-    
+
     Note:
         Sublayers will be added to this container in the order of argument in the constructor.
         The argument passed to the constructor can be iterable Layers or iterable name Layer pairs.
-    
     """
-    def __init__(self, *operators: Operator):
+    def __init__(self, *operators: pq.Operator):
         super().__init__()
         self.index = 0
-        if len(operators) > 0 and isinstance(operators[0], (list, tuple)):
+        if operators and isinstance(operators[0], (list, tuple)):
             for name, oper in operators:
                 self.add_sublayer(name, oper)
         else:
             for idx, oper in enumerate(operators):
                 self.add_sublayer(str(idx), oper)
 
-    def __getitem__(self, name: Union[str, slice]) -> Operator:
+    def __getitem__(self, name: Union[str, slice]) -> pq.Operator:
         if isinstance(name, slice):
             return self.__class__(*(list(self._sub_layers.values())[name]))
         if isinstance(name, str):
             return self._sub_layers[name]
         if name >= len(self._sub_layers):
             raise IndexError(f'index {name:s} is out of range')
         if 0 > name >= -len(self._sub_layers):
             name += len(self._sub_layers)
         elif name < -len(self._sub_layers):
             raise IndexError(f'index {name:s} is out of range')
         return self._sub_layers[str(name)]
 
-    def __setitem__(self, name: Any, layer: Operator) -> None:
-        assert isinstance(layer, Operator)
+    def __setitem__(self, name: Any, layer: pq.Operator) -> None:
+        assert isinstance(layer, pq.Operator)
         setattr(self, str(name), layer)
 
     def __delitem__(self, name: Any) -> None:
         name = str(name)
         assert name in self._sub_layers
         del self._sub_layers[name]
 
     def __iter__(self):
         return self
 
-    def __next__(self) -> Union[Operator, StopIteration]:
+    def __next__(self) -> Union[pq.Operator, StopIteration]:
         if self.index < len(self._sub_layers):
             oper = self._sub_layers[str(self.index)]
             self.index += 1
             return oper
         self.index = 0
         raise StopIteration
 
     def __len__(self):
         return len(self._sub_layers)
+    
+    @property
+    def oper_history(self) -> List[Dict[str, Union[str, List[int], paddle.Tensor]]]:
+        r"""Return the operator history of this Sequential
+        """
+        oper_history = []
+        for op in self.sublayers():
+            if isinstance(op, pq.gate.ParamGate):
+                oper_history.append({
+                    'name': op.__class__.__name__,
+                    'qubits_idx': op.qubits_idx,
+                    'depth': op.depth,
+                    'param': op.theta,
+                    'param_sharing': op.param_sharing
+                })
+            elif hasattr(op, 'qubits_idx'):
+                oper_history.append({
+                    'name': op.__class__.__name__,
+                    'qubits_idx': op.qubits_idx,
+                    'depth': op.depth if hasattr(op, 'depth') else 1
+                })
+            else:
+                warnings.warn(
+                    f"Cannot recognize the operator: expected an operator with attribute qubits_idx, received {type(op)}.", UserWarning)
+                oper_history.append(None)
+        return oper_history
 
-    def append(self, operator: Union[Iterable, Operator]) -> None:
+    # TODO: append only a operator, don't allow to append a list of operators
+    def append(self, operator: Union[Iterable, pq.Operator]) -> None:
         r""" append an operator
-        
+
         Args:
             operator: operator with a name or just an operator
-        
         """
-        if isinstance(operator, Operator):
+        if isinstance(operator, pq.Operator):
             idx = len(self._sub_layers)
             self.add_sublayer(str(idx), operator)
         elif isinstance(operator, Iterable):
             name, oper = operator
             self.add_sublayer(name, oper)
 
-
-    def extend(self, operators: List[Operator]) -> None:
+    def extend(self, operators: List[pq.Operator]) -> None:
         r""" append a list of operators
-        
+
         Args:
             operator: list of operators
-        
         """
-        if len(operators) > 0 and isinstance(operators[0], (list, tuple)):
+        if operators and isinstance(operators[0], (list, tuple)):
             for name, oper in operators:
                 self.add_sublayer(name, oper)
         else:
             origin_len = len(self._sub_layers)
             for idx, oper in enumerate(operators):
                 self.add_sublayer(str(idx + origin_len), oper)
 
-    def insert(self, index: int, operator: Operator) -> None:
+    def insert(self, index: int, operator: pq.Operator) -> None:
         r""" insert an operator at ``index``
-        
+
         Args:
             index: index to be inserted
             operator: an operator
-        
         """
         new_operators = collections.OrderedDict()
-        assert index <= len(self._sub_layers), 'the index ' + str(index) + ' should be no more than ' + str(len(self._sub_layers))
+        assert index <= len(self._sub_layers), f'the index {index} should be no more than {len(self._sub_layers)}'
         if index == len(self._sub_layers):
             self.append(operator)
         for idx, name in enumerate(self._sub_layers):
             if idx < index:
                 new_operators[name] = self._sub_layers[name]
             elif idx == index:
                 if isinstance(operator, (list, tuple)):
                     name, oper = operator
                     new_operators[name] = oper
-                elif isinstance(operator, Operator):
+                elif isinstance(operator, pq.Operator):
                     new_operators[str(index)] = operator
                 if name.isdigit():
                     new_operators[str(int(name) + 1)] = self._sub_layers[name]
                 else:
                     new_operators[name] = self._sub_layers[name]
             elif name.isdigit():
                 new_operators[str(int(name) + 1)] = self._sub_layers[name]
             else:
                 new_operators[name] = self._sub_layers[name]
         self._sub_layers = new_operators
 
-    def pop(self, index: int = None, operator:  Optional[Operator] = None):
+    def pop(self, index: int = None, operator:  Optional[pq.Operator] = None):
         r""" remove the operator at ``index`` or matched with ``operator``
-        
+
         Args:
             index: at which the operator will be popped
             operator: matched with which the operator will be popped
-        
         """
         if index is not None:
-            assert index < len(self._sub_layers), 'the index ' + str(index) + ' should be less than ' + str(len(self._sub_layers))
+            assert index < len(self._sub_layers), f'the index {index} should be less than {len(self._sub_layers)}'
             if isinstance(index, int):
                 index = str(index)
             operator = self._sub_layers[index]
         if operator is None:
             raise ValueError("The index or operator must be input.")
         new_operators = collections.OrderedDict()
         behind_operator = False
@@ -163,21 +186,20 @@
             elif not behind_operator:
                 new_operators[name] = self._sub_layers[name]
             elif name.isdigit():
                 new_operators[str(int(name) - 1)] = self._sub_layers[name]
             else:
                 new_operators[name] = self._sub_layers[name]
         self._sub_layers = new_operators
-
+        
     def forward(self, state: Any) -> Any:
         r""" forward the input
-        
+
         Args:
             state: initial state
-            
+
         Returns:
             output state
-        
-        """        
+        """
         for layer in self._sub_layers.values():
             state = layer(state)
         return state
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/ansatz/vans.py` & `paddle-quantum-2.4.0/paddle_quantum/ansatz/vans.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         param = gate_info['theta']
         # get gate function
         if param is None:
             getattr(new_cir, gate_name)(qubits_idx)
             continue
         
         if trainable:
-            param = param.reshape([1] + param.shape)
+            param = param.reshape([1] + [1] + param.shape)
             param = paddle.create_parameter(
                 shape=param.shape, dtype=param.dtype,
                 default_initializer=paddle.nn.initializer.Assign(param))
         getattr(new_cir, gate_name)(qubits_idx, param=param)
     return new_cir
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/backend/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/backend/density_matrix.py` & `paddle-quantum-2.4.0/paddle_quantum/backend/state_vector.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,37 +10,39 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
-The source file of the density_matrix backend.
+The source file of the state_vector backend.
 """
 
 import paddle
-from typing import List, Iterable, Union
+import numpy as np
+import paddle_quantum as pq
+from typing import List, Iterable, Union, Tuple
 
 
 def unitary_transformation(
         state: paddle.Tensor, gate: paddle.Tensor, qubit_idx: Union[List[int], int], num_qubits: int
 ) -> paddle.Tensor:
-    r"""The function of unitary transformation in the mode of density matrix.
+    r"""The function of unitary transformation in the mode of state vector.
 
     Args:
         state: The input quantum state.
         gate: The gate that represents the unitary transformation.
         qubit_idx: The indices of the qubits on which the gate is acted.
         num_qubits: The number of the qubits in the input quantum state.
 
     Returns:
         The transformed quantum state.
     """
     # The order of the tensor in paddle is less than 10.
-    higher_dims = state.shape[:-2]
+    higher_dims = state.shape[:-1]
     num_higher_dims = len(higher_dims)
 
     if not isinstance(qubit_idx, Iterable):
         qubit_idx = [qubit_idx]
 
     # generate swap_list
     num_acted_qubits = len(qubit_idx)
@@ -55,76 +57,74 @@
             while not swapped[seq_for_acted[next_idx]]:
                 swapped[seq_for_acted[next_idx]] = True
                 if next_idx < seq_for_acted[next_idx]:
                     swap_ops.append((next_idx, seq_for_acted[next_idx]))
                 else:
                     swap_ops.append((seq_for_acted[next_idx], next_idx))
                 next_idx = seq_for_acted[next_idx]
-
     for swap_op in swap_ops:
         shape = higher_dims.copy()
         last_idx = -1
         for idx in swap_op:
             shape.append(2 ** (idx - last_idx - 1))
             shape.append(2)
             last_idx = idx
-        shape.append(2 ** (2 * num_qubits - last_idx - 1))
+        shape.append(2 ** (num_qubits - last_idx - 1))
         state = paddle.reshape(state, shape)
         state = paddle.transpose(
-            state, list(range(0, num_higher_dims)) + [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
+            state, list(range(0, num_higher_dims)) +
+            [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
         )
-    state = paddle.reshape(
-        state, higher_dims.copy() + [2 ** num_acted_qubits, 2 ** (2 * num_qubits - num_acted_qubits)]
-    )
+    state = paddle.reshape(state, higher_dims.copy(
+    ) + [2 ** num_acted_qubits, 2 ** (num_qubits - num_acted_qubits)])
     state = paddle.matmul(gate, state)
     swap_ops.reverse()
     for swap_op in swap_ops:
         shape = higher_dims.copy()
         last_idx = -1
         for idx in swap_op:
             shape.append(2 ** (idx - last_idx - 1))
             shape.append(2)
             last_idx = idx
-        shape.append(2 ** (2 * num_qubits - last_idx - 1))
-        state = paddle.reshape(state, shape)
-        state = paddle.transpose(
-            state, list(range(0, num_higher_dims)) + [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
-        )
-    swap_ops.reverse()
-    for idx, swap_op in enumerate(swap_ops):
-        swap_ops[idx] = (swap_op[0] + num_qubits, swap_op[1] + num_qubits)
-    for swap_op in swap_ops:
-        shape = higher_dims.copy()
-        last_idx = - 1
-        for idx in swap_op:
-            shape.append(2 ** (idx - last_idx - 1))
-            shape.append(2)
-            last_idx = idx
-        shape.append(2 ** (2 * num_qubits - last_idx - 1))
+        shape.append(2 ** (num_qubits - last_idx - 1))
         state = paddle.reshape(state, shape)
         state = paddle.transpose(
-            state, list(range(0, num_higher_dims)) + [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
-        )
-    state = paddle.reshape(
-        state, higher_dims.copy() + [2 ** num_qubits, 2 ** num_acted_qubits, 2 ** (num_qubits - num_acted_qubits)]
-    )
-    # gate_dagger = paddle.conj(paddle.t(gate))
-    # state = paddle.einsum('abc,bx->axc', state, gate_dagger)
-    # The computation below is equivalent to the einsum above.
-    gate_dagger = paddle.conj(gate)
-    state = paddle.matmul(gate_dagger, state)
-    swap_ops.reverse()
-    for swap_op in swap_ops:
-        shape = higher_dims.copy()
-        last_idx = - 1
-        for idx in swap_op:
-            shape.append(2 ** (idx - last_idx - 1))
-            shape.append(2)
-            last_idx = idx
-        shape.append(2 ** (2 * num_qubits - last_idx - 1))
-        state = paddle.reshape(state, shape)
-        state = paddle.transpose(
-            state, list(range(0, num_higher_dims)) + [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
+            state, list(range(0, num_higher_dims)) +
+            [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
         )
 
-    state = paddle.reshape(state, higher_dims.copy() + [2 ** num_qubits, 2 ** num_qubits])
+    state = paddle.reshape(state, higher_dims.copy() + [2 ** num_qubits])
     return state
+
+
+def unitary_transformation_without_swapback(
+        state: paddle.Tensor, gate: List[paddle.Tensor], qubit_idx: List[int], num_qubits: int, qubit_sequence: List[int]
+) -> Tuple[paddle.Tensor, List[int]]:
+    r"""The function of unitary transformation in the mode of state vector.
+
+    Args:
+        state: The input quantum state.
+        gate: The list of gates that represents the unitary transformation.
+        qubit_idx: The list of indices of the qubits on which the gate is acted.
+        num_qubits: The number of the qubits in the input quantum state.
+        qubit_sequence: The sequence of qubit indices at this moment.
+
+    Returns:
+        The transformed quantum state.
+    """
+    # The order of the tensor in paddle is less than 10.
+    higher_dims = state.shape[:-1]
+    gate = pq.intrinsic._gate_tensor(gate)
+
+    # generate base index order
+    num_acted_qubits = len(qubit_idx)
+    seq_for_acted = qubit_idx + \
+        [x for x in qubit_sequence if x not in qubit_idx]
+    perm_map = pq.intrinsic._perm_of_list(qubit_sequence, seq_for_acted)
+    state = pq.intrinsic._base_transpose(state, perm_map)
+
+    # matrix multiplication
+    state = paddle.reshape(state, higher_dims.copy(
+    ) + [2 ** num_acted_qubits, 2 ** (num_qubits - num_acted_qubits)])
+    state = paddle.matmul(gate, state)
+    state = paddle.reshape(state, higher_dims.copy() + [2 ** num_qubits])
+    return state, seq_for_acted
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/backend/quleaf.py` & `paddle-quantum-2.4.0/paddle_quantum/backend/quleaf.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 
 import copy
 import math
 import numpy as np
 import paddle
 import QCompute
 import re
+import paddle_quantum as pq
 from QCompute import MeasureZ, RX, RY
-import paddle_quantum
+from typing import Optional, List
 
 BACKEND = 'local_baidu_sim2'
 TOKEN = None
 QCompute.Define.Settings.outputInfo = False
 QCompute.Define.Settings.drawCircuitControl = []
 
 
@@ -71,91 +72,103 @@
 
     Returns:
         The token you set.
     """
     return TOKEN
 
 
-def _act_gates_to_state(gate_history: list, quleaf_state: QCompute.QEnv, param_all: list) -> QCompute.QEnv:
+single_qubit_gates = {
+    'S': QCompute.S, 'T': QCompute.T, 'Sdg': QCompute.SDG, 'Tdg': QCompute.TDG,
+    'H': QCompute.H, 'X': QCompute.X, 'Y': QCompute.Y, 'Z': QCompute.Z,
+    'U3': QCompute.U, 'RX': QCompute.RX, 'RY': QCompute.RY, 'RZ': QCompute.RZ
+}
+multi_qubits_gates = {
+    'CNOT': QCompute.CX, 'CX': QCompute.CX, 'CY': QCompute.CY, 'CZ': QCompute.CZ, 'SWAP': QCompute.SWAP,
+    'CU': QCompute.CU, 'CRX': QCompute.CRX, 'CRY': QCompute.CRY, 'CRZ': QCompute.CRZ,
+    'CSWAP': QCompute.CSWAP, 'CCX': QCompute.CCX
+}
+fixed_gates = {'S', 'T', 'Sdg', 'Tdg', 'H', 'X', 'Y', 'Z', 'CNOT', 'CX', 'CY', 'CZ', 'SWAP', 'CSWAP', 'CCX'}
+parameterized_gates = {'U3', 'RX', 'RY', 'RZ', 'CU', 'CRX', 'CRY', 'CRZ'}
+
+
+# TODO: need to check whether the logic is right when the param_sharing is True.
+def _act_gates_to_state(
+        oper_history: List[dict], quleaf_state: QCompute.QEnv,
+        _gate_idx: Optional[int] = None, _depth_idx: Optional[int] = None, _qubits_idx: Optional[int] = None,
+        _param_idx: Optional[int] = None, _param_shift_val: Optional[int] = None
+) -> QCompute.QEnv:
     r"""The function to act the quantum gate to the quantum state in the QuLeaf backend.
 
     Args:
-        gate_history: The history of quantum gate, which records the type, parameters and qubits index of the gates.
+        oper_history: The history of quantum gate, which records the type, parameters and qubits index of the gates.
         quleaf_state: The quantum state in QuLeaf.
         param_all: All the parameters in the gates.
 
     Raises:
         NotImplementedError: Some quantum gate is not supported in QuLeaf yet.
 
     Returns:
         The acted quantum state.
     """
-    single_qubit_gates = {
-        's': QCompute.S, 't': QCompute.T, 'sdg': QCompute.SDG, 'tdg': QCompute.TDG,
-        'h': QCompute.H, 'x': QCompute.X, 'y': QCompute.Y, 'z': QCompute.Z,
-        'u3': QCompute.U, 'rx': QCompute.RX, 'ry': QCompute.RY, 'rz': QCompute.RZ
-    }
-    multi_qubits_gates = {
-        'cnot': QCompute.CX, 'cx': QCompute.CX, 'cy': QCompute.CY, 'cz': QCompute.CZ, 'swap': QCompute.SWAP,
-        'cu': QCompute.CU, 'crx': QCompute.CRX, 'cry': QCompute.CRY, 'crz': QCompute.CRZ,
-        'cswap': QCompute.CSWAP, 'ccx': QCompute.CCX
-    }
-    for gate in gate_history:
-        gate_name = gate['gate_name']
+    for gate_idx, gate_info in enumerate(oper_history):
+        gate_name = gate_info['name']
         if gate_name in single_qubit_gates:
             gate_func = single_qubit_gates[gate_name]
-            fixed_gate = ['s', 't', 'sdg', 'tdg', 'h', 'x', 'y', 'z']
-            if gate_name in fixed_gate:
-                for _ in range(0, gate['depth']):
-                    for qubit_idx in gate['qubits_idx']:
+            if gate_name in fixed_gates:
+                for _ in range(gate_info['depth']):
+                    for qubit_idx in gate_info['qubits_idx']:
                         gate_func(quleaf_state.Q[qubit_idx])
-            elif gate_name == 'u':
-                for depth_idx in range(0, gate['depth']):
-                    for idx, qubit_idx in enumerate(gate['qubits_idx']):
-                        if gate['param_sharing']:
-                            param_idx = gate['param'][depth_idx]
+            elif gate_name == 'U3':
+                for depth_idx in range(gate_info['depth']):
+                    for idx, qubit_idx in enumerate(gate_info['qubits_idx']):
+                        if gate_info['param_sharing']:
+                            param = gate_info['param'][depth_idx].tolist()
                         else:
-                            param_idx = gate['param'][depth_idx][idx]
-                        gate_param = [param_all[idx] for idx in param_idx]
-                        gate_func(*gate_param)(quleaf_state.Q[qubit_idx])
+                            param = gate_info['param'][depth_idx][idx].tolist()
+                        if gate_idx == _gate_idx and depth_idx == _depth_idx and idx == _qubits_idx:
+                            param[_param_idx] += _param_shift_val
+                        gate_func(*param)(quleaf_state.Q[qubit_idx])
             else:
-                for depth_idx in range(0, gate['depth']):
-                    for idx, qubit_idx in enumerate(gate['qubits_idx']):
-                        if gate['param_sharing']:
-                            param_idx = gate['param'][depth_idx]
+                # Single qubit parameterized quantum gate
+                for depth_idx in range(gate_info['depth']):
+                    for idx, qubit_idx in enumerate(gate_info['qubits_idx']):
+                        if gate_info['param_sharing']:
+                            param = gate_info['param'][depth_idx][0].item()
                         else:
-                            param_idx = gate['param'][depth_idx][idx]
-                        gate_func(param_all[param_idx])(quleaf_state.Q[qubit_idx])
+                            param = gate_info['param'][depth_idx][idx][0].item()
+                        if gate_idx == _gate_idx and depth_idx == _depth_idx and idx == _qubits_idx:
+                            param += _param_shift_val
+                        gate_func(param)(quleaf_state.Q[qubit_idx])
         elif gate_name in multi_qubits_gates:
             gate_func = multi_qubits_gates[gate_name]
-            fixed_gate = ['cnot', 'cx', 'cy', 'cz', 'swap', 'cswap', 'ccx']
-            if gate_name in fixed_gate:
-                for _ in range(0, gate['depth']):
-                    for qubits_idx in gate['qubits_idx']:
-                        qubit_list = [quleaf_state.Q[qubit_idx] for qubit_idx in qubits_idx]
-                        gate_func(*qubit_list)
-            elif gate_name == 'cu':
-                for depth_idx in range(0, gate['depth']):
-                    for idx, qubits_idx in enumerate(gate['qubits_idx']):
-                        if gate['param_sharing']:
-                            param_idx = gate['param'][depth_idx]
+            if gate_name in fixed_gates:
+                for _ in range(gate_info['depth']):
+                    for qubits_idx in gate_info['qubits_idx']:
+                        gate_func(*[quleaf_state.Q[qubit_idx] for qubit_idx in qubits_idx])
+            elif gate_name == 'CU':
+                for depth_idx in range(gate_info['depth']):
+                    for idx, qubits_idx in enumerate(gate_info['qubits_idx']):
+                        if gate_info['param_sharing']:
+                            param = gate_info['param'][depth_idx].tolist()
                         else:
-                            param_idx = gate['param'][depth_idx][idx]
-                        gate_param = [param_all[idx] for idx in param_idx]
-                        qubit_list = [quleaf_state.Q[qubit_idx] for qubit_idx in qubits_idx]
-                        gate_func(*gate_param)(*qubit_list)
+                            param = gate_info['param'][depth_idx][idx].tolist()
+                        if gate_idx == _gate_idx and depth_idx == _depth_idx and idx == _qubits_idx:
+                            param[_param_idx] += _param_shift_val
+                        gate_func(*param)(*[quleaf_state.Q[qubit_idx] for qubit_idx in qubits_idx])
             else:
-                for depth_idx in range(0, gate['depth']):
-                    for idx, qubits_idx in enumerate(gate['qubits_idx']):
-                        if gate['param_sharing']:
-                            param_idx = gate['param'][0]
+                # CRx, CRy, CRz
+                for depth_idx in range(gate_info['depth']):
+                    for idx, qubits_idx in enumerate(gate_info['qubits_idx']):
+                        if gate_info['param_sharing']:
+                            param = gate_info['param'][depth_idx][0].item()
                         else:
-                            param_idx = gate['param'][depth_idx][idx]
-                        qubit_list = [quleaf_state.Q[qubit_idx] for qubit_idx in qubits_idx]
-                        gate_func(param_all[param_idx])(*qubit_list)
+                            param = gate_info['param'][depth_idx][idx][0].item()
+                        if gate_idx == _gate_idx and depth_idx == _depth_idx and idx == _qubits_idx:
+                            param += _param_shift_val
+                        gate_func(param)(*[quleaf_state.Q[qubit_idx] for qubit_idx in qubits_idx])
         else:
             raise NotImplementedError
     return quleaf_state
 
 
 def _expec_val_on_quleaf(state: 'QCompute.QEnv', coeff: 'float', pauli_str: 'str', shots: 'int') -> float:
     r"""Compute the expectation value of the observable with respect to the input state in the QuLeaf backend.
@@ -179,148 +192,142 @@
     # _state = state
     _state = copy.deepcopy(state)
     for pauli_term in pauli_terms:
         pauli_matrix = pauli_term[0]
         qubit_idx = int(pauli_term[1:])
         observed_qubits.append(qubit_idx)
         if pauli_matrix == 'x':
-            RY(-np.pi / 2)(_state.Q[qubit_idx])
+            RY(-math.pi / 2)(_state.Q[qubit_idx])
         elif pauli_matrix == 'y':
-            RX(np.pi / 2)(_state.Q[qubit_idx])
-        elif pauli_matrix == 'z':
-            pass
-        else:
+            RX(math.pi / 2)(_state.Q[qubit_idx])
+        elif pauli_matrix != 'z':
             raise ValueError("Cannot recognize the pauli words of the hamiltonian.")
     MeasureZ(*_state.Q.toListPair())
     counts = _state.commit(shots, fetchMeasure=True)['counts']
     filtered_counts = [(counts[key], [key[-idx - 1] for idx in observed_qubits]) for key in counts]
-    val = coeff * sum([((-1) ** key.count('1')) * val / shots for val, key in filtered_counts])
-    return val
-
-
-def _get_param_for_gate_list(gate_history: list) -> list:
-    r"""Get the all parameters from the gate list.
-
-    Args:
-        gate_history: The gate history, it is automatically generated.
-
-    Returns:
-        The list of the parameters.
-    """
-    param_for_gate_list = []
-    num_param_in_gate = {
-        'rx': 1, 'ry': 1, 'rz': 1, 'u3': 3,
-        'crx': 1, 'cry': 1, 'crz': 1, 'cu': 1,
-    }
-    for gate in gate_history:
-        gate_name = gate['gate_name']
-        if gate_name in num_param_in_gate:
-            num_param = np.array(gate['param']).size
-            for _ in range(0, num_param):
-                param_for_gate_list.append(gate_name)
-    return param_for_gate_list
+    return coeff * sum(
+        (
+            ((-1) ** key.count('1')) * val / shots
+            for val, key in filtered_counts
+        )
+    )
 
 
 class ExpecValOp(paddle.autograd.PyLayer):
     @staticmethod
     def forward(
             ctx: paddle.autograd.PyLayerContext,
-            param: paddle.Tensor,
-            state: 'paddle_quantum.State',
-            hamiltonian: 'paddle_quantum.Hamiltonian',
-            shots: int,
+            state: 'pq.State',
+            hamiltonian: 'pq.Hamiltonian',
+            shots: paddle.Tensor,
+            *parameters
     ) -> paddle.Tensor:
         r"""The forward function to compute the expectation value of the observable in the QuLeaf Backend.
 
         Args:
             ctx: To save some variables so that they can be used in the backward function.
             param: The parameters in the previous quantum gates.
             state: The quantum state to be measured.
             hamiltonian: The observable.
             shots: The number of measurement shots.
+            *parameters: The parameters in the parameterized quantum circuit.
 
         Returns:
             The expectation value of the observable for the input state.
         """
-        ctx.save_for_backward(param)
+        dtype = shots.dtype
+        shots = int(shots.item())
+        ctx.save_for_backward(*parameters)
         quleaf_state = copy.deepcopy(state.data)
+        oper_history = state.oper_history
         ctx.quleaf_state = quleaf_state
-        gate_history = state.gate_history
-        ctx.gate_history = gate_history
+        ctx.oper_history = oper_history
         ctx.hamiltonian = hamiltonian
         ctx.shots = shots
-        state.gate_history = []
-        state.param_list = []
-        state.num_param = 0
-        param_all = param.tolist()
+        ctx.dtype = dtype
         _state = copy.deepcopy(quleaf_state)
-        acted_state = _act_gates_to_state(gate_history, _state, param_all)
+        acted_state = _act_gates_to_state(oper_history, _state, parameters)
         expec_val = 0
         for coeff, pauli_str in hamiltonian.pauli_str:
             _state = copy.deepcopy(acted_state)
             expec_val += _expec_val_on_quleaf(_state, coeff, pauli_str, shots)
-        expec_val = paddle.to_tensor([expec_val], dtype=param.dtype)
+        expec_val = paddle.to_tensor([expec_val], dtype=dtype)
         return expec_val
 
     @staticmethod
     def backward(ctx: paddle.autograd.PyLayerContext, expec_val_grad: paddle.Tensor) -> paddle.Tensor:
         r"""The backward function which is to compute the gradient of the input parameters.
 
         Args:
             ctx: To get the variables saved in the forward function.
             expec_val_grad: The gradient of the expectation value.
 
         Returns:
             The gradient of the parameters for the quantum gates.
         """
-        param, = ctx.saved_tensor()
-        param_all = param.tolist()
+        parameters = ctx.saved_tensor()
+        dtype = ctx.dtype
         quleaf_state = ctx.quleaf_state
-        gate_history = ctx.gate_history
+        oper_history = ctx.oper_history
         hamiltonian = ctx.hamiltonian
         shots = ctx.shots
-        param_for_gate_list = _get_param_for_gate_list(gate_history)
-        assert len(param_for_gate_list) == len(param_all)
 
-        def expec_val_shift(param_idx: int, param_shift: float) -> float:
-            param_temp = copy.deepcopy(param_all)
-            param_temp[param_idx] += param_shift
+        def expec_val_shift(
+                _gate_idx: int, _depth_idx: int, _qubits_idx: int, _param_idx: int, param_shift_val: float
+        ) -> float:
             _state = copy.deepcopy(quleaf_state)
-            acted_state = _act_gates_to_state(gate_history, _state, param_temp)
+            acted_state = _act_gates_to_state(
+                oper_history, _state, _gate_idx, _depth_idx, _qubits_idx, _param_idx, param_shift_val)
             expec_val = 0
             for coeff, pauli_str in hamiltonian.pauli_str:
                 _state = copy.deepcopy(acted_state)
                 expec_val += _expec_val_on_quleaf(_state, coeff, pauli_str, shots)
             # expec_val = paddle.to_tensor([expec_val], dtype=expec_val_grad.dtype)
             return expec_val
 
-        def general_param_shift(param_idx: int) -> float:
-            gate_name = param_for_gate_list[param_idx]
-            if gate_name in ['crx', 'cry', 'crz', 'cu']:
+        def general_param_shift(
+                gate_name: str, _gate_idx: int, _depth_idx: int, _qubits_idx: int, _param_idx: int
+        ) -> float:
+            if gate_name in {'CRX', 'CRY', 'CRZ', 'CU'}:
                 coeff_list = [
                     1 / (16 * math.pow(math.sin(math.pi / 8), 2)),
                     -1 / (16 * math.pow(math.sin(3 * math.pi / 8), 2)),
                     1 / (16 * math.pow(math.sin(5 * math.pi / 8), 2)),
                     - 1 / (16 * math.pow(math.sin(7 * math.pi / 8), 2)),
                 ]
                 shift_list = [math.pi / 2, 3 * math.pi / 2, 5 * math.pi / 2, 7 * math.pi / 2]
                 grad_terms = map(
-                    lambda coeff, shift: coeff * expec_val_shift(param_idx, shift),
+                    lambda coeff, shift_val: coeff * expec_val_shift(
+                        _gate_idx, _depth_idx, _qubits_idx, _param_idx, shift_val
+                    ),
                     coeff_list, shift_list
                 )
                 grad = sum(grad_terms)
             else:
                 coeff1 = 0.5
                 coeff2 = -0.5
                 grad = (
-                    coeff1 * expec_val_shift(param_idx, math.pi / 2) +
-                    coeff2 * expec_val_shift(param_idx, 3 * math.pi / 2)
+                    coeff1 * expec_val_shift(_gate_idx, _depth_idx, _qubits_idx, _param_idx, math.pi / 2) +
+                    coeff2 * expec_val_shift(_gate_idx, _depth_idx, _qubits_idx, _param_idx, 3 * math.pi / 2)
                 )
             return grad
 
-        param_grad = np.zeros(param.size)
-        for idx in range(0, param_grad.size):
-            param_grad[idx] = general_param_shift(idx)
-        param_grad = np.reshape(param_grad, param.shape)
-        param_grad = paddle.to_tensor(param_grad, dtype=param.dtype)
-        param_grad = expec_val_grad * param_grad
-        return param_grad
+        params_idx = 0
+        params_grad = [None]
+        for gate_idx, gate_info in enumerate(oper_history):
+            gate_name = gate_info['name']
+            if gate_name not in parameterized_gates:
+                continue
+            if parameters[params_idx].stop_gradient is True:
+                params_grad.append(None)
+                params_idx += 1
+                continue
+            shape = parameters[params_idx].shape
+            param_grad = np.zeros(shape=shape)
+            for _depth_idx in range(shape[0]):
+                for _qubits_idx in range(shape[1]):
+                    for _param_idx in range(shape[2]):
+                        grad = general_param_shift(gate_name, gate_idx, _depth_idx, _qubits_idx, _param_idx)
+                        param_grad[_depth_idx, _qubits_idx, _param_idx] += grad
+            params_grad.append(expec_val_grad * paddle.to_tensor(param_grad, dtype=dtype))
+            params_idx += 1
+        return params_grad
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/backend/state_vector.py` & `paddle-quantum-2.4.0/paddle_quantum/backend/unitary_matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,42 +10,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
-The source file of the state_vector backend.
+The source file of the unitary_matrix backend.
 """
 
 import paddle
 from typing import List, Iterable, Union
 
-
 def unitary_transformation(
         state: paddle.Tensor, gate: paddle.Tensor, qubit_idx: Union[List[int], int], num_qubits: int
 ) -> paddle.Tensor:
-    r"""The function of unitary transformation in the mode of state vector.
+    r"""The function of unitary transformation in the mode of computing the unitary matrix.
 
     Args:
         state: The input quantum state.
         gate: The gate that represents the unitary transformation.
         qubit_idx: The indices of the qubits on which the gate is acted.
         num_qubits: The number of the qubits in the input quantum state.
 
     Returns:
         The transformed quantum state.
     """
     # The order of the tensor in paddle is less than 10.
-    higher_dims = state.shape[:-1]
+    higher_dims = state.shape[:-2]
     num_higher_dims = len(higher_dims)
     
     if not isinstance(qubit_idx, Iterable):
         qubit_idx = [qubit_idx]
-       
+        
     # generate swap_list
     num_acted_qubits = len(qubit_idx)
     origin_seq = list(range(0, num_qubits))
     seq_for_acted = qubit_idx + [x for x in origin_seq if x not in qubit_idx]
     swapped = [False] * num_qubits
     swap_ops = []
     for idx in range(0, num_qubits):
@@ -55,37 +54,41 @@
             while not swapped[seq_for_acted[next_idx]]:
                 swapped[seq_for_acted[next_idx]] = True
                 if next_idx < seq_for_acted[next_idx]:
                     swap_ops.append((next_idx, seq_for_acted[next_idx]))
                 else:
                     swap_ops.append((seq_for_acted[next_idx], next_idx))
                 next_idx = seq_for_acted[next_idx]
+
     for swap_op in swap_ops:
         shape = higher_dims.copy()
         last_idx = -1
         for idx in swap_op:
             shape.append(2 ** (idx - last_idx - 1))
             shape.append(2)
             last_idx = idx
-        shape.append(2 ** (num_qubits - last_idx - 1))
+        shape.append(2 ** (2 * num_qubits - last_idx - 1))
         state = paddle.reshape(state, shape)
         state = paddle.transpose(
             state, list(range(0, num_higher_dims)) + [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
         )
-    state = paddle.reshape(state, higher_dims.copy() + [2 ** num_acted_qubits, 2 ** (num_qubits - num_acted_qubits)])
+    state = paddle.reshape(
+        state, higher_dims.copy() + [2 ** num_acted_qubits, 2 ** (2 * num_qubits - num_acted_qubits)]
+    )
     state = paddle.matmul(gate, state)
     swap_ops.reverse()
     for swap_op in swap_ops:
         shape = higher_dims.copy()
         last_idx = -1
         for idx in swap_op:
             shape.append(2 ** (idx - last_idx - 1))
             shape.append(2)
             last_idx = idx
-        shape.append(2 ** (num_qubits - last_idx - 1))
+        shape.append(2 ** (2 * num_qubits - last_idx - 1))
         state = paddle.reshape(state, shape)
         state = paddle.transpose(
             state, list(range(0, num_higher_dims)) + [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
         )
-
-    state = paddle.reshape(state, higher_dims.copy() + [2 ** num_qubits])
+    state = paddle.reshape(state, higher_dims.copy() + [2 ** num_qubits, 2 ** num_qubits])
     return state
+
+# TODO Update same tensor contraction logic
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/backend/unitary_matrix.py` & `paddle-quantum-2.4.0/paddle_quantum/gate/functional/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,84 +10,113 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
-The source file of the unitary_matrix backend.
+The source file of the basic function for quantum gates.
 """
 
+import copy
 import paddle
-from typing import List, Iterable, Union
+import paddle_quantum as pq
+from ...backend import state_vector
+from ...backend import density_matrix
+from ...backend import unitary_matrix
+from typing import Union, List
 
 
-def unitary_transformation(
-        state: paddle.Tensor, gate: paddle.Tensor, qubit_idx: Union[List[int], int], num_qubits: int
-) -> paddle.Tensor:
-    r"""The function of unitary transformation in the mode of computing the unitary matrix.
+def simulation(state: pq.State, gate: List[paddle.Tensor], qubit_idx: Union[int, List[int]]) -> pq.State:
+    r"""Apply the gate on the input state.
 
     Args:
-        state: The input quantum state.
-        gate: The gate that represents the unitary transformation.
-        qubit_idx: The indices of the qubits on which the gate is acted.
-        num_qubits: The number of the qubits in the input quantum state.
+        state: Input state.
+        gate: List of Gates to be executed.
+        qubit_idx: Indices of the qubits on which the gate is applied.
 
     Returns:
-        The transformed quantum state.
+        Output state.
     """
-    # The order of the tensor in paddle is less than 10.
-    higher_dims = state.shape[:-2]
-    num_higher_dims = len(higher_dims)
-    
-    if not isinstance(qubit_idx, Iterable):
+    if isinstance(qubit_idx, int):
         qubit_idx = [qubit_idx]
-        
-    # generate swap_list
-    num_acted_qubits = len(qubit_idx)
-    origin_seq = list(range(0, num_qubits))
-    seq_for_acted = qubit_idx + [x for x in origin_seq if x not in qubit_idx]
-    swapped = [False] * num_qubits
-    swap_ops = []
-    for idx in range(0, num_qubits):
-        if not swapped[idx]:
-            next_idx = idx
-            swapped[next_idx] = True
-            while not swapped[seq_for_acted[next_idx]]:
-                swapped[seq_for_acted[next_idx]] = True
-                if next_idx < seq_for_acted[next_idx]:
-                    swap_ops.append((next_idx, seq_for_acted[next_idx]))
-                else:
-                    swap_ops.append((seq_for_acted[next_idx], next_idx))
-                next_idx = seq_for_acted[next_idx]
-
-    for swap_op in swap_ops:
-        shape = higher_dims.copy()
-        last_idx = -1
-        for idx in swap_op:
-            shape.append(2 ** (idx - last_idx - 1))
-            shape.append(2)
-            last_idx = idx
-        shape.append(2 ** (2 * num_qubits - last_idx - 1))
-        state = paddle.reshape(state, shape)
-        state = paddle.transpose(
-            state, list(range(0, num_higher_dims)) + [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
-        )
-    state = paddle.reshape(
-        state, higher_dims.copy() + [2 ** num_acted_qubits, 2 ** (2 * num_qubits - num_acted_qubits)]
-    )
-    state = paddle.matmul(gate, state)
-    swap_ops.reverse()
-    for swap_op in swap_ops:
-        shape = higher_dims.copy()
-        last_idx = -1
-        for idx in swap_op:
-            shape.append(2 ** (idx - last_idx - 1))
-            shape.append(2)
-            last_idx = idx
-        shape.append(2 ** (2 * num_qubits - last_idx - 1))
-        state = paddle.reshape(state, shape)
-        state = paddle.transpose(
-            state, list(range(0, num_higher_dims)) + [item + num_higher_dims for item in [0, 3, 2, 1, 4]]
-        )
-    state = paddle.reshape(state, higher_dims.copy() + [2 ** num_qubits, 2 ** num_qubits])
+    
+    if state.is_swap_back:
+        if len(gate) > 1:
+            for gate_i in range(len(gate)):
+                state = __simulation_with_swapback(
+                    state, gate[gate_i], qubit_idx[gate_i])
+        else:
+            state = __simulation_with_swapback(state, gate[0], qubit_idx)
+        return state
+
+    return __simulation_without_swapback(state, gate, qubit_idx)
+
+
+def __simulation_with_swapback(
+        state: pq.State, gate: paddle.Tensor, qubit_idx: List[int]
+) -> pq.State:
+    r"""Apply the gate on the input state (old logic).
+
+    Args:
+        state: Input state.
+        gate: Gate to be executed.
+        qubit_idx: Indices of the qubits on which the gate is applied.
+
+    Returns:
+        Output state.
+    """
+    num_qubits, backend = state.num_qubits, state.backend
+    data = state.data
+
+    if backend == pq.Backend.StateVector:
+        data = state_vector.unitary_transformation(
+            data, gate, qubit_idx, num_qubits)
+    elif backend == pq.Backend.DensityMatrix:
+        data = density_matrix.unitary_transformation(
+            data, gate, qubit_idx, num_qubits)
+    elif backend == pq.Backend.UnitaryMatrix:
+        data = unitary_matrix.unitary_transformation(
+            data, gate, qubit_idx, num_qubits)
+    else:
+        raise NotImplementedError
+
+    state = copy.copy(state)
+    state.data = data
+    return state
+
+
+def __simulation_without_swapback(
+        state: pq.State, gate: List[paddle.Tensor], qubit_idx: List[int]
+) -> pq.State:
+    r"""Apply the gate on the input state (new logic).
+
+    Args:
+        state: Input state.
+        gate: List of Gates to be executed.
+        qubit_idx: Indices of the qubits on which the gate is applied.
+
+    Returns:
+        Output state.
+    """
+    num_qubits, backend = state.num_qubits, state.backend
+    data = state.data
+    qubit_sequence = state.qubit_sequence
+
+    if backend == pq.Backend.StateVector:
+        data, qubit_sequence = state_vector.unitary_transformation_without_swapback(
+            data, gate, qubit_idx, num_qubits, qubit_sequence)
+    elif backend == pq.Backend.DensityMatrix:
+        data, qubit_sequence = density_matrix.unitary_transformation_without_swapback(
+            data, gate, qubit_idx, num_qubits, qubit_sequence)
+    else:
+        if len(gate) > 1:
+            for gate_i in range(len(gate)):
+                data = unitary_matrix.unitary_transformation(
+                    data, gate[gate_i], qubit_idx[gate_i], num_qubits)
+        else:
+            data = unitary_matrix.unitary_transformation(
+                data, gate[0], qubit_idx, num_qubits)
+
+    state.data = data
+    state.qubit_sequence = qubit_sequence
     return state
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/base.py` & `paddle-quantum-2.4.0/paddle_quantum/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -93,37 +93,42 @@
     Returns:
         Currently used data type.
     """
     return DEFAULT_DTYPE
 
 
 class Operator(paddle.nn.Layer):
-    r"""The basic class to implement the quantum operation.
+    r"""The basic class to implement the operation in Paddle Quantum.
 
     Args:
         backend: The backend implementation of the operator.
             Defaults to ``None``, which means to use the default backend implementation.
         dtype: The data type of the operator.
             Defaults to ``None``, which means to use the default data type.
         name_scope: Prefix name used by the operator to name parameters. Defaults to ``None``.
     """
-    def __init__(self, backend: Optional[paddle_quantum.Backend] = None, dtype: Optional[str] = None,
-                 name_scope: Optional[str] = None):
+    def __init__(
+            self, backend: Optional[paddle_quantum.Backend] = None,
+            dtype: Optional[str] = None, name_scope: Optional[str] = None
+    ):
         if dtype is None:
             super().__init__(name_scope)
         else:
             super().__init__(name_scope, dtype)
         self.dtype = dtype if dtype is not None else get_dtype()
 
-        if backend == paddle_quantum.Backend.StateVector:
-            self.backend = backend
-        elif backend == paddle_quantum.Backend.DensityMatrix:
-            self.backend = backend
-        elif backend is None:
-            self.backend = get_backend()
+        self.backend = backend if backend is not None else get_backend()
+
+    def __setattr__(self, name, value):
+        super().__setattr__(name, value)
+        if isinstance(value, Operator):
+            if value.backend is None:
+                value.backend = get_backend() if self.backend is None else self.backend
+            if value.dtype is None:
+                value.dtype = get_dtype() if self.dtype is None else self.dtype
 
     def to(self, backend: Optional[paddle_quantum.Backend] = None, device: Optional[str] = None,
            dtype: Optional[str] = None, blocking: Optional[str] = None):
         super().to(device, dtype, blocking)
         if backend is not None:
             self.backend = backend
             for sub_layer in self.children():
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/biocomputing/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/biocomputing/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/biocomputing/algorithm.py` & `paddle-quantum-2.4.0/paddle_quantum/biocomputing/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,43 +73,38 @@
         cvar_val0 += e*p
         cutoff_idx += 1
     Hj = results[cutoff_idx][0]
     return (1/alpha)*(cvar_val0 + Hj*(alpha - running_probability))
 
 
 class ProteinFoldingSolver(VQESolver):
+    r"""
+    Args:
+        penalty_factors: penalty factor ``[lambda0, lambda1]`` used in building the protein's Hamiltonian.
+        alpha: the cutoff probability for CVaR expectation value calculation.
+        optimizer: paddle's optimizer used to perform parameter update.
+        num_iterations : number of VQE iterations.
+        tol: convergence criteria.
+        save_every : number of steps between two recorded VQE loss.
+    """
     def __init__(
-        self,
-        penalty_factors: List[float],
-        alpha: float,
-        optimizer: Optimizer,
-        num_iterations: int,
-        tol: float = 1e-8,
-        save_every: int = 1,
+            self,
+            penalty_factors: List[float],
+            alpha: float,
+            optimizer: Optimizer,
+            num_iterations: int,
+            tol: float = 1e-8,
+            save_every: int = 1,
     ) -> None:
-        r"""
-        Args:
-            penalty_factors: penalty factor ``[lambda0, lambda1]`` used in building the protein's Hamiltonian.
-            alpha: the cutoff probability for CVaR expectation value calculation.
-            optimizer: paddle's optimizer used to perform parameter update.
-            num_iterations : number of VQE iterations.
-            tol: convergence criteria.
-            save_every : number of steps between two recorded VQE loss.
-        """
         super().__init__(optimizer, num_iterations, tol, save_every)
         self.lambda0 = penalty_factors[0]
         self.lambda1 = penalty_factors[1]
         self.alpha = alpha
 
-    def solve(
-        self,
-        protein: Protein,
-        ansatz: Circuit,
-        **optimizer_kwargs
-    ) -> Tuple[float, str]:
+    def solve(self, protein: Protein, ansatz: Circuit, **optimizer_kwargs) -> Tuple[float, str]:
         r"""Run VQE to calculate the structure of the protein that satisfies various constraints.
 
         Args:
             protein: the protein structure to be optimized.
             ansatz: the quantum circuit represents the unitary transformation.
             optimizer_kwargs: see PaddlePaddle's optimizer API for details https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/optimizer/Overview_cn.html (Chinese) or https://www.paddlepaddle.org.cn/documentation/docs/en/api/paddle/optimizer/Optimizer_en.html (English).
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/biocomputing/data_loader.py` & `paddle-quantum-2.4.0/paddle_quantum/biocomputing/data_loader.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/biocomputing/mj_matrix.txt` & `paddle-quantum-2.4.0/paddle_quantum/biocomputing/mj_matrix.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/biocomputing/operators.py` & `paddle-quantum-2.4.0/paddle_quantum/biocomputing/operators.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/biocomputing/protein.py` & `paddle-quantum-2.4.0/paddle_quantum/biocomputing/protein.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/biocomputing/visualize.py` & `paddle-quantum-2.4.0/paddle_quantum/biocomputing/visualize.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/channel/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/channel/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
 r"""
 The module of the quantum channels.
 """
 
 from .base import Channel
 from .common import *
-from .custom import ChoiRepr, KrausRepr, StinespringRepr
+from .custom import *
 from .representation import *
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/channel/common.py` & `paddle-quantum-2.4.0/paddle_quantum/channel/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,23 +13,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
 The source file of the classes for common quantum channels.
 """
 
+import numpy as np
 import paddle
-from .custom import KrausRepr
+from .base import Channel
 from ..intrinsic import _format_qubits_idx
 from ..qinfo import kraus_unitary_random
-from .representation import *
+from ..state import State
+from .representation import (
+    bit_flip_kraus, phase_flip_kraus, bit_phase_flip_kraus,
+    amplitude_damping_kraus, generalized_amplitude_damping_kraus, phase_damping_kraus,
+    depolarizing_kraus, generalized_depolarizing_kraus, pauli_kraus, reset_kraus,
+    thermal_relaxation_kraus, replacement_choi
+)
 from typing import Union, Iterable
 
 
-class BitFlip(KrausRepr):
+class BitFlip(Channel):
     r"""A collection of bit flip channels.
 
     Such a channel's Kraus operators are
 
     .. math::
 
         E_0 = \sqrt{1-p} I,
@@ -40,18 +47,18 @@
         qubits_idx: Indices of the qubits on which the channels act. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
     """
     def __init__(
             self, prob: Union[paddle.Tensor, float],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(bit_flip_kraus(prob), qubits_idx, num_qubits, check_complete=False)
-        
+        super().__init__('kraus', bit_flip_kraus(prob), qubits_idx, num_qubits, check_legality=False)
 
-class PhaseFlip(KrausRepr):
+
+class PhaseFlip(Channel):
     r"""A collection of phase flip channels.
 
     Such a channel's Kraus operators are
 
     .. math::
 
         E_0 = \sqrt{1 - p} I,
@@ -62,18 +69,18 @@
         qubits_idx: Indices of the qubits on which the channels act. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
     """
     def __init__(
             self, prob: Union[paddle.Tensor, float],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(phase_flip_kraus(prob), qubits_idx, num_qubits, check_complete=False)
+        super().__init__('kraus', phase_flip_kraus(prob), qubits_idx, num_qubits, check_legality=False)
 
 
-class BitPhaseFlip(KrausRepr):
+class BitPhaseFlip(Channel):
     r"""A collection of bit phase flip channels.
 
     Such a channel's Kraus operators are
 
     .. math::
 
         E_0 = \sqrt{1 - p} I,
@@ -84,18 +91,18 @@
         qubits_idx: Indices of the qubits on which the channels act. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
     """
     def __init__(
             self, prob: Union[paddle.Tensor, float],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(bit_phase_flip_kraus(prob), qubits_idx, num_qubits, check_complete=False)
+        super().__init__('kraus', bit_phase_flip_kraus(prob), qubits_idx, num_qubits, check_legality=False)
 
 
-class AmplitudeDamping(KrausRepr):
+class AmplitudeDamping(Channel):
     r"""A collection of amplitude damping channels.
 
     Such a channel's Kraus operators are
 
     .. math::
 
         E_0 =
@@ -114,18 +121,18 @@
         qubits_idx: Indices of the qubits on which the channels act. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
     """
     def __init__(
             self, gamma: Union[paddle.Tensor, float],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(amplitude_damping_kraus(gamma), qubits_idx, num_qubits, check_complete=False)
+        super().__init__('kraus', amplitude_damping_kraus(gamma), qubits_idx, num_qubits, check_legality=False)
 
 
-class GeneralizedAmplitudeDamping(KrausRepr):
+class GeneralizedAmplitudeDamping(Channel):
     r"""A collection of generalized amplitude damping channels.
 
     Such a channel's Kraus operators are
 
     .. math::
 
         E_0 = \sqrt{p}
@@ -143,18 +150,19 @@
         qubits_idx: Indices of the qubits on which the channels act. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
     """
     def __init__(
             self, gamma: Union[paddle.Tensor, float], prob: Union[paddle.Tensor, float],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(generalized_amplitude_damping_kraus(gamma, prob), qubits_idx, num_qubits, check_complete=False)
+        super().__init__(
+            'kraus', generalized_amplitude_damping_kraus(gamma, prob), qubits_idx, num_qubits, check_legality=False)
 
 
-class PhaseDamping(KrausRepr):
+class PhaseDamping(Channel):
     r"""A collection of phase damping channels.
 
     Such a channel's Kraus operators are
 
     .. math::
 
         E_0 =
@@ -173,18 +181,18 @@
         qubits_idx: Indices of the qubits on which the channels act. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
     """
     def __init__(
             self, gamma: Union[paddle.Tensor, float],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(phase_damping_kraus(gamma), qubits_idx, num_qubits, check_complete=False)
+        super().__init__('kraus', phase_damping_kraus(gamma), qubits_idx, num_qubits, check_legality=False)
 
 
-class Depolarizing(KrausRepr):
+class Depolarizing(Channel):
     r"""A collection of depolarizing channels.
 
     Such a channel's Kraus operators are
 
     .. math::
 
         E_0 = \sqrt{1-3p/4} I,
@@ -204,43 +212,46 @@
         Reference: Nielsen, M., & Chuang, I. (2010). Quantum Computation and Quantum Information: 10th
         Anniversary Edition. Cambridge: Cambridge University Press. doi:10.1017/CBO9780511976667
     """
     def __init__(
             self, prob: Union[paddle.Tensor, float],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(depolarizing_kraus(prob), qubits_idx, num_qubits, check_complete=False)
+        super().__init__('kraus', depolarizing_kraus(prob), qubits_idx, num_qubits, check_legality=False)
 
 
-class GeneralizedDepolarizing(KrausRepr):
+class GeneralizedDepolarizing(Channel):
     r"""A generalized depolarizing channel.
 
     Such a channel's Kraus operators are
 
     .. math::
 
         E_0 = \sqrt{1-(D - 1)p/D} I, \text{ where } D = 4^n, \\
         E_k = \sqrt{p/D} \sigma_k, \text{ for } 0 < k < D.
-    
+
     Args:
         prob: probability :math:`p`. Its value should be in the range :math:`[0, 1]`.
         qubits_idx: Indices of the qubits on which the channels act, the length of which is :math:`n`.
+            Defaults to be ``None``.
         num_qubits: Total number of qubits. Defaults to ``None``.
-    
     """
     def __init__(
             self, prob: Union[paddle.Tensor, float],
-            qubits_idx: Union[Iterable[int], int, str], num_qubits: int = None
+            qubits_idx: Union[Iterable[int], int, str] = None, num_qubits: int = None
     ):
-        num_acted_qubits = np.size(np.array(qubits_idx)).item()
-        super().__init__(generalized_depolarizing_kraus(prob, num_acted_qubits),
-                         qubits_idx, num_qubits, check_complete=False)
+        num_acted_qubits = np.size(np.array(qubits_idx))
+        if qubits_idx is None:
+            qubits_idx = 'full' if num_acted_qubits == 1 else 'cycle'
+        super().__init__(
+            'kraus', generalized_depolarizing_kraus(prob, num_acted_qubits),
+            qubits_idx, num_qubits, check_legality=False)
 
 
-class PauliChannel(KrausRepr):
+class PauliChannel(Channel):
     r"""A collection of Pauli channels.
 
     Args:
         prob: Probabilities corresponding to the Pauli X, Y, and Z operators. Each value should be in the
             range :math:`[0, 1]`.
         qubits_idx: Indices of the qubits on which the channels act. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
@@ -248,18 +259,18 @@
     Note:
         The sum of three input probabilities should be less than or equal to 1.
     """
     def __init__(
             self, prob: Union[paddle.Tensor, Iterable[float]],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(pauli_kraus(prob), qubits_idx, num_qubits, check_complete=False)
+        super().__init__('kraus', pauli_kraus(prob), qubits_idx, num_qubits, check_legality=False)
 
 
-class ResetChannel(KrausRepr):
+class ResetChannel(Channel):
     r"""A collection of reset channels.
 
     Such a channel reset the state to :math:`|0\rangle` with a probability of p and to :math:`|1\rangle` with
     a probability of q. Its Kraus operators are
 
     .. math::
 
@@ -294,18 +305,18 @@
     Note:
         The sum of two input probabilities should be less than or equal to 1.
     """
     def __init__(
             self, prob: Union[paddle.Tensor, Iterable[float]],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(reset_kraus(prob), qubits_idx, num_qubits, check_complete=False)
+        super().__init__('kraus', reset_kraus(prob), qubits_idx, num_qubits, check_legality=False)
 
 
-class ThermalRelaxation(KrausRepr):
+class ThermalRelaxation(Channel):
     r"""A collection of thermal relaxation channels.
 
     Such a channel simulates the mixture of the :math:`T_1` and the :math:`T_2` processes on superconducting devices.
 
     Args:
         const_t: :math:`T_1` and :math:`T_2` relaxation time in microseconds.
         exec_time: Quantum gate execution time in the process of relaxation in nanoseconds.
@@ -315,34 +326,61 @@
     Note:
         Relaxation time must satisfy :math:`T_2 \le T_1`. For reference please see https://arxiv.org/abs/2101.02109.
     """
     def __init__(
             self, const_t: Union[paddle.Tensor, Iterable[float]], exec_time: Union[paddle.Tensor, float],
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        super().__init__(thermal_relaxation_kraus(const_t, exec_time), qubits_idx, num_qubits, check_complete=False)
+        super().__init__(
+            'kraus', thermal_relaxation_kraus(const_t, exec_time),
+            qubits_idx, num_qubits, check_legality=False)
 
 
-class MixedUnitaryChannel(KrausRepr):
+class MixedUnitaryChannel(Channel):
     r"""A collection of single-qubit mixed unitary channels.
 
     Such a channel's Kraus operators are randomly generated unitaries times related probabilities
+    
     .. math::
 
         N(\rho) = \sum_{i}  p_{i} U_{i} \rho U_{i}^{\dagger}
 
     Args:
         num_unitary: The amount of random unitaries to be generated.
         qubits_idx: Indices of the qubits on which the channels act. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
 
     Note:
-    The probability distribution of unitaries is set to be uniform distribution.
+        The probability distribution of unitaries is set to be uniform distribution.
     """
     def __init__(
             self, num_unitary: int,
             qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ):
-        #TODO: increase the number of acting qubits, currently only support 1
-        super().__init__(kraus_unitary_random(1, num_unitary), 
-                         _format_qubits_idx(qubits_idx, num_qubits, 1), 
-                         num_qubits, check_complete=False)
+        # TODO: increase the number of acting qubits, currently only support 1
+        super().__init__(
+            'kraus', kraus_unitary_random(1, num_unitary),
+            _format_qubits_idx(qubits_idx, num_qubits, 1), num_qubits, check_legality=False)
+
+
+class ReplacementChannel(Channel):
+    r"""A collection of quantum replacement channels.
+
+    For a quantum state :math:`\sigma`, the corresponding replacement channel :math:`R` is defined as
+
+    .. math::
+
+        R(\rho) = \text{tr}(\rho)\sigma
+
+    Args:
+        sigma: The state to be replaced.
+        qubits_idx: Indices of the qubits on which the channels act, the length of which is :math:`n`.
+            Defaults to be ``None``.
+        num_qubits: Total number of qubits. Defaults to ``None``.
+    """
+    def __init__(
+            self, sigma: State,
+            qubits_idx: Union[Iterable[int], int, str] = None, num_qubits: int = None
+    ):
+        if qubits_idx is None:
+            qubits_idx = list(range(sigma.num_qubits))
+        super().__init__('choi', replacement_choi(sigma), qubits_idx, num_qubits)
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/channel/functional/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/channel/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/channel/functional/common.py` & `paddle-quantum-2.4.0/paddle_quantum/channel/functional/common.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/channel/representation.py` & `paddle-quantum-2.4.0/paddle_quantum/channel/representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,32 +19,33 @@
 
 import numpy as np
 
 import paddle
 from ..base import get_dtype
 from ..intrinsic import _zero, _one, _get_float_dtype
 from ..linalg import pauli_basis_generation
+from ..state import State
 from typing import List, Union
 
 
 def bit_flip_kraus(prob: Union[float, np.ndarray, paddle.Tensor], dtype: str = None) -> List[paddle.Tensor]:
     r"""Kraus representation of a bit flip channel with form
 
     .. math::
 
         E_0 = \sqrt{1-p} I,
         E_1 = \sqrt{p} X.
 
     Args:
         prob: probability :math:`p`.
         dtype: data type. Defaults to be ``None``.
-    
+
     Returns:
         a list of Kraus operators
-        
+
     """
     dtype = get_dtype() if dtype is None else dtype
     prob = prob if isinstance(prob, paddle.Tensor) else paddle.to_tensor(prob, dtype=_get_float_dtype(dtype))
     kraus_oper = [
         [
             paddle.sqrt(1 - prob).cast(dtype), _zero(dtype),
             _zero(dtype), paddle.sqrt(1 - prob).cast(dtype),
@@ -62,22 +63,21 @@
 def phase_flip_kraus(prob: Union[float, np.ndarray, paddle.Tensor], dtype: str = None) -> List[paddle.Tensor]:
     r"""Kraus representation of a phase flip channel with form
 
     .. math::
 
         E_0 = \sqrt{1 - p} I,
         E_1 = \sqrt{p} Z.
-    
+
     Args:
         prob: probability :math:`p`.
         dtype: data type. Defaults to be ``None``.
-    
+
     Returns:
         a list of Kraus operators
-        
     """
     dtype = get_dtype() if dtype is None else dtype
     prob = prob if isinstance(prob, paddle.Tensor) else paddle.to_tensor(prob, dtype=_get_float_dtype(dtype))
     kraus_oper = [
         [
             paddle.sqrt(1 - prob).cast(dtype), _zero(dtype),
             _zero(dtype), paddle.sqrt(1 - prob).cast(dtype),
@@ -95,33 +95,32 @@
 def bit_phase_flip_kraus(prob: Union[float, np.ndarray, paddle.Tensor], dtype: str = None) -> List[paddle.Tensor]:
     r"""Kraus representation of a bit-phase flip channel with form
 
     .. math::
 
         E_0 = \sqrt{1 - p} I,
         E_1 = \sqrt{p} Y.
-    
+
     Args:
         prob: probability :math:`p`.
         dtype: data type. Defaults to be ``None``.
-    
+
     Returns:
         a list of Kraus operators
-        
     """
     dtype = get_dtype() if dtype is None else dtype
     prob = prob if isinstance(prob, paddle.Tensor) else paddle.to_tensor(prob, dtype=_get_float_dtype(dtype))
     kraus_oper = [
         [
             paddle.sqrt(1 - prob).cast(dtype), _zero(dtype),
             _zero(dtype), paddle.sqrt(1 - prob).cast(dtype),
         ],
         [
             _zero(dtype), -1j * paddle.sqrt(prob),
-            1j * -paddle.sqrt(prob), _zero(dtype),
+            1j * paddle.sqrt(prob), _zero(dtype),
         ]
     ]
     for idx, oper in enumerate(kraus_oper):
         kraus_oper[idx] = paddle.reshape(paddle.concat(oper), [2, 2])
     return kraus_oper
 
 
@@ -136,22 +135,21 @@
             0 & \sqrt{1-\gamma}
         \end{bmatrix},
         E_1 =
         \begin{bmatrix}
             0 & \sqrt{\gamma} \\
             0 & 0
         \end{bmatrix}.
-    
+
     Args:
         gamma: coefficient :math:`\gamma`.
         dtype: data type. Defaults to be ``None``.
-    
+
     Returns:
         a list of Kraus operators
-        
     """
     dtype = get_dtype() if dtype is None else dtype
     gamma = gamma if isinstance(gamma, paddle.Tensor) else paddle.to_tensor(gamma, dtype=_get_float_dtype(dtype))
     kraus_oper = [
         [
             _one(dtype), _zero(dtype),
             _zero(dtype), paddle.sqrt(1 - gamma).cast(dtype),
@@ -162,33 +160,34 @@
 
     ]
     for idx, oper in enumerate(kraus_oper):
         kraus_oper[idx] = paddle.reshape(paddle.concat(oper), [2, 2])
     return kraus_oper
 
 
-def generalized_amplitude_damping_kraus(gamma: Union[float, np.ndarray, paddle.Tensor], 
-                                  prob: Union[float, np.ndarray, paddle.Tensor], dtype: str = None) -> List[paddle.Tensor]:
+def generalized_amplitude_damping_kraus(
+        gamma: Union[float, np.ndarray, paddle.Tensor],
+        prob: Union[float, np.ndarray, paddle.Tensor], dtype: str = None
+) -> List[paddle.Tensor]:
     r"""Kraus representation of a generalized amplitude damping channel with form
 
     .. math::
 
         E_0 = \sqrt{p} \begin{bmatrix} 1 & 0 \\ 0 & \sqrt{1-\gamma} \end{bmatrix},
         E_1 = \sqrt{p} \begin{bmatrix} 0 & \sqrt{\gamma} \\ 0 & 0 \end{bmatrix},\\
         E_2 = \sqrt{1-p} \begin{bmatrix} \sqrt{1-\gamma} & 0 \\ 0 & 1 \end{bmatrix},
         E_3 = \sqrt{1-p} \begin{bmatrix} 0 & 0 \\ \sqrt{\gamma} & 0 \end{bmatrix}.
-    
+
     Args:
         gamma: coefficient :math:`\gamma`.
         prob: probability :math:`p`.
         dtype: data type. Defaults to be ``None``.
-    
+
     Returns:
         a list of Kraus operators
-        
     """
     dtype = get_dtype() if dtype is None else dtype
     float_dtype = _get_float_dtype(dtype)
     gamma = gamma if isinstance(gamma, paddle.Tensor) else paddle.to_tensor(gamma, dtype=float_dtype)
     prob = prob if isinstance(prob, paddle.Tensor) else paddle.to_tensor(prob, dtype=float_dtype)
     kraus_oper = [
         [
@@ -224,22 +223,21 @@
             0 & \sqrt{1-\gamma}
         \end{bmatrix},
         E_1 =
         \begin{bmatrix}
             0 & 0 \\
             0 & \sqrt{\gamma}
         \end{bmatrix}.
-    
+
     Args:
         gamma: coefficient :math:`\gamma`.
         dtype: data type. Defaults to be ``None``.
-    
+
     Returns:
         a list of Kraus operators
-        
     """
     dtype = get_dtype() if dtype is None else dtype
     gamma = gamma if isinstance(gamma, paddle.Tensor) else paddle.to_tensor(gamma, dtype=_get_float_dtype(dtype))
     kraus_oper = [
         [
             _one(dtype), _zero(dtype),
             _zero(dtype), paddle.sqrt(1 - gamma).cast(dtype),
@@ -259,22 +257,21 @@
 
     .. math::
 
         E_0 = \sqrt{1-3p/4} I,
         E_1 = \sqrt{p/4} X,
         E_2 = \sqrt{p/4} Y,
         E_3 = \sqrt{p/4} Z.
-    
+
     Args:
         prob: probability :math:`p`.
         dtype: data type. Defaults to be ``None``.
-    
+
     Returns:
         a list of Kraus operators
-        
     """
     dtype = get_dtype() if dtype is None else dtype
     prob = prob if isinstance(prob, paddle.Tensor) else paddle.to_tensor(prob, dtype=_get_float_dtype(dtype))
     kraus_oper = [
         [
             paddle.sqrt(1 - 3 * prob / 4).cast(dtype), _zero(dtype),
             _zero(dtype), paddle.sqrt(1 - 3 * prob / 4).cast(dtype),
@@ -295,59 +292,59 @@
     for idx, oper in enumerate(kraus_oper):
         kraus_oper[idx] = paddle.reshape(paddle.concat(oper), [2, 2])
     return kraus_oper
 
 
 def generalized_depolarizing_kraus(prob: float, num_qubits: int, dtype: str = None) -> List[paddle.Tensor]:
     r"""Kraus representation of a generalized depolarizing channel with form
-    
+
     .. math::
 
         E_0 = \sqrt{1-(D - 1)p/D} I, \text{ where } D = 4^n,
         E_k = \sqrt{p/D} \sigma_k, \text{ for } 0 < k < D.
-    
+
     Args:
         prob: probability :math:`p`.
         num_qubits: number of qubits :math:`n` of this channel.
         dtype: data type. Defaults to be ``None``.
-        
+
     Returns:
         a list of Kraus operators
-    
     """
     dtype = get_dtype() if dtype is None else dtype
     prob = prob if isinstance(prob, paddle.Tensor) else paddle.to_tensor(prob, dtype=_get_float_dtype(dtype))
-    
+
     basis = [ele.cast(dtype) * (2 ** num_qubits + 0j) for ele in pauli_basis_generation(num_qubits)]
     I, other_elements = basis[0], basis[1:]
-    
+
     dim = 4 ** num_qubits
-    return ([I * (paddle.sqrt(1 - (dim - 1) * prob / dim) + 0j)] +
-            [ele * (paddle.sqrt(prob / dim) + 0j) for ele in other_elements])
+    return (
+        [I * (paddle.sqrt(1 - (dim - 1) * prob / dim) + 0j)] +
+        [ele * (paddle.sqrt(prob / dim) + 0j) for ele in other_elements]
+    )
 
 
 def pauli_kraus(prob: Union[List[float], np.ndarray, paddle.Tensor], dtype: str = None) -> List[paddle.Tensor]:
     r"""Kraus representation of a pauli channel
-    
+
     Args:
         prob: a list of three probabilities corresponding to X, Y, Z gate :math:`p`.
         dtype: data type. Defaults to be ``None``.
-    
+
     Returns:
         a list of Kraus operators
-        
     """
     dtype = get_dtype() if dtype is None else dtype
     float_dtype = _get_float_dtype(dtype)
     prob = prob.cast(float_dtype) if isinstance(prob, paddle.Tensor) else paddle.to_tensor(prob, dtype=float_dtype)
     prob_x, prob_y, prob_z = prob[0], prob[1], prob[2]
     prob_sum = paddle.sum(prob)
     assert prob_sum <= 1, \
         f"The sum of input probabilities should not be greater than 1: received {prob_sum.item()}"
-    prob_i = paddle.sqrt(1 - prob_sum)
+    prob_i = 1 - prob_sum
     kraus_oper = [
         [
             paddle.sqrt(prob_i).cast(dtype), _zero(dtype),
             _zero(dtype), paddle.sqrt(prob_i).cast(dtype),
         ],
         [
             _zero(dtype), paddle.sqrt(prob_x).cast(dtype),
@@ -396,15 +393,14 @@
 
     Args:
         prob: list of two probabilities of resetting to state :math:`|0\rangle` and :math:`|1\rangle`.
         dtype: data type. Defaults to be ``None``.
 
     Returns:
         a list of Kraus operators
-        
     """
     dtype = get_dtype() if dtype is None else dtype
     float_dtype = _get_float_dtype(dtype)
     prob = prob.cast(float_dtype) if isinstance(prob, paddle.Tensor) else paddle.to_tensor(prob, dtype=float_dtype)
     prob_0, prob_1 = prob[0], prob[1]
     prob_sum = paddle.sum(prob)
     assert prob_sum <= 1, \
@@ -433,34 +429,40 @@
         ],
     ]
     for idx, oper in enumerate(kraus_oper):
         kraus_oper[idx] = paddle.reshape(paddle.concat(oper), [2, 2])
     return kraus_oper
 
 
-def thermal_relaxation_kraus(const_t: Union[List[float], np.ndarray, paddle.Tensor], 
-                       exec_time: Union[List[float], np.ndarray, paddle.Tensor], dtype: str = None) -> List[paddle.Tensor]:
+def thermal_relaxation_kraus(
+        const_t: Union[List[float], np.ndarray, paddle.Tensor],
+        exec_time: Union[List[float], np.ndarray, paddle.Tensor], dtype: str = None
+) -> List[paddle.Tensor]:
     r"""Kraus representation of a thermal relaxation channel
 
     Args:
         const_t: list of :math:`T_1` and :math:`T_2` relaxation time in microseconds.
         exec_time: quantum gate execution time in the process of relaxation in nanoseconds.
         dtype: data type. Defaults to be ``None``.
 
     Returns:
         a list of Kraus operators.
-        
     """
     dtype = get_dtype() if dtype is None else dtype
     float_dtype = _get_float_dtype(dtype)
+    
     const_t = const_t.cast(float_dtype) if isinstance(const_t, paddle.Tensor) else paddle.to_tensor(const_t, dtype=float_dtype)
     t1, t2 = const_t[0], const_t[1]
+    assert t2 <= t1, \
+        f"The relaxation time T2 and T1 must satisfy T2 <= T1: received T2 {t2} and T1{t1}"
+    
     exec_time = exec_time.cast(float_dtype) / 1000 if isinstance(exec_time, paddle.Tensor) else paddle.to_tensor(exec_time / 1000, dtype=float_dtype)
     prob_reset = 1 - paddle.exp(-exec_time / t1)
     prob_z = (1 - prob_reset) * (1 - paddle.exp(-exec_time / t2) * paddle.exp(exec_time / t1)) / 2
+    prob_z = _zero(float_dtype) if paddle.abs(prob_z) <= 0 else prob_z
     prob_i = 1 - prob_reset - prob_z
     kraus_oper = [
         [
             paddle.sqrt(prob_i).cast(dtype), _zero(dtype),
             _zero(dtype), paddle.sqrt(prob_i).cast(dtype),
         ],
         [
@@ -474,8 +476,29 @@
         [
             _zero(dtype), paddle.sqrt(prob_reset).cast(dtype),
             _zero(dtype), _zero(dtype),
         ],
     ]
     for idx, oper in enumerate(kraus_oper):
         kraus_oper[idx] = paddle.reshape(paddle.concat(oper), [2, 2])
-    return kraus_oper
+    return kraus_oper
+
+
+def replacement_choi(sigma: Union[np.ndarray, paddle.Tensor, State], dtype: str = None) -> paddle.Tensor:
+    r"""Choi representation of a replacement channel
+
+    Args:
+        sigma: output state of this channel.
+        dtype: data type. Defaults to be ``None``.
+
+    Returns:
+        a Choi operator.
+    """
+    dtype = get_dtype() if dtype is None else dtype
+
+    # sanity check
+    sigma = sigma if isinstance(sigma, State) else State(sigma)
+    sigma.to('density_matrix')
+    sigma = sigma.data
+
+    dim = sigma.shape[0]
+    return paddle.kron(paddle.eye(dim), sigma).cast(dtype)
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/data_analysis/vqls.py` & `paddle-quantum-2.4.0/paddle_quantum/data_analysis/vqls.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,16 @@
     Returns:
         Return the real and imaginary part of the calculation.
 
     """
     # Return the real part
     cir = Circuit(2*num_qubits + 1)
     cir.h([0])
-    cir.control_oracle(An, range(num_qubits + 1), num_qubits=num_qubits+1)
-    cir.control_oracle(Am.conj().T, [0]+list(range(num_qubits+1, 2*num_qubits+1)), num_qubits=num_qubits+1)
+    cir.control_oracle(An, range(num_qubits + 1))
+    cir.control_oracle(Am.conj().T, [0]+list(range(num_qubits+1, 2*num_qubits+1)))
     for idx in range(num_qubits):
         cir.cnot([idx+1, idx+1+num_qubits])
     cir.h(range(num_qubits+1))
 
     input_state = to_state(paddle.kron(paddle.kron(zero_state(1).data, phi.data), b.data))
     result_state = cir(input_state)
     measure = pq.loss.measure.Measure()
@@ -177,16 +177,16 @@
                 P_0 = P_0 - measure(result_state, desired_result='0'+i+j)
                 P_1 = P_1 - measure(result_state, desired_result='1'+i+j)
     real_exp = P_0 - P_1
 
     # Return the imaginary part
     cir = Circuit(2*num_qubits + 1)
     cir.h([0])
-    cir.control_oracle(An, range(num_qubits + 1), num_qubits=num_qubits+1)
-    cir.control_oracle(Am.conj().T, [0]+list(range(num_qubits+1, 2*num_qubits+1)), num_qubits=num_qubits+1)
+    cir.control_oracle(An, range(num_qubits + 1))
+    cir.control_oracle(Am.conj().T, [0]+list(range(num_qubits+1, 2*num_qubits+1)))
     for idx in range(num_qubits):
         cir.cnot([idx+1,idx+1+num_qubits])
     cir.rz(qubits_idx=0, param=-np.pi/2)
     cir.h(range(num_qubits+1))
 
     result_state = cir(input_state)
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/data_analysis/vqr.py` & `paddle-quantum-2.4.0/paddle_quantum/data_analysis/vqr.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,17 @@
                       'mean_tweedie_deviance', 'mean_poisson_deviance', 'mean_gamma_deviance', 
                       'd2_tweedie_score', 'd2_pinball_score', 'd2_absolute_error_score']
 import warnings
 
 # paddle libs
 import paddle
 import paddle_quantum as pq
-from paddle_quantum.ansatz import Circuit
-from paddle_quantum.state import State, _type_fetch, _type_transform
+from ..ansatz import Circuit
+from ..state import State
+from ..intrinsic import _type_fetch, _type_transform
 from paddle_quantum.loss import Measure
 
 # format figures
 font_legend = font_manager.FontProperties(family='Times New Roman',
                                             # weight='bold',
                                             style='normal', size=12)
 font_label = {"family": "Times New Roman", "size": 14}
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/dataset.py` & `paddle-quantum-2.4.0/paddle_quantum/dataset.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/finance/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/finance/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 from .finance import(
     DataSimulator,
     portfolio_optimization_hamiltonian,
     portfolio_diversification_hamiltonian,
     arbitrage_opportunities_hamiltonian
 )
-from .pricing import qae_alg, qae_cir, qmc_alg, EuroOptionEstimator
+from .pricing import qae_alg, qae_cir, qmc_alg, EuroOptionEstimator, CreditRiskAnalyzer
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/finance/finance.py` & `paddle-quantum-2.4.0/paddle_quantum/finance/finance.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/finance/qpo.py` & `paddle-quantum-2.4.0/paddle_quantum/finance/qpo.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/fisher.py` & `paddle-quantum-2.4.0/paddle_quantum/fisher.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/gate/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/gate/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,21 +16,18 @@
 r"""
 The module of the quantum gates.
 """
 
 from . import functional
 from .base import Gate, ParamGate
 from .clifford import Clifford, compose_clifford_circuit
-from .single_qubit_gate import H, S, Sdg, T, Tdg, X, Y, Z, P, RX, RY, RZ, U3
-from .multi_qubit_gate import CNOT, CX, CY, CZ, SWAP
-from .multi_qubit_gate import CP, CRX, CRY, CRZ, CU, RXX, RYY, RZZ
-from .multi_qubit_gate import MS, CSWAP, Toffoli
-from .multi_qubit_gate import UniversalTwoQubits, UniversalThreeQubits
-from .custom import Oracle, ControlOracle
-from .layer import SuperpositionLayer, WeakSuperpositionLayer
-from .layer import LinearEntangledLayer, RealEntangledLayer, ComplexEntangledLayer
-from .layer import RealBlockLayer, ComplexBlockLayer
-from .layer import QAOALayer
+from .custom import Oracle, ControlOracle, ParamOracle
 from .encoding import BasisEncoding
 from .encoding import AmplitudeEncoding
 from .encoding import AngleEncoding
 from .encoding import IQPEncoding
+from .matrix import *
+from .multi_qubit_gate import CNOT, CX, CY, CZ, SWAP
+from .multi_qubit_gate import CP, CRX, CRY, CRZ, CU, RXX, RYY, RZZ
+from .multi_qubit_gate import MS, CSWAP, Toffoli, CCX
+from .multi_qubit_gate import UniversalTwoQubits, UniversalThreeQubits
+from .single_qubit_gate import H, S, Sdg, T, Tdg, X, Y, Z, P, RX, RY, RZ, U3
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/gate/clifford.py` & `paddle-quantum-2.4.0/paddle_quantum/gate/clifford.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/gate/custom.py` & `paddle-quantum-2.4.0/paddle_quantum/gate/custom.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,64 +16,38 @@
 r"""
 The source file of the oracle class and the control oracle class.
 """
 
 import math
 import matplotlib
 import paddle
+from typing import Callable, List, Union, Iterable
 
 import warnings
 import paddle_quantum as pq
 from . import functional
-from .base import Gate
-from ..intrinsic import _format_qubits_idx
-from typing import Union, Iterable
+from .base import Gate, ParamGate
 from .functional.visual import _c_oracle_like_display, _oracle_like_display
+from ..intrinsic import _format_qubits_idx
 
 
 class Oracle(Gate):
     """An oracle as a gate.
 
     Args:
         oracle: Unitary oracle to be implemented.
         qubits_idx: Indices of the qubits on which the gates are applied.
         num_qubits: Total number of qubits. Defaults to ``None``.
         depth: Number of layers. Defaults to ``1``.
     """
     def __init__(
-            self, oracle: paddle.Tensor, qubits_idx: Union[Iterable[Iterable[int]], Iterable[int], int],
+            self, oracle: paddle.Tensor, qubits_idx: Union[Iterable[Iterable[int]], Iterable[int], int] = None,
             num_qubits: int = None, depth: int = 1, gate_info: dict = None
     ):
-        super().__init__(depth)
-        complex_dtype = pq.get_dtype()
-        oracle = oracle.cast(complex_dtype)
-
-        dimension = oracle.shape[0]
-        err = paddle.norm(paddle.abs(oracle @ paddle.conj(oracle.T) - paddle.cast(paddle.eye(dimension), complex_dtype))).item()
-        if err > min(1e-6 * dimension, 0.01):
-            warnings.warn(
-                f"\nThe input oracle may not be a unitary: norm(U * U^d - I) = {err}.", UserWarning)
-
-        num_acted_qubits = int(math.log2(dimension))
-        self.oracle = oracle
-        self.qubits_idx = _format_qubits_idx(qubits_idx, num_qubits, num_acted_qubits)
-
-        self.gate_info = {
-            'gatename': 'O',
-            'texname': r'$O$',
-            'plot_width': 0.6,
-        }
-        if gate_info:
-            self.gate_info.update(gate_info)
-
-    def forward(self, state: pq.State) -> pq.State:
-        for _ in range(self.depth):
-            for qubits_idx in self.qubits_idx:
-                state = functional.oracle(state, self.oracle, qubits_idx, self.backend)
-        return state
+        super().__init__(oracle, qubits_idx, depth, gate_info, num_qubits)
     
     def display_in_circuit(self, ax: matplotlib.axes.Axes, x: float,) -> float:
         return _oracle_like_display(self, ax, x)
 
 
 class ControlOracle(Gate):
     """A controlled oracle as a gate.
@@ -84,42 +58,51 @@
         num_qubits: Total number of qubits. Defaults to ``None``.
         depth: Number of layers. Defaults to ``1``.
     """
     def __init__(
             self, oracle: paddle.Tensor, qubits_idx: Union[Iterable[Iterable[int]], Iterable[int]],
             num_qubits: int = None, depth: int = 1, gate_info: dict = None
     ) -> None:
-        super().__init__(depth)
-        complex_dtype = pq.get_dtype()
-        oracle = oracle.cast(complex_dtype)
+        complex_dtype = oracle.dtype
         
         dimension = oracle.shape[0]
-        err = paddle.norm(paddle.abs(oracle @ paddle.conj(oracle.T) - paddle.cast(paddle.eye(dimension), complex_dtype))).item()
-        if  err > min(1e-6 * dimension, 0.01):
-            warnings.warn(
-                f"\nThe input oracle may not be a unitary: norm(U * U^d - I) = {err}.", UserWarning)
-
-        num_acted_qubits = int(math.log2(dimension))
         oracle = (
-            paddle.kron(paddle.to_tensor([[1.0, 0], [0, 0]], dtype=complex_dtype), paddle.eye(2 ** num_acted_qubits)) +
+            paddle.kron(paddle.to_tensor([[1.0, 0], [0, 0]], dtype=complex_dtype), paddle.eye(dimension).cast(complex_dtype)) +
             paddle.kron(paddle.to_tensor([[0.0, 0], [0, 1]], dtype=complex_dtype), oracle)
         )
-        num_acted_qubits += 1
-        self.oracle = oracle
-        self.qubits_idx = _format_qubits_idx(qubits_idx, num_qubits, num_acted_qubits)
 
-        self.gate_info = {
+        default_gate_info = {
             'gatename': 'cO',
             'texname': r'$O$',
             'plot_width': 0.6,
         }
-        if gate_info:
-            self.gate_info.update(gate_info)
-
-    def forward(self, state: pq.State) -> pq.State:
-        for _ in range(self.depth):
-            for qubits_idx in self.qubits_idx:
-                state = functional.oracle(state, self.oracle, qubits_idx, self.backend)
-        return state
+        if gate_info is not None:
+            default_gate_info.update(gate_info)
+        super().__init__(oracle, qubits_idx, depth, gate_info, num_qubits)
 
     def display_in_circuit(self, ax: matplotlib.axes.Axes, x: float,) -> float:
         return _c_oracle_like_display(self, ax, x)
+
+
+class ParamOracle(ParamGate):
+    """An parameterized oracle as a gate
+
+    Args:
+        generator: function that generates the oracle.
+        param: input parameters of quantum parameterized gates. Defaults to ``None`` i.e. randomized.
+        qubits_idx: indices of the qubits on which this gate acts on. Defaults to ``None`` i.e. list(range(num_qubits)).
+        depth: number of layers. Defaults to ``1``.
+        num_acted_param: the number of parameters required for a single operation.
+        param_sharing: whether all operations are shared by the same parameter set.
+        gate_info: information of this gate that will be placed into the gate history or plotted by a Circuit. 
+        Defaults to ``None``.
+        num_qubits: total number of qubits. Defaults to ``None``.
+
+    """
+    def __init__(
+            self, generator: Callable[[paddle.Tensor], paddle.Tensor],
+            param: Union[paddle.Tensor, float, List[float]] = None,
+            depth: int = 1, num_acted_param: int = 1, param_sharing: bool = False,
+            qubits_idx: Union[Iterable[Iterable[int]], Iterable[int], int] = None,
+            gate_info: dict = None, num_qubits: int = None
+    ):
+        super().__init__(generator, param, depth, num_acted_param, param_sharing, qubits_idx, gate_info, num_qubits)
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/gate/encoding.py` & `paddle-quantum-2.4.0/paddle_quantum/gate/encoding.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,85 +14,96 @@
 # limitations under the License.
 
 r"""
 The source file of the classes for quantum encoding.
 """
 
 import paddle
-import paddle_quantum
-from paddle_quantum.gate import functional
-from .base import Gate
-from paddle_quantum.intrinsic import _get_float_dtype, _format_qubits_idx
+import paddle_quantum as pq
+from .functional.base import simulation
+from .matrix import x_gate, h_gate, cnot_gate, rx_gate, ry_gate, rz_gate
+from ..base import Operator
+from ..intrinsic import _get_float_dtype, _format_qubits_idx
 from typing import Iterable, Optional, Union
 
 
-class BasisEncoding(Gate):
+class BasisEncoding(Operator):
     r"""Basis encoding gate for encoding input classical data into quantum states.
 
     In basis encoding, the input classical data can only consist of 0's and 1's. If the input data are 1101,
     then the quantum state after encoding is :math:`|1101\rangle`. Note that the quantum state before encoding is
     assumed to be :math:`|00\ldots 0\rangle`.
 
     Args:
         qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
     """
+    
+    __x = x_gate('complex128')
+    
     def __init__(
             self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None
     ) -> None:
         super().__init__()
         self.num_qubits = num_qubits
         self.qubits_idx = _format_qubits_idx(qubits_idx, num_qubits)
-        self.gate_info['gatename'] = 'BasisEnc'
+        self.gate_info = {
+            'gatename': 'BasisEnc',
+            'texname': r'$\text{BasisEnc}$',
+            'plot_width': 1.5,
+        }
 
-    def forward(self, feature: paddle.Tensor, state: 'paddle_quantum.State' = None) -> 'paddle_quantum.State':
+    def forward(self, feature: paddle.Tensor, state: pq.State = None) -> pq.State:
+        x = BasisEncoding.__x.cast(self.dtype)
         if state is None:
-            state = paddle_quantum.state.zero_state(self.num_qubits)
+            state = pq.state.zero_state(self.num_qubits)
         feature = paddle.cast(feature, 'int32')
         gate_history = []
         for idx, element in enumerate(feature):
             if element:
-                state = functional.x(state, self.qubits_idx[idx], self.dtype, self.backend)
+                state = simulation(state, [x], self.qubits_idx[idx])
                 gate_history.append({'gate': 'x', 'which_qubits': self.qubits_idx[idx], 'theta': None})
         self.gate_history = gate_history
         return state
     
     def gate_history_generation(self) -> None:
         if self.gate_history is None:
-            raise RuntimeError("you must forward the encoding to receive the gate history")
-        pass
-        
+            raise RuntimeError("you must forward the encoding to receive the gate history")        
 
 
-class AmplitudeEncoding(Gate):
+class AmplitudeEncoding(Operator):
     r"""Amplitude encoding gate for encoding input classical data into quantum states.
 
     Args:
         qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
     """
     def __init__(
             self, qubits_idx: Optional[Union[Iterable[int], int, str]] = 'full', num_qubits: Optional[int] = None
     ) -> None:
         if num_qubits is None:
             num_qubits = max(qubits_idx)
         super().__init__()
         self.num_qubits = num_qubits
         self.qubits_idx = _format_qubits_idx(qubits_idx, num_qubits)
-        self.gate_info['gatename'] = 'AmpEnc'
+        self.gate_info = {
+            'gatename': 'AmpEnc',
+            'texname': r'$\text{AmpEnc}$',
+            'plot_width': 1.5,
+        }
 
-    def forward(self, feature: paddle.Tensor) -> 'paddle_quantum.State':
+    def forward(self, feature: paddle.Tensor) -> pq.State:
         def calc_location(location_of_bits_list):
             if len(location_of_bits_list) <= 1:
                 result_list = [0, location_of_bits_list[0]]
             else:
                 current_tmp = location_of_bits_list[0]
                 inner_location_of_qubits_list = calc_location(location_of_bits_list[1:])
                 current_list_len = len(inner_location_of_qubits_list)
-                for each in range(0, current_list_len):
+                for each in range(current_list_len):
                     inner_location_of_qubits_list.append(inner_location_of_qubits_list[each] + current_tmp)
                 result_list = inner_location_of_qubits_list
             return result_list
 
         def encoding_location_list(which_qubits):
             location_of_bits_list = []
             for qubit_idx in which_qubits:
@@ -101,35 +112,39 @@
             result_list = calc_location(location_of_bits_list)
 
             return sorted(result_list)
 
         # Get the specific position of the code, denoted by sequence number (list)
         location_of_qubits_list = encoding_location_list(self.qubits_idx)
         # Classical data preprocessing
-        feature = paddle.cast(feature, _get_float_dtype(paddle_quantum.get_dtype()))
+        feature = paddle.cast(feature, _get_float_dtype(pq.get_dtype()))
         feature = paddle.flatten(feature)
         length = paddle.norm(feature, p=2)
         # Normalization
         feature = paddle.divide(feature, length)
         # Create a quantum state with all zero amplitudes
         data = paddle.zeros((2 ** self.num_qubits,), feature.dtype)
         # The value of the encoded amplitude is filled into the specified qubits
-        for idx in range(0, len(feature)):
+        for idx in range(len(feature)):
             data[location_of_qubits_list[idx]] = feature[idx]
-        data = paddle.cast(data, dtype=paddle_quantum.get_dtype())
-        if self.backend == paddle_quantum.Backend.DensityMatrix:
+        data = paddle.cast(data, dtype=pq.get_dtype())
+        if self.backend == pq.Backend.DensityMatrix:
             data = paddle.unsqueeze(data, axis=1)
-            data = paddle.matmul(data, paddle_quantum.linalg.dagger(data))
-        elif self.backend != paddle_quantum.Backend.StateVector:
+            data = paddle.matmul(data, pq.linalg.dagger(data))
+        elif self.backend != pq.Backend.StateVector:
             raise ValueError("the mode should be state_vector or density_matrix")
-        encoding_state = paddle_quantum.state.to_state(data, self.num_qubits)
+        encoding_state = pq.state.to_state(data, self.num_qubits)
         return encoding_state
+    
+    def gate_history_generation(self) -> None:
+        if self.gate_history is None:
+            raise RuntimeError("you must forward the encoding to receive the gate history")
 
 
-class AngleEncoding(Gate):
+class AngleEncoding(Operator):
     r"""Angle encoding gate for encoding input classical data into quantum states.
 
     Args:
         feature: Vector to be encoded.
         qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``'full'``.
         num_qubits: Total number of qubits. Defaults to ``None``.
         encoding_gate: The type of quantum gates used for encoding, which should be one of ``"rx"``, ``"ry"``,
@@ -142,126 +157,138 @@
         if num_qubits is None:
             num_qubits = max(qubits_idx)
         super().__init__()
         self.num_qubits = num_qubits
         self.qubits_idx = _format_qubits_idx(qubits_idx, num_qubits)
         
         if encoding_gate == 'rx':
-            self.encoding_gate = functional.rx
+            self.encoding_gate = rx_gate
         elif encoding_gate == 'ry':
-            self.encoding_gate = functional.ry
+            self.encoding_gate = ry_gate
         elif encoding_gate == 'rz':
-            self.encoding_gate = functional.rz
+            self.encoding_gate = rz_gate
         self.encoding_gate_name = encoding_gate
         
-        feature = paddle.cast(feature, _get_float_dtype(paddle_quantum.get_dtype()))
+        feature = paddle.cast(feature, _get_float_dtype(pq.get_dtype()))
         feature = paddle.flatten(feature)
         self.feature = feature
         
-        self.gate_info['gatename'] = 'AngleEnc'
+        self.gate_info = {
+            'gatename': 'AngleEnc',
+            'texname': r'$\text{AngleEnc}$',
+            'plot_width': 1.5,
+        }
 
     def forward(
-            self, state: 'paddle_quantum.State' = None, invert: bool = False
-    ) -> 'paddle_quantum.State':
+            self, state: pq.State = None, invert: bool = False
+    ) -> pq.State:
         gate_history = []
         if state is None:
-            state = paddle_quantum.state.zero_state(self.num_qubits)
-        if invert:
-            feature = -1 * self.feature
-        else:
-            feature = self.feature
+            state = pq.state.zero_state(self.num_qubits)
+        feature = -1 * self.feature if invert else self.feature
+        
         for idx, element in enumerate(feature):
-            state = self.encoding_gate(
-                state, element[0], self.qubits_idx[idx],
-                dtype=self.dtype, backend=self.backend
-            )
+            param_matrix = self.encoding_gate(element[0])
+            state = simulation(state, [param_matrix], self.qubits_idx[idx])
             gate_history.append({'gate': self.encoding_gate_name, 'which_qubits': self.qubits_idx[idx], 'theta': element[0]})
         self.gate_history = gate_history
         return state
     
     def gate_history_generation(self) -> None:
         if self.gate_history is None:
             raise RuntimeError("you must forward the encoding to receive the gate history")
-        pass
 
 
-class IQPEncoding(Gate):
+class IQPEncoding(Operator):
     r"""IQP style encoding gate for encoding input classical data into quantum states.
 
     Args:
         feature: Vector to be encoded.
         qubits_idx: Indices of the qubits on which the gates are applied. Defaults to ``None``.
         num_qubits: Total number of qubits. Defaults to ``None``.
         num_repeat: Number of encoding layers. Defaults to ``1``.
     """
+    
+    __cnot = cnot_gate('complex128')
+    __h = h_gate('complex128')
+    
     def __init__(
             self, feature: paddle.Tensor, qubits_idx: Optional[Iterable[Iterable[int]]] = None,
             num_qubits: Optional[int] = None, num_repeat: Optional[int] = 1,
     ) -> None:
         super().__init__()
-        self.qubits_idx = [list(idx) for idx in qubits_idx]
+
         self.num_repeat = num_repeat
         self.num_qubits = num_qubits
         if feature is not None:
-            feature = paddle.cast(feature, _get_float_dtype(paddle_quantum.get_dtype()))
+            feature = paddle.cast(feature, _get_float_dtype(pq.get_dtype()))
             feature = paddle.flatten(feature)
             self.feature = feature
-            
-        self.gate_info['gatename'] = 'IQPEnc'
+
+        if qubits_idx is None:
+            assert num_qubits is not None, \
+                    f"Number of qubits must be known to create default patterns: received {num_qubits}"
+            qubits_idx = []
+            for idx0 in range(num_qubits):
+                qubits_idx.extend([idx0, idx1] for idx1 in range(idx0 + 1, num_qubits))
+        
+        self.qubits_idx = _format_qubits_idx(qubits_idx, num_qubits, num_acted_qubits=2)
+
+        self.gate_info = {
+            'gatename': 'IQPEnc',
+            'texname': r'$\text{IQPEnc}$',
+            'plot_width': 1.5,
+        }
 
     def forward(
-            self, state: paddle_quantum.State = None, invert: Optional[bool] = False
-    ) -> paddle_quantum.State:
+            self, state: pq.State = None, invert: Optional[bool] = False
+    ) -> pq.State:
         gate_history = []
+        h, cnot = IQPEncoding.__h.cast(self.dtype), IQPEncoding.__cnot.cast(self.dtype)
         if state is None:
-            state = paddle_quantum.state.zero_state(self.num_qubits)
-        for _ in range(0, self.num_repeat):
+            state = pq.state.zero_state(self.num_qubits)
+        for _ in range(self.num_repeat):
             if invert:
                 for qubits_idx in self.qubits_idx:
-                    state = functional.cnot(state, qubits_idx, dtype=self.dtype, backend=self.backend)
-                    state = functional.rz(
-                        state, -self.feature[qubits_idx[0]] * self.feature[qubits_idx[1]], qubits_idx[1],
-                        dtype=self.dtype, backend=self.backend
-                    )
-                    state = functional.cnot(state, qubits_idx, dtype=self.dtype, backend=self.backend)
+                    rz_param = -self.feature[qubits_idx[0]] * self.feature[qubits_idx[1]]
+                    state = simulation(state, [cnot], qubits_idx)
+                    state = simulation(state, [rz_gate(rz_param)], qubits_idx[1])
+                    state = simulation(state, [cnot], qubits_idx)
+
+                    gate_history.extend([
+                        {'gate': 'cnot', 'which_qubits': qubits_idx, 'theta': None},
+                        {'gate': 'rz', 'which_qubits': qubits_idx[1], 'theta': rz_param},
+                        {'gate': 'cnot', 'which_qubits': qubits_idx, 'theta': None}])
                     
-                    gate_history.append({'gate': 'cnot', 'which_qubits': qubits_idx, 'theta': None})
-                    gate_history.append({'gate': 'rz', 'which_qubits': qubits_idx[1], 
-                                         'theta': -self.feature[qubits_idx[0]] * self.feature[qubits_idx[1]]})
-                    gate_history.append({'gate': 'cnot', 'which_qubits': qubits_idx, 'theta': None})
-                    
-                for idx in range(0, self.feature.size):
-                    state = functional.rz(state, -self.feature[idx], idx, dtype=self.dtype, backend=self.backend)
+                for idx in range(self.feature.size):
+                    state = simulation(state, [rz_gate(-self.feature[idx])], idx)
                     gate_history.append({'gate': 'rz', 'which_qubits': idx, 'theta': -self.feature[idx]})
-                    
-                for idx in range(0, self.feature.size):
-                    state = functional.h(state, idx, dtype=self.dtype, backend=self.backend)
+
+                for idx in range(self.feature.size):
+                    state = simulation(state, [h], idx)
                     gate_history.append({'gate': 'h', 'which_qubits': idx, 'theta': None})
             else:
-                for idx in range(0, self.feature.size):
-                    state = functional.h(state, idx, dtype=self.dtype, backend=self.backend)
+                for idx in range(self.feature.size):
+                    state = simulation(state, [h], idx)
                     gate_history.append({'gate': 'h', 'which_qubits': idx, 'theta': None})
-                    
-                for idx in range(0, self.feature.size):
-                    state = functional.rz(state, self.feature[idx], idx, dtype=self.dtype, backend=self.backend)
+
+                for idx in range(self.feature.size):
+                    state = simulation(state, [rz_gate(self.feature[idx])], idx)
                     gate_history.append({'gate': 'rz', 'which_qubits': idx, 'theta': self.feature[idx]})
-                    
+
                 for qubits_idx in self.qubits_idx:
-                    state = functional.cnot(state, qubits_idx, dtype=self.dtype, backend=self.backend)
-                    state = functional.rz(
-                        state, self.feature[qubits_idx[0]] * self.feature[qubits_idx[1]], qubits_idx[1],
-                        dtype=self.dtype, backend=self.backend
-                    )
-                    state = functional.cnot(state, qubits_idx, dtype=self.dtype, backend=self.backend)
-                    
-                    gate_history.append({'gate': 'cnot', 'which_qubits': qubits_idx, 'theta': None})
-                    gate_history.append({'gate': 'rz', 'which_qubits': qubits_idx[1], 
-                                         'theta': self.feature[qubits_idx[0]] * self.feature[qubits_idx[1]]})
-                    gate_history.append({'gate': 'cnot', 'which_qubits': qubits_idx, 'theta': None})
+                    rz_param = self.feature[qubits_idx[0]] * self.feature[qubits_idx[1]]
+                    state = simulation(state, [cnot], qubits_idx)
+                    state = simulation(state, [rz_gate(rz_param)], qubits_idx[1])
+                    state = simulation(state, [cnot], qubits_idx)
                     
+                    gate_history.extend([
+                        {'gate': 'cnot', 'which_qubits': qubits_idx, 'theta': None},
+                        {'gate': 'rz', 'which_qubits': qubits_idx[1], 'theta': rz_param},
+                        {'gate': 'cnot', 'which_qubits': qubits_idx, 'theta': None}])
+        
         self.gate_history = gate_history
         return state
 
     def gate_history_generation(self) -> None:
         if self.gate_history is None:
             raise RuntimeError("you must forward the encoding to receive the gate history")
-        pass
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/gate/functional/visual.py` & `paddle-quantum-2.4.0/paddle_quantum/gate/functional/visual.py`

 * *Files 20% similar despite different names*

```diff
@@ -268,27 +268,42 @@
         qubits_idx: a list with different elements
     '''
     return len(qubits_idx) == max(qubits_idx) - min(qubits_idx) + 1
 
 
 def _not_exist_intersection(list_a: List[float], list_b: List[float]) -> bool:
     r'''Check whether there is an overlap in ``List_a`` and ``List_b``.
+
     Args:
         List_a: a list with two elements
         List_b: a list with two elements
     '''
     min_a = min(list_a)
     max_a = max(list_a)
     min_b = min(list_b)
     max_b = max(list_b)
     min_ab = min(min_a, min_b)
     max_ab = max(max_a, max_b)
     return max_a+max_b-min_a-min_b < max_ab-min_ab
 
 
+def _index_no_intersection_(index_list: List[List[int]]):
+    r'''Check whether there is an overlap in ``index_list``, 
+        which is a List of the List with two interger.
+
+    Args:
+        index_list: List of the List with two interger
+    '''
+    for i in range(len(index_list)):
+        for j in range(i+1, len(index_list)):
+            if not _not_exist_intersection(index_list[i], index_list[j]):
+                return False
+    return True
+
+
 def _base_gate_display(gate, ax: matplotlib.axes.Axes, x: float,) -> float:
     r'''The display function for single qubit base gate.
 
     Args:
         gate: the ``paddle_quantum.gate.Gate`` instance
         ax: the ``matplotlib.axes.Axes`` instance
         x: the start horizontal position
@@ -489,20 +504,24 @@
 
     Returns:
         the total width occupied
     '''
     x_start = x
     h = __CIRCUIT_PLOT_PARAM['circuit_height']
     w = __CIRCUIT_PLOT_PARAM['scale'] * gate.gate_info['plot_width']
+    parallel = _index_no_intersection_(gate.qubits_idx)
     for _ in range(gate.depth):
         for act_qubits in gate.qubits_idx:
             x_c = x + 0.5 * w
             _patch_display(ax, x_c, act_qubits[0]*h, mode='.')
             _patch_display(ax, x_c, act_qubits[1]*h, mode='+')
             _vertical_line_display(ax, x_c, act_qubits[0]*h, act_qubits[1]*h)
+            if not parallel:
+                x += w
+        if parallel:
             x += w
     return x - x_start
 
 
 def _swap_display(gate, ax: matplotlib.axes.Axes,  x: float,) -> float:
     r'''The display function for ``swap`` like gate.
 
@@ -513,20 +532,24 @@
 
     Returns:
         the total width occupied
     '''
     x_start = x
     h = __CIRCUIT_PLOT_PARAM['circuit_height']
     w = __CIRCUIT_PLOT_PARAM['scale'] * gate.gate_info['plot_width']
+    parallel = _index_no_intersection_(gate.qubits_idx)
     for _ in range(gate.depth):
         for act_qubits in gate.qubits_idx:
             x_c = x + 0.5 * w
             _patch_display(ax, x_c, act_qubits[0]*h, mode='x')
             _patch_display(ax, x_c, act_qubits[1]*h, mode='x')
             _vertical_line_display(ax, x_c, act_qubits[0]*h, act_qubits[1]*h)
+            if not parallel:
+                x += w
+        if parallel:
             x += w
     return x - x_start
 
 
 def _cswap_display(gate, ax: matplotlib.axes.Axes, x: float,) -> float:
     r'''The display function for ``cswap`` like gate.
 
@@ -573,244 +596,7 @@
             x_c = x + 0.5 * w
             _patch_display(ax, x_c, act_qubits[0]*h, mode='.')
             _patch_display(ax, x_c, act_qubits[1]*h, mode='.')
             _patch_display(ax, x_c, act_qubits[2]*h, mode='+')
             _vertical_line_display(ax, x_c, min(act_qubits)*h, max(act_qubits)*h)
             x += w
     return x - x_start
-
-
-def _linear_entangled_layer_display(gate, ax: matplotlib.axes.Axes, x: float,) -> float:
-    r'''The display function for ``linear entangled layer`` gate.
-
-    Args:
-        gate: the ``paddle_quantum.gate.Gate`` instance
-        ax: the ``matplotlib.axes.Axes`` instance
-        x: the start horizontal position
-
-    Returns:
-        the total width occupied
-    '''
-    x_start = x
-    h = __CIRCUIT_PLOT_PARAM['circuit_height']
-    block_w = __CIRCUIT_PLOT_PARAM['scale'] * gate.gate_info['plot_width']
-    dot_w = __CIRCUIT_PLOT_PARAM['node_width']
-
-    for depth in range(gate.depth):
-        for param_idx, act_qubits in enumerate(gate.qubits_idx):   # `ry` layer
-            _single_qubit_gate_display(ax, x, act_qubits*h, h, block_w,
-                                       f'$R_y({float(gate.theta[depth][param_idx][0]):.2f})$')
-        x += block_w
-
-        for idx in range(len(gate.qubits_idx)-1):   # `cnot` layer
-            act_qubits = [gate.qubits_idx[idx], gate.qubits_idx[idx + 1]]
-            x_c = x + 0.5 * dot_w
-            _patch_display(ax, x_c, act_qubits[0]*h, mode='.')
-            _patch_display(ax, x_c, act_qubits[1]*h, mode='+')
-            _vertical_line_display(ax, x_c, act_qubits[0]*h, act_qubits[1]*h)
-            x += dot_w
-
-        for param_idx, act_qubits in enumerate(gate.qubits_idx):   # `rz` layer
-            _single_qubit_gate_display(ax, x, act_qubits*h, h, block_w,
-                                       f'$R_z({float(gate.theta[depth][param_idx][1]):.2f})$')
-        x += block_w
-
-        for idx in range(len(gate.qubits_idx)-1):  # `cnot` layer
-            act_qubits = [gate.qubits_idx[idx], gate.qubits_idx[idx + 1]]
-            x_c = x + 0.5 * dot_w
-            _patch_display(ax, x_c, act_qubits[0]*h, mode='.')
-            _patch_display(ax, x_c, act_qubits[1]*h, mode='+')
-            _vertical_line_display(ax, x_c, act_qubits[0]*h, act_qubits[1]*h)
-            x += dot_w
-    return x - x_start
-
-
-def _cr_entangled_layer_display(gate, ax: matplotlib.axes.Axes, x: float,) -> float:
-    r'''The display function for ``complex or real entangled layer`` gate.
-
-    Args:
-        gate: the ``paddle_quantum.gate.Gate`` instance
-        ax: the ``matplotlib.axes.Axes`` instance
-        x: the start horizontal position
-
-    Returns:
-        the total width occupied
-    '''
-    tex_name = gate.gate_info['texname']
-    x_start = x
-    h = __CIRCUIT_PLOT_PARAM['circuit_height']
-    block_w = __CIRCUIT_PLOT_PARAM['scale'] * gate.gate_info['plot_width']
-    dot_w = __CIRCUIT_PLOT_PARAM['node_width']
-
-    if tex_name == '$REntLayer$':   # define the tex name generator for deferent gates
-        def _name_generator(theta):
-            return f'$R_y({float(theta):.2f})$'
-    elif tex_name == '$CEntLayer$':
-        def _name_generator(theta):
-            name = '$U('
-            for value in theta:
-                name += f'{float(value):.2f},'
-            name = name.strip(',')
-            name += ')$'
-            return name
-
-    for depth in range(gate.depth):
-        for param_idx, act_qubits in enumerate(gate.qubits_idx):
-            _single_qubit_gate_display(ax, x, act_qubits*h, h, block_w,
-                                       _name_generator(gate.theta[depth][param_idx]))
-        x += block_w
-        for idx in range(len(gate.qubits_idx)):
-            act_qubits = [gate.qubits_idx[idx], gate.qubits_idx[(idx + 1) % len(gate.qubits_idx)]]
-            x_c = x + 0.5 * dot_w
-            _patch_display(ax, x_c, act_qubits[0]*h, mode='.')
-            _patch_display(ax, x_c, act_qubits[1]*h, mode='+')
-            _vertical_line_display(ax, x_c, act_qubits[0]*h, act_qubits[1]*h)
-            x += dot_w
-    return x - x_start
-
-
-def _cr_block_layer_display(gate, ax: matplotlib.axes.Axes, x: float,) -> float:
-    r'''The display function for ``complex or real block layer`` gate.
-
-    Args:
-        gate: the ``paddle_quantum.gate.Gate`` instance
-        ax: the ``matplotlib.axes.Axes`` instance
-        x: the start horizontal position
-
-    Returns:
-        the total width occupied
-    '''
-    x_start = x
-    h = __CIRCUIT_PLOT_PARAM['circuit_height']
-    block_w = __CIRCUIT_PLOT_PARAM['scale'] * gate.gate_info['plot_width']
-    tex_name = gate.gate_info['texname']
-    dot_w = __CIRCUIT_PLOT_PARAM['node_width']
-
-    if tex_name == '$RBLayer$':
-        def _add_block(ax, x, theta, pos):  # add a block including 4 `ry` and 1 `cnot`
-            _single_qubit_gate_display(ax, x, pos[0]*h, h, block_w,
-                                       tex_name=f'$R_y({float(theta[0]):.2f})$')
-            _single_qubit_gate_display(ax, x, pos[1]*h, h, block_w,
-                                       tex_name=f'$R_y({float(theta[1]):.2f})$')
-            _single_qubit_gate_display(ax, x+block_w+dot_w, pos[0]*h, h, block_w,
-                                       tex_name=f'$R_y({float(theta[2]):.2f})$')
-            _single_qubit_gate_display(ax, x+block_w+dot_w, pos[1]*h, h, block_w,
-                                       tex_name=f'$R_y({float(theta[3]):.2f})$')
-            _patch_display(ax, x+block_w+0.5*dot_w, pos[0]*h, mode='.')
-            _patch_display(ax, x+block_w+0.5*dot_w, pos[1]*h, mode='+')
-            _vertical_line_display(ax, x+block_w+0.5*dot_w, pos[0]*h, pos[1]*h)
-
-    elif tex_name == '$CBLayer$':
-        def _add_block(ax, x, theta, pos,):     # add a block including 4 `u3` and 1 `cnot`
-            _single_qubit_gate_display(ax, x, pos[0]*h, h, block_w,
-                                       tex_name=f'$U({float(theta[0]):.2f},\
-                                        {float(theta[1]):.2f},{float(theta[2]):.2f})$')
-            _single_qubit_gate_display(ax, x, pos[1]*h, h, block_w,
-                                       tex_name=f'$U({float(theta[3]):.2f},\
-                                        {float(theta[4]):.2f},{float(theta[5]):.2f})$')
-            _single_qubit_gate_display(ax, x+block_w+dot_w, pos[0]*h, h, block_w,
-                                       tex_name=f'$U({float(theta[6]):.2f},\
-                                        {float(theta[7]):.2f},{float(theta[8]):.2f})$')
-            _single_qubit_gate_display(ax, x+block_w+dot_w, pos[1]*h, h, block_w,
-                                       tex_name=f'$U({float(theta[9]):.2f},\
-                                        {float(theta[10]):.2f},{float(theta[11]):.2f})$')
-            _patch_display(ax, x+block_w+0.5*dot_w, pos[0]*h, mode='.')
-            _patch_display(ax, x+block_w+0.5*dot_w, pos[1]*h, mode='+')
-            _vertical_line_display(ax, x+block_w+0.5*dot_w, pos[0]*h, pos[1]*h)
-
-    def _get_display_layer():  # arrange the order of block and compress
-        display_layer = []
-        num_theta_layer = [0, 0]
-        act_qubits = gate.qubits_idx
-        for layer in range(2):
-            indices = []
-            for i in range(1, len(act_qubits), 2):
-                indices.append([act_qubits[i-1], act_qubits[i]])
-            while len(indices) > 0:
-                indcs_list = [indices.pop(0)]
-                num_theta_layer[layer] += 1
-                for _ in range(len(indices)):
-                    candidate = indices.pop(0)
-                    if all(_not_exist_intersection(indcs, candidate) for indcs in indcs_list):
-                        indcs_list.append(candidate)
-                    else:
-                        indices.append(candidate)
-                display_layer.append(indcs_list)
-            act_qubits = act_qubits[1:]
-        return display_layer, num_theta_layer
-
-    def _add_layer(ax, x, theta, pos_list,):  # add block into layer
-        plotted_list = []
-        for pos in pos_list:
-            _add_block(ax, x, theta[int((gate.qubits_idx.index(pos[0])) / 2)], pos,)
-            plotted_list.extend(list(range(min(pos), max(pos)+1)))
-
-    display_layer, num_theta_layer = _get_display_layer()    # get layers
-    for depth in range(gate.depth):
-        for num_theta, layer in enumerate(display_layer):
-            if num_theta < num_theta_layer[0]:   # get parameters
-                _add_layer(ax, x, gate.theta[depth, :int((len(gate.qubits_idx)) / 2)], layer)
-            else:
-                _add_layer(ax, x, gate.theta[depth, int((len(gate.qubits_idx)) / 2):], layer)
-            x += 2 * block_w + dot_w
-    return x - x_start
-
-
-def _qaoa_layer_display(gate, ax: matplotlib.axes.Axes, x: float,) -> float:
-    r'''The display function for ``qaoa layer`` gate.
-
-    Args:
-        gate: the ``paddle_quantum.gate.Gate`` instance
-        ax: the ``matplotlib.axes.Axes`` instance
-        x: the start horizontal position
-
-    Returns:
-        the total width occupied
-    '''
-
-    x_start = x
-    h = __CIRCUIT_PLOT_PARAM['circuit_height']
-    block_w = __CIRCUIT_PLOT_PARAM['scale'] * gate.gate_info['plot_width']
-    dot_w = __CIRCUIT_PLOT_PARAM['node_width']
-
-    def _get_display_layer():    # arrange the order of block and compress
-        indices = gate.edges
-        display_layer = []
-        while len(indices) > 0:
-            indcs_list = [indices.pop(0)]
-            for _ in range(len(indices)):
-                candidate = indices.pop(0)
-                if all(_not_exist_intersection(indcs, candidate) for indcs in indcs_list):
-                    indcs_list.append(candidate)
-                else:
-                    indices.append(candidate)
-            display_layer.append(indcs_list)
-        return display_layer
-
-    def _add_block(ax, x, theta, pos):  # add a block including 2 `cnot` and 1 `rz`
-        _single_qubit_gate_display(ax, x+dot_w, pos[1]*h, h, block_w, tex_name=f'$R_z({float(theta):.2f})$')
-        _patch_display(ax, x+0.5*dot_w, pos[0]*h, mode='.')
-        _patch_display(ax, x+0.5*dot_w, pos[1]*h, mode='+')
-        _vertical_line_display(ax, x+0.5*dot_w, pos[0]*h, pos[1]*h)
-        _patch_display(ax, x+block_w+1.5*dot_w, pos[0]*h, mode='.')
-        _patch_display(ax, x+block_w+1.5*dot_w, pos[1]*h, mode='+')
-        _vertical_line_display(ax, x+block_w+1.5*dot_w, pos[0]*h, pos[1]*h)
-
-    def _add_layer(axis, x, theta, pos_list):  # add block into layer
-        plotted_list = []
-        for pos in pos_list:
-            _add_block(axis, x, theta, pos)
-            plotted_list.extend(list(range(min(pos), max(pos)+1)))
-
-    x_start = x
-    gamma = gate.theta[:gate.depth]
-    beta = gate.theta[gate.depth:]
-    display_layer = _get_display_layer()
-
-    for depth in range(gate.depth):
-        for layer in display_layer:
-            _add_layer(ax, x, gamma[depth], layer)
-            x += block_w + 2 * dot_w
-        for y in gate.nodes:
-            _single_qubit_gate_display(ax, x, y*h, h, block_w, tex_name=f'$R_x({float(beta[depth]):.2f})$')
-        x += block_w
-    return x - x_start
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/gradtool.py` & `paddle-quantum-2.4.0/paddle_quantum/gradtool.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/hamiltonian.py` & `paddle-quantum-2.4.0/paddle_quantum/hamiltonian.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import re
 from typing import Optional, Tuple
 import numpy as np
 from scipy import sparse
 import paddle
 import paddle_quantum
 import openfermion
+import math
 
 
 class Hamiltonian:
     r"""Hamiltonian ``class`` in Paddle Quantum.
 
     User can instantiate the ``class`` with a Pauli string.
 
@@ -297,15 +298,15 @@
             self.__decompose()
         return self.coefficients, self.__pauli_words
 
     def construct_h_matrix(self, qubit_num: Optional[int] = None) -> np.ndarray:
         r"""Construct a matrix form of the Hamiltonian in Z-basis.
 
         Args:
-            qubit_num: The number of qubits. Defaults to ``1``.
+            qubit_num: The number of qubits. Defaults to ``None``.
 
         Returns:
             The matrix form of the Hamiltonian in Z-basis.
         """
         coefs, pauli_words, sites = self.decompose_with_sites()
         if qubit_num is None:
             qubit_num = 1
@@ -329,14 +330,19 @@
             h_matrix += op
         return h_matrix
 
     @classmethod
     def from_qubit_operator(cls, qubitOp: openfermion.QubitOperator):
         pauli_strs = []
         for xyz_tuple, coef in qubitOp.terms.items():
+            if isinstance(coef, complex):
+                if not math.isclose(coef.imag, 0.0):
+                    raise ValueError("Coefficients in qubit Hamiltonian must be real since Hamiltonian is Hermitian.")
+                else:
+                    coef = coef.real
             if len(xyz_tuple) == 0:
                 pauli_strs.append((coef, "I"))
             else:
                 term = ", ".join(
                     [f"{g:s}{i:d}" for i, g in xyz_tuple]
                 )
                 pauli_strs.append((coef, term))
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/linalg.py` & `paddle-quantum-2.4.0/paddle_quantum/linalg.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,33 +20,32 @@
 import paddle
 import math
 import numpy as np
 import scipy
 import itertools
 from scipy.stats import unitary_group
 from functools import reduce
-from typing import Optional, Union, Callable, List
+from typing import Optional, Union, Callable, List, Tuple
 
 import paddle_quantum as pq
-from .intrinsic import _get_float_dtype
-from .state import State, _type_fetch, _type_transform
+from .intrinsic import get_dtype, _get_float_dtype, _type_fetch, _type_transform
 
 
-def abs_norm(mat: Union[np.ndarray, paddle.Tensor, State]) -> float:
+def abs_norm(mat: Union[np.ndarray, paddle.Tensor, pq.State]) -> float:
     r""" tool for calculation of matrix norm
 
     Args:
         mat: matrix
 
     Returns:
         norm of input matrix
 
     """
     mat = _type_transform(mat, "tensor")
-    mat = mat.cast(pq.get_dtype())
+    mat = mat.cast(get_dtype())
     return paddle.norm(paddle.abs(mat)).item()
 
 
 def dagger(mat: Union[np.ndarray, paddle.Tensor]) -> Union[np.ndarray, paddle.Tensor]:
     r""" tool for calculation of matrix dagger
 
     Args:
@@ -90,14 +89,90 @@
     
     """
     if is_hermitian(mat, eps):
         mat = _type_transform(mat, "tensor").cast('complex128')
         return (min(paddle.linalg.eigvalsh(mat)) >= -eps).item()
     return False
 
+
+def is_state_vector(vec: Union[np.ndarray, paddle.Tensor], eps: Optional[float] = None) -> Tuple[bool, int]:
+    r""" verify whether ``vec`` is a legal quantum state vector
+    
+    Args:
+        vec: state vector candidate :math:`x`
+        eps: tolerance of error, default to be `None` i.e. no testing for data correctness
+    
+    Returns:
+        determine whether :math:`x^\dagger x = 1`, and return the number of qubits or an error message
+        
+    Note:
+        error message is:
+        * ``-1`` if the above equation does not hold
+        * ``-2`` if the dimension of ``vec`` is not a power of 2
+        * ``-3`` if ``vec`` is not a vector
+    
+    """
+    vec = _type_transform(vec, "tensor")
+    vec = paddle.squeeze(vec)
+    
+    dimension = vec.shape[0]
+    if len(vec.shape) != 1:
+        return False, -3
+    
+    num_qubits = int(math.log2(dimension))
+    if 2 ** num_qubits != dimension:
+        return False, -2
+    
+    if eps is None:
+        return True, num_qubits
+    
+    vec = vec.reshape([dimension, 1])
+    vec_bra = paddle.conj(vec.T)   
+    eps = min(eps * dimension, 1e-2)
+    return {False, -1} if paddle.abs(vec_bra @ vec - (1 + 0j)) > eps else {True, num_qubits}
+
+
+def is_density_matrix(rho: Union[np.ndarray, paddle.Tensor], eps: Optional[float] = None) -> Tuple[bool, int]:
+    r""" verify whether ``rho`` is a legal quantum density matrix
+    
+    Args:
+        rho: density matrix candidate
+        eps: tolerance of error, default to be `None` i.e. no testing for data correctness
+    
+    Returns:
+        determine whether ``rho`` is a PSD matrix with trace 1 and return the number of qubits or an error message.
+    
+    Note:
+        error message is:
+        * ``-1`` if ``rho`` is not PSD
+        * ``-2`` if the trace of ``rho`` is not 1
+        * ``-3`` if the dimension of ``rho`` is not a power of 2 
+        * ``-4`` if ``rho`` is not a square matrix
+    
+    """
+    rho = _type_transform(rho, "tensor")
+    
+    dimension = rho.shape[0]
+    if len(rho.shape) != 2 or dimension != rho.shape[1]:
+        return False, -4
+    
+    num_qubits = int(math.log2(dimension))
+    if 2 ** num_qubits != dimension:
+        return False, -3
+    
+    if eps is None:
+        return True, num_qubits
+    
+    eps = min(eps * dimension, 1e-2)
+    if paddle.abs(paddle.trace(rho) - (1 + 0j)).item() > eps:
+        return False, -2
+    
+    return {False, -1} if not is_positive(rho, eps) else {True, num_qubits}
+
+
 def is_projector(mat: Union[np.ndarray, paddle.Tensor], eps: Optional[float] = 1e-6) -> bool:
     r""" verify whether ``mat`` is a projector
 
     Args:
         mat: projector candidate :math:`P`
         eps: tolerance of error
 
@@ -150,29 +225,29 @@
     for i in range(n):
         mat[i, i] = np.abs(mat[i, i])
         for j in range(i):
             mat[i, j] = np.conj(mat[j, i])
     
     eigval= np.linalg.eigvalsh(mat)
     max_eigval = np.max(np.abs(eigval))
-    return paddle.to_tensor(mat / max_eigval, dtype=pq.get_dtype())
+    return paddle.to_tensor(mat / max_eigval, dtype=get_dtype())
 
 
 def orthogonal_projection_random(num_qubits: int) -> paddle.Tensor:
     r"""randomly generate a :math:`2^n \times 2^n` rank-1 orthogonal projector
 
     Args:
         num_qubits: number of qubits :math:`n`
 
     Returns:
          a :math:`2^n \times 2^n` orthogonal projector
     """
     assert num_qubits > 0
     n = 2 ** num_qubits
-    float_dtype = _get_float_dtype(pq.get_dtype())
+    float_dtype = _get_float_dtype(get_dtype())
     vec = paddle.randn([n, 1], dtype=float_dtype) + 1j * paddle.randn([n, 1], dtype=float_dtype)
     mat = vec @ dagger(vec)
     return mat / paddle.trace(mat)
 
 
 def density_matrix_random(num_qubits: int) -> paddle.Tensor:
     r""" randomly generate an num_qubits-qubit state in density matrix form
@@ -180,33 +255,28 @@
     Args:
         num_qubits: number of qubits :math:`n`
     
     Returns:
         a :math:`2^n \times 2^n` density matrix
         
     """
-    float_dtype = _get_float_dtype(pq.get_dtype())
-    real = paddle.rand([2 ** num_qubits, 2 ** num_qubits], dtype=float_dtype)
-    imag = paddle.rand([2 ** num_qubits, 2 ** num_qubits], dtype=float_dtype)
-    M = real + 1j * imag
-    M = M @ dagger(M)
-    return M / paddle.trace(M)
+    return haar_density_operator(num_qubits, rank=np.random.randint(1,2**num_qubits))
 
 
 def unitary_random(num_qubits: int) -> paddle.Tensor:
     r"""randomly generate a :math:`2^n \times 2^n` unitary
 
     Args:
         num_qubits: number of qubits :math:`n`
 
     Returns:
          a :math:`2^n \times 2^n` unitary matrix
          
     """
-    return paddle.to_tensor(unitary_group.rvs(2 ** num_qubits), dtype=pq.get_dtype())
+    return paddle.to_tensor(unitary_group.rvs(2 ** num_qubits), dtype=get_dtype())
 
 
 def unitary_hermitian_random(num_qubits: int) -> paddle.Tensor:
     r"""randomly generate a :math:`2^n \times 2^n` hermitian unitary
 
     Args:
         num_qubits: number of qubits :math:`n`
@@ -238,15 +308,15 @@
     else:
         mat0 = hermitian_random(num_qubits - 1).numpy()
     id_mat = np.eye(2 ** (num_qubits - 1))
     mat1 = 1j * scipy.linalg.sqrtm(id_mat - np.matmul(mat0, mat0))
 
     mat = np.block([[mat0, mat1], [mat1, mat0]])
 
-    return paddle.to_tensor(mat, dtype=pq.get_dtype())
+    return paddle.to_tensor(mat, dtype=get_dtype())
 
 
 def block_enc_herm(mat: Union[np.ndarray, paddle.Tensor], 
                    num_block_qubits: int = 1) -> Union[np.ndarray, paddle.Tensor]:
     r""" generate a (qubitized) block encoding of hermitian ``mat``
     
     Args:
@@ -290,15 +360,15 @@
     # Step 1: sample from Ginibre ensemble
     ginibre = (np.random.randn(dim, dim))
     # Step 2: perform QR decomposition of G
     mat_q, mat_r = np.linalg.qr(ginibre)
     # Step 3: make the decomposition unique
     mat_lambda = np.diag(mat_r) / abs(np.diag(mat_r))
     mat_u = mat_q @ np.diag(mat_lambda)
-    return paddle.to_tensor(mat_u, dtype=pq.get_dtype())
+    return paddle.to_tensor(mat_u, dtype=get_dtype())
 
 
 def haar_unitary(num_qubits: int) -> paddle.Tensor:
     r""" randomly generate a unitary following Haar random, referenced by arXiv:math-ph/0609050v2
 
     Args:
         num_qubits: number of qubits :math:`n`
@@ -312,15 +382,15 @@
     # Step 1: sample from Ginibre ensemble
     ginibre = (np.random.randn(dim, dim) + 1j * np.random.randn(dim, dim)) / np.sqrt(2)
     # Step 2: perform QR decomposition of G
     mat_q, mat_r = np.linalg.qr(ginibre)
     # Step 3: make the decomposition unique
     mat_lambda = np.diag(mat_r) / np.abs(np.diag(mat_r))
     mat_u = mat_q @ np.diag(mat_lambda)
-    return paddle.to_tensor(mat_u, dtype=pq.get_dtype())
+    return paddle.to_tensor(mat_u, dtype=get_dtype())
 
 
 def haar_state_vector(num_qubits: int, is_real: Optional[bool] = False) -> paddle.Tensor:
     r""" randomly generate a state vector following Haar random
 
         Args:
             num_qubits: number of qubits :math:`n`
@@ -339,23 +409,23 @@
         phi = mat_orthog[:, 0]
     else:
         # Generate a Haar random unitary
         unitary = haar_unitary(num_qubits)
         # Perform u onto |0>, i.e., the first column of u
         phi = unitary[:, 0]
 
-    return paddle.to_tensor(phi, dtype=pq.get_dtype())
+    return paddle.to_tensor(phi, dtype=get_dtype())
 
 
 def haar_density_operator(num_qubits: int, rank: Optional[int] = None, is_real: Optional[bool] = False) -> paddle.Tensor:
     r""" randomly generate a density matrix following Haar random
 
         Args:
             num_qubits: number of qubits :math:`n`
-            rank: rank of density matrix, default to be False refering to full ranks
+            rank: rank of density matrix, default to be ``None`` refering to full ranks
             is_real: whether the density matrix is real, default to be False
 
         Returns:
             a :math:`2^n \times 2^n` density matrix
     """
     dim = 2 ** num_qubits
     rank = rank if rank is not None else dim
@@ -363,15 +433,15 @@
     if is_real:
         ginibre_matrix = np.random.randn(dim, rank)
         rho = ginibre_matrix @ ginibre_matrix.T
     else:
         ginibre_matrix = np.random.randn(dim, rank) + 1j * np.random.randn(dim, rank)
         rho = ginibre_matrix @ ginibre_matrix.conj().T
     rho = rho / np.trace(rho)
-    return paddle.to_tensor(rho / np.trace(rho), dtype=pq.get_dtype())
+    return paddle.to_tensor(rho, dtype=get_dtype())
 
 
 def direct_sum(A: Union[np.ndarray, paddle.Tensor], 
                B: Union[np.ndarray, paddle.Tensor]) -> Union[np.ndarray, paddle.Tensor]:
     r""" calculate the direct sum of A and B
     
     Args:
@@ -407,16 +477,16 @@
         *args: other matrices, as paddle.Tensor or numpy.ndarray
 
     Returns:
         Kronecker product of matrices, determined by input type of matrix_A
 
     .. code-block:: python
 
-        from pq.state import density_op_random
-        from pq.linalg import NKron
+        from paddle_quantum.state import density_op_random
+        from paddle_quantum.linalg import NKron
         A = density_op_random(2)
         B = density_op_random(2)
         C = density_op_random(2)
         result = NKron(A, B, C)
 
     Note:
         ``result`` from above code block should be A \otimes B \otimes C
@@ -426,15 +496,15 @@
 
     if type_A == "tensor":
         return reduce(lambda result, index: paddle.kron(result, index), args, paddle.kron(matrix_A, matrix_B), )
     else:
         return reduce(lambda result, index: np.kron(result, index), args, np.kron(matrix_A, matrix_B), )
 
     
-def herm_transform(fcn: Callable[[float], float], mat: Union[paddle.Tensor, np.ndarray, State], 
+def herm_transform(fcn: Callable[[float], float], mat: Union[paddle.Tensor, np.ndarray, pq.State], 
                    ignore_zero: Optional[bool] = False) -> paddle.Tensor:
     r""" function transformation for Hermitian matrix
     
     Args:
         fcn: function :math:`f` that can be expanded by Taylor series
         mat: hermitian matrix :math:`H`
         ignore_zero: whether ignore eigenspaces with zero eigenvalue, defaults to be ``False``
@@ -472,15 +542,15 @@
         The Pauli basis of :math:`\mathbb{C}^{2^n \times 2^n}`.
 
     """
     
     def __single_pauli_basis() -> List[paddle.Tensor]:
         r"""The Pauli basis in single-qubit case.
         """
-        complex_dtype = pq.get_dtype()
+        complex_dtype = get_dtype()
         I = paddle.to_tensor([[0.5, 0],
                             [0, 0.5]], dtype=complex_dtype)
         X = paddle.to_tensor([[0, 0.5],
                             [0.5, 0]], dtype=complex_dtype)
         Y = paddle.to_tensor([[0, -0.5j],
                             [0.5j, 0]], dtype=complex_dtype)
         Z = paddle.to_tensor([[0.5, 0],
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/locc/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/locc/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/locc/locc_ansatz.py` & `paddle-quantum-2.4.0/paddle_quantum/locc/locc_ansatz.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import collections
 import paddle
 import paddle_quantum
 from ..gate import H, S, T, X, Y, Z, P, RX, RY, RZ, U3
 from ..gate import CNOT, CX, CY, CZ, SWAP
 from ..gate import CP, CRX, CRY, CRZ, CU, RXX, RYY, RZZ
-from ..gate import MS, CSWAP, Toffoli
+from ..gate import MS, CSWAP, CCX
 from ..gate import UniversalTwoQubits, UniversalThreeQubits
 from ..gate import Oracle, ControlOracle
 from .locc_party import LoccParty
 from .locc_state import LoccState
 from paddle_quantum import Operator
 from typing import Iterable, Union, Optional, List
 
@@ -681,15 +681,15 @@
         """
         if num_qubits is None:
             num_qubits = self.num_local_qubits
         oper = CSWAP(qubits_idx, num_qubits, depth)
         self.append(oper)
         if num_qubits is None:
             num_qubits = self.num_local_qubits
-        oper = Toffoli(qubits_idx, num_qubits, depth)
+        oper = CCX(qubits_idx, num_qubits, depth)
         self.append(oper)
 
     def universal_two_qubits(
         self,
         qubits_idx: Union[Iterable, str] = "cycle",
         num_qubits: int = None,
         depth: int = 1,
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/locc/locc_net.py` & `paddle-quantum-2.4.0/paddle_quantum/locc/locc_net.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/locc/locc_party.py` & `paddle-quantum-2.4.0/paddle_quantum/locc/locc_party.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/locc/locc_state.py` & `paddle-quantum-2.4.0/paddle_quantum/locc/locc_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,29 @@
                 self.num_qubits = int(math.log2(data.shape[-1]))
             else:
                 self.num_qubits = num_qubits
         backend = paddle_quantum.get_backend() if backend is None else backend
         assert backend == paddle_quantum.Backend.DensityMatrix
         self.backend = backend
         self.dtype = dtype if dtype is not None else paddle_quantum.get_dtype()
+    
+    @property
+    def is_swap_back(self) -> bool:
+        return True
+    
+    @is_swap_back.setter
+    def is_swap_back(self, value: bool) -> None:
+        # Currently is_swap_back for LOCC state is banned.
+        # TODO: add optimization logic for LOCC module
+        pass
+    
+    def reset_sequence(self) -> None:
+        # Currently reset_sequence for LOCC state is banned.
+        # TODO: add optimization logic for LOCC module
+        pass
 
     def clone(self) -> "LoccState":
         r"""Create a copy of the current object.
 
         Returns:
             A copy of the current object.
         """
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/loss/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/loss/distance.py` & `paddle-quantum-2.4.0/paddle_quantum/loss/distance.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/loss/measure.py` & `paddle-quantum-2.4.0/paddle_quantum/loss/measure.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,136 +16,125 @@
 r"""
 The source file of the class for the measurement.
 """
 
 import paddle
 import paddle_quantum
 from ..backend import quleaf
-from ..backend import Backend
-from ..intrinsic import _get_float_dtype
-from typing import Optional, Union, Iterable
+from ..backend import Backend, state_vector
+from ..intrinsic import _get_float_dtype, _perm_of_list, _base_transpose, _base_transpose_for_dm
+from typing import Optional, Union, Iterable, List
 
 
 class ExpecVal(paddle_quantum.Operator):
     r"""The class of the loss function to compute the expectation value for the observable.
 
     This interface can make you using the expectation value for the observable as the loss function.
 
     Args:
         hamiltonian: The input observable.
         shots: The number of measurement shots. Defaults to ``0``. Now it just need to be input when the backend is QuLeaf.
     """
+
     def __init__(self, hamiltonian: paddle_quantum.Hamiltonian, shots: Optional[int] = 0):
         super().__init__()
         self.hamiltonian = hamiltonian
         self.shots = shots
         self.num_terms = self.hamiltonian.n_terms
         self.coeffs = paddle.to_tensor(self.hamiltonian.coefficients)
         self.sites = self.hamiltonian.sites
         self.matrices = self.hamiltonian.pauli_words_matrix
 
-    def __state_qubits_swap(self, pauli_site, state_data, num_qubits):
-        # generate swap_list
-        origin_seq = list(range(0, num_qubits))
-        target_seq = pauli_site + [x for x in origin_seq if x not in pauli_site]
-        swapped = [False] * num_qubits
-        swap_list = []
-        for idx in range(0, num_qubits):
-            if not swapped[idx]:
-                next_idx = idx
-                swapped[next_idx] = True
-                while not swapped[target_seq[next_idx]]:
-                    swapped[target_seq[next_idx]] = True
-                    if next_idx < target_seq[next_idx]:
-                        swap_list.append((next_idx, target_seq[next_idx]))
-                    else:
-                        swap_list.append((target_seq[next_idx], next_idx))
-                    next_idx = target_seq[next_idx]
-
-        # function for swapping ath and bth qubit in state
-        def swap_a_and_b(target_state, size, pos_a, pos_b):
-            target_state = target_state.reshape([2 ** pos_a, 2, 2 ** (pos_b - pos_a - 1), 2, 2 ** (size - pos_b - 1)])
-            return paddle.transpose(target_state, [0, 3, 2, 1, 4])
-
-        # begin swap
-        if self.backend == paddle_quantum.Backend.DensityMatrix:
-            for a, b in swap_list:
-                state_data = swap_a_and_b(state_data, 2 * num_qubits, a, b)
-                state_data = swap_a_and_b(state_data, 2 * num_qubits, a + num_qubits, b + num_qubits)
-        else:
-            for a, b in swap_list:
-                state_data = swap_a_and_b(state_data, num_qubits, a, b)
-        return state_data
-
-    def forward(self, state: paddle_quantum.State) -> paddle.Tensor:
+    def forward(self, state: paddle_quantum.State, decompose: Optional[bool] = False) -> Union[
+        paddle.Tensor, List[paddle.Tensor]]:
         r"""Compute the expectation value of the observable with respect to the input state.
 
         The value computed by this function can be used as a loss function to optimize.
 
         Args:
             state: The input state which will be used to compute the expectation value.
+            decompose: Defaults to ``False``.  If decompose is ``True``, it will return the expectation value of each term.
 
         Raises:
             NotImplementedError: The backend is wrong or not supported.
 
         Returns:
             The expectation value. If the backend is QuLeaf, it is computed by sampling.
         """
         if self.backend == Backend.QuLeaf:
-            if len(state.param_list) > 0:
-                param = paddle.concat(state.param_list)
-            else:
-                param = paddle.to_tensor(state.param_list)
+            param_list = [history['param'] for history in filter(lambda x: 'param' in x, state.oper_history)]
             expec_val = quleaf.ExpecValOp.apply(
-                param,
-                state, self.hamiltonian, self.shots
+                state,
+                self.hamiltonian,
+                paddle.to_tensor([self.shots], dtype=paddle.get_default_dtype()),
+                *param_list
             )
             return expec_val
 
         num_qubits = state.num_qubits
         float_dtype = _get_float_dtype(paddle_quantum.get_dtype())
-        expec_val = paddle.zeros([1], dtype=float_dtype)
+        origin_seq = list(range(num_qubits))
         state_data = state.data
-        for i in range(0, self.num_terms):
+        if self.backend == Backend.StateVector:
+            expec_val = paddle.zeros([state_data.reshape([-1, 2 ** num_qubits]).shape[0]], dtype=float_dtype)
+        elif self.backend == Backend.DensityMatrix:
+            expec_val = paddle.zeros([state_data.reshape([-1, 2 ** num_qubits, 2 ** num_qubits]).shape[0]],
+                                     dtype=float_dtype)
+        else:
+            raise NotImplementedError
+        expec_val_each_term = []
+        for i in range(self.num_terms):
             pauli_site = self.sites[i]
             if pauli_site == ['']:
                 expec_val += self.coeffs[i]
+                expec_val_each_term.append(self.coeffs[i])
                 continue
             num_applied_qubits = len(pauli_site)
             matrix = self.matrices[i]
-            # extract current state and do swap operation
-            if num_qubits != 1:
-                _state_data = self.__state_qubits_swap(pauli_site, state_data, num_qubits)
-            else:
-                _state_data = state_data
-            # use einstein sum notation to shrink the size of operation of matrix multiplication
+
             if self.backend == Backend.StateVector:
-                _state_data = _state_data.reshape([2 ** num_applied_qubits, 2 ** (num_qubits - num_applied_qubits)])
-                output_state = paddle.einsum('ia, ab->ib', matrix, _state_data).reshape([2 ** num_qubits])
-                _state_data = paddle.conj(_state_data.reshape([2 ** num_qubits]))
-                expec_val += paddle.real(paddle.matmul(_state_data, output_state)) * self.coeffs[i]
+                output_state, seq_for_acted = state_vector.unitary_transformation_without_swapback(
+                    state_data, [matrix], pauli_site, num_qubits, origin_seq)
+                perm_map = _perm_of_list(seq_for_acted, origin_seq)
+                output_state = _base_transpose(output_state, perm_map).reshape([-1, 2 ** num_qubits, 1])
+                state_data_bra = paddle.conj(state_data.reshape([-1, 1, 2 ** num_qubits]))
+                batch_values = paddle.squeeze(paddle.real(paddle.matmul(state_data_bra, output_state)), axis=[-2, -1]) * \
+                               self.coeffs[i]
+                expec_val_each_term.append(batch_values)
+                expec_val += batch_values
+
             elif self.backend == Backend.DensityMatrix:
-                _state_data = _state_data.reshape([2 ** num_applied_qubits, 2 ** (2 * num_qubits - num_applied_qubits)])
-                output_state = paddle.einsum('ia, ab->ib', matrix, _state_data)
-                output_state = output_state.reshape([2 ** num_qubits, 2 ** num_qubits])
-                expec_val += paddle.real(paddle.trace(output_state)) * self.coeffs[i]
+                seq_for_acted = pauli_site + [x for x in origin_seq if x not in pauli_site]
+                perm_map = _perm_of_list(origin_seq, seq_for_acted)
+                output_state = _base_transpose_for_dm(state_data, perm=perm_map).reshape(
+                    [-1, 2 ** num_applied_qubits, 2 ** (2 * num_qubits - num_applied_qubits)])
+                output_state = paddle.matmul(matrix, output_state).reshape(
+                    [-1, 2 ** num_qubits, 2 ** num_qubits])
+                batch_values = paddle.real(paddle.trace(output_state, axis1=-2, axis2=-1)) * self.coeffs[i]
+                expec_val_each_term.append(batch_values)
+                expec_val += batch_values
+
             else:
                 raise NotImplementedError
+
+        if decompose:
+            return expec_val_each_term
         return expec_val
 
 
 class Measure(paddle_quantum.Operator):
     r"""Compute the probability of the specified measurement result.
 
     Args:
         measure_basis: Specify the basis of the measurement. Defaults to ``'z'``.
 
     Raises:
         NotImplementedError: Currently we just support the z basis.
     """
+
     def __init__(self, measure_basis: Optional[Union[Iterable[paddle.Tensor], str]] = 'z'):
         super().__init__()
         if measure_basis == 'z' or measure_basis == 'computational_basis':
             self.measure_basis = 'z'
         else:
             raise NotImplementedError
 
@@ -160,15 +149,15 @@
             qubits_idx: The index of the qubits to be measured. Defaults to ``'full'`` which means measure all the qubits.
             desired_result: Specify the results of the measurement to return. Defaults to ``None`` which means return the probability of all the results.
 
         Raises:
             NotImplementedError: The backend is wrong or not supported.
             NotImplementedError: The qubit index is wrong or not supported.
             NotImplementedError: Currently we just support the z basis.
-            
+
         Returns:
             The probability of the measurement.
         """
         float_dtype = _get_float_dtype(paddle_quantum.get_dtype())
         num_qubits = state.num_qubits
         if self.measure_basis == 'z':
             if state.backend == paddle_quantum.Backend.StateVector:
@@ -194,15 +183,15 @@
                         target_qubits += binary[qubit_idx]
                     prob_array[int(target_qubits, base=2)] += prob_amplitude[idx]
             elif qubits_idx == 'full':
                 prob_array = prob_amplitude
             else:
                 raise NotImplementedError("The qubit index is wrong or not supported.")
 
-            prob_array = prob_array / paddle.sum(prob_array) # normalize calculation error
+            prob_array = prob_array / paddle.sum(prob_array)  # normalize calculation error
             if desired_result is None:
                 return prob_array
             if isinstance(desired_result, str):
                 desired_result = [desired_result]
                 prob_array = paddle.concat([prob_array[int(res, base=2)] for res in desired_result])
             return prob_array
         else:
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/main.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/main.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_0.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_0.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_1.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_1.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_2.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_2.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_3.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_3.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_4.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_4.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_5.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_5.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_6.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_6.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_7.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_7.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_8.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_8.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_9.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x5_10_9.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_0.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_0.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_1.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_1.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_2.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_2.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_3.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_3.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_4.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_4.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_5.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_5.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_6.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_6.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_7.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_7.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_8.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_8.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_9.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_5x6_10_9.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_0.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_0.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_1.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_1.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_2.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_2.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_3.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_3.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_4.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_4.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_5.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_5.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_6.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_6.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_7.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_7.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_8.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_8.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_9.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x6_10_9.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_0.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_0.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_1.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_1.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_2.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_2.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_3.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_3.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_4.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_4.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_5.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_5.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_6.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_6.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_7.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_7.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_8.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_8.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_9.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_6x7_10_9.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_0.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_0.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_1.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_1.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_2.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_2.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_3.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_3.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_4.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_4.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_5.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_5.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_6.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_6.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_7.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_7.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_8.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_8.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_9.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/example/rectangular/depth10/inst_7x7_10_9.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/GRCS/supremacy.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/GRCS/supremacy.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/example/maxcut_main.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/example/maxcut_main.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/example/pubo_main.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/example/pubo_main.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/maxcut.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/maxcut.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/pubo.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/pubo.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/QAOA/qaoa.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/QAOA/qaoa.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/QKernel/example/main.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/QKernel/example/main.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/QKernel/example/record_time.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/QKernel/example/record_time.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/QKernel/qkernel.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/QKernel/qkernel.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/VQSVD/example/main.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/VQSVD/example/main.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/VQSVD/example/record_time.txt` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/VQSVD/example/record_time.txt`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/VQSVD/vqsvd.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/VQSVD/vqsvd.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/mcalculus_tests/cnot_test.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/mcalculus_tests/cnot_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 CNOT test
 """
 
+import paddle
+import paddle_quantum
 from paddle_quantum.mbqc.utils import random_state_vector, compare_by_vector, compare_by_density
 from paddle_quantum.mbqc.simulator import MBQC
 from paddle_quantum.mbqc.qobject import Circuit, State
 from paddle_quantum.mbqc.mcalculus import MCalculus
-from paddle_quantum.circuit import UAnsatz
 
 n = 2  # Set the circuit width
 # Generate a random state vector
 input_psi = random_state_vector(2, is_real=False)
 
 # Instantiate a Circuit class
 cir = Circuit(n)
@@ -52,15 +53,16 @@
 mbqc.set_input_state(State(input_psi, [0, 1]))
 # Run computation by pattern
 mbqc.run_pattern()
 # Obtain the output state
 state_out = mbqc.get_quantum_output()
 
 # Find the standard result
-cir_std = UAnsatz(n)
+cir_std = paddle_quantum.Circuit(n)
 cir_std.cnot([0, 1])
-vec_std = cir_std.run_state_vector(input_psi.astype("complex128"))
+vec_std = cir_std(paddle_quantum.state.to_state(paddle.flatten(input_psi)))
+vec_std = vec_std.data
 system_std = state_out.system
 state_std = State(vec_std, system_std)
 # Compare with the standard result in UAnsatz
 compare_by_vector(state_out, state_std)
 compare_by_density(state_out, state_std)
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/mcalculus_tests/random_test.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/mcalculus_tests/random_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,48 +10,56 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from numpy import random, pi
 from paddle import to_tensor
-from paddle_quantum.circuit import UAnsatz
+import paddle
+import paddle_quantum
 from paddle_quantum.mbqc.simulator import MBQC
 from paddle_quantum.mbqc.transpiler import transpile
 from paddle_quantum.mbqc.qobject import Circuit, State
 from paddle_quantum.mbqc.utils import random_state_vector, compare_by_vector, compare_by_density
 
 n = 5  # Set the circuit width
 theta = to_tensor(random.rand(n) * 2 * pi, dtype='float64')  # Generate random angles
 
 # Instantiate a Circuit class
 cir_mbqc = Circuit(n)
 # Instantiate a UAnsatz class
-cir_ansatz = UAnsatz(n)
+cir_ansatz = paddle_quantum.Circuit(n)
 
 # Construct a circuit
-for cir in [cir_mbqc, cir_ansatz]:
-    for i in range(n):
-        cir.h(i)
-        cir.rx(theta[i], i)
-    cir.cnot([0, 1])
-    for i in range(n):
-        cir.ry(theta[i], i)
-        cir.rz(theta[i], i)
-
+# for cir in [cir_mbqc, cir_ansatz]:
+for i in range(n):
+    cir_mbqc.h(i)
+    cir_mbqc.rx(theta[i], i)
+cir_mbqc.cnot([0, 1])
+for i in range(n):
+    cir_mbqc.ry(theta[i], i)
+    cir_mbqc.rz(theta[i], i)
+for i in range(n):
+    cir_ansatz.h(i)
+    cir_ansatz.rx(i, param=theta[i])
+cir_ansatz.cnot([0, 1])
+for i in range(n):
+    cir_ansatz.ry(i, param=theta[i])
+    cir_ansatz.rz(i, param=theta[i])
 # Generate a random state vector
 input_psi = random_state_vector(n, is_real=False)
 # Transpile circuit to measurement pattern
 pattern = transpile(cir_mbqc)
 mbqc = MBQC()
 mbqc.set_pattern(pattern)
 mbqc.set_input_state(State(input_psi, list(range(n))))
 mbqc.run_pattern()
 # Obtain the output state
 state_out = mbqc.get_quantum_output()
 
 # Find the standard result
-vec_ansatz = cir_ansatz.run_state_vector(input_psi.astype("complex128"))
+vec_ansatz = cir_ansatz(paddle_quantum.state.to_state(paddle.flatten(input_psi)))
+vec_ansatz = vec_ansatz.data
 system_ansatz = state_out.system
 state_ansatz = State(vec_ansatz, system_ansatz)
 compare_by_vector(state_out, state_ansatz)
 compare_by_density(state_out, state_ansatz)
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/mcalculus_tests/single_qubit_unitary_test.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/mcalculus_tests/single_qubit_unitary_test.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/simulator_tests/cnot_test.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/simulator_tests/cnot_test.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/gates/simulator_tests/single_qubit_unitary_test.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/gates/simulator_tests/single_qubit_unitary_test.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/qobject.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/qobject.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,42 +8,43 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-此模块包含量子信息处理的常用对象，如量子态、量子电路、测量模式等。
+r"""
+This module contains the commonly used class in quantum information, e.g. quantum state, quantum circuit and measurement
+patterns.
 """
 
 from numpy import log2, sqrt
 from paddle import Tensor, to_tensor, t, conj, matmul
 
 __all__ = [
     "State",
     "Circuit",
     "Pattern"
 ]
 
 
 class State:
-    r"""定义量子态。
+    r"""Define the quantum state.
 
     Attributes:
-        vector (Tensor): 量子态的列向量
-        system (list): 量子态的系统标签列表
+        vector (Tensor): the column vector of the quantum state.
+        system (list): the list of system labels of the quantum state.
     """
 
     def __init__(self, vector=None, system=None):
-        r"""构造函数，用于实例化一个 ``"State"`` 量子态对象。
+        r""" the constructor for initialize an object of the class `` "State`` .
 
         Args:
-            vector (Tensor, optional): 量子态的列向量
-            system (list, optional): 量子态的系统标签列表
+            vector (Tensor, optional): the column vector of the quantum state.
+            system (list, optional): the list of system labels of the quantum state.
         """
         if vector is None and system is None:
             self.vector = to_tensor([1], dtype='float64')  # A trivial state
             self.system = []
             self.length = 1  # Length of state vector
             self.size = 0  # Number of qubits
         elif vector is not None and system is not None:
@@ -58,15 +59,15 @@
 
         else:
             raise ValueError("we should either input both 'vector' and 'system' or input nothing.")
         self.state = [self.vector, self.system]
         self.norm = sqrt(matmul(t(conj(self.vector)), self.vector).numpy())
 
     def __str__(self):
-        r"""打印该 ``State`` 类的信息，便于用户查看。
+        r"""print the information of this class
         """
         class_type_str = "State"
         vector_str = str(self.vector.numpy())
         system_str = str(self.system)
         length_str = str(self.length)
         size_str = str(self.size)
         print_str = class_type_str + "(" + \
@@ -74,50 +75,52 @@
                     "system=" + system_str + ", " + \
                     "length=" + length_str + ", " + \
                     "vector=\r\n" + vector_str + ")"
         return print_str
 
 
 class Circuit:
-    r"""定义量子电路。
+    r"""Define the quantum circuit.
 
     Note:
-        该类与 ``UAnsatz`` 类似，用户可以仿照 ``UAnsatz`` 电路的调用方式对此类进行实例化，完成电路图的构建。
+        This class is similar to ``UAnsatz``, one can imitate the use of ``UAnsatz`` to instantiate this class and
+        construct the circuit diagram.
 
     Warning:
-        当前版本仅支持 ``H, X, Y, Z, S, T, Rx, Ry, Rz, Rz_5, U, CNOT, CNOT_15, CZ`` 中的量子门以及测量操作。
+        The current version supports the quantum operations(gates and measurement) in ``H, X, Y, Z, S, T, Rx, Ry,
+        Rz, Rz_5, U, CNOT, CNOT_15, CZ``.
 
     Attributes:
-        width (int): 电路的宽度（比特数）
+        width (int): The width of the circuit(number of qubits).
     """
 
     def __init__(self, width):
-        r"""``Circuit`` 的构造函数，用于实例化一个 ``Circuit`` 对象。
+        r""" The constructor of the class ``Circuit`` used of instantiate an object.
 
         Args:
-            width (int): 电路的宽度（比特数）
+            width (int): The width of the circuit(number of qubits).
         """
         assert isinstance(width, int), "circuit 'width' must be a int."
         self.__history = []  # A list to record the circuit information
         self.__measured_qubits = []  # A list to record the measurement indices in the circuit
         self.__width = width  # The width of circuit
 
     def h(self, which_qubit):
-        r"""添加 ``Hadamard`` 门。
+        r"""Add a ``Hadamard`` gate.
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \frac{1}{\sqrt{2}}\begin{bmatrix} 1&1\\1&-1 \end{bmatrix}
 
         Args:
-            which_qubit (int): 作用量子门的量子位编号
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
             which_qubit = 0
@@ -130,26 +133,26 @@
         """
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['h', [which_qubit], None])
 
     def x(self, which_qubit):
-        r"""添加 ``Pauli X`` 门。
+        r"""Add a ``Pauli X`` gate.
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
 
         Args:
-            which_qubit (int): 作用量子门的量子位编号
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
             which_qubit = 0
@@ -162,26 +165,26 @@
         """
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['x', [which_qubit], None])
 
     def y(self, which_qubit):
-        r"""添加 ``Pauli Y`` 门。
+        r"""Add a ``Pauli Y`` gate.
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix}
 
         Args:
-            which_qubit (int): 作用量子门的量子位编号
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
             which_qubit = 0
@@ -194,26 +197,26 @@
         """
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['y', [which_qubit], None])
 
     def z(self, which_qubit):
-        r"""添加 ``Pauli Z`` 门。
+        r"""Add a ``Pauli Z`` gate.
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}
 
         Args:
-            which_qubit (int): 作用量子门的量子位编号
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
             which_qubit = 0
@@ -226,26 +229,26 @@
         """
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['z', [which_qubit], None])
 
     def s(self, which_qubit):
-        r"""添加 ``S`` 门。
+        r"""Add a ``S`` gate.
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \begin{bmatrix} 1&0\\0& i \end{bmatrix}
 
         Args:
-            which_qubit (int): 作用量子门的量子位编号
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
             which_qubit = 0
@@ -258,26 +261,26 @@
         """
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['s', [which_qubit], None])
 
     def t(self, which_qubit):
-        r"""添加 ``T`` 门。
+        r"""Add ``T`` gate.
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \begin{bmatrix} 1&0\\0& e^{i\pi/ 4} \end{bmatrix}
 
         Args:
-            which_qubit (int): 作用量子门的量子位编号
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
             which_qubit = 0
@@ -290,27 +293,27 @@
         """
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['t', [which_qubit], None])
 
     def rx(self, theta, which_qubit):
-        r"""添加关于 x 轴的旋转门。
+        r"""Add a rotation gate in x direction.
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \begin{bmatrix} \cos\frac{\theta}{2} & -i\sin\frac{\theta}{2} \\ -i\sin\frac{\theta}{2} & \cos\frac{\theta}{2} \end{bmatrix}
 
         Args:
-            theta (Tensor): 旋转角度
-            which_qubit (int): 作用量子门的量子位编号
+            theta (Tensor): rotation angle
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         ..  code-block:: python
 
             from paddle import to_tensor
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
@@ -326,27 +329,27 @@
         assert isinstance(theta, Tensor) and theta.shape == [1], "'theta' must be a 'Tensor' of shape [1]."
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['rx', [which_qubit], theta])
 
     def ry(self, theta, which_qubit):
-        r"""添加关于 y 轴的旋转门。
+        r"""Add a rotation gate in y direction.
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \begin{bmatrix} \cos\frac{\theta}{2} & -\sin\frac{\theta}{2} \\ \sin\frac{\theta}{2} & \cos\frac{\theta}{2} \end{bmatrix}
 
         Args:
-            theta (Tensor): 旋转角度
-            which_qubit (int): 作用量子门的量子位编号
+            theta (Tensor): rotation angle
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         ..  code-block:: python
 
             from paddle import to_tensor
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
@@ -362,27 +365,27 @@
         assert isinstance(theta, Tensor) and theta.shape == [1], "'theta' must be a 'Tensor' of shape [1]."
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['ry', [which_qubit], theta])
 
     def rz(self, theta, which_qubit):
-        r"""添加关于 z 轴的旋转门。
+        r"""Add a rotation gate in z direction.
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \begin{bmatrix} 1 & 0 \\ 0 & e^{i\theta} \end{bmatrix}
 
         Args:
-            theta (Tensor): 旋转角度
-            which_qubit (int): 作用量子门的量子位编号
+            theta (Tensor): rotation angle
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         ..  code-block:: python
 
             from paddle import to_tensor
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
@@ -398,27 +401,28 @@
         assert isinstance(theta, Tensor) and theta.shape == [1], "'theta' must be a 'Tensor' of shape [1]."
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['rz', [which_qubit], theta])
 
     def rz_5(self, theta, which_qubit):
-        r"""添加关于 z 轴的旋转门（该旋转门对应的测量模式由五个量子比特构成）。
+        r"""Add a rotation gate in the z direction(the measurement pattern corresponding to this gate
+        is composed of five qubits).
 
-        其矩阵形式为：
+        The matrix form:
 
         .. math::
 
             \begin{bmatrix} 1 & 0 \\ 0 & e^{i\theta} \end{bmatrix}
 
         Args:
-            theta (Tensor): 旋转角度
-            which_qubit (int): 作用量子门的量子位编号
+            theta (Tensor): rotation angle
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         ..  code-block:: python
 
             from paddle import to_tensor
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
             cir = Circuit(width)
@@ -434,30 +438,31 @@
         assert isinstance(theta, Tensor) and theta.shape == [1], "'theta' must be a 'Tensor' of shape [1]."
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['rz_5', [which_qubit], theta])
 
     def u(self, params, which_qubit):
-        r"""添加单量子比特的任意酉门。
+        r"""Add a general single qubit gate.
 
         Warning:
-            与 ``UAnsatz`` 类中的 U3 的三个参数不同，这里的酉门采用 ``Rz Rx Rz`` 分解，
+            Different from the 3 parameters of the U3 gate in ``UAnsatz``  class，
+            the unitary here adopts a ``Rz Rx Rz`` decomposition.
 
-        其分解形式为：
+        The decomposition takes the form:
 
         .. math::
 
             U(\alpha, \beta, \gamma) = Rz(\gamma) Rx(\beta) Rz(\alpha)
 
         Args:
-            params (list): 单比特酉门的三个旋转角度
-            which_qubit (int): 作用量子门的量子位编号
+            params (list): three rotation angles of the unitary gate
+            which_qubit (int): The number(No.) of the qubit that the gate applies to.
 
-        代码示例：
+        Code example:
 
         ..  code-block:: python
 
             from paddle import to_tensor
             from numpy import pi
             from paddle_quantum.mbqc.qobject import Circuit
             width = 1
@@ -481,26 +486,27 @@
             "item in 'params' must be 'Tensor' of shape [1]."
         assert isinstance(which_qubit, int), "'which_qubit' must be a 'int'."
         assert 0 <= which_qubit < self.__width, "'which_qubit' must be a int between zero and circuit width."
         assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
         self.__history.append(['u', [which_qubit], params])
 
     def cnot(self, which_qubits):
-        r"""添加控制非门。
+        r"""Add a CNOT gate.
 
-        当 ``which_qubits`` 为 ``[0, 1]`` 时，其矩阵形式为：
+        When  ``which_qubits`` is ``[0, 1]`` ，the matrix form is:
 
         .. math::
 
             \begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 1 & 0 \end{bmatrix}
 
         Args:
-            which_qubits (list): 作用量子门的量子位，其中列表第一个元素为控制位，第二个元素为受控位
+            which_qubits (list): A two element list contains the qubits that the CNOT gate applies to, the first
+                element is the control qubit, the second is the target qubit.
 
-        代码示例：
+        Code example:
 
         ..  code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             width = 2
             cir = Circuit(width)
             which_qubits = [0, 1]
@@ -518,26 +524,27 @@
         assert which_qubits[0] != which_qubits[1], \
             "control qubit must not be the same as the target qubit."
         assert which_qubits[0] not in self.__measured_qubits and which_qubits[1] not in self.__measured_qubits, \
             "one of the qubits has already been measured."
         self.__history.append(['cnot', which_qubits, None])
 
     def cnot_15(self, which_qubits):
-        r"""添加控制非门 （该门对应的测量模式由十五个量子比特构成）。
+        r"""Add a CNOT gate(the measurement pattern corresponding to this gate is composed of 15 qubits).
 
-        当 ``which_qubits`` 为 ``[0, 1]`` 时，其矩阵形式为：
+        When ``which_qubits`` is ``[0, 1]`` ，the matrix form is:
 
         .. math::
 
             \begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 1 & 0 \end{bmatrix}
 
         Args:
-            which_qubits (list): 作用量子门的量子位，其中列表第一个元素为控制位，第二个元素为受控位
+            which_qubits (list): A two element list contains the qubits that the CNOT gate applies to, the first
+                element is the control qubit, the second is the target qubit.
 
-        代码示例：
+        Code example:
 
         ..  code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             width = 2
             cir = Circuit(width)
             which_qubits = [0, 1]
@@ -555,26 +562,27 @@
         assert which_qubits[0] != which_qubits[1], \
             "control qubit must not be the same as the target qubit."
         assert which_qubits[0] not in self.__measured_qubits and which_qubits[1] not in self.__measured_qubits, \
             "one of the qubits has already been measured."
         self.__history.append(['cnot_15', which_qubits, None])
 
     def cz(self, which_qubits):
-        r"""添加控制 Z 门。
+        r"""Add a controlled-Z gate.
 
-        当 ``which_qubits`` 为 ``[0, 1]`` 时，其矩阵形式为：
+        When ``which_qubits`` is ``[0, 1]`` ，the matrix form is:
 
         .. math::
 
             \begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & -1 \end{bmatrix}
 
         Args:
-            which_qubits (list): 作用量子门的量子位，其中列表第一个元素为控制位，第二个元素为受控位
+            which_qubits (list): A two element list contains the qubits that the CZ gate applies to, the first
+                element is the control qubit, the second is the target qubit.
 
-        代码示例：
+        Code example:
 
         ..  code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             width = 2
             cir = Circuit(width)
             which_qubits = [0, 1]
@@ -592,30 +600,33 @@
         assert which_qubits[0] != which_qubits[1], \
             "control qubit must not be the same as the target qubit."
         assert which_qubits[0] not in self.__measured_qubits and which_qubits[1] not in self.__measured_qubits, \
             "one of the qubits has already been measured."
         self.__history.append(['cz', which_qubits, None])
 
     def measure(self, which_qubit=None, basis_list=None):
-        r"""对量子电路输出的量子态进行测量。
+        r"""Measure the output state of the quantum circuit.
 
         Note:
-            与 ``UAnsatz`` 类中的测量不同，除默认的 Z 测量外，此处的测量方式可以由用户自定义，但需要将测量方式与测量比特相对应。
+            Unlike the measurement operations in the ``UAnsatz`` class, besides the default measurement in Z basis,
+            the users can define the measurement ways themselves by providing the measurement basis and the qubits
+            to be measured.
 
         Warning:
-            此方法只接受三种输入方式：
-            1. 不输入任何参数，表示对所有的量子位进行 Z 测量；
-            2. 输入量子位，但不输入测量基，表示对输入的量子位进行 Z 测量；
-            3. 输入量子位和对应测量基，表示对输入量子位进行指定的测量。
-            如果用户希望自定义测量基参数，需要注意输入格式为 ``[angle, plane, domain_s, domain_t]``，
-            且当前版本的测量平面 ``plane`` 只能支持 ``XY`` 或 ``YZ``。
+            There are three kinds of inputs:
+            1. which_qubit=None,basis_list=None(default): measure all the qubits in Z basis.
+            2. which_qubit=input, basis_list=None: measure the input qubit in Z basis.
+            3. which_qubit=input1, basis_list=input2: measure the input1 qubit by the basis in input2.
+            If the users want to define the measurement basis themselves, the input format looks like:
+            ``[angle,plane,domain_s,domain_t]``. By the way,in the current version paddle_quantum, the
+            ``plane`` parameter can only take ``XY`` or ``YZ``.
 
         Args:
-            which_qubit (int, optional): 被测量的量子位
-            basis_list (list, optional): 测量方式
+            which_qubit (int, optional): the qubit to be measured
+            basis_list (list, optional): measurement basis
         """
         # Measure all the qubits by Z measurement
         if which_qubit is None and basis_list is None:
             # Set Z measurement by default
             basis_list = [to_tensor([0], dtype='float64'), 'YZ', [], []]
             for which_qubit in range(self.__width):
                 assert which_qubit not in self.__measured_qubits, "this qubit has already been measured."
@@ -641,60 +652,60 @@
             assert basis_list[1] in ["XY", "YZ"], "measurement plane must be 'XY' or 'YZ'."
             self.__measured_qubits.append(which_qubit)
             self.__history.append(['m', [which_qubit], basis_list])
         else:
             raise ValueError("such a combination of input parameters is not supported. Please see our API for details.")
 
     def is_valid(self):
-        r"""检查输入的量子电路是否符合规定。
+        r"""Check that if the circuit is valid.
 
-        我们规定输入的量子电路中，每一个量子位上至少作用一个量子门。
+        We require that for each qubit in the quantum circuit, at least one quantum gate should be applied to it.
 
         Returns:
-            bool: 量子电路是否符合规定的布尔值
+            bool: the boolean values of whether the quantum circuit is valid.
         """
         all_qubits = []
         for gate in self.__history:
             if gate[0] != 'm':
                 all_qubits += gate[1]
         effective_qubits = list(set(all_qubits))
 
         return self.__width == len(effective_qubits)
 
     def get_width(self):
-        r"""返回量子电路的宽度。
+        r"""Return the width of the quantum circuit.
 
         Returns:
-           int: 量子电路的宽度
+           int: the width of the quantum circuit.
         """
         return self.__width
 
     def get_circuit(self):
-        r"""返回量子电路列表。
+        r"""Return the list of quantum circuits.
 
         Returns:
-            list: 量子电路列表
+            list: the list of quantum circuits
         """
         return self.__history
 
     def get_measured_qubits(self):
-        r"""返回量子电路中测量的比特位。
+        r"""Return the list of measured qubits in the quantum circuit.
 
         Returns:
-            list: 量子电路中测量的比特位列表
+            list: the list of measured qubits in the quantum circuit.
         """
         return self.__measured_qubits
 
     def print_circuit_list(self):
-        r"""打印电路图的列表。
+        r"""Print the list of the circuit.
 
         Returns:
-            string: 用来打印的字符串
+            string: the strings to be printed
 
-        代码示例:
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             from paddle import to_tensor
             from numpy import pi
 
@@ -738,168 +749,177 @@
             else:
                 par_show = parameters
             print(str(name).ljust(16) + str(which_qubits).ljust(16) + str(par_show).ljust(16))
         print("--------------------------------------------------")
 
 
 class Pattern:
-    r"""定义测量模式。
+    r"""Define the measurement pattern.
 
-    该测量模式的结构依据文献 [The measurement calculus, arXiv: 0704.1263]。
+    see more details of the measurement pattern in [The measurement calculus, arXiv: 0704.1263].
 
     Attributes:
-        name (str): 测量模式的名称
-        space (list): 测量模式所有节点列表
-        input_ (list): 测量模式的输入节点列表
-        output_ (list): 测量模式的输出节点列表
-        commands (list): 测量模式的命令列表
+        name (str): the name of the measurement pattern.
+        space (list): the list contains all the nodes of the measurement pattern.
+        input_ (list): the list contains the input nodes of the measurement pattern.
+        output_ (list): the list contains the output nodes of the measurement pattern.
+        commands (list): the list contains the commands of the measurement pattern.
     """
 
     def __init__(self, name, space, input_, output_, commands):
-        r"""构造函数，用于实例化一个 ``Pattern`` 对象。
+        r"""Constructor of the class ``Pattern`` used for instantiated an object.
 
         Args:
-            name (str): 测量模式的名称
-            space (list): 测量模式所有节点列表
-            input_ (list): 测量模式的输入节点列表
-            output_ (list): 测量模式的输出节点列表
-            commands (list): 测量模式的命令列表
+            name (str): the name of the measurement pattern.
+            space (list): the list contains all the nodes of the measurement pattern.
+            input_ (list): the list contains the input nodes of the measurement pattern.
+            output_ (list): the list contains the output nodes of the measurement pattern.
+            commands (list): the list contains the commands of the measurement pattern.
         """
         self.name = name
         self.space = space
         self.input_ = input_
         self.output_ = output_
         self.commands = commands
 
     class CommandE:
-        r"""定义纠缠命令类。
+        r"""Define the class ``CommandE`` corresponding to some entanglement commands.
 
         Note:
-            此处纠缠命令对应作用控制 Z 门。
+            The entanglement command here corresponds to the controlled-Z gate.
 
         Attributes:
-            which_qubits (list): 作用纠缠命令的两个节点标签构成的列表
+            which_qubits (list): A two-element list contains the labels of the node
+            that the entanglement command applies to.
         """
 
         def __init__(self, which_qubits):
-            r"""纠缠命令类构造函数，用于实例化一个 ``CommandE`` 对象。
+            r""" Constructor of the ``CommandE`` class used for instantiate an object.
 
             Args:
-                which_qubits (list): 作用纠缠命令的两个节点标签构成的列表
+                which_qubits (list): A two-element list contains the labels of the node
+            that the entanglement command applies to.
             """
             self.name = "E"
             self.which_qubits = which_qubits
 
     class CommandM:
-        r"""定义测量命令类。
+        r"""Define the ``CommandM`` class corresponding to the measurement commands.
 
-        测量命令有五个属性，分别为测量比特的标签 ``which_qubit``，原始的测量角度 ``angle``，
-        测量平面 ``plane``，域 s 对应的节点标签列表 ``domain_s``，域 t 对应的节点标签列表 ``domain_t``。
-        设原始角度为 :math:`\alpha`，则考虑域中节点依赖关系后的测量角度 :math:`\theta` 为：
+        ``CommandM`` has 5 attributes, including:
+            1.which_qubit: the qubit to be measured.
+            2.angle: the original measurement angle.
+            3.plane: the measurement plane.
+            4.domain_s: the node list corresponding to domain s.
+            5.domain_t: the node list corresponding to domain t.
 
+        The original angle :math:`\alpha` is transformed into :math:`\theta` as:
         .. math::
 
             \theta = (-1)^s \times \alpha + t \times \pi
+        after considering the node dependence in the domain.
 
         Note:
-            域 s 和域 t 是 MBQC 模型中的概念，分别记录了 Pauli X 算符和 Pauli Z 算符对测量角度产生的影响，
-            二者共同记录了该测量节点对其他节点的测量结果的依赖关系。
+            Domain s(domain t) is the concept in MBQC containing the influence on the measurement angles induced
+            by Pauli X(Pauli Z) operator. Both of them record the dependence of the measurement node on the
+            measurement results of other nodes.
 
         Warning:
-            该命令当前只支持 XY 和 YZ 平面的测量。
+            Only measurements in "XY" and "YZ" planes are allowed in this version.
 
         Attributes:
-            which_qubit (any): 作用测量命令的节点标签
-            angle (Tensor): 原始的测量角度
-            plane (str): 测量平面
-            domain_s (list): 域 s 对应的节点标签列表
-            domain_t (list): 域 t 对应的节点标签列表
+            which_qubit (any): the qubit to be measured.
+            angle (Tensor): the original measurement angle.
+            plane (str): the measurement plane.
+            domain_s (list): the node list corresponding to domain s.
+            domain_t (list): the node list corresponding to domain t.
         """
 
         def __init__(self, which_qubit, angle, plane, domain_s, domain_t):
-            r"""构造函数，用于实例化一个 ``CommandM`` 对象。
+            r"""The constructor of the ``CommandM`` class used for instantiated an object.
 
             Args:
-                which_qubit (any): 作用测量命令的节点标签
-                angle (Tensor): 原始的测量角度
-                plane (str): 测量平面
-                domain_s (list): 域 s 对应的节点标签列表
-                domain_t (list): 域 t 对应的节点标签列表
+                which_qubit (any): the qubit to be measured.
+                angle (Tensor): the original measurement angle.
+                plane (str): the measurement plane.
+                domain_s (list): the node list corresponding to domain s.
+                domain_t (list): the node list corresponding to domain t.
             """
             self.name = "M"
             self.which_qubit = which_qubit
             self.angle = angle
             self.plane = plane
             self.domain_s = domain_s
             self.domain_t = domain_t
 
     class CommandX:
-        r"""定义 Pauli X 副产品修正命令类。
+        r"""Define the ``CommandX`` class used for correcting the byproduct induced by Pauli X.
 
         Attributes:
-            which_qubit (any): 作用修正算符的节点标签
-            domain (list): 依赖关系列表
+            which_qubit (any): the label of the qubit that the correcting operator applies to.
+            domain (list): the list contains the dependence relation.
         """
 
         def __init__(self, which_qubit, domain):
-            r"""构造函数，用于实例化一个 ``CommandX`` 对象。
+            r"""The constructor of the ``CommandX`` class used for instantiated an object.
 
             Args:
-                which_qubit (any): 作用修正算符的节点标签
-                domain (list): 依赖关系列表
+                which_qubit (any): the label of the qubit that the correcting operator applies to.
+                domain (list): the list contains the dependence relation.
             """
             self.name = "X"
             self.which_qubit = which_qubit
             self.domain = domain
 
     class CommandZ:
-        r"""定义 Pauli Z 副产品修正命令。
+        r"""Define the ``CommandZ`` class used for correcting the byproduct induced by Pauli Z.
 
         Attributes:
-            which_qubit (any): 作用修正命令的节点标签
-            domain (list): 依赖关系列表
+            which_qubit (any): the label of the qubit that the correcting operator applies to.
+            domain (list): the list contains the dependence relation.
         """
 
         def __init__(self, which_qubit, domain):
-            r"""构造函数，用于实例化一个 ``CommandZ`` 对象。
+            r"""The constructor of the ``CommandZ`` class used for instantiated an object.
 
             Args:
-                which_qubit (any): 作用修正命令的节点标签
-                domain (list): 依赖关系列表
+                which_qubit (any): the label of the qubit that the correcting operator applies to.
+                domain (list): the list contains the dependence relation.
             """
             self.name = "Z"
             self.which_qubit = which_qubit
             self.domain = domain
 
     class CommandS:
-        r"""定义 "信号转移" 命令类。
+        r"""Define the ``CommandS`` class used for signal shifting.
 
         Note:
-            "信号转移" 是一类特殊的操作，用于消除测量命令对域 t 中节点的依赖关系，在某些情况下对测量模式进行简化。
+            Signal shifting is a class of special operations used for eliminating the measurement operations' dependence
+            on the nodes in domain t and simplify the measurement patterns on some conditions.
 
         Attributes:
-            which_qubit (any): 消除依赖关系的测量命令作用的节点标签
-            domain (list): 依赖关系列表
+            which_qubit (any): the labels of the nodes applied by the signal shifting operations.
+            domain (list): the list contains the dependence relation.
         """
 
         def __init__(self, which_qubit, domain):
-            r"""构造函数，用于实例化一个 ``CommandS`` 对象。
+            r"""The constructor of the ``CommandS`` class used for instantiated an object.
 
             Args:
-                which_qubit (any): 消除依赖关系的测量命令作用的节点标签
-                domain (list): 依赖关系列表
+                which_qubit (any): the labels of the nodes applied by the signal shifting operations.
+                domain (list): the list contains the dependence relation.
             """
             self.name = "S"
             self.which_qubit = which_qubit
             self.domain = domain
 
     def print_command_list(self):
-        r"""打印该 ``Pattern`` 类中的命令的信息，便于用户查看。
+        r"""Print the information of commands in the ``Pattern`` class.
 
-        代码示例:
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.qobject import Circuit
             from paddle_quantum.mbqc.mcalculus import MCalculus
 
             n = 1
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/simulator.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/simulator.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-此模块包含构造 MBQC 模型的常用类和配套的运算模拟工具。
+r"""
+This module contains the commonly used class and simulation tools in MBQC.
 """
 
 from numpy import random, pi
 from networkx import Graph, spring_layout, draw_networkx
 import matplotlib.pyplot as plt
 from paddle import t, to_tensor, matmul, conj, real, reshape, multiply
 from paddle_quantum.mbqc.utils import plus_state, cz_gate, pauli_gate
@@ -29,22 +29,19 @@
 __all__ = [
     "MBQC",
     "simulate_by_mbqc"
 ]
 
 
 class MBQC:
-    r"""定义基于测量的量子计算模型 ``MBQC`` 类。
+    r""" Define a ``MBQC`` class used for measurement based quantum computation.
 
-    用户可以通过实例化该类来定义自己的 MBQC 模型。
+    The users can define their MBQC models by instantiate the objects of this class.
     """
-
     def __init__(self):
-        r"""MBQC 类的构造函数，用于实例化一个 ``MBQC`` 对象。
-        """
         self.__graph = None  # Graph in a MBQC model
         self.__pattern = None  # Measurement pattern in a MBQC model
 
         self.__bg_state = State()  # Background state of computation
         self.__history = [self.__bg_state]  # History of background states
         self.__status = self.__history[-1] if self.__history != [] else None  # latest history item
 
@@ -54,79 +51,75 @@
 
         self.__draw = False  # Switch to draw the dynamical running process
         self.__track = False  # Switch to track the running progress
         self.__pause_time = None  # Pause time for drawing
         self.__pos = None  # Position for drawing
 
     class Vertex:
-        r"""定义维护点列表，用于实例化一个 ``Vertex`` 对象。
+        r"""Define the list of maintenance point used for instantiate a ``Vertex`` object.
 
-        将 MBQC 算法中图的节点分为三类，并进行动态维护。
+        Device the nodes in MBQC to three classes and maintain them dynamically.
 
         Note:
-            这是内部类，用户不需要直接调用到该类。
+            This is an internal class and the users don't need to use it directly.
 
-        Attributes:
-            total (list): MBQC 算法中图上的全部节点，不随运算而改变
-            pending (list): 待激活的节点，随着运算的执行而逐渐减少
-            active (list): 激活的节点，与当前测量步骤直接相关的节点
-            measured (list): 已被测量过的节点，随着运算的执行而逐渐增加
+        Args:
+            total (list): a list contains all the nodes in MBQC diagram, irrespective of the computation process.
+            pending (list): a list contains the nodes to be activated. The number of nodes decreases as the operations
+            are performed.
+            active (list): a list contains the active nodes directly related to the current measurement operations.
+            measured (list): a list contains the nodes which have been measured. The number of nodes decreases as the
+            operations are performed.
+            
+        :meta private:
         """
-
         def __init__(self, total=None, pending=None, active=None, measured=None):
-            r"""``Vertex`` 类的构造函数，用于实例化一个 ``Vertex`` 对象。
-
-            Args:
-                total (list): MBQC 算法中图上的全部节点，不随运算而改变
-                pending (list): 待激活的节点，随着运算的执行而逐渐减少
-                active (list): 激活的节点，与当前测量步骤直接相关的节点
-                measured (list): 已被测量过的节点，随着运算的执行而逐渐增加
-            """
             self.total = [] if total is None else total
             self.pending = [] if pending is None else pending
             self.active = [] if active is None else active
             self.measured = [] if measured is None else measured
 
     def set_graph(self, graph):
-        r"""设置 MBQC 模型中的图。
+        r"""Set the graphs in MBQC model.
 
-        该函数用于将用户自己构造的图传递给 ``MBQC`` 实例。
+        The users can use this function to transport their own graphs to the ``MBQC`` object.
         
         Args:
-            graph (list): MBQC 模型中的图，由列表 ``[V, E]`` 给出， 其中 ``V`` 为节点列表，``E`` 为边列表
+            graph: The graphs in MBQC model. The list takes the form ``[V, E]``, where ``V`` are nodes, and ``E`` are edges.
         """
         vertices, edges = graph
 
         vertices_of_edges = set([vertex for edge in edges for vertex in list(edge)])
         assert vertices_of_edges.issubset(vertices), "edge must be between the graph vertices."
 
         self.__graph = Graph()
         self.__graph.add_nodes_from(vertices)
         self.__graph.add_edges_from(edges)
 
         self.vertex = self.Vertex(total=vertices, pending=vertices, active=[], measured=[])
 
     def get_graph(self):
-        r"""获取图的信息。
+        r"""Get the information of graphs.
 
         Returns:
-            nx.Graph: 图
+            nx.Graph: graph
         """
         return self.__graph
 
     def set_pattern(self, pattern):
-        r"""设置 MBQC 模型的测量模式。
+        r"""Set the measurement patterns of the MBQC model.
 
-        该函数用于将用户由电路图翻译得到或自己构造的测量模式传递给 ``MBQC`` 实例。
+        This function is used for transport the measurement patterns to ``MBQC`` object. The measurement patterns
+        are acquired by either translation from the quantum circuit or the construction of users.
 
         Warning:
-            输入的 pattern 参数是 ``Pattern`` 类型，其中命令列表为标准 ``EMC`` 命令。
+            The input pattern parameter is of type ``Pattern``, in which the command list contains ``EMC`` commands.
 
         Args:
-            pattern (Pattern): MBQC 算法对应的测量模式
+            pattern (Pattern): The measurement patterns corresponding to the MBQC algorithms.
         """
         assert isinstance(pattern, Pattern), "please input a pattern of type 'Pattern'."
 
         self.__pattern = pattern
         cmds = self.__pattern.commands[:]
 
         # Check if the pattern is a standard EMC form
@@ -139,30 +132,32 @@
         # Set graph by entanglement commands
         edges = [tuple(cmd.which_qubits) for cmd in cmds if cmd.name == "E"]
         vertices = list(set([vertex for edge in edges for vertex in list(edge)]))
         graph = [vertices, edges]
         self.set_graph(graph)
 
     def get_pattern(self):
-        r"""获取测量模式的信息。
+        r"""Get the information of the measurement patterns.
 
         Returns:
-            Pattern: 测量模式
+            Pattern: measurement pattern
         """
         return self.__pattern
 
     def set_input_state(self, state=None):
-        r"""设置需要替换的输入量子态。
+        r"""Set the input state to be replaced.
 
         Warning:
-            与电路模型不同，MBQC 模型通常默认初始态为加态。如果用户不调用此方法设置初始量子态，则默认为加态。
-            如果用户以测量模式运行 MBQC，则此处输入量子态的系统标签会被限制为从零开始的自然数，类型为整型。
+            Unlike the circuit model, the initial state of MBQC model is |+> state. If the users don't use
+            this method to initialize the quantum state, the initial state will be |+> state.
+            If the users run the MBQC model in measurement mode, the system labels of the input state here
+            will be restricted to natural number(start from 0) of ``int`` type.
 
         Args:
-            state (State): 需要替换的量子态，默认为加态
+            state: the input state to be replaced, the default is |+> state.
         """
         assert self.__graph is not None, "please set 'graph' or 'pattern' before calling 'set_input_state'."
         assert isinstance(state, State) or state is None, "please input a state of type 'State'."
         vertices = list(self.__graph.nodes)
 
         if state is None:
             vector = plus_state()
@@ -185,41 +180,44 @@
         self.vertex = self.Vertex(total=vertices,
                                   pending=list(set(vertices).difference(system)),
                                   active=system,
                                   measured=[])
         self.max_active = len(self.vertex.active)
 
     def __set_position(self, pos):
-        r"""设置动态过程图绘制时节点的位置坐标。
+        r"""Set the coordinates of the nodes during the dynamical plotting process.
 
         Note:
-            这是内部方法，用户并不需要直接调用到该方法。
+            This is an internal method and the users don't need to use it directly.
 
         Args:
-            pos (dict or bool, optional): 节点坐标的字典数据或者内置的坐标选择，
-                                          内置的坐标选择有：``True`` 为测量模式自带的坐标，``False`` 为 ``spring_layout`` 坐标
+            pos (dict or bool, optional): the dict of the nodes' labels or built-in choice of coordinates.
+            The built-in choice of coordinates are: ``True`` is the coordinates of the measurement patterns,
+            ``False`` is the ``spring_layout`` coordinates.
         """
         assert isinstance(pos, bool) or isinstance(pos, dict), "'pos' should be either bool or dict."
         if isinstance(pos, dict):
             self.__pos = pos
         elif pos:
             assert self.__pattern is not None, "'pos=True' must be chosen after a pattern is set."
             self.__pos = {v: [div_str_to_float(v[1]), - div_str_to_float(v[0])] for v in list(self.__graph.nodes)}
         else:
             self.__pos = spring_layout(self.__graph)  # Use 'spring_layout' otherwise
 
     def __draw_process(self, which_process, which_qubit):
-        r"""根据当前节点状态绘图，用以实时展示 MBQC 模型的模拟计算过程。
+        r""" Draw pictures according to the status of the nodes. This method is used for showing the
+            computation process of the MBQC model.
 
         Note:
-            这是内部方法，用户并不需要直接调用到该方法。
+            This is an internal method and the users don't need to use directly.
 
         Args:
-            which_process (str): MBQC 执行的阶段，"measuring", "active" 或者 "measured"
-            which_qubit (any): 当前关注的节点，可以是 ``str``, ``tuple`` 等任意数据类型，但需要和图的标签类型匹配
+            which_process (str): The status of MBQC model, "measuring", "active" or "measured"
+            which_qubit (any): the current focal node. Any type(e.g. ``str``, ``tuple``) can be input, but should
+            match the type of the labels of the graph.
         """
         if self.__draw:
             assert which_process in ["measuring", "active", "measured"]
             assert which_qubit in self.vertex.total, "'which_qubit' must be in the graph."
 
             vertex_sets = []
             # Find where the 'which_qubit' is
@@ -265,21 +263,22 @@
                     ax = plt.gca()
                     ax.margins(0.20)
                     plt.axis("on")
                     ax.set_axisbelow(True)
             plt.pause(self.__pause_time)
 
     def draw_process(self, draw=True, pos=False, pause_time=0.5):
-        r"""动态过程图绘制，用以实时展示 MBQC 模型的模拟计算过程。
+        r"""Dynamically plot the computation process of the MBQC model.
 
         Args:
-            draw (bool, optional): 是否绘制动态过程图的布尔开关
-            pos (bool or dict, optional): 节点坐标的字典数据或者内置的坐标选择，内置的坐标选择有：
-                                            ``True`` 为测量模式自带的坐标，``False`` 为 `spring_layout` 坐标
-            pause_time (float, optional): 绘制动态过程图时每次更新的停顿时间
+            draw (bool, optional): The boolean switch of whether plot the computation process.
+            pos (bool or dict, optional): the dict of the nodes' labels or built-in choice of coordinates. 
+                The built-in choice of coordinates are: ``True`` is the coordinates of the measurement patterns, 
+                ``False`` is the ``spring_layout`` coordinates.
+            pause_time (float, optional): The time step for updating the picture.
         """
         assert self.__graph is not None, "please set 'graph' or 'pattern' before calling 'draw_process'."
         assert isinstance(draw, bool), "'draw' must be bool."
         assert isinstance(pos, bool) or isinstance(pos, dict), "'pos' should be either bool or dict."
         assert pause_time > 0, "'pause_time' must be strictly larger than 0."
 
         self.__draw = draw
@@ -287,33 +286,34 @@
 
         if self.__draw:
             plt.figure()
             plt.ion()
             self.__set_position(pos)
 
     def track_progress(self, track=True):
-        r""" 显示 MBQC 模型运行进度的开关。
+        r""" A switch for whether showing the progress bar of MBQC computation process.
 
         Args:
-            track (bool, optional): ``True`` 打开进度条显示功能， ``False`` 关闭进度条显示功能
+            track (bool, optional): ``True`` open the progress bar,  ``False`` close the progress bar.
         """
         assert isinstance(track, bool), "the parameter 'track' must be bool."
         self.__track = track
 
     def __apply_cz(self, which_qubits_list):
-        r"""对给定的两个比特作用控制 Z 门。
+        r"""Apply a controlled-Z gate to given two qubits.
 
         Note:
-            这是内部方法，用户并不需要直接调用到该方法。
+            This is an internal method and the users don't use it directly.
 
         Warning:
-            作用控制 Z 门的两个比特一定是被激活的。
+            The two qubits that the CZ gate applies to must be active.
 
         Args:
-            which_qubits_list (list): 作用控制 Z 门的比特对标签列表，例如 ``[(1, 2), (3, 4),...]``
+            which_qubits_list (list): A list contains the qubits that the CZ gate applies to.
+            e.g.``[(1, 2), (3, 4),...]``
         """
         for which_qubits in which_qubits_list:
             assert set(which_qubits).issubset(self.vertex.active), \
                 "vertices in 'which_qubits_list' must be activated first."
             assert which_qubits[0] != which_qubits[1], \
                 'the control and target qubits must not be the same.'
 
@@ -329,43 +329,45 @@
             new_state.vector = reshape(matmul(cz, reshape(new_state.vector, [4, qua_length])), [new_state_len, 1])
 
             # Update the order of active vertices and the background state
             self.vertex.active = new_state.system
             self.__bg_state = State(new_state.vector, new_state.system)
 
     def __apply_pauli_gate(self, gate, which_qubit):
-        r"""对给定的单比特作用 Pauli 门。
+        r"""Apply a Pauli gate to the given single qubit.
 
         Note:
-            这是内部方法，用户并不需要直接调用到该方法。
+            This is an internal method and the users don't use it directly.
 
         Args:
-            gate (str): Pauli 门的索引字符，"I", "X", "Y", "Z" 分别表示对应的门，在副产品处理时用 "X" 和 "Z" 门
-            which_qubit (any): 作用 Pauli 门的系统标签，
-                               可以是 ``str``, ``tuple`` 等任意数据类型，但需要和 MBQC 模型中节点的标签类型匹配
+            gate (str): Pauli gate, "I", "X", "Y", "Z". Use "X" and "Z" gate when correcting the byproduct.
+            which_qubit (any): The label of the system that the Pauli gate applies to. Any type
+            (e.g. ``str``, ``tuple`` ) can be used, as long as the type matches the type of labels of the
+            nodes in MBQC model.
         """
         new_state = permute_to_front(self.__bg_state, which_qubit)
         new_state_len = new_state.length
         half_length = int(new_state_len / 2)
         gate_mat = pauli_gate(gate)
         # Reshape the state, apply X and reshape it back
         new_state.vector = reshape(matmul(gate_mat, reshape(new_state.vector, [2, half_length])), [new_state_len, 1])
         # Update the order of active vertices and the background state
         self.vertex.active = new_state.system
         self.__bg_state = State(new_state.vector, new_state.system)
 
     def __create_graph_state(self, which_qubit):
-        r"""以待测量的比特为输入参数，生成测量当前节点所需要的最小的量子图态。
+        r""" Generate the minimal graph state for measuring the current node.
 
         Note:
-            这是内部方法，用户并不需要直接调用到该方法。
+            This is an internal method and the users don't use it directly.
 
         Args:
-            which_qubit (any): 待测量比特的系统标签。
-                                可以是 ``str``, ``tuple`` 等任意数据类型，但需要和 MBQC 模型中节点的标签类型匹配
+            which_qubit (any): The system labels of the qubit to be measured. Any type
+            (e.g. ``str``, ``tuple`` ) can be used, as long as the type matches the type of labels of the
+            nodes in MBQC model.
         """
         # Find the neighbors of 'which_qubit'
         which_qubit_neighbors = set(self.__graph.neighbors(which_qubit))
         # Exclude the qubits already measured
         neighbors_not_measured = which_qubit_neighbors.difference(set(self.vertex.measured))
         # Create a list of system labels that will be applied to cz gates
         cz_list = [(which_qubit, qubit) for qubit in neighbors_not_measured]
@@ -380,36 +382,40 @@
 
         # Update the background state and apply cz
         self.__bg_state = State(new_bg_state_vector, self.vertex.active)
         self.__apply_cz(cz_list)
         self.__draw_process("active", which_qubit)
 
     def __update(self):
-        r"""更新历史列表和量子态信息。
+        r"""Update the history and the quantum states' information.
         """
         self.__history.append(self.__bg_state)
         self.__status = self.__history[-1]
 
     def measure(self, which_qubit, basis_list):
-        r"""以待测量的比特和测量基为输入参数，对该比特进行测量。
+        r"""Measure given qubits with given measurement basis.
 
         Note:
-            这是用户在实例化 MBQC 类之后最常调用的方法之一，此处我们对单比特测量模拟进行了最大程度的优化，
-            随着用户对该函数的调用，MBQC 类将自动完成激活相关节点、生成所需的图态以及对特定比特进行测量的全过程，
-            并记录测量结果和对应测量后的量子态。用户每调用一次该函数，就完成一次对单比特的测量操作。
+            This is one of the most common methods we use after instantiating an MBQC object.
+            Here we optimize the single bit measurement simulation to the maximum extent.
+            Once use this method, the MBQC class will automatically activate the related nodes, generate
+            the corresponding graph state, measure specific qubits and store the results of the numerical
+            simulations.
 
         Warning:
-            当且仅当用户调用 ``measure`` 类方法时，MBQC 模型才真正进行运算。
+            If and only if the users use this method, the MBQC model carries out the computation.
 
         Args:
-            which_qubit (any): 待测量量子比特的系统标签，
-                                可以是 ``str``, ``tuple`` 等任意数据类型，但需要和 MBQC 模型的图上标签匹配
-            basis_list (list): 测量基向量构成的列表，列表元素为 ``Tensor`` 类型的列向量
+            which_qubit (any): The system labels of the qubit to be measured. Any type
+                (e.g. ``str``, ``tuple`` ) can be used, as long as the type matches the type of labels 
+                of the nodes in MBQC model.
+            basis_list (list): a list composed of measurement basis, the elements are column vectors
+                of type ``Tensor``.
 
-        代码示例：
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.simulator import MBQC
             from paddle_quantum.mbqc.qobject import State
             from paddle_quantum.mbqc.utils import zero_state, basis
 
@@ -470,27 +476,30 @@
         # Update the background state and history list
         self.__bg_state = State(post_state_vector, self.vertex.active)
         self.__update()
 
         self.__draw_process("measured", which_qubit)
 
     def sum_outcomes(self, which_qubits, start=0):
-        r"""根据输入的量子系统标签，在存储测量结果的字典中找到对应的测量结果，并进行求和。
+        r"""Based on the input system labels, find the corresponding measurement results in the dict and sum over.
 
-        Note:
-            在进行副产品纠正操作和定义适应性测量角度时，用户可以调用该方法对特定比特的测量结果求和。
 
+        Note:
+            When correcting the byproduct or defining the angle of adaptive measurement, one
+            can use this method to sum over the measurement results of given qubits.
+        
         Args:
-            which_qubits (list): 需要查找测量结果并求和的比特的系统标签列表
-            start (int): 对结果进行求和后需要额外相加的整数
+            which_qubits (list):the list contains the system labels of the nodes whose measurement
+                results should be find out and summed over.
+            start (int): an extra integer added to the results.
 
         Returns:
-            int: 指定比特的测量结果的和
+            int: The sum of the measurement results of given qubit.
 
-        代码示例：
+        Code example:
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.simulator import MBQC
             from paddle_quantum.mbqc.qobject import State
             from paddle_quantum.mbqc.utils import zero_state, basis
 
@@ -513,27 +522,28 @@
             Sum of outcomes of qubits '1', '2' and '3' with an extra 1:  2
         """
         assert isinstance(start, int), "'start' must be of type int."
 
         return sum([self.__outcome[label] for label in which_qubits], start)
 
     def correct_byproduct(self, gate, which_qubit, power):
-        r"""对测量后的量子态进行副产品纠正。
+        r"""Correct the byproduct of the measured quantum state.
 
         Note:
-            这是用户在实例化 MBQC 类并完成测量后，经常需要调用的一个方法。
+            This is a commonly used method after the measurement process of the MBQC model.
 
         Args:
-            gate (str): ``'X'`` 或者 ``'Z'``，分别表示 Pauli X 或 Z 门修正
-            which_qubit (any): 待操作的量子比特的系统标签，可以是 ``str``, ``tuple`` 等任意数据类型，但需要和 MBQC 中图的标签类型匹配
-            power (int): 副产品纠正算符的指数
-
-        代码示例：
+            gate (str): ``'X'`` or ``'Z'``, representing Pauli X or Pauli Z correction respectively.
+                which_qubit (any): The system labels of the qubit to be processed. Any type
+                (e.g. ``str``, ``tuple`` ) can be used, as long as the type matches the type of labels of the
+                nodes in MBQC model.
+            power (int): the index of the byproduct correcting.
 
-            此处展示的是 MBQC 模型下实现隐形传态的一个例子。
+        Code example:
+            Here is an example of quantum teleportation in MBQC framework.
 
         .. code-block:: python
 
             from paddle_quantum.mbqc.simulator import MBQC
             from paddle_quantum.mbqc.qobject import State
             from paddle_quantum.mbqc.utils import random_state_vector, basis, compare_by_vector
 
@@ -561,49 +571,52 @@
         assert isinstance(power, int), "'power' must be of type 'int'."
 
         if power % 2 == 1:
             self.__apply_pauli_gate(gate, which_qubit)
         self.__update()
 
     def __run_cmd(self, cmd):
-        r"""执行测量或副产品处理命令。
+        r"""Carry out the command of measurement or byproduct correction.
 
         Args:
-            cmd (Pattern.CommandM / Pattern.CommandX / Pattern.CommandZ): 测量或副产品处理命令
+            cmd (Pattern.CommandM / Pattern.CommandX / Pattern.CommandZ): the command of measurement
+            or byproduct correction.
         """
         assert cmd.name in ["M", "X", "Z"], "the input 'cmd' must be CommandM, CommandX or CommandZ."
         if cmd.name == "M":  # Execute measurement commands
             signal_s = self.sum_outcomes(cmd.domain_s)
             signal_t = self.sum_outcomes(cmd.domain_t)
             # The adaptive angle is (-1)^{signal_s} * angle + {signal_t} * pi
             adaptive_angle = multiply(to_tensor([(-1) ** signal_s], dtype="float64"), cmd.angle) \
                              + to_tensor([signal_t * pi], dtype="float64")
             self.measure(cmd.which_qubit, basis(cmd.plane, adaptive_angle))
         else:  # Execute byproduct correction commands
             power = self.sum_outcomes(cmd.domain)
             self.correct_byproduct(cmd.name, cmd.which_qubit, power)
 
     def __run_cmd_lst(self, cmd_lst, bar_start, bar_end):
-        r"""对列表执行测量或副产品处理命令。
+        r"""Carry out a list of commands, including measurement and byproduct correction.
 
         Args:
-            cmd_lst (list): 命令列表，包含测量或副产品处理命令
-            bar_start (int): 进度条的开始点
-            bar_end (int): 进度条的结束点
+            cmd_lst (list): the list of commands, including measurement and byproduct correction.
+            bar_start (int): the starting point of the progress bar.
+            bar_end (int): the end point of the progress bar.
         """
         for i in range(len(cmd_lst)):
             cmd = cmd_lst[i]
             self.__run_cmd(cmd)
             print_progress((bar_start + i + 1) / bar_end, "Pattern Running Progress", self.__track)
 
     def __kron_unmeasured_qubits(self):
-        r"""该方法将没有被作用 CZ 纠缠的节点初始化为 |+> 态，并与当前的量子态做张量积。
+        r"""This method initialize the nodes without being applied by CZ gate to |+> state, and take the tensor
+        product between these nodes and the current quantum state.
 
         Warning:
-            该方法仅在用户输入测量模式时调用，当用户输入图时，如果节点没有被激活，我们默认用户没有对该节点进行任何操作。
+            This method is used when the users input the measurement patterns. When the users input a graph,
+            if the nodes are not activated, we deem the users do nothing to the node by default.
         """
         # Turn off the plot switch
         self.__draw = False
         # As the create_graph_state function would change the measured qubits list, we need to record it
         measured_qubits = self.vertex.measured[:]
 
         for qubit in list(self.__graph.nodes):
@@ -614,18 +627,18 @@
                 self.max_active = max(len(self.vertex.active), self.max_active)
                 self.__bg_state = State(self.__bg_state.vector, self.vertex.active)
 
         # Restore the measured qubits
         self.vertex.measured = measured_qubits
 
     def run_pattern(self):
-        r"""按照设置的测量模式对 MBQC 模型进行模拟。
+        r"""Run the MBQC model by the measurement patterns set before.
 
         Warning:
-            该方法必须在 ``set_pattern`` 调用后调用。
+            This method must be used after ``set_pattern``.
         """
         assert self.__pattern is not None, "please use this method after calling 'set_pattern'!"
 
         # Execute measurement commands and correction commands
         cmd_m_lst = [cmd for cmd in self.__pattern.commands if cmd.name == "M"]
         cmd_c_lst = [cmd for cmd in self.__pattern.commands if cmd.name in ["X", "Z"]]
         bar_end = len(cmd_m_lst + cmd_c_lst)
@@ -639,26 +652,28 @@
         # so we permute the systems in order
         q_output = self.__pattern.output_[1]
         self.__bg_state = permute_systems(self.__status, q_output)
         self.__update()
 
     @staticmethod
     def __map_qubit_to_row(out_lst):
-        r"""将输出比特的标签与行数对应起来，便于查找其对应关系。
+        r"""Construct a map between the labels of output qubits and the number of rows.
 
         Returns:
-            dict: 返回字典，代表行数与标签的对应关系
+            dict: return a dict representing the correspondence between labels and number of rows.
         """
         return {int(div_str_to_float(qubit[0])): qubit for qubit in out_lst}
 
     def get_classical_output(self):
-        r"""获取 MBQC 模型运行后的经典输出结果。
+        r"""Get the classical output of the MBQC model.
 
         Returns:
-            str or dict: 如果用户输入是测量模式，则返回测量输出节点得到的比特串，与原电路的测量结果相一致，没有被测量的比特位填充 "？"，如果用户输入是图，则返回所有节点的测量结果
+            str or dict: if the users input the measurement patterns, the method returns the bit strings of the
+            measurement results of the output qubits which is the same as the results of the circuit based model. The
+            qubits haven't been measured fills "?". If the input is graph, return the measurement results of all nodes.
         """
         # If the input is pattern, return the equivalent result as the circuit model
         if self.__pattern is not None:
             width = len(self.__pattern.input_)
             c_output = self.__pattern.output_[0]
             q_output = self.__pattern.output_[1]
             # Acquire the relationship between row number and corresponding output qubit label
@@ -674,48 +689,49 @@
             return string
 
         # If the input is graph, return the outcome dictionary
         else:
             return self.__outcome
 
     def get_history(self):
-        r"""获取 MBQC 计算模拟时的中间步骤信息。
+        r"""Get the information during the MBQC computation process.
 
         Returns:
-            list: 生成图态、进行测量、纠正副产品后运算结果构成的列表
+            list: the list of the results, including generate graph state, measurement and byproduct correction.
         """
         return self.__history
 
     def get_quantum_output(self):
-        r"""获取 MBQC 模型运行后的量子态输出结果。
+        r"""Get the quantum state output of the MBQC model.
 
         Returns:
-            State: MBQC 模型运行后的量子态
+            State: the quantum state output of the MBQC model.
         """
         return self.__status
 
 
 def simulate_by_mbqc(circuit, input_state=None):
-    r"""使用等价的 MBQC 模型模拟量子电路。
+    r"""Simulate the quantum circuit by equivalent MBQC model.
 
-    该函数通过将量子电路转化为等价的 MBQC 模型并运行，从而获得等价于原始量子电路的输出结果。
+    This function transform the quantum circuit to equivalent MBQC models and acquire output equivalent to the circuit
+    based model.
 
     Warning:
-        与 ``UAnsatz`` 不同，此处输入的 ``circuit`` 参数包含了测量操作。
-        另，MBQC 模型默认初始态为加态，因此，如果用户不输入参数 ``input_state`` 设置初始量子态，则默认为加态。
+        Unlike the ``UAnsatz``, the input ``circuit`` here contains the measurement operations.
+        By the way, if the users set ``input_state=None``, the initial state of the MBQC is |+> state.
 
     Args:
-        circuit (Circuit): 量子电路图
-        input_state (State, optional): 量子电路的初始量子态，默认为 :math:`|+\rangle` 态
+        circuit (Circuit): quantum circuit
+        input_state (State, optional): the initial state of quantum circuit, default to :math:`|+\rangle`.
 
     Returns:
-        tuple: 包含如下两个元素:
+        tuple: contains two elements:
 
-            - str: 经典输出
-            - State: 量子输出
+            - str: classical output
+            - State: quantum output
     """
     if input_state is not None:
         assert isinstance(input_state, State), "the 'input_state' must be of type 'State'."
 
     pattern = transpile(circuit)
     mbqc = MBQC()
     mbqc.set_pattern(pattern)
@@ -725,23 +741,24 @@
     q_output = mbqc.get_quantum_output()
 
     # Return the classical and quantum outputs
     return c_output, q_output
 
 
 def __get_sample_dict(bit_num, mea_bits, samples):
-    r"""根据比特数和测量比特索引的列表，统计采样结果。
+    r"""Make statistics of the sampling results based on the number of qubits and the list of the
+        index of the measured qubits.
 
     Args:
-        bit_num (int): 比特数
-        mea_bits (list): 测量的比特列表
-        samples (list): 采样结果
+        bit_num (int): number of qubits.
+        mea_bits (list): the list of the measured qubits.
+        samples (list): the list of the measurement results.
 
     Returns:
-        dict: 统计得到的采样结果
+        dict: the statistical results
     """
     sample_dict = {}
     for i in range(2 ** len(mea_bits)):
         str_of_order = bin(i)[2:].zfill(len(mea_bits))
         bit_str = []
         idx = 0
         for j in range(bit_num):
@@ -756,30 +773,32 @@
     # Count sampling results
     for string in list(set(samples)):
         sample_dict[string] += samples.count(string)
     return sample_dict
 
 
 def sample_by_mbqc(circuit, input_state=None, plot=False, shots=1024, print_or_not=True):
-    r"""将 MBQC 模型重复运行多次，获得经典结果的统计分布。
+    r""" Repeatedly run the MBQC model and acquire the distributions of the results.
    
     Warning:
-        与 ``UAnsatz`` 不同，此处输入的 circuit 参数包含了测量操作。
-        另，MBQC 模型默认初始态为加态，因此，如果用户不输入参数 `input_state` 设置初始量子态，则默认为加态。
+        Unlike the ``UAnsatz``, the input ``circuit`` here contains the measurement operations.
+        By the way, if the users set ``input_state=None``, the initial state of the MBQC is |+> state.
 
     Args:
-        circuit (Circuit): 量子电路图
-        input_state (State, optional): 量子电路的初始量子态，默认为加态
-        plot (bool, optional): 绘制经典采样结果的柱状图开关，默认为关闭状态
-        shots (int, optional): 采样次数，默认为 1024 次
-        print_or_not (bool, optional): 是否打印采样结果和绘制采样进度，默认为开启状态
+        circuit (Circuit): quantum circuit
+        input_state (State, optional): the initial state of quantum circuit, default to |+>
+        plot (bool, optional): the boolean switch of whether plotting the histogram of the sampling results,
+        default to ``False``.
+        shots (int, optional): the number of samples, default to 1024.
+        print_or_not (bool, optional): boolean switch of whether print the sampling results and the progress bar,
+        default to open.
 
     Returns:
-        dict: 经典结果构成的频率字典
-        list: 经典测量结果和所有采样结果（包括经典输出和量子输出）的列表
+        dict: the frequency dict composed of the classical results.
+        list: the list contains all the sampling results(both quantum and classical).
     """
     # Initialize
     if shots == 1:
         print_or_not = False
     if print_or_not:
         print("Sampling " + str(shots) + " times." + "\nWill return the sampling results.\r\n")
     width = circuit.get_width()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/mbqc/utils.py` & `paddle-quantum-2.4.0/paddle_quantum/mbqc/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-此模块包含计算所需的各种常用类和函数。
+r"""
+This module contains various common classes and functions used for computation.
 """
 
 from numpy import array, exp, pi, linalg
 from numpy import sqrt as np_sqrt
 from numpy import random as np_random
 from paddle import Tensor, to_tensor, t, cos, eye, sin
 from paddle import kron as pp_kron
@@ -54,26 +54,26 @@
            "plot_results",
            "write_running_data",
            "read_running_data"
            ]
 
 
 def plus_state():
-    r"""定义加态。
+    r"""Define plus state.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \frac{1}{\sqrt{2}}  \begin{bmatrix}  1 \\ 1 \end{bmatrix}
 
     Returns:
-        Tensor: 加态对应的 ``Tensor`` 形式
+        Tensor: The ``Tensor`` form of plus state.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import plus_state
         print("State vector of plus state: \n", plus_state().numpy())
 
     ::
@@ -82,26 +82,26 @@
          [[0.70710678]
          [0.70710678]]
     """
     return to_tensor([[1 / np_sqrt(2)], [1 / np_sqrt(2)]], dtype='float64')
 
 
 def minus_state():
-    r"""定义减态。
+    r"""Define minus state.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \frac{1}{\sqrt{2}}  \begin{bmatrix}  1 \\ -1 \end{bmatrix}
 
     Returns:
-        Tensor: 减态对应的 ``Tensor`` 形式
+        Tensor: The ``Tensor`` form of minus state.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import minus_state
         print("State vector of minus state: \n", minus_state().numpy())
 
     ::
@@ -110,26 +110,26 @@
          [[ 0.70710678]
          [-0.70710678]]
     """
     return to_tensor([[1 / np_sqrt(2)], [-1 / np_sqrt(2)]], dtype='float64')
 
 
 def zero_state():
-    r"""定义零态。
+    r"""Define zero state.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \begin{bmatrix}  1 \\ 0 \end{bmatrix}
 
     Returns:
-        Tensor: 零态对应的 ``Tensor`` 形式
+        Tensor: The ``Tensor`` form of zero state.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import zero_state
         print("State vector of zero state: \n", zero_state().numpy())
 
     ::
@@ -138,26 +138,26 @@
          [[1.]
          [0.]]
     """
     return to_tensor([[1], [0]], dtype='float64')
 
 
 def one_state():
-    r"""定义一态。
+    r"""Define one state.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \begin{bmatrix}  0 \\ 1 \end{bmatrix}
 
     Returns:
-        Tensor: 一态对应的 ``Tensor`` 形式
+        Tensor: The ``Tensor`` form of one state.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import one_state
         print("State vector of one state: \n", one_state().numpy())
 
     ::
@@ -166,26 +166,26 @@
          [[0.]
          [1.]]
     """
     return to_tensor([[0], [1]], dtype='float64')
 
 
 def h_gate():
-    r"""定义 ``Hadamard`` 门。
+    r"""Define ``Hadamard`` gate.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \frac{1}{\sqrt{2}} \begin{bmatrix}  1 & 1 \\ 1 & -1 \end{bmatrix}
 
     Returns:
-        Tensor: ``Hadamard`` 门对应矩阵的 ``Tensor`` 形式
+        Tensor: The ``Tensor`` form of ``Hadamard`` gate.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import h_gate
         print("Matrix of Hadamard gate: \n", h_gate().numpy())
 
     ::
@@ -194,26 +194,26 @@
          [[ 0.70710678  0.70710678]
          [ 0.70710678 -0.70710678]]
     """
     return to_tensor((1 / np_sqrt(2)) * array([[1, 1], [1, -1]]), dtype='float64')
 
 
 def s_gate():
-    r"""定义 ``S`` 门。
+    r"""Define ``S`` gate.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \begin{bmatrix}  1 & 0 \\ 0 & i \end{bmatrix}
 
     Returns:
         Tensor: ``S`` 门矩阵对应的 ``Tensor`` 形式
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import s_gate
         print("Matrix of S gate:\n", s_gate().numpy())
 
     ::
@@ -222,26 +222,26 @@
          [[1.+0.j 0.+0.j]
          [0.+0.j 0.+1.j]]
     """
     return to_tensor([[1, 0], [0, 1j]], dtype='complex128')
 
 
 def t_gate():
-    r"""定义 ``T`` 门。
+    r"""Define ``T`` gate.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \begin{bmatrix}  1 & 0 \\ 0 & e^{i \pi / 4} \end{bmatrix}
 
     Returns:
-        Tensor: ``T`` 门矩阵对应的 ``Tensor`` 形式
+        Tensor: The ``Tensor`` form of ``T`` gate.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import t_gate
         print("Matrix of T gate: \n", t_gate().numpy())
 
     ::
@@ -250,26 +250,26 @@
          [[1.        +0.j         0.        +0.j        ]
          [0.        +0.j         0.70710678+0.70710678j]]
     """
     return to_tensor([[1, 0], [0, exp(1j * pi / 4)]], dtype='complex128')
 
 
 def cz_gate():
-    r"""定义 ``Controlled-Z`` 门。
+    r"""Define ``Controlled-Z`` gate.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \begin{bmatrix}  1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & -1 \end{bmatrix}
 
     Returns:
-        Tensor: ``Controlled-Z`` 门矩阵对应的 ``Tensor`` 形式
+        Tensor: The ``Tensor`` form of ``Controlled-Z`` gate.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import cz_gate
         print("Matrix of CZ gate: \n", cz_gate().numpy())
 
     ::
@@ -283,26 +283,26 @@
     return to_tensor([[1, 0, 0, 0],
                       [0, 1, 0, 0],
                       [0, 0, 1, 0],
                       [0, 0, 0, -1]], dtype='float64')
 
 
 def cnot_gate():
-    r"""定义 ``Controlled-NOT (CNOT)`` 门。
+    r"""Define ``Controlled-NOT (CNOT)`` gate.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \begin{bmatrix}  1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 1 & 0 \end{bmatrix}
 
     Returns:
-        Tensor: ``Controlled-NOT (CNOT)`` 门矩阵对应的 ``Tensor`` 形式
+        Tensor: The ``Tensor`` form of ``Controlled-NOT (CNOT)`` gate.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import cnot_gate
         print("Matrix of CNOT gate: \n", cnot_gate().numpy())
 
     ::
@@ -316,26 +316,26 @@
     return to_tensor([[1, 0, 0, 0],
                       [0, 1, 0, 0],
                       [0, 0, 0, 1],
                       [0, 0, 1, 0]], dtype='float64')
 
 
 def swap_gate():
-    r"""定义 ``SWAP`` 门。
+    r"""Define ``SWAP`` gate.
 
-    其矩阵形式为：
+    The matrix form is:
 
     .. math::
 
         \begin{bmatrix}  1 & 0 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 1 \end{bmatrix}
 
     Returns:
-        Tensor: ``SWAP`` 门矩阵对应的 ``Tensor`` 形式
+        Tensor: The ``Tensor`` form of ``SWAP`` gate.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import swap_gate
         print("Matrix of Swap gate: \n", swap_gate().numpy())
 
     ::
@@ -349,47 +349,47 @@
     return to_tensor([[1, 0, 0, 0],
                       [0, 0, 1, 0],
                       [0, 1, 0, 0],
                       [0, 0, 0, 1]], dtype='float64')
 
 
 def pauli_gate(gate):
-    r"""定义 ``Pauli`` 门。
+    r"""Define ``Pauli`` gate.
 
-    单位阵 ``I`` 的矩阵形式为：
+    The matrix form of Identity gate ``I`` is:
 
     .. math::
 
         \begin{bmatrix}  1 & 0 \\ 0 & 1 \end{bmatrix}
 
-    ``Pauli X`` 门的矩阵形式为：
+    The matrix form of Pauli gate ``X`` is:
 
     .. math::
 
         \begin{bmatrix}  0 & 1 \\ 1 & 0 \end{bmatrix}
 
-    ``Pauli Y`` 门的矩阵形式为：
+    The matrix form of Pauli gate ``Y`` is:
 
     .. math::
 
         \begin{bmatrix}  0 & - i \\ i & 0 \end{bmatrix}
 
-    ``Pauli Z`` 门的矩阵形式为：
+    The matrix form of Pauli gate ``Z`` is:
 
     .. math::
 
         \begin{bmatrix}  1 & 0 \\ 0 & - 1 \end{bmatrix}
 
     Args:
-        gate (str): Pauli 门的索引字符，"I", "X", "Y", "Z" 分别表示对应的门
+        gate (str): Index of Pauli gate. “I”, “X”, “Y”, or “Z” denotes the corresponding gate.
 
     Returns:
-        Tensor: Pauli 门对应的矩阵
+        Tensor: The matrix form of the Pauli gate.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import pauli_gate
         I = pauli_gate('I')
         X = pauli_gate('X')
         Y = pauli_gate('Y')
@@ -424,32 +424,32 @@
         return to_tensor([[1, 0], [0, -1]], dtype='float64')
     else:
         print("The Pauli gate must be 'I', 'X', 'Y' or 'Z'.")
         raise KeyError("invalid Pauli gate index: %s" % gate + ".")
 
 
 def rotation_gate(axis, theta):
-    r"""定义旋转门矩阵。
+    r"""Define Rotation gate.
 
     .. math::
 
         R_{x}(\theta) = \cos(\theta / 2) I - i\sin(\theta / 2) X
 
         R_{y}(\theta) = \cos(\theta / 2) I - i\sin(\theta / 2) Y
 
         R_{z}(\theta) = \cos(\theta / 2) I - i\sin(\theta / 2) Z
 
     Args:
-        axis (str): 旋转轴，绕 ``X`` 轴旋转输入 'x'，绕 ``Y`` 轴旋转输入 'y'，绕 ``Z`` 轴旋转输入 'z'
-        theta (Tensor): 旋转的角度
+        axis (str): Rotation axis. 'x', 'y' or 'z' denotes the corresponding axis.
+        theta (Tensor): Rotation angle.
 
     Returns:
-        Tensor: 旋转门对应的矩阵
+        Tensor: The matrix form of Rotation gate.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from numpy import pi
         from paddle import to_tensor
         from paddle_quantum.mbqc.utils import rotation_gate
 
@@ -491,27 +491,27 @@
         return multiply(pauli_gate('I'), cos(half_theta)) + \
                multiply(pauli_gate('Z'), multiply(sin(half_theta), to_tensor([-1j], dtype='complex128')))
     else:
         raise KeyError("invalid rotation gate index: %s, the rotation axis must be 'x', 'y' or 'z'." % axis)
 
 
 def to_projector(vector):
-    r"""把列向量转化为密度矩阵（或测量基对应的投影算符）。
+    r"""Transform a vector into its density matrix (or measurement projector).
 
     .. math::
 
         |\psi\rangle \to |\psi\rangle\langle\psi|
 
     Args:
-        vector (Tensor): 量子态列向量（或投影测量中的测量基向量）
+        vector (Tensor): Vector of a quantum state or a measurement basis
 
     Returns:
-        Tensor: 密度矩阵（或测量基对应的投影算符）
+        Tensor: Density matrix (or measurement projector)
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import zero_state, plus_state
         from paddle_quantum.mbqc.utils import to_projector
 
         zero_proj = to_projector(zero_state())
@@ -530,36 +530,38 @@
     """
     assert isinstance(vector, Tensor) and vector.shape[0] >= 1 and vector.shape[1] == 1, \
         "'vector' must be a Tensor of shape (x, 1) with x >= 1."
     return matmul(vector, t(conj(vector)))
 
 
 def basis(label, theta=to_tensor([0], dtype='float64')):
-    r"""测量基。
+    r"""Measurement basis.
 
     Note:
-        常用的测量方式有 XY-平面测量，YZ-平面测量，X 测量，Y 测量，Z 测量。
+        Commonly used measurements are measurements in the XY and YZ planes, and Pauli X, Y, Z measurements.
 
     .. math::
         \begin{align*}
         & M^{XY}(\theta) = \{R_{z}(\theta)|+\rangle, R_{z}(\theta)|-\rangle\}\\
         & M^{YZ}(\theta) = \{R_{x}(\theta)|0\rangle, R_{x}(\theta)|1\rangle\}\\
         & X = M^{XY}(0)\\
         & Y = M^{YZ}(\pi / 2) = M^{XY}(-\pi / 2)\\
         & Z = M_{YZ}(0)
         \end{align*}
 
     Args:
-        label (str): 测量基索引字符，"XY" 表示 XY-平面测量，"YZ" 表示 YZ-平面测量，"X" 表示 X 测量，"Y" 表示 Y 测量，"Z" 表示 Z 测量
-        theta (Tensor, optional): 测量角度，这里只有 XY-平面测量和 YZ-平面测量时需要
+        label (str): the labels of the measurement basis, "XY" denotes XY plane, "YZ" denotes YZ plane, 
+            "X" denotes X measurement, "Y" denotes Y measurement, "Z" denotes Z measurement.
+        theta (Tensor, optional): measurement angle, the parameter is needed when the measurement is in
+            XY plane or YZ plane.
 
     Returns:
-        list: 测量基向量构成的列表，列表元素为 ``Tensor`` 类型
+        list: the list composed of measurement basis, the elements are of type ``Tensor``.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from numpy import pi
         from paddle import to_tensor
         from paddle_quantum.mbqc.utils import basis
         theta = to_tensor(pi / 6, dtype='float64')
@@ -630,27 +632,28 @@
         return [matmul(rotation_gate('z', to_tensor([pi / 2], dtype='float64')), plus_state()),
                 matmul(rotation_gate('z', to_tensor([pi / 2], dtype='float64')), minus_state())]
     elif label == 'Z':  # Define the Z-measurement basis
         return [zero_state(), one_state()]
 
 
 def kron(tensor_list):
-    r"""把列表中的所有元素做张量积。
+    r"""Take the tensor product of all the elements in the list.
 
     .. math::
 
         [A, B, C, \cdots] \to A \otimes B \otimes C \otimes \cdots
 
     Args:
-        tensor_list (list): 需要做张量积的元素组成的列表
+        tensor_list (list): a list contains the element to taking tensor product.
 
     Returns:
-        Tensor: 所有元素做张量积运算得到的 ``Tensor``，当列表中只有一个 ``Tensor`` 时，返回该 ``Tensor`` 本身
+        Tensor: the results of the tensor product are of type ``Tensor``. If there is only
+        one ``Tensor`` in the list, return the ``Tensor``.
 
-    代码示例 1：
+    Code example 1:
 
     .. code-block:: python
 
         from paddle import to_tensor
         from paddle_quantum.mbqc.utils import pauli_gate, kron
         tensor0 = pauli_gate('I')
         tensor1 = to_tensor([[1, 1], [1, 1]], dtype='float64')
@@ -667,15 +670,15 @@
          [1. 2. 1. 2. 0. 0. 0. 0.]
          [3. 4. 3. 4. 0. 0. 0. 0.]
          [0. 0. 0. 0. 1. 2. 1. 2.]
          [0. 0. 0. 0. 3. 4. 3. 4.]
          [0. 0. 0. 0. 1. 2. 1. 2.]
          [0. 0. 0. 0. 3. 4. 3. 4.]]
 
-    代码示例 2：
+    Code example 2:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import pauli_gate, kron
         tensor0 = pauli_gate('I')
         tensor_list = [tensor0]
         tensor_all = kron(tensor_list)
@@ -694,43 +697,43 @@
         for i in range(1, len(tensor_list)):
             tensor = tensor_list[i]
             kron_all = pp_kron(kron_all, tensor)
     return kron_all
 
 
 def permute_to_front(state, which_system):
-    r"""将一个量子态中某个子系统的顺序变换到最前面。
+    r"""Move a subsystem of a system to the first.
 
-    假设当前系统的量子态列向量 :math:`\psi\rangle` 可以分解成多个子系统列向量的 tensor product 形式：
+    Assume that a quantum state :math:`\psi\rangle` can be decomposed to tensor product form: 
 
     .. math::
 
         |\psi\rangle = |\psi_1\rangle \otimes |\psi_2\rangle \otimes |\psi_3\rangle \otimes \cdots
 
 
-    每个 :math:`|\psi_i\rangle` 的系统标签为 :math:`i` ，则当前总系统的标签为：
+    the labels of each :math:`|\psi_i\rangle` is :math:`i` , so the total labels of the current system are: 
 
     .. math::
 
         \text{label} = \{1, 2, 3, \cdots \}
 
-    假设需要操作的子系统的标签为：i
+    Assume that the label of the subsystem to be moved is: i
 
-    输出新系统量子态的列向量为：
+    The output new quantum state is: 
 
     .. math::
 
         |\psi_i\rangle \otimes |\psi_1\rangle \otimes \cdots |\psi_{i-1}\rangle \otimes |\psi_{i+1}\rangle \otimes \cdots
 
     Args:
-        state (State): 需要操作的量子态
-        which_system (str): 要变换到最前面的子系统标签
+        state (State): the quantum state to be processed
+        which_system (str): the labels of the subsystem to be moved.
 
     Returns:
-        State: 系统顺序变换后的量子态
+        State: the final state after the move operation.
     """
     assert which_system in state.system, 'the system to permute must be in the state systems.'
     system_idx = state.system.index(which_system)
     if system_idx == 0:  # system in the front
         return state
     elif system_idx == state.size - 1:  # system in the end
         new_shape = [2 ** (state.size - 1), 2]
@@ -742,58 +745,58 @@
         new_system = [which_system] + state.system[: system_idx] + state.system[system_idx + 1:]
     new_vector = reshape(transpose(reshape(state.vector, new_shape), new_axis), [state.length, 1])
 
     return State(new_vector, new_system)
 
 
 def permute_systems(state, new_system):
-    r"""变换量子态的系统到指定顺序。
+    r""" Permute the quantum system to given order
 
-    假设当前系统的量子态列向量 :math:`|\psi\rangle` 可以分解成多个子系统列向量的 tensor product 形式：
+    Assume that a quantum state :math:`\psi\rangle` can be decomposed to tensor product form: 
 
     .. math::
 
         |\psi\rangle = |\psi_1\rangle \otimes |\psi_2\rangle \otimes |\psi_3\rangle \otimes \cdots
 
-    每个 :math:`\psi_i\rangle` 的系统标签为 :math:`i` ，则当前总系统的标签为：
+    the labels of each :math:`|\psi_i\rangle` is :math:`i` , so the total labels of the current system are: 
 
     .. math::
 
         \text{label} = \{1, 2, 3, \cdots \}
 
-    给定新系统的标签顺序为：
+    the order of labels of the given new system is: 
 
     .. math::
 
         \{i_1, i_2, i_3, \cdots \}
 
-    输出新系统量子态的列向量为：
+    The output new quantum state is: 
 
     .. math::
 
         |\psi_{i_1}\rangle \otimes |\psi_{i_2}\rangle \otimes |\psi_{i_3}\rangle \otimes \cdots
 
     Args:
-        state (State): 需要操作的量子态
-        new_system (list): 目标系统顺序
+        state (State): the quantum state to be processed
+        new_system (list): target order of the system
 
     Returns:
-        State: 系统顺序变换后的量子态
+        State: the quantum state after permutation.
     """
     for label in reversed(new_system):
         state = permute_to_front(state, label)
     return state
 
 
 def compare_by_density(state1, state2):
-    r"""通过密度矩阵形式比较两个量子态是否相同。
+    r"""Compare whether two quantum states are the same by their density operators.
 
     Args:
-        state1 (State): 第一个量子态
-        state2 (State): 第二个量子态
+        state1 (State): the first quantum state
+        state2 (State): the second quantum state
     """
     assert state1.size == state2.size, "two state vectors compared are not of the same length."
 
     # Permute the system order
     new_state1 = permute_systems(state1, state2.system)
     # Transform the vector to density
     density1 = to_projector(new_state1.vector)
@@ -808,19 +811,19 @@
     elif 1e-10 > error >= eps:
         print("They are probably the same states.")
     else:
         print("They are not the same states.")
 
 
 def compare_by_vector(state1, state2):
-    r"""通过列向量形式比较两个量子态是否相同。
+    r"""Compare whether two quantum states are the same by their column vector form.
 
     Args:
-        state1 (State): 第一个量子态
-        state2 (State): 第二个量子态
+        state1 (State): the first quantum state
+        state2 (State): the second quantum state
     """
     assert state1.size == state2.size, "two state vectors compared are not of the same length."
     # Check if they are normalized quantum states
     eps = 1e-12  # Error criterion
     if state1.norm >= 1 + eps or state1.norm <= 1 - eps:
         raise ValueError("the first state is not normalized.")
     elif state2.norm >= 1 + eps or state2.norm <= 1 - eps:
@@ -843,24 +846,25 @@
             elif 1e-10 > error >= eps:
                 print("They are probably the same states.")
             else:
                 print("They are not the same states.")
 
 
 def random_state_vector(n, is_real=False):
-    r"""随机生成一个量子态列向量。
+    r"""Generate a state vector randomly.
 
     Args:
-        n (int): 随机生成的量子态的比特数
-        is_real (int, optional): ``True`` 表示实数量子态，``False`` 表示复数量子态，默认为 ``False``
+        n (int): the number of qubits of the random state.
+        is_real (int, optional): ``True`` denotes a state vector with real values, ``False`` denotes a quantum
+        state with complex values, default to ``False``
 
     Returns:
-        Tensor: 随机生成量子态的列向量
+        Tensor: the column vector of the random quantum state.
 
-    代码示例：
+    Code example:
 
     .. code-block:: python
 
         from paddle_quantum.mbqc.utils import random_state_vector
         random_vec = random_state_vector(2)
         print(random_vec.numpy())
         random_vec = random_state_vector(1, is_real=True)
@@ -886,25 +890,25 @@
         inner_prod = real(matmul(t(conj(psi)), psi))
 
     psi = psi / pp_sqrt(inner_prod)  # Normalize the vector
     return psi
 
 
 def div_str_to_float(div_str):
-    r"""将除式字符串转化为对应的浮点数。
+    r"""Converts the division string to the corresponding floating point number.
 
-    例如将字符串 '3/2' 转化为 1.5。
+    For example, the string '3/2' to the float number 1.5.
 
     Args:
-        div_str (str): 除式字符串
+        div_str (str): division string
 
     Returns:
-        float: 除式对应的浮点数结果
+        float: the float number
 
-    代码示例：
+    Code example:
 
     ..  code-block:: python
 
         from paddle_quantum.mbqc.utils import div_str_to_float
         division_str = "1/2"
         division_float = div_str_to_float(division_str)
         print("The corresponding float value is: ", division_float)
@@ -914,24 +918,24 @@
         The corresponding float value is:  0.5
     """
     div_str = div_str.split("/")
     return float(div_str[0]) / float(div_str[1])
 
 
 def int_to_div_str(idx1, idx2=1):
-    r"""将两个整数转化为除式字符串。
+    r"""Transform two integers to a division string.
 
     Args:
-        idx1 (int): 第一个整数
-        idx2 (int): 第二个整数
+        idx1 (int): the first integer
+        idx2 (int): the second integer
 
     Returns:
-        str: 对应的除式字符串
+        str: the division string
 
-    代码示例：
+    Code example:
 
     ..  code-block:: python
 
         from paddle_quantum.mbqc.utils import int_to_div_str
         one = 1
         two = 2
         division_string = int_to_div_str(one, two)
@@ -942,22 +946,22 @@
         The corresponding division string is:  1/2
     """
     assert isinstance(idx1, int) and isinstance(idx2, int), "two input parameters must be int."
     return str(idx1) + "/" + str(idx2)
 
 
 def print_progress(current_progress, progress_name, track=True):
-    r"""画出当前步骤的进度条。
+    r"""Plot the progress bar.
 
     Args:
-        current_progress (float / int): 当前的进度百分比
-        progress_name (str): 当前步骤的名称
-        track (bool): 是否绘图的布尔开关
+        current_progress (float / int): the percentage of the current progress.
+        progress_name (str): the name of the current progress.
+        track (bool): the boolean switch of whether plot.
 
-    代码示例：
+    Code example:
 
     ..  code-block:: python
 
         from paddle_quantum.mbqc.utils import print_progress
         print_progress(14/100, "Current Progress")
 
     ::
@@ -974,26 +978,27 @@
             f"\033[94m {'{:6.2f}'.format(100 * current_progress)}% \033[0m ", flush=True, end=""
         )
         if current_progress == 1:
             print(" (Done)")
 
 
 def plot_results(dict_lst, bar_label, title, xlabel, ylabel, xticklabels=None):
-    r"""根据字典的键值对，以键为横坐标，对应的值为纵坐标，画出柱状图。
+    r"""Plot the histogram based on the key-value pair of the dict.
+        The key is the abscissa, and the corresponding value is the ordinate
 
     Note:
-        该函数主要调用来画出采样分布或时间比较的柱状图。
+        The function is mainly used for plotting the sampling statistics or histogram.
 
     Args:
-        dict_lst (list): 待画图的字典列表
-        bar_label (list): 每种柱状图对应的名称
-        title (str): 整个图的标题
-        xlabel (str): 横坐标的名称
-        ylabel (str): 纵坐标的名称
-        xticklabels (list, optional): 柱状图中每个横坐标的名称
+        dict_lst (list): a list contains the data to be plotted
+        bar_label (list): the name of different bars in the histogram
+        title (str): the title of the figure
+        xlabel (str): the label of the x axis.
+        ylabel (str): the label of the y axis.
+        xticklabels (list, optional): the label of each ticks of the x-axis.
     """
     assert isinstance(dict_lst, list), "please input a list with dictionaries."
     assert isinstance(bar_label, list), "please input a list with bar_labels."
     assert len(dict_lst) == len(bar_label), \
         "please check your input as the number of dictionaries and bar labels are not equal."
     bars_num = len(dict_lst)
     bar_width = 1 / (bars_num + 1)
@@ -1019,53 +1024,56 @@
     plt.xlabel(xlabel, fontproperties='SimHei')
     plt.ylabel(ylabel, fontproperties='SimHei')
     plt.ioff()
     plt.show()
 
 
 def write_running_data(textfile, eg, width, mbqc_time, reference_time):
-    r"""写入电路模拟运行的时间。
+    r"""Write the running times of the quantum circuit.
 
-    由于在许多电路模型模拟案例中，需要比较我们的 ``MBQC`` 模拟思路与 ``Qiskit`` 或量桨平台的 ``UAnsatz`` 电路模型模拟思路的运行时间。
-    因而单独定义了写入文件函数。
+    In many cases of circuit models, we need to compare the simulation time of our MBQC model with other methods
+    such as qiskit or ``UAnsatz`` circuit model in paddle_quantum. So we define this function.
 
     Hint:
-        该函数与 ``read_running_data`` 函数配套使用。
+        this function is used with the ``read_running_data`` function.
 
     Warning:
-        在调用该函数之前，需要调用 ``open`` 打开 ``textfile``；在写入结束之后，需要调用 ``close`` 关闭 ``textfile``。
+        Before using this function, we need to open a textfile. After using this function,
+        we need to close the textfile.
 
     Args:
-        textfile (TextIOWrapper): 待写入的文件
-        eg (str): 当前案例的名称
-        width (float): 电路宽度（比特数）
-        mbqc_time (float): ``MBQC`` 模拟电路运行时间
-        reference_time (float):  ``Qiskit`` 或量桨平台的 ``UAnsatz`` 电路模型运行时间
+        textfile (TextIOWrapper): the file to be written in.
+        eg (str): the name of the current case
+        width (float): the width of the circuit(number of qubits)
+        mbqc_time (float): `the simulation time of the ``MBQC`` model.
+        reference_time (float):  the simulation time of the circuit
+        based model in qiskit or ``UAnsatz`` in paddle_quantum.
     """
     textfile.write("The current example is: " + eg + "\n")
     textfile.write("The qubit number is: " + str(width) + "\n")
     textfile.write("MBQC running time is: " + str(mbqc_time) + " s\n")
     textfile.write("Circuit model running time is: " + str(reference_time) + " s\n\n")
 
 
 def read_running_data(file_name):
-    r"""读取电路模拟运行的时间。
+    r"""Read the running time of the quantum circuit.
 
-    由于在许多电路模型模拟案例中，需要比较我们的 ``MBQC`` 模拟思路与 ``Qiskit`` 或量桨平台的 ``UAnsatz`` 电路模型模拟思路的运行时间。
-    因而单独定义了读取文件函数读取运行时间，将其处理为一个列表，
-    列表中的两个元素分别为 ``Qiskit`` 或 ``UAnsatz`` 电路模型模拟思路运行时间的字典和 ``MBQC`` 模拟思路运行时间的字典。
+    In many cases of circuit models, we need to compare the simulation time of our MBQC model with other methods
+    such as qiskit or ``UAnsatz`` circuit model in paddle_quantum. So we define this function and save the running
+    time to a list. There are two dicts in the list, the first dict contains the running time of qiskit or ``UAnsatz``,
+    the second contains the simulation time of our MBQC model.
 
     Hint:
-        该函数与 ``write_running_data`` 函数配套使用。
+        This function is used with the ``write_running_data`` function.
 
     Args:
-        file_name (str): 待读取的文件名
+        file_name (str): the name of the file to be read.
 
     Returns:
-        list: 运行时间列表
+        list: The list of running time.
     """
     bit_num_lst = []
     mbqc_list = []
     reference_list = []
     remainder = {2: bit_num_lst, 3: mbqc_list, 4: reference_list}
     # Read data
     with open(file_name, 'r') as file:
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/model.py` & `paddle-quantum-2.4.0/paddle_quantum/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 # General settings for the QNN model
 rcParams = {
     # settings for the optimizer
     'optimizer': 'Adam',  # optimizer in PaddlePaddle
     'scheduler': 'StepDecay',  # scheduler in PaddlePaddle: can be set to None.
     'learning_rate': 0.2,  # (initial) learning rate of the optimizer
-    'scheduler_args': 100,  # arguments of the scheduler other than learning rate
+    'scheduler_args': {100},  # arguments (in list or tuple) of the scheduler other than learning rate
 
     # settings for the training
     'num_itr': 200,  # number of iterations during the training
     'num_print': 10,  # number of messages printed during the training
     'print_digits': 6,  # number of decimal digits for printed number
     'print_style': 'uniform',  # the style of how printed iterations are arranged: can be 'exponential'
 
@@ -156,15 +156,15 @@
     def __print_itr_generation(self, num_itr: int, num_print: int):
         r"""Determine the list of iterations to be printed during the training process
         """
         if num_itr < 1:
             return []    
         
         if rcParams['print_style'] == 'exponential':
-            # print list is generated by poisson distribution
+            # print list is generated by exponential distribution
             lamb = 4 * math.log(2) / num_itr
             poisson = lambda x: lamb * math.exp(-lamb * x)
             list_itr = list(range(1, num_itr))
             print_prob = [poisson(itr) for itr in list_itr]
             print_prob /= np.sum(print_prob)
             print_list = np.sort(np.random.choice(list_itr, size=num_print - 1, replace=False, p=print_prob)).tolist()
             print_list.append(num_itr)
@@ -172,14 +172,19 @@
             # print list is uniformly distributed
             print_ratio = num_itr / num_print
             print_list = list(filter(lambda itr: itr % print_ratio < 1, list(range(1, num_itr + 1))))
             print_list = print_list + [num_itr] if print_list[-1] != num_itr else print_list
         
         return print_list
     
+    def __scheduler_step(self, scheduler_name: str) -> List:
+        r""" Generate the argument for the scheduler.step()
+        """
+        return (lambda x: [x]) if scheduler_name == 'ReduceOnPlateau' else (lambda x: [])
+    
     def prepare(self, loss_fcn: Callable[[Union[State, Circuit, Sequential], Any], Any],
                 metric_fcn: Callable[[Union[Circuit, Sequential]], float] = None, 
                 metric_name: str = None) -> None:
         r"""General function setup for QNN
         
         Args:
             loss_fcn: loss function for the QNN
@@ -206,15 +211,16 @@
                 raise ValueError(
                     "The metric_name cannot be empty for a metric function.")
         
         self._metric_fcn, self._metric_name = metric_fcn, metric_name
         
         # setup the scheduler and optimizer
         self.__sch = NullScheduler(learning_rate=rcParams['learning_rate']) if rcParams['scheduler'] is None else \
-            getattr(paddle.optimizer.lr, rcParams['scheduler'])(rcParams['learning_rate'], rcParams['scheduler_args'])
+            getattr(paddle.optimizer.lr, rcParams['scheduler'])(rcParams['learning_rate'], *rcParams['scheduler_args'])
+        self.__step = self.__scheduler_step(rcParams['scheduler'])
         self.__opt = getattr(paddle.optimizer, rcParams["optimizer"])(learning_rate=self.__sch, parameters=self.parameters())
         
         # take the setting of rcParams
         self.__validate_settings()
         self.__print_list = self.__print_itr_generation(rcParams['num_itr'], rcParams['num_print'])
         self.__num_itr, self.__print_digits = rcParams['num_itr'], rcParams['print_digits']
         self.__num_epoch, self.__test_frequency, self.__batch_size = rcParams['num_epoch'], rcParams['test_frequency'], rcParams['batch_size']
@@ -300,15 +306,15 @@
                     metric = self._metric_fcn(self.network)
                     metric_list.append(metric)
                     if best_metric <= metric:
                         best_metric, best_metric_itr = metric, itr
                 
                 self.__opt.minimize(loss)
                 self.__opt.clear_grad()
-                self.__sch.step()
+                self.__sch.step(*self.__step(loss))
 
                 # update loss
                 loss = loss.item()
                 loss_list.append(loss)
                 if loss <= best_loss:
                     best_loss, best_loss_itr = loss, itr
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/operator/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/operator/operator.py` & `paddle-quantum-2.4.0/paddle_quantum/operator/operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,20 @@
     def __init__(self, qubits_idx: Union[Iterable[int], int, str] = 'full', num_qubits: int = None,
                  desired_result: Union[int, str] = None, if_print: bool = False,
                  measure_basis: Union[Iterable[paddle.Tensor], str] = 'z'):
         super().__init__()
         self.measure_basis = []
 
         # the qubit indices must be sorted
-        self.qubits_idx = sorted(_format_qubits_idx(qubits_idx, num_qubits))
+        self.qubits_idx = _format_qubits_idx(qubits_idx, num_qubits)
+        idx_shape = np.array(self.qubits_idx).shape
+        assert len(idx_shape) < 2, \
+            f"The input qubit indices for Collapse must be a flattened list or a integer: received {idx_shape}"
+        assert sorted(self.qubits_idx) == self.qubits_idx, \
+            f"The input qubit indices for Collapse must be sorted: received {self.qubits_idx}"
 
         self.desired_result = desired_result
         self.if_print = if_print
 
         if measure_basis in ['z', 'computational_basis']:
             self.measure_basis = 'z'
         else:
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qchem/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/qchem/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qchem/algorithm.py` & `paddle-quantum-2.4.0/paddle_quantum/qchem/algorithm.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from typing import Optional, Tuple
 import logging
 import numpy as np
 import paddle
 from paddle.optimizer import Optimizer
 from paddle_quantum.loss import ExpecVal
+from paddle_quantum import Hamiltonian
 from ..ansatz import Circuit
 from ..state import State
 from .molecule import Molecule
 
 __all__ = ["VQESolver", "GroundStateSolver"]
 
 
@@ -73,39 +74,54 @@
         tol: float = 1e-8,
         save_every: int = 1,
     ) -> None:
         super().__init__(optimizer, num_iterations, tol, save_every)
 
     def solve(
         self,
-        mol: Molecule,
         ansatz: Circuit,
+        mol: Optional[Molecule] = None,
+        ham: Optional[Hamiltonian] = None,
         init_state: Optional[State] = None,
         **optimizer_kwargs
     ) -> Tuple[float, paddle.Tensor]:
         r"""Run VQE to calculate the ground state energy for a given molecule.
 
         Args:
-            mol: the molecule object.
-            ansatz : the quantum circuit represents the wfn transformation.
-            init_state: default is None, the initial state passed to the ansatz.
-            **optimizer_kwargs: The other args.
+            ansatz (Circuit): the quantum circuit represents the wfn transformation.
+            mol (Molecule): default is None, the molecule object.
+            ham (Hamiltonian): default is None, the Hamiltonian on which to calculate the ground state energy.
+            init_state (State): default is None, the initial state passed to the ansatz.
+            optimizer_kwargs.
 
         Returns:
             The estimated ground state energy and the ground state wave function.
         """
+        if mol is None:
+            if ham is None:
+                raise ValueError("`mol` and `ham` can't be None simultaneously.")
+            elif isinstance(ham, Hamiltonian):
+                num_qubits = ham.n_qubits
+                h = ham
+            else:
+                raise ValueError("`ham` must be an instance of `paddle_quantum.Hamiltonian`.")
+        elif isinstance(mol, Molecule):
+            num_qubits = mol.num_qubits
+            h = mol.get_molecular_hamiltonian()
+        else:
+            raise ValueError("`mol` must be an instance of `paddle_quantum.qchem.Molecule`")
+
         logging.info("\n#######################################\nVQE (Ground State)\n#######################################")
-        logging.info(f"Number of qubits: {mol.num_qubits:d}")
+        logging.info(f"Number of qubits: {num_qubits:d}")
         logging.info(f"Ansatz: {ansatz.__class__.__name__:s}")
         logging.info(f"Optimizer: {self.optimizer.__name__:s}")
 
         optimizer = self.optimizer(parameters=ansatz.parameters(), **optimizer_kwargs)
         logging.info(f"\tlearning_rate: {optimizer.get_lr()}")
 
-        h = mol.get_molecular_hamiltonian()
         energy_fn = ExpecVal(h)
 
         logging.info("\nOptimization:")
         loss0 = paddle.to_tensor(np.inf)
         for n in range(self.num_iters):
             intm_state: State = ansatz(init_state)
             loss = energy_fn(intm_state)
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qchem/ansatz.py` & `paddle-quantum-2.4.0/paddle_quantum/qchem/ansatz.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qchem/drivers.py` & `paddle-quantum-2.4.0/paddle_quantum/qchem/drivers.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qchem/fermionic_state.py` & `paddle-quantum-2.4.0/paddle_quantum/qchem/fermionic_state.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qchem/molecule.py` & `paddle-quantum-2.4.0/paddle_quantum/qchem/molecule.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qchem/properties.py` & `paddle-quantum-2.4.0/paddle_quantum/qchem/properties.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qchem/utils.py` & `paddle-quantum-2.4.0/paddle_quantum/qchem/utils.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qinfo.py` & `paddle-quantum-2.4.0/paddle_quantum/qinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,31 +22,28 @@
 import re
 import numpy as np
 from scipy.linalg import logm, sqrtm
 from scipy.stats import unitary_group
 import cvxpy
 import matplotlib.image
 from itertools import product
+from typing import Optional, Tuple, List, Union
 
 import paddle
 import paddle_quantum as pq
-from .state import State, _type_fetch, _type_transform
 from .base import get_dtype
-from .linalg import abs_norm, dagger, NKron, unitary_random, is_positive
-from .channel.custom import ChoiRepr, KrausRepr, StinespringRepr
-from .channel.custom import (
-    _choi_to_kraus, _choi_to_stinespring, 
-    _kraus_to_choi, _kraus_to_stinespring, 
-    _stinespring_to_choi, _stinespring_to_kraus
-)
-from typing import Optional, Tuple, List, Union
+from .intrinsic import _type_fetch, _type_transform
+from .linalg import dagger, NKron, unitary_random, is_positive
+from .channel import Channel
+from .hamiltonian import Hamiltonian
+from .shadow import shadow_sample
 
 
-def partial_trace(state: Union[np.ndarray, paddle.Tensor, State], 
-                  dim1: int, dim2: int, A_or_B: int) -> Union[np.ndarray, paddle.Tensor, State]:
+def partial_trace(state: Union[np.ndarray, paddle.Tensor, pq.State], 
+                  dim1: int, dim2: int, A_or_B: int) -> Union[np.ndarray, paddle.Tensor, pq.State]:
     r"""Calculate the partial trace of the quantum state.
 
     Args:
         state: Input quantum state.
         dim1: The dimension of system A.
         dim2: The dimension of system B.
         A_or_B: 1 or 2. 1 means to calculate partial trace on system A; 2 means to calculate partial trace on system B.
@@ -67,16 +64,16 @@
         axis1 = -1 + A_or_B + len(higher_dims), 
         axis2 = 1 + A_or_B + len(higher_dims)
     )
     
     return _type_transform(new_state, type_str)
 
 
-def partial_trace_discontiguous(state: Union[np.ndarray, paddle.Tensor, State], 
-                                preserve_qubits: list=None) -> Union[np.ndarray, paddle.Tensor, State]:
+def partial_trace_discontiguous(state: Union[np.ndarray, paddle.Tensor, pq.State], 
+                                preserve_qubits: list=None) -> Union[np.ndarray, paddle.Tensor, pq.State]:
     r"""Calculate the partial trace of the quantum state with arbitrarily selected subsystem
 
     Args:
         state: Input quantum state.
         preserve_qubits: Remaining qubits, default is None, indicate all qubits remain.
 
     Returns:
@@ -106,16 +103,16 @@
     
     for i, at in enumerate(x for x in range(n) if x not in preserve_qubits):
         rho = new_partial_trace_singleOne(rho, at - i)
     
     return _type_transform(rho, type_str)
 
 
-def trace_distance(rho: Union[np.ndarray, paddle.Tensor, State], 
-                   sigma: Union[np.ndarray, paddle.Tensor, State]) -> Union[np.ndarray, paddle.Tensor]:
+def trace_distance(rho: Union[np.ndarray, paddle.Tensor, pq.State], 
+                   sigma: Union[np.ndarray, paddle.Tensor, pq.State]) -> Union[np.ndarray, paddle.Tensor]:
     r"""Calculate the trace distance of two quantum states.
 
     .. math::
         D(\rho, \sigma) = 1 / 2 * \text{tr}|\rho-\sigma|
 
     Args:
         rho: a quantum state.
@@ -131,16 +128,16 @@
     assert rho.shape == sigma.shape, 'The shape of two quantum states are different'
     eigval, _ = paddle.linalg.eig(rho - sigma)
     dist = 0.5 * paddle.sum(paddle.abs(eigval))
 
     return dist.item() if type_rho == "numpy" and type_sigma == "numpy" else dist
 
 
-def state_fidelity(rho: Union[np.ndarray, paddle.Tensor, State], 
-                   sigma: Union[np.ndarray, paddle.Tensor, State]) -> Union[np.ndarray, paddle.Tensor]:
+def state_fidelity(rho: Union[np.ndarray, paddle.Tensor, pq.State], 
+                   sigma: Union[np.ndarray, paddle.Tensor, pq.State]) -> Union[np.ndarray, paddle.Tensor]:
     r"""Calculate the fidelity of two quantum states.
 
     .. math::
         F(\rho, \sigma) = \text{tr}(\sqrt{\sqrt{\rho}\sigma\sqrt{\rho}})
 
     Args:
         rho: a quantum state.
@@ -150,16 +147,15 @@
         The fidelity between the input quantum states.
     """
     type_rho, type_sigma = _type_fetch(rho), _type_fetch(sigma)
     rho = _type_transform(rho, "density_matrix").numpy()
     sigma = _type_transform(sigma, "density_matrix").numpy()
     
     assert rho.shape == sigma.shape, 'The shape of two quantum states are different'
-    fidelity = np.trace(sqrtm(sqrtm(rho) @ sigma @ sqrtm(rho))).real
-
+    fidelity = np.trace(sqrtm(sqrtm(rho) @ sigma @ sqrtm(rho)).astype(rho.dtype)).real
     if type_rho == "numpy" and type_sigma == "numpy":
         return fidelity
     return paddle.to_tensor(fidelity)
 
 
 def gate_fidelity(U: Union[np.ndarray, paddle.Tensor], 
                   V: Union[np.ndarray, paddle.Tensor]) -> Union[np.ndarray, paddle.Tensor]:
@@ -185,15 +181,15 @@
     V = paddle.cast(V, dtype=U.dtype)
     assert U.shape == V.shape, 'The shape of two matrices are different'
     fidelity = paddle.abs(paddle.trace(U @ dagger(V))) / U.shape[0]
 
     return fidelity.item() if type_u == "numpy" or type_v == "numpy" else fidelity
 
 
-def purity(rho: Union[np.ndarray, paddle.Tensor, State]) -> Union[np.ndarray, paddle.Tensor]:
+def purity(rho: Union[np.ndarray, paddle.Tensor, pq.State]) -> Union[np.ndarray, paddle.Tensor]:
     r"""Calculate the purity of a quantum state.
 
     .. math::
 
         P = \text{tr}(\rho^2)
 
     Args:
@@ -205,15 +201,15 @@
     type_rho = _type_fetch(rho)
     rho = _type_transform(rho, "density_matrix").data
     gamma = paddle.trace(rho @ rho).real()
 
     return gamma.item() if type_rho == "numpy" else gamma
 
 
-def von_neumann_entropy(rho: Union[np.ndarray, paddle.Tensor, State], base: Optional[int] = 2) -> Union[np.ndarray, paddle.Tensor]:
+def von_neumann_entropy(rho: Union[np.ndarray, paddle.Tensor, pq.State], base: Optional[int] = 2) -> Union[np.ndarray, paddle.Tensor]:
     r"""Calculate the von Neumann entropy of a quantum state.
 
     .. math::
 
         S = -\text{tr}(\rho \log(\rho))
 
     Args:
@@ -227,16 +223,16 @@
     rho = _type_transform(rho, "density_matrix").data
     rho_eigenvalues = paddle.real(paddle.linalg.eigvals(rho))
     entropy = -1 * (math.log(math.e, base)) * sum([eigenvalue * paddle.log(eigenvalue) for eigenvalue in rho_eigenvalues if eigenvalue >= 1e-8])
 
     return entropy.item() if type_rho == "numpy" else entropy
 
 
-def relative_entropy(rho: Union[np.ndarray, paddle.Tensor, State], 
-                     sig: Union[np.ndarray, paddle.Tensor, State], base: Optional[int] = 2) -> Union[np.ndarray, paddle.Tensor]:
+def relative_entropy(rho: Union[np.ndarray, paddle.Tensor, pq.State], 
+                     sig: Union[np.ndarray, paddle.Tensor, pq.State], base: Optional[int] = 2) -> Union[np.ndarray, paddle.Tensor]:
     r"""Calculate the relative entropy of two quantum states.
 
     .. math::
 
         S(\rho \| \sigma)=\text{tr} \rho(\log \rho-\log \sigma)
 
     Args:
@@ -254,39 +250,72 @@
     entropy = (math.log(math.e, base)) * np.trace(rho @ logm(rho) - rho @ logm(sig)).real
     
     if type_rho == "numpy" or type_sig == "numpy":
         return entropy
     return paddle.to_tensor(entropy)
 
 
-def random_pauli_str_generator(n: int, terms: Optional[int] = 3) -> List:
+def random_pauli_str_generator(num_qubits: int, terms: Optional[int] = 3) -> List:
     r"""Generate a random observable in list form.
 
     An observable :math:`O=0.3X\otimes I\otimes I+0.5Y\otimes I\otimes Z`'s list form is
     ``[[0.3, 'x0'], [0.5, 'y0,z2']]``.  Such an observable is generated by 
     ``random_pauli_str_generator(3, terms=2)`` 
 
     Args:
-        n: Number of qubits.
+        num_qubits: Number of qubits.
         terms: Number of terms in the observable. Defaults to 3.
 
     Returns:
-        The randomly generated observable's list form.
+        The Hamiltonian of randomly generated observable.
     """
     pauli_str = []
-    for sublen in np.random.randint(1, high=n + 1, size=terms):
+    for sublen in np.random.randint(1, high=num_qubits + 1, size=terms):
         # Tips: -1 <= coeff < 1
         coeff = np.random.rand() * 2 - 1
         ops = np.random.choice(['x', 'y', 'z'], size=sublen)
-        pos = np.random.choice(range(n), size=sublen, replace=False)
+        pos = np.random.choice(range(num_qubits), size=sublen, replace=False)
         op_list = [ops[i] + str(pos[i]) for i in range(sublen)]
+        op_list.sort(key=lambda x: int(x[1:]))
         pauli_str.append([coeff, ','.join(op_list)])
     return pauli_str
 
 
+def pauli_str_convertor(observable: List) -> List:
+    r"""Concatenate the input observable with coefficient 1.
+    
+    For example, if the input ``observable`` is ``[['z0,x1'], ['z1']]``, 
+    then this function returns the observable ``[[1, 'z0,x1'], [1, 'z1']]``.
+
+    Args:
+        observable: The observable to be concatenated with coefficient 1.
+
+    Returns:
+        The observable with coefficient 1
+    """
+
+    for i in range(len(observable)):
+        assert len(observable[i]) == 1, 'Each term should only contain one string'
+
+    return [[1, term] for term in observable]
+
+
+def random_hamiltonian_generator(num_qubits: int, terms: Optional[int] = 3) -> List:
+    r"""Generate a random Hamiltonian. 
+
+    Args:
+        num_qubits: Number of qubits.
+        terms: Number of terms in the Hamiltonian. Defaults to 3.
+
+    Returns:
+        The randomly generated Hamiltonian.
+    """
+    return Hamiltonian(random_pauli_str_generator(num_qubits, terms))
+
+
 def pauli_str_to_matrix(pauli_str: list, n: int) -> paddle.Tensor:
     r"""Convert the input list form of an observable to its matrix form.
 
     For example, if the input ``pauli_str`` is ``[[0.7, 'z0,x1'], [0.2, 'z1']]`` and ``n=3``,
     then this function returns the observable :math:`0.7Z\otimes X\otimes I+0.2I\otimes Z\otimes I`
     in matrix form.
 
@@ -328,15 +357,15 @@
             for idx in range(1, len(sub_matrices)):
                 mat = np.kron(mat, sub_matrices[idx])
             matrices.append(coeff * mat)
 
     return paddle.to_tensor(sum(matrices), dtype=get_dtype())
 
 
-def partial_transpose_2(density_op: Union[np.ndarray, paddle.Tensor, State], 
+def partial_transpose_2(density_op: Union[np.ndarray, paddle.Tensor, pq.State], 
                         sub_system: int = None) -> Union[np.ndarray, paddle.Tensor]:
     r"""Calculate the partial transpose :math:`\rho^{T_A}` of the input quantum state.
 
     Args:
         density_op: Density matrix form of the quantum state.
         sub_system: 1 or 2. 1 means to perform partial transpose on system A; 
                     2 means to perform partial transpose on system B. Default is 2.
@@ -377,15 +406,15 @@
         transposed_density_op[0:2, 2:4] = density_op[2:4, 0:2]
 
     if type_str == "numpy":
         return transposed_density_op
     return paddle.to_tensor(transposed_density_op)
 
 
-def partial_transpose(density_op: Union[np.ndarray, paddle.Tensor, State], 
+def partial_transpose(density_op: Union[np.ndarray, paddle.Tensor, pq.State], 
                       n: int) -> Union[np.ndarray, paddle.Tensor]:
     r"""Calculate the partial transpose :math:`\rho^{T_A}` of the input quantum state.
 
     Args:
         density_op: Density matrix form of the quantum state.
         n: Number of qubits of subsystem A, with qubit indices as [0, 1, ..., n-1]
 
@@ -401,16 +430,16 @@
     density_op = paddle.reshape(density_op, [2 ** n, 2 ** (n_qubits - n), 2 ** n, 2 ** (n_qubits - n)])
     density_op = paddle.transpose(density_op, [2, 1, 0, 3])
     density_op = paddle.reshape(density_op, [2 ** n_qubits, 2 ** n_qubits])
 
     return density_op.numpy() if type_str == "numpy" else density_op
 
 
-def permute_systems(mat: Union[np.ndarray, paddle.Tensor, State], 
-                    perm_list: List[int], dim_list: List[int]) -> Union[np.ndarray, paddle.Tensor, State]:
+def permute_systems(mat: Union[np.ndarray, paddle.Tensor, pq.State], 
+                    perm_list: List[int], dim_list: List[int]) -> Union[np.ndarray, paddle.Tensor, pq.State]:
     r"""Permute quantum system based on a permute list
 
     Args:
         mat: A given matrix representation which is usually a quantum state.
         perm: The permute list. e.g. input ``[0,2,1,3]`` will permute the 2nd and 3rd subsystems. 
         dim: A list of dimension sizes of each subsystem. 
 
@@ -434,15 +463,15 @@
             row_perm_idx = sum(perm_idx[i] * dim_list ** np.array(range(len(perm_idx[i])-1, -1, -1)))
             col_perm_idx = sum(perm_idx[j] * dim_list ** np.array(range(len(perm_idx[i])-1, -1, -1)))
             perm_mat[row_perm_idx, col_perm_idx] = mat[i,j].item()
 
     return _type_transform(perm_mat, mat_type)
 
 
-def negativity(density_op: Union[np.ndarray, paddle.Tensor, State]) -> Union[np.ndarray, paddle.Tensor]:
+def negativity(density_op: Union[np.ndarray, paddle.Tensor, pq.State]) -> Union[np.ndarray, paddle.Tensor]:
     r"""Compute the Negativity :math:`N = ||\frac{\rho^{T_A}-1}{2}||` of the input quantum state.
 
     Args:
         density_op: Density matrix form of the quantum state.
 
     Returns:
         The Negativity of the input quantum state.
@@ -458,30 +487,30 @@
     for val in eigen_val:
         if val < 0:
             n = n + np.abs(val)
 
     return n if type_str == "numpy" else paddle.to_tensor(n)
 
 
-def logarithmic_negativity(density_op: Union[np.ndarray, paddle.Tensor, State]) -> Union[np.ndarray, paddle.Tensor]:
+def logarithmic_negativity(density_op: Union[np.ndarray, paddle.Tensor, pq.State]) -> Union[np.ndarray, paddle.Tensor]:
     r"""Calculate the Logarithmic Negativity :math:`E_N = ||\rho^{T_A}||` of the input quantum state.
 
     Args:
         density_op: Density matrix form of the quantum state.
 
     Returns:
         The Logarithmic Negativity of the input quantum state.
     """
     # Calculate the negativity
     n = negativity(density_op)
 
     return paddle.log2(2 * n + 1)
 
 
-def is_ppt(density_op: Union[np.ndarray, paddle.Tensor, State]) -> bool:
+def is_ppt(density_op: Union[np.ndarray, paddle.Tensor, pq.State]) -> bool:
     r"""Check if the input quantum state is PPT.
 
     Args:
         density_op: Density matrix form of the quantum state.
 
     Returns:
         Whether the input quantum state is PPT.
@@ -510,15 +539,15 @@
     if is_positive(op):
 
         op_partial = partial_trace(op, sys_dim, sys_dim, 2)
             
         return is_positive(paddle.eye(sys_dim) - op_partial)
     return False
 
-def schmidt_decompose(psi: Union[np.ndarray, paddle.Tensor, State], 
+def schmidt_decompose(psi: Union[np.ndarray, paddle.Tensor, pq.State], 
                       sys_A: List[int]=None) -> Union[Tuple[paddle.Tensor, paddle.Tensor, paddle.Tensor],
                                                       Tuple[np.ndarray, np.ndarray, np.ndarray]]:
     r"""Calculate the Schmidt decomposition of a quantum state :math:`\lvert\psi\rangle=\sum_ic_i\lvert i_A\rangle\otimes\lvert i_B \rangle`.
 
     Args:
         psi: State vector form of the quantum state, with shape (2**n)
         sys_A: Qubit indices to be included in subsystem A (other qubits are included in subsystem B), default are the first half qubits of :math:`\lvert \psi\rangle`
@@ -553,15 +582,15 @@
     c, u, v = c[:k], u.T[:k].reshape([k, -1, 1]), v[:k].reshape([k, -1, 1])
 
     if type_psi == "numpy":
         return c, u, v
     return paddle.to_tensor(c), paddle.to_tensor(u), paddle.to_tensor(v)
 
 
-def image_to_density_matrix(image_filepath: str) -> State:
+def image_to_density_matrix(image_filepath: str) -> pq.State:
     r"""Encode image to density matrix
 
     Args:
         image_filepath: Path to the image file.
 
     Returns:
         The density matrix obtained by encoding
@@ -573,18 +602,18 @@
 
     # Fill the matrix so that it becomes a matrix whose shape is [2**n,2**n]
     length = int(2**np.ceil(np.log2(np.max(image_matrix.shape))))
     image_matrix = np.pad(image_matrix, ((0, length-image_matrix.shape[0]), (0, length-image_matrix.shape[1])), 'constant')
     # Density matrix whose trace  is 1
     rho = image_matrix@image_matrix.T
     rho = rho/np.trace(rho)
-    return State(rho, backend=pq.Backend.DensityMatrix)
+    return _type_transform(rho, "density_matrix")
 
 
-def shadow_trace(state: 'State', hamiltonian: pq.Hamiltonian, 
+def shadow_trace(state: pq.State, hamiltonian: Hamiltonian, 
                  sample_shots: int, method: Optional[str] = 'CS') -> float:
     r"""Estimate the expectation value :math:`\text{trace}(H\rho)`  of an observable :math:`H`.
 
     Args:
         state: Quantum state.
         hamiltonian: Observable.
         sample_shots: Number of samples.
@@ -597,17 +626,17 @@
         The estimated expectation value for the hamiltonian.
     """
     if not isinstance(hamiltonian, list):
         hamiltonian = hamiltonian.pauli_str
     num_qubits = state.num_qubits
     mode = state.backend
     if method == "LBCS":
-        result, beta = pq.shadow.shadow_sample(state, num_qubits, sample_shots, mode, hamiltonian, method)
+        result, beta = shadow_sample(state, num_qubits, sample_shots, mode, hamiltonian, method)
     else:
-        result = pq.shadow.shadow_sample(state, num_qubits, sample_shots, mode, hamiltonian, method)
+        result = shadow_sample(state, num_qubits, sample_shots, mode, hamiltonian, method)
 
     def prepare_hamiltonian(hamiltonian, num_qubits):
         new_hamiltonian = []
         for idx, (coeff, pauli_str) in enumerate(hamiltonian):
             pauli_str = re.split(r',\s*', pauli_str.lower())
             pauli_term = ['i'] * num_qubits
             for item in pauli_str:
@@ -719,15 +748,15 @@
             for coeff, pauli_term in hamiltonian:
                 estimation += coeff * pauli_estimator[pauli_term]['value'][sample_idx + 1]
             trace_estimation = estimation
 
     return trace_estimation
 
 
-def tensor_state(state_a: State, state_b: State, *args: State) -> State:
+def tensor_state(state_a: pq.State, state_b: pq.State, *args: pq.State) -> pq.State:
     r"""calculate tensor product (kronecker product) between at least two state. This function automatically returns State instance
 
     Args:
         state_a: State
         state_b: State
         *args: other states
 
@@ -736,52 +765,48 @@
         
     Note:
         Need to be careful with the backend of states; 
         Use ``paddle_quantum.linalg.NKron`` if the input datatype is ``paddle.Tensor`` or ``numpy.ndarray``.
         
     """
     state_a, state_b = _type_transform(state_a, "tensor"), _type_transform(state_b, "tensor")
-    return State(NKron(state_a, state_b, [_type_transform(st, "tensor") for st in args]))
+    return pq.State(NKron(state_a, state_b, [_type_transform(st, "tensor") for st in args]))
 
 
-def diamond_norm(channel_repr: Union[ChoiRepr, KrausRepr, StinespringRepr, paddle.Tensor],
+def diamond_norm(channel_repr: Union[Channel, paddle.Tensor],
                  dim_io: Union[int, Tuple[int, int]] = None, **kwargs) -> float:
     r'''Calculate the diamond norm of input.
 
     Args:
-        channel_repr: A ``ChoiRepr`` or ``KrausRepr`` or ``StinespringRepr`` instance or a ``paddle.Tensor`` instance.
+        channel_repr: A ``Channel`` or a ``paddle.Tensor`` instance.
         dim_io: The input and output dimensions.
         **kwargs: Parameters to set cvx.
 
     Raises:
-        RuntimeError: `channel_repr` must be `ChoiRepr`or `KrausRepr` or `StinespringRepr` or `paddle.Tensor`.
+        RuntimeError: `channel_repr` must be `Channel` or `paddle.Tensor`.
         TypeError: "dim_io" should be "int" or "tuple".
 
     Warning:
         `channel_repr` is not in Choi representaiton, and is converted into `ChoiRepr`.
 
     Returns:
         Its diamond norm.
 
     Reference:
         Khatri, Sumeet, and Mark M. Wilde. "Principles of quantum communication theory: A modern approach."
         arXiv preprint arXiv:2011.04672 (2020).
         Watrous, J. . "Semidefinite Programs for Completely Bounded Norms." 
         Theory of Computing 5.1(2009):217-238.
     '''
-    if isinstance(channel_repr, ChoiRepr):
+    if isinstance(channel_repr, Channel):
         choi_matrix = channel_repr.choi_repr
 
     elif isinstance(channel_repr, paddle.Tensor):
         choi_matrix = channel_repr
 
-    elif isinstance(channel_repr, (KrausRepr, StinespringRepr)):
-        warnings.warn('`channel_repr` is not in Choi representaiton, and is converted into `ChoiRepr`')
-        choi_matrix = channel_repr.to_choi().choi_repr
-
     else:
         raise RuntimeError('`channel_repr` must be `ChoiRepr`or `KrausRepr` or `StinespringRepr` or `paddle.Tensor`.')
 
     if dim_io is None:    # Default to dim_in == dim_out
         dim_in = dim_out = int(math.sqrt(choi_matrix.shape[0]))
     elif isinstance(dim_io, tuple):
         dim_in = int(dim_io[0])
@@ -843,43 +868,46 @@
     source, target = source.capitalize(), target.capitalize()
     if target not in ['Choi', 'Kraus', 'Stinespring']:
         raise ValueError(f"Unsupported channel representation: require Choi, Kraus or Stinespring, not {target}")
     if source == target:
         return representation
     if source not in ['Choi', 'Kraus', 'Stinespring']:
         raise ValueError(f"Unsupported channel representation: require Choi, Kraus or Stinespring, not {source}")
-    is_ndarray = False
-    if isinstance(representation, np.ndarray):
-        is_ndarray = True
-        representation = paddle.to_tensor(representation)
-    elif isinstance(representation, List) and isinstance(representation[0], np.ndarray):
-        is_ndarray = True
-        representation = [paddle.to_tensor(representation[i]) for i in range(len(representation))]
+    
+    if isinstance(representation, List):
+        assert source == 'Kraus', \
+            f"Unsupported data input: expected Kraus representation, received {source}"
+        type_str = _type_fetch(representation[0])
+        representation = [_type_transform(repr, 'tensor') for repr in representation]
+    else:
+        type_str = _type_fetch(representation)
+        representation = _type_transform(repr, 'tensor')
+        
+    oper = Channel(source, representation)
     
     if source == 'Choi':
         if target == 'Kraus':
-            representation = _choi_to_kraus(representation, tol) 
-            return [representation[i].numpy() for i in range(len(representation))] if is_ndarray else representation
+            representation = oper.kraus_repr
+            return [_type_transform(repr, type_str) for repr in representation]
         
         # stinespring repr
-        representation = _choi_to_stinespring(representation, tol)
+        representation = oper.stinespring_repr
 
     elif source == 'Kraus':
-        representation = representation if isinstance(representation, List) else [representation]
-        representation = _kraus_to_choi(representation) if target == 'Choi' else _kraus_to_stinespring(representation) 
+        representation = oper.choi_repr if target == 'Choi' else oper.stinespring_repr
 
     else: # if source == 'Stinespring'
         if target == 'Kraus':
-            representation = _stinespring_to_kraus(representation)
-            return [representation[i].numpy() for i in range(len(representation))] if is_ndarray else representation
+            representation = oper.kraus_repr
+            return [_type_transform(repr, type_str) for repr in representation]
         
         # choi repr
-        representation = _stinespring_to_choi(representation)
+        representation = oper.choi_repr
 
-    return representation.numpy() if is_ndarray else representation
+    return _type_transform(representation, type_str)
 
 
 def random_channel(num_qubits: int, rank: int = None, target: str = 'Kraus') -> Union[paddle.Tensor, List[paddle.Tensor]]:
     r"""Generate a random channel from its Stinespring representation
     
     Args:
         num_qubits: number of qubits :math:`n`
@@ -894,15 +922,15 @@
     dim = 2 ** num_qubits
     rank = np.random.randint(dim) + 1 if rank is None else rank
     assert 1 <= rank <= dim, \
         f"rank must be positive and no larger than the dimension {dim} of the channel: received {rank}"
     
     # rank = 1
     unitary = unitary_group.rvs(rank * dim)
-    stinespring_mat = paddle.to_tensor(unitary[:, :dim], dtype=pq.get_dtype()).reshape([rank, dim, dim])
+    stinespring_mat = paddle.to_tensor(unitary[:, :dim], dtype=get_dtype()).reshape([rank, dim, dim])
     list_kraus = [stinespring_mat[j] for j in list(range(rank))]
     
     if target == 'Choi':
         return channel_repr_convert(list_kraus, source='Kraus', target='Choi')
     elif target == 'Stinespring':
         return channel_repr_convert(list_kraus, source='Kraus', target='Stinespring')
     return list_kraus
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qml/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/qpp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # !/usr/bin/env python3
-# Copyright (c) 2022 Institute for Quantum Computing, Baidu Inc. All Rights Reserved.
+# Copyright (c) 2021 Institute for Quantum Computing, Baidu Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
-The quantum machine learning module.
+The module of quantum phase processing.
 """
+
+from .laurent import *
+from .angles import *
+from .utils import *
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qml/qnnmic.py` & `paddle-quantum-2.4.0/paddle_quantum/qml/qnnmic.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,25 +39,28 @@
 
 
 class ImageDataset(Dataset):
     r"""
     The class used for loading classical datasets.
 
     Args:
-    file_path: The path of the input image.
-    num_samples: The number of the data in the test dataset.
-    task: The training, validation, or testing task.
-    pca: Whether use principal component analysis. Defaults to None.
-    scaler: Whether scale the data. Defaults to None.
-    centering: Whether remove the mean. Defaults to None.
+        file_path: The path of the input image.
+        num_samples: The number of the data in the test dataset.
+        task: The training, validation, or testing task.
+        pca: Whether use principal component analysis. Defaults to None.
+        scaler: Whether scale the data. Defaults to None.
+        centering: Whether remove the mean. Defaults to None.
 
     Raises:
         ValueError: If the task is not training, validation, or test, raises the error.
     """
-    def __init__(self, file_path: str, num_samples: int, task: str, pca: PCA=None, scaler: StandardScaler=None, centering: MinMaxScaler=None):
+    def __init__(
+            self, file_path: str, num_samples: int, task: str, pca: PCA = None,
+            scaler: StandardScaler = None, centering: MinMaxScaler = None
+    ):
         super().__init__()
         # load data
         data, labels = [], []
         npz_file = np.load('medical_image/' + file_path + '.npz')
 
         if task == "train":
             data_set = list(npz_file['train_images'])
@@ -131,15 +134,15 @@
 
 def _filter_circuit(num_qubits: int, depth:int) -> pq.ansatz.Circuit:
     r"""
     The function that generates a filter circuit for extracting features.
     """
     cir = Circuit(num_qubits)
 
-    cir.complex_entangled_layer(qubits_idx='full', depth=depth)
+    cir.complex_entangled_layer(depth=depth)
 
     return cir
 
 
 def _encoding_circuit(num_qubits: int, data: paddle.Tensor) -> pq.ansatz.Circuit:
     r"""
     The function that encodes the classical data into quantum states.
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qml/qnnqd.py` & `paddle-quantum-2.4.0/paddle_quantum/qml/qnnqd.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 def _filter_circuit(num_qubits: int, depth:int) -> pq.ansatz.Circuit:
     r"""
     The function that generates a filter circuit for extracting features.
     """
     cir = Circuit(num_qubits)
 
-    cir.complex_entangled_layer(qubits_idx='full', depth=depth)
+    cir.complex_entangled_layer(depth=depth)
 
     return cir
 
 
 def _encoding_circuit(num_qubits: int, data: paddle.Tensor) -> pq.ansatz.Circuit:
     r"""
     The function that encodes the classical data into quantum states.
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qml/qsann.py` & `paddle-quantum-2.4.0/paddle_quantum/qml/qsann.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,60 +115,42 @@
 
         Returns:
             The quantum state which embeds the word.
         """
         embedding_state = pq.state.zero_state(num_qubits)
         for d in range(depth):
             for idx in range(num_qubits):
+                qubits_idx = [idx, (idx + 1) % num_qubits]
                 param_idx = 2 * num_qubits * d + 2 * idx
-                embedding_state = functional.rx(
-                    state=embedding_state, qubit_idx=idx,
-                    theta=params[param_idx][0],
-                    dtype=embedding_state.dtype, backend=embedding_state.backend
-                )
-                embedding_state = functional.ry(
-                    state=embedding_state, qubit_idx=idx,
-                    theta=params[param_idx][1],
-                    dtype=embedding_state.dtype, backend=embedding_state.backend
-                )
-                embedding_state = functional.rx(
-                    state=embedding_state, qubit_idx=(idx + 1) % num_qubits,
-                    theta=params[param_idx + 1][0],
-                    dtype=embedding_state.dtype, backend=embedding_state.backend
-                )
-                embedding_state = functional.ry(
-                    state=embedding_state, qubit_idx=(idx + 1) % num_qubits,
-                    theta=params[param_idx + 1][1],
-                    dtype=embedding_state.dtype, backend=embedding_state.backend
-                )
-                embedding_state = functional.cnot(
-                    state=embedding_state, qubit_idx=[idx, (idx + 1) % num_qubits],
-                    dtype=embedding_state.dtype, backend=embedding_state.backend
-                )
+                
+                cir = pq.Circuit(embedding_state.num_qubits)
+                cir.rx(qubits_idx, param=params[param_idx:param_idx+2][0])
+                cir.ry(qubits_idx, param=params[param_idx:param_idx+2][1])
+                cir.cnot(qubits_idx)
+                embedding_state = cir(embedding_state)
+        
         for idx in range(num_qubits):
             param_idx = 2 * num_qubits * depth + idx
-            embedding_state = functional.rx(
-                state=embedding_state, qubit_idx=idx, theta=params[param_idx][0],
-                dtype=embedding_state.dtype, backend=embedding_state.backend
-            )
-            embedding_state = functional.ry(
-                state=embedding_state, qubit_idx=idx, theta=params[param_idx][1],
-                dtype=embedding_state.dtype, backend=embedding_state.backend
-            )
+            
+            cir = pq.Circuit(embedding_state.num_qubits)
+            cir.rx(idx, param=params[param_idx][0])
+            cir.ry(idx, param=params[param_idx][1])
+            embedding_state = cir(embedding_state)
+        
         return embedding_state
 
     def forward(self, batch_text: List[List[int]]) -> List[paddle.Tensor]:
         r"""
-        The forward function to excute the model.
+        The forward function to execute the model.
 
         Args:
             batch_text: The batch of input texts. Each of them is a list of int.
 
         Returns:
-            Retrun a list which contains the predictions of the input texts.
+            Return a list which contains the predictions of the input texts.
         """
         predictions = []
         for text in batch_text:
             text_feature = [self.embedding_param[word] for word in text]
             for layer_idx in range(self.num_layers):
                 queries = []
                 keys = []
@@ -473,15 +455,15 @@
     logging.info(msg)
     print(msg)
 
 
 def inference(
         text: str, model_path: str, vocab_path: str, classes: List[str],
         num_qubits: int, num_layers: int, depth_ebd: int,
-        depth_query: int, depth_key: int, depth_value: int,
+        depth_query: int, depth_key: int, depth_value: int
 ) -> str:
     r"""
     The inference function. Using the trained model to predict new data.
 
     Args:
         text: The path of the image to be predicted.
         model_path: The path of the model file.
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qml/vsql.py` & `paddle-quantum-2.4.0/paddle_quantum/qml/vsql.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qpp/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/gate/functional/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # !/usr/bin/env python3
-# Copyright (c) 2021 Institute for Quantum Computing, Baidu Inc. All Rights Reserved.
+# Copyright (c) 2022 Institute for Quantum Computing, Baidu Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
-The module of quantum phase processing.
+The module that contains the functions of various quantum gates.
 """
 
-from .laurent import *
-from .angles import *
-from .utils import *
+from .base import simulation
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qpp/angles.py` & `paddle-quantum-2.4.0/paddle_quantum/qpp/angles.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qpp/laurent.py` & `paddle-quantum-2.4.0/paddle_quantum/qpp/laurent.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qpp/utils.py` & `paddle-quantum-2.4.0/paddle_quantum/qpp/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 from .angles import qpp_angle_finder, qpp_angle_approximator
 from .laurent import Q_generation, pair_generation, laurent_generator, revise_tol
 
 from ..ansatz import Circuit
 from ..backend import Backend
 from ..base import get_dtype
 from ..gate import X
-from ..intrinsic import _get_float_dtype
+from ..intrinsic import _get_float_dtype, _type_transform
 from ..linalg import unitary_random, is_unitary
 from ..loss import Measure
 from ..operator import Collapse
 from ..qinfo import dagger, partial_trace
-from ..state import State, _type_transform, zero_state
+from ..state import State, zero_state
 
 
 r"""
 QPP circuit and related tools, see Theorem 6 in paper https://arxiv.org/abs/2209.14278 for more details.
 """
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qsvt/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/qsvt/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qsvt/qsp.py` & `paddle-quantum-2.4.0/paddle_quantum/qsvt/qsp.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qsvt/qsp_utils.py` & `paddle-quantum-2.4.0/paddle_quantum/qsvt/qsp_utils.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/qsvt/qsvt.py` & `paddle-quantum-2.4.0/paddle_quantum/qsvt/qsvt.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/shadow.py` & `paddle-quantum-2.4.0/paddle_quantum/shadow.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 Shadow sample module.
 """
 
 import math
 import numpy as np
 import paddle
 import re
-import paddle_quantum
+import paddle_quantum as pq
 from paddle_quantum import Hamiltonian
 from typing import List, Optional
 
 __all__ = [
     "shadow_sample"
 ]
 
 
 def shadow_sample(
-        state: 'paddle_quantum.State', num_qubits: int, sample_shots: int, mode: paddle_quantum.Backend,
-        hamiltonian: Optional[paddle_quantum.Hamiltonian] = None, method: str = 'CS'
+        state: 'pq.State', num_qubits: int, sample_shots: int, mode: pq.Backend,
+        hamiltonian: Optional[pq.Hamiltonian] = None, method: str = 'CS'
 ) -> list:
     r"""Measure a given quantum state with random Pauli operators and return the measurement results.
 
     Args:
         state: Input quantum state, which is either a state vector or a density matrix.
         num_qubits: The number of qubits.
         sample_shots: The number of random samples.
@@ -92,23 +92,23 @@
             # Add the clifford function
             pass
         else:
             # Other method are transformed as follows
             # Convert to tensor form
             for qubit in range(num_qubits):
                 if pauli_str[qubit] == 'x':
-                    input_state = paddle_quantum.gate.functional.h(input_state, qubit, input_state.dtype, input_state.backend)
+                    input_state = pq.gate.H(qubits_idx=qubit)(input_state)
                 elif pauli_str[qubit] == 'y':
-                    input_state = paddle_quantum.gate.functional.s(input_state, qubit, input_state.dtype, input_state.backend)
-                    input_state = paddle_quantum.gate.functional.z(input_state, qubit, input_state.dtype, input_state.backend)
-                    input_state = paddle_quantum.gate.functional.h(input_state, qubit, input_state.dtype, input_state.backend)
-            if input_state.backend == paddle_quantum.Backend.StateVector:
+                    input_state = pq.gate.S(qubits_idx=qubit)(input_state)
+                    input_state = pq.gate.Z(qubits_idx=qubit)(input_state)
+                    input_state = pq.gate.H(qubits_idx=qubit)(input_state)
+            if input_state.backend == pq.Backend.StateVector:
                 data = input_state.data.numpy()
                 prob_array = np.real(np.multiply(data, np.conj(data)))
-            elif input_state.backend == paddle_quantum.Backend.DensityMatrix:
+            elif input_state.backend == pq.Backend.DensityMatrix:
                 data = input_state.data.numpy()
                 prob_array = np.real(np.diag(data))
             else:
                 raise NotImplementedError
             sample = np.random.choice(range(0, 2 ** num_qubits), size=1, p=prob_array)
             bit_string = bin(sample[0])[2:].zfill(num_qubits)
             return bit_string
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/state/__init__.py` & `paddle-quantum-2.4.0/paddle_quantum/state/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
 The module of the quantum state.
 """
 
-from .state import State, is_state_vector, is_density_matrix
-from .state import _type_fetch, _type_transform
+from .state import State
 from .common import zero_state
 from .common import computational_basis
 from .common import bell_state
 from .common import random_state
 from .common import to_state
 from .common import w_state
 from .common import ghz_state
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/state/common.py` & `paddle-quantum-2.4.0/paddle_quantum/state/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 
 r"""
 The common function of the quantum state.
 """
 
 import numpy as np
 import paddle
-import paddle_quantum
+import paddle_quantum as pq
 import QCompute
-from ..backend import Backend
-from ..backend import quleaf
+from ..base import get_backend, get_dtype
+from ..backend import Backend, quleaf
 from .state import State
 from typing import Union, Optional, List
 
 
 def to_state(
         data: Union[paddle.Tensor, np.ndarray, QCompute.QEnv], num_qubits: Optional[int] = None,
-        backend: Optional[paddle_quantum.Backend] = None, dtype: Optional[str] = None
+        backend: Optional[Backend] = None, dtype: Optional[str] = None
 ) -> State:
     r"""The function to generate a specified state instance.
 
     Args:
         data: The analytical form of quantum state.
         num_qubits: The number of qubits contained in the quantum state. Defaults to ``None``, which means it will be inferred by the data.
         backend: Used to specify the backend used. Defaults to ``None``, which means to use the default backend.
@@ -44,35 +44,35 @@
     """
     if isinstance(data, np.ndarray):
         data = paddle.to_tensor(data)
     return State(data, num_qubits, backend, dtype)
 
 
 def zero_state(
-        num_qubits: int, backend: Optional[paddle_quantum.Backend] = None, dtype: Optional[str] = None
+        num_qubits: int, backend: Optional[Backend] = None, dtype: Optional[str] = None
 ) -> State:
     r"""The function to generate a zero state.
 
     Args:
         num_qubits: The number of qubits contained in the quantum state.
         backend: Used to specify the backend used. Defaults to ``None``, which means to use the default backend.
         dtype: Used to specify the data dtype of the data. Defaults to ``None``, which means to use the default data type.
 
     Raises:
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
        The generated quantum state.
     """
-    dtype = paddle_quantum.get_dtype() if dtype is None else dtype
+    dtype = get_dtype() if dtype is None else dtype
     np_dtype = np.complex64 if dtype == 'complex64' else np.complex128
     data = np.zeros((2 ** num_qubits,), dtype=np_dtype)
     data[0] = 1
     data = paddle.to_tensor(data)
-    backend = paddle_quantum.get_backend() if backend is None else backend
+    backend = get_backend() if backend is None else backend
     if backend == Backend.StateVector:
         state = State(data, num_qubits, backend=backend, dtype=dtype)
     elif backend == Backend.DensityMatrix:
         data = paddle.unsqueeze(data, axis=1)
         data = paddle.matmul(data, paddle.conj(paddle.t(data)))
         state = State(data, num_qubits, backend=backend, dtype=dtype)
     elif backend == Backend.QuLeaf:
@@ -82,15 +82,15 @@
         state = State(data, num_qubits, backend=backend, dtype=dtype)
     else:
         raise NotImplementedError
     return state
 
 
 def computational_basis(
-        num_qubits: int, index: int, backend: Optional[paddle_quantum.Backend] = None, dtype: Optional[str] = None
+        num_qubits: int, index: int, backend: Optional[Backend] = None, dtype: Optional[str] = None
 ) -> State:
     r"""Generate a computational basis state :math:`|e_{i}\rangle` , whose i-th element is 1 and all the other elements are 0.
 
     Args:
         num_qubits: The number of qubits contained in the quantum state.
         index:  Index :math:`i` of the computational basis state :math`|e_{i}rangle` .
         backend: Used to specify the backend used. Defaults to ``None``, which means to use the default backend.
@@ -98,32 +98,32 @@
 
     Raises:
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
         The generated quantum state.
     """
-    dtype = paddle_quantum.get_dtype() if dtype is None else dtype
+    dtype = get_dtype() if dtype is None else dtype
     np_dtype = np.complex64 if dtype == 'complex64' else np.complex128
     data = np.zeros((2 ** num_qubits,), dtype=np_dtype)
     data[index] = 1
     data = paddle.to_tensor(data)
-    backend = paddle_quantum.get_backend() if backend is None else backend
+    backend = get_backend() if backend is None else backend
     if backend == Backend.StateVector:
         state = State(data, num_qubits, backend=backend)
     elif backend == Backend.DensityMatrix:
         data = paddle.unsqueeze(data, axis=1)
         data = paddle.matmul(data, paddle.conj(paddle.t(data)))
         state = State(data, num_qubits, backend=backend)
     else:
         raise NotImplementedError
     return state
 
 
-def bell_state(num_qubits: int, backend: Optional[paddle_quantum.Backend] = None) -> State:
+def bell_state(num_qubits: int, backend: Optional[Backend] = None) -> State:
     r"""Generate a bell state.
 
     Its matrix form is:
 
     .. math::
 
         |\Phi_{D}\rangle=\frac{1}{\sqrt{D}} \sum_{j=0}^{D-1}|j\rangle_{A}|j\rangle_{B}
@@ -134,23 +134,23 @@
 
     Raises:
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
         The generated quantum state.
     """
-    np_dtype = np.complex64 if paddle_quantum.get_dtype() == 'complex64' else np.complex128
+    np_dtype = np.complex64 if get_dtype() == 'complex64' else np.complex128
     dim = 2 ** num_qubits
     local_dim = 2 ** int(num_qubits / 2)
     coeff = 1 / local_dim
     data = np.zeros((dim, dim), dtype=np_dtype)
     for i in range(0, dim, local_dim + 1):
         for j in range(0, dim, local_dim + 1):
             data[i, j] = coeff
-    backend = paddle_quantum.get_backend() if backend is None else backend
+    backend = get_backend() if backend is None else backend
     if backend == Backend.StateVector:
         eigenvalue, eigenvector = paddle.linalg.eig(paddle.to_tensor(data))
         data = eigenvector[:, paddle.argmax(paddle.real(eigenvalue))]
         state = State(data, num_qubits, backend=backend)
     elif backend == Backend.DensityMatrix:
         state = State(paddle.to_tensor(data), num_qubits, backend=backend)
     else:
@@ -178,28 +178,28 @@
     Returns:
         The generated quantum state.
     """
     p1, p2, p3, p4 = prob
     assert 0 <= p1 <= 1 and 0 <= p2 <= 1 and 0 <= p3 <= 1 and 0 <= p4 <= 1, "Each probability must be in [0, 1]."
     assert abs(p1 + p2 + p3 + p4 - 1) < 1e-6, "The sum of probabilities should be 1."
 
-    np_dtype = np.complex64 if paddle_quantum.get_dtype() == 'complex64' else np.complex128
+    np_dtype = np.complex64 if get_dtype() == 'complex64' else np.complex128
     coeff = np.sqrt(0.5)
     phi_p_vec = np.array([[coeff, 0, 0, coeff]], dtype=np_dtype)
     phi_p_mat = np.matmul(phi_p_vec.T, phi_p_vec)
     phi_m_vec = np.array([[coeff, 0, 0, -coeff]], dtype=np_dtype)
     phi_m_mat = np.matmul(phi_m_vec.T, phi_m_vec)
     psi_p_vec = np.array([[0, coeff, coeff, 0]], dtype=np_dtype)
     psi_p_mat = np.matmul(psi_p_vec.T, psi_p_vec)
     psi_m_vec = np.array([[0, coeff, -coeff, 0]], dtype=np_dtype)
     psi_m_mat = np.matmul(psi_m_vec.T, psi_m_vec)
 
     state = p1 * phi_p_mat + p2 * psi_p_mat + p3 * phi_m_mat + p4 * psi_m_mat
 
-    backend = paddle_quantum.get_backend()
+    backend = get_backend()
     if backend == Backend.StateVector:
         trace_rho = paddle.trace(paddle.to_tensor(state) @ paddle.to_tensor(state))
         if trace_rho.numpy()[0] == 1:
             eigenvalue, eigenvector = paddle.linalg.eig(paddle.to_tensor(state))
             data = eigenvector[:, paddle.argmax(paddle.real(eigenvalue))]
             state = State(data, backend=backend)
         else:
@@ -221,59 +221,41 @@
 
     Raises:
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
         The generated quantum state.
     """
-    float_dtype = 'float32' if paddle_quantum.get_dtype() == 'complex64' else 'float64'
-    backend = paddle_quantum.get_backend()
+    backend = get_backend()
     if backend == Backend.StateVector:
-        if is_real:
-            data = paddle.rand((2 ** num_qubits,), dtype=float_dtype)
-        else:
-            data_real = paddle.rand((2 ** num_qubits,), dtype=float_dtype)
-            data_imag = paddle.rand((2 ** num_qubits,), dtype=float_dtype)
-            data = data_real + 1j * data_imag
-        norm = np.linalg.norm(data.numpy())
-        data = data / paddle.to_tensor(norm)
-        state = State(data, num_qubits, backend=backend)
+        data = pq.linalg.haar_state_vector(num_qubits, is_real)
     elif backend == Backend.DensityMatrix:
-        rank = 2 ** num_qubits if rank is None else rank
-        if is_real:
-            data = paddle.rand((2 ** num_qubits, rank), dtype=float_dtype)
-        else:
-            data_real = paddle.rand((2 ** num_qubits, rank), dtype=float_dtype)
-            data_imag = paddle.rand((2 ** num_qubits, rank), dtype=float_dtype)
-            data = data_real + 1j * data_imag
-        data = paddle.matmul(data, paddle.conj(paddle.t(data)))
-        data = data / paddle.trace(data)
-        state = State(data, num_qubits, backend=backend)
+        data = pq.linalg.haar_density_operator(num_qubits, rank, is_real)
     else:
         raise NotImplementedError
-    return state
+    return State(data, num_qubits, backend=backend)
 
 
 def w_state(num_qubits: int) -> 'State':
     r"""Generate a W-state.
 
     Args:
         num_qubits: The number of qubits contained in the quantum state.
 
     Raises:
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
         The generated quantum state.
     """
-    np_dtype = np.complex64 if paddle_quantum.get_dtype() == 'complex64' else np.complex128
-    coeff = np.ones((1, 2 ** num_qubits)) / np.sqrt(num_qubits)
-    backend = paddle_quantum.get_backend()
+    np_dtype = np.complex64 if get_dtype() == 'complex64' else np.complex128
+    coeff = np.ones(2 ** num_qubits) / np.sqrt(num_qubits)
+    backend = get_backend()
     if backend == Backend.StateVector:
-        state = np.zeros((1, 2 ** num_qubits), dtype=np_dtype)
+        state = np.zeros(2 ** num_qubits, dtype=np_dtype)
         for i in range(num_qubits):
             state[0][2 ** i] = coeff[0][num_qubits - i - 1]
         state = State(paddle.to_tensor(state), num_qubits, backend=backend)
     elif backend == Backend.DensityMatrix:
         state = np.zeros(2 ** num_qubits, dtype=np_dtype)
         for i in range(num_qubits):
             state[2 ** i] = coeff[0][num_qubits - i - 1]
@@ -294,20 +276,20 @@
 
     Raises:
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
         The generated quantum state.
     """
-    np_dtype = np.complex64 if paddle_quantum.get_dtype() == 'complex64' else np.complex128
-    backend = paddle_quantum.get_backend()
+    np_dtype = np.complex64 if get_dtype() == 'complex64' else np.complex128
+    backend = get_backend()
     if backend == Backend.StateVector:
-        state = np.zeros((1, 2 ** num_qubits))
-        state[0][0] = 1 / np.sqrt(2)
-        state[0][-1] = 1 / np.sqrt(2)
+        state = np.zeros(2 ** num_qubits, dtype=np_dtype)
+        state[0] = 1 / np.sqrt(2)
+        state[-1] = 1 / np.sqrt(2)
         state = State(paddle.to_tensor(state), num_qubits, backend=backend)
     elif backend == Backend.DensityMatrix:
         state = np.zeros(2 ** num_qubits, dtype=np_dtype)
         state[0] = 1 / np.sqrt(2)
         state[-1] = 1 / np.sqrt(2)
         state = paddle.to_tensor(state)
         state = paddle.unsqueeze(state, axis=1)
@@ -329,18 +311,18 @@
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
         The generated quantum state.
     """
     assert num_qubits > 0, 'qubit number must be positive'
 
-    np_dtype = np.complex64 if paddle_quantum.get_dtype() == 'complex64' else np.complex128
+    np_dtype = np.complex64 if get_dtype() == 'complex64' else np.complex128
     state = np.eye(2 ** num_qubits) / (2 ** num_qubits)
     state = state.astype(np_dtype)
-    backend = paddle_quantum.get_backend()
+    backend = get_backend()
     if backend == Backend.StateVector:
         trace_rho = paddle.trace(paddle.to_tensor(state) @ paddle.to_tensor(state))
         if trace_rho.numpy()[0] == 1:
             eigenvalue, eigenvector = paddle.linalg.eig(paddle.to_tensor(state))
             data = eigenvector[:, paddle.argmax(paddle.real(eigenvalue))]
             state = State(data, backend=backend)
         else:
@@ -369,23 +351,23 @@
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
         The generated quantum state.
     """
     assert 0 <= prob <= 1, "Probability must be in [0, 1]"
 
-    np_dtype = np.complex64 if paddle_quantum.get_dtype() == 'complex64' else np.complex128
+    np_dtype = np.complex64 if get_dtype() == 'complex64' else np.complex128
     coeff = np.sqrt(0.5)
     psi_p_vec = np.array([[0, coeff, coeff, 0]])
     psi_p_mat = np.matmul(psi_p_vec.T, psi_p_vec)
     state_11 = np.zeros((4, 4))
     state_11[3, 3] = 1
     state = prob * psi_p_mat + (1 - prob) * state_11
     state = state.astype(np_dtype)
-    backend = paddle_quantum.get_backend()
+    backend = get_backend()
     if backend == Backend.StateVector:
         trace_rho = paddle.trace(paddle.to_tensor(state) @ paddle.to_tensor(state))
         if trace_rho.numpy()[0] == 1:
             eigenvalue, eigenvector = paddle.linalg.eig(paddle.to_tensor(state))
             data = eigenvector[:, paddle.argmax(paddle.real(eigenvalue))]
             state = State(data, backend=backend)
         else:
@@ -414,22 +396,22 @@
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
         The generated quantum state.
     """
     assert 0 <= prob <= 1, "Probability must be in [0, 1]"
 
-    np_dtype = np.complex64 if paddle_quantum.get_dtype() == 'complex64' else np.complex128
+    np_dtype = np.complex64 if get_dtype() == 'complex64' else np.complex128
     phi_p = bell_state(2).data.numpy()
     psi0 = np.zeros_like(phi_p)
     psi0[0, 0] = 1
     state = prob * phi_p + (1 - prob) * psi0
     state = state.astype(np_dtype)
 
-    backend = paddle_quantum.get_backend()
+    backend = get_backend()
     if backend == Backend.StateVector:
         trace_rho = paddle.trace(paddle.to_tensor(state) @ paddle.to_tensor(state))
         if trace_rho.numpy()[0] == 1:
             eigenvalue, eigenvector = paddle.linalg.eig(paddle.to_tensor(state))
             data = eigenvector[:, paddle.argmax(paddle.real(eigenvalue))]
             state = State(data, backend=backend)
         else:
@@ -459,21 +441,21 @@
         NotImplementedError: If the backend is wrong or not implemented.
 
     Returns:
         The generated quantum state.
     """
     assert 0 <= prob <= 1, "Probability must be in [0, 1]"
 
-    np_dtype = np.complex64 if paddle_quantum.get_dtype() == 'complex64' else np.complex128
+    np_dtype = np.complex64 if get_dtype() == 'complex64' else np.complex128
     dim = 2 ** num_qubits
     phi_b = bell_state(num_qubits).data.numpy()
     state = prob * phi_b + (1 - prob) * np.eye(dim) / dim
     state = state.astype(np_dtype)
 
-    backend = paddle_quantum.get_backend()
+    backend = get_backend()
     if backend == Backend.StateVector:
         trace_rho = paddle.trace(paddle.to_tensor(state) @ paddle.to_tensor(state))
         if trace_rho.numpy()[0] == 1:
             eigenvalue, eigenvector = paddle.linalg.eig(paddle.to_tensor(state))
             data = eigenvector[:, paddle.argmax(paddle.real(eigenvalue))]
             state = State(data, backend=backend)
         else:
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/state/state.py` & `paddle-quantum-2.4.0/paddle_quantum/state/state.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,92 +14,97 @@
 # limitations under the License.
 
 r"""
 The basic class of the quantum state.
 """
 
 import collections
+import copy
 import math
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.linalg import expm
 import random
 
 import paddle
 import QCompute
-import paddle_quantum
-from ..backend import Backend
-from ..backend import state_vector, density_matrix, quleaf
-from ..hamiltonian import Hamiltonian
-from typing import Optional, Union, Iterable, Tuple
+import paddle_quantum as pq
+from ..backend import Backend, state_vector, density_matrix, quleaf
+from ..base import get_backend, get_dtype
+from typing import Optional, Union, Iterable, List, Dict
 
 
 class State(object):
     r"""The quantum state class.
 
         Args:
             data: The mathematical analysis of quantum state.
             num_qubits: The number of qubits contained in the quantum state. Defaults to ``None``, which means it will be inferred by the data.
             backend: Used to specify the backend used. Defaults to ``None``, which means to use the default backend.
             dtype: Used to specify the data dtype of the data. Defaults to ``None``, which means to use the default data type.
             override: whether override the input test. ONLY for internal use. Defaults to ``False``.
-        
+
         Raises:
             ValueError: Cannot recognize the backend.
         """
     def __init__(
             self, data: Union[paddle.Tensor, np.ndarray, QCompute.QEnv], num_qubits: Optional[int] = None,
-            backend: Optional[paddle_quantum.Backend] = None, dtype: Optional[str] = None, override: Optional[bool] = False
+            backend: Optional[Backend] = None, dtype: Optional[str] = None, override: Optional[bool] = False
     ):
         # TODO: need to check whether it is a legal quantum state
         super().__init__()
-        self.backend = paddle_quantum.get_backend() if backend is None else backend
-        self.dtype = dtype if dtype is not None else paddle_quantum.get_dtype()
-        if self.backend != Backend.QuLeaf and not isinstance(data, paddle.Tensor):
+        self.backend = get_backend() if backend is None else backend
+        self.dtype = dtype if dtype is not None else get_dtype()
+        # TODO: If the dtype is right, don't do the cast operation.
+        if isinstance(data, paddle.Tensor):
+            self.data = paddle.cast(data, self.dtype) if data.dtype != self.dtype else data
+        elif self.backend != Backend.QuLeaf:
             data = paddle.to_tensor(data, dtype=self.dtype)
-        self.data = paddle.cast(data, self.dtype) if data.dtype != self.dtype else data
-
+            self.data = paddle.cast(data, self.dtype)
         # data input test
         if self.backend == Backend.StateVector:
             if data.shape[-1] == 1:
                 self.data = paddle.squeeze(data)
-
             if not override:
-                is_vec, data_message = is_state_vector(data)
-                assert is_vec, \
-                        f"The input data is not a legal state vector: error message {data_message}"
-                assert num_qubits is None or num_qubits == data_message, \
-                        f"num_qubits does not agree: expected {num_qubits}, received {data_message}"
+                is_vec, data_message = pq.linalg.is_state_vector(data)
+                assert is_vec, f"The input data is not a legal state vector: error message {data_message}"
+                assert num_qubits is None or num_qubits == data_message, (
+                    f"num_qubits does not agree: expected {num_qubits}, received {data_message}")
                 num_qubits = data_message
-
         elif self.backend == Backend.DensityMatrix:
-
             if not override:
-                is_den, data_message = is_density_matrix(data)
-                assert is_den, \
-                        f"The input data is not a legal density matrix: error message {data_message}"
-                assert num_qubits is None or num_qubits == data_message, \
-                        f"num_qubits does not agree: expected {num_qubits}, received {data_message}"
+                is_den, data_message = pq.linalg.is_density_matrix(data)
+                assert is_den, f"The input data is not a legal density matrix: error message {data_message}"
+                assert num_qubits is None or num_qubits == data_message, (
+                    f"num_qubits does not agree: expected {num_qubits}, received {data_message}")
                 num_qubits = data_message
-
         elif self.backend == Backend.UnitaryMatrix:
             # no need to check the state in unitary backend
             if num_qubits is None:
                 num_qubits = int(math.log2(data.shape[0]))
-
         elif self.backend == Backend.QuLeaf:
+            self.data = data
             if quleaf.get_quleaf_backend() != QCompute.BackendName.LocalBaiduSim2:
                 assert quleaf.get_quleaf_token() is not None, "You must input token tu use cloud server."
-            self.gate_history = []
-            self.param_list = []
-            self.num_param = 0
         else:
             raise ValueError(
                 f"Cannot recognize the backend {self.backend}")
         self.num_qubits = num_qubits
+        
+        # initialize default qubit sequence 
+        self.qubit_sequence = list(range(num_qubits))
+
+        # whether use the old doubly-swap logic to compute the matrix multiplication. Defaults to ``False``.
+        self.is_swap_back = True
+
+    def __getitem__(self, key: Union[int, slice]) -> 'State':
+        r"""Indexing of the State class
+        """
+        qubits = list(range(self.num_qubits))[key]
+        return pq.qinfo.partial_trace_discontiguous(self, qubits if isinstance(qubits, List) else [qubits])
 
     @property
     def ket(self) -> paddle.Tensor:
         r"""Return the ket form in state_vector backend
 
         Raises:
             ValueError: the backend must be in StateVector
@@ -109,15 +114,15 @@
 
         """
         if self.backend != Backend.StateVector:
             raise ValueError(
                 f"the backend must be in StateVector: received {self.backend}")
 
         return self.data.reshape([2 ** self.num_qubits, 1])
-    
+
     @property
     def bra(self) -> paddle.Tensor:
         r"""Return the bra form in state_vector backend
 
         Raises:
             ValueError: the backend must be in StateVector
 
@@ -126,85 +131,83 @@
 
         """
         if self.backend != Backend.StateVector:
             raise ValueError(
                 f"the backend must be in StateVector: received {self.backend}")
 
         return paddle.conj(self.data.reshape([1, 2 ** self.num_qubits]))
-    
+
     def normalize(self) -> None:
         r"""Normalize this state
-        
+
         Raises:
             NotImplementedError: does not support normalization for the backend
-
         """
         data = self.data
         if self.backend == Backend.StateVector:
             data /= paddle.norm(paddle.abs(data))
         elif self.backend == Backend.DensityMatrix:
             data /= paddle.trace(data)
         else:
             raise NotImplementedError(
                 f"Does not support normalization for the backend {self.backend}")
         self.data = data
-        
-    def evolve(self, H: Union[np.ndarray, paddle.Tensor, Hamiltonian], t: float) -> None:
+
+    def evolve(self, H: Union[np.ndarray, paddle.Tensor, 'pq.Hamiltonian'], t: float) -> None:
         r"""Evolve the state under the Hamiltonian `H` i.e. apply unitary operator :math:`e^{-itH}`
-        
+
         Args:
             H: the Hamiltonian of the system
             t: the evolution time
-        
+
         Raises:
             NotImplementedError: does not support evolution for the backend
 
         """
-        if isinstance(H, Hamiltonian):
+        if isinstance(H, pq.Hamiltonian):
             num_qubits = max(self.num_qubits, H.n_qubits)
             H = H.construct_h_matrix(qubit_num=num_qubits)
         else:
             num_qubits = int(math.log2(H.shape[0]))
-            H = _type_transform(H, "numpy")
-        assert num_qubits == self.num_qubits, \
-            f"the # of qubits of Hamiltonian and this state are not the same: received {num_qubits}, expect {self.num_qubits}"
+            H = pq.intrinsic._type_transform(H, "numpy")
+        assert num_qubits == self.num_qubits, (
+            "the # of qubits of Hamiltonian and this state are not the same: "
+            f"received {num_qubits}, expect {self.num_qubits}")
         e_itH = paddle.to_tensor(expm(-1j * t * H), dtype=self.dtype)
-        
+
         if self.backend == Backend.StateVector:
             self.data = paddle.squeeze(e_itH @ self.ket)
         elif self.backend == Backend.DensityMatrix:
             self.data = e_itH @ self.data @ paddle.conj(e_itH.T)
         else:
             raise NotImplementedError(
                 f"Does not support evolution for the backend {self.backend}")
-    
+
     def kron(self, other: 'State') -> 'State':
         r"""Kronecker product between states
-        
+
         Args:
             other: a quantum state
-            
+
         Returns:
             the tensor product of these two states
-            
         """
         backend, dtype = self.backend, self.dtype
         assert backend == other.backend, \
             f"backends between two States are not the same: received {backend} and {other.backend}"
         assert dtype == other.dtype, \
             f"dtype between two States are not the same: received {dtype} and {other.dtype}"
-        
         if backend == Backend.StateVector:
             return State(paddle.kron(self.ket, other.ket), backend=backend)
         else:
             return State(paddle.kron(self.data, other.data), backend=backend, dtype=dtype)
-        
+
     def __matmul__(self, other: 'State') -> paddle.Tensor:
         r"""Matrix product between states or between tensor and state
-        
+
         Args:
             other: a quantum state
 
         Raises:
             NotImplementedError: does not support the product between State and input format.
             ValueError: Cannot multiply two state vectors: check the backend
 
@@ -214,37 +217,36 @@
         if not isinstance(other, State):
             raise NotImplementedError(
                 f"does not support the product between State and {type(other)}")
         if self.backend == Backend.StateVector:
             raise ValueError(
                 "Cannot multiply two state vectors: check the backend")
         return self.data @ other.data
-    
+
     def __rmatmul__(self, other: 'State') -> paddle.Tensor:
         r"""Matrix product between states or between state and tensor
-        
+
         Args:
             other: a quantum state
 
         Raises:
             NotImplementedError: does not support the product between State and input format.
             ValueError: Cannot multiply two state vectors: check the backend
 
         Returns:
             the product of these two states
-
         """
         if not isinstance(other, State):
             raise NotImplementedError(
                 f"does not support the product between {type(other)} and State")
         if self.backend == Backend.StateVector:
             raise ValueError(
                 "Cannot multiply two state vectors: check your backend")
         return other.data @ self.data
-    
+
     def numpy(self) -> np.ndarray:
         r"""Get the data in numpy.
 
         Returns:
             The numpy array of the data for the quantum state.
         """
         return self.data.numpy()
@@ -253,58 +255,90 @@
         r"""Change the property of the state.
 
         Args:
             backend: Specify the new backend of the state.
             dtype: Specify the new data type of the state.
             device: Specify the new device of the state.
             blocking: Specify the new blocking of the state.
-        
+
         Raises
             NotImplementedError: only support transformation between StateVector and DensityMatrix
             NotImplementedError: Transformation for device or blocking is not supported.
-
         """
-        if (backend not in {"state_vector", "density_matrix"} or 
-            self.backend not in {Backend.StateVector, Backend.DensityMatrix}):
+        if (
+            backend not in {"state_vector", "density_matrix"} or
+            self.backend not in {Backend.StateVector, Backend.DensityMatrix}
+        ):
             raise NotImplementedError(
                 "Only support transformation between StateVector and DensityMatrix")
-        
+
         if device is not None or blocking is not None:
             raise NotImplementedError(
                 "Transformation for device or blocking is not supported")
-        
-        self.data = _type_transform(self, backend).data
+
+        self.data = pq.intrinsic._type_transform(self, backend).data
         self.dtype = self.dtype if dtype is None else dtype
 
     def clone(self) -> 'State':
         r"""Return a copy of the quantum state.
 
         Returns:
             A new state which is identical to this state.
         """
-        return State(self.data, self.num_qubits, self.backend, self.dtype, override=True)
+        new_state = State(paddle.clone(self.data), self.num_qubits, self.backend, self.dtype, override=True)
+        new_state.qubit_sequence = self.qubit_sequence
+        new_state.is_swap_back = self.is_swap_back
+        return new_state
+
+    def __copy__(self) -> 'State':
+        return self.clone()
 
     def __str__(self):
         return str(self.data.numpy())
+    
+    @property
+    def oper_history(self) -> List[Dict[str, Union[str, List[int], paddle.Tensor]]]:
+        r"""The operator history stored for the QPU backend
+        
+        Raises:
+            NotImplementedError: This property should be called for the backend ``quleaf`` only.
+            ValueError: This state does not have operator history: run the circuit first.
+        
+        """
+        if self.backend != Backend.QuLeaf:
+            raise NotImplementedError(
+                "This property should be called for backend `quleaf only.")
+        
+        if not hasattr(self, '_State__oper_history'):
+            raise ValueError(
+                "This state does not have operator history: run the circuit first.")
+        return self.__oper_history
+
+    @oper_history.setter
+    def oper_history(self, oper_history: List[Dict[str, Union[str, List[int], paddle.Tensor]]]) -> None:
+        if self.backend != Backend.QuLeaf:
+            raise NotImplementedError(
+                "This property should be changed for backend `quleaf only.")
+        self.__oper_history = oper_history
 
-    def expec_val(self, hamiltonian: Hamiltonian, shots: Optional[int] = 0) -> float:
+    def expec_val(self, hamiltonian: 'pq.Hamiltonian', shots: Optional[int] = 0) -> float:
         r"""The expectation value of the observable with respect to the quantum state.
 
         Args:
             hamiltonian: Input observable.
             shots: Number of measurement shots.
 
         Raises:
             NotImplementedError: If the backend is wrong or not implemented.
 
         Returns:
             The expectation value of the input observable for the quantum state.
         """
         if shots == 0:
-            func = paddle_quantum.loss.ExpecVal(hamiltonian)
+            func = pq.loss.ExpecVal(hamiltonian)
             result = func(self)
             return result.item()
         result = 0
         gate_for_x = paddle.to_tensor([
             [1 / math.sqrt(2), 1 / math.sqrt(2)],
             [1 / math.sqrt(2), -1 / math.sqrt(2)],
         ], dtype=self.dtype)
@@ -333,300 +367,153 @@
                     state_data = simulator(
                         state_data, gate_for_x, idx, self.num_qubits
                     )
                 elif pauli.lower() == 'y':
                     state_data = simulator(
                         state_data, gate_for_y, idx, self.num_qubits
                     )
-            if self.backend == paddle_quantum.Backend.StateVector:
+            if self.backend == Backend.StateVector:
                 prob_amplitude = paddle.multiply(paddle.conj(state_data), state_data).real()
-            elif self.backend == paddle_quantum.Backend.DensityMatrix:
+            elif self.backend == Backend.DensityMatrix:
                 prob_amplitude = paddle.zeros([2 ** self.num_qubits])
                 for idx in range(2 ** self.num_qubits):
                     prob_amplitude[idx] += state_data[idx, idx].real()
             else:
                 raise NotImplementedError
             prob_amplitude = prob_amplitude.tolist()
             all_case = [bin(element)[2:].zfill(self.num_qubits) for element in range(2 ** self.num_qubits)]
             samples = random.choices(all_case, weights=prob_amplitude, k=shots)
             counter = collections.Counter(samples)
             measured_results = [([key[idx] for idx in qubits_list], val) for key, val in counter.items()]
             temp_res = sum(((-1) ** key.count('1') * val / shots for key, val in measured_results))
             result += coeff * temp_res
         return result
 
-    def measure(self, shots: Optional[int] = 0, qubits_idx: Optional[Union[Iterable[int], int]] = None, 
-                plot: Optional[bool] = False) -> dict:
+    def measure(
+            self, shots: Optional[int] = 0, qubits_idx: Optional[Union[Iterable[int], int]] = None,
+            plot: Optional[bool] = False, record: Optional[bool] = False
+    ) -> dict:
         r"""Measure the quantum state
 
         Args:
             shots: the number of measurements on the quantum state output by the quantum circuit.
                 Default is ``0``, which means the exact probability distribution of measurement results are returned.
             qubits_idx: The index of the qubit to be measured. Defaults to ``None``, which means all qubits are measured.
             plot: Whether to draw the measurement result plot. Defaults to ``False`` which means no plot.
+            record: Whether to return the original measurement record. Defaults to ``False`` which means no record.
 
         Raises:
-            Exception: The number of shots should be greater than 0.
+            ValueError: The number of shots should be greater than 0.
+            NotImplementedError: When the backend is Quleaf, record is not supprted .
             NotImplementedError: If the backend is wrong or not implemented.
             NotImplementedError: The qubit index is wrong or not supported.
+            ValueError: Returning records requires the number of shots to be greater than 0.
 
         Returns:
             Measurement results
         """
-        if self.backend == paddle_quantum.Backend.QuLeaf:
+        if self.backend == Backend.QuLeaf:
             if shots == 0:
-                    raise Exception("The quleaf server requires the number of shots to be greater than 0.")
-            state_data = self.data
-            QCompute.MeasureZ(*state_data.Q.toListPair())
-            result = state_data.commit(shots, fetchMeasure=True)['counts']
-            result = {''.join(reversed(key)): value for key, value in result.items()}
-        elif self.backend == paddle_quantum.Backend.StateVector:
-            prob_amplitude = paddle.multiply(paddle.conj(self.data), self.data).real()
-        elif self.backend == paddle_quantum.Backend.DensityMatrix:
-            prob_amplitude = paddle.zeros([2 ** self.num_qubits])
-            for idx in range(2 ** self.num_qubits):
-                prob_amplitude[idx] += self.data[idx, idx].real()
-        else:
-            raise NotImplementedError
-        if qubits_idx is None:
-            prob_array = prob_amplitude
-            num_measured = self.num_qubits
-        elif isinstance(qubits_idx, (Iterable, int)):
-            qubits_idx = [qubits_idx] if isinstance(qubits_idx, int) else list(qubits_idx)
+                raise ValueError("The quleaf server requires the number of shots to be greater than 0.")
+            if record == True:
+                raise NotImplementedError
+            state_data = copy.deepcopy(self.data)
+            if qubits_idx is None:
+                qubits_idx = list(range(self.num_qubits))
+            elif isinstance(qubits_idx, int):
+                qubits_idx = [qubits_idx]
             num_measured = len(qubits_idx)
-            prob_array = paddle.zeros([2 ** num_measured])
-            for idx in range(2 ** self.num_qubits):
-                binary = bin(idx)[2:].zfill(self.num_qubits)
-                target_qubits = ''.join(binary[qubit_idx] for qubit_idx in qubits_idx)
-                prob_array[int(target_qubits, base=2)] += prob_amplitude[idx]
-        else:
-            raise NotImplementedError
-        if shots == 0:
-            freq = prob_array.tolist()
-            result = {bin(idx)[2:].zfill(num_measured): val for idx, val in enumerate(freq)}
+            q_reg, _ = state_data.Q.toListPair()
+            q_reg = [q_reg[idx] for idx in qubits_idx]
+            c_reg = list(range(num_measured))
+            state_data = quleaf._act_gates_to_state(self.oper_history, state_data)
+            QCompute.MeasureZ(q_reg, c_reg)
+            result = state_data.commit(shots, fetchMeasure=True)['counts']
+            result = {key[::-1]: value for key, value in result.items()}
+            basis_list = [bin(idx)[2:].zfill(num_measured) for idx in range(2 ** num_measured)]
+            freq = [0 if basis not in result else result[basis] / shots for basis in basis_list]
         else:
-            samples = random.choices(range(0, 2 ** num_measured), weights=prob_array, k=shots)
-            freq = [0] * (2 ** num_measured)
-            for item in samples:
-                freq[item] += 1
-            freq = [val / shots for val in freq]
-            result = {bin(idx)[2:].zfill(num_measured): val for idx, val in enumerate(freq)}
+            if self.backend == Backend.StateVector:
+                prob_amplitude = paddle.multiply(paddle.conj(self.data), self.data).real()
+            elif self.backend == Backend.DensityMatrix:
+                prob_amplitude = paddle.zeros([2 ** self.num_qubits])
+                for idx in range(2 ** self.num_qubits):
+                    prob_amplitude[idx] += self.data[idx, idx].real()
+            else:
+                raise NotImplementedError
+            if qubits_idx is None:
+                prob_array = prob_amplitude
+                num_measured = self.num_qubits
+            elif isinstance(qubits_idx, (Iterable, int)):
+                qubits_idx = [qubits_idx] if isinstance(qubits_idx, int) else list(qubits_idx)
+                num_measured = len(qubits_idx)
+                prob_array = paddle.zeros([2 ** num_measured])
+                for idx in range(2 ** self.num_qubits):
+                    binary = bin(idx)[2:].zfill(self.num_qubits)
+                    target_qubits = ''.join(binary[qubit_idx] for qubit_idx in qubits_idx)
+                    prob_array[int(target_qubits, base=2)] += prob_amplitude[idx]
+            else:
+                raise NotImplementedError
+            if shots == 0:
+                if record == True:
+                    raise ValueError("Returning records requires the number of shots to be greater than 0.")
+                freq = prob_array.tolist()
+            else:
+                result_record = [] # record of original measurement results
+                samples = random.choices(range(2 ** num_measured), weights=prob_array, k=shots)
+                freq = [0] * (2 ** num_measured)
+                for item in samples:
+                    freq[item] += 1
+                    result_record.append(bin(item)[2:].zfill(num_measured))
+                freq = [val / shots for val in freq]
+            if record == False:
+                result = {bin(idx)[2:].zfill(num_measured): val for idx, val in enumerate(freq)}
+            else:
+                result = {"Measurement Record": result_record}
         if plot:
             assert num_measured < 6, "Too many qubits to plot"
             ylabel = "Measured Probabilities" if shots == 0 else "Probabilities"
-            state_list = [bin(idx)[2:].zfill(num_measured) for idx in range(0, 2 ** num_measured)]
-            plt.bar(range(2 ** num_measured), freq, tick_label=state_list)
+            basis_list = [bin(idx)[2:].zfill(num_measured) for idx in range(2 ** num_measured)]
+            plt.bar(range(2 ** num_measured), freq, tick_label=basis_list)
             plt.xticks(rotation=90)
             plt.xlabel("Qubit State")
             plt.ylabel(ylabel)
             plt.show()
         return result
-
-
-def _type_fetch(data: Union[np.ndarray, paddle.Tensor, State]) -> str:
-    r""" fetch the type of ``data``
-    
-    Args:
-        data: the input data, and datatype of which should be either ``numpy.ndarray``,
-    ''paddle.Tensor'' or ``paddle_quantum.State``
-    
-    Returns:
-        string of datatype of ``data``, can be either ``"numpy"``, ``"tensor"``,
-    ``"state_vector"`` or ``"density_matrix"``
     
-    Raises:
-        ValueError: does not support the current backend of input state.
-        TypeError: cannot recognize the current type of input data.
-    
-    """
-    if isinstance(data, np.ndarray):
-        return "numpy"
-    
-    if isinstance(data, paddle.Tensor):
-        return "tensor"
-    
-    if isinstance(data, State):
-        if data.backend == Backend.StateVector:
-            return "state_vector"
-        if data.backend == Backend.DensityMatrix:
-            return "density_matrix"
-        raise ValueError(
-            f"does not support the current backend {data.backend} of input state.")
-        
-    raise TypeError(
-        f"cannot recognize the current type {type(data)} of input data.")
+    def __set_qubit_seq__(self, qubit_sequence: List[int]) -> None:
 
+        data = self.data
+        perm_map = pq.intrinsic._perm_of_list(self.qubit_sequence, qubit_sequence)
+        if self.backend == Backend.StateVector:
+            higher_dims = data.shape[:-1]
+            data = pq.intrinsic._base_transpose(data, perm_map)
+            data = paddle.reshape(data, higher_dims.copy() + [2 ** self.num_qubits])
 
-def _density_to_vector(rho: Union[np.ndarray, paddle.Tensor]) -> Union[np.ndarray, paddle.Tensor]:
-    r""" transform a density matrix to a state vector
-    
-    Args:
-        rho: a density matrix (pure state)
-        
-    Returns:
-        a state vector
-    
-    Raises:
-        ValueError: the output state may not be a pure state
-    
-    """
-    type_str = _type_fetch(rho)
-    rho = paddle.to_tensor(rho)
-    eigval, eigvec = paddle.linalg.eigh(rho)
-            
-    max_eigval = paddle.max(eigval).item()
-    err = np.abs(max_eigval - 1)
-    if err > 1e-6:
-        raise ValueError(
-            f"the output state may not be a pure state, maximum distance: {err}")
-    
-    state = eigvec[:, paddle.argmax(eigval)]
-    
-    return state.numpy() if type_str == "numpy" else state
-    
+        elif self.backend == Backend.DensityMatrix:
+            higher_dims = data.shape[:-2]
+            data = pq.intrinsic._base_transpose_for_dm(data, perm_map)
+            data = paddle.reshape(data, higher_dims.copy() + [2 ** self.num_qubits] * 2)
+        else:
+            raise NotImplementedError
 
-def _type_transform(data: Union[np.ndarray, paddle.Tensor, State],
-                   output_type: str) -> Union[np.ndarray, paddle.Tensor, State]:
-    r""" transform the datatype of ``input`` to ``output_type``
-    
-    Args:
-        data: data to be transformed
-        output_type: datatype of the output data, type is either ``"numpy"``, ``"tensor"``,
-    ``"state_vector"`` or ``"density_matrix"``
-    
-    Returns:
-        the output data with expected type
-        
-    Raises:
-        ValueError: does not support transformation to type.
-    
-    """
-    current_type = _type_fetch(data)
-    
-    support_type = {"numpy", "tensor", "state_vector", "density_matrix"}
-    if output_type not in support_type:
-        raise ValueError(
-            f"does not support transformation to type {output_type}")
-        
-    if current_type == output_type:
-        return data
-    
-    if current_type == "numpy":
-        if output_type == "tensor":
-            return paddle.to_tensor(data)
-        
-        data = np.squeeze(data)        
-        # state_vector case
-        if output_type == "state_vector":
-            if len(data.shape) == 2:
-                data = _density_to_vector(data)
-            return State(data, backend=Backend.StateVector)
-        # density_matrix case
-        if len(data.shape) == 1:
-            data = data.reshape([len(data), 1])
-            data = data @ np.conj(data.T)
-        return State(data, backend=Backend.DensityMatrix)
-    
-    if current_type == "tensor":
-        if output_type == "numpy":
-            return data.numpy()
-        
-        data = paddle.squeeze(data)
-        # state_vector case
-        if output_type == "state_vector":
-            if len(data.shape) == 2:
-                data = _density_to_vector(data)
-            return State(data, backend=Backend.StateVector)
-        
-        # density_matrix case
-        if len(data.shape) == 1:
-            data = data.reshape([len(data), 1])
-            data = data @ paddle.conj(data.T)
-        return State(data, backend=Backend.DensityMatrix)
-
-    if current_type == "state_vector":
-        if output_type == "density_matrix":
-            return State(data.ket @ data.bra, backend=Backend.DensityMatrix, num_qubits=data.num_qubits, override=True)
-        return data.ket.numpy() if output_type == "numpy" else data.ket
-    
-    # density_matrix data
-    if output_type == "state_vector":
-        return State(_density_to_vector(data.data), backend=Backend.StateVector, num_qubits=data.num_qubits, override=True)
-    return data.numpy() if output_type == "numpy" else data.data
+        self.data = data
+        self.qubit_sequence = qubit_sequence
 
+    def reset_sequence(self, target_sequence: Optional[List[int]] = None) -> None: 
+        r"""reset the qubit order to a given sequence
 
-def is_state_vector(vec: Union[np.ndarray, paddle.Tensor], 
-                    eps: Optional[float] = None) -> Tuple[bool, int]:
-    r""" verify whether ``vec`` is a legal quantum state vector
-    
-    Args:
-        vec: state vector candidate :math:`x`
-        eps: tolerance of error, default to be `None` i.e. no testing for data correctness
-    
-    Returns:
-        determine whether :math:`x^\dagger x = 1`, and return the number of qubits or an error message
-        
-    Note:
-        error message is:
-        * ``-1`` if the above equation does not hold
-        * ``-2`` if the dimension of ``vec`` is not a power of 2
-        * ``-3`` if ``vec`` is not a vector
-    
-    """
-    vec = _type_transform(vec, "tensor")
-    vec = paddle.squeeze(vec)
-    
-    dimension = vec.shape[0]
-    if len(vec.shape) != 1:
-        return False, -3
-    
-    num_qubits = int(math.log2(dimension))
-    if 2 ** num_qubits != dimension:
-        return False, -2
-    
-    if eps is None:
-        return True, num_qubits
-    
-    vec = vec.reshape([dimension, 1])
-    vec_bra = paddle.conj(vec.T)   
-    eps = min(eps * dimension, 1e-2)
-    return {False, -1} if paddle.abs(vec_bra @ vec - (1 + 0j)) > eps else {True, num_qubits}
+        Args:
+            target_sequence: target sequence. Defaults to None.
 
+        Returns:
+            State: state with given qubit order
+        """
 
-def is_density_matrix(rho: Union[np.ndarray, paddle.Tensor], 
-                      eps: Optional[float] = None) -> Tuple[bool, int]:
-    r""" verify whether ``rho`` is a legal quantum density matrix
-    
-    Args:
-        rho: density matrix candidate
-        eps: tolerance of error, default to be `None` i.e. no testing for data correctness
-    
-    Returns:
-        determine whether ``rho`` is a PSD matrix with trace 1 and return the number of qubits or an error message.
-    
-    Note:
-        error message is:
-        * ``-1`` if ``rho`` is not PSD
-        * ``-2`` if the trace of ``rho`` is not 1
-        * ``-3`` if the dimension of ``rho`` is not a power of 2 
-        * ``-4`` if ``rho`` is not a square matrix
-    
-    """
-    rho = _type_transform(rho, "tensor")
-    
-    dimension = rho.shape[0]
-    if len(rho.shape) != 2 or dimension != rho.shape[1]:
-        return False, -4
-    
-    num_qubits = int(math.log2(dimension))
-    if 2 ** num_qubits != dimension:
-        return False, -3
-    
-    if eps is None:
-        return True, num_qubits
-    
-    eps = min(eps * dimension, 1e-2)
-    if paddle.abs(paddle.trace(rho) - (1 + 0j)).item() > eps:
-        return False, -2
-    
-    min_eigval = paddle.min(paddle.linalg.eigvalsh(rho))
-    return {False, -1} if paddle.abs(min_eigval) > eps else {True, num_qubits}
+        if target_sequence is None:
+            self.__set_qubit_seq__(list(range(self.num_qubits)))
+        elif target_sequence == self.qubit_sequence:
+            pass
+        else:
+            if len(target_sequence) != self.num_qubits:
+                raise ValueError(f"The length of target sequence does not match! expected {self.num_qubits}, received {len(target_sequence)}")
+            self.__set_qubit_seq__(target_sequence)
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum/trotter.py` & `paddle-quantum-2.4.0/paddle_quantum/trotter.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum/visual.py` & `paddle-quantum-2.4.0/paddle_quantum/visual.py`

 * *Files identical despite different names*

### Comparing `paddle-quantum-2.3.0/paddle_quantum.egg-info/PKG-INFO` & `paddle-quantum-2.4.0/paddle_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: paddle-quantum
-Version: 2.3.0
+Version: 2.4.0
 Summary: Paddle Quantum is a quantum machine learning (QML) toolkit developed based on Baidu PaddlePaddle.
 Home-page: http://qml.baidu.com
 Author: Institute for Quantum Computing, Baidu INC.
 Author-email: qml@baidu.com
 Project-URL: Documentation, https://qml.baidu.com/api/introduction.html
 Project-URL: Source, https://github.com/PaddlePaddle/Quantum/
 Project-URL: Tracker, https://github.com/PaddlePaddle/Quantum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+English | [简体中文](README_CN.md)
+
 # Paddle Quantum (量桨)
 
 - [Features](#features)
 - [Install](#install)
    - [Install PaddlePaddle](#install-paddlepaddle)
    - [Install Paddle Quantum](#install-paddle-quantum)
    - [Environment setup for Quantum Chemistry module](#environment_setup_for_quantum_chemistry_module)
@@ -44,15 +46,15 @@
 <p align="center">
   <!-- docs -->
   <a href="https://qml.baidu.com/api/paddle_quantum.circuit.html">
     <img src="https://img.shields.io/badge/docs-link-green.svg?style=flat-square&logo=read-the-docs"/>
   </a>
   <!-- PyPI -->
   <a href="https://pypi.org/project/paddle-quantum/">
-    <img src="https://img.shields.io/badge/pypi-v2.3.0-orange.svg?style=flat-square&logo=pypi"/>
+    <img src="https://img.shields.io/badge/pypi-v2.4.0-orange.svg?style=flat-square&logo=pypi"/>
   </a>
   <!-- Python -->
   <a href="https://www.python.org/">
     <img src="https://img.shields.io/badge/Python-3.6+-blue.svg?style=flat-square&logo=python"/>
   </a>
   <!-- License -->
   <a href="./LICENSE">
@@ -94,15 +96,15 @@
 
 ```bash
 pip install paddle-quantum
 ```
 or download all the files and finish the installation locally,
 
 ```bash
-git clone http://github.com/PaddlePaddle/quantum
+git clone https://github.com/PaddlePaddle/quantum
 cd quantum
 pip install -e .
 ```
 
 ### Environment setup for Quantum Chemistry module
 
 Currently, our `qchem` module uses `PySCF` as its backend to compute molecular integrals, so before executing quantum chemistry, we have to install this Python package.
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: paddle-quantum Version: 2.3.0 Summary: Paddle
+Metadata-Version: 2.1 Name: paddle-quantum Version: 2.4.0 Summary: Paddle
 Quantum is a quantum machine learning (QML) toolkit developed based on Baidu
 PaddlePaddle. Home-page: http://qml.baidu.com Author: Institute for Quantum
 Computing, Baidu INC. Author-email: qml@baidu.com Project-URL: Documentation,
 https://qml.baidu.com/api/introduction.html Project-URL: Source, https://
 github.com/PaddlePaddle/Quantum/ Project-URL: Tracker, https://github.com/
 PaddlePaddle/Quantum/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6, <4 Description-
-Content-Type: text/markdown License-File: LICENSE # Paddle Quantum (éæ¡¨) -
-[Features](#features) - [Install](#install) - [Install PaddlePaddle](#install-
-paddlepaddle) - [Install Paddle Quantum](#install-paddle-quantum) -
-[Environment setup for Quantum Chemistry module]
-(#environment_setup_for_quantum_chemistry_module) - [Run Example](#run-example)
-- [Introduction and developments](#introduction-and-developments) - [Quick
-start](#quick-start) - [Tutorials](#tutorials) - [API documentation](#api-
-documentation) - [Feedbacks](#feedbacks) - [Research with Paddle Quantum]
+Content-Type: text/markdown License-File: LICENSE English | [ç®ä½ä¸­æ]
+(README_CN.md) # Paddle Quantum (éæ¡¨) - [Features](#features) - [Install]
+(#install) - [Install PaddlePaddle](#install-paddlepaddle) - [Install Paddle
+Quantum](#install-paddle-quantum) - [Environment setup for Quantum Chemistry
+module](#environment_setup_for_quantum_chemistry_module) - [Run Example](#run-
+example) - [Introduction and developments](#introduction-and-developments) -
+[Quick start](#quick-start) - [Tutorials](#tutorials) - [API documentation]
+(#api-documentation) - [Feedbacks](#feedbacks) - [Research with Paddle Quantum]
 (#research-based-on-paddle-quantum) - [Frequently Asked Questions](#frequently-
 asked-questions) - [Copyright and License](#copyright-and-license) -
 [References](#references) [Paddle Quantum (éæ¡¨)](https://qml.baidu.com/) is
 the world's first cloud-integrated quantum machine learning platform based on
 Baidu PaddlePaddle. It supports the building and training of quantum neural
 networks, making PaddlePaddle the first deep learning framework in China.
 Paddle Quantum is feature-rich and easy to use. It provides comprehensive API
 documentation and tutorials help users get started right away.
           [https://release-data.cdn.bcebos.com/Paddle%20Quantum.png]
  [https://img.shields.io/badge/docs-link-green.svg?style=flat-square&logo=read-
-  the-docs]  [https://img.shields.io/badge/pypi-v2.3.0-orange.svg?style=flat-
+  the-docs]  [https://img.shields.io/badge/pypi-v2.4.0-orange.svg?style=flat-
          square&logo=pypi]  [https://img.shields.io/badge/Python-3.6+-
 blue.svg?style=flat-square&logo=python]  [https://img.shields.io/badge/license-
 Apache%202.0-blue.svg?style=flat-square&logo=apache]  [https://img.shields.io/
    badge/OS-MacOS%20|%20Windows%20|%20Linux-lightgrey.svg?style=flat-square]
 Paddle Quantum aims at establishing a bridge between artificial intelligence
 (AI) and quantum computing (QC). It has been utilized for developing several
 quantum machine learning applications. With the PaddlePaddle deep learning
@@ -44,15 +44,15 @@
 information processing - Self-developed QML algorithms ## Install ### Install
 PaddlePaddle This dependency will be automatically satisfied when users install
 Paddle Quantum. Please refer to [PaddlePaddle](https://www.paddlepaddle.org.cn/
 install/quick)'s official installation and configuration page. This project
 requires PaddlePaddle 2.2.0 to 2.3.0. ### Install Paddle Quantum We recommend
 the following way of installing Paddle Quantum with `pip`, ```bash pip install
 paddle-quantum ``` or download all the files and finish the installation
-locally, ```bash git clone http://github.com/PaddlePaddle/quantum cd quantum
+locally, ```bash git clone https://github.com/PaddlePaddle/quantum cd quantum
 pip install -e . ``` ### Environment setup for Quantum Chemistry module
 Currently, our `qchem` module uses `PySCF` as its backend to compute molecular
 integrals, so before executing quantum chemistry, we have to install this
 Python package. > It is recommended that `PySCF` is installed in a Python
 environment whose Python version >=3.6. We highly recommend you to install
 `PySCF` via conda. **MacOS/Linux** user can use the command: ```bash conda
 install -c pyscf pyscf ``` > NOTE: For **Windows** user, if your operating
```

### Comparing `paddle-quantum-2.3.0/paddle_quantum.egg-info/SOURCES.txt` & `paddle-quantum-2.4.0/paddle_quantum.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 paddle_quantum/VQE/example/main.py
 paddle_quantum/VQSD/HGenerator.py
 paddle_quantum/VQSD/Paddle_VQSD.py
 paddle_quantum/VQSD/example/main.py
 paddle_quantum/ansatz/__init__.py
 paddle_quantum/ansatz/circuit.py
 paddle_quantum/ansatz/container.py
+paddle_quantum/ansatz/layer.py
 paddle_quantum/ansatz/vans.py
 paddle_quantum/backend/__init__.py
 paddle_quantum/backend/density_matrix.py
 paddle_quantum/backend/quleaf.py
 paddle_quantum/backend/state_vector.py
 paddle_quantum/backend/unitary_matrix.py
 paddle_quantum/biocomputing/__init__.py
@@ -57,32 +58,32 @@
 paddle_quantum/channel/__init__.py
 paddle_quantum/channel/base.py
 paddle_quantum/channel/common.py
 paddle_quantum/channel/custom.py
 paddle_quantum/channel/representation.py
 paddle_quantum/channel/functional/__init__.py
 paddle_quantum/channel/functional/common.py
+paddle_quantum/data_analysis/power_flow.py
+paddle_quantum/data_analysis/rand_num.py
 paddle_quantum/data_analysis/vqls.py
 paddle_quantum/data_analysis/vqr.py
 paddle_quantum/finance/__init__.py
 paddle_quantum/finance/finance.py
 paddle_quantum/finance/pricing.py
 paddle_quantum/finance/qpo.py
 paddle_quantum/gate/__init__.py
 paddle_quantum/gate/base.py
 paddle_quantum/gate/clifford.py
 paddle_quantum/gate/custom.py
 paddle_quantum/gate/encoding.py
-paddle_quantum/gate/layer.py
+paddle_quantum/gate/matrix.py
 paddle_quantum/gate/multi_qubit_gate.py
 paddle_quantum/gate/single_qubit_gate.py
 paddle_quantum/gate/functional/__init__.py
 paddle_quantum/gate/functional/base.py
-paddle_quantum/gate/functional/multi_qubit_gate.py
-paddle_quantum/gate/functional/single_qubit_gate.py
 paddle_quantum/gate/functional/visual.py
 paddle_quantum/locc/__init__.py
 paddle_quantum/locc/locc_ansatz.py
 paddle_quantum/locc/locc_net.py
 paddle_quantum/locc/locc_party.py
 paddle_quantum/locc/locc_state.py
 paddle_quantum/loss/__init__.py
@@ -170,14 +171,16 @@
 paddle_quantum/qchem/ansatz.py
 paddle_quantum/qchem/drivers.py
 paddle_quantum/qchem/fermionic_state.py
 paddle_quantum/qchem/molecule.py
 paddle_quantum/qchem/properties.py
 paddle_quantum/qchem/utils.py
 paddle_quantum/qml/__init__.py
+paddle_quantum/qml/bert_qtc.py
+paddle_quantum/qml/qcaan.py
 paddle_quantum/qml/qnnmic.py
 paddle_quantum/qml/qnnqd.py
 paddle_quantum/qml/qsann.py
 paddle_quantum/qml/vsql.py
 paddle_quantum/qpp/__init__.py
 paddle_quantum/qpp/angles.py
 paddle_quantum/qpp/laurent.py
```

### Comparing `paddle-quantum-2.3.0/setup.py` & `paddle-quantum-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='paddle-quantum',
-    version='2.3.0',
+    version='2.4.0',
     author='Institute for Quantum Computing, Baidu INC.',
     author_email='qml@baidu.com',
     description='Paddle Quantum is a quantum machine learning (QML) toolkit developed based on Baidu PaddlePaddle.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://qml.baidu.com',
     packages=[
@@ -90,14 +90,15 @@
         'qcompute',
         'networkx>=2.5',
         'matplotlib>=3.3.0',
         'scipy',
         'tqdm',
         'openfermion',
         'pyscf; platform_system == "Linux" or platform_system == "Darwin"',
+        'paddlenlp',
         'opencv-python',
         'scikit-learn',
         'fastdtw',
         'cvxpy',
         'rich',
         'imbalanced-learn',
     ],
```

