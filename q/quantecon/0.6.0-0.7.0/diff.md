# Comparing `tmp/quantecon-0.6.0.tar.gz` & `tmp/quantecon-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantecon-0.6.0.tar", last modified: Sun Dec 18 00:58:25 2022, max compression
+gzip compressed data, was "quantecon-0.7.0.tar", last modified: Mon Apr 24 09:24:58 2023, max compression
```

## Comparing `quantecon-0.6.0.tar` & `quantecon-0.7.0.tar`

### file list

```diff
@@ -1,129 +1,131 @@
--rw-r--r--   0        0        0    23006 2022-12-18 00:58:21.375725 quantecon-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1540 2022-12-18 00:58:21.375725 quantecon-0.6.0/LICENSE
--rw-r--r--   0        0        0       79 2022-12-18 00:58:21.375725 quantecon-0.6.0/MANIFEST.in
--rw-r--r--   0        0        0     3016 2022-12-18 00:58:21.375725 quantecon-0.6.0/README.md
--rw-r--r--   0        0        0     1477 2022-12-18 00:58:21.375725 quantecon-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       81 2022-12-18 00:58:21.375725 quantecon-0.6.0/pytest.ini
--rw-r--r--   0        0        0     1951 2022-12-18 00:58:21.375725 quantecon-0.6.0/quantecon/__init__.py
--rw-r--r--   0        0        0     8070 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_arma.py
--rw-r--r--   0        0        0     3142 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_ce_util.py
--rw-r--r--   0        0        0    11809 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_compute_fp.py
--rw-r--r--   0        0        0     1940 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_discrete_rv.py
--rw-r--r--   0        0        0    13901 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_dle.py
--rw-r--r--   0        0        0     1121 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_ecdf.py
--rw-r--r--   0        0        0     4820 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_estspec.py
--rw-r--r--   0        0        0     1682 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_filter.py
--rw-r--r--   0        0        0    13594 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_graph_tools.py
--rw-r--r--   0        0        0    10926 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_gridtools.py
--rw-r--r--   0        0        0     3700 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_inequality.py
--rw-r--r--   0        0        0     8993 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_ivp.py
--rw-r--r--   0        0        0     9604 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_kalman.py
--rw-r--r--   0        0        0     2066 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_lae.py
--rw-r--r--   0        0        0    21811 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_lqcontrol.py
--rw-r--r--   0        0        0     5224 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_lqnash.py
--rw-r--r--   0        0        0    15141 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_lss.py
--rw-r--r--   0        0        0    10492 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_matrix_eqn.py
--rw-r--r--   0        0        0     2802 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_quadsums.py
--rw-r--r--   0        0        0     2965 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_rank_nullspace.py
--rw-r--r--   0        0        0    12504 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/_robustlq.py
--rw-r--r--   0        0        0      743 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/arma.py
--rw-r--r--   0        0        0      236 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/bld.bat
--rw-r--r--   0        0        0      219 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/build.sh
--rw-r--r--   0        0        0      808 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/ce_util.py
--rw-r--r--   0        0        0      822 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/compute_fp.py
--rw-r--r--   0        0        0      817 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/discrete_rv.py
--rw-r--r--   0        0        0     3164 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/distributions.py
--rw-r--r--   0        0        0      757 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/dle.py
--rw-r--r--   0        0        0      762 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/ecdf.py
--rw-r--r--   0        0        0      809 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/estspec.py
--rw-r--r--   0        0        0      781 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/filter.py
--rw-r--r--   0        0        0      881 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/__init__.py
--rw-r--r--   0        0        0     7676 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/brd.py
--rw-r--r--   0        0        0     7225 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/fictplay.py
--rw-r--r--   0        0        0       87 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/game_generators/__init__.py
--rw-r--r--   0        0        0    23553 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/game_generators/bimatrix_generators.py
--rw-r--r--   0        0        0        0 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/game_generators/tests/__init__.py
--rw-r--r--   0        0        0     5706 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/game_generators/tests/test_bimatrix_generators.py
--rw-r--r--   0        0        0    15471 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/lemke_howson.py
--rw-r--r--   0        0        0     7506 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/localint.py
--rw-r--r--   0        0        0     5214 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/logitdyn.py
--rw-r--r--   0        0        0     9187 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/mclennan_tourky.py
--rw-r--r--   0        0        0    32150 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/normal_form_game.py
--rw-r--r--   0        0        0     1740 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/pure_nash.py
--rw-r--r--   0        0        0     6000 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/random.py
--rw-r--r--   0        0        0    14180 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/repeated_game.py
--rw-r--r--   0        0        0     5562 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/support_enumeration.py
--rw-r--r--   0        0        0        0 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/__init__.py
--rw-r--r--   0        0        0     2072 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_brd.py
--rw-r--r--   0        0        0     3819 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_fictplay.py
--rw-r--r--   0        0        0     4625 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_lemke_howson.py
--rw-r--r--   0        0        0     1995 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_localint.py
--rw-r--r--   0        0        0     1854 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_logitdyn.py
--rw-r--r--   0        0        0     4993 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_mclennan_tourky.py
--rw-r--r--   0        0        0    18048 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_normal_form_game.py
--rw-r--r--   0        0        0     2231 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_pure_nash.py
--rw-r--r--   0        0        0     2890 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_random.py
--rw-r--r--   0        0        0     1829 2022-12-18 00:58:21.379725 quantecon-0.6.0/quantecon/game_theory/tests/test_repeated_game.py
--rw-r--r--   0        0        0     2403 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/game_theory/tests/test_support_enumeration.py
--rw-r--r--   0        0        0     1292 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/game_theory/tests/test_utilities.py
--rw-r--r--   0        0        0     4751 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/game_theory/tests/test_vertex_enumeration.py
--rw-r--r--   0        0        0     2148 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/game_theory/utilities.py
--rw-r--r--   0        0        0    11232 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/game_theory/vertex_enumeration.py
--rw-r--r--   0        0        0      837 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/graph_tools.py
--rw-r--r--   0        0        0      887 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/gridtools.py
--rw-r--r--   0        0        0      845 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/inequality.py
--rw-r--r--   0        0        0      756 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/ivp.py
--rw-r--r--   0        0        0      771 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/kalman.py
--rw-r--r--   0        0        0      756 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/lae.py
--rw-r--r--   0        0        0      792 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/lqcontrol.py
--rw-r--r--   0        0        0      770 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/lqnash.py
--rw-r--r--   0        0        0      758 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/lss.py
--rw-r--r--   0        0        0      452 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/__init__.py
--rw-r--r--   0        0        0     5267 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/_ddp_linprog_simplex.py
--rw-r--r--   0        0        0     6754 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/approximation.py
--rw-r--r--   0        0        0    25386 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/core.py
--rw-r--r--   0        0        0    35365 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/ddp.py
--rw-r--r--   0        0        0     1847 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/estimate.py
--rw-r--r--   0        0        0     4312 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/gth_solve.py
--rw-r--r--   0        0        0     6660 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/random.py
--rw-r--r--   0        0        0        0 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/tests/__init__.py
--rw-r--r--   0        0        0     3117 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/tests/test_approximation.py
--rw-r--r--   0        0        0    19619 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/tests/test_core.py
--rw-r--r--   0        0        0    11341 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/tests/test_ddp.py
--rw-r--r--   0        0        0     2044 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/tests/test_estimate.py
--rw-r--r--   0        0        0     5792 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/tests/test_gth_solve.py
--rw-r--r--   0        0        0     4804 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/tests/test_random.py
--rw-r--r--   0        0        0      471 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/tests/test_utilities.py
--rw-r--r--   0        0        0     3553 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/markov/utilities.py
--rw-r--r--   0        0        0      874 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/matrix_eqn.py
--rw-r--r--   0        0        0     1438 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/meta.yaml
--rw-r--r--   0        0        0      345 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/__init__.py
--rw-r--r--   0        0        0    14315 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/linprog_simplex.py
--rw-r--r--   0        0        0     2591 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/minmax.py
--rw-r--r--   0        0        0    14379 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/nelder_mead.py
--rw-r--r--   0        0        0     4892 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/pivoting.py
--rw-r--r--   0        0        0    15046 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/root_finding.py
--rw-r--r--   0        0        0     4066 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/scalar_maximization.py
--rw-r--r--   0        0        0        0 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/tests/__init__.py
--rw-r--r--   0        0        0    10405 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/tests/test_linprog_simplex.py
--rw-r--r--   0        0        0     1082 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/tests/test_minmax.py
--rw-r--r--   0        0        0     9891 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/tests/test_nelder_mead.py
--rw-r--r--   0        0        0     2763 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/tests/test_root_finding.py
--rw-r--r--   0        0        0     1263 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/optimize/tests/test_scalar_max.py
--rw-r--r--   0        0        0    31716 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/quad.py
--rw-r--r--   0        0        0      809 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/quadsums.py
--rw-r--r--   0        0        0      298 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/random/__init__.py
--rw-r--r--   0        0        0        0 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/random/tests/__init__.py
--rw-r--r--   0        0        0     2502 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/random/tests/test_utilities.py
--rw-r--r--   0        0        0     5923 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/random/utilities.py
--rw-r--r--   0        0        0      814 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/rank_nullspace.py
--rw-r--r--   0        0        0      777 2022-12-18 00:58:21.383725 quantecon-0.6.0/quantecon/robustlq.py
--rw-r--r--   0        0        0      228 2022-12-18 00:58:21.387725 quantecon-0.6.0/quantecon/util/__init__.py
--rw-r--r--   0        0        0     1223 2022-12-18 00:58:21.387725 quantecon-0.6.0/quantecon/util/array.py
--rw-r--r--   0        0        0     2723 2022-12-18 00:58:21.387725 quantecon-0.6.0/quantecon/util/combinatorics.py
--rw-r--r--   0        0        0      481 2022-12-18 00:58:21.387725 quantecon-0.6.0/quantecon/util/common_messages.py
--rw-r--r--   0        0        0     3849 2022-12-18 00:58:21.387725 quantecon-0.6.0/quantecon/util/notebooks.py
--rw-r--r--   0        0        0     2864 2022-12-18 00:58:21.387725 quantecon-0.6.0/quantecon/util/numba.py
--rw-r--r--   0        0        0     1257 2022-12-18 00:58:21.387725 quantecon-0.6.0/quantecon/util/random.py
--rw-r--r--   0        0        0     5239 2022-12-18 00:58:21.387725 quantecon-0.6.0/quantecon/util/timing.py
--rw-r--r--   0        0        0     4391 1970-01-01 00:00:00.000000 quantecon-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    24921 2023-04-24 09:24:51.390751 quantecon-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1540 2023-04-24 09:24:51.390751 quantecon-0.7.0/LICENSE
+-rw-r--r--   0        0        0       79 2023-04-24 09:24:51.390751 quantecon-0.7.0/MANIFEST.in
+-rw-r--r--   0        0        0     2667 2023-04-24 09:24:51.390751 quantecon-0.7.0/README.md
+-rw-r--r--   0        0        0     1485 2023-04-24 09:24:51.390751 quantecon-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       81 2023-04-24 09:24:51.390751 quantecon-0.7.0/pytest.ini
+-rw-r--r--   0        0        0     1865 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/__init__.py
+-rw-r--r--   0        0        0     8070 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_arma.py
+-rw-r--r--   0        0        0     3142 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_ce_util.py
+-rw-r--r--   0        0        0    11894 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_compute_fp.py
+-rw-r--r--   0        0        0     1940 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_discrete_rv.py
+-rw-r--r--   0        0        0    13901 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_dle.py
+-rw-r--r--   0        0        0     1121 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_ecdf.py
+-rw-r--r--   0        0        0     4820 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_estspec.py
+-rw-r--r--   0        0        0     1682 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_filter.py
+-rw-r--r--   0        0        0    13594 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_graph_tools.py
+-rw-r--r--   0        0        0    10926 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_gridtools.py
+-rw-r--r--   0        0        0     3701 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_inequality.py
+-rw-r--r--   0        0        0     8993 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_ivp.py
+-rw-r--r--   0        0        0     9604 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_kalman.py
+-rw-r--r--   0        0        0     2066 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_lae.py
+-rw-r--r--   0        0        0    21811 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_lqcontrol.py
+-rw-r--r--   0        0        0     5224 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_lqnash.py
+-rw-r--r--   0        0        0    15079 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_lss.py
+-rw-r--r--   0        0        0    10492 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_matrix_eqn.py
+-rw-r--r--   0        0        0     2802 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_quadsums.py
+-rw-r--r--   0        0        0     2965 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_rank_nullspace.py
+-rw-r--r--   0        0        0    12504 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_robustlq.py
+-rw-r--r--   0        0        0      743 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/arma.py
+-rw-r--r--   0        0        0      236 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/bld.bat
+-rw-r--r--   0        0        0      219 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/build.sh
+-rw-r--r--   0        0        0      808 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/ce_util.py
+-rw-r--r--   0        0        0      822 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/compute_fp.py
+-rw-r--r--   0        0        0      817 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/discrete_rv.py
+-rw-r--r--   0        0        0     3164 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/distributions.py
+-rw-r--r--   0        0        0      757 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/dle.py
+-rw-r--r--   0        0        0      762 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/ecdf.py
+-rw-r--r--   0        0        0      809 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/estspec.py
+-rw-r--r--   0        0        0      781 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/filter.py
+-rw-r--r--   0        0        0      881 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/__init__.py
+-rw-r--r--   0        0        0     7676 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/brd.py
+-rw-r--r--   0        0        0     7225 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/fictplay.py
+-rw-r--r--   0        0        0       87 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/game_generators/__init__.py
+-rw-r--r--   0        0        0    23553 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/game_generators/bimatrix_generators.py
+-rw-r--r--   0        0        0        0 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/game_generators/tests/__init__.py
+-rw-r--r--   0        0        0     5706 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/game_generators/tests/test_bimatrix_generators.py
+-rw-r--r--   0        0        0    15486 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/lemke_howson.py
+-rw-r--r--   0        0        0     7502 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/localint.py
+-rw-r--r--   0        0        0     5214 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/logitdyn.py
+-rw-r--r--   0        0        0     9194 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/mclennan_tourky.py
+-rw-r--r--   0        0        0    32142 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/normal_form_game.py
+-rw-r--r--   0        0        0     1740 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/pure_nash.py
+-rw-r--r--   0        0        0     6000 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/random.py
+-rw-r--r--   0        0        0    14180 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/repeated_game.py
+-rw-r--r--   0        0        0     5561 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/support_enumeration.py
+-rw-r--r--   0        0        0        0 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_brd.py
+-rw-r--r--   0        0        0     3819 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_fictplay.py
+-rw-r--r--   0        0        0     4625 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_lemke_howson.py
+-rw-r--r--   0        0        0     1995 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_localint.py
+-rw-r--r--   0        0        0     1854 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_logitdyn.py
+-rw-r--r--   0        0        0     4993 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_mclennan_tourky.py
+-rw-r--r--   0        0        0    18048 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_normal_form_game.py
+-rw-r--r--   0        0        0     2231 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_pure_nash.py
+-rw-r--r--   0        0        0     2890 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_random.py
+-rw-r--r--   0        0        0     1829 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_repeated_game.py
+-rw-r--r--   0        0        0     2403 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_support_enumeration.py
+-rw-r--r--   0        0        0     1292 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_utilities.py
+-rw-r--r--   0        0        0     4751 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_vertex_enumeration.py
+-rw-r--r--   0        0        0     2148 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/utilities.py
+-rw-r--r--   0        0        0    11232 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/vertex_enumeration.py
+-rw-r--r--   0        0        0      837 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/graph_tools.py
+-rw-r--r--   0        0        0      914 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/gridtools.py
+-rw-r--r--   0        0        0      845 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/inequality.py
+-rw-r--r--   0        0        0      756 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/ivp.py
+-rw-r--r--   0        0        0      771 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/kalman.py
+-rw-r--r--   0        0        0      756 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/lae.py
+-rw-r--r--   0        0        0      792 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/lqcontrol.py
+-rw-r--r--   0        0        0      770 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/lqnash.py
+-rw-r--r--   0        0        0      794 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/lss.py
+-rw-r--r--   0        0        0      483 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/markov/__init__.py
+-rw-r--r--   0        0        0     5267 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/markov/_ddp_linprog_simplex.py
+-rw-r--r--   0        0        0    14449 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/markov/approximation.py
+-rw-r--r--   0        0        0    25355 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/markov/core.py
+-rw-r--r--   0        0        0    35365 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/ddp.py
+-rw-r--r--   0        0        0     3315 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/estimate.py
+-rw-r--r--   0        0        0     4312 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/gth_solve.py
+-rw-r--r--   0        0        0     6660 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/random.py
+-rw-r--r--   0        0        0        0 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/__init__.py
+-rw-r--r--   0        0        0     8533 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_approximation.py
+-rw-r--r--   0        0        0    19897 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_core.py
+-rw-r--r--   0        0        0    11341 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_ddp.py
+-rw-r--r--   0        0        0     3333 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_estimate.py
+-rw-r--r--   0        0        0     5792 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_gth_solve.py
+-rw-r--r--   0        0        0     4804 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_random.py
+-rw-r--r--   0        0        0      471 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_utilities.py
+-rw-r--r--   0        0        0     3553 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/utilities.py
+-rw-r--r--   0        0        0      874 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/matrix_eqn.py
+-rw-r--r--   0        0        0     1438 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/meta.yaml
+-rw-r--r--   0        0        0      378 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/__init__.py
+-rw-r--r--   0        0        0     7357 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/lcp_lemke.py
+-rw-r--r--   0        0        0    14318 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/linprog_simplex.py
+-rw-r--r--   0        0        0     2591 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/minmax.py
+-rw-r--r--   0        0        0    14379 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/nelder_mead.py
+-rw-r--r--   0        0        0     4892 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/pivoting.py
+-rw-r--r--   0        0        0    15046 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/root_finding.py
+-rw-r--r--   0        0        0     4066 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/scalar_maximization.py
+-rw-r--r--   0        0        0        0 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/__init__.py
+-rw-r--r--   0        0        0     3218 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_lcp_lemke.py
+-rw-r--r--   0        0        0    10405 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_linprog_simplex.py
+-rw-r--r--   0        0        0     1082 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_minmax.py
+-rw-r--r--   0        0        0     9891 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_nelder_mead.py
+-rw-r--r--   0        0        0     2763 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_root_finding.py
+-rw-r--r--   0        0        0     1263 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_scalar_max.py
+-rw-r--r--   0        0        0    31716 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/quad.py
+-rw-r--r--   0        0        0      809 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/quadsums.py
+-rw-r--r--   0        0        0      298 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/random/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/random/tests/__init__.py
+-rw-r--r--   0        0        0     2876 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/random/tests/test_utilities.py
+-rw-r--r--   0        0        0     6368 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/random/utilities.py
+-rw-r--r--   0        0        0      814 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/rank_nullspace.py
+-rw-r--r--   0        0        0      777 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/robustlq.py
+-rw-r--r--   0        0        0      228 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/__init__.py
+-rw-r--r--   0        0        0     1223 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/array.py
+-rw-r--r--   0        0        0     2723 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/combinatorics.py
+-rw-r--r--   0        0        0      481 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/common_messages.py
+-rw-r--r--   0        0        0     3849 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/notebooks.py
+-rw-r--r--   0        0        0     2883 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/numba.py
+-rw-r--r--   0        0        0     1257 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/random.py
+-rw-r--r--   0        0        0     5239 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/timing.py
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 quantecon-0.7.0/PKG-INFO
```

### Comparing `quantecon-0.6.0/CHANGELOG.md` & `quantecon-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,33 @@
 # Changelog
 
+## Ver 0.7.0 (24-February-2023)
+
+### New
+
+1. [END: Add function fit_discrete_mc](https://github.com/QuantEcon/QuantEcon.py/pull/681) ([jstac](https://github.com/jstac)), ([Smit-create](https://github.com/Smit-create)) and ([oyamad](https://github.com/oyamad)) which takes a time series and fits a finite markov chain
+2. [ENH: Adding Discrete Approximation of VAR Methods](https://github.com/QuantEcon/QuantEcon.py/pull/640) ([crondonm](https://github.com/crondonm)) 
+3. [ENH: Implement LCP solver](https://github.com/QuantEcon/QuantEcon.py/pull/690) ([oyamad](https://github.com/oyamad))
+
+### Fixes and Maintenance
+
+1. [FIX: Fix period of reducible MarkovChain with custom state_values](https://github.com/QuantEcon/QuantEcon.py/pull/684) ([oyamad](https://github.com/oyamad))
+
+There were a range of additional maitenance and fixes including
+[RFC: Replace `@generated_jit` with `@overload`](https://github.com/QuantEcon/QuantEcon.py/pull/701),
+[Update __Iss.py - Remove broken link](https://github.com/QuantEcon/QuantEcon.py/pull/692),
+[FIX: Add `__dir__` to lss.py](https://github.com/QuantEcon/QuantEcon.py/pull/693),
+[MAINT: Rename ivy.py to ivp.py](https://github.com/QuantEcon/QuantEcon.py/pull/689),
+[Bring estimate_mc into top level namespace](https://github.com/QuantEcon/QuantEcon.py/pull/688),
+[Warn only when n in not int in tauchen](https://github.com/QuantEcon/QuantEcon.py/pull/673),
+[FIX: Avoid bare 'except'](https://github.com/QuantEcon/QuantEcon.py/pull/686),
+[FIX: DOC: Remove 2-byte spaces](https://github.com/QuantEcon/QuantEcon.py/pull/685)
+
+Thank you to ([bensonarafat](https://github.com/bensonarafat)), ([crondonm](https://github.com/crondonm)), ([oyamad](https://github.com/oyamad)), ([jstac](https://github.com/jstac)), and ([Smit-create](https://github.com/Smit-create)) for all your contributions, PR reviews, and comments. 
+
 ## Ver 0.6.0 (18-December-2022)
 
 This is the next major release of the `quantecon` package as it includes some **breaking changes** as listed below. It also
 includes a number of new features and enhancements including learning algorithms in the game theory module, MLE estimation
 for Markov Chains, in addition to some useful helper functions. 
 
 [PR #601: Updates to public and private API](https://github.com/QuantEcon/QuantEcon.py/pull/601) 
@@ -15,26 +39,26 @@
 1. [MAINT: Unify tauchen and rouwenhorst API](https://github.com/QuantEcon/QuantEcon.py/pull/664) ([Smit-create](https://github.com/Smit-create))
 
 ### New
 
 1. [ENH: Add MLE Estimation for Markov Chains](https://github.com/QuantEcon/QuantEcon.py/pull/658) ([jstac](https://github.com/jstac))
 2. [ENH: Implement cartesian_nearest_index](https://github.com/QuantEcon/QuantEcon.py/pull/660) ([oyamad](https://github.com/oyamad))
 3. [ENH: check_random_state: Accept np.random.Generator](https://github.com/QuantEcon/QuantEcon.py/pull/654) ([oyamad](https://github.com/oyamad))
-4. [ENH: Add learning algorithms to Game Theory module](https://github.com/QuantEcon/QuantEcon.py/pull/487) ([Yuya-Furusawa](https://github.com/oyamad)
+4. [ENH: Add learning algorithms to Game Theory module](https://github.com/QuantEcon/QuantEcon.py/pull/487) ([Yuya-Furusawa](https://github.com/Yuya-Furusawa))
 
 ### Fixes
 
 1. [FIX: Fix dtype in cartesian](https://github.com/QuantEcon/QuantEcon.py/pull/659) ([oyamad](https://github.com/oyamad))
 2. [FIX: Bugfix in brd.py](https://github.com/QuantEcon/QuantEcon.py/pull/657) ([oyamad](https://github.com/oyamad))
 3. [MAINT: player.is_dominated: Allow recent methods for scipy.optimize.linprog](https://github.com/QuantEcon/QuantEcon.py/pull/648) ([oyamad](https://github.com/oyamad))
 4. [MAINT: Distinguish between private and public namespaces](https://github.com/QuantEcon/QuantEcon.py/pull/601) ([Smit-create](https://github.com/Smit-create)).
 5. [MAINT: Clairfy hamilton_filter API](https://github.com/QuantEcon/QuantEcon.py/pull/634) ([rht](https://github.com/rht))
 
-Thank you to ([oyamad](https://github.com/oyamad)), ([jstac](https://github.com/jstac)), ([Smit-create](https://github.com/Smit-create)), 
-and ([rht](https://github.com/rht)) for all your contributions, PR reviews, and comments. 
+Thank you to ([oyamad](https://github.com/oyamad)), ([jstac](https://github.com/jstac)), ([Smit-create](https://github.com/Smit-create)),
+([rht](https://github.com/rht)), and ([Yuya-Furusawa](https://github.com/Yuya-Furusawa)) for all your contributions, PR reviews, and comments. 
 
 ## Ver 0.5.3 (07-April-2022)
 
 This is primarily a maintenance release to fix a number of deprecation notices, migrating the tests to use `pytest` rather than `nose`,  and python packaging is moving to `flit`
 
 **Enhancement:**
```

### Comparing `quantecon-0.6.0/LICENSE` & `quantecon-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/README.md` & `quantecon-0.7.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 
 ```python
   from quantecon.markov import DiscreteDP
   aiyagari_ddp = DiscreteDP(R, Q, beta)
   results = aiyagari_ddp.solve(method='policy_iteration')
 ```
 
-[![Build Status](https://github.com/QuantEcon/QuantEcon.py/workflows/build/badge.svg)](https://github.com/QuantEcon/QuantEcon.py/actions?query=workflow%3Abuild)
+[![Build Status](https://github.com/QuantEcon/QuantEcon.py/actions/workflows/ci.yml/badge.svg)](https://github.com/QuantEcon/QuantEcon.py/actions?query=workflow%3Abuild)
 [![Coverage Status](https://coveralls.io/repos/QuantEcon/QuantEcon.py/badge.svg)](https://coveralls.io/r/QuantEcon/QuantEcon.py)
-[![Code Quality: Python](https://img.shields.io/lgtm/grade/python/g/QuantEcon/QuantEcon.py.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/QuantEcon/QuantEcon.py/context:python)
-[![Total Alerts](https://img.shields.io/lgtm/alerts/g/QuantEcon/QuantEcon.py.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/QuantEcon/QuantEcon.py/alerts)
 [![Documentation Status](https://readthedocs.org/projects/quanteconpy/badge/?version=latest)](https://quanteconpy.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 Before installing `quantecon` we recommend you install the [Anaconda](https://www.anaconda.com/download/) Python distribution, which includes a full suite of scientific python tools. **Note:** `quantecon` is now only supporting Python version 3.5+. This is mainly to allow code to be written taking full advantage of new features such as using the `@` symbol for matrix multiplication. Therefore please install the latest Python 3 Anaconda distribution.
 
 Next you can install quantecon by opening a terminal prompt and typing
@@ -40,19 +38,18 @@
 
     pip install --upgrade quantecon
 
 ## Examples and Sample Code
 
 Many examples of QuantEcon.py in action can be found at [Quantitative Economics](https://lectures.quantecon.org/). See also the
 
-*   [Documentation](http://quanteconpy.readthedocs.org/en/latest/)
-*   [Notebook gallery](/notebooks)
-*   [Additional Examples](/python-examples)
+*   [Documentation](https://quanteconpy.readthedocs.org/en/latest/)
+*   [Notebook gallery](https://notes.quantecon.org)
 
-QuantEcon.py is supported financially by the [Alfred P. Sloan Foundation](http://www.sloan.org/) and is part of the [QuantEcon organization](/).
+QuantEcon.py is supported financially by the [Alfred P. Sloan Foundation](http://www.sloan.org/) and is part of the [QuantEcon organization](https://quantecon.org).
 
 ## Downloading the `quantecon` Repository
 
 An alternative is to download the sourcecode of the `quantecon` package and install it manually from [the github repository](https://github.com/QuantEcon/QuantEcon.py/). For example, if you have git installed type
 
     git clone https://github.com/QuantEcon/QuantEcon.py
```

### Comparing `quantecon-0.6.0/pyproject.toml` & `quantecon-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 keywords = [
     'quantitative', 
     'economics'
 ]
 dynamic = ["description", "version"]
 requires-python = ">=3.7"
 dependencies = [
-    'numba',
+    'numba>=0.49.0',
     'numpy>=1.17.0',
     'requests',
     'scipy>=1.5.0',
     'sympy',
 ]
 
 [project.optional-dependencies]
```

### Comparing `quantecon-0.6.0/quantecon/_arma.py` & `quantecon-0.7.0/quantecon/_arma.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_ce_util.py` & `quantecon-0.7.0/quantecon/_ce_util.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_compute_fp.py` & `quantecon-0.7.0/quantecon/_compute_fp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 Compute an approximate fixed point of a given operator T, starting from
 specified initial condition v.
 
 """
 import time
 import warnings
 import numpy as np
-from numba import jit, generated_jit, types
+from numba import jit, types
+from numba.extending import overload
 from .game_theory.lemke_howson import _lemke_howson_tbl, _get_mixed_actions
 
 
 def _print_after_skip(skip, it=None, dist=None, etime=None):
     if it is None:
         # print initial header
         msg = "{i:<13}{d:<15}{t:<17}".format(i="Iteration",
@@ -348,16 +349,20 @@
     for pl, start in enumerate([m, 0]):
         for i in range(m):
             bases[pl][i] = start + i
 
     return tableaux, bases
 
 
-@generated_jit(nopython=True, cache=True)
-def _square_sum(a):
+def _square_sum(a):  # pragma: no cover
+    pass
+
+
+@overload(_square_sum, jit_options={'cache':True})
+def _square_sum_ol(a):
     if isinstance(a, types.Number):
         return lambda a: a**2
     elif isinstance(a, types.Array):
         return _square_sum_array
 
 
 def _square_sum_array(a):  # pragma: no cover
```

### Comparing `quantecon-0.6.0/quantecon/_discrete_rv.py` & `quantecon-0.7.0/quantecon/_discrete_rv.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_dle.py` & `quantecon-0.7.0/quantecon/_dle.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_ecdf.py` & `quantecon-0.7.0/quantecon/_ecdf.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_estspec.py` & `quantecon-0.7.0/quantecon/_estspec.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_filter.py` & `quantecon-0.7.0/quantecon/_filter.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_graph_tools.py` & `quantecon-0.7.0/quantecon/_graph_tools.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_gridtools.py` & `quantecon-0.7.0/quantecon/_gridtools.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_inequality.py` & `quantecon-0.7.0/quantecon/_inequality.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,7 +146,8 @@
         Size data for top (c x 100)% of the observations
     """
     w = - np.sort(- data)                  # Reverse sort
     w = w[:int(len(w) * c)]                # extract top (c * 100)%
     rank_data = np.arange(len(w)) + 1
     size_data = w
     return rank_data, size_data
+
```

### Comparing `quantecon-0.6.0/quantecon/_ivp.py` & `quantecon-0.7.0/quantecon/_ivp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_kalman.py` & `quantecon-0.7.0/quantecon/_kalman.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_lae.py` & `quantecon-0.7.0/quantecon/_lae.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_lqcontrol.py` & `quantecon-0.7.0/quantecon/_lqcontrol.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_lqnash.py` & `quantecon-0.7.0/quantecon/_lqnash.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_lss.py` & `quantecon-0.7.0/quantecon/_lss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 """
 Computes quantities associated with the Gaussian linear state space model.
 
-References
-----------
-
-https://lectures.quantecon.org/py/linear_models.html
-
 """
 
 from textwrap import dedent
 import numpy as np
 from scipy.linalg import solve
 from ._matrix_eqn import solve_discrete_lyapunov
 from numba import jit
 from .util import check_random_state
 
 
-@jit
+@jit(nopython=True)
 def simulate_linear_model(A, x0, v, ts_length):
     r"""
     This is a separate function for simulating a vector linear system of
     the form
 
     .. math::
```

### Comparing `quantecon-0.6.0/quantecon/_matrix_eqn.py` & `quantecon-0.7.0/quantecon/_matrix_eqn.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_quadsums.py` & `quantecon-0.7.0/quantecon/_quadsums.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_rank_nullspace.py` & `quantecon-0.7.0/quantecon/_rank_nullspace.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/_robustlq.py` & `quantecon-0.7.0/quantecon/_robustlq.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/arma.py` & `quantecon-0.7.0/quantecon/arma.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/ce_util.py` & `quantecon-0.7.0/quantecon/ce_util.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/compute_fp.py` & `quantecon-0.7.0/quantecon/compute_fp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/discrete_rv.py` & `quantecon-0.7.0/quantecon/discrete_rv.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/distributions.py` & `quantecon-0.7.0/quantecon/distributions.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/dle.py` & `quantecon-0.7.0/quantecon/dle.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/ecdf.py` & `quantecon-0.7.0/quantecon/ecdf.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/estspec.py` & `quantecon-0.7.0/quantecon/estspec.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/filter.py` & `quantecon-0.7.0/quantecon/filter.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/__init__.py` & `quantecon-0.7.0/quantecon/game_theory/__init__.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/brd.py` & `quantecon-0.7.0/quantecon/game_theory/brd.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/fictplay.py` & `quantecon-0.7.0/quantecon/game_theory/fictplay.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/game_generators/bimatrix_generators.py` & `quantecon-0.7.0/quantecon/game_theory/game_generators/bimatrix_generators.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/game_generators/tests/test_bimatrix_generators.py` & `quantecon-0.7.0/quantecon/game_theory/game_generators/tests/test_bimatrix_generators.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/lemke_howson.py` & `quantecon-0.7.0/quantecon/game_theory/lemke_howson.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
        in Strategic and Extensive Form," Chapter 3, N. Nisan, T.
        Roughgarden, E. Tardos, and V. Vazirani eds., Algorithmic Game
        Theory, 2007.
 
     """
     try:
         N = g.N
-    except:
+    except AttributeError:
         raise TypeError('g must be a 2-player NormalFormGame')
     if N != 2:
         raise NotImplementedError('Implemented only for 2-player games')
 
     payoff_matrices = g.payoff_arrays
     nums_actions = g.nums_actions
     total_num = sum(nums_actions)
```

### Comparing `quantecon-0.6.0/quantecon/game_theory/localint.py` & `quantecon-0.7.0/quantecon/game_theory/localint.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 class LocalInteraction:
     """
     Class representing the local interaction model.
 
     Parameters
     ----------
     payoff_matrix : array_like(float, ndim=2)
-        The payoff matrix of the symmetric two-player game played in　each
+        The payoff matrix of the symmetric two-player game played in each
         interaction.
 
     adj_matrix : array_like(float, ndim=2)
-        The adjacency matrix of the network. Non constant weights and　asymmetry
+        The adjacency matrix of the network. Non constant weights and asymmetry
         in interactions are allowed.
 
     Attributes
     ----------
     players : list(Player)
         The list consisting of all players with the given payoff matrix.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `quantecon-0.6.0/quantecon/game_theory/logitdyn.py` & `quantecon-0.7.0/quantecon/game_theory/logitdyn.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/mclennan_tourky.py` & `quantecon-0.7.0/quantecon/game_theory/mclennan_tourky.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Compute mixed Nash equilibria of an N-player normal form game by
 applying the imitation game algorithm by McLennan and Tourky to the best
 response correspondence.
 
 """
 import numbers
 import numpy as np
-from quantecon._compute_fp import _compute_fixed_point_ig
+from .._compute_fp import _compute_fixed_point_ig
 from .normal_form_game import pure2mixed
 from .utilities import NashResult
 
 
 def mclennan_tourky(g, init=None, epsilon=1e-3, max_iter=200,
                     full_output=False):
     r"""
@@ -102,15 +102,15 @@
     ----------
     .. [1] A. McLennan and R. Tourky, "From Imitation Games to
        Kakutani," 2006.
 
     """
     try:
         N = g.N
-    except:
+    except AttributeError:
         raise TypeError('g must be a NormalFormGame')
     if N < 2:
         raise NotImplementedError('Not implemented for 1-player games')
 
     if init is None:
         init = (0,) * N
     try:
```

### Comparing `quantecon-0.6.0/quantecon/game_theory/normal_form_game.py` & `quantecon-0.7.0/quantecon/game_theory/normal_form_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 """
 import re
 import numbers
 import numpy as np
 from numba import jit
 
-from quantecon.util import check_random_state, rng_integers
+from ..util import check_random_state, rng_integers
 
 
 class Player:
     """
     Class representing a player in an N-player normal form game.
 
     Parameters
```

### Comparing `quantecon-0.6.0/quantecon/game_theory/pure_nash.py` & `quantecon-0.7.0/quantecon/game_theory/pure_nash.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/random.py` & `quantecon-0.7.0/quantecon/game_theory/random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/repeated_game.py` & `quantecon-0.7.0/quantecon/game_theory/repeated_game.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/support_enumeration.py` & `quantecon-0.7.0/quantecon/game_theory/support_enumeration.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 B. von Stengel, "Equilibrium Computation for Two-Player Games in
 Strategic and Extensive Form," Chapter 3, N. Nisan, T. Roughgarden, E.
 Tardos, and V. Vazirani eds., Algorithmic Game Theory, 2007.
 
 """
 import numpy as np
 from numba import jit
-from quantecon.util.numba import _numba_linalg_solve
-from quantecon.util.combinatorics import next_k_array
+from ..util.numba import _numba_linalg_solve
+from ..util.combinatorics import next_k_array
 
 
 def support_enumeration(g):
     """
     Compute mixed-action Nash equilibria with equal support size for a
     2-player normal form game by support enumeration. For a
     non-degenerate game input, these are all the Nash equilibria.
@@ -52,15 +52,15 @@
     ------
     tuple(ndarray(float, ndim=1))
         Tuple of Nash equilibrium mixed actions.
 
     """
     try:
         N = g.N
-    except:
+    except AttributeError:
         raise TypeError('input must be a 2-player NormalFormGame')
     if N != 2:
         raise NotImplementedError('Implemented only for 2-player games')
     return _support_enumeration_gen(g.payoff_arrays)
 
 
 @jit(nopython=True)  # cache=True raises _pickle.PicklingError
```

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_brd.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_brd.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_fictplay.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_fictplay.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_lemke_howson.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_lemke_howson.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_localint.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_localint.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_logitdyn.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_logitdyn.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_mclennan_tourky.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_mclennan_tourky.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_normal_form_game.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_normal_form_game.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_pure_nash.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_pure_nash.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_random.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_repeated_game.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_repeated_game.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_support_enumeration.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_support_enumeration.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_utilities.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/tests/test_vertex_enumeration.py` & `quantecon-0.7.0/quantecon/game_theory/tests/test_vertex_enumeration.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/utilities.py` & `quantecon-0.7.0/quantecon/game_theory/utilities.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/game_theory/vertex_enumeration.py` & `quantecon-0.7.0/quantecon/game_theory/vertex_enumeration.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/graph_tools.py` & `quantecon-0.7.0/quantecon/graph_tools.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/gridtools.py` & `quantecon-0.7.0/quantecon/gridtools.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # Use the `quantecon` namespace for importing the objects
 # included below.
 
 import warnings
 from . import _gridtools
 
 
-__all__ = ['cartesian', 'mlinspace', 'simplex_grid', 'simplex_index',
-           'num_compositions', 'num_compositions_jit']
+__all__ = ['cartesian', 'mlinspace', 'cartesian_nearest_index', 'simplex_grid',
+           'simplex_index', 'num_compositions', 'num_compositions_jit']
 
 
 def __dir__():
     return __all__
 
 
 def __getattr__(name):
```

### Comparing `quantecon-0.6.0/quantecon/inequality.py` & `quantecon-0.7.0/quantecon/inequality.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/ivp.py` & `quantecon-0.7.0/quantecon/ivp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/kalman.py` & `quantecon-0.7.0/quantecon/kalman.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/lae.py` & `quantecon-0.7.0/quantecon/lae.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/lqcontrol.py` & `quantecon-0.7.0/quantecon/lqcontrol.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/lqnash.py` & `quantecon-0.7.0/quantecon/lqnash.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/lss.py` & `quantecon-0.7.0/quantecon/lss.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import warnings
 from . import _lss
 
 
 __all__ = ['LinearStateSpace', 'simulate_linear_model']
 
 
+def __dir__():
+    return __all__
+
+
 def __getattr__(name):
     if name not in __all__:
         raise AttributeError(
                 "`quantecon.lss` is deprecated and has no attribute "
                 f"'{name}'."
             )
```

### Comparing `quantecon-0.6.0/quantecon/markov/_ddp_linprog_simplex.py` & `quantecon-0.7.0/quantecon/markov/_ddp_linprog_simplex.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/markov/core.py` & `quantecon-0.7.0/quantecon/markov/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,19 +353,17 @@
             return self.period == 1
 
     @property
     def period(self):
         if self.is_irreducible:
             return self.digraph.period
         else:
-            rec_classes = self.recurrent_classes
-
             # Determine the period, the LCM of the periods of rec_classes
             d = 1
-            for rec_class in rec_classes:
+            for rec_class in self.recurrent_classes_indices:
                 period = self.digraph.subgraph(rec_class).period
                 d = (d * period) // gcd(d, period)
 
             return d
 
     @property
     def cyclic_classes(self):
```

### Comparing `quantecon-0.6.0/quantecon/markov/ddp.py` & `quantecon-0.7.0/quantecon/markov/ddp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/markov/gth_solve.py` & `quantecon-0.7.0/quantecon/markov/gth_solve.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/markov/random.py` & `quantecon-0.7.0/quantecon/markov/random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/markov/tests/test_core.py` & `quantecon-0.7.0/quantecon/markov/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 import numpy as np
 from scipy import sparse
 import itertools
 from numpy.testing import (
     assert_allclose, assert_array_equal, assert_array_less, assert_raises,
-    assert_
+    assert_, assert_equal
 )
 
 from quantecon.markov import (
     MarkovChain, mc_compute_stationary, mc_sample_path
 )
 
 
@@ -413,23 +413,25 @@
         state_values = [[0, 1], [2, 3], [4, 5]]  # Pass python list
         self.state_values = np.array(state_values)
 
         self.mc_reducible_dict = {
             'mc': MarkovChain([[1, 0, 0], [1, 0, 0], [0, 0, 1]],
                               state_values=state_values),
             'coms': [[0], [1], [2]],
-            'recs': [[0], [2]]
+            'recs': [[0], [2]],
+            'period': 1
         }
 
         self.mc_periodic_dict = {
             'mc': MarkovChain([[0, 1, 0], [0, 0, 1], [1, 0, 0]],
                               state_values=state_values),
             'coms': [[0, 1, 2]],
             'recs': [[0, 1, 2]],
-            'cycs': [[0], [1], [2]]
+            'cycs': [[0], [1], [2]],
+            'period': 3
         }
 
     def test_com_rec_classes(self):
         for mc_dict in [self.mc_reducible_dict, self.mc_periodic_dict]:
             mc = mc_dict['mc']
             coms = mc_dict['coms']
             recs = mc_dict['recs']
@@ -467,14 +469,20 @@
                     prop = prop0
                     key = lambda x: x[0, 0]
                 list_of_array_equal(
                     sorted(getattr(mc, prop), key=key),
                     sorted(classes, key=key)
                 )
 
+    def test_period(self):
+        for mc_dict in [self.mc_reducible_dict, self.mc_periodic_dict]:
+            mc = mc_dict['mc']
+            period = mc_dict['period']
+            assert_equal(mc.period, period)
+
     def test_simulate(self):
         # Deterministic mc
         mc = self.mc_periodic_dict['mc']
         ts_length = 6
 
         methods = ['simulate_indices', 'simulate']
```

### Comparing `quantecon-0.6.0/quantecon/markov/tests/test_ddp.py` & `quantecon-0.7.0/quantecon/markov/tests/test_ddp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/markov/tests/test_gth_solve.py` & `quantecon-0.7.0/quantecon/markov/tests/test_gth_solve.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/markov/tests/test_random.py` & `quantecon-0.7.0/quantecon/markov/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/markov/utilities.py` & `quantecon-0.7.0/quantecon/markov/utilities.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/matrix_eqn.py` & `quantecon-0.7.0/quantecon/matrix_eqn.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/meta.yaml` & `quantecon-0.7.0/quantecon/meta.yaml`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/linprog_simplex.py` & `quantecon-0.7.0/quantecon/optimize/linprog_simplex.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 TOL_PIV = 1e-7
 TOL_RATIO_DIFF = 1e-13
 
 PivOptions = namedtuple(
     'PivOptions', ['fea_tol', 'tol_piv', 'tol_ratio_diff']
 )
 PivOptions.__new__.__defaults__ = (FEA_TOL, TOL_PIV, TOL_RATIO_DIFF)
-PivOptions.__doc__ = 'namedtuple to hold tolerance values for pivoting'
+PivOptions.__doc__ = 'namedtuple to hold tolerance values for pivoting.'
 
 
 # Delete useless docstring for fields of namedtuple
 def _del_field_docstring(nt):
     for field in nt._fields:
         getattr(nt, field).__doc__ = ''
 
 
-for nt in [SimplexResult, PivOptions]:
-    _del_field_docstring(nt)
+for _nt in [SimplexResult, PivOptions]:
+    _del_field_docstring(_nt)
 
 
 @jit(nopython=True, cache=True)
 def linprog_simplex(c, A_ub=np.empty((0, 0)), b_ub=np.empty((0,)),
                     A_eq=np.empty((0, 0)), b_eq=np.empty((0,)),
                     max_iter=10**6, piv_options=PivOptions(),
                     tableau=None, basis=None, x=None, lambd=None):
```

### Comparing `quantecon-0.6.0/quantecon/optimize/minmax.py` & `quantecon-0.7.0/quantecon/optimize/minmax.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/nelder_mead.py` & `quantecon-0.7.0/quantecon/optimize/nelder_mead.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/pivoting.py` & `quantecon-0.7.0/quantecon/optimize/pivoting.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/root_finding.py` & `quantecon-0.7.0/quantecon/optimize/root_finding.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/scalar_maximization.py` & `quantecon-0.7.0/quantecon/optimize/scalar_maximization.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/tests/test_linprog_simplex.py` & `quantecon-0.7.0/quantecon/optimize/tests/test_linprog_simplex.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/tests/test_minmax.py` & `quantecon-0.7.0/quantecon/optimize/tests/test_minmax.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/tests/test_nelder_mead.py` & `quantecon-0.7.0/quantecon/optimize/tests/test_nelder_mead.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/tests/test_root_finding.py` & `quantecon-0.7.0/quantecon/optimize/tests/test_root_finding.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/optimize/tests/test_scalar_max.py` & `quantecon-0.7.0/quantecon/optimize/tests/test_scalar_max.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/quad.py` & `quantecon-0.7.0/quantecon/quad.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/quadsums.py` & `quantecon-0.7.0/quantecon/quadsums.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/random/tests/test_utilities.py` & `quantecon-0.7.0/quantecon/random/tests/test_utilities.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 sample_without_replacement
 
 """
 import numbers
 import numpy as np
 from numpy.testing import (assert_array_equal, assert_allclose, assert_raises,
                            assert_)
+from numba import njit
 from quantecon.random import probvec, sample_without_replacement, draw
 
 
 # probvec #
 
 class TestProbvec:
     def setup_method(self):
@@ -63,36 +64,47 @@
 
     # k > n
     assert_raises(ValueError, sample_without_replacement, 2, 3)
 
 
 # draw #
 
+@njit
+def draw_jitted(cdf, size=None):
+    return draw(cdf, size)
+
+
 class TestDraw:
     def setup_method(self):
         self.pmf = np.array([0.4, 0.1, 0.5])
         self.cdf = np.cumsum(self.pmf)
         self.n = len(self.pmf)
+        self.draw_funcs = [draw, draw_jitted]
 
     def test_return_types(self):
-        out = draw(self.cdf)
-        assert_(isinstance(out, numbers.Integral))
+        for func in self.draw_funcs:
+            out = func(self.cdf)
+            assert_(isinstance(out, numbers.Integral))
 
         size = 10
-        out = draw(self.cdf, size)
-        assert_(out.shape == (size,))
+        for func in self.draw_funcs:
+            out = func(self.cdf, size)
+            assert_(out.shape == (size,))
 
     def test_return_values(self):
-        out = draw(self.cdf)
-        assert_(out in range(self.n))
+        for func in self.draw_funcs:
+            out = func(self.cdf)
+            assert_(out in range(self.n))
 
         size = 10
-        out = draw(self.cdf, size)
-        assert_(np.isin(out, range(self.n)).all())
+        for func in self.draw_funcs:
+            out = func(self.cdf, size)
+            assert_(np.isin(out, range(self.n)).all())
 
     def test_lln(self):
         size = 1000000
-        out = draw(self.cdf, size)
-        hist, bin_edges = np.histogram(out, bins=self.n, density=True)
-        pmf_computed = hist * np.diff(bin_edges)
-        atol = 1e-2
-        assert_allclose(pmf_computed, self.pmf, atol=atol)
+        for func in self.draw_funcs:
+            out = func(self.cdf, size)
+            hist, bin_edges = np.histogram(out, bins=self.n, density=True)
+            pmf_computed = hist * np.diff(bin_edges)
+            atol = 1e-2
+            assert_allclose(pmf_computed, self.pmf, atol=atol)
```

### Comparing `quantecon-0.6.0/quantecon/random/utilities.py` & `quantecon-0.7.0/quantecon/random/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Utilities to Support Random Operations and Generating Vectors and Matrices
 
 """
 
 import numpy as np
-from numba import guvectorize, generated_jit, types
-
+from numba import guvectorize, types
+from numba.extending import overload
 from ..util import check_random_state, searchsorted
 
 
 # Generating Arrays and Vectors #
 
 def probvec(m, k, random_state=None, parallel=True):
     """
@@ -59,15 +59,15 @@
         _probvec_parallel(r, x)
     else:
         _probvec_cpu(r, x)
 
     return x
 
 
-def _probvec(r, out):
+def _probvec(r, out):  # pragma: no cover
     """
     Fill `out` with randomly sampled probability vectors as rows.
 
     To be complied as a ufunc by guvectorize of Numba. The inputs must
     have the same shape except the last axis; the length of the last
     axis of `r` must be that of `out` minus 1, i.e., if out.shape[-1] is
     k, then r.shape[-1] must be k-1.
@@ -165,15 +165,15 @@
     pool = np.arange(n)
     for j in range(k):
         idx = np.intp(np.floor(r[j] * (n-j)))  # np.floor returns a float
         out[j] = pool[idx]
         pool[idx] = pool[n-j-1]
 
 
-@generated_jit(nopython=True)
+# Pure python implementation that will run if the JIT compiler is disabled
 def draw(cdf, size=None):
     """
     Generate a random sample according to the cumulative distribution
     given by `cdf`. Jit-complied by Numba in nopython mode.
 
     Parameters
     ----------
@@ -194,14 +194,28 @@
     >>> cdf = np.cumsum([0.4, 0.6])
     >>> qe.random.draw(cdf)
     1
     >>> qe.random.draw(cdf, 10)
     array([1, 0, 1, 0, 1, 0, 0, 0, 1, 0])
 
     """
+    if isinstance(size, int):
+        rs = np.random.random(size)
+        out = np.empty(size, dtype=np.int_)
+        for i in range(size):
+            out[i] = searchsorted(cdf, rs[i])
+        return out
+    else:
+        r = np.random.random()
+        return searchsorted(cdf, r)
+
+
+# Overload for the `draw` function
+@overload(draw)
+def ol_draw(cdf, size):
     if isinstance(size, types.Integer):
         def draw_impl(cdf, size):
             rs = np.random.random(size)
             out = np.empty(size, dtype=np.int_)
             for i in range(size):
                 out[i] = searchsorted(cdf, rs[i])
             return out
```

### Comparing `quantecon-0.6.0/quantecon/rank_nullspace.py` & `quantecon-0.7.0/quantecon/rank_nullspace.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/robustlq.py` & `quantecon-0.7.0/quantecon/robustlq.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/util/array.py` & `quantecon-0.7.0/quantecon/util/array.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/util/combinatorics.py` & `quantecon-0.7.0/quantecon/util/combinatorics.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/util/notebooks.py` & `quantecon-0.7.0/quantecon/util/notebooks.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/util/numba.py` & `quantecon-0.7.0/quantecon/util/numba.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """
 Utilities to support Numba jitted functions
 
 """
 import numpy as np
-from numba import jit, generated_jit, types
-try:
-    from numba.np.linalg import _LAPACK  # for Numba >= 0.49.0
-except ModuleNotFoundError:
-    from numba.targets.linalg import _LAPACK  # for Numba < 0.49.0
+from numba import jit, types
+from numba.extending import overload
+from numba.np.linalg import _LAPACK
 
 
 # BLAS kinds as letters
 _blas_kinds = {
     types.float32: 's',
     types.float64: 'd',
     types.complex64: 'c',
     types.complex128: 'z',
 }
 
 
-@generated_jit(nopython=True, cache=True)
-def _numba_linalg_solve(a, b):
+def _numba_linalg_solve(a, b):  # pragma: no cover
+    pass
+
+
+@overload(_numba_linalg_solve, jit_options={'cache':True})
+def _numba_linalg_solve_ol(a, b):
     """
     Solve the linear equation ax = b directly calling a Numba internal
     function. The data in `a` and `b` are interpreted in Fortran order,
     and dtype of `a` and `b` must be the same, one of {float32, float64,
     complex64, complex128}. `a` and `b` are modified in place, and the
     solution is stored in `b`. *No error check is made for the inputs.*
+    Only work in a Numba-jitted function.
 
     Parameters
     ----------
     a : ndarray(ndim=2)
         2-dimensional ndarray of shape (n, n).
 
     b : ndarray(ndim=1 or 2)
```

### Comparing `quantecon-0.6.0/quantecon/util/random.py` & `quantecon-0.7.0/quantecon/util/random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/quantecon/util/timing.py` & `quantecon-0.7.0/quantecon/util/timing.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.6.0/PKG-INFO` & `quantecon-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: quantecon
-Version: 0.6.0
+Version: 0.7.0
 Summary: Import the main names to top level.
 Keywords: quantitative,economics
 Author-email: QuantEcon Project <admin@quantecon.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: numba
+Requires-Dist: numba>=0.49.0
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: requests
 Requires-Dist: scipy>=1.5.0
 Requires-Dist: sympy
 Requires-Dist: pytest ; extra == "testing"
 Requires-Dist: coverage ; extra == "testing"
 Requires-Dist: flake8 ; extra == "testing"
@@ -39,18 +39,16 @@
 
 ```python
   from quantecon.markov import DiscreteDP
   aiyagari_ddp = DiscreteDP(R, Q, beta)
   results = aiyagari_ddp.solve(method='policy_iteration')
 ```
 
-[![Build Status](https://github.com/QuantEcon/QuantEcon.py/workflows/build/badge.svg)](https://github.com/QuantEcon/QuantEcon.py/actions?query=workflow%3Abuild)
+[![Build Status](https://github.com/QuantEcon/QuantEcon.py/actions/workflows/ci.yml/badge.svg)](https://github.com/QuantEcon/QuantEcon.py/actions?query=workflow%3Abuild)
 [![Coverage Status](https://coveralls.io/repos/QuantEcon/QuantEcon.py/badge.svg)](https://coveralls.io/r/QuantEcon/QuantEcon.py)
-[![Code Quality: Python](https://img.shields.io/lgtm/grade/python/g/QuantEcon/QuantEcon.py.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/QuantEcon/QuantEcon.py/context:python)
-[![Total Alerts](https://img.shields.io/lgtm/alerts/g/QuantEcon/QuantEcon.py.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/QuantEcon/QuantEcon.py/alerts)
 [![Documentation Status](https://readthedocs.org/projects/quanteconpy/badge/?version=latest)](https://quanteconpy.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 Before installing `quantecon` we recommend you install the [Anaconda](https://www.anaconda.com/download/) Python distribution, which includes a full suite of scientific python tools. **Note:** `quantecon` is now only supporting Python version 3.5+. This is mainly to allow code to be written taking full advantage of new features such as using the `@` symbol for matrix multiplication. Therefore please install the latest Python 3 Anaconda distribution.
 
 Next you can install quantecon by opening a terminal prompt and typing
@@ -75,19 +73,18 @@
 
     pip install --upgrade quantecon
 
 ## Examples and Sample Code
 
 Many examples of QuantEcon.py in action can be found at [Quantitative Economics](https://lectures.quantecon.org/). See also the
 
-*   [Documentation](http://quanteconpy.readthedocs.org/en/latest/)
-*   [Notebook gallery](/notebooks)
-*   [Additional Examples](/python-examples)
+*   [Documentation](https://quanteconpy.readthedocs.org/en/latest/)
+*   [Notebook gallery](https://notes.quantecon.org)
 
-QuantEcon.py is supported financially by the [Alfred P. Sloan Foundation](http://www.sloan.org/) and is part of the [QuantEcon organization](/).
+QuantEcon.py is supported financially by the [Alfred P. Sloan Foundation](http://www.sloan.org/) and is part of the [QuantEcon organization](https://quantecon.org).
 
 ## Downloading the `quantecon` Repository
 
 An alternative is to download the sourcecode of the `quantecon` package and install it manually from [the github repository](https://github.com/QuantEcon/QuantEcon.py/). For example, if you have git installed type
 
     git clone https://github.com/QuantEcon/QuantEcon.py
```

