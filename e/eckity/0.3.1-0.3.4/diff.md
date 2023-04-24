# Comparing `tmp/eckity-0.3.1.tar.gz` & `tmp/eckity-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eckity-0.3.1.tar", last modified: Thu Mar 30 09:07:12 2023, max compression
+gzip compressed data, was "eckity-0.3.4.tar", last modified: Mon Apr 24 14:24:01 2023, max compression
```

## Comparing `eckity-0.3.1.tar` & `eckity-0.3.4.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.847751 eckity-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-30 09:06:55.000000 eckity-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-03-30 09:07:12.847751 eckity-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-03-30 09:06:55.000000 eckity-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.827751 eckity-0.3.1/eckity/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.827751 eckity-0.3.1/eckity/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/algorithms/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/algorithms/simple_evolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.827751 eckity-0.3.1/eckity/base/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/before_after_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.831751 eckity-0.3.1/eckity/breeders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/breeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/breeders/breeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/breeders/simple_breeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.831751 eckity-0.3.1/eckity/creators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.831751 eckity-0.3.1/eckity/creators/ga_creators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/ga_creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/ga_creators/bit_string_vector_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/ga_creators/float_vector_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/ga_creators/int_vector_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/ga_creators/simple_vector_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.831751 eckity-0.3.1/eckity/creators/gp_creators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/gp_creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/gp_creators/full.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/gp_creators/grow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/gp_creators/ramped_hh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/creators/gp_creators/tree_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.835751 eckity-0.3.1/eckity/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/evaluators/individual_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/evaluators/population_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/evaluators/simple_individual_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/evaluators/simple_population_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/event_based_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.835751 eckity-0.3.1/eckity/fitness/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/fitness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/fitness/fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/fitness/gp_fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/fitness/simple_fitness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.835751 eckity-0.3.1/eckity/genetic_encodings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.835751 eckity-0.3.1/eckity/genetic_encodings/ga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/ga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/ga/bit_string_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/ga/float_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/ga/int_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/ga/vector_individual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.835751 eckity-0.3.1/eckity/genetic_encodings/gp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/gp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.835751 eckity-0.3.1/eckity/genetic_encodings/gp/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/gp/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/gp/tree/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/gp/tree/tree_individual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_encodings/gp/tree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.835751 eckity-0.3.1/eckity/genetic_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.839751 eckity-0.3.1/eckity/genetic_operators/crossovers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/crossovers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/crossovers/subtree_crossover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/crossovers/vector_k_point_crossover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/failable_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/genetic_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.839751 eckity-0.3.1/eckity/genetic_operators/mutations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/mutations/erc_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/mutations/identity_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/mutations/subtree_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/mutations/vector_n_point_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/mutations/vector_random_mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.839751 eckity-0.3.1/eckity/genetic_operators/selections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/selections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/selections/elitism_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/selections/selection_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/genetic_operators/selections/tournament_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/individual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.839751 eckity-0.3.1/eckity/multi_objective_evolution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/multi_objective_evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/multi_objective_evolution/crowding_termination_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/multi_objective_evolution/nsga2_breeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/multi_objective_evolution/nsga2_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/multi_objective_evolution/nsga2_fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/multi_objective_evolution/nsga2_front_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/multi_objective_evolution/nsga2_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/population.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.839751 eckity-0.3.1/eckity/sklearn_compatible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/sklearn_compatible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/sklearn_compatible/classification_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/sklearn_compatible/regression_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/sklearn_compatible/sk_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/sklearn_compatible/sk_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/sklearn_compatible/sklearn_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.839751 eckity-0.3.1/eckity/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/statistics/best_average_worst_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/statistics/best_avg_worst_size_tree_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/statistics/minimal_print_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/statistics/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/subpopulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.839751 eckity-0.3.1/eckity/termination_checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/termination_checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/termination_checkers/termination_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-30 09:06:55.000000 eckity-0.3.1/eckity/termination_checkers/threshold_from_target_termination_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.827751 eckity-0.3.1/eckity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-03-30 09:07:12.000000 eckity-0.3.1/eckity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-03-30 09:07:12.000000 eckity-0.3.1/eckity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 09:07:12.000000 eckity-0.3.1/eckity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 09:07:12.000000 eckity-0.3.1/eckity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 09:07:12.000000 eckity-0.3.1/eckity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/multi_objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/multi_objective/moe_base_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/multi_objective/moe_base_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/multi_objective/moe_base_test/nsga2_basic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/multi_objective/zdt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/multi_objective/zdt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/multi_objective/zdt/nsga2zdt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/multi_objective/zdt/nsga2zdt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/multi_objective/zdt/nsga2zdt3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/treegp/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/treegp/non_sklearn_mode/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/non_sklearn_mode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/treegp/non_sklearn_mode/multiplexer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/non_sklearn_mode/multiplexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/non_sklearn_mode/multiplexer/mux_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/non_sklearn_mode/multiplexer/mux_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/treegp/non_sklearn_mode/symbolic_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/non_sklearn_mode/symbolic_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/treegp/sklearn_mode/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/sklearn_mode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/treegp/sklearn_mode/breast_cancer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/sklearn_mode/breast_cancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/sklearn_mode/breast_cancer/breast_cancer_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/sklearn_mode/breast_cancer/classification_gridsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/treegp/sklearn_mode/symbolic_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/sklearn_mode/symbolic_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/sklearn_mode/symbolic_regression/regression_gridsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/sklearn_mode/symbolic_regression/regression_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/treegp/sklearn_mode/symbolic_regression/sklearn_sym_reg_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/vectorga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/vectorga/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/vectorga/knapsack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/vectorga/knapsack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/vectorga/knapsack/knapsack_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/vectorga/knapsack/knapsack_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/examples/vectorga/one_max/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/vectorga/one_max/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/vectorga/one_max/one_max_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-30 09:06:55.000000 eckity-0.3.1/examples/vectorga/one_max/one_max_problem_float.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 09:07:12.847751 eckity-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-30 09:06:55.000000 eckity-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.843751 eckity-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:07:12.847751 eckity-0.3.1/tests/moe_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:06:55.000000 eckity-0.3.1/tests/moe_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-30 09:06:55.000000 eckity-0.3.1/tests/moe_test/test_moe_base_test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-03-30 09:06:55.000000 eckity-0.3.1/tests/moe_test/test_moe_front_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-30 09:06:55.000000 eckity-0.3.1/tests/test_sklearn_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-03-30 09:06:55.000000 eckity-0.3.1/tests/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.621170 eckity-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-24 14:23:50.000000 eckity-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-24 14:24:01.621170 eckity-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-24 14:23:50.000000 eckity-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/algorithms/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/algorithms/simple_evolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/before_after_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity/breeders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/breeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/breeders/breeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/breeders/simple_breeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/creators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/creators/ga_creators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/bit_string_vector_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/float_vector_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/int_vector_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/simple_vector_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/creators/gp_creators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/grow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/ramped_hh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/tree_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/individual_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/population_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/simple_individual_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/simple_population_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/event_based_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/fitness/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/fitness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/fitness/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/fitness/gp_fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/fitness/simple_fitness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/genetic_encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/genetic_encodings/ga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/bit_string_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/float_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/int_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/vector_individual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_encodings/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_encodings/gp/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/tree/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/tree/tree_individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/tree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_operators/crossovers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/crossovers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/crossovers/subtree_crossover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/crossovers/vector_k_point_crossover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/failable_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/genetic_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_operators/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/erc_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/identity_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/subtree_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/vector_n_point_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/vector_random_mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_operators/selections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/selections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/selections/elitism_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/selections/selection_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/selections/tournament_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/individual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.613170 eckity-0.3.4/eckity/multi_objective_evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/crowding_termination_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_breeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_front_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/population.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.613170 eckity-0.3.4/eckity/sklearn_compatible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/classification_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/regression_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/sk_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/sk_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/sklearn_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.613170 eckity-0.3.4/eckity/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/best_average_worst_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/best_avg_worst_size_tree_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/minimal_print_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/subpopulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/eckity/termination_checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/termination_checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/termination_checkers/termination_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/termination_checkers/threshold_from_target_termination_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/multi_objective/moe_base_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/moe_base_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/moe_base_test/nsga2_basic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/multi_objective/zdt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/zdt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/non_sklearn_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/mux_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/mux_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/sklearn_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/breast_cancer_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/classification_gridsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/regression_gridsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/regression_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/sklearn_sym_reg_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/vectorga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/vectorga/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/knapsack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/knapsack/knapsack_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/knapsack/knapsack_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/vectorga/one_max/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/one_max/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/one_max/one_max_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/one_max/one_max_problem_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:24:01.621170 eckity-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 14:23:50.000000 eckity-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.621170 eckity-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.621170 eckity-0.3.4/tests/moe_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/moe_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/moe_test/test_moe_base_test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/moe_test/test_moe_front_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/test_sklearn_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/test_vector.py
```

### Comparing `eckity-0.3.1/LICENSE` & `eckity-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/PKG-INFO` & `eckity-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eckity
-Version: 0.3.1
+Version: 0.3.4
 Summary: EC-KitY: Evolutionary Computation Tool Kit in Python.
 Home-page: https://www.eckity.org
 Author: Moshe Sipper, Achiya Elyasaf, Itai Tzruia, Tomer Halperin
 Author-email: sipper@gmail.com, achiya@bgu.ac.il, itaitz@post.bgu.ac.il, tomerhal@post.bgu.ac.il
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/EC-KitY/EC-KitY/issues
 Description-Content-Type: text/markdown
@@ -108,19 +108,21 @@
 Tomer Halperin
 
 ### Citation
 
 Citations are always appreciated 😊:
 ```
 @article{eckity2023,
-    author = {Sipper, Moshe and Halperin, Tomer and Tzruia, Itai and  Elyasaf, Achiya},
-    title = {{EC-KitY}: Evolutionary Computation Tool Kit in {Python}},
-    journal = {SoftwareX},
-    year = {2023},
-    url = {https://arxiv.org/abs/2207.10367},
+author = {Moshe Sipper and Tomer Halperin and Itai Tzruia and Achiya Elyasaf},
+title = {{EC-KitY}: Evolutionary computation tool kit in {Python} with seamless machine learning integration},
+journal = {SoftwareX},
+volume = {22},
+pages = {101381},
+year = {2023},
+url = {https://www.sciencedirect.com/science/article/pii/S2352711023000778},
 }
 
 @misc{eckity2022git,
     author = {Sipper, Moshe and Halperin, Tomer and Tzruia, Itai and  Elyasaf, Achiya},
     title = {{EC-KitY}: Evolutionary Computation Tool Kit in {Python}},
     year = {2022},
     publisher = {GitHub},
```

### Comparing `eckity-0.3.1/README.md` & `eckity-0.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -96,19 +96,21 @@
 Tomer Halperin
 
 ### Citation
 
 Citations are always appreciated 😊:
 ```
 @article{eckity2023,
-    author = {Sipper, Moshe and Halperin, Tomer and Tzruia, Itai and  Elyasaf, Achiya},
-    title = {{EC-KitY}: Evolutionary Computation Tool Kit in {Python}},
-    journal = {SoftwareX},
-    year = {2023},
-    url = {https://arxiv.org/abs/2207.10367},
+author = {Moshe Sipper and Tomer Halperin and Itai Tzruia and Achiya Elyasaf},
+title = {{EC-KitY}: Evolutionary computation tool kit in {Python} with seamless machine learning integration},
+journal = {SoftwareX},
+volume = {22},
+pages = {101381},
+year = {2023},
+url = {https://www.sciencedirect.com/science/article/pii/S2352711023000778},
 }
 
 @misc{eckity2022git,
     author = {Sipper, Moshe and Halperin, Tomer and Tzruia, Itai and  Elyasaf, Achiya},
     title = {{EC-KitY}: Evolutionary Computation Tool Kit in {Python}},
     year = {2022},
     publisher = {GitHub},
```

### Comparing `eckity-0.3.1/eckity/algorithms/algorithm.py` & `eckity-0.3.4/eckity/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/algorithms/simple_evolution.py` & `eckity-0.3.4/eckity/algorithms/simple_evolution.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/before_after_publisher.py` & `eckity-0.3.4/eckity/before_after_publisher.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/breeders/breeder.py` & `eckity-0.3.4/eckity/breeders/breeder.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/breeders/simple_breeder.py` & `eckity-0.3.4/eckity/breeders/simple_breeder.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/creators/creator.py` & `eckity-0.3.4/eckity/creators/creator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/creators/ga_creators/simple_vector_creator.py` & `eckity-0.3.4/eckity/creators/ga_creators/simple_vector_creator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/creators/gp_creators/full.py` & `eckity-0.3.4/eckity/creators/gp_creators/full.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/creators/gp_creators/grow.py` & `eckity-0.3.4/eckity/creators/gp_creators/grow.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/creators/gp_creators/ramped_hh.py` & `eckity-0.3.4/eckity/creators/gp_creators/ramped_hh.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/creators/gp_creators/tree_creator.py` & `eckity-0.3.4/eckity/creators/gp_creators/tree_creator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/evaluators/individual_evaluator.py` & `eckity-0.3.4/eckity/evaluators/individual_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/evaluators/population_evaluator.py` & `eckity-0.3.4/eckity/evaluators/population_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/evaluators/simple_individual_evaluator.py` & `eckity-0.3.4/eckity/evaluators/simple_individual_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 		Returns
 		-------
 		Individual
 			the individual with the best fitness out of the given individuals
 		"""
 		super().evaluate(individual, environment_individuals)
-		fitness_score = self._evaluate_individual(individual)
+		fitness_score = self.evaluate_individual(individual)
 		individual.fitness.set_fitness(fitness_score)
 		return individual
 
 	@abstractmethod
 	def evaluate_individual(self, individual):
 		"""
 		Evaluate the fitness score for the given individual.
@@ -50,15 +50,7 @@
 
 		Returns
 		-------
 		float
 			The evaluated fitness value for the given individual
 		"""
 		raise ValueError("evaluate_individual is an abstract method in SimpleIndividualEvaluator")
-
-	def _evaluate_individual(self, individual):
-		"""
-		Evaluate the fitness score for the given individual.
-		Used for backward compatability, since this evaluate_individual is now public.
-		"""
-		return self.evaluate_individual(individual)
-
```

### Comparing `eckity-0.3.1/eckity/evaluators/simple_population_evaluator.py` & `eckity-0.3.4/eckity/evaluators/simple_population_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/event_based_operator.py` & `eckity-0.3.4/eckity/event_based_operator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/fitness/fitness.py` & `eckity-0.3.4/eckity/fitness/fitness.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/fitness/gp_fitness.py` & `eckity-0.3.4/eckity/fitness/gp_fitness.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/fitness/simple_fitness.py` & `eckity-0.3.4/eckity/fitness/simple_fitness.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_encodings/ga/bit_string_vector.py` & `eckity-0.3.4/eckity/genetic_encodings/ga/bit_string_vector.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_encodings/ga/float_vector.py` & `eckity-0.3.4/eckity/genetic_encodings/ga/float_vector.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_encodings/ga/int_vector.py` & `eckity-0.3.4/eckity/genetic_encodings/ga/int_vector.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_encodings/ga/vector_individual.py` & `eckity-0.3.4/eckity/genetic_encodings/ga/vector_individual.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_encodings/gp/tree/functions.py` & `eckity-0.3.4/eckity/genetic_encodings/gp/tree/functions.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_encodings/gp/tree/tree_individual.py` & `eckity-0.3.4/eckity/genetic_encodings/gp/tree/tree_individual.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_encodings/gp/tree/utils.py` & `eckity-0.3.4/eckity/genetic_encodings/gp/tree/utils.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_operators/crossovers/subtree_crossover.py` & `eckity-0.3.4/eckity/genetic_operators/crossovers/subtree_crossover.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_operators/crossovers/vector_k_point_crossover.py` & `eckity-0.3.4/eckity/genetic_operators/crossovers/vector_k_point_crossover.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from random import sample
 
 from eckity.genetic_operators.genetic_operator import GeneticOperator
+from eckity.genetic_encodings.ga.vector_individual import Vector
 
 
 class VectorKPointsCrossover(GeneticOperator):
     def __init__(self, probability=1, arity=2, k=1, events=None):
         """
             Vector N Point Mutation.
 
@@ -41,18 +42,24 @@
 
         Returns
         ----------
         list of individuals
             individuals after the crossover
         """
         self.individuals = individuals
-        self.points = sorted(sample(range(0, individuals[0].size()), self.k))
-
+        self.points = sorted(sample(range(1, individuals[0].size()), self.k))
+        
         start_index = 0
-        for end_point in self.points:
+        for i in range(0, len(self.points), 2):
+            end_point = self.points[i]
             replaced_part = individuals[0].get_vector_part(start_index, end_point)
             replaced_part = individuals[1].replace_vector_part(replaced_part, start_index)
             individuals[0].replace_vector_part(replaced_part, start_index)
-            start_index = end_point  # todo add last iter
+            start_index = end_point
+
+        # replace the last part (from last point to end)
+        replaced_part = individuals[0].get_vector_part(self.points[-1], individuals[0].size())
+        replaced_part = individuals[1].replace_vector_part(replaced_part, self.points[-1])
+        individuals[0].replace_vector_part(replaced_part, self.points[-1])
 
         self.applied_individuals = individuals
         return individuals
```

### Comparing `eckity-0.3.1/eckity/genetic_operators/failable_operator.py` & `eckity-0.3.4/eckity/genetic_operators/failable_operator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_operators/genetic_operator.py` & `eckity-0.3.4/eckity/genetic_operators/genetic_operator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_operators/mutations/erc_mutation.py` & `eckity-0.3.4/eckity/genetic_operators/mutations/erc_mutation.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_operators/mutations/subtree_mutation.py` & `eckity-0.3.4/eckity/genetic_operators/mutations/subtree_mutation.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_operators/mutations/vector_n_point_mutation.py` & `eckity-0.3.4/eckity/genetic_operators/mutations/vector_n_point_mutation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from random import choices
-from random import sample
+import random
 
 from eckity.genetic_operators.failable_operator import FailableOperator
+from eckity.genetic_encodings.ga.vector_individual import Vector
+
+from typing import List, Tuple, Union
 
 
 class VectorNPointMutation(FailableOperator):
     """
     Vector N Point Mutation.
 
     Randomly chooses N vector cells and performs a small change in their values.
@@ -17,84 +19,86 @@
 
     probability : float
         The probability of the mutation operator to be applied
 
     arity : int
         The number of individuals this mutation is applied on
 
+    cell_selector: callable
+        Returns the indices of the cells to mutate
+
     mut_val_getter: callable
         Returns a mutated value of a certain cell
 
     success_checker: callable
         Checks if a given (mutated) cell value is legal
 
     events: list of strings
         Events to publish before/after the mutation operator
     """
-    def __init__(self, n=1, probability=1, arity=1, mut_val_getter=None,
-                 success_checker=None, events=None, attempts=5):
+    def __init__(self,
+                 n=1,
+                 probability=1.0,
+                 arity=1,
+                 cell_selector=None,
+                 mut_val_getter=None,
+                 success_checker=None,
+                 events=None,
+                 attempts=5):
         super().__init__(probability=probability, arity=arity, events=events, attempts=attempts)
         self.n = n
 
+        if cell_selector is None:
+            cell_selector = self.default_cell_selector
+        self.cell_selector = cell_selector
+
         if success_checker is None:
             success_checker = self.default_success_checker
         self.success_checker = success_checker
 
         if mut_val_getter is None:
             mut_val_getter = self.default_mut_val_getter
         self.mut_val_getter = mut_val_getter
 
     @staticmethod
-    def default_mut_val_getter(vec, idx):
-        """
-        Default implementation for mutated value getter
-
-        Parameters
-        ----------
-        vec : Vector
-            a vector individual
-
-        idx : int
-            vector cell index
-
-        Returns
-        ----------
-        object
-            Mutated vector cell value
-        """
+    def default_mut_val_getter(vec: Vector, idx: int) -> Union[int, float]:
         return vec.get_random_number_in_bounds(vec, idx)
 
     @staticmethod
-    def default_success_checker(old_vec, new_vec):
+    def default_success_checker(old_vec: Vector, new_vec: Vector) -> bool:
         return new_vec.check_if_in_bounds()
+    
+    def default_cell_selector(self, vec: Vector) -> List[int]:
+        vector_indices = range(vec.size())
+        return random.sample(vector_indices, k=self.n)
 
-    def attempt_operator(self, individuals, attempt_num):
+    def attempt_operator(self, individuals: List[Vector], attempt_num) -> Tuple[bool, List[Vector]]:
         """
         Attempt to perform the mutation operator
 
         Parameters
         ----------
-        individuals : list of individuals
-            individuals to mutate
+        individuals : list of vectors
+            vectors to mutate
 
         attempt_num : int
             Current attempt number
 
         Returns
         ----------
-        tuple of (bool, list of individuals)
+        tuple of (bool, list of vectors)
             first return value determines if the the attempt succeeded
             second return value is the operator result
         """
         succeeded = True
         for individual in individuals:
             old_individual = individual.clone()
 
             # randomly select n points of the vector (without repetitions)
-            m_points = sample(range(individual.size()), k=self.n)
+            m_points = self.cell_selector(individual)
             # obtain the mutated values
             mut_vals = [self.mut_val_getter(individual, m_point) for m_point in m_points]
 
             # update the mutated value in-place
             for m_point, mut_val in zip(m_points, mut_vals):
                 individual.set_cell_value(m_point, mut_val)
```

### Comparing `eckity-0.3.1/eckity/genetic_operators/mutations/vector_random_mutation.py` & `eckity-0.3.4/eckity/genetic_operators/mutations/vector_random_mutation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from random import random
 
 from eckity.genetic_operators.mutations.vector_n_point_mutation import VectorNPointMutation
+from eckity.genetic_encodings.ga.vector_individual import Vector
 
 
 class FloatVectorUniformOnePointMutation(VectorNPointMutation):
     """
     Uniform One Point Float Mutation
     """
     def __init__(self, probability=1.0, arity=1, events=None):
```

### Comparing `eckity-0.3.1/eckity/genetic_operators/selections/elitism_selection.py` & `eckity-0.3.4/eckity/genetic_operators/selections/elitism_selection.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_operators/selections/selection_method.py` & `eckity-0.3.4/eckity/genetic_operators/selections/selection_method.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/genetic_operators/selections/tournament_selection.py` & `eckity-0.3.4/eckity/genetic_operators/selections/tournament_selection.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/individual.py` & `eckity-0.3.4/eckity/individual.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/multi_objective_evolution/crowding_termination_checker.py` & `eckity-0.3.4/eckity/multi_objective_evolution/crowding_termination_checker.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/multi_objective_evolution/nsga2_breeder.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_breeder.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/multi_objective_evolution/nsga2_evolution.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_evolution.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/multi_objective_evolution/nsga2_fitness.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_fitness.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/multi_objective_evolution/nsga2_front_sorting.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_front_sorting.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/multi_objective_evolution/nsga2_plot.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_plot.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/population.py` & `eckity-0.3.4/eckity/population.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/sklearn_compatible/classification_evaluator.py` & `eckity-0.3.4/eckity/sklearn_compatible/classification_evaluator.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 
 
 class ClassificationEvaluator(SimpleIndividualEvaluator):
     """
     Class to compute the fitness of an individual in classification problems.
     """
 
-    def __init__(self, X=None, y=None):
+    def __init__(self, X=None, y=None, metric=accuracy_score):
         super().__init__()
         self.X = X
         self.y = y
+        self.metric = metric
 
     def set_context(self, context):
         """
         Receive X and y values and assign them to X and y fields.
 
         Parameters
         ----------
@@ -33,15 +34,15 @@
         Returns
         -------
         None.
         """
         self.X = context[0]
         self.y = context[1]
 
-    def _evaluate_individual(self, individual):
+    def evaluate_individual(self, individual):
         """
         Compute the fitness value by comparing the program tree execution result to the result vector y
 
         Parameters
         ----------
         individual: Tree
             An individual program tree in the GP population, whose fitness needs to be computed.
@@ -51,11 +52,11 @@
 
         Returns
         -------
         float:
             computed fitness value
         """
         y_pred = self.classify_individual(individual)
-        return accuracy_score(y_true=self.y, y_pred=y_pred)
+        return self.metric(y_true=self.y, y_pred=y_pred)
 
     def classify_individual(self, individual):
         return np.where(individual.execute(self.X) > CLASSIFICATION_THRESHOLD, 1, 0)
```

### Comparing `eckity-0.3.1/eckity/sklearn_compatible/regression_evaluator.py` & `eckity-0.3.4/eckity/sklearn_compatible/regression_evaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,20 +15,25 @@
     Parameters
     ----------
     X: array-like of shape (n_samples, n_features), default=None
     Training/Test data.
 
     y: array-like of shape (n_samples,) or (n_samples, 1), default=None
     Target vector. used during the training phase.
+
+    metric: callable (optional, default=mean_absolute_error)
+    A function which receives two array-like of shapes (n_samples,) or (n_samples, 1) and returns a float or
+    ndarray of floats
     """
         
-    def __init__(self, X=None, y=None):
+    def __init__(self, X=None, y=None, metric=mean_absolute_error):
         super().__init__()
         self.X = X
         self.y = y
+        self.metric = metric
 
     def set_context(self, context):
         """
         Receive X and y values and assign them to X and y fields.
 
         Parameters
         ----------
@@ -46,25 +51,26 @@
         X, y = make_regression()
         X_train, X_test, y_train, y_test = train_test_split()
         reg_eval.set_context(X_train, y_train)
         """
         self.X = context[0]
         self.y = context[1]
 
-    def _evaluate_individual(self, individual):
+    def evaluate_individual(self, individual):
         """
         compute fitness value by computing the MAE between program tree execution result and y result vector
 
         Parameters
         ----------
         individual : Tree
             An individual program tree in the GP population, whose fitness needs to be computed.
             Makes use of GPTree.execute, which runs the program.
             In Sklearn settings, calling `individual.execute` must use a numpy array.
             For example, if self.X is X_train/X_test, the call is `individual.execute(self.X)`.
 
         Returns
         ----------
         float
-            Computed fitness value - evaluated using MAE between the execution result of X and the vector y.
+            Computed fitness value - evaluated using the provided scoring function between the execution result of X and
+            the vector y.
         """
-        return mean_absolute_error(self.y, individual.execute(self.X))
+        return self.metric(self.y, individual.execute(self.X))
```

### Comparing `eckity-0.3.1/eckity/sklearn_compatible/sk_classifier.py` & `eckity-0.3.4/eckity/sklearn_compatible/sk_classifier.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/sklearn_compatible/sklearn_wrapper.py` & `eckity-0.3.4/eckity/sklearn_compatible/sklearn_wrapper.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/statistics/best_average_worst_statistics.py` & `eckity-0.3.4/eckity/statistics/best_average_worst_statistics.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/statistics/best_avg_worst_size_tree_statistics.py` & `eckity-0.3.4/eckity/statistics/best_avg_worst_size_tree_statistics.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/statistics/minimal_print_statistics.py` & `eckity-0.3.4/eckity/statistics/minimal_print_statistics.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/statistics/statistics.py` & `eckity-0.3.4/eckity/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/subpopulation.py` & `eckity-0.3.4/eckity/subpopulation.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/termination_checkers/termination_checker.py` & `eckity-0.3.4/eckity/termination_checkers/termination_checker.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity/termination_checkers/threshold_from_target_termination_checker.py` & `eckity-0.3.4/eckity/termination_checkers/threshold_from_target_termination_checker.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/eckity.egg-info/PKG-INFO` & `eckity-0.3.4/eckity.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eckity
-Version: 0.3.1
+Version: 0.3.4
 Summary: EC-KitY: Evolutionary Computation Tool Kit in Python.
 Home-page: https://www.eckity.org
 Author: Moshe Sipper, Achiya Elyasaf, Itai Tzruia, Tomer Halperin
 Author-email: sipper@gmail.com, achiya@bgu.ac.il, itaitz@post.bgu.ac.il, tomerhal@post.bgu.ac.il
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/EC-KitY/EC-KitY/issues
 Description-Content-Type: text/markdown
@@ -108,19 +108,21 @@
 Tomer Halperin
 
 ### Citation
 
 Citations are always appreciated 😊:
 ```
 @article{eckity2023,
-    author = {Sipper, Moshe and Halperin, Tomer and Tzruia, Itai and  Elyasaf, Achiya},
-    title = {{EC-KitY}: Evolutionary Computation Tool Kit in {Python}},
-    journal = {SoftwareX},
-    year = {2023},
-    url = {https://arxiv.org/abs/2207.10367},
+author = {Moshe Sipper and Tomer Halperin and Itai Tzruia and Achiya Elyasaf},
+title = {{EC-KitY}: Evolutionary computation tool kit in {Python} with seamless machine learning integration},
+journal = {SoftwareX},
+volume = {22},
+pages = {101381},
+year = {2023},
+url = {https://www.sciencedirect.com/science/article/pii/S2352711023000778},
 }
 
 @misc{eckity2022git,
     author = {Sipper, Moshe and Halperin, Tomer and Tzruia, Itai and  Elyasaf, Achiya},
     title = {{EC-KitY}: Evolutionary Computation Tool Kit in {Python}},
     year = {2022},
     publisher = {GitHub},
```

### Comparing `eckity-0.3.1/eckity.egg-info/SOURCES.txt` & `eckity-0.3.4/eckity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/examples/multi_objective/moe_base_test/nsga2_basic_test.py` & `eckity-0.3.4/examples/multi_objective/moe_base_test/nsga2_basic_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 import random
 random.seed(0)
 
 
 class NSGA2BasicTestEvaluator(SimpleIndividualEvaluator):
-	def _evaluate_individual(self, individual):
+	def evaluate_individual(self, individual):
 		"""
             Compute the fitness value of a given individual.
 
             Parameters
             ----------
             individual: Vector
                 The individual to compute the fitness value for.
```

### Comparing `eckity-0.3.1/examples/multi_objective/zdt/nsga2zdt1.py` & `eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt1.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from eckity.statistics.minimal_print_statistics import MinimalPrintStatistics
 from eckity.subpopulation import Subpopulation
 from eckity.genetic_encodings.ga.float_vector import FloatVector
 
 
 
 class Zdt1Evaluator(SimpleIndividualEvaluator):
-	def _evaluate_individual(self, individual):
+	def evaluate_individual(self, individual):
 		"""
             Compute the fitness value of a given individual.
 
             Parameters
             ----------
             individual: Vector
                 The individual to compute the fitness value for.
```

### Comparing `eckity-0.3.1/examples/multi_objective/zdt/nsga2zdt2.py` & `eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from eckity.statistics.minimal_print_statistics import MinimalPrintStatistics
 from eckity.subpopulation import Subpopulation
 from eckity.genetic_encodings.ga.float_vector import FloatVector
 
 
 
 class Zdt2Evaluator(SimpleIndividualEvaluator):
-	def _evaluate_individual(self, individual):
+	def evaluate_individual(self, individual):
 		"""
 			Compute the fitness value of a given individual.
 
 			Parameters
 			----------
 			individual: Vector
 				The individual to compute the fitness value for.
```

### Comparing `eckity-0.3.1/examples/multi_objective/zdt/nsga2zdt3.py` & `eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt3.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from eckity.population import Population
 from eckity.statistics.minimal_print_statistics import MinimalPrintStatistics
 from eckity.subpopulation import Subpopulation
 from eckity.genetic_encodings.ga.float_vector import FloatVector
 
 
 class Zdt3Evaluator(SimpleIndividualEvaluator):
-	def _evaluate_individual(self, individual):
+	def evaluate_individual(self, individual):
 		"""
             Compute the fitness value of a given individual.
 
             Parameters
             ----------
             individual: Vector
                 The individual to compute the fitness value for.
```

### Comparing `eckity-0.3.1/examples/treegp/non_sklearn_mode/multiplexer/mux_evaluator.py` & `eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/mux_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         values = [list(x) + [_target_func(*x)] for x in product([0, 1], repeat=_target_func.__code__.co_argcount)]
         truth_tbl = pd.DataFrame(values, columns=(list(_target_func.__code__.co_varnames) + ['output']))
 
         # split dataframe to input columns and an output column
         self.inputs = truth_tbl.iloc[:, :NUM_COLUMNS]
         self.output = truth_tbl['output']
 
-    def _evaluate_individual(self, individual):
+    def evaluate_individual(self, individual):
         """
         Compute the fitness value of a given individual.
 
         Fitness evaluation is done calculating the accuracy between the tree execution result and the optimal result
         (multiplexer truth table).
 
         Parameters
```

### Comparing `eckity-0.3.1/examples/treegp/non_sklearn_mode/multiplexer/mux_main.py` & `eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/mux_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_evaluator.py` & `eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         # np.random.seed(0)
 
         data = np.random.uniform(-100, 100, size=(200, 3))
         self.df = pd.DataFrame(data, columns=['x', 'y', 'z'])
         self.df['target'] = _target_func(self.df['x'], self.df['y'], self.df['z'])
 
-    def _evaluate_individual(self, individual):
+    def evaluate_individual(self, individual):
         """
         Parameters
         ----------
         individual : Tree
             An individual program tree in the gp population, whose fitness needs to be computed.
             Makes use of GPTree.execute, which runs the program.
             Calling `gptree.execute` must use keyword arguments that match the terminal-set variables.
```

### Comparing `eckity-0.3.1/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_main.py` & `eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/examples/treegp/sklearn_mode/breast_cancer/breast_cancer_main.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/breast_cancer_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/examples/treegp/sklearn_mode/breast_cancer/classification_gridsearch.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/classification_gridsearch.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/examples/treegp/sklearn_mode/symbolic_regression/regression_gridsearch.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/regression_gridsearch.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/examples/treegp/sklearn_mode/symbolic_regression/regression_pipeline.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/examples/treegp/sklearn_mode/symbolic_regression/sklearn_sym_reg_main.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/sklearn_sym_reg_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/examples/vectorga/knapsack/knapsack_evaluator.py` & `eckity-0.3.4/examples/vectorga/knapsack/knapsack_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                     raise ValueError('Elements in items list must be tuples of (weight: int, price: int or float)')
 
             # Convert items list to dictionary by adding item id
             items = {i: items[i] for i in range(len(items))}
         self.items = items
         self.max_weight = max_weight
 
-    def _evaluate_individual(self, individual):
+    def evaluate_individual(self, individual):
         """
         Compute the fitness value of a given individual.
 
         Parameters
         ----------
         individual: Vector
             The individual to compute the fitness value for.
```

### Comparing `eckity-0.3.1/examples/vectorga/knapsack/knapsack_main.py` & `eckity-0.3.4/examples/vectorga/knapsack/knapsack_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/examples/vectorga/one_max/one_max_problem.py` & `eckity-0.3.4/examples/vectorga/one_max/one_max_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from eckity.genetic_operators.selections.tournament_selection import TournamentSelection
 from eckity.statistics.best_average_worst_statistics import BestAverageWorstStatistics
 from eckity.subpopulation import Subpopulation
 from eckity.termination_checkers.threshold_from_target_termination_checker import ThresholdFromTargetTerminationChecker
 
 
 class OneMaxEvaluator(SimpleIndividualEvaluator):
-    def _evaluate_individual(self, individual):
+    def evaluate_individual(self, individual):
         """
             Compute the fitness value of a given individual.
 
             Parameters
             ----------
             individual: Vector
                 The individual to compute the fitness value for.
```

### Comparing `eckity-0.3.1/examples/vectorga/one_max/one_max_problem_float.py` & `eckity-0.3.4/examples/vectorga/one_max/one_max_problem_float.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from eckity.genetic_operators.selections.tournament_selection import TournamentSelection
 from eckity.statistics.best_average_worst_statistics import BestAverageWorstStatistics
 from eckity.subpopulation import Subpopulation
 from eckity.termination_checkers.threshold_from_target_termination_checker import ThresholdFromTargetTerminationChecker
 
 
 class OneMaxEvaluator(SimpleIndividualEvaluator):
-    def _evaluate_individual(self, individual):
+    def evaluate_individual(self, individual):
         """
             Compute the fitness value of a given individual.
 
             Parameters
             ----------
             individual: Vector
                 The individual to compute the fitness value for.
```

### Comparing `eckity-0.3.1/setup.py` & `eckity-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/tests/moe_test/test_moe_base_test_eval.py` & `eckity-0.3.4/tests/moe_test/test_moe_base_test_eval.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,51 +37,51 @@
 		ans.append(1 - math.exp(-sum((chromosome - 1 / math.sqrt(n)) ** 2)))
 		ans.append(1 - math.exp(-sum((chromosome + 1 / math.sqrt(n)) ** 2)))
 		return ans
 
 	def test_eval_fixed_vals(self):
 		ind = GAVectorCreator(length=3, bounds=(-4, 4), fitness_type=NSGA2Fitness, vector_type=FloatVector)
 		ind.vector = [-1.04, 2.844, -2.54]
-		actual = self.evaluator._evaluate_individual(ind)
+		actual = self.evaluator.evaluate_individual(ind)
 		expected = [0.999, 0.999]
 		self.assert_vector_almost_equal(actual, expected, 0.01)
 
 	def test_eval_fixed_vals_2_first_half(self):
 		ind = GAVectorCreator(length=3, bounds=(-4, 4), fitness_type=NSGA2Fitness, vector_type=FloatVector)
 		ind.vector = [-3.5158362080315237, 0.06631935351665152, -2.921231400536878]
-		actual = self.evaluator._evaluate_individual(ind)
+		actual = self.evaluator.evaluate_individual(ind)
 		expected = [0.9999999999998029, 0.999999516777658]
 		self.assert_vector_almost_equal(actual, expected, tolerance=0.000000000000001)
 
 	def test_eval_fixed_5_vals_grate_values(self):
 		ind = GAVectorCreator(length=3, bounds=(-4, 4), fitness_type=NSGA2Fitness, vector_type=FloatVector)
 		ind.vector = [-3.4817449392563073, -2.728885522520228, 3.7399170615305213]
-		actual = self.evaluator._evaluate_individual(ind)
+		actual = self.evaluator.evaluate_individual(ind)
 		expected = [1.0, 0.9999999999999993]
 		self.assert_vector_almost_equal(actual, expected, tolerance=0.000000000000001)
 
 	def test_eval_fixed_vals_6_first_half(self):
 		ind = GAVectorCreator(length=3, bounds=(-4, 4), fitness_type=NSGA2Fitness, vector_type=FloatVector)
 		ind.vector = [-2.841398594290565, -1.4434725567566344, 3.6928271437413196]
-		actual = self.evaluator._evaluate_individual(ind)
+		actual = self.evaluator.evaluate_individual(ind)
 		expected = [0.9999999999913871, 0.9999999999661979]
 		self.assert_vector_almost_equal(actual, expected, tolerance=0.000000000000001)
 
 	def test_eval_fixed_vals_7_second_half(self):
 		ind = GAVectorCreator(length=3, bounds=(-4, 4), fitness_type=NSGA2Fitness, vector_type=FloatVector)
 		ind.vector = [3.768444634957887, -1.2647927144943072, 3.5023114497554335]
-		actual = self.evaluator._evaluate_individual(ind)
+		actual = self.evaluator.evaluate_individual(ind)
 		expected = [0.9999999997555407, 0.9999999999999998]
 		self.assert_vector_almost_equal(actual, expected, tolerance=0.000000000000001)
 
 	def test_eval_random_vals(self):
 		random_tests_count = 10
 		for i in range(random_tests_count):
 			vector = list(np.random.uniform(-4, 4, 3))
 			self.check_sigel_vector(vector)
 
 	def check_sigel_vector(self, initial_vector):
 		ind = GAVectorCreator(length=3, bounds=(-4, 4), fitness_type=NSGA2Fitness, vector_type=FloatVector)
 		ind.vector = initial_vector
-		actual = self.evaluator._evaluate_individual(ind)
+		actual = self.evaluator.evaluate_individual(ind)
 		expected = self.evaluation_valid(initial_vector)
 		self.assert_vector_almost_equal(actual, expected)
```

### Comparing `eckity-0.3.1/tests/moe_test/test_moe_front_selection.py` & `eckity-0.3.4/tests/moe_test/test_moe_front_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from eckity.multi_objective_evolution.nsga2_front_sorting import NSGA2FrontSorting
 
 from eckity.population import Population
 from eckity.subpopulation import Subpopulation
 
 
 class FitnessIsVectorEval(SimpleIndividualEvaluator):
-	def _evaluate_individual(self, individual):
+	def evaluate_individual(self, individual):
 		''' sets the fitness to be the value of the vector'''
 		return individual.vector
 
 
 class TestNSGA2FrontSelection:
 
 	@classmethod
```

### Comparing `eckity-0.3.1/tests/test_sklearn_compatibility.py` & `eckity-0.3.4/tests/test_sklearn_compatibility.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.1/tests/test_vector.py` & `eckity-0.3.4/tests/test_vector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 from collections import Counter
 
 import pytest
+import random
 
 from eckity.fitness.simple_fitness import SimpleFitness
+from eckity.genetic_encodings.ga.vector_individual import Vector
 from eckity.genetic_encodings.ga.bit_string_vector import BitStringVector
 from eckity.genetic_encodings.ga.float_vector import FloatVector
 from eckity.genetic_encodings.ga.int_vector import IntVector
 from eckity.genetic_operators.mutations.vector_random_mutation import FloatVectorGaussOnePointMutation, \
 	FloatVectorUniformNPointMutation, FloatVectorGaussNPointMutation, IntVectorOnePointMutation, \
 	BitStringVectorNFlipMutation, IntVectorNPointMutation
+from eckity.genetic_operators.crossovers.vector_k_point_crossover import VectorKPointsCrossover
 
+@pytest.fixture(autouse=True)
+def run_before_and_after_tests():
+	"""Fixture to execute asserts before and after a test is run"""
+	# Setup
+	random.seed(0)
+
+	yield # this is where the testing happens
+
+	# Teardown
+	pass
 
 class TestVector:
 	def test_bad_bounds(self):
 		length = 5
 		bounds = [(i, i + 1) for i in range(length)]
 
 		with pytest.raises(ValueError):
@@ -181,7 +194,29 @@
 		mut = FloatVectorGaussNPointMutation(n=n_points)
 
 		mut.apply_operator([vec1])
 		cnt = Counter(vec1.vector)
 
 		assert len(cnt.keys()) == n_points + 1
 		assert cnt[0.0] == length - n_points
+
+	def test_vector_two_point_crossover(self):
+		length = 4
+		v1 = IntVector(SimpleFitness(), length, bounds=(1, 10))
+		v1.set_vector(list(range(1, 5)))
+		v2 = IntVector(SimpleFitness(), length, bounds=(1, 10))
+		v2.set_vector(list(range(5, 9)))
+		
+		# random sample will return [2, 3]
+		expected_v1 = [5, 6, 3, 8]
+		expected_v2 = [1, 2, 7, 4]
+
+		crossover = VectorKPointsCrossover(k=2)
+		crossover.apply([v1, v2])
+		assert v1.vector == expected_v1
+		assert v2.vector == expected_v2
+
+	def test_get_vector_part_last_cell(self):
+		length = 4
+		v1 = IntVector(SimpleFitness(), length, bounds=(1, 10))
+		v1.set_vector(list(range(1, 5)))
+		assert v1.get_vector_part(length - 1, length) == [4]
```

