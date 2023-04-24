# Comparing `tmp/unified_planning-0.5.0.93.dev1.tar.gz` & `tmp/unified_planning-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unified_planning-0.5.0.93.dev1.tar", last modified: Tue Jan 24 18:25:18 2023, max compression
+gzip compressed data, was "unified_planning-0.6.0.tar", last modified: Mon Apr 24 16:18:18 2023, max compression
```

## Comparing `unified_planning-0.5.0.93.dev1.tar` & `unified_planning-0.6.0.tar`

### file list

```diff
@@ -1,209 +1,360 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.664664 unified_planning-0.5.0.93.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-24 18:25:18.664664 unified_planning-0.5.0.93.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 18:25:18.664664 unified_planning-0.5.0.93.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.648664 unified_planning-0.5.0.93.dev1/unified_planning/
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.648664 unified_planning-0.5.0.93.dev1/unified_planning/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.648664 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    17366 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/credits.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    37012 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/meta_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.652664 unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/oneshot_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/oversubscription_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/engines/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.652664 unified_planning-0.5.0.93.dev1/unified_planning/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/grpc/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.652664 unified_planning-0.5.0.93.dev1/unified_planning/grpc/generated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/grpc/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29238 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/grpc/proto_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/grpc/proto_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.652664 unified_planning-0.5.0.93.dev1/unified_planning/interop/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16893 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/interop/from_tarski.py
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/interop/to_tarski.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.652664 unified_planning-0.5.0.93.dev1/unified_planning/io/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/io/anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    55978 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/io/pddl_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    34687 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/io/pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    26053 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/io/python_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.652664 unified_planning-0.5.0.93.dev1/unified_planning/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    39697 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/contingent_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/fnode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.656664 unified_planning-0.5.0.93.dev1/unified_planning/model/htn/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/htn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/htn/hierarchical_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/htn/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/htn/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/htn/task_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.656664 unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/actions_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/agents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/fluents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/objects_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/user_types_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.656664 unified_planning-0.5.0.93.dev1/unified_planning/model/multi_agent/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/multi_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/multi_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/multi_agent/ma_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/multi_agent/ma_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    39865 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/problem_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.656664 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/free_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/identitydag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/linear_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/operators_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/quantifier_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/state_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.656664 unified_planning-0.5.0.93.dev1/unified_planning/plans/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/plans/contingent_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/plans/partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/plans/sequential_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/plans/time_triggered_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    24091 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.660664 unified_planning-0.5.0.93.dev1/unified_planning/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.660664 unified_planning-0.5.0.93.dev1/unified_planning/test/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/examples/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14613 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/examples/minimals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/examples/multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    38705 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/examples/realistic.py
--rw-r--r--   0 runner    (1001) docker     (123)    30647 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/examples/testing_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.660664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.660664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/citycar/
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/citycar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/citycar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.660664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/counters/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/counters/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/counters/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/counters/problem2.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.660664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/depot/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/depot/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/depot/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/enhsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.660664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/htn-transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.660664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/matchcellar/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.660664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/miconic/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/miconic/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/miconic/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.664664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/robot_fastener/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.664664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/safe_road/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/safe_road/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/safe_road/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.664664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/sailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/sailing/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/sailing/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.664664 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/visit_precedence/
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_anytime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_compilers_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_contingent_pddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_credits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_infix_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    32310 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_pddl_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    25466 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_protobuf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_pyperplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_python_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_quantifier_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25132 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_simulated_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_tarski_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_trajectory_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-24 18:25:15.000000 unified_planning-0.5.0.93.dev1/unified_planning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:25:18.648664 unified_planning-0.5.0.93.dev1/unified_planning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-24 18:25:18.000000 unified_planning-0.5.0.93.dev1/unified_planning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-01-24 18:25:18.000000 unified_planning-0.5.0.93.dev1/unified_planning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 18:25:18.000000 unified_planning-0.5.0.93.dev1/unified_planning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-24 18:25:18.000000 unified_planning-0.5.0.93.dev1/unified_planning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-24 18:25:18.000000 unified_planning-0.5.0.93.dev1/unified_planning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.168364 unified_planning-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 16:18:15.000000 unified_planning-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-24 16:18:15.000000 unified_planning-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 16:18:18.168364 unified_planning-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-24 16:18:15.000000 unified_planning-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:18:18.168364 unified_planning-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-24 16:18:15.000000 unified_planning-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.140364 unified_planning-0.6.0/unified_planning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.144364 unified_planning-0.6.0/unified_planning/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.144364 unified_planning-0.6.0/unified_planning/engines/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17677 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18492 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/compilers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41064 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/meta_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.144364 unified_planning-0.6.0/unified_planning/engines/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/mixins/anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/mixins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/mixins/oneshot_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/mixins/plan_repairer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/mixins/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/mixins/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/mixins/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/mixins/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/oversubscription_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27821 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/engines/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.144364 unified_planning-0.6.0/unified_planning/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/grpc/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.144364 unified_planning-0.6.0/unified_planning/grpc/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/grpc/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35468 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/grpc/generated/unified_planning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32998 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/grpc/proto_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33343 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/grpc/proto_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.144364 unified_planning-0.6.0/unified_planning/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/interop/from_tarski.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/interop/to_tarski.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.148364 unified_planning-0.6.0/unified_planning/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/io/anml_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41213 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/io/anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/io/anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37842 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/io/ma_pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74227 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/io/pddl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37139 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/io/pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26929 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/io/python_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.148364 unified_planning-0.6.0/unified_planning/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28291 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/contingent_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/delta_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/fnode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.148364 unified_planning-0.6.0/unified_planning/model/htn/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/htn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/htn/hierarchical_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/htn/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/htn/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/htn/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/htn/task_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.148364 unified_planning-0.6.0/unified_planning/model/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/actions_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/agents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/fluents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/initial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/objects_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/time_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/timed_conds_effs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/mixins/user_types_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.152364 unified_planning-0.6.0/unified_planning/model/multi_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/multi_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/multi_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/multi_agent/ma_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/multi_agent/ma_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38729 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/problem_kind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.152364 unified_planning-0.6.0/unified_planning/model/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/scheduling/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/scheduling/chronicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/scheduling/scheduling_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.152364 unified_planning-0.6.0/unified_planning/model/tamp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/tamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/tamp/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/tamp/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/tamp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/tamp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.152364 unified_planning-0.6.0/unified_planning/model/walkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/expression_quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/fluents_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/free_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/identitydag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/linear_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/names_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/operators_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/quantifier_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/state_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/model/walkers/usertype_fluents_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.152364 unified_planning-0.6.0/unified_planning/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/plans/contingent_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/plans/hierarchical_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/plans/partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/plans/sequential_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/plans/stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/plans/time_triggered_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27425 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.156364 unified_planning-0.6.0/unified_planning/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/anml/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/basic.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/basic_conditional.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/connected_locations.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/constants.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/constants_no_variable_duration.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/durative_goals.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/forall.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/hierarchical_blocks_world.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/hydrone.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/match.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/match_int_id.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/match_test_parser.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/simple_mais.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/anml/tils.anml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.132364 unified_planning-0.6.0/unified_planning/test/contingent_pddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/contingent_pddl/colorballs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/contingent_pddl/colorballs/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/contingent_pddl/colorballs/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/contingent_pddl/logistic_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/examples/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/examples/minimals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/examples/multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38724 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/examples/realistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/examples/tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30699 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/examples/testing_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.140364 unified_planning-0.6.0/unified_planning/test/hddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-PCP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-PCP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Rover/
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Rover/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Satellite/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Childsnack/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Depots/
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Depots/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.160364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Factories-simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Hiking/
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Minecraft-Player/
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Minecraft-Regular/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Robot/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Rover-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Snake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Snake/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Towers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Towers/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Woodworking/
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/pddl/citycar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/citycar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/citycar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/pddl/counters/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/counters/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/counters/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/counters/problem2.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/pddl/depot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/depot/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/depot/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/enhsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.164364 unified_planning-0.6.0/unified_planning/test/pddl/htn-transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/htn-transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/htn-transport/problem.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.168364 unified_planning-0.6.0/unified_planning/test/pddl/matchcellar/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/matchcellar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/matchcellar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.168364 unified_planning-0.6.0/unified_planning/test/pddl/miconic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/miconic/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/miconic/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.168364 unified_planning-0.6.0/unified_planning/test/pddl/robot_fastener/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/robot_fastener/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/robot_fastener/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.168364 unified_planning-0.6.0/unified_planning/test/pddl/safe_road/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/safe_road/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/safe_road/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.168364 unified_planning-0.6.0/unified_planning/test/pddl/sailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/sailing/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/sailing/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.168364 unified_planning-0.6.0/unified_planning/test/pddl/visit_precedence/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/visit_precedence/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/pddl/visit_precedence/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.168364 unified_planning-0.6.0/unified_planning/test/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/scheduling/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/scheduling/jobshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27049 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_anytime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_compilers_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_contingent_pddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_expression_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_htn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_infix_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32858 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_pddl_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_protobuf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_pyperplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_python_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_quantifier_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_simulated_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_tarski_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_trajectory_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-24 16:18:15.000000 unified_planning-0.6.0/unified_planning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:18:18.140364 unified_planning-0.6.0/unified_planning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 16:18:17.000000 unified_planning-0.6.0/unified_planning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-04-24 16:18:18.000000 unified_planning-0.6.0/unified_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:18:17.000000 unified_planning-0.6.0/unified_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-24 16:18:17.000000 unified_planning-0.6.0/unified_planning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 16:18:17.000000 unified_planning-0.6.0/unified_planning.egg-info/top_level.txt
```

### Comparing `unified_planning-0.5.0.93.dev1/LICENSE` & `unified_planning-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/PKG-INFO` & `unified_planning-0.6.0/unified_planning.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unified_planning
-Version: 0.5.0.93.dev1
+Name: unified-planning
+Version: 0.6.0
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: UNKNOWN
 Keywords: planning logic STRIPS RDDL
@@ -22,8 +22,11 @@
 Provides-Extra: dev
 Provides-Extra: grpc
 Provides-Extra: tarski
 Provides-Extra: pyperplan
 Provides-Extra: tamer
 Provides-Extra: enhsp
 Provides-Extra: fast-downward
+Provides-Extra: lpg
+Provides-Extra: fmap
+Provides-Extra: aries
 Provides-Extra: engines
```

### Comparing `unified_planning-0.5.0.93.dev1/README.md` & `unified_planning-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         print("No plan found.")
 ```
 
 ## Documentation
 
 The documentation is available [here](https://unified-planning.readthedocs.io/en/latest/)
 
-## Notebooks
+## Examples
 
-More complex live demos are available as notebooks [here](notebooks/README.md).
+More complex examples are available as notebooks [here](https://unified-planning.readthedocs.io/en/latest/examples.html).
 
 
 ## Acknowledgments
 
 <img src="https://www.aiplan4eu-project.eu/wp-content/uploads/2021/07/euflag.png" width="60" height="40">
 
 This library is being developed for the AIPlan4EU H2020 project (https://aiplan4eu-project.eu) that is funded by the European Commission under grant agreement number 101016442.
```

### Comparing `unified_planning-0.5.0.93.dev1/setup.py` & `unified_planning-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,24 +21,30 @@
     include_package_data=True,
     python_requires=">=3.7",  # supported Python ranges
     install_requires=["pyparsing", "networkx"],
     extras_require={
         "dev": ["tarski[arithmetic]", "pytest", "pytest-cov", "mypy"],
         "grpc": ["grpcio", "grpcio-tools", "grpc-stubs"],
         "tarski": ["tarski[arithmetic]"],
-        "pyperplan": ["up-pyperplan==0.3.0"],
-        "tamer": ["up-tamer==0.3.1"],
-        "enhsp": ["up-enhsp==0.0.9"],
-        "fast-downward": ["up-fast-downward==0.1.1"],
+        "pyperplan": ["up-pyperplan==0.3.0.4.dev1"],
+        "tamer": ["up-tamer==0.3.1.22.dev1"],
+        "enhsp": ["up-enhsp==0.0.13"],
+        "fast-downward": ["up-fast-downward==0.2.1"],
+        "lpg": ["up-lpg==0.0.6.3"],
+        "fmap": ["up-fmap==0.0.6"],
+        "aries": ["up-aries>=0.0.8"],
         "engines": [
             "tarski[arithmetic]",
-            "up-pyperplan==0.3.0",
-            "up-tamer==0.3.1",
-            "up-enhsp==0.0.9",
-            "up-fast-downward==0.1.1",
+            "up-pyperplan==0.3.0.4.dev1",
+            "up-tamer==0.3.1.22.dev1",
+            "up-enhsp==0.0.13",
+            "up-fast-downward==0.2.1",
+            "up-lpg==0.0.6.3",
+            "up-fmap==0.0.6",
+            "up-aries>=0.0.8",
         ],
     },
     license="APACHE",
     keywords="planning logic STRIPS RDDL",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/__init__.py` & `unified_planning-0.6.0/unified_planning/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 if TYPE_CHECKING:
     # can't actually subclass Any at runtime
     AnyBaseClass = Any
 else:
     AnyBaseClass = object
 
 
-VERSION: Tuple[Union[int, str], ...] = (0, 5, 0)
+VERSION: Tuple[Union[int, str], ...] = (0, 6, 0)
 __version__ = ".".join(str(x) for x in VERSION)
 
 # Try to provide human-readable version of latest commit for dev versions
 # E.g. v0.5.1-4-g49a49f2-wip
 #      * 4 commits after tag v0.5.1
 #      * Latest commit "49a49f2"
 #      * -wip: Working tree is dirty (non committed stuff)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/__init__.py` & `unified_planning-0.6.0/unified_planning/engines/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,46 +28,51 @@
     LogMessage,
     PlanGenerationResult,
     LogLevel,
     PlanGenerationResultStatus,
     ValidationResult,
     ValidationResultStatus,
     CompilerResult,
+    FailedValidationReason,
 )
 from unified_planning.engines.sequential_simulator import (
-    SequentialSimulator,
-    InstantaneousEvent,
+    UPSequentialSimulator,
+    evaluate_quality_metric,
+    evaluate_quality_metric_in_initial_state,
+)
+from unified_planning.engines.mixins.sequential_simulator import (
+    SequentialSimulatorMixin,
 )
-from unified_planning.engines.mixins.simulator import SimulatorMixin, Event
 from unified_planning.engines.mixins.oneshot_planner import OptimalityGuarantee
 from unified_planning.engines.mixins.anytime_planner import AnytimeGuarantee
 from unified_planning.engines.mixins.compiler import CompilationKind
 from unified_planning.engines.mixins.portfolio import PortfolioSelectorMixin
 
 __all__ = [
     "Factory",
     "Grounder",
     "Parallel",
     "PDDLPlanner",
     "SequentialPlanValidator",
-    "SimulatorMixin",
-    "SequentialSimulator",
+    "SequentialSimulatorMixin",
+    "UPSequentialSimulator",
     "Event",
     "InstantaneousEvent",
     "Engine",
     "OptimalityGuarantee",
     "CompilationKind",
     "Credits",
     "Result",
     "LogMessage",
     "PlanGenerationResult",
     "LogLevel",
     "PlanGenerationResultStatus",
     "ValidationResult",
     "ValidationResultStatus",
+    "FailedValidationReason",
     "CompilerResult",
     "PortfolioSelectorMixin",
     "OperationMode",
     "AnytimeGuarantee",
     "MetaEngine",
     "OversubscriptionPlanner",
     "Replanner",
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/__init__.py` & `unified_planning-0.6.0/unified_planning/engines/compilers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+
+from unified_planning.engines.compilers.bounded_types_remover import BoundedTypesRemover
 from unified_planning.engines.compilers.conditional_effects_remover import (
     ConditionalEffectsRemover,
 )
 from unified_planning.engines.compilers.disjunctive_conditions_remover import (
     DisjunctiveConditionsRemover,
 )
 from unified_planning.engines.compilers.grounder import Grounder, GrounderHelper
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/compilers_pipeline.py` & `unified_planning-0.6.0/unified_planning/engines/compilers/compilers_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,24 @@
         map_back_functions.reverse()
         return CompilerResult(
             new_problem,
             partial(map_back_action_instance, map_back_functions=map_back_functions),
             self.name,
         )
 
+    def _compile(
+        self,
+        problem: "up.model.AbstractProblem",
+        compilation_kind: "up.engines.CompilationKind",
+    ) -> "up.engines.results.CompilerResult":
+        """Method called by :func:`~unified_planning.engines.mixins.CompilerMixin.compile` to get the returned :class:`~unified_planning.engines.CompilerResult`."""
+        raise UPUsageError(
+            "The CompilersPipeline does not implement the _compile method but overrides the compile method directly."
+        )
+
 
 def map_back_action_instance(
     action: ActionInstance,
     map_back_functions: List[Callable[[ActionInstance], ActionInstance]],
 ) -> Optional[ActionInstance]:
     for f in map_back_functions:
         action = f(action)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/conditional_effects_remover.py` & `unified_planning-0.6.0/unified_planning/engines/compilers/conditional_effects_remover.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 """This module defines the conditional effects remover class."""
 
 
 import unified_planning as up
 import unified_planning.engines as engines
 from unified_planning.engines.mixins.compiler import CompilationKind, CompilerMixin
+from unified_planning.engines.compilers.utils import updated_minimize_action_costs
 from unified_planning.engines.results import CompilerResult
 from unified_planning.exceptions import (
     UPProblemDefinitionError,
     UPConflictingEffectsException,
 )
 from unified_planning.model import Problem, ProblemKind
 from unified_planning.engines.compilers.utils import (
@@ -67,33 +68,47 @@
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
+        supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-        supported_kind.set_time("TIMED_EFFECT")
+        supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
+        supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
+        supported_kind.set_quality_metrics("ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_quality_metrics("PLAN_LENGTH")
+        supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
+        supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
+        supported_kind.set_quality_metrics("MAKESPAN")
+        supported_kind.set_quality_metrics("FINAL_VALUE")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind):
         return problem_kind <= ConditionalEffectsRemover.supported_kind()
 
     @staticmethod
@@ -123,15 +138,15 @@
         :param compilation_kind: The :class:`~unified_planning.engines.CompilationKind` that must be applied on the given problem;
             only :class:`~unified_planning.engines.CompilationKind.CONDITIONAL_EFFECTS_REMOVING` is supported by this compiler
         :return: The resulting :class:`~unified_planning.engines.results.CompilerResult` data structure.
         :raises: :exc:`~unified_planning.exceptions.UPProblemDefinitionError` when the :meth:`condition<unified_planning.model.Effect.condition>` of an
             :class:`~unified_planning.model.Effect` can't be removed without changing the :class:`~unified_planning.model.Problem` semantic.
         """
         assert isinstance(problem, Problem)
-        env = problem.env
+        env = problem.environment
         simplifier = env.simplifier
 
         new_to_old = {}
 
         new_problem = problem.clone()
         new_problem.name = f"{self.name}_{problem.name}"
         new_problem.clear_timed_effects()
@@ -167,15 +182,18 @@
                     for e in action.unconditional_effects:
                         new_action._add_effect_instance(e.clone())
                     for i, e in enumerate(cond_effects):
                         if i in p:
                             # positive precondition
                             new_action.add_precondition(e.condition)
                             ne = up.model.Effect(
-                                e.fluent, e.value, env.expression_manager.TRUE(), e.kind
+                                e.fluent,
+                                e.value,
+                                env.expression_manager.TRUE(),
+                                e.kind,
                             )
                             # We try to add the new effect, but it might be in conflict with exising effects,
                             # so the action is not added to the problem
                             try:
                                 new_action._add_effect_instance(ne)
                             except UPConflictingEffectsException:
                                 continue
@@ -211,15 +229,18 @@
                         for e in el:
                             new_action._add_effect_instance(t, e.clone())
                     for i, (e, t) in enumerate(cond_effects_timing):
                         if i in p:
                             # positive precondition
                             new_action.add_condition(t, e.condition)
                             ne = up.model.Effect(
-                                e.fluent, e.value, env.expression_manager.TRUE(), e.kind
+                                e.fluent,
+                                e.value,
+                                env.expression_manager.TRUE(),
+                                e.kind,
                             )
                             # We try to add the new effect, but it might be in conflict with exising effects,
                             # so the action is not added to the problem
                             try:
                                 new_action._add_effect_instance(t, ne)
                             except UPConflictingEffectsException:
                                 continue
@@ -241,10 +262,21 @@
                             for interval, c in simplified_conditions:
                                 new_action.add_condition(interval, c)
                             new_to_old[new_action] = action
                             new_problem.add_action(new_action)
             else:
                 raise NotImplementedError
 
+        new_problem.clear_quality_metrics()
+        for qm in problem.quality_metrics:
+            if qm.is_minimize_action_costs():
+                new_problem.add_quality_metric(
+                    updated_minimize_action_costs(
+                        qm, new_to_old, new_problem.environment
+                    )
+                )
+            else:
+                new_problem.add_quality_metric(qm)
+
         return CompilerResult(
             new_problem, partial(replace_action, map=new_to_old), self.name
         )
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py` & `unified_planning-0.6.0/unified_planning/engines/compilers/disjunctive_conditions_remover.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,33 +10,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines the dnf remover class."""
 
+from fractions import Fraction
 import unified_planning as up
 import unified_planning.engines as engines
 from unified_planning.engines.mixins.compiler import CompilationKind, CompilerMixin
-from unified_planning.engines.compilers.utils import get_fresh_name, replace_action
+from unified_planning.engines.compilers.utils import (
+    get_fresh_name,
+    replace_action,
+    updated_minimize_action_costs,
+)
 from unified_planning.engines.results import CompilerResult
 from unified_planning.exceptions import UPProblemDefinitionError
 from unified_planning.model import (
     FNode,
     Problem,
+    BoolExpression,
+    NumericConstant,
     InstantaneousAction,
     DurativeAction,
     TimeInterval,
     Timing,
     Action,
     ProblemKind,
     Oversubscription,
+    TemporalOversubscription,
 )
 from unified_planning.model.walkers import Dnf
-from typing import List, Optional, Tuple, Dict, cast
+from typing import List, Optional, Tuple, Dict, Union, cast
 from itertools import product
 from functools import partial
 
 
 class DisjunctiveConditionsRemover(engines.engine.Engine, CompilerMixin):
     """
     DisjunctiveConditions remover class: this class offers the capability
@@ -62,36 +70,45 @@
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
+        supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-        supported_kind.set_time("TIMED_EFFECT")
+        supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
+        supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
+        supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind):
         return problem_kind <= DisjunctiveConditionsRemover.supported_kind()
@@ -120,15 +137,15 @@
         :param problem: The instance of the `Problem` that must be returned without disjunctive conditions.
         :param compilation_kind: The `CompilationKind` that must be applied on the given problem;
             only `DISJUNCTIVE_CONDITIONS_REMOVING` is supported by this compiler
         :return: The resulting `CompilerResult` data structure.
         """
         assert isinstance(problem, Problem)
 
-        env = problem.env
+        env = problem.environment
 
         new_to_old: Dict[Action, Optional[Action]] = {}
         new_fluents: List["up.model.Fluent"] = []
 
         new_problem = problem.clone()
         new_problem.name = f"{self.name}_{problem.name}"
         new_problem.clear_actions()
@@ -201,25 +218,14 @@
                 new_to_old,
                 new_fluents,
                 gl,
                 t,
             )
             new_problem.add_timed_goal(t, goal_to_add)
 
-        for qm in problem.quality_metrics:
-            if isinstance(qm, Oversubscription):
-                new_oversubscription = {}
-                for g, v in qm.goals.items():
-                    new_goal = self._goals_without_disjunctions_adding_new_elements(
-                        dnf, new_problem, new_to_old, new_fluents, [g]
-                    )
-                    new_oversubscription[new_goal] = v
-                new_problem.add_quality_metric(Oversubscription(new_oversubscription))
-            else:
-                new_problem.add_quality_metric(qm)
         # Every meaningful action must set to False every new fluent added.
         # For the DurativeActions this must happen every time the action modifies something
         em = env.expression_manager
         # new_effects is the List of effects that must be added to every meaningful action
         new_effects: List["up.model.Effect"] = [
             up.model.Effect(em.FluentExp(f), em.FALSE(), em.TRUE()) for f in new_fluents
         ]
@@ -233,28 +239,68 @@
                 for tim in a.effects:
                     for e in new_effects:
                         a._add_effect_instance(tim, e)
             else:
                 raise NotImplementedError
             new_to_old[a] = old_action
 
+        for qm in problem.quality_metrics:
+            if qm.is_minimize_action_costs():
+                new_problem.add_quality_metric(
+                    updated_minimize_action_costs(
+                        qm, new_to_old, new_problem.environment
+                    )
+                )
+            elif qm.is_oversubscription():
+                assert isinstance(qm, Oversubscription)
+                new_oversubscription: Dict[BoolExpression, NumericConstant] = {}
+                for g, v in qm.goals.items():
+                    new_goal = self._goals_without_disjunctions_adding_new_elements(
+                        dnf, new_problem, new_to_old, new_fluents, [g]
+                    )
+                    new_oversubscription[new_goal] = v
+                new_problem.add_quality_metric(
+                    Oversubscription(
+                        new_oversubscription, environment=new_problem.environment
+                    )
+                )
+            elif qm.is_temporal_oversubscription():
+                assert isinstance(qm, TemporalOversubscription)
+                new_temporal_oversubscription: Dict[
+                    Tuple["up.model.timing.TimeInterval", "up.model.BoolExpression"],
+                    NumericConstant,
+                ] = {}
+                for (t, g), v in qm.goals.items():
+                    new_goal = self._goals_without_disjunctions_adding_new_elements(
+                        dnf, new_problem, new_to_old, new_fluents, [g]
+                    )
+                    new_temporal_oversubscription[(t, new_goal)] = v
+                new_problem.add_quality_metric(
+                    TemporalOversubscription(
+                        new_temporal_oversubscription,
+                        environment=new_problem.environment,
+                    )
+                )
+            else:
+                new_problem.add_quality_metric(qm)
+
         return CompilerResult(
             new_problem, partial(replace_action, map=new_to_old), self.name
         )
 
     def _goals_without_disjunctions_adding_new_elements(
         self,
         dnf: Dnf,
         new_problem: "up.model.Problem",
         new_to_old: Dict[Action, Optional[Action]],
         new_fluents: List["up.model.Fluent"],
         goals: List["up.model.FNode"],
         timing: Optional["up.model.timing.TimeInterval"] = None,
     ) -> "up.model.FNode":
-        env = new_problem.env
+        env = new_problem.environment
         new_goal = dnf.get_dnf_expression(env.expression_manager.And(goals))
         if new_goal.is_or():
             new_name = self.name if timing is None else f"{self.name}_timed"
             fake_fluent = up.model.Fluent(
                 get_fresh_name(new_problem, f"{new_name}_fake_goal")
             )
             fake_action = InstantaneousAction(f"{new_name}_fake_action", _env=env)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/grounder.py` & `unified_planning-0.6.0/unified_planning/engines/compilers/grounder.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,18 +24,17 @@
     Problem,
     ProblemKind,
     Action,
     Type,
     Expression,
     FNode,
     MinimizeActionCosts,
-    Parameter,
 )
 from unified_planning.model.types import domain_size, domain_item
-from unified_planning.model.walkers import Substituter, Simplifier
+from unified_planning.model.walkers import Simplifier
 from unified_planning.engines.compilers.utils import (
     lift_action_instance,
     create_action_with_given_subs,
 )
 from unified_planning.exceptions import UPUsageError
 from typing import Dict, Iterable, List, Optional, Tuple, Iterator, cast
 from itertools import product
@@ -64,18 +63,18 @@
         Creates an instance of the GrounderHelper.
 
         :param problem: The `Problem` to ground.
         :param grounding_actions_map: Optionally, a map from `Action` to a List of Tuples of expressions.
             When this map is set, it represents the groundings that this class does.
             So, for every key in the map, the `Action` is grounded with every `tuple of parameters` in the mapped value.
             For example, if the map is `{a: [(o1, o2), (o2, o3)], b: [(o3), (o4)]}`, the resulting grounded actions will be:
-            - `a (o1, o2)`
-            - `a (o2, o3)`
-            - `b (o3)`
-            - `b (o4)`
+            * `a (o1, o2)`
+            * `a (o2, o3)`
+            * `b (o3)`
+            * `b (o4)`
             If this map is `None`, the `unified_planning` grounding algorithm is applied.
         """
         assert isinstance(problem, Problem)
         self._problem = problem
         self._grounding_actions_map = grounding_actions_map
         # grounded_actions is a map from an Action of the original problem and it's parameters
         # to the grounded instance of the Action with the given parameters.
@@ -84,42 +83,37 @@
         # An Action is meaningless when:
         # - it has no effects
         # - his conditions create a contradiction
         # - the action has conflicting effects
         self._grounded_actions: Dict[
             Tuple[Action, Tuple[FNode, ...]], Optional[Action]
         ] = {}
-        env = problem.env
-        self._substituter = Substituter(env)
+        env = problem.environment
         self._simplifier = Simplifier(env, problem)
 
     @property
-    def substituter(self) -> Substituter:
-        return self._substituter
-
-    @property
     def simplifier(self) -> Simplifier:
         return self._simplifier
 
     def ground_action(
         self, action: Action, parameters: Tuple[FNode, ...] = tuple()
     ) -> Optional[Action]:
         """
-        Grounds the given `action` with the given `parameters`.
-        An `Action` is grounded when it has no :func:`parameters <unified_planning.model.Action.parameters>`.
+        Grounds the given action with the given parameters.
+        An ``Action`` is grounded when it has no :func:`parameters <unified_planning.model.Action.parameters>`.
 
-        The returned `Action` is cached, so if the same method is called twice with the same function parameters,
+        The returned ``Action`` is cached, so if the same method is called twice with the same function parameters,
         the same object is returned, and the same object will be returned in the total problem grounding, so
-        if the resulting `Action` or :class:`~unified_planning.model.Problem` are modified, all the copies
+        if the resulting ``Action`` or :class:`~unified_planning.model.Problem` are modified, all the copies
         returned by this class will be modified.
 
-        :param action: The `Action` that must be grounded with the given `parameters`.
-        :param parameters: The tuple of expressions used to ground the given `action`.
-        :return: The `action` grounded with the given `parameters` or `None` if the grounded
-            action does not have `effects` or the `action conditions` can be easily evaluated as a
+        :param action: The ``Action`` that must be grounded with the given ``parameters``.
+        :param parameters: The tuple of expressions used to ground the given ``action``.
+        :return: The ``action`` grounded with the given ``parameters`` or ``None`` if the grounded
+            action does not have ``effects`` or the ``action conditions`` can be easily evaluated as a
             contradiction.
         """
         assert len(action.parameters) == len(
             parameters
         ), "The number of given parameters for the grounding is different from the action's parameters"
         key = (action, tuple(parameters))
         value = self._grounded_actions.get(key, 0)
@@ -137,31 +131,32 @@
                 else:
                     new_action = None
             else:
                 subs: Dict[Expression, Expression] = dict(
                     zip(action.parameters, list(parameters))
                 )
                 new_action = create_action_with_given_subs(
-                    self._problem, action, self._simplifier, self._substituter, subs
+                    self._problem, action, self._simplifier, subs
                 )
             self._grounded_actions[key] = new_action
             return new_action
 
     def get_grounded_actions(
         self,
     ) -> Iterator[Tuple[Action, Tuple[FNode, ...], Optional[Action]]]:
         """
-        Returns an `Iterator` over all the possible grounded `Actions` of the `Problem` given at construction time.
-        Every resulting `Tuple` is made of 3 elements: `original_action`, `parameters`, `grounded_action` where:
-            - The `original_action` is the `Action` of the `Problem` that is grounded.
-            - The `parameters` is the `Tuple of expressions` used to ground the `original_action`.
-            - The `grounded_action` is the `Action` created by grounding the `original_action` with the given `parameters`;
-                the `grounded_action` can be `None` if the grounding of the `original_action` with the given parameters
-                creates an invalid or meaningless `Action` (invalid if it has conflicting `Effects`,
-                meaningless if it has no `effects` or contradicting `conditions`).
+        Returns an iterator over all the possible grounded actions of the problem given at construction time.
+        Every resulting tuple is made of 3 elements: ``original_action``, ``parameters``, ``grounded_action`` where:
+
+        * The ``original_action`` is the `Action` of the ``Problem`` that is grounded.
+        * The ``parameters`` is the `Tuple of expressions` used to ground the ``original_action``.
+        * The ``grounded_action`` is the `Action` created by grounding the ``original_action`` with the given ``parameters``;
+        the ``grounded_action`` can be ``None`` if the grounding of the ``original_action`` with the given parameters
+        creates an invalid or meaningless `Action` (invalid if it has conflicting `Effects`,
+        meaningless if it has no `effects` or contradicting `conditions`).
         """
         for old_action in self._problem.actions:
             for grounded_params in self.get_possible_parameters(old_action):
                 assert isinstance(grounded_params, tuple)
                 new_action = self.ground_action(old_action, grounded_params)
                 yield (old_action, grounded_params, new_action)
 
@@ -246,39 +241,48 @@
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
+        supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-        supported_kind.set_time("TIMED_EFFECT")
+        supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
+        supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATION")
-        supported_kind.set_expression_duration("FLUENTS_IN_DURATION")
+        supported_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
+        supported_kind.set_expression_duration("FLUENTS_IN_DURATIONS")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
+        supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind):
         return problem_kind <= Grounder.supported_kind()
@@ -323,32 +327,49 @@
         ) in grounder_helper.get_grounded_actions():
             if new_action is not None:
                 new_problem.add_action(new_action)
                 trace_back_map[new_action] = (old_action, list(parameters))
 
         new_problem.clear_quality_metrics()
         for qm in problem.quality_metrics:
-            if isinstance(qm, MinimizeActionCosts):
-                substituter = grounder_helper.substituter
-                simplifier = grounder_helper.simplifier
-                new_costs: Dict[Action, Optional[FNode]] = {}
-                for new_action, (old_action, params) in trace_back_map.items():
-                    subs = cast(
-                        Dict[Expression, Expression],
-                        dict(zip(old_action.parameters, params)),
-                    )
-                    old_cost = qm.get_action_cost(old_action)
-                    if old_cost is None:
-                        new_costs[new_action] = None
-                    else:
-                        new_costs[new_action] = simplifier.simplify(
-                            substituter.substitute(old_cost, subs)
-                        )
-                new_problem.add_quality_metric(MinimizeActionCosts(new_costs))
+            if qm.is_minimize_action_costs():
+                assert isinstance(qm, MinimizeActionCosts)
+                new_metric = ground_minimize_action_costs_metric(
+                    qm, trace_back_map, grounder_helper.simplifier
+                )
+                new_problem.add_quality_metric(new_metric)
             else:
                 new_problem.add_quality_metric(qm)
 
         return CompilerResult(
             new_problem,
             partial(lift_action_instance, map=trace_back_map),
             self.name,
         )
+
+
+def ground_minimize_action_costs_metric(
+    metric: MinimizeActionCosts,
+    trace_back_map: Dict[Action, Tuple[Action, List[FNode]]],
+    simplifier: Simplifier,
+) -> MinimizeActionCosts:
+    """
+    Support method for a grounder to handle the MinimizeActionCosts metric.
+
+    :param metric: The metric to convert.
+    :param trace_back_map: The grounding map from a grounded Action to the Action
+        and parameters that created the grounded action.
+    :param simplifier: The simplifier used to evaluate the cost; if this simplifier
+        has the Instance of the problem at construction time, it will also substitute
+        the static fluents in the action cost with their value.
+    :return: The equivalent MinimizeActionCosts metric for the grounded problem.
+    """
+    new_costs: Dict[Action, Expression] = {}
+    for new_action, (old_action, params) in trace_back_map.items():
+        subs = cast(
+            Dict[Expression, Expression],
+            dict(zip(old_action.parameters, params)),
+        )
+        old_cost = metric.get_action_cost(old_action)
+        if old_cost is not None:
+            new_costs[new_action] = simplifier.simplify(old_cost.substitute(subs))
+    return MinimizeActionCosts(new_costs)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/negative_conditions_remover.py` & `unified_planning-0.6.0/unified_planning/engines/compilers/negative_conditions_remover.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,31 +22,35 @@
     Fluent,
     Problem,
     InstantaneousAction,
     DurativeAction,
     FNode,
     Action,
     Effect,
-    Timing,
     ProblemKind,
     Oversubscription,
+    TemporalOversubscription,
 )
 from unified_planning.model.walkers.identitydag import IdentityDagWalker
-from unified_planning.engines.compilers.utils import get_fresh_name, replace_action
+from unified_planning.engines.compilers.utils import (
+    get_fresh_name,
+    replace_action,
+    updated_minimize_action_costs,
+)
 from unified_planning.exceptions import (
     UPExpressionDefinitionError,
     UPProblemDefinitionError,
 )
 from typing import List, Dict, Union, Optional
 from functools import partial
 
 
 class NegativeFluentRemover(IdentityDagWalker):
-    def __init__(self, problem, env):
-        self._env = env
+    def __init__(self, problem, environment):
+        self._env = environment
         IdentityDagWalker.__init__(self, self._env)
         self._fluent_mapping: Dict[Fluent, Fluent] = {}
         self._problem = problem
 
     def remove_negative_fluents(self, expression: FNode) -> FNode:
         return self.walk(expression)
 
@@ -99,35 +103,44 @@
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
+        supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-        supported_kind.set_time("TIMED_EFFECT")
+        supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
+        supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
         supported_kind.set_quality_metrics("ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
+        supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind):
         return problem_kind <= NegativeConditionsRemover.supported_kind()
@@ -156,15 +169,15 @@
         :param problem: The instance of the `Problem` to compile.
         :param compilation_kind: The `CompilationKind` that must be applied on the given `problem`;
             only `NEGATIVE_CONDITIONS_REMOVING` is supported by this compiler
         :return: The resulting `CompilerResult`.
         """
         assert isinstance(problem, Problem)
 
-        env = problem.env
+        env = problem.environment
         simplifier = env.simplifier
 
         fluent_remover = NegativeFluentRemover(problem, env)
 
         new_to_old: Dict[Action, Action] = {}
 
         new_problem = Problem(f"{self.name}_{problem.name}", env)
@@ -217,21 +230,40 @@
                 new_problem.add_timed_goal(i, ng)
 
         for g in problem.goals:
             ng = fluent_remover.remove_negative_fluents(g)
             new_problem.add_goal(ng)
 
         for qm in problem.quality_metrics:
-            if isinstance(qm, Oversubscription):
+            if qm.is_minimize_action_costs():
+                new_problem.add_quality_metric(
+                    updated_minimize_action_costs(
+                        qm, new_to_old, new_problem.environment
+                    )
+                )
+            elif qm.is_oversubscription():
+                assert isinstance(qm, Oversubscription)
                 new_problem.add_quality_metric(
                     Oversubscription(
                         {
                             fluent_remover.remove_negative_fluents(g): v
                             for g, v in qm.goals.items()
-                        }
+                        },
+                        environment=new_problem.environment,
+                    )
+                )
+            elif qm.is_temporal_oversubscription():
+                assert isinstance(qm, TemporalOversubscription)
+                new_problem.add_quality_metric(
+                    TemporalOversubscription(
+                        {
+                            (t, fluent_remover.remove_negative_fluents(g)): v
+                            for (t, g), v in qm.goals.items()
+                        },
+                        environment=new_problem.environment,
                     )
                 )
             else:
                 new_problem.add_quality_metric(qm)
 
         # fluent_mapping is the map between a fluent and it's negation, when the
         # negation is None it means the fluent is never found in a negation into
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/quantifiers_remover.py` & `unified_planning-0.6.0/unified_planning/engines/compilers/quantifiers_remover.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,34 +22,45 @@
 from unified_planning.model import (
     Problem,
     InstantaneousAction,
     DurativeAction,
     Action,
     ProblemKind,
     Oversubscription,
+    TemporalOversubscription,
 )
 from unified_planning.model.walkers import ExpressionQuantifiersRemover
-from unified_planning.engines.compilers.utils import get_fresh_name, replace_action
+from unified_planning.engines.compilers.utils import (
+    get_fresh_name,
+    replace_action,
+    updated_minimize_action_costs,
+)
 from typing import Dict, Optional
 from functools import partial
 
 
 class QuantifiersRemover(engines.engine.Engine, CompilerMixin):
-    """Quantifiers remover class: this class offers the capability
+    """
+    Quantifiers remover class: this class offers the capability
     to transform a problem with quantifiers into a problem without.
     Every quantifier is compiled away by it's respective logic formula
     instantiated on object.
+
     For example the formula:
-        Forall (s-sempahore) is_green(s)
-    in a problem with 3 objects of type semaphores {s1, s2, s3} is compiled in:
-        And(is_green(s1), is_green(s2), is_green(s3)).
+        ``Forall (s-sempahore) is_green(s)``
+
+    in a problem with 3 objects of type ``semaphores {s1, s2, s3}`` is compiled in:
+        ``And(is_green(s1), is_green(s2), is_green(s3))``
+
     While the respective formula on the same problem:
-        Exists (s-semaphore) is_green(s)
+        ``Exists (s-semaphore) is_green(s)``
+
     becomes:
-        Or(is_green(s1), is_green(s2), is_green(s3))."""
+        ``Or(is_green(s1), is_green(s2), is_green(s3))``
+    """
 
     def __init__(self):
         engines.engine.Engine.__init__(self)
         CompilerMixin.__init__(self, CompilationKind.QUANTIFIERS_REMOVING)
 
     @property
     def name(self):
@@ -59,36 +70,45 @@
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
+        supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-        supported_kind.set_time("TIMED_EFFECT")
+        supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
+        supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
+        supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind):
         return problem_kind <= QuantifiersRemover.supported_kind()
@@ -114,21 +134,22 @@
         """
         Takes an instance of a up.model.Problem and the up.engines.CompilationKind.QUANTIFIERS_REMOVING
         and returns a CompilerResult where the problem does not have universal or existential (Forall or Exists)
         operands; The quantifiers are substituted with their grounded version by using the problem's objects.
 
         :param problem: The instance of the up.model.Problem that must be returned without quantifiers.
         :param compilation_kind: The up.engines.CompilationKind that must be applied on the given problem;
-        only QUANTIFIERS_REMOVING is supported by this compiler
+            only QUANTIFIERS_REMOVING is supported by this compiler
         :return: The resulting up.engines.results.CompilerResult data structure.
         """
         assert isinstance(problem, Problem)
 
-        env = problem.env
-        expression_quantifier_remover = ExpressionQuantifiersRemover(env)
+        expression_quantifier_remover = ExpressionQuantifiersRemover(
+            problem.environment
+        )
 
         new_to_old: Dict[Action, Action] = {}
 
         new_problem = problem.clone()
         new_problem.name = f"{self.name}_{problem.name}"
         new_problem.clear_timed_goals()
         new_problem.clear_goals()
@@ -201,23 +222,47 @@
             for g in gl:
                 ng = expression_quantifier_remover.remove_quantifiers(g, problem)
                 new_problem.add_timed_goal(i, ng)
         for g in problem.goals:
             ng = expression_quantifier_remover.remove_quantifiers(g, problem)
             new_problem.add_goal(ng)
         for qm in problem.quality_metrics:
-            if isinstance(qm, Oversubscription):
+            if qm.is_minimize_action_costs():
+                new_problem.add_quality_metric(
+                    updated_minimize_action_costs(
+                        qm, new_to_old, new_problem.environment
+                    )
+                )
+            elif qm.is_oversubscription():
+                assert isinstance(qm, Oversubscription)
                 new_problem.add_quality_metric(
                     Oversubscription(
                         {
                             expression_quantifier_remover.remove_quantifiers(
                                 g, problem
                             ): v
                             for g, v in qm.goals.items()
-                        }
+                        },
+                        environment=new_problem.environment,
+                    )
+                )
+            elif qm.is_temporal_oversubscription():
+                assert isinstance(qm, TemporalOversubscription)
+                new_problem.add_quality_metric(
+                    TemporalOversubscription(
+                        {
+                            (
+                                i,
+                                expression_quantifier_remover.remove_quantifiers(
+                                    g, problem
+                                ),
+                            ): v
+                            for (i, g), v in qm.goals.items()
+                        },
+                        environment=new_problem.environment,
                     )
                 )
             else:
                 new_problem.add_quality_metric(qm)
 
         return CompilerResult(
             new_problem, partial(replace_action, map=new_to_old), self.name
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/tarski_grounder.py` & `unified_planning-0.6.0/unified_planning/engines/compilers/tarski_grounder.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,21 +66,22 @@
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
+        supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind: "unified_planning.model.ProblemKind") -> bool:
         return problem_kind <= TarskiGrounder.supported_kind()
@@ -131,20 +132,27 @@
             parameters = {parameter.name: parameter for parameter in action.parameters}
             grounded_actions_map[action] = []
             for tuple_of_parameters in list_of_tuple_of_parameters:
                 temp_list_of_converted_parameters = []
                 for p in tuple_of_parameters:
                     if isinstance(p, str):
                         temp_list_of_converted_parameters.append(
-                            problem.env.expression_manager.ObjectExp(problem.object(p))
+                            problem.environment.expression_manager.ObjectExp(
+                                problem.object(p)
+                            )
                         )
                     else:
                         temp_list_of_converted_parameters.append(
                             convert_tarski_formula(
-                                problem.env, fluents, objects, parameters, types, p
+                                problem.environment,
+                                fluents,
+                                objects,
+                                parameters,
+                                types,
+                                p,
                             )
                         )
                 grounded_actions_map[action].append(
                     tuple(temp_list_of_converted_parameters)
                 )
         up_grounder = Grounder(grounding_actions_map=grounded_actions_map)
         up_res = up_grounder.compile(problem, compilation_kind)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py` & `unified_planning-0.6.0/unified_planning/engines/compilers/trajectory_constraints_remover.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import unified_planning as up
 import unified_planning.engines as engines
 from unified_planning.exceptions import UPProblemDefinitionError
 from unified_planning.engines.mixins.compiler import CompilationKind, CompilerMixin
 from unified_planning.engines.results import CompilerResult
 from unified_planning.model import InstantaneousAction, Action, FNode, Fluent
 from unified_planning.model.walkers import Substituter, ExpressionQuantifiersRemover
-from unified_planning.model import Problem, ProblemKind
+from unified_planning.model import Problem, ProblemKind, MinimizeActionCosts
 from unified_planning.model.operators import OperatorKind
 from functools import partial
 from unified_planning.engines.compilers.utils import (
     lift_action_instance,
 )
 from typing import List, Dict, Tuple, Optional
 
@@ -81,80 +81,86 @@
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
+        supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
-        supported_kind.set_time("CONTINUOUS_TIME")
-        supported_kind.set_time("DISCRETE_TIME")
-        supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-        supported_kind.set_time("TIMED_EFFECT")
-        supported_kind.set_time("TIMED_GOALS")
-        supported_kind.set_time("DURATION_INEQUALITIES")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_quality_metrics("ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_quality_metrics("FINAL_VALUE")
+        supported_kind.set_quality_metrics("MAKESPAN")
+        supported_kind.set_quality_metrics("PLAN_LENGTH")
+        supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
+        supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         return supported_kind
 
     def _compile(
         self,
         problem: "up.model.AbstractProblem",
         compilation_kind: "up.engines.CompilationKind",
     ) -> CompilerResult:
         """
         Takes an instance of a :class:`~unified_planning.model.Problem` and the `TRAJECTORY_CONSTRAINTS_REMOVING` :class:`~unified_planning.engines.CompilationKind`
-        and returns a `CompilerResult` where the problem whitout trajectory_constraints.
+        and returns a `CompilerResult` where the problem without trajectory_constraints.
 
-        :param problem: The instance of the `Problem` that contains the trajecotry constraints.
+        :param problem: The instance of the `Problem` that contains the trajectory constraints.
         :param compilation_kind: The `CompilationKind` that must be applied on the given problem;
             only `TRAJECTORY_CONSTRAINTS_REMOVING` is supported by this compiler
         :return: The resulting `CompilerResult` data structure.
         """
         assert isinstance(problem, Problem)
-        env = problem.env
-        substituter = Substituter(env)
-        expression_quantifier_remover = ExpressionQuantifiersRemover(problem.env)
+        env = problem.environment
+        expression_quantifier_remover = ExpressionQuantifiersRemover(env)
         grounding_result = engines.compilers.grounder.Grounder().compile(
             problem, CompilationKind.GROUNDING
         )
         assert isinstance(grounding_result.problem, Problem)
-        problem = grounding_result.problem.clone()
-        assert isinstance(problem, Problem)
-        problem.name = f"{self.name}_{problem.name}"
-        A = problem.actions
-        I = problem.initial_values
+        grounded_problem = grounding_result.problem
+        new_problem = grounded_problem.clone()
+        assert isinstance(new_problem, Problem)
+        new_problem.name = f"{self.name}_{problem.name}"
+        I = new_problem.initial_values
         C = []
-        for c in problem.trajectory_constraints:
-            new_c = expression_quantifier_remover.remove_quantifiers(c, problem)
+        for c in new_problem.trajectory_constraints:
+            new_c = expression_quantifier_remover.remove_quantifiers(c, new_problem)
             if new_c.is_and():
                 C.extend(new_c.args)
             else:
                 C.append(new_c)
         # create a list that contains trajectory_constraints
         # trajectory_constraints can contain quantifiers and need to be remove
         relevancy_dict = self._build_relevancy_dict(env, C)
         A_prime: List["up.model.effect.Effect"] = list()
-        I_prime, F_prime = self._get_monitoring_atoms(env, substituter, C, I)
+        I_prime, F_prime = self._get_monitoring_atoms(env, C, I)
         G_prime = env.expression_manager.And(
             [self._monitoring_atom_dict[c] for c in self._get_landmark_constraints(C)]
         )
         trace_back_map: Dict[Action, Tuple[Action, List[FNode]]] = {}
         assert isinstance(grounding_result.map_back_action_instance, partial)
         map_grounded_action = grounding_result.map_back_action_instance.keywords["map"]
-        for a in A:
+        for a in new_problem.actions:
             map_value = map_grounded_action[a]
             assert isinstance(a, InstantaneousAction)
             E: List["up.model.effect.Effect"] = list()
             # create an empty list to store the new effects for each trajectory constraints
             relevant_constraints = self._get_relevant_constraints(a, relevancy_dict)
             for c in relevant_constraints:
                 # manage the action for each trajectory_constraints that is relevant
@@ -188,29 +194,44 @@
             for eff in E:
                 a.effects.append(eff)
             if env.expression_manager.FALSE() not in a.preconditions:
                 A_prime.append(a)
             trace_back_map[a] = map_value
         # create new problem to return
         # adding new fluents, goal, initial values and actions
-        G_new = (env.expression_manager.And(problem.goals, G_prime)).simplify()
-        problem.clear_goals()
-        problem.add_goal(G_new)
-        problem.clear_trajectory_constraints()
+        G_new = (env.expression_manager.And(new_problem.goals, G_prime)).simplify()
+        new_problem.clear_goals()
+        new_problem.add_goal(G_new)
+        new_problem.clear_trajectory_constraints()
         for fluent in F_prime:
-            problem.add_fluent(fluent)
-        problem.clear_actions()
+            new_problem.add_fluent(fluent)
+        new_problem.clear_actions()
         for action in A_prime:
-            problem.add_action(action)
+            new_problem.add_action(action)
         for init_val in I_prime:
-            problem.set_initial_value(
+            new_problem.set_initial_value(
                 up.model.Fluent(f"{init_val}", env.type_manager.BoolType()), True
             )
+
+        new_problem.clear_quality_metrics()
+        for qm in grounded_problem.quality_metrics:
+            if qm.is_minimize_action_costs():
+                assert isinstance(qm, MinimizeActionCosts)
+                new_costs = {
+                    na: qm.get_action_cost(grounded_problem.action(na.name))
+                    for na in new_problem.actions
+                }
+                new_problem.add_quality_metric(
+                    MinimizeActionCosts(new_costs), environment=new_problem.environment
+                )
+            else:
+                new_problem.add_quality_metric(qm)
+
         return CompilerResult(
-            problem, partial(lift_action_instance, map=trace_back_map), self.name
+            new_problem, partial(lift_action_instance, map=trace_back_map), self.name
         )
 
     def _manage_sa_compilation(self, env, phi, psi, m_atom, a, E):
         R1 = (self._regression(env, phi, a)).simplify()
         R2 = (self._regression(env, psi, a)).simplify()
         if phi != R1 or psi != R2:
             cond = (
@@ -286,67 +307,63 @@
         for eff in a.effects:
             constr = relevancy_dict.get(eff.fluent, [])
             for c in constr:
                 if c not in relevant_constrains:
                     relevant_constrains.append(c)
         return relevant_constrains
 
-    def _evaluate_constraint(self, env, substituter, constr, init_values):
+    def _evaluate_constraint(self, env, constr, init_values):
         if constr.is_sometime():
-            return HOLD, substituter.substitute(constr.args[0], init_values).simplify()
+            return HOLD, constr.args[0].substitute(init_values).simplify()
         elif constr.is_sometime_after():
             return (
                 HOLD,
                 env.expression_manager.Or(
-                    substituter.substitute(constr.args[1], init_values),
-                    env.expression_manager.Not(
-                        substituter.substitute(constr.args[0], init_values)
-                    ),
+                    constr.args[1].substitute(init_values),
+                    env.expression_manager.Not(constr.args[0].substitute(init_values)),
                 ).simplify(),
             )
         elif constr.is_sometime_before():
             return (
                 SEEN_PSI,
-                substituter.substitute(constr.args[1], init_values).simplify(),
+                constr.args[1].substitute(init_values).simplify(),
             )
         elif constr.is_at_most_once():
             return (
                 SEEN_PHI,
-                substituter.substitute(constr.args[0], init_values).simplify(),
+                constr.args[0].substitute(init_values).simplify(),
             )
         elif constr.is_bool_constant():
-            return None, substituter.substitute(constr)
+            return None, constr
         else:
-            return None, substituter.substitute(constr.args[0], init_values).simplify()
+            return None, constr.args[0].substitute(init_values).simplify()
 
-    def _get_monitoring_atoms(self, env, substituter, C, I):
+    def _get_monitoring_atoms(self, env, C, I):
         monitoring_atoms = []
         monitoring_atoms_counter = 0
         initial_state_prime = []
         for constr in C:
             if constr.is_always():
-                if substituter.substitute(constr.args[0], I).simplify().is_false():
+                if constr.args[0].substitute(I).simplify().is_false():
                     raise UPProblemDefinitionError(
                         "PROBLEM NOT SOLVABLE: an always is violated in the initial state"
                     )
             else:
-                type, init_state_value = self._evaluate_constraint(
-                    env, substituter, constr, I
-                )
+                type, init_state_value = self._evaluate_constraint(env, constr, I)
                 fluent = up.model.Fluent(
                     f"{type}{SEPARATOR}{monitoring_atoms_counter}",
                     env.type_manager.BoolType(),
                 )
                 monitoring_atoms.append(fluent)
                 monitoring_atom = env.expression_manager.FluentExp(fluent)
                 self._monitoring_atom_dict[constr] = monitoring_atom
                 if init_state_value.is_true():
                     initial_state_prime.append(monitoring_atom)
                 if constr.is_sometime_before():
-                    if substituter.substitute(constr.args[0], I).simplify().is_true():
+                    if constr.args[0].substitute(I).simplify().is_true():
                         raise UPProblemDefinitionError(
                             "PROBLEM NOT SOLVABLE: a sometime-before is violated in the initial state"
                         )
                 monitoring_atoms_counter += 1
         return initial_state_prime, monitoring_atoms
 
     def _build_relevancy_dict(self, env, C):
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/credits.py` & `unified_planning-0.6.0/unified_planning/engines/credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/engine.py` & `unified_planning-0.6.0/unified_planning/engines/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,37 +10,39 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines the engine interface."""
 
-from enum import Enum
 from unified_planning.model import ProblemKind
 from unified_planning.engines.credits import Credits
+from abc import ABCMeta, abstractmethod, ABC
+from enum import Enum
 from typing import Optional
 
 
 class OperationMode(Enum):
     """
     This class represents all the operation modes that the library supports.
     """
 
     ONESHOT_PLANNER = "oneshot_planner"
     ANYTIME_PLANNER = "anytime_planner"
     PLAN_VALIDATOR = "plan_validator"
     PORTFOLIO_SELECTOR = "portfolio_selector"
     COMPILER = "compiler"
-    SIMULATOR = "simulator"
+    SEQUENTIAL_SIMULATOR = "sequential_simulator"
     REPLANNER = "replanner"
+    PLAN_REPAIRER = "plan_repairer"
 
 
-class EngineMeta(type):
+class EngineMeta(ABCMeta):
     def __new__(cls, name, bases, dct):
-        obj = type.__new__(cls, name, bases, dct)
+        obj = super().__new__(cls, name, bases, dct)
         for base in bases:
             for om in OperationMode:
                 if (
                     hasattr(base, "is_" + om.value)
                     and getattr(base, "is_" + om.value)()
                 ):
                     setattr(obj, "is_" + om.value, staticmethod(lambda: True))
@@ -59,14 +61,15 @@
     """
 
     def __init__(self, **kwargs):
         self._skip_checks = False
         self._error_on_failed_checks = True
 
     @property
+    @abstractmethod
     def name(self) -> str:
         """Returns the engine name."""
         raise NotImplementedError
 
     @property
     def skip_checks(self) -> bool:
         """
@@ -112,20 +115,22 @@
         """
         Sets the flag deciding if a fail on the problem's :func:`kind <unified_planning.model.AbstractProblem.kind>` checks should return in an error or
         just in a warning.
         """
         self._error_on_failed_checks = new_value
 
     @staticmethod
+    @abstractmethod
     def supported_kind() -> ProblemKind:
         """
         Returns the `ProblemKind` supported by this `Engine`."""
         raise NotImplementedError
 
     @staticmethod
+    @abstractmethod
     def supports(problem_kind: "ProblemKind") -> bool:
         """
         If an unsupported `Problem` is given to this `Engine`, an exception is raised, unless the
         :func:`skip_checks <unified_planning.engines.Engine.skip_checks>` or :func:`error_on_failed_checks <unified_planning.engines.Engine.error_on_failed_checks>`
         prevent this from happening.
 
         NOTE that deactivating the checks might result in an Internal Error of the `Engine` or in a wrong result.
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/factory.py` & `unified_planning-0.6.0/unified_planning/engines/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,45 +17,60 @@
 import importlib
 import sys
 import os
 import inspect
 import configparser
 import unified_planning as up
 from unified_planning.environment import Environment
+from unified_planning.exceptions import UPUsageError
 from unified_planning.model import ProblemKind
 from unified_planning.plans import PlanKind
 from unified_planning.engines.mixins.oneshot_planner import OptimalityGuarantee
 from unified_planning.engines.mixins.anytime_planner import AnytimeGuarantee
 from unified_planning.engines.mixins.anytime_planner import AnytimePlannerMixin
 from unified_planning.engines.mixins.compiler import CompilationKind, CompilerMixin
 from unified_planning.engines.mixins.oneshot_planner import OneshotPlannerMixin
 from unified_planning.engines.mixins.plan_validator import PlanValidatorMixin
 from unified_planning.engines.mixins.portfolio import PortfolioSelectorMixin
 from unified_planning.engines.mixins.replanner import ReplannerMixin
-from unified_planning.engines.mixins.simulator import SimulatorMixin
+from unified_planning.engines.mixins.plan_repairer import PlanRepairerMixin
+from unified_planning.engines.mixins.sequential_simulator import (
+    SequentialSimulatorMixin,
+)
 from unified_planning.engines.engine import OperationMode
-from typing import IO, Any, Dict, Tuple, Optional, List, Union, Type, cast
+from typing import IO, Any, Dict, Tuple, Optional, List, Union, Type, Sequence
 from pathlib import PurePath
 
 
 DEFAULT_ENGINES = {
     "fast-downward": ("up_fast_downward", "FastDownwardPDDLPlanner"),
     "fast-downward-opt": ("up_fast_downward", "FastDownwardOptimalPDDLPlanner"),
     "pyperplan": ("up_pyperplan.engine", "EngineImpl"),
     "pyperplan-opt": ("up_pyperplan.engine", "OptEngineImpl"),
     "enhsp": ("up_enhsp.enhsp_planner", "ENHSPSatEngine"),
     "enhsp-opt": ("up_enhsp.enhsp_planner", "ENHSPOptEngine"),
+    "enhsp-any": ("up_enhsp.enhsp_planner", "ENHSPAnytimeEngine"),
     "tamer": ("up_tamer.engine", "EngineImpl"),
+    "lpg": ("up_lpg.lpg_planner", "LPGEngine"),
+    "lpg-anytime": ("up_lpg.lpg_planner", "LPGAnytimeEngine"),
+    "lpg-repairer": ("up_lpg.lpg_planner", "LPGPlanRepairer"),
+    "fmap": ("up_fmap.fmap_planner", "FMAPsolver"),
+    "aries": ("up_aries", "Aries"),
+    "aries-val": ("up_aries", "AriesVal"),
     "sequential_plan_validator": (
         "unified_planning.engines.plan_validator",
         "SequentialPlanValidator",
     ),
     "sequential_simulator": (
         "unified_planning.engines.sequential_simulator",
-        "SequentialSimulator",
+        "UPSequentialSimulator",
+    ),
+    "up_bounded_types_remover": (
+        "unified_planning.engines.compilers.bounded_types_remover",
+        "BoundedTypesRemover",
     ),
     "up_conditional_effects_remover": (
         "unified_planning.engines.compilers.conditional_effects_remover",
         "ConditionalEffectsRemover",
     ),
     "up_disjunctive_conditions_remover": (
         "unified_planning.engines.compilers.disjunctive_conditions_remover",
@@ -65,14 +80,18 @@
         "unified_planning.engines.compilers.negative_conditions_remover",
         "NegativeConditionsRemover",
     ),
     "up_quantifiers_remover": (
         "unified_planning.engines.compilers.quantifiers_remover",
         "QuantifiersRemover",
     ),
+    "up_usertype_fluents_remover": (
+        "unified_planning.engines.compilers.usertype_fluents_remover",
+        "UsertypeFluentsRemover",
+    ),
     "tarski_grounder": (
         "unified_planning.engines.compilers.tarski_grounder",
         "TarskiGrounder",
     ),
     "fast-downward-grounder": ("up_fast_downward", "FastDownwardGrounder"),
     "fast-downward-reachability-grounder": (
         "up_fast_downward",
@@ -95,25 +114,34 @@
 DEFAULT_ENGINES_PREFERENCE_LIST = [
     "fast-downward",
     "fast-downward-opt",
     "pyperplan",
     "pyperplan-opt",
     "enhsp",
     "enhsp-opt",
+    "enhsp-any",
     "tamer",
     "sequential_plan_validator",
     "sequential_simulator",
+    "up_bounded_types_remover",
     "up_conditional_effects_remover",
     "up_disjunctive_conditions_remover",
     "up_negative_conditions_remover",
     "up_quantifiers_remover",
+    "up_usertype_fluents_remover",
     "tarski_grounder",
     "fast-downward-reachability-grounder",
     "fast-downward-grounder",
     "up_grounder",
+    "lpg",
+    "lpg-anytime",
+    "lpg-repairer",
+    "fmap",
+    "aries",
+    "aries-val",
 ]
 
 DEFAULT_META_ENGINES_PREFERENCE_LIST = ["oversubscription"]
 
 
 def format_table(header: List[str], rows: List[List[str]]) -> str:
     row_template = "|"
@@ -145,16 +173,16 @@
 
 class Factory:
     """
     Class that manages all the different :class:`Engines <unified_planning.engines.Engine>` classes
     and handles the operation modes available in the library.
     """
 
-    def __init__(self, env: "Environment"):
-        self._env = env
+    def __init__(self, environment: "Environment"):
+        self._env = environment
         self._engines: Dict[str, Type["up.engines.engine.Engine"]] = {}
         self._engines_info: List[Tuple[str, str, str]] = []
         self._meta_engines: Dict[str, Type["up.engines.meta_engine.MetaEngine"]] = {}
         self._meta_engines_info: List[Tuple[str, str, str]] = []
         self._credit_disclaimer_printed = False
         for name, (module_name, class_name) in DEFAULT_ENGINES.items():
             try:
@@ -432,14 +460,26 @@
                     assert optimality_guarantee is None
                     assert compilation_kind is None
                     assert plan_kind is None
                     if anytime_guarantee is not None and not EngineClass.ensures(
                         anytime_guarantee
                     ):
                         continue
+                elif operation_mode == OperationMode.PLAN_REPAIRER:
+                    assert issubclass(EngineClass, PlanRepairerMixin)
+                    assert anytime_guarantee is None
+                    assert compilation_kind is None
+                    if plan_kind is not None and not EngineClass.supports_plan(
+                        plan_kind
+                    ):
+                        continue
+                    if optimality_guarantee is not None and not EngineClass.satisfies(
+                        optimality_guarantee
+                    ):
+                        continue
                 else:
                     assert optimality_guarantee is None
                     assert anytime_guarantee is None
                     assert compilation_kind is None
                     assert plan_kind is None
                 if EngineClass.supports(problem_kind):
                     return EngineClass
@@ -460,15 +500,15 @@
             msg = f"No available engine supports {optimality_guarantee}"
         elif anytime_guarantee is not None:
             msg = f"No available engine supports {anytime_guarantee}"
         else:
             msg = f"No available {operation_mode} engine"
         raise up.exceptions.UPNoSuitableEngineAvailableException(msg)
 
-    def _print_credits(self, all_credits: List[Optional["up.engines.Credits"]]):
+    def _print_credits(self, all_credits: Sequence[Optional["up.engines.Credits"]]):
         """
         This function prints the credits of the engine(s) used by an operation mode
         """
         credits: List["up.engines.Credits"] = [c for c in all_credits if c is not None]
         if len(credits) == 0:
             return
 
@@ -493,15 +533,15 @@
 
         if self.environment.credits_stream is not None:
             w = PaleWriter(self.environment.credits_stream)
 
             if not self._credit_disclaimer_printed:
                 self._credit_disclaimer_printed = True
                 w.write(
-                    f"\033[1mNOTE: To disable printing of planning engine credits, add this line to your code: `up.shortcuts.get_env().credits_stream = None`\n"
+                    f"\033[1mNOTE: To disable printing of planning engine credits, add this line to your code: `up.shortcuts.get_environment().credits_stream = None`\n"
                 )
             w.write("  *** Credits ***\n")
             w.write(
                 f"  * In operation mode `{operation_mode_name}` at line {line} of `{fname}`, "
             )
             if len(credits) > 1:
                 w.write(
@@ -513,46 +553,46 @@
                 c.write_credits(w)
             w.write("\n")
 
     def _get_engine(
         self,
         operation_mode: "OperationMode",
         name: Optional[str] = None,
-        names: Optional[List[str]] = None,
-        params: Optional[Union[Dict[str, str], List[Dict[str, str]]]] = None,
+        names: Optional[Sequence[str]] = None,
+        params: Optional[Union[Dict[str, str], Sequence[Dict[str, str]]]] = None,
         problem_kind: ProblemKind = ProblemKind(),
         optimality_guarantee: Optional["OptimalityGuarantee"] = None,
         compilation_kind: Optional["CompilationKind"] = None,
-        compilation_kinds: Optional[List["CompilationKind"]] = None,
+        compilation_kinds: Optional[Sequence["CompilationKind"]] = None,
         plan_kind: Optional["PlanKind"] = None,
         anytime_guarantee: Optional["AnytimeGuarantee"] = None,
         problem: Optional["up.model.AbstractProblem"] = None,
     ) -> "up.engines.engine.Engine":
         if names is not None and operation_mode != OperationMode.COMPILER:
             assert name is None
             assert problem is None, "Parallel simulation is not supported"
             if params is None:
-                params = [{} for i in range(len(names))]
+                params = [{} for _ in names]
             assert isinstance(params, List) and len(names) == len(params)
             engines = []
             all_credits = []
             for name, param in zip(names, params):
                 EngineClass = self._get_engine_class(operation_mode, name)
                 all_credits.append(EngineClass.get_credits(**param))
                 engines.append((name, param))
             self._print_credits(all_credits)
             p_engine = up.engines.parallel.Parallel(self, engines)
             return p_engine
         elif operation_mode == OperationMode.COMPILER and compilation_kinds is not None:
             assert name is None
             assert names is not None or problem_kind is not None
             if names is None:
-                names = [None for i in range(len(compilation_kinds))]  # type: ignore
+                names = [None for _ in compilation_kinds]  # type: ignore
             if params is None:
-                params = [{} for i in range(len(compilation_kinds))]
+                params = [{} for _ in compilation_kinds]
             assert isinstance(params, List) and len(names) == len(params)
             compilers: List["up.engines.engine.Engine"] = []
             all_credits = []
             for name, param, compilation_kind in zip(names, params, compilation_kinds):
                 EngineClass = self._get_engine_class(
                     operation_mode,
                     name,
@@ -591,34 +631,37 @@
                 if (
                     problem.kind.has_quality_metrics()
                     and optimality_guarantee == OptimalityGuarantee.SOLVED_OPTIMALLY
                 ):
                     msg = f"The problem has no quality metrics but the engine is required to be optimal!"
                     raise up.exceptions.UPUsageError(msg)
                 res = EngineClass(problem=problem, **params)
-            elif operation_mode == OperationMode.SIMULATOR:
+            elif operation_mode == OperationMode.SEQUENTIAL_SIMULATOR:
                 assert problem is not None
                 res = EngineClass(
                     problem=problem,
                     error_on_failed_checks=error_failed_checks,
                     **params,
                 )
-                assert isinstance(res, SimulatorMixin)
+                assert isinstance(res, SequentialSimulatorMixin)
             elif operation_mode == OperationMode.COMPILER:
                 res = EngineClass(**params)
                 assert isinstance(res, CompilerMixin)
                 if compilation_kind is not None:
                     res.default = compilation_kind
             elif (
                 operation_mode == OperationMode.ONESHOT_PLANNER
+                or operation_mode == OperationMode.PLAN_REPAIRER
                 or operation_mode == OperationMode.PORTFOLIO_SELECTOR
             ):
                 res = EngineClass(**params)
-                assert isinstance(res, OneshotPlannerMixin) or isinstance(
-                    res, PortfolioSelectorMixin
+                assert (
+                    isinstance(res, OneshotPlannerMixin)
+                    or isinstance(res, PortfolioSelectorMixin)
+                    or isinstance(res, PlanRepairerMixin)
                 )
                 if optimality_guarantee == OptimalityGuarantee.SOLVED_OPTIMALLY:
                     res.optimality_metric_required = True
             elif operation_mode == OperationMode.ANYTIME_PLANNER:
                 res = EngineClass(**params)
                 assert isinstance(res, AnytimePlannerMixin)
                 if (
@@ -636,32 +679,36 @@
         """Returns the environment in which this factory is created"""
         return self._env
 
     def OneshotPlanner(
         self,
         *,
         name: Optional[str] = None,
-        names: Optional[List[str]] = None,
-        params: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
+        names: Optional[Sequence[str]] = None,
+        params: Optional[Union[Dict[str, Any], Sequence[Dict[str, Any]]]] = None,
         problem_kind: ProblemKind = ProblemKind(),
         optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
     ) -> "up.engines.engine.Engine":
         """
         Returns a oneshot planner. There are three ways to call this method:
-        - using 'name' (the name of a specific planner) and 'params' (planner dependent options).
-          e.g. OneshotPlanner(name='tamer', params={'heuristic': 'hadd'})
-        - using 'names' (list of specific planners name) and 'params' (list of
-          planners dependent options) to get a Parallel engine.
-          e.g. OneshotPlanner(names=['tamer', 'tamer'],
-                              params=[{'heuristic': 'hadd'}, {'heuristic': 'hmax'}])
-        - using 'problem_kind' and 'optimality_guarantee'.
-          e.g. OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)
+
+        *   | using ``name`` (the name of a specific planner) and ``params`` (planner dependent options).
+            | e.g. ``OneshotPlanner(name='tamer', params={'heuristic': 'hadd'})``
+        *   | using ``names`` (list of specific planners name) and ``params`` (list of planner dependent options) to get a ``Parallel`` engine.
+            | e.g. ``OneshotPlanner(names=['tamer', 'tamer'], params=[{'heuristic': 'hadd'}, {'heuristic': 'hmax'}])``
+        *   | using ``problem_kind`` and ``optimality_guarantee``.
+            | e.g. ``OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
         """
         if isinstance(optimality_guarantee, str):
-            optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+            try:
+                optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+            except KeyError:
+                raise UPUsageError(
+                    f"{optimality_guarantee} is not a valid OptimalityGuarantee."
+                )
         return self._get_engine(
             OperationMode.ONESHOT_PLANNER,
             name,
             names,
             params,
             problem_kind,
             optimality_guarantee,
@@ -673,27 +720,29 @@
         name: Optional[str] = None,
         params: Optional[Dict[str, str]] = None,
         problem_kind: ProblemKind = ProblemKind(),
         anytime_guarantee: Optional[Union["AnytimeGuarantee", str]] = None,
     ) -> "up.engines.engine.Engine":
         """
         Returns a anytime planner. There are two ways to call this method:
-        - using 'name' (the name of a specific planner) and 'params' (planner dependent options).
-          e.g. AnytimePlanner(name='tamer', params={'heuristic': 'hadd'})
-        - using 'problem_kind' and 'anytime_guarantee'.
-          e.g. AnytimePlanner(problem_kind=problem.kind, anytime_guarantee=INCREASING_QUALITY)
-
-        An AnytimePlanner is a planner that returns an iterator of solutions.
-        Depending on the given anytime_guarantee parameter, every plan being generated is:
-        - strictly better in terms of quality than the previous one (INCREASING_QUALITY);
-        - optimal (OPTIMAL_PLANS);
-        - just a different plan, with no specific guarantee (None).
+
+        *   | using ``name`` (the name of a specific planner) and ``params`` (planner dependent options).
+            | e.g. ``AnytimePlanner(name='tamer', params={'heuristic': 'hadd'})``
+        *   | using ``problem_kind`` and ``anytime_guarantee``.
+            | e.g. ``AnytimePlanner(problem_kind=problem.kind, anytime_guarantee=INCREASING_QUALITY)``
+
+        An ``AnytimePlanner`` is a planner that returns an ``Iterator`` of solutions.
+        Depending on the given ``anytime_guarantee`` parameter, every plan being generated is:
+
+        * strictly better in terms of quality than the previous one (``INCREASING_QUALITY``);
+        * optimal (``OPTIMAL_PLANS``);
+        * just a different plan, with no specific guarantee (``None``).
 
         It raises an exception if the problem has no optimality metrics and anytime_guarantee
-        is equal to INCREASING_QUALITY or OPTIMAL_PLAN.
+        is equal to ``INCREASING_QUALITY`` or ``OPTIMAL_PLAN``.
         """
         if isinstance(anytime_guarantee, str):
             anytime_guarantee = AnytimeGuarantee[anytime_guarantee]
         return self._get_engine(
             OperationMode.ANYTIME_PLANNER,
             name,
             None,
@@ -702,30 +751,28 @@
             anytime_guarantee=anytime_guarantee,
         )
 
     def PlanValidator(
         self,
         *,
         name: Optional[str] = None,
-        names: Optional[List[str]] = None,
-        params: Optional[Union[Dict[str, str], List[Dict[str, str]]]] = None,
+        names: Optional[Sequence[str]] = None,
+        params: Optional[Union[Dict[str, str], Sequence[Dict[str, str]]]] = None,
         problem_kind: ProblemKind = ProblemKind(),
         plan_kind: Optional[Union["PlanKind", str]] = None,
     ) -> "up.engines.engine.Engine":
         """
         Returns a plan validator. There are three ways to call this method:
-        - using 'name' (the name of a specific plan validator) and 'params'
-          (plan validator dependent options).
-          e.g. PlanValidator(name='tamer', params={'opt': 'val'})
-        - using 'names' (list of specific plan validators name) and 'params' (list of
-          plan validators dependent options) to get a Parallel engine.
-          e.g. PlanValidator(names=['tamer', 'tamer'],
-                             params=[{'opt1': 'val1'}, {'opt2': 'val2'}])
-        - using 'problem_kind' and 'plan_kind' parameters.
-          e.g. PlanValidator(problem_kind=problem.kind, plan_kind=plan.kind)
+
+        *   | using ``name`` (the name of a specific plan validator) and ``params`` (plan validator dependent options).
+            | e.g. ``PlanValidator(name='tamer', params={'opt': 'val'})``
+        *   | using ``names`` (list of specific plan validators name) and ``params`` (list of plan validators dependent options) to get a ``Parallel`` engine.
+            | e.g. ``PlanValidator(names=['tamer', 'tamer'], params=[{'opt1': 'val1'}, {'opt2': 'val2'}])``
+        *   | using ``problem_kind`` and ``plan_kind`` parameters.
+            | e.g. ``PlanValidator(problem_kind=problem.kind, plan_kind=plan.kind)``
         """
         if isinstance(plan_kind, str):
             plan_kind = PlanKind[plan_kind]
         return self._get_engine(
             OperationMode.PLAN_VALIDATOR,
             name,
             names,
@@ -734,39 +781,36 @@
             plan_kind=plan_kind,
         )
 
     def Compiler(
         self,
         *,
         name: Optional[str] = None,
-        names: Optional[List[str]] = None,
-        params: Optional[Union[Dict[str, str], List[Dict[str, str]]]] = None,
+        names: Optional[Sequence[str]] = None,
+        params: Optional[Union[Dict[str, str], Sequence[Dict[str, str]]]] = None,
         problem_kind: ProblemKind = ProblemKind(),
         compilation_kind: Optional[Union["CompilationKind", str]] = None,
-        compilation_kinds: Optional[List[Union["CompilationKind", str]]] = None,
+        compilation_kinds: Optional[Sequence[Union["CompilationKind", str]]] = None,
     ) -> "up.engines.engine.Engine":
         """
-        Returns a Compiler or a pipeline of Compilers.
+        Returns a compiler or a pipeline of compilers.
+
+        To get a compiler there are two ways to call this method:
 
-        To get a Compiler there are two ways to call this method:
-        - using 'name' (the name of a specific compiler) and 'params'
-          (compiler dependent options).
-          e.g. Compiler(name='tamer', params={'opt': 'val'})
-        - using 'problem_kind' and 'compilation_kind' parameters.
-          e.g. Compiler(problem_kind=problem.kind, compilation_kind=GROUNDING)
-
-        To get a pipeline of Compilers there are two ways to call this method:
-        - using 'names' (the names of the specific compilers), 'params'
-          (compilers dependent options) and 'compilation_kinds'.
-          e.g. Compiler(names=['up_quantifiers_remover', 'up_grounder'],
-                        params=[{'opt1': 'val1'}, {'opt2': 'val2'}],
-                        compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])
-        - using 'problem_kind' and 'compilation_kinds' parameters.
-          e.g. Compiler(problem_kind=problem.kind,
-                        compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])
+        *   | using ``name`` (the name of a specific compiler) and ``params`` (compiler dependent options).
+            | e.g. ``Compiler(name='tamer', params={'opt': 'val'})``
+        *   | using ``problem_kind`` and ``compilation_kind`` parameters.
+            | e.g. ``Compiler(problem_kind=problem.kind, compilation_kind=GROUNDING)``
+
+        To get a pipeline of compilers there are two ways to call this method:
+
+        *   | using ``names`` (the names of the specific compilers), ``params`` (compilers dependent options) and ``compilation_kinds``.
+            | e.g. ``Compiler(names=['up_quantifiers_remover', 'up_grounder'], params=[{'opt1': 'val1'}, {'opt2': 'val2'}], compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])``
+        *   | using ``problem_kind`` and ``compilation_kinds`` parameters.
+            | e.g. ``Compiler(problem_kind=problem.kind, compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])``
         """
         if isinstance(compilation_kind, str):
             compilation_kind = CompilationKind[compilation_kind]
 
         kinds: Optional[List[CompilationKind]] = None
         if compilation_kinds is not None:
             kinds = []
@@ -783,79 +827,129 @@
             names,
             params,
             problem_kind,
             compilation_kind=compilation_kind,
             compilation_kinds=kinds,
         )
 
-    def Simulator(
+    def SequentialSimulator(
         self,
         problem: "up.model.AbstractProblem",
         *,
         name: Optional[str] = None,
         params: Optional[Dict[str, str]] = None,
     ) -> "up.engines.engine.Engine":
         """
-        Returns a Simulator. There are two ways to call this method:
-        - using 'problem_kind' through the problem field.
-          e.g. Simulator(problem)
-        - using 'name' (the name of a specific simulator) and eventually some 'params'
-          (simulator dependent options).
-          e.g. Simulator(problem, name='sequential_simulator')
+        Returns a sequential simulator. There are two ways to call this method:
+
+        *   | using ``problem_kind`` through the problem field.
+            | e.g. ``SequentialSimulator(problem)``
+        *   | using ``name`` (the name of a specific simulator) and eventually some ``params`` (simulator dependent options).
+            | e.g. ``SequentialSimulator(problem, name='sequential_simulator')``
         """
         return self._get_engine(
-            OperationMode.SIMULATOR, name, None, params, problem.kind, problem=problem
+            OperationMode.SEQUENTIAL_SIMULATOR,
+            name,
+            None,
+            params,
+            problem.kind,
+            problem=problem,
         )
 
     def Replanner(
         self,
         problem: "up.model.AbstractProblem",
         *,
         name: Optional[str] = None,
         params: Optional[Dict[str, str]] = None,
         optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
     ) -> "up.engines.engine.Engine":
         """
         Returns a Replanner. There are two ways to call this method:
-        - using 'problem' (with its kind) and 'optimality_guarantee' parameters.
-          e.g. Replanner(problem, optimality_guarantee=SOLVED_OPTIMALLY)
-        - using 'name' (the name of a specific replanner) and 'params'
-          (replanner dependent options).
-          e.g. Replanner(problem, name='replanner[tamer]')
+
+        *   | using ``problem`` (with its kind) and ``optimality_guarantee`` parameters.
+            | e.g. ``Replanner(problem, optimality_guarantee=SOLVED_OPTIMALLY)``
+        *   | using ``name`` (the name of a specific replanner) and ``params`` (replanner dependent options).
+            | e.g. ``Replanner(problem, name='replanner[tamer]')``
         """
         if isinstance(optimality_guarantee, str):
-            optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+            try:
+                optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+            except KeyError:
+                raise UPUsageError(
+                    f"{optimality_guarantee} is not a valid OptimalityGuarantee."
+                )
         return self._get_engine(
             OperationMode.REPLANNER,
             name,
             None,
             params,
             problem.kind,
             optimality_guarantee,
             problem=problem,
         )
 
+    def PlanRepairer(
+        self,
+        *,
+        name: Optional[str] = None,
+        params: Optional[Dict[str, Any]] = None,
+        problem_kind: ProblemKind = ProblemKind(),
+        plan_kind: Optional[Union["PlanKind", str]] = None,
+        optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
+    ) -> "up.engines.engine.Engine":
+        """
+        Returns a plan repairer. There are two ways to call this method:
+
+        *   | using ``name`` (the name of a plan repairer) and eventually ``params``.
+            | e.g. ``PlanRepairer(name='xxx')``
+        *   | using ``problem_kind``, ``plan_kind`` and ``optimality_guarantee``.
+            | e.g. ``PlanRepairer(problem_kind=problem.kind, plan_kind=plan.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
+        """
+        if isinstance(plan_kind, str):
+            plan_kind = PlanKind[plan_kind]
+        if isinstance(optimality_guarantee, str):
+            try:
+                optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+            except KeyError:
+                raise UPUsageError(
+                    f"{optimality_guarantee} is not a valid OptimalityGuarantee."
+                )
+        return self._get_engine(
+            OperationMode.PLAN_REPAIRER,
+            name=name,
+            params=params,
+            problem_kind=problem_kind,
+            plan_kind=plan_kind,
+            optimality_guarantee=optimality_guarantee,
+        )
+
     def PortfolioSelector(
         self,
         *,
         name: Optional[str] = None,
         params: Optional[Dict[str, Any]] = None,
         problem_kind: ProblemKind = ProblemKind(),
         optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
     ) -> "up.engines.engine.Engine":
         """
         Returns a portfolio selector. There are two ways to call this method:
-        - using 'name' (the name of a specific portfolio) and eventually 'params'
-            (portfolio dependent options).
-          e.g. PortfolioSelector(name='ibacop')
-        - using 'problem_kind' and 'optimality_guarantee'.
-          e.g. OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)
+
+        *   | using ``name`` (the name of a specific portfolio) and eventually ``params`` (portfolio dependent options).
+            | e.g. ``PortfolioSelector(name='ibacop')``
+        *   | using ``problem_kind`` and ``optimality_guarantee``.
+            | e.g. ``OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
         """
         if isinstance(optimality_guarantee, str):
-            optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+            try:
+                optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+            except KeyError:
+                raise UPUsageError(
+                    f"{optimality_guarantee} is not a valid OptimalityGuarantee."
+                )
         return self._get_engine(
             OperationMode.PORTFOLIO_SELECTOR,
             name=name,
             params=params,
             problem_kind=problem_kind,
             optimality_guarantee=optimality_guarantee,
         )
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/meta_engine.py` & `unified_planning-0.6.0/unified_planning/engines/meta_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines the meta engine interface."""
 
+from abc import abstractmethod
 from unified_planning.exceptions import UPUsageError
 from unified_planning.engines.engine import Engine, EngineMeta
 from unified_planning.model import ProblemKind
 from functools import partial
 from typing import Type
 
 
@@ -78,26 +79,29 @@
     @error_on_failed_checks.setter
     def error_on_failed_checks(self, new_value: bool):
         """Same as :func:`error_on_failed_checks <unified_planning.engines.Engine.error_on_failed_checks>`"""
         self._error_on_failed_checks = new_value
         self.engine.error_on_failed_checks = new_value
 
     @staticmethod
+    @abstractmethod
     def is_compatible_engine(engine: Type[Engine]) -> bool:
         """
         Returns `True` iff the given `engine` is compatible with this `MetaEngine`.
 
         :param engine: The `Engine` Class tested for compatibility.
         :return: `True` iff the given `engine` is compatible with this `MetaEngine`
         """
         raise NotImplementedError
 
     @staticmethod
+    @abstractmethod
     def _supported_kind(engine: Type[Engine]) -> ProblemKind:
         """Returns the supported kind of this meta engine with the given engine"""
         raise NotImplementedError
 
     @staticmethod
+    @abstractmethod
     def _supports(problem_kind: ProblemKind, engine: Type[Engine]) -> bool:
         """Returns true iff the given problem kind is supported by this meta
         engine with the given engine"""
         raise NotImplementedError
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/__init__.py` & `unified_planning-0.6.0/unified_planning/engines/mixins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,9 +20,12 @@
 )
 from unified_planning.engines.mixins.anytime_planner import (
     AnytimePlannerMixin,
     AnytimeGuarantee,
 )
 from unified_planning.engines.mixins.plan_validator import PlanValidatorMixin
 from unified_planning.engines.mixins.portfolio import PortfolioSelectorMixin
-from unified_planning.engines.mixins.simulator import Event, SimulatorMixin
+from unified_planning.engines.mixins.sequential_simulator import (
+    SequentialSimulatorMixin,
+)
 from unified_planning.engines.mixins.replanner import ReplannerMixin
+from unified_planning.engines.mixins.plan_repairer import PlanRepairerMixin
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/anytime_planner.py` & `unified_planning-0.6.0/unified_planning/engines/mixins/anytime_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import unified_planning as up
+from abc import ABC, abstractmethod
 from enum import Enum, auto
 from typing import IO, Optional, Iterator
 from warnings import warn
 
 
 class AnytimeGuarantee(Enum):
     INCREASING_QUALITY = auto()
     OPTIMAL_PLANS = auto()
 
 
-class AnytimePlannerMixin:
+class AnytimePlannerMixin(ABC):
     """Base class that must be extended by an :class:`~unified_planning.engines.Engine` that is also a `AnytimePlanner`."""
 
     def __init__(self):
         self.optimality_metric_required = False
 
     @staticmethod
     def is_anytime_planner() -> bool:
@@ -71,14 +72,15 @@
                 warn(msg)
         if not problem_kind.has_quality_metrics() and self.optimality_metric_required:
             msg = f"The problem has no quality metrics but the engine is required to satisfies some optimality guarantee!"
             raise up.exceptions.UPUsageError(msg)
         for res in self._get_solutions(problem, timeout, output_stream):
             yield res
 
+    @abstractmethod
     def _get_solutions(
         self,
         problem: "up.model.AbstractProblem",
         timeout: Optional[float] = None,
         output_stream: Optional[IO[str]] = None,
     ) -> Iterator["up.engines.results.PlanGenerationResult"]:
         """
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/compiler.py` & `unified_planning-0.6.0/unified_planning/engines/mixins/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from warnings import warn
 import unified_planning as up
 from unified_planning.model import ProblemKind
+from abc import ABC, abstractmethod
 from enum import Enum, auto
 from typing import Optional
+from warnings import warn
 
 
 class CompilationKind(Enum):
     """Enum representing the available compilation kinds currently in the library."""
 
     GROUNDING = auto()
     CONDITIONAL_EFFECTS_REMOVING = auto()
     DISJUNCTIVE_CONDITIONS_REMOVING = auto()
     NEGATIVE_CONDITIONS_REMOVING = auto()
     QUANTIFIERS_REMOVING = auto()
     TRAJECTORY_CONSTRAINTS_REMOVING = auto()
+    USERTYPE_FLUENTS_REMOVING = auto()
+    BOUNDED_TYPES_REMOVING = auto()
 
 
-class CompilerMixin:
+class CompilerMixin(ABC):
     """Generic class for a compiler defining it's interface."""
 
     def __init__(self, default: Optional[CompilationKind] = None):
         self._default = default
 
     def compile(
         self,
@@ -105,34 +108,37 @@
 
     @staticmethod
     def is_compiler() -> bool:
         """Returns True."""
         return True
 
     @staticmethod
+    @abstractmethod
     def supports_compilation(compilation_kind: CompilationKind) -> bool:
         """
         :param compilation_kind: The tested `CompilationKind`.
         :return: True if the given `CompilationKind` is supported
             by this compiler, False otherwise.
         """
         raise NotImplementedError
 
     @staticmethod
+    @abstractmethod
     def resulting_problem_kind(
         problem_kind: ProblemKind, compilation_kind: Optional[CompilationKind] = None
     ) -> ProblemKind:
         """
         Returns the `ProblemKind` of an :class:`~unified_planning.model.AbstractProblem` which is returned by the
         :meth:`~unified_planning.engines.mixins.compiler.CompilerMixin.compile` method with the given `CompilationKind`.
 
         :param problem_kind: The given `ProblemKind`.
         :param compilation_kind: The `CompilationKind` applied to modify the `ProblemKind`.
         :return: The resulting `ProblemKind`.
         """
         raise NotImplementedError
 
+    @abstractmethod
     def _compile(
         self, problem: "up.model.AbstractProblem", compilation_kind: CompilationKind
     ) -> "up.engines.results.CompilerResult":
         """Method called by :func:`~unified_planning.engines.mixins.CompilerMixin.compile` to get the returned :class:`~unified_planning.engines.CompilerResult`."""
         raise NotImplementedError
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/oneshot_planner.py` & `unified_planning-0.6.0/unified_planning/engines/mixins/oneshot_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from warnings import warn
 import unified_planning as up
+from abc import ABC, abstractmethod
 from enum import Enum, auto
 from typing import IO, Optional, Callable
 
 
 class OptimalityGuarantee(Enum):
     SATISFICING = auto()
     SOLVED_OPTIMALLY = auto()
 
 
-class OneshotPlannerMixin:
+class OneshotPlannerMixin(ABC):
     """Base class that must be extended by an :class:`~unified_planning.engines.Engine` that is also a `OneshotPlanner`."""
 
     def __init__(self):
         self.optimality_metric_required = False
 
     @staticmethod
     def is_oneshot_planner() -> bool:
@@ -42,17 +43,15 @@
         `optimality_guarantee`, `False` otherwise.
         """
         return False
 
     def solve(
         self,
         problem: "up.model.AbstractProblem",
-        heuristic: Optional[
-            Callable[["up.model.state.ROState"], Optional[float]]
-        ] = None,
+        heuristic: Optional[Callable[["up.model.state.State"], Optional[float]]] = None,
         timeout: Optional[float] = None,
         output_stream: Optional[IO[str]] = None,
     ) -> "up.engines.results.PlanGenerationResult":
         """
         This method takes a `AbstractProblem` and returns a `PlanGenerationResult`,
         which contains information about the solution to the problem given by the planner.
 
@@ -76,18 +75,17 @@
             else:
                 warn(msg)
         if not problem_kind.has_quality_metrics() and self.optimality_metric_required:
             msg = f"The problem has no quality metrics but the engine is required to be optimal!"
             raise up.exceptions.UPUsageError(msg)
         return self._solve(problem, heuristic, timeout, output_stream)
 
+    @abstractmethod
     def _solve(
         self,
         problem: "up.model.AbstractProblem",
-        heuristic: Optional[
-            Callable[["up.model.state.ROState"], Optional[float]]
-        ] = None,
+        heuristic: Optional[Callable[["up.model.state.State"], Optional[float]]] = None,
         timeout: Optional[float] = None,
         output_stream: Optional[IO[str]] = None,
     ) -> "up.engines.results.PlanGenerationResult":
         """Method called by the OneshotPlannerMixin.solve method."""
         raise NotImplementedError
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/plan_validator.py` & `unified_planning-0.6.0/unified_planning/engines/mixins/plan_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from abc import ABC, abstractmethod
 from warnings import warn
 import unified_planning as up
 
 
-class PlanValidatorMixin:
+class PlanValidatorMixin(ABC):
     """Base class that must be extended by an :class:`~unified_planning.engines.Engine` that is also a `PlanValidator`."""
 
     @staticmethod
     def is_plan_validator() -> bool:
         return True
 
     @staticmethod
+    @abstractmethod
     def supports_plan(plan_kind: "up.plans.PlanKind") -> bool:
         """
         :param plan_kind: The :func:`kind <unified_planning.plans.Plan.kind>` of the :class:`~unified_planning.plans.Plan` that must be supported.
         :return: `True` if the given `kind` of `Plan` is supported, False otherwise.
         """
         raise NotImplementedError
 
@@ -55,12 +57,13 @@
             msg = f"{self.name} cannot validate this kind of plan!"
             if self.error_on_failed_checks:
                 raise up.exceptions.UPUsageError(msg)
             else:
                 warn(msg)
         return self._validate(problem, plan)
 
+    @abstractmethod
     def _validate(
         self, problem: "up.model.AbstractProblem", plan: "up.plans.Plan"
     ) -> "up.engines.results.ValidationResult":
         """Method called by the PlanValidator.validate method."""
         raise NotImplementedError
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/portfolio.py` & `unified_planning-0.6.0/unified_planning/engines/mixins/portfolio.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from abc import ABC, abstractmethod
 from warnings import warn
 import unified_planning as up
 from typing import Any, Dict, List, Optional, Tuple
 
 
-class PortfolioSelectorMixin:
+class PortfolioSelectorMixin(ABC):
     """Base class that must be extended by an :class:`~unified_planning.engines.Engine` that is also a `PortfolioSelector`."""
 
     def __init__(self):
         self.optimality_metric_required = False
 
     @staticmethod
     def is_portfolio_selector() -> bool:
@@ -76,14 +77,15 @@
             raise up.exceptions.UPUsageError(msg)
         if max_planners is not None and max_planners <= 0:
             raise up.exceptions.UPUsageError(
                 f"The specified number of max_planners must be > 0 but {max_planners} is given!"
             )
         return self._get_best_oneshot_planners(problem, max_planners)
 
+    @abstractmethod
     def _get_best_oneshot_planners(
         self,
         problem: "up.model.AbstractProblem",
         max_planners: Optional[int] = None,
     ) -> Tuple[List[str], List[Dict[str, Any]]]:
         """Method called by the PortfolioSelectorMixin.get_best_oneshot_planners method."""
         raise NotImplementedError
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/replanner.py` & `unified_planning-0.6.0/unified_planning/engines/mixins/replanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import unified_planning as up
+from abc import ABC, abstractmethod
 from fractions import Fraction
 from typing import IO, Optional, Union
 from warnings import warn
 
 
-class ReplannerMixin:
+class ReplannerMixin(ABC):
     """Base class that must be extended by an :class:`~unified_planning.engines.Engine` that is also a `Replanner`."""
 
     def __init__(self, problem: "up.model.AbstractProblem"):
         self._problem = problem.clone()
         self_class = type(self)
         assert issubclass(self_class, up.engines.engine.Engine)
         assert isinstance(self, up.engines.engine.Engine)
@@ -120,25 +121,27 @@
         """
         Removes the given action.
 
         :param action: the action to remove to the problem.
         """
         return self._remove_action(name)
 
+    @abstractmethod
     def _resolve(
         self,
         timeout: Optional[float] = None,
         output_stream: Optional[IO[str]] = None,
     ) -> "up.engines.results.PlanGenerationResult":
         """
         Method called by the ReplannerMixin.resolve method that has to be implemented
         by the engines that implement this operation mode.
         """
         raise NotImplementedError
 
+    @abstractmethod
     def _update_initial_value(
         self,
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: Union[
             "up.model.fnode.FNode",
             "up.model.fluent.Fluent",
             "up.model.object.Object",
@@ -150,38 +153,42 @@
     ):
         """
         Method called by the ReplannerMixin.update_initial_value method that has to be implemented
         by the engines that implement this operation mode.
         """
         raise NotImplementedError
 
+    @abstractmethod
     def _add_goal(
         self, goal: Union["up.model.fnode.FNode", "up.model.fluent.Fluent", bool]
     ):
         """
         Method called by the ReplannerMixin.add_goal method that has to be implemented
         by the engines that implement this operation mode.
         """
         raise NotImplementedError
 
+    @abstractmethod
     def _remove_goal(
         self, goal: Union["up.model.fnode.FNode", "up.model.fluent.Fluent", bool]
     ):
         """
         Method called by the ReplannerMixin.remove_goal method that has to be implemented
         by the engines that implement this operation mode.
         """
         raise NotImplementedError
 
+    @abstractmethod
     def _add_action(self, action: "up.model.action.Action"):
         """
         Method called by the ReplannerMixin.add_action method that has to be implemented
         by the engines that implement this operation mode.
         """
         raise NotImplementedError
 
+    @abstractmethod
     def _remove_action(self, name: str):
         """
         Method called by the ReplannerMixin.remove_action method that has to be implemented
         by the engines that implement this operation mode.
         """
         raise NotImplementedError
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/mixins/simulator.py` & `unified_planning-0.6.0/unified_planning/engines/mixins/sequential_simulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,237 +9,216 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from typing import Iterator, List, Optional, Tuple, Union
+from abc import ABC, abstractmethod
+import inspect
+from typing import Iterator, List, Optional, Tuple, Union, Sequence
 from warnings import warn
 import unified_planning as up
 from unified_planning.exceptions import UPUsageError
 
 
-class Event:
-    """This is an abstract class representing an event."""
-
-    @property
-    def conditions(self) -> List["up.model.FNode"]:
-        """Returns the list of expressions that must be True in order for this event to be applicable."""
-        raise NotImplementedError
-
-    @property
-    def effects(self) -> List["up.model.Effect"]:
-        """Returns the list of effects linked to this event."""
-        raise NotImplementedError
-
-    @property
-    def simulated_effect(self) -> Optional["up.model.SimulatedEffect"]:
-        """Returns the list of simulated effects linked to this event."""
-        raise NotImplementedError
-
-
-class SimulatorMixin:
+class SequentialSimulatorMixin(ABC):
     """
-    SimulatorMixin abstract class.
+    SequentialSimulatorMixin abstract class.
     This class defines the interface that an :class:`~unified_planning.engines.Engine`
-    that is also a `Simulator` must implement.
+    that is also a `SequentialSimulator` must implement.
 
     Important NOTE: The `AbstractProblem` instance is given at the constructor.
     """
 
     def __init__(self, problem: "up.model.AbstractProblem") -> None:
         """
         Takes an instance of a `problem` and eventually some parameters, that represent
-        some specific settings of the `SimulatorMixin`.
+        some specific settings of the `SequentialSimulatorMixin`.
 
         :param problem: the `problem` that defines the domain in which the simulation exists.
         """
         self._problem = problem
         self_class = type(self)
         assert issubclass(
             self_class, up.engines.engine.Engine
-        ), "SimulatorMixin does not implement the up.engines.Engine class"
+        ), "SequentialSimulatorMixin does not implement the up.engines.Engine class"
         assert isinstance(self, up.engines.engine.Engine)
         if not self.skip_checks and not self_class.supports(problem.kind):
             msg = f"We cannot establish whether {self.name} is able to handle this problem!"
             if self.error_on_failed_checks:
                 raise UPUsageError(msg)
             else:
                 warn(msg)
 
-    def is_applicable(self, event: "Event", state: "up.model.ROState") -> bool:
-        """
-        Returns `True` if the given `event conditions` are evaluated as `True` in the given `state`;
-        returns `False` otherwise.
-
-        :param state: the `state` where the `event conditions` are checked.
-        :param event: the `event` whose `conditions` are checked.
-        :return: Whether or not the `event` is applicable in the given `state`.
-        """
-        return self._is_applicable(event, state)
-
-    def _is_applicable(self, event: "Event", state: "up.model.ROState") -> bool:
-        return (
-            len(self.get_unsatisfied_conditions(event, state, early_termination=True))
-            == 0
-        )
+    def _get_action_and_parameters(
+        self,
+        action_or_action_instance: Union["up.model.Action", "up.plans.ActionInstance"],
+        parameters: Optional[Sequence["up.model.Expression"]] = None,
+    ) -> Tuple["up.model.Action", Tuple["up.model.FNode", ...]]:
+        """
+        This is a utility method to handle the methods polymorphism.
+
+        :param action_or_action_instance: The ActionInstance given to the method or the
+            Action.
+        :param parameters: The parameter or the Sequence of parameters. The length of this
+            field must be equal to the len of the action's parameters. If action_or_action_instance
+            is an ActionInstance this param must be None.
+        :param method name: The name of the original method. Used for better error indexing.
+        :return: The couple of the Action together with it's parameters.
+        """
+        if isinstance(action_or_action_instance, up.plans.ActionInstance):
+            if parameters is not None:
+                method_name = inspect.stack()[1].function
+                assert isinstance(self, up.engines.engine.Engine)
+                raise UPUsageError(
+                    f"{self.name}.{method_name} method does not accept an ActionInstance and also the parameters."
+                )
+            act = action_or_action_instance.action
+            params = action_or_action_instance.actual_parameters
+            return act, params
+        act = action_or_action_instance
+        assert isinstance(act, up.model.Action), "Typing not respected"
+        auto_promote = self._problem.environment.expression_manager.auto_promote
+        if parameters is None:
+            params = tuple()
+        else:
+            assert isinstance(parameters, Sequence), "Typing not respected"
+            params = tuple(auto_promote(parameters))
+        if len(params) != len(act.parameters) or any(
+            not ap.type.is_compatible(p.type) for p, ap in zip(params, act.parameters)
+        ):
+            method_name = inspect.stack()[1].function
+            assert isinstance(self, up.engines.engine.Engine)
+            raise UPUsageError(
+                f"The parameters given to the {self.name}.{method_name} method are ",
+                "not compatible with the given action's parameters.",
+            )
+        return act, params
 
-    def get_unsatisfied_conditions(
-        self, event: "Event", state: "up.model.ROState", early_termination: bool = False
-    ) -> List["up.model.FNode"]:
-        """
-        Returns the list of `unsatisfied event conditions` evaluated in the given `state`.
-        If the flag `early_termination` is set, the method ends and returns at the first `unsatisfied condition`.
-
-        :param state: The `State` in which the `event conditions` are evaluated.
-        :param early_termination: Flag deciding if the method ends and returns at the first `unsatisfied condition`.
-        :return: The list of all the `event conditions` that evaluated to `False` or the list containing the first
-            `condition` evaluated to `False` if the flag `early_termination` is set.
+    def get_initial_state(self) -> "up.model.State":
         """
-        return self._get_unsatisfied_conditions(
-            event, state, early_termination=early_termination
-        )
+        Returns the problem's initial state.
 
-    def _get_unsatisfied_conditions(
-        self, event: "Event", state: "up.model.ROState", early_termination: bool = False
-    ) -> List["up.model.FNode"]:
-        """
-        Method called by the up.engines.mixins.simulator.SimulatorMixin.get_unsatisfied_conditions.
+        NOTE: Every different SequentialSimulator might assume that the State class
+        implementation given to it's other methods is the same returned by this method.
         """
+        return self._get_initial_state()
+
+    @abstractmethod
+    def _get_initial_state(self) -> "up.model.State":
+        """Method called by the up.engines.mixins.sequential_simulator.SequentialSimulatorMixin.get_initial_state."""
         raise NotImplementedError
 
-    def apply(
-        self, event: "Event", state: "up.model.COWState"
-    ) -> Optional["up.model.COWState"]:
+    def is_applicable(
+        self,
+        state: "up.model.State",
+        action_or_action_instance: Union["up.model.Action", "up.plans.ActionInstance"],
+        parameters: Optional[Sequence["up.model.Expression"]] = None,
+    ) -> bool:
         """
-        Returns `None` if the `event` is not applicable in the given `state`, otherwise returns a new `COWState`,
-        which is a copy of the given `state` where the `applicable effects` of the `event` are applied; therefore
-        some `fluent values` are updated.
+        Returns `True` if the given `action conditions` are evaluated as `True` in the given `state`;
+        returns `False` otherwise.
 
-        :param state: the `state` where the event formulas are calculated.
-        :param event: the `event` that has the information about the `conditions` to check and the `effects` to apply.
-        :return: `None` if the `event` is not applicable in the given `state`, a new `COWState` with some updated `values`
-            if the `event` is applicable.
-        """
-        return self._apply(event, state)
+        :param state: The state in which the given action is checked for applicability.
+        :param action_or_action_instance: The `ActionInstance` or the `Action` that must be checked
+            for applicability.
+        :param parameters: The parameters to ground the given `Action`. This param must be `None` if
+            an `ActionInstance` is given instead.
+        :return: Whether or not the action is applicable in the given `state`.
+        """
+        act, params = self._get_action_and_parameters(
+            action_or_action_instance,
+            parameters,
+        )
+        return self._is_applicable(state, act, params)
 
-    def _apply(
-        self, event: "Event", state: "up.model.COWState"
-    ) -> Optional["up.model.COWState"]:
+    @abstractmethod
+    def _is_applicable(
+        self,
+        state: "up.model.State",
+        action: "up.model.Action",
+        parameters: Tuple["up.model.FNode", ...],
+    ) -> bool:
         """
-        Method called by the up.engines.mixins.simulator.SimulatorMixin.apply.
+        Method called by the up.engines.mixins.sequential_simulator.SequentialSimulatorMixin.is_applicable.
         """
         raise NotImplementedError
 
-    def apply_unsafe(
-        self, event: "Event", state: "up.model.COWState"
-    ) -> "up.model.COWState":
+    def apply(
+        self,
+        state: "up.model.State",
+        action_or_action_instance: Union["up.model.Action", "up.plans.ActionInstance"],
+        parameters: Optional[Sequence["up.model.Expression"]] = None,
+    ) -> Optional["up.model.State"]:
         """
-        Returns a new `COWState`, which is a copy of the given `state` but the applicable `effects` of the
-        `event` are applied; therefore some `fluent` values are updated.
-        IMPORTANT NOTE: Assumes that `self.is_applicable(state, event)` returns `True`.
+        Returns `None` if the given `action` is not applicable in the given `state`, otherwise returns a new `State`,
+        which is a copy of the given `state` where the `applicable effects` of the `action` are applied; therefore
+        some `fluent values` are updated.
 
-        :param state: the `state` where the `event formulas` are evaluated.
-        :param event: the `event` that has the information about the `effects` to apply.
-        :return: A new `COWState` with some updated values.
-        """
-        return self._apply_unsafe(event, state)
+        :param state: The state in which the given action's conditions are checked and the effects evaluated.
+        :param action_or_action_instance: The `ActionInstance` or the `Action` of which conditions are checked
+            and effects evaluated.
+        :param parameters: The parameters to ground the given `Action`. This param must be `None` if
+            an `ActionInstance` is given instead.
+        :return: `None` if the `action` is not applicable in the given `state`, the new State generated
+            if the action is applicable.
+        """
+        act, params = self._get_action_and_parameters(
+            action_or_action_instance,
+            parameters,
+        )
+        return self._apply(state, act, params)
 
-    def _apply_unsafe(
-        self, event: "Event", state: "up.model.COWState"
-    ) -> "up.model.COWState":
+    @abstractmethod
+    def _apply(
+        self,
+        state: "up.model.State",
+        action: "up.model.Action",
+        parameters: Tuple["up.model.FNode", ...],
+    ) -> Optional["up.model.State"]:
         """
-        Method called by the up.engines.mixins.simulator.SimulatorMixin.apply_unsafe.
+        Method called by the up.engines.mixins.sequential_simulator.SequentialSimulatorMixin.apply.
         """
         raise NotImplementedError
 
-    def get_applicable_events(self, state: "up.model.ROState") -> Iterator["Event"]:
+    def get_applicable_actions(
+        self, state: "up.model.State"
+    ) -> Iterator[Tuple["up.model.Action", Tuple["up.model.FNode", ...]]]:
         """
-        Returns a view over all the `events` that are applicable in the given `State`;
-        an `Event` is considered applicable in a given `State`, when all the `Event condition`
-        simplify as `True` when evaluated in the `State`.
+        Returns a view over all the `action + parameters` that are applicable in the given `State`.
 
         :param state: the `state` where the formulas are evaluated.
-        :return: an `Iterator` of applicable `Events`.
+        :return: an `Iterator` of applicable actions + parameters.
         """
-        return self._get_applicable_events(state)
+        return self._get_applicable_actions(state)
 
-    def _get_applicable_events(self, state: "up.model.ROState") -> Iterator["Event"]:
+    @abstractmethod
+    def _get_applicable_actions(
+        self, state: "up.model.State"
+    ) -> Iterator[Tuple["up.model.Action", Tuple["up.model.FNode", ...]]]:
         """
-        Method called by the up.engines.mixins.simulator.SimulatorMixin.get_applicable_events.
-        """
-        raise NotImplementedError
-
-    def get_events(
-        self,
-        action: "up.model.Action",
-        parameters: Union[
-            Tuple["up.model.Expression", ...], List["up.model.Expression"]
-        ],
-    ) -> List["Event"]:
-        """
-        Returns a list containing all the `events` derived from the given `action`, grounded with the given `parameters`.
-
-        :param action: the `action` containing the information to create the `event`.
-        :param parameters: the `parameters` needed to ground the `action`.
-        :return: the List of `Events` derived from this `action` with these `parameters`.
-        """
-        if len(action.parameters) != len(parameters):
-            raise UPUsageError(
-                "The parameters given action do not have the same length of the given parameters."
-            )
-        return self._get_events(action, parameters)
-
-    def _get_events(
-        self,
-        action: "up.model.Action",
-        parameters: Union[
-            Tuple["up.model.Expression", ...], List["up.model.Expression"]
-        ],
-    ) -> List["Event"]:
-        """
-        Method called by the up.engines.mixins.simulator.SimulatorMixin.get_events.
+        Method called by the up.engines.mixins.sequential_simulator.SequentialSimulatorMixin.get_applicable_actions.
         """
         raise NotImplementedError
 
     @staticmethod
-    def is_simulator():
+    def is_sequential_simulator():
         return True
 
-    def is_goal(self, state: "up.model.ROState") -> bool:
+    def is_goal(self, state: "up.model.State") -> bool:
         """
         Returns `True` if the given `state` satisfies the :class:`~unified_planning.model.AbstractProblem` :func:`goals <unified_planning.model.Problem.goals>`.
 
         NOTE: This method does not consider the :func:`quality_metrics <unified_planning.model.Problem.quality_metrics>` of the problem.
 
         :param state: the `State` in which the `problem goals` are evaluated.
         :return: `True` if the evaluation of every `goal` is `True`, `False` otherwise.
         """
         return self._is_goal(state)
 
-    def _is_goal(self, state: "up.model.ROState") -> bool:
-        """
-        Method called by the up.engines.mixins.simulator.SimulatorMixin.is_goal.
-        """
-        return len(self.get_unsatisfied_goals(state, early_termination=True)) == 0
-
-    def get_unsatisfied_goals(
-        self, state: "up.model.ROState", early_termination: bool = False
-    ) -> List["up.model.FNode"]:
-        """
-        Returns the list of `unsatisfied goals` evaluated in the given `state`.
-        If the flag `early_termination` is set, the method ends and returns at the first `unsatisfied goal`.
-
-        :param state: The `State` in which the `problem goals` are evaluated.
-        :param early_termination: Flag deciding if the method ends and returns at the first `unsatisfied goal`.
-        :return: The list of all the `goals` that evaluated to `False` or the list containing the first `goal` evaluated to `False` if the flag `early_termination` is set.
-        """
-        return self._get_unsatisfied_goals(state, early_termination)
-
-    def _get_unsatisfied_goals(
-        self, state: "up.model.ROState", early_termination: bool = False
-    ) -> List["up.model.FNode"]:
+    @abstractmethod
+    def _is_goal(self, state: "up.model.State") -> bool:
         """
-        Method called by the up.engines.mixins.simulator.SimulatorMixin.get_unsatisfied_goals.
+        Method called by the up.engines.mixins.sequential_simulator.SequentialSimulatorMixin.is_goal.
         """
         raise NotImplementedError
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/oversubscription_planner.py` & `unified_planning-0.6.0/unified_planning/engines/oversubscription_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,84 +51,103 @@
     def satisfies(optimality_guarantee: OptimalityGuarantee) -> bool:
         if optimality_guarantee == OptimalityGuarantee.SATISFICING:
             return True
         return False
 
     @staticmethod
     def is_compatible_engine(engine: Type[Engine]) -> bool:
-        return engine.is_oneshot_planner() and engine.supports(ProblemKind({"ACTION_BASED"}))  # type: ignore
+        return engine.is_oneshot_planner() and engine.supports(ProblemKind({"ACTION_BASED", "NEGATIVE_CONDITIONS"}))  # type: ignore
 
     @staticmethod
     def _supported_kind(engine: Type[Engine]) -> "ProblemKind":
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
+        supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
+        supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
+        supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-        supported_kind.set_time("TIMED_EFFECT")
+        supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
+        supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATION")
-        supported_kind.set_expression_duration("FLUENTS_IN_DURATION")
+        supported_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
+        supported_kind.set_expression_duration("FLUENTS_IN_DURATIONS")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         final_supported_kind = supported_kind.intersection(engine.supported_kind())
         final_supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
+        final_supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         return final_supported_kind
 
     @staticmethod
     def _supports(problem_kind: "ProblemKind", engine: Type[Engine]) -> bool:
         return problem_kind <= OversubscriptionPlanner._supported_kind(engine)
 
     def _solve(
         self,
         problem: "up.model.AbstractProblem",
-        heuristic: Optional[
-            Callable[["up.model.state.ROState"], Optional[float]]
-        ] = None,
+        heuristic: Optional[Callable[["up.model.state.State"], Optional[float]]] = None,
         timeout: Optional[float] = None,
         output_stream: Optional[IO[str]] = None,
     ) -> "PlanGenerationResult":
         assert isinstance(problem, up.model.Problem)
         assert isinstance(self.engine, mixins.OneshotPlannerMixin)
+        em = problem.environment.expression_manager
         if len(problem.quality_metrics) == 0:
-            goals: List[Tuple["up.model.FNode", Union[Fraction, int]]] = []
+            goals: List = []
         else:
             assert len(problem.quality_metrics) == 1
             qm = problem.quality_metrics[0]
-            assert isinstance(qm, up.model.metrics.Oversubscription)
+            assert isinstance(
+                qm,
+                (
+                    up.model.metrics.Oversubscription,
+                    up.model.metrics.TemporalOversubscription,
+                ),
+            )
             goals = list(qm.goals.items())
         q = []
         for l in powerset(goals):
-            cost: Union[Fraction, int] = 0
+            weight: Union[Fraction, int] = 0
             sg = []
             for g, c in l:
-                cost += c
+                weight += c
                 sg.append(g)
-            q.append((cost, sg))
+            q.append((weight, sg))
         q.sort(reverse=True, key=lambda t: t[0])
         incomplete = False
         for t in q:
             new_problem = problem.clone()
             new_problem.clear_quality_metrics()
-            for g in t[1]:
-                new_problem.add_goal(g)
+            for g, _ in goals:
+                if isinstance(g, tuple):
+                    goal = g[1] if g[1] in t[1] else em.Not(g[1])
+                    new_problem.add_timed_goal(g[0], goal)
+                else:
+                    goal = g if g in t[1] else em.Not(g)
+                    new_problem.add_goal(goal)
             start = time.time()
             res = self.engine.solve(new_problem, heuristic, timeout, output_stream)
             if timeout is not None:
                 timeout -= min(timeout, time.time() - start)
             if res.status in up.engines.results.POSITIVE_OUTCOMES:
                 if incomplete or len(goals) == 0:
                     status = PlanGenerationResultStatus.SOLVED_SATISFICING
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/parallel.py` & `unified_planning-0.6.0/unified_planning/engines/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 from unified_planning.engines.results import (
     LogLevel,
     PlanGenerationResultStatus,
     Result,
     ValidationResult,
     PlanGenerationResult,
 )
-from typing import IO, Dict, List, Optional, Tuple, Type, Callable, cast
-from fractions import Fraction
+from typing import IO, Dict, List, Optional, Tuple, Callable, cast
 from multiprocessing import Process, Queue
 
 
 class Parallel(
     engines.engine.Engine,
     engines.mixins.OneshotPlannerMixin,
     engines.mixins.PlanValidatorMixin,
@@ -120,17 +119,15 @@
         if definitive_result_found:  # A planner found a definitive result
             return [res]
         return results
 
     def _solve(
         self,
         problem: "up.model.AbstractProblem",
-        heuristic: Optional[
-            Callable[["up.model.state.ROState"], Optional[float]]
-        ] = None,
+        heuristic: Optional[Callable[["up.model.state.State"], Optional[float]]] = None,
         timeout: Optional[float] = None,
         output_stream: Optional[IO[str]] = None,
     ) -> "up.engines.results.PlanGenerationResult":
         for engine_name, _ in self.engines:
             engine = self._factory.engine(engine_name)
             assert issubclass(engine, engines.mixins.OneshotPlannerMixin)
         if output_stream is not None:
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/pddl_planner.py` & `unified_planning-0.6.0/unified_planning/engines/pddl_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines an interface for a generic PDDL planner."""
 
+from abc import ABCMeta, abstractmethod
 import asyncio
 from asyncio.subprocess import PIPE
 import select
 import subprocess
 import sys
 import tempfile
 import os
@@ -60,21 +61,29 @@
 
 class PDDLPlanner(engines.engine.Engine, mixins.OneshotPlannerMixin):
     """
     This class is the interface of a generic PDDL :class:`OneshotPlanner <unified_planning.engines.mixins.OneshotPlannerMixin>`
     that can be invocated through a subprocess call.
     """
 
-    def __init__(self, needs_requirements=True):
+    def __init__(self, needs_requirements=True, rewrite_bool_assignments=False):
+        """
+        :param self: The PDDLEngine instance.
+        :param needs_requirements: Flag defining if the Engine needs the PDDL requirements.
+        :param rewrite_bool_assignments: Flag defining if the non-constant boolean assignments
+            will be rewritten as conditional effects in the PDDL file submitted to the Engine.
+        """
         engines.engine.Engine.__init__(self)
         mixins.OneshotPlannerMixin.__init__(self)
         self._needs_requirements = needs_requirements
+        self._rewrite_bool_assignments = rewrite_bool_assignments
         self._process = None
         self._writer = None
 
+    @abstractmethod
     def _get_cmd(
         self, domain_filename: str, problem_filename: str, plan_filename: str
     ) -> List[str]:
         """
         Takes in input two filenames where the problem's domain and problem are written, a
         filename where to write the plan and returns a list of command to run the engine on the
         problem and write the plan on the file called plan_filename.
@@ -83,14 +92,21 @@
         :param problem_filename: The path of the PDDl problem file.
         :param plan_filename: The path where the generated plan will be written.
         :return: The list of commands needed to execute the planner from command line using the given
             paths.
         """
         raise NotImplementedError
 
+    def _get_engine_epsilon(self) -> Optional[Fraction]:
+        """
+        | Returns the epsilon used by the engine.
+        | Note: must be implemented only if the engine supports temporal problems.
+        """
+        raise NotImplementedError
+
     def _plan_from_file(
         self,
         problem: "up.model.Problem",
         plan_filename: str,
         get_item_named: Callable[
             [str],
             Union[
@@ -169,36 +185,36 @@
 
             action = get_item_named(name)
             assert isinstance(action, up.model.Action), "Wrong plan or renaming."
             parameters = []
             for p in params_name:
                 obj = get_item_named(p)
                 assert isinstance(obj, up.model.Object), "Wrong plan or renaming."
-                parameters.append(problem.env.expression_manager.ObjectExp(obj))
+                parameters.append(problem.environment.expression_manager.ObjectExp(obj))
             act_instance = up.plans.ActionInstance(action, tuple(parameters))
             if is_tt:
                 actions.append((start, act_instance, dur))
             else:
                 actions.append(act_instance)
         if is_tt:
             return up.plans.TimeTriggeredPlan(actions)
         else:
             return up.plans.SequentialPlan(actions)
 
     def _solve(
         self,
         problem: "up.model.AbstractProblem",
-        heuristic: Optional[
-            Callable[["up.model.state.ROState"], Optional[float]]
-        ] = None,
+        heuristic: Optional[Callable[["up.model.state.State"], Optional[float]]] = None,
         timeout: Optional[float] = None,
         output_stream: Optional[Union[Tuple[IO[str], IO[str]], IO[str]]] = None,
     ) -> "up.engines.results.PlanGenerationResult":
         assert isinstance(problem, up.model.Problem)
-        self._writer = PDDLWriter(problem, self._needs_requirements)
+        self._writer = PDDLWriter(
+            problem, self._needs_requirements, self._rewrite_bool_assignments
+        )
         plan = None
         logs: List["up.engines.results.LogMessage"] = []
         with tempfile.TemporaryDirectory() as tempdir:
             domain_filename = os.path.join(tempdir, "domain.pddl")
             problem_filename = os.path.join(tempdir, "problem.pddl")
             plan_filename = os.path.join(tempdir, "plan.txt")
             self._writer.write_domain(domain_filename)
@@ -260,18 +276,26 @@
                     plan=plan,
                     log_messages=logs,
                     engine_name=self.name,
                 )
         status: PlanGenerationResultStatus = self._result_status(
             problem, plan, retval, logs
         )
-        return PlanGenerationResult(
+        res = PlanGenerationResult(
             status, plan, log_messages=logs, engine_name=self.name
         )
+        problem_kind = problem.kind
+        if problem_kind.has_continuous_time() or problem_kind.has_discrete_time():
+            if isinstance(plan, up.plans.TimeTriggeredPlan) or plan is None:
+                return up.engines.results.correct_plan_generation_result(
+                    res, problem, self._get_engine_epsilon()
+                )
+        return res
 
+    @abstractmethod
     def _result_status(
         self,
         problem: "up.model.Problem",
         plan: Optional["up.plans.Plan"],
         retval: int,
         log_messages: Optional[List[LogMessage]] = None,
     ) -> "up.engines.results.PlanGenerationResultStatus":
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/plan_validator.py` & `unified_planning-0.6.0/unified_planning/engines/plan_validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,52 +10,62 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
+from typing import Optional
 import unified_planning as up
 import unified_planning.environment
 import unified_planning.engines as engines
 import unified_planning.engines.mixins as mixins
 import unified_planning.model.walkers as walkers
 from unified_planning.model import (
     AbstractProblem,
     Problem,
     ProblemKind,
-    COWState,
-    UPCOWState,
+    State,
 )
 from unified_planning.engines.results import (
     ValidationResult,
     ValidationResultStatus,
     LogMessage,
     LogLevel,
+    FailedValidationReason,
 )
 from unified_planning.engines.sequential_simulator import (
-    SequentialSimulator,
-    InstantaneousEvent,
+    UPSequentialSimulator,
+    evaluate_quality_metric,
+    evaluate_quality_metric_in_initial_state,
 )
 from unified_planning.plans import SequentialPlan, PlanKind
+from unified_planning.exceptions import (
+    UPConflictingEffectsException,
+    UPUsageError,
+    UPProblemDefinitionError,
+    UPInvalidActionError,
+)
 
 
 class SequentialPlanValidator(engines.engine.Engine, mixins.PlanValidatorMixin):
     """
     Performs :class:`~unified_planning.plans.Plan` validation.
 
     If the given :class:`~unified_planning.model.Problem` has any quality metric,
     the metric is simply ignored because it predicates over the Optimality of
     the Plan, but not the Validity!
     """
 
     def __init__(self, **options):
         engines.engine.Engine.__init__(self)
         self._env: "unified_planning.environment.Environment" = (
-            unified_planning.environment.get_env(options.get("env", None))
+            unified_planning.environment.get_environment(
+                options.get("environment", None)
+            )
         )
         self.manager = self._env.expression_manager
         self._substituter = walkers.Substituter(self._env)
 
     @property
     def name(self):
         return "sequential_plan_validator"
@@ -68,29 +78,37 @@
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
+        supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
+        supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind):
         return problem_kind <= SequentialPlanValidator.supported_kind()
@@ -106,31 +124,77 @@
         :param problem: The problem for which the plan to validate was generated.
         :param plan: The plan that must be validated.
         :return: The generated up.engines.results.ValidationResult; a data structure containing the information
             about the plan validity and eventually some additional log messages for the user.
         """
         assert isinstance(plan, SequentialPlan)
         assert isinstance(problem, Problem)
-        simulator = SequentialSimulator(problem)
-        current_state: "COWState" = UPCOWState(problem.initial_values)
-        count = 0  # used for better error indexing
-        for ai in plan.actions:
-            action = ai.action
-            assert isinstance(action, unified_planning.model.InstantaneousAction)
-            count = count + 1
-            events = simulator.get_events(action, ai.actual_parameters)
-            assert len(events) < 2, f"{str(ai)} + {len(events)}"
-            for event in events:
-                if not simulator.is_applicable(event, current_state):
-                    error = f"Preconditions {event.conditions} of {str(count)}-th action instance {str(ai)} are not satisfied."
-                    logs = [LogMessage(LogLevel.ERROR, error)]
-                    return ValidationResult(
-                        ValidationResultStatus.INVALID, self.name, logs
-                    )
-                current_state = simulator.apply_unsafe(event, current_state)
-        unsatisfied_goals = simulator.get_unsatisfied_goals(current_state)
-        if len(unsatisfied_goals) == 0:
-            return ValidationResult(ValidationResultStatus.VALID, self.name, [])
+        metric = None
+        if len(problem.quality_metrics) > 0:
+            if len(problem.quality_metrics) == 1:
+                metric = problem.quality_metrics[0]
+            else:
+                raise UPProblemDefinitionError(
+                    "The UP does not support more than one quality metric in the problem."
+                )
+        simulator = UPSequentialSimulator(problem)
+        prev_state: Optional[State] = simulator.get_initial_state()
+        if metric is not None:
+            metric_value = evaluate_quality_metric_in_initial_state(simulator, metric)
+        msg = None
+        for i, ai in enumerate(plan.actions):
+            assert prev_state is not None
+            try:
+                unsat_conds = simulator.get_unsatisfied_conditions(prev_state, ai)
+                if unsat_conds:
+                    msg = f"Preconditions {unsat_conds} of {str(i)}-th action instance {str(ai)} are not satisfied."
+            except UPConflictingEffectsException as e:
+                msg = f"{str(i)}-th action instance {str(ai)} creates conflicting effects: {str(e)}"
+            except UPUsageError as e:
+                msg = f"{str(i)}-th action instance {str(ai)} creates a UsageError: {str(e)}"
+            except UPInvalidActionError as e:
+                msg = f"{str(i)}-th action instance {str(ai)} creates an Invalid Action: {str(e)}"
+            next_state = simulator.apply_unsafe(prev_state, ai)
+            if next_state is None:
+                msg = f"{str(i)}-th action instance {str(ai)} creates conflicting effects."
+            if msg is not None:
+                logs = [LogMessage(LogLevel.INFO, msg)]
+                return ValidationResult(
+                    ValidationResultStatus.INVALID,
+                    self.name,
+                    logs,
+                    None,
+                    FailedValidationReason.INAPPLICABLE_ACTION,
+                    ai,
+                )
+            assert next_state is not None
+            if metric is not None:
+                metric_value = evaluate_quality_metric(
+                    simulator,
+                    metric,
+                    metric_value,
+                    prev_state,
+                    ai.action,
+                    ai.actual_parameters,
+                    next_state,
+                )
+            prev_state = next_state
+        assert next_state is not None
+        unsatisfied_goals = simulator.get_unsatisfied_goals(next_state)
+        if not unsatisfied_goals:
+            metric_evalutations = None
+            if metric is not None:
+                metric_evalutations = {metric: metric_value}
+            logs = []
+            return ValidationResult(
+                ValidationResultStatus.VALID, self.name, logs, metric_evalutations
+            )
         else:
-            error = f"Goals {unsatisfied_goals} are not satisfied by the plan."
-            logs = [LogMessage(LogLevel.ERROR, error)]
-            return ValidationResult(ValidationResultStatus.INVALID, self.name, logs)
+            msg = f"Goals {unsatisfied_goals} are not satisfied by the plan."
+            logs = [LogMessage(LogLevel.INFO, msg)]
+            return ValidationResult(
+                ValidationResultStatus.INVALID,
+                self.name,
+                logs,
+                None,
+                FailedValidationReason.UNSATISFIED_GOALS,
+            )
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/engines/replanner.py` & `unified_planning-0.6.0/unified_planning/engines/replanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         assert isinstance(self._problem, up.model.Problem)
         self._problem.add_goal(goal)
 
     def _remove_goal(
         self, goal: Union["up.model.fnode.FNode", "up.model.fluent.Fluent", bool]
     ):
         assert isinstance(self._problem, up.model.Problem)
-        (goal_exp,) = self._problem.env.expression_manager.auto_promote(goal)
+        (goal_exp,) = self._problem.environment.expression_manager.auto_promote(goal)
         goals = self._problem.goals
         self._problem.clear_goals()
         for g in goals:
             if not g is goal_exp:
                 self._problem.add_goal(g)
 
     def _add_action(self, action: "up.model.action.Action"):
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/environment.py` & `unified_planning-0.6.0/unified_planning/environment.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,23 +35,27 @@
 
     """
 
     def __init__(self):
         import unified_planning.model
         import unified_planning.engines
         import unified_planning.model.walkers
+        import unified_planning.model.type_manager
 
-        self._type_manager = unified_planning.model.TypeManager()
+        self._type_manager = unified_planning.model.type_manager.TypeManager()
         self._factory = unified_planning.engines.Factory(self)
         self._tc = unified_planning.model.walkers.TypeChecker(self)
         self._expression_manager = unified_planning.model.ExpressionManager(self)
         self._free_vars_oracle = unified_planning.model.FreeVarsOracle()
         self._simplifier = unified_planning.model.walkers.Simplifier(self)
+        self._substituter = unified_planning.model.walkers.Substituter(self)
         self._free_vars_extractor = unified_planning.model.walkers.FreeVarsExtractor()
+        self._names_extractor = unified_planning.model.walkers.NamesExtractor()
         self._credits_stream: Optional[IO[str]] = sys.stdout
+        self._error_used_name: bool = True
 
     # The getstate and setstate method are needed in the Parallel engine. The
     #  Parallel engine creates a deep copy of the Environment instance in
     #  another process by pickling the environment fields.
     # Since the IO[str] class is not picklable, we need to remove it from the
     #  state and then add it as None in the new process
     def __getstate__(self):
@@ -62,25 +66,42 @@
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         # Add _credits_stream back since it doesn't exist in the pickle
         self._credits_stream = None
 
     @property
+    def error_used_name(self) -> bool:
+        return self._error_used_name
+
+    @error_used_name.setter
+    def error_used_name(self, new_val: bool):
+        """
+        This flag determines if a problem in this environment can have the same
+        name for different elements (like an Action and a Fluent). If it is
+        True, this name duplication will raise an exception, if it is False it
+        will only raise a warning.
+
+        It always raise an exception to name in the same way 2 elements
+        belonging to the same category, like 2 actions.
+        """
+        self._error_used_name = new_val
+
+    @property
     def free_vars_oracle(self) -> "unified_planning.model.FreeVarsOracle":
         """Returns the environment's `FreeVarsOracle`."""
         return self._free_vars_oracle
 
     @property
     def expression_manager(self) -> "unified_planning.model.ExpressionManager":
         """Returns the environment's `ExpressionManager`."""
         return self._expression_manager
 
     @property
-    def type_manager(self) -> "unified_planning.model.TypeManager":
+    def type_manager(self) -> "unified_planning.model.type_manager.TypeManager":
         """Returns the environment's `TypeManager`."""
         return self._type_manager
 
     @property
     def type_checker(self) -> "unified_planning.model.walkers.TypeChecker":
         """Returns the environment's `TypeChecker`."""
         """Get the Type Checker"""
@@ -93,39 +114,49 @@
 
     @property
     def simplifier(self) -> "unified_planning.model.walkers.Simplifier":
         """Returns the environment's `Simplifier`."""
         return self._simplifier
 
     @property
+    def substituter(self) -> "unified_planning.model.walkers.Substituter":
+        """Returns the environment's `Substituter`."""
+        return self._substituter
+
+    @property
     def free_vars_extractor(self) -> "unified_planning.model.walkers.FreeVarsExtractor":
         """Returns the environment's `FreeVarsExtractor`."""
         return self._free_vars_extractor
 
     @property
+    def names_extractor(self) -> "unified_planning.model.walkers.NamesExtractor":
+        """Returns the environment's `NamesExtractor`."""
+        return self._names_extractor
+
+    @property
     def credits_stream(self) -> "Optional[IO[str]]":
         """Returns the stream where the :class:`Engines <unified_planning.engines.Engine>` :func:`credits <unified_planning.engines.Engine.get_credits>` are printed."""
         return self._credits_stream
 
     @credits_stream.setter
     def credits_stream(self, new_credits_stream: Optional[IO[str]]):
         """Sets the stream where the :class:`Engines <unified_planning.engines.Engine>` :func:`credits <unified_planning.engines.Engine.get_credits>` are printed."""
         self._credits_stream = new_credits_stream
 
 
 GLOBAL_ENVIRONMENT: Optional[Environment] = None
 
 
-def get_env(env: Optional[Environment] = None) -> Environment:
+def get_environment(environment: Optional[Environment] = None) -> Environment:
     """
-    Returns the given env if it is not `None`, returns the `GLOBAL_ENVIRONMENT` otherwise.
+    Returns the given environment if it is not `None`, returns the `GLOBAL_ENVIRONMENT` otherwise.
 
-    :param env: The environment to return.
+    :param environment: The environment to return.
     :return: The given `environment` if it is not `None`, the `GLOBAL_ENVIRONMENT` otherwise.
     """
     global GLOBAL_ENVIRONMENT
-    if env is None:
+    if environment is None:
         if GLOBAL_ENVIRONMENT is None:
             GLOBAL_ENVIRONMENT = Environment()
         return GLOBAL_ENVIRONMENT
     else:
-        return env
+        return environment
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/exceptions.py` & `unified_planning-0.6.0/unified_planning/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     pass
 
 
 class UPProblemDefinitionError(UPException):
     pass
 
 
+class UPPlanDefinitionError(UPException):
+    pass
+
+
 class UPTypeError(UPException, TypeError):
     pass
 
 
 class UPUnsupportedProblemTypeError(UPException):
     pass
 
@@ -59,7 +63,15 @@
 
 class UPNoRequestedEngineAvailableException(UPException):
     pass
 
 
 class UPConflictingEffectsException(UPException):
     pass
+
+
+class ANMLSyntaxError(UPException, SyntaxError):
+    pass
+
+
+class UPInvalidActionError(UPException):
+    pass
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/grpc/converter.py` & `unified_planning-0.6.0/unified_planning/grpc/converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/grpc/generated/unified_planning_pb2.py` & `unified_planning-0.6.0/unified_planning/grpc/generated/unified_planning_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16unified_planning.proto\"i\n\nExpression\x12\x13\n\x04\x61tom\x18\x01 \x01(\x0b\x32\x05.Atom\x12\x19\n\x04list\x18\x02 \x03(\x0b\x32\x0b.Expression\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x1d\n\x04kind\x18\x04 \x01(\x0e\x32\x0f.ExpressionKind\"\\\n\x04\x41tom\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x15\n\x04real\x18\x03 \x01(\x0b\x32\x05.RealH\x00\x12\x11\n\x07\x62oolean\x18\x04 \x01(\x08H\x00\x42\t\n\x07\x63ontent\".\n\x04Real\x12\x11\n\tnumerator\x18\x01 \x01(\x03\x12\x13\n\x0b\x64\x65nominator\x18\x02 \x01(\x03\"9\n\x0fTypeDeclaration\x12\x11\n\ttype_name\x18\x01 \x01(\t\x12\x13\n\x0bparent_type\x18\x02 \x01(\t\"\'\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"n\n\x06\x46luent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nvalue_type\x18\x02 \x01(\t\x12\x1e\n\nparameters\x18\x03 \x03(\x0b\x32\n.Parameter\x12\"\n\rdefault_value\x18\x04 \x01(\x0b\x32\x0b.Expression\"/\n\x11ObjectDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\xcd\x01\n\x10\x45\x66\x66\x65\x63tExpression\x12*\n\x04kind\x18\x01 \x01(\x0e\x32\x1c.EffectExpression.EffectKind\x12\x1b\n\x06\x66luent\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x03 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\tcondition\x18\x04 \x01(\x0b\x32\x0b.Expression\"4\n\nEffectKind\x12\n\n\x06\x41SSIGN\x10\x00\x12\x0c\n\x08INCREASE\x10\x01\x12\x0c\n\x08\x44\x45\x43REASE\x10\x02\"M\n\x06\x45\x66\x66\x65\x63t\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"C\n\tCondition\x12\x19\n\x04\x63ond\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1b\n\x04span\x18\x02 \x01(\x0b\x32\r.TimeInterval\"\x8d\x01\n\x06\x41\x63tion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.Duration\x12\x1e\n\nconditions\x18\x04 \x03(\x0b\x32\n.Condition\x12\x18\n\x07\x65\x66\x66\x65\x63ts\x18\x05 \x03(\x0b\x32\x07.Effect\"\x90\x01\n\tTimepoint\x12&\n\x04kind\x18\x01 \x01(\x0e\x32\x18.Timepoint.TimepointKind\x12\x14\n\x0c\x63ontainer_id\x18\x02 \x01(\t\"E\n\rTimepointKind\x12\x10\n\x0cGLOBAL_START\x10\x00\x12\x0e\n\nGLOBAL_END\x10\x01\x12\t\n\x05START\x10\x02\x12\x07\n\x03\x45ND\x10\x03\"=\n\x06Timing\x12\x1d\n\ttimepoint\x18\x01 \x01(\x0b\x32\n.Timepoint\x12\x14\n\x05\x64\x65lay\x18\x02 \x01(\x0b\x32\x05.Real\"o\n\x08Interval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x1a\n\x05lower\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x1a\n\x05upper\x18\x04 \x01(\x0b\x32\x0b.Expression\"k\n\x0cTimeInterval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x16\n\x05lower\x18\x02 \x01(\x0b\x32\x07.Timing\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x16\n\x05upper\x18\x04 \x01(\x0b\x32\x07.Timing\"5\n\x08\x44uration\x12)\n\x16\x63ontrollable_in_bounds\x18\x01 \x01(\x0b\x32\t.Interval\"G\n\x17\x41\x62stractTaskDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\"F\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\ttask_name\x18\x02 \x01(\t\x12\x1f\n\nparameters\x18\x03 \x03(\x0b\x32\x0b.Expression\"\xaf\x01\n\x06Method\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1c\n\rachieved_task\x18\x03 \x01(\x0b\x32\x05.Task\x12\x17\n\x08subtasks\x18\x04 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x05 \x03(\x0b\x32\x0b.Expression\x12\x1e\n\nconditions\x18\x06 \x03(\x0b\x32\n.Condition\"g\n\x0bTaskNetwork\x12\x1d\n\tvariables\x18\x01 \x03(\x0b\x32\n.Parameter\x12\x17\n\x08subtasks\x18\x02 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x03 \x03(\x0b\x32\x0b.Expression\"\x83\x01\n\tHierarchy\x12\x30\n\x0e\x61\x62stract_tasks\x18\x01 \x03(\x0b\x32\x18.AbstractTaskDeclaration\x12\x18\n\x07methods\x18\x02 \x03(\x0b\x32\x07.Method\x12*\n\x14initial_task_network\x18\x03 \x01(\x0b\x32\x0c.TaskNetwork\"@\n\x04Goal\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\"R\n\x0bTimedEffect\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"E\n\nAssignment\x12\x1b\n\x06\x66luent\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression\">\n\x0cGoalWithCost\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x13\n\x04\x63ost\x18\x02 \x01(\x0b\x32\x05.Real\"\xd0\x03\n\x06Metric\x12 \n\x04kind\x18\x01 \x01(\x0e\x32\x12.Metric.MetricKind\x12\x1f\n\nexpression\x18\x02 \x01(\x0b\x32\x0b.Expression\x12.\n\x0c\x61\x63tion_costs\x18\x03 \x03(\x0b\x32\x18.Metric.ActionCostsEntry\x12(\n\x13\x64\x65\x66\x61ult_action_cost\x18\x04 \x01(\x0b\x32\x0b.Expression\x12\x1c\n\x05goals\x18\x05 \x03(\x0b\x32\r.GoalWithCost\x1a?\n\x10\x41\x63tionCostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression:\x02\x38\x01\"\xc9\x01\n\nMetricKind\x12\x19\n\x15MINIMIZE_ACTION_COSTS\x10\x00\x12#\n\x1fMINIMIZE_SEQUENTIAL_PLAN_LENGTH\x10\x01\x12\x15\n\x11MINIMIZE_MAKESPAN\x10\x02\x12&\n\"MINIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x03\x12&\n\"MAXIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x04\x12\x14\n\x10OVERSUBSCRIPTION\x10\x05\"\xe2\x02\n\x07Problem\x12\x13\n\x0b\x64omain_name\x18\x01 \x01(\t\x12\x14\n\x0cproblem_name\x18\x02 \x01(\t\x12\x1f\n\x05types\x18\x03 \x03(\x0b\x32\x10.TypeDeclaration\x12\x18\n\x07\x66luents\x18\x04 \x03(\x0b\x32\x07.Fluent\x12#\n\x07objects\x18\x05 \x03(\x0b\x32\x12.ObjectDeclaration\x12\x18\n\x07\x61\x63tions\x18\x06 \x03(\x0b\x32\x07.Action\x12\"\n\rinitial_state\x18\x07 \x03(\x0b\x32\x0b.Assignment\x12#\n\rtimed_effects\x18\x08 \x03(\x0b\x32\x0c.TimedEffect\x12\x14\n\x05goals\x18\t \x03(\x0b\x32\x05.Goal\x12\x1a\n\x08\x66\x65\x61tures\x18\n \x03(\x0e\x32\x08.Feature\x12\x18\n\x07metrics\x18\x0b \x03(\x0b\x32\x07.Metric\x12\x1d\n\thierarchy\x18\x0c \x01(\x0b\x32\n.Hierarchy\"\x80\x01\n\x0e\x41\x63tionInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63tion_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12\x19\n\nstart_time\x18\x04 \x01(\x0b\x32\x05.Real\x12\x17\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x05.Real\"(\n\x04Plan\x12 \n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x0f.ActionInstance\"\x83\x02\n\x0bPlanRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12*\n\x0fresolution_mode\x18\x02 \x01(\x0e\x32\x11.PlanRequest.Mode\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x37\n\x0e\x65ngine_options\x18\x04 \x03(\x0b\x32\x1f.PlanRequest.EngineOptionsEntry\x1a\x34\n\x12\x45ngineOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x04Mode\x12\x0f\n\x0bSATISFIABLE\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\"C\n\x11ValidationRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\"{\n\nLogMessage\x12#\n\x05level\x18\x01 \x01(\x0e\x32\x14.LogMessage.LogLevel\x12\x0f\n\x07message\x18\x02 \x01(\t\"7\n\x08LogLevel\x12\t\n\x05\x44\x45\x42UG\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\t\n\x05\x45RROR\x10\x03\"\xbf\x03\n\x14PlanGenerationResult\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.PlanGenerationResult.Status\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\x12\x33\n\x07metrics\x18\x03 \x03(\x0b\x32\".PlanGenerationResult.MetricsEntry\x12!\n\x0clog_messages\x18\x04 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x05 \x01(\x0b\x32\x07.Engine\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc2\x01\n\x06Status\x12\x16\n\x12SOLVED_SATISFICING\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\x12\x15\n\x11UNSOLVABLE_PROVEN\x10\x02\x12\x1b\n\x17UNSOLVABLE_INCOMPLETELY\x10\x03\x12\x0b\n\x07TIMEOUT\x10\r\x12\n\n\x06MEMOUT\x10\x0e\x12\x12\n\x0eINTERNAL_ERROR\x10\x0f\x12\x17\n\x13UNSUPPORTED_PROBLEM\x10\x10\x12\x10\n\x0cINTERMEDIATE\x10\x11\"\x16\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xba\x01\n\x10ValidationResult\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.ValidationResult.ValidationResultStatus\x12!\n\x0clog_messages\x18\x02 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x03 \x01(\x0b\x32\x07.Engine\"0\n\x16ValidationResultStatus\x12\t\n\x05VALID\x10\x00\x12\x0b\n\x07INVALID\x10\x01\"\xe5\x01\n\x0e\x43ompilerResult\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x37\n\rmap_back_plan\x18\x02 \x03(\x0b\x32 .CompilerResult.MapBackPlanEntry\x12!\n\x0clog_messages\x18\x03 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x04 \x01(\x0b\x32\x07.Engine\x1a\x43\n\x10MapBackPlanEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.ActionInstance:\x02\x38\x01*\xb0\x01\n\x0e\x45xpressionKind\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x43ONSTANT\x10\x01\x12\r\n\tPARAMETER\x10\x02\x12\x0c\n\x08VARIABLE\x10\x07\x12\x11\n\rFLUENT_SYMBOL\x10\x03\x12\x13\n\x0f\x46UNCTION_SYMBOL\x10\x04\x12\x12\n\x0eSTATE_VARIABLE\x10\x05\x12\x18\n\x14\x46UNCTION_APPLICATION\x10\x06\x12\x10\n\x0c\x43ONTAINER_ID\x10\x08*\xde\x05\n\x07\x46\x65\x61ture\x12\x10\n\x0c\x41\x43TION_BASED\x10\x00\x12\x10\n\x0cHIERARCHICAL\x10\x1a\x12\x1b\n\x17SIMPLE_NUMERIC_PLANNING\x10\x1e\x12\x1c\n\x18GENERAL_NUMERIC_PLANNING\x10\x1f\x12\x13\n\x0f\x43ONTINUOUS_TIME\x10\x01\x12\x11\n\rDISCRETE_TIME\x10\x02\x12\'\n#INTERMEDIATE_CONDITIONS_AND_EFFECTS\x10\x03\x12\x10\n\x0cTIMED_EFFECT\x10\x04\x12\x0f\n\x0bTIMED_GOALS\x10\x05\x12\x19\n\x15\x44URATION_INEQUALITIES\x10\x06\x12\x1e\n\x1aSTATIC_FLUENTS_IN_DURATION\x10\x1b\x12\x17\n\x13\x46LUENTS_IN_DURATION\x10\x1c\x12\x16\n\x12\x43ONTINUOUS_NUMBERS\x10\x07\x12\x14\n\x10\x44ISCRETE_NUMBERS\x10\x08\x12\x17\n\x13NEGATIVE_CONDITIONS\x10\t\x12\x1a\n\x16\x44ISJUNCTIVE_CONDITIONS\x10\n\x12\x0c\n\x08\x45QUALITY\x10\x0b\x12\x1a\n\x16\x45XISTENTIAL_CONDITIONS\x10\x0c\x12\x18\n\x14UNIVERSAL_CONDITIONS\x10\r\x12\x17\n\x13\x43ONDITIONAL_EFFECTS\x10\x0e\x12\x14\n\x10INCREASE_EFFECTS\x10\x0f\x12\x14\n\x10\x44\x45\x43REASE_EFFECTS\x10\x10\x12\x0f\n\x0b\x46LAT_TYPING\x10\x11\x12\x17\n\x13HIERARCHICAL_TYPING\x10\x12\x12\x13\n\x0fNUMERIC_FLUENTS\x10\x13\x12\x12\n\x0eOBJECT_FLUENTS\x10\x14\x12\x10\n\x0c\x41\x43TIONS_COST\x10\x15\x12\x0f\n\x0b\x46INAL_VALUE\x10\x16\x12\x0c\n\x08MAKESPAN\x10\x17\x12\x0f\n\x0bPLAN_LENGTH\x10\x18\x12\x14\n\x10OVERSUBSCRIPTION\x10\x1d\x12\x15\n\x11SIMULATED_EFFECTS\x10\x19\x32\xd8\x01\n\x0fUnifiedPlanning\x12\x34\n\x0bplanAnytime\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult0\x01\x12\x32\n\x0bplanOneShot\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult\x12\x35\n\x0cvalidatePlan\x12\x12.ValidationRequest\x1a\x11.ValidationResult\x12$\n\x07\x63ompile\x12\x08.Problem\x1a\x0f.CompilerResultb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16unified_planning.proto\"i\n\nExpression\x12\x13\n\x04\x61tom\x18\x01 \x01(\x0b\x32\x05.Atom\x12\x19\n\x04list\x18\x02 \x03(\x0b\x32\x0b.Expression\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x1d\n\x04kind\x18\x04 \x01(\x0e\x32\x0f.ExpressionKind\"\\\n\x04\x41tom\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x15\n\x04real\x18\x03 \x01(\x0b\x32\x05.RealH\x00\x12\x11\n\x07\x62oolean\x18\x04 \x01(\x08H\x00\x42\t\n\x07\x63ontent\".\n\x04Real\x12\x11\n\tnumerator\x18\x01 \x01(\x03\x12\x13\n\x0b\x64\x65nominator\x18\x02 \x01(\x03\"9\n\x0fTypeDeclaration\x12\x11\n\ttype_name\x18\x01 \x01(\t\x12\x13\n\x0bparent_type\x18\x02 \x01(\t\"\'\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"n\n\x06\x46luent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nvalue_type\x18\x02 \x01(\t\x12\x1e\n\nparameters\x18\x03 \x03(\x0b\x32\n.Parameter\x12\"\n\rdefault_value\x18\x04 \x01(\x0b\x32\x0b.Expression\"/\n\x11ObjectDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\xcd\x01\n\x10\x45\x66\x66\x65\x63tExpression\x12*\n\x04kind\x18\x01 \x01(\x0e\x32\x1c.EffectExpression.EffectKind\x12\x1b\n\x06\x66luent\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x03 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\tcondition\x18\x04 \x01(\x0b\x32\x0b.Expression\"4\n\nEffectKind\x12\n\n\x06\x41SSIGN\x10\x00\x12\x0c\n\x08INCREASE\x10\x01\x12\x0c\n\x08\x44\x45\x43REASE\x10\x02\"M\n\x06\x45\x66\x66\x65\x63t\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"C\n\tCondition\x12\x19\n\x04\x63ond\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1b\n\x04span\x18\x02 \x01(\x0b\x32\r.TimeInterval\"\x8d\x01\n\x06\x41\x63tion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.Duration\x12\x1e\n\nconditions\x18\x04 \x03(\x0b\x32\n.Condition\x12\x18\n\x07\x65\x66\x66\x65\x63ts\x18\x05 \x03(\x0b\x32\x07.Effect\"\x90\x01\n\tTimepoint\x12&\n\x04kind\x18\x01 \x01(\x0e\x32\x18.Timepoint.TimepointKind\x12\x14\n\x0c\x63ontainer_id\x18\x02 \x01(\t\"E\n\rTimepointKind\x12\x10\n\x0cGLOBAL_START\x10\x00\x12\x0e\n\nGLOBAL_END\x10\x01\x12\t\n\x05START\x10\x02\x12\x07\n\x03\x45ND\x10\x03\"=\n\x06Timing\x12\x1d\n\ttimepoint\x18\x01 \x01(\x0b\x32\n.Timepoint\x12\x14\n\x05\x64\x65lay\x18\x02 \x01(\x0b\x32\x05.Real\"o\n\x08Interval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x1a\n\x05lower\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x1a\n\x05upper\x18\x04 \x01(\x0b\x32\x0b.Expression\"k\n\x0cTimeInterval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x16\n\x05lower\x18\x02 \x01(\x0b\x32\x07.Timing\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x16\n\x05upper\x18\x04 \x01(\x0b\x32\x07.Timing\"5\n\x08\x44uration\x12)\n\x16\x63ontrollable_in_bounds\x18\x01 \x01(\x0b\x32\t.Interval\"G\n\x17\x41\x62stractTaskDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\"F\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\ttask_name\x18\x02 \x01(\t\x12\x1f\n\nparameters\x18\x03 \x03(\x0b\x32\x0b.Expression\"\xaf\x01\n\x06Method\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1c\n\rachieved_task\x18\x03 \x01(\x0b\x32\x05.Task\x12\x17\n\x08subtasks\x18\x04 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x05 \x03(\x0b\x32\x0b.Expression\x12\x1e\n\nconditions\x18\x06 \x03(\x0b\x32\n.Condition\"g\n\x0bTaskNetwork\x12\x1d\n\tvariables\x18\x01 \x03(\x0b\x32\n.Parameter\x12\x17\n\x08subtasks\x18\x02 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x03 \x03(\x0b\x32\x0b.Expression\"\x83\x01\n\tHierarchy\x12\x30\n\x0e\x61\x62stract_tasks\x18\x01 \x03(\x0b\x32\x18.AbstractTaskDeclaration\x12\x18\n\x07methods\x18\x02 \x03(\x0b\x32\x07.Method\x12*\n\x14initial_task_network\x18\x03 \x01(\x0b\x32\x0c.TaskNetwork\"@\n\x04Goal\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\"R\n\x0bTimedEffect\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"E\n\nAssignment\x12\x1b\n\x06\x66luent\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression\"B\n\x0eGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x15\n\x06weight\x18\x02 \x01(\x0b\x32\x05.Real\"f\n\x13TimedGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\x12\x15\n\x06weight\x18\x03 \x01(\x0b\x32\x05.Real\"\x9c\x04\n\x06Metric\x12 \n\x04kind\x18\x01 \x01(\x0e\x32\x12.Metric.MetricKind\x12\x1f\n\nexpression\x18\x02 \x01(\x0b\x32\x0b.Expression\x12.\n\x0c\x61\x63tion_costs\x18\x03 \x03(\x0b\x32\x18.Metric.ActionCostsEntry\x12(\n\x13\x64\x65\x66\x61ult_action_cost\x18\x04 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\x05goals\x18\x05 \x03(\x0b\x32\x0f.GoalWithWeight\x12)\n\x0btimed_goals\x18\x06 \x03(\x0b\x32\x14.TimedGoalWithWeight\x1a?\n\x10\x41\x63tionCostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression:\x02\x38\x01\"\xe8\x01\n\nMetricKind\x12\x19\n\x15MINIMIZE_ACTION_COSTS\x10\x00\x12#\n\x1fMINIMIZE_SEQUENTIAL_PLAN_LENGTH\x10\x01\x12\x15\n\x11MINIMIZE_MAKESPAN\x10\x02\x12&\n\"MINIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x03\x12&\n\"MAXIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x04\x12\x14\n\x10OVERSUBSCRIPTION\x10\x05\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10\x06\"\xe2\x02\n\x07Problem\x12\x13\n\x0b\x64omain_name\x18\x01 \x01(\t\x12\x14\n\x0cproblem_name\x18\x02 \x01(\t\x12\x1f\n\x05types\x18\x03 \x03(\x0b\x32\x10.TypeDeclaration\x12\x18\n\x07\x66luents\x18\x04 \x03(\x0b\x32\x07.Fluent\x12#\n\x07objects\x18\x05 \x03(\x0b\x32\x12.ObjectDeclaration\x12\x18\n\x07\x61\x63tions\x18\x06 \x03(\x0b\x32\x07.Action\x12\"\n\rinitial_state\x18\x07 \x03(\x0b\x32\x0b.Assignment\x12#\n\rtimed_effects\x18\x08 \x03(\x0b\x32\x0c.TimedEffect\x12\x14\n\x05goals\x18\t \x03(\x0b\x32\x05.Goal\x12\x1a\n\x08\x66\x65\x61tures\x18\n \x03(\x0e\x32\x08.Feature\x12\x18\n\x07metrics\x18\x0b \x03(\x0b\x32\x07.Metric\x12\x1d\n\thierarchy\x18\x0c \x01(\x0b\x32\n.Hierarchy\"\x80\x01\n\x0e\x41\x63tionInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63tion_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12\x19\n\nstart_time\x18\x04 \x01(\x0b\x32\x05.Real\x12\x17\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x05.Real\"\xae\x01\n\x0eMethodInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bmethod_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12/\n\x08subtasks\x18\x06 \x03(\x0b\x32\x1d.MethodInstance.SubtasksEntry\x1a/\n\rSubtasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x96\x01\n\rPlanHierarchy\x12\x31\n\nroot_tasks\x18\x01 \x03(\x0b\x32\x1d.PlanHierarchy.RootTasksEntry\x12 \n\x07methods\x18\x02 \x03(\x0b\x32\x0f.MethodInstance\x1a\x30\n\x0eRootTasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"K\n\x04Plan\x12 \n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x0f.ActionInstance\x12!\n\thierarchy\x18\x02 \x01(\x0b\x32\x0e.PlanHierarchy\"\x83\x02\n\x0bPlanRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12*\n\x0fresolution_mode\x18\x02 \x01(\x0e\x32\x11.PlanRequest.Mode\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x37\n\x0e\x65ngine_options\x18\x04 \x03(\x0b\x32\x1f.PlanRequest.EngineOptionsEntry\x1a\x34\n\x12\x45ngineOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x04Mode\x12\x0f\n\x0bSATISFIABLE\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\"C\n\x11ValidationRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\"{\n\nLogMessage\x12#\n\x05level\x18\x01 \x01(\x0e\x32\x14.LogMessage.LogLevel\x12\x0f\n\x07message\x18\x02 \x01(\t\"7\n\x08LogLevel\x12\t\n\x05\x44\x45\x42UG\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\t\n\x05\x45RROR\x10\x03\"\xbf\x03\n\x14PlanGenerationResult\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.PlanGenerationResult.Status\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\x12\x33\n\x07metrics\x18\x03 \x03(\x0b\x32\".PlanGenerationResult.MetricsEntry\x12!\n\x0clog_messages\x18\x04 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x05 \x01(\x0b\x32\x07.Engine\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc2\x01\n\x06Status\x12\x16\n\x12SOLVED_SATISFICING\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\x12\x15\n\x11UNSOLVABLE_PROVEN\x10\x02\x12\x1b\n\x17UNSOLVABLE_INCOMPLETELY\x10\x03\x12\x0b\n\x07TIMEOUT\x10\r\x12\n\n\x06MEMOUT\x10\x0e\x12\x12\n\x0eINTERNAL_ERROR\x10\x0f\x12\x17\n\x13UNSUPPORTED_PROBLEM\x10\x10\x12\x10\n\x0cINTERMEDIATE\x10\x11\"\x16\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xba\x01\n\x10ValidationResult\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.ValidationResult.ValidationResultStatus\x12!\n\x0clog_messages\x18\x02 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x03 \x01(\x0b\x32\x07.Engine\"0\n\x16ValidationResultStatus\x12\t\n\x05VALID\x10\x00\x12\x0b\n\x07INVALID\x10\x01\"\xe5\x01\n\x0e\x43ompilerResult\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x37\n\rmap_back_plan\x18\x02 \x03(\x0b\x32 .CompilerResult.MapBackPlanEntry\x12!\n\x0clog_messages\x18\x03 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x04 \x01(\x0b\x32\x07.Engine\x1a\x43\n\x10MapBackPlanEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.ActionInstance:\x02\x38\x01*\xb0\x01\n\x0e\x45xpressionKind\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x43ONSTANT\x10\x01\x12\r\n\tPARAMETER\x10\x02\x12\x0c\n\x08VARIABLE\x10\x07\x12\x11\n\rFLUENT_SYMBOL\x10\x03\x12\x13\n\x0f\x46UNCTION_SYMBOL\x10\x04\x12\x12\n\x0eSTATE_VARIABLE\x10\x05\x12\x18\n\x14\x46UNCTION_APPLICATION\x10\x06\x12\x10\n\x0c\x43ONTAINER_ID\x10\x08*\xbc\t\n\x07\x46\x65\x61ture\x12\x10\n\x0c\x41\x43TION_BASED\x10\x00\x12\x10\n\x0cHIERARCHICAL\x10\x1a\x12\x1b\n\x17SIMPLE_NUMERIC_PLANNING\x10\x1e\x12\x1c\n\x18GENERAL_NUMERIC_PLANNING\x10\x1f\x12\x13\n\x0f\x43ONTINUOUS_TIME\x10\x01\x12\x11\n\rDISCRETE_TIME\x10\x02\x12\'\n#INTERMEDIATE_CONDITIONS_AND_EFFECTS\x10\x03\x12#\n\x1f\x45XTERNAL_CONDITIONS_AND_EFFECTS\x10\'\x12\x11\n\rTIMED_EFFECTS\x10\x04\x12\x0f\n\x0bTIMED_GOALS\x10\x05\x12\x19\n\x15\x44URATION_INEQUALITIES\x10\x06\x12\x1f\n\x1bSTATIC_FLUENTS_IN_DURATIONS\x10\x1b\x12\x18\n\x14\x46LUENTS_IN_DURATIONS\x10\x1c\x12\x16\n\x12\x43ONTINUOUS_NUMBERS\x10\x07\x12\x14\n\x10\x44ISCRETE_NUMBERS\x10\x08\x12\x11\n\rBOUNDED_TYPES\x10&\x12\x17\n\x13NEGATIVE_CONDITIONS\x10\t\x12\x1a\n\x16\x44ISJUNCTIVE_CONDITIONS\x10\n\x12\x0e\n\nEQUALITIES\x10\x0b\x12\x1a\n\x16\x45XISTENTIAL_CONDITIONS\x10\x0c\x12\x18\n\x14UNIVERSAL_CONDITIONS\x10\r\x12\x17\n\x13\x43ONDITIONAL_EFFECTS\x10\x0e\x12\x14\n\x10INCREASE_EFFECTS\x10\x0f\x12\x14\n\x10\x44\x45\x43REASE_EFFECTS\x10\x10\x12)\n%STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS\x10)\x12)\n%STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS\x10*\x12\"\n\x1e\x46LUENTS_IN_BOOLEAN_ASSIGNMENTS\x10+\x12\"\n\x1e\x46LUENTS_IN_NUMERIC_ASSIGNMENTS\x10,\x12\x0f\n\x0b\x46LAT_TYPING\x10\x11\x12\x17\n\x13HIERARCHICAL_TYPING\x10\x12\x12\x13\n\x0fNUMERIC_FLUENTS\x10\x13\x12\x12\n\x0eOBJECT_FLUENTS\x10\x14\x12\x10\n\x0c\x41\x43TIONS_COST\x10\x15\x12\x0f\n\x0b\x46INAL_VALUE\x10\x16\x12\x0c\n\x08MAKESPAN\x10\x17\x12\x0f\n\x0bPLAN_LENGTH\x10\x18\x12\x14\n\x10OVERSUBSCRIPTION\x10\x1d\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10(\x12\"\n\x1eSTATIC_FLUENTS_IN_ACTIONS_COST\x10-\x12\x1b\n\x17\x46LUENTS_IN_ACTIONS_COST\x10.\x12\x15\n\x11SIMULATED_EFFECTS\x10\x19\x12\x18\n\x14METHOD_PRECONDITIONS\x10 \x12\x1c\n\x18TASK_NETWORK_CONSTRAINTS\x10!\x12\"\n\x1eINITIAL_TASK_NETWORK_VARIABLES\x10\"\x12\x14\n\x10TASK_ORDER_TOTAL\x10#\x12\x16\n\x12TASK_ORDER_PARTIAL\x10$\x12\x17\n\x13TASK_ORDER_TEMPORAL\x10%2\xd8\x01\n\x0fUnifiedPlanning\x12\x34\n\x0bplanAnytime\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult0\x01\x12\x32\n\x0bplanOneShot\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult\x12\x35\n\x0cvalidatePlan\x12\x12.ValidationRequest\x1a\x11.ValidationResult\x12$\n\x07\x63ompile\x12\x08.Problem\x1a\x0f.CompilerResultb\x06proto3')
 
 _EXPRESSIONKIND = DESCRIPTOR.enum_types_by_name['ExpressionKind']
 ExpressionKind = enum_type_wrapper.EnumTypeWrapper(_EXPRESSIONKIND)
 _FEATURE = DESCRIPTOR.enum_types_by_name['Feature']
 Feature = enum_type_wrapper.EnumTypeWrapper(_FEATURE)
 UNKNOWN = 0
 CONSTANT = 1
@@ -33,39 +33,54 @@
 ACTION_BASED = 0
 HIERARCHICAL = 26
 SIMPLE_NUMERIC_PLANNING = 30
 GENERAL_NUMERIC_PLANNING = 31
 CONTINUOUS_TIME = 1
 DISCRETE_TIME = 2
 INTERMEDIATE_CONDITIONS_AND_EFFECTS = 3
-TIMED_EFFECT = 4
+EXTERNAL_CONDITIONS_AND_EFFECTS = 39
+TIMED_EFFECTS = 4
 TIMED_GOALS = 5
 DURATION_INEQUALITIES = 6
-STATIC_FLUENTS_IN_DURATION = 27
-FLUENTS_IN_DURATION = 28
+STATIC_FLUENTS_IN_DURATIONS = 27
+FLUENTS_IN_DURATIONS = 28
 CONTINUOUS_NUMBERS = 7
 DISCRETE_NUMBERS = 8
+BOUNDED_TYPES = 38
 NEGATIVE_CONDITIONS = 9
 DISJUNCTIVE_CONDITIONS = 10
-EQUALITY = 11
+EQUALITIES = 11
 EXISTENTIAL_CONDITIONS = 12
 UNIVERSAL_CONDITIONS = 13
 CONDITIONAL_EFFECTS = 14
 INCREASE_EFFECTS = 15
 DECREASE_EFFECTS = 16
+STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS = 41
+STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS = 42
+FLUENTS_IN_BOOLEAN_ASSIGNMENTS = 43
+FLUENTS_IN_NUMERIC_ASSIGNMENTS = 44
 FLAT_TYPING = 17
 HIERARCHICAL_TYPING = 18
 NUMERIC_FLUENTS = 19
 OBJECT_FLUENTS = 20
 ACTIONS_COST = 21
 FINAL_VALUE = 22
 MAKESPAN = 23
 PLAN_LENGTH = 24
 OVERSUBSCRIPTION = 29
+TEMPORAL_OVERSUBSCRIPTION = 40
+STATIC_FLUENTS_IN_ACTIONS_COST = 45
+FLUENTS_IN_ACTIONS_COST = 46
 SIMULATED_EFFECTS = 25
+METHOD_PRECONDITIONS = 32
+TASK_NETWORK_CONSTRAINTS = 33
+INITIAL_TASK_NETWORK_VARIABLES = 34
+TASK_ORDER_TOTAL = 35
+TASK_ORDER_PARTIAL = 36
+TASK_ORDER_TEMPORAL = 37
 
 
 _EXPRESSION = DESCRIPTOR.message_types_by_name['Expression']
 _ATOM = DESCRIPTOR.message_types_by_name['Atom']
 _REAL = DESCRIPTOR.message_types_by_name['Real']
 _TYPEDECLARATION = DESCRIPTOR.message_types_by_name['TypeDeclaration']
 _PARAMETER = DESCRIPTOR.message_types_by_name['Parameter']
@@ -84,19 +99,24 @@
 _TASK = DESCRIPTOR.message_types_by_name['Task']
 _METHOD = DESCRIPTOR.message_types_by_name['Method']
 _TASKNETWORK = DESCRIPTOR.message_types_by_name['TaskNetwork']
 _HIERARCHY = DESCRIPTOR.message_types_by_name['Hierarchy']
 _GOAL = DESCRIPTOR.message_types_by_name['Goal']
 _TIMEDEFFECT = DESCRIPTOR.message_types_by_name['TimedEffect']
 _ASSIGNMENT = DESCRIPTOR.message_types_by_name['Assignment']
-_GOALWITHCOST = DESCRIPTOR.message_types_by_name['GoalWithCost']
+_GOALWITHWEIGHT = DESCRIPTOR.message_types_by_name['GoalWithWeight']
+_TIMEDGOALWITHWEIGHT = DESCRIPTOR.message_types_by_name['TimedGoalWithWeight']
 _METRIC = DESCRIPTOR.message_types_by_name['Metric']
 _METRIC_ACTIONCOSTSENTRY = _METRIC.nested_types_by_name['ActionCostsEntry']
 _PROBLEM = DESCRIPTOR.message_types_by_name['Problem']
 _ACTIONINSTANCE = DESCRIPTOR.message_types_by_name['ActionInstance']
+_METHODINSTANCE = DESCRIPTOR.message_types_by_name['MethodInstance']
+_METHODINSTANCE_SUBTASKSENTRY = _METHODINSTANCE.nested_types_by_name['SubtasksEntry']
+_PLANHIERARCHY = DESCRIPTOR.message_types_by_name['PlanHierarchy']
+_PLANHIERARCHY_ROOTTASKSENTRY = _PLANHIERARCHY.nested_types_by_name['RootTasksEntry']
 _PLAN = DESCRIPTOR.message_types_by_name['Plan']
 _PLANREQUEST = DESCRIPTOR.message_types_by_name['PlanRequest']
 _PLANREQUEST_ENGINEOPTIONSENTRY = _PLANREQUEST.nested_types_by_name['EngineOptionsEntry']
 _VALIDATIONREQUEST = DESCRIPTOR.message_types_by_name['ValidationRequest']
 _LOGMESSAGE = DESCRIPTOR.message_types_by_name['LogMessage']
 _PLANGENERATIONRESULT = DESCRIPTOR.message_types_by_name['PlanGenerationResult']
 _PLANGENERATIONRESULT_METRICSENTRY = _PLANGENERATIONRESULT.nested_types_by_name['MetricsEntry']
@@ -275,20 +295,27 @@
 Assignment = _reflection.GeneratedProtocolMessageType('Assignment', (_message.Message,), {
   'DESCRIPTOR' : _ASSIGNMENT,
   '__module__' : 'unified_planning_pb2'
   # @@protoc_insertion_point(class_scope:Assignment)
   })
 _sym_db.RegisterMessage(Assignment)
 
-GoalWithCost = _reflection.GeneratedProtocolMessageType('GoalWithCost', (_message.Message,), {
-  'DESCRIPTOR' : _GOALWITHCOST,
+GoalWithWeight = _reflection.GeneratedProtocolMessageType('GoalWithWeight', (_message.Message,), {
+  'DESCRIPTOR' : _GOALWITHWEIGHT,
   '__module__' : 'unified_planning_pb2'
-  # @@protoc_insertion_point(class_scope:GoalWithCost)
+  # @@protoc_insertion_point(class_scope:GoalWithWeight)
   })
-_sym_db.RegisterMessage(GoalWithCost)
+_sym_db.RegisterMessage(GoalWithWeight)
+
+TimedGoalWithWeight = _reflection.GeneratedProtocolMessageType('TimedGoalWithWeight', (_message.Message,), {
+  'DESCRIPTOR' : _TIMEDGOALWITHWEIGHT,
+  '__module__' : 'unified_planning_pb2'
+  # @@protoc_insertion_point(class_scope:TimedGoalWithWeight)
+  })
+_sym_db.RegisterMessage(TimedGoalWithWeight)
 
 Metric = _reflection.GeneratedProtocolMessageType('Metric', (_message.Message,), {
 
   'ActionCostsEntry' : _reflection.GeneratedProtocolMessageType('ActionCostsEntry', (_message.Message,), {
     'DESCRIPTOR' : _METRIC_ACTIONCOSTSENTRY,
     '__module__' : 'unified_planning_pb2'
     # @@protoc_insertion_point(class_scope:Metric.ActionCostsEntry)
@@ -311,14 +338,44 @@
 ActionInstance = _reflection.GeneratedProtocolMessageType('ActionInstance', (_message.Message,), {
   'DESCRIPTOR' : _ACTIONINSTANCE,
   '__module__' : 'unified_planning_pb2'
   # @@protoc_insertion_point(class_scope:ActionInstance)
   })
 _sym_db.RegisterMessage(ActionInstance)
 
+MethodInstance = _reflection.GeneratedProtocolMessageType('MethodInstance', (_message.Message,), {
+
+  'SubtasksEntry' : _reflection.GeneratedProtocolMessageType('SubtasksEntry', (_message.Message,), {
+    'DESCRIPTOR' : _METHODINSTANCE_SUBTASKSENTRY,
+    '__module__' : 'unified_planning_pb2'
+    # @@protoc_insertion_point(class_scope:MethodInstance.SubtasksEntry)
+    })
+  ,
+  'DESCRIPTOR' : _METHODINSTANCE,
+  '__module__' : 'unified_planning_pb2'
+  # @@protoc_insertion_point(class_scope:MethodInstance)
+  })
+_sym_db.RegisterMessage(MethodInstance)
+_sym_db.RegisterMessage(MethodInstance.SubtasksEntry)
+
+PlanHierarchy = _reflection.GeneratedProtocolMessageType('PlanHierarchy', (_message.Message,), {
+
+  'RootTasksEntry' : _reflection.GeneratedProtocolMessageType('RootTasksEntry', (_message.Message,), {
+    'DESCRIPTOR' : _PLANHIERARCHY_ROOTTASKSENTRY,
+    '__module__' : 'unified_planning_pb2'
+    # @@protoc_insertion_point(class_scope:PlanHierarchy.RootTasksEntry)
+    })
+  ,
+  'DESCRIPTOR' : _PLANHIERARCHY,
+  '__module__' : 'unified_planning_pb2'
+  # @@protoc_insertion_point(class_scope:PlanHierarchy)
+  })
+_sym_db.RegisterMessage(PlanHierarchy)
+_sym_db.RegisterMessage(PlanHierarchy.RootTasksEntry)
+
 Plan = _reflection.GeneratedProtocolMessageType('Plan', (_message.Message,), {
   'DESCRIPTOR' : _PLAN,
   '__module__' : 'unified_planning_pb2'
   # @@protoc_insertion_point(class_scope:Plan)
   })
 _sym_db.RegisterMessage(Plan)
 
@@ -397,24 +454,28 @@
 
 _UNIFIEDPLANNING = DESCRIPTOR.services_by_name['UnifiedPlanning']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _METRIC_ACTIONCOSTSENTRY._options = None
   _METRIC_ACTIONCOSTSENTRY._serialized_options = b'8\001'
+  _METHODINSTANCE_SUBTASKSENTRY._options = None
+  _METHODINSTANCE_SUBTASKSENTRY._serialized_options = b'8\001'
+  _PLANHIERARCHY_ROOTTASKSENTRY._options = None
+  _PLANHIERARCHY_ROOTTASKSENTRY._serialized_options = b'8\001'
   _PLANREQUEST_ENGINEOPTIONSENTRY._options = None
   _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_options = b'8\001'
   _PLANGENERATIONRESULT_METRICSENTRY._options = None
   _PLANGENERATIONRESULT_METRICSENTRY._serialized_options = b'8\001'
   _COMPILERRESULT_MAPBACKPLANENTRY._options = None
   _COMPILERRESULT_MAPBACKPLANENTRY._serialized_options = b'8\001'
-  _EXPRESSIONKIND._serialized_start=4719
-  _EXPRESSIONKIND._serialized_end=4895
-  _FEATURE._serialized_start=4898
-  _FEATURE._serialized_end=5632
+  _EXPRESSIONKIND._serialized_start=5268
+  _EXPRESSIONKIND._serialized_end=5444
+  _FEATURE._serialized_start=5447
+  _FEATURE._serialized_end=6659
   _EXPRESSION._serialized_start=26
   _EXPRESSION._serialized_end=131
   _ATOM._serialized_start=133
   _ATOM._serialized_end=225
   _REAL._serialized_start=227
   _REAL._serialized_end=273
   _TYPEDECLARATION._serialized_start=275
@@ -459,52 +520,62 @@
   _HIERARCHY._serialized_end=2083
   _GOAL._serialized_start=2085
   _GOAL._serialized_end=2149
   _TIMEDEFFECT._serialized_start=2151
   _TIMEDEFFECT._serialized_end=2233
   _ASSIGNMENT._serialized_start=2235
   _ASSIGNMENT._serialized_end=2304
-  _GOALWITHCOST._serialized_start=2306
-  _GOALWITHCOST._serialized_end=2368
-  _METRIC._serialized_start=2371
-  _METRIC._serialized_end=2835
-  _METRIC_ACTIONCOSTSENTRY._serialized_start=2568
-  _METRIC_ACTIONCOSTSENTRY._serialized_end=2631
-  _METRIC_METRICKIND._serialized_start=2634
-  _METRIC_METRICKIND._serialized_end=2835
-  _PROBLEM._serialized_start=2838
-  _PROBLEM._serialized_end=3192
-  _ACTIONINSTANCE._serialized_start=3195
-  _ACTIONINSTANCE._serialized_end=3323
-  _PLAN._serialized_start=3325
-  _PLAN._serialized_end=3365
-  _PLANREQUEST._serialized_start=3368
-  _PLANREQUEST._serialized_end=3627
-  _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_start=3528
-  _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_end=3580
-  _PLANREQUEST_MODE._serialized_start=3582
-  _PLANREQUEST_MODE._serialized_end=3627
-  _VALIDATIONREQUEST._serialized_start=3629
-  _VALIDATIONREQUEST._serialized_end=3696
-  _LOGMESSAGE._serialized_start=3698
-  _LOGMESSAGE._serialized_end=3821
-  _LOGMESSAGE_LOGLEVEL._serialized_start=3766
-  _LOGMESSAGE_LOGLEVEL._serialized_end=3821
-  _PLANGENERATIONRESULT._serialized_start=3824
-  _PLANGENERATIONRESULT._serialized_end=4271
-  _PLANGENERATIONRESULT_METRICSENTRY._serialized_start=4028
-  _PLANGENERATIONRESULT_METRICSENTRY._serialized_end=4074
-  _PLANGENERATIONRESULT_STATUS._serialized_start=4077
-  _PLANGENERATIONRESULT_STATUS._serialized_end=4271
-  _ENGINE._serialized_start=4273
-  _ENGINE._serialized_end=4295
-  _VALIDATIONRESULT._serialized_start=4298
-  _VALIDATIONRESULT._serialized_end=4484
-  _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_start=4436
-  _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_end=4484
-  _COMPILERRESULT._serialized_start=4487
-  _COMPILERRESULT._serialized_end=4716
-  _COMPILERRESULT_MAPBACKPLANENTRY._serialized_start=4649
-  _COMPILERRESULT_MAPBACKPLANENTRY._serialized_end=4716
-  _UNIFIEDPLANNING._serialized_start=5635
-  _UNIFIEDPLANNING._serialized_end=5851
+  _GOALWITHWEIGHT._serialized_start=2306
+  _GOALWITHWEIGHT._serialized_end=2372
+  _TIMEDGOALWITHWEIGHT._serialized_start=2374
+  _TIMEDGOALWITHWEIGHT._serialized_end=2476
+  _METRIC._serialized_start=2479
+  _METRIC._serialized_end=3019
+  _METRIC_ACTIONCOSTSENTRY._serialized_start=2721
+  _METRIC_ACTIONCOSTSENTRY._serialized_end=2784
+  _METRIC_METRICKIND._serialized_start=2787
+  _METRIC_METRICKIND._serialized_end=3019
+  _PROBLEM._serialized_start=3022
+  _PROBLEM._serialized_end=3376
+  _ACTIONINSTANCE._serialized_start=3379
+  _ACTIONINSTANCE._serialized_end=3507
+  _METHODINSTANCE._serialized_start=3510
+  _METHODINSTANCE._serialized_end=3684
+  _METHODINSTANCE_SUBTASKSENTRY._serialized_start=3637
+  _METHODINSTANCE_SUBTASKSENTRY._serialized_end=3684
+  _PLANHIERARCHY._serialized_start=3687
+  _PLANHIERARCHY._serialized_end=3837
+  _PLANHIERARCHY_ROOTTASKSENTRY._serialized_start=3789
+  _PLANHIERARCHY_ROOTTASKSENTRY._serialized_end=3837
+  _PLAN._serialized_start=3839
+  _PLAN._serialized_end=3914
+  _PLANREQUEST._serialized_start=3917
+  _PLANREQUEST._serialized_end=4176
+  _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_start=4077
+  _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_end=4129
+  _PLANREQUEST_MODE._serialized_start=4131
+  _PLANREQUEST_MODE._serialized_end=4176
+  _VALIDATIONREQUEST._serialized_start=4178
+  _VALIDATIONREQUEST._serialized_end=4245
+  _LOGMESSAGE._serialized_start=4247
+  _LOGMESSAGE._serialized_end=4370
+  _LOGMESSAGE_LOGLEVEL._serialized_start=4315
+  _LOGMESSAGE_LOGLEVEL._serialized_end=4370
+  _PLANGENERATIONRESULT._serialized_start=4373
+  _PLANGENERATIONRESULT._serialized_end=4820
+  _PLANGENERATIONRESULT_METRICSENTRY._serialized_start=4577
+  _PLANGENERATIONRESULT_METRICSENTRY._serialized_end=4623
+  _PLANGENERATIONRESULT_STATUS._serialized_start=4626
+  _PLANGENERATIONRESULT_STATUS._serialized_end=4820
+  _ENGINE._serialized_start=4822
+  _ENGINE._serialized_end=4844
+  _VALIDATIONRESULT._serialized_start=4847
+  _VALIDATIONRESULT._serialized_end=5033
+  _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_start=4985
+  _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_end=5033
+  _COMPILERRESULT._serialized_start=5036
+  _COMPILERRESULT._serialized_end=5265
+  _COMPILERRESULT_MAPBACKPLANENTRY._serialized_start=5198
+  _COMPILERRESULT_MAPBACKPLANENTRY._serialized_end=5265
+  _UNIFIEDPLANNING._serialized_start=6662
+  _UNIFIEDPLANNING._serialized_end=6878
 # @@protoc_insertion_point(module_scope)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py` & `unified_planning-0.6.0/unified_planning/grpc/generated/unified_planning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/grpc/proto_reader.py` & `unified_planning-0.6.0/unified_planning/grpc/proto_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # type: ignore
+from abc import ABC
 from functools import partial
 from typing import Tuple, Union, Optional
 import fractions
 from typing import OrderedDict
 
 import unified_planning.grpc.generated.unified_planning_pb2 as proto
 from unified_planning.exceptions import UPException
@@ -31,29 +32,32 @@
     InstantaneousAction,
     Parameter,
     Problem,
     Variable,
 )
 from unified_planning.model.effect import EffectKind
 from unified_planning.model.operators import OperatorKind
+from unified_planning.plans import ActionInstance
+from unified_planning.plans.hierarchical_plan import MethodInstance, Decomposition
+from unified_planning.model.htn.hierarchical_problem import HierarchicalProblem
 
 
 def convert_type_str(s: str, problem: Problem) -> model.types.Type:
     if s == "up:bool":
-        return problem.env.type_manager.BoolType()
+        return problem.environment.type_manager.BoolType()
     elif s == "up:integer":
-        return problem.env.type_manager.IntType()
+        return problem.environment.type_manager.IntType()
     elif "up:integer[" in s:
         lb = int(s.split("[")[1].split(",")[0])
         ub = int(s.split(",")[1].split("]")[0])
-        return problem.env.type_manager.IntType(lb, ub)
+        return problem.environment.type_manager.IntType(lb, ub)
     elif s == "up:real":
-        return problem.env.type_manager.RealType()
+        return problem.environment.type_manager.RealType()
     elif "up:real[" in s:
-        return problem.env.type_manager.RealType(
+        return problem.environment.type_manager.RealType(
             lower_bound=fractions.Fraction(s.split("[")[1].split(",")[0]),
             upper_bound=fractions.Fraction(s.split(",")[1].split("]")[0]),
         )
     else:
         assert not s.startswith("up:"), f"Unhandled builtin type: {s}"
         return problem.user_type(s)
 
@@ -99,24 +103,24 @@
     """
 
     @handles(proto.Parameter)
     def _convert_parameter(
         self, msg: proto.Parameter, problem: Problem
     ) -> model.Parameter:
         return model.Parameter(
-            msg.name, convert_type_str(msg.type, problem), problem.env
+            msg.name, convert_type_str(msg.type, problem), problem.environment
         )
 
     @handles(proto.Fluent)
     def _convert_fluent(self, msg: proto.Fluent, problem: Problem) -> model.Fluent:
         value_type: model.types.Type = convert_type_str(msg.value_type, problem)
         sig: list = []
         for p in msg.parameters:
             sig.append(self.convert(p, problem))
-        fluent = model.Fluent(msg.name, value_type, sig, problem.env)
+        fluent = model.Fluent(msg.name, value_type, sig, problem.environment)
         return fluent
 
     @handles(proto.ObjectDeclaration)
     def _convert_object(
         self, msg: proto.ObjectDeclaration, problem: Problem
     ) -> model.Object:
         return model.Object(msg.name, convert_type_str(msg.type, problem))
@@ -126,36 +130,42 @@
         self, msg: proto.Expression, problem: Problem
     ) -> model.Expression:
         if msg.kind == proto.ExpressionKind.Value("CONSTANT"):
             assert msg.atom is not None
             return self.convert(msg.atom, problem)
 
         elif msg.kind == proto.ExpressionKind.Value("PARAMETER"):
-            return problem.env.expression_manager.ParameterExp(
+            return problem.environment.expression_manager.ParameterExp(
                 param=Parameter(
-                    msg.atom.symbol, convert_type_str(msg.type, problem), problem.env
+                    msg.atom.symbol,
+                    convert_type_str(msg.type, problem),
+                    problem.environment,
                 ),
             )
         elif msg.kind == proto.ExpressionKind.Value("VARIABLE"):
-            return problem.env.expression_manager.VariableExp(
+            return problem.environment.expression_manager.VariableExp(
                 var=Variable(
-                    msg.atom.symbol, convert_type_str(msg.type, problem), problem.env
+                    msg.atom.symbol,
+                    convert_type_str(msg.type, problem),
+                    problem.environment,
                 ),
             )
         elif msg.kind == proto.ExpressionKind.Value("STATE_VARIABLE"):
             args = []
             payload = None
 
             fluent = msg.list.pop(0)
             if fluent.kind == proto.ExpressionKind.Value("FLUENT_SYMBOL"):
                 payload = self.convert(fluent.atom, problem)
 
             args.extend([self.convert(m, problem) for m in msg.list])
             if payload is not None:
-                return problem.env.expression_manager.FluentExp(payload, tuple(args))
+                return problem.environment.expression_manager.FluentExp(
+                    payload, tuple(args)
+                )
             else:
                 raise UPException(f"Unable to form fluent expression {msg}")
         elif (
             msg.kind == proto.ExpressionKind.Value("FUNCTION_APPLICATION")
             and msg.type != "up:time"
         ):
             node_type = None
@@ -174,101 +184,124 @@
                     [self.convert(var, problem).variable() for var in variables]
                 )
             else:
                 args.extend([self.convert(m, problem) for m in msg.list])
 
             assert node_type is not None
 
-            return problem.env.expression_manager.create_node(
+            return problem.environment.expression_manager.create_node(
                 node_type=node_type,
                 args=tuple(args),
                 payload=payload,
             )
         elif (
             msg.kind == proto.ExpressionKind.Value("FUNCTION_APPLICATION")
             and msg.type == "up:time"
         ):
-            fn = msg.list[0].atom.symbol
+            if (
+                len(msg.list) == 3
+            ):  # Expect something of the form (up:plus (QUALIFIER [CONTAINER]) DELAY)
+                assert (
+                    msg.list[0].atom.symbol == "up:plus"
+                ), f"Unexpected expression {msg.list[0].atom.symbol}"
+                if msg.list[2].type == "up:integer":
+                    dl = int(msg.list[2].atom.int)
+                elif msg.list[2].type == "up:real":
+                    dl = self.convert(msg.list[2].atom.real)
+                else:
+                    raise ValueError(f"Invalid delay type {msg.list[2].type}")
+                timepoint_expr = msg.list[1].list
+            else:  # Expects a single timepoint of the form (QUALIFIER [CONTAINER])
+                dl = 0
+                timepoint_expr = msg.list
+
+            fn = timepoint_expr[0].atom.symbol
             if fn == "up:start":
                 kd = model.TimepointKind.START
             elif fn == "up:end":
                 kd = model.TimepointKind.END
             elif fn == "up:global_start":
                 kd = model.TimepointKind.GLOBAL_START
             elif fn == "up:global_end":
                 kd = model.TimepointKind.GLOBAL_END
             else:
                 raise ValueError(f"Invalid temporal qualifier {fn}")
             container = None
-            if len(msg.list) > 1:
-                container = msg.list[1].atom.symbol
+            if len(timepoint_expr) > 1:
+                container = timepoint_expr[1].atom.symbol
             tp = model.timing.Timepoint(kd, container)
-            return problem.env.expression_manager.TimingExp(model.Timing(0, tp))
+            return problem.environment.expression_manager.TimingExp(
+                model.Timing(dl, tp)
+            )
 
         raise ValueError(f"Unknown expression kind `{msg.kind}`")
 
     @handles(proto.Atom)
     def _convert_atom(
         self, msg: proto.Atom, problem: Problem
     ) -> Union[model.FNode, model.Fluent, model.Object]:
         field = msg.WhichOneof("content")
 
         value = getattr(msg, field)
         if field == "int":
-            return problem.env.expression_manager.Int(value)
+            return problem.environment.expression_manager.Int(value)
         elif field == "real":
-            return problem.env.expression_manager.Real(
+            return problem.environment.expression_manager.Real(
                 fractions.Fraction(value.numerator, value.denominator)
             )
         elif field == "boolean":
-            return problem.env.expression_manager.Bool(value)
+            return problem.environment.expression_manager.Bool(value)
         else:
             # If atom symbols, return the equivalent UP alternative
             # Note that parameters are directly handled at expression level
             if problem.has_object(value):
-                return problem.env.expression_manager.ObjectExp(
+                return problem.environment.expression_manager.ObjectExp(
                     obj=problem.object(value)
                 )
             else:
                 return problem.fluent(value)
 
     @handles(proto.TypeDeclaration)
     def _convert_type_declaration(
         self, msg: proto.TypeDeclaration, problem: Problem
     ) -> model.Type:
         if msg.type_name == "up:bool":
-            return problem.env.type_manager.BoolType()
+            return problem.environment.type_manager.BoolType()
         elif msg.type_name.startswith("up:integer["):
             tmp = msg.type_name.split("[")[1].split("]")[0].split(", ")
-            return problem.env.type_manager.IntType(
+            return problem.environment.type_manager.IntType(
                 lower_bound=int(tmp[0]) if tmp[0] != "-inf" else None,
                 upper_bound=int(tmp[1]) if tmp[1] != "inf" else None,
             )
         elif msg.type_name.startswith("up:real["):
             tmp = msg.type_name.split("[")[1].split("]")[0].split(", ")
             lower_bound = fractions.Fraction(tmp[0]) if tmp[0] != "-inf" else None
             upper_bound = fractions.Fraction(tmp[1]) if tmp[1] != "inf" else None
-            return problem.env.type_manager.RealType(
+            return problem.environment.type_manager.RealType(
                 lower_bound=lower_bound, upper_bound=upper_bound
             )
         else:
             father = (
                 problem.user_type(msg.parent_type) if msg.parent_type != "" else None
             )
-            return problem.env.type_manager.UserType(name=msg.type_name, father=father)
+            return problem.environment.type_manager.UserType(
+                name=msg.type_name, father=father
+            )
 
     @handles(proto.Problem)
     def _convert_problem(
-        self, msg: proto.Problem, env: Optional[Environment] = None
+        self, msg: proto.Problem, environment: Optional[Environment] = None
     ) -> Problem:
         problem_name = str(msg.problem_name) if str(msg.problem_name) != "" else None
         if msg.HasField("hierarchy"):
-            problem = model.htn.HierarchicalProblem(name=problem_name, env=env)
+            problem = model.htn.HierarchicalProblem(
+                name=problem_name, environment=environment
+            )
         else:
-            problem = Problem(name=problem_name, env=env)
+            problem = Problem(name=problem_name, environment=environment)
 
         for t in msg.types:
             problem._add_user_type(self.convert(t, problem))
         for obj in msg.objects:
             problem.add_object(self.convert(obj, problem))
         for f in msg.fluents:
             problem.add_fluent(
@@ -318,38 +351,42 @@
         return problem
 
     @handles(proto.AbstractTaskDeclaration)
     def _convert_abstract_task(
         self, msg: proto.AbstractTaskDeclaration, problem: Problem
     ):
         return model.htn.Task(
-            msg.name, [self.convert(p, problem) for p in msg.parameters], problem.env
+            msg.name,
+            [self.convert(p, problem) for p in msg.parameters],
+            problem.environment,
         )
 
     @handles(proto.Task)
     def _convert_task(
         self, msg: proto.Task, problem: model.htn.HierarchicalProblem
     ) -> model.htn.Subtask:
         if problem.has_task(msg.task_name):
             task = problem.get_task(msg.task_name)
         elif problem.has_action(msg.task_name):
             task = problem.action(msg.task_name)
         else:
             raise ValueError(f"Unknown task name: {msg.task_name}")
         parameters = [self.convert(p, problem) for p in msg.parameters]
-        return model.htn.Subtask(task, *parameters, ident=msg.id, _env=problem.env)
+        return model.htn.Subtask(
+            task, *parameters, ident=msg.id, _env=problem.environment
+        )
 
     @handles(proto.Method)
     def _convert_method(
         self, msg: proto.Method, problem: model.htn.HierarchicalProblem
     ) -> model.htn.Method:
         method = model.htn.Method(
             msg.name,
             [self.convert(p, problem) for p in msg.parameters],
-            problem.env,
+            problem.environment,
         )
         achieved_task_params = []
         for p in msg.achieved_task.parameters:
             achieved_task_params.append(method.parameter(p.atom.symbol))
         method.set_task(
             problem.get_task(msg.achieved_task.task_name), *achieved_task_params
         )
@@ -362,15 +399,15 @@
             method.add_precondition(self.convert(c.cond, problem))
         return method
 
     @handles(proto.TaskNetwork)
     def _convert_task_network(
         self, msg: proto.TaskNetwork, problem: model.htn.HierarchicalProblem
     ) -> model.htn.TaskNetwork:
-        tn = model.htn.TaskNetwork(problem.env)
+        tn = model.htn.TaskNetwork(problem.environment)
         for v in msg.variables:
             tn.add_variable(v.name, convert_type_str(v.type, problem))
         for st in msg.subtasks:
             tn.add_subtask(self.convert(st, problem))
         for c in msg.constraints:
             tn.add_constraint(self.convert(c, problem))
 
@@ -382,14 +419,15 @@
     ) -> Union[
         metrics.MinimizeActionCosts,
         metrics.MinimizeSequentialPlanLength,
         metrics.MinimizeMakespan,
         metrics.MinimizeExpressionOnFinalState,
         metrics.MaximizeExpressionOnFinalState,
         metrics.Oversubscription,
+        metrics.TemporalOversubscription,
     ]:
         if msg.kind == proto.Metric.MINIMIZE_ACTION_COSTS:
             costs = {}
             for a, cost in msg.action_costs.items():
                 costs[problem.action(a)] = self.convert(cost, problem)
             return metrics.MinimizeActionCosts(
                 costs=costs,
@@ -412,16 +450,23 @@
         elif msg.kind == proto.Metric.MAXIMIZE_EXPRESSION_ON_FINAL_STATE:
             return metrics.MaximizeExpressionOnFinalState(
                 expression=self.convert(msg.expression, problem)
             )
         elif msg.kind == proto.Metric.OVERSUBSCRIPTION:
             goals = {}
             for g in msg.goals:
-                goals[self.convert(g.goal, problem)] = self.convert(g.cost)
+                goals[self.convert(g.goal, problem)] = self.convert(g.weight)
             return metrics.Oversubscription(goals)
+        elif msg.kind == proto.Metric.TEMPORAL_OVERSUBSCRIPTION:
+            timed_goals = {}
+            for g in msg.timed_goals:
+                timed_goals[
+                    (self.convert(g.timing, problem), self.convert(g.goal, problem))
+                ] = self.convert(g.weight)
+            return metrics.TemporalOversubscription(timed_goals)
         else:
             raise UPException(f"Unknown metric kind `{msg.kind}`")
 
     @handles(proto.Action)
     def _convert_action(self, msg: proto.Action, problem: Problem) -> model.Action:
         action: model.Action
 
@@ -541,55 +586,91 @@
         container = msg.container_id if msg.container_id != "" else None
         return model.timing.Timepoint(kind, container)
 
     @handles(proto.Plan)
     def _convert_plan(
         self, msg: proto.Plan, problem: Problem
     ) -> unified_planning.plans.Plan:
-        actions = [self.convert(a, problem) for a in msg.actions]
-        if all(isinstance(a, tuple) for a in actions):
-            # If all actions are tuples, we can assume that they are
-            # (absolute start time, action, duration)
-            return unified_planning.plans.TimeTriggeredPlan(actions)
+        actions = [self._convert_action_instance(a, problem) for a in msg.actions]
+        if all(a[2] is not None for a in actions):
+            # If all actions have temporal term, we can assume that they are
+            # (id, action, (absolute start time, duration))
+            time_triggered_actions = [
+                (start, action, duration) for _, action, (start, duration) in actions
+            ]
+            flat_plan = unified_planning.plans.TimeTriggeredPlan(time_triggered_actions)
+        else:
+            # Otherwise, we assume they are a sequence of actions (id, action, None)
+            action_sequence = [action for _, action, _ in actions]
+            flat_plan = unified_planning.plans.SequentialPlan(actions=action_sequence)
+
+        if msg.HasField("hierarchy"):
+            assert isinstance(problem, HierarchicalProblem)
+            # map each action/method ID with the correcponding instance
+            instances = {id: action for id, action, _ in actions}
+
+            # return the Action/Method with the given id
+            # this recursively build any needed instance.
+            def instance_with_id(id: str) -> Union[ActionInstance, MethodInstance]:
+                if id not in instances:
+                    proto_method = next(
+                        filter(lambda m: m.id == id, msg.hierarchy.methods)
+                    )
+                    method = problem.method(proto_method.method_name)
+                    parameters = tuple(
+                        [
+                            self._convert_atom(param, problem)
+                            for param in proto_method.parameters
+                        ]
+                    )
+                    subtasks = {
+                        id: instance_with_id(impl)
+                        for id, impl in proto_method.subtasks.items()
+                    }
+                    instance = MethodInstance(
+                        method, parameters, Decomposition(subtasks)
+                    )
+                    instances[id] = instance
+                return instances[id]
+
+            decomposition = Decomposition(
+                {
+                    id: instance_with_id(impl)
+                    for id, impl in msg.hierarchy.root_tasks.items()
+                }
+            )
+
+            return unified_planning.plans.HierarchicalPlan(flat_plan, decomposition)
+
         else:
-            # Otherwise, we assume they are instantenous actions
-            return unified_planning.plans.SequentialPlan(actions=actions)
+            return flat_plan
 
     @handles(proto.ActionInstance)
     def _convert_action_instance(
         self, msg: proto.ActionInstance, problem: Problem
-    ) -> Union[
-        Tuple[
-            model.timing.Timing,
-            unified_planning.plans.ActionInstance,
-            model.timing.Duration,
-        ],
-        unified_planning.plans.ActionInstance,
+    ) -> Tuple[
+        str, ActionInstance, Optional[Tuple[model.Timing, model.timing.Duration]]
     ]:
         # action instance parameters are atoms but in UP they are FNodes
         # converting to up.model.FNode
         parameters = tuple([self.convert(param, problem) for param in msg.parameters])
 
+        id = msg.id
         action_instance = unified_planning.plans.ActionInstance(
             problem.action(msg.action_name),
             parameters,
         )
 
-        start_time = (
-            self.convert(msg.start_time) if msg.HasField("start_time") else None
-        )
-        end_time = self.convert(msg.end_time) if msg.HasField("end_time") else None
-        if start_time is not None:
-            return (
-                start_time,  # Absolute Start Time
-                action_instance,
-                end_time - start_time if end_time else None,  # Duration
-            )
+        if msg.HasField("start_time") and msg.HasField("end_time"):
+            start_time = self.convert(msg.start_time)
+            end_time = self.convert(msg.end_time)
+            duration = end_time - start_time
+            return id, action_instance, (start_time, duration)
         else:
-            return action_instance
+            return id, action_instance, None
 
     @handles(proto.PlanGenerationResult)
     def _convert_plan_generation_result(
         self, result: proto.PlanGenerationResult, problem: Problem
     ) -> unified_planning.engines.PlanGenerationResult:
         if result.status == proto.PlanGenerationResult.Status.Value(
             "SOLVED_SATISFICING"
@@ -643,15 +724,17 @@
             metrics = dict(result.metrics)
 
         if len(result.log_messages) > 0:
             log_messages = [self.convert(log) for log in result.log_messages]
 
         return unified_planning.engines.PlanGenerationResult(
             status=status,
-            plan=self.convert(result.plan, problem),
+            plan=self.convert(result.plan, problem)
+            if result.HasField("plan")
+            else None,
             engine_name=result.engine.name,
             metrics=metrics,
             log_messages=log_messages,
         )
 
     @handles(proto.LogMessage)
     def _convert_log_message(
@@ -682,23 +765,23 @@
 
     @handles(proto.CompilerResult)
     def _convert_compiler_result(
         self,
         result: proto.CompilerResult,
         lifted_problem: unified_planning.model.Problem,
     ) -> unified_planning.engines.CompilerResult:
-        problem = self.convert(result.problem, lifted_problem.env)
+        problem = self.convert(result.problem, lifted_problem.environment)
         map: Dict[
             unified_planning.model.Action,
             Tuple[unified_planning.model.Action, List[unified_planning.model.FNode]],
         ] = {}
         for grounded_action in problem.actions:
             original_action_instance = self.convert(
                 result.map_back_plan[grounded_action.name], lifted_problem
-            )
+            )[1]
             map[grounded_action] = (
                 original_action_instance.action,
                 original_action_instance.actual_parameters,
             )
         return unified_planning.engines.CompilerResult(
             problem=problem,
             map_back_action_instance=partial(
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/grpc/proto_writer.py` & `unified_planning-0.6.0/unified_planning/grpc/proto_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # type: ignore
 import fractions
 from itertools import product
-from typing import List
+from typing import List, Union
 
 import unified_planning.grpc.generated.unified_planning_pb2 as proto
 from unified_planning import model
+import unified_planning.engines
 import unified_planning.model.htn
+import unified_planning.engines
+import unified_planning.plans
+from unified_planning.plans.hierarchical_plan import *
 import unified_planning.model.walkers as walkers
+import unified_planning.plans
 from unified_planning.model.types import domain_size, domain_item
 from unified_planning.exceptions import UPException
 from unified_planning.grpc.converter import Converter, handles
 from unified_planning.model.operators import (
     BOOL_OPERATORS,
     IRA_OPERATORS,
     RELATIONS,
@@ -72,14 +77,46 @@
         return "up:time"
     elif tpe.is_int_type() or tpe.is_real_type():
         return f"up:{tpe}"
     elif isinstance(tpe, model.types._UserType):
         return str(tpe.name)
 
 
+def int_expression(value: int) -> proto.Expression:
+    return proto.Expression(
+        atom=proto.Atom(int=value),
+        type="up:integer",
+        kind=proto.ExpressionKind.Value("CONSTANT"),
+    )
+
+
+def real_expression(value: fractions.Fraction) -> proto.Expression:
+    return proto.Expression(
+        atom=proto.Atom(
+            real=proto.Real(
+                numerator=value.numerator,
+                denominator=value.denominator,
+            )
+        ),
+        type="up:real",
+        kind=proto.ExpressionKind.Value("CONSTANT"),
+    )
+
+
+def num_expression(value: Union[int, fractions.Fraction]) -> proto.Expression:
+    if isinstance(value, int):
+        return int_expression(value)
+    elif isinstance(value, fractions.Fraction):
+        return real_expression(value)
+    else:
+        raise ValueError(
+            f"Cannot be converted into a numeric protobuf expression: {value}"
+        )
+
+
 class FNode2Protobuf(walkers.DagWalker):
     def __init__(self, protobuf_writer):
         super().__init__()
         self._protobuf_writer = protobuf_writer
 
     def convert(self, expression: model.FNode) -> proto.Expression:
         return self.walk(expression)
@@ -93,32 +130,20 @@
             kind=proto.ExpressionKind.Value("CONSTANT"),
             type="up:bool",
         )
 
     def walk_int_constant(
         self, expression: model.FNode, args: List[proto.Expression]
     ) -> proto.Expression:
-        return proto.Expression(
-            atom=proto.Atom(int=expression.int_constant_value()),
-            list=[],
-            kind=proto.ExpressionKind.Value("CONSTANT"),
-            type="up:integer",
-        )
+        return int_expression(expression.int_constant_value())
 
     def walk_real_constant(
         self, expression: model.FNode, args: List[proto.Expression]
     ) -> proto.Expression:
-        return proto.Expression(
-            atom=proto.Atom(
-                real=self._protobuf_writer.convert(expression.real_constant_value())
-            ),
-            list=[],
-            kind=proto.ExpressionKind.Value("CONSTANT"),
-            type="up:real",
-        )
+        return real_expression(expression.real_constant_value())
 
     def walk_param_exp(
         self, expression: model.FNode, args: List[proto.Expression]
     ) -> proto.Expression:
         return proto.Expression(
             atom=proto.Atom(symbol=expression.parameter().name),
             list=[],
@@ -176,16 +201,30 @@
             kind=proto.ExpressionKind.Value("FUNCTION_SYMBOL"),
         )
         tp_exp = proto.Expression(
             list=[fn_exp] + args,
             type="up:time",
             kind=proto.ExpressionKind.Value("FUNCTION_APPLICATION"),
         )
-        assert timing.delay == 0
-        return tp_exp
+        if timing.delay == 0:
+            # no delay for this timing, the expression will somthing of the form (QUALIFIER [CONTAINER])
+            return tp_exp
+
+        else:
+            # we have a delay, build an expression of the form (up:plus (QUALIFIER [CONTAINER]) DELAY)
+            add_exp = proto.Expression(
+                atom=proto.Atom(symbol=map_operator(OperatorKind.PLUS)),
+                kind=proto.ExpressionKind.Value("FUNCTION_SYMBOL"),
+            )
+            dl_exp = num_expression(timing.delay)
+            return proto.Expression(
+                list=[add_exp, tp_exp, dl_exp],
+                type="up:time",
+                kind=proto.ExpressionKind.Value("FUNCTION_APPLICATION"),
+            )
 
     def walk_fluent_exp(
         self, expression: model.FNode, args: List[proto.Expression]
     ) -> proto.Expression:
         sub_list = []
         sub_list.append(
             proto.Expression(
@@ -485,15 +524,15 @@
             abstract_tasks=[self.convert(t) for t in problem.tasks],
             methods=[self.convert(m) for m in problem.methods],
         )
 
     @handles(model.Problem, model.htn.HierarchicalProblem)
     def _convert_problem(self, problem: model.Problem) -> proto.Problem:
         goals = [proto.Goal(goal=self.convert(g)) for g in problem.goals]
-        for (t, gs) in problem.timed_goals:
+        for t, gs in problem.timed_goals:
             goals += [
                 proto.Goal(goal=self.convert(g), timing=self.convert(t)) for g in gs
             ]
 
         problem_name = str(problem.name) if problem.name is not None else ""
         hierarchy = None
         if isinstance(problem, model.htn.HierarchicalProblem):
@@ -566,23 +605,41 @@
     @handles(model.metrics.Oversubscription)
     def _convert_oversubscription_metric(
         self, metric: model.metrics.Oversubscription
     ) -> proto.Metric:
         goals = []
         for g, c in metric.goals.items():
             goals.append(
-                proto.GoalWithCost(
-                    goal=self.convert(g), cost=self.convert(fractions.Fraction(c))
+                proto.GoalWithWeight(
+                    goal=self.convert(g), weight=self.convert(fractions.Fraction(c))
                 )
             )
         return proto.Metric(
             kind=proto.Metric.OVERSUBSCRIPTION,
             goals=goals,
         )
 
+    @handles(model.metrics.TemporalOversubscription)
+    def _convert_temporal_oversubscription_metric(
+        self, metric: model.metrics.TemporalOversubscription
+    ) -> proto.Metric:
+        timed_goals = []
+        for (i, g), c in metric.goals.items():
+            timed_goals.append(
+                proto.TimedGoalWithWeight(
+                    timing=self.convert(i),
+                    goal=self.convert(g),
+                    weight=self.convert(fractions.Fraction(c)),
+                )
+            )
+        return proto.Metric(
+            kind=proto.Metric.TEMPORAL_OVERSUBSCRIPTION,
+            timed_goals=timed_goals,
+        )
+
     @handles(model.Parameter)
     def _convert_action_parameter(self, p: model.Parameter) -> proto.Parameter:
         return proto.Parameter(name=p.name, type=proto_type(p.type))
 
     @handles(model.Variable)
     def _convert_expression_variable(
         self, variable: model.Variable
@@ -593,54 +650,103 @@
             list=[],
             kind=proto.ExpressionKind.Value("VARIABLE"),
             type=proto_type(variable.type),
         )
 
     @handles(unified_planning.plans.ActionInstance)
     def _convert_action_instance(
-        self, a: unified_planning.plans.ActionInstance, start_time=None, end_time=None
+        self,
+        a: unified_planning.plans.ActionInstance,
+        start_time=None,
+        end_time=None,
+        id=None,
     ) -> proto.ActionInstance:
-        parameters = []
-        for param in a.actual_parameters:
-            # The parameters are atoms
-            parameters.append(self.convert(param).atom)
+        parameters = [self.convert(param).atom for param in a.actual_parameters]
 
         return proto.ActionInstance(
+            id=id,
             action_name=a.action.name,
             parameters=parameters,
             start_time=start_time,
             end_time=end_time,
         )
 
     @handles(str)
     def _convert_str_atom(self, s: str) -> proto.Atom:
         return proto.Atom(symbol=s)
 
     @handles(unified_planning.plans.SequentialPlan)
     def _convert_sequential_plan(
-        self, plan: unified_planning.plans.SequentialPlan
+        self,
+        plan: unified_planning.plans.SequentialPlan,
+        ids: Dict[ActionInstance, str] = None,
     ) -> proto.Plan:
-        return proto.Plan(actions=[self.convert(a) for a in plan.actions])
+        def id(a: ActionInstance):
+            return ids.get(a) if ids is not None else None
+
+        return proto.Plan(
+            actions=[self._convert_action_instance(a, id=id(a)) for a in plan.actions]
+        )
 
     @handles(unified_planning.plans.TimeTriggeredPlan)
     def _convert_time_triggered_plan(
-        self, plan: unified_planning.plans.TimeTriggeredPlan
+        self,
+        plan: unified_planning.plans.TimeTriggeredPlan,
+        ids: Dict[ActionInstance, str] = None,
     ) -> proto.Plan:
         action_instances = []
 
         for a in plan.timed_actions:
+            id = ids.get(a[1]) if ids else None
             start_time = self.convert(a[0])
             end_time = self.convert(a[0] + a[2])
             instance = self._convert_action_instance(
-                a[1], start_time=start_time, end_time=end_time
+                a[1], start_time=start_time, end_time=end_time, id=id
             )
             action_instances.append(instance)
 
         return proto.Plan(actions=action_instances)
 
+    @handles(unified_planning.plans.HierarchicalPlan)
+    def _convert_hierarchical_plan(
+        self, plan: unified_planning.plans.HierarchicalPlan
+    ) -> proto.Plan:
+        ids = {act: id for id, act in plan.actions()}
+        flat_plan: proto.Plan = self.convert(plan.action_plan, ids)
+
+        def get_subtasks(prefix: str, d: Decomposition) -> Dict[str, str]:
+            mapping = {}
+            for task_id in d.subtasks:
+                instance = d.subtasks[task_id]
+                if isinstance(instance, MethodInstance):
+                    mapping[task_id] = f"{prefix}{task_id}::{instance.method.name}"
+                else:
+                    assert isinstance(instance, ActionInstance)
+                    mapping[task_id] = f"{prefix}{task_id}"
+            return mapping
+
+        methods = []
+        for id, method in plan.methods():
+            parameters = [self.convert(param).atom for param in method.parameters]
+            subtasks = get_subtasks(id + "::", method.decomposition)
+            m = proto.MethodInstance(
+                id=id,
+                method_name=method.method.name,
+                parameters=parameters,
+                subtasks=subtasks,
+            )
+            methods.append(m)
+        root_tasks = get_subtasks("", plan.decomposition)
+
+        plan = proto.Plan(
+            actions=flat_plan.actions,
+            hierarchy=proto.PlanHierarchy(root_tasks=root_tasks, methods=methods),
+        )
+        return plan
+
     @handles(unified_planning.engines.PlanGenerationResult)
     def _convert_plan_generation_result(
         self, result: unified_planning.engines.PlanGenerationResult
     ) -> proto.PlanGenerationResult:
         log_messages = None
         if result.log_messages is not None:
             log_messages = [self.convert(log) for log in result.log_messages]
@@ -686,15 +792,14 @@
             status == unified_planning.engines.PlanGenerationResultStatus.INTERNAL_ERROR
         ):
             return proto.PlanGenerationResult.Status.Value("INTERNAL_ERROR")
         elif (
             status
             == unified_planning.engines.PlanGenerationResultStatus.UNSUPPORTED_PROBLEM
         ):
-
             return proto.PlanGenerationResult.Status.Value("UNSUPPORTED_PROBLEM")
         elif status == unified_planning.engines.PlanGenerationResultStatus.INTERMEDIATE:
             return proto.PlanGenerationResult.Status.Value("INTERMEDIATE")
         else:
             raise ValueError("Unknown status: {}".format(status))
 
     @handles(unified_planning.engines.LogMessage)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/interop/__init__.py` & `unified_planning-0.6.0/unified_planning/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/interop/from_tarski.py` & `unified_planning-0.6.0/unified_planning/interop/from_tarski.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,45 +31,56 @@
 )
 from tarski.syntax.terms import Term, CompoundTerm, BuiltinPredicateSymbol
 from tarski.syntax.terms import Constant, Variable, BuiltinFunctionSymbol
 from tarski.fstrips.fstrips import AddEffect, DelEffect, FunctionalEffect
 
 
 def convert_tarski_formula(
-    env: Environment,
+    environment: Environment,
     fluents: Dict[str, "unified_planning.model.Fluent"],
     objects: Dict[str, "unified_planning.model.Object"],
     action_parameters: Dict[str, "unified_planning.model.Parameter"],
     types: Dict[str, Optional["unified_planning.model.Type"]],
     formula: Union[Formula, Term],
 ) -> "unified_planning.model.FNode":
     """Converts a tarski formula in a unified_planning expression."""
-    em = env.expression_manager
+    em = environment.expression_manager
     if is_and(formula):
         children = [
-            convert_tarski_formula(env, fluents, objects, action_parameters, types, f)
+            convert_tarski_formula(
+                environment, fluents, objects, action_parameters, types, f
+            )
             for f in formula.subformulas
         ]
         return em.And(*children)
     elif is_or(formula):
         children = [
-            convert_tarski_formula(env, fluents, objects, action_parameters, types, f)
+            convert_tarski_formula(
+                environment, fluents, objects, action_parameters, types, f
+            )
             for f in formula.subformulas
         ]
         return em.Or(*children)
     elif is_neg(formula):
         assert len(formula.subformulas) == 1
         return em.Not(
             convert_tarski_formula(
-                env, fluents, objects, action_parameters, types, formula.subformulas[0]
+                environment,
+                fluents,
+                objects,
+                action_parameters,
+                types,
+                formula.subformulas[0],
             )
         )
     elif is_atom(formula) or isinstance(formula, CompoundTerm):
         children = [
-            convert_tarski_formula(env, fluents, objects, action_parameters, types, f)
+            convert_tarski_formula(
+                environment, fluents, objects, action_parameters, types, f
+            )
             for f in formula.subterms
         ]
         if is_atom(formula):
             symbol = formula.predicate.symbol
         else:
             symbol = formula.symbol.name
         if symbol == BuiltinPredicateSymbol.EQ:
@@ -132,34 +143,37 @@
         else:
             return em.VariableExp(
                 unified_planning.model.Variable(
                     formula.symbol,
                     cast(
                         unified_planning.model.Type,
                         _convert_type_and_update_dict(
-                            formula.sort, types, env.type_manager, formula.sort.language
+                            formula.sort,
+                            types,
+                            environment.type_manager,
+                            formula.sort.language,
                         ),
                     ),
-                    env,
+                    environment,
                 )
             )
     elif isinstance(formula, QuantifiedFormula):
         expression = convert_tarski_formula(
-            env, fluents, objects, action_parameters, types, formula.formula
+            environment, fluents, objects, action_parameters, types, formula.formula
         )
         variables = [
             unified_planning.model.Variable(
                 v.symbol,
                 cast(
                     unified_planning.model.Type,
                     _convert_type_and_update_dict(
-                        v.sort, types, env.type_manager, v.sort.language
+                        v.sort, types, environment.type_manager, v.sort.language
                     ),
                 ),
-                env,
+                environment,
             )
             for v in formula.variables
         ]
         if formula.quantifier == Quantifier.Exists:
             return em.Exists(expression, *variables)
         elif formula.quantifier == Quantifier.Forall:
             return em.Forall(expression, *variables)
@@ -202,15 +216,15 @@
                 return True
     return False
 
 
 def _convert_type_and_update_dict(
     sort: tarski.syntax.Sort,
     types_dict: Dict[str, Optional["unified_planning.model.Type"]],
-    tm: "unified_planning.model.TypeManager",
+    tm: "unified_planning.model.type_manager.TypeManager",
     lang: "tarski.fol.FirstOrderLanguage",
 ) -> Optional["unified_planning.model.Type"]:
     """Converts a tarski type in a unified_planning type and inserts it into the types_dict.
     Important NOTE: This function modifies the parameter types_dict."""
     if str(sort.name) in types_dict:  # type already defined
         return types_dict[str(sort.name)]
     if isinstance(sort, Interval):  # if the type is an Interval
@@ -238,25 +252,25 @@
         up_type = tm.UserType(str(sort.name), up_father)
     assert up_type is not None  # sanity check
     types_dict[str(sort.name)] = up_type
     return up_type
 
 
 def convert_problem_from_tarski(
-    env: Environment, tarski_problem: tarski.fstrips.Problem
+    environment: Environment, tarski_problem: tarski.fstrips.Problem
 ) -> "unified_planning.model.Problem":
     """
     Converts a tarski problem in a `Problem`.
 
-    :param env: The unified_planning `Environment`.
+    :param environment: The unified_planning `Environment`.
     :param tarski_problem: The tarski problem to convert.
     :return: The generated `Problem`.
     """
-    em = env.expression_manager
-    tm = env.type_manager
+    em = environment.expression_manager
+    tm = environment.type_manager
     lang = tarski_problem.language
     problem = unified_planning.model.Problem(tarski_problem.name)
 
     # Convert types
     types: Dict[str, Optional["unified_planning.model.Type"]] = {}
     uses_object_type: bool = _check_if_tarski_problem_uses_object_type(tarski_problem)
     if not uses_object_type:
@@ -334,15 +348,15 @@
         problem.add_fluent(fluent)
 
     # Convert objects
     objects = {}
     for c in lang.constants():
         type = types[str(c.sort.name)]
         assert type is not None
-        o = unified_planning.model.Object(str(c.name), type, env)
+        o = unified_planning.model.Object(str(c.name), type, environment)
         objects[o.name] = o
         problem.add_object(o)
 
     # Convert actions
     for a_name in tarski_problem.actions:
         a = tarski_problem.get_action(a_name)
         parameters: OrderedDict[str, "unified_planning.model.Type"] = OrderedDict()
@@ -351,37 +365,37 @@
             assert type is not None
             parameters[p.symbol] = type
         action = unified_planning.model.InstantaneousAction(a_name, parameters)
         action_parameters = {}
         for p in parameters.keys():
             action_parameters[p] = action.parameter(p)
         f = convert_tarski_formula(
-            env, fluents, objects, action_parameters, types, a.precondition
+            environment, fluents, objects, action_parameters, types, a.precondition
         )
         action.add_precondition(f)
         for eff in a.effects:
             condition = convert_tarski_formula(
-                env, fluents, objects, action_parameters, types, eff.condition
+                environment, fluents, objects, action_parameters, types, eff.condition
             )
             if isinstance(eff, AddEffect):
                 f = convert_tarski_formula(
-                    env, fluents, objects, action_parameters, types, eff.atom
+                    environment, fluents, objects, action_parameters, types, eff.atom
                 )
                 action.add_effect(f, True, condition)
             elif isinstance(eff, DelEffect):
                 f = convert_tarski_formula(
-                    env, fluents, objects, action_parameters, types, eff.atom
+                    environment, fluents, objects, action_parameters, types, eff.atom
                 )
                 action.add_effect(f, False, condition)
             elif isinstance(eff, FunctionalEffect):
                 lhs = convert_tarski_formula(
-                    env, fluents, objects, action_parameters, types, eff.lhs
+                    environment, fluents, objects, action_parameters, types, eff.lhs
                 )
                 rhs = convert_tarski_formula(
-                    env, fluents, objects, action_parameters, types, eff.rhs
+                    environment, fluents, objects, action_parameters, types, eff.rhs
                 )
                 action.add_effect(lhs, rhs, condition)
             else:
                 raise UPProblemDefinitionError(eff + " not supported!")
         problem.add_action(action)
 
     # Set initial values
@@ -399,22 +413,24 @@
         if len(l) == 0:
             initial_values[em.FluentExp(fluent)] = default_value
         else:
             for args in itertools.product(*l):
                 initial_values[fluent(*args)] = default_value
     for i in tarski_problem.init.as_atoms():
         if isinstance(i, tuple):
-            lhs = convert_tarski_formula(env, fluents, objects, {}, types, i[0])
-            rhs = convert_tarski_formula(env, fluents, objects, {}, types, i[1])
+            lhs = convert_tarski_formula(environment, fluents, objects, {}, types, i[0])
+            rhs = convert_tarski_formula(environment, fluents, objects, {}, types, i[1])
             initial_values[lhs] = rhs
         else:
-            f = convert_tarski_formula(env, fluents, objects, {}, types, i)
+            f = convert_tarski_formula(environment, fluents, objects, {}, types, i)
             initial_values[f] = em.TRUE()
     for lhs, rhs in initial_values.items():
         problem.set_initial_value(lhs, rhs)
 
     # Convert goals
     problem.add_goal(
-        convert_tarski_formula(env, fluents, objects, {}, types, tarski_problem.goal)
+        convert_tarski_formula(
+            environment, fluents, objects, {}, types, tarski_problem.goal
+        )
     )
 
     return problem
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/interop/to_tarski.py` & `unified_planning-0.6.0/unified_planning/interop/to_tarski.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,23 @@
 )
 
 import tarski
 
 
 class TarskiFormulaConverter(walkers.DagWalker):
     def __init__(
-        self, language: "tarski.fol.FirstOrderLanguage", env, object_freshname: str
+        self,
+        language: "tarski.fol.FirstOrderLanguage",
+        environment,
+        object_freshname: str,
     ) -> None:
         walkers.DagWalker.__init__(self)
         self.object_freshname = object_freshname
         self.lang = language
-        self.env = env
+        self.environment = environment
 
     def convert_formula(
         self, expression: "unified_planning.model.FNode"
     ) -> "tarski.syntax.formulas.Formula":
         return self.walk(expression)
 
     def walk_and(
@@ -298,15 +301,15 @@
     `tarski.fstrips.Problem` representation.
 
     :param problem: The `Problem` to convert.
     :return: The generated `tarski.fstrips.Problem`.
     """
     features: List[str] = []
     kind = problem.kind
-    if kind.has_equality():
+    if kind.has_equalities():
         features.append("equality")
     if (
         kind.has_continuous_numbers()
         or kind.has_discrete_numbers()
         or kind.has_numeric_fluents()
     ):
         features.append("arithmetic")
@@ -356,17 +359,19 @@
             lang.get_sort(
                 cast(UT, o.type).name
                 if cast(UT, o.type).name != "object"
                 else object_freshname
             ),
         )
     # creating tarski problem
-    em = problem.env.expression_manager
+    em = problem.environment.expression_manager
     tfc = TarskiFormulaConverter(
-        language=lang, env=problem.env, object_freshname=object_freshname
+        language=lang,
+        environment=problem.environment,
+        object_freshname=object_freshname,
     )
     new_problem = tarski.fstrips.problem.create_fstrips_problem(
         lang, problem.name, f"{problem.name}_domain"
     )
     for action in problem.actions:
         if not isinstance(action, unified_planning.model.InstantaneousAction):
             raise unified_planning.exceptions.UPProblemDefinitionError(
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/io/anml_writer.py` & `unified_planning-0.6.0/unified_planning/io/anml_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,19 +108,19 @@
                 "up.model.Action",
                 "up.model.Parameter",
                 "up.model.Fluent",
                 "up.model.Object",
             ],
             str,
         ],
-        env: "up.environment.Environment",
+        environment: "up.environment.Environment",
     ):
         walkers.DagWalker.__init__(self)
         self._names_mapping = names_mapping
-        self.simplifier = env.simplifier
+        self.simplifier = environment.simplifier
 
     def convert(self, expression):
         """Converts the given expression to a ANML string."""
         return self.walk(
             self.simplifier.simplify(expression)
         )  # NOTE maybe the converter could remove the first and last char, if they are '(' and ')'
 
@@ -241,17 +241,18 @@
                 "up.model.Parameter",
                 "up.model.Fluent",
                 "up.model.Object",
             ],
             str,
         ] = {}
         # Init names_mapping.
-        names_mapping[self.problem.env.type_manager.BoolType()] = "boolean"
-        names_mapping[self.problem.env.type_manager.IntType()] = "integer"
-        names_mapping[self.problem.env.type_manager.RealType()] = "float"
+        env = self.problem.environment
+        names_mapping[env.type_manager.BoolType()] = "boolean"
+        names_mapping[env.type_manager.IntType()] = "integer"
+        names_mapping[env.type_manager.RealType()] = "float"
         for t in self.problem.user_types:
             ut = cast(_UserType, t)
             if _is_valid_anml_name(ut.name):  # No renaming needed
                 names_mapping[t] = ut.name
         for a in self.problem.actions:
             if _is_valid_anml_name(a.name):  # No renaming needed
                 names_mapping[a] = a.name
@@ -285,15 +286,15 @@
                     f"constant {_get_anml_name(f.type, names_mapping)} {_get_anml_name(f, names_mapping)}{params_written};\n"
                 )
             else:
                 out.write(
                     f"fluent {_get_anml_name(f.type, names_mapping)} {_get_anml_name(f, names_mapping)}{params_written};\n"
                 )
 
-        converter = ConverterToANMLString(names_mapping, self.problem.env)
+        converter = ConverterToANMLString(names_mapping, self.problem.environment)
 
         for a in self.problem.actions:
             if isinstance(a, up.model.InstantaneousAction):
                 parameters = [
                     f"{_get_anml_name(ap.type, names_mapping)} {_get_anml_name(ap, names_mapping)}"
                     for ap in a.parameters
                 ]
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/io/pddl_reader.py` & `unified_planning-0.6.0/unified_planning/io/pddl_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,76 +15,84 @@
 
 from itertools import product
 import unified_planning as up
 import unified_planning.model.htn as htn
 import unified_planning.model.walkers
 import typing
 from unified_planning.model import ContingentProblem
-from unified_planning.environment import Environment, get_env
+from unified_planning.environment import Environment, get_environment
 from unified_planning.exceptions import UPUsageError
+from unified_planning.io.utils import parse_string, set_results_name, Located
 from collections import OrderedDict
 from fractions import Fraction
 from typing import Dict, Union, Callable, List, cast
 
 import pyparsing
-
-assert (
-    pyparsing.__version__ >= "3.0.0"
-), f"unified_planning needs a pyparsing version >= 3. Current version detected: {pyparsing.__version__}, please update it."
+from pyparsing import ParseResults
+from pyparsing import CharsNotIn, Empty, col, lineno
 from pyparsing import Word, alphanums, alphas, ZeroOrMore, OneOrMore, Keyword
-from pyparsing import Suppress, Group, rest_of_line, Optional, Forward
-from pyparsing import CharsNotIn, Empty
-from pyparsing.results import ParseResults
-from pyparsing import one_of
-
-
-class CaseInsensitiveToken:
-    """A case-insensitive representation of a string."""
-
-    def __init__(self, name: Union[str, pyparsing.ParseResults]):
-        if isinstance(name, pyparsing.ParseResults):
-            name = name[0]
-        assert isinstance(name, str)
-        self._name = name
-        self._canonical = name.lower()
-
-    def __repr__(self):
-        return self._name
-
-    def __hash__(self):
-        return hash(self._canonical)
-
-    def __eq__(self, other):
-        if isinstance(other, str):
-            return other.lower() == self._canonical
-        elif isinstance(other, CaseInsensitiveToken):
-            return self._canonical == other._canonical
-        else:
-            return False
+from pyparsing import Suppress, Group, Optional, Forward
+
+if pyparsing.__version__ < "3.0.0":
+    from pyparsing import oneOf as one_of
+    from pyparsing import restOfLine as rest_of_line
+else:
+    from pyparsing import one_of
+    from pyparsing import rest_of_line
+
+
+class CustomParseResults:
+    def __init__(self, r):
+        self.res = r
+        self.value = r.value
+        self.locn_start = r.locn_start
+        self.locn_end = r.locn_end
+        if len(self.value) == 1 and isinstance(self.value[0], str):
+            self.value = self.value[0]
+
+    def __getitem__(self, i):
+        return CustomParseResults(self.value[i])
+
+    def __len__(self):
+        return len(self.value)
+
+    def line_start(self, complete_str: str) -> int:
+        return lineno(self.locn_start, complete_str)
+
+    def col_start(self, complete_str: str) -> int:
+        return col(self.locn_start, complete_str)
 
+    def line_end(self, complete_str: str) -> int:
+        return lineno(self.locn_end, complete_str)
 
-Object = CaseInsensitiveToken("object")
-TypesMap = Dict[CaseInsensitiveToken, unified_planning.model.Type]
+    def col_end(self, complete_str: str) -> int:
+        return col(self.locn_end, complete_str)
+
+
+Object = "object"
+TypesMap = Dict[str, unified_planning.model.Type]
 
 
 def nested_expr():
     """
     A hand-rolled alternative to pyparsing.nested_expr() that substantially improves its performance in our case.
     """
     cnt = Empty() + CharsNotIn("() \n\t\r")
     nested = Forward()
-    nested <<= Group(Suppress("(") + ZeroOrMore(cnt | nested) + Suppress(")"))
+    nested <<= Group(
+        Located(
+            Suppress("(") + ZeroOrMore(Group(Located(cnt)) | nested) + Suppress(")")
+        )
+    )
     return nested
 
 
 class PDDLGrammar:
     def __init__(self):
         name = Word(alphas, alphanums + "_" + "-")
-        # Parser for types that convert the string into a token that is case-insensitive
-        tpe = name.copy().add_parse_action(lambda t: CaseInsensitiveToken(t))
         variable = Suppress("?") + name
 
         require_def = (
             Suppress("(")
             + ":requirements"
             + OneOrMore(
                 one_of(
@@ -93,198 +101,220 @@
             )
             + Suppress(")")
         )
 
         types_def = (
             Suppress("(")
             + ":types"
-            - OneOrMore(
-                Group(Group(OneOrMore(tpe)) + Optional(Suppress("-") + tpe))
-            ).setResultsName("types")
+            - set_results_name(
+                OneOrMore(
+                    Group(Group(OneOrMore(name)) + Optional(Suppress("-") + name))
+                ),
+                "types",
+            )
             + Suppress(")")
         )
 
         constants_def = (
             Suppress("(")
             + ":constants"
-            - ZeroOrMore(
-                Group(Group(OneOrMore(name)) + Optional(Suppress("-") + tpe))
-            ).setResultsName("constants")
+            - set_results_name(
+                ZeroOrMore(
+                    Group(
+                        Located(Group(OneOrMore(name)) + Optional(Suppress("-") + name))
+                    )
+                ),
+                "constants",
+            )
             + Suppress(")")
         )
 
         predicate = (
             Suppress("(")
             + Group(
                 name
                 + Group(
                     ZeroOrMore(
                         Group(
-                            Group(OneOrMore(variable)) + Optional(Suppress("-") + tpe)
+                            Located(
+                                Group(OneOrMore(variable))
+                                + Optional(Suppress("-") + name)
+                            )
                         )
                     )
                 )
             )
             + Suppress(")")
         )
 
         predicates_def = (
             Suppress("(")
             + ":predicates"
-            - Group(OneOrMore(predicate)).setResultsName("predicates")
+            - set_results_name(Group(OneOrMore(predicate)), "predicates")
             + Suppress(")")
         )
 
         functions_def = (
             Suppress("(")
             + ":functions"
-            - Group(
-                OneOrMore(predicate + Optional(Suppress("- number")))
-            ).setResultsName("functions")
+            - set_results_name(
+                Group(OneOrMore(predicate + Optional(Suppress("- number")))),
+                "functions",
+            )
             + Suppress(")")
         )
 
-        parameters = ZeroOrMore(
-            Group(Group(OneOrMore(variable)) + Optional(Suppress("-") + tpe))
-        ).setResultsName("params")
+        parameters = set_results_name(
+            ZeroOrMore(
+                Group(
+                    Located(Group(OneOrMore(variable)) + Optional(Suppress("-") + name))
+                )
+            ),
+            "params",
+        )
         action_def = Group(
             Suppress("(")
             + ":action"
-            - name.setResultsName("name")
+            - set_results_name(name, "name")
             + ":parameters"
             - Suppress("(")
             + parameters
             + Suppress(")")
-            + Optional(":precondition" - nested_expr().setResultsName("pre"))
-            + Optional(":effect" - nested_expr().setResultsName("eff"))
-            + Optional(":observe" - nested_expr().setResultsName("obs"))
+            + Optional(":precondition" - set_results_name(nested_expr(), "pre"))
+            + Optional(":effect" - set_results_name(nested_expr(), "eff"))
+            + Optional(":observe" - set_results_name(nested_expr(), "obs"))
             + Suppress(")")
         )
 
         dur_action_def = Group(
             Suppress("(")
             + ":durative-action"
-            - name.setResultsName("name")
+            - set_results_name(name, "name")
             + ":parameters"
             - Suppress("(")
             + parameters
             + Suppress(")")
             + ":duration"
-            - nested_expr().setResultsName("duration")
+            - set_results_name(nested_expr(), "duration")
             + ":condition"
-            - nested_expr().setResultsName("cond")
+            - set_results_name(nested_expr(), "cond")
             + ":effect"
-            - nested_expr().setResultsName("eff")
+            - set_results_name(nested_expr(), "eff")
             + Suppress(")")
         )
 
         task_def = Group(
             Suppress("(")
             + ":task"
-            - name.setResultsName("name")
+            - set_results_name(name, "name")
             + ":parameters"
             - Suppress("(")
             + parameters
             + Suppress(")")
             + Suppress(")")
         )
 
         method_def = Group(
             Suppress("(")
             + ":method"
-            - name.setResultsName("name")
+            - set_results_name(name, "name")
             + ":parameters"
             - Suppress("(")
             + parameters
             + Suppress(")")
             + ":task"
-            - nested_expr().setResultsName("task")
-            + Optional(":precondition" - nested_expr().setResultsName("precondition"))
+            - set_results_name(nested_expr(), "task")
+            + Optional(
+                ":precondition" - set_results_name(nested_expr(), "precondition")
+            )
             + Optional(
                 one_of(":ordered-subtasks :ordered-tasks")
-                - nested_expr().setResultsName("ordered-subtasks")
+                - set_results_name(nested_expr(), "ordered-subtasks")
             )
             + Optional(
-                one_of(":subtasks :tasks") - nested_expr().setResultsName("subtasks")
+                one_of(":subtasks :tasks") - set_results_name(nested_expr(), "subtasks")
             )
-            + Optional(":ordering" - nested_expr().setResultsName("ordering"))
-            + Optional(":constraints" - nested_expr().setResultsName("constraints"))
+            + Optional(":ordering" - set_results_name(nested_expr(), "ordering"))
+            + Optional(":constraints" - set_results_name(nested_expr(), "constraints"))
             + Suppress(")")
         )
 
         domain = (
             Suppress("(")
             + "define"
             + Suppress("(")
             + "domain"
-            + name.setResultsName("name")
+            + set_results_name(name, "name")
             + Suppress(")")
-            + Optional(require_def).setResultsName("features")
+            + set_results_name(Optional(require_def), "features")
             + Optional(types_def)
             + Optional(constants_def)
             + Optional(predicates_def)
             + Optional(functions_def)
-            + Group(ZeroOrMore(task_def)).setResultsName("tasks")
-            + Group(ZeroOrMore(method_def)).setResultsName("methods")
-            + Group(ZeroOrMore(action_def | dur_action_def)).setResultsName("actions")
+            + set_results_name(Group(ZeroOrMore(task_def)), "tasks")
+            + set_results_name(Group(ZeroOrMore(method_def)), "methods")
+            + set_results_name(
+                Group(ZeroOrMore(action_def | dur_action_def)), "actions"
+            )
             + Suppress(")")
         )
 
-        objects = OneOrMore(
-            Group(Group(OneOrMore(name)) + Optional(Suppress("-") + tpe))
-        ).setResultsName("objects")
+        objects = set_results_name(
+            OneOrMore(Group(Group(OneOrMore(name)) + Optional(Suppress("-") + name))),
+            "objects",
+        )
 
         htn_def = Group(
             Suppress("(")
             + ":htn"
             - Optional(":parameters" - Suppress("(") + parameters + Suppress(")"))
             + Optional(
                 one_of(":ordered-tasks :ordered-subtasks")
-                - nested_expr().setResultsName("ordered-tasks")
+                - set_results_name(nested_expr(), "ordered-tasks")
             )
             + Optional(
-                one_of(":tasks :subtasks") - nested_expr().setResultsName("tasks")
+                one_of(":tasks :subtasks") - set_results_name(nested_expr(), "tasks")
             )
-            + Optional(":ordering" - nested_expr().setResultsName("ordering"))
-            + Optional(":constraints" - nested_expr().setResultsName("constraints"))
+            + Optional(":ordering" - set_results_name(nested_expr(), "ordering"))
+            + Optional(":constraints" - set_results_name(nested_expr(), "constraints"))
             + Suppress(")")
         )
 
-        metric = (Keyword("minimize") | Keyword("maximize")).setResultsName(
-            "optimization"
-        ) + (name | nested_expr()).setResultsName("metric")
+        metric = set_results_name(
+            (Keyword("minimize") | Keyword("maximize")), "optimization"
+        ) + set_results_name((name | nested_expr()), "metric")
 
         problem = (
             Suppress("(")
             + "define"
             + Suppress("(")
             + "problem"
-            + name.setResultsName("name")
+            + set_results_name(name, "name")
             + Suppress(")")
             + Suppress("(")
             + ":domain"
             + name
             + Suppress(")")
             + Optional(require_def)
             + Optional(Suppress("(") + ":objects" + objects + Suppress(")"))
-            + Optional(htn_def.setResultsName("htn"))
+            + Optional(set_results_name(htn_def, "htn"))
             + Suppress("(")
             + ":init"
-            + ZeroOrMore(nested_expr()).setResultsName("init")
+            + set_results_name(ZeroOrMore(nested_expr()), "init")
             + Suppress(")")
             + Optional(
                 Suppress("(")
                 + ":goal"
-                + nested_expr().setResultsName("goal")
+                + set_results_name(nested_expr(), "goal")
                 + Suppress(")")
             )
             + Optional(
                 Suppress("(")
                 + ":constraints"
-                + nested_expr().setResultsName("constraints")
+                + set_results_name(nested_expr(), "constraints")
                 + Suppress(")")
             )
             + Optional(Suppress("(") + ":metric" + metric + Suppress(")"))
             + Suppress(")")
         )
 
         domain.ignore(";" + rest_of_line)
@@ -306,18 +336,22 @@
     def parameters(self):
         return self._parameters
 
 
 class PDDLReader:
     """
     Parse a `PDDL` domain file and, optionally, a `PDDL` problem file and generate the equivalent :class:`~unified_planning.model.Problem`.
+
+    Note: in the error report messages, a tabulation counts as one column; and due to PDDL case-insensitivity, everything in the
+    PDDL files will be turned to lower case, so the names of fluents, actions etc. and the error report
+    will all be in lower-case.
     """
 
-    def __init__(self, env: typing.Optional[Environment] = None):
-        self._env = get_env(env)
+    def __init__(self, environment: typing.Optional[Environment] = None):
+        self._env = get_environment(environment)
         self._em = self._env.expression_manager
         self._tm = self._env.type_manager
         self._operators: Dict[str, Callable] = {
             "and": self._em.And,
             "or": self._em.Or,
             "not": self._em.Not,
             "imply": self._em.Implies,
@@ -347,363 +381,518 @@
 
     def _parse_exp(
         self,
         problem: up.model.Problem,
         act: typing.Optional[Union[up.model.Action, htn.Method, htn.TaskNetwork]],
         types_map: TypesMap,
         var: Dict[str, up.model.Variable],
-        exp: Union[ParseResults, str],
+        exp: CustomParseResults,
+        complete_str: str,
         assignments: Dict[str, "up.model.Object"] = {},
     ) -> up.model.FNode:
         stack = [(var, exp, False)]
         solved: List[up.model.FNode] = []
         while len(stack) > 0:
             var, exp, status = stack.pop()
             if status:
-                if exp[0] == "-" and len(exp) == 2:  # unary minus
+                if exp[0].value == "-" and len(exp) == 2:  # unary minus
                     solved.append(self._em.Times(-1, solved.pop()))
-                elif exp[0] in self._operators:  # n-ary operators
-                    op: Callable = self._operators[exp[0]]
-                    solved.append(op(*[solved.pop() for _ in exp[1:]]))
-                elif exp[0] in ["exists", "forall"]:  # quantifier operators
+                elif exp[0].value in self._operators:  # n-ary operators
+                    op: Callable = self._operators[exp[0].value]
+                    solved.append(op(*[solved.pop() for _ in range(1, len(exp))]))
+                elif exp[0].value in ["exists", "forall"]:  # quantifier operators
                     q_op: Callable = (
-                        self._em.Exists if exp[0] == "exists" else self._em.Forall
+                        self._em.Exists if exp[0].value == "exists" else self._em.Forall
                     )
                     solved.append(q_op(solved.pop(), *var.values()))
                 elif (
-                    exp[0] in self._trajectory_constraints
+                    exp[0].value in self._trajectory_constraints
                 ):  # trajectory_constraints reference
-                    t_op: Callable = self._trajectory_constraints[exp[0]]
-                    solved.append(t_op(*[solved.pop() for _ in exp[1:]]))
-                elif problem.has_fluent(exp[0]):  # fluent reference
-                    f = problem.fluent(exp[0])
-                    args = [solved.pop() for _ in exp[1:]]
-                    solved.append(self._em.FluentExp(f, tuple(args)))
-                elif exp[0] in assignments:  # quantified assignment variable
+                    t_op: Callable = self._trajectory_constraints[exp[0].value]
+                    solved.append(t_op(*[solved.pop() for _ in range(1, len(exp))]))
+                elif problem.has_fluent(exp[0].value):  # fluent reference
+                    f = problem.fluent(exp[0].value)
+                    args = [solved.pop() for _ in range(1, len(exp))]
+                    try:
+                        solved.append(self._em.FluentExp(f, tuple(args)))
+                    except Exception as e:
+                        start_line, start_col = exp.line_start(
+                            complete_str
+                        ), exp.col_start(complete_str)
+                        end_line, end_col = exp.line_end(complete_str), exp.col_end(
+                            complete_str
+                        )
+                        raise SyntaxError(
+                            repr(e)
+                            + f"\nError from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                        )
+                elif exp[0].value in assignments:  # quantified assignment variable
                     assert len(exp) == 1
-                    solved.append(self._em.ObjectExp(assignments[exp[0]]))
+                    solved.append(self._em.ObjectExp(assignments[exp[0].value]))
                 else:
-                    raise up.exceptions.UPUnreachableCodeError
+                    start_line, start_col = exp.line_start(complete_str), exp.col_start(
+                        complete_str
+                    )
+                    end_line, end_col = exp.line_end(complete_str), exp.col_end(
+                        complete_str
+                    )
+                    raise up.exceptions.UPUnreachableCodeError(
+                        f"Invalid expression from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                    )
             else:
-                if isinstance(exp, ParseResults):
+                if isinstance(exp.value, ParseResults):
                     if len(exp) == 0:  # empty precodition
                         solved.append(self._em.TRUE())
-                    elif exp[0] == "-" and len(exp) == 2:  # unary minus
+                    elif exp[0].value == "-" and len(exp) == 2:  # unary minus
                         stack.append((var, exp, True))
                         stack.append((var, exp[1], False))
-                    elif exp[0] in self._operators:  # n-ary operators
+                    elif exp[0].value in self._operators:  # n-ary operators
                         stack.append((var, exp, True))
-                        for e in exp[1:]:
-                            stack.append((var, e, False))
-                    elif exp[0] in ["exists", "forall"]:  # quantifier operators
-                        vars_string = " ".join(exp[1])
+                        for i in range(1, len(exp)):
+                            stack.append((var, exp[i], False))
+                    elif exp[0].value in ["exists", "forall"]:  # quantifier operators
+                        vars_string = " ".join([e.value for e in exp[1]])
                         vars_res = self._pp_parameters.parseString(vars_string)
                         new_vars = {}
                         for g in vars_res["params"]:
-                            t = types_map[g[1] if len(g) > 1 else Object]
-                            for o in g[0]:
+                            try:
+                                t = types_map[
+                                    g.value[1] if len(g.value) > 1 else Object
+                                ]
+                            except KeyError:
+                                g_start_line, g_start_col = lineno(
+                                    g.locn_start, complete_str
+                                ), col(g.locn_start, complete_str)
+                                g_end_line, g_end_col = lineno(
+                                    g.locn_end, complete_str
+                                ), col(g.locn_end, complete_str)
+                                raise SyntaxError(
+                                    f"Undefined variable's type: {g[1]}."
+                                    + f"\nError from line: {g_start_line}, col: {g_start_col} to line: {g_end_line}, col: {g_end_col}."
+                                )
+                            for o in g.value[0]:
                                 new_vars[o] = up.model.Variable(o, t, self._env)
                         # new_vars are the variables defined by the quantifier currently being solved
                         # all_vars are the variables defined by all the quantifiers around this expression
                         stack.append((new_vars, exp, True))
                         all_vars = var.copy()
                         all_vars.update(new_vars)
                         stack.append((all_vars, exp[2], False))
                     elif (
-                        exp[0] in self._trajectory_constraints
+                        exp[0].value in self._trajectory_constraints
                     ):  # trajectory_constraints reference
                         stack.append((var, exp, True))
-                        for e in exp[1:]:
-                            stack.append((var, e, False))
-                    elif problem.has_fluent(exp[0]):  # fluent reference
+                        for i in range(1, len(exp)):
+                            stack.append((var, exp[i], False))
+                    elif problem.has_fluent(exp[0].value):  # fluent reference
                         stack.append((var, exp, True))
-                        for e in exp[1:]:
-                            stack.append((var, e, False))
-                    elif exp[0] in assignments:  # quantified assignment variable
+                        for i in range(1, len(exp)):
+                            stack.append((var, exp[i], False))
+                    elif exp[0].value in assignments:  # quantified assignment variable
                         assert len(exp) == 1
                         stack.append((var, exp, True))
                     elif len(exp) == 1:  # expand an element inside brackets
                         stack.append((var, exp[0], False))
                     else:
-                        raise SyntaxError(f"Not able to handle: {exp}")
-                elif isinstance(exp, str):
+                        start_line, start_col = exp.line_start(
+                            complete_str
+                        ), exp.col_start(complete_str)
+                        end_line, end_col = exp.line_end(complete_str), exp.col_end(
+                            complete_str
+                        )
+                        raise SyntaxError(
+                            f"Not able to handle: {complete_str[exp.locn_start: exp.locn_end]} found at line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                        )
+                elif isinstance(exp.value, str):
                     if (
-                        exp[0] == "?" and exp[1:] in var
+                        exp.value[0] == "?" and exp.value[1:] in var
                     ):  # variable in a quantifier expression
-                        solved.append(self._em.VariableExp(var[exp[1:]]))
-                    elif exp in assignments:  # quantified assignment variable
-                        solved.append(self._em.ObjectExp(assignments[exp]))
-                    elif exp[0] == "?":  # action parameter
+                        solved.append(self._em.VariableExp(var[exp.value[1:]]))
+                    elif exp.value in assignments:  # quantified assignment variable
+                        solved.append(self._em.ObjectExp(assignments[exp.value]))
+                    elif exp.value[0] == "?":  # action parameter
                         assert act is not None
-                        solved.append(self._em.ParameterExp(act.parameter(exp[1:])))
-                    elif problem.has_fluent(exp):  # fluent
-                        solved.append(self._em.FluentExp(problem.fluent(exp)))
-                    elif problem.has_object(exp):  # object
-                        solved.append(self._em.ObjectExp(problem.object(exp)))
+                        try:
+                            solved.append(
+                                self._em.ParameterExp(act.parameter(exp.value[1:]))
+                            )
+                        except KeyError:
+                            start_line, start_col = exp.line_start(
+                                complete_str
+                            ), exp.col_start(complete_str)
+                            end_line, end_col = exp.line_end(complete_str), exp.col_end(
+                                complete_str
+                            )
+                            raise SyntaxError(
+                                f"Undefined name found: {exp.value[1:]}.\nError in expression from"
+                                + f" line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                            )
+                    elif problem.has_fluent(exp.value):  # fluent
+                        solved.append(self._em.FluentExp(problem.fluent(exp.value)))
+                    elif problem.has_object(exp.value):  # object
+                        solved.append(self._em.ObjectExp(problem.object(exp.value)))
                     else:  # number
-                        n = Fraction(exp)
+                        try:
+                            n = Fraction(exp.value)
+                        except ValueError:
+                            start_line, start_col = exp.line_start(
+                                complete_str
+                            ), exp.col_start(complete_str)
+                            end_line, end_col = exp.line_end(complete_str), exp.col_end(
+                                complete_str
+                            )
+                            raise SyntaxError(
+                                f"Found invalid expression: {complete_str[exp.locn_start:exp.locn_end]}. From line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                            )
                         if n.denominator == 1:
                             solved.append(self._em.Int(n.numerator))
                         else:
                             solved.append(self._em.Real(n))
                 else:
-                    raise SyntaxError(f"Not able to handle: {exp}")
+                    start_line, start_col = exp.line_start(complete_str), exp.col_start(
+                        complete_str
+                    )
+                    end_line, end_col = exp.line_end(complete_str), exp.col_end(
+                        complete_str
+                    )
+                    raise SyntaxError(
+                        f"Not able to handle: {exp}, from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                    )
         assert len(solved) == 1  # sanity check
         return solved.pop()
 
     def _add_effect(
         self,
         problem: up.model.Problem,
         act: Union[up.model.InstantaneousAction, up.model.DurativeAction],
         types_map: TypesMap,
         universal_assignments: typing.Optional[
-            Dict["up.model.Action", List[ParseResults]]
+            Dict["up.model.Action", List[CustomParseResults]]
         ],
-        exp: Union[ParseResults, str],
+        exp: CustomParseResults,
+        complete_str: str,
         cond: Union[up.model.FNode, bool] = True,
         timing: typing.Optional[up.model.Timing] = None,
         assignments: Dict[str, "up.model.Object"] = {},
     ):
         to_add = [(exp, cond)]
         while to_add:
             exp, cond = to_add.pop(0)
             if len(exp) == 0:
                 continue  # ignore the case where the effect list is empty, e.g., `:effect ()`
-            op = exp[0]
+            op = exp[0].value
             if op == "and":
-                exp = exp[1:]
-                for e in exp:
-                    to_add.append((e, cond))
+                for i in range(1, len(exp)):
+                    to_add.append((exp[i], cond))
             elif op == "when":
-                cond = self._parse_exp(problem, act, types_map, {}, exp[1], assignments)
-                to_add.append((exp[2], cond))
+                cond = self._parse_exp(
+                    problem, act, types_map, {}, exp[1], complete_str, assignments
+                )
+                cond = cond.simplify()
+                if not cond.is_false():
+                    to_add.append((exp[2], cond))
             elif op == "not":
                 exp = exp[1]
                 eff = (
-                    self._parse_exp(problem, act, types_map, {}, exp, assignments),
+                    self._parse_exp(
+                        problem, act, types_map, {}, exp, complete_str, assignments
+                    ),
                     self._em.FALSE(),
                     cond,
                 )
                 act.add_effect(*eff if timing is None else (timing, *eff))  # type: ignore
             elif op == "assign":
                 eff = (
-                    self._parse_exp(problem, act, types_map, {}, exp[1], assignments),
-                    self._parse_exp(problem, act, types_map, {}, exp[2], assignments),
+                    self._parse_exp(
+                        problem, act, types_map, {}, exp[1], complete_str, assignments
+                    ),
+                    self._parse_exp(
+                        problem, act, types_map, {}, exp[2], complete_str, assignments
+                    ),
                     cond,
                 )
                 act.add_effect(*eff if timing is None else (timing, *eff))  # type: ignore
             elif op == "increase":
                 eff = (
-                    self._parse_exp(problem, act, types_map, {}, exp[1], assignments),
-                    self._parse_exp(problem, act, types_map, {}, exp[2], assignments),
+                    self._parse_exp(
+                        problem, act, types_map, {}, exp[1], complete_str, assignments
+                    ),
+                    self._parse_exp(
+                        problem, act, types_map, {}, exp[2], complete_str, assignments
+                    ),
                     cond,
                 )
                 act.add_increase_effect(*eff if timing is None else (timing, *eff))  # type: ignore
             elif op == "decrease":
                 eff = (
-                    self._parse_exp(problem, act, types_map, {}, exp[1], assignments),
-                    self._parse_exp(problem, act, types_map, {}, exp[2], assignments),
+                    self._parse_exp(
+                        problem, act, types_map, {}, exp[1], complete_str, assignments
+                    ),
+                    self._parse_exp(
+                        problem, act, types_map, {}, exp[2], complete_str, assignments
+                    ),
                     cond,
                 )
                 act.add_decrease_effect(*eff if timing is None else (timing, *eff))  # type: ignore
             elif op == "forall":
-                assert isinstance(exp, ParseResults)
+                assert isinstance(exp, CustomParseResults)
                 # Get the list of universal_assignments linked to this action. If it does not exist, default it to the empty list
                 assert universal_assignments is not None
                 action_assignments = universal_assignments.setdefault(act, [])
                 action_assignments.append(exp)
             else:
                 eff = (
-                    self._parse_exp(problem, act, types_map, {}, exp, assignments),
+                    self._parse_exp(
+                        problem, act, types_map, {}, exp, complete_str, assignments
+                    ),
                     self._em.TRUE(),
                     cond,
                 )
                 act.add_effect(*eff if timing is None else (timing, *eff))  # type: ignore
 
     def _add_condition(
         self,
         problem: up.model.Problem,
         act: up.model.DurativeAction,
-        exp: Union[ParseResults, str],
+        exp: CustomParseResults,
         types_map: TypesMap,
+        complete_str: str,
         vars: typing.Optional[Dict[str, up.model.Variable]] = None,
     ):
         to_add = [(exp, vars)]
         while to_add:
             exp, vars = to_add.pop(0)
-            op = exp[0]
+            op = exp[0].value
             if op == "and":
-                for e in exp[1:]:
-                    to_add.append((e, vars))
+                for i in range(1, len(exp)):
+                    to_add.append((exp[i], vars))
             elif op == "forall":
-                vars_string = " ".join(exp[1])
+                vars_string = " ".join([e.value for e in exp[1]])
                 vars_res = self._pp_parameters.parseString(vars_string)
                 if vars is None:
                     vars = {}
                 for g in vars_res["params"]:
-                    t = types_map[g[1] if len(g) > 1 else Object]
-                    for o in g[0]:
+                    try:
+                        t = types_map[g.value[1] if len(g.value) > 1 else Object]
+                    except KeyError:
+                        g_start_line, g_start_col = lineno(
+                            g.locn_start, complete_str
+                        ), col(g.locn_start, complete_str)
+                        g_end_line, g_end_col = lineno(g.locn_end, complete_str), col(
+                            g.locn_end, complete_str
+                        )
+                        raise SyntaxError(
+                            f"Undefined variable's type: {g[1]}."
+                            + f"\nError from line: {g_start_line}, col: {g_start_col} to line: {g_end_line}, col: {g_end_col}."
+                        )
+                    for o in g.value[0]:
                         vars[o] = up.model.Variable(o, t, self._env)
                 to_add.append((exp[2], vars))
-            elif len(exp) == 3 and op == "at" and exp[1] == "start":
+            elif len(exp) == 3 and op == "at" and exp[1].value == "start":
                 cond = self._parse_exp(
-                    problem, act, types_map, {} if vars is None else vars, exp[2]
+                    problem,
+                    act,
+                    types_map,
+                    {} if vars is None else vars,
+                    exp[2],
+                    complete_str,
                 )
                 if vars is not None:
                     cond = self._em.Forall(cond, *vars.values())
                 act.add_condition(up.model.StartTiming(), cond)
-            elif len(exp) == 3 and op == "at" and exp[1] == "end":
+            elif len(exp) == 3 and op == "at" and exp[1].value == "end":
                 cond = self._parse_exp(
-                    problem, act, types_map, {} if vars is None else vars, exp[2]
+                    problem,
+                    act,
+                    types_map,
+                    {} if vars is None else vars,
+                    exp[2],
+                    complete_str,
                 )
                 if vars is not None:
                     cond = self._em.Forall(cond, *vars.values())
                 act.add_condition(up.model.EndTiming(), cond)
-            elif len(exp) == 3 and op == "over" and exp[1] == "all":
+            elif len(exp) == 3 and op == "over" and exp[1].value == "all":
                 t_all = up.model.OpenTimeInterval(
                     up.model.StartTiming(), up.model.EndTiming()
                 )
                 cond = self._parse_exp(
-                    problem, act, types_map, {} if vars is None else vars, exp[2]
+                    problem,
+                    act,
+                    types_map,
+                    {} if vars is None else vars,
+                    exp[2],
+                    complete_str,
                 )
                 if vars is not None:
                     cond = self._em.Forall(cond, *vars.values())
                 act.add_condition(t_all, cond)
             else:
-                raise SyntaxError(f"Not able to handle: {exp}")
+                start_line, start_col = exp.line_start(complete_str), exp.col_start(
+                    complete_str
+                )
+                end_line, end_col = exp.line_end(complete_str), exp.col_end(
+                    complete_str
+                )
+                raise SyntaxError(
+                    f"Not able to handle: {exp}, from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                )
 
     def _add_timed_effects(
         self,
         problem: up.model.Problem,
         act: up.model.DurativeAction,
         types_map: TypesMap,
         universal_assignments: typing.Optional[
-            Dict["up.model.Action", List[ParseResults]]
+            Dict["up.model.Action", List[CustomParseResults]]
         ],
-        eff: ParseResults,
+        eff: CustomParseResults,
+        complete_str: str,
         assignments: Dict[str, "up.model.Object"] = {},
     ):
         to_add = [eff]
         while to_add:
             eff = to_add.pop(0)
-            op = eff[0]
+            op = eff[0].value
             if op == "and":
-                for e in eff[1:]:
-                    to_add.append(e)
-            elif len(eff) == 3 and op == "at" and eff[1] == "start":
+                for i in range(1, len(eff)):
+                    to_add.append(eff[i])
+            elif len(eff) == 3 and op == "at" and eff[1].value == "start":
                 self._add_effect(
                     problem,
                     act,
                     types_map,
                     universal_assignments,
                     eff[2],
+                    complete_str,
                     timing=up.model.StartTiming(),
                     assignments=assignments,
                 )
-            elif len(eff) == 3 and op == "at" and eff[1] == "end":
+            elif len(eff) == 3 and op == "at" and eff[1].value == "end":
                 self._add_effect(
                     problem,
                     act,
                     types_map,
                     universal_assignments,
                     eff[2],
+                    complete_str,
                     timing=up.model.EndTiming(),
                     assignments=assignments,
                 )
             elif len(eff) == 3 and op == "forall":
                 assert universal_assignments is not None
                 action_assignments = universal_assignments.setdefault(act, [])
                 action_assignments.append(eff)
             else:
-                raise SyntaxError(f"Not able to handle: {eff}")
+                start_line, start_col = eff.line_start(complete_str), eff.col_start(
+                    complete_str
+                )
+                end_line, end_col = eff.line_end(complete_str), eff.col_end(
+                    complete_str
+                )
+                raise SyntaxError(
+                    f"Not able to handle: {eff}, from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                )
 
     def _parse_subtask(
         self,
         e,
         method: typing.Optional[Union[htn.Method, htn.TaskNetwork]],
         problem: htn.HierarchicalProblem,
         types_map: TypesMap,
+        complete_str: str,
     ) -> typing.Optional[htn.Subtask]:
         """Returns the Subtask corresponding to the given expression e or
         None if the expression cannot be interpreted as a subtask."""
         if len(e) == 0:
             return None
 
-        task_name = e[0]
+        task_name = e[0].value
         if problem.has_task(task_name) or problem.has_action(task_name):
             # check the form '(task_name param1 param2...)'
             task: Union[htn.Task, up.model.Action]
             if problem.has_task(task_name):
                 task = problem.get_task(task_name)
             else:
                 task = problem.action(task_name)
             assert isinstance(task, htn.Task) or isinstance(task, up.model.Action)
             parameters = [
-                self._parse_exp(problem, method, types_map, {}, param)
-                for param in e[1:]
+                self._parse_exp(problem, method, types_map, {}, e[i], complete_str)
+                for i in range(1, len(e))
             ]
             return htn.Subtask(task, *parameters)
-        elif len(e) == 2 and e[0] != "and":
+        elif len(e) == 2 and e[0].value != "and":
             # check the form "(task_id (task param1 param2...))"
-            task_id = e[0]
-            subtask = self._parse_subtask(e[1], method, problem, types_map)
+            task_id = e[0].value
+            subtask = self._parse_subtask(
+                e[1], method, problem, types_map, complete_str
+            )
             if subtask is not None:
                 # the second element of the list is a valid subtask,
                 # return the subtask, with the given identifier
                 return htn.Subtask(subtask.task, *subtask.parameters, ident=task_id)
             else:
                 return None
         else:
             return None
 
     def _parse_subtasks(
         self,
-        e,
+        e: CustomParseResults,
         method: typing.Optional[Union[htn.Method, htn.TaskNetwork]],
         problem: htn.HierarchicalProblem,
         types_map: TypesMap,
+        complete_str: str,
     ) -> List[htn.Subtask]:
         """Returns the list of subtasks of the expression"""
-        single_task = self._parse_subtask(e, method, problem, types_map)
+        single_task = self._parse_subtask(e, method, problem, types_map, complete_str)
         if single_task is not None:
             return [single_task]
         elif len(e) == 0:
             return []
-        elif e[0] == "and":
+        elif e[0].value == "and":
             return [
                 subtask
-                for e2 in e[1:]
-                for subtask in self._parse_subtasks(e2, method, problem, types_map)
+                for i in range(1, len(e))
+                for subtask in self._parse_subtasks(
+                    e[i], method, problem, types_map, complete_str
+                )
             ]
         else:
-            raise SyntaxError(f"Could not parse the subtasks list: {e}")
+            start_line, start_col = e.line_start(complete_str), e.col_start(
+                complete_str
+            )
+            end_line, end_col = e.line_end(complete_str), e.col_end(complete_str)
+            raise SyntaxError(
+                f"Could not parse the subtasks list: {e}, from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+            )
 
     def _check_if_object_type_is_needed(self, domain_res) -> bool:
         for p in domain_res.get("predicates", []):
             for g in p[1]:
-                if len(g) <= 1 or g[1] == Object:
+                if len(g.value) <= 1 or g.value[1] == Object:
                     return True
         for p in domain_res.get("functions", []):
             for g in p[1]:
-                if len(g) <= 1 or g[1] == Object:
+                if len(g.value) <= 1 or g.value[1] == Object:
                     return True
         for g in domain_res.get("constants", []):
-            if len(g) <= 1 or g[1] == Object:
+            if len(g.value) <= 1 or g.value[1] == Object:
                 return True
         for a in domain_res.get("actions", []):
             for g in a.get("params", []):
-                if len(g) <= 1 or g[1] == Object:
+                if len(g.value) <= 1 or g.value[1] == Object:
                     return True
         for a in domain_res.get("tasks", []):
             for g in a.get("params", []):
-                if len(g) <= 1 or g[1] == Object:
+                if len(g.value) <= 1 or g.value[1] == Object:
                     return True
         for a in domain_res.get("methods", []):
             for g in a.get("params", []):
-                if len(g) <= 1 or g[1] == Object:
+                if len(g.value) <= 1 or g.value[1] == Object:
                     return True
         return False
 
     def _durative_action_has_cost(self, dur_act: up.model.DurativeAction):
         if self._totalcost in self._fve.get(
             dur_act.duration.lower
         ) or self._totalcost in self._fve.get(dur_act.duration.upper):
@@ -756,15 +945,19 @@
                     return False
         for c in problem.goals:
             if self._totalcost in self._fve.get(c):
                 return False
         return True
 
     def _parse_problem(
-        self, domain_res: ParseResults, problem_res: typing.Optional[ParseResults]
+        self,
+        domain_res: ParseResults,
+        domain_str: str,
+        problem_res: typing.Optional[ParseResults],
+        problem_str=typing.Optional[str],
     ) -> "up.model.Problem":
         problem: up.model.Problem
         if ":hierarchy" in set(domain_res.get("features", [])):
             problem = htn.HierarchicalProblem(
                 domain_res["name"],
                 self._env,
                 initial_defaults={self._tm.BoolType(): self._em.FALSE()},
@@ -780,39 +973,35 @@
                 domain_res["name"],
                 self._env,
                 initial_defaults={self._tm.BoolType(): self._em.FALSE()},
             )
 
         types_map: TypesMap = {}
         object_type_needed: bool = self._check_if_object_type_is_needed(domain_res)
-        universal_assignments: Dict["up.model.Action", List[ParseResults]] = {}
+        universal_assignments: Dict["up.model.Action", List[CustomParseResults]] = {}
 
         # extract all type declarations into a dictionary
-        type_declarations: Dict[
-            CaseInsensitiveToken, typing.Optional[CaseInsensitiveToken]
-        ] = {}
+        type_declarations: Dict[str, typing.Optional[str]] = {}
         for type_line in domain_res.get("types", []):
-            father_name = (
-                None if len(type_line) <= 1 else CaseInsensitiveToken(str(type_line[1]))
-            )
+            father_name = None if len(type_line) <= 1 else str(type_line[1])
             if father_name is None and object_type_needed:
                 father_name = Object
             for declared_type in type_line[0]:
-                declared_type = CaseInsensitiveToken(str(declared_type))
+                declared_type = str(declared_type)
                 if declared_type in type_declarations:
                     raise SyntaxError(
                         f"Type {declared_type} is declared more than once"
                     )
                 type_declarations[declared_type] = father_name
 
         # Processes a type and adds it to the `types_map`.
         # If the father was not previously declared, it will be recursively declared as well.
         def declare_type(
-            type: CaseInsensitiveToken,
-            father_name: typing.Optional[CaseInsensitiveToken],
+            type: str,
+            father_name: typing.Optional[str],
         ):
             if type in types_map:
                 # type was already processed which might happen if it already appeared as the parent of another type
                 return
             father: typing.Optional["up.model.Type"]
             if father_name is None:
                 father = None
@@ -824,231 +1013,341 @@
                 father = types_map[father_name]
             elif father_name == Object and not object_type_needed:
                 father = None
             else:  # not "object" and not explicitly declared
                 father = self._env.type_manager.UserType(str(father_name), None)
                 types_map[father_name] = father
             # we identified the father, add the type to our map
-            # note that the type_map allows retrieving the `Type` object in a case-insensitive way
             types_map[type] = self._env.type_manager.UserType(str(type), father)
             # Force declaration of the type in the `Problem`, even if it is not explicitly used yet
             problem._add_user_type(types_map[type])
 
         # declare all types
-        for type, father_name in type_declarations.items():
-            declare_type(type, father_name)
+        for declared_type, father_name in type_declarations.items():
+            declare_type(declared_type, father_name)
 
         if object_type_needed and Object not in types_map:
             # The object type is needed, but has not been defined explicitly. We manually define it
             types_map[Object] = self._env.type_manager.UserType("object", None)
 
         has_actions_cost = False
 
         for p in domain_res.get("predicates", []):
             n = p[0]
             params = OrderedDict()
             for g in p[1]:
-                param_type = types_map[g[1] if len(g) > 1 else Object]
-                for param_name in g[0]:
+                try:
+                    param_type = types_map[g.value[1] if len(g.value) > 1 else Object]
+                except KeyError:
+                    g_start_line, g_start_col = lineno(g.locn_start, domain_str), col(
+                        g.locn_start, domain_str
+                    )
+                    g_end_line, g_end_col = lineno(g.locn_end, domain_str), col(
+                        g.locn_end, domain_str
+                    )
+                    raise SyntaxError(
+                        f"Undefined parameter's type: {g.value[1]}."
+                        + f"\nError from line: {g_start_line}, col: {g_start_col} to line: {g_end_line}, col: {g_end_col}."
+                    )
+                for param_name in g.value[0]:
                     params[param_name] = param_type
             f = up.model.Fluent(n, self._tm.BoolType(), params, self._env)
             problem.add_fluent(f)
 
         for p in domain_res.get("functions", []):
             n = p[0]
             params = OrderedDict()
             for g in p[1]:
-                param_type = types_map[g[1] if len(g) > 1 else Object]
-                for param_name in g[0]:
-                    params[param_name] = param_type
+                g_start_line, g_start_col = lineno(g.locn_start, domain_str), col(
+                    g.locn_start, domain_str
+                )
+                g_end_line, g_end_col = lineno(g.locn_end, domain_str), col(
+                    g.locn_end, domain_str
+                )
+                try:
+                    param_type = types_map[g.value[1] if len(g.value) > 1 else Object]
+                except KeyError:
+                    raise SyntaxError(
+                        f"Undefined parameter's type: {g.value[1]}."
+                        + f"\nError from line: {g_start_line}, col: {g_start_col} to line: {g_end_line}, col: {g_end_col}."
+                    )
+                for param_name in g.value[0]:
+                    if param_name not in params:
+                        params[param_name] = param_type
+                    else:
+                        g_start_line, g_start_col = lineno(
+                            g.locn_start, domain_str
+                        ), col(g.locn_start, domain_str)
+                        g_end_line, g_end_col = lineno(g.locn_end, domain_str), col(
+                            g.locn_end, domain_str
+                        )
+                        raise SyntaxError(
+                            f"In definition of function {n} the parameter {param_name} "
+                            + f"is defined twice.\nError from line: {g_start_line}, col: {g_start_col}"
+                            + f" to line: {g_end_line}, col: {g_end_col}."
+                        )
             f = up.model.Fluent(n, self._tm.RealType(), params, self._env)
             if n == "total-cost":
                 has_actions_cost = True
                 self._totalcost = cast(up.model.FNode, self._em.FluentExp(f))
             problem.add_fluent(f)
 
         for g in domain_res.get("constants", []):
-            t = types_map[g[1] if len(g) > 1 else Object]
-            for o in g[0]:
-                problem.add_object(up.model.Object(o, t, problem.env))
+            try:
+                t = types_map[g.value[1] if len(g.value) > 1 else Object]
+            except KeyError:
+                g_start_line, g_start_col = lineno(g.locn_start, domain_str), col(
+                    g.locn_start, domain_str
+                )
+                g_end_line, g_end_col = lineno(g.locn_end, domain_str), col(
+                    g.locn_end, domain_str
+                )
+                raise SyntaxError(
+                    f"Undefined variable's type: {g.value[1]}."
+                    + f"\nError from line: {g_start_line}, col: {g_start_col} to line: {g_end_line}, col: {g_end_col}."
+                )
+            for o in g.value[0]:
+                problem.add_object(up.model.Object(o, t, problem.environment))
 
         for task in domain_res.get("tasks", []):
             assert isinstance(problem, htn.HierarchicalProblem)
             name = task["name"]
             task_params = OrderedDict()
             for g in task.get("params", []):
-                t = types_map[g[1] if len(g) > 1 else Object]
-                for p in g[0]:
+                try:
+                    t = types_map[g.value[1] if len(g.value) > 1 else Object]
+                except KeyError:
+                    g_start_line, g_start_col = lineno(g.locn_start, domain_str), col(
+                        g.locn_start, domain_str
+                    )
+                    g_end_line, g_end_col = lineno(g.locn_end, domain_str), col(
+                        g.locn_end, domain_str
+                    )
+                    raise SyntaxError(
+                        f"Undefined parameter's type: {g.value[1]}."
+                        + f"\nError from line: {g_start_line}, col: {g_start_col} to line: {g_end_line}, col: {g_end_col}."
+                    )
+                for p in g.value[0]:
                     task_params[p] = t
             task = htn.Task(name, task_params)
             problem.add_task(task)
 
         for a in domain_res.get("actions", []):
             n = a["name"]
             a_params = OrderedDict()
             for g in a.get("params", []):
-                t = types_map[g[1] if len(g) > 1 else Object]
-                for p in g[0]:
+                try:
+                    t = types_map[g.value[1] if len(g.value) > 1 else Object]
+                except KeyError:
+                    g_start_line, g_start_col = lineno(g.locn_start, domain_str), col(
+                        g.locn_start, domain_str
+                    )
+                    g_end_line, g_end_col = lineno(g.locn_end, domain_str), col(
+                        g.locn_end, domain_str
+                    )
+                    raise SyntaxError(
+                        f"Undefined parameter's type: {g.value[1]}."
+                        + f"\nError from line: {g_start_line}, col: {g_start_col} to line: {g_end_line}, col: {g_end_col}."
+                    )
+                for p in g.value[0]:
                     a_params[p] = t
             if "duration" in a:
                 dur_act = up.model.DurativeAction(n, a_params, self._env)
-                dur = a["duration"][0]
-                if dur[0] == "=":
-                    dur.pop(0)
-                    dur.pop(0)
+                dur = CustomParseResults(a["duration"][0])
+                if dur[0].value == "=":
                     dur_act.set_fixed_duration(
-                        self._parse_exp(problem, dur_act, types_map, {}, dur)
+                        self._parse_exp(
+                            problem, dur_act, types_map, {}, dur[2], domain_str
+                        )
                     )
-                elif dur[0] == "and":
+                elif dur[0].value == "and":
                     upper = None
                     lower = None
                     for j in range(1, len(dur)):
-                        if dur[j][0] == ">=" and lower is None:
-                            dur[j].pop(0)
-                            dur[j].pop(0)
+                        if dur[j][0].value == ">=" and lower is None:
                             lower = self._parse_exp(
-                                problem, dur_act, types_map, {}, dur[j]
+                                problem, dur_act, types_map, {}, dur[j][2], domain_str
                             )
-                        elif dur[j][0] == "<=" and upper is None:
-                            dur[j].pop(0)
-                            dur[j].pop(0)
+                        elif dur[j][0].value == "<=" and upper is None:
                             upper = self._parse_exp(
-                                problem, dur_act, types_map, {}, dur[j]
+                                problem, dur_act, types_map, {}, dur[j][2], domain_str
                             )
                         else:
                             raise SyntaxError(
                                 f"Not able to handle duration constraint of action {n}"
+                                + f"Line: {dur.line_start(domain_str)}, col: {dur.col_start(domain_str)}",
                             )
                     if lower is None or upper is None:
                         raise SyntaxError(
                             f"Not able to handle duration constraint of action {n}"
+                            + f"Line: {dur.line_start(domain_str)}, col: {dur.col_start(domain_str)}",
                         )
                     d = up.model.ClosedDurationInterval(lower, upper)
                     dur_act.set_duration_constraint(d)
                 else:
                     raise SyntaxError(
                         f"Not able to handle duration constraint of action {n}"
+                        + f"Line: {dur.line_start(domain_str)}, col: {dur.col_start(domain_str)}",
                     )
-                cond = a["cond"][0]
-                self._add_condition(problem, dur_act, cond, types_map)
-                eff = a["eff"][0]
+                cond = CustomParseResults(a["cond"][0])
+                self._add_condition(problem, dur_act, cond, types_map, domain_str)
+                eff = CustomParseResults(a["eff"][0])
                 self._add_timed_effects(
-                    problem, dur_act, types_map, universal_assignments, eff
+                    problem, dur_act, types_map, universal_assignments, eff, domain_str
                 )
                 problem.add_action(dur_act)
                 has_actions_cost = has_actions_cost and self._durative_action_has_cost(
                     dur_act
                 )
             else:
                 act: typing.Optional[
                     Union[up.model.SensingAction, up.model.InstantaneousAction]
                 ] = None
                 if "obs" in a:
                     act = up.model.SensingAction(n, a_params, self._env)
-                    obs_fluent = a["obs"][0]
-                    if obs_fluent[0] == "and":  # more than 1 fluent
-                        for o in obs_fluent[1:]:
+                    obs_fluent = CustomParseResults(a["obs"][0])
+                    if obs_fluent[0].value == "and":  # more than 1 fluent
+                        for i in range(1, len(obs_fluent)):
                             act.add_observed_fluent(
-                                self._parse_exp(problem, act, types_map, {}, o)
+                                self._parse_exp(
+                                    problem,
+                                    act,
+                                    types_map,
+                                    {},
+                                    obs_fluent[i],
+                                    domain_str,
+                                )
                             )
                     else:
                         act.add_observed_fluent(
-                            self._parse_exp(problem, act, types_map, {}, obs_fluent)
+                            self._parse_exp(
+                                problem, act, types_map, {}, obs_fluent, domain_str
+                            )
                         )
                 else:
                     act = up.model.InstantaneousAction(n, a_params, self._env)
                 if "pre" in a:
                     act.add_precondition(
-                        self._parse_exp(problem, act, types_map, {}, a["pre"][0])
+                        self._parse_exp(
+                            problem,
+                            act,
+                            types_map,
+                            {},
+                            CustomParseResults(a["pre"][0]),
+                            domain_str,
+                        )
                     )
                 if "eff" in a:
                     self._add_effect(
-                        problem, act, types_map, universal_assignments, a["eff"][0]
+                        problem,
+                        act,
+                        types_map,
+                        universal_assignments,
+                        CustomParseResults(a["eff"][0]),
+                        domain_str,
                     )
                 problem.add_action(act)
                 has_actions_cost = (
                     has_actions_cost and self._instantaneous_action_has_cost(act)
                 )
 
         for m in domain_res.get("methods", []):
             assert isinstance(problem, htn.HierarchicalProblem)
             name = m["name"]
             method_params = OrderedDict()
             for g in m.get("params", []):
-                t = types_map[g[1] if len(g) > 1 else Object]
-                for p in g[0]:
+                t = types_map[g.value[1] if len(g.value) > 1 else Object]
+                for p in g.value[0]:
                     method_params[p] = t
 
             method = htn.Method(name, method_params)
-            achieved_task = m["task"][
-                0
-            ]  # a list of the form ["go", "?robot", "?target"]
-            for pname in achieved_task[1:]:
+            achieved_task = CustomParseResults(m["task"][0])
+            pnames = []
+            for i in range(1, len(achieved_task)):
+                pname = achieved_task[i].value
                 if pname[0] != "?":
                     raise SyntaxError(
-                        f"All arguments of the task should be parameters: {achieved_task}"
+                        f"All arguments of the task {achieved_task} should be parameters."
+                        + f"Line: {achieved_task.line_start(domain_str)}, col: {achieved_task.col_start(domain_str)}",
                     )
-            achieved_task_params = [
-                method.parameter(pname[1:]) for pname in achieved_task[1:]
-            ]
-            method.set_task(problem.get_task(achieved_task[0]), *achieved_task_params)
-            for ord_subs in m.get("ordered-subtasks", []):
-                ord_subs = self._parse_subtasks(ord_subs, method, problem, types_map)
+                pnames.append(pname)
+            achieved_task_params = [method.parameter(pname[1:]) for pname in pnames]
+            method.set_task(
+                problem.get_task(achieved_task[0].value), *achieved_task_params
+            )
+            if "ordered-subtasks" in m:
+                ost = CustomParseResults(m.get("ordered-subtasks")[0])
+                ord_subs = self._parse_subtasks(
+                    ost, method, problem, types_map, domain_str
+                )
                 for s in ord_subs:
                     method.add_subtask(s)
                 method.set_ordered(*ord_subs)
-            for subs in m.get("subtasks", []):
-                subs = self._parse_subtasks(subs, method, problem, types_map)
+            if "subtasks" in m:
+                st = CustomParseResults(m.get("subtasks")[0])
+                subs = self._parse_subtasks(st, method, problem, types_map, domain_str)
                 for s in subs:
                     method.add_subtask(s)
-            orderings_queue = list(m.get("ordering", []))
-            while not len(orderings_queue) == 0:
-                ordering = orderings_queue.pop(0)
-                if len(ordering) == 0:
-                    pass
-                elif ordering[0] == "and":
-                    # add the rest of the expression to the queue
-                    orderings_queue += ordering[1:]
-                elif ordering[0] == "<":
-                    if len(ordering) != 3:
+            if "ordering" in m:
+                stack = [CustomParseResults(m.get("ordering")[0])]
+                while stack:
+                    ordering = stack.pop(0)
+                    if len(ordering) == 0:
+                        pass
+                    elif ordering[0].value == "and":
+                        # add the rest of the expression to the queue
+                        for i in range(1, len(ordering)):
+                            stack.append(ordering[i])
+                    elif ordering[0].value == "<":
+                        if len(ordering) != 3:
+                            raise SyntaxError(
+                                f"Wrong number of parameters in ordering relation: {ordering}"
+                                + f"Line: {ordering.line_start(domain_str)}, col: {ordering.col_start(domain_str)}",
+                            )
+                        left = method.get_subtask(ordering[1].value)
+                        right = method.get_subtask(ordering[2].value)
+                        method.set_strictly_before(left, right)
+                    else:
                         raise SyntaxError(
-                            f"Wrong number of parameters in ordering relation: {ordering}"
+                            f"Invalid expression in ordering, expected 'and' or '<' but got '{ordering[0]}"
+                            + f"Line: {ordering.line_start(domain_str)}, col: {ordering.col_start(domain_str)}",
                         )
-                    left = method.get_subtask(ordering[1])
-                    right = method.get_subtask(ordering[2])
-                    method.set_strictly_before(left, right)
-                else:
-                    raise SyntaxError(
-                        f"Invalid expression in ordering, expected 'and' or '<' but got '{ordering[0]}"
-                    )
-            for precondition in m.get("precondition", []):
+            if "precondition" in m:
                 method.add_precondition(
-                    self._parse_exp(problem, method, types_map, {}, precondition)
+                    self._parse_exp(
+                        problem,
+                        method,
+                        types_map,
+                        {},
+                        CustomParseResults(m["precondition"][0]),
+                        domain_str,
+                    )
                 )
             problem.add_method(method)
 
         if problem_res is not None:
+            assert problem_str is not None
             problem.name = problem_res["name"]
 
             for g in problem_res.get("objects", []):
                 t = types_map[g[1] if len(g) > 1 else Object]
                 for o in g[0]:
-                    problem.add_object(up.model.Object(o, t, problem.env))
+                    problem.add_object(up.model.Object(o, t, problem.environment))
 
             for action, eff_list in universal_assignments.items():
                 for eff in eff_list:
                     # Parse the variable definition part and create 2 lists, the first one with the variable names,
                     # the second one with the variable types.
-                    vars_string = " ".join(eff[1])
+                    vars_string = " ".join([e.value for e in eff[1]])
                     vars_res = self._pp_parameters.parseString(vars_string)
                     var_names: List[str] = []
                     var_types: List["up.model.Type"] = []
                     for g in vars_res["params"]:
-                        t = types_map[g[1] if len(g) > 1 else Object]
-                        for o in g[0]:
+                        t = types_map[g.value[1] if len(g.value) > 1 else Object]
+                        for o in g.value[0]:
                             var_names.append(f"?{o}")
                             var_types.append(t)
                     # for each variable type, get all the objects of that type and calculate the cartesian
                     # product between all the given objects and iterate over them, changing the variable assignments
                     # in the added effect
                     for objects in product(*(problem.objects(t) for t in var_types)):
                         assert len(var_names) == len(objects)
@@ -1058,174 +1357,248 @@
                         if isinstance(action, up.model.InstantaneousAction):
                             self._add_effect(
                                 problem,
                                 action,
                                 types_map,
                                 None,
                                 eff[2],
+                                domain_str,
                                 assignments=assignments,
                             )
                         elif isinstance(action, up.model.DurativeAction):
                             self._add_timed_effects(
                                 problem,
                                 action,
                                 types_map,
                                 None,
                                 eff[2],
+                                domain_str,
                                 assignments=assignments,
                             )
                         else:
                             raise NotImplementedError
 
             tasknet = problem_res.get("htn", None)
             if tasknet is not None:
                 assert isinstance(problem, htn.HierarchicalProblem)
 
                 for tn_variables in tasknet.get("params", []):
                     tn_var_type = types_map[
-                        tn_variables[1] if len(tn_variables) > 1 else Object
+                        tn_variables.value[1] if len(tn_variables.value) > 1 else Object
                     ]
-                    for tn_var_name in tn_variables[0]:
+                    for tn_var_name in tn_variables.value[0]:
                         problem.task_network.add_variable(tn_var_name, tn_var_type)
 
-                for subtasks_expr in tasknet.get("tasks", []):
+                ta = tasknet.get("tasks", None)
+                if ta:
                     subtasks = self._parse_subtasks(
-                        subtasks_expr, problem.task_network, problem, types_map
+                        CustomParseResults(ta[0]),
+                        problem.task_network,
+                        problem,
+                        types_map,
+                        problem_str,
                     )
                     for task in subtasks:
                         problem.task_network.add_subtask(task)
-                for subtasks_expr in tasknet.get("ordered-tasks", []):
+
+                ot = tasknet.get("ordered-tasks", None)
+                if ot:
                     subtasks = self._parse_subtasks(
-                        subtasks_expr, problem.task_network, problem, types_map
+                        CustomParseResults(ot[0]),
+                        problem.task_network,
+                        problem,
+                        types_map,
+                        problem_str,
                     )
                     prev = None
                     for task in subtasks:
                         cur = problem.task_network.add_subtask(task)
                         if prev is not None:
                             problem.task_network.set_strictly_before(prev, cur)
                         prev = cur
 
-                orderings_queue = list(tasknet.get("ordering", []))
-                while not len(orderings_queue) == 0:
-                    ordering = orderings_queue.pop(0)
+                oq = tasknet.get("ordering", None)
+                stack = []
+                if oq:
+                    stack.append(CustomParseResults(oq[0]))
+                while len(stack) > 0:
+                    ordering = stack.pop(0)
                     if len(ordering) == 0:
                         pass
-                    elif ordering[0] == "and":
+                    elif ordering[0].value == "and":
                         # add the rest of the expression to the queue
-                        orderings_queue += ordering[1:]
-                    elif ordering[0] == "<":
+                        for i in range(1, len(ordering)):
+                            stack.append(ordering[i])
+                    elif ordering[0].value == "<":
                         if len(ordering) != 3:
                             raise SyntaxError(
                                 f"Wrong number of parameters in ordering relation: {ordering}"
+                                + f"Line: {ordering.line_start(domain_str)}, col: {ordering.col_start(domain_str)}",
                             )
-                        left = problem.task_network.get_subtask(ordering[1])
-                        right = problem.task_network.get_subtask(ordering[2])
+                        left = problem.task_network.get_subtask(ordering[1].value)
+                        right = problem.task_network.get_subtask(ordering[2].value)
                         problem.task_network.set_strictly_before(left, right)
                     else:
                         raise SyntaxError(
                             f"Invalid expression in ordering, expected 'and' or '<' but got '{ordering[0]}"
+                            + f"Line: {ordering.line_start(domain_str)}, col: {ordering.col_start(domain_str)}",
                         )
 
-                for constraint in tasknet.get("constraints", []):
-                    problem.task_network.add_constraint(
-                        self._parse_exp(
-                            problem, problem.task_network, types_map, {}, constraint
+                cs = tasknet.get("constraints", None)
+                if cs:
+                    constraints = CustomParseResults(cs[0])
+                    for i in range(len(constraints)):
+                        constraint = constraints[i]
+                        problem.task_network.add_constraint(
+                            self._parse_exp(
+                                problem,
+                                problem.task_network,
+                                types_map,
+                                {},
+                                constraint,
+                                problem_str,
+                            )
                         )
-                    )
 
             init_list = problem_res.get("init", [])
-            if len(init_list) == 1 and init_list[0][0] == "and":
-                init_list = init_list[0][1:]
-            for i in init_list:
-                operator = i[0]
+            if len(init_list) == 1 and list(init_list[0].value[0].value) == ["and"]:
+                init_list = init_list[0].value[1:]
+            for j in init_list:
+                init = CustomParseResults(j)
+                operator = init[0].value
                 if operator == "=":
                     problem.set_initial_value(
-                        self._parse_exp(problem, None, types_map, {}, i[1]),
-                        self._parse_exp(problem, None, types_map, {}, i[2]),
+                        self._parse_exp(
+                            problem, None, types_map, {}, init[1], problem_str
+                        ),
+                        self._parse_exp(
+                            problem, None, types_map, {}, init[2], problem_str
+                        ),
                     )
                 elif (
-                    len(i) == 3
+                    len(init) == 3
                     and operator == "at"
-                    and i[1].replace(".", "", 1).isdigit()
+                    and init[1].value.replace(".", "", 1).isdigit()
                 ):
-                    ti = up.model.StartTiming(Fraction(i[1]))
-                    va = self._parse_exp(problem, None, types_map, {}, i[2])
+                    try:
+                        ti = up.model.StartTiming(Fraction(init[1].value))
+                    except ValueError:
+                        start_line, start_col = init.line_start(
+                            problem_str
+                        ), init.col_start(problem_str)
+                        end_line, end_col = init.line_end(problem_str), init.col_end(
+                            problem_str
+                        )
+                        raise SyntaxError(
+                            f"Expected number, found {init[1].value} in expression from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                        )
+                    va = self._parse_exp(
+                        problem, None, types_map, {}, init[2], problem_str
+                    )
                     if va.is_fluent_exp():
                         problem.add_timed_effect(ti, va, self._em.TRUE())
                     elif va.is_not():
                         problem.add_timed_effect(ti, va.arg(0), self._em.FALSE())
                     elif va.is_equals():
                         problem.add_timed_effect(ti, va.arg(0), va.arg(1))
                     else:
-                        raise SyntaxError(f"Not able to handle this TIL {i}")
+                        raise SyntaxError(
+                            f"Not able to handle this TIL {init}"
+                            + f"Line: {init.line_start(problem_str)}, col: {init.col_start(problem_str)}",
+                        )
                 elif operator == "oneof":
                     assert isinstance(problem, ContingentProblem)
                     fluents = [
-                        self._parse_exp(problem, None, types_map, {}, x) for x in i[1:]
+                        self._parse_exp(
+                            problem, None, types_map, {}, init[x], problem_str
+                        )
+                        for x in range(1, len(init))
                     ]
                     problem.add_oneof_initial_constraint(fluents)
                 elif operator == "or":
                     assert isinstance(problem, ContingentProblem)
                     fluents = [
-                        self._parse_exp(problem, None, types_map, {}, x) for x in i[1:]
+                        self._parse_exp(
+                            problem, None, types_map, {}, init[x], problem_str
+                        )
+                        for x in range(1, len(init))
                     ]
                     problem.add_or_initial_constraint(fluents)
                 elif operator == "unknown":
                     assert isinstance(problem, ContingentProblem)
-                    if len(i) != 2:
+                    if len(init) != 2:
                         raise SyntaxError(
                             "`unknown` constraint requires exactly one argument."
+                            + f"Line: {init.line_start(problem_str)}, col: {init.col_start(problem_str)}",
                         )
-                    arg = self._parse_exp(problem, None, types_map, {}, i[1])
+                    arg = self._parse_exp(
+                        problem, None, types_map, {}, init[1], problem_str
+                    )
                     problem.add_unknown_initial_constraint(arg)
                 else:
                     problem.set_initial_value(
-                        self._parse_exp(problem, None, types_map, {}, i),
+                        self._parse_exp(
+                            problem, None, types_map, {}, init, problem_str
+                        ),
                         self._em.TRUE(),
                     )
 
             if "goal" in problem_res:
                 problem.add_goal(
                     self._parse_exp(
-                        problem, None, types_map, {}, problem_res["goal"][0]
+                        problem,
+                        None,
+                        types_map,
+                        {},
+                        CustomParseResults(problem_res["goal"][0]),
+                        problem_str,
                     )
                 )
             elif not isinstance(problem, htn.HierarchicalProblem):
                 raise SyntaxError("Missing goal section in problem file.")
 
             if "constraints" in problem_res:
                 problem.add_trajectory_constraint(
                     self._parse_exp(
-                        problem, None, types_map, {}, problem_res["constraints"][0]
+                        problem,
+                        None,
+                        types_map,
+                        {},
+                        CustomParseResults(problem_res["constraints"][0]),
+                        problem_str,
                     )
                 )
 
             has_actions_cost = has_actions_cost and self._problem_has_actions_cost(
                 problem
             )
             optimization = problem_res.get("optimization", None)
-            metric = problem_res.get("metric", None)
+            m = problem_res.get("metric", None)
 
-            if metric is not None:
+            if m is not None:
+                metric = CustomParseResults(m[0])
                 if (
                     optimization == "minimize"
                     and len(metric) == 1
-                    and metric[0] == "total-time"
+                    and metric[0].value == "total-time"
                 ):
                     problem.add_quality_metric(up.model.metrics.MinimizeMakespan())
                 else:
-                    metric_exp = self._parse_exp(problem, None, types_map, {}, metric)
+                    metric_exp = self._parse_exp(
+                        problem, None, types_map, {}, metric, problem_str
+                    )
                     if (
                         has_actions_cost
                         and optimization == "minimize"
                         and metric_exp == self._totalcost
                     ):
                         costs = {}
                         problem._fluents.remove(self._totalcost.fluent())
-                        problem._initial_value.pop(self._totalcost)
+                        if self._totalcost in problem._initial_value:
+                            problem._initial_value.pop(self._totalcost)
                         use_plan_length = all(False for _ in problem.durative_actions)
                         for a in problem.instantaneous_actions:
                             cost = None
                             for e in a.effects:
                                 if e.fluent == self._totalcost:
                                     cost = e
                                     break
@@ -1269,41 +1642,54 @@
     def parse_problem(
         self, domain_filename: str, problem_filename: typing.Optional[str] = None
     ) -> "up.model.Problem":
         """
         Takes in input a filename containing the `PDDL` domain and optionally a filename
         containing the `PDDL` problem and returns the parsed `Problem`.
 
-        Note that if the `problem_filename` is `None`, an incomplete `Problem` will be returned.
+        Note: that if the `problem_filename` is `None`, an incomplete `Problem` will be returned.
+
+        Note: due to PDDL case-insensitivity, everything in the PDDL files will be turned to
+        lower case, so the names of fluents, actions etc. and the error report will all be
+        in lower-case.
 
         :param domain_filename: The path to the file containing the `PDDL` domain.
         :param problem_filename: Optionally the path to the file containing the `PDDL` problem.
         :return: The `Problem` parsed from the given pddl domain + problem.
         """
-        domain_res = self._pp_domain.parse_file(domain_filename, parse_all=True)
+        with open(domain_filename, "r") as domain_file:
+            domain_str = domain_file.read()
 
-        problem_res = None
+        problem_str = None
         if problem_filename is not None:
-            problem_res = self._pp_problem.parse_file(problem_filename, parse_all=True)
+            with open(problem_filename, "r") as problem_file:
+                problem_str = problem_file.read()
 
-        return self._parse_problem(domain_res, problem_res)
+        return self.parse_problem_string(domain_str, problem_str)
 
     def parse_problem_string(
         self, domain_str: str, problem_str: typing.Optional[str] = None
     ) -> "up.model.Problem":
         """
         Takes in input a str representing the `PDDL` domain and optionally a str
         representing the `PDDL` problem and returns the parsed `Problem`.
 
         Note that if the `problem_str` is `None`, an incomplete `Problem` will be returned.
 
+        Note: due to PDDL case-insensitivity, everything in the PDDL files will be turned to
+        lower case, so the names of fluents, actions etc. and the error report will all be
+        in lower-case.
+
         :param domain_filename: The string representing the `PDDL` domain.
         :param problem_filename: Optionally the string representing the `PDDL` problem.
         :return: The `Problem` parsed from the given pddl domain + problem.
         """
-        domain_res = self._pp_domain.parse_string(domain_str, parse_all=True)
+        domain_str = domain_str.replace("\t", " ").lower()
+        domain_res = parse_string(self._pp_domain, domain_str, parse_all=True)
+
         if problem_str is not None:
-            problem_res = self._pp_problem.parse_string(problem_str, parse_all=True)
+            problem_str = problem_str.replace("\t", " ").lower()
+            problem_res = parse_string(self._pp_problem, problem_str, parse_all=True)
         else:
             problem_res = None
 
-        return self._parse_problem(domain_res, problem_res)
+        return self._parse_problem(domain_res, domain_str, problem_res, problem_str)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/io/pddl_writer.py` & `unified_planning-0.6.0/unified_planning/io/ma_pddl_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,748 +9,721 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-
+import os as osy
 from fractions import Fraction
 import sys
 import re
 
 from decimal import Decimal, localcontext
 from warnings import warn
-
 import unified_planning as up
 import unified_planning.environment
 import unified_planning.model.walkers as walkers
 from unified_planning.model import (
     InstantaneousAction,
     DurativeAction,
     Fluent,
     Parameter,
     Problem,
     Object,
 )
+from unified_planning.model.multi_agent.agent import Agent
 from unified_planning.exceptions import (
     UPTypeError,
     UPProblemDefinitionError,
     UPException,
 )
 from unified_planning.model.types import _UserType
 from typing import Callable, Dict, IO, List, Optional, Set, Union, cast
 from io import StringIO
 from functools import reduce
+from unified_planning.io.pddl_writer import (
+    ObjectsExtractor,
+    ConverterToPDDLString,
+    PDDL_KEYWORDS,
+    INITIAL_LETTER,
+    _write_effect,
+)
 
-PDDL_KEYWORDS = {
-    "define",
-    "domain",
-    "requirements",
-    "types",
-    "constants",
-    "atomic",
-    "predicates",
-    "problem",
-    "atomic",
-    "constraints",
-    "either",
-    "number",
-    "action",
-    "parameters",
-    "precondition",
-    "effect",
-    "and",
-    "forall",
-    "preference",
-    "or",
-    "not",
-    "imply",
-    "exists",
-    "scale-up",
-    "scale-down",
-    "increase",
-    "decrease",
-    "durative-action",
-    "duration",
-    "condition",
-    "at",
-    "over",
-    "start",
-    "end",
-    "all",
-    "derived",
-    "objects",
-    "init",
-    "goal",
-    "when",
-    "decrease",
-    "always",
-    "sometime",
-    "within",
-    "at-most-once",
-    "sometime-after",
-    "sometime-before",
-    "always-within",
-    "hold-during",
-    "hold-after",
-    "metric",
-    "minimize",
-    "maximize",
-    "total-time",
-    "is-violated",
-    "strips",
-    "negative-preconditions",
-    "typing",
-    "disjunctive-preconditions",
-    "equality",
-    "existential-preconditions",
-    "universal-preconditions",
-    "quantified-preconditions",
-    "conditional-effects",
-    "fluents",
-    "adl",
-    "durative-actions",
-    "derived-predicates",
-    "timed-initial-literals",
-    "preferences",
-    "contingent",
-}
-
-# The following map is used to mangle the invalid names by their class.
-INITIAL_LETTER: Dict[type, str] = {
-    InstantaneousAction: "a",
-    DurativeAction: "a",
-    Fluent: "f",
-    Parameter: "p",
-    Problem: "p",
-    Object: "o",
-}
-
-
-class ObjectsExtractor(walkers.DagWalker):
-    """Returns the object instances appearing in the expression."""
-
-    def __init__(self):
-        walkers.dag.DagWalker.__init__(self)
-
-    def get(self, expression: "up.model.FNode") -> Dict[_UserType, Set[Object]]:
-        """Returns all the free vars of the given expression."""
-        return self.walk(expression)
-
-    def walk_object_exp(
-        self, expression: "up.model.FNode", args: List[Dict[_UserType, Set[Object]]]
-    ) -> Dict[_UserType, Set[Object]]:
-        res: Dict[_UserType, Set[Object]] = {}
-        for a in args:
-            _update_domain_objects(res, a)
-        obj = expression.object()
-        assert obj.type.is_user_type()
-        res.setdefault(cast(_UserType, obj.type), set()).add(obj)
-        return res
-
-    @walkers.handles(
-        set(up.model.OperatorKind).difference((up.model.OperatorKind.OBJECT_EXP,))
-    )
-    def walk_all_types(
-        self, expression: "up.model.FNode", args: List[Dict[_UserType, Set[Object]]]
-    ) -> Dict[_UserType, Set[Object]]:
-        res: Dict[_UserType, Set[Object]] = {}
-        for a in args:
-            _update_domain_objects(res, a)
-        return res
-
-
-class ConverterToPDDLString(walkers.DagWalker):
-    """Expression converter to a PDDL string."""
 
-    DECIMAL_PRECISION = 10  # Number of decimal places to print real constants
+class ConverterToMAPDDLString(ConverterToPDDLString):
+    """Expression converter to a MA-PDDL string."""
 
     def __init__(
         self,
         env: "up.environment.Environment",
         get_mangled_name: Callable[
             [
                 Union[
                     "up.model.Type",
                     "up.model.Action",
                     "up.model.Fluent",
                     "up.model.Object",
+                    "up.model.multi_agent.Agent",
                 ]
             ],
             str,
         ],
+        agent: Optional["up.model.multi_agent.Agent"],
     ):
-        walkers.DagWalker.__init__(self)
-        self.get_mangled_name = get_mangled_name
-        self.simplifier = env.simplifier
-
-    def convert(self, expression):
-        """Converts the given expression to a PDDL string."""
-        return self.walk(self.simplifier.simplify(expression))
-
-    def walk_exists(self, expression, args):
-        assert len(args) == 1
-        vars_string_list = [
-            f"{self.get_mangled_name(v)} - {self.get_mangled_name(v.type)}"
-            for v in expression.variables()
-        ]
-        return f'(exists ({" ".join(vars_string_list)})\n {args[0]})'
-
-    def walk_forall(self, expression, args):
-        assert len(args) == 1
-        vars_string_list = [
-            f"{self.get_mangled_name(v)} - {self.get_mangled_name(v.type)}"
-            for v in expression.variables()
-        ]
-        return f'(forall ({" ".join(vars_string_list)})\n {args[0]})'
-
-    def walk_always(self, expression, args):
-        assert len(args) == 1
-        return f"(always {args[0]})"
-
-    def walk_at_most_once(self, expression, args):
-        assert len(args) == 1
-        return f"(at-most-once {args[0]})"
-
-    def walk_sometime(self, expression, args):
-        assert len(args) == 1
-        return f"(sometime {args[0]})"
-
-    def walk_sometime_before(self, expression, args):
-        assert len(args) == 2
-        return f"(sometime-before {args[0]} {args[1]})"
-
-    def walk_sometime_after(self, expression, args):
-        assert len(args) == 2
-        return f"(sometime-after {args[0]} {args[1]})"
-
-    def walk_variable_exp(self, expression, args):
-        assert len(args) == 0
-        return f"{self.get_mangled_name(expression.variable())}"
-
-    def walk_and(self, expression, args):
-        assert len(args) > 1
-        return f'(and {" ".join(args)})'
-
-    def walk_or(self, expression, args):
-        assert len(args) > 1
-        return f'(or {" ".join(args)})'
-
-    def walk_not(self, expression, args):
-        assert len(args) == 1
-        return f"(not {args[0]})"
-
-    def walk_implies(self, expression, args):
-        assert len(args) == 2
-        return f"(imply {args[0]} {args[1]})"
-
-    def walk_iff(self, expression, args):
-        assert len(args) == 2
-        return f"(and (imply {args[0]} {args[1]}) (imply {args[1]} {args[0]}) )"
+        ConverterToPDDLString.__init__(self, env, get_mangled_name)
+        self.agent = agent
+
+    def walk_dot(self, expression, args):
+        agent = expression.agent()
+        fluent = expression.args[0].fluent()
+        objects = expression.args[0].args
+        return f'(a_{self.get_mangled_name(fluent)} {self.get_mangled_name(agent)} {" ".join([self.convert(obj) for obj in objects])})'
 
     def walk_fluent_exp(self, expression, args):
         fluent = expression.fluent()
-        return f'({self.get_mangled_name(fluent)}{" " if len(args) > 0 else ""}{" ".join(args)})'
-
-    def walk_param_exp(self, expression, args):
-        assert len(args) == 0
-        p = expression.parameter()
-        return f"{self.get_mangled_name(p)}"
-
-    def walk_object_exp(self, expression, args):
-        assert len(args) == 0
-        o = expression.object()
-        return f"{self.get_mangled_name(o)}"
-
-    def walk_bool_constant(self, expression, args):
-        raise up.exceptions.UPUnreachableCodeError
-
-    def walk_real_constant(self, expression, args):
-        assert len(args) == 0
-        frac = expression.constant_value()
-
-        with localcontext() as ctx:
-            ctx.prec = self.DECIMAL_PRECISION
-            dec = frac.numerator / Decimal(frac.denominator, ctx)
-
-            if Fraction(dec) != frac:
-                warn(
-                    "The PDDL printer cannot exactly represent the real constant '%s'"
-                    % frac
-                )
-            return str(dec)
-
-    def walk_int_constant(self, expression, args):
-        assert len(args) == 0
-        return str(expression.constant_value())
-
-    def walk_plus(self, expression, args):
-        assert len(args) > 1
-        return reduce(lambda x, y: f"(+ {y} {x})", args)
-
-    def walk_minus(self, expression, args):
-        assert len(args) == 2
-        return f"(- {args[0]} {args[1]})"
-
-    def walk_times(self, expression, args):
-        assert len(args) > 1
-        return reduce(lambda x, y: f"(* {y} {x})", args)
-
-    def walk_div(self, expression, args):
-        assert len(args) == 2
-        return f"(/ {args[0]} {args[1]})"
-
-    def walk_le(self, expression, args):
-        assert len(args) == 2
-        return f"(<= {args[0]} {args[1]})"
-
-    def walk_lt(self, expression, args):
-        assert len(args) == 2
-        return f"(< {args[0]} {args[1]})"
-
-    def walk_equals(self, expression, args):
-        assert len(args) == 2
-        return f"(= {args[0]} {args[1]})"
+        if self.agent is not None and fluent in self.agent.fluents:
+            return f'(a_{self.get_mangled_name(fluent)} ?{self.agent.name}{" " if len(args) > 0 else ""}{" ".join(args)})'
+        else:
+            return f'({self.get_mangled_name(fluent)}{" " if len(args) > 0 else ""}{" ".join(args)})'
 
 
-class PDDLWriter:
-    """This class can be used to write a :class:`~unified_planning.model.Problem` in `PDDL`."""
+class MAPDDLWriter:
+    """
+    This class can be used to write a :class:`~unified_planning.model.MultiAgentProblem` in `MA-PDDL`.
+    The constructor of this class takes the problem to write and 2 flags:
+    needs_requirements determines if the printed problem must have the :requirements,
+    rewrite_bool_assignments determines if this writer will write
+    non constant boolean assignment as conditional effects.
+    """
 
-    def __init__(self, problem: "up.model.Problem", needs_requirements: bool = True):
+    def __init__(
+        self,
+        problem: "up.model.multi_agent.MultiAgentProblem",
+        needs_requirements: bool = True,
+        rewrite_bool_assignments: bool = False,
+    ):
+        self._env = problem.environment
         self.problem = problem
         self.problem_kind = self.problem.kind
         self.needs_requirements = needs_requirements
+        self.rewrite_bool_assignments = rewrite_bool_assignments
         # otn represents the old to new renamings
         self.otn_renamings: Dict[
             Union[
                 "up.model.Type",
                 "up.model.Action",
                 "up.model.Fluent",
                 "up.model.Object",
                 "up.model.Parameter",
                 "up.model.Variable",
+                "up.model.multi_agent.Agent",
             ],
             str,
         ] = {}
         # nto represents the new to old renamings
         self.nto_renamings: Dict[
             str,
             Union[
                 "up.model.Type",
                 "up.model.Action",
                 "up.model.Fluent",
                 "up.model.Object",
                 "up.model.Parameter",
                 "up.model.Variable",
+                "up.model.multi_agent.Agent",
             ],
         ] = {}
         # those 2 maps are "simmetrical", meaning that "(otn[k] == v) implies (nto[v] == k)"
         self.domain_objects: Optional[Dict[_UserType, Set[Object]]] = None
+        self.domain_objects_agents: Dict[up.model.multi_agent.Agent, str]
+        self.all_public_fluents: Set[Fluent] = set()
 
-    def _write_domain(self, out: IO[str]):
-        if self.problem_kind.has_intermediate_conditions_and_effects():
-            raise UPProblemDefinitionError(
-                "PDDL2.1 does not support ICE.\nICE are Intermediate Conditions and Effects therefore when an Effect (or Condition) are not at StartTIming(0) or EndTIming(0)."
-            )
-        if self.problem_kind.has_timed_effect() or self.problem_kind.has_timed_goals():
-            raise UPProblemDefinitionError(
-                "PDDL2.1 does not support timed effects or timed goals."
-            )
-        obe = ObjectsExtractor()
-        out.write("(define ")
-        if self.problem.name is None:
-            name = "pddl"
-        else:
-            name = _get_pddl_name(self.problem)
-        out.write(f"(domain {name}-domain)\n")
-
-        if self.needs_requirements:
-            out.write(" (:requirements :strips")
-            if self.problem_kind.has_flat_typing():
-                out.write(" :typing")
-            if self.problem_kind.has_negative_conditions():
-                out.write(" :negative-preconditions")
-            if self.problem_kind.has_disjunctive_conditions():
-                out.write(" :disjunctive-preconditions")
-            if self.problem_kind.has_equality():
-                out.write(" :equality")
-            if (
-                self.problem_kind.has_continuous_numbers()
-                or self.problem_kind.has_discrete_numbers()
-            ):
-                out.write(" :numeric-fluents")
-            if self.problem_kind.has_conditional_effects():
-                out.write(" :conditional-effects")
-            if self.problem_kind.has_existential_conditions():
-                out.write(" :existential-preconditions")
-            if self.problem_kind.has_trajectory_constraints():
-                out.write(" :constraints")
-            if self.problem_kind.has_universal_conditions():
-                out.write(" :universal-preconditions")
-            if (
-                self.problem_kind.has_continuous_time()
-                or self.problem_kind.has_discrete_time()
-            ):
-                out.write(" :durative-actions")
-            if self.problem_kind.has_duration_inequalities():
-                out.write(" :duration-inequalities")
+    def _write_domain(self):
+        ag_domains = {}
+        for ag in self.problem.agents:
+            out = StringIO()
+            if self.problem_kind.has_intermediate_conditions_and_effects():
+                raise UPProblemDefinitionError(
+                    "PDDL2.1 does not support ICE.\nICE are Intermediate Conditions and Effects therefore when an Effect (or Condition) are not at StartTIming(0) or EndTIming(0)."
+                )
             if (
-                self.problem_kind.has_actions_cost()
-                or self.problem_kind.has_plan_length()
+                self.problem_kind.has_timed_effects()
+                or self.problem_kind.has_timed_goals()
             ):
-                out.write(" :action-costs")
-            out.write(")\n")
+                raise UPProblemDefinitionError(
+                    "PDDL2.1 does not support timed effects or timed goals."
+                )
+            obe = ObjectsExtractor()
+            out.write("(define ")
+            if self.problem.name is None:
+                name = "ma-pddl"
+            else:
+                name = _get_pddl_name(self.problem)
+            out.write(f"(domain {name}-domain)\n")
 
-        if self.problem_kind.has_hierarchical_typing():
-            user_types_hierarchy = self.problem.user_types_hierarchy
-            out.write(f" (:types\n")
-            stack: List["unified_planning.model.Type"] = (
-                user_types_hierarchy[None] if None in user_types_hierarchy else []
-            )
-            out.write(
-                f'    {" ".join(self._get_mangled_name(t) for t in stack)} - object\n'
-            )
-            while stack:
-                current_type = stack.pop()
-                direct_sons: List["unified_planning.model.Type"] = user_types_hierarchy[
-                    current_type
-                ]
-                if direct_sons:
-                    stack.extend(direct_sons)
-                    out.write(
-                        f'    {" ".join([self._get_mangled_name(t) for t in direct_sons])} - {self._get_mangled_name(current_type)}\n'
-                    )
-            out.write(" )\n")
-        else:
-            pddl_types = [
-                self._get_mangled_name(t)
-                for t in self.problem.user_types
-                if cast(_UserType, t).name != "object"
-            ]
-            out.write(
-                f' (:types {" ".join(pddl_types)})\n' if len(pddl_types) > 0 else ""
-            )
-
-        if self.domain_objects is None:
-            # This method populates the self._domain_objects map
-            self._populate_domain_objects(obe)
-        assert self.domain_objects is not None
-
-        if len(self.domain_objects) > 0:
-            out.write(" (:constants")
-            for ut, os in self.domain_objects.items():
-                if len(os) > 0:
-                    out.write(
-                        f'\n   {" ".join([self._get_mangled_name(o) for o in os])} - {self._get_mangled_name(ut)}'
-                    )
-            out.write("\n )\n")
+            if self.needs_requirements:
+                out.write(" (:requirements :factored-privacy")
+                # out.write(" (:requirements :strips")
+                if self.problem_kind.has_flat_typing():
+                    out.write(" :typing")
+                if self.problem_kind.has_negative_conditions():
+                    out.write(" :negative-preconditions")
+                if self.problem_kind.has_disjunctive_conditions():
+                    out.write(" :disjunctive-preconditions")
+                if self.problem_kind.has_equalities():
+                    out.write(" :equality")
+                if (
+                    self.problem_kind.has_continuous_numbers()
+                    or self.problem_kind.has_discrete_numbers()
+                ):
+                    out.write(" :numeric-fluents")
+                if self.problem_kind.has_conditional_effects():
+                    out.write(" :conditional-effects")
+                if self.problem_kind.has_existential_conditions():
+                    out.write(" :existential-preconditions")
+                if self.problem_kind.has_universal_conditions():
+                    out.write(" :universal-preconditions")
+                if (
+                    self.problem_kind.has_continuous_time()
+                    or self.problem_kind.has_discrete_time()
+                ):
+                    out.write(" :durative-actions")
+                if self.problem_kind.has_duration_inequalities():
+                    out.write(" :duration-inequalities")
+                if (
+                    self.problem_kind.has_actions_cost()
+                    or self.problem_kind.has_plan_length()
+                ):
+                    out.write(" :action-costs")
+                out.write(")\n")
 
-        predicates = []
-        functions = []
-        for f in self.problem.fluents:
-            if f.type.is_bool_type():
-                params = []
-                i = 0
-                for param in f.signature:
-                    if param.type.is_user_type():
-                        params.append(
-                            f" {self._get_mangled_name(param)} - {self._get_mangled_name(param.type)}"
+            if self.problem_kind.has_hierarchical_typing():
+                user_types_hierarchy = self.problem.user_types_hierarchy
+                out.write(f" (:types\n")
+                stack: List["unified_planning.model.Type"] = (
+                    user_types_hierarchy[None] if None in user_types_hierarchy else []
+                )
+                out.write(
+                    f'    {" ".join(self._get_mangled_name(t) for t in stack)}{" " if len(self.problem.agents) > 0 else ""}ag - object\n'
+                )
+                out.write(
+                    f'    {" ".join(self._get_mangled_name(ag) + "_type" for ag in self.problem.agents)} - ag\n'
+                )
+                while stack:
+                    current_type = stack.pop()
+                    direct_sons: List[
+                        "unified_planning.model.Type"
+                    ] = user_types_hierarchy[current_type]
+                    if direct_sons:
+                        stack.extend(direct_sons)
+                        out.write(
+                            f'    {" ".join([self._get_mangled_name(t) for t in direct_sons])} - {self._get_mangled_name(current_type)}\n'
                         )
-                        i += 1
-                    else:
-                        raise UPTypeError("PDDL supports only user type parameters")
-                predicates.append(f'({self._get_mangled_name(f)}{"".join(params)})')
-            elif f.type.is_int_type() or f.type.is_real_type():
+                out.write(" )\n")
+            else:
+                out.write(
+                    f' (:types {" ".join([self._get_mangled_name(t) for t in self.problem.user_types])}{" " if len(self.problem.agents) > 0 else ""}ag - object\n'
+                    if len(self.problem.user_types) > 0
+                    else ""
+                )
+                out.write(
+                    f'    {" ".join(self._get_mangled_name(ag) + "_type" for ag in self.problem.agents)} - ag\n'
+                )
+                out.write(" )\n")
+
+            if self.domain_objects is None:
+                # This method populates the self._domain_objects map
+                self._populate_domain_objects(obe, ag)
+            assert self.domain_objects is not None
+
+            if len(self.all_public_fluents) == 0:
+                self._all_public_fluents(self.all_public_fluents, self.problem.agents)
+
+            if len(self.domain_objects) > 0:
+                out.write(" (:constants")
+                for ut, os in self.domain_objects.items():
+                    if len(os) > 0:
+                        out.write(
+                            f'\n   {" ".join([self._get_mangled_name(o) for o in os])} - {self._get_mangled_name(ut)}'
+                        )
+            if len(self.domain_objects_agents) > 0:
+                for k, v in self.domain_objects_agents.items():
+                    if len(v) > 0:
+                        out.write(f"\n   {self._get_mangled_name(k)} - {v}")
+
+            if len(self.domain_objects) > 0 or len(self.domain_objects_agents) > 0:
+                out.write("\n )\n")
+
+            (
+                predicates_environment,
+                functions_environment,
+            ) = self.get_predicates_functions(self.problem.ma_environment)
+            predicates_agent, functions_agent = self.get_predicates_functions(
+                ag, is_private=True
+            )
+
+            predicates_public_agent = []
+            functions_public_agent = []
+            for f in self.all_public_fluents:
                 params = []
                 i = 0
                 for param in f.signature:
                     if param.type.is_user_type():
                         params.append(
                             f" {self._get_mangled_name(param)} - {self._get_mangled_name(param.type)}"
                         )
                         i += 1
                     else:
-                        raise UPTypeError("PDDL supports only user type parameters")
-                functions.append(f'({self._get_mangled_name(f)}{"".join(params)})')
-            else:
-                raise UPTypeError("PDDL supports only boolean and numerical fluents")
-        if self.problem.kind.has_actions_cost() or self.problem.kind.has_plan_length():
-            functions.append("(total-cost)")
-        out.write(
-            f' (:predicates {" ".join(predicates)})\n' if len(predicates) > 0 else ""
-        )
-        out.write(
-            f' (:functions {" ".join(functions)})\n' if len(functions) > 0 else ""
-        )
+                        raise UPTypeError("MA-PDDL supports only user type parameters")
+                expression = (
+                    f'(a_{self._get_mangled_name(f)} ?agent - {"ag"}{"".join(params)})'
+                )
+                if f.type.is_bool_type():
+                    predicates_public_agent.append(expression)
+                elif f.type.is_int_type() or f.type.is_real_type():
+                    functions_public_agent.append(expression)
+                else:
+                    raise UPTypeError(
+                        "MA-PDDL supports only boolean and numerical fluents"
+                    )
 
-        converter = ConverterToPDDLString(self.problem.env, self._get_mangled_name)
-        costs = {}
-        metrics = self.problem.quality_metrics
-        if len(metrics) == 1:
-            metric = metrics[0]
-            if isinstance(metric, up.model.metrics.MinimizeActionCosts):
-                for a in self.problem.actions:
-                    cost_exp = metric.get_action_cost(a)
-                    costs[a] = cost_exp
-                    if cost_exp is not None:
-                        _update_domain_objects(self.domain_objects, obe.get(cost_exp))
-            elif isinstance(metric, up.model.metrics.MinimizeSequentialPlanLength):
-                for a in self.problem.actions:
-                    costs[a] = self.problem.env.expression_manager.Int(1)
-        elif len(metrics) > 1:
-            raise up.exceptions.UPUnsupportedProblemTypeError(
-                "Only one metric is supported!"
+            predicates_agent_goal = []
+            functions_agent_goal = []
+            for g in self.problem.goals:
+                if g.is_dot():
+                    f = g.args[0].fluent()
+                    agent = g.agent()
+                    # args = g.args
+                    # objects = g.args[0].args
+                    if f not in ag.fluents:
+                        if f.type.is_bool_type():
+                            params = []
+                            i = 0
+                            for param in f.signature:
+                                if param.type.is_user_type():
+                                    params.append(
+                                        f" {self._get_mangled_name(param)} - {self._get_mangled_name(param.type)}"
+                                    )
+                                    i += 1
+                                else:
+                                    raise UPTypeError(
+                                        "MA-PDDL supports only user type parameters"
+                                    )
+                            predicates_agent_goal.append(
+                                f'(a_{self._get_mangled_name(f)} ?agent - {self._get_mangled_name(agent) + "_type"}{"".join(params)})'
+                            )
+                        elif f.type.is_int_type() or f.type.is_real_type():
+                            params = []
+                            i = 0
+                            for param in f.signature:
+                                if param.type.is_user_type():
+                                    params.append(
+                                        f" {self._get_mangled_name(param)} - {self._get_mangled_name(param.type)}"
+                                    )
+                                    i += 1
+                                else:
+                                    raise UPTypeError(
+                                        "MA-PDDL supports only user type parameters"
+                                    )
+                            functions_agent_goal.append(
+                                f'(a_{self._get_mangled_name(f)} ?agent - {self._get_mangled_name(agent) + "_type"}{"".join(params)})'
+                            )
+                        else:
+                            raise UPTypeError(
+                                "MA-PDDL supports only boolean and numerical fluents"
+                            )
+
+            nl = "\n  "
+            out.write(
+                f" (:predicates\n "
+                if len(predicates_environment) > 0
+                or len(predicates_agent) > 0
+                or len(predicates_agent_goal) > 0
+                or len(predicates_public_agent) > 0
+                else ""
+            )
+            out.write(
+                f" {nl.join(predicates_environment)}\n"
+                if len(predicates_environment) > 0
+                else ""
+            )
+            out.write(
+                f"  {nl.join(predicates_agent_goal)}\n"
+                if len(predicates_agent_goal) > 0
+                else ""
+            )
+            out.write(
+                f"  {nl.join(predicates_public_agent)}\n"
+                if len(predicates_public_agent) > 0
+                else ""
             )
 
-        em = self.problem.env.expression_manager
-        for a in self.problem.actions:
-            if isinstance(a, up.model.InstantaneousAction):
-                if em.FALSE() in a.preconditions:
-                    continue
-                out.write(f" (:action {self._get_mangled_name(a)}")
-                out.write(f"\n  :parameters (")
-                for ap in a.parameters:
-                    if ap.type.is_user_type():
-                        out.write(
-                            f" {self._get_mangled_name(ap)} - {self._get_mangled_name(ap.type)}"
-                        )
-                    else:
-                        raise UPTypeError("PDDL supports only user type parameters")
-                out.write(")")
-                if len(a.preconditions) > 0:
+            nl = "\n   "
+            out.write(
+                f"  (:private\n   {nl.join(predicates_agent)})"
+                if len(predicates_agent) > 0
+                else ""
+            )
+            out.write(
+                f")\n"
+                if len(predicates_environment) > 0
+                or len(predicates_agent) > 0
+                or len(predicates_agent_goal) > 0
+                or len(predicates_public_agent) > 0
+                else ""
+            )
+
+            out.write(
+                f" (:functions\n"
+                if len(functions_environment) > 0
+                or len(functions_agent) > 0
+                or len(functions_agent_goal) > 0
+                or len(functions_public_agent) > 0
+                else ""
+            )
+            out.write(
+                f' {" ".join(functions_environment)}\n'
+                if len(functions_environment) > 0
+                else ""
+            )
+            out.write(
+                f' {" ".join(functions_agent_goal)}\n'
+                if len(functions_agent_goal) > 0
+                else ""
+            )
+            out.write(
+                f' {" ".join(functions_public_agent)}\n'
+                if len(functions_public_agent) > 0
+                else ""
+            )
+            out.write(
+                f'  (:private{" ".join(functions_agent)})\n'
+                if len(functions_agent) > 0
+                else ""
+            )
+            out.write(
+                f" )\n"
+                if len(functions_environment) > 0
+                or len(functions_agent) > 0
+                or len(functions_agent_goal) > 0
+                or len(functions_public_agent) > 0
+                else ""
+            )
+
+            converter = ConverterToMAPDDLString(
+                self.problem.environment, self._get_mangled_name, ag
+            )
+            costs: dict = {}
+            for a in ag.actions:
+                if isinstance(a, up.model.InstantaneousAction):
+                    out.write(f" (:action {self._get_mangled_name(a)}")
+                    out.write(f"\n  :parameters (")
                     out.write(
-                        f'\n  :precondition (and {" ".join([converter.convert(p) for p in a.preconditions])})'
+                        f' ?{self._get_mangled_name(ag)} - {self._get_mangled_name(ag) +"_type"}'
                     )
-                if len(a.effects) > 0:
-                    out.write("\n  :effect (and")
-                    for e in a.effects:
-                        if e.is_conditional():
-                            out.write(f" (when {converter.convert(e.condition)}")
-                        if e.value.is_true():
-                            out.write(f" {converter.convert(e.fluent)}")
-                        elif e.value.is_false():
-                            out.write(f" (not {converter.convert(e.fluent)})")
-                        elif e.is_increase():
+                    for ap in a.parameters:
+                        if ap.type.is_user_type():
+                            out.write(
+                                f" {self._get_mangled_name(ap)} - {self._get_mangled_name(ap.type)}"
+                            )
+                        else:
+                            raise UPTypeError(
+                                "MA-PDDL supports only user type parameters"
+                            )
+                    out.write(")")
+                    if len(a.preconditions) > 0:
+                        out.write(f"\n  :precondition (and \n")
+                        for p in a.preconditions:
+                            out.write(f"   {converter.convert(p)}\n")
+                        out.write(f"  )")
+
+                    if len(a.effects) > 0:
+                        out.write("\n  :effect (and\n")
+                        for e in a.effects:
+                            _write_effect(
+                                e,
+                                None,
+                                out,
+                                converter,
+                                self.rewrite_bool_assignments,
+                            )
+
+                        if a in costs:
                             out.write(
-                                f" (increase {converter.convert(e.fluent)} {converter.convert(e.value)})"
+                                f"   (increase (total-cost) {converter.convert(costs[a])})"
                             )
-                        elif e.is_decrease():
+                        out.write(")")
+                    out.write(")\n")
+                elif isinstance(a, DurativeAction):
+                    out.write(f" (:durative-action {self._get_mangled_name(a)}")
+                    out.write(f"\n  :parameters (")
+                    for ap in a.parameters:
+                        if ap.type.is_user_type():
                             out.write(
-                                f" (decrease {converter.convert(e.fluent)} {converter.convert(e.value)})"
+                                f" {self._get_mangled_name(ap)} - {self._get_mangled_name(ap.type)}"
                             )
                         else:
+                            raise UPTypeError(
+                                "MA-PDDL supports only user type parameters"
+                            )
+                    out.write(")")
+                    l, r = a.duration.lower, a.duration.upper
+                    if l == r:
+                        out.write(f"\n  :duration (= ?duration {converter.convert(l)})")
+                    else:
+                        out.write(f"\n  :duration (and ")
+                        if a.duration.is_left_open():
+                            out.write(f"(> ?duration {converter.convert(l)})")
+                        else:
+                            out.write(f"(>= ?duration {converter.convert(l)})")
+                        if a.duration.is_right_open():
+                            out.write(f"(< ?duration {converter.convert(r)})")
+                        else:
+                            out.write(f"(<= ?duration {converter.convert(r)})")
+                        out.write(")")
+                    if len(a.conditions) > 0:
+                        out.write(f"\n  :condition (and ")
+                        for interval, cl in a.conditions.items():
+                            for c in cl:
+                                if interval.lower == interval.upper:
+                                    if interval.lower.is_from_start():
+                                        out.write(f"(at start {converter.convert(c)})")
+                                    else:
+                                        out.write(f"(at end {converter.convert(c)})")
+                                else:
+                                    if not interval.is_left_open():
+                                        out.write(f"(at start {converter.convert(c)})")
+                                    out.write(f"(over all {converter.convert(c)})")
+                                    if not interval.is_right_open():
+                                        out.write(f"(at end {converter.convert(c)})")
+                        out.write(")")
+                    if len(a.effects) > 0:
+                        out.write("\n  :effect (and")
+                        for t, el in a.effects.items():
+                            for e in el:
+                                _write_effect(
+                                    e,
+                                    t,
+                                    out,
+                                    converter,
+                                    self.rewrite_bool_assignments,
+                                )
+                        if a in costs:
                             out.write(
-                                f" (assign {converter.convert(e.fluent)} {converter.convert(e.value)})"
+                                f" (at end (increase (total-cost) {converter.convert(costs[a])}))"
                             )
-                        if e.is_conditional():
-                            out.write(f")")
+                        out.write(")")
+                    out.write(")\n")
+                else:
+                    raise NotImplementedError
+            out.write(")\n")
 
-                    if a in costs:
+            ag_domains[self._get_mangled_name(ag)] = out.getvalue()
+            out.close()
+            self.domain_objects = None
+            self.domain_objects_agents = {}
+            # self.all_public_fluents = []
+
+        return ag_domains
+
+    def _write_problem(self):
+        ag_problems = {}
+        for ag in self.problem.agents:
+            out = StringIO()
+            if self.problem.name is None:
+                name = "ma-pddl"
+            else:
+                name = _get_pddl_name(self.problem)
+            out.write(f"(define (problem {name}-problem)\n")
+            out.write(f" (:domain {name}-domain)\n")
+            if self.domain_objects is None:
+                # This method populates the self._domain_objects map
+                self._populate_domain_objects(ObjectsExtractor(), ag)
+            assert self.domain_objects is not None
+            if len(self.problem.user_types) > 0:
+                out.write(" (:objects")
+                for t in self.problem.user_types:
+                    constants_of_this_type = self.domain_objects.get(
+                        cast(_UserType, t), None
+                    )
+                    if constants_of_this_type is None:
+                        objects = [o for o in self.problem.all_objects if o.type == t]
+                    else:
+                        objects = [
+                            o
+                            for o in self.problem.all_objects
+                            if o.type == t and o not in constants_of_this_type
+                        ]
+                    if len(objects) > 0:
                         out.write(
-                            f" (increase (total-cost) {converter.convert(costs[a])})"
+                            f'\n   {" ".join([self._get_mangled_name(o) for o in objects])} - {self._get_mangled_name(t)}'
                         )
-                    out.write(")")
-                out.write(")\n")
-            elif isinstance(a, DurativeAction):
-                if any(em.FALSE() in cl for cl in a.conditions.values()):
-                    continue
-                out.write(f" (:durative-action {self._get_mangled_name(a)}")
-                out.write(f"\n  :parameters (")
-                for ap in a.parameters:
-                    if ap.type.is_user_type():
+
+            # If agents are not defined as "constant" in the domain, they are defined in the problem
+            if len(self.problem.agents) > 0:
+                for agent in self.problem.agents:
+                    if agent not in self.domain_objects_agents.keys():
                         out.write(
-                            f" {self._get_mangled_name(ap)} - {self._get_mangled_name(ap.type)}"
+                            f'\n   {self._get_mangled_name(agent)} - {self._get_mangled_name(agent) + "_type"}'
                         )
                     else:
-                        raise UPTypeError("PDDL supports only user type parameters")
-                out.write(")")
-                l, r = a.duration.lower, a.duration.upper
-                if l == r:
-                    out.write(f"\n  :duration (= ?duration {converter.convert(l)})")
-                else:
-                    out.write(f"\n  :duration (and ")
-                    if a.duration.is_left_open():
-                        out.write(f"(> ?duration {converter.convert(l)})")
-                    else:
-                        out.write(f"(>= ?duration {converter.convert(l)})")
-                    if a.duration.is_right_open():
-                        out.write(f"(< ?duration {converter.convert(r)})")
+                        out.write(f"")
+
+            out.write("\n )\n")
+            converter = ConverterToMAPDDLString(
+                self.problem.environment, self._get_mangled_name, ag
+            )
+            out.write(" (:init")
+
+            for f, v in self.problem.initial_values.items():
+                if v.is_true():
+                    if f.is_dot():
+                        fluent = f.args[0].fluent()
+                        args = f.args
+                        if (
+                            fluent in self.all_public_fluents
+                            or fluent in ag.fluents
+                            and f.agent().name == ag.name
+                        ):
+                            out.write(f"\n  {converter.convert(f)}")
+                        elif (
+                            f.agent().name != ag.name
+                            and fluent in self.all_public_fluents
+                        ):
+                            out.write(f"\n  {converter.convert(f)}")
+                        else:
+                            out.write(f"")
                     else:
-                        out.write(f"(<= ?duration {converter.convert(r)})")
-                    out.write(")")
-                if len(a.conditions) > 0:
-                    out.write(f"\n  :condition (and ")
-                    for interval, cl in a.conditions.items():
-                        for c in cl:
-                            if interval.lower == interval.upper:
-                                if interval.lower.is_from_start():
-                                    out.write(f"(at start {converter.convert(c)})")
-                                else:
-                                    out.write(f"(at end {converter.convert(c)})")
-                            else:
-                                if not interval.is_left_open():
-                                    out.write(f"(at start {converter.convert(c)})")
-                                out.write(f"(over all {converter.convert(c)})")
-                                if not interval.is_right_open():
-                                    out.write(f"(at end {converter.convert(c)})")
-                    out.write(")")
-                if len(a.effects) > 0:
-                    out.write("\n  :effect (and")
-                    for t, el in a.effects.items():
-                        for e in el:
-                            if t.is_from_start():
-                                out.write(f" (at start")
-                            else:
-                                out.write(f" (at end")
-                            if e.is_conditional():
-                                out.write(f" (when {converter.convert(e.condition)}")
-                            if e.value.is_true():
-                                out.write(f" {converter.convert(e.fluent)}")
-                            elif e.value.is_false():
-                                out.write(f" (not {converter.convert(e.fluent)})")
-                            elif e.is_increase():
-                                out.write(
-                                    f" (increase {converter.convert(e.fluent)} {converter.convert(e.value)})"
-                                )
-                            elif e.is_decrease():
-                                out.write(
-                                    f" (decrease {converter.convert(e.fluent)} {converter.convert(e.value)})"
-                                )
-                            else:
-                                out.write(
-                                    f" (assign {converter.convert(e.fluent)} {converter.convert(e.value)})"
-                                )
-                            if e.is_conditional():
-                                out.write(f")")
-                            out.write(")")
-                    if a in costs:
-                        out.write(
-                            f" (at end (increase (total-cost) {converter.convert(costs[a])}))"
-                        )
-                    out.write(")")
-                out.write(")\n")
-            else:
-                raise NotImplementedError
-        out.write(")\n")
+                        out.write(f"\n  {converter.convert(f)}")
+                elif v.is_false():
+                    pass
+                else:
+                    out.write(f"\n  (= {converter.convert(f)} {converter.convert(v)})")
+            if self.problem.kind.has_actions_cost():
+                out.write(f" (= (total-cost) 0)")
+            out.write(")\n")
+            out.write(f" (:goal (and")
+            for p in self.problem.goals:
+                out.write(f" {converter.convert(p)}")
+            out.write(f"))")
+            out.write("\n)")
+            ag_problems[self._get_mangled_name(ag)] = out.getvalue()
+            out.close()
+            self.domain_objects = None
+            self.domain_objects_agents = {}
+            # self.all_public_fluents = []
+        return ag_problems
+
+    def print_ma_domain_agent(self, agent_name):
+        """Prints to std output the `MA-PDDL` domain."""
+        domains = self._write_domain()
+        domain_agent = domains[agent_name]
+        sys.stdout.write(domain_agent)
+
+    def print_ma_problem_agent(self, agent_name):
+        """Prints to std output the `MA-PDDL` problem."""
+        problems = self._write_problem()
+        problem_agent = problems[agent_name]
+        sys.stdout.write(problem_agent)
+
+    def get_ma_domains(self) -> Dict:
+        """Returns the `MA-PDDL` domains."""
+        domains = self._write_domain()
+        return domains
+
+    def get_ma_domain_agent(self, agent_name) -> str:
+        """Returns the `MA-PDDL` agent domain."""
+        domains = self._write_domain()
+        domain_agent = domains[agent_name]
+        return domain_agent
+
+    def get_ma_problems(self) -> Dict:
+        """Returns the `MA-PDDL` problems."""
+        problems = self._write_problem()
+        return problems
+
+    def get_ma_problem_agent(self, agent_name) -> str:
+        """Returns the `MA-PDDL` agent problem."""
+        problems = self._write_problem()
+        problem_agent = problems[agent_name]
+        return problem_agent
+
+    def write_ma_domain(self, directory_name):
+        """Dumps to file the `MA-PDDL` domains."""
+        ag_domains = self._write_domain()
+        outdir_ma_pddl = "ma_pddl_" + directory_name
+        osy.makedirs(outdir_ma_pddl, exist_ok=True)
+        for ag, domain in ag_domains.items():
+            path_ma_pddl = osy.path.join(outdir_ma_pddl, ag + "_domain.pddl")
+            with open(path_ma_pddl, "w") as f:
+                f.write(domain)
+
+    def write_ma_problem(self, directory_name):
+        """Dumps to file the `MA-PDDL` problems."""
+        ag_problems = self._write_problem()
+        outdir_ma_pddl = "ma_pddl_" + directory_name
+        osy.makedirs(outdir_ma_pddl, exist_ok=True)
+        for ag, problem in ag_problems.items():
+            path_ma_pddl = osy.path.join(outdir_ma_pddl, ag + "_problem.pddl")
+            with open(path_ma_pddl, "w") as f:
+                f.write(problem)
 
-    def _write_problem(self, out: IO[str]):
-        if self.problem.name is None:
-            name = "pddl"
+    def get_predicates_functions(
+        self,
+        obj: Union[
+            up.model.multi_agent.Agent,
+            up.model.multi_agent.ma_environment.MAEnvironment,
+        ],
+        is_private: bool = False,
+    ):
+        if isinstance(obj, up.model.multi_agent.Agent):
+            fluents_list = obj.private_fluents if is_private else obj.public_fluents
+            prefix = "a_"
         else:
-            name = _get_pddl_name(self.problem)
-        out.write(f"(define (problem {name}-problem)\n")
-        out.write(f" (:domain {name}-domain)\n")
-        if self.domain_objects is None:
-            # This method populates the self._domain_objects map
-            self._populate_domain_objects(ObjectsExtractor())
-        assert self.domain_objects is not None
-        if len(self.problem.user_types) > 0:
-            out.write(" (:objects")
-            for t in self.problem.user_types:
-                constants_of_this_type = self.domain_objects.get(
-                    cast(_UserType, t), None
-                )
-                if constants_of_this_type is None:
-                    objects = [o for o in self.problem.all_objects if o.type == t]
-                else:
-                    objects = [
-                        o
-                        for o in self.problem.all_objects
-                        if o.type == t and o not in constants_of_this_type
-                    ]
-                if len(objects) > 0:
-                    out.write(
-                        f'\n   {" ".join([self._get_mangled_name(o) for o in objects])} - {self._get_mangled_name(t)}'
+            fluents_list = obj.fluents
+            prefix = ""
+        predicates = []
+        functions = []
+        for f in fluents_list:
+            params = []
+            i = 0
+            for param in f.signature:
+                if param.type.is_user_type():
+                    params.append(
+                        f" {self._get_mangled_name(param)} - {self._get_mangled_name(param.type)}"
                     )
-            out.write("\n )\n")
-        converter = ConverterToPDDLString(self.problem.env, self._get_mangled_name)
-        out.write(" (:init")
-        for f, v in self.problem.initial_values.items():
-            if v.is_true():
-                out.write(f" {converter.convert(f)}")
-            elif v.is_false():
-                pass
+                    i += 1
+                else:
+                    raise UPTypeError("MA-PDDL supports only user type parameters")
+            if isinstance(obj, up.model.multi_agent.Agent):
+                expression = f'({prefix}{self._get_mangled_name(f)} ?agent - {"ag"}{"".join(params)})'
             else:
-                out.write(f" (= {converter.convert(f)} {converter.convert(v)})")
-        if self.problem.kind.has_actions_cost():
-            out.write(f" (= (total-cost) 0)")
-        out.write(")\n")
-        out.write(
-            f' (:goal (and {" ".join([converter.convert(p) for p in self.problem.goals])}))\n'
-        )
-        if len(self.problem.trajectory_constraints) > 0:
-            out.write(
-                f' (:constraints {" ".join([converter.convert(c) for c in self.problem.trajectory_constraints])})\n'
-            )
-        metrics = self.problem.quality_metrics
-        if len(metrics) == 1:
-            metric = metrics[0]
-            out.write(" (:metric ")
-            if isinstance(metric, up.model.metrics.MinimizeExpressionOnFinalState):
-                out.write(f"minimize {converter.convert(metric.expression)}")
-            elif isinstance(metric, up.model.metrics.MaximizeExpressionOnFinalState):
-                out.write(f"maximize {converter.convert(metric.expression)}")
-            elif isinstance(metric, up.model.metrics.MinimizeActionCosts) or isinstance(
-                metric, up.model.metrics.MinimizeSequentialPlanLength
-            ):
-                out.write(f"minimize (total-cost)")
-            elif isinstance(metric, up.model.metrics.MinimizeMakespan):
-                out.write(f"minimize (total-time)")
+                expression = f'({prefix}{self._get_mangled_name(f)}{"".join(params)})'
+            if f.type.is_bool_type():
+                predicates.append(expression)
+            elif f.type.is_int_type() or f.type.is_real_type():
+                functions.append(expression)
             else:
-                raise NotImplementedError
-            out.write(")\n")
-        elif len(metrics) > 1:
-            raise up.exceptions.UPUnsupportedProblemTypeError(
-                "Only one metric is supported!"
-            )
-        out.write(")\n")
-
-    def print_domain(self):
-        """Prints to std output the `PDDL` domain."""
-        self._write_domain(sys.stdout)
-
-    def print_problem(self):
-        """Prints to std output the `PDDL` problem."""
-        self._write_problem(sys.stdout)
-
-    def get_domain(self) -> str:
-        """Returns the `PDDL` domain."""
-        out = StringIO()
-        self._write_domain(out)
-        return out.getvalue()
-
-    def get_problem(self) -> str:
-        """Returns the `PDDL` problem."""
-        out = StringIO()
-        self._write_problem(out)
-        return out.getvalue()
-
-    def write_domain(self, filename: str):
-        """Dumps to file the `PDDL` domain."""
-        with open(filename, "w") as f:
-            self._write_domain(f)
-
-    def write_problem(self, filename: str):
-        """Dumps to file the `PDDL` problem."""
-        with open(filename, "w") as f:
-            self._write_problem(f)
+                raise UPTypeError("MA-PDDL supports only boolean and numerical fluents")
+        return predicates, functions
 
     def _get_mangled_name(
         self,
         item: Union[
             "up.model.Type",
             "up.model.Action",
             "up.model.Fluent",
             "up.model.Object",
             "up.model.Parameter",
             "up.model.Variable",
+            "up.model.multi_agent.Agent",
         ],
     ) -> str:
-        """This function returns a valid and unique PDDL name."""
+        """This function returns a valid and unique MA-PDDL name."""
 
         # If we already encountered this item, return it
         if item in self.otn_renamings:
             return self.otn_renamings[item]
 
         if isinstance(item, up.model.Type):
             assert item.is_user_type()
@@ -758,15 +731,15 @@
             tmp_name = _get_pddl_name(item)
             # If the problem is hierarchical and the name is object, we want to change it
             if self.problem_kind.has_hierarchical_typing() and tmp_name == "object":
                 tmp_name = f"{tmp_name}_"
         else:
             original_name = item.name
             tmp_name = _get_pddl_name(item)
-        # if the pddl valid name is the same of the original one and it does not create conflicts,
+        # if the ma-pddl valid name is the same of the original one and it does not create conflicts,
         # it can be returned
         if tmp_name == original_name and tmp_name not in self.nto_renamings:
             new_name = tmp_name
         else:
             count = 0
             new_name = tmp_name
             while self.problem.has_name(new_name) or new_name in self.nto_renamings:
@@ -774,89 +747,109 @@
                 count += 1
         assert (
             new_name not in self.nto_renamings
             and new_name not in self.otn_renamings.values()
         )
         self.otn_renamings[item] = new_name
         self.nto_renamings[new_name] = item
+
         return new_name
 
     def get_item_named(
         self, name: str
     ) -> Union[
         "up.model.Type",
         "up.model.Action",
         "up.model.Fluent",
         "up.model.Object",
         "up.model.Parameter",
         "up.model.Variable",
+        "up.model.multi_agent.Agent",
     ]:
         """
-        Since `PDDL` has a stricter set of possible naming compared to the `unified_planning`, when writing
-        a :class:`~unified_planning.model.Problem` it is possible that some things must be renamed. This is why the `PDDLWriter`
-        offers this method, that takes a `PDDL` name and returns the original `unified_planning` data structure that corresponds
-        to the `PDDL` entity with the given name.
+        Since `MA-PDDL` has a stricter set of possible naming compared to the `unified_planning`, when writing
+        a :class:`~unified_planning.model.Problem` it is possible that some things must be renamed. This is why the `MAPDDLWriter`
+        offers this method, that takes a `MA-PDDL` name and returns the original `unified_planning` data structure that corresponds
+        to the `MA-PDDL` entity with the given name.
 
-        This method takes a name used in the `PDDL` domain or `PDDL` problem generated by this `PDDLWriter` and returns the original
+        This method takes a name used in the `MA-PDDL` domain or `MA-PDDL` problem generated by this `MAPDDLWriter` and returns the original
         item in the `unified_planning` `Problem`.
 
-        :param name: The name used in the generated `PDDL`.
+        :param name: The name used in the generated `MA-PDDL`.
         :return: The `unified_planning` model entity corresponding to the given name.
         """
         try:
             return self.nto_renamings[name]
         except KeyError:
             raise UPException(f"The name {name} does not correspond to any item.")
 
-    def get_pddl_name(
+    def get_ma_pddl_name(
         self,
         item: Union[
             "up.model.Type",
             "up.model.Action",
             "up.model.Fluent",
             "up.model.Object",
             "up.model.Parameter",
             "up.model.Variable",
         ],
     ) -> str:
         """
-        This method takes an item in the :class:`~unified_planning.model.Problem` and returns the chosen name for the same item in the `PDDL` problem
-        or `PDDL` domain generated by this `PDDLWriter`.
+        This method takes an item in the :class:`~unified_planning.model.MultiAgentProblem` and returns the chosen name for the same item in the `MA-PDDL` problem
+        or `MA-PDDL` domain generated by this `MAPDDLWriter`.
 
-        :param item: The `unified_planning` entity renamed by this `PDDLWriter`.
-        :return: The `PDDL` name of the given item.
+        :param item: The `unified_planning` entity renamed by this `MAPDDLWriter`.
+        :return: The `MA-PDDL` name of the given item.
         """
         try:
             return self.otn_renamings[item]
         except KeyError:
             raise UPException(
                 f"The item {item} does not correspond to any item renamed."
             )
 
-    def _populate_domain_objects(self, obe: ObjectsExtractor):
+    def _all_public_fluents(
+        self,
+        list_to_update: Set[Fluent],
+        agents: List[up.model.multi_agent.Agent],
+    ) -> None:
+        """This function creates a list with all public fluents of all agents."""
+        for agent in agents:
+            for fluent in agent.public_fluents:
+                list_to_update.add(fluent)
+
+    def _populate_domain_objects(
+        self, obe: ObjectsExtractor, agent: "up.model.multi_agent.Agent"
+    ):
         self.domain_objects = {}
+        self.domain_objects_agents = {}
         # Iterate the actions to retrieve domain objects
-        for a in self.problem.actions:
+        import unified_planning.model.walkers as walkers
+
+        get_dots = walkers.AnyGetter(lambda x: x.is_dot())
+        for a in agent.actions:
             if isinstance(a, up.model.InstantaneousAction):
                 for p in a.preconditions:
+                    for d in get_dots.get(p):
+                        _update_domain_objects_ag(self.domain_objects_agents, d.agent())
                     _update_domain_objects(self.domain_objects, obe.get(p))
                 for e in a.effects:
                     if e.is_conditional():
                         _update_domain_objects(
                             self.domain_objects, obe.get(e.condition)
                         )
                     _update_domain_objects(self.domain_objects, obe.get(e.fluent))
                     _update_domain_objects(self.domain_objects, obe.get(e.value))
             elif isinstance(a, DurativeAction):
                 _update_domain_objects(self.domain_objects, obe.get(a.duration.lower))
                 _update_domain_objects(self.domain_objects, obe.get(a.duration.upper))
-                for interval, cl in a.conditions.items():
+                for cl in a.conditions.values():
                     for c in cl:
                         _update_domain_objects(self.domain_objects, obe.get(c))
-                for t, el in a.effects.items():
+                for el in a.effects.values():
                     for e in el:
                         if e.is_conditional():
                             _update_domain_objects(
                                 self.domain_objects, obe.get(e.condition)
                             )
                         _update_domain_objects(self.domain_objects, obe.get(e.fluent))
                         _update_domain_objects(self.domain_objects, obe.get(e.value))
@@ -867,17 +860,19 @@
         "up.model.Type",
         "up.model.Action",
         "up.model.Fluent",
         "up.model.Object",
         "up.model.Parameter",
         "up.model.Variable",
         "up.model.Problem",
+        "up.model.multi_agent.MultiAgentProblem",
+        "up.model.multi_agent.Agent",
     ]
 ) -> str:
-    """This function returns a pddl name for the chosen item"""
+    """This function returns a ma-pddl name for the chosen item"""
     name = item.name  # type: ignore
     assert name is not None
     name = name.lower()
     regex = re.compile(r"^[a-zA-Z]+.*")
     if (
         re.match(regex, name) is None
     ):  # If the name does not start with an alphabetic char, we make it start with one.
@@ -896,7 +891,15 @@
 def _update_domain_objects(
     dict_to_update: Dict[_UserType, Set[Object]], values: Dict[_UserType, Set[Object]]
 ) -> None:
     """Small utility method that updated a UserType -> Set[Object] dict with another dict of the same type."""
     for ut, os in values.items():
         os_to_update = dict_to_update.setdefault(ut, set())
         os_to_update |= os
+
+
+def _update_domain_objects_ag(
+    dict_to_update: Dict["up.model.multi_agent.Agent", str],
+    agent: up.model.multi_agent.Agent,
+) -> None:
+    """Small utility method that updated the dict domain_objects_agents."""
+    dict_to_update.setdefault(agent, agent.name + "_type")
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/io/python_writer.py` & `unified_planning-0.6.0/unified_planning/io/python_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from io import StringIO
 
 
 class ConverterToPythonString(walkers.DagWalker):
     """Expression converter to a Python string."""
 
     def __init__(
-        self, env: "up.environment.Environment", names_mapping: Dict[str, str]
+        self, environment: "up.environment.Environment", names_mapping: Dict[str, str]
     ):
         walkers.DagWalker.__init__(self)
         self._names_mapping = names_mapping
 
     def convert(self, expression):
         """Converts the given expression to a python command."""
         if expression is None:
@@ -86,15 +86,15 @@
         if args:
             return f'{_get_mangled_name(f"fluent_{fluent.name}", self._names_mapping)}({", ".join(args)})'
         return f'emgr.FluentExp({_get_mangled_name(f"fluent_{fluent.name}", self._names_mapping)})'
 
     def walk_param_exp(self, expression, args):
         assert len(args) == 0
         p = expression.parameter()
-        return f'emgr.ParameterExp(up.model.Parameter("{p.name}", {_print_python_type(p.type, self._names_mapping)}, env))'
+        return f'emgr.ParameterExp(up.model.Parameter("{p.name}", {_print_python_type(p.type, self._names_mapping)}, environment))'
 
     def walk_object_exp(self, expression, args):
         assert len(args) == 0
         o = expression.object()
         return f'emgr.ObjectExp({_get_mangled_name(f"object_{o.name}", self._names_mapping)})'
 
     def walk_timing_exp(self, expression, args):
@@ -181,21 +181,21 @@
             if object_var_name.isidentifier():
                 names_mapping[object_var_name] = object_var_name
         for action in self.problem.actions:
             action_var_name = f"act_{action.name}"
             if action_var_name.isidentifier():
                 names_mapping[action_var_name] = action_var_name
 
-        converter = ConverterToPythonString(self.problem.env, names_mapping)
+        converter = ConverterToPythonString(self.problem.environment, names_mapping)
         out.write("from fractions import Fraction\n")
         out.write("from collections import OrderedDict\n")
         out.write("import unified_planning as up\n")
-        out.write("env = up.environment.get_env()\n")
-        out.write("emgr = env.expression_manager\n")
-        out.write("tm = env.type_manager\n")
+        out.write("environment = up.environment.get_environment()\n")
+        out.write("emgr = environment.expression_manager\n")
+        out.write("tm = environment.type_manager\n")
 
         for type in self.problem.user_types:  # define user_types
             utype = cast(_UserType, type)
             if utype.father is None:
                 out.write(
                     f'{_get_mangled_name(f"type_{utype.name}", names_mapping)} = tm.UserType("{utype.name}")\n'
                 )
@@ -229,15 +229,15 @@
             problem_class = "htn.HierarchicalProblem"
         else:
             problem_class = "Problem"
         problem_name = (
             f'"{self.problem.name}"' if self.problem.name is not None else "None"
         )
         out.write(
-            f"problem = up.model.{problem_class}({problem_name}, env, initial_defaults=problem_initial_defaults)\n"
+            f"problem = up.model.{problem_class}({problem_name}, environment, initial_defaults=problem_initial_defaults)\n"
         )
 
         for o in self.problem.all_objects:  # add objects to the problem
             out.write(
                 f'problem.add_object({_get_mangled_name(f"object_{o.name}", names_mapping)})\n'
             )
 
@@ -349,39 +349,54 @@
                     f"problem.add_timed_goal(interval={_convert_interval(i)}, goal={converter.convert(g)})\n"
                 )
 
         for g in self.problem.goals:  # add goals
             out.write(f"problem.add_goal(goal={converter.convert(g)})\n")
 
         for qm in self.problem.quality_metrics:  # adding metrics
-            if isinstance(qm, up.model.metrics.MinimizeActionCosts):
+            if qm.is_minimize_action_costs():
+                assert isinstance(qm, up.model.metrics.MinimizeActionCosts)
                 out.write("costs = {}\n")
                 for a, ac in qm.costs.items():
                     out.write(f"costs[act_{a.name}] = {converter.convert(ac)}\n")
-            elif isinstance(qm, up.model.metrics.Oversubscription):
+            elif qm.is_oversubscription():
+                assert isinstance(qm, up.model.metrics.Oversubscription)
                 out.write("goals = {}\n")
                 for goal, cost in qm.goals.items():
                     out.write(f"goals[{converter.convert(goal)}] = {cost}\n")
+            elif qm.is_temporal_oversubscription():
+                assert isinstance(qm, up.model.metrics.TemporalOversubscription)
+                out.write("goals = {}\n")
+                for (i, goal), cost in qm.goals.items():
+                    out.write(
+                        f"goals[({_convert_interval(i)}, {converter.convert(goal)})] = {cost}\n"
+                    )
             out.write("problem.add_quality_metric(")
-            if isinstance(qm, up.model.metrics.MinimizeActionCosts):
+            if qm.is_minimize_action_costs():
+                assert isinstance(qm, up.model.metrics.MinimizeActionCosts)
                 out.write(f"up.model.metrics.MinimizeActionCosts(costs, {qm.default})")
-            elif isinstance(qm, up.model.metrics.MinimizeSequentialPlanLength):
+            elif qm.is_minimize_sequential_plan_length():
                 out.write("up.model.metrics.MinimizeSequentialPlanLength()")
-            elif isinstance(qm, up.model.metrics.MinimizeMakespan):
+            elif qm.is_minimize_makespan():
                 out.write("up.model.metrics.MinimizeMakespan()")
-            elif isinstance(qm, up.model.metrics.MinimizeExpressionOnFinalState):
+            elif qm.is_minimize_expression_on_final_state():
+                assert isinstance(qm, up.model.metrics.MinimizeExpressionOnFinalState)
                 out.write(
                     f"up.model.metrics.MinimizeExpressionOnFinalState({converter.convert(qm.expression)})"
                 )
-            elif isinstance(qm, up.model.metrics.MaximizeExpressionOnFinalState):
+            elif qm.is_maximize_expression_on_final_state():
+                assert isinstance(qm, up.model.metrics.MaximizeExpressionOnFinalState)
                 out.write(
                     f"up.model.metrics.MaximizeExpressionOnFinalState({converter.convert(qm.expression)})"
                 )
-            elif isinstance(qm, up.model.metrics.Oversubscription):
+            elif qm.is_oversubscription():
                 out.write("up.model.metrics.Oversubscription(goals)")
+            elif qm.is_temporal_oversubscription():
+                assert isinstance(qm, up.model.metrics.TemporalOversubscription)
+                out.write("up.model.metrics.TemporalOversubscription(goals)")
             else:
                 raise NotImplementedError
             out.write(")\n")
 
         if self.problem.kind.has_hierarchical():
             assert isinstance(
                 self.problem, up.model.htn.hierarchical_problem.HierarchicalProblem
@@ -530,21 +545,21 @@
 
     tp = timing.timepoint
     if timing.is_global():
         assert tp.container is None
         if timing.is_from_start():
             return f"up.model.GlobalStartTiming({delay})"
         else:
-            return f"up.model.GlobalEndTiming({delay})"
+            return f"up.model.GlobalEndTiming() + {delay}"
     else:
         container = f'"{tp.container}"' if tp.container is not None else "None"
         if timing.is_from_start():
             return f"up.model.StartTiming({delay}, container={container})"
         else:
-            return f"up.model.EndTiming({delay}, container={container})"
+            return f"up.model.EndTiming(container={container}) + {delay}"
 
 
 def _convert_interval(interval: up.model.TimeInterval) -> str:
     interval_feature: str = "up.model.ClosedTimeInterval"
     if interval.is_left_open() and interval.is_right_open():
         interval_feature = "up.model.OpenTimeInterval"
     elif interval.is_left_open() and not interval.is_right_open():
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/__init__.py` & `unified_planning-0.6.0/unified_planning/model/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,29 @@
     DurativeAction,
     SensingAction,
 )
 from unified_planning.model.effect import Effect, SimulatedEffect, EffectKind
 from unified_planning.model.expression import (
     BoolExpression,
     Expression,
+    NumericConstant,
+    NumericExpression,
     ExpressionManager,
 )
 from unified_planning.model.fnode import FNode
 from unified_planning.model.fluent import Fluent
 from unified_planning.model.object import Object
 from unified_planning.model.operators import OperatorKind
 from unified_planning.model.parameter import Parameter
 from unified_planning.model.abstract_problem import AbstractProblem
 from unified_planning.model.problem import Problem
 from unified_planning.model.contingent_problem import ContingentProblem
+from unified_planning.model.delta_stn import DeltaSimpleTemporalNetwork
 from unified_planning.model.problem_kind import ProblemKind
-from unified_planning.model.state import ROState, COWState, UPCOWState
+from unified_planning.model.state import State, UPState
 from unified_planning.model.timing import (
     Timepoint,
     TimepointKind,
     Timing,
     StartTiming,
     EndTiming,
     GlobalStartTiming,
@@ -57,48 +60,51 @@
     TimeInterval,
     TimePointInterval,
     ClosedTimeInterval,
     OpenTimeInterval,
     LeftOpenTimeInterval,
     RightOpenTimeInterval,
 )
-from unified_planning.model.types import Type, TypeManager
+from unified_planning.model.types import Type
 from unified_planning.model.variable import Variable, FreeVarsOracle
 from unified_planning.model.metrics import (
     PlanQualityMetric,
     MinimizeActionCosts,
     MinimizeSequentialPlanLength,
     MinimizeMakespan,
     MinimizeExpressionOnFinalState,
     MaximizeExpressionOnFinalState,
     Oversubscription,
+    TemporalOversubscription,
 )
 import unified_planning.model.multi_agent
+import unified_planning.model.scheduling
 
 __all__ = [
     "Action",
     "InstantaneousAction",
     "DurativeAction",
     "Effect",
     "SimulatedEffect",
     "EffectKind",
     "BoolExpression",
     "Expression",
+    "NumericConstant",
+    "NumericExpression",
     "ExpressionManager",
     "FNode",
     "Fluent",
     "Object",
     "OperatorKind",
     "Parameter",
     "AbstractProblem",
     "Problem",
     "ProblemKind",
-    "ROState",
-    "COWState",
-    "UPCOWState",
+    "State",
+    "UPState",
     "Timepoint",
     "TimepointKind",
     "Timing",
     "StartTiming",
     "EndTiming",
     "GlobalStartTiming",
     "GlobalEndTiming",
@@ -111,18 +117,19 @@
     "TimeInterval",
     "TimePointInterval",
     "ClosedTimeInterval",
     "OpenTimeInterval",
     "LeftOpenTimeInterval",
     "RightOpenTimeInterval",
     "Type",
-    "TypeManager",
     "Variable",
     "FreeVarsOracle",
     "PlanQualityMetric",
     "MinimizeActionCosts",
     "MinimizeSequentialPlanLength",
     "MinimizeMakespan",
     "MinimizeExpressionOnFinalState",
     "MaximizeExpressionOnFinalState",
     "Oversubscription",
+    "TemporalOversubscription",
+    "DeltaSimpleTemporalNetwork",
 ]
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/abstract_problem.py` & `unified_planning-0.6.0/unified_planning/model/abstract_problem.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,66 +11,71 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines an abstract problem class."""
 
 import unified_planning as up
+from abc import ABC, abstractmethod
 from typing import Optional
 
 
-class AbstractProblem:
+class AbstractProblem(ABC):
     """
     This is an abstract class that represents a generic `planning problem`.
 
     Together with the `unified_planning.model.mixins` classes it defines the most common
     functionalities of `planning problems`.
     """
 
     def __init__(
         self,
         name: Optional[str] = None,
-        env: Optional["up.environment.Environment"] = None,
+        environment: Optional["up.environment.Environment"] = None,
     ):
-        self._env = up.environment.get_env(env)
+        self._env = up.environment.get_environment(environment)
         self._name = name
 
     @property
-    def env(self) -> "up.environment.Environment":
+    def environment(self) -> "up.environment.Environment":
         """Returns the `Problem` `Environment`."""
         return self._env
 
     @property
     def name(self) -> Optional[str]:
         """Returns the `Problem` `name`."""
         return self._name
 
     @name.setter
     def name(self, new_name: str):
         """Sets the `Problem` `name`."""
         self._name = new_name
 
+    @abstractmethod
     def clone(self):
         raise NotImplementedError
 
     @property
+    @abstractmethod
     def kind(self) -> "up.model.problem_kind.ProblemKind":
         """Returns the :class:`~unified_planning.model.ProblemKind` of this `Problem`."""
         raise NotImplementedError
 
+    @abstractmethod
     def has_name(self, name: str) -> bool:
         """
         Returns `True` the given `name` is already used inside this `Problem`,
         `False` otherwise.
 
         :param name: The target `name` to search in the `Problem`.
         :return: `True` if the `name` is already used in the `Problem`, `False` otherwise.
         """
         raise NotImplementedError
 
+    @abstractmethod
     def normalize_plan(self, plan: "up.plans.Plan") -> "up.plans.Plan":
         """
         Normalizes the given `Plan`, that is potentially the result of another
         `Problem`, updating the `Object` references in the `Plan` with the ones of
         this `Problem` which are syntactically equal.
 
         :param plan: The `Plan` that must be normalized.
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/action.py` & `unified_planning-0.6.0/unified_planning/model/action.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,68 +16,76 @@
 This module defines the `Action` base class and some of his extensions.
 An `Action` has a `name`, a `list` of `Parameter`, a `list` of `preconditions`
 and a `list` of `effects`.
 """
 
 
 import unified_planning as up
-from unified_planning.environment import get_env, Environment
+from unified_planning.environment import get_environment, Environment
 from unified_planning.exceptions import (
     UPTypeError,
     UPUnboundedVariablesError,
     UPProblemDefinitionError,
-    UPConflictingEffectsException,
+    UPUsageError,
 )
-from fractions import Fraction
-from typing import Dict, List, Set, Tuple, Union, Optional
+from unified_planning.model.mixins.timed_conds_effs import TimedCondsEffs
+from abc import ABC, abstractmethod
+from typing import Dict, List, Set, Union, Optional, Iterable
 from collections import OrderedDict
 
 
-class Action:
+class Action(ABC):
     """This is the `Action` interface."""
 
     def __init__(
         self,
         _name: str,
         _parameters: Optional["OrderedDict[str, up.model.types.Type]"] = None,
         _env: Optional[Environment] = None,
         **kwargs: "up.model.types.Type",
     ):
-        self._env = get_env(_env)
+        self._environment = get_environment(_env)
         self._name = _name
         self._parameters: "OrderedDict[str, up.model.parameter.Parameter]" = (
             OrderedDict()
         )
         if _parameters is not None:
             assert len(kwargs) == 0
             for n, t in _parameters.items():
-                assert self._env.type_manager.has_type(
+                assert self._environment.type_manager.has_type(
                     t
                 ), "type of parameter does not belong to the same environment of the action"
-                self._parameters[n] = up.model.parameter.Parameter(n, t, self._env)
+                self._parameters[n] = up.model.parameter.Parameter(
+                    n, t, self._environment
+                )
         else:
             for n, t in kwargs.items():
-                assert self._env.type_manager.has_type(
+                assert self._environment.type_manager.has_type(
                     t
                 ), "type of parameter does not belong to the same environment of the action"
-                self._parameters[n] = up.model.parameter.Parameter(n, t, self._env)
+                self._parameters[n] = up.model.parameter.Parameter(
+                    n, t, self._environment
+                )
 
+    @abstractmethod
     def __eq__(self, oth: object) -> bool:
         raise NotImplementedError
 
+    @abstractmethod
     def __hash__(self) -> int:
         raise NotImplementedError
 
+    @abstractmethod
     def clone(self):
         raise NotImplementedError
 
     @property
-    def env(self) -> Environment:
+    def environment(self) -> Environment:
         """Returns this `Action` `Environment`."""
-        return self._env
+        return self._environment
 
     @property
     def name(self) -> str:
         """Returns the `Action` `name`."""
         return self._name
 
     @name.setter
@@ -90,19 +98,49 @@
         """Returns the `list` of the `Action parameters`."""
         return list(self._parameters.values())
 
     def parameter(self, name: str) -> "up.model.parameter.Parameter":
         """
         Returns the `parameter` of the `Action` with the given `name`.
 
+        Example
+        -------
+        >>> from unified_planning.shortcuts import *
+        >>> location_type = UserType("Location")
+        >>> move = InstantaneousAction("move", source=location_type, target=location_type)
+        >>> move.parameter("source")  # return the "source" parameter of the action, with type "Location"
+        Location source
+        >>> move.parameter("target")
+        Location target
+
+        If a parameter's name (1) does not conflict with an existing attribute of `Action` and (2) does not start with '_'
+        it can also be accessed as if it was an attribute of the action. For instance:
+
+        >>> move.source
+        Location source
+
         :param name: The `name` of the target `parameter`.
         :return: The `parameter` of the `Action` with the given `name`.
         """
+        if name not in self._parameters:
+            raise ValueError(f"Action '{self.name}' has no parameter '{name}'")
         return self._parameters[name]
 
+    def __getattr__(self, parameter_name: str) -> "up.model.parameter.Parameter":
+        if parameter_name.startswith("_"):
+            # guard access as pickling relies on attribute error to be thrown even when
+            # no attributes of the object have been set.
+            # In this case accessing `self._name` or `self._parameters`, would re-invoke __getattr__
+            raise AttributeError(f"Action has no attribute '{parameter_name}'")
+        if parameter_name not in self._parameters:
+            raise AttributeError(
+                f"Action '{self.name}' has no attribute or parameter '{parameter_name}'"
+            )
+        return self._parameters[parameter_name]
+
     def is_conditional(self) -> bool:
         """Returns `True` if the `Action` has `conditional effects`, `False` otherwise."""
         raise NotImplementedError
 
 
 class InstantaneousAction(Action):
     """Represents an instantaneous action."""
@@ -114,16 +152,18 @@
         _env: Optional[Environment] = None,
         **kwargs: "up.model.types.Type",
     ):
         Action.__init__(self, _name, _parameters, _env, **kwargs)
         self._preconditions: List["up.model.fnode.FNode"] = []
         self._effects: List[up.model.effect.Effect] = []
         self._simulated_effect: Optional[up.model.effect.SimulatedEffect] = None
-        # fluent assigned is the set of the fluent that have an unconditional assignment
-        self._fluents_assigned: Set["up.model.fnode.FNode"] = set()
+        # fluent assigned is the mapping of the fluent to it's value if it is an unconditional assignment
+        self._fluents_assigned: Dict[
+            "up.model.fnode.FNode", "up.model.fnode.FNode"
+        ] = {}
         # fluent_inc_dec is the set of the fluents that have an unconditional increase or decrease
         self._fluents_inc_dec: Set["up.model.fnode.FNode"] = set()
 
     def __repr__(self) -> str:
         s = []
         s.append(f"action {self.name}")
         first = True
@@ -141,22 +181,23 @@
         for c in self.preconditions:
             s.append(f"      {str(c)}\n")
         s.append("    ]\n")
         s.append("    effects = [\n")
         for e in self.effects:
             s.append(f"      {str(e)}\n")
         s.append("    ]\n")
-        s.append(f"    simulated effect = {self._simulated_effect}\n")
+        if self._simulated_effect is not None:
+            s.append(f"    simulated effect = {self._simulated_effect}\n")
         s.append("  }")
         return "".join(s)
 
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, InstantaneousAction):
             cond = (
-                self._env == oth._env
+                self._environment == oth._environment
                 and self._name == oth._name
                 and self._parameters == oth._parameters
             )
             return (
                 cond
                 and set(self._preconditions) == set(oth._preconditions)
                 and set(self._effects) == set(oth._effects)
@@ -177,15 +218,15 @@
         return res
 
     def clone(self):
         new_params = OrderedDict(
             (param_name, param.type) for param_name, param in self._parameters.items()
         )
         new_instantaneous_action = InstantaneousAction(
-            self._name, new_params, self._env
+            self._name, new_params, self._environment
         )
         new_instantaneous_action._preconditions = self._preconditions[:]
         new_instantaneous_action._effects = [e.clone() for e in self._effects]
         new_instantaneous_action._fluents_assigned = self._fluents_assigned.copy()
         new_instantaneous_action._fluents_inc_dec = self._fluents_inc_dec.copy()
         new_instantaneous_action._simulated_effect = self._simulated_effect
         return new_instantaneous_action
@@ -203,16 +244,17 @@
     def effects(self) -> List["up.model.effect.Effect"]:
         """Returns the `list` of the `Action effects`."""
         return self._effects
 
     def clear_effects(self):
         """Removes all the `Action's effects`."""
         self._effects = []
-        self._fluents_assigned = set()
+        self._fluents_assigned = {}
         self._fluents_inc_dec = set()
+        self._simulated_effect = None
 
     @property
     def conditional_effects(self) -> List["up.model.effect.Effect"]:
         """Returns the `list` of the `action conditional effects`.
 
         IMPORTANT NOTE: this property does some computation, so it should be called as
         seldom as possible."""
@@ -240,19 +282,23 @@
         ],
     ):
         """
         Adds the given expression to `action's preconditions`.
 
         :param precondition: The expression that must be added to the `action's preconditions`.
         """
-        (precondition_exp,) = self._env.expression_manager.auto_promote(precondition)
-        assert self._env.type_checker.get_type(precondition_exp).is_bool_type()
-        if precondition_exp == self._env.expression_manager.TRUE():
+        (precondition_exp,) = self._environment.expression_manager.auto_promote(
+            precondition
+        )
+        assert self._environment.type_checker.get_type(precondition_exp).is_bool_type()
+        if precondition_exp == self._environment.expression_manager.TRUE():
             return
-        free_vars = self._env.free_vars_oracle.get_free_variables(precondition_exp)
+        free_vars = self._environment.free_vars_oracle.get_free_variables(
+            precondition_exp
+        )
         if len(free_vars) != 0:
             raise UPUnboundedVariablesError(
                 f"The precondition {str(precondition_exp)} has unbounded variables:\n{str(free_vars)}"
             )
         if precondition_exp not in self._preconditions:
             self._preconditions.append(precondition_exp)
 
@@ -270,20 +316,26 @@
         :param condition: The `condition` in which this `effect` is applied; the default
             value is `True`.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
-        ) = self._env.expression_manager.auto_promote(fluent, value, condition)
-        assert fluent_exp.is_fluent_exp()
-        if not self._env.type_checker.get_type(condition_exp).is_bool_type():
+        ) = self._environment.expression_manager.auto_promote(fluent, value, condition)
+        if not fluent_exp.is_fluent_exp():
+            raise UPUsageError(
+                "fluent field of add_effect must be a Fluent or a FluentExp"
+            )
+        if not self._environment.type_checker.get_type(condition_exp).is_bool_type():
             raise UPTypeError("Effect condition is not a Boolean condition!")
         if not fluent_exp.type.is_compatible(value_exp.type):
-            raise UPTypeError("InstantaneousAction effect has not compatible types!")
+            # Value is not assignable to fluent (its type is not a subset of the fluent's type).
+            raise UPTypeError(
+                f"InstantaneousAction effect has an incompatible value type. Fluent type: {fluent_exp.type} // Value type: {value_exp.type}"
+            )
         self._add_effect_instance(
             up.model.effect.Effect(fluent_exp, value_exp, condition_exp)
         )
 
     def add_increase_effect(
         self,
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
@@ -298,20 +350,25 @@
         :param condition: The `condition` in which this `effect` is applied; the default
             value is `True`.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
-        ) = self._env.expression_manager.auto_promote(fluent, value, condition)
-        assert fluent_exp.is_fluent_exp()
+        ) = self._environment.expression_manager.auto_promote(fluent, value, condition)
+        if not fluent_exp.is_fluent_exp():
+            raise UPUsageError(
+                "fluent field of add_increase_effect must be a Fluent or a FluentExp"
+            )
         if not condition_exp.type.is_bool_type():
             raise UPTypeError("Effect condition is not a Boolean condition!")
         if not fluent_exp.type.is_compatible(value_exp.type):
-            raise UPTypeError("InstantaneousAction effect has not compatible types!")
+            raise UPTypeError(
+                f"InstantaneousAction effect has an incompatible value type. Fluent type: {fluent_exp.type} // Value type: {value_exp.type}"
+            )
         if not fluent_exp.type.is_int_type() and not fluent_exp.type.is_real_type():
             raise UPTypeError("Increase effects can be created only on numeric types!")
         self._add_effect_instance(
             up.model.effect.Effect(
                 fluent_exp,
                 value_exp,
                 condition_exp,
@@ -333,114 +390,94 @@
         :param condition: The `condition` in which this `effect` is applied; the default
             value is `True`.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
-        ) = self._env.expression_manager.auto_promote(fluent, value, condition)
-        assert fluent_exp.is_fluent_exp()
+        ) = self._environment.expression_manager.auto_promote(fluent, value, condition)
+        if not fluent_exp.is_fluent_exp():
+            raise UPUsageError(
+                "fluent field of add_decrease_effect must be a Fluent or a FluentExp"
+            )
         if not condition_exp.type.is_bool_type():
             raise UPTypeError("Effect condition is not a Boolean condition!")
         if not fluent_exp.type.is_compatible(value_exp.type):
-            raise UPTypeError("InstantaneousAction effect has not compatible types!")
+            raise UPTypeError(
+                f"InstantaneousAction effect has an incompatible value type. Fluent type: {fluent_exp.type} // Value type: {value_exp.type}"
+            )
         if not fluent_exp.type.is_int_type() and not fluent_exp.type.is_real_type():
             raise UPTypeError("Decrease effects can be created only on numeric types!")
         self._add_effect_instance(
             up.model.effect.Effect(
                 fluent_exp,
                 value_exp,
                 condition_exp,
                 kind=up.model.effect.EffectKind.DECREASE,
             )
         )
 
     def _add_effect_instance(self, effect: "up.model.effect.Effect"):
         assert (
-            effect.environment == self._env
+            effect.environment == self._environment
         ), "effect does not have the same environment of the action"
-        if not effect.is_conditional():
-            if effect.is_assignment():
-                if (
-                    effect.fluent in self._fluents_assigned
-                    or effect.fluent in self._fluents_inc_dec
-                ):
-                    raise UPConflictingEffectsException(
-                        f"The effect {effect} is in conflict with the effects already in the action."
-                    )
-                self._fluents_assigned.add(effect.fluent)
-            elif effect.is_increase() or effect.is_decrease():
-                if effect.fluent in self._fluents_assigned:
-                    raise UPConflictingEffectsException(
-                        f"The effect {effect} is in conflict with the effects already in the action."
-                    )
-                self._fluents_inc_dec.add(effect.fluent)
-            else:
-                raise NotImplementedError
-        if (
-            self._simulated_effect is not None
-            and effect.fluent in self._simulated_effect.fluents
-        ):
-            raise UPConflictingEffectsException(
-                f"The effect {effect} is in conflict with the simulated effects already in the action."
-            )
+        up.model.effect.check_conflicting_effects(
+            effect,
+            None,
+            self._simulated_effect,
+            self._fluents_assigned,
+            self._fluents_inc_dec,
+            "action",
+        )
         self._effects.append(effect)
 
     @property
     def simulated_effect(self) -> Optional["up.model.effect.SimulatedEffect"]:
         """Returns the `action` `simulated effect`."""
         return self._simulated_effect
 
     def set_simulated_effect(self, simulated_effect: "up.model.effect.SimulatedEffect"):
         """
         Sets the given `simulated effect` as the only `action's simulated effect`.
 
         :param simulated_effect: The `SimulatedEffect` instance that must be set as this `action`'s only
             `simulated effect`.
         """
-        for f in simulated_effect.fluents:
-            if f in self._fluents_assigned or f in self._fluents_inc_dec:
-                raise UPConflictingEffectsException(
-                    f"The simulated effect {simulated_effect} is in conflict with the effects already in the action."
-                )
+        up.model.effect.check_conflicting_simulated_effects(
+            simulated_effect,
+            None,
+            self._fluents_assigned,
+            self._fluents_inc_dec,
+            "action",
+        )
+        if simulated_effect.environment != self.environment:
+            raise UPUsageError(
+                "The added SimulatedEffect does not have the same environment of the Action"
+            )
         self._simulated_effect = simulated_effect
 
     def _set_preconditions(self, preconditions: List["up.model.fnode.FNode"]):
         self._preconditions = preconditions
 
 
-class DurativeAction(Action):
+class DurativeAction(Action, TimedCondsEffs):
     """Represents a durative action."""
 
     def __init__(
         self,
         _name: str,
         _parameters: Optional["OrderedDict[str, up.model.types.Type]"] = None,
         _env: Optional[Environment] = None,
         **kwargs: "up.model.types.Type",
     ):
         Action.__init__(self, _name, _parameters, _env, **kwargs)
+        TimedCondsEffs.__init__(self, _env)
         self._duration: "up.model.timing.DurationInterval" = (
-            up.model.timing.FixedDuration(self._env.expression_manager.Int(0))
+            up.model.timing.FixedDuration(self._environment.expression_manager.Int(0))
         )
-        self._conditions: Dict[
-            "up.model.timing.TimeInterval", List["up.model.fnode.FNode"]
-        ] = {}
-        self._effects: Dict[
-            "up.model.timing.Timing", List["up.model.effect.Effect"]
-        ] = {}
-        self._simulated_effects: Dict[
-            "up.model.timing.Timing", "up.model.effect.SimulatedEffect"
-        ] = {}
-        self._fluents_assigned: Dict[
-            "up.model.timing.Timing", Set["up.model.fnode.FNode"]
-        ] = {}
-        self._fluents_inc_dec: Dict[
-            "up.model.timing.Timing", Set["up.model.fnode.FNode"]
-        ] = {}
 
     def __repr__(self) -> str:
         s = []
         s.append(f"durative action {self.name}")
         first = True
         for p in self.parameters:
             if first:
@@ -469,169 +506,58 @@
         for t, se in self.simulated_effects.items():
             s.append(f"      {str(t)}: {se}\n")
         s.append("    ]\n")
         s.append("  }")
         return "".join(s)
 
     def __eq__(self, oth: object) -> bool:
-        if isinstance(oth, DurativeAction):
-            if (
-                self._env != oth._env
-                or self._name != oth._name
-                or self._parameters != oth._parameters
-                or self._duration != oth._duration
-            ):
-                return False
-            if len(self._conditions) != len(oth._conditions):
-                return False
-            for i, cl in self._conditions.items():
-                oth_cl = oth._conditions.get(i, None)
-                if oth_cl is None:
-                    return False
-                elif set(cl) != set(oth_cl):
-                    return False
-            if len(self._effects) != len(oth._effects):
-                return False
-            for t, el in self._effects.items():
-                oth_el = oth._effects.get(t, None)
-                if oth_el is None:
-                    return False
-                elif set(el) != set(oth_el):
-                    return False
-            for t, se in self._simulated_effects.items():
-                oth_se = oth._simulated_effects.get(t, None)
-                if oth_se is None:
-                    return False
-                elif se != oth_se:
-                    return False
-            return True
-        else:
+        if not isinstance(oth, DurativeAction):
+            return False
+        if (
+            self._environment != oth._environment
+            or self._name != oth._name
+            or self._parameters != oth._parameters
+            or self._duration != oth._duration
+        ):
             return False
+        if not TimedCondsEffs.__eq__(self, oth):
+            return False
+        return True
 
     def __hash__(self) -> int:
         res = hash(self._name) + hash(self._duration)
         for ap in self._parameters.items():
             res += hash(ap)
-        for i, cl in self._conditions.items():
-            res += hash(i)
-            for c in cl:
-                res += hash(c)
-        for t, el in self._effects.items():
-            res += hash(t)
-            for e in el:
-                res += hash(e)
-        for t, se in self._simulated_effects.items():
-            res += hash(t) + hash(se)
+        res += TimedCondsEffs.__hash__(self)
         return res
 
     def clone(self):
         new_params = OrderedDict(
             (param_name, param.type) for param_name, param in self._parameters.items()
         )
-        new_durative_action = DurativeAction(self._name, new_params, self._env)
+        new_durative_action = DurativeAction(self._name, new_params, self._environment)
         new_durative_action._duration = self._duration
-        new_durative_action._conditions = {
-            t: cl[:] for t, cl in self._conditions.items()
-        }
-        new_durative_action._effects = {
-            t: [e.clone() for e in el] for t, el in self._effects.items()
-        }
-        new_durative_action._simulated_effects = {
-            t: se for t, se in self._simulated_effects.items()
-        }
-        new_durative_action._fluents_assigned = {
-            t: fs.copy() for t, fs in self._fluents_assigned.items()
-        }
-        new_durative_action._fluents_inc_dec = {
-            t: fs.copy() for t, fs in self._fluents_inc_dec.items()
-        }
+
+        TimedCondsEffs._clone_to(self, new_durative_action)
         return new_durative_action
 
     @property
     def duration(self) -> "up.model.timing.DurationInterval":
         """Returns the `action` `duration interval`."""
         return self._duration
 
-    @property
-    def conditions(
-        self,
-    ) -> Dict["up.model.timing.TimeInterval", List["up.model.fnode.FNode"]]:
-        """
-        Returns the `action conditions`; a map from `TimeInterval` to a `list` of `Expressions`
-        indicating that for this `action` to be applicable, during the whole `TimeInterval`
-        set as `key`, all the `expression` in the `mapped list` must evaluate to `True`.
-        """
-        return self._conditions
-
-    def clear_conditions(self):
-        """Removes all `conditions`."""
-        self._conditions = {}
-
-    @property
-    def effects(self) -> Dict["up.model.timing.Timing", List["up.model.effect.Effect"]]:
-        """
-        Returns the all the `action's effects`; a map from `Timing` to `list` of `Effects`
-        indicating that, when the action is applied, all the `Effects` must be applied at the
-        `Timing` set as `key` in the map.
-        """
-        return self._effects
-
-    def clear_effects(self):
-        """Removes all `effects` from the `Action`."""
-        self._effects = {}
-        self._fluents_assigned = {}
-        self._fluents_inc_dec = {}
-
-    @property
-    def conditional_effects(
-        self,
-    ) -> Dict["up.model.timing.Timing", List["up.model.effect.Effect"]]:
-        """
-        Return the `action` `conditional effects`.
-
-        IMPORTANT NOTE: this property does some computation, so it should be called as
-        seldom as possible.
-        """
-        retval: Dict[up.model.timing.Timing, List[up.model.effect.Effect]] = {}
-        for timing, effect_list in self._effects.items():
-            cond_effect_list = [e for e in effect_list if e.is_conditional()]
-            if len(cond_effect_list) > 0:
-                retval[timing] = cond_effect_list
-        return retval
-
-    @property
-    def unconditional_effects(
-        self,
-    ) -> Dict["up.model.timing.Timing", List["up.model.effect.Effect"]]:
-        """
-        Return the `action` `unconditional effects`.
-
-        IMPORTANT NOTE: this property does some computation, so it should be called as
-        seldom as possible.
-        """
-        retval: Dict[up.model.timing.Timing, List[up.model.effect.Effect]] = {}
-        for timing, effect_list in self._effects.items():
-            uncond_effect_list = [e for e in effect_list if not e.is_conditional()]
-            if len(uncond_effect_list) > 0:
-                retval[timing] = uncond_effect_list
-        return retval
-
-    def is_conditional(self) -> bool:
-        """Returns `True` if the `action` has `conditional effects`, `False` otherwise."""
-        return any(e.is_conditional() for l in self._effects.values() for e in l)
-
     def set_duration_constraint(self, duration: "up.model.timing.DurationInterval"):
         """
         Sets the `duration interval` for this `action`.
 
         :param duration: The new `duration interval` of this `action`.
         """
         lower, upper = duration.lower, duration.upper
-        tlower = self._env.type_checker.get_type(lower)
-        tupper = self._env.type_checker.get_type(upper)
+        tlower = self._environment.type_checker.get_type(lower)
+        tupper = self._environment.type_checker.get_type(upper)
         assert tlower.is_int_type() or tlower.is_real_type()
         assert tupper.is_int_type() or tupper.is_real_type()
         if (
             lower.is_constant()
             and upper.is_constant()
             and (
                 upper.constant_value() < lower.constant_value()
@@ -642,292 +568,105 @@
             )
         ):
             raise UPProblemDefinitionError(
                 f"{duration} is an empty interval duration of action: {self.name}."
             )
         self._duration = duration
 
-    def set_fixed_duration(self, value: Union["up.model.fnode.FNode", int, Fraction]):
+    def set_fixed_duration(self, value: "up.model.expression.NumericExpression"):
         """
         Sets the `duration interval` for this `action` as the interval `[value, value]`.
 
         :param value: The `value` set as both edges of this `action's duration`.
         """
-        (value_exp,) = self._env.expression_manager.auto_promote(value)
+        (value_exp,) = self._environment.expression_manager.auto_promote(value)
         self.set_duration_constraint(up.model.timing.FixedDuration(value_exp))
 
     def set_closed_duration_interval(
         self,
-        lower: Union["up.model.fnode.FNode", int, Fraction],
-        upper: Union["up.model.fnode.FNode", int, Fraction],
+        lower: "up.model.expression.NumericExpression",
+        upper: "up.model.expression.NumericExpression",
     ):
         """
         Sets the `duration interval` for this `action` as the interval `[lower, upper]`.
 
         :param lower: The value set as the lower edge of this `action's duration`.
         :param upper: The value set as the upper edge of this `action's duration`.
         """
-        lower_exp, upper_exp = self._env.expression_manager.auto_promote(lower, upper)
+        lower_exp, upper_exp = self._environment.expression_manager.auto_promote(
+            lower, upper
+        )
         self.set_duration_constraint(
             up.model.timing.ClosedDurationInterval(lower_exp, upper_exp)
         )
 
     def set_open_duration_interval(
         self,
-        lower: Union["up.model.fnode.FNode", int, Fraction],
-        upper: Union["up.model.fnode.FNode", int, Fraction],
+        lower: "up.model.expression.NumericExpression",
+        upper: "up.model.expression.NumericExpression",
     ):
         """
         Sets the `duration interval` for this action as the interval `]lower, upper[`.
 
         :param lower: The value set as the lower edge of this `action's duration`.
         :param upper: The value set as the upper edge of this `action's duration`.
 
         Note that `lower` and `upper` are not part of the interval.
         """
-        lower_exp, upper_exp = self._env.expression_manager.auto_promote(lower, upper)
+        lower_exp, upper_exp = self._environment.expression_manager.auto_promote(
+            lower, upper
+        )
         self.set_duration_constraint(
             up.model.timing.OpenDurationInterval(lower_exp, upper_exp)
         )
 
     def set_left_open_duration_interval(
         self,
-        lower: Union["up.model.fnode.FNode", int, Fraction],
-        upper: Union["up.model.fnode.FNode", int, Fraction],
+        lower: "up.model.expression.NumericExpression",
+        upper: "up.model.expression.NumericExpression",
     ):
         """
         Sets the `duration interval` for this `action` as the interval `]lower, upper]`.
 
         :param lower: The value set as the lower edge of this `action's duration`.
         :param upper: The value set as the upper edge of this `action's duration`.
 
         Note that `lower` is not part of the interval.
         """
-        lower_exp, upper_exp = self._env.expression_manager.auto_promote(lower, upper)
+        lower_exp, upper_exp = self._environment.expression_manager.auto_promote(
+            lower, upper
+        )
         self.set_duration_constraint(
             up.model.timing.LeftOpenDurationInterval(lower_exp, upper_exp)
         )
 
     def set_right_open_duration_interval(
         self,
-        lower: Union["up.model.fnode.FNode", int, Fraction],
-        upper: Union["up.model.fnode.FNode", int, Fraction],
+        lower: "up.model.expression.NumericExpression",
+        upper: "up.model.expression.NumericExpression",
     ):
         """
         Sets the `duration interval` for this `action` as the interval `[lower, upper[`.
 
         :param lower: The value set as the lower edge of this `action's duration`.
         :param upper: The value set as the upper edge of this `action's duration`.
 
         Note that `upper` is not part of the interval.
         """
-        lower_exp, upper_exp = self._env.expression_manager.auto_promote(lower, upper)
+        lower_exp, upper_exp = self._environment.expression_manager.auto_promote(
+            lower, upper
+        )
         self.set_duration_constraint(
             up.model.timing.RightOpenDurationInterval(lower_exp, upper_exp)
         )
 
-    def add_condition(
-        self,
-        interval: Union["up.model.timing.Timing", "up.model.timing.TimeInterval"],
-        condition: Union[
-            "up.model.fnode.FNode",
-            "up.model.fluent.Fluent",
-            "up.model.parameter.Parameter",
-            bool,
-        ],
-    ):
-        """
-        Adds the given expression to the `action's conditions`. For this `action` to be applicable
-        the given expression must evaluate to `True` during the whole given `interval`.
-
-        :param interval: The `interval` in which the given expression must evaluate to `True` for this
-            `action` to be applicable.
-        :param condition: The expression that must be `True` in the given `interval` for this
-            `action` to be applicable.
-        """
-        if isinstance(interval, up.model.Timing):
-            interval = up.model.TimePointInterval(interval)
-        (condition_exp,) = self._env.expression_manager.auto_promote(condition)
-        assert self._env.type_checker.get_type(condition_exp).is_bool_type()
-        conditions = self._conditions.setdefault(interval, [])
-        if condition_exp not in conditions:
-            conditions.append(condition_exp)
-
-    def _set_conditions(
-        self,
-        interval: "up.model.timing.TimeInterval",
-        conditions: List["up.model.fnode.FNode"],
-    ):
-        self._conditions[interval] = conditions
-
-    def add_effect(
-        self,
-        timing: "up.model.timing.Timing",
-        fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
-        value: "up.model.expression.Expression",
-        condition: "up.model.expression.BoolExpression" = True,
-    ):
-        """
-        At the given time, adds the given assignment to the `action's effects`.
-
-        :param timing: The exact time in which the assignment is applied.
-        :param fluent: The `fluent` which value is modified by the assignment.
-        :param value: The `value` to assign to the given `fluent`.
-        :param condition: The `condition` in which this `effect` is applied; the default
-            value is `True`.
-        """
-        (
-            fluent_exp,
-            value_exp,
-            condition_exp,
-        ) = self._env.expression_manager.auto_promote(fluent, value, condition)
-        assert fluent_exp.is_fluent_exp()
-        if not self._env.type_checker.get_type(condition_exp).is_bool_type():
-            raise UPTypeError("Effect condition is not a Boolean condition!")
-        if not fluent_exp.type.is_compatible(value_exp.type):
-            raise UPTypeError("DurativeAction effect has not compatible types!")
-        self._add_effect_instance(
-            timing, up.model.effect.Effect(fluent_exp, value_exp, condition_exp)
-        )
-
-    def add_increase_effect(
-        self,
-        timing: "up.model.timing.Timing",
-        fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
-        value: "up.model.expression.Expression",
-        condition: "up.model.expression.BoolExpression" = True,
-    ):
-        """
-        At the given time, adds the given `increment` to the `action's effects`.
-
-        :param timing: The exact time in which the increment is applied.
-        :param fluent: The `fluent` which value is incremented by the added `effect`.
-        :param value: The given `fluent` is incremented by the given `value`.
-        :param condition: The `condition` in which this effect is applied; the default
-            value is `True`.
-        """
-        (
-            fluent_exp,
-            value_exp,
-            condition_exp,
-        ) = self._env.expression_manager.auto_promote(fluent, value, condition)
-        assert fluent_exp.is_fluent_exp()
-        if not condition_exp.type.is_bool_type():
-            raise UPTypeError("Effect condition is not a Boolean condition!")
-        if not fluent_exp.type.is_compatible(value_exp.type):
-            raise UPTypeError("DurativeAction effect has not compatible types!")
-        if not fluent_exp.type.is_int_type() and not fluent_exp.type.is_real_type():
-            raise UPTypeError("Increase effects can be created only on numeric types!")
-        self._add_effect_instance(
-            timing,
-            up.model.effect.Effect(
-                fluent_exp,
-                value_exp,
-                condition_exp,
-                kind=up.model.effect.EffectKind.INCREASE,
-            ),
-        )
-
-    def add_decrease_effect(
-        self,
-        timing: "up.model.timing.Timing",
-        fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
-        value: "up.model.expression.Expression",
-        condition: "up.model.expression.BoolExpression" = True,
-    ):
-        """
-        At the given time, adds the given `decrement` to the `action's effects`.
-
-        :param timing: The exact time in which the `decrement` is applied.
-        :param fluent: The `fluent` which value is decremented by the added effect.
-        :param value: The given `fluent` is decremented by the given `value`.
-        :param condition: The `condition` in which this effect is applied; the default
-            value is `True`.
-        """
-        (
-            fluent_exp,
-            value_exp,
-            condition_exp,
-        ) = self._env.expression_manager.auto_promote(fluent, value, condition)
-        assert fluent_exp.is_fluent_exp()
-        if not condition_exp.type.is_bool_type():
-            raise UPTypeError("Effect condition is not a Boolean condition!")
-        if not fluent_exp.type.is_compatible(value_exp.type):
-            raise UPTypeError("DurativeAction effect has not compatible types!")
-        if not fluent_exp.type.is_int_type() and not fluent_exp.type.is_real_type():
-            raise UPTypeError("Decrease effects can be created only on numeric types!")
-        self._add_effect_instance(
-            timing,
-            up.model.effect.Effect(
-                fluent_exp,
-                value_exp,
-                condition_exp,
-                kind=up.model.effect.EffectKind.DECREASE,
-            ),
-        )
-
-    def _add_effect_instance(
-        self, timing: "up.model.timing.Timing", effect: "up.model.effect.Effect"
-    ):
-        assert (
-            self._env == effect.environment
-        ), "effect does not have the same environment of the action"
-        fluents_assigned = self._fluents_assigned.setdefault(timing, set())
-        fluents_inc_dec = self._fluents_inc_dec.setdefault(timing, set())
-        simulated_effect = self._simulated_effects.get(timing, None)
-        if not effect.is_conditional():
-            if effect.is_assignment():
-                if (
-                    effect.fluent in fluents_assigned
-                    or effect.fluent in fluents_inc_dec
-                ):
-                    raise UPConflictingEffectsException(
-                        f"The effect {effect} at timing {timing} is in conflict with the effects already in the action."
-                    )
-                fluents_assigned.add(effect.fluent)
-            elif effect.is_increase() or effect.is_decrease():
-                if effect.fluent in fluents_assigned:
-                    raise UPConflictingEffectsException(
-                        f"The effect {effect} at timing {timing} is in conflict with the effects already in the action."
-                    )
-                fluents_inc_dec.add(effect.fluent)
-            else:
-                raise NotImplementedError
-        if simulated_effect is not None and effect.fluent in simulated_effect.fluents:
-            raise UPConflictingEffectsException(
-                f"The effect {effect} is in conflict with the simulated effects already in the action."
-            )
-        self._effects.setdefault(timing, []).append(effect)
-
-    @property
-    def simulated_effects(
-        self,
-    ) -> Dict["up.model.timing.Timing", "up.model.effect.SimulatedEffect"]:
-        """Returns the `action` `simulated effects`."""
-        return self._simulated_effects
-
-    def set_simulated_effect(
-        self,
-        timing: "up.model.timing.Timing",
-        simulated_effect: "up.model.effect.SimulatedEffect",
-    ):
-        """
-        Sets the given `simulated effect` at the specified `timing`.
-
-        :param timing: The time in which the `simulated effect` must be applied.
-        :param simulated effects: The `simulated effect` that must be applied at the given `timing`.
-        """
-        for f in simulated_effect.fluents:
-            if f in self._fluents_assigned.get(
-                timing, set()
-            ) or f in self._fluents_inc_dec.get(timing, set()):
-                raise UPConflictingEffectsException(
-                    f"The simulated effect {simulated_effect} is in conflict with the effects already in the action."
-                )
-        self._simulated_effects[timing] = simulated_effect
+    def is_conditional(self) -> bool:
+        """Returns `True` if the `action` has `conditional effects`, `False` otherwise."""
+        # re-implemenation needed for inheritance, delegate implementation.
+        return TimedCondsEffs.is_conditional(self)
 
 
 class SensingAction(InstantaneousAction):
     """This class represents a sensing action."""
 
     def __init__(
         self,
@@ -953,24 +692,24 @@
             res += hash(of)
         return res
 
     def clone(self):
         new_params = OrderedDict()
         for param_name, param in self._parameters.items():
             new_params[param_name] = param.type
-        new_sensing_action = SensingAction(self._name, new_params, self._env)
+        new_sensing_action = SensingAction(self._name, new_params, self._environment)
         new_sensing_action._preconditions = self._preconditions[:]
         new_sensing_action._effects = [e.clone() for e in self._effects]
         new_sensing_action._fluents_assigned = self._fluents_assigned.copy()
         new_sensing_action._fluents_inc_dec = self._fluents_inc_dec.copy()
         new_sensing_action._simulated_effect = self._simulated_effect
         new_sensing_action._observed_fluents = self._observed_fluents.copy()
         return new_sensing_action
 
-    def add_observed_fluents(self, observed_fluents: List["up.model.fnode.FNode"]):
+    def add_observed_fluents(self, observed_fluents: Iterable["up.model.fnode.FNode"]):
         """
         Adds the given list of observed fluents.
 
         :param observed_fluents: The list of observed fluents that must be added.
         """
         for of in observed_fluents:
             self.add_observed_fluent(of)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/contingent_problem.py` & `unified_planning-0.6.0/unified_planning/model/contingent_problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 class ContingentProblem(Problem):
     """This class represent a contingent planning problem."""
 
     def __init__(
         self,
         name: Optional[str] = None,
-        env: Optional["up.environment.Environment"] = None,
+        environment: Optional["up.environment.Environment"] = None,
         *,
         initial_defaults: Dict["up.model.types.Type", "ConstantExpression"] = {},
     ):
-        Problem.__init__(self, name, env, initial_defaults=initial_defaults)
+        Problem.__init__(self, name, environment, initial_defaults=initial_defaults)
         self._hidden_fluents: Set["up.model.fnode.FNode"] = set()
         self._or_initial_constraints: List[List["up.model.fnode.FNode"]] = []
         self._oneof_initial_constraints: List[List["up.model.fnode.FNode"]] = []
 
     def __repr__(self) -> str:
         s = []
         s.append(super().__repr__())
@@ -85,16 +85,19 @@
         new_p._timed_effects = {
             t: [e.clone() for e in el] for t, el in self._timed_effects.items()
         }
         new_p._timed_goals = {i: [g for g in gl] for i, gl in self._timed_goals.items()}
         new_p._goals = self._goals[:]
         new_p._metrics = []
         for m in self._metrics:
-            if isinstance(m, up.model.metrics.MinimizeActionCosts):
-                costs = {new_p.action(a.name): c for a, c in m.costs.items()}
+            if m.is_minimize_action_costs():
+                assert isinstance(m, up.model.metrics.MinimizeActionCosts)
+                costs: Dict["up.model.Action", "up.model.Expression"] = {
+                    new_p.action(a.name): c for a, c in m.costs.items()
+                }
                 new_p._metrics.append(up.model.metrics.MinimizeActionCosts(costs))
             else:
                 new_p._metrics.append(m)
         new_p._initial_defaults = self._initial_defaults.copy()
         new_p._fluents_defaults = self._fluents_defaults.copy()
         new_p._hidden_fluents = self._hidden_fluents.copy()
         new_p._or_initial_constraints = self._or_initial_constraints.copy()
@@ -103,39 +106,35 @@
 
     def add_oneof_initial_constraint(
         self, fluents: Iterable[Union["up.model.fnode.FNode", "up.model.fluent.Fluent"]]
     ):
         """
         Adds a oneof initial constraint on some hidden fluents.
 
-        :param fluents: a list of fluent expressions, exatly one of them must hold in the initial state.
+        :param fluents: a sequence of fluents expressions, exactly one of them must hold in the initial state.
         """
         em = self._env.expression_manager
-        c = []
-        for f in fluents:
-            (f_exp,) = em.auto_promote(f)
+        constraints: List["up.model.fnode.FNode"] = em.auto_promote(fluents)
+        for f_exp in constraints:
             self._hidden_fluents.add(f_exp)
-            c.append(f_exp)
-        self._oneof_initial_constraints.append(c)
+        self._oneof_initial_constraints.append(constraints)
 
     def add_or_initial_constraint(
         self, fluents: Iterable[Union["up.model.fnode.FNode", "up.model.fluent.Fluent"]]
     ):
         """
         Adds a or initial constraint on some hidden fluents.
 
         :param fluents: a list of fluent expressions, at least one of them must hold in the initial state.
         """
         em = self._env.expression_manager
-        c = []
-        for f in fluents:
-            (f_exp,) = em.auto_promote(f)
+        constraints: List["up.model.fnode.FNode"] = em.auto_promote(fluents)
+        for f_exp in constraints:
             self._hidden_fluents.add(f_exp)
-            c.append(f_exp)
-        self._or_initial_constraints.append(c)
+        self._or_initial_constraints.append(constraints)
 
     def add_unknown_initial_constraint(
         self, fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"]
     ):
         """
         Adds an unknown initial constraint on a hidden fluent.
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/effect.py` & `unified_planning-0.6.0/unified_planning/model/fluent.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,223 +9,264 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-This module defines the `Effect` class.
-A basic `Effect` has a `fluent` and an `expression`.
-A `condition` can be added to make it a `conditional effect`.
+This module defines the Fluent class.
+A Fluent has a name, a type and a signature
+that defines the types of its parameters.
 """
 
-
 import unified_planning as up
-from enum import Enum, auto
-from typing import List, Callable, Dict
+from unified_planning.environment import get_environment, Environment
+from unified_planning.model.types import domain_size, domain_item
+from typing import List, OrderedDict, Optional, Union, Iterator
 
 
-class EffectKind(Enum):
-    """
-    The `Enum` representing the possible `Effects` in the `unified_planning`.
-
-    The semantic is the following of an `effect` with fluent `F`, value `V` and condition `C`:
-    `ASSIGN`   => `if C then F <= V`
-    `INCREASE` => `if C then F <= F + V`
-    `DECREASE` => `if C then F <= F - V`
-    """
-
-    ASSIGN = auto()
-    INCREASE = auto()
-    DECREASE = auto()
-
-
-class Effect:
-    """
-    This class represent an effect. It has a :class:`~unified_planning.model.Fluent`, modified by this effect, a value
-    that determines how the `Fluent` is modified, a `condition` that determines if the `Effect`
-    is actually applied or not and an `EffectKind` that determines the semantic of the `Effect`.
-    """
+class Fluent:
+    """Represents a fluent."""
 
     def __init__(
         self,
-        fluent: "up.model.fnode.FNode",
-        value: "up.model.fnode.FNode",
-        condition: "up.model.fnode.FNode",
-        kind: EffectKind = EffectKind.ASSIGN,
+        name: str,
+        typename: Optional["up.model.types.Type"] = None,
+        _signature: Optional[
+            Union[
+                OrderedDict[str, "up.model.types.Type"],
+                List["up.model.parameter.Parameter"],
+            ]
+        ] = None,
+        environment: Optional[Environment] = None,
+        **kwargs: "up.model.types.Type",
     ):
-        self._fluent = fluent
-        self._value = value
-        self._condition = condition
-        self._kind = kind
-        assert (
-            fluent.environment == value.environment
-            and value.environment == condition.environment
-        ), "Effect expressions have different environment."
+        self._env = get_environment(environment)
+        self._name = name
+        if typename is None:
+            self._typename = self._env.type_manager.BoolType()
+        else:
+            assert self._env.type_manager.has_type(
+                typename
+            ), "type of parameter does not belong to the same environment of the fluent"
+            self._typename = typename
+        self._signature: List["up.model.parameter.Parameter"] = []
+        if _signature is not None:
+            assert len(kwargs) == 0
+            if isinstance(_signature, OrderedDict):
+                for param_name, param_type in _signature.items():
+                    self._signature.append(
+                        up.model.parameter.Parameter(param_name, param_type, self._env)
+                    )
+            elif isinstance(_signature, List):
+                assert all(
+                    p.environment == self._env for p in _signature
+                ), "one of the parameters does not belong to the same environment of the fluent"
+                self._signature = _signature[:]
+            else:
+                raise NotImplementedError
+        else:
+            for param_name, param_type in kwargs.items():
+                self._signature.append(
+                    up.model.parameter.Parameter(param_name, param_type, self._env)
+                )
 
     def __repr__(self) -> str:
-        s = []
-        if self.is_conditional():
-            s.append(f"if {str(self._condition)} then")
-        s.append(f"{str(self._fluent)}")
-        if self.is_assignment():
-            s.append(":=")
-        elif self.is_increase():
-            s.append("+=")
-        elif self.is_decrease():
-            s.append("-=")
-        s.append(f"{str(self._value)}")
-        return " ".join(s)
+        sign = ""
+        if self.arity > 0:
+            sign_items = [f"{p.name}={str(p.type)}" for p in self.signature]
+            sign = f'[{", ".join(sign_items)}]'
+        return f"{str(self.type)} {self.name}{sign}"
 
     def __eq__(self, oth: object) -> bool:
-        if isinstance(oth, Effect):
+        if isinstance(oth, Fluent):
             return (
-                self._fluent == oth._fluent
-                and self._value == oth._value
-                and self._condition == oth._condition
-                and self._kind == oth._kind
+                self._name == oth._name
+                and self._typename == oth._typename
+                and self._signature == oth._signature
+                and self._env == oth._env
             )
         else:
             return False
 
     def __hash__(self) -> int:
-        return (
-            hash(self._fluent)
-            + hash(self._value)
-            + hash(self._condition)
-            + hash(self._kind)
-        )
-
-    def clone(self):
-        new_effect = Effect(self._fluent, self._value, self._condition, self._kind)
-        return new_effect
+        res = hash(self._typename)
+        for p in self._signature:
+            res += hash(p)
+        return res ^ hash(self._name)
 
-    def is_conditional(self) -> bool:
-        """
-        Returns `True` if the `Effect` condition is not `True`; this means that the `Effect` might
-        not always be applied but depends on the runtime evaluation of it's :func:`condition <unified_planning.model.Effect.condition>`.
-        """
-        return not self._condition.is_true()
+    @property
+    def name(self) -> str:
+        """Returns the `Fluent` `name`."""
+        return self._name
 
     @property
-    def fluent(self) -> "up.model.fnode.FNode":
-        """Returns the `Fluent` that is modified by this `Effect`."""
-        return self._fluent
+    def type(self) -> "up.model.types.Type":
+        """Returns the `Fluent` `Type`."""
+        return self._typename
 
     @property
-    def value(self) -> "up.model.fnode.FNode":
-        """Returns the `value` given to the `Fluent` by this `Effect`."""
-        return self._value
+    def signature(self) -> List["up.model.parameter.Parameter"]:
+        """
+        Returns the `Fluent` `signature`.
+        The `signature` is the `List` of `Parameters` indicating the :class:`Types <unified_planning.model.Type>` compatible with this `Fluent`.
+        """
+        return self._signature
 
-    def set_value(self, new_value: "up.model.fnode.FNode"):
+    @property
+    def arity(self) -> int:
         """
-        Sets the `value` given to the `Fluent` by this `Effect`.
+        Returns the `Fluent` arity.
 
-        :param new_value: The `value` that will be set as this `effect's value`.
+        IMPORTANT NOTE: this property does some computation, so it should be called as
+        seldom as possible.
         """
-        self._value = new_value
+        return len(self._signature)
 
     @property
-    def condition(self) -> "up.model.fnode.FNode":
-        """Returns the `condition` required for this `Effect` to be applied."""
-        return self._condition
-
-    def set_condition(self, new_condition: "up.model.fnode.FNode"):
+    def environment(self) -> "Environment":
+        """Returns the `Fluent` `Environment`."""
+        return self._env
+
+    def __call__(
+        self, *args: "up.model.expression.Expression"
+    ) -> "up.model.fnode.FNode":
         """
-        Sets the `condition` required for this `Effect` to be applied.
+        Returns a fluent expression with the given parameters.
 
-        :param new_condition: The expression set as this `effect's condition`.
+        :param args: The expressions used as this fluent's parameters in the created expression.
+        :return: The created FluentExp.
         """
-        self._condition = new_condition
+        return self._env.expression_manager.FluentExp(self, args)
 
-    @property
-    def kind(self) -> EffectKind:
-        """Returns the `kind` of this `Effect`."""
-        return self._kind
+    #
+    # Infix operators
+    #
 
-    @property
-    def environment(self) -> "up.environment.Environment":
-        """Returns this `Effect's Environment`."""
-        return self._fluent.environment
-
-    def is_assignment(self) -> bool:
-        """Returns `True` if the :func:`kind <unified_planning.model.Effect.kind>` of this `Effect` is an `assignment`, `False` otherwise."""
-        return self._kind == EffectKind.ASSIGN
-
-    def is_increase(self) -> bool:
-        """Returns `True` if the :func:`kind <unified_planning.model.Effect.kind>` of this `Effect` is an `increase`, `False` otherwise."""
-        return self._kind == EffectKind.INCREASE
-
-    def is_decrease(self) -> bool:
-        """Returns `True` if the :func:`kind <unified_planning.model.Effect.kind>` of this `Effect` is a `decrease`, `False` otherwise."""
-        return self._kind == EffectKind.DECREASE
-
-
-class SimulatedEffect:
-    """
-    This class represents a `simulated effect` over a list of :class:`~unified_planning.model.Fluent` expressions.
-    The `fluent's parameters` must be constants or :class:`~unified_planning.model.Action` `parameters`.
-    The callable function must return the result of the `simulated effects` applied
-    in the given :class:`~unified_planning.model.ROState` for the specified `fluent` expressions.
-    """
+    def __add__(self, right):
+        return self._env.expression_manager.Plus(self, right)
 
-    def __init__(
-        self,
-        fluents: List["up.model.fnode.FNode"],
-        function: Callable[
-            [
-                "up.model.problem.AbstractProblem",
-                "up.model.state.ROState",
-                Dict["up.model.parameter.Parameter", "up.model.fnode.FNode"],
-            ],
-            List["up.model.fnode.FNode"],
-        ],
-    ):
-        for f in fluents:
-            if not f.is_fluent_exp():
-                raise up.exceptions.UPUsageError(
-                    "Simulated effects can be defined on fluent expressions with constant parameters"
-                )
-            for c in f.args:
-                if not (c.is_constant() or c.is_parameter_exp()):
-                    raise up.exceptions.UPUsageError(
-                        "Simulated effects can be defined on fluent expressions with constant parameters"
-                    )
-        self._fluents = fluents
-        self._function = function
+    def __radd__(self, left):
+        return self._env.expression_manager.Plus(left, self)
 
-    def __repr__(self) -> str:
-        return f"{self._fluents} := simulated"
+    def __sub__(self, right):
+        return self._env.expression_manager.Minus(self, right)
 
-    def __eq__(self, oth: object) -> bool:
-        if isinstance(oth, SimulatedEffect):
-            return self._fluents == oth._fluents and self._function == oth._function
-        else:
-            return False
+    def __rsub__(self, left):
+        return self._env.expression_manager.Minus(left, self)
 
-    def __hash__(self) -> int:
-        res = hash(self._function)
-        for f in self._fluents:
-            res += hash(f)
-        return res
+    def __mul__(self, right):
+        return self._env.expression_manager.Times(self, right)
 
-    @property
-    def fluents(self) -> List["up.model.fnode.FNode"]:
-        """Returns the `list` of `Fluents Expressions` modified by this `SimulatedEffect`."""
-        return self._fluents
+    def __rmul__(self, left):
+        return self._env.expression_manager.Times(left, self)
 
-    @property
-    def function(
-        self,
-    ) -> Callable[
-        [
-            "up.model.problem.AbstractProblem",
-            "up.model.state.ROState",
-            Dict["up.model.parameter.Parameter", "up.model.fnode.FNode"],
-        ],
-        List["up.model.fnode.FNode"],
-    ]:
-        """
-        Return the function that contains the information on how the `fluents` of this `SimulatedEffect`
-        are modified when this `simulated effect` is applied.
-        """
-        return self._function
+    def __truediv__(self, right):
+        return self._env.expression_manager.Div(self, right)
+
+    def __rtruediv__(self, left):
+        return self._env.expression_manager.Div(left, self)
+
+    def __floordiv__(self, right):
+        return self._env.expression_manager.Div(self, right)
+
+    def __rfloordiv__(self, left):
+        return self._env.expression_manager.Div(left, self)
+
+    def __gt__(self, right):
+        return self._env.expression_manager.GT(self, right)
+
+    def __ge__(self, right):
+        return self._env.expression_manager.GE(self, right)
+
+    def __lt__(self, right):
+        return self._env.expression_manager.LT(self, right)
+
+    def __le__(self, right):
+        return self._env.expression_manager.LE(self, right)
+
+    def __pos__(self):
+        return self._env.expression_manager.Plus(0, self)
+
+    def __neg__(self):
+        return self._env.expression_manager.Minus(0, self)
+
+    def Equals(self, right):
+        return self._env.expression_manager.Equals(self, right)
+
+    def And(self, *other):
+        return self._env.expression_manager.And(self, *other)
+
+    def __and__(self, *other):
+        return self._env.expression_manager.And(self, *other)
+
+    def __rand__(self, *other):
+        return self._env.expression_manager.And(*other, self)
+
+    def Or(self, *other):
+        return self._env.expression_manager.Or(self, *other)
+
+    def __or__(self, *other):
+        return self._env.expression_manager.Or(self, *other)
+
+    def __ror__(self, *other):
+        return self._env.expression_manager.Or(*other, self)
+
+    def Not(self):
+        return self._env.expression_manager.Not(self)
+
+    def __invert__(self):
+        return self._env.expression_manager.Not(self)
+
+    def Xor(self, *other):
+        em = self._env.expression_manager
+        return em.And(em.Or(self, *other), em.Not(em.And(self, *other)))
+
+    def __xor__(self, *other):
+        em = self._env.expression_manager
+        return em.And(em.Or(self, *other), em.Not(em.And(self, *other)))
+
+    def __rxor__(self, other):
+        em = self._env.expression_manager
+        return em.And(em.Or(*other, self), em.Not(em.And(*other, self)))
+
+    def Implies(self, right):
+        return self._env.expression_manager.Implies(self, right)
+
+    def Iff(self, right):
+        return self._env.expression_manager.Iff(self, right)
+
+
+def get_ith_fluent_exp(
+    objects_set: "up.model.mixins.ObjectsSetMixin",
+    fluent: "up.model.fluent.Fluent",
+    domain_sizes: List[int],
+    idx: int,
+) -> "up.model.fnode.FNode":
+    """Returns the ith ground fluent expression."""
+    quot = idx
+    rem = 0
+    actual_parameters = []
+    for i, p in enumerate(fluent.signature):
+        ds = domain_sizes[i]
+        rem = quot % ds
+        quot //= ds
+        v = domain_item(objects_set, p.type, rem)
+        actual_parameters.append(v)
+    return fluent(*actual_parameters)
+
+
+def get_all_fluent_exp(
+    objects_set: "up.model.mixins.ObjectsSetMixin",
+    fluent: "up.model.fluent.Fluent",
+) -> Iterator["up.model.fnode.FNode"]:
+    if fluent.arity == 0:
+        yield fluent.environment.expression_manager.FluentExp(fluent)
+    else:
+        ground_size = 1
+        domain_sizes = []
+        for p in fluent.signature:
+            ds = domain_size(objects_set, p.type)
+            domain_sizes.append(ds)
+            ground_size *= ds
+        for i in range(ground_size):
+            yield get_ith_fluent_exp(objects_set, fluent, domain_sizes, i)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/expression.py` & `unified_planning-0.6.0/unified_planning/model/expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,133 +18,151 @@
 are represented by the same object.
 """
 
 
 import unified_planning as up
 import unified_planning.model.types
 from unified_planning.model.operators import OperatorKind
-from unified_planning.exceptions import UPTypeError, UPExpressionDefinitionError
+from unified_planning.exceptions import (
+    UPTypeError,
+    UPExpressionDefinitionError,
+    UPValueError,
+)
 from fractions import Fraction
-from typing import Optional, Iterable, List, Union, Dict, Tuple
+from typing import Optional, Iterable, List, Union, Dict, Tuple, Iterator, Sequence
 
-Expression = Union[
-    "up.model.fnode.FNode",
-    "up.model.fluent.Fluent",
-    "up.model.object.Object",
-    "up.model.parameter.Parameter",
-    "up.model.variable.Variable",
-    "up.model.timing.Timing",
-    bool,
-    int,
-    float,
-    Fraction,
-]
 BoolExpression = Union[
     "up.model.fnode.FNode",
     "up.model.fluent.Fluent",
     "up.model.parameter.Parameter",
     "up.model.variable.Variable",
     bool,
 ]
+NumericConstant = Union[int, float, Fraction, str]
+NumericExpression = Union["up.model.fnode.FNode", NumericConstant]
 ConstantExpression = Union[
-    "up.model.fnode.FNode", "up.model.object.Object", bool, int, float, Fraction
+    NumericExpression,
+    "up.model.object.Object",
+    bool,
+]
+Expression = Union[
+    "up.model.timing.Timing",
+    BoolExpression,
+    ConstantExpression,
 ]
 
 
+def uniform_numeric_constant(value: NumericConstant) -> Union[Fraction, int]:
+    """Utility method to handle NumericConstant polymorphism."""
+    if not isinstance(value, (float, Fraction)):
+        try:
+            return int(value)
+        except ValueError:
+            pass
+    try:
+        number = Fraction(value)
+    except ValueError:
+        raise UPValueError(f"Numeric constant {value} can't be converted to a number")
+    return number
+
+
 class ExpressionManager(object):
     """ExpressionManager is responsible for the creation of all expressions."""
 
-    def __init__(self, env: "up.environment.Environment"):
-        self.env = env
+    def __init__(self, environment: "up.environment.Environment"):
+        self.environment = environment
         self.expressions: Dict[
             "up.model.fnode.FNodeContent", "up.model.fnode.FNode"
         ] = {}
         self._next_free_id = 1
 
         self.true_expression = self.create_node(
             node_type=OperatorKind.BOOL_CONSTANT, args=tuple(), payload=True
         )
         self.false_expression = self.create_node(
             node_type=OperatorKind.BOOL_CONSTANT, args=tuple(), payload=False
         )
         return
 
-    def _polymorph_args_to_tuple(
+    def _polymorph_args_to_iterator(
         self, *args: Union[Expression, Iterable[Expression]]
-    ) -> Tuple[Expression, ...]:
+    ) -> Iterator[Expression]:
         """
-        Helper function to return a tuple of arguments from args.
+        Helper function to return an Iterator of arguments from args.
         This function is used to allow N-ary operators to express their arguments
-        both as a list of arguments or as a tuple of arguments: e.g.,
-           And([a,b,c]) and And(a,b,c)
-        are both valid, and they are converted into a tuple (a,b,c)
-        """
-
-        res = []
-        for p in args:
-            if isinstance(p, Iterable):
-                res.extend(list(p))
+        both as a list of arguments or as a tuple of arguments:
+        e.g. And([a,b,c]) and And(a,b,c)
+        are both valid, and they are converted into (a,b,c)
+        """
+        for a in args:
+            if isinstance(a, Iterable) and not isinstance(a, str):
+                for p in a:
+                    yield p
             else:
-                res.append(p)
-        return tuple(res)
+                yield a
 
     def auto_promote(
         self, *args: Union[Expression, Iterable[Expression]]
     ) -> List["up.model.fnode.FNode"]:
         """
         Method that takes an iterable of expressions and returns the list
         of these expressions casted to FNode.
 
         :param args: The iterable of expression that must be promoted to FNode.
         :return: The resulting list of FNode.
         """
-        tuple_args = self._polymorph_args_to_tuple(*args)
         res = []
-        for e in tuple_args:
+        for e in self._polymorph_args_to_iterator(*args):
             if isinstance(e, up.model.fluent.Fluent):
                 assert (
-                    e.environment == self.env
+                    e.environment == self.environment
                 ), "Fluent has a different environment of the expression manager"
                 res.append(self.FluentExp(e))
             elif isinstance(e, up.model.parameter.Parameter):
                 assert (
-                    e.environment == self.env
+                    e.environment == self.environment
                 ), "Parameter has a different environment of the expression manager"
                 res.append(self.ParameterExp(e))
             elif isinstance(e, up.model.variable.Variable):
                 assert (
-                    e.environment == self.env
+                    e.environment == self.environment
                 ), "Variable has a different environment of the expression manager"
                 res.append(self.VariableExp(e))
             elif isinstance(e, up.model.object.Object):
                 assert (
-                    e.environment == self.env
+                    e.environment == self.environment
                 ), "Object has a different environment of the expression manager"
                 res.append(self.ObjectExp(e))
             elif isinstance(e, up.model.timing.Timing):
                 res.append(self.TimingExp(e))
             elif isinstance(e, bool):
                 res.append(self.Bool(e))
-            elif isinstance(e, int):
-                res.append(self.Int(e))
-            elif isinstance(e, float):
-                res.append(self.Real(Fraction(e)))
-            elif isinstance(e, Fraction):
-                res.append(self.Real(e))
+            elif (
+                isinstance(e, int)
+                or isinstance(e, float)
+                or isinstance(e, Fraction)
+                or isinstance(e, str)
+            ):
+                number = uniform_numeric_constant(e)
+                if isinstance(number, int):
+                    res.append(self.Int(number))
+                else:
+                    assert isinstance(number, Fraction)
+                    res.append(self.Real(number))
             else:
                 assert (
-                    e.environment == self.env
+                    e.environment == self.environment
                 ), "Expression has a different environment of the expression manager"
                 res.append(e)
         return res
 
     def create_node(
         self,
         node_type: OperatorKind,
-        args: Iterable["up.model.fnode.FNode"],
+        args: Tuple["up.model.fnode.FNode", ...],
         payload: Optional[
             Union[
                 "up.model.fluent.Fluent",
                 "up.model.object.Object",
                 "up.model.parameter.Parameter",
                 "up.model.variable.Variable",
                 "up.model.timing.Timing",
@@ -157,89 +175,97 @@
         ] = None,
     ) -> "up.model.fnode.FNode":
         """
         Creates the unified_planning expressions if it hasn't been created yet in the environment. Otherwise
         returns the existing one.
 
         :param node_type: The OperationKind referring to this expression (like a PLUS, MINUS, FLUENT_EXP, etc.).
-        :param args: The direct sons in this expression tree; an iterable of expressions.
+        :param args: The direct sons in this expression tree; a tuple of expressions.
         :param payload: In some OperationKind contains the information about the expression; for an INT_EXP
-        contains the integer, for a FLUENT_EXP the fluent etc.
+            contains the integer, for a FLUENT_EXP the fluent etc.
         :return: The created expression.
         """
         content = up.model.fnode.FNodeContent(node_type, args, payload)
-        if content in self.expressions:
-            return self.expressions[content]
+        res = self.expressions.get(content, None)
+        if res is not None:
+            return res
         else:
             assert all(
-                a.environment == self.env for a in args
+                a.environment == self.environment for a in args
             ), "2 FNode in the same expression have different environments"
-            n = up.model.fnode.FNode(content, self._next_free_id, self.env)
+            n = up.model.fnode.FNode(content, self._next_free_id, self.environment)
             self._next_free_id += 1
             self.expressions[content] = n
-            self.env.type_checker.get_type(n)
+            self.environment.type_checker.get_type(n)
             return n
 
     def And(
         self, *args: Union[BoolExpression, Iterable[BoolExpression]]
     ) -> "up.model.fnode.FNode":
         """
-        Returns a conjunction of terms.
-        This function has polymorphic n-arguments:
-          - `And(a,b,c)`
-          - `And([a,b,c])`
-        Restriction: Arguments must be `boolean`.
-
-        :param *args: Either an `Iterable` of `boolean expressions`, like `[a, b, c]`, or an unpacked version
-        of it, like `a, b, c`.
-        :return: The `AND` expression created.
+        | Returns a conjunction of terms.
+        | This function has polymorphic n-arguments:
+
+            * ``And(a,b,c)``
+            * ``And([a,b,c])``
+
+        | Restriction: Arguments must be ``boolean``.
+
+        :param \*args: Either an ``Iterable`` of ``boolean`` expressions, like ``[a, b, c]``, or an unpacked version
+            of it, like ``a, b, c``.
+        :return: The ``AND`` expression created.
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.TRUE()
         elif len(tuple_args) == 1:
             return tuple_args[0]
         else:
             return self.create_node(node_type=OperatorKind.AND, args=tuple_args)
 
     def Or(
         self, *args: Union[BoolExpression, Iterable[BoolExpression]]
     ) -> "up.model.fnode.FNode":
         """
-        Returns an disjunction of terms.
-        This function has polymorphic n-arguments:
-          - `Or(a,b,c)`
-          - `Or([a,b,c])`
-        Restriction: Arguments must be `boolean`
-
-        :param *args: Either an `Iterable` of `boolean expressions`, like `[a, b, c]`, or an unpacked version
-        of it, like `a, b, c`.
-        :return: The `OR` expression created.
+        | Returns an disjunction of terms.
+        | This function has polymorphic n-arguments:
+
+            * ``Or(a,b,c)``
+            * ``Or([a,b,c])``
+
+        | Restriction: Arguments must be ``boolean``
+
+        :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+            of it, like ``a, b, c``.
+        :return: The ``OR`` expression created.
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.FALSE()
         elif len(tuple_args) == 1:
             return tuple_args[0]
         else:
             return self.create_node(node_type=OperatorKind.OR, args=tuple_args)
 
     def XOr(
         self, *args: Union[BoolExpression, Iterable[BoolExpression]]
     ) -> "up.model.fnode.FNode":
-        """Returns an exclusive disjunction of terms in CNF form.
-        This function has polimorphic n-arguments:
-          - XOr(a,b,c)
-          - XOr([a,b,c])
-        Restriction: Arguments must be boolean
+        """
+        | Returns an exclusive disjunction of terms in CNF form.
+        | This function has polimorphic n-arguments:
+
+            * XOr(a,b,c)
+            * XOr([a,b,c])
 
-        :param *args: Either an `Iterable` of `boolean expressions`, like `[a, b, c]`, or an unpacked version
-        of it, like `a, b, c`.
+        | Restriction: Arguments must be boolean
+
+        :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+            of it, like ``a, b, c``.
         :return: The exclusive disjunction in CNF form.
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.FALSE()
         elif len(tuple_args) == 1:
@@ -251,69 +277,73 @@
                     self.And([a] + [self.Not(o) for o in tuple_args if o is not a])
                 )
             return self.Or(new_args)
 
     def Not(self, expression: BoolExpression) -> "up.model.fnode.FNode":
         """
         Creates an expression of the form:
-                `not expression`
-        Restriction: `expression` must be of `boolean type`
+            ``not expression``
+
+        Restriction: ``expression`` must be of ``boolean type``
 
-        :param expression: The `boolean` expression of which the negation must be created.
-        :return: The created `NOT` expression.
+        :param expression: The ``boolean`` expression of which the negation must be created.
+        :return: The created ``Not`` expression.
         """
         (expression,) = self.auto_promote(expression)
         if expression.is_not():
             return expression.arg(0)
         return self.create_node(node_type=OperatorKind.NOT, args=(expression,))
 
     def Implies(
         self, left: BoolExpression, right: BoolExpression
     ) -> "up.model.fnode.FNode":
         """
         Creates an expression of the form:
-            `left -> right`
-        Restriction: `Left` and `Right` must be of `boolean type`
+            ``left -> right``
+
+        Restriction: ``Left`` and ``Right`` must be of ``boolean type``
 
-        :param left: The `boolean` expression acting as the premise of the `Implies`.
-        :param right: The `boolean` expression acting as the implied part of the `Implies`.
-        :return: The created `Implication`.
+        :param left: The ``boolean`` expression acting as the premise of the ``Implies``.
+        :param right: The ``boolean`` expression acting as the implied part of the ``Implies``.
+        :return: The created ``Implication``.
         """
         left, right = self.auto_promote(left, right)
         return self.create_node(node_type=OperatorKind.IMPLIES, args=(left, right))
 
     def Iff(
         self, left: BoolExpression, right: BoolExpression
     ) -> "up.model.fnode.FNode":
         """
         Creates an expression of the form:
-            `left <-> right`
-        Semantically, The expression is `True` only if `left` and `right` have the same value.
-        Restriction: `Left` and `Right` must be of `boolean type`
-
-        :param left: The `left` member of the `Iff expression`.
-        :param right: The `right` member of the `Iff expression`.
-        :return: The created `Iff` expression.
+            ``left <-> right``
+
+        Semantically, The expression is ``True`` only if ``left`` and ``right`` have the same value.
+        Restriction: ``Left`` and ``Right`` must be of ``boolean type``
+
+        :param left: The ``left`` member of the ``Iff expression``.
+        :param right: The ``right`` member of the ``Iff expression``.
+        :return: The created ``Iff`` expression.
         """
         left, right = self.auto_promote(left, right)
         return self.create_node(node_type=OperatorKind.IFF, args=(left, right))
 
     def Exists(
         self, expression: BoolExpression, *vars: "up.model.variable.Variable"
     ) -> "up.model.fnode.FNode":
         """
         Creates an expression of the form:
-            `Exists (var[0]... var[n]) | expression`
-        Restriction: expression must be of `boolean type` and
-                    vars must be of `Variable` type
-
-        :param expression: The main expression of the `existential`. The expression should contain
-            the given `variables`.
-        :param *vars: All the `Variables` appearing in the `existential` expression.
-        :return: The created `Existential` expression.
+            ``Exists (var[0]... var[n]) | expression``
+
+        Restriction: expression must be of ``boolean type`` and
+        vars must be of ``Variable`` type
+
+        :param expression: The main expression of the ``existential``. The expression should contain
+            the given ``variables``.
+        :param \*vars: All the ``Variables`` appearing in the ``existential`` expression.
+        :return: The created ``Existential`` expression.
         """
         expressions = tuple(self.auto_promote(expression))
         if len(vars) == 0:
             raise UPExpressionDefinitionError(
                 f"Exists of expression: {str(expression)} must be created with at least one variable, otherwise it is not needed."
             )
         for v in vars:
@@ -323,22 +353,23 @@
             node_type=OperatorKind.EXISTS, args=expressions, payload=vars
         )
 
     def Forall(
         self, expression: BoolExpression, *vars: "up.model.variable.Variable"
     ) -> "up.model.fnode.FNode":
         """Creates an expression of the form:
-            `Forall (var[0]... var[n]) | expression`
-        Restriction: expression must be of `boolean type` and
-                    vars must be of `Variable` type
-
-        :param expression: The main expression of the `universal` quantifier. The expression should contain
-            the given `variables`.
-        :param *vars: All the `Variables` appearing in the `universal` expression.
-        :return: The created `Forall` expression.
+            ``Forall (var[0]... var[n]) | expression``
+
+        Restriction: expression must be of ``boolean type`` and
+        vars must be of ``Variable`` type
+
+        :param expression: The main expression of the ``universal`` quantifier. The expression should contain
+            the given ``variables``.
+        :param \*vars: All the ``Variables`` appearing in the ``universal`` expression.
+        :return: The created ``Forall`` expression.
         """
         expressions = tuple(self.auto_promote(expression))
         if len(vars) == 0:
             raise UPExpressionDefinitionError(
                 f"Forall of expression: {str(expression)} must be created with at least one variable, otherwise it is not needed."
             )
         for v in vars:
@@ -346,323 +377,334 @@
                 raise UPTypeError("Expecting 'up.Variable', got %s", type(v))
         return self.create_node(
             node_type=OperatorKind.FORALL, args=expressions, payload=vars
         )
 
     def Always(self, expression: BoolExpression) -> "up.model.fnode.FNode":
         """Creates an expression of the form:
-            `Always(a)`
-        Restriction: expression must be of `boolean type` and with only one arg.
+            ``Always(a)``
 
-        :param expression: The `boolean` expression of the trajectory constraints.
-        :return: The created `Always` expression.
+        Restriction: expression must be of ``boolean type`` and with only one arg.
+
+        :param expression: The ``boolean`` expression of the trajectory constraints.
+        :return: The created ``Always`` expression.
         """
         expressions = tuple(self.auto_promote(expression))
         return self.create_node(node_type=OperatorKind.ALWAYS, args=expressions)
 
     def Sometime(self, expression: BoolExpression) -> "up.model.fnode.FNode":
         """Creates an expression of the form:
-            `Sometime(a)`
-        Restriction: expression must be of `boolean type` and with only one arg.
+            ``Sometime(a)``
+
+        Restriction: expression must be of ``boolean type`` and with only one arg.
 
-        :param expression: The `boolean` expression of the trajectory constraints.
-        :return: The created `Sometime` expression.
+        :param expression: The ``boolean`` expression of the trajectory constraints.
+        :return: The created ``Sometime`` expression.
         """
         expressions = tuple(self.auto_promote(expression))
         return self.create_node(node_type=OperatorKind.SOMETIME, args=expressions)
 
     def AtMostOnce(self, expression: BoolExpression) -> "up.model.fnode.FNode":
         """Creates an expression of the form:
-            `At-Most-Once(a, b)`
-        Restriction: expression must be of `boolean type` and with only two arg.
+            ``At-Most-Once(a, b)``
+
+        Restriction: expression must be of ``boolean type`` and with only two arg.
 
-        :param expression: The `boolean` expression of the trajectory constraints.
-        :return: The created `At-Most-Once(a, b)` expression.
+        :param expression: The ``boolean`` expression of the trajectory constraints.
+        :return: The created ``At-Most-Once(a, b)`` expression.
         """
         expressions = tuple(self.auto_promote(expression))
         return self.create_node(node_type=OperatorKind.AT_MOST_ONCE, args=expressions)
 
     def SometimeBefore(
         self, phi: BoolExpression, psi: BoolExpression
     ) -> "up.model.fnode.FNode":
         """Creates an expression of the form:
-            `Sometime-Before(a, b)`
-        Restriction: expression must be of `boolean type` and with only one args
+            ``Sometime-Before(a, b)``
 
-        :param expression: The `boolean` expression of the trajectory constraints.
-        :return: The created `Sometime` expression.
+        Restriction: expression must be of ``boolean type`` and with only one args
+
+        :param expression: The ``boolean`` expression of the trajectory constraints.
+        :return: The created ``Sometime`` expression.
         """
         expressions = tuple(self.auto_promote(phi, psi))
         return self.create_node(
             node_type=OperatorKind.SOMETIME_BEFORE, args=expressions
         )
 
     def SometimeAfter(
         self, phi: BoolExpression, psi: BoolExpression
     ) -> "up.model.fnode.FNode":
         """Creates an expression of the form:
-            `Sometime-After(a, b)`
-        Restriction: expression must be of `boolean type` and with only two arg.
+            ``Sometime-After(a, b)``
+
+        Restriction: expression must be of ``boolean type`` and with only two arg.
 
-        :param expression: The `boolean` expression of the trajectory constraints.
-        :return: The created `Sometime-After(a, b)` expression.
+        :param expression: The ``boolean`` expression of the trajectory constraints.
+        :return: The created ``Sometime-After(a, b)`` expression.
         """
         expressions = tuple(self.auto_promote(phi, psi))
         return self.create_node(node_type=OperatorKind.SOMETIME_AFTER, args=expressions)
 
     def FluentExp(
-        self, fluent: "up.model.fluent.Fluent", params: Iterable[Expression] = tuple()
+        self, fluent: "up.model.fluent.Fluent", params: Sequence[Expression] = tuple()
     ) -> "up.model.fnode.FNode":
         """
-        Creates an expression for the given `fluent` and `parameters`.
-        Restriction: `parameters type` must be compatible with the `Fluent` :func:`signature <unified_planning.model.Fluent.signature>`
+        | Creates an expression for the given ``fluent`` and ``parameters``.
+        | Restriction: ``parameters type`` must be compatible with the ``Fluent`` :func:``signature <unified_planning.model.Fluent.signature>``
 
-        :param fluent: The `Fluent` that will be set as the `payload` of this expression.
-        :param params: The Iterable of expressions acting as `parameters` for this `Fluent`; mainly the parameters will
-            be :class:`Objects <unified_planning.model.Object>` (when the `FluentExp` is grounded) or
-            :func:`Action parameters <unified_planning.model.Action.parameters>` (when the `FluentExp` is lifted).
-        :return: The created `Fluent` Expression.
+        :param fluent: The ``Fluent`` that will be set as the ``payload`` of this expression.
+        :param params: The Sequence of expressions acting as ``parameters`` for this ``Fluent``; mainly the parameters will
+            be :class:``Objects <unified_planning.model.Object>`` (when the ``FluentExp`` is grounded) or
+            :func:``Action parameters <unified_planning.model.Action.parameters>`` (when the ``FluentExp`` is lifted).
+        :return: The created ``Fluent`` Expression.
         """
-        assert fluent.environment == self.env
+        assert fluent.environment == self.environment
         params_exp = self.auto_promote(params)
         if fluent.arity != len(params_exp):
             raise UPExpressionDefinitionError(
-                f"In FluentExp, fluent has arity {fluent.arity} but {len(params_exp)} parameters were passed."
+                f"In FluentExp, fluent: {fluent.name} has arity {fluent.arity} but {len(params_exp)} parameters were passed."
             )
         return self.create_node(
             node_type=OperatorKind.FLUENT_EXP, args=tuple(params_exp), payload=fluent
         )
 
     def Dot(
         self,
         agent: "up.model.multi_agent.Agent",
         fluent_exp: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
     ) -> "up.model.fnode.FNode":
         """
-        Creates an expression for the given `agent` and `fluent_exp`.
-        Restriction: agent must be of `agent type` and fluent_exp must be of `fluentExp type`
+        Creates an expression for the given ``agent`` and ``fluent_exp``.
+        Restriction: agent must be of ``agent type`` and fluent_exp must be of ``fluentExp type``
 
-        :param agent: The `Agent` that will be set as the `payload` of this expression.
-        :param fluent_exp: The `Fluent_exp` that will be set as the `args` of this expression.
-        :return: The created `Dot` Expression.
+        :param agent: The ``Agent`` that will be set as the ``payload`` of this expression.
+        :param fluent_exp: The ``Fluent_exp`` that will be set as the ``args`` of this expression.
+        :return: The created ``Dot`` Expression.
         """
-        assert agent.env == self.env
+        assert agent.environment == self.environment
         (fluent_exp,) = self.auto_promote(fluent_exp)
         return self.create_node(
             node_type=OperatorKind.DOT, args=(fluent_exp,), payload=agent
         )
 
     def ParameterExp(
         self, param: "up.model.parameter.Parameter"
     ) -> "up.model.fnode.FNode":
         """
         Returns an expression for the given :func:`Action parameter <unified_planning.model.Action.parameters>`.
 
-        :param param: The `Parameter` that must be promoted to `FNode`.
-        :return: The `FNode` containing the given `param` as his payload.
+        :param param: The ``Parameter`` that must be promoted to ``FNode``.
+        :return: The ``FNode`` containing the given ``param`` as his payload.
         """
         return self.create_node(
             node_type=OperatorKind.PARAM_EXP, args=tuple(), payload=param
         )
 
     def VariableExp(self, var: "up.model.variable.Variable") -> "up.model.fnode.FNode":
         """
-        Returns an expression for the given `Variable`.
+        Returns an expression for the given ``Variable``.
 
-        :param var: The `Variable` that must be promoted to `FNode`.
-        :return: The `FNode` containing the given `variable` as his payload.
+        :param var: The ``Variable`` that must be promoted to ``FNode``.
+        :return: The ``FNode`` containing the given ``variable`` as his payload.
         """
-        assert var.environment == self.env
+        assert var.environment == self.environment
         return self.create_node(
             node_type=OperatorKind.VARIABLE_EXP, args=tuple(), payload=var
         )
 
     def ObjectExp(self, obj: "up.model.object.Object") -> "up.model.fnode.FNode":
         """
         Returns an expression for the given object.
 
-        :param obj: The `Object` that must be promoted to `FNode`.
-        :return: The `FNode` containing the given object as his payload.
+        :param obj: The ``Object`` that must be promoted to ``FNode``.
+        :return: The ``FNode`` containing the given object as his payload.
         """
-        assert obj.environment == self.env
+        assert obj.environment == self.environment
         return self.create_node(
             node_type=OperatorKind.OBJECT_EXP, args=tuple(), payload=obj
         )
 
     def TimingExp(self, timing: "up.model.timing.Timing") -> "up.model.fnode.FNode":
         """
-        Returns an expression for the given `Timing`.
+        Returns an expression for the given ``Timing``.
 
-        :param timing: The `Timing` that must be promoted to `FNode`.
-        :return: The `FNode` containing the given `timing` as his payload.
+        :param timing: The ``Timing`` that must be promoted to ``FNode``.
+        :return: The ``FNode`` containing the given ``timing`` as his payload.
         """
         return self.create_node(
             node_type=OperatorKind.TIMING_EXP, args=tuple(), payload=timing
         )
 
     def TRUE(self) -> "up.model.fnode.FNode":
-        """Return the boolean constant `True`."""
+        """Return the boolean constant ``True``."""
         return self.true_expression
 
     def FALSE(self) -> "up.model.fnode.FNode":
-        """Return the boolean constant `False`."""
+        """Return the boolean constant ``False``."""
         return self.false_expression
 
     def Bool(self, value: bool) -> "up.model.fnode.FNode":
         """
         Return a boolean constant.
 
-        :param value: The boolean value that must be promoted to `FNode`.
-        :return: The `FNode` containing the given `value` as his payload.
+        :param value: The boolean value that must be promoted to ``FNode``.
+        :return: The ``FNode`` containing the given ``value`` as his payload.
         """
-        if type(value) != bool:
+        if not isinstance(value, bool):
             raise UPTypeError("Expecting bool, got %s" % type(value))
 
         if value:
             return self.true_expression
         else:
             return self.false_expression
 
     def Int(self, value: int) -> "up.model.fnode.FNode":
         """
-        Return an `int` constant.
+        Return an ``int`` constant.
 
-        :param value: The integer that must be promoted to `FNode`.
-        :return: The `FNode` containing the given `integer` as his payload.
+        :param value: The integer that must be promoted to ``FNode``.
+        :return: The ``FNode`` containing the given ``integer`` as his payload.
         """
-        if type(value) != int:
+        if not isinstance(value, int):
             raise UPTypeError("Expecting int, got %s" % type(value))
         return self.create_node(
             node_type=OperatorKind.INT_CONSTANT, args=tuple(), payload=value
         )
 
     def Real(self, value: Fraction) -> "up.model.fnode.FNode":
         """
-        Return a `real` constant.
+        Return a ``real`` constant.
 
-        :param value: The `Fraction` that must be promoted to `FNode`.
-        :return: The `FNode` containing the given `value` as his payload.
+        :param value: The ``Fraction`` that must be promoted to ``FNode``.
+        :return: The ``FNode`` containing the given ``value`` as his payload.
         """
-        if type(value) != Fraction:
+        if not isinstance(value, Fraction):
             raise UPTypeError("Expecting Fraction, got %s" % type(value))
         return self.create_node(
             node_type=OperatorKind.REAL_CONSTANT, args=tuple(), payload=value
         )
 
     def Plus(
         self, *args: Union[Expression, Iterable[Expression]]
     ) -> "up.model.fnode.FNode":
         """
         Creates an expression of the form:
-        `args[0] + ... + args[n]`
+            ``args[0] + ... + args[n]``
 
-        :param *args: Either an `Iterable` of expressions, like `[a, b, 3]`, or an unpacked version
-            of it, like `a, b, 3`.
-        :return: The `PLUS` expression created. (like `a + b + 3`)
+        :param \*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
+            of it, like ``a, b, 3``.
+        :return: The ``PLUS`` expression created. (like ``a + b + 3``)
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.Int(0)
         elif len(tuple_args) == 1:
             return tuple_args[0]
         else:
             return self.create_node(node_type=OperatorKind.PLUS, args=tuple_args)
 
     def Minus(self, left: Expression, right: Expression) -> "up.model.fnode.FNode":
         """
-        Creates an expression of the form: `left - right`.
+        Creates an expression of the form: ``left - right``.
 
-        :param left: The `Minus minuend`.
-        :param right: The `Minus subtrahend`.
-        :return: The created `Minus` expression.
+        :param left: The ``Minus minuend``.
+        :param right: The ``Minus subtrahend``.
+        :return: The created ``Minus`` expression.
         """
         left, right = self.auto_promote(left, right)
         return self.create_node(node_type=OperatorKind.MINUS, args=(left, right))
 
     def Times(
         self, *args: Union[Expression, Iterable[Expression]]
     ) -> "up.model.fnode.FNode":
         """
         Creates an expression of the form:
-        `args[0] * ... * args[n]`
+            ``args[0] * ... * args[n]``
 
-        :param *args: Either an `Iterable` of expressions, like `[a, b, 3]`, or an unpacked version
-            of it, like `a, b, 3`.
-        :return: The `TIMES` expression created. (like `a * b * 3`)
+        :param \*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
+            of it, like ``a, b, 3``.
+        :return: The ``TIMES`` expression created. (like ``a * b * 3``)
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.Int(1)
         elif len(tuple_args) == 1:
             return tuple_args[0]
         else:
             return self.create_node(node_type=OperatorKind.TIMES, args=tuple_args)
 
     def Div(self, left: Expression, right: Expression) -> "up.model.fnode.FNode":
         """
-        Creates an expression of the form: `left / right`.
+        Creates an expression of the form:
+            ``left / right``
 
-        :param left: The `Div dividend`.
-        :param right: The `Div divisor`.
-        :return: The created `DIV` expression.
+        :param left: The ``Div dividend``.
+        :param right: The ``Div divisor``.
+        :return: The created ``DIV`` expression.
         """
         left, right = self.auto_promote(left, right)
         return self.create_node(node_type=OperatorKind.DIV, args=(left, right))
 
     def LE(self, left: Expression, right: Expression) -> "up.model.fnode.FNode":
         """
-        Creates an expression of the form: `left <= right`.
+        Creates an expression of the form:
+            ``left <= right``.
 
-        :param left: The left side of the `<=`.
-        :param right: The right side of the `<=`.
-        :return: The created `LE` expression.
+        :param left: The left side of the ``<=``.
+        :param right: The right side of the ``<=``.
+        :return: The created ``LE`` expression.
         """
         left, right = self.auto_promote(left, right)
         return self.create_node(node_type=OperatorKind.LE, args=(left, right))
 
     def GE(self, left: Expression, right: Expression) -> "up.model.fnode.FNode":
         """
-        Creates an expression of the form: `left >= right`.
+        Creates an expression of the form:
+            ``left >= right``.
 
-        :param left: The left side of the `>=`.
-        :param right: The right side of the `>=`.
-        :return: The created `GE` expression.
+        :param left: The left side of the ``>=``.
+        :param right: The right side of the ``>=``.
+        :return: The created ``GE`` expression.
         """
         left, right = self.auto_promote(left, right)
         return self.create_node(node_type=OperatorKind.LE, args=(right, left))
 
     def LT(self, left: Expression, right: Expression) -> "up.model.fnode.FNode":
         """
-        Creates an expression of the form: `left < right`.
+        Creates an expression of the form:
+            ``left < right``.
 
-        :param left: The left side of the `<`.
-        :param right: The right side of the `<`.
-        :return: The created `LT` expression.
+        :param left: The left side of the ``<``.
+        :param right: The right side of the ``<``.
+        :return: The created ``LT`` expression.
         """
         left, right = self.auto_promote(left, right)
         return self.create_node(node_type=OperatorKind.LT, args=(left, right))
 
     def GT(self, left: Expression, right: Expression) -> "up.model.fnode.FNode":
         """
-        Creates an expression of the form: `left > right`.
+        Creates an expression of the form:
+            ``left > right``.
 
-        :param left: The left side of the `>`.
-        :param right: The right side of the `>`.
-        :return: The created `GT` expression.
+        :param left: The left side of the ``>``.
+        :param right: The right side of the ``>``.
+        :return: The created ``GT`` expression.
         """
         left, right = self.auto_promote(left, right)
         return self.create_node(node_type=OperatorKind.LT, args=(right, left))
 
     def Equals(self, left: Expression, right: Expression) -> "up.model.fnode.FNode":
         """
-        Creates an expression of the form: `left == right`.
+        Creates an expression of the form:
+            ``left == right``.
 
-        NOTE: Is not valid for boolean expression, for those use `Iff`.
+        NOTE: Is not valid for boolean expression, for those use ``Iff``.
 
-        :param left: The left side of the `==`.
-        :param right: The right side of the `==`.
-        :return: The created `Equals` expression.
+        :param left: The left side of the ``==``.
+        :param right: The right side of the ``==``.
+        :return: The created ``Equals`` expression.
         """
         left, right = self.auto_promote(left, right)
         return self.create_node(node_type=OperatorKind.EQUALS, args=(left, right))
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/fnode.py` & `unified_planning-0.6.0/unified_planning/model/fnode.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """FNode are the building blocks of expressions."""
 
 import unified_planning
 import unified_planning.model.fluent
 import collections
 from unified_planning.environment import Environment
 from unified_planning.model.operators import OperatorKind
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Set, Union
 from fractions import Fraction
 
 FNodeContent = collections.namedtuple("FNodeContent", ["node_type", "args", "payload"])
 
 
 class FNode(object):
 
@@ -149,14 +149,18 @@
         return self._content.args
 
     @property
     def type(self) -> "unified_planning.model.Type":
         """Returns the `Type` of this expression."""
         return self._env.type_checker.get_type(self)
 
+    def get_contained_names(self) -> Set[str]:
+        """Returns all the names contained in this expression."""
+        return self._env.names_extractor.extract_names(self)
+
     def arg(self, idx: int) -> "FNode":
         """
         Return the given subexpression at the given position.
 
         :param idx: The `index` of the wanted subexpression.
         :return: The expression at the position `idx`.
         """
@@ -230,14 +234,33 @@
         """
         Returns the simplified version of this expression.
 
         The simplification is done just by constant propagation by the :class:`~unified_planning.model.walkers.Simplifier`
         """
         return self._env.simplifier.simplify(self)
 
+    def substitute(
+        self,
+        substitutions: Dict[
+            "unified_planning.model.expression.Expression",
+            "unified_planning.model.expression.Expression",
+        ],
+    ):
+        """
+        Returns the version of this expression where every expression that is a key of the substitutions
+        map is substituted with it's value in the map.
+
+        NOTE: check the :class:`~unified_planning.model.walkers.Substituter` documentation for more details!
+
+        :param substitutions: The mapping of expressions that must be substituted.
+        :return: The expression where every instance of a key value in the substitutions map
+            is substituted with it's value.
+        """
+        return self._env.substituter.substitute(self, substitutions)
+
     def is_bool_constant(self) -> bool:
         """Test whether the expression is a `boolean` constant."""
         return self.node_type == OperatorKind.BOOL_CONSTANT
 
     def is_int_constant(self) -> bool:
         """Test whether the expression is an `integer` constant."""
         return self.node_type == OperatorKind.INT_CONSTANT
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/htn/hierarchical_problem.py` & `unified_planning-0.6.0/unified_planning/model/htn/hierarchical_problem.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,42 +9,39 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
-from fractions import Fraction
 from typing import Optional, List, Union, Dict
+from warnings import warn
 
 import unified_planning as up
+from unified_planning.model.expression import ConstantExpression
 from unified_planning.model.htn.method import Method
 from unified_planning.model.htn.task import Task
-from unified_planning.model.htn.task_network import TaskNetwork
+from unified_planning.model.htn.task_network import TaskNetwork, AbstractTaskNetwork
+from unified_planning.exceptions import UPProblemDefinitionError
 
 
 class HierarchicalProblem(up.model.problem.Problem):
     def __init__(
         self,
         name: Optional[str] = None,
-        env: Optional["up.environment.Environment"] = None,
+        environment: Optional["up.environment.Environment"] = None,
         *,
         initial_defaults: Dict[
             "up.model.types.Type",
-            Union[
-                "up.model.fnode.FNode",
-                "up.model.object.Object",
-                bool,
-                int,
-                float,
-                Fraction,
-            ],
+            ConstantExpression,
         ] = {},
     ):
-        super().__init__(name=name, env=env, initial_defaults=initial_defaults)
+        super().__init__(
+            name=name, environment=environment, initial_defaults=initial_defaults
+        )
         self._abstract_tasks: OrderedDict[str, Task] = OrderedDict()
         self._methods: OrderedDict[str, Method] = OrderedDict()
         self._initial_task_network = TaskNetwork()
 
     def __repr__(self):
         s = [super().__repr__()]
         s.append("abstract tasks = [\n")
@@ -87,16 +84,19 @@
         new_p._timed_effects = {
             t: [e.clone() for e in el] for t, el in self._timed_effects.items()
         }
         new_p._timed_goals = {i: [g for g in gl] for i, gl in self._timed_goals.items()}
         new_p._goals = self._goals[:]
         new_p._metrics = []
         for m in self._metrics:
-            if isinstance(m, up.model.metrics.MinimizeActionCosts):
-                costs = {new_p.action(a.name): c for a, c in m.costs.items()}
+            if m.is_minimize_action_costs():
+                assert isinstance(m, up.model.metrics.MinimizeActionCosts)
+                costs: Dict["up.model.Action", "up.model.Expression"] = {
+                    new_p.action(a.name): c for a, c in m.costs.items()
+                }
                 new_p._metrics.append(up.model.metrics.MinimizeActionCosts(costs))
             else:
                 new_p._metrics.append(m)
         new_p._initial_defaults = self._initial_defaults.copy()
         new_p._fluents_defaults = self._fluents_defaults.copy()
         new_p._initial_task_network = self._initial_task_network.clone()
         new_p._methods = self._methods.copy()
@@ -107,16 +107,64 @@
     def kind(self) -> "up.model.problem_kind.ProblemKind":
         """Returns the problem kind of this planning problem.
 
         IMPORTANT NOTE: this property does a lot of computation, so it should be called as
         minimum time as possible."""
         self._kind = super().kind
         self._kind.set_problem_class("HIERARCHICAL")
+        (TO, PO, TEMPORAL) = (0, 1, 2)
+
+        def lvl(tn: AbstractTaskNetwork):
+            """Determines the expressivity level of temporal constraints within a task network"""
+            if tn.total_order() is not None:
+                return TO
+            elif tn.partial_order() is not None:
+                return PO
+            else:
+                return TEMPORAL
+
+        ordering_kind = lvl(self.task_network)
+        if len(self.task_network.variables) > 0:
+            self._kind.set_hierarchical("INITIAL_TASK_NETWORK_VARIABLES")
+        if len(self.task_network.non_temporal_constraints()) > 0:
+            self._kind.set_hierarchical("TASK_NETWORK_CONSTRAINTS")
+
+        linear_checker = up.model.walkers.linear_checker.LinearChecker(self)
+        for method in self.methods:
+            ordering_kind = max(ordering_kind, lvl(method))
+            for method_cond in method.preconditions:
+                self._kind.set_hierarchical("METHOD_PRECONDITIONS")
+                self._update_problem_kind_condition(method_cond, linear_checker)
+            if len(method.non_temporal_constraints()) > 0:
+                self._kind.set_hierarchical("TASK_NETWORK_CONSTRAINTS")
+
+        if ordering_kind == TO:
+            self._kind.set_hierarchical("TASK_ORDER_TOTAL")
+        elif ordering_kind == PO:
+            self._kind.set_hierarchical("TASK_ORDER_PARTIAL")
+        else:
+            self._kind.set_hierarchical("TASK_ORDER_TEMPORAL")
+
         return self._kind
 
+    def has_name(self, name: str) -> bool:
+        """
+        Returns `True` if the given `name` is already in the `HierarchicalProblem`, `False` otherwise.
+
+        :param name: The target name to find in the `HierarchicalProblem`.
+        :return: `True` if the given `name` is already in the `HierarchicalProblem`, `False` otherwise."""
+        return (
+            self.has_action(name)
+            or self.has_fluent(name)
+            or self.has_object(name)
+            or self.has_type(name)
+            or self.has_task(name)
+            or name in self._methods
+        )
+
     @property
     def tasks(self) -> List[Task]:
         return list(self._abstract_tasks.values())
 
     def get_task(self, task_name: str) -> Task:
         return self._abstract_tasks[task_name]
 
@@ -124,17 +172,22 @@
         return task_name in self._abstract_tasks
 
     def add_task(self, task: Union[Task, str], **kwargs: "up.model.types.Type") -> Task:
         if isinstance(task, str):
             task = Task(task, _parameters=OrderedDict(**kwargs))
         else:
             assert len(kwargs) == 0
-        assert (
-            task.name not in self._abstract_tasks
-        ), f"A task with name '{task.name}' already exists."
+        if self.has_name(task.name):
+            msg = f"Name of task {task.name} already defined! Different elements of a problem can have the same name if the environment flag error_used_named is disabled."
+            if self._env.error_used_name or any(
+                task.name == t for t in self._abstract_tasks
+            ):
+                raise UPProblemDefinitionError(msg)
+            else:
+                warn(msg)
         self._abstract_tasks[task.name] = task
         for param in task.parameters:
             if param.type.is_user_type():
                 self._add_user_type(param.type)
         return task
 
     @property
@@ -144,17 +197,22 @@
     def method(self, method_name) -> Method:
         return self._methods[method_name]
 
     def add_method(self, method: Method):
         assert (
             method.achieved_task is not None
         ), f"No achieved task was specified for this method."
-        assert (
-            method.name not in self._methods
-        ), f"A method with name '{method.name}' already exists."
+        if self.has_name(method.name):
+            msg = f"Name of method {method.name} already defined! Different elements of a problem can have the same name if the environment flag error_used_named is disabled."
+            if self._env.error_used_name or any(
+                method.name == m for m in self._methods
+            ):
+                raise UPProblemDefinitionError(msg)
+            else:
+                warn(msg)
         assert (
             method.achieved_task.task.name in self._abstract_tasks
         ), f"Method is associated to an unregistered task '{method.achieved_task.task.name}'"
         self._methods[method.name] = method
         for param in method.parameters:
             if param.type.is_user_type():
                 self._add_user_type(param.type)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/htn/method.py` & `unified_planning-0.6.0/unified_planning/model/htn/method.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,20 +17,19 @@
 A Method has a name, a list of Parameters, a list of conditions
 and a list of subtasks.
 """
 from collections import OrderedDict
 from typing import List, Union, Optional
 
 import unified_planning as up
-from unified_planning.environment import get_env, Environment
+from unified_planning.environment import Environment
 from unified_planning.exceptions import UPUnboundedVariablesError, UPValueError
+from unified_planning.model.htn.task_network import AbstractTaskNetwork
 from unified_planning.model.parameter import Parameter
-from unified_planning.model.action import Action
-from unified_planning.model.htn.task import Task, Subtask
-from unified_planning.model.timing import Timing, Timepoint
+from unified_planning.model.htn.task import Task
 from unified_planning.model.expression import Expression
 
 
 class ParameterizedTask:
     """A task instantiated with some parameters."""
 
     def __init__(self, task: Task, *params: Parameter):
@@ -57,33 +56,31 @@
         return self._task
 
     @property
     def parameters(self) -> List[up.model.parameter.Parameter]:
         return self._params
 
 
-class Method:
-    """This is the method interface."""
+class Method(AbstractTaskNetwork):
+    """HTN Method: encoding of a procedure for achieving a high-level task."""
 
     def __init__(
         self,
         _name: str,
         _parameters: Optional[
             "Union[OrderedDict[str, up.model.types.Type], List[Parameter]]"
         ] = None,
         _env: Optional[Environment] = None,
         **kwargs: "up.model.types.Type",
     ):
-        self._env = get_env(_env)
+        super(Method, self).__init__(_env)
         self._task: Optional[ParameterizedTask] = None
         self._name = _name
         self._parameters: "OrderedDict[str, Parameter]" = OrderedDict()
         self._preconditions: List[up.model.fnode.FNode] = []
-        self._constraints: List[up.model.fnode.FNode] = []
-        self._subtasks: List[Subtask] = []
         if _parameters is None:
             for n, t in kwargs.items():
                 self._parameters[n] = Parameter(n, t, self._env)
         elif isinstance(_parameters, List):
             assert len(kwargs) == 0
             for p in _parameters:
                 self._parameters[p.name] = p
@@ -104,48 +101,51 @@
             else:
                 s.append(", ")
             s.append(str(p))
         if not first:
             s.append(")")
         s.append(" {\n")
         s.append(f"  task = {self._task}\n")
-        s.append("  preconditions = [\n")
-        for c in self.preconditions:
-            s.append(f"    {str(c)}\n")
-        s.append("  ]\n")
-        s.append("  constraints = [\n")
-        for c in self.constraints:
-            s.append(f"    {str(c)}\n")
-        s.append("  ]\n")
-        s.append("  subtasks = [\n")
-        for st in self.subtasks:
-            s.append(f"      {str(st)}\n")
-        s.append("  ]\n")
+        if len(self.preconditions) > 0:
+            s.append("  preconditions = [\n")
+            for c in self.preconditions:
+                s.append(f"    {str(c)}\n")
+            s.append("  ]\n")
+        if len(self.constraints) > 0:
+            s.append("  constraints = [\n")
+            for c in self.constraints:
+                s.append(f"    {str(c)}\n")
+            s.append("  ]\n")
+        if len(self.subtasks) > 0:
+            s.append("  subtasks = [\n")
+            for st in self.subtasks:
+                s.append(f"      {str(st)}\n")
+            s.append("  ]\n")
         s.append("}")
         return "".join(s)
 
     def __eq__(self, oth: object) -> bool:
         if not isinstance(oth, Method):
             return False
         return (
             self._env == oth._env
             and self._name == oth._name
             and self._parameters == oth._parameters
             and self._task == oth._task
             and set(self._preconditions) == set(oth._preconditions)
-            and set(self._subtasks) == set(oth._subtasks)
-            and set(self._constraints) == set(oth._constraints)
+            and set(self.subtasks) == set(oth.subtasks)
+            and set(self.constraints) == set(oth.constraints)
         )
 
     def __hash__(self) -> int:
         res = hash(self._name)
         res += hash(self._task)
         res += sum(map(hash, self.parameters))
         res += sum(map(hash, self._preconditions))
-        res += sum(map(hash, self._constraints))
+        res += sum(map(hash, self.constraints))
         res += sum(map(hash, self.subtasks))
         return res
 
     @property
     def name(self) -> str:
         """Returns the action name."""
         return self._name
@@ -201,20 +201,55 @@
 
     @property
     def parameters(self) -> List[Parameter]:
         """Returns the list of the method's parameters."""
         return list(self._parameters.values())
 
     def parameter(self, name: str) -> Parameter:
-        """Returns the parameter of the action with the given name."""
+        """
+        Returns the `parameter` of the `Method` with the given `name`.
+
+        Example
+        -------
+        >>> from unified_planning.shortcuts import *
+        >>> from unified_planning.model.htn import *
+        >>> location_type = UserType("Location")
+        >>> robot_type = UserType("Robot")
+        >>> goto = Method("goto", robot=robot_type, target=location_type)
+        >>> goto.parameter("robot")  # return the "robot" parameter of the method, with type "Robot"
+        Robot robot
+        >>> goto.parameter("target")
+        Location target
+
+        If a parameter's name (1) does not conflict with an existing attribute of `Method` and (2) does not start with '_'
+        it can also be accessed as if it was an attribute of the method. For instance:
+
+        >>> goto.target
+        Location target
+
+        :param name: The `name` of the target `parameter`.
+        :return: The `parameter` of the `Method` with the given `name`.
+        """
         for param in self.parameters:
             if param.name == name:
                 return param
         raise UPValueError(f"Unknown parameter name: {name}")
 
+    def __getattr__(self, parameter_name: str) -> "up.model.parameter.Parameter":
+        if parameter_name.startswith("_"):
+            # guard access as pickling relies on attribute error to be thrown even when
+            # no attributes of the object have been set.
+            # In this case accessing `self._name` or `self._parameters`, would re-invoke __getattr__
+            raise AttributeError(f"Method has no attribute '{parameter_name}'")
+        if parameter_name not in self._parameters:
+            raise AttributeError(
+                f"Method '{self.name}' has no attribute or parameter '{parameter_name}'"
+            )
+        return self._parameters[parameter_name]
+
     @property
     def preconditions(self) -> List["up.model.fnode.FNode"]:
         """Returns the list of the method's preconditions."""
         return self._preconditions
 
     def add_precondition(self, precondition: Expression):
         """Adds the given method precondition."""
@@ -225,82 +260,7 @@
         free_vars = self._env.free_vars_oracle.get_free_variables(precondition_exp)
         if len(free_vars) != 0:
             raise UPUnboundedVariablesError(
                 f"The precondition {str(precondition_exp)} has unbounded variables:\n{str(free_vars)}"
             )
         if precondition_exp not in self._preconditions:
             self._preconditions.append(precondition_exp)
-
-    @property
-    def constraints(self) -> List["up.model.fnode.FNode"]:
-        """Returns the list of the method's constraints."""
-        return self._constraints
-
-    def add_constraint(self, constraint: Expression):
-        """Adds the given constraint to the method."""
-        (constraint_exp,) = self._env.expression_manager.auto_promote(constraint)
-        assert self._env.type_checker.get_type(constraint_exp).is_bool_type()
-        if constraint_exp == self._env.expression_manager.TRUE():
-            return
-        free_vars = self._env.free_vars_oracle.get_free_variables(constraint_exp)
-        if len(free_vars) != 0:
-            raise UPUnboundedVariablesError(
-                f"The constraint {str(constraint_exp)} has unbounded variables:\n{str(free_vars)}"
-            )
-        if constraint_exp not in self._constraints:
-            self._constraints.append(constraint_exp)
-
-    @property
-    def subtasks(self) -> List["Subtask"]:
-        """Returns the list of the method's subtasks."""
-        return self._subtasks
-
-    def add_subtask(
-        self,
-        subtask: Union[Subtask, Action, Task],
-        *args: Expression,
-        ident: Optional[str] = None,
-    ) -> Subtask:
-        """Adds a subtask to this method, with no particular ordering relative to the existing ones."""
-        if not isinstance(subtask, Subtask):
-            parameters = self._env.expression_manager.auto_promote(*args)
-            subtask = Subtask(subtask, *parameters, ident=ident)
-        else:
-            assert len(args) == 0
-        assert isinstance(subtask, Subtask)
-        assert all([subtask.identifier != prev.identifier for prev in self.subtasks])
-        self._subtasks.append(subtask)
-        return subtask
-
-    def get_subtask(self, ident: str) -> Subtask:
-        """Returns the subtask with the given identifier."""
-        for st in self._subtasks:
-            if st.identifier == ident:
-                return st
-        raise ValueError(f"Method {self._name} has not subtask with identifier {ident}")
-
-    def set_ordered(self, *subtasks: Subtask):
-        """Imposes a sequential order between the given subtasks."""
-        if len(subtasks) < 2:
-            return
-        prev = subtasks[0]
-        for i in range(1, len(subtasks)):
-            next = subtasks[i]
-            self.set_strictly_before(prev, next)
-            prev = next
-
-    def set_strictly_before(
-        self,
-        lhs: Union[Subtask, Timepoint, Timing],
-        rhs: Union[Subtask, Timepoint, Timing],
-    ):
-        if isinstance(lhs, Subtask):
-            lhs = lhs.end
-        if isinstance(lhs, Timepoint):
-            lhs = Timing(timepoint=lhs, delay=0)
-        assert isinstance(lhs, Timing)
-        if isinstance(rhs, Subtask):
-            rhs = rhs.start
-        if isinstance(rhs, Timepoint):
-            rhs = Timing(timepoint=rhs, delay=0)
-        assert isinstance(rhs, Timing)
-        self.add_constraint(self._env.expression_manager.LT(lhs, rhs))
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/htn/task.py` & `unified_planning-0.6.0/unified_planning/model/htn/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 """
 This module defines the Task class.
 A Task has a name and a signature that defines the types of its parameters.
 """
 
 import unified_planning as up
-from unified_planning.environment import get_env, Environment
+from unified_planning.environment import get_environment, Environment
 from typing import List, OrderedDict, Optional, Union
 from unified_planning.model.fnode import FNode
 from unified_planning.model.action import Action
 from unified_planning.model.timing import Timepoint, TimepointKind
 from unified_planning.model.types import Type
 from unified_planning.model.expression import Expression
 from unified_planning.model.parameter import Parameter
@@ -34,15 +34,15 @@
     def __init__(
         self,
         name: str,
         _parameters: Optional[Union[OrderedDict[str, Type], List[Parameter]]] = None,
         _env: Optional[Environment] = None,
         **kwargs: Type,
     ):
-        self._env = get_env(_env)
+        self._env = get_environment(_env)
         self._name = name
         self._parameters: List[Parameter] = []
         if _parameters is not None:
             assert len(kwargs) == 0
             if isinstance(_parameters, OrderedDict):
                 for param_name, param_type in _parameters.items():
                     self._parameters.append(
@@ -101,26 +101,30 @@
     def __init__(
         self,
         _task: Union[Action, Task],
         *args: Expression,
         ident: Optional[str] = None,
         _env: Optional[Environment] = None,
     ):
-        self._env = get_env(_env)
+        self._env = get_environment(_env)
         self._task = _task
         self._ident: str
         if ident is not None:
             self._ident = ident
         else:
             # we have to create an unambiguous identifier as there might otherwise identical tasks
             global _task_id_counter
             _task_id_counter += 1
             self._ident = f"_t{_task_id_counter}"
         self._args = self._env.expression_manager.auto_promote(*args)
-        assert len(self._args) == len(self._task.parameters)
+
+        if len(self._args) != len(self._task.parameters):
+            raise ValueError(
+                f"Wrong number of arguments. Expected: {self._task.parameters}. Provided: {self._args}"
+            )
 
     def __repr__(self):
         params = ", ".join([str(a) for a in self._args])
         return f"{self.identifier}: {self._task.name}({params})"
 
     def __eq__(self, other):
         if not isinstance(other, Subtask):
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/htn/task_network.py` & `unified_planning-0.6.0/unified_planning/model/scheduling/chronicle.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,153 +1,150 @@
-# Copyright 2022 AIPlan4EU project
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-from collections import OrderedDict
-from typing import List, Union, Optional
-
-from unified_planning.environment import get_env, Environment
-from unified_planning.model.timing import Timing
-from unified_planning.model.parameter import Parameter
-from unified_planning.model.fnode import FNode
+from typing import Optional, List, OrderedDict, Union
+
+import unified_planning as up
+from unified_planning import Environment
+from unified_planning.model import Parameter
+from unified_planning.model.mixins.timed_conds_effs import TimedCondsEffs
 from unified_planning.model.types import Type
-from unified_planning.model.expression import Expression
-from unified_planning.model.operators import OperatorKind
-from unified_planning.model.action import Action
-from unified_planning.model.htn.task import Task, Subtask
-from unified_planning.model.timing import Timepoint
-from unified_planning.model.walkers import OperatorsExtractor
-
-
-class TaskNetwork:
-    """Represents an initial task network."""
-
-    def __init__(self, _env: Optional[Environment] = None):
-        self._env = get_env(_env)
-        self._variables: OrderedDict[str, Parameter] = OrderedDict()
-        self._subtasks: List[Subtask] = []
-        self._constraints: List[FNode] = []
-        self._operators_extractor = OperatorsExtractor()  # maybe add to Environment?
-
-    def __repr__(self):
-        s = ["task network {\n"]
-        if len(self._variables) > 0:
-            s.append("  variables = [\n")
-            for v in self.variables:
-                s.append(f"    {v}\n")
-            s.append("  ]\n")
-        s.append("  subtasks = [\n")
-        for t in self.subtasks:
-            s.append(f"    {t}\n")
-        s.append("  ]\n")
+
+
+class Chronicle(TimedCondsEffs):
+    """Core structure to represent a set of timed conditions and effects."""
+
+    def __init__(
+        self,
+        name: str,
+        _parameters: Optional["OrderedDict[str, up.model.types.Type]"] = None,
+        _env: Optional[Environment] = None,
+        **kwargs: "up.model.types.Type",
+    ):
+        TimedCondsEffs.__init__(self, _env)
+        self._name = name
+        self._constraints: List["up.model.fnode.FNode"] = []
+        self._parameters: "OrderedDict[str, up.model.parameter.Parameter]" = (
+            OrderedDict()
+        )
+
+        if _parameters is not None:
+            assert len(kwargs) == 0
+            for n, t in _parameters.items():
+                assert self._environment.type_manager.has_type(
+                    t
+                ), "type of parameter does not belong to the same environment of the action"
+                self._parameters[n] = up.model.parameter.Parameter(
+                    n, t, self._environment
+                )
+        else:
+            for n, t in kwargs.items():
+                assert self._environment.type_manager.has_type(
+                    t
+                ), "type of parameter does not belong to the same environment of the action"
+                self._parameters[n] = up.model.parameter.Parameter(
+                    n, t, self._environment
+                )
+
+    def __repr__(self) -> str:
+        s = []
+        s.append(f"{self.name}")
+        first = True
+        for p in self.parameters:
+            if first:
+                s.append("(")
+                first = False
+            else:
+                s.append(", ")
+            s.append(str(p))
+        if not first:
+            s.append(")")
+        s.append(" {\n")
         if len(self._constraints) > 0:
-            s.append("  constraints = [\n")
-            for c in self.constraints:
-                s.append(f"    {c}\n")
-            s.append("  ]\n")
-        s.append("}")
+            s.append("    constraints = [\n")
+            for c in self._constraints:
+                s.append(f"      {str(c)}\n")
+            s.append("    ]\n")
+        if len(self.conditions) > 0:
+            s.append("    conditions = [\n")
+            for i, cl in self.conditions.items():
+                s.append(f"      {str(i)}:\n")
+                for c in cl:
+                    s.append(f"        {str(c)}\n")
+            s.append("    ]\n")
+        if len(self.effects) > 0:
+            s.append("    effects = [\n")
+            for t, el in self.effects.items():
+                s.append(f"      {str(t)}:\n")
+                for e in el:
+                    s.append(f"        {str(e)}:\n")
+            s.append("    ]\n")
+        s.append("  }")
         return "".join(s)
 
-    def __eq__(self, oth):
-        if not isinstance(oth, TaskNetwork):
+    def __eq__(self, oth: object) -> bool:
+        if not isinstance(oth, Chronicle):
             return False
-        return (
-            set(self.variables) == set(oth.variables)
-            and set(self.subtasks) == set(oth.subtasks)
-            and set(self.constraints) == set(oth.constraints)
-        )
+        if (
+            self._environment != oth._environment
+            or self._parameters != oth._parameters
+            or self._name != oth._name
+        ):
+            return False
+        if set(self._constraints) != set(oth._constraints):
+            return False
+        if not TimedCondsEffs.__eq__(self, oth):
+            return False
+        return True
 
-    def __hash__(self):
-        return (
-            sum(map(hash, self.variables))
-            + sum(map(hash, self.subtasks))
-            + sum(map(hash, self.constraints))
-        )
+    def __hash__(self) -> int:
+        res = hash(self._name)
+        res += sum(map(hash, self._parameters.items()))
+        res += sum(map(hash, self._constraints))
+        res += TimedCondsEffs.__hash__(self)
+        return res
+
+    @property
+    def name(self) -> str:
+        """Returns the `Chronicle` `name`."""
+        return self._name
 
     def clone(self):
-        new = TaskNetwork(self._env)
-        new._variables = self._variables.copy()
-        new._subtasks = self._subtasks[:]
-        new._constraints = self._constraints[:]
+        new = Chronicle(self._name, _env=self._environment)
+        new._parameters = self._parameters.copy()
+        new._constraints = self._constraints.copy()
+        TimedCondsEffs._clone_to(self, new)
         return new
 
-    @property
-    def variables(self) -> List[Parameter]:
-        return list(self._variables.values())
-
-    def add_variable(self, name: str, typename: Type) -> Parameter:
-        if name in self._variables:
-            raise ValueError(f"A variable with name {name} already exists.")
-        param = Parameter(name, typename, self._env)
-        self._variables[name] = param
+    def add_parameter(self, name: str, tpe: Type) -> Parameter:
+        """Adds a new decision variable associated to this activity.
+        The resulting parameter's identifier will be prefixed with the activity's name but may be
+        used outside the activity itself. For instance, it could appear in global constraints or
+        constraints involving more than one activity."""
+        assert ":" not in name, f"Usage of ':' is forbidden in names: {name}"
+        scoped_name = f"{self.name}:{name}"
+        if name in self._parameters:
+            raise ValueError(f"Name '{name}' already used in chronicle '{self.name}'")
+        param = Parameter(scoped_name, tpe)
+        self._parameters[name] = param
         return param
 
-    def parameter(self, name: str) -> Parameter:
-        """Returns the variable with the given name."""
-        return self._variables[name]
-
-    @property
-    def subtasks(self) -> List["Subtask"]:
-        """Returns the list of the subtasks."""
-        return self._subtasks
-
-    def add_subtask(
-        self,
-        task: Union[Subtask, Action, Task],
-        *args: Expression,
-        ident: Optional[str] = None,
-    ) -> Subtask:
-        if isinstance(task, Subtask):
-            assert len(args) == 0 and ident is None
-            subtask = task
-        else:
-            subtask = Subtask(task, *args, ident=ident)
-        assert all([subtask.identifier != prev.identifier for prev in self.subtasks])
-        self._subtasks.append(subtask)
-        return subtask
-
-    def get_subtask(self, ident: str) -> Subtask:
-        """Returns the subtask with the given identifier."""
-        for st in self._subtasks:
-            if st.identifier == ident:
-                return st
-        raise ValueError(f"The task network has not subtask with identifier {ident}")
-
     @property
-    def constraints(self) -> List[FNode]:
-        return self._constraints
+    def parameters(self) -> List["up.model.parameter.Parameter"]:
+        """Returns the `list` of the `Action parameters`."""
+        return list(self._parameters.values())
 
-    def add_constraint(self, constraint: Expression):
-        (constraint,) = self._env.expression_manager.auto_promote(constraint)
-        assert isinstance(constraint, FNode)
-        assert self._env.type_checker.get_type(constraint).is_bool_type()
-        assert OperatorKind.FLUENT_EXP not in self._operators_extractor.get(
-            constraint
-        ), f"The expression is not static (references a fluent): {constraint}"
-        self._constraints.append(constraint)
-
-    def set_strictly_before(
+    def add_constraint(
         self,
-        lhs: Union[Subtask, Timepoint, Timing],
-        rhs: Union[Subtask, Timepoint, Timing],
+        constraint: Union[
+            "up.model.fnode.FNode",
+            "up.model.fluent.Fluent",
+            "up.model.parameter.Parameter",
+            bool,
+        ],
     ):
-        if isinstance(lhs, Subtask):
-            lhs = lhs.end
-        if isinstance(lhs, Timepoint):
-            lhs = Timing(timepoint=lhs, delay=0)
-        assert isinstance(lhs, Timing)
-        if isinstance(rhs, Subtask):
-            rhs = rhs.start
-        if isinstance(rhs, Timepoint):
-            rhs = Timing(timepoint=rhs, delay=0)
-        assert isinstance(rhs, Timing)
-        self.add_constraint(self._env.expression_manager.LT(lhs, rhs))
+        """
+        Adds the given expression to the `chronicle's constraints`.
+        """
+        (constraint_exp,) = self._environment.expression_manager.auto_promote(
+            constraint
+        )
+        assert self._environment.type_checker.get_type(constraint_exp).is_bool_type()
+        if constraint_exp not in self._constraints:
+            self._constraints.append(constraint_exp)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/__init__.py` & `unified_planning-0.6.0/unified_planning/model/mixins/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from unified_planning.model.mixins.actions_set import ActionsSetMixin
+from unified_planning.model.mixins.time_model import TimeModelMixin
 from unified_planning.model.mixins.fluents_set import FluentsSetMixin
 from unified_planning.model.mixins.objects_set import ObjectsSetMixin
 from unified_planning.model.mixins.user_types_set import UserTypesSetMixin
 from unified_planning.model.mixins.agents_set import AgentsSetMixin
+from unified_planning.model.mixins.initial_state import InitialStateMixin
+from unified_planning.model.mixins.metrics import MetricsMixin
 
 __all__ = [
     "ActionsSetMixin",
+    "TimeModelMixin",
     "FluentsSetMixin",
     "ObjectsSetMixin",
     "UserTypesSetMixin",
     "AgentsSetMixin",
+    "InitialStateMixin",
+    "MetricsMixin",
 ]
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/actions_set.py` & `unified_planning-0.6.0/unified_planning/model/mixins/actions_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,36 +9,37 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from warnings import warn
 import unified_planning as up
 from unified_planning.exceptions import UPProblemDefinitionError, UPValueError
-from typing import Iterator, List
+from typing import Iterator, List, Iterable
 
 
 class ActionsSetMixin:
     """
     This class is a mixin that contains a `set` of `actions` with some related methods.
 
     NOTE: when this mixin is used in combination with other mixins that share some
-    of the attributes (e.g. `env`, `add_user_type_method`, `has_name_method`), it is required
+    of the attributes (e.g. `environment`, `add_user_type_method`, `has_name_method`), it is required
     to pass the very same arguments to the mixins constructors.
     """
 
-    def __init__(self, env, add_user_type_method, has_name_method):
-        self._env = env
+    def __init__(self, environment, add_user_type_method, has_name_method):
+        self._env = environment
         self._add_user_type_method = add_user_type_method
         self._has_name_method = has_name_method
         self._actions: List["up.model.action.Action"] = []
 
     @property
-    def env(self) -> "up.environment.Environment":
+    def environment(self) -> "up.environment.Environment":
         """Returns the `Problem` environment."""
         return self._env
 
     @property
     def actions(self) -> List["up.model.action.Action"]:
         """Returns the list of the `Actions` in the `Problem`."""
         return self._actions
@@ -129,24 +130,30 @@
     def add_action(self, action: "up.model.action.Action"):
         """
         Adds the given `action` to the `problem`.
 
         :param action: The `action` that must be added to the `problem`.
         """
         assert (
-            action.env == self._env
+            action.environment == self._env
         ), "Action does not have the same environment of the problem"
         if self._has_name_method(action.name):
-            raise UPProblemDefinitionError("Name " + action.name + " already defined!")
+            msg = f"Name {action.name} already defined! Different elements of a problem can have the same name if the environment flag error_used_named is disabled."
+            if self._env.error_used_name or any(
+                action.name == a.name for a in self._actions
+            ):
+                raise UPProblemDefinitionError(msg)
+            else:
+                warn(msg)
         self._actions.append(action)
         for param in action.parameters:
             if param.type.is_user_type():
                 self._add_user_type_method(param.type)
 
-    def add_actions(self, actions: List["up.model.action.Action"]):
+    def add_actions(self, actions: Iterable["up.model.action.Action"]):
         """
         Adds the given `actions` to the `problem`.
 
-        :param actions: The `list` of `actions` that must be added to the `problem`.
+        :param actions: The `actions` that must be added to the `problem`.
         """
         for action in actions:
             self.add_action(action)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/agents_set.py` & `unified_planning-0.6.0/unified_planning/model/mixins/agents_set.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from warnings import warn
 import unified_planning as up
 from unified_planning.model.types import _UserType
 from unified_planning.exceptions import UPProblemDefinitionError, UPValueError
 from typing import List, Dict, Optional, cast
 
 
 class AgentsSetMixin:
@@ -24,31 +25,35 @@
     This class is a mixin that contains a set of agents with some related methods.
 
     NOTE: when this mixin is used in combination with other mixins that share some
     of the attributes (e.g. has_name_method), it is required to pass the very same
     arguments to the mixins constructors.
     """
 
-    def __init__(self, env, has_name_method):
-        self._env: "up.environment.Environment" = env
+    def __init__(self, environment, has_name_method):
+        self._env: "up.environment.Environment" = environment
         self._has_name_method = has_name_method
         self._agents: List["up.model.multi_agent.Agent"] = []
 
     @property
-    def env(self) -> "up.environment.Environment":
+    def environment(self) -> "up.environment.Environment":
         """Returns the problem environment."""
         return self._env
 
     def add_agent(self, agent: "up.model.multi_agent.Agent"):
         """This method adds an Agent"""
         if agent not in self._agents:
             if self._has_name_method(agent.name):
-                raise UPProblemDefinitionError(
-                    f"The agent name {agent.name} is already used in the problem"
-                )
+                msg = f"The agent name {agent.name} is already used in the problem!  Different elements of a problem can have the same name if the environment flag error_used_named is disabled."
+                if self._env.error_used_name or any(
+                    agent.name == a.name for a in self._agents
+                ):
+                    raise UPProblemDefinitionError(msg)
+                else:
+                    warn(msg)
             self._agents.append(agent)
 
     @property
     def agents(self) -> List["up.model.multi_agent.Agent"]:
         """Returns the agents."""
         return self._agents
 
@@ -58,10 +63,10 @@
             if agent._name == name:
                 return agent
         raise UPValueError(f"Agent {name} is not defined!")
 
     def has_agent(self, name: str) -> bool:
         """Returns True iff the agent 'name' is defined."""
         for agent in self._agents:
-            if agent._name == name:
+            if agent.name == name:
                 return True
         return False
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/fluents_set.py` & `unified_planning-0.6.0/unified_planning/model/mixins/fluents_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,52 +9,53 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from warnings import warn
 import unified_planning as up
 from unified_planning.model.expression import ConstantExpression
 from unified_planning.exceptions import UPProblemDefinitionError, UPValueError
-from typing import Optional, List, Dict, Union
+from typing import Optional, List, Dict, Union, Iterable
 
 
 class FluentsSetMixin:
     """
     This class is a mixin that contains a `set` of `fluents` with some related methods.
 
     NOTE: when this mixin is used in combination with other mixins that share some
-    of the attributes (e.g. `env`, `add_user_type_method`, `has_name_method`), it is required
+    of the attributes (e.g. `environment`, `add_user_type_method`, `has_name_method`), it is required
     to pass the very same arguments to the mixins constructors.
     """
 
     def __init__(
         self,
-        env,
+        environment,
         add_user_type_method,
         has_name_method,
         initial_defaults: Dict["up.model.types.Type", "ConstantExpression"] = {},
     ):
-        self._env = env
+        self._env = environment
         self._add_user_type_method = add_user_type_method
         self._has_name_method = has_name_method
         self._fluents: List["up.model.fluent.Fluent"] = []
         self._fluents_defaults: Dict[
             "up.model.fluent.Fluent", "up.model.fnode.FNode"
         ] = {}
         self._initial_defaults: Dict["up.model.types.Type", "up.model.fnode.FNode"] = {}
         for k, v in initial_defaults.items():
-            (v_exp,) = self.env.expression_manager.auto_promote(v)
+            (v_exp,) = self.environment.expression_manager.auto_promote(v)
             self._initial_defaults[k] = v_exp
         # The field initial default optionally associates a type to a default value. When a new fluent is
         # created with no explicit default, it will be associated with the initial-default of his type, if any.
 
     @property
-    def env(self) -> "up.environment.Environment":
+    def environment(self) -> "up.environment.Environment":
         """Returns the `problem` `Environment`."""
         return self._env
 
     @property
     def fluents(self) -> List["up.model.fluent.Fluent"]:
         """Returns the `fluents` currently in the `problem`."""
         return self._fluents
@@ -81,19 +82,19 @@
             `False` otherwise.
         """
         for f in self._fluents:
             if f.name == name:
                 return True
         return False
 
-    def add_fluents(self, fluents: List["up.model.fluent.Fluent"]):
+    def add_fluents(self, fluents: Iterable["up.model.fluent.Fluent"]):
         """
-        Adds the given `list` of `fluents` to the `problem`.
+        Adds the given `fluents` to the `problem`.
 
-        :param fluents: The `list` of `fluents` that must be added to the `problem`.
+        :param fluents: The `fluents` that must be added to the `problem`.
         """
         for fluent in fluents:
             self.add_fluent(fluent)
 
     def add_fluent(
         self,
         fluent_or_name: Union["up.model.fluent.Fluent", str],
@@ -129,36 +130,67 @@
             assert len(kwargs) == 0 and typename is None
             fluent = fluent_or_name
             assert (
                 fluent.environment == self._env
             ), "Fluent does not have the same environment of the problem"
         else:
             fluent = up.model.fluent.Fluent(
-                fluent_or_name, typename, None, env=self.env, **kwargs
+                fluent_or_name, typename, None, environment=self.environment, **kwargs
             )
         if self._has_name_method(fluent.name):
-            raise UPProblemDefinitionError("Name " + fluent.name + " already defined!")
+            msg = f"Name {fluent.name} already defined! Different elements of a problem can have the same name if the environment flag error_used_named is disabled."
+            if self._env.error_used_name or any(
+                fluent.name == f.name for f in self._fluents
+            ):
+                raise UPProblemDefinitionError(msg)
+            else:
+                warn(msg)
         self._fluents.append(fluent)
         if not default_initial_value is None:
-            (v_exp,) = self.env.expression_manager.auto_promote(default_initial_value)
+            (v_exp,) = self.environment.expression_manager.auto_promote(
+                default_initial_value
+            )
             self._fluents_defaults[fluent] = v_exp
         elif fluent.type in self._initial_defaults:
             self._fluents_defaults[fluent] = self._initial_defaults[fluent.type]
         if fluent.type.is_user_type():
             self._add_user_type_method(fluent.type)
         for param in fluent.signature:
             if param.type.is_user_type():
                 self._add_user_type_method(param.type)
 
         return fluent
 
+    def clear_fluents(self):
+        """
+        Removes all the Fluent from the current Problem, together with their default.
+        """
+        self._fluents = []
+        self._fluents_defaults = {}
+
     @property
     def fluents_defaults(
         self,
     ) -> Dict["up.model.fluent.Fluent", "up.model.fnode.FNode"]:
         """Returns the `problem's fluents defaults`."""
         return self._fluents_defaults
 
     @property
     def initial_defaults(self) -> Dict["up.model.types.Type", "up.model.fnode.FNode"]:
         """Returns the `problem's fluents defaults` for each `type`."""
         return self._initial_defaults
+
+    def __eq__(self, oth):
+        # ignores default values as they may have no impact on the initial state
+        if not isinstance(oth, FluentsSetMixin):
+            return False
+        if set(self._fluents) != set(oth._fluents):
+            return False
+        return True
+
+    def __hash__(self):
+        return sum(map(hash, self._fluents))
+
+    def _clone_to(self, other: "FluentsSetMixin"):
+        other._fluents = self._fluents.copy()
+        other._initial_defaults = self._initial_defaults.copy()
+        other._fluents_defaults = self._fluents_defaults.copy()
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/objects_set.py` & `unified_planning-0.6.0/unified_planning/model/mixins/objects_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,37 +9,38 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from warnings import warn
 import unified_planning as up
 from unified_planning.model.types import _UserType
 from unified_planning.exceptions import UPProblemDefinitionError, UPValueError
-from typing import Iterator, List, Union, Optional, cast
+from typing import Iterator, List, Union, Optional, cast, Iterable
 
 
 class ObjectsSetMixin:
     """
     This class is a mixin that contains a `set` of `objects` with some related methods.
 
     NOTE: when this mixin is used in combination with other mixins that share some
-    of the attributes (e.g. `env`, `add_user_type_method`, `has_name_method`), it is required
+    of the attributes (e.g. `environment`, `add_user_type_method`, `has_name_method`), it is required
     to pass the very same arguments to the mixins constructors.
     """
 
-    def __init__(self, env, add_user_type_method, has_name_method):
-        self._env = env
+    def __init__(self, environment, add_user_type_method, has_name_method):
+        self._env = environment
         self._add_user_type_method = add_user_type_method
         self._has_name_method = has_name_method
         self._objects: List["up.model.object.Object"] = []
 
     @property
-    def env(self) -> "up.environment.Environment":
+    def environment(self) -> "up.environment.Environment":
         """Returns the `problem` `environment`."""
         return self._env
 
     def add_object(
         self,
         obj_or_name: Union["up.model.object.Object", str],
         typename: Optional["up.model.types.Type"] = None,
@@ -67,25 +68,32 @@
             assert (
                 obj.environment == self._env
             ), "Object does not have the same environemt fo the problem"
         else:
             assert typename is not None, "Missing type of the object"
             obj = up.model.object.Object(obj_or_name, typename, self._env)
         if self._has_name_method(obj.name):
-            raise UPProblemDefinitionError("Name " + obj.name + " already defined!")
+            msg = f"Name {obj.name} already defined! Different elements of a problem can have the same name if the environment flag error_used_named is disabled."
+            if self._env.error_used_name or any(
+                obj.name == o.name for o in self._objects
+            ):
+                raise UPProblemDefinitionError(msg)
+            else:
+                warn(msg)
+            raise UPProblemDefinitionError()
         self._objects.append(obj)
         if obj.type.is_user_type():
             self._add_user_type_method(obj.type)
         return obj
 
-    def add_objects(self, objects: List["up.model.object.Object"]):
+    def add_objects(self, objects: Iterable["up.model.object.Object"]):
         """
         Adds the given `objects` to the `problem`.
 
-        :param objects: The `list` of `objects` that must be added to the `problem`.
+        :param objects: The `objects` that must be added to the `problem`.
         """
         for obj in objects:
             self.add_object(obj)
 
     def object(self, name: str) -> "up.model.object.Object":
         """
         Returns the `object` with the given `name`.
@@ -126,7 +134,18 @@
             if cast(_UserType, obj.type).is_subtype(typename):
                 yield obj
 
     @property
     def all_objects(self) -> List["up.model.object.Object"]:
         """Returns the `list` containing all the `objects` in the `problem`."""
         return self._objects
+
+    def __eq__(self, other):
+        return isinstance(other, ObjectsSetMixin) and set(self._objects) == set(
+            other._objects
+        )
+
+    def __hash__(self):
+        return sum(map(hash, self._objects))
+
+    def _clone_to(self, other: "ObjectsSetMixin"):
+        other._objects = self._objects.copy()
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/mixins/user_types_set.py` & `unified_planning-0.6.0/unified_planning/model/mixins/user_types_set.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from warnings import warn
 import unified_planning as up
 from unified_planning.model.types import _UserType
 from unified_planning.exceptions import UPProblemDefinitionError, UPValueError
 from typing import List, Dict, Optional, cast
 
 
 class UserTypesSetMixin:
@@ -24,33 +25,38 @@
     This class is a mixin that contains a `set` of `user types` with some related methods.
 
     NOTE: when this mixin is used in combination with other mixins that share some
     of the attributes (e.g. `has_name_method`), it is required to pass the very same
     arguments to the mixins constructors.
     """
 
-    def __init__(self, has_name_method):
+    def __init__(self, env, has_name_method):
+        self._env = env
         self._has_name_method = has_name_method
         self._user_types: List["up.model.types.Type"] = []
         # The field _user_types_hierarchy stores the information about the types and the list of their sons.
         self._user_types_hierarchy: Dict[
             Optional["up.model.types.Type"], List["up.model.types.Type"]
         ] = {}
 
     def _add_user_type(self, type: "up.model.types.Type"):
         """This method adds a Type, together with all it's ancestors, to the user_types_hierarchy"""
         assert type.is_user_type()
         if type not in self._user_types:
-            t = cast(_UserType, type)
-            if self._has_name_method(t.name):
-                raise UPProblemDefinitionError(
-                    f"The type name {t.name} is already used in the problem"
-                )
-            if t.father is not None:
-                self._add_user_type(t.father)
+            ut = cast(_UserType, type)
+            if self._has_name_method(ut.name):
+                msg = f"The type name {ut.name} is already used in the problem! Different elements of a problem can have the same name if the environment flag error_used_named is disabled."
+                if self._env.error_used_name or any(
+                    ut.name == cast(_UserType, t).name for t in self._user_types
+                ):
+                    raise UPProblemDefinitionError(msg)
+                else:
+                    warn(msg)
+            if ut.father is not None:
+                self._add_user_type(ut.father)
             self._user_types.append(type)
 
     @property
     def user_types(self) -> List["up.model.types.Type"]:
         """Returns the `list` of all the `user types` in the `problem`."""
         return self._user_types
 
@@ -98,7 +104,19 @@
                 res[t] = []
             f = cast(_UserType, t).father
             if f not in res:
                 res[f] = [t]
             else:
                 res[f].append(t)
         return res
+
+    def __eq__(self, other):
+        return isinstance(other, UserTypesSetMixin) and set(self._user_types) == set(
+            other._user_types
+        )
+
+    def __hash__(self):
+        return sum(map(hash, self._user_types))
+
+    def _clone_to(self, other: "UserTypesSetMixin"):
+        other._user_types = self._user_types[:]
+        other._user_types_hierarchy = self._user_types_hierarchy.copy()
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/multi_agent/__init__.py` & `unified_planning-0.6.0/unified_planning/model/multi_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/multi_agent/agent.py` & `unified_planning-0.6.0/unified_planning/model/multi_agent/ma_environment.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,97 +8,67 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-"""This module defines an agent class."""
-
+"""This module defines an ma_environment class."""
 import unified_planning as up
 from unified_planning.model.mixins import (
-    ActionsSetMixin,
     FluentsSetMixin,
 )
 
 
-class Agent(
+class MAEnvironment(
     FluentsSetMixin,
-    ActionsSetMixin,
 ):
     """
-    This is an agent class that represents a generic `agent`.
+    This is an MAEnvironment class that represents a generic `MAEnvironment`.
     """
 
     def __init__(
         self,
-        name: str,
         ma_problem: "up.model.multi_agent.ma_problem.MultiAgentProblem",
     ):
         FluentsSetMixin.__init__(
             self,
-            ma_problem.env,
+            ma_problem.environment,
             ma_problem._add_user_type,
-            self.has_name,
+            ma_problem.has_name,
             ma_problem._initial_defaults,
         )
-        ActionsSetMixin.__init__(
-            self, ma_problem.env, ma_problem._add_user_type, self.has_name
-        )
-        self._env = ma_problem.env
-        self._name: str = name
+        self._env = ma_problem.environment
 
-    def __getstate__(self):
-        state = self.__dict__.copy()
-        # Don't pickle _add_user_type_method
-        state["_add_user_type_method"] = None
-        return state
+    @property
+    def environment(self) -> "up.Environment":
+        """Returns this `MAEnvironment` `Environment`."""
+        return self._env
 
     def has_name(self, name: str) -> bool:
         """
         Returns `True` if the given `name` is already in the `MultiAgentProblem`, `False` otherwise.
 
         :param name: The target name to find in the `MultiAgentProblem`.
         :return: `True` if the given `name` is already in the `MultiAgentProblem`, `False` otherwise."""
-        return self.has_action(name) or self.has_fluent(name)
-
-    @property
-    def name(self) -> str:
-        """Returns the `Agent` `name`."""
-        return self._name
-
-    @property
-    def env(self) -> "up.Environment":
-        """Returns this `Agent` `Environment`."""
-        return self._env
+        return self.has_fluent(name)
 
     def __repr__(self) -> str:
         s = []
-        s.append(f"Agent name = {str(self._name)}\n\n")
         s.append("fluents = [\n")
         for f in self._fluents:
             s.append(f" {str(f)}\n")
         s.append("]\n\n")
-        s.append("actions = [\n")
-        for a in self._actions:
-            s.append(f" {str(a)}\n")
-        s.append("]\n\n")
         return "".join(s)
 
     def __eq__(self, oth: object) -> bool:
-        if not (isinstance(oth, Agent)) or self._env != oth._env:
-            return False
-        if self._name != oth._name:
+        if not (isinstance(oth, MAEnvironment)) or self._env != oth._env:
             return False
         if set(self._fluents) != set(oth._fluents):
             return False
-        if set(self._actions) != set(oth._actions):
-            return False
         return True
 
     def __hash__(self) -> int:
-        res = hash(self._name)
+        res = 0
         for f in self._fluents:
             res += hash(f)
-        for a in self._actions:
-            res += hash(a)
         return res
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/multi_agent/ma_environment.py` & `unified_planning-0.6.0/unified_planning/model/object.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,67 +8,78 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-"""This module defines an ma_environment class."""
-import unified_planning as up
-from unified_planning.model.mixins import (
-    FluentsSetMixin,
-)
+"""
+This module defines an Object of a planning problem.
+An Object is represented by a name and by its type.
+"""
 
+from typing import Optional
+from unified_planning.environment import Environment, get_environment
+import unified_planning.model.types
 
-class MAEnvironment(
-    FluentsSetMixin,
-):
+
+class Object:
     """
-    This is an MAEnvironment class that represents a generic `MAEnvironment`.
+    Represents an `Object` of the `unified_planning` library.
+
+    An `Object` contains 2 parts:
+    - `name`: a string containing the `Object's` :func:`name <unified_planning.model.Object.name>`.
+    - `type`: a :class:`~unified_planning.model.Type` representing the planning :func:`user_type <unified_planning.model.Object.type>` associated to this `Object`.
+
+    The `Object` class is immutable.
     """
 
     def __init__(
         self,
-        ma_problem: "up.model.multi_agent.ma_problem.MultiAgentProblem",
+        name: str,
+        typename: "unified_planning.model.types.Type",
+        environment: Optional[Environment] = None,
     ):
-        FluentsSetMixin.__init__(
-            self,
-            ma_problem.env,
-            ma_problem._add_user_type,
-            self.has_name,
-            ma_problem._initial_defaults,
-        )
-        self._env = ma_problem.env
-
-    @property
-    def env(self) -> "up.Environment":
-        """Returns this `MAEnvironment` `Environment`."""
-        return self._env
-
-    def has_name(self, name: str) -> bool:
-        """
-        Returns `True` if the given `name` is already in the `MultiAgentProblem`, `False` otherwise.
-
-        :param name: The target name to find in the `MultiAgentProblem`.
-        :return: `True` if the given `name` is already in the `MultiAgentProblem`, `False` otherwise."""
-        return self.has_fluent(name)
+        self._name = name
+        self._typename = typename
+        self._env = get_environment(environment)
+        assert self._env.type_manager.has_type(
+            typename
+        ), "type of the object does not belong to the same environment of the object"
 
     def __repr__(self) -> str:
-        s = []
-        s.append("fluents = [\n")
-        for f in self._fluents:
-            s.append(f" {str(f)}\n")
-        s.append("]\n\n")
-        return "".join(s)
+        return self.name
 
     def __eq__(self, oth: object) -> bool:
-        if not (isinstance(oth, MAEnvironment)) or self._env != oth._env:
+        if isinstance(oth, Object):
+            return (
+                self._name == oth._name
+                and self._typename == oth._typename
+                and self._env == oth._env
+            )
+        else:
             return False
-        if set(self._fluents) != set(oth._fluents):
-            return False
-        return True
 
     def __hash__(self) -> int:
-        res = 0
-        for f in self._fluents:
-            res += hash(f)
-        return res
+        return hash(self._name) + hash(self._typename)
+
+    @property
+    def name(self) -> str:
+        """Returns the `Object` `name`."""
+        return self._name
+
+    @property
+    def type(self) -> "unified_planning.model.types.Type":
+        """Returns the `Object` `Type`."""
+        return self._typename
+
+    @property
+    def environment(self) -> "Environment":
+        """Return the `Object` `Environment`"""
+        return self._env
+
+    #
+    # Infix operators
+    #
+
+    def Equals(self, right):
+        return self._env.expression_manager.Equals(self, right)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/multi_agent/ma_problem.py` & `unified_planning-0.6.0/unified_planning/model/multi_agent/ma_problem.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,62 +15,64 @@
 """This module defines the MultiAgentProblem class."""
 
 import unified_planning as up
 from unified_planning.model.abstract_problem import AbstractProblem
 from unified_planning.model.expression import ConstantExpression
 from unified_planning.model.operators import OperatorKind
 from unified_planning.model.fluent import get_all_fluent_exp
-from unified_planning.model.walkers.substituter import Substituter
 from unified_planning.exceptions import (
     UPProblemDefinitionError,
     UPTypeError,
     UPExpressionDefinitionError,
-    UPValueError,
+    UPPlanDefinitionError,
 )
-from fractions import Fraction
-from typing import Optional, List, Dict, Union, cast
+from typing import Optional, List, Dict, Union, cast, Iterable
 from unified_planning.model.mixins import (
     ObjectsSetMixin,
     UserTypesSetMixin,
     AgentsSetMixin,
 )
+from fractions import Fraction
 
 
-class MultiAgentProblem(
+class MultiAgentProblem(  # type: ignore[misc]
     AbstractProblem,
     UserTypesSetMixin,
     ObjectsSetMixin,
     AgentsSetMixin,
 ):
     """
     Represents the multi-agent planning problem, with :class:`Agent <unified_planning.model.multi_agent.agent>`, with :class:`MAEnvironment <unified_planning.model.multi_agent.ma_environment>`, :class:`Fluents <unified_planning.model.Fluent>`, :class:`Objects <unified_planning.model.Object>` and :class:`UserTypes <unified_planning.model.Type>`.
     """
 
     def __init__(
         self,
         name: Optional[str] = None,
-        env: Optional["up.environment.Environment"] = None,
+        environment: Optional["up.environment.Environment"] = None,
         *,
         initial_defaults: Dict["up.model.types.Type", "ConstantExpression"] = {},
     ):
-        AbstractProblem.__init__(self, name, env)
-        UserTypesSetMixin.__init__(self, self.has_name)
-        ObjectsSetMixin.__init__(self, self.env, self._add_user_type, self.has_name)
-        AgentsSetMixin.__init__(self, self.env, self.has_name)
+        AbstractProblem.__init__(self, name, environment)
+        UserTypesSetMixin.__init__(self, self.environment, self.has_name)
+        ObjectsSetMixin.__init__(
+            self, self.environment, self._add_user_type, self.has_name
+        )
+        AgentsSetMixin.__init__(self, self.environment, self.has_name)
 
         self._initial_defaults = initial_defaults
         self._env_ma = up.model.multi_agent.ma_environment.MAEnvironment(self)
         self._goals: List["up.model.fnode.FNode"] = list()
         self._initial_value: Dict["up.model.fnode.FNode", "up.model.fnode.FNode"] = {}
         self._operators_extractor = up.model.walkers.OperatorsExtractor()
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         for a in self._agents:
             a._add_user_type_method = self._add_user_type
+            a._ma_problem_has_name_not_in_agents = self.has_name_not_in_agents
 
     def __repr__(self) -> str:
         s = []
         if not self.name is None:
             s.append(f"problem name = {str(self.name)}\n\n")
         if len(self.user_types) > 0:
             s.append(f"types = {str(list(self.user_types))}\n\n")
@@ -155,33 +157,52 @@
         return new_p
 
     def has_name(self, name: str) -> bool:
         """
         Returns `True` if the given `name` is already in the `MultiAgentProblem`, `False` otherwise.
 
         :param name: The target name to find in the `MultiAgentProblem`.
-        :return: `True` if the given `name` is already in the `MultiAgentProblem`, `False` otherwise."""
-        return self.has_object(name) or self.has_type(name) or self.has_agent(name)
+        :return: `True` if the given `name` is already in the `MultiAgentProblem`, `False` otherwise.
+        """
+        return (
+            self.has_object(name)
+            or self.has_type(name)
+            or self.has_agent(name)
+            or self._env_ma.has_name(name)
+            or any(a.has_name_in_agent(name) for a in self._agents)
+        )
+
+    def has_name_not_in_agents(self, name: str) -> bool:
+        """
+        Returns `True` if the given `name` is already in the `MultiAgentProblem`, `False` otherwise;
+        this method does not check in the problem's agents
+
+        :param name: The target name to find in the `MultiAgentProblem` without checking Agents.
+        :return: `True` if the given `name` is already in the `MultiAgentProblem`, `False` otherwise.
+        """
+        return (
+            self.has_object(name)
+            or self.has_type(name)
+            or self.has_agent(name)
+            or self._env_ma.has_name(name)
+        )
 
     @property
     def ma_environment(self) -> "up.model.multi_agent.ma_environment.MAEnvironment":
         """Returns this `MultiAgentProblem` `MAEnvironment`."""
         return self._env_ma
 
     def set_initial_value(
         self,
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: Union[
-            "up.model.fnode.FNode",
+            "up.model.expression.NumericExpression",
             "up.model.fluent.Fluent",
             "up.model.object.Object",
             bool,
-            int,
-            float,
-            Fraction,
         ],
     ):
         """
         Sets the initial value for the given `Fluent`. The given `Fluent` must be grounded, therefore if
         it's :func:`arity <unified_planning.model.Fluent.arity>` is `> 0`, the `fluent` parameter must be
         an `FNode` and the method :func:`~unified_planning.model.FNode.is_fluent_exp` must return `True`.
 
@@ -236,15 +257,15 @@
         res = self._initial_value
         for f in self.ma_environment.fluents:
             for f_exp in get_all_fluent_exp(self, f):
                 res[f_exp] = self.initial_value(f_exp)
         for a in self.agents:
             for f in a.fluents:
                 for f_exp in get_all_fluent_exp(self, f):
-                    d = self.env.expression_manager.Dot(a, f_exp)
+                    d = self.environment.expression_manager.Dot(a, f_exp)
                     res[d] = self.initial_value(d)
         return res
 
     @property
     def explicit_initial_values(
         self,
     ) -> Dict["up.model.fnode.FNode", "up.model.fnode.FNode"]:
@@ -265,25 +286,28 @@
 
         :param goal: The expression added to the `MultiAgentProblem` :func:`goals <unified_planning.model.multi_agent.MultiAgentProblem.goals>`.
         """
         assert (
             isinstance(goal, bool) or goal.environment == self._env
         ), "goal does not have the same environment of the problem"
         (goal_exp,) = self._env.expression_manager.auto_promote(goal)
-        assert self._env.type_checker.get_type(goal_exp).is_bool_type()
+        assert self._env.type_checker.get_type(
+            goal_exp
+        ).is_bool_type(), "A goal must be a boolean expression"
         if goal_exp != self._env.expression_manager.TRUE():
             self._goals.append(goal_exp)
 
     def add_goals(
-        self, goals: List[Union["up.model.fnode.FNode", "up.model.fluent.Fluent", bool]]
+        self,
+        goals: Iterable[Union["up.model.fnode.FNode", "up.model.fluent.Fluent", bool]],
     ):
         """
         Adds the given `goal` to the `MultiAgentProblem`.
 
-        :param goals: The `list` of `goals` that must be added to the `MultiAgentProblem`.
+        :param goals: The `goals` that must be added to the `MultiAgentProblem`.
         """
         for goal in goals:
             self.add_goal(goal)
 
     @property
     def goals(self) -> List["up.model.fnode.FNode"]:
         """Returns all the `goals` in the `MultiAgentProblem`."""
@@ -324,15 +348,15 @@
             self._kind.set_effects_kind("INCREASE_EFFECTS")
         elif e.is_decrease():
             self._kind.set_effects_kind("DECREASE_EFFECTS")
 
     def _update_problem_kind_condition(self, exp: "up.model.fnode.FNode"):
         ops = self._operators_extractor.get(exp)
         if OperatorKind.EQUALS in ops:
-            self._kind.set_conditions_kind("EQUALITY")
+            self._kind.set_conditions_kind("EQUALITIES")
         if OperatorKind.NOT in ops:
             self._kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         if OperatorKind.OR in ops:
             self._kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         if OperatorKind.EXISTS in ops:
             self._kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         if OperatorKind.FORALL in ops:
@@ -347,24 +371,69 @@
             self._kind.set_numbers("DISCRETE_NUMBERS")
         elif type.is_real_type():
             self._kind.set_numbers("CONTINUOUS_NUMBERS")
 
     def _update_problem_kind_fluent(self, fluent: "up.model.fluent.Fluent"):
         self._update_problem_kind_type(fluent.type)
         if fluent.type.is_int_type() or fluent.type.is_real_type():
+            numeric_type = fluent.type
+            assert isinstance(
+                numeric_type, (up.model.types._RealType, up.model.types._IntType)
+            )
+            if (
+                numeric_type.lower_bound is not None
+                or numeric_type.upper_bound is not None
+            ):
+                self._kind.set_numbers("BOUNDED_TYPES")
             self._kind.set_fluents_type("NUMERIC_FLUENTS")
         elif fluent.type.is_user_type():
             self._kind.set_fluents_type("OBJECT_FLUENTS")
         for p in fluent.signature:
             self._update_problem_kind_type(p.type)
 
     def _update_problem_kind_action(self, action: "up.model.action.Action"):
         for p in action.parameters:
             self._update_problem_kind_type(p.type)
         if isinstance(action, up.model.action.InstantaneousAction):
             for c in action.preconditions:
                 self._update_problem_kind_condition(c)
             for e in action.effects:
                 self._update_problem_kind_effect(e)
+        elif isinstance(action, up.model.action.DurativeAction):
             self._kind.set_time("CONTINUOUS_TIME")
         else:
             raise NotImplementedError
+
+    def normalize_plan(self, plan: "up.plans.Plan") -> "up.plans.Plan":
+        """
+        Normalizes the given `Plan`, that is potentially the result of another
+        `MAProblem`, updating the `Object` references in the `Plan` with the ones of
+        this `MAProblem` which are syntactically equal.
+
+        :param plan: The `Plan` that must be normalized.
+        :return: A `Plan` syntactically valid for this `Problem`.
+        """
+        return plan.replace_action_instances(self._replace_action_instance)
+
+    def _replace_action_instance(
+        self, action_instance: "up.plans.ActionInstance"
+    ) -> "up.plans.ActionInstance":
+        em = self.environment.expression_manager
+        if action_instance.agent is None:
+            raise UPPlanDefinitionError(
+                f"An ActionInstance for a multi-agent problem must have an Agent; {action_instance} has no Agent."
+            )
+        new_a = action_instance.agent.action(action_instance.action.name)
+        params = []
+        for p in action_instance.actual_parameters:
+            if p.is_object_exp():
+                obj = self.object(p.object().name)
+                params.append(em.ObjectExp(obj))
+            elif p.is_bool_constant():
+                params.append(em.Bool(p.is_true()))
+            elif p.is_int_constant():
+                params.append(em.Int(cast(int, p.constant_value())))
+            elif p.is_real_constant():
+                params.append(em.Real(cast(Fraction, p.constant_value())))
+            else:
+                raise NotImplementedError
+        return up.plans.ActionInstance(new_a, tuple(params), action_instance.agent)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/operators.py` & `unified_planning-0.6.0/unified_planning/model/operators.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/parameter.py` & `unified_planning-0.6.0/unified_planning/model/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 """
 This module defines the Parameter class. Both actions and fluents use this class to represent their parameters.
 """
 
 
 from typing import Optional
-from unified_planning.environment import Environment, get_env
+from unified_planning.environment import Environment, get_environment
 import unified_planning as up
 
 
 class Parameter:
     """
     Represents an :func:`action parameter <unified_planning.model.Action.parameters>` or a :func:`fluent parameter <unified_planning.model.Fluent.signature>`.
     A `Parameter` has a :func:`name <unified_planning.model.Parameter.name>`, and a :func:`Type <unified_planning.model.Parameter.type>`.
@@ -30,19 +30,19 @@
     The Parameter class is immutable.
     """
 
     def __init__(
         self,
         name: str,
         typename: "up.model.types.Type",
-        env: Optional[Environment] = None,
+        environment: Optional[Environment] = None,
     ):
         self._name = name
         self._typename = typename
-        self._env = get_env(env)
+        self._env = get_environment(environment)
         assert self._env.type_manager.has_type(
             typename
         ), "type of parameter does not belong to the same environment given to the parameter"
 
     def __repr__(self) -> str:
         return f"{str(self.type)} {self.name}"
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/problem.py` & `unified_planning-0.6.0/unified_planning/model/problem.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,77 +11,98 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines the problem class."""
 
 
+from numbers import Real
 import unified_planning as up
+import unified_planning.model.tamp
 from unified_planning.model.abstract_problem import AbstractProblem
 from unified_planning.model.mixins import (
     ActionsSetMixin,
+    TimeModelMixin,
     FluentsSetMixin,
     ObjectsSetMixin,
     UserTypesSetMixin,
+    InitialStateMixin,
+    MetricsMixin,
 )
 from unified_planning.model.expression import ConstantExpression
 from unified_planning.model.operators import OperatorKind
-from unified_planning.model.fluent import get_all_fluent_exp
 from unified_planning.exceptions import (
     UPProblemDefinitionError,
     UPTypeError,
-    UPExpressionDefinitionError,
+    UPConflictingEffectsException,
 )
 from fractions import Fraction
-from typing import Optional, List, Dict, Set, Union, cast
+from typing import Optional, List, Dict, Set, Tuple, Union, cast
 
 
-class Problem(
+class Problem(  # type: ignore[misc]
     AbstractProblem,
     UserTypesSetMixin,
+    TimeModelMixin,
     FluentsSetMixin,
     ActionsSetMixin,
     ObjectsSetMixin,
+    InitialStateMixin,
+    MetricsMixin,
 ):
     """
     Represents the classical planning problem, with :class:`Actions <unified_planning.model.Action>`, :class:`Fluents <unified_planning.model.Fluent>`, :class:`Objects <unified_planning.model.Object>` and :class:`UserTypes <unified_planning.model.Type>`.
 
     The `Actions` can be :class:`DurativeActions <unified_planning.model.DurativeAction>` when the `Problem` deals with time.
     """
 
     def __init__(
         self,
         name: Optional[str] = None,
-        env: Optional["up.environment.Environment"] = None,
+        environment: Optional["up.environment.Environment"] = None,
         *,
         initial_defaults: Dict["up.model.types.Type", "ConstantExpression"] = {},
     ):
-        AbstractProblem.__init__(self, name, env)
-        UserTypesSetMixin.__init__(self, self.has_name)
+        AbstractProblem.__init__(self, name, environment)
+        UserTypesSetMixin.__init__(self, self.environment, self.has_name)
+        TimeModelMixin.__init__(self, epsilon_default=None, discrete_time=False)
         FluentsSetMixin.__init__(
-            self, self.env, self._add_user_type, self.has_name, initial_defaults
+            self, self.environment, self._add_user_type, self.has_name, initial_defaults
         )
-        ActionsSetMixin.__init__(self, self.env, self._add_user_type, self.has_name)
-        ObjectsSetMixin.__init__(self, self.env, self._add_user_type, self.has_name)
+        ActionsSetMixin.__init__(
+            self, self.environment, self._add_user_type, self.has_name
+        )
+        ObjectsSetMixin.__init__(
+            self, self.environment, self._add_user_type, self.has_name
+        )
+        InitialStateMixin.__init__(self, self, self, self.environment)
+        MetricsMixin.__init__(self, self.environment)
         self._operators_extractor = up.model.walkers.OperatorsExtractor()
-        self._initial_value: Dict["up.model.fnode.FNode", "up.model.fnode.FNode"] = {}
         self._timed_effects: Dict[
             "up.model.timing.Timing", List["up.model.effect.Effect"]
         ] = {}
         self._timed_goals: Dict[
             "up.model.timing.TimeInterval", List["up.model.fnode.FNode"]
         ] = {}
         self._trajectory_constraints: List["up.model.fnode.FNode"] = list()
         self._goals: List["up.model.fnode.FNode"] = list()
-        self._metrics: List["up.model.metrics.PlanQualityMetric"] = []
+        self._fluents_assigned: Dict[
+            "up.model.timing.Timing",
+            Dict["up.model.fnode.FNode", "up.model.fnode.FNode"],
+        ] = {}
+        self._fluents_inc_dec: Dict[
+            "up.model.timing.Timing", Set["up.model.fnode.FNode"]
+        ] = {}
 
     def __repr__(self) -> str:
         s = []
-        if not self.name is None:
+        if self.name is not None:
             s.append(f"problem name = {str(self.name)}\n\n")
+        if self._epsilon is not None:
+            s.append(f"epsilon separation = {self._epsilon}\n\n")
         if len(self.user_types) > 0:
             s.append(f"types = {str(list(self.user_types))}\n\n")
         s.append("fluents = [\n")
         for f in self.fluents:
             s.append(f"  {str(f)}\n")
         s.append("]\n\n")
         s.append("actions = [\n")
@@ -96,15 +117,15 @@
         s.append("initial fluents default = [\n")
         for f in self._fluents:
             if f in self._fluents_defaults:
                 v = self._fluents_defaults[f]
                 s.append(f"  {str(f)} := {str(v)}\n")
         s.append("]\n\n")
         s.append("initial values = [\n")
-        for k, v in self._initial_value.items():
+        for k, v in self.explicit_initial_values.items():
             s.append(f"  {str(k)} := {str(v)}\n")
         s.append("]\n\n")
         if len(self.timed_effects) > 0:
             s.append("timed effects = [\n")
             for t, el in self.timed_effects.items():
                 s.append(f"  {str(t)} :\n")
                 for e in el:
@@ -134,36 +155,33 @@
         return "".join(s)
 
     def __eq__(self, oth: object) -> bool:
         if not (isinstance(oth, Problem)) or self._env != oth._env:
             return False
         if self.kind != oth.kind or self._name != oth._name:
             return False
-        if set(self._fluents) != set(oth._fluents) or set(self._goals) != set(
-            oth._goals
-        ):
+
+        if not UserTypesSetMixin.__eq__(self, oth):
             return False
-        if set(self._user_types) != set(oth._user_types) or set(self._objects) != set(
-            oth._objects
-        ):
+        if not ObjectsSetMixin.__eq__(self, oth):
+            return False
+        if not FluentsSetMixin.__eq__(self, oth):
+            return False
+        if not InitialStateMixin.__eq__(self, oth):
+            return False
+        if not MetricsMixin.__eq__(self, oth):
+            return False
+
+        if set(self._goals) != set(oth._goals):
             return False
         if set(self._actions) != set(oth._actions):
             return False
         if set(self._trajectory_constraints) != set(oth._trajectory_constraints):
             return False
-        oth_initial_values = oth.initial_values
-        initial_values = self.initial_values
-        if len(initial_values) != len(oth_initial_values):
-            return False
-        for fluent, value in initial_values.items():
-            oth_value = oth_initial_values.get(fluent, None)
-            if oth_value is None:
-                return False
-            elif value != oth_value:
-                return False
+
         if len(self._timed_effects) != len(oth._timed_effects):
             return False
         for t, tel in self._timed_effects.items():
             oth_tel = oth._timed_effects.get(t, None)
             if oth_tel is None:
                 return False
             elif set(tel) != set(oth_tel):
@@ -175,62 +193,59 @@
             if oth_tgl is None:
                 return False
             elif set(tgl) != set(oth_tgl):
                 return False
         return True
 
     def __hash__(self) -> int:
-        res = hash(self._kind) + hash(self._name)
-        for f in self._fluents:
-            res += hash(f)
+        res = hash(self._name)
+
+        res += FluentsSetMixin.__hash__(self)
+        res += ObjectsSetMixin.__hash__(self)
+        res += UserTypesSetMixin.__hash__(self)
+        res += InitialStateMixin.__hash__(self)
+        res += MetricsMixin.__hash__(self)
+
         for a in self._actions:
             res += hash(a)
-        for ut in self._user_types:
-            res += hash(ut)
-        for o in self._objects:
-            res += hash(o)
         for c in self._trajectory_constraints:
             res += hash(c)
-        for iv in self.initial_values.items():
-            res += hash(iv)
         for t, el in self._timed_effects.items():
             res += hash(t)
             for e in set(el):
                 res += hash(e)
         for i, gl in self._timed_goals.items():
             res += hash(i)
             for g in set(gl):
                 res += hash(g)
         for g in self._goals:
             res += hash(g)
         return res
 
     def clone(self):
         new_p = Problem(self._name, self._env)
-        new_p._fluents = self._fluents[:]
+        UserTypesSetMixin._clone_to(self, new_p)
+        ObjectsSetMixin._clone_to(self, new_p)
+        FluentsSetMixin._clone_to(self, new_p)
+        InitialStateMixin._clone_to(self, new_p)
+        TimeModelMixin._clone_to(self, new_p)
+
         new_p._actions = [a.clone() for a in self._actions]
-        new_p._user_types = self._user_types[:]
-        new_p._user_types_hierarchy = self._user_types_hierarchy.copy()
-        new_p._objects = self._objects[:]
-        new_p._initial_value = self._initial_value.copy()
         new_p._timed_effects = {
             t: [e.clone() for e in el] for t, el in self._timed_effects.items()
         }
         new_p._timed_goals = {i: [g for g in gl] for i, gl in self._timed_goals.items()}
         new_p._goals = self._goals[:]
         new_p._trajectory_constraints = self._trajectory_constraints[:]
-        new_p._metrics = []
-        for m in self._metrics:
-            if isinstance(m, up.model.metrics.MinimizeActionCosts):
-                costs = {new_p.action(a.name): c for a, c in m.costs.items()}
-                new_p._metrics.append(up.model.metrics.MinimizeActionCosts(costs))
-            else:
-                new_p._metrics.append(m)
-        new_p._initial_defaults = self._initial_defaults.copy()
-        new_p._fluents_defaults = self._fluents_defaults.copy()
+        new_p._fluents_assigned = {
+            t: d.copy() for t, d in self._fluents_assigned.items()
+        }
+
+        # last as it requires actions to be cloned already
+        MetricsMixin._clone_to(self, new_p, new_actions=new_p)
         return new_p
 
     def has_name(self, name: str) -> bool:
         """
         Returns `True` if the given `name` is already in the `Problem`, `False` otherwise.
 
         :param name: The target name to find in the `Problem`.
@@ -252,15 +267,15 @@
         :return: A `Plan` syntactically valid for this `Problem`.
         """
         return plan.replace_action_instances(self._replace_action_instance)
 
     def _replace_action_instance(
         self, action_instance: "up.plans.ActionInstance"
     ) -> "up.plans.ActionInstance":
-        em = self.env.expression_manager
+        em = self.environment.expression_manager
         new_a = self.action(action_instance.action.name)
         params = []
         for p in action_instance.actual_parameters:
             if p.is_object_exp():
                 obj = self.object(p.object().name)
                 params.append(em.ObjectExp(obj))
             elif p.is_bool_constant():
@@ -269,118 +284,94 @@
                 params.append(em.Int(cast(int, p.constant_value())))
             elif p.is_real_constant():
                 params.append(em.Real(cast(Fraction, p.constant_value())))
             else:
                 raise NotImplementedError
         return up.plans.ActionInstance(new_a, tuple(params))
 
-    def get_static_fluents(self) -> Set["up.model.fluent.Fluent"]:
+    def _get_static_and_unused_fluents(
+        self,
+    ) -> Tuple[Set["up.model.fluent.Fluent"], Set["up.model.fluent.Fluent"]]:
         """
-        Returns the set of the `static fluents`.
-
-        `Static fluents` are those who can't change their values because they never
-        appear in the :func:`fluent <unified_planning.model.Effect.fluent>` field of an `Effect`, therefore there are no :func:`Actions <unified_planning.model.Problem.actions>`
-        in the `Problem` that can change their value.
+        Support method to calculate the set of static fluents (The fluents that are never modified in the problem)
+        and the set of the unused fluents (The fluents that are never red in the problem.
+        NOTE: The fluents used only in the ActionCost quality metric are in the unused_fluents set anyway).
         """
         static_fluents: Set["up.model.fluent.Fluent"] = set(self._fluents)
+        unused_fluents: Set["up.model.fluent.Fluent"] = set(self._fluents)
+        fve = self._env.free_vars_extractor
+        # function that takes an FNode and removes all the fluents contained in the given FNode
+        # from the unused_fluents  set.
+        remove_used_fluents = lambda *exps: unused_fluents.difference_update(
+            (f.fluent() for e in exps for f in fve.get(e))
+        )
         for a in self._actions:
             if isinstance(a, up.model.action.InstantaneousAction):
+                remove_used_fluents(*a.preconditions)
                 for e in a.effects:
+                    remove_used_fluents(e.fluent, e.value, e.condition)
                     static_fluents.discard(e.fluent.fluent())
                 if a.simulated_effect is not None:
+                    # empty the set because a simulated effect reads all the fluents
+                    unused_fluents.clear()
                     for f in a.simulated_effect.fluents:
                         static_fluents.discard(f.fluent())
             elif isinstance(a, up.model.action.DurativeAction):
+                for cl in a.conditions.values():
+                    remove_used_fluents(*cl)
                 for el in a.effects.values():
                     for e in el:
+                        remove_used_fluents(e.fluent, e.value, e.condition)
                         static_fluents.discard(e.fluent.fluent())
-                for _, se in a.simulated_effects.items():
+                for se in a.simulated_effects.values():
+                    unused_fluents.clear()
                     for f in se.fluents:
                         static_fluents.discard(f.fluent())
             else:
                 raise NotImplementedError
         for el in self._timed_effects.values():
             for e in el:
-                if e.fluent.fluent() in static_fluents:
-                    static_fluents.remove(e.fluent.fluent())
-        return static_fluents
-
-    def set_initial_value(
-        self,
-        fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
-        value: Union[
-            "up.model.fnode.FNode",
-            "up.model.fluent.Fluent",
-            "up.model.object.Object",
-            bool,
-            int,
-            float,
-            Fraction,
-        ],
-    ):
-        """
-        Sets the initial value for the given `Fluent`. The given `Fluent` must be grounded, therefore if
-        it's :func:`arity <unified_planning.model.Fluent.arity>` is `> 0`, the `fluent` parameter must be
-        an `FNode` and the method :func:`~unified_planning.model.FNode.is_fluent_exp` must return `True`.
-
-        :param fluent: The grounded `Fluent` of which the initial value must be set.
-        :param value: The `value` assigned in the initial state to the given `fluent`.
-        """
-        fluent_exp, value_exp = self._env.expression_manager.auto_promote(fluent, value)
-        if not fluent_exp.type.is_compatible(value_exp.type):
-            raise UPTypeError("Initial value assignment has not compatible types!")
-        self._initial_value[fluent_exp] = value_exp
-
-    def initial_value(
-        self, fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"]
-    ) -> "up.model.fnode.FNode":
-        """
-        Retrieves the initial value assigned to the given `fluent`.
-
-        :param fluent: The target `fluent` of which the `value` in the initial state must be retrieved.
-        :return: The `value` expression assigned to the given `fluent` in the initial state.
-        """
-        (fluent_exp,) = self._env.expression_manager.auto_promote(fluent)
-        for a in fluent_exp.args:
-            if not a.is_constant():
-                raise UPExpressionDefinitionError(
-                    f"Impossible to return the initial value of a fluent expression with no constant arguments: {fluent_exp}."
-                )
-        if fluent_exp in self._initial_value:
-            return self._initial_value[fluent_exp]
-        elif fluent_exp.fluent() in self._fluents_defaults:
-            return self._fluents_defaults[fluent_exp.fluent()]
-        else:
-            raise UPProblemDefinitionError("Initial value not set!")
+                remove_used_fluents(e.fluent, e.value, e.condition)
+                static_fluents.discard(e.fluent.fluent())
+        for gl in self._timed_goals.values():
+            remove_used_fluents(*gl)
+        remove_used_fluents(*self._trajectory_constraints)
+        remove_used_fluents(*self._goals)
+        for qm in self.quality_metrics:
+            if isinstance(
+                qm,
+                (
+                    up.model.metrics.MinimizeExpressionOnFinalState,
+                    up.model.metrics.MaximizeExpressionOnFinalState,
+                ),
+            ):
+                remove_used_fluents(qm.expression)
+            elif isinstance(qm, up.model.metrics.Oversubscription):
+                remove_used_fluents(*qm.goals.keys())
+            elif isinstance(qm, up.model.metrics.TemporalOversubscription):
+                for _, g in qm.goals.keys():
+                    remove_used_fluents(g)
+        return static_fluents, unused_fluents
 
-    @property
-    def initial_values(self) -> Dict["up.model.fnode.FNode", "up.model.fnode.FNode"]:
+    def get_static_fluents(self) -> Set["up.model.fluent.Fluent"]:
         """
-        Gets the initial value of all the grounded fluents present in the `Problem`.
+        Returns the set of the `static fluents`.
 
-        IMPORTANT NOTE: this property does a lot of computation, so it should be called as
-        seldom as possible.
+        `Static fluents` are those who can't change their values because they never
+        appear in the :func:`fluent <unified_planning.model.Effect.fluent>` field of an `Effect`, therefore there are no :func:`Actions <unified_planning.model.Problem.actions>`
+        in the `Problem` that can change their value.
         """
-        res = self._initial_value
-        for f in self._fluents:
-            for f_exp in get_all_fluent_exp(self, f):
-                res[f_exp] = self.initial_value(f_exp)
-        return res
+        return self._get_static_and_unused_fluents()[0]
 
     @property
-    def explicit_initial_values(
+    def timed_goals(
         self,
-    ) -> Dict["up.model.fnode.FNode", "up.model.fnode.FNode"]:
-        """
-        Returns the problem's defined initial values; those are only the initial values set with the
-        :func:`~unified_planning.model.Problem.set_initial_value` method.
-
-        IMPORTANT NOTE: For all the initial values of the problem use :func:`initial_values <unified_planning.model.Problem.initial_values>`.
-        """
-        return self._initial_value
+    ) -> Dict["up.model.timing.TimeInterval", List["up.model.fnode.FNode"]]:
+        """Returns all the `timed goals` in the `Problem`."""
+        return self._timed_goals
 
     def add_timed_goal(
         self,
         interval: Union["up.model.timing.Timing", "up.model.timing.TimeInterval"],
         goal: Union["up.model.fnode.FNode", "up.model.fluent.Fluent", bool],
     ):
         """
@@ -403,25 +394,25 @@
             )
         (goal_exp,) = self._env.expression_manager.auto_promote(goal)
         assert self._env.type_checker.get_type(goal_exp).is_bool_type()
         goals = self._timed_goals.setdefault(interval, [])
         if goal_exp not in goals:
             goals.append(goal_exp)
 
-    @property
-    def timed_goals(
-        self,
-    ) -> Dict["up.model.timing.TimeInterval", List["up.model.fnode.FNode"]]:
-        """Returns all the `timed goals` in the `Problem`."""
-        return self._timed_goals
-
     def clear_timed_goals(self):
         """Removes all the `timed goals` from the `Problem`."""
         self._timed_goals = {}
 
+    @property
+    def timed_effects(
+        self,
+    ) -> Dict["up.model.timing.Timing", List["up.model.effect.Effect"]]:
+        """Returns all the `timed effects` in the `Problem`."""
+        return self._timed_effects
+
     def add_timed_effect(
         self,
         timing: "up.model.timing.Timing",
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
     ):
@@ -530,28 +521,36 @@
 
     def _add_effect_instance(
         self, timing: "up.model.timing.Timing", effect: "up.model.effect.Effect"
     ):
         assert (
             effect.environment == self._env
         ), "effect does not have the same environment of the problem"
-        effects = self._timed_effects.setdefault(timing, [])
-        if effect not in effects:
-            effects.append(effect)
+        fluents_inc_dec = self._fluents_inc_dec.setdefault(timing, set())
 
-    @property
-    def timed_effects(
-        self,
-    ) -> Dict["up.model.timing.Timing", List["up.model.effect.Effect"]]:
-        """Returns all the `timed effects` in the `Problem`."""
-        return self._timed_effects
+        up.model.effect.check_conflicting_effects(
+            effect,
+            timing,
+            None,
+            self._fluents_assigned.setdefault(timing, {}),
+            fluents_inc_dec,
+            "problem",
+        )
+        self._timed_effects.setdefault(timing, []).append(effect)
 
     def clear_timed_effects(self):
         """Removes all the `timed effects` from the `Problem`."""
         self._timed_effects = {}
+        self._fluents_assigned = {}
+        self._fluents_inc_dec = {}
+
+    @property
+    def goals(self) -> List["up.model.fnode.FNode"]:
+        """Returns all the `goals` in the `Problem`."""
+        return self._goals
 
     def add_goal(
         self, goal: Union["up.model.fnode.FNode", "up.model.fluent.Fluent", bool]
     ):
         """
         Adds the given `goal` to the `Problem`; a goal is an expression that must be evaluated to `True` at the
         end of the execution of a :class:`~unified_planning.plans.Plan`. If a `Plan` does not satisfy all the given `goals`, it is not valid.
@@ -562,14 +561,23 @@
             isinstance(goal, bool) or goal.environment == self._env
         ), "goal does not have the same environment of the problem"
         (goal_exp,) = self._env.expression_manager.auto_promote(goal)
         assert self._env.type_checker.get_type(goal_exp).is_bool_type()
         if goal_exp != self._env.expression_manager.TRUE():
             self._goals.append(goal_exp)
 
+    def clear_goals(self):
+        """Removes all the `goals` from the `Problem`."""
+        self._goals = []
+
+    @property
+    def trajectory_constraints(self) -> List["up.model.fnode.FNode"]:
+        """Returns the 'trajectory_constraints' in the 'Problem'."""
+        return self._trajectory_constraints
+
     def add_trajectory_constraint(self, constraint: "up.model.fnode.FNode"):
         """
         Adds the given `trajectory_constraint` to the `Problem`;
         a trajectory_constraint is an expression defined as:
         Always, Sometime, At-Most-Once, Sometime-Before, Sometime-After or
         defined with universal quantifiers.
         Nesting of these temporal operators is forbidden.
@@ -591,135 +599,62 @@
                 or constraint.is_sometime_after()
                 or constraint.is_sometime_before()
                 or constraint.is_at_most_once()
                 or constraint.is_always()
             ), "trajectory constraint not in the correct form"
         self._trajectory_constraints.append(constraint.simplify())
 
-    @property
-    def goals(self) -> List["up.model.fnode.FNode"]:
-        """Returns all the `goals` in the `Problem`."""
-        return self._goals
-
-    @property
-    def trajectory_constraints(self) -> List["up.model.fnode.FNode"]:
-        """Returns the 'trajectory_constraints' in the 'Problem'."""
-        return self._trajectory_constraints
-
-    def clear_goals(self):
-        """Removes all the `goals` from the `Problem`."""
-        self._goals = []
-
     def clear_trajectory_constraints(self):
         """Removes the trajectory_constraints."""
         self._trajectory_constraints = []
 
-    def add_quality_metric(self, metric: "up.model.metrics.PlanQualityMetric"):
-        """
-        Adds the given `quality metric` to the `Problem`; a `quality metric` defines extra requirements that a :class:`~unified_planning.plans.Plan`
-        must satisfy in order to be valid.
-
-        :param metric: The `quality metric` that a `Plan` of this `Problem` must satisfy in order to be valid.
-        """
-        self._metrics.append(metric)
-
-    @property
-    def quality_metrics(self) -> List["up.model.metrics.PlanQualityMetric"]:
-        """Returns all the `quality metrics` in the `Problem`."""
-        return self._metrics
-
-    def clear_quality_metrics(self):
-        """Removes all the `quality metrics` in the `Problem`."""
-        self._metrics = []
-
     @property
     def kind(self) -> "up.model.problem_kind.ProblemKind":
         """
         Calculates and returns the `problem kind` of this `planning problem`.
         If the `Problem` is modified, this method must be called again in order to be reliable.
 
         IMPORTANT NOTE: this property does a lot of computation, so it should be called as
         seldom as possible.
         """
         # Create the needed data structures
-        fluents_to_only_increase: Set["up.model.fluent.Fluent"] = set()
-        fluents_to_only_decrease: Set["up.model.fluent.Fluent"] = set()
-        static_fluents: Set["up.model.fluent.Fluent"] = self.get_static_fluents()
+        static_fluents, unused_fluents = self._get_static_and_unused_fluents()
 
         # Create a simplifier and a linear_checker with the problem, so static fluents can be considered as constants
         simplifier = up.model.walkers.simplifier.Simplifier(self._env, self)
         linear_checker = up.model.walkers.linear_checker.LinearChecker(self)
         self._kind = up.model.problem_kind.ProblemKind()
         self._kind.set_problem_class("ACTION_BASED")
         self._kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
-        for metric in self._metrics:
-            if isinstance(metric, up.model.metrics.MinimizeExpressionOnFinalState):
-                self._kind.set_quality_metrics("FINAL_VALUE")
-                (
-                    is_linear,
-                    fnode_to_only_increase,  # positive fluents in minimize can only be increased
-                    fnode_to_only_decrease,  # negative fluents in minimize can only be decreased
-                ) = linear_checker.get_fluents(metric.expression)
-                if is_linear:
-                    fluents_to_only_increase = {
-                        e.fluent() for e in fnode_to_only_increase
-                    }
-                    fluents_to_only_decrease = {
-                        e.fluent() for e in fnode_to_only_decrease
-                    }
-                else:
-                    self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
-            elif isinstance(metric, up.model.metrics.MaximizeExpressionOnFinalState):
-                self._kind.set_quality_metrics("FINAL_VALUE")
-                (
-                    is_linear,
-                    fnode_to_only_decrease,  # positive fluents in maximize can only be decreased
-                    fnode_to_only_increase,  # negative fluents in maximize can only be increased
-                ) = linear_checker.get_fluents(metric.expression)
-                if is_linear:
-                    fluents_to_only_increase = {
-                        e.fluent() for e in fnode_to_only_increase
-                    }
-                    fluents_to_only_decrease = {
-                        e.fluent() for e in fnode_to_only_decrease
-                    }
-                else:
-                    self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
-            elif isinstance(metric, up.model.metrics.MinimizeActionCosts):
-                self._kind.set_quality_metrics("ACTIONS_COST")
-            elif isinstance(metric, up.model.metrics.MinimizeMakespan):
-                self._kind.set_quality_metrics("MAKESPAN")
-            elif isinstance(metric, up.model.metrics.MinimizeSequentialPlanLength):
-                self._kind.set_quality_metrics("PLAN_LENGTH")
-            elif isinstance(metric, up.model.metrics.Oversubscription):
-                self._kind.set_quality_metrics("OVERSUBSCRIPTION")
-            else:
-                assert False, "Unknown quality metric"
+        fluents_to_only_increase, fluents_to_only_decrease = self._update_kind_metric(
+            self._kind, linear_checker, static_fluents
+        )
         for fluent in self._fluents:
-            self._update_problem_kind_fluent(fluent)
+            self._update_problem_kind_fluent(fluent, unused_fluents)
         for object in self._objects:
             self._update_problem_kind_type(object.type)
         for action in self._actions:
             self._update_problem_kind_action(
                 action,
                 fluents_to_only_increase,
                 fluents_to_only_decrease,
                 static_fluents,
                 simplifier,
                 linear_checker,
             )
         if len(self._timed_effects) > 0:
             self._kind.set_time("CONTINUOUS_TIME")
-            self._kind.set_time("TIMED_EFFECT")
+            self._kind.set_time("TIMED_EFFECTS")
         for effect_list in self._timed_effects.values():
             for effect in effect_list:
                 self._update_problem_kind_effect(
                     effect,
                     fluents_to_only_increase,
                     fluents_to_only_decrease,
+                    static_fluents,
                     simplifier,
                     linear_checker,
                 )
         if len(self._timed_goals) > 0:
             self._kind.set_time("TIMED_GOALS")
             self._kind.set_time("CONTINUOUS_TIME")
         if len(self._trajectory_constraints) > 0:
@@ -733,21 +668,25 @@
             not self._kind.has_continuous_numbers()
             and not self._kind.has_discrete_numbers()
         ):
             self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
         else:
             if not self._kind.has_simple_numeric_planning():
                 self._kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
+        if self._kind.has_continuous_time() and self.discrete_time:
+            self._kind.set_time("DISCRETE_TIME")
+            self._kind.unset_time("CONTINUOUS_TIME")
         return self._kind
 
     def _update_problem_kind_effect(
         self,
         e: "up.model.effect.Effect",
         fluents_to_only_increase: Set["up.model.fluent.Fluent"],
         fluents_to_only_decrease: Set["up.model.fluent.Fluent"],
+        static_fluents: Set["up.model.fluent.Fluent"],
         simplifier: "up.model.walkers.simplifier.Simplifier",
         linear_checker: "up.model.walkers.linear_checker.LinearChecker",
     ):
         value = simplifier.simplify(e.value)
         if e.is_conditional():
             self._update_problem_kind_condition(e.condition, linear_checker)
             self._kind.set_effects_kind("CONDITIONAL_EFFECTS")
@@ -781,33 +720,44 @@
                     e.fluent in fluents_to_only_decrease and value.constant_value() < 0
                 ):
                     self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
             else:
                 self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
         elif e.is_assignment():
             value_type = value.type
+            value = e.value
+            fluents_in_value = self._env.free_vars_extractor.get(value)
             if (
                 value_type.is_int_type() or value_type.is_real_type()
             ):  # the value is a number
                 if (  # if the fluent has increase/decrease constraints or the value assigned is not a constant,
                     # unset "SIMPLE_NUMERIC_PLANNING"
                     e.fluent in fluents_to_only_increase
                     or e.fluent in fluents_to_only_decrease
                     or not value.is_constant()
                 ):
                     self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+            if any(f in static_fluents for f in fluents_in_value):
+                self._kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+            if any(f not in static_fluents for f in fluents_in_value):
+                self._kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+            elif value.type.is_bool_type():
+                if any(f in static_fluents for f in fluents_in_value):
+                    self._kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+                if any(f not in static_fluents for f in fluents_in_value):
+                    self._kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
 
     def _update_problem_kind_condition(
         self,
         exp: "up.model.fnode.FNode",
         linear_checker: "up.model.walkers.linear_checker.LinearChecker",
     ):
         ops = self._operators_extractor.get(exp)
         if OperatorKind.EQUALS in ops:
-            self._kind.set_conditions_kind("EQUALITY")
+            self._kind.set_conditions_kind("EQUALITIES")
         if OperatorKind.NOT in ops:
             self._kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         if OperatorKind.OR in ops:
             self._kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         if OperatorKind.EXISTS in ops:
             self._kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         if OperatorKind.FORALL in ops:
@@ -822,21 +772,40 @@
             if cast(up.model.types._UserType, type).father is not None:
                 self._kind.set_typing("HIERARCHICAL_TYPING")
         elif type.is_int_type():
             self._kind.set_numbers("DISCRETE_NUMBERS")
         elif type.is_real_type():
             self._kind.set_numbers("CONTINUOUS_NUMBERS")
 
-    def _update_problem_kind_fluent(self, fluent: "up.model.fluent.Fluent"):
-        self._update_problem_kind_type(fluent.type)
-        if fluent.type.is_int_type() or fluent.type.is_real_type():
-            self._kind.set_fluents_type("NUMERIC_FLUENTS")
-        elif fluent.type.is_user_type():
+    def _update_problem_kind_fluent(
+        self,
+        fluent: "up.model.fluent.Fluent",
+        unused_fluents: Set["up.model.fluent.Fluent"],
+    ):
+        type = fluent.type
+        if fluent not in unused_fluents or (
+            not type.is_int_type() and not type.is_real_type()
+        ):
+            self._update_problem_kind_type(type)
+        if fluent.type.is_int_type() or type.is_real_type():
+            numeric_type = type
+            assert isinstance(
+                numeric_type, (up.model.types._RealType, up.model.types._IntType)
+            )
+            if (
+                numeric_type.lower_bound is not None
+                or numeric_type.upper_bound is not None
+            ):
+                self._kind.set_numbers("BOUNDED_TYPES")
+            if fluent not in unused_fluents:
+                self._kind.set_fluents_type("NUMERIC_FLUENTS")
+        elif type.is_user_type():
             self._kind.set_fluents_type("OBJECT_FLUENTS")
         for p in fluent.signature:
+            # TODO understant if here we need a check that the fluent is not unused
             self._update_problem_kind_type(p.type)
 
     def _update_problem_kind_action(
         self,
         action: "up.model.action.Action",
         fluents_to_only_increase: Set["up.model.fluent.Fluent"],
         fluents_to_only_decrease: Set["up.model.fluent.Fluent"],
@@ -844,57 +813,73 @@
         simplifier: "up.model.walkers.simplifier.Simplifier",
         linear_checker: "up.model.walkers.linear_checker.LinearChecker",
     ):
         for p in action.parameters:
             self._update_problem_kind_type(p.type)
         if isinstance(action, up.model.action.SensingAction):
             self._kind.set_problem_class("CONTINGENT")
+        if isinstance(action, up.model.tamp.InstantaneousMotionAction):
+            if len(action.motion_constraints) > 0:
+                self._kind.set_problem_class("TAMP")
         if isinstance(action, up.model.action.InstantaneousAction):
             for c in action.preconditions:
                 self._update_problem_kind_condition(c, linear_checker)
             for e in action.effects:
                 self._update_problem_kind_effect(
                     e,
                     fluents_to_only_increase,
                     fluents_to_only_decrease,
+                    static_fluents,
                     simplifier,
                     linear_checker,
                 )
             if action.simulated_effect is not None:
                 self._kind.set_simulated_entities("SIMULATED_EFFECTS")
         elif isinstance(action, up.model.action.DurativeAction):
             lower, upper = action.duration.lower, action.duration.upper
             if lower != upper:
                 self._kind.set_time("DURATION_INEQUALITIES")
-            free_vars = self.env.free_vars_extractor.get(
+            free_vars = self.environment.free_vars_extractor.get(
                 lower
-            ) | self.env.free_vars_extractor.get(upper)
+            ) | self.environment.free_vars_extractor.get(upper)
             if len(free_vars) > 0:
                 only_static = True
                 for fv in free_vars:
                     if fv.fluent() not in static_fluents:
                         only_static = False
                         break
                 if only_static:
-                    self._kind.set_expression_duration("STATIC_FLUENTS_IN_DURATION")
+                    self._kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
                 else:
-                    self._kind.set_expression_duration("FLUENTS_IN_DURATION")
+                    self._kind.set_expression_duration("FLUENTS_IN_DURATIONS")
             for i, lc in action.conditions.items():
                 if i.lower.delay != 0 or i.upper.delay != 0:
-                    self._kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
+                    for t in [i.lower, i.upper]:
+                        if (t.is_from_start() and t.delay > 0) or (
+                            t.is_from_end() and t.delay < 0
+                        ):
+                            self._kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
+                        else:
+                            self._kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
                 for c in lc:
                     self._update_problem_kind_condition(c, linear_checker)
             for t, le in action.effects.items():
                 if t.delay != 0:
-                    self._kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
+                    if (t.is_from_start() and t.delay > 0) or (
+                        t.is_from_end() and t.delay < 0
+                    ):
+                        self._kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
+                    else:
+                        self._kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
                 for e in le:
                     self._update_problem_kind_effect(
                         e,
                         fluents_to_only_increase,
                         fluents_to_only_decrease,
+                        static_fluents,
                         simplifier,
                         linear_checker,
                     )
             if len(action.simulated_effects) > 0:
                 self._kind.set_simulated_entities("SIMULATED_EFFECTS")
             self._kind.set_time("CONTINUOUS_TIME")
         else:
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/problem_kind.py` & `unified_planning-0.6.0/unified_planning/model/problem_kind.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,45 +16,71 @@
 from functools import partialmethod, total_ordering
 from typing import Dict, List, Set
 import unified_planning as up
 
 
 # TODO: This features map needs to be extended with all the problem characterizations.
 FEATURES = {
-    "PROBLEM_CLASS": ["ACTION_BASED", "HIERARCHICAL", "CONTINGENT"],
+    "PROBLEM_CLASS": [
+        "ACTION_BASED",
+        "HIERARCHICAL",
+        "CONTINGENT",
+        "ACTION_BASED_MULTI_AGENT",
+        "SCHEDULING",
+        "TAMP",
+    ],
     "PROBLEM_TYPE": ["SIMPLE_NUMERIC_PLANNING", "GENERAL_NUMERIC_PLANNING"],
     "TIME": [
         "CONTINUOUS_TIME",
         "DISCRETE_TIME",
         "INTERMEDIATE_CONDITIONS_AND_EFFECTS",
-        "TIMED_EFFECT",
+        "EXTERNAL_CONDITIONS_AND_EFFECTS",
+        "TIMED_EFFECTS",
         "TIMED_GOALS",
         "DURATION_INEQUALITIES",
     ],
-    "EXPRESSION_DURATION": ["STATIC_FLUENTS_IN_DURATION", "FLUENTS_IN_DURATION"],
-    "NUMBERS": ["CONTINUOUS_NUMBERS", "DISCRETE_NUMBERS"],
+    "EXPRESSION_DURATION": ["STATIC_FLUENTS_IN_DURATIONS", "FLUENTS_IN_DURATIONS"],
+    "NUMBERS": ["CONTINUOUS_NUMBERS", "DISCRETE_NUMBERS", "BOUNDED_TYPES"],
     "CONDITIONS_KIND": [
         "NEGATIVE_CONDITIONS",
         "DISJUNCTIVE_CONDITIONS",
-        "EQUALITY",
+        "EQUALITIES",
         "EXISTENTIAL_CONDITIONS",
         "UNIVERSAL_CONDITIONS",
     ],
-    "EFFECTS_KIND": ["CONDITIONAL_EFFECTS", "INCREASE_EFFECTS", "DECREASE_EFFECTS"],
+    "EFFECTS_KIND": [
+        "CONDITIONAL_EFFECTS",
+        "INCREASE_EFFECTS",
+        "DECREASE_EFFECTS",
+        "STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS",
+        "STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS",
+        "FLUENTS_IN_BOOLEAN_ASSIGNMENTS",
+        "FLUENTS_IN_NUMERIC_ASSIGNMENTS",
+    ],
     "TYPING": ["FLAT_TYPING", "HIERARCHICAL_TYPING"],
     "FLUENTS_TYPE": ["NUMERIC_FLUENTS", "OBJECT_FLUENTS"],
     "QUALITY_METRICS": [
         "ACTIONS_COST",
         "FINAL_VALUE",
         "MAKESPAN",
         "PLAN_LENGTH",
         "OVERSUBSCRIPTION",
+        "TEMPORAL_OVERSUBSCRIPTION",
     ],
+    "ACTIONS_COST_KIND": ["STATIC_FLUENTS_IN_ACTIONS_COST", "FLUENTS_IN_ACTIONS_COST"],
     "SIMULATED_ENTITIES": ["SIMULATED_EFFECTS"],
     "CONSTRAINTS_KIND": ["TRAJECTORY_CONSTRAINTS"],
+    "HIERARCHICAL": [
+        "METHOD_PRECONDITIONS",
+        "TASK_NETWORK_CONSTRAINTS",
+        "INITIAL_TASK_NETWORK_VARIABLES",
+        "TASK_ORDER_TOTAL",
+        "TASK_ORDER_PARTIAL",
+        "TASK_ORDER_TEMPORAL",
+    ],
 }
 
 
 class ProblemKindMeta(type):
     """Meta class used to interpret the nodehandler decorator."""
 
     def __new__(cls, name, bases, dct):
@@ -162,22 +188,22 @@
 hierarchical_kind.set_typing("HIERARCHICAL_TYPING")
 
 classical_kind = ProblemKind()
 classical_kind.set_problem_class("ACTION_BASED")
 classical_kind.set_typing("FLAT_TYPING")
 classical_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
 classical_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-classical_kind.set_conditions_kind("EQUALITY")
+classical_kind.set_conditions_kind("EQUALITIES")
 
 full_classical_kind = ProblemKind()
 full_classical_kind.set_problem_class("ACTION_BASED")
 full_classical_kind.set_typing("FLAT_TYPING")
 full_classical_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
 full_classical_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-full_classical_kind.set_conditions_kind("EQUALITY")
+full_classical_kind.set_conditions_kind("EQUALITIES")
 full_classical_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
 full_classical_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
 full_classical_kind.set_effects_kind("CONDITIONAL_EFFECTS")
 
 object_fluent_kind = ProblemKind()
 object_fluent_kind.set_fluents_type("OBJECT_FLUENTS")
 
@@ -195,32 +221,48 @@
 general_numeric_kind.set_problem_class("ACTION_BASED")
 general_numeric_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
 general_numeric_kind.set_typing("FLAT_TYPING")
 general_numeric_kind.set_numbers("DISCRETE_NUMBERS")
 general_numeric_kind.set_numbers("CONTINUOUS_NUMBERS")
 general_numeric_kind.set_fluents_type("NUMERIC_FLUENTS")
 
+bounded_types_kind = ProblemKind()
+bounded_types_kind.set_numbers("BOUNDED_TYPES")
+
 basic_temporal_kind = ProblemKind()
 basic_temporal_kind.set_problem_class("ACTION_BASED")
 basic_temporal_kind.set_typing("FLAT_TYPING")
 basic_temporal_kind.set_time("CONTINUOUS_TIME")
 
 temporal_kind = ProblemKind()
 temporal_kind.set_problem_class("ACTION_BASED")
 temporal_kind.set_typing("FLAT_TYPING")
 temporal_kind.set_time("CONTINUOUS_TIME")
 temporal_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-temporal_kind.set_time("TIMED_EFFECT")
+temporal_kind.set_time("TIMED_EFFECTS")
 temporal_kind.set_time("TIMED_GOALS")
 temporal_kind.set_time("DURATION_INEQUALITIES")
-temporal_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATION")
+temporal_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
 
 quality_metrics_kind = ProblemKind()
 quality_metrics_kind.set_quality_metrics("PLAN_LENGTH")
 quality_metrics_kind.set_quality_metrics("ACTIONS_COST")
 quality_metrics_kind.set_quality_metrics("FINAL_VALUE")
 
 oversubscription_kind = ProblemKind()
 oversubscription_kind.set_quality_metrics("OVERSUBSCRIPTION")
 
 actions_cost_kind = ProblemKind()
 actions_cost_kind.set_quality_metrics("ACTIONS_COST")
+
+multi_agent_kind = ProblemKind()
+multi_agent_kind.set_problem_class("ACTION_BASED_MULTI_AGENT")
+multi_agent_kind.set_typing("FLAT_TYPING")
+multi_agent_kind.set_typing("HIERARCHICAL_TYPING")
+multi_agent_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
+multi_agent_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
+multi_agent_kind.set_conditions_kind("EQUALITIES")
+multi_agent_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
+multi_agent_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
+multi_agent_kind.set_effects_kind("CONDITIONAL_EFFECTS")
+multi_agent_kind.set_fluents_type("NUMERIC_FLUENTS")
+multi_agent_kind.set_fluents_type("OBJECT_FLUENTS")
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/timing.py` & `unified_planning-0.6.0/unified_planning/model/timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 from unified_planning.environment import Environment
 from unified_planning.model.fnode import FNode
+from unified_planning.model.expression import NumericConstant, uniform_numeric_constant
+from abc import ABC
 from enum import Enum, auto
 from fractions import Fraction
 from typing import Union, Optional
 
 
 class TimepointKind(Enum):
     """
@@ -78,14 +80,20 @@
             return self._kind == oth._kind and self._container == oth._container
         else:
             return False
 
     def __hash__(self) -> int:
         return hash(self._kind) + hash(self._container)
 
+    def __add__(self, delay: Union[int, Fraction]) -> "Timing":
+        return Timing(delay, self)
+
+    def __sub__(self, delay: Union[int, Fraction]) -> "Timing":
+        return Timing(-delay, self)
+
     @property
     def kind(self) -> TimepointKind:
         """Returns the `kind` of this `Timepoint`; the `kind` defines the semantic of the `Timepoint`."""
         return self._kind
 
     @property
     def container(self):
@@ -97,17 +105,17 @@
     """
     Class that used a :class:`~unified_planning.model.Timepoint` to define from when this `Timing` is considered and a :func:`delay <unified_planning.model.Timing.delay>`,
     representing the distance from the given `Timepoint`.
     For example:
     A `GLOBAL_START Timepoint` with a `delay` of `5` means `5` units of time after the start of the `Plan`.
     """
 
-    def __init__(self, delay: Union[int, Fraction], timepoint: Timepoint):
+    def __init__(self, delay: NumericConstant, timepoint: Timepoint):
         self._timepoint = timepoint
-        self._delay = delay
+        self._delay = uniform_numeric_constant(delay)
 
     def __repr__(self):
         if self._delay == 0:
             return f"{self._timepoint}"
         else:
             return f"{self._timepoint} + {self._delay}"
 
@@ -116,14 +124,20 @@
             return self._delay == oth._delay and self._timepoint == oth._timepoint
         else:
             return False
 
     def __hash__(self) -> int:
         return hash(self._delay) ^ hash(self._timepoint)
 
+    def __add__(self, delay: Union[int, Fraction]) -> "Timing":
+        return Timing(self.delay + delay, self.timepoint)
+
+    def __sub__(self, delay: Union[int, Fraction]) -> "Timing":
+        return Timing(self.delay - delay, self.timepoint)
+
     @property
     def delay(self) -> Union[int, Fraction]:
         """Returns the `delay` set for this `Timing` from the `timepoint`."""
         return self._delay
 
     @property
     def timepoint(self) -> Timepoint:
@@ -148,17 +162,15 @@
         )
 
     def is_from_end(self) -> bool:
         """Returns `True` if this `Timing` is from the end, `False` if it is from the start."""
         return not self.is_from_start()
 
 
-def StartTiming(
-    delay: Union[int, Fraction] = 0, container: Optional[str] = None
-) -> Timing:
+def StartTiming(delay: NumericConstant = 0, container: Optional[str] = None) -> Timing:
     """
     Returns the start timing of an :class:`~unified_planning.model.Action`.
     Created with a delay > 0 represents "delay" time
     after the start of the `Action`.
 
     For example, action starts at time 5:
     `StartTiming() = 5`
@@ -169,59 +181,54 @@
         If not set, then refers to the enclosing `Action or method`.
     :return: The created `Timing`.
     """
 
     return Timing(delay, Timepoint(TimepointKind.START, container=container))
 
 
-def EndTiming(
-    delay: Union[int, Fraction] = 0, container: Optional[str] = None
-) -> Timing:
+def EndTiming(container: Optional[str] = None) -> Timing:
     """
     Returns the end timing of an :class:`~unified_planning.model.Action`.
-    Created with a delay > 0 represents `delay` time
-    before the end of the `Action`.
 
     For example, `Action` ends at time 10:
     `EndTiming() = 10`
-    `EndTiming(1.5) = 10-Fraction(3, 2) = Fraction(17, 2) = 8.5`.
+    `EndTiming() - 4 = 10 - 4 = 6`.
 
-    :param delay: The delay from the end of an `Action`.
     :param container: Identifier of the container in which the `Timepoint` is defined.
         If not set, then refers to the enclosing `action or method`.
     :return: The created `Timing`.
     """
 
-    return Timing(delay, Timepoint(TimepointKind.END, container=container))
+    return Timing(delay=0, timepoint=Timepoint(TimepointKind.END, container=container))
 
 
-def GlobalStartTiming(delay: Union[int, Fraction] = 0):
+def GlobalStartTiming(delay: NumericConstant = 0):
     """
     Represents the absolute `Timing`.
     Created with a delay > 0 represents `delay` time
     after the start of the execution.
 
     :param delay: The delay from the start of the `Plan`.
     :return: The created `Timing`.
     """
 
     return Timing(delay, Timepoint(TimepointKind.GLOBAL_START))
 
 
-def GlobalEndTiming(delay: Union[int, Fraction] = 0):
+def GlobalEndTiming():
     """
     Represents the end `Timing` of an execution.
     Created with a delay > 0 represents "delay" time
     before the end of the execution.
 
     :param delay: The delay from the start of the `Plan`.
     :return: The created `Timing`.
     """
 
-    return Timing(delay, Timepoint(TimepointKind.GLOBAL_END))
+    return Timing(delay=0, timepoint=Timepoint(TimepointKind.GLOBAL_END))
 
 
 class Interval:
     """Class that defines an `interval` with 2 :class:`expressions <unified_planning.model.FNode>` as bounds."""
 
     def __init__(
         self,
@@ -288,15 +295,15 @@
         return self._is_left_open
 
     def is_right_open(self) -> bool:
         """Returns `True` if the `upper` bound of this `Interval` is not included in the `Interval`, `False` otherwise."""
         return self._is_right_open
 
 
-class Duration:
+class Duration(ABC):
     pass
 
 
 class DurationInterval(Duration, Interval):
     """Class used to indicate that an `Interval` is also a `Duration`."""
 
     def __init__(
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/types.py` & `unified_planning-0.6.0/unified_planning/model/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines all the types."""
 
 import unified_planning
-from fractions import Fraction
-from typing import Iterator, Optional, Dict, Tuple, Union, cast
+from typing import Iterator, Optional, cast
 from unified_planning.exceptions import UPProblemDefinitionError, UPTypeError
+from abc import ABC
+from fractions import Fraction
 
 
-class Type:
+class Type(ABC):
     """Base class for representing a `Type`."""
 
     def is_bool_type(self) -> bool:
         """Returns `True` iff is `boolean Type`."""
         return False
 
     def is_user_type(self) -> bool:
@@ -36,15 +37,23 @@
         return False
 
     def is_int_type(self) -> bool:
         """Returns `True` iff is `integer Type`."""
         return False
 
     def is_time_type(self) -> bool:
-        """Returns `True` iff is `time `True`."""
+        """Returns `True` iff is `time Type`."""
+        return False
+
+    def is_movable_type(self) -> bool:
+        """Returns `True` iff is `movable Type`."""
+        return False
+
+    def is_configuration_type(self) -> bool:
+        """Returns `True` iff is `configuration Type`."""
         return False
 
     def is_compatible(self, t_right: "Type") -> bool:
         """
         Returns `True` if the `Type` `t_right` can be assigned to a :class:`~unified_planning.model.Fluent` that which :func:`type <unified_planning.model.Fluent.type>` is self.
         Note that types compatibility is not a symmetric property.
 
@@ -131,20 +140,26 @@
             if p == t:
                 return True
             p = cast(_UserType, p).father
         return False
 
 
 class _IntType(Type):
-    """Represents an Integer type. The given bounds are not semantically bounding for the planners."""
+    """Represents an Integer type. The given bounds are semantically bounding for the planners."""
 
     def __init__(
         self, lower_bound: Optional[int] = None, upper_bound: Optional[int] = None
     ):
         Type.__init__(self)
+        assert lower_bound is None or isinstance(
+            lower_bound, int
+        ), "typing not respected"
+        assert upper_bound is None or isinstance(
+            upper_bound, int
+        ), "typing not respected"
         self._lower_bound = lower_bound
         self._upper_bound = upper_bound
 
     def __repr__(self) -> str:
         b = []
         if (not self.lower_bound is None) or (not self.upper_bound is None):
             b.append("[")
@@ -165,22 +180,28 @@
         return self._upper_bound
 
     def is_int_type(self) -> bool:
         return True
 
 
 class _RealType(Type):
-    """Represents a Real type. The given bounds are not semantically bounding for the planners."""
+    """Represents a Real type. The given bounds are semantically bounding for the planners."""
 
     def __init__(
         self,
         lower_bound: Optional[Fraction] = None,
         upper_bound: Optional[Fraction] = None,
     ):
         Type.__init__(self)
+        assert lower_bound is None or isinstance(
+            lower_bound, Fraction
+        ), "typing not respected"
+        assert upper_bound is None or isinstance(
+            upper_bound, Fraction
+        ), "typing not respected"
         self._lower_bound = lower_bound
         self._upper_bound = upper_bound
 
     def __repr__(self) -> str:
         b = []
         if (not self.lower_bound is None) or (not self.upper_bound is None):
             b.append("[")
@@ -204,120 +225,14 @@
         return True
 
 
 BOOL = _BoolType()
 TIME = _TimeType()
 
 
-class TypeManager:
-    """Class that manages the :class:`Types <unified_planning.model.Type>` in the :class:`~unified_planning.Environment`."""
-
-    def __init__(self):
-        self._bool = BOOL
-        self._ints: Dict[Tuple[Optional[int], Optional[int]], Type] = {}
-        self._reals: Dict[Tuple[Optional[Fraction], Optional[Fraction]], Type] = {}
-        self._user_types: Dict[Tuple[str, Optional[Type]], Type] = {}
-
-    def has_type(self, type: Type) -> bool:
-        """
-        Returns `True` if the given type is already defined in this :class:`~unified_planning.Environment`.
-
-        :param type: The type searched in this `Environment`.
-        :return: `True` if the given `type` is found, `False` otherwise.
-        """
-        if type.is_bool_type():
-            return type == self._bool
-        elif type.is_int_type():
-            assert isinstance(type, _IntType)
-            return self._ints.get((type.lower_bound, type.upper_bound), None) == type
-        elif type.is_real_type():
-            assert isinstance(type, _RealType)
-            return self._reals.get((type.lower_bound, type.upper_bound), None) == type
-        elif type.is_time_type():
-            return type == TIME
-        elif type.is_user_type():
-            assert isinstance(type, _UserType)
-            return self._user_types.get((type.name, type.father), None) == type
-        else:
-            raise NotImplementedError
-
-    def BoolType(self) -> Type:
-        """Returns this `Environment's` boolean `Type`."""
-        return self._bool
-
-    def IntType(
-        self, lower_bound: Optional[int] = None, upper_bound: Optional[int] = None
-    ) -> Type:
-        """
-        Returns the `integer type` defined in this :class:`~unified_planning.Environment` with the given bounds.
-        If the `Type` already exists, it is returned, otherwise it is created and returned.
-
-        :param lower_bound: The integer used as this type's lower bound.
-        :param upper_bound: The integer used as this type's upper bound.
-        :return: The retrieved or created `Type`.
-        """
-        k = (lower_bound, upper_bound)
-        if k in self._ints:
-            return self._ints[k]
-        else:
-            it = _IntType(lower_bound, upper_bound)
-            self._ints[k] = it
-            return it
-
-    def RealType(
-        self,
-        lower_bound: Optional[Union[Fraction, int]] = None,
-        upper_bound: Optional[Union[Fraction, int]] = None,
-    ) -> Type:
-        """
-        Returns the `real type` defined in this :class:`~unified_planning.Environment` with the given bounds.
-        If the type already exists, it is returned, otherwise it is created and returned.
-
-        :param lower_bound: The Fraction or int used as this type's lower bound.
-        :param upper_bound: The Fraction or int used as this type's upper bound.
-        :return: The retrieved or created `Type`.
-        """
-        if isinstance(lower_bound, int):
-            lower_bound = Fraction(lower_bound)
-        if isinstance(upper_bound, int):
-            upper_bound = Fraction(upper_bound)
-        k = (lower_bound, upper_bound)
-        if k in self._reals:
-            return self._reals[k]
-        else:
-            rt = _RealType(lower_bound, upper_bound)
-            self._reals[k] = rt
-            return rt
-
-    def UserType(self, name: str, father: Optional[Type] = None) -> Type:
-        """
-        Returns the user type defined in this :class:`~unified_planning.Environment` with the given `name` and `father`.
-        If the type already exists, it is returned, otherwise it is created and returned.
-
-        :param name: The name of this user type.
-        :param father: The user type that must be set as the father for this type.
-        :return: The retrieved or created `Type`.
-        """
-        if (name, father) in self._user_types:
-            return self._user_types[(name, father)]
-        else:
-            if father is not None:
-                assert isinstance(father, _UserType)
-                if any(
-                    cast(_UserType, ancestor).name == name
-                    for ancestor in father.ancestors
-                ):
-                    raise UPTypeError(
-                        f"The name: {name} is already used. A UserType and one of his ancestors can not share the name."
-                    )
-            ut = _UserType(name, father)
-            self._user_types[(name, father)] = ut
-            return ut
-
-
 def domain_size(
     objects_set: "unified_planning.model.mixins.ObjectsSetMixin",
     typename: "unified_planning.model.types.Type",
 ) -> int:
     """
     Returns the domain size of the given type; the domain size is the number of values
     that an element with the given `Type` can have.
@@ -351,26 +266,26 @@
 
     :param object_set: The :class:`~unified_planning.model.AbstractProblem` instance containing the :class:`Objects <unified_planning.model.Object>`.
     :param typename: The type of which the `idx` element is returned.
     :param idx: The index of the domain item that is returned
     :return: The `idx` domain item of the given `Type` in the domain of the given `Problem` instance.
     """
     if typename.is_bool_type():
-        return objects_set.env.expression_manager.Bool(idx == 0)
+        return objects_set.environment.expression_manager.Bool(idx == 0)
     elif typename.is_user_type():
-        return objects_set.env.expression_manager.ObjectExp(
+        return objects_set.environment.expression_manager.ObjectExp(
             list(objects_set.objects(typename))[idx]
         )
     elif typename.is_int_type():
         typename = cast(_IntType, typename)
         lb = typename.lower_bound
         ub = typename.upper_bound
         if lb is None or ub is None:
             raise UPProblemDefinitionError("Parameter not groundable!")
-        return objects_set.env.expression_manager.Int(lb + idx)
+        return objects_set.environment.expression_manager.Int(lb + idx)
     else:
         raise UPProblemDefinitionError("Parameter not groundable!")
 
 
 def is_compatible_type(
     t_left: "Type",
     t_right: "Type",
@@ -382,15 +297,16 @@
     :param t_right: the type of the element that wants to be assigned to the element of type t_left.
     :return: True if the element of type t_left can be assigned to the element of type t_right; False otherwise.
     """
     if t_left == t_right:
         return True
     if t_left.is_user_type() and t_right.is_user_type():
         assert isinstance(t_left, _UserType) and isinstance(t_right, _UserType)
-        return t_right in t_left.ancestors
+        # compatible if t_right is a subclass of t_left
+        return t_left in t_right.ancestors
     if not (
         (t_left.is_int_type() and t_right.is_int_type())
         or (t_left.is_real_type() and t_right.is_real_type())
         or (t_left.is_real_type() and t_right.is_int_type())
     ):
         return False
     assert isinstance(t_left, _IntType) or isinstance(t_left, _RealType)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/variable.py` & `unified_planning-0.6.0/unified_planning/model/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 """
 This module defines the Variable class.
 A Variable has a name and a type.
 """
 
 
 from typing import List, Optional, Set
-from unified_planning.environment import Environment, get_env
+from unified_planning.environment import Environment, get_environment
 from unified_planning.model.fnode import FNode
 from unified_planning.model.operators import OperatorKind
 import unified_planning
 import unified_planning.model.walkers as walkers
 import unified_planning.model.operators as op
 
 
 class Variable:
     """Represents a variable; a `Variable` has a name and a type."""
 
     def __init__(
         self,
         name: str,
         typename: "unified_planning.model.types.Type",
-        env: Optional[Environment] = None,
+        environment: Optional[Environment] = None,
     ):
         self._name = name
         self._typename = typename
-        self._env = get_env(env)
+        self._env = get_environment(environment)
         assert self._env.type_manager.has_type(
             typename
         ), "type of variable does not belong to the same environment of the variable"
 
     def __repr__(self) -> str:
         return f"{str(self.type)} {self.name}"
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/__init__.py` & `unified_planning-0.6.0/unified_planning/model/walkers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 
 from unified_planning.model.walkers.dag import DagWalker
 from unified_planning.model.walkers.generic import handles
 from unified_planning.model.walkers.dnf import Dnf, Nnf
 from unified_planning.model.walkers.expression_quantifiers_remover import (
     ExpressionQuantifiersRemover,
 )
+from unified_planning.model.walkers.fluents_substituter import FluentsSubstituter
 from unified_planning.model.walkers.linear_checker import LinearChecker
 from unified_planning.model.walkers.operators_extractor import OperatorsExtractor
 from unified_planning.model.walkers.quantifier_simplifier import QuantifierSimplifier
 from unified_planning.model.walkers.simplifier import Simplifier
 from unified_planning.model.walkers.state_evaluator import StateEvaluator
 from unified_planning.model.walkers.substituter import Substituter
 from unified_planning.model.walkers.type_checker import TypeChecker
 from unified_planning.model.walkers.free_vars import FreeVarsExtractor
+from unified_planning.model.walkers.any import AnyChecker, AnyGetter
+from unified_planning.model.walkers.usertype_fluents_walker import UsertypeFluentsWalker
+from unified_planning.model.walkers.names_extractor import NamesExtractor
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/dag.py` & `unified_planning-0.6.0/unified_planning/model/walkers/dag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/dnf.py` & `unified_planning-0.6.0/unified_planning/model/walkers/dnf.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     Class used to transform a logic expression into the equivalent
     Negation Normal Form expression.
 
     This is done first by removing all the Implications and Equalities,
     then by pushing all the not to the leaves of the Tree representing the expression.
     """
 
-    def __init__(self, env: "unified_planning.environment.Environment"):
-        self.env = env
-        self.manager = env.expression_manager
+    def __init__(self, environment: "unified_planning.environment.Environment"):
+        self.environment = environment
+        self.manager = environment.expression_manager
 
     def get_nnf_expression(self, expression: FNode) -> FNode:
         """Function used to transform a logic expression into the equivalent
         Negational Normal Form expression.
 
         This is done first by removing all the Implications and Equalities,
         and by pushing all the not to the leaves of the Tree representing the expression.
@@ -122,20 +122,20 @@
 
     This is done first by transforming the expression into a NNF expression,
     and then every And and Or are propagated to be a unique equivalent Or of
     Ands or Atomic expressions, where 'atomic expressions' could also be a
     Not of an atomic expression.
     """
 
-    def __init__(self, env: "unified_planning.environment.Environment"):
+    def __init__(self, environment: "unified_planning.environment.Environment"):
         walkers.dag.DagWalker.__init__(self, True)
-        self.env = env
-        self.manager = env.expression_manager
-        self._nnf = Nnf(self.env)
-        self._simplifier = walkers.simplifier.Simplifier(self.env)
+        self.environment = environment
+        self.manager = environment.expression_manager
+        self._nnf = Nnf(self.environment)
+        self._simplifier = walkers.simplifier.Simplifier(self.environment)
 
     def get_dnf_expression(self, expression: FNode) -> FNode:
         """Function used to transform a logic expression into the equivalent
         Disjunctive Normal Form expression.
 
         This is done first by transforming the expression into a NNF expression,
         and then every And and Or are propagated to be a unique equivalent Or of
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py` & `unified_planning-0.6.0/unified_planning/model/walkers/expression_quantifiers_remover.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,17 @@
     This walker is used to remove all the quantifiers from an expression by substituting
     them with the semantically equivalent grounded expression; this is why this walker
     also needs an instance of the `problem` containing the `objects` (an implementation of
     `ObjectsSetMixin`) when the `remove_quantifiers` method is called, and the result can not
     be cached because the `problem` can change, and therefore the resulting expression changes.
     """
 
-    def __init__(self, env):
-        self._env = env
+    def __init__(self, environment):
+        self._env = environment
         IdentityDagWalker.__init__(self, self._env, True)
-        self._substituter = walkers.substituter.Substituter(self._env)
 
     def remove_quantifiers(
         self, expression: FNode, objects_set: "ObjectsSetMixin"
     ) -> FNode:
         """
         This method takes in input an expression that might contain quantifiers and a `problem`
         containing `objects`, and returns an equivalent expression in the given `problem`.
@@ -71,15 +70,15 @@
         # every tuple has n elements and the tuples make every possible
         # combination of 1 item for each iterable. For example:
         # product([1,2], [3,4], [5,6], [7]) =
         # (1,3,5,7) (1,3,6,7) (1,4,5,7) (1,4,6,7) (2,3,5,7) (2,3,6,7) (2,4,5,7) (2,4,6,7)
         subs_results = []
         for o in product(*possible_objects):
             subs: Dict[Expression, Expression] = dict(zip(vars, list(o)))
-            subs_results.append(self._substituter.substitute(args[0], subs))
+            subs_results.append(args[0].substitute(subs))
         return subs_results
 
     @walkers.handles(OperatorKind.EXISTS)
     def walk_exists(self, expression: FNode, args: List[FNode], **kwargs) -> FNode:
         subs_results = self._help_walk_quantifiers(expression, args)
         return self._env.expression_manager.Or(subs_results)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/free_vars.py` & `unified_planning-0.6.0/unified_planning/model/walkers/free_vars.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/generic.py` & `unified_planning-0.6.0/unified_planning/model/walkers/generic.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 
 
 class handles(object):
     """Decorator for walker functions.
     Use it by specifying the nodetypes that need to be handled by the
     given function. It is possible to use groupd (e.g., OperatorKind.RELATIONS)
     directly. ::
-      @handles(OperatorKind.NODE, ...)
-      def walk_special(...):
-         ...
+    `@handles(OperatorKind.NODE, ...)
+    def walk_special(...):
+        ...`
+
     """
 
     def __init__(self, *nodetypes):
         if len(nodetypes) == 1 and isinstance(nodetypes[0], Iterable):
             nodetypes = nodetypes[0]  # type: ignore
         self.nodetypes = list(nodetypes)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/identitydag.py` & `unified_planning-0.6.0/unified_planning/model/walkers/identitydag.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     identically.
     This could be useful when only some nodes needs to be rewritten
     but the structure of the expression has to be kept.
     """
 
     def __init__(
         self,
-        env: "unified_planning.environment.Environment",
+        environment: "unified_planning.environment.Environment",
         invalidate_memoization=False,
     ):
         walkers.dag.DagWalker.__init__(self, invalidate_memoization)
-        self.env = env
-        self.manager = env.expression_manager
+        self.environment = environment
+        self.manager = environment.expression_manager
 
     def walk_and(self, expression: FNode, args: List[FNode], **kwargs):
         return self.manager.And(args)
 
     def walk_or(self, expression: FNode, args: List[FNode], **kwargs):
         return self.manager.Or(args)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/linear_checker.py` & `unified_planning-0.6.0/unified_planning/model/walkers/linear_checker.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 import unified_planning as up
 import unified_planning.model.walkers as walkers
-from unified_planning.environment import Environment, get_env
+from unified_planning.environment import Environment, get_environment
 from unified_planning.model.walkers.dag import DagWalker
 from unified_planning.model.operators import OperatorKind
 from unified_planning.model.types import _IntType, _RealType
 from typing import List, Optional, Set, Tuple
 
 
 class LinearChecker(DagWalker):
@@ -33,30 +33,30 @@
     After the initialization, the problem given as input can not be modified
     or the `LinearChecker` behavior is undefined.
     """
 
     def __init__(
         self,
         problem: Optional["up.model.problem.Problem"] = None,
-        env: Optional["up.environment.Environment"] = None,
+        environment: Optional["up.environment.Environment"] = None,
     ):
         DagWalker.__init__(self)
         if problem is not None:
-            if env is not None:
+            if environment is not None:
                 assert (
-                    problem.env == env
+                    problem.environment == environment
                 ), "The given environemt is different from the given problem environment"
             self._static_fluents: Set[
                 "up.model.fluent.Fluent"
             ] = problem.get_static_fluents()
-            self._env = problem.env
+            self._env = problem.environment
             self._simplifier = walkers.Simplifier(self._env, problem)
         else:
             self._static_fluents = set()
-            self._env = get_env(env)
+            self._env = get_environment(environment)
             self._simplifier = self._env.simplifier
 
     def get_fluents(
         self, expression: "up.model.fnode.FNode"
     ) -> Tuple[bool, Set["up.model.fnode.FNode"], Set["up.model.fnode.FNode"]]:
         """
         Returns the tuple containing a flag saying if the expression is linear or not,
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/operators_extractor.py` & `unified_planning-0.6.0/unified_planning/model/walkers/operators_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/quantifier_simplifier.py` & `unified_planning-0.6.0/unified_planning/model/walkers/quantifier_simplifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,20 +30,20 @@
     """
     Same to the :class:`~unified_planning.model.walkers.Simplifier`, but does not expand quantifiers and solves them
     locally using the :class:`~unified_planning.model.Problem` given at construction time.
     """
 
     def __init__(
         self,
-        env: "unified_planning.environment.Environment",
+        environment: "unified_planning.environment.Environment",
         problem: "up.model.problem.Problem",
     ):
         DagWalker.__init__(self, True)
-        self._env = env
-        self.manager = env.expression_manager
+        self._env = environment
+        self.manager = environment.expression_manager
         self._problem = problem
         self._assignments: Optional[Dict["Expression", "Expression"]] = None
         self._variable_assignments: Optional[Dict["Expression", "Expression"]] = None
 
     def qsimplify(
         self,
         expression: "FNode",
@@ -171,15 +171,15 @@
         res = self._assignments.get(new_exp, None)
         if res is not None:
             (res,) = self.manager.auto_promote(res)
             assert type(res) is FNode
             return res
         else:
             raise UPProblemDefinitionError(
-                f"Value of Fluent {str(expression)} not found in {str(self._assignments)}"
+                f"Value of Fluent {str(new_exp)} not found in {str(self._assignments)}"
             )
 
     def walk_variable_exp(self, expression: "FNode", args: List["FNode"]) -> "FNode":
         assert self._variable_assignments is not None
         res = self._variable_assignments.get(expression.variable(), None)
         if res is not None:
             (res,) = self.manager.auto_promote(res)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/simplifier.py` & `unified_planning-0.6.0/unified_planning/model/walkers/simplifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from fractions import Fraction
 from collections import OrderedDict
-from typing import List, Optional, Set, Union
+from typing import Dict, List, Optional, Set, Union
 import unified_planning as up
 import unified_planning.environment
 import unified_planning.model.walkers as walkers
 from unified_planning.model.fnode import FNode
 import unified_planning.model.operators as op
 
 
@@ -28,20 +28,20 @@
 
     Important NOTE:
     After the initialization, the :class:`~unified_planning.model.Problem` given as input can not be modified
     or the `Simplifier` behavior is undefined."""
 
     def __init__(
         self,
-        env: "unified_planning.environment.Environment",
+        environment: "unified_planning.environment.Environment",
         problem: Optional["unified_planning.model.problem.Problem"] = None,
     ):
         walkers.dag.DagWalker.__init__(self)
-        self.env = env
-        self.manager = env.expression_manager
+        self.environment = environment
+        self.manager = environment.expression_manager
         if problem is not None:
             self.static_fluents = problem.get_static_fluents()
         else:
             self.static_fluents = set()
         self.problem: Optional["unified_planning.model.problem.Problem"] = problem
 
     def _number_to_fnode(self, value: Union[int, float, Fraction]) -> FNode:
@@ -175,25 +175,61 @@
         else:
             return self.manager.Implies(sl, sr)
 
     def walk_exists(self, expression: FNode, args: List[FNode]) -> FNode:
         assert len(args) == 1
         free_vars: Set[
             "up.model.variable.Variable"
-        ] = self.env.free_vars_oracle.get_free_variables(args[0])
-        vars = tuple(var for var in expression.variables() if var in free_vars)
-        if len(vars) == 0:
-            return args[0]
-        return self.manager.Exists(args[0], *vars)
+        ] = self.environment.free_vars_oracle.get_free_variables(args[0])
+        vars = set(var for var in expression.variables() if var in free_vars)
+        # Here we check if the arg is in the form:
+        # phi(l_i) and l_i == x with phi and x general formulae and l_i a variable
+        # bounded to this Exists.
+        # if it is, it can be simplified with phi(x) and l_i is removed from the free variables.
+        # this process is repeated until there are no more equalities with variables bounded to this
+        # Exists
+        new_arg, check_equality_simplification = args[0], True
+        while check_equality_simplification:
+            check_equality_simplification = False
+            if new_arg.is_and():
+                for i, and_arg in enumerate(new_arg.args):
+                    if and_arg.is_equals():
+                        variable, value = and_arg.args
+                        if (
+                            not variable.is_variable_exp()
+                            or variable.variable() not in vars
+                        ):
+                            variable, value = value, variable
+                        value_free_vars = (
+                            self.environment.free_vars_oracle.get_free_variables(
+                                args[0]
+                            )
+                        )
+                        if (
+                            variable.is_variable_exp()
+                            and variable.variable() in vars
+                            and variable not in value_free_vars
+                        ):
+                            check_equality_simplification = True
+                            new_arg = self.manager.And(
+                                *(a for j, a in enumerate(new_arg.args) if i != j)
+                            )
+                            new_arg = new_arg.substitute({variable: value})
+                            vars.remove(variable.variable())
+                            break
+        if vars:
+            return self.manager.Exists(new_arg, *vars)
+        else:
+            return new_arg
 
     def walk_forall(self, expression: FNode, args: List[FNode]) -> FNode:
         assert len(args) == 1
         free_vars: Set[
             "up.model.variable.Variable"
-        ] = self.env.free_vars_oracle.get_free_variables(args[0])
+        ] = self.environment.free_vars_oracle.get_free_variables(args[0])
         vars = tuple(var for var in expression.variables() if var in free_vars)
         if len(vars) == 0:
             return args[0]
         return self.manager.Forall(args[0], *vars)
 
     def walk_always(self, expression: FNode, args: List[FNode]) -> FNode:
         assert len(args) == 1
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/state_evaluator.py` & `unified_planning-0.6.0/unified_planning/model/walkers/state_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,28 @@
 from unified_planning.model.expression import Expression
 from unified_planning.exceptions import UPProblemDefinitionError
 from unified_planning.model.walkers.quantifier_simplifier import QuantifierSimplifier
 
 
 class StateEvaluator(QuantifierSimplifier):
     """Same to the :class:`~unified_planning.model.walkers.QuantifierSimplifier`, but takes an instance of
-    :class:`~unified_planning.model.ROState` instead of the `assignment` map."""
+    :class:`~unified_planning.model.State` instead of the `assignment` map."""
 
     def __init__(self, problem: "up.model.problem.Problem"):
-        QuantifierSimplifier.__init__(self, problem.env, problem)
+        QuantifierSimplifier.__init__(self, problem.environment, problem)
 
     def evaluate(
         self,
         expression: "FNode",
-        state: "up.model.state.ROState",
+        state: "up.model.state.State",
         _variable_assignments: Dict["Expression", "Expression"] = {},
     ) -> FNode:
         """
         Evaluates the given expression in the given `State`.
+
         :param expression: The expression that needs to be evaluated.
         :param state: The `State` where the expression needs to be evaluated.
         :param _variable_assignment: For internal use only. Parameter used to solve quantifiers.
         :return: The constant expression corresponding to the given expression evaluated in the
             given `State`.
         """
         assert self._problem is not None
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/model/walkers/type_checker.py` & `unified_planning-0.6.0/unified_planning/model/walkers/type_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 import unified_planning.model.types
 import unified_planning.environment
 import unified_planning.model.walkers as walkers
 from unified_planning.model.types import BOOL, TIME, _IntType, _RealType
 from unified_planning.model.fnode import FNode
 from unified_planning.model.operators import OperatorKind
 from unified_planning.exceptions import UPTypeError
-from typing import List, Optional
+from typing import List, Optional, cast
+import math
 
 
 class TypeChecker(walkers.dag.DagWalker):
     """Walker used to retrieve the `Type` of an expression."""
 
-    def __init__(self, env: "unified_planning.environment.Environment"):
+    def __init__(self, environment: "unified_planning.environment.Environment"):
         walkers.dag.DagWalker.__init__(self)
-        self.env = env
+        self.environment = environment
 
     def get_type(self, expression: FNode) -> "unified_planning.model.types.Type":
         """
         Returns the `Type` of the expression.
 
         :param expression: The expression of which the `Type` must be retrieved.
         :return: The expression `Type`.
@@ -68,16 +69,16 @@
     def walk_fluent_exp(
         self, expression: FNode, args: List["unified_planning.model.types.Type"]
     ) -> Optional["unified_planning.model.types.Type"]:
         assert expression.is_fluent_exp()
         f = expression.fluent()
         if len(args) != len(f.signature):
             return None
-        for (arg, param) in zip(args, f.signature):
-            if not arg.is_compatible(param.type):
+        for (param, arg) in zip(f.signature, args):
+            if not param.type.is_compatible(arg):
                 return None
         return f.type
 
     def walk_param_exp(
         self, expression: FNode, args: List["unified_planning.model.types.Type"]
     ) -> "unified_planning.model.types.Type":
         assert expression is not None
@@ -178,35 +179,40 @@
         assert len(args) == 0
         return BOOL
 
     @walkers.handles(OperatorKind.REAL_CONSTANT)
     def walk_identity_real(self, expression, args):
         assert expression is not None
         assert len(args) == 0
-        return self.env.type_manager.RealType(
+        return self.environment.type_manager.RealType(
             expression.constant_value(), expression.constant_value()
         )
 
     @walkers.handles(OperatorKind.INT_CONSTANT)
     def walk_identity_int(self, expression, args):
         assert expression is not None
         assert len(args) == 0
-        return self.env.type_manager.IntType(
+        return self.environment.type_manager.IntType(
             expression.constant_value(), expression.constant_value()
         )
 
     def walk_plus(self, expression, args):
         has_real = False
         lower = None
         upper = None
+        is_time = False
         for x in args:
-            if x is None or not (x.is_int_type() or x.is_real_type()):
+            if x == TIME:
+                is_time = True
+            elif x is None or not (x.is_int_type() or x.is_real_type()):
                 return None
             if x.is_real_type():
                 has_real = True
+        if is_time:
+            return TIME
         for x in args:
             if x.lower_bound is None:
                 lower = -float("inf")
             elif lower is None:
                 lower = x.lower_bound
             else:
                 lower += x.lower_bound
@@ -219,46 +225,51 @@
         if lower == -float("inf"):
             lower = None
         if upper == float("inf"):
             upper = None
         if has_real:
             assert lower is None or isinstance(lower, Fraction)
             assert upper is None or isinstance(upper, Fraction)
-            return self.env.type_manager.RealType(lower, upper)
+            return self.environment.type_manager.RealType(lower, upper)
         else:
             assert lower is None or isinstance(lower, int)
             assert upper is None or isinstance(upper, int)
-            return self.env.type_manager.IntType(lower, upper)
+            return self.environment.type_manager.IntType(lower, upper)
 
     def walk_minus(self, expression, args):
         assert len(args) == 2
         has_real = False
         lower = None
         upper = None
+        is_time = False
         for x in args:
-            if x is None or not (x.is_int_type() or x.is_real_type()):
+            if x == TIME:
+                is_time = True
+            elif x is None or not (x.is_int_type() or x.is_real_type()):
                 return None
             if x.is_real_type():
                 has_real = True
+        if is_time:
+            return TIME
         left = args[0]
         right = args[1]
         left_lower = -float("inf") if left.lower_bound is None else left.lower_bound
         left_upper = float("inf") if left.upper_bound is None else left.upper_bound
         right_lower = -float("inf") if right.lower_bound is None else right.lower_bound
         right_upper = float("inf") if right.upper_bound is None else right.upper_bound
         lower = left_lower - right_upper
         upper = left_upper - right_lower
         if lower == -float("inf"):
             lower = None
         if upper == float("inf"):
             upper = None
         if has_real:
-            return self.env.type_manager.RealType(lower, upper)
+            return self.environment.type_manager.RealType(lower, upper)
         else:
-            return self.env.type_manager.IntType(lower, upper)
+            return self.environment.type_manager.IntType(lower, upper)
 
     def walk_times(self, expression, args):
         has_real = False
         lower = None
         upper = None
         for x in args:
             if x is None or not (x.is_int_type() or x.is_real_type()):
@@ -270,34 +281,35 @@
             u = float("inf") if x.upper_bound is None else x.upper_bound
             if lower is None:
                 lower = l
                 upper = u
             else:
                 lower = min(lower * l, lower * u, upper * l, upper * u)
                 upper = max(lower * l, lower * u, upper * l, upper * u)
-        if lower == -float("inf"):
+        if lower == -float("inf") or (
+            lower is not None and math.isnan(cast(float, lower))
+        ):
             lower = None
-        if upper == float("inf"):
+        if upper == float("inf") or (
+            upper is not None and math.isnan(cast(float, upper))
+        ):
             upper = None
         if has_real:
-            return self.env.type_manager.RealType(lower, upper)
+            return self.environment.type_manager.RealType(lower, upper)
         else:
-            return self.env.type_manager.IntType(lower, upper)
+            return self.environment.type_manager.IntType(lower, upper)
 
     def walk_div(self, expression, args):
         assert len(args) == 2
-        has_real = False
         to_skip = False
         lower = None
         upper = None
         for x in args:
             if x is None or not (x.is_int_type() or x.is_real_type()):
                 return None
-            if x.is_real_type():
-                has_real = True
             if x.lower_bound is None and x.upper_bound is None:
                 to_skip = True
         left = args[0]
         right = args[1]
         if to_skip or right.lower_bound != right.upper_bound:
             pass
         else:
@@ -306,18 +318,19 @@
             right = right.lower_bound
             lower = min(left_lower / right, left_upper / right)
             upper = max(left_lower / right, left_upper / right)
         if lower == -float("inf"):
             lower = None
         if upper == float("inf"):
             upper = None
-        if has_real:
-            return self.env.type_manager.RealType(lower, upper)
-        else:
-            return self.env.type_manager.IntType(lower, upper)
+        if lower is not None:
+            lower = Fraction(lower)
+        if upper is not None:
+            upper = Fraction(upper)
+        return self.environment.type_manager.RealType(lower, upper)
 
     @walkers.handles(OperatorKind.LE, OperatorKind.LT)
     def walk_math_relation(self, expression, args):
         for x in args:
             if x is None or not (
                 x.is_int_type() or x.is_real_type() or x.is_time_type()
             ):
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/plans/__init__.py` & `unified_planning-0.6.0/unified_planning/plans/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,22 @@
 #
 
 from unified_planning.plans.plan import Plan, ActionInstance, PlanKind
 from unified_planning.plans.sequential_plan import SequentialPlan
 from unified_planning.plans.time_triggered_plan import TimeTriggeredPlan
 from unified_planning.plans.partial_order_plan import PartialOrderPlan
 from unified_planning.plans.contingent_plan import ContingentPlan
+from unified_planning.plans.stn_plan import STNPlanNode, STNPlan
+from unified_planning.plans.hierarchical_plan import HierarchicalPlan
 
 __all__ = [
     "Plan",
     "PlanKind",
     "ActionInstance",
     "SequentialPlan",
     "TimeTriggeredPlan",
     "PartialOrderPlan",
     "ContingentPlan",
+    "STNPlanNode",
+    "STNPlan",
+    "HierarchicalPlan",
 ]
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/plans/contingent_plan.py` & `unified_planning-0.6.0/unified_planning/plans/contingent_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def children(
         self,
     ) -> List[Tuple[Dict["up.model.FNode", "up.model.FNode"], "ContingentPlanNode"]]:
         return self._children
 
     @property
     def environment(self) -> "up.environment.Environment":
-        return self._action_instance.action.env
+        return self._action_instance.action.environment
 
     def add_child(
         self,
         observation: Dict["up.model.FNode", "up.model.FNode"],
         node: "ContingentPlanNode",
     ):
         """Adds the given `ContingentPlanNode` as a new child for the given observation."""
@@ -127,25 +127,25 @@
     """Represents a contingent plan."""
 
     def __init__(
         self,
         root_node: Optional["ContingentPlanNode"] = None,
         environment: Optional["up.Environment"] = None,
     ):
-        # if we have a specific env or we don't have any actions
+        # if we have a specific environment or we don't have any actions
         if environment is not None or root_node is None:
             plans.plan.Plan.__init__(
                 self, plans.plan.PlanKind.CONTINGENT_PLAN, environment
             )
-        # If we don't have a specific env and have at least 1 action, use the env of the first action
+        # If we don't have a specific environment and have at least 1 action, use the environment of the first action
         else:
             plans.plan.Plan.__init__(
                 self,
                 plans.plan.PlanKind.CONTINGENT_PLAN,
-                root_node.action_instance.action.env,
+                root_node.action_instance.action.environment,
             )
         self._root_node = root_node
 
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, ContingentPlan) and self.environment == self.environment:
             return self.root_node == oth.root_node
         else:
@@ -169,15 +169,15 @@
         replace_function: Callable[
             ["plans.plan.ActionInstance"], Optional["plans.plan.ActionInstance"]
         ],
     ) -> "up.plans.plan.Plan":
         if self.root_node is None:
             return ContingentPlan(None, self._environment)
         new_root = self.root_node.replace_action_instances(replace_function)
-        new_env = new_root.action_instance.action.env
+        new_env = new_root.action_instance.action.environment
         return ContingentPlan(new_root, new_env)
 
     def convert_to(
         self,
         plan_kind: "plans.plan.PlanKind",
         problem: "up.model.AbstractProblem",
     ) -> "plans.plan.Plan":
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/plans/partial_order_plan.py` & `unified_planning-0.6.0/unified_planning/plans/partial_order_plan.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,30 +35,30 @@
         environment: Optional["Environment"] = None,
         _graph: Optional[nx.DiGraph] = None,
     ):
         """
         Constructs the PartialOrderPlan using the adjacency list representation.
 
         :param adjacency_list: The Dictionary representing the adjacency list for this PartialOrderPlan.
-        :param env: The environment in which the ActionInstances in the adjacency_list are created.
-        :param _graph: The graph that is semnatically equivalent to the adjacency_list.
+        :param environment: The environment in which the ActionInstances in the adjacency_list are created.
+        :param _graph: The graph that is semantically equivalent to the adjacency_list.
             NOTE: This parameter is for internal use only and it's maintainance is not guaranteed by any means.
         :return: The created PartialOrderPlan.
         """
-        # if we have a specific env or we don't have any actions
+        # if we have a specific environment or we don't have any actions
         if environment is not None or not adjacency_list:
             plans.plan.Plan.__init__(
                 self, plans.plan.PlanKind.PARTIAL_ORDER_PLAN, environment
             )
-        # If we don't have a specific env, use the env of the first action
+        # If we don't have a specific environment, use the environment of the first action
         else:
             assert len(adjacency_list) > 0
             for ai in adjacency_list.keys():
                 plans.plan.Plan.__init__(
-                    self, plans.plan.PlanKind.PARTIAL_ORDER_PLAN, ai.action.env
+                    self, plans.plan.PlanKind.PARTIAL_ORDER_PLAN, ai.action.environment
                 )
                 break
         if _graph is not None:
             # sanity checks
             assert len(adjacency_list) == 0
             assert all(isinstance(n, ActionInstance) for n in _graph.nodes)
             assert all(
@@ -68,21 +68,21 @@
             self._graph = _graph
         else:
             for (
                 ai_k,
                 ai_v_list,
             ) in (
                 adjacency_list.items()
-            ):  # check that given env and the env in the actions is the same
-                if ai_k.action.env != self._environment:
+            ):  # check that given environment and the environment in the actions is the same
+                if ai_k.action.environment != self._environment:
                     raise UPUsageError(
                         "The environment given to the plan is not the same of the actions in the plan."
                     )
                 for ai in ai_v_list:
-                    if ai.action.env != self._environment:
+                    if ai.action.environment != self._environment:
                         raise UPUsageError(
                             "The environment given to the plan is not the same of the actions in the plan."
                         )
             self._graph = nx.convert.from_dict_of_lists(
                 adjacency_list, create_using=nx.DiGraph
             )
 
@@ -138,28 +138,31 @@
             replaced_ai = replace_function(ai)
             if replaced_ai is not None:
                 original_to_replaced_ai[ai] = replaced_ai
 
         new_adj_list: Dict[
             "plans.plan.ActionInstance", List["plans.plan.ActionInstance"]
         ] = {}
+
+        # Populate the new adjacency list with the replaced action instances
+
         for ai in self._graph.nodes:
             replaced_ai = original_to_replaced_ai.get(ai, None)
             if replaced_ai is not None:
                 replaced_ai = original_to_replaced_ai[ai]
                 replaced_neighbors = []
                 for successor in self._graph.neighbors(ai):
                     replaced_successor = original_to_replaced_ai.get(successor, None)
                     if replaced_successor is not None:
                         replaced_neighbors.append(replaced_successor)
                 new_adj_list[replaced_ai] = replaced_neighbors
 
         new_env = self._environment
         for ai in new_adj_list.keys():
-            new_env = ai.action.env
+            new_env = ai.action.environment
             break
         return up.plans.PartialOrderPlan(new_adj_list, new_env)
 
     def convert_to(
         self,
         plan_kind: "plans.plan.PlanKind",
         problem: "up.model.AbstractProblem",
@@ -205,12 +208,33 @@
             retval = self._graph.neighbors(action_instance)
         except nx.NetworkXError:
             raise UPUsageError(
                 f"The action instance {str(action_instance)} does not belong to this Partial Order Plan. \n Note that 2 Action Instances are equals if and only if they are the exact same object."
             )
         return retval
 
+    def create_graphviz_output(
+        self,
+        adjacency_list: Dict[
+            "plans.plan.ActionInstance", List["plans.plan.ActionInstance"]
+        ],
+    ) -> str:
+        graphviz_out = ""
+        graphviz_out += "digraph {\n"
+        for start, end_list in adjacency_list.items():
+            for end in end_list:
+                graphviz_out += f'\t"{start}" -> "{end}"\n'
+        graphviz_out += "}"
+        return graphviz_out
+
+    def get_graph_file(self, file_name: str) -> str:
+        adjacency_list = self.get_adjacency_list
+        graphviz_out = self.create_graphviz_output(adjacency_list)
+        with open(f"{file_name}.dot", "w") as f:
+            f.write(graphviz_out)
+        return graphviz_out
+
 
 def _semantically_equivalent_action_instances(
     action_instance_1: ActionInstance, action_instance_2: ActionInstance
 ) -> bool:
     return action_instance_1.is_semantically_equivalent(action_instance_2)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/plans/plan.py` & `unified_planning-0.6.0/unified_planning/plans/plan.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 import unified_planning as up
-from unified_planning.environment import Environment, get_env
+from unified_planning.environment import Environment, get_environment
 from unified_planning.model import AbstractProblem
-from typing import Callable, Optional, Tuple
+from abc import ABC, abstractmethod
+from typing import Callable, Optional, Tuple, Dict
 from enum import Enum, auto
 
 
 """This module defines the general `Plan` interface and the `ActionInstance` class."""
 
 
 class ActionInstance:
@@ -33,19 +34,23 @@
     """
 
     def __init__(
         self,
         action: "up.model.Action",
         params: Tuple["up.model.FNode", ...] = tuple(),
         agent: Optional["up.model.multi_agent.Agent"] = None,
+        motion_paths: Optional[
+            Dict["up.model.tamp.MotionConstraint", "up.model.tamp.Path"]
+        ] = None,
     ):
         assert len(action.parameters) == len(params)
         self._agent = agent
         self._action = action
         self._params = tuple(params)
+        self._motion_paths = motion_paths
 
     def __repr__(self) -> str:
         s = []
         if len(self._params) > 0:
             s.append("(")
             first = True
             for p in self._params:
@@ -62,14 +67,21 @@
 
     @property
     def agent(self) -> Optional["up.model.multi_agent.Agent"]:
         """Returns the `Agent` of this `ActionInstance`."""
         return self._agent
 
     @property
+    def motion_paths(
+        self,
+    ) -> Optional[Dict["up.model.tamp.MotionConstraint", "up.model.tamp.Path"]]:
+        """Returns the motion paths of this `ActionInstance`."""
+        return self._motion_paths
+
+    @property
     def action(self) -> "up.model.Action":
         """Returns the `Action` of this `ActionInstance`."""
         return self._action
 
     @property
     def actual_parameters(self) -> Tuple["up.model.FNode", ...]:
         """Returns the actual parameters used to ground the `Action` in this `ActionInstance`."""
@@ -96,49 +108,53 @@
     Enum referring to the possible kinds of `Plans`.
     """
 
     SEQUENTIAL_PLAN = auto()
     TIME_TRIGGERED_PLAN = auto()
     PARTIAL_ORDER_PLAN = auto()
     CONTINGENT_PLAN = auto()
+    STN_PLAN = auto()
+    HIERARCHICAL_PLAN = auto()
 
 
-class Plan:
+class Plan(ABC):
     """Represents a generic plan."""
 
     def __init__(
         self, kind: PlanKind, environment: Optional["Environment"] = None
     ) -> None:
         self._kind = kind
-        self._environment = get_env(environment)
+        self._environment = get_environment(environment)
 
     @property
     def environment(self) -> "Environment":
         """Return this `plan's` `Environment`."""
         return self._environment
 
     @property
     def kind(self) -> PlanKind:
         """Returns the `Plan` `kind`"""
         return self._kind
 
+    @abstractmethod
     def replace_action_instances(
         self, replace_function: Callable[[ActionInstance], Optional[ActionInstance]]
     ) -> "Plan":
         """
         This function takes a function from `ActionInstance` to `ActionInstance` and returns a new `Plan`
         that have the `ActionInstance` modified by the `replace_function` function.
 
         If the returned `ActionInstance` is `None` it means that the `ActionInstance` should not go in the resulting `Plan`.
 
         :param replace_function: The function that must be used on the `ActionInstances` that must be replaced.
         :return: The new `Plan` in which every `ActionInstance` of the original `Plan` is modified by the given `replace_function`.
         """
         raise NotImplementedError
 
+    @abstractmethod
     def convert_to(self, plan_kind: PlanKind, problem: AbstractProblem) -> "Plan":
         """
         This function takes a `PlanKind` and returns the representation of `self`
         in the given `plan_kind`. If the conversion does not make sense, raises
         an exception.
 
         :param plan_kind: The plan_kind of the returned plan.
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/plans/sequential_plan.py` & `unified_planning-0.6.0/unified_planning/plans/sequential_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,29 +28,31 @@
     """Represents a sequential plan."""
 
     def __init__(
         self,
         actions: List["plans.plan.ActionInstance"],
         environment: Optional["Environment"] = None,
     ):
-        # if we have a specific env or we don't have any actions
+        # if we have a specific environment or we don't have any actions
         if environment is not None or not actions:
             plans.plan.Plan.__init__(
                 self, plans.plan.PlanKind.SEQUENTIAL_PLAN, environment
             )
-        # If we don't have a specific env and have at least 1 action, use the env of the first action
+        # If we don't have a specific environment and have at least 1 action, use the environment of the first action
         else:
             assert len(actions) > 0
             plans.plan.Plan.__init__(
-                self, plans.plan.PlanKind.SEQUENTIAL_PLAN, actions[0].action.env
+                self, plans.plan.PlanKind.SEQUENTIAL_PLAN, actions[0].action.environment
             )
         for (
             ai
-        ) in actions:  # check that given env and the env in the actions is the same
-            if ai.action.env != self._environment:
+        ) in (
+            actions
+        ):  # check that given environment and the environment in the actions is the same
+            if ai.action.environment != self._environment:
                 raise UPUsageError(
                     "The environment given to the plan is not the same of the actions in the plan."
                 )
         self._actions = actions
 
     def __repr__(self) -> str:
         return str(self._actions)
@@ -97,15 +99,15 @@
         new_ai = []
         for ai in self._actions:
             replaced_ai = replace_function(ai)
             if replaced_ai is not None:
                 new_ai.append(replaced_ai)
         new_env = self._environment
         if len(new_ai) > 0:
-            new_env = new_ai[0].action.env
+            new_env = new_ai[0].action.environment
         return SequentialPlan(new_ai, new_env)
 
     def _to_partial_order_plan(
         self, problem: "up.model.mixins.ObjectsSetMixin"
     ) -> "up.plans.partial_order_plan.PartialOrderPlan":
         """
         Returns the `PartialOrderPlan` version of this `SequentialPlan`.
@@ -116,15 +118,15 @@
             assign a value to said `fluent`)
         - `AND` the other `ActionInstance` reads or writes on the same `grounded fluent` (reads means that one of his preconditions
             or one of his condition in a conditional effect depends on said fluent).
 
         :param problem: The `problem` for which this `SequentialPlan` is created.
         :return: A `PartialOrderPlan` compatible with the given `problem`.
         """
-        subs = walkers.Substituter(self._environment)
+        subs = self._environment.substituter
         simp = self._environment.simplifier
         eqr = walkers.ExpressionQuantifiersRemover(self._environment)
         fve = self._environment.free_vars_extractor
         # last_modifier is the mapping from a grounded fluent to the last action instance that assigned a value to
         # that fluent
         last_modifier: Dict[FNode, "plans.plan.ActionInstance"] = {}
         # all_required is the mapping from a grounded fluent to all the action instances that read the value of that
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/shortcuts.py` & `unified_planning-0.6.0/unified_planning/shortcuts.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,480 +17,539 @@
 called without the need to specify an environment or a ExpressionManager.
 """
 
 import sys
 import unified_planning as up
 import unified_planning.model.types
 import unified_planning.model.multi_agent
-from unified_planning.environment import get_env
+from unified_planning.environment import get_environment
 from unified_planning.model import *
+from unified_planning.model.tamp import *
 from unified_planning.engines import (
     Engine,
     CompilationKind,
     OptimalityGuarantee,
     OperationMode,
 )
 from unified_planning.plans import PlanKind
-from typing import IO, Any, Iterable, List, Union, Dict, Tuple, Optional
+from typing import IO, Any, Iterable, Union, Dict, Optional, Sequence
 from fractions import Fraction
 
 
 def And(*args: Union[BoolExpression, Iterable[BoolExpression]]) -> FNode:
     """
-    Returns a conjunction of terms.
-    This function has polymorphic n-arguments:
-        - `And(a,b,c)`
-        - `And([a,b,c])`
-    Restriction: Arguments must be `boolean`.
-
-    :param *args: Either an `Iterable` of `boolean expressions`, like `[a, b, c]`, or an unpacked version
-    of it, like `a, b, c`.
-    :return: The `AND` expression created.
+    | Returns a conjunction of terms.
+    | This function has polymorphic n-arguments:
+
+        * ``And(a,b,c)``
+        * ``And([a,b,c])``
+
+    | Restriction: Arguments must be ``boolean``.
+
+    :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+        of it, like ``a, b, c``.
+    :return: The ``AND`` expression created.
     """
-    return get_env().expression_manager.And(*args)
+    return get_environment().expression_manager.And(*args)
 
 
 def Or(*args: Union[BoolExpression, Iterable[BoolExpression]]) -> FNode:
     """
-    Returns an disjunction of terms.
-    This function has polymorphic n-arguments:
-        - `Or(a,b,c)`
-        - `Or([a,b,c])`
-    Restriction: Arguments must be `boolean`
-
-    :param *args: Either an `Iterable` of `boolean expressions`, like `[a, b, c]`, or an unpacked version
-    of it, like `a, b, c`.
-    :return: The `OR` expression created.
+    | Returns an disjunction of terms.
+    | This function has polymorphic n-arguments:
+
+        * ``Or(a,b,c)``
+        * ``Or([a,b,c])``
+
+    | Restriction: Arguments must be ``boolean``
+
+    :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+        of it, like ``a, b, c``.
+    :return: The ``OR`` expression created.
     """
-    return get_env().expression_manager.Or(*args)
+    return get_environment().expression_manager.Or(*args)
 
 
 def XOr(*args: Union[BoolExpression, Iterable[BoolExpression]]) -> FNode:
     """
-    Returns an exclusive disjunction of terms in CNF form.
-    This function has polimorphic n-arguments:
-        - XOr(a,b,c)
-        - XOr([a,b,c])
-    Restriction: Arguments must be boolean
+    | Returns an exclusive disjunction of terms in CNF form.
+    | This function has polimorphic n-arguments:
 
-    :param *args: Either an `Iterable` of `boolean expressions`, like `[a, b, c]`, or an unpacked version
-    of it, like `a, b, c`.
+        * XOr(a,b,c)
+        * XOr([a,b,c])
+
+    | Restriction: Arguments must be boolean
+
+    :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+        of it, like ``a, b, c``.
     :return: The exclusive disjunction in CNF form.
     """
-    return get_env().expression_manager.XOr(*args)
+    return get_environment().expression_manager.XOr(*args)
 
 
 def Not(expression: BoolExpression) -> FNode:
     """
     Creates an expression of the form:
-        `not expression`
-    Restriction: `expression` must be of `boolean type`
+        ``not expression``
+
+    Restriction: ``expression`` must be of ``boolean type``
 
-    :param expression: The `boolean` expression of which the negation must be created.
-    :return: The created `NOT` expression.
+    :param expression: The ``boolean`` expression of which the negation must be created.
+    :return: The created ``Not`` expression.
     """
-    return get_env().expression_manager.Not(expression)
+    return get_environment().expression_manager.Not(expression)
 
 
 def Implies(left: BoolExpression, right: BoolExpression) -> FNode:
     """
     Creates an expression of the form:
-        `left -> right`
-    Restriction: `Left` and `Right` must be of `boolean type`
+        ``left -> right``
 
-    :param left: The `boolean` expression acting as the premise of the `Implies`.
-    :param right: The `boolean` expression acting as the implied part of the `Implies`.
-    :return: The created `Implication`.
+    Restriction: ``Left`` and ``Right`` must be of ``boolean type``
+
+    :param left: The ``boolean`` expression acting as the premise of the ``Implies``.
+    :param right: The ``boolean`` expression acting as the implied part of the ``Implies``.
+    :return: The created ``Implication``.
     """
-    return get_env().expression_manager.Implies(left, right)
+    return get_environment().expression_manager.Implies(left, right)
 
 
 def Iff(left: BoolExpression, right: BoolExpression) -> FNode:
     """
     Creates an expression of the form:
-        `left <-> right`
-    Semantically, The expression is `True` only if `left` and `right` have the same value.
-    Restriction: `Left` and `Right` must be of `boolean type`
-
-    :param left: The `left` member of the `Iff expression`.
-    :param right: The `right` member of the `Iff expression`.
-    :return: The created `Iff` expression.
+        ``left <-> right``
+
+    Semantically, The expression is ``True`` only if ``left`` and ``right`` have the same value.
+    Restriction: ``Left`` and ``Right`` must be of ``boolean type``
+
+    :param left: The ``left`` member of the ``Iff expression``.
+    :param right: The ``right`` member of the ``Iff expression``.
+    :return: The created ``Iff`` expression.
     """
-    return get_env().expression_manager.Iff(left, right)
+    return get_environment().expression_manager.Iff(left, right)
 
 
 def Exists(
     expression: BoolExpression, *vars: "unified_planning.model.Variable"
 ) -> FNode:
     """
     Creates an expression of the form:
-        `Exists (var[0]... var[n]) | expression`
-    Restriction: expression must be of `boolean type` and
-                vars must be of `Variable` type
-
-    :param expression: The main expression of the `existential`. The expression should contain
-        the given `variables`.
-    :param *vars: All the `Variables` appearing in the `existential` expression.
-    :return: The created `Existential` expression.
+        ``Exists (var[0]... var[n]) | expression``
+
+    Restriction: expression must be of ``boolean type`` and
+    vars must be of ``Variable`` type
+
+    :param expression: The main expression of the ``existential``. The expression should contain
+        the given ``variables``.
+    :param \*vars: All the ``Variables`` appearing in the ``existential`` expression.
+    :return: The created ``Existential`` expression.
     """
-    return get_env().expression_manager.Exists(expression, *vars)
+    return get_environment().expression_manager.Exists(expression, *vars)
 
 
 def Forall(
     expression: BoolExpression, *vars: "unified_planning.model.Variable"
 ) -> FNode:
     """Creates an expression of the form:
-        `Forall (var[0]... var[n]) | expression`
-    Restriction: expression must be of `boolean type` and
-                vars must be of `Variable` type
-
-    :param expression: The main expression of the `universal` quantifier. The expression should contain
-        the given `variables`.
-    :param *vars: All the `Variables` appearing in the `universal` expression.
-    :return: The created `Forall` expression.
+        ``Forall (var[0]... var[n]) | expression``
+
+    Restriction: expression must be of ``boolean type`` and
+                vars must be of ``Variable`` type
+
+    :param expression: The main expression of the ``universal`` quantifier. The expression should contain
+        the given ``variables``.
+    :param \*vars: All the ``Variables`` appearing in the ``universal`` expression.
+    :return: The created ``Forall`` expression.
     """
-    return get_env().expression_manager.Forall(expression, *vars)
+    return get_environment().expression_manager.Forall(expression, *vars)
 
 
 def FluentExp(
-    fluent: "unified_planning.model.Fluent", params: Iterable[Expression] = tuple()
+    fluent: "unified_planning.model.Fluent", params: Sequence[Expression] = tuple()
 ) -> FNode:
     """
-    Creates an expression for the given `fluent` and `parameters`.
-    Restriction: `parameters type` must be compatible with the `Fluent` :func:`signature <unified_planning.model.Fluent.signature>`
+    | Creates an expression for the given ``fluent`` and ``parameters``.
+    | Restriction: ``parameters type`` must be compatible with the ``Fluent`` :func:``signature <unified_planning.model.Fluent.signature>``
 
-    :param fluent: The `Fluent` that will be set as the `payload` of this expression.
-    :param params: The Iterable of expressions acting as `parameters` for this `Fluent`; mainly the parameters will
-        be :class:`Objects <unified_planning.model.Object>` (when the `FluentExp` is grounded) or :func:`Action parameters <unified_planning.model.Action.parameters>` (when the `FluentExp` is lifted).
-    :return: The created `Fluent` Expression.
+    :param fluent: The ``Fluent`` that will be set as the ``payload`` of this expression.
+    :param params: The Iterable of expressions acting as ``parameters`` for this ``Fluent``; mainly the parameters will
+        be :class:``Objects <unified_planning.model.Object>`` (when the ``FluentExp`` is grounded) or :func:``Action parameters <unified_planning.model.Action.parameters>`` (when the ``FluentExp`` is lifted).
+    :return: The created ``Fluent`` Expression.
     """
-    return get_env().expression_manager.FluentExp(fluent, params)
+    return get_environment().expression_manager.FluentExp(fluent, params)
 
 
 def Always(expression: BoolExpression) -> FNode:
-    """Creates an expression of the form:
-        `Always(a)`
-    Restriction: expression must be of `boolean type` and with only one arg.
+    """
+    Creates an expression of the form:
+        ``Always(a)``
+
+    Restriction: expression must be of ``boolean type`` and with only one arg.
 
-    :param expression: The `boolean` expression of the trajectory constraints.
-    :return: The created `Always` expression.
+    :param expression: The ``boolean`` expression of the trajectory constraints.
+    :return: The created ``Always`` expression.
     """
-    return get_env().expression_manager.Always(expression)
+    return get_environment().expression_manager.Always(expression)
 
 
 def Sometime(expression: BoolExpression) -> FNode:
-    """Creates an expression of the form:
-        `Sometime(a)`
-    Restriction: expression must be of `boolean type` and with only one arg.
+    """
+    Creates an expression of the form:
+        ``Sometime(a)``
+
+    Restriction: expression must be of ``boolean type`` and with only one arg.
 
-    :param expression: The `boolean` expression of the trajectory constraints.
-    :return: The created `Sometime` expression.
+    :param expression: The ``boolean`` expression of the trajectory constraints.
+    :return: The created ``Sometime`` expression.
     """
-    return get_env().expression_manager.Sometime(expression)
+    return get_environment().expression_manager.Sometime(expression)
 
 
 def SometimeBefore(*expression: BoolExpression) -> FNode:
-    """Creates an expression of the form:
-        `Sometime-Before(a, b)`
-    Restriction: expression must be of `boolean type` and with only one args
+    """
+    Creates an expression of the form:
+        ``Sometime-Before(a, b)``
+
+    Restriction: expression must be of ``boolean type`` and with only one args
 
-    :param expression: The `boolean` expression of the trajectory constraints.
-    :return: The created `Sometime` expression.
+    :param expression: The ``boolean`` expression of the trajectory constraints.
+    :return: The created ``Sometime`` expression.
     """
-    return get_env().expression_manager.SometimeBefore(*expression)
+    return get_environment().expression_manager.SometimeBefore(*expression)
 
 
 def SometimeAfter(*expression: BoolExpression) -> FNode:
-    """Creates an expression of the form:
-        `Sometime-After(a, b)`
-    Restriction: expression must be of `boolean type` and with only two arg.
+    """
+    Creates an expression of the form:
+        ``Sometime-After(a, b)``
 
-    :param expression: The `boolean` expression of the trajectory constraints.
-    :return: The created `Sometime-After(a, b)` expression.
+    Restriction: expression must be of ``boolean type`` and with only two arg.
+
+    :param expression: The ``boolean`` expression of the trajectory constraints.
+    :return: The created ``Sometime-After(a, b)`` expression.
     """
-    return get_env().expression_manager.SometimeAfter(*expression)
+    return get_environment().expression_manager.SometimeAfter(*expression)
 
 
 def AtMostOnce(expression: BoolExpression) -> FNode:
-    """Creates an expression of the form:
-        `At-Most-Once(a, b)`
-    Restriction: expression must be of `boolean type` and with only two arg.
+    """
+    Creates an expression of the form:
+        ``At-Most-Once(a, b)``
+
+    Restriction: expression must be of ``boolean type`` and with only two arg.
 
-    :param expression: The `boolean` expression of the trajectory constraints.
-    :return: The created `At-Most-Once(a, b)` expression.
+    :param expression: The ``boolean`` expression of the trajectory constraints.
+    :return: The created ``At-Most-Once(a, b)`` expression.
     """
-    return get_env().expression_manager.AtMostOnce(expression)
+    return get_environment().expression_manager.AtMostOnce(expression)
 
 
 def ParameterExp(param: "unified_planning.model.Parameter") -> FNode:
     """
     Returns an expression for the given :func:`Action parameter <unified_planning.model.Action.parameters>`.
 
-    :param param: The `Parameter` that must be promoted to `FNode`.
-    :return: The `FNode` containing the given `param` as his payload.
+    :param param: The ``Parameter`` that must be promoted to ``FNode``.
+    :return: The ``FNode`` containing the given ``param`` as his payload.
     """
-    return get_env().expression_manager.ParameterExp(param)
+    return get_environment().expression_manager.ParameterExp(param)
 
 
 def VariableExp(var: "unified_planning.model.Variable") -> FNode:
     """
-    Returns an expression for the given `Variable`.
+    Returns an expression for the given ``Variable``.
 
-    :param var: The `Variable` that must be promoted to `FNode`.
-    :return: The `FNode` containing the given `variable` as his payload.
+    :param var: The ``Variable`` that must be promoted to ``FNode``.
+    :return: The ``FNode`` containing the given ``variable`` as his payload.
     """
-    return get_env().expression_manager.VariableExp(var)
+    return get_environment().expression_manager.VariableExp(var)
 
 
 def ObjectExp(obj: "unified_planning.model.Object") -> FNode:
     """
     Returns an expression for the given object.
 
-    :param obj: The `Object` that must be promoted to `FNode`.
-    :return: The `FNode` containing the given object as his payload.
+    :param obj: The ``Object`` that must be promoted to ``FNode``.
+    :return: The ``FNode`` containing the given object as his payload.
     """
-    return get_env().expression_manager.ObjectExp(obj)
+    return get_environment().expression_manager.ObjectExp(obj)
 
 
 def TimingExp(timing: "up.model.timing.Timing") -> "up.model.fnode.FNode":
     """
-    Returns an expression for the given `Timing`.
+    Returns an expression for the given ``Timing``.
 
-    :param timing: The `Timing` that must be promoted to `FNode`.
-    :return: The `FNode` containing the given `timing` as his payload.
+    :param timing: The ``Timing`` that must be promoted to ``FNode``.
+    :return: The ``FNode`` containing the given ``timing`` as his payload.
     """
-    return get_env().expression_manager.TimingExp(timing)
+    return get_environment().expression_manager.TimingExp(timing)
 
 
 def TRUE() -> FNode:
-    """Return the boolean constant `True`."""
-    return get_env().expression_manager.TRUE()
+    """Return the boolean constant ``True``."""
+    return get_environment().expression_manager.TRUE()
 
 
 def FALSE() -> FNode:
-    """Return the boolean constant `False`."""
-    return get_env().expression_manager.FALSE()
+    """Return the boolean constant ``False``."""
+    return get_environment().expression_manager.FALSE()
 
 
 def Bool(value: bool) -> FNode:
     """
     Return a boolean constant.
 
-    :param value: The boolean value that must be promoted to `FNode`.
-    :return: The `FNode` containing the given `value` as his payload.
+    :param value: The boolean value that must be promoted to ``FNode``.
+    :return: The ``FNode`` containing the given ``value`` as his payload.
     """
-    return get_env().expression_manager.Bool(value)
+    return get_environment().expression_manager.Bool(value)
 
 
 def Int(value: int) -> FNode:
     """
-    Return an `int` constant.
+    Return an ``int`` constant.
 
-    :param value: The integer that must be promoted to `FNode`.
-    :return: The `FNode` containing the given `integer` as his payload.
+    :param value: The integer that must be promoted to ``FNode``.
+    :return: The ``FNode`` containing the given ``integer`` as his payload.
     """
-    return get_env().expression_manager.Int(value)
+    return get_environment().expression_manager.Int(value)
 
 
 def Real(value: Fraction) -> FNode:
     """
-    Return a `real` constant.
+    Return a ``real`` constant.
 
-    :param value: The `Fraction` that must be promoted to `FNode`.
-    :return: The `FNode` containing the given `value` as his payload.
+    :param value: The ``Fraction`` that must be promoted to ``FNode``.
+    :return: The ``FNode`` containing the given ``value`` as his payload.
     """
-    return get_env().expression_manager.Real(value)
+    return get_environment().expression_manager.Real(value)
 
 
 def Plus(*args: Union[Expression, Iterable[Expression]]) -> FNode:
     """
     Creates an expression of the form:
-    `args[0] + ... + args[n]`
+        ``args[0] + ... + args[n]``
 
-    :param *args: Either an `Iterable` of expressions, like `[a, b, 3]`, or an unpacked version
-        of it, like `a, b, 3`.
-    :return: The `PLUS` expression created. (like `a + b + 3`)
+    :param \*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
+        of it, like ``a, b, 3``.
+    :return: The ``PLUS`` expression created. (like ``a + b + 3``)
     """
-    return get_env().expression_manager.Plus(*args)
+    return get_environment().expression_manager.Plus(*args)
 
 
 def Minus(left: Expression, right: Expression) -> FNode:
     """
-    Creates an expression of the form: `left - right`.
+    Creates an expression of the form:
+        ``left - right``
 
-    :param left: The `Minus minuend`.
-    :param right: The `Minus subtrahend`.
-    :return: The created `Minus` expression.
+    :param left: The ``Minus minuend``.
+    :param right: The ``Minus subtrahend``.
+    :return: The created ``Minus`` expression.
     """
-    return get_env().expression_manager.Minus(left, right)
+    return get_environment().expression_manager.Minus(left, right)
 
 
 def Times(*args: Union[Expression, Iterable[Expression]]) -> FNode:
     """
     Creates an expression of the form:
-    `args[0] * ... * args[n]`
+        ``args[0] * ... * args[n]``
 
-    :param *args: Either an `Iterable` of expressions, like `[a, b, 3]`, or an unpacked version
-        of it, like `a, b, 3`.
-    :return: The `TIMES` expression created. (like `a * b * 3`)
+    :param \*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
+        of it, like ``a, b, 3``.
+    :return: The ``TIMES`` expression created. (like ``a * b * 3``)
     """
-    return get_env().expression_manager.Times(*args)
+    return get_environment().expression_manager.Times(*args)
 
 
 def Div(left: Expression, right: Expression) -> FNode:
     """
-    Creates an expression of the form: `left / right`.
+    Creates an expression of the form:
+        ``left / right``.
 
-    :param left: The `Div dividend`.
-    :param right: The `Div divisor`.
-    :return: The created `DIV` expression.
+    :param left: The ``Div dividend``.
+    :param right: The ``Div divisor``.
+    :return: The created ``DIV`` expression.
     """
-    return get_env().expression_manager.Div(left, right)
+    return get_environment().expression_manager.Div(left, right)
 
 
 def LE(left: Expression, right: Expression) -> FNode:
     """
-    Creates an expression of the form: `left <= right`.
+    Creates an expression of the form:
+        ``left <= right``.
 
-    :param left: The left side of the `<=`.
-    :param right: The right side of the `<=`.
-    :return: The created `LE` expression.
+    :param left: The left side of the ``<=``.
+    :param right: The right side of the ``<=``.
+    :return: The created ``LE`` expression.
     """
-    return get_env().expression_manager.LE(left, right)
+    return get_environment().expression_manager.LE(left, right)
 
 
 def GE(left: Expression, right: Expression) -> FNode:
     """
-    Creates an expression of the form: `left >= right`.
+    Creates an expression of the form:
+        ``left >= right``.
 
-    :param left: The left side of the `>=`.
-    :param right: The right side of the `>=`.
-    :return: The created `GE` expression.
+    :param left: The left side of the ``>=``.
+    :param right: The right side of the ``>=``.
+    :return: The created ``GE`` expression.
     """
-    return get_env().expression_manager.GE(left, right)
+    return get_environment().expression_manager.GE(left, right)
 
 
 def LT(left: Expression, right: Expression) -> FNode:
     """
-    Creates an expression of the form: `left < right`.
+    Creates an expression of the form:
+        ``left < right``.
 
-    :param left: The left side of the `<`.
-    :param right: The right side of the `<`.
-    :return: The created `LT` expression.
+    :param left: The left side of the ``<``.
+    :param right: The right side of the ``<``.
+    :return: The created ``LT`` expression.
     """
-    return get_env().expression_manager.LT(left, right)
+    return get_environment().expression_manager.LT(left, right)
 
 
 def GT(left: Expression, right: Expression) -> FNode:
     """
-    Creates an expression of the form: `left > right`.
+    Creates an expression of the form:
+        ``left > right``.
 
-    :param left: The left side of the `>`.
-    :param right: The right side of the `>`.
-    :return: The created `GT` expression.
+    :param left: The left side of the ``>``.
+    :param right: The right side of the ``>``.
+    :return: The created ``GT`` expression.
     """
-    return get_env().expression_manager.GT(left, right)
+    return get_environment().expression_manager.GT(left, right)
 
 
 def Equals(left: Expression, right: Expression) -> FNode:
     """
-    Creates an expression of the form: `left == right`.
+    Creates an expression of the form:
+        ``left == right``.
 
-    NOTE: Is not valid for boolean expression, for those use `Iff`.
+    NOTE: Is not valid for boolean expression, for those use ``Iff``.
 
-    :param left: The left side of the `==`.
-    :param right: The right side of the `==`.
-    :return: The created `Equals` expression.
+    :param left: The left side of the ``==``.
+    :param right: The right side of the ``==``.
+    :return: The created ``Equals`` expression.
     """
-    return get_env().expression_manager.Equals(left, right)
+    return get_environment().expression_manager.Equals(left, right)
 
 
 def Dot(
     agent: "unified_planning.model.multi_agent.Agent",
     fluent_exp: Union[FNode, "unified_planning.model.Fluent"],
 ) -> FNode:
     """
-    Creates an expression for the given `agent` and `fluent_exp`.
-    Restriction: agent must be of `agent type` and fluent_exp must be of `fluentExp type`
+    Creates an expression for the given ``agent`` and ``fluent_exp``.
+    Restriction: agent must be of ``agent type`` and fluent_exp must be of ``fluentExp type``
 
-    :param agent: The `Agent` that will be set as the `payload` of this expression.
-    :param fluent_exp: The `Fluent_exp` that will be set as the `args` of this expression.
-    :return: The created `Dot` Expression.
+    :param agent: The ``Agent`` that will be set as the ``payload`` of this expression.
+    :param fluent_exp: The ``Fluent_exp`` that will be set as the ``args`` of this expression.
+    :return: The created ``Dot`` Expression.
     """
-    return get_env().expression_manager.Dot(agent, fluent_exp)
+    return get_environment().expression_manager.Dot(agent, fluent_exp)
 
 
 def BoolType() -> unified_planning.model.types.Type:
     """Returns the global environment's boolean type."""
-    return get_env().type_manager.BoolType()
+    return get_environment().type_manager.BoolType()
 
 
 def IntType(
     lower_bound: Optional[int] = None, upper_bound: Optional[int] = None
 ) -> unified_planning.model.types.Type:
     """
     Returns the `integer` type defined in the global environment with the given `bounds`.
     If the type already exists, it is returned, otherwise it is created and returned.
 
     :param lower_bound: The integer used as this type's `lower bound`.
     :param upper_bound: The integer used as this type's `upper bound`.
     :return: The retrieved or created type.
     """
-    return get_env().type_manager.IntType(lower_bound, upper_bound)
+    return get_environment().type_manager.IntType(lower_bound, upper_bound)
 
 
 def RealType(
     lower_bound: Optional[Union[Fraction, int]] = None,
     upper_bound: Optional[Union[Fraction, int]] = None,
 ) -> unified_planning.model.types.Type:
     """
     Returns the `real` type defined in the global environment with the given `bounds`.
     If the type already exists, it is returned, otherwise it is created and returned.
 
     :param lower_bound: The `Fraction` used as this type's `lower bound`.
     :param upper_bound: The `Fraction` used as this type's `upper bound`.
     :return: The retrieved or created `type`.
     """
-    return get_env().type_manager.RealType(lower_bound, upper_bound)
+    return get_environment().type_manager.RealType(lower_bound, upper_bound)
 
 
 def UserType(
     name: str, father: Optional[Type] = None
 ) -> unified_planning.model.types.Type:
     """
     Returns the user type defined in the global environment with the given `name` and `father`.
     If the type already exists, it is returned, otherwise it is created and returned.
 
     :param name: The name of this `user type`.
     :param father: The user type that must be set as the `father` for the created `type`.
     :return:  The retrieved or created `type`.
     """
-    return get_env().type_manager.UserType(name, father)
+    return get_environment().type_manager.UserType(name, father)
+
+
+def MovableType(
+    name: str, father: Optional[Type] = None
+) -> unified_planning.model.types.Type:
+    """
+    Returns the movable type defined in this :class:`~unified_planning.Environment`
+    with the given `name` and `father`.
+    If the type already exists, it is returned, otherwise it is created and returned.
+
+    :param name: The name of this movable type.
+    :param father: The movable type that must be set as the father for this type.
+    :return: The retrieved or created `Type`.
+    """
+    return get_environment().type_manager.MovableType(name, father)
+
+
+def ConfigurationType(
+    name: str, occupancy_map: OccupancyMap, size: int
+) -> unified_planning.model.types.Type:
+    """
+    Returns the configuration type defined in this :class:`~unified_planning.Environment`
+    with the given `name`, `occupancy_map` and `size`.
+    If the type already exists, it is returned, otherwise it is created and returned.
+
+    :param name: The name of this configuration type.
+    :param occupancy_map: The occupancy map.
+    :param size: The size of the configuration.
+    :return: The retrieved or created `Type`.
+    """
+    return get_environment().type_manager.ConfigurationType(name, occupancy_map, size)
 
 
 def OneshotPlanner(
     *,
     name: Optional[str] = None,
-    names: Optional[List[str]] = None,
-    params: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
+    names: Optional[Sequence[str]] = None,
+    params: Optional[Union[Dict[str, Any], Sequence[Dict[str, Any]]]] = None,
     problem_kind: ProblemKind = ProblemKind(),
     optimality_guarantee: Optional[Union["up.engines.OptimalityGuarantee", str]] = None,
 ) -> Engine:
     """
     Returns a oneshot planner. There are three ways to call this method:
-    - using 'name' (the name of a specific planner) and 'params' (planner dependent options).
-      e.g. OneshotPlanner(name='tamer', params={'heuristic': 'hadd'})
-    - using 'names' (list of specific planners name) and 'params' (list of
-      planner dependent options) to get a Parallel engine.
-      e.g. OneshotPlanner(names=['tamer', 'tamer'],
-                          params=[{'heuristic': 'hadd'}, {'heuristic': 'hmax'}])
-    - using 'problem_kind' and 'optimality_guarantee'.
-          e.g. OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)
+
+    *   | using ``name`` (the name of a specific planner) and ``params`` (planner dependent options).
+        | e.g. ``OneshotPlanner(name='tamer', params={'heuristic': 'hadd'})``
+    *   | using ``names`` (list of specific planners name) and ``params`` (list of planner dependent options) to get a ``Parallel`` engine.
+        | e.g. ``OneshotPlanner(names=['tamer', 'tamer'], params=[{'heuristic': 'hadd'}, {'heuristic': 'hmax'}])``
+    *   | using ``problem_kind`` and ``optimality_guarantee``.
+        | e.g. ``OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
     """
-    return get_env().factory.OneshotPlanner(
+    return get_environment().factory.OneshotPlanner(
         name=name,
         names=names,
         params=params,
         problem_kind=problem_kind,
         optimality_guarantee=optimality_guarantee,
     )
 
@@ -500,166 +559,192 @@
     name: Optional[str] = None,
     params: Optional[Dict[str, str]] = None,
     problem_kind: ProblemKind = ProblemKind(),
     anytime_guarantee: Optional[Union["up.engines.AnytimeGuarantee", str]] = None,
 ) -> Engine:
     """
     Returns a anytime planner. There are two ways to call this method:
-    - using 'name' (the name of a specific planner) and 'params' (planner dependent options).
-      e.g. AnytimePlanner(name='tamer', params={'heuristic': 'hadd'})
-    - using 'problem_kind' and 'anytime_guarantee'.
-      e.g. AnytimePlanner(problem_kind=problem.kind, anytime_guarantee=INCREASING_QUALITY)
-
-    An AnytimePlanner is a planner that returns an iterator of solutions.
-    Depending on the given anytime_guarantee parameter, every plan being generated is:
-    - strictly better in terms of quality than the previous one (INCREASING_QUALITY);
-    - optimal (OPTIMAL_PLANS);
-    - just a different plan, with no specific guarantee (None).
+
+    *   | using ``name`` (the name of a specific planner) and ``params`` (planner dependent options).
+        | e.g. ``AnytimePlanner(name='tamer', params={'heuristic': 'hadd'})``
+    *   | using ``problem_kind`` and ``anytime_guarantee``.
+        | e.g. ``AnytimePlanner(problem_kind=problem.kind, anytime_guarantee=INCREASING_QUALITY)``
+
+    An ``AnytimePlanner`` is a planner that returns an ``Iterator`` of solutions.
+    Depending on the given ``anytime_guarantee`` parameter, every plan being generated is:
+
+    * strictly better in terms of quality than the previous one (``INCREASING_QUALITY``);
+    * optimal (``OPTIMAL_PLANS``);
+    * just a different plan, with no specific guarantee (``None``).
 
     It raises an exception if the problem has no optimality metrics and anytime_guarantee
-    is equal to INCREASING_QUALITY or OPTIMAL_PLAN.
+    is equal to ``INCREASING_QUALITY`` or ``OPTIMAL_PLAN``.
     """
-    return get_env().factory.AnytimePlanner(
+    return get_environment().factory.AnytimePlanner(
         name=name,
         params=params,
         problem_kind=problem_kind,
         anytime_guarantee=anytime_guarantee,
     )
 
 
 def PlanValidator(
     *,
     name: Optional[str] = None,
-    names: Optional[List[str]] = None,
-    params: Optional[Union[Dict[str, str], List[Dict[str, str]]]] = None,
+    names: Optional[Sequence[str]] = None,
+    params: Optional[Union[Dict[str, str], Sequence[Dict[str, str]]]] = None,
     problem_kind: ProblemKind = ProblemKind(),
     plan_kind: Optional[Union["up.plans.PlanKind", str]] = None,
 ) -> Engine:
     """
     Returns a plan validator. There are three ways to call this method:
-    - using 'name' (the name of a specific plan validator) and 'params'
-      (plan validator dependent options).
-      e.g. PlanValidator(name='tamer', params={'opt': 'val'})
-    - using 'names' (list of specific plan validators name) and 'params' (list of
-      plan validators dependent options) to get a Parallel engine.
-      e.g. PlanValidator(names=['tamer', 'tamer'],
-                         params=[{'opt1': 'val1'}, {'opt2': 'val2'}])
-    - using 'problem_kind' and 'plan_kind' parameters.
-      e.g. PlanValidator(problem_kind=problem.kind, plan_kind=plan.kind)
+
+    *   | using ``name`` (the name of a specific plan validator) and ``params`` (plan validator dependent options).
+        | e.g. ``PlanValidator(name='tamer', params={'opt': 'val'})``
+    *   | using ``names`` (list of specific plan validators name) and ``params`` (list of plan validators dependent options) to get a ``Parallel`` engine.
+        | e.g. ``PlanValidator(names=['tamer', 'tamer'], params=[{'opt1': 'val1'}, {'opt2': 'val2'}])``
+    *   | using ``problem_kind`` and ``plan_kind`` parameters.
+        | e.g. ``PlanValidator(problem_kind=problem.kind, plan_kind=plan.kind)``
     """
-    return get_env().factory.PlanValidator(
+    return get_environment().factory.PlanValidator(
         name=name,
         names=names,
         params=params,
         problem_kind=problem_kind,
         plan_kind=plan_kind,
     )
 
 
 def Compiler(
     *,
     name: Optional[str] = None,
-    names: Optional[List[str]] = None,
-    params: Optional[Union[Dict[str, str], List[Dict[str, str]]]] = None,
+    names: Optional[Sequence[str]] = None,
+    params: Optional[Union[Dict[str, str], Sequence[Dict[str, str]]]] = None,
     problem_kind: ProblemKind = ProblemKind(),
     compilation_kind: Optional[Union["up.engines.CompilationKind", str]] = None,
-    compilation_kinds: Optional[List[Union["up.engines.CompilationKind", str]]] = None,
+    compilation_kinds: Optional[
+        Sequence[Union["up.engines.CompilationKind", str]]
+    ] = None,
 ) -> "up.engines.engine.Engine":
     """
-    Returns a Compiler or a pipeline of Compilers.
+    Returns a compiler or a pipeline of compilers.
+
+    To get a compiler there are two ways to call this method:
+
+    *   | using ``name`` (the name of a specific compiler) and ``params`` (compiler dependent options).
+        | e.g. ``Compiler(name='tamer', params={'opt': 'val'})``
+    *   | using ``problem_kind`` and ``compilation_kind`` parameters.
+        | e.g. ``Compiler(problem_kind=problem.kind, compilation_kind=GROUNDING)``
+
+    To get a pipeline of compilers there are two ways to call this method:
 
-    To get a Compiler there are two ways to call this method:
-    - using 'name' (the name of a specific compiler) and 'params'
-      (compiler dependent options).
-      e.g. Compiler(name='tamer', params={'opt': 'val'})
-    - using 'problem_kind' and 'compilation_kind' parameters.
-      e.g. Compiler(problem_kind=problem.kind, compilation_kind=GROUNDING)
-
-    To get a pipeline of Compilers there are two ways to call this method:
-    - using 'names' (the names of the specific compilers), 'params'
-      (compilers dependent options) and 'compilation_kinds'.
-      e.g. Compiler(names=['up_quantifiers_remover', 'up_grounder'],
-                    params=[{'opt1': 'val1'}, {'opt2': 'val2'}],
-                    compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])
-    - using 'problem_kind' and 'compilation_kinds' parameters.
-      e.g. Compiler(problem_kind=problem.kind,
-                    compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])
+    *   | using ``names`` (the names of the specific compilers), ``params`` (compilers dependent options) and ``compilation_kinds``.
+        | e.g. ``Compiler(names=['up_quantifiers_remover', 'up_grounder'], params=[{'opt1': 'val1'}, {'opt2': 'val2'}], compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])``
+    *   | using ``problem_kind`` and ``compilation_kinds`` parameters.
+        | e.g. ``Compiler(problem_kind=problem.kind, compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])``
     """
-    return get_env().factory.Compiler(
+    return get_environment().factory.Compiler(
         name=name,
         names=names,
         params=params,
         problem_kind=problem_kind,
         compilation_kind=compilation_kind,
         compilation_kinds=compilation_kinds,
     )
 
 
-def Simulator(
+def SequentialSimulator(
     problem: "up.model.AbstractProblem",
     *,
     name: Optional[str] = None,
     params: Optional[Dict[str, str]] = None,
 ) -> "up.engines.engine.Engine":
     """
-    Returns a Simulator. There are two ways to call this method:
-    - using 'problem_kind' through the problem field.
-        e.g. Simulator(problem)
-    - using 'name' (the name of a specific simulator) and eventually some 'params'
-        (simulator dependent options).
-        e.g. Simulator(problem, name='sequential_simulator')
+    Returns a sequential simulator. There are two ways to call this method:
+
+    *   | using ``problem_kind`` through the problem field.
+        | e.g. ``SequentialSimulator(problem)``
+    *   | using ``name`` (the name of a specific simulator) and eventually some ``params`` (simulator dependent options).
+        | e.g. ``SequentialSimulator(problem, name='sequential_simulator')``
     """
-    return get_env().factory.Simulator(problem=problem, name=name, params=params)
+    return get_environment().factory.SequentialSimulator(
+        problem=problem, name=name, params=params
+    )
 
 
 def Replanner(
     problem: "up.model.AbstractProblem",
     *,
     name: Optional[str] = None,
     params: Optional[Dict[str, str]] = None,
     optimality_guarantee: Optional[Union["up.engines.OptimalityGuarantee", str]] = None,
 ) -> "up.engines.engine.Engine":
     """
     Returns a Replanner. There are two ways to call this method:
-    - using 'problem' (with its kind) and 'optimality_guarantee' parameters.
-      e.g. Replanner(problem, optimality_guarantee=SOLVED_OPTIMALLY)
-    - using 'name' (the name of a specific replanner) and 'params'
-      (replanner dependent options).
-      e.g. Replanner(problem, name='replanner[tamer]')
+
+    *   | using ``problem`` (with its kind) and ``optimality_guarantee`` parameters.
+        | e.g. ``Replanner(problem, optimality_guarantee=SOLVED_OPTIMALLY)``
+    *   | using ``name`` (the name of a specific replanner) and ``params`` (replanner dependent options).
+        | e.g. ``Replanner(problem, name='replanner[tamer]')``
     """
-    return get_env().factory.Replanner(
+    return get_environment().factory.Replanner(
         problem=problem,
         name=name,
         params=params,
         optimality_guarantee=optimality_guarantee,
     )
 
 
+def PlanRepairer(
+    *,
+    name: Optional[str] = None,
+    params: Optional[Dict[str, Any]] = None,
+    problem_kind: ProblemKind = ProblemKind(),
+    plan_kind: Optional[Union["PlanKind", str]] = None,
+    optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
+) -> "up.engines.engine.Engine":
+    """
+    Returns a plan repairer. There are two ways to call this method:
+
+    *   | using ``name`` (the name of a plan repairer) and eventually ``params``.
+        | e.g. ``PlanRepairer(name='xxx')``
+    *   | using ``problem_kind``, ``plan_kind`` and ``optimality_guarantee``.
+        | e.g. ``PlanRepairer(problem_kind=problem.kind, plan_kind=plan.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
+    """
+    return get_environment().factory.PlanRepairer(
+        name=name,
+        params=params,
+        problem_kind=problem_kind,
+        plan_kind=plan_kind,
+        optimality_guarantee=optimality_guarantee,
+    )
+
+
 def PortfolioSelector(
     *,
     name: Optional[str] = None,
     params: Optional[Dict[str, Any]] = None,
     problem_kind: ProblemKind = ProblemKind(),
     optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
 ) -> "up.engines.engine.Engine":
     """
     Returns a portfolio selector. There are two ways to call this method:
-    - using 'name' (the name of a specific portfolio) and eventually 'params'
-        (portfolio dependent options).
-        e.g. PortfolioSelector(name='ibacop')
-    - using 'problem_kind' and 'optimality_guarantee'.
-        e.g. OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)
+
+    *   | using ``name`` (the name of a specific portfolio) and eventually ``params`` (portfolio dependent options).
+        | e.g. ``PortfolioSelector(name='ibacop')``
+    *   | using ``problem_kind`` and ``optimality_guarantee``.
+        | e.g. ``OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
     """
-    return get_env().factory.PortfolioSelector(
+    return get_environment().factory.PortfolioSelector(
         name=name,
         params=params,
         problem_kind=problem_kind,
         optimality_guarantee=optimality_guarantee,
     )
 
 
 def print_engines_info(stream: IO[str] = sys.stdout, full_credits: bool = False):
-    get_env().factory.print_engines_info(stream, full_credits)
+    get_environment().factory.print_engines_info(stream, full_credits)
 
 
 def set_credits_stream(stream: Optional[IO[str]]):
-    get_env().credits_stream = stream
+    get_environment().credits_stream = stream
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/__init__.py` & `unified_planning-0.6.0/unified_planning/test/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,33 +14,34 @@
 
 
 import unittest
 import unified_planning as up
 from functools import wraps
 from importlib.util import find_spec
 from unified_planning.engines import OperationMode
-from unified_planning.environment import get_env
+from unified_planning.environment import get_environment
 from unified_planning.model import ProblemKind
 from unified_planning.test.pddl import enhsp
 from typing import Optional
+import unified_planning.test.scheduling
 
 
 skipIf = unittest.skipIf
 SkipTest = unittest.SkipTest
 
 
 class skipIfEngineNotAvailable(object):
     """Skip a test if the given engine is not available."""
 
     def __init__(self, engine):
         self.engine = engine
 
     def __call__(self, test_fun):
         msg = "%s not available" % self.engine
-        cond = self.engine not in get_env().factory.engines
+        cond = self.engine not in get_environment().factory.engines
 
         @unittest.skipIf(cond, msg)
         @wraps(test_fun)
         def wrapper(*args, **kwargs):
             return test_fun(*args, **kwargs)
 
         return wrapper
@@ -57,15 +58,15 @@
         self.kind = kind
         self.optimality_guarantee = optimality_guarantee
 
     def __call__(self, test_fun):
         msg = "no oneshot planner available for the given problem kind"
         cond = False
         try:
-            get_env().factory._get_engine_class(
+            get_environment().factory._get_engine_class(
                 OperationMode.ONESHOT_PLANNER,
                 problem_kind=self.kind,
                 optimality_guarantee=self.optimality_guarantee,
             )
         except:
             cond = True
 
@@ -88,15 +89,15 @@
         self.kind = kind
         self.anytime_guarantee = anytime_guarantee
 
     def __call__(self, test_fun):
         msg = "no anytime planner available for the given problem kind"
         cond = False
         try:
-            get_env().factory._get_engine_class(
+            get_environment().factory._get_engine_class(
                 OperationMode.ANYTIME_PLANNER,
                 problem_kind=self.kind,
                 anytime_guarantee=self.anytime_guarantee,
             )
         except:
             cond = True
 
@@ -114,15 +115,15 @@
     def __init__(self, kind: ProblemKind):
         self.kind = kind
 
     def __call__(self, test_fun):
         msg = "no plan validator available for the given problem kind"
         cond = False
         try:
-            get_env().factory._get_engine_class(
+            get_environment().factory._get_engine_class(
                 OperationMode.PLAN_VALIDATOR, problem_kind=self.kind
             )
         except:
             cond = True
 
         @unittest.skipIf(cond, msg)
         @wraps(test_fun)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/examples/__init__.py` & `unified_planning-0.6.0/unified_planning/test/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/examples/minimals.py` & `unified_planning-0.6.0/unified_planning/test/examples/minimals.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
     )
     basic_with_costs = Example(problem=problem, plan=plan)
     problems["basic_with_costs"] = basic_with_costs
 
     # counter
     counter_1 = Fluent("counter_1", IntType(0, 10))
     counter_2 = Fluent("counter_2", IntType(0, 10))
-    fake_counter = Fluent("fake_counter", IntType(0, 10))
+    fake_counter = Fluent("fake_counter", RealType(0, 10))
     increase = InstantaneousAction("increase")
     increase.add_increase_effect(counter_1, 1)
     increase.add_effect(counter_2, Plus(counter_2, 1))
     increase.add_effect(fake_counter, Div(Times(fake_counter, 2), 2))
     problem = Problem("counter")
     problem.add_fluent(counter_1)
     problem.add_fluent(counter_2)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/examples/multi_agent.py` & `unified_planning-0.6.0/unified_planning/test/examples/multi_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,32 +26,33 @@
 
     Location = UserType("Location")
 
     is_connected = Fluent("is_connected", BoolType(), l1=Location, l2=Location)
     problem.ma_environment.add_fluent(is_connected, default_initial_value=False)
 
     r = Agent("robot", problem)
-    pos = Fluent("pos", Location)
-    r.add_fluent(pos)
+    pos = Fluent("pos", position=Location)
+    r.add_fluent(pos, default_initial_value=False)
     move = InstantaneousAction("move", l_from=Location, l_to=Location)
     l_from = move.parameter("l_from")
     l_to = move.parameter("l_to")
-    move.add_precondition(Equals(pos, l_from))
+    move.add_precondition(pos(l_from))
     move.add_precondition(is_connected(l_from, l_to))
-    move.add_effect(pos, l_to)
+    move.add_effect(pos(l_to), True)
+    move.add_effect(pos(l_from), False)
     r.add_action(move)
     problem.add_agent(r)
 
     l1 = Object("l1", Location)
     l2 = Object("l2", Location)
     problem.add_objects([l1, l2])
 
     problem.set_initial_value(is_connected(l1, l2), True)
-    problem.set_initial_value(Dot(r, pos), l1)
-    problem.add_goal(Equals(Dot(r, pos), l2))
+    problem.set_initial_value(Dot(r, pos(l1)), True)
+    problem.add_goal(Dot(r, pos(l2)))
 
     plan = up.plans.SequentialPlan(
         [up.plans.ActionInstance(move, (ObjectExp(l1), ObjectExp(l2)), r)]
     )
 
     basic = Example(problem=problem, plan=plan)
     problems["ma-basic"] = basic
@@ -64,41 +65,42 @@
     is_connected = Fluent("is_connected", BoolType(), l1=Location, l2=Location)
     cargo_at = Fluent("cargo_at", BoolType(), position=Location)
     problem.ma_environment.add_fluent(is_connected, default_initial_value=False)
     problem.ma_environment.add_fluent(cargo_at, default_initial_value=False)
 
     robot1 = Agent("robot1", problem)
     robot2 = Agent("robot2", problem)
-    pos = Fluent("pos", Location)
+    pos = Fluent("pos", position=Location)
 
     cargo_mounted = Fluent("cargo_mounted")
-    robot1.add_fluent(pos)
+    robot1.add_fluent(pos, default_initial_value=False)
     robot1.add_fluent(cargo_mounted)
-    robot2.add_fluent(pos)
+    robot2.add_fluent(pos, default_initial_value=False)
     robot2.add_fluent(cargo_mounted)
 
     move = InstantaneousAction("move", l_from=Location, l_to=Location)
     l_from = move.parameter("l_from")
     l_to = move.parameter("l_to")
-    move.add_precondition(Equals(pos, l_from))
+    move.add_precondition(pos(l_from))
     move.add_precondition(is_connected(l_from, l_to))
-    move.add_effect(pos, l_to)
+    move.add_effect(pos(l_to), True)
+    move.add_effect(pos(l_from), False)
 
     load = InstantaneousAction("load", loc=Location)
     loc = load.parameter("loc")
     load.add_precondition(cargo_at(loc))
-    load.add_precondition(Equals(pos, loc))
+    load.add_precondition(pos(loc))
     load.add_precondition(Not(cargo_mounted))
     load.add_effect(cargo_at(loc), False)
     load.add_effect(cargo_mounted, True)
 
     unload = InstantaneousAction("unload", loc=Location)
     loc = unload.parameter("loc")
     unload.add_precondition(Not(cargo_at(loc)))
-    unload.add_precondition(Equals(pos, loc))
+    unload.add_precondition(pos(loc))
     unload.add_precondition(cargo_mounted)
     unload.add_effect(cargo_at(loc), True)
     unload.add_effect(cargo_mounted, False)
 
     robot1.add_action(move)
     robot2.add_action(move)
     robot1.add_action(load)
@@ -112,16 +114,16 @@
     l2 = Object("l2", Location)
     l3 = Object("l3", Location)
     problem.add_objects([l1, l2, l3])
 
     problem.set_initial_value(is_connected(l1, l2), True)
     problem.set_initial_value(is_connected(l2, l1), True)
     problem.set_initial_value(is_connected(l2, l3), True)
-    problem.set_initial_value(Dot(robot1, pos), l2)
-    problem.set_initial_value(Dot(robot2, pos), l2)
+    problem.set_initial_value(Dot(robot1, pos(l2)), True)
+    problem.set_initial_value(Dot(robot2, pos(l2)), True)
     problem.set_initial_value(cargo_at(l1), True)
     problem.set_initial_value(cargo_at(l2), False)
     problem.set_initial_value(cargo_at(l3), False)
     problem.set_initial_value(Dot(robot1, cargo_mounted), False)
     problem.set_initial_value(Dot(robot2, cargo_mounted), False)
 
     problem.add_goal(cargo_at(l3))
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/examples/realistic.py` & `unified_planning-0.6.0/unified_planning/test/examples/realistic.py`

 * *Files 0% similar despite different names*

```diff
@@ -697,15 +697,15 @@
                 ),
                 Or(is_connected(l_to, mid_location), is_connected(mid_location, l_to)),
             ),
             mid_location,
         ),
     )
     dur_move.add_effect(StartTiming(1), is_at(l_from), False)
-    dur_move.add_effect(EndTiming(5), is_at(l_to), True)
+    dur_move.add_effect(EndTiming() - 5, is_at(l_to), True)
     l1 = Object("l1", Location)
     l2 = Object("l2", Location)
     l3 = Object("l3", Location)
     l4 = Object("l4", Location)
     l5 = Object("l5", Location)
     problem = Problem("timed_connected_locations")
     problem.add_fluent(is_at, default_initial_value=False)
@@ -726,15 +726,15 @@
         [
             (
                 Fraction(0, 1),
                 up.plans.ActionInstance(dur_move, (ObjectExp(l1), ObjectExp(l3))),
                 Fraction(6, 1),
             ),
             (
-                Fraction(6, 1),
+                Fraction(601, 100),
                 up.plans.ActionInstance(dur_move, (ObjectExp(l3), ObjectExp(l5))),
                 Fraction(6, 1),
             ),
         ]
     )
     timed_connected_locations = Example(problem=problem, plan=t_plan)
     problems["timed_connected_locations"] = timed_connected_locations
@@ -857,29 +857,29 @@
                 Fraction(0, 1),
                 up.plans.ActionInstance(
                     dur_move, (ObjectExp(r1), ObjectExp(l1), ObjectExp(l2))
                 ),
                 Fraction(10, 1),
             ),
             (
-                Fraction(10, 1),
+                Fraction(1001, 100),
                 up.plans.ActionInstance(
                     dur_move, (ObjectExp(r1), ObjectExp(l2), ObjectExp(l3))
                 ),
                 Fraction(10, 1),
             ),
             (
-                Fraction(10, 1),
+                Fraction(2002, 100),
                 up.plans.ActionInstance(
                     dur_move, (ObjectExp(r1), ObjectExp(l3), ObjectExp(l4))
                 ),
                 Fraction(10, 1),
             ),
             (
-                Fraction(10, 1),
+                Fraction(3003, 100),
                 up.plans.ActionInstance(
                     dur_move, (ObjectExp(r1), ObjectExp(l4), ObjectExp(l5))
                 ),
                 Fraction(10, 1),
             ),
         ]
     )
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/examples/testing_variants.py` & `unified_planning-0.6.0/unified_planning/test/examples/testing_variants.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,16 @@
     problem = Problem("robot_fluent_of_user_type_with_int_id")
     problem.add_fluent(is_at)
     problem.add_action(move)
     problem.add_object(l1)
     problem.add_object(l2)
     problem.set_initial_value(is_at(Int(0)), l1)
     problem.set_initial_value(is_at(1), l1)
+    problem.add_goal(is_at(0).Equals(l2))
+    problem.add_goal(is_at(1).Equals(l2))
     plan = unified_planning.plans.SequentialPlan(
         [
             unified_planning.plans.ActionInstance(
                 move, (Int(0), ObjectExp(l1), ObjectExp(l2))
             ),
             unified_planning.plans.ActionInstance(
                 move, (Int(1), ObjectExp(l1), ObjectExp(l2))
@@ -594,15 +596,15 @@
     visited = Fluent("visited", BoolType(), location=Location)
     move = InstantaneousAction("move", l_from=Location, l_to=Location)
     l_from = move.parameter("l_from")
     l_to = move.parameter("l_to")
     move.add_precondition(Not(Equals(l_from, l_to)))
     move.add_precondition(is_at(l_from))
     move.add_precondition(Not(is_at(l_to)))
-    move.add_precondition(Or(is_connected(l_from, l_to), is_connected(l_to, l_from)))
+    move.add_precondition(is_connected(l_from, l_to))
     move.add_effect(is_at(l_from), False)
     move.add_effect(is_at(l_to), True)
     move.add_effect(visited(l_to), True)
     l1 = Object("l1", Location)
     l2 = Object("l2", Location)
     l3 = Object("l3", Location)
     l4 = Object("l4", Location)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/citycar/domain.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/citycar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/citycar/problem.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/citycar/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/counters/domain.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/counters/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/counters/problem2.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/counters/problem2.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/depot/domain.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/depot/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/depot/problem.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/depot/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/enhsp.py` & `unified_planning-0.6.0/unified_planning/test/pddl/enhsp.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # limitations under the License.
 
 import os
 import unified_planning as up
 import unified_planning.engines
 from unified_planning.model.problem_kind import ProblemKind
 from unified_planning.engines import PlanGenerationResult, PlanGenerationResultStatus
-from unified_planning.environment import get_env
+from unified_planning.environment import get_environment
 from typing import List, Optional, Union, IO, Iterator
 
 
 FILE_PATH = os.path.dirname(os.path.abspath(__file__))
 
 
 class ENHSP(up.engines.PDDLPlanner, up.engines.mixins.AnytimePlannerMixin):
     def __init__(self):
-        up.engines.PDDLPlanner.__init__(self, False)
+        up.engines.PDDLPlanner.__init__(self, False, True)
         self._options = ["-planner", "opt-hrmax"]
 
     @property
     def name(self) -> str:
         return "ENHSP"
 
     def _get_cmd(
@@ -152,40 +152,47 @@
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
+        supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
+        supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind: "ProblemKind") -> bool:
         return problem_kind <= ENHSP.supported_kind()
 
     @staticmethod
     def get_credits(**kwargs) -> Optional[up.engines.Credits]:
         return None
 
 
-env = get_env()
+environment = get_environment()
 if os.path.isfile(
     os.path.join(FILE_PATH, "..", "..", "..", ".planners", "enhsp-20", "enhsp.jar")
 ):
-    env.factory.add_engine(
+    environment.factory.add_engine(
         "opt-pddl-planner", "unified_planning.test.pddl.enhsp", "ENHSP"
     )
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/htn-transport/domain.hddl` & `unified_planning-0.6.0/unified_planning/test/pddl/htn-transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/htn-transport/problem.hddl` & `unified_planning-0.6.0/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/matchcellar/domain.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/matchcellar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/miconic/domain.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/miconic/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/robot_fastener/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/safe_road/domain.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/safe_road/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/sailing/domain.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/sailing/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl` & `unified_planning-0.6.0/unified_planning/test/pddl/visit_precedence/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_anml_writer.py` & `unified_planning-0.6.0/unified_planning/test/test_anml_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from unified_planning.test import TestCase, main, skipIfEngineNotAvailable
 from unified_planning.test.examples import get_example_problems
 from unified_planning.io import ANMLWriter
 import tempfile
 import os
 
 
-class TestPythonWriter(TestCase):
+class TestANMLWriter(TestCase):
     def setUp(self):
         TestCase.setUp(self)
         self.problems = get_example_problems()
 
     def test_basic(self):
         problem = self.problems["basic"].problem
         aw = ANMLWriter(problem)
@@ -106,15 +106,15 @@
 action move(Location l_from, Location l_to) {
    duration >= 6 and duration <= 6;
    [ start, start ] is_at(l_from);
    [ start, start ] (not is_at(l_to));
    [ start, start ] (exists(Location mid_loc) { ((not ((mid_loc == l_from) or (mid_loc == l_to))) and (is_connected(l_from, mid_loc) or is_connected(mid_loc, l_from)) and (is_connected(l_to, mid_loc) or is_connected(mid_loc, l_to))) });
    [ start, end ] (exists(Location mid_loc) { ((not ((mid_loc == l_from) or (mid_loc == l_to))) and (is_connected(l_from, mid_loc) or is_connected(mid_loc, l_from)) and (is_connected(l_to, mid_loc) or is_connected(mid_loc, l_to))) });
    [ start + 1 ] is_at(l_from) := false;
-   [ end + 5 ] is_at(l_to) := true;
+   [ end - 5 ] is_at(l_to) := true;
 };
 instance Location l1, l2, l3, l4, l5;
 [ start ] is_at(l1) := true;
 is_connected(l1, l2) := true;
 is_connected(l2, l3) := true;
 is_connected(l3, l4) := true;
 is_connected(l4, l5) := true;
@@ -264,15 +264,20 @@
         import pytamer
 
         with tempfile.TemporaryDirectory() as tempdir:
             temp_file_name = os.path.join(tempdir, "test_file.anml")
             with OneshotPlanner(name="tamer") as tamer:
                 for example in self.problems.values():
                     problem = example.problem
-                    if tamer.supports(problem.kind):
+                    kind = problem.kind
+                    if (
+                        tamer.supports(kind)
+                        and not kind.has_increase_effects()
+                        and not kind.has_decrease_effects()
+                    ):
                         aw = ANMLWriter(problem)
                         aw.write_problem(temp_file_name)
                         tamer_env = pytamer.tamer_env_new()
                         pytamer_problem = pytamer.tamer_parse_anml(
                             tamer_env, temp_file_name
                         )
                         tamer_actions = list(
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_anytime.py` & `unified_planning-0.6.0/unified_planning/test/test_anytime.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import unified_planning as up
-import unified_planning.engines
 from unified_planning.shortcuts import *
 from unified_planning.model.problem_kind import (
     simple_numeric_kind,
     quality_metrics_kind,
 )
 from unified_planning.io import PDDLReader
 from unified_planning.model.metrics import MinimizeSequentialPlanLength
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_compilers_pipeline.py` & `unified_planning-0.6.0/unified_planning/test/test_compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_compilers_quality_metrics.py` & `unified_planning-0.6.0/unified_planning/test/test_compilers_quality_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,19 @@
                 CompilationKind.DISJUNCTIVE_CONDITIONS_REMOVING,
                 CompilationKind.NEGATIVE_CONDITIONS_REMOVING,
             ],
         ) as compiler:
             res = compiler.compile(problem)
         new_problem = res.problem
 
-        with OneshotPlanner(problem_kind=problem.kind) as planner:
+        with OneshotPlanner(problem_kind=new_problem.kind) as planner:
             self.assertNotEqual(planner, None)
-            plan = planner.solve(new_problem).plan
+
+            solve_res = planner.solve(new_problem)
+            plan = solve_res.plan
             new_plan = plan.replace_action_instances(res.map_back_action_instance)
             self.assertEqual(new_plan, test_plan)
 
     @skipIfNoOneshotPlannerForProblemKind(simple_numeric_kind.union(actions_cost_kind))
     def test_locations_connected_cost_minimize(self):
         problem, test_plan = self.problems["locations_connected_cost_minimize"]
         with Compiler(
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_conditional_effects_remover.py` & `unified_planning-0.6.0/unified_planning/test/test_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_contingent_pddl.py` & `unified_planning-0.6.0/unified_planning/test/test_contingent_pddl.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,24 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License
 
 import os
-import tempfile
-from typing import cast
-import pytest
 import unified_planning
 from unified_planning.shortcuts import *
-from unified_planning.test import TestCase, main, skipIfNoOneshotPlannerForProblemKind
-from unified_planning.io import PDDLWriter, PDDLReader
+from unified_planning.test import TestCase, main
+from unified_planning.io import PDDLReader
 from unified_planning.test.examples import get_example_problems
-from unified_planning.model.types import _UserType
-from unified_planning.engines import PlanGenerationResultStatus
 
 
 FILE_PATH = os.path.dirname(os.path.abspath(__file__))
 CONTINGENT_PDDL_DOMAINS_PATH = os.path.join(FILE_PATH, "contingent_pddl")
 
 
 class TestPddlIO(TestCase):
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_credits.py` & `unified_planning-0.6.0/unified_planning/test/test_credits.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             "  * Engine name: ",
             "  * Developers:  ",
             "  * Description: ",
             "  * Contacts:    ",
             "  * Website:     ",
             "  * License:     ",
         ]
-        get_env().factory.print_engines_info(credits, True)
+        get_environment().factory.print_engines_info(credits, True)
         credits_printed = credits.getvalue()
         # test that every keyword occur the same number of time in the printed result
         number_of_credits_printed = credits_printed.count(credits_keywords[0])
         if number_of_credits_printed > 0:  # If at least one credit was printed
             for keyword in credits_keywords:
                 self.assertIn(keyword, credits_printed)
                 self.assertEqual(
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_disjunctive_conditions_remover.py` & `unified_planning-0.6.0/unified_planning/test/test_disjunctive_conditions_remover.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import unified_planning
 from unified_planning.shortcuts import *
 from unified_planning.model.problem_kind import (
     basic_classical_kind,
     classical_kind,
     simple_numeric_kind,
+    bounded_types_kind,
     full_classical_kind,
     basic_temporal_kind,
 )
 from unified_planning.test import (
     TestCase,
     skipIfNoPlanValidatorForProblemKind,
     skipIfNoOneshotPlannerForProblemKind,
@@ -36,16 +37,20 @@
 
 
 class TestDisjunctiveConditionsRemover(TestCase):
     def setUp(self):
         TestCase.setUp(self)
         self.problems = get_example_problems()
 
-    @skipIfNoOneshotPlannerForProblemKind(classical_kind.union(simple_numeric_kind))
-    @skipIfNoPlanValidatorForProblemKind(full_classical_kind.union(simple_numeric_kind))
+    @skipIfNoOneshotPlannerForProblemKind(
+        classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
+    @skipIfNoPlanValidatorForProblemKind(
+        full_classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
     def test_robot_locations_visited(self):
         problem = self.problems["robot_locations_visited"].problem
 
         with Compiler(
             problem_kind=problem.kind,
             compilation_kind=CompilationKind.DISJUNCTIVE_CONDITIONS_REMOVING,
         ) as dnfr:
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_dnf.py` & `unified_planning-0.6.0/unified_planning/test/test_dnf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,57 +12,57 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import unified_planning
 from unified_planning.shortcuts import *
 from unified_planning.test import TestCase, main
-from unified_planning.environment import get_env
+from unified_planning.environment import get_environment
 from unified_planning.model.walkers import Dnf, Nnf, Substituter
 
 
 class TestDnf(TestCase):
     def setUp(self):
         TestCase.setUp(self)
-        self.sub = Substituter(get_env())
-        self.simp = get_env().simplifier
+        self.sub = Substituter(get_environment())
+        self.simp = get_environment().simplifier
 
     def _subs_simp(self, exp, subs):
         ne = self.sub.substitute(exp, subs)
         return self.simp.simplify(ne)
 
     def test_nnf_dnf_1(self):
-        n = Nnf(get_env())
-        dnf = Dnf(get_env())
+        n = Nnf(get_environment())
+        dnf = Dnf(get_environment())
 
         a = FluentExp(Fluent("a"))
         b = FluentExp(Fluent("b"))
         c = FluentExp(Fluent("c"))
         # !(a => (b && c))
         e1 = Not(Implies(a, And(b, c)))
         nnf1 = n.get_nnf_expression(e1)
         self.assertIn("(a and ((not b) or (not c)))", str(nnf1))
         dnf1 = dnf.get_dnf_expression(e1)
         self.assertIn("((a and (not b)) or (a and (not c)))", str(dnf1))
 
     def test_dnf_2(self):
-        dnf = Dnf(get_env())
+        dnf = Dnf(get_environment())
 
         a = FluentExp(Fluent("a"))
         b = FluentExp(Fluent("b"))
         c = FluentExp(Fluent("c"))
         d = FluentExp(Fluent("d"))
         # a && (!b || (!c && d))
         e2 = And(a, Or(Not(b), And(Not(c), d)))
         dnf2 = dnf.get_dnf_expression(e2)
         self.assertIn("((a and (not b)) or (a and (not c) and d))", str(dnf2))
 
     def test_nnf_dnf_3(self):
-        n = Nnf(get_env())
-        dnf = Dnf(get_env())
+        n = Nnf(get_environment())
+        dnf = Dnf(get_environment())
 
         a = FluentExp(Fluent("a"))
         b = FluentExp(Fluent("b"))
         c = FluentExp(Fluent("c"))
         # (a => b) Iff (a => c)
         e3 = Iff(Implies(a, b), Implies(a, c))
         nnf3 = n.get_nnf_expression(e3)
@@ -73,16 +73,16 @@
         )
         self.assertIn(
             "(not a) or ((not a) and c) or (b and (not a)) or (b and c) or (a and (not b) and (not c)",
             str(dnf3),
         )
 
     def test_nnf_dnf_4(self):
-        n = Nnf(get_env())
-        dnf = Dnf(get_env())
+        n = Nnf(get_environment())
+        dnf = Dnf(get_environment())
 
         a = FluentExp(Fluent("a"))
         b = FluentExp(Fluent("b"))
         # (a && ( a => b)) Iff (b || ( ((a => b ) && (b => a)) Iff ( a Iff b)))
         e4 = Iff(
             And(a, Implies(a, b)),
             Or(b, Iff(And(Implies(a, b), Implies(b, a)), Iff(a, b))),
@@ -99,16 +99,16 @@
         self.assertEqual(self._subs_simp(e4, subs), self._subs_simp(nnf4, subs))
         self.assertEqual(self._subs_simp(e4, subs), self._subs_simp(dnf4, subs))
         subs = {a: False, b: True}
         self.assertEqual(self._subs_simp(e4, subs), self._subs_simp(nnf4, subs))
         self.assertEqual(self._subs_simp(e4, subs), self._subs_simp(dnf4, subs))
 
     def test_nnf_dnf_5(self):
-        n = Nnf(get_env())
-        dnf = Dnf(get_env())
+        n = Nnf(get_environment())
+        dnf = Dnf(get_environment())
 
         a = FluentExp(Fluent("a"))
         b = FluentExp(Fluent("b"))
         c = FluentExp(Fluent("c"))
         d = FluentExp(Fluent("d"))
         # ((a && (c => a)) => d) Iff (( b => d) => c)
         e5 = Iff(Implies(And(a, Implies(c, a)), d), Implies(Implies(b, d), c))
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_factory.py` & `unified_planning-0.6.0/unified_planning/test/test_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 from unified_planning.test import TestCase, skipIfEngineNotAvailable
 
 
 class TestFactory(TestCase):
     @skipIfEngineNotAvailable("pyperplan")
     @skipIfEngineNotAvailable("tamer")
     def test_config_file(self):
-        self.assertTrue("pyperplan" in get_env().factory.preference_list)
+        self.assertTrue("pyperplan" in get_environment().factory.preference_list)
         with tempfile.TemporaryDirectory() as tempdir:
             config_filename = os.path.join(tempdir, "up.ini")
             with open(config_filename, "w") as config:
                 config.write("[global]\n")
                 config.write("engine_preference_list: tamer\n")
-            env = unified_planning.environment.Environment()
-            env.factory.configure_from_file(config_filename)
-            self.assertTrue("pyperplan" not in env.factory.preference_list)
-            self.assertEqual(env.factory.preference_list, ["tamer"])
+            environment = unified_planning.environment.Environment()
+            environment.factory.configure_from_file(config_filename)
+            self.assertTrue("pyperplan" not in environment.factory.preference_list)
+            self.assertEqual(environment.factory.preference_list, ["tamer"])
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_grounder.py` & `unified_planning-0.6.0/unified_planning/test/test_grounder.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 #
 
 from typing import cast
 import unified_planning
 from unified_planning.shortcuts import *
 from unified_planning.model.problem_kind import (
-    basic_classical_kind,
     classical_kind,
     simple_numeric_kind,
     general_numeric_kind,
+    bounded_types_kind,
     basic_temporal_kind,
     hierarchical_kind,
 )
 from unified_planning.test import (
     TestCase,
     skipIfNoPlanValidatorForProblemKind,
     skipIfNoOneshotPlannerForProblemKind,
@@ -51,16 +51,20 @@
         res_2 = gro.compile(problem, CompilationKind.GROUNDING)
         grounded_problem_2 = res_2.problem
 
         self.assertEqual(grounded_problem, grounded_problem_2)
         grounded_problem.name = problem.name
         self.assertEqual(grounded_problem, problem)
 
-    @skipIfNoOneshotPlannerForProblemKind(classical_kind.union(general_numeric_kind))
-    @skipIfNoPlanValidatorForProblemKind(classical_kind.union(general_numeric_kind))
+    @skipIfNoOneshotPlannerForProblemKind(
+        classical_kind.union(general_numeric_kind).union(bounded_types_kind)
+    )
+    @skipIfNoPlanValidatorForProblemKind(
+        classical_kind.union(general_numeric_kind).union(bounded_types_kind)
+    )
     def test_robot(self):
         problem = self.problems["robot"].problem
 
         gro = Grounder()
         res = gro.compile(problem, CompilationKind.GROUNDING)
         grounded_problem = res.problem
         assert isinstance(grounded_problem, Problem)
@@ -74,16 +78,20 @@
             plan = grounded_plan.replace_action_instances(res.map_back_action_instance)
             for ai in plan.actions:
                 a = ai.action
                 self.assertEqual(a, problem.action(a.name))
             with PlanValidator(problem_kind=problem.kind, plan_kind=plan.kind) as pv:
                 self.assertTrue(pv.validate(problem, plan))
 
-    @skipIfNoOneshotPlannerForProblemKind(classical_kind.union(simple_numeric_kind))
-    @skipIfNoPlanValidatorForProblemKind(classical_kind.union(simple_numeric_kind))
+    @skipIfNoOneshotPlannerForProblemKind(
+        classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
+    @skipIfNoPlanValidatorForProblemKind(
+        classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
     def test_robot_locations_connected(self):
         problem = self.problems["robot_locations_connected"].problem
 
         gro = Grounder()
         res = gro.compile(problem, CompilationKind.GROUNDING)
         grounded_problem = res.problem
         assert isinstance(grounded_problem, Problem)
@@ -97,16 +105,20 @@
             plan = grounded_plan.replace_action_instances(res.map_back_action_instance)
             for ai in plan.actions:
                 a = ai.action
                 self.assertEqual(a, problem.action(a.name))
             with PlanValidator(problem_kind=problem.kind, plan_kind=plan.kind) as pv:
                 self.assertTrue(pv.validate(problem, plan))
 
-    @skipIfNoOneshotPlannerForProblemKind(classical_kind.union(simple_numeric_kind))
-    @skipIfNoPlanValidatorForProblemKind(classical_kind.union(simple_numeric_kind))
+    @skipIfNoOneshotPlannerForProblemKind(
+        classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
+    @skipIfNoPlanValidatorForProblemKind(
+        classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
     def test_robot_locations_connected_from_factory(self):
         problem = self.problems["robot_locations_connected"].problem
 
         with Compiler(name="up_grounder") as grounder:
             self.assertTrue(grounder.supports(problem.kind))
             res = grounder.compile(problem, CompilationKind.GROUNDING)
             grounded_problem = res.problem
@@ -125,16 +137,20 @@
                     a = ai.action
                     self.assertEqual(a, problem.action(a.name))
                 with PlanValidator(
                     problem_kind=problem.kind, plan_kind=plan.kind
                 ) as pv:
                     self.assertTrue(pv.validate(problem, plan))
 
-    @skipIfNoOneshotPlannerForProblemKind(classical_kind.union(simple_numeric_kind))
-    @skipIfNoPlanValidatorForProblemKind(classical_kind.union(simple_numeric_kind))
+    @skipIfNoOneshotPlannerForProblemKind(
+        classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
+    @skipIfNoPlanValidatorForProblemKind(
+        classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
     def test_robot_locations_connected_from_factory_with_problem_kind(self):
         problem = self.problems["robot_locations_connected"].problem
         kind = problem.kind
 
         with Compiler(
             problem_kind=kind, compilation_kind=CompilationKind.GROUNDING
         ) as embedded_grounder:
@@ -167,15 +183,15 @@
     def test_hierarchical_blocks_world(self):
         problem = self.problems["hierarchical_blocks_world"].problem
 
         gro = Grounder()
         ground_result = gro.compile(problem, CompilationKind.GROUNDING)
         grounded_problem = ground_result.problem
         assert isinstance(grounded_problem, Problem)
-        self.assertEqual(len(grounded_problem.actions), 90)
+        self.assertEqual(len(grounded_problem.actions), 108)
         for a in grounded_problem.actions:
             self.assertEqual(len(a.parameters), 0)
 
         with OneshotPlanner(problem_kind=grounded_problem.kind) as planner:
             self.assertNotEqual(planner, None)
             grounded_plan = planner.solve(grounded_problem).plan
             plan = grounded_plan.replace_action_instances(
@@ -252,15 +268,15 @@
         assert isinstance(grounded_problem, Problem)
         self.assertEqual(len(grounded_problem.actions), 20)
         for a in grounded_problem.actions:
             self.assertEqual(len(a.parameters), 0)
 
     def test_matchcellar_static_duration(self):
         problem = self.problems["matchcellar_static_duration"].problem
-        fvo = problem.env.free_vars_oracle
+        fvo = problem.environment.free_vars_oracle
         gro = Grounder()
         ground_result = gro.compile(problem, CompilationKind.GROUNDING)
         grounded_problem = ground_result.problem
         assert isinstance(grounded_problem, Problem)
         self.assertEqual(len(grounded_problem.actions), 6)
         for a in grounded_problem.actions:
             a = cast(DurativeAction, a)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_infix_notation.py` & `unified_planning-0.6.0/unified_planning/test/test_infix_notation.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import unified_planning
 from unified_planning.shortcuts import *
 from unified_planning.test import TestCase
+from typing import List, Tuple
 
 
 class TestInfixNotation(TestCase):
     def setUp(self):
         TestCase.setUp(self)
 
     def test_infix_with_exp(self):
@@ -49,22 +50,22 @@
         r_2 = Variable("r_2", RealType())
         b_1 = Variable("b_1", BoolType())
         b_2 = Variable("b_2", BoolType())
         b_3 = Variable("b_3", BoolType())
         self._test_helper_function(i_1, r_1, i_2, r_2, b_1, b_2, b_3)
 
     def test_infix_with_parameters(self):
-        env = get_env()
-        i_1 = Parameter("i_1", IntType(), env)
-        r_1 = Parameter("r_1", RealType(), env)
-        i_2 = Parameter("i_2", IntType(), env)
-        r_2 = Parameter("r_2", RealType(), env)
-        b_1 = Parameter("b_1", BoolType(), env)
-        b_2 = Parameter("b_2", BoolType(), env)
-        b_3 = Parameter("b_3", BoolType(), env)
+        environment = get_environment()
+        i_1 = Parameter("i_1", IntType(), environment)
+        r_1 = Parameter("r_1", RealType(), environment)
+        i_2 = Parameter("i_2", IntType(), environment)
+        r_2 = Parameter("r_2", RealType(), environment)
+        b_1 = Parameter("b_1", BoolType(), environment)
+        b_2 = Parameter("b_2", BoolType(), environment)
+        b_3 = Parameter("b_3", BoolType(), environment)
         self._test_helper_function(i_1, r_1, i_2, r_2, b_1, b_2, b_3)
 
     def test_infix_on_objects(self):
         ut = UserType("ut")
         o_1 = Object("o_1", ut)
         o_2 = Object("o_2", ut)
         f_i = Fluent("f_i", ut, id=IntType())
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_multi_agent.py` & `unified_planning-0.6.0/unified_planning/test/test_multi_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,34 +43,35 @@
 
         Location = problem.user_type("Location")
         self.assertTrue(Location.is_user_type())
         self.assertEqual(Location.name, "Location")
         self.assertEqual(str(Location), "Location")
 
         pos = ag1.fluent("pos")
-        self.assertEqual(str(pos), "Location pos")
-        self.assertEqual(pos.arity, 0)
-        self.assertTrue(pos.type.is_user_type())
+        self.assertEqual(str(pos), "bool pos[position=Location]")
+        self.assertEqual(pos.arity, 1)
+        self.assertTrue(pos.type.is_bool_type())
 
         cargo_at = problem.ma_environment.fluent("cargo_at")
         self.assertEqual(cargo_at.name, "cargo_at")
         self.assertEqual(cargo_at.arity, 1)
         self.assertEqual(
-            cargo_at.signature, [up.model.Parameter("position", Location, problem.env)]
+            cargo_at.signature,
+            [up.model.Parameter("position", Location, problem.environment)],
         )
         self.assertTrue(cargo_at.type.is_bool_type())
 
         is_connected = problem.ma_environment.fluent("is_connected")
         self.assertEqual(is_connected.name, "is_connected")
         self.assertEqual(is_connected.arity, 2)
         self.assertEqual(
             is_connected.signature,
             [
-                up.model.Parameter("l1", Location, problem.env),
-                up.model.Parameter("l2", Location, problem.env),
+                up.model.Parameter("l1", Location, problem.environment),
+                up.model.Parameter("l2", Location, problem.environment),
             ],
         )
         self.assertTrue(is_connected.type.is_bool_type())
 
         cargo_mounted = ag1.fluent("cargo_mounted")
         self.assertEqual(cargo_mounted.name, "cargo_mounted")
         self.assertEqual(cargo_mounted.arity, 0)
@@ -82,15 +83,15 @@
         self.assertEqual(move.name, "move")
         self.assertEqual(len(move.parameters), 2)
         self.assertEqual(l_from.name, "l_from")
         self.assertEqual(l_from.type, Location)
         self.assertEqual(l_to.name, "l_to")
         self.assertEqual(l_to.type, Location)
         self.assertEqual(len(move.preconditions), 2)
-        self.assertEqual(len(move.effects), 1)
+        self.assertEqual(len(move.effects), 2)
 
         load = ag1.action("load")
         loc = load.parameter("loc")
         self.assertEqual(load.name, "load")
         self.assertEqual(len(load.parameters), 1)
         self.assertEqual(loc.name, "loc")
         self.assertEqual(loc.type, Location)
@@ -132,9 +133,19 @@
         self.assertEqual(ag1.action("move"), move)
         self.assertEqual(ag1.action("load"), load)
         self.assertEqual(ag1.action("unload"), unload)
         self.assertTrue(problem.initial_value(Dot(ag1, cargo_mounted)) is not None)
         self.assertTrue(problem.initial_value(cargo_at(l1)) is not None)
         self.assertTrue(problem.initial_value(cargo_at(l2)) is not None)
         self.assertTrue(problem.initial_value(cargo_at(l3)) is not None)
-        self.assertTrue(problem.initial_value(Dot(ag1, pos)) is not None)
+        self.assertTrue(problem.initial_value(Dot(ag1, pos(l1))) is not None)
+        self.assertTrue(problem.initial_value(Dot(ag1, pos(l2))) is not None)
+        self.assertTrue(problem.initial_value(Dot(ag1, pos(l3))) is not None)
         self.assertEqual(len(problem.goals), 1)
+
+    def test_normalize_plan(self):
+        problem, plan = self.problems["ma-loader"]
+
+        cloned_problem = problem.clone()
+        cloned_plan = cloned_problem.normalize_plan(plan)
+        for a, ca in zip(plan.actions, cloned_plan.actions):
+            self.assertTrue(a.is_semantically_equivalent(ca))
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_negative_conditions_remover.py` & `unified_planning-0.6.0/unified_planning/test/test_negative_conditions_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from fractions import Fraction
 import os
 from unified_planning.plans import ActionInstance
 import unified_planning
-from unified_planning.environment import get_env
+from unified_planning.environment import get_environment
 from unified_planning.shortcuts import *
 from unified_planning.test import (
     TestCase,
     main,
     skipIfNoPlanValidatorForProblemKind,
     skipIfNoOneshotPlannerForProblemKind,
 )
@@ -39,15 +39,15 @@
     UPProblemDefinitionError,
 )
 
 
 class TestNegativeConditionsRemover(TestCase):
     def setUp(self):
         TestCase.setUp(self)
-        self.env = get_env()
+        self.environment = get_environment()
         self.problems = get_example_problems()
 
     @skipIfNoOneshotPlannerForProblemKind(basic_classical_kind)
     @skipIfNoPlanValidatorForProblemKind(classical_kind)
     def test_basic(self):
         problem = self.problems["basic"].problem
         with Compiler(
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_partial_order_plan.py` & `unified_planning-0.6.0/unified_planning/test/test_partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_pddl_io.py` & `unified_planning-0.6.0/unified_planning/test/test_pddl_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 from typing import cast
 import pytest
 import unified_planning
 from unified_planning.shortcuts import *
 from unified_planning.test import TestCase, main, skipIfNoOneshotPlannerForProblemKind
 from unified_planning.io import PDDLWriter, PDDLReader
 from unified_planning.test.examples import get_example_problems
+from unified_planning.exceptions import UPProblemDefinitionError
 from unified_planning.model.problem_kind import simple_numeric_kind
 from unified_planning.model.metrics import MinimizeSequentialPlanLength
 from unified_planning.model.types import _UserType
-from unified_planning.engines import PlanGenerationResultStatus
 
 
 FILE_PATH = os.path.dirname(os.path.abspath(__file__))
 PDDL_DOMAINS_PATH = os.path.join(FILE_PATH, "pddl")
 
 
 class TestPddlIO(TestCase):
@@ -50,14 +50,42 @@
         self.assertIn(":effect (and (x))", pddl_domain)
 
         pddl_problem = w.get_problem()
         self.assertIn("(:domain basic-domain)", pddl_problem)
         self.assertIn("(:init)", pddl_problem)
         self.assertIn("(:goal (and (x)))", pddl_problem)
 
+    def test_basic_non_constant_boolean_assignment(self):
+        problem = self.problems["basic"].problem.clone()
+        x = problem.fluent("x")
+        y = problem.add_fluent("y", default_initial_value=True)
+        a = problem.action("a")
+        a.clear_effects()
+        a.add_effect(x, y)
+
+        w = PDDLWriter(problem)
+        with self.assertRaises(UPProblemDefinitionError) as e:
+            _ = w.get_domain()
+
+        w = PDDLWriter(problem, rewrite_bool_assignments=True)
+        pddl_domain = w.get_domain()
+        self.assertIn("(:requirements :strips :negative-preconditions)", pddl_domain)
+        self.assertIn("(:predicates (x) (y))", pddl_domain)
+        self.assertIn("(:action a", pddl_domain)
+        self.assertIn(":parameters ()", pddl_domain)
+        self.assertIn(":precondition (and (not (x)))", pddl_domain)
+        self.assertIn(
+            ":effect (and (when (y) (x)) (when (not (y)) (not (x)))))", pddl_domain
+        )
+
+        pddl_problem = w.get_problem()
+        self.assertIn("(:domain basic-domain)", pddl_problem)
+        self.assertIn("(:init (y))", pddl_problem)
+        self.assertIn("(:goal (and (x)))", pddl_problem)
+
     def test_basic_conditional_writer(self):
         problem = self.problems["basic_conditional"].problem
 
         self.assertTrue(problem.action("a_x").is_conditional())
         self.assertFalse(problem.action("a_y").is_conditional())
 
         w = PDDLWriter(problem)
@@ -434,27 +462,14 @@
             domain_str = file.read()
         with open(problem_filename, "r", encoding="utf-8") as file:
             problem_str = file.read()
 
         problem_2 = reader.parse_problem_string(domain_str, problem_str)
         self._test_htn_transport_reader(problem_2)
 
-    def test_hddl_parsing(self):
-        """Tests that all HDDL benchmarks are successfully parsed."""
-        hddl_dir = os.path.join(FILE_PATH, "hddl")
-        subfolders = [f.path for f in os.scandir(hddl_dir) if f.is_dir()]
-        for id, domain in enumerate(subfolders[:]):
-            print(f"=== [{id}] {domain} ===")
-            domain_filename = os.path.join(domain, "domain.hddl")
-            problem_filename = os.path.join(domain, "instance.1.pb.hddl")
-            reader = PDDLReader()
-            problem = reader.parse_problem(domain_filename, problem_filename)
-
-            assert isinstance(problem, up.model.htn.HierarchicalProblem)
-
     def test_examples_io(self):
 
         for example in self.problems.values():
             problem = example.problem
             kind = problem.kind
             if (
                 kind.has_intermediate_conditions_and_effects()
@@ -642,15 +657,15 @@
         domain_filename = os.path.join(
             PDDL_DOMAINS_PATH, "visit_precedence", "domain.pddl"
         )
         problem_filename = os.path.join(
             PDDL_DOMAINS_PATH, "visit_precedence", "problem.pddl"
         )
         problem = reader.parse_problem(domain_filename, problem_filename)
-        em = problem.env.expression_manager
+        em = problem.environment.expression_manager
 
         self.assertIsNotNone(problem)
         self.assertEqual(len(problem.fluents), 2)
         self.assertEqual(len(problem.actions), 1)
         self.assertEqual(len(list(problem.objects(problem.user_type("location")))), 3)
         self.assertEqual(len(problem.goals), 1)
         self.assertEqual(len(problem.timed_goals), 0)
@@ -658,24 +673,24 @@
 
         visit = problem.action("visit")
         assert isinstance(visit, DurativeAction)
         to_visit = visit.parameter("to_visit")
         location = problem.user_type("location")
         precedes = problem.fluent("precedes")
         visited = problem.fluent("visited")
-        p = Variable("p", location, problem.env)
+        p = Variable("p", location, problem.environment)
         cond_test = em.Forall(
             em.And(
                 em.Or(em.Not(precedes(p, to_visit)), visited(p)),
                 em.Not(visited(to_visit)),
             ),
             p,
         )
-        l = Variable("l_0", location, problem.env)
-        l2 = Variable("l2", location, problem.env)
+        l = Variable("l_0", location, problem.environment)
+        l2 = Variable("l2", location, problem.environment)
         goal_test = em.Forall(
             em.And(
                 visited(l), em.Forall(em.Or(em.Not(precedes(l2, l)), visited(l2)), l2)
             ),
             l,
         )
         self.assertEqual(
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_pddl_planner.py` & `unified_planning-0.6.0/unified_planning/test/test_pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_planner.py` & `unified_planning-0.6.0/unified_planning/test/test_planner.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from typing import Callable
 import warnings
 import unified_planning as up
 from unified_planning.shortcuts import *
 from unified_planning.model.problem_kind import (
     basic_classical_kind,
     classical_kind,
     general_numeric_kind,
+    bounded_types_kind,
     quality_metrics_kind,
     oversubscription_kind,
 )
 from unified_planning.test import TestCase, main, skipIfEngineNotAvailable
 from unified_planning.test import skipIfNoOneshotPlannerForProblemKind
 from unified_planning.test.examples import get_example_problems
 from unified_planning.engines import PlanGenerationResultStatus, CompilationKind
 from unified_planning.engines.results import POSITIVE_OUTCOMES
+from unified_planning.engines.mixins.oneshot_planner import OneshotPlannerMixin
 from unified_planning.exceptions import UPUsageError
 from unified_planning.model.metrics import MinimizeSequentialPlanLength
 
 
 class TestPlanner(TestCase):
     def setUp(self):
         TestCase.setUp(self)
@@ -190,15 +193,17 @@
             final_report = planner.solve(problem)
             plan = final_report.plan
             self.assertEqual(
                 final_report.status, PlanGenerationResultStatus.SOLVED_OPTIMALLY
             )
             self.assertEqual(plan, opt_plan)
 
-    @skipIfNoOneshotPlannerForProblemKind(classical_kind.union(general_numeric_kind))
+    @skipIfNoOneshotPlannerForProblemKind(
+        classical_kind.union(general_numeric_kind).union(bounded_types_kind)
+    )
     def test_robot(self):
         problem = self.problems["robot"].problem
         move = problem.action("move")
 
         with OneshotPlanner(problem_kind=problem.kind) as planner:
             self.assertNotEqual(planner, None)
             final_report = planner.solve(problem)
@@ -282,10 +287,46 @@
             self.assertEqual(error_msg, str(e.exception))
 
             # Or we can set the check to be completely skipped
             planner.skip_checks = True
             plan = planner.solve(problem).plan
             self.assertIsNotNone(plan)
 
+    def test_engine_class(self):
+        with self.assertRaises(TypeError):
+            Engine()  # type: ignore[abstract]
+
+        class OneshotEnginePartial(Engine, OneshotPlannerMixin):
+            @property
+            def name(self):
+                return "PartialEngine"
+
+            def supports(self):
+                return True
+
+            def supported_kind(self):
+                return ProblemKind()
+
+        with self.assertRaises(TypeError):
+            OneshotEnginePartial()  # type: ignore[abstract]
+
+        class OneshotEngineComplete(OneshotEnginePartial):
+            @property
+            def name(self):
+                return "CompleteEngine"
+
+            def _solve(
+                self,
+                problem: "up.model.AbstractProblem",
+                heuristic: Optional[
+                    Callable[["up.model.state.State"], Optional[float]]
+                ] = None,
+                timeout: Optional[float] = None,
+                output_stream: Optional[IO[str]] = None,
+            ) -> "up.engines.results.PlanGenerationResult":
+                raise NotImplementedError
+
+        OneshotEngineComplete()
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_problem.py` & `unified_planning-0.6.0/unified_planning/test/test_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 
 import unified_planning as up
 from unified_planning.shortcuts import *
 from unified_planning.test import TestCase, main, examples
 from unified_planning.test.examples import get_example_problems
+from unified_planning.exceptions import UPTypeError
 
 
 class TestProblem(TestCase):
     def setUp(self):
         TestCase.setUp(self)
         self.problems = get_example_problems()
 
@@ -122,15 +123,16 @@
         self.assertEqual(str(Location), "Location")
 
         robot_at = problem.fluent("robot_at")
         self.assertEqual(robot_at.name, "robot_at")
         self.assertEqual(str(robot_at), "bool robot_at[position=Location]")
         self.assertEqual(robot_at.arity, 1)
         self.assertEqual(
-            robot_at.signature, [up.model.Parameter("position", Location, problem.env)]
+            robot_at.signature,
+            [up.model.Parameter("position", Location, problem.environment)],
         )
         self.assertTrue(robot_at.type.is_bool_type())
 
         battery_charge = problem.fluent("battery_charge")
         self.assertEqual(battery_charge.name, "battery_charge")
         self.assertEqual(str(battery_charge), "real[0, 100] battery_charge")
         self.assertEqual(battery_charge.arity, 0)
@@ -197,23 +199,25 @@
         self.assertTrue(Location.is_user_type())
         self.assertEqual(Location.name, "Location")
 
         robot_at = problem.fluent("robot_at")
         self.assertEqual(robot_at.name, "robot_at")
         self.assertEqual(robot_at.arity, 1)
         self.assertEqual(
-            robot_at.signature, [up.model.Parameter("position", Location, problem.env)]
+            robot_at.signature,
+            [up.model.Parameter("position", Location, problem.environment)],
         )
         self.assertTrue(robot_at.type.is_bool_type())
 
         cargo_at = problem.fluent("cargo_at")
         self.assertEqual(cargo_at.name, "cargo_at")
         self.assertEqual(cargo_at.arity, 1)
         self.assertEqual(
-            cargo_at.signature, [up.model.Parameter("position", Location, problem.env)]
+            cargo_at.signature,
+            [up.model.Parameter("position", Location, problem.environment)],
         )
         self.assertTrue(cargo_at.type.is_bool_type())
 
         cargo_mounted = problem.fluent("cargo_mounted")
         self.assertEqual(cargo_mounted.name, "cargo_mounted")
         self.assertEqual(cargo_mounted.arity, 0)
         self.assertTrue(cargo_mounted.type.is_bool_type())
@@ -292,40 +296,40 @@
 
         robot_at = problem.fluent("robot_at")
         self.assertEqual(robot_at.name, "robot_at")
         self.assertEqual(robot_at.arity, 2)
         self.assertEqual(
             robot_at.signature,
             [
-                up.model.Parameter("robot", Robot, problem.env),
-                up.model.Parameter("position", Location, problem.env),
+                up.model.Parameter("robot", Robot, problem.environment),
+                up.model.Parameter("position", Location, problem.environment),
             ],
         )
         self.assertTrue(robot_at.type.is_bool_type())
 
         cargo_at = problem.fluent("cargo_at")
         self.assertEqual(cargo_at.name, "cargo_at")
         self.assertEqual(cargo_at.arity, 2)
         self.assertEqual(
             cargo_at.signature,
             [
-                up.model.Parameter("cargo", Container, problem.env),
-                up.model.Parameter("position", Location, problem.env),
+                up.model.Parameter("cargo", Container, problem.environment),
+                up.model.Parameter("position", Location, problem.environment),
             ],
         )
         self.assertTrue(cargo_at.type.is_bool_type())
 
         cargo_mounted = problem.fluent("cargo_mounted")
         self.assertEqual(cargo_mounted.name, "cargo_mounted")
         self.assertEqual(cargo_mounted.arity, 2)
         self.assertEqual(
             cargo_mounted.signature,
             [
-                up.model.Parameter("cargo", Container, problem.env),
-                up.model.Parameter("robot", Robot, problem.env),
+                up.model.Parameter("cargo", Container, problem.environment),
+                up.model.Parameter("robot", Robot, problem.environment),
             ],
         )
         self.assertTrue(cargo_mounted.type.is_bool_type())
 
         move = problem.action("move")
         l_from = move.parameter("l_from")
         l_to = move.parameter("l_to")
@@ -493,38 +497,14 @@
                         problem.initial_value(distance(locations[i], locations[j])),
                         Int(-1),
                     )
                     self.assertEqual(
                         problem.initial_value(cost(locations[i], locations[j])), Int(0)
                     )
 
-    def test_htn_problem_creation(self):
-        problems = examples.hierarchical.get_example_problems()
-        problem = problems["htn-go"].problem
-        self.assertTrue(isinstance(problem, up.model.htn.HierarchicalProblem))
-        self.assertTrue(problem.kind.has_hierarchical())
-        self.assertEqual(2, len(problem.fluents))
-        self.assertEqual(1, len(problem.actions))
-        self.assertEqual(["go"], [task.name for task in problem.tasks])
-        self.assertEqual(
-            ["go-noop", "go-recursive"], [method.name for method in problem.methods]
-        )
-
-        go_direct = problem.method("go-noop")
-        self.assertEqual(0, len(go_direct.subtasks))
-        self.assertEqual(1, len(go_direct.preconditions))
-        self.assertEqual(0, len(go_direct.constraints))
-
-        go_indirect = problem.method("go-recursive")
-        self.assertEqual(2, len(go_indirect.subtasks))
-        self.assertEqual(2, len(go_indirect.preconditions))
-        self.assertEqual(1, len(go_indirect.constraints))
-
-        self.assertEqual(2, len(problem.task_network.subtasks))
-
     def test_simple_numeric_planning_kind(self):
 
         problem = self.problems["robot"].problem
         # False because the problem has an assignment instead of a decrease
         self.assertFalse(problem.kind.has_simple_numeric_planning())
 
         problem = self.problems["robot_decrease"].problem
@@ -540,18 +520,15 @@
         self.assertFalse(problem.kind.has_simple_numeric_planning())
 
         names_of_SNP_problems = [
             "counter_to_50",
             "robot_decrease",
             "robot_locations_connected",
             "robot_locations_visited",
-            "robot_with_durative_action",
             "robot_fluent_of_user_type_with_int_id",
-            "matchcellar_static_duration",
-            "locations_connected_cost_minimize",
         ]
         for problem, _ in self.problems.values():
             if problem.name in names_of_SNP_problems:
                 self.assertTrue(problem.kind.has_simple_numeric_planning())
             else:
                 self.assertFalse(problem.kind.has_simple_numeric_planning())
 
@@ -573,22 +550,33 @@
         l1 = Object("l1", Location)
         l2 = Object("l2", Location)
         problem.add_fluent(is_at, default_initial_value=False)
         problem.add_fluent(distance, default_initial_value=100)
         problem.add_fluent(total_distance, default_initial_value=0)
         problem.set_initial_value(distance(l1, l2), 5)
         problem.add_action(move)
+        problem.add_goal(distance(l1, l2) < 6)
 
         # This problem is not SNP because of the increase of 2*distance(l_from, l_to)
         # by grounding, this distance(l_from, l_to) becomes distance(l1, l2), so it can be seen as a constant.
         self.assertFalse(problem.kind.has_simple_numeric_planning())
         with Compiler(
             problem_kind=problem.kind, compilation_kind=CompilationKind.GROUNDING
         ) as grounder:
             grounded_problem = grounder.compile(
                 problem, CompilationKind.GROUNDING
             ).problem
             self.assertTrue(grounded_problem.kind.has_simple_numeric_planning())
 
+        with self.assertRaises(UPTypeError):
+            problem.set_initial_value(distance(l2, l1), 2.0)
+        with self.assertRaises(UPTypeError):
+            problem.set_initial_value(distance(l2, l1), "2.0")
+        with self.assertRaises(UPTypeError):
+            problem.set_initial_value(distance(l2, l1), "4/2")
+        with self.assertRaises(UPTypeError):
+            problem.set_initial_value(distance(l2, l1), Div(4, 2))
+        problem.set_initial_value(distance(l2, l1), "20")
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_pyperplan.py` & `unified_planning-0.6.0/unified_planning/test/test_pyperplan.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # limitations under the License.
 
 import warnings
 import unified_planning as up
 from unified_planning.shortcuts import *
 from unified_planning.engines.results import POSITIVE_OUTCOMES
 from unified_planning.test import TestCase, main, skipIfEngineNotAvailable
-from unified_planning.environment import get_env
+from unified_planning.environment import get_environment
 from unified_planning.test.examples import get_example_problems
 
 
 class TestPyperplan(TestCase):
     def setUp(self):
         TestCase.setUp(self)
-        self.env = get_env()
+        self.environment = get_environment()
         self.problems = get_example_problems()
 
     @skipIfEngineNotAvailable("pyperplan")
     def test_pyperplan(self):
         problem, plan = self.problems["robot_no_negative_preconditions"]
         with OneshotPlanner(name="pyperplan") as planner:
             self.assertNotEqual(planner, None)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_python_writer.py` & `unified_planning-0.6.0/unified_planning/test/test_python_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_quantifier_remover.py` & `unified_planning-0.6.0/unified_planning/test/test_quantifier_remover.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import os
 import unified_planning
-from unified_planning.environment import get_env
+from unified_planning.environment import get_environment
 from unified_planning.shortcuts import *
 from unified_planning.model.problem_kind import (
     classical_kind,
     full_classical_kind,
     basic_temporal_kind,
     simple_numeric_kind,
-    hierarchical_kind,
+    bounded_types_kind,
 )
 from unified_planning.test import (
     TestCase,
     skipIfNoPlanValidatorForProblemKind,
     skipIfNoOneshotPlannerForProblemKind,
 )
 from unified_planning.test.examples import get_example_problems
@@ -83,16 +83,20 @@
             uq_plan = planner.solve(uq_problem).plan
             new_plan = uq_plan.replace_action_instances(res.map_back_action_instance)
             with PlanValidator(
                 problem_kind=problem.kind, plan_kind=new_plan.kind
             ) as pv:
                 self.assertTrue(pv.validate(problem, new_plan))
 
-    @skipIfNoOneshotPlannerForProblemKind(classical_kind.union(simple_numeric_kind))
-    @skipIfNoPlanValidatorForProblemKind(full_classical_kind.union(simple_numeric_kind))
+    @skipIfNoOneshotPlannerForProblemKind(
+        classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
+    @skipIfNoPlanValidatorForProblemKind(
+        full_classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
     def test_robot_locations_connected(self):
         problem = self.problems["robot_locations_connected"].problem
         qr = QuantifiersRemover()
         res = qr.compile(problem, CompilationKind.QUANTIFIERS_REMOVING)
         uq_problem = res.problem
         assert isinstance(uq_problem, Problem)
         self.assertTrue(problem.kind.has_existential_conditions())
@@ -104,16 +108,20 @@
             uq_plan = planner.solve(uq_problem).plan
             new_plan = uq_plan.replace_action_instances(res.map_back_action_instance)
             with PlanValidator(
                 problem_kind=problem.kind, plan_kind=new_plan.kind
             ) as pv:
                 self.assertTrue(pv.validate(problem, new_plan))
 
-    @skipIfNoOneshotPlannerForProblemKind(classical_kind.union(simple_numeric_kind))
-    @skipIfNoPlanValidatorForProblemKind(full_classical_kind.union(simple_numeric_kind))
+    @skipIfNoOneshotPlannerForProblemKind(
+        classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
+    @skipIfNoPlanValidatorForProblemKind(
+        full_classical_kind.union(simple_numeric_kind).union(bounded_types_kind)
+    )
     def test_robot_locations_visited(self):
         problem = self.problems["robot_locations_visited"].problem
         qr = QuantifiersRemover()
         res = qr.compile(problem, CompilationKind.QUANTIFIERS_REMOVING)
         uq_problem = res.problem
         assert isinstance(uq_problem, Problem)
         self.assertTrue(problem.kind.has_existential_conditions())
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_replanner.py` & `unified_planning-0.6.0/unified_planning/test/test_replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_simplifier.py` & `unified_planning-0.6.0/unified_planning/test/test_simplifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 # limitations under the License.
 
 
 import unified_planning
 from unified_planning.shortcuts import *
 from unified_planning.test import TestCase, main
 from unified_planning.model.walkers import Simplifier, Substituter
-from unified_planning.environment import get_env
+from unified_planning.environment import get_environment
 from fractions import Fraction
+from typing import List
 
 
 class TestBoolOperators(TestCase):
     def setUp(self):
         TestCase.setUp(self)
 
     def test_and_constant(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         t = Bool(True)
         f = Bool(False)
         e1 = And(t, f)
         r1 = s.simplify(e1)
         self.assertEqual(r1, f)
         self.assertEqual(r1.constant_value(), False)
         e2 = And(t, e1)
@@ -39,15 +40,15 @@
         self.assertEqual(r2.constant_value(), False)
         e3 = And(t, t)
         r3 = s.simplify(e3)
         self.assertTrue(r3.is_constant())
         self.assertEqual(r3, t)
 
     def test_and_fluent(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = Fluent("x")
         y = Fluent("y")
         t = Bool(True)
         f = Bool(False)
         e1 = And(x, f)
         r1 = s.simplify(e1)
         self.assertEqual(r1, f)
@@ -70,15 +71,15 @@
         r7 = s.simplify(e7)
         self.assertEqual(r7, f)
         e8 = And(And(x, y), Not(x))
         r8 = s.simplify(e8)
         self.assertEqual(r8, f)
 
     def test_or_constant(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         t = Bool(True)
         f = Bool(False)
         e1 = Or(t, f)
         r1 = s.simplify(e1)
         self.assertEqual(r1, t)
         self.assertEqual(r1.constant_value(), True)
         e2 = Or(t, e1)
@@ -87,15 +88,15 @@
         self.assertEqual(r2.constant_value(), True)
         e3 = Or(f, f)
         r3 = s.simplify(e3)
         self.assertTrue(r3.is_constant())
         self.assertEqual(r3, f)
 
     def test_or_fluent(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = Fluent("x")
         y = Fluent("y")
         t = Bool(True)
         f = Bool(False)
         e1 = Or(x, t)
         r1 = s.simplify(e1)
         self.assertEqual(r1, t)
@@ -118,15 +119,15 @@
         r7 = s.simplify(e7)
         self.assertEqual(r7, t)
         e8 = Or(Or(x, y), Not(x))
         r8 = s.simplify(e8)
         self.assertEqual(r8, t)
 
     def test_not(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = Fluent("x")
         t = Bool(True)
         f = Bool(False)
         e1 = Or(x, Not(t))
         r1 = s.simplify(e1)
         self.assertEqual(r1, FluentExp(x))
         e2 = Not(Or(x, e1))
@@ -137,15 +138,15 @@
         r4 = s.simplify(Not(e4))
         self.assertEqual(FluentExp(x), r4)
         e5 = Not(Not(x))
         r5 = s.simplify(e5)
         self.assertEqual(r5, FluentExp(x))
 
     def test_iff(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = FluentExp(Fluent("x"))
         y = FluentExp(Fluent("y"))
         t = Bool(True)
         f = Bool(False)
         e1 = Iff(x, y)
         r1 = s.simplify(e1)
         self.assertEqual(r1, e1)
@@ -174,15 +175,15 @@
         r9 = s.simplify(e9)
         self.assertEqual(r9, Not(x))
         e10 = Iff(t, And(x, t))
         r10 = s.simplify(e10)
         self.assertEqual(r10, x)
 
     def test_implies(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = FluentExp(Fluent("x"))
         y = FluentExp(Fluent("y"))
         t = Bool(True)
         f = Bool(False)
         e1 = Implies(x, y)
         r1 = s.simplify(e1)
         self.assertEqual(r1, e1)
@@ -208,15 +209,15 @@
         r8 = s.simplify(e8)
         self.assertEqual(r8, x)
         e9 = Implies(x, f)
         r9 = s.simplify(e9)
         self.assertEqual(r9, Not(x))
 
     def test_equals(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = FluentExp(Fluent("x", IntType()))
         y = FluentExp(Fluent("y", IntType()))
         t = Bool(True)
         f = Bool(False)
         i1 = Int(5)
         i2 = Int(6)
         i3 = Real(Fraction(6))
@@ -230,15 +231,15 @@
         r3 = s.simplify(e3)
         self.assertEqual(r3, t)
         e4 = Equals(x, x)
         r4 = s.simplify(e4)
         self.assertEqual(r4, t)
 
     def test_le(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = FluentExp(Fluent("x", IntType()))
         y = FluentExp(Fluent("y", IntType()))
         t = Bool(True)
         f = Bool(False)
         i1 = Int(5)
         i2 = Int(6)
         i3 = Real(Fraction(6))
@@ -252,15 +253,15 @@
         r3 = s.simplify(e3)
         self.assertEqual(r3, t)
         e4 = LE(i2, i1)
         r4 = s.simplify(e4)
         self.assertEqual(r4, f)
 
     def test_lt(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = FluentExp(Fluent("x", IntType()))
         y = FluentExp(Fluent("y", IntType()))
         t = Bool(True)
         f = Bool(False)
         i1 = Int(5)
         i2 = Int(6)
         i3 = Real(Fraction(6))
@@ -274,15 +275,15 @@
         r3 = s.simplify(e3)
         self.assertEqual(r3, f)
         e4 = LT(i2, i1)
         r4 = s.simplify(e4)
         self.assertEqual(r4, f)
 
     def test_gt(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = FluentExp(Fluent("x", IntType()))
         y = FluentExp(Fluent("y", IntType()))
         t = Bool(True)
         f = Bool(False)
         i1 = Int(5)
         i2 = Int(6)
         i3 = Real(Fraction(6))
@@ -296,15 +297,15 @@
         r3 = s.simplify(e3)
         self.assertEqual(r3, f)
         e4 = GT(i2, i1)
         r4 = s.simplify(e4)
         self.assertEqual(r4, t)
 
     def test_ge(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = FluentExp(Fluent("x", IntType()))
         y = FluentExp(Fluent("y", IntType()))
         t = Bool(True)
         f = Bool(False)
         i1 = Int(5)
         i2 = Int(6)
         i3 = Real(Fraction(6))
@@ -324,15 +325,15 @@
 
 class TestArithmeticOperators(TestCase):
     def setUp(self):
         TestCase.setUp(self)
 
     def test_plus_constant(self):
         # simple plus
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         data1 = Fraction(5.0)
         data2 = 3
         fnode1 = Real(data1)
         fnode2 = Int(data2)
         fnode1_2 = Plus(fnode1, fnode2)
         result1_2 = s.simplify(fnode1_2)
         self.assertTrue(result1_2.constant_value() == 8)
@@ -345,15 +346,15 @@
         fnode_of_data_list = Plus(data_list)
         fnode_simplified = s.simplify(fnode_of_data_list)
         self.assertTrue(fnode_simplified.is_int_constant())
         self.assertEqual(fnode_simplified.constant_value(), 0)
 
     def test_plus_fluent(self):
         # plus with fluent
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         data2 = 3
         x = Fluent("x", IntType())
         y = Fluent("y", IntType())
         fnode2 = Int(data2)
         fnodex_2 = Plus(x, fnode2)
         data_list: List[Union[int, Fluent]] = [1, 5, 6, 2, 3, 4, -3, 5]
 
@@ -365,15 +366,15 @@
         data_list = [1, 5, 6, 2, -10, -5, 3, -2, x, y]
         fnode_of_data_list = Plus(data_list)
         fnode_simplified = s.simplify(fnode_of_data_list)
         self.assertEqual(fnode_simplified, Plus(x, y))
 
     def test_minus_constant(self):
         # simple minus
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         data1 = 5
         data2 = 3
         fnode1 = Int(data1)
         fnode2 = Int(data2)
         fnode1_2 = Minus(fnode1, fnode2)
         result1_2 = s.simplify(fnode1_2)
         self.assertEqual(result1_2.constant_value(), 2)
@@ -382,15 +383,15 @@
         for a in data_list:
             fnode_of_data_list = Minus(fnode_of_data_list, Int(a))
         fnode_simplified = s.simplify(fnode_of_data_list)
         self.assertEqual(fnode_simplified.constant_value(), -21)
 
     def test_minus_fluent(self):
         # minus with fluent
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         data2 = 3
         x = Fluent("x", IntType())
         y = Fluent("y", IntType())
         fnode2 = Int(data2)
         x_2 = Minus(x, fnode2)
         data_list = [1, 5, 6, 2, 3, 4, -3, 5]
         fnode_of_data_list = x_2
@@ -414,15 +415,15 @@
 
         e1 = Minus(x, y)
         r1 = s.simplify(e1)
         self.assertEqual(r1, e1)
 
     def test_times_constant(self):
         # simple times
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         data1 = 5
         data2 = 3
         fnode1 = Int(data1)
         fnode2 = Int(data2)
         fnode1_2 = Times(fnode1, fnode2)
         result1_2 = s.simplify(fnode1_2)
 
@@ -442,15 +443,15 @@
         r1 = s.simplify(e1)
         self.assertTrue(r1.is_constant())
         self.assertTrue(r1.constant_value() == 0)
         self.assertEqual(r1, Int(0))
 
     def test_times_fluent(self):
         # plus with fluent
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         data2 = 3
         x = FluentExp(Fluent("x", IntType()))
         fnode2 = Int(data2)
         x_2 = Times(x, fnode2)
         data_list = [1, 5, 6, 2, 3, 4, -3, 5]
 
         fnode_of_data_list = Int(0)
@@ -469,15 +470,15 @@
 
         e1 = Times(x, Div(1, 5), Int(5))
         r1 = s.simplify(e1)
         self.assertEqual(r1, x)
 
     def test_div_constant(self):
         # simple div
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         data1 = 5
         data2 = 3
         fnode1 = Int(data1)
         fnode2 = Int(data2)
         fnode1_2 = Div(fnode1, fnode2)
         result1_2 = s.simplify(fnode1_2)
         self.assertTrue(result1_2.is_constant())
@@ -509,15 +510,15 @@
             fnode_of_data_list = Div(fnode_of_data_list, Real(Fraction(a)))
         fnode_simplified = s.simplify(fnode_of_data_list)
         self.assertTrue(fnode_simplified.is_real_constant())
         self.assertEqual(fnode_simplified.constant_value(), 800)
 
     def test_div_fluent(self):
         # div with fluent
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         data2 = 3
         x = Fluent("x", IntType())
         fnode2 = Int(data2)
         x_2 = Div(x, fnode2)
         data_list: List[Union[Fraction, str]] = [Fraction(5), Fraction(1, 5)]
 
         fnode_of_data_list = Int(1)
@@ -532,15 +533,15 @@
         for a in data_list:
             fnode_of_data_list = Div(fnode_of_data_list, Real(Fraction(a)))
         fnode_of_data_list = Div(fnode_of_data_list, x_2)
         fnode_simplified = s.simplify(fnode_of_data_list)
         self.assertEqual(fnode_simplified, Div(Fraction("6.4"), Div(x, Int(3))))
 
     def test_general(self):
-        s = Simplifier(get_env())
+        s = Simplifier(get_environment())
         x = FluentExp(Fluent("x"))
         y = FluentExp(Fluent("y", IntType()))
         t = Bool(True)
         f = Bool(False)
         # ((25/5)*30*2*2) - (20*5) (500) == (25*4*10) / 2 (500)
         e1 = Equals(
             Minus(Times([Div(25, 5), 30, 2, 2]), Times(20, 5)), Div(Times(25, 4, 10), 2)
@@ -559,16 +560,16 @@
 
 
 class TestWithSubstituter(TestCase):
     def setUp(self):
         TestCase.setUp(self)
 
     def test_and_fluent(self):
-        s = Simplifier(get_env())
-        su = Substituter(get_env())
+        s = get_environment().simplifier
+        su = get_environment().substituter
         x = Fluent("x")
         y = FluentExp(Fluent("y"))
         t = Bool(True)
         f = Bool(False)
         e1 = And(x, f)
         sub: Dict[Expression, Expression] = {x: True}
         s1 = su.substitute(e1, sub)
@@ -604,16 +605,16 @@
         e7 = And(And(x, y), And(y, Not(x)))
         sub = {x: True, y: True}
         s7 = su.substitute(e7, sub)
         r7 = s.simplify(s7)
         self.assertEqual(r7, f)
 
     def test_or_fluent(self):
-        s = Simplifier(get_env())
-        su = Substituter(get_env())
+        s = Simplifier(get_environment())
+        su = Substituter(get_environment())
         x = Fluent("x")
         y = FluentExp(Fluent("y"))
         t = Bool(True)
         f = Bool(False)
         e1 = Or(x, t)
         sub: Dict[Expression, Expression] = {x: False}
         s1 = su.substitute(e1, sub)
@@ -658,16 +659,16 @@
         self.assertEqual(r8, t)
         sub = {x: False}
         s9 = su.substitute(e7, sub)
         r9 = s.simplify(s9)
         self.assertEqual(r9, t)
 
     def test_not(self):
-        s = Simplifier(get_env())
-        su = Substituter(get_env())
+        s = Simplifier(get_environment())
+        su = Substituter(get_environment())
         x = Fluent("x")
         t = Bool(True)
         f = Bool(False)
         e1 = Or(x, Not(t))
         sub: Dict[Expression, Expression] = {x: False}
         s1 = su.substitute(e1, sub)
         r1 = s.simplify(s1)
@@ -675,16 +676,16 @@
         e2 = Not(Or(x, e1))
         sub = {x: False}
         s2 = su.substitute(e2, sub)
         r2 = s.simplify(s2)
         self.assertEqual(r2, t)
 
     def test_iff(self):
-        s = Simplifier(get_env())
-        su = Substituter(get_env())
+        s = Simplifier(get_environment())
+        su = Substituter(get_environment())
         x = FluentExp(Fluent("x"))
         y = FluentExp(Fluent("y"))
         t = Bool(True)
         f = Bool(False)
         e1 = Iff(x, y)
         sub: Dict[Expression, Expression] = {x: False}
         s1 = su.substitute(e1, sub)
@@ -698,16 +699,16 @@
         e5 = Iff(And(x, t), f)
         sub = {x: False}
         s5 = su.substitute(e5, sub)
         r5 = s.simplify(s5)
         self.assertEqual(r5, t)
 
     def test_implies(self):
-        s = Simplifier(get_env())
-        su = Substituter(get_env())
+        s = Simplifier(get_environment())
+        su = Substituter(get_environment())
         x = FluentExp(Fluent("x"))
         y = FluentExp(Fluent("y"))
         t = Bool(True)
         e1 = Implies(x, y)
         sub: Dict[Expression, Expression] = {x: False}
         s1 = su.substitute(e1, sub)
         r1 = s.simplify(s1)
@@ -715,16 +716,16 @@
         e3 = Implies(And(t, y), x)
         sub = {y: x, x: False}
         s3 = su.substitute(e3, sub)
         r3 = s.simplify(s3)
         self.assertEqual(r3, Not(x))
 
     def test_num_to_bools_operators(self):
-        s = Simplifier(get_env())
-        su = Substituter(get_env())
+        s = Simplifier(get_environment())
+        su = Substituter(get_environment())
         a = FluentExp(Fluent("a", IntType()))
         b = FluentExp(Fluent("b", IntType()))
         c = FluentExp(Fluent("c", IntType()))
         d = FluentExp(Fluent("d", IntType()))
         x = FluentExp(Fluent("x"))
         y = FluentExp(Fluent("y"))
         t = Bool(True)
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_simulated_effects.py` & `unified_planning-0.6.0/unified_planning/test/test_simulated_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_tarski_converter.py` & `unified_planning-0.6.0/unified_planning/test/test_tarski_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,40 +59,40 @@
             "robot_locations_connected",
             "robot_locations_visited",
         ]
         for n in problems_to_test:
             problem, plan = self.problems[n]
             tarski_problem = up.interop.convert_problem_to_tarski(problem)
             new_problem = up.interop.convert_problem_from_tarski(
-                problem.env, tarski_problem
+                problem.environment, tarski_problem
             )
             new_plan = _switch_plan(plan, new_problem)
             pv = SequentialPlanValidator()
             self.assertTrue(pv.validate(new_problem, new_plan))
 
     @skipIfEngineNotAvailable("tarski_grounder")
     @skipIfNoOneshotPlannerForProblemKind(hierarchical_kind)
     def test_plan_hierarchical_blocks_world_object_as_root(self):
         problem, plan = self.problems["hierarchical_blocks_world_object_as_root"]
         tarski_problem = up.interop.convert_problem_to_tarski(problem)
         new_problem = up.interop.convert_problem_from_tarski(
-            problem.env, tarski_problem
+            problem.environment, tarski_problem
         )
         with OneshotPlanner(problem_kind=new_problem.kind) as planner:
             new_plan = planner.solve(new_problem).plan
             self.assertIsNotNone(new_plan)
             self.assertEqual(str(plan), str(new_plan))
 
     @skipIfEngineNotAvailable("tarski_grounder")
     @skipIfNoOneshotPlannerForProblemKind(hierarchical_kind)
     def test_plan_hierarchical_blocks_world_with_object(self):
         problem, plan = self.problems["hierarchical_blocks_world_with_object"]
         tarski_problem = up.interop.convert_problem_to_tarski(problem)
         new_problem = up.interop.convert_problem_from_tarski(
-            problem.env, tarski_problem
+            problem.environment, tarski_problem
         )
         with OneshotPlanner(problem_kind=new_problem.kind) as planner:
             new_plan = planner.solve(new_problem).plan
             self.assertIsNotNone(new_plan)
             self.assertEqual(str(plan), str(new_plan))
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_tarski_grounder.py` & `unified_planning-0.6.0/unified_planning/test/test_tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_trajectory_constraint.py` & `unified_planning-0.6.0/unified_planning/test/test_trajectory_constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 
 import unified_planning
 from unified_planning.io.pddl_reader import PDDLReader
 from unified_planning.test.examples import get_example_problems
 from unified_planning.shortcuts import *
 from unified_planning.test import TestCase, main
-from unified_planning.environment import get_env
 from unified_planning.engines.compilers.trajectory_constraints_remover import (
     TrajectoryConstraintsRemover,
 )
 
 
 class TestTrajectoryConstraint(TestCase):
     def setUp(self):
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_trajectory_constraints_remover.py` & `unified_planning-0.6.0/unified_planning/test/test_trajectory_constraints_remover.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from unified_planning.test import TestCase
 
 
 class TestTrajectoryConstraintsRemoverCase(TestCase):
     def setUp(self):
         TestCase.setUp(self)
         problem, fluents, actions = self.get_problem()
-        self.simplifier = Simplifier(problem.env)
+        self.simplifier = Simplifier(problem.environment)
         self.problem = problem
         self.fluents = fluents
         self.actions = actions
         self.traj_remover = TrajectoryConstraintsRemover()
 
     def get_problem(self):
         problem = Problem("test_traj_constr_remover")
@@ -69,27 +69,27 @@
         a_phi = FluentExp(self.fluents[0])
         b_phi = FluentExp(self.fluents[1])
         c_phi = FluentExp(self.fluents[2])
         d_phi = FluentExp(self.fluents[3])
         e_phi = FluentExp(self.fluents[4])
         act_1 = self.actions[0]
         R_a = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, a_phi, act_1)
+            self.traj_remover._regression(self.problem.environment, a_phi, act_1)
         )
         R_b = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, b_phi, act_1)
+            self.traj_remover._regression(self.problem.environment, b_phi, act_1)
         )
         R_c = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, c_phi, act_1)
+            self.traj_remover._regression(self.problem.environment, c_phi, act_1)
         )
         R_d = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, d_phi, act_1)
+            self.traj_remover._regression(self.problem.environment, d_phi, act_1)
         )
         R_e = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, e_phi, act_1)
+            self.traj_remover._regression(self.problem.environment, e_phi, act_1)
         )
         self.assertTrue(
             R_a.is_true()
             and R_b == b_phi
             and R_c == c_phi
             and R_d == d_phi
             and R_e == e_phi
@@ -100,27 +100,27 @@
         a_phi = FluentExp(self.fluents[0])
         b_phi = FluentExp(self.fluents[1])
         c_phi = FluentExp(self.fluents[2])
         d_phi = FluentExp(self.fluents[3])
         e_phi = FluentExp(self.fluents[4])
         act_2 = self.actions[1]
         R_a = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, a_phi, act_2)
+            self.traj_remover._regression(self.problem.environment, a_phi, act_2)
         )
         R_b = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, b_phi, act_2)
+            self.traj_remover._regression(self.problem.environment, b_phi, act_2)
         )
         R_c = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, c_phi, act_2)
+            self.traj_remover._regression(self.problem.environment, c_phi, act_2)
         )
         R_d = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, d_phi, act_2)
+            self.traj_remover._regression(self.problem.environment, d_phi, act_2)
         )
         R_e = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, e_phi, act_2)
+            self.traj_remover._regression(self.problem.environment, e_phi, act_2)
         )
         self.assertTrue(
             R_a.is_true()
             and R_b != b_phi
             and R_c != c_phi
             and R_d == d_phi
             and R_e == e_phi
@@ -131,27 +131,27 @@
         a_phi = FluentExp(self.fluents[0])
         b_phi = FluentExp(self.fluents[1])
         c_phi = FluentExp(self.fluents[2])
         d_phi = FluentExp(self.fluents[3])
         e_phi = FluentExp(self.fluents[4])
         act_3 = self.actions[2]
         R_a = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, a_phi, act_3)
+            self.traj_remover._regression(self.problem.environment, a_phi, act_3)
         )
         R_b = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, b_phi, act_3)
+            self.traj_remover._regression(self.problem.environment, b_phi, act_3)
         )
         R_c = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, c_phi, act_3)
+            self.traj_remover._regression(self.problem.environment, c_phi, act_3)
         )
         R_d = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, d_phi, act_3)
+            self.traj_remover._regression(self.problem.environment, d_phi, act_3)
         )
         R_e = self.simplifier.simplify(
-            self.traj_remover._regression(self.problem.env, e_phi, act_3)
+            self.traj_remover._regression(self.problem.environment, e_phi, act_3)
         )
         self.assertTrue(
             R_a == a_phi
             and R_b == b_phi
             and R_c == c_phi
             and R_d != d_phi
             and R_e != e_phi
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/test/test_validator.py` & `unified_planning-0.6.0/unified_planning/test/test_validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unified_planning as up
 from unified_planning.shortcuts import *
-from unified_planning.model.problem_kind import classical_kind, general_numeric_kind
+from unified_planning.engines import SequentialPlanValidator, FailedValidationReason
+from unified_planning.plans import SequentialPlan, ActionInstance
+from unified_planning.model.problem_kind import (
+    classical_kind,
+    general_numeric_kind,
+    bounded_types_kind,
+)
 from unified_planning.test import TestCase, main, skipIfNoPlanValidatorForProblemKind
 from unified_planning.test.examples import get_example_problems
 
 
 class TestPlanValidator(TestCase):
     def setUp(self):
         TestCase.setUp(self)
@@ -34,15 +40,17 @@
             res = validator.validate(problem, plan)
             self.assertEqual(res.status, up.engines.ValidationResultStatus.VALID)
 
             plan = up.plans.SequentialPlan([])
             res = validator.validate(problem, plan)
             self.assertEqual(res.status, up.engines.ValidationResultStatus.INVALID)
 
-    @skipIfNoPlanValidatorForProblemKind(classical_kind.union(general_numeric_kind))
+    @skipIfNoPlanValidatorForProblemKind(
+        classical_kind.union(general_numeric_kind).union(bounded_types_kind)
+    )
     def test_robot(self):
         problem, plan = self.problems["robot"]
 
         with PlanValidator(problem_kind=problem.kind, plan_kind=plan.kind) as validator:
             self.assertNotEqual(validator, None)
 
             res = validator.validate(problem, plan)
@@ -76,10 +84,31 @@
             res = validator.validate(problem, plan)
             self.assertEqual(res.status, up.engines.ValidationResultStatus.VALID)
 
             plan = up.plans.SequentialPlan([])
             res = validator.validate(problem, plan)
             self.assertEqual(res.status, up.engines.ValidationResultStatus.INVALID)
 
+    def test_invalid_report(self):
+        problem, plan = self.problems["travel"]
+        up_validator = SequentialPlanValidator()
+
+        # without the last action the goal fails.
+        failed_goal_plan = SequentialPlan([*plan.actions[:-1]])
+        res = up_validator.validate(problem, failed_goal_plan)
+        self.assertEqual(res.reason, FailedValidationReason.UNSATISFIED_GOALS)
+
+        # add an invalid action to the plan
+        move = problem.action("move")
+        l1 = problem.object("l1")
+        l2 = problem.object("l2")
+        invalid_action = ActionInstance(move, (ObjectExp(l2), ObjectExp(l1)))
+        actions = [*plan.actions]
+        actions.append(invalid_action)
+        invalid_action_plan = SequentialPlan(actions)
+        res = up_validator.validate(problem, invalid_action_plan)
+        self.assertEqual(res.reason, FailedValidationReason.INAPPLICABLE_ACTION)
+        self.assertEqual(res.inapplicable_action, invalid_action)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `unified_planning-0.5.0.93.dev1/unified_planning/utils.py` & `unified_planning-0.6.0/unified_planning/utils.py`

 * *Files identical despite different names*

