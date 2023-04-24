# Comparing `tmp/polars_lts_cpu-0.17.7.tar.gz` & `tmp/polars_lts_cpu-0.17.8.tar.gz`

## Comparing `polars_lts_cpu-0.17.7.tar` & `polars_lts_cpu-0.17.8.tar`

### file list

```diff
@@ -1,1098 +1,1113 @@
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123     6297 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0    10541 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3249 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8778 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20207 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       44 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17826 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      189 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123     6258 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    10844 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30013 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7044 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      988 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      702 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10285 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1064 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10139 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1655 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5381 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4476 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6444 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123    12591 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123    15314 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    17592 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123     1920 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/keywords.rs
--rw-r--r--   0     1001      123    28145 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123    15237 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     4572 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123     8985 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     4591 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/encodings/fixed.rs
--rw-r--r--   0     1001      123       47 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/encodings/mod.rs
--rw-r--r--   0     1001      123     4508 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/encodings/variable.rs
--rw-r--r--   0     1001      123    13678 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     2079 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123       98 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      229 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      548 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3247 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     2324 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6479 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    10473 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4554 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123     3030 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
--rw-r--r--   0     1001      123     6275 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
--rw-r--r--   0     1001      123    13665 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
--rw-r--r--   0     1001      123     2681 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
--rw-r--r--   0     1001      123     2534 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
--rw-r--r--   0     1001      123     5961 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
--rw-r--r--   0     1001      123    10673 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
--rw-r--r--   0     1001      123     2164 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4666 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     3906 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20859 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23518 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     8395 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5485 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    14279 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11824 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2002 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      589 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     3808 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     6295 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3801 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      635 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5076 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      366 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     3387 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      430 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    20481 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    13982 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1237 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123     1796 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4359 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     4505 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     6754 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2899 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9278 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4309 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    47176 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     3440 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6376 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123     1049 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1284 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3908 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     3577 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13439 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4335 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     6058 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     7074 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2986 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4151 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1208 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     1922 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     3702 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1284 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    21873 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    17432 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    17488 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     3153 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     2003 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5809 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     4131 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    21103 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     3929 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    11541 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14360 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31819 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2039 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      414 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    27366 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    18862 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9425 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123    20891 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
--rw-r--r--   0     1001      123      219 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     3333 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14990 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7031 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12749 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4207 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4288 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    14812 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6799 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3158 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47910 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     8358 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2886 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1028 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123     7265 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123       45 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/constants.rs
--rw-r--r--   0     1001      123    17248 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     4171 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123      935 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      650 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123     9424 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123    13169 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123      753 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123       85 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
--rw-r--r--   0     1001      123     1431 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1327 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123     4221 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
--rw-r--r--   0     1001      123     1910 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
--rw-r--r--   0     1001      123     1216 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
--rw-r--r--   0     1001      123      344 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123     1593 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
--rw-r--r--   0     1001      123    13227 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123      810 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     2541 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123     8119 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123      581 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
--rw-r--r--   0     1001      123    19222 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123      462 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      260 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
--rw-r--r--   0     1001      123      200 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    13416 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    19923 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     2700 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123      170 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
--rw-r--r--   0     1001      123    43864 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/functions.rs
--rw-r--r--   0     1001      123    10196 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     2181 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    64804 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2100 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123    15238 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      175 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     6825 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11393 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25656 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    24898 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29652 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15191 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    11905 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123     9752 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10463 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8115 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15277 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     3250 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3236 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14479 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6644 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    28276 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15130 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15747 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26502 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     2692 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27361 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13845 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     3161 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    19820 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10187 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    15276 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     4584 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13038 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      809 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    11879 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123     2645 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123      514 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/hash.rs
--rw-r--r--   0     1001      123     2709 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      583 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      573 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     1792 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1115 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      616 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123    19606 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
--rw-r--r--   0     1001      123     8679 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1207 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     1556 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    20366 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8845 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1410 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2291 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    11560 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    48300 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123     9463 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     5069 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    38411 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1395 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2986 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7728 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     2802 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19796 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10220 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6453 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     4443 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2549 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    15081 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23524 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4826 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2853 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32120 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123     9946 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2875 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123     9670 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2365 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    27269 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6214 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123     6264 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    25614 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8339 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     5308 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     4436 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    15385 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123    22376 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2403 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     2585 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     1539 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10234 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     6151 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5467 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7430 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    30762 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    20472 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     6630 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123     1859 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5041 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6064 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123    11229 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     7753 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1959 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2501 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    11998 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      533 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     2724 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    25934 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7689 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2650 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42410 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    12083 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5456 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     7675 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      433 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    36116 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     7874 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    33715 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     6634 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5179 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16609 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    16518 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     4115 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
--rw-r--r--   0     1001      123     7643 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    39255 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123     5636 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
--rw-r--r--   0     1001      123      218 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    15470 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14048 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39375 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10593 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    17214 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123    18264 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22392 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    16352 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     4295 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6076 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4247 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    11879 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123   124236 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    27513 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     3732 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5976 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     8795 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2183 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10935 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      457 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2684 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17653 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1896 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15733 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2411 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123    16406 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     6551 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9929 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    18441 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28511 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    13187 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    25008 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     9217 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10850 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    12962 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    18304 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15242 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     5829 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    15106 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14223 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6207 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18305 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5336 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     8004 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11029 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9735 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4471 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6297 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    37684 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      853 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5204 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1347 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4247 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5072 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18204 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2840 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     8117 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123     1396 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/utils/flatten.rs
--rw-r--r--   0     1001      123    31704 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1598 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13773 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123     1975 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     3160 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     6459 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     7771 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123      878 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/null.rs
--rw-r--r--   0     1001      123     1125 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     1807 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      232 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123       56 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123    24907 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123     1042 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      915 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4740 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1015 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1895 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9731 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3703 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2022 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    18684 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3924 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11659 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5504 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     8683 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1749 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14367 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123     9070 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11609 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4698 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8335 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     2310 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
--rw-r--r--   0     1001      123     4343 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
--rw-r--r--   0     1001      123     2606 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
--rw-r--r--   0     1001      123     4417 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      434 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      762 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2821 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2533 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5020 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0     4341 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123     2383 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3608 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28678 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1898 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19712 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    21432 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10817 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13909 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    31242 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    25183 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    13265 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7586 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9222 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8282 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123    11046 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/json.rs
--rw-r--r--   0     1001      123     4864 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7215 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ndjson_core/buffer.rs
--rw-r--r--   0     1001      123       39 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ndjson_core/mod.rs
--rw-r--r--   0     1001      123    12172 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
--rw-r--r--   0     1001      123      273 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7360 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4784 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9606 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    16886 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10106 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      628 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4467 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      234 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1679 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2452 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    22005 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     5269 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      489 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9380 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8251 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123     2486 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18025 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13486 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      217 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     9623 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
--rw-r--r--   0     1001      123      118 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
--rw-r--r--   0     1001      123    11872 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3680 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     3423 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     3626 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123     1106 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123     3565 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    10476 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     7368 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     2717 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    21192 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    20108 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     4115 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123     9692 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     2960 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    31413 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      535 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123      320 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1568 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     4028 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12466 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1630 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     7059 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2567 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2008 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    23538 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    20089 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    24202 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    11624 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/LICENSE
--rw-r--r--   0     1001      123     2414 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/Makefile
--rw-r--r--   0     1001      123    12625 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/README.md
--rw-r--r--   0     1001      123      651 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/build.rs
--rw-r--r--   0     1001      123       32 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      450 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1567 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7302 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     1694 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1513 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      663 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      391 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      309 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1061 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1114 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      461 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      695 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      374 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      125 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      639 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      860 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123      968 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      692 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      392 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1269 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      252 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123      988 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123      358 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      256 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1103 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      744 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      428 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      749 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123      922 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      396 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1118 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      302 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123      647 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     6335 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/__init__.py
--rw-r--r--   0     1001      123    13396 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/api.py
--rw-r--r--   0     1001      123    25956 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/config.py
--rw-r--r--   0     1001      123    27169 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5057 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   304087 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    33240 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2628 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    11397 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1577 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4430 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    15109 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7338 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/dependencies.py
--rw-r--r--   0     1001      123     3436 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/expr/__init__.py
--rw-r--r--   0     1001      123     2730 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/expr/binary.py
--rw-r--r--   0     1001      123     1708 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/expr/categorical.py
--rw-r--r--   0     1001      123    69359 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/expr/datetime.py
--rw-r--r--   0     1001      123   250779 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/expr/expr.py
--rw-r--r--   0     1001      123    22899 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/expr/list.py
--rw-r--r--   0     1001      123     2059 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/expr/meta.py
--rw-r--r--   0     1001      123    44737 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/expr/string.py
--rw-r--r--   0     1001      123     5436 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/expr/struct.py
--rw-r--r--   0     1001      123     1981 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/functions/__init__.py
--rw-r--r--   0     1001      123    29688 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/functions/eager.py
--rw-r--r--   0     1001      123    90827 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/functions/lazy.py
--rw-r--r--   0     1001      123     6293 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      280 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/internals.py
--rw-r--r--   0     1001      123      978 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/_utils.py
--rw-r--r--   0     1001      123      878 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1082 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4691 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35533 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     8655 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/database.py
--rw-r--r--   0     1001      123    10988 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18459 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     6476 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1271 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5840 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      519 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/json.py
--rw-r--r--   0     1001      123     2257 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1299 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7212 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2331 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3611 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   166798 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24178 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/py.typed
--rw-r--r--   0     1001      123       69 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/__init__.py
--rw-r--r--   0     1001      123     1579 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/_numpy.py
--rw-r--r--   0     1001      123     1920 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/binary.py
--rw-r--r--   0     1001      123     1699 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/categorical.py
--rw-r--r--   0     1001      123    47526 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/datetime.py
--rw-r--r--   0     1001      123    12385 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/list.py
--rw-r--r--   0     1001      123   164038 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/series.py
--rw-r--r--   0     1001      123    27401 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/string.py
--rw-r--r--   0     1001      123     2287 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/struct.py
--rw-r--r--   0     1001      123     5375 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/series/utils.py
--rw-r--r--   0     1001      123     7638 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/sql/__init__.py
--rw-r--r--   0     1001      123     1351 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/sql/context.py
--rw-r--r--   0     1001      123     4764 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/testing/__init__.py
--rw-r--r--   0     1001      123      929 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/testing/_private.py
--rw-r--r--   0     1001      123     3689 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/testing/_tempdir.py
--rw-r--r--   0     1001      123    13597 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/testing/asserts.py
--rw-r--r--   0     1001      123      684 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/testing/parametric/__init__.py
--rw-r--r--   0     1001      123    25067 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/testing/parametric/primitives.py
--rw-r--r--   0     1001      123     7359 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/testing/parametric/strategies.py
--rw-r--r--   0     1001      123     5681 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/type_aliases.py
--rw-r--r--   0     1001      123     1211 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/__init__.py
--rw-r--r--   0     1001      123    50687 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/_construction.py
--rw-r--r--   0     1001      123     2782 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      721 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/_scan.py
--rw-r--r--   0     1001      123      687 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/build_info.py
--rw-r--r--   0     1001      123     8812 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/convert.py
--rw-r--r--   0     1001      123     5789 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2339 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    11592 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/polars/utils/various.py
--rw-r--r--   0     1001      123     5378 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/pyproject.toml
--rw-r--r--   0     1001      123      699 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/requirements-dev.txt
--rw-r--r--   0     1001      123       70 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/requirements-lint.txt
--rw-r--r--   0     1001      123     1640 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    11023 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     8388 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/apply/mod.rs
--rw-r--r--   0     1001      123    71480 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3902 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5250 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/batched_csv.rs
--rw-r--r--   0     1001      123    46606 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/conversion.rs
--rw-r--r--   0     1001      123    45472 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/dataframe.rs
--rw-r--r--   0     1001      123     3799 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/error.rs
--rw-r--r--   0     1001      123     9482 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/file.rs
--rw-r--r--   0     1001      123     7468 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/lazy/apply.rs
--rw-r--r--   0     1001      123    33439 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/lazy/dataframe.rs
--rw-r--r--   0     1001      123    62419 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/lazy/dsl.rs
--rw-r--r--   0     1001      123     1082 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/lazy/meta.rs
--rw-r--r--   0     1001      123      727 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/lazy/mod.rs
--rw-r--r--   0     1001      123      212 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/lazy/utils.rs
--rw-r--r--   0     1001      123    20992 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/lib.rs
--rw-r--r--   0     1001      123     8642 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/npy.rs
--rw-r--r--   0     1001      123     1029 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/object.rs
--rw-r--r--   0     1001      123      122 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/py_modules.rs
--rw-r--r--   0     1001      123    54535 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/series.rs
--rw-r--r--   0     1001      123     3478 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/set.rs
--rw-r--r--   0     1001      123      843 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7945 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     6530 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123     1633 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/parametric/conftest.py
--rw-r--r--   0     1001      123     3823 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     6863 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     8299 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3382 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      351 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    12662 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     2766 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123      280 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_duration.py
--rw-r--r--   0     1001      123    16033 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2801 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    29644 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    91606 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      418 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/datatypes/test_time.py
--rw-r--r--   0     1001      123      218 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1937 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    39498 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     6360 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     3456 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11169 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5919 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3720 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     6849 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2881 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11849 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    13735 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3259 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123     3218 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    15436 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    12750 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1748 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23698 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    16930 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     6238 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123     9412 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     4390 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123      956 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     2906 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     8252 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3664 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    22696 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123     2959 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_is_in.py
--rw-r--r--   0     1001      123    16937 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    10467 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    18639 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123    19550 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     3643 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     3631 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123     9814 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     4775 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1077 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    19856 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    39286 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     3497 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   120890 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_df.py
--rw-r--r--   0     1001      123     1196 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    16867 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2387 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    32643 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3305 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123    11420 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_functions.py
--rw-r--r--   0     1001      123     3763 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    33952 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    49534 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2369 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4014 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     6995 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11550 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     4743 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    13181 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     2634 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    83663 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_series.py
--rw-r--r--   0     1001      123     2561 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    13877 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_streaming.py
--rw-r--r--   0     1001      123    10700 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123      247 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     4307 2023-04-22 20:09:12.000000 polars_lts_cpu-0.17.7/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    66145 2023-04-22 20:10:10.000000 polars_lts_cpu-0.17.7/Cargo.lock
--rw-r--r--   0        0        0    15163 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.7/PKG-INFO
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123    19606 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
+-rw-r--r--   0     1001      123     8699 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1207 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     1556 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    20366 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8845 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1410 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2291 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    11560 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    48300 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123     9463 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     5069 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    38411 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1395 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2986 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7728 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     2802 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19796 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10220 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6453 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     4443 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2549 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    15081 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23524 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4826 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2853 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32120 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123     9946 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2875 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123     9670 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     2365 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    27269 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6214 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123     6264 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    25614 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8339 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     5308 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     4436 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    15385 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123     2658 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
+-rw-r--r--   0     1001      123    22407 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2403 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     2585 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     1539 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10234 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     6151 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5467 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7430 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    30762 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    20472 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     6630 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123     1859 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     5041 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6064 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123    11229 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     7753 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1959 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2501 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    11998 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      533 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     2724 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8113 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    25182 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7689 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     3946 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2650 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42410 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    12083 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5456 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     7675 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      433 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    36116 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     7874 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    33715 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     6634 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5179 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16609 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    16518 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     4115 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
+-rw-r--r--   0     1001      123     7643 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    39255 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123     5636 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
+-rw-r--r--   0     1001      123      218 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    19976 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14075 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39375 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10593 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    18842 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123    18264 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22392 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    16352 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     4295 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6076 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4247 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    11884 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123   124136 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    27513 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     3732 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5976 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     8795 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2183 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10935 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      457 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2684 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17653 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1896 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15733 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2411 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123    16652 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     4218 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     6551 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9929 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    18441 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28511 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    13187 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    25008 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     9217 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10850 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    12962 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18304 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15242 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     5829 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    15106 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14223 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6207 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18305 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5336 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     8004 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11029 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9735 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4471 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6297 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    37684 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5204 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4247 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5072 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18204 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2840 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     8117 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123     2494 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/utils/flatten.rs
+-rw-r--r--   0     1001      123    31704 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1598 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13773 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123     6297 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123     1796 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4359 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     4505 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     6754 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2899 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9278 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4309 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    47176 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     3440 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      416 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6376 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123     1049 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1284 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3908 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     3577 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13439 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4335 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     6058 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     7074 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1677 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2986 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4151 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1208 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     1922 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     3702 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1284 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    21873 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    17432 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    17488 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     3153 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     2003 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5809 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     4131 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    21103 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     3929 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    11541 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14360 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31819 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2039 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      414 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    27366 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    18862 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123     9425 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123    20891 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
+-rw-r--r--   0     1001      123      219 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     3333 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14990 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7031 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12749 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4207 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4288 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    14812 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6799 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3158 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47910 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     8358 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2886 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1028 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123    16037 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    20245 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123     1920 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/keywords.rs
+-rw-r--r--   0     1001      123      211 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123    15240 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     4572 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0     1001      123     1682 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/functions_cumulative.rs
+-rw-r--r--   0     1001      123     3063 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/functions_io.rs
+-rw-r--r--   0     1001      123     1539 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/functions_math.rs
+-rw-r--r--   0     1001      123     2982 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/functions_string.rs
+-rw-r--r--   0     1001      123     1056 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/iss_7436.rs
+-rw-r--r--   0     1001      123      888 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/iss_7437.rs
+-rw-r--r--   0     1001      123      652 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/iss_7440.rs
+-rw-r--r--   0     1001      123      700 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/iss_8395.rs
+-rw-r--r--   0     1001      123     1062 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/iss_8419.rs
+-rw-r--r--   0     1001      123    14296 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-sql/tests/simple_exprs.rs
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123       45 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/constants.rs
+-rw-r--r--   0     1001      123    17248 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4171 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123      935 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      650 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123     9880 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123    13169 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123      753 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1327 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4221 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123     1910 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
+-rw-r--r--   0     1001      123     1216 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
+-rw-r--r--   0     1001      123      344 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123     1593 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123    15231 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      810 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     2541 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123     8119 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    19416 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      260 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
+-rw-r--r--   0     1001      123      200 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    13668 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    19923 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     2700 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     5122 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123    43864 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/functions.rs
+-rw-r--r--   0     1001      123    10196 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2181 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    64804 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2100 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123    15238 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      175 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     6825 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11393 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25656 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    24898 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29652 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15191 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    11905 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123     9752 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10463 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8115 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15277 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     3250 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14479 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6644 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28276 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15130 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15747 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26502 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     3707 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27361 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13845 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     3161 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    19820 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10187 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    15276 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     4584 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13038 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      809 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    11879 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123     2645 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1373 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123      514 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/hash.rs
+-rw-r--r--   0     1001      123     2709 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      583 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      573 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     1792 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1115 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123      616 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123     1975 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     3160 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     6459 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     7771 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     1807 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      232 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123       56 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123    24907 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123     1042 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      915 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4740 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1015 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4907 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1895 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9731 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3703 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2022 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    18684 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3924 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11659 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5504 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     8683 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1749 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14367 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123     9070 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11609 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4698 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     8335 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4752 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      841 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     2310 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
+-rw-r--r--   0     1001      123     4343 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
+-rw-r--r--   0     1001      123     2606 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
+-rw-r--r--   0     1001      123     4417 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      434 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      762 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2821 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2533 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5232 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123     3565 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     7302 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    10495 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      428 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     7642 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     2717 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    21192 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    20108 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     4115 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123     9692 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     2960 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    31461 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      613 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123     3262 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/month_end.rs
+-rw-r--r--   0     1001      123     3468 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/month_start.rs
+-rw-r--r--   0     1001      123      320 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1568 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     4028 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12466 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1630 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     7255 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2567 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2491 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    25599 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    19317 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    24372 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    11624 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123     7393 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123     2383 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3608 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28678 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1898 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19712 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    21432 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10817 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13909 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    31242 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    25183 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    13265 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7586 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9222 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8282 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123    11046 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/json.rs
+-rw-r--r--   0     1001      123     4864 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7215 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ndjson_core/buffer.rs
+-rw-r--r--   0     1001      123       39 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ndjson_core/mod.rs
+-rw-r--r--   0     1001      123    12172 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
+-rw-r--r--   0     1001      123      273 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7360 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4784 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9606 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    16886 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10106 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      628 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4467 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123       98 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      229 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      548 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3247 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     2324 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6479 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    10473 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4554 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123     3030 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
+-rw-r--r--   0     1001      123     6275 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
+-rw-r--r--   0     1001      123    13665 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
+-rw-r--r--   0     1001      123     2681 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
+-rw-r--r--   0     1001      123     2534 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
+-rw-r--r--   0     1001      123     5961 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
+-rw-r--r--   0     1001      123    10673 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
+-rw-r--r--   0     1001      123     2164 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4666 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     3906 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20859 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23518 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     8395 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5485 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    14279 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11824 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2002 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      589 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     3808 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     6295 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3801 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      635 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5076 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      366 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     3387 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      430 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    20481 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    13982 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1237 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123     8985 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     4591 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/encodings/fixed.rs
+-rw-r--r--   0     1001      123       47 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/encodings/mod.rs
+-rw-r--r--   0     1001      123     4508 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/encodings/variable.rs
+-rw-r--r--   0     1001      123    13678 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     2079 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0        0        0    10541 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3592 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8778 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20207 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       44 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17826 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      189 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123     6258 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    10844 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30013 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7044 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      988 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      702 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10285 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1064 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10139 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1655 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5381 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4476 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6444 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123    12591 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      234 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1679 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2452 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    22005 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     5269 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      489 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9380 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     7490 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8251 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14731 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123     2486 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18025 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4174 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13486 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      217 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     9623 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
+-rw-r--r--   0     1001      123      118 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
+-rw-r--r--   0     1001      123    11872 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3688 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     3423 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123     1106 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2500 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/Makefile
+-rw-r--r--   0     1001      123    12625 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/README.md
+-rw-r--r--   0     1001      123      651 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/build.rs
+-rw-r--r--   0     1001      123       32 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      468 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1164 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/run_live_docs_server.py
+-rw-r--r--   0     1001      123     1567 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7326 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     1694 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1513 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      663 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      391 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      309 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1061 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1114 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      461 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      695 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      374 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      125 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      639 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      860 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123     1014 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      692 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      392 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1269 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      252 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123      988 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123      358 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      256 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      744 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      428 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      749 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123      922 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      396 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1168 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      302 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123     8067 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     6335 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/__init__.py
+-rw-r--r--   0     1001      123    13396 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/api.py
+-rw-r--r--   0     1001      123    25956 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/config.py
+-rw-r--r--   0     1001      123    27169 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5237 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   304748 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    33240 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2668 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    12133 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1603 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4430 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    15109 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7338 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/dependencies.py
+-rw-r--r--   0     1001      123     3436 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     2730 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1708 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    72692 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   251875 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/expr/expr.py
+-rw-r--r--   0     1001      123    22899 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/expr/list.py
+-rw-r--r--   0     1001      123     2059 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/expr/meta.py
+-rw-r--r--   0     1001      123    44737 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/expr/string.py
+-rw-r--r--   0     1001      123     5436 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/expr/struct.py
+-rw-r--r--   0     1001      123     1981 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    29637 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/functions/eager.py
+-rw-r--r--   0     1001      123    90827 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/functions/lazy.py
+-rw-r--r--   0     1001      123     6293 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      280 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/internals.py
+-rw-r--r--   0     1001      123      978 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/_utils.py
+-rw-r--r--   0     1001      123      878 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1082 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4691 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35533 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     8655 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/database.py
+-rw-r--r--   0     1001      123    10988 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18459 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     6476 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1271 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5840 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      519 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/json.py
+-rw-r--r--   0     1001      123     2257 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1299 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7212 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2331 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3611 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   167301 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24178 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/py.typed
+-rw-r--r--   0     1001      123       69 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1579 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     1920 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/binary.py
+-rw-r--r--   0     1001      123     1699 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/categorical.py
+-rw-r--r--   0     1001      123    49474 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/datetime.py
+-rw-r--r--   0     1001      123    12385 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/list.py
+-rw-r--r--   0     1001      123   164038 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/series.py
+-rw-r--r--   0     1001      123    27401 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/string.py
+-rw-r--r--   0     1001      123     2287 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/struct.py
+-rw-r--r--   0     1001      123     5375 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/series/utils.py
+-rw-r--r--   0     1001      123     7638 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/sql/__init__.py
+-rw-r--r--   0     1001      123     1351 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/sql/context.py
+-rw-r--r--   0     1001      123     4764 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/testing/__init__.py
+-rw-r--r--   0     1001      123      929 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/testing/_private.py
+-rw-r--r--   0     1001      123     3689 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/testing/_tempdir.py
+-rw-r--r--   0     1001      123    13597 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      800 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/testing/parametric/__init__.py
+-rw-r--r--   0     1001      123    25149 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/testing/parametric/primitives.py
+-rw-r--r--   0     1001      123     3409 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/testing/parametric/profiles.py
+-rw-r--r--   0     1001      123     7711 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/testing/parametric/strategies.py
+-rw-r--r--   0     1001      123     5824 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1211 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    50687 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     2782 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      721 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      687 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     8812 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/convert.py
+-rw-r--r--   0     1001      123     5789 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2339 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    11592 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/polars/utils/various.py
+-rw-r--r--   0     1001      123     5378 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/pyproject.toml
+-rw-r--r--   0     1001      123      699 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/requirements-dev.txt
+-rw-r--r--   0     1001      123       70 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/requirements-lint.txt
+-rw-r--r--   0     1001      123     1640 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    11023 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     8388 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/apply/mod.rs
+-rw-r--r--   0     1001      123    71480 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3902 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5250 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/batched_csv.rs
+-rw-r--r--   0     1001      123    46606 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/conversion.rs
+-rw-r--r--   0     1001      123    45472 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/dataframe.rs
+-rw-r--r--   0     1001      123     3799 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/error.rs
+-rw-r--r--   0     1001      123     9482 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/file.rs
+-rw-r--r--   0     1001      123     7468 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/lazy/apply.rs
+-rw-r--r--   0     1001      123    33439 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/lazy/dataframe.rs
+-rw-r--r--   0     1001      123    62598 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/lazy/dsl.rs
+-rw-r--r--   0     1001      123     1082 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/lazy/meta.rs
+-rw-r--r--   0     1001      123      727 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/lazy/mod.rs
+-rw-r--r--   0     1001      123      212 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/lazy/utils.rs
+-rw-r--r--   0     1001      123    20992 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/lib.rs
+-rw-r--r--   0     1001      123     8642 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/npy.rs
+-rw-r--r--   0     1001      123     1029 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/py_modules.rs
+-rw-r--r--   0     1001      123    54535 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/series.rs
+-rw-r--r--   0     1001      123     3478 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/set.rs
+-rw-r--r--   0     1001      123      843 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7945 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     6530 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123      179 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/parametric/conftest.py
+-rw-r--r--   0     1001      123     3823 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     1692 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123     6863 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     8299 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3382 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      351 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    12662 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     2826 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123      280 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_duration.py
+-rw-r--r--   0     1001      123    16033 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2801 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    29644 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    91697 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      418 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/datatypes/test_time.py
+-rw-r--r--   0     1001      123      218 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1937 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    39498 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     6360 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     3456 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11169 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5919 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3720 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     6849 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2881 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11849 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    13735 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3259 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123     3218 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    18655 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    12750 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1748 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    23698 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    16930 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     6238 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123     9412 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     4390 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123      956 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     2906 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     8252 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3664 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    22696 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123     2959 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_is_in.py
+-rw-r--r--   0     1001      123    16937 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    10467 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    18639 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123    19550 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     3643 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     3631 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123     9814 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     4775 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1077 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    19856 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    39286 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     3817 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   121069 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     1196 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    16867 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2387 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    32643 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3305 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123    11420 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_functions.py
+-rw-r--r--   0     1001      123     3763 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    33952 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    49534 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2369 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4014 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     6995 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11550 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     4743 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    13181 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     2634 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    84354 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_series.py
+-rw-r--r--   0     1001      123     2561 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    13877 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_streaming.py
+-rw-r--r--   0     1001      123    10700 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123      247 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     4307 2023-04-24 15:07:24.000000 polars_lts_cpu-0.17.8/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    65631 2023-04-24 15:08:19.000000 polars_lts_cpu-0.17.8/Cargo.lock
+-rw-r--r--   0        0        0    15163 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.8/PKG-INFO
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-error/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-error/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-error/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-error/src/lib.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/Makefile` & `polars_lts_cpu-0.17.8/local_dependencies/polars/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 .PHONY: fmt check check-features clippy clippy-default test test-doc integration-tests
 
 fmt:
 	cargo fmt --all
 	dprint fmt
 
+generate_test_files:
+	cargo run -p polars-cli "select * from read_csv('../examples/datasets/foods1.csv')" -o parquet > ../examples/datasets/foods1.parquet
+	cargo run -p polars-cli "select * from read_csv('../examples/datasets/foods1.csv')" -o arrow > ../examples/datasets/foods1.ipc
+
 check:
 	cargo check --all-features \
 		-p polars-core \
 		-p polars-io \
 		-p polars-lazy \
 		-p polars-arrow \
 		-p polars-time \
@@ -66,15 +70,16 @@
 	    --
 
 test-doc:
 	cargo test --doc \
 	    -p polars-lazy \
 	    -p polars-io \
 	    -p polars-core \
-	    -p polars-arrow
+	    -p polars-arrow \
+			-p polars-sql
 
 pre-commit: fmt clippy clippy-default  ## Run autoformatting and linting
 
 
 check-features:
 	cargo hack check --each-feature --no-dev-deps --features private 
 
@@ -89,14 +94,15 @@
 	cargo doc --all-features -p polars-utils
 	cargo doc --features=docs-selection -p polars-core
 	cargo doc -p polars-time
 	cargo doc -p polars-ops
 	cargo doc --all-features -p polars-io
 	cargo doc --all-features -p polars-lazy
 	cargo doc --features=docs-selection -p polars
+	cargo doc --all-features -p polars-sql
 
 publish:
 #	cargo publish --allow-dirty -p polars-error
 #	sleep 20
 #	cargo publish --allow-dirty -p polars-utils
 #	sleep 20
 #	cargo publish --allow-dirty -p polars-row
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/src/docs/eager.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/src/docs/lazy.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/src/docs/performance.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/src/lib.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/joins.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/random.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/core/series.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/io/csv.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/io/json.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/joins.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars/tests/it/schema.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-sql/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-sql/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 ipc = ["polars-lazy/ipc"]
 parquet = ["polars-lazy/parquet"]
 private = []
 
 [dependencies]
 polars-arrow = { version = "0.28.0", path = "../polars-arrow", features = ["like"] }
 polars-core = { version = "0.28.0", path = "../polars-core", features = [] }
-polars-lazy = { version = "0.28.0", path = "../polars-lazy", features = ["compile", "strings", "cross_join", "trigonometry", "abs", "round_series", "log", "regex", "is_in", "meta"] }
+polars-lazy = { version = "0.28.0", path = "../polars-lazy", features = ["compile", "strings", "cross_join", "trigonometry", "abs", "round_series", "log", "regex", "is_in", "meta", "cum_agg"] }
 polars-plan = { version = "0.28.0", path = "../polars-plan", features = ["compile"] }
 serde = "1"
 serde_json = { version = "1" }
 sqlparser = { version = "0.30" }
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-sql/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/context.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/context.rs`

 * *Files 16% similar despite different names*

```diff
@@ -12,63 +12,99 @@
 };
 use sqlparser::dialect::GenericDialect;
 use sqlparser::parser::Parser;
 
 use crate::sql_expr::{parse_sql_expr, process_join_constraint};
 use crate::table_functions::PolarsTableFunctions;
 
-thread_local! {pub(crate) static TABLES: RefCell<Vec<String>> = RefCell::new(vec![])}
-
 /// The SQLContext is the main entry point for executing SQL queries.
 #[derive(Default, Clone)]
 pub struct SQLContext {
     pub(crate) table_map: PlHashMap<String, LazyFrame>,
     pub(crate) tables: Vec<String>,
     cte_map: RefCell<PlHashMap<String, LazyFrame>>,
 }
 
 impl SQLContext {
     /// Create a new SQLContext
+    /// ```rust
+    /// # use polars_sql::SQLContext;
+    /// # fn main() {
+    /// let ctx = SQLContext::new();
+    /// # }
+    /// ```
     pub fn new() -> Self {
         Self {
             table_map: PlHashMap::new(),
             tables: vec![],
             cte_map: RefCell::new(PlHashMap::new()),
         }
     }
 
     /// Register a DataFrame as a table in the SQLContext.
+    /// ```rust
+    /// # use polars_sql::SQLContext;
+    /// # use polars_core::prelude::*;
+    /// # use polars_lazy::prelude::*;
+    /// # fn main() {
+    ///
+    /// let mut ctx = SQLContext::new();
+    ///
+    /// let df = df! {
+    ///    "a" =>  [1, 2, 3],
+    /// }.unwrap().lazy();
+    ///
+    /// ctx.register("df", df);
+    /// # }
+    ///```
     pub fn register(&mut self, name: &str, lf: LazyFrame) {
         self.table_map.insert(name.to_owned(), lf);
         self.tables.push(name.to_owned());
     }
 
+    /// Execute a sql query and return the result as a LazyFrame.
+    /// ```rust
+    /// # use polars_sql::SQLContext;
+    /// # use polars_core::prelude::*;
+    /// # use polars_lazy::prelude::*;
+    /// # fn main() {
+    ///
+    /// let mut ctx = SQLContext::new();
+    /// let df = df! {
+    ///    "a" =>  [1, 2, 3],
+    /// }
+    /// .unwrap();
+    ///
+    /// ctx.register("df", df.clone().lazy());
+    /// let sql_df = ctx.execute("SELECT * FROM df").unwrap().collect().unwrap();
+    /// assert!(sql_df.frame_equal(&df));
+    /// # }
+    ///```
+    pub fn execute(&mut self, query: &str) -> PolarsResult<LazyFrame> {
+        let ast = Parser::parse_sql(&GenericDialect::default(), query).map_err(to_compute_err)?;
+        polars_ensure!(ast.len() == 1, ComputeError: "One and only one statement at a time please");
+        let res = self.execute_statement(ast.get(0).unwrap());
+        // every execution should clear the cte map
+        self.cte_map.borrow_mut().clear();
+        res
+    }
+}
+
+impl SQLContext {
     fn register_cte(&mut self, name: &str, lf: LazyFrame) {
         self.cte_map.borrow_mut().insert(name.to_owned(), lf);
     }
 
     fn get_table_from_current_scope(&mut self, name: &str) -> Option<LazyFrame> {
         if let Some(lf) = self.table_map.get(name) {
             Some(lf.clone())
         } else {
             self.cte_map.borrow().get(name).cloned()
         }
     }
-}
-
-impl SQLContext {
-    /// Execute a sql query and return the result as a LazyFrame.
-    pub fn execute(&mut self, query: &str) -> PolarsResult<LazyFrame> {
-        let ast = Parser::parse_sql(&GenericDialect::default(), query).map_err(to_compute_err)?;
-        polars_ensure!(ast.len() == 1, ComputeError: "One and only one statement at a time please");
-        let res = self.execute_statement(ast.get(0).unwrap());
-        // every execution should clear the cte map
-        self.cte_map.borrow_mut().clear();
-        res
-    }
 
     pub(crate) fn execute_statement(&mut self, stmt: &Statement) -> PolarsResult<LazyFrame> {
         let ast = stmt;
         Ok(match ast {
             Statement::Query(query) => self.execute_query(query)?,
             stmt @ Statement::ShowTables { .. } => self.execute_show_tables(stmt)?,
             stmt @ Statement::CreateTable { .. } => self.execute_create_table(stmt)?,
@@ -374,23 +410,14 @@
             })
             .collect::<Vec<_>>();
 
         Ok(aggregated.select(&final_projection))
     }
 }
 
-impl Drop for SQLContext {
-    fn drop(&mut self) {
-        // drop old tables
-        TABLES.with(|cell| {
-            cell.borrow_mut().clear();
-        });
-    }
-}
-
 #[cfg(feature = "private")]
 impl SQLContext {
     /// get all registered tables. For internal use only.
     pub fn get_tables(&self) -> Vec<String> {
         self.tables.clone()
     }
     /// get internal table map. For internal use only.
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/functions.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/functions.rs`

 * *Files 18% similar despite different names*

```diff
@@ -341,14 +341,15 @@
 
 impl SqlFunctionVisitor<'_> {
     pub(crate) fn visit_function(&self) -> PolarsResult<Expr> {
         let function = self.func;
 
         let function_name: PolarsSqlFunctions = function.try_into()?;
         use PolarsSqlFunctions::*;
+
         match function_name {
             // ----
             // Math functions
             // ----
             Abs => self.visit_unary(Expr::abs),
             Acos => self.visit_unary(Expr::arccos),
             Asin => self.visit_unary(Expr::arcsin),
@@ -385,17 +386,17 @@
             },
             StartsWith => self.visit_binary(|e, s| e.str().starts_with(s)),
             EndsWith => self.visit_binary(|e, s| e.str().ends_with(s)),
             // ----
             // Aggregate functions
             // ----
             Count => self.visit_count(),
-            Sum => self.visit_unary(Expr::sum),
-            Min => self.visit_unary(Expr::min),
-            Max => self.visit_unary(Expr::max),
+            Sum => self.visit_unary_with_opt_cumulative(Expr::sum, Expr::cumsum),
+            Min => self.visit_unary_with_opt_cumulative(Expr::min, Expr::cummin),
+            Max => self.visit_unary_with_opt_cumulative(Expr::max, Expr::cummax),
             Avg => self.visit_unary(Expr::mean),
             StdDev => self.visit_unary(|e| e.std(1)),
             Variance => self.visit_unary(|e| e.var(1)),
             First => self.visit_unary(Expr::first),
             Last => self.visit_unary(Expr::last),
             // ----
             // Array functions
@@ -410,23 +411,72 @@
             Explode => self.visit_unary(|e| e.explode()),
             ArrayContains => self.visit_binary::<Expr>(|e, s| e.arr().contains(s)),
             ArrayGet => self.visit_binary(|e, i| e.arr().get(i)),
         }
     }
 
     fn visit_unary(&self, f: impl Fn(Expr) -> Expr) -> PolarsResult<Expr> {
+        self.visit_unary_no_window(f)
+            .and_then(|e| self.apply_window_spec(e, &self.func.over))
+    }
+
+    /// Some functions have cumulative equivalents that can be applied to window specs
+    /// e.g. SUM(a) OVER (ORDER BY b DESC) -> CUMSUM(a, false)
+    /// visit_unary_with_cumulative_window will take in a function & a cumulative function
+    /// if there is a cumulative window spec, it will apply the cumulative function,
+    /// otherwise it will apply the function
+    fn visit_unary_with_opt_cumulative(
+        &self,
+        f: impl Fn(Expr) -> Expr,
+        cumulative_f: impl Fn(Expr, bool) -> Expr,
+    ) -> PolarsResult<Expr> {
+        match self.func.over.as_ref() {
+            Some(spec) => self.apply_cumulative_window(f, cumulative_f, spec),
+            _ => self.visit_unary(f),
+        }
+    }
+    /// Window specs without partition bys are essentially cumulative functions
+    /// e.g. SUM(a) OVER (ORDER BY b DESC) -> CUMSUM(a, false)
+    fn apply_cumulative_window(
+        &self,
+        f: impl Fn(Expr) -> Expr,
+        cumulative_f: impl Fn(Expr, bool) -> Expr,
+        WindowSpec {
+            partition_by,
+            order_by,
+            ..
+        }: &WindowSpec,
+    ) -> PolarsResult<Expr> {
+        if !order_by.is_empty() && partition_by.is_empty() {
+            let (order_by, desc): (Vec<Expr>, Vec<bool>) = order_by
+                .iter()
+                .map(|o| {
+                    let expr = parse_sql_expr(&o.expr, self.ctx)?;
+                    Ok(match o.asc {
+                        Some(b) => (expr, !b),
+                        None => (expr, false),
+                    })
+                })
+                .collect::<PolarsResult<Vec<_>>>()?
+                .into_iter()
+                .unzip();
+            self.visit_unary_no_window(|e| cumulative_f(e.sort_by(&order_by, &desc), false))
+        } else {
+            self.visit_unary(f)
+        }
+    }
+
+    fn visit_unary_no_window(&self, f: impl Fn(Expr) -> Expr) -> PolarsResult<Expr> {
         let function = self.func;
         let args = extract_args(function);
         if let FunctionArgExpr::Expr(sql_expr) = args[0] {
             // parse the inner sql expr -- e.g. SUM(a) -> a
             let expr = parse_sql_expr(sql_expr, self.ctx)?;
             // apply the function on the inner expr -- e.g. SUM(a) -> SUM
-            let expr = f(expr);
-            // apply the window spec if present
-            self.apply_window_spec(expr, &function.over)
+            Ok(f(expr))
         } else {
             not_supported_error(function.name.0[0].value.as_str(), &args)
         }
     }
 
     fn visit_binary<Arg: FromSqlExpr>(&self, f: impl Fn(Expr, Arg) -> Expr) -> PolarsResult<Expr> {
         let function = self.func;
@@ -474,28 +524,44 @@
                     // count(distinct *) or count(distinct tbl.*) is not supported
                     return not_supported_error("count", &args);
                 }
             }
             _ => return not_supported_error("count", &args),
         })
     }
+
     fn apply_window_spec(
         &self,
         expr: Expr,
         window_spec: &Option<WindowSpec>,
     ) -> PolarsResult<Expr> {
         Ok(match &window_spec {
             Some(window_spec) => {
-                // Process for simple window specification, partition by first
-                let partition_by = window_spec
-                    .partition_by
-                    .iter()
-                    .map(|p| parse_sql_expr(p, self.ctx))
-                    .collect::<PolarsResult<Vec<_>>>()?;
-                expr.over(partition_by)
+                if window_spec.partition_by.is_empty() {
+                    let exprs = window_spec
+                        .order_by
+                        .iter()
+                        .map(|o| {
+                            let e = parse_sql_expr(&o.expr, self.ctx)?;
+                            match o.asc {
+                                Some(b) => Ok(e.sort(!b)),
+                                None => Ok(e),
+                            }
+                        })
+                        .collect::<PolarsResult<Vec<_>>>()?;
+                    expr.over(exprs)
+                } else {
+                    // Process for simple window specification, partition by first
+                    let partition_by = window_spec
+                        .partition_by
+                        .iter()
+                        .map(|p| parse_sql_expr(p, self.ctx))
+                        .collect::<PolarsResult<Vec<_>>>()?;
+                    expr.over(partition_by)
+                }
                 // Order by and Row range may not be supported at the moment
             }
             None => expr,
         })
     }
 }
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/keywords.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/keywords.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         polars_ensure!(
             refers_main_table, ComputeError:
             "compound identifier {:?} is not yet supported if multiple tables are registered",
             idents
         );
         Ok(col(&idents[1].value))
     }
+
     fn visit_unary_op(&self, op: &UnaryOperator, expr: &SqlExpr) -> PolarsResult<Expr> {
         let expr = self.visit_expr(expr)?;
         Ok(match op {
             UnaryOperator::Plus => lit(0) + expr,
             UnaryOperator::Minus => lit(0) - expr,
             UnaryOperator::Not => expr.not(),
             other => polars_bail!(ComputeError: "Unary operator {:?} is not supported", other),
@@ -222,14 +223,15 @@
             | SqlValue::HexStringLiteral(s)
             | SqlValue::DoubleQuotedString(s) => AnyValue::Utf8Owned(s.into()),
             SqlValue::Boolean(b) => AnyValue::Boolean(*b),
             SqlValue::Null => AnyValue::Null,
             other => polars_bail!(ComputeError: "SQL value {:?} is not yet supported", other),
         })
     }
+
     /// Visit a SQL `BETWEEN` expression
     /// See [sqlparser::ast::Expr::Between] for more details
     fn visit_between(
         &self,
         expr: &SqlExpr,
         negated: bool,
         low: &SqlExpr,
@@ -241,14 +243,15 @@
 
         if negated {
             Ok(expr.clone().lt(low).or(expr.gt(high)))
         } else {
             Ok(expr.clone().gt(low).and(expr.lt(high)))
         }
     }
+
     /// Visit a SQL 'TRIM' function
     /// See [sqlparser::ast::Expr::Trim] for more details
     fn visit_trim(
         &self,
         expr: &SqlExpr,
         trim_where: &Option<TrimWhereField>,
         trim_what: &Option<Box<SqlExpr>>,
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-sql/src/table_functions.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-row/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-row/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-row/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/encode.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/encode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/encodings/fixed.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/encodings/fixed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/encodings/variable.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/encodings/variable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/lib.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/row.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-row/src/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dot.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/lib.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/prelude.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-lazy/src/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-algo/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-algo/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-algo/src/algo.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-algo/src/algo.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use polars_core::error::PolarsResult as Result;
 use polars_core::prelude::*;
+use polars_core::series::IsSorted;
 use polars_lazy::prelude::*;
 use polars_ops::prelude::*;
 
 pub fn hist(s: &Series, bins: Option<&Series>, bin_count: Option<usize>) -> Result<DataFrame> {
     let breakpoint_str = &"break_point";
     let s = s.cast(&DataType::Float64)?.sort(false);
 
@@ -150,17 +151,22 @@
     let var_name = s.name();
     let breakpoint_str = break_point_label.unwrap_or("break_point");
     let category_str = category_label.unwrap_or("category");
 
     let bins_len = bins.len();
 
     bins.rename(breakpoint_str);
+
+    let mut s_bins = bins
+        .cast(&DataType::Float64)
+        .map_err(|_| PolarsError::ComputeError("expected numeric bins".into()))?
+        .extend_constant(AnyValue::Float64(f64::INFINITY), 1)?;
+    s_bins.set_sorted_flag(IsSorted::Ascending);
     let cuts_df = df![
-        breakpoint_str => bins.cast(&DataType::Float64).map_err(|_| PolarsError::ComputeError("expected numeric bins".into()))?
-            .extend_constant(AnyValue::Float64(f64::INFINITY), 1)?
+        breakpoint_str => s_bins
     ]?;
 
     let cuts_df = if let Some(labels) = labels {
         polars_ensure!(
             labels.len() == (bins_len + 1),
             ShapeMismatch: "labels count must equal bins count",
         );
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dot.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files 3% similar despite different names*

```diff
@@ -223,14 +223,28 @@
         let offset = offset.as_ref().into();
         self.0
             .map_private(FunctionExpr::TemporalExpr(TemporalFunction::Truncate(
                 every, offset,
             )))
     }
 
+    // roll backward to the first day of the month
+    #[cfg(feature = "date_offset")]
+    pub fn month_start(self) -> Expr {
+        self.0
+            .map_private(FunctionExpr::TemporalExpr(TemporalFunction::MonthStart))
+    }
+
+    // roll forward to the last day of the month
+    #[cfg(feature = "date_offset")]
+    pub fn month_end(self) -> Expr {
+        self.0
+            .map_private(FunctionExpr::TemporalExpr(TemporalFunction::MonthEnd))
+    }
+
     pub fn round<S: AsRef<str>>(self, every: S, offset: S) -> Expr {
         let every = every.as_ref().into();
         let offset = offset.as_ref().into();
         self.0
             .map_private(FunctionExpr::TemporalExpr(TemporalFunction::Round(
                 every, offset,
             )))
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     Minute,
     Second,
     Millisecond,
     Microsecond,
     Nanosecond,
     TimeStamp(TimeUnit),
     Truncate(String, String),
+    #[cfg(feature = "date_offset")]
+    MonthStart,
+    #[cfg(feature = "date_offset")]
+    MonthEnd,
     Round(String, String),
     #[cfg(feature = "timezones")]
     CastTimezone(Option<TimeZone>, Option<bool>),
     #[cfg(feature = "timezones")]
     TzLocalize(TimeZone),
     DateRange {
         name: String,
@@ -65,14 +69,18 @@
             Minute => "minute",
             Second => "second",
             Millisecond => "millisecond",
             Microsecond => "microsecond",
             Nanosecond => "nanosecond",
             TimeStamp(tu) => return write!(f, "dt.timestamp({tu})"),
             Truncate(..) => "truncate",
+            #[cfg(feature = "date_offset")]
+            MonthStart => "month_start",
+            #[cfg(feature = "date_offset")]
+            MonthEnd => "month_end",
             Round(..) => "round",
             #[cfg(feature = "timezones")]
             CastTimezone(_, _) => "replace_timezone",
             #[cfg(feature = "timezones")]
             TzLocalize(_) => "tz_localize",
             DateRange { .. } => return write!(f, "date_range"),
             Combine(_) => "combine",
@@ -201,14 +209,56 @@
             .unwrap()
             .truncate(every, offset, NO_TIMEZONE)?
             .into_series(),
         dt => polars_bail!(opq = round, got = dt, expected = "date/datetime"),
     })
 }
 
+#[cfg(feature = "date_offset")]
+pub(super) fn month_start(s: &Series) -> PolarsResult<Series> {
+    Ok(match s.dtype() {
+        DataType::Datetime(_, tz) => match tz {
+            #[cfg(feature = "timezones")]
+            Some(tz) => match tz.parse::<Tz>() {
+                Ok(tz) => s.datetime().unwrap().month_start(Some(&tz))?.into_series(),
+                Err(_) => match parse_offset(tz) {
+                    Ok(tz) => s.datetime().unwrap().month_start(Some(&tz))?.into_series(),
+                    Err(_) => unreachable!(),
+                },
+            },
+            _ => s
+                .datetime()
+                .unwrap()
+                .month_start(NO_TIMEZONE)?
+                .into_series(),
+        },
+        DataType::Date => s.date().unwrap().month_start(NO_TIMEZONE)?.into_series(),
+        dt => polars_bail!(opq = month_start, got = dt, expected = "date/datetime"),
+    })
+}
+
+#[cfg(feature = "date_offset")]
+pub(super) fn month_end(s: &Series) -> PolarsResult<Series> {
+    Ok(match s.dtype() {
+        DataType::Datetime(_, tz) => match tz {
+            #[cfg(feature = "timezones")]
+            Some(tz) => match tz.parse::<Tz>() {
+                Ok(tz) => s.datetime().unwrap().month_end(Some(&tz))?.into_series(),
+                Err(_) => match parse_offset(tz) {
+                    Ok(tz) => s.datetime().unwrap().month_end(Some(&tz))?.into_series(),
+                    Err(_) => unreachable!(),
+                },
+            },
+            _ => s.datetime().unwrap().month_end(NO_TIMEZONE)?.into_series(),
+        },
+        DataType::Date => s.date().unwrap().month_end(NO_TIMEZONE)?.into_series(),
+        dt => polars_bail!(opq = month_end, got = dt, expected = "date/datetime"),
+    })
+}
+
 pub(super) fn round(s: &Series, every: &str, offset: &str) -> PolarsResult<Series> {
     let every = Duration::parse(every);
     let offset = Duration::parse(offset);
     Ok(match s.dtype() {
         DataType::Datetime(_, tz) => match tz {
             #[cfg(feature = "timezones")]
             Some(tz) => match tz.parse::<Tz>() {
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/log.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -559,14 +559,18 @@
             Minute => map!(datetime::minute),
             Second => map!(datetime::second),
             Millisecond => map!(datetime::millisecond),
             Microsecond => map!(datetime::microsecond),
             Nanosecond => map!(datetime::nanosecond),
             TimeStamp(tu) => map!(datetime::timestamp, tu),
             Truncate(every, offset) => map!(datetime::truncate, &every, &offset),
+            #[cfg(feature = "date_offset")]
+            MonthStart => map!(datetime::month_start),
+            #[cfg(feature = "date_offset")]
+            MonthEnd => map!(datetime::month_end),
             Round(every, offset) => map!(datetime::round, &every, &offset),
             #[cfg(feature = "timezones")]
             CastTimezone(tz, use_earliest) => {
                 map!(datetime::replace_timezone, tz.as_deref(), use_earliest)
             }
             #[cfg(feature = "timezones")]
             TzLocalize(tz) => map!(datetime::tz_localize, &tz),
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,18 @@
                     Time => DataType::Time,
                     Date => DataType::Date,
                     Datetime => match mapper.with_same_dtype().unwrap().dtype {
                         DataType::Datetime(tu, _) => DataType::Datetime(tu, None),
                         dtype => polars_bail!(ComputeError: "expected Datetime, got {}", dtype),
                     },
                     Truncate(..) => mapper.with_same_dtype().unwrap().dtype,
+                    #[cfg(feature = "date_offset")]
+                    MonthStart => mapper.with_same_dtype().unwrap().dtype,
+                    #[cfg(feature = "date_offset")]
+                    MonthEnd => mapper.with_same_dtype().unwrap().dtype,
                     Round(..) => mapper.with_same_dtype().unwrap().dtype,
                     #[cfg(feature = "timezones")]
                     CastTimezone(tz, _use_earliest) => {
                         return mapper.map_datetime_dtype_timezone(tz.as_ref())
                     }
                     #[cfg(feature = "timezones")]
                     TzLocalize(tz) => return mapper.map_datetime_dtype_timezone(Some(tz)),
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/functions.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/prelude.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-plan/src/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-plan/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/arena.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/atomic.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/cell.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/functions.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/hash.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/lib.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/macros.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/macros.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/slice.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/sort.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/sync.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/unwrap.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-utils/src/wasm.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/arithmetic.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::ops::{BitAnd, BitOr, BitXor, Not};
 
 use arrow::compute;
 
 use super::*;
-use crate::utils::{align_chunks_binary, combine_validities, CustomIterTools};
+use crate::utils::{align_chunks_binary, combine_validities_and, CustomIterTools};
 
 impl<T> BitAnd for &ChunkedArray<T>
 where
     T: PolarsIntegerType,
     T::Native: BitAnd<Output = T::Native>,
 {
     type Output = ChunkedArray<T>;
@@ -16,15 +16,15 @@
         let (l, r) = align_chunks_binary(self, rhs);
         let chunks = l
             .downcast_iter()
             .zip(r.downcast_iter())
             .map(|(l_arr, r_arr)| {
                 let l_vals = l_arr.values().as_slice();
                 let r_vals = r_arr.values().as_slice();
-                let validity = combine_validities(l_arr.validity(), r_arr.validity());
+                let validity = combine_validities_and(l_arr.validity(), r_arr.validity());
 
                 let av = l_vals
                     .iter()
                     .zip(r_vals)
                     .map(|(l, r)| *l & *r)
                     .collect_trusted::<Vec<_>>();
 
@@ -49,15 +49,15 @@
         let (l, r) = align_chunks_binary(self, rhs);
         let chunks = l
             .downcast_iter()
             .zip(r.downcast_iter())
             .map(|(l_arr, r_arr)| {
                 let l_vals = l_arr.values().as_slice();
                 let r_vals = r_arr.values().as_slice();
-                let validity = combine_validities(l_arr.validity(), r_arr.validity());
+                let validity = combine_validities_and(l_arr.validity(), r_arr.validity());
 
                 let av = l_vals
                     .iter()
                     .zip(r_vals)
                     .map(|(l, r)| *l | *r)
                     .collect_trusted::<Vec<_>>();
 
@@ -82,15 +82,15 @@
         let (l, r) = align_chunks_binary(self, rhs);
         let chunks = l
             .downcast_iter()
             .zip(r.downcast_iter())
             .map(|(l_arr, r_arr)| {
                 let l_vals = l_arr.values().as_slice();
                 let r_vals = r_arr.values().as_slice();
-                let validity = combine_validities(l_arr.validity(), r_arr.validity());
+                let validity = combine_validities_and(l_arr.validity(), r_arr.validity());
 
                 let av = l_vals
                     .iter()
                     .zip(r_vals)
                     .map(|(l, r)| l.bitxor(*r))
                     .collect_trusted::<Vec<_>>();
 
@@ -186,15 +186,15 @@
         }
 
         let (l, r) = align_chunks_binary(self, rhs);
         let chunks = l
             .downcast_iter()
             .zip(r.downcast_iter())
             .map(|(l_arr, r_arr)| {
-                let validity = combine_validities(l_arr.validity(), r_arr.validity());
+                let validity = combine_validities_and(l_arr.validity(), r_arr.validity());
                 let values = l_arr.values() ^ r_arr.values();
 
                 let arr = BooleanArray::from_data_default(values, validity);
                 Box::new(arr) as ArrayRef
             })
             .collect::<Vec<_>>();
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 mod filter;
 pub mod full;
 #[cfg(feature = "interpolate")]
 mod interpolate;
 #[cfg(feature = "is_in")]
 mod is_in;
 mod len;
+pub(crate) mod min_max_binary;
 mod nulls;
 mod peaks;
 #[cfg(feature = "repeat_by")]
 mod repeat_by;
 mod reverse;
 pub(crate) mod rolling_window;
 mod set;
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 use crate::chunked_array::builder::{
     get_list_builder, AnonymousListBuilder, AnonymousOwnedListBuilder,
 };
 #[cfg(feature = "object")]
 use crate::chunked_array::object::ObjectArray;
 use crate::prelude::*;
+use crate::utils::flatten::flatten_par;
 use crate::utils::{get_iter_capacity, CustomIterTools, NoNull};
 
 impl<T: PolarsDataType> Default for ChunkedArray<T> {
     fn default() -> Self {
         ChunkedArray {
             field: Arc::new(Field::new("default", DataType::Null)),
             chunks: Default::default(),
@@ -535,43 +536,14 @@
             }
         }
         let arr: LargeStringArray = builder.into();
         unsafe { Self::from_chunks("", vec![Box::new(arr)]) }
     }
 }
 
-pub fn flatten_par<T: Send + Sync + Copy>(bufs: &[&[T]]) -> Vec<T> {
-    let len = bufs.iter().map(|b| b.as_ref().len()).sum();
-    let offsets = bufs
-        .iter()
-        .scan(0usize, |acc, buf| {
-            let out = *acc;
-            *acc += buf.len();
-            Some(out)
-        })
-        .collect::<Vec<_>>();
-
-    let mut out = Vec::with_capacity(len);
-    let out_ptr = unsafe { SyncPtr::new(out.as_mut_ptr()) };
-
-    offsets.into_par_iter().enumerate().for_each(|(i, offset)| {
-        let buf = bufs[i];
-        let ptr: *mut T = out_ptr.get();
-        unsafe {
-            let dst = ptr.add(offset);
-            let src = buf.as_ptr();
-            std::ptr::copy_nonoverlapping(src, dst, buf.len())
-        }
-    });
-    unsafe {
-        out.set_len(len);
-    }
-    out
-}
-
 impl<Ptr> FromParallelIterator<Option<Ptr>> for Utf8Chunked
 where
     Ptr: AsRef<str> + Send + Sync,
 {
     fn from_par_iter<I: IntoParallelIterator<Item = Option<Ptr>>>(iter: I) -> Self {
         let vectors = collect_into_linked_list(iter);
         let vectors = vectors.into_iter().collect::<Vec<_>>();
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/cloud.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/config.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/fmt.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/explode.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/from.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files 20% similar despite different names*

```diff
@@ -4,23 +4,72 @@
 use hashbrown::HashMap;
 use polars_utils::sync::SyncPtr;
 use polars_utils::HashSingle;
 use rayon::prelude::*;
 
 use super::GroupsProxy;
 use crate::datatypes::PlHashMap;
-use crate::frame::groupby::GroupsIdx;
+use crate::frame::groupby::{GroupsIdx, IdxItem};
 use crate::hashing::{
     df_rows_to_hashes_threaded_vertical, this_partition, AsU64, IdBuildHasher, IdxHash,
 };
 use crate::prelude::compare_inner::PartialEqInner;
 use crate::prelude::*;
-use crate::utils::{split_df, CustomIterTools};
+use crate::utils::{flatten, split_df, CustomIterTools};
 use crate::POOL;
 
+fn finish_group_order(mut out: Vec<Vec<IdxItem>>, sorted: bool) -> GroupsProxy {
+    if sorted {
+        // we can just take the first value, no need to flatten
+        let mut out = if out.len() == 1 {
+            out.pop().unwrap()
+        } else {
+            let (cap, offsets) = flatten::cap_and_offsets(&out);
+            // we write (first, all) tuple because of sorting
+            let mut items = Vec::with_capacity(cap);
+            let items_ptr = unsafe { SyncPtr::new(items.as_mut_ptr()) };
+
+            POOL.install(|| {
+                out.into_par_iter()
+                    .zip(offsets)
+                    .for_each(|(mut g, offset)| {
+                        // pre-sort every array
+                        // this will make the final single threaded sort much faster
+                        g.sort_unstable_by_key(|g| g.0);
+
+                        unsafe {
+                            let mut items_ptr: *mut (IdxSize, Vec<IdxSize>) = items_ptr.get();
+                            items_ptr = items_ptr.add(offset);
+
+                            for (i, g) in g.into_iter().enumerate() {
+                                std::ptr::write(items_ptr.add(i), g)
+                            }
+                        }
+                    });
+            });
+            unsafe {
+                items.set_len(cap);
+            }
+            items
+        };
+        out.sort_unstable_by_key(|g| g.0);
+        let mut idx = GroupsIdx::from_iter(out.into_iter());
+        idx.sorted = true;
+        GroupsProxy::Idx(idx)
+    } else {
+        // we can just take the first value, no need to flatten
+        if out.len() == 1 {
+            GroupsProxy::Idx(GroupsIdx::from(out.pop().unwrap()))
+        } else {
+            // flattens
+            GroupsProxy::Idx(GroupsIdx::from(out))
+        }
+    }
+}
+
 fn finish_group_order_vecs(
     mut vecs: Vec<(Vec<IdxSize>, Vec<Vec<IdxSize>>)>,
     sorted: bool,
 ) -> GroupsProxy {
     if sorted {
         if vecs.len() == 1 {
             let (first, all) = vecs.pop().unwrap();
@@ -113,82 +162,149 @@
         idx.sorted = true;
         GroupsProxy::Idx(idx)
     } else {
         GroupsProxy::Idx(hash_tbl.into_values().collect())
     }
 }
 
-pub(crate) fn groupby_threaded_num2<T, I>(
+// giving the slice info to the compiler is much
+// faster than the using an iterator, that's why we
+// have the code duplication
+pub(crate) fn groupby_threaded_slice<T, IntoSlice>(
+    keys: Vec<IntoSlice>,
+    n_partitions: u64,
+    sorted: bool,
+) -> GroupsProxy
+where
+    T: Send + Hash + Eq + Sync + Copy + AsU64,
+    IntoSlice: AsRef<[T]> + Send + Sync,
+{
+    assert!(n_partitions.is_power_of_two());
+
+    // We will create a hashtable in every thread.
+    // We use the hash to partition the keys to the matching hashtable.
+    // Every thread traverses all keys/hashes and ignores the ones that doesn't fall in that partition.
+    let out = POOL.install(|| {
+        (0..n_partitions)
+            .into_par_iter()
+            .map(|thread_no| {
+                let mut hash_tbl: PlHashMap<T, (IdxSize, Vec<IdxSize>)> =
+                    PlHashMap::with_capacity(HASHMAP_INIT_SIZE);
+
+                let mut offset = 0;
+                for keys in &keys {
+                    let keys = keys.as_ref();
+                    let len = keys.len() as IdxSize;
+                    let hasher = hash_tbl.hasher().clone();
+
+                    let mut cnt = 0;
+                    keys.iter().for_each(|k| {
+                        let idx = cnt + offset;
+                        cnt += 1;
+
+                        if this_partition(k.as_u64(), thread_no, n_partitions) {
+                            let hash = hasher.hash_single(k);
+                            let entry = hash_tbl.raw_entry_mut().from_key_hashed_nocheck(hash, k);
+
+                            match entry {
+                                RawEntryMut::Vacant(entry) => {
+                                    let tuples = vec![idx];
+                                    entry.insert_with_hasher(hash, *k, (idx, tuples), |k| {
+                                        hasher.hash_single(k)
+                                    });
+                                }
+                                RawEntryMut::Occupied(mut entry) => {
+                                    let v = entry.get_mut();
+                                    v.1.push(idx);
+                                }
+                            }
+                        }
+                    });
+                    offset += len;
+                }
+                hash_tbl
+                    .into_iter()
+                    .map(|(_k, v)| v)
+                    .collect_trusted::<Vec<_>>()
+            })
+            .collect::<Vec<_>>()
+    });
+    finish_group_order(out, sorted)
+}
+
+pub(crate) fn groupby_threaded_iter<T, I>(
     keys: &[I],
     n_partitions: u64,
     sorted: bool,
 ) -> GroupsProxy
 where
     I: IntoIterator<Item = T> + Send + Sync + Copy,
     I::IntoIter: ExactSizeIterator,
     T: Send + Hash + Eq + Sync + Copy + AsU64,
 {
     assert!(n_partitions.is_power_of_two());
 
     // We will create a hashtable in every thread.
     // We use the hash to partition the keys to the matching hashtable.
     // Every thread traverses all keys/hashes and ignores the ones that doesn't fall in that partition.
-    let v = POOL.install(|| {
+    let out = POOL.install(|| {
         (0..n_partitions)
             .into_par_iter()
             .map(|thread_no| {
-                let mut hash_tbl: PlHashMap<T, IdxSize> =
+                let mut hash_tbl: PlHashMap<T, (IdxSize, Vec<IdxSize>)> =
                     PlHashMap::with_capacity(HASHMAP_INIT_SIZE);
-                let mut first_vals = Vec::with_capacity(HASHMAP_INIT_SIZE);
-                let mut all_vals = Vec::with_capacity(HASHMAP_INIT_SIZE);
 
                 let mut offset = 0;
                 for keys in keys {
                     let keys = keys.into_iter();
                     let len = keys.len() as IdxSize;
                     let hasher = hash_tbl.hasher().clone();
 
                     let mut cnt = 0;
                     keys.for_each(|k| {
-                        let row_idx = cnt + offset;
+                        let idx = cnt + offset;
                         cnt += 1;
 
                         if this_partition(k.as_u64(), thread_no, n_partitions) {
                             let hash = hasher.hash_single(k);
                             let entry = hash_tbl.raw_entry_mut().from_key_hashed_nocheck(hash, &k);
 
                             match entry {
                                 RawEntryMut::Vacant(entry) => {
-                                    let offset_idx = first_vals.len() as IdxSize;
-
-                                    let tuples = vec![row_idx];
-                                    all_vals.push(tuples);
-                                    first_vals.push(row_idx);
-
-                                    entry.insert_with_hasher(hash, k, offset_idx, |k| {
+                                    let tuples = vec![idx];
+                                    entry.insert_with_hasher(hash, k, (idx, tuples), |k| {
                                         hasher.hash_single(k)
                                     });
                                 }
-                                RawEntryMut::Occupied(entry) => {
-                                    let offset_idx = *entry.get();
-                                    unsafe {
-                                        let buf = all_vals.get_unchecked_mut(offset_idx as usize);
-                                        buf.push(row_idx)
-                                    }
+                                RawEntryMut::Occupied(mut entry) => {
+                                    let v = entry.get_mut();
+                                    v.1.push(idx);
                                 }
                             }
                         }
                     });
                     offset += len;
                 }
-                (first_vals, all_vals)
+                // iterating the hash tables locally
+                // was faster than iterating in the materialization phase directly
+                // the proper end vec. I believe this is because the hash-table
+                // currently is local to the thread so in hot cache
+                // So we first collect into a tight vec and then do a second
+                // materialization run
+                // this is also faster than the index-map approach where we
+                // directly locally store to a vec at the cost of an extra
+                // indirection
+                hash_tbl
+                    .into_iter()
+                    .map(|(_k, v)| v)
+                    .collect_trusted::<Vec<_>>()
             })
             .collect::<Vec<_>>()
     });
-    finish_group_order_vecs(v, sorted)
+    finish_group_order(out, sorted)
 }
 
 /// Utility function used as comparison function in the hashmap.
 /// The rationale is that equality is an AND operation and therefore its probability of success
 /// declines rapidly with the number of keys. Instead of first copying an entire row from both
 /// sides and then do the comparison, we do the comparison value by value catching early failures
 /// eagerly.
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #[cfg(feature = "groupby_list")]
 use polars_arrow::kernels::list_bytes_iter::numeric_list_bytes_iter;
 use polars_arrow::kernels::sort_partition::{create_clean_partitions, partition_to_groups};
 use polars_arrow::prelude::*;
-use polars_utils::{flatten, HashSingle};
+use polars_utils::HashSingle;
 
 use super::*;
 use crate::config::verbose;
 use crate::utils::_split_offsets;
+use crate::utils::flatten::flatten_par;
 
 /// Used to create the tuples for a groupby operation.
 pub trait IntoGroupsProxy {
     /// Create the tuples need for a groupby operation.
     ///     * The first value in the tuple is the first index of the group.
     ///     * The second value in the tuple is are the indexes of the groups including the first value.
     fn group_tuples(&self, _multithreaded: bool, _sorted: bool) -> PolarsResult<GroupsProxy> {
@@ -34,18 +35,18 @@
 
         // use the arrays as iterators
         if ca.null_count() == 0 {
             let keys = ca
                 .downcast_iter()
                 .map(|arr| arr.values().as_slice())
                 .collect::<Vec<_>>();
-            groupby_threaded_num2(&keys, n_partitions, sorted)
+            groupby_threaded_slice(keys, n_partitions, sorted)
         } else {
             let keys = ca.downcast_iter().collect::<Vec<_>>();
-            groupby_threaded_num2(&keys, n_partitions, sorted)
+            groupby_threaded_iter(&keys, n_partitions, sorted)
         }
     } else if !ca.has_validity() {
         groupby(ca.into_no_null_iter(), sorted)
     } else {
         groupby(ca.into_iter(), sorted)
     }
 }
@@ -115,15 +116,15 @@
                             };
 
                             partition_to_groups(part, 0, false, offset)
                         }
                     })
                 })
                 .collect::<Vec<_>>();
-            flatten(&groups, None)
+            flatten_par(&groups)
         } else {
             partition_to_groups(values, null_count as IdxSize, nulls_first, 0)
         };
         groups
     }
 }
 
@@ -267,15 +268,15 @@
                                 }
                             })
                             .collect_trusted::<Vec<_>>()
                     })
                     .collect::<Vec<_>>()
             });
             let byte_hashes = byte_hashes.iter().collect::<Vec<_>>();
-            groupby_threaded_num2(&byte_hashes, n_partitions as u64, sorted)
+            groupby_threaded_slice(byte_hashes, n_partitions as u64, sorted)
         } else {
             let byte_hashes = self
                 .into_iter()
                 .map(|opt_b| {
                     let hash = match opt_b {
                         Some(s) => hb.hash_single(s),
                         None => null_h,
@@ -334,16 +335,16 @@
                         .into_par_iter()
                         .map(|(offset, len)| {
                             let ca = self.slice(offset as i64, len);
                             arr_to_hashes(&ca)
                         })
                         .collect::<PolarsResult<Vec<_>>>()?;
                     let bytes_hashes = bytes_hashes.iter().collect::<Vec<_>>();
-                    Ok(groupby_threaded_num2(
-                        &bytes_hashes,
+                    Ok(groupby_threaded_slice(
+                        bytes_hashes,
                         n_partitions as u64,
                         sorted,
                     ))
                 });
                 groups
             } else {
                 let hashes = arr_to_hashes(self)?;
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 use polars_arrow::utils::CustomIterTools;
 use polars_utils::sync::SyncPtr;
 use rayon::iter::plumbing::UnindexedConsumer;
 use rayon::prelude::*;
 
 use crate::prelude::*;
-use crate::utils::{slice_slice, NoNull};
+use crate::utils::{flatten, slice_slice, NoNull};
 use crate::POOL;
 
 /// Indexes of the groups, the first index is stored separately.
 /// this make sorting fast.
 #[derive(Debug, Clone, PartialEq, Eq, Default)]
 pub struct GroupsIdx {
     pub(crate) sorted: bool,
@@ -93,14 +93,56 @@
             sorted: false,
             first: global_first,
             all: global_all,
         }
     }
 }
 
+impl From<Vec<Vec<IdxItem>>> for GroupsIdx {
+    fn from(v: Vec<Vec<IdxItem>>) -> Self {
+        // single threaded flatten: 10% faster than `iter().flatten().collect()
+        // this is the multi-threaded impl of that
+        let (cap, offsets) = flatten::cap_and_offsets(&v);
+        let mut first = Vec::with_capacity(cap);
+        let first_ptr = first.as_ptr() as usize;
+        let mut all = Vec::with_capacity(cap);
+        let all_ptr = all.as_ptr() as usize;
+
+        POOL.install(|| {
+            v.into_par_iter()
+                .zip(offsets)
+                .for_each(|(mut inner, offset)| {
+                    unsafe {
+                        let first = (first_ptr as *const IdxSize as *mut IdxSize).add(offset);
+                        let all = (all_ptr as *const Vec<IdxSize> as *mut Vec<IdxSize>).add(offset);
+
+                        let inner_ptr = inner.as_mut_ptr();
+                        for i in 0..inner.len() {
+                            let (first_val, vals) = std::ptr::read(inner_ptr.add(i));
+                            std::ptr::write(first.add(i), first_val);
+                            std::ptr::write(all.add(i), vals);
+                        }
+                        // set len to 0 so that the contents will not get dropped
+                        // they are moved to `first` and `all`
+                        inner.set_len(0);
+                    }
+                });
+        });
+        unsafe {
+            all.set_len(cap);
+            first.set_len(cap);
+        }
+        GroupsIdx {
+            sorted: false,
+            first,
+            all,
+        }
+    }
+}
+
 impl GroupsIdx {
     pub fn new(first: Vec<IdxSize>, all: Vec<Vec<IdxSize>>, sorted: bool) -> Self {
         Self { sorted, first, all }
     }
 
     pub fn sort(&mut self) {
         let mut idx = 0;
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-use polars_utils::flatten;
-
 use super::single_keys::create_probe_table;
 use super::*;
 use crate::frame::hash_join::single_keys::probe_to_offsets;
+use crate::utils::flatten::flatten_par;
 
 #[cfg(feature = "chunked_ids")]
 unsafe fn apply_mapping(idx: Vec<IdxSize>, chunk_mapping: &[ChunkId]) -> Vec<ChunkId> {
     idx.iter()
         .map(|idx| *chunk_mapping.get_unchecked(*idx as usize))
         .collect()
 }
@@ -54,49 +53,49 @@
     #[cfg(feature = "chunked_ids")]
     {
         let left = if result[0].0.is_left() {
             let lefts = result
                 .iter()
                 .map(|join_id| join_id.0.as_ref().left().unwrap())
                 .collect::<Vec<_>>();
-            let lefts = flatten(&lefts, None);
+            let lefts = flatten_par(&lefts);
             JoinIds::Left(lefts)
         } else {
             let lefts = result
                 .iter()
                 .map(|join_id| join_id.0.as_ref().right().unwrap())
                 .collect::<Vec<_>>();
-            let lefts = flatten(&lefts, None);
+            let lefts = flatten_par(&lefts);
             JoinIds::Right(lefts)
         };
 
         let right = if result[0].1.is_left() {
             let rights = result
                 .iter()
                 .map(|join_id| join_id.1.as_ref().left().unwrap())
                 .collect::<Vec<_>>();
-            let rights = flatten(&rights, None);
+            let rights = flatten_par(&rights);
             JoinOptIds::Left(rights)
         } else {
             let rights = result
                 .iter()
                 .map(|join_id| join_id.1.as_ref().right().unwrap())
                 .collect::<Vec<_>>();
-            let rights = flatten(&rights, None);
+            let rights = flatten_par(&rights);
             JoinOptIds::Right(rights)
         };
 
         (left, right)
     }
     #[cfg(not(feature = "chunked_ids"))]
     {
         let lefts = result.iter().map(|join_id| &join_id.0).collect::<Vec<_>>();
         let rights = result.iter().map(|join_id| &join_id.1).collect::<Vec<_>>();
-        let lefts = flatten(&lefts, None);
-        let rights = flatten(&rights, None);
+        let lefts = flatten_par(&lefts);
+        let rights = flatten_par(&rights);
         (lefts, rights)
     }
 }
 
 pub(super) fn hash_join_tuples_left<T, IntoSlice>(
     probe: Vec<IntoSlice>,
     build: Vec<IntoSlice>,
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #[cfg(feature = "performant")]
 use polars_arrow::kernels::sorted_join;
-#[cfg(feature = "performant")]
-use polars_utils::flatten;
 
 use super::*;
 #[cfg(feature = "performant")]
 use crate::utils::_split_offsets;
+#[cfg(feature = "performant")]
+use crate::utils::flatten::flatten_par;
 
 #[cfg(feature = "performant")]
 fn par_sorted_merge_left_impl<T>(
     s_left: &ChunkedArray<T>,
     s_right: &ChunkedArray<T>,
 ) -> (Vec<IdxSize>, Vec<Option<IdxSize>>)
 where
@@ -29,15 +29,15 @@
             let slice_left = &slice_left[offset..offset + len];
             sorted_join::left::join(slice_left, slice_right, offset as IdxSize)
         })
         .collect::<Vec<_>>();
     let lefts = indexes.iter().map(|t| &t.0).collect::<Vec<_>>();
     let rights = indexes.iter().map(|t| &t.1).collect::<Vec<_>>();
 
-    (flatten(&lefts, None), flatten(&rights, None))
+    (flatten_par(&lefts), flatten_par(&rights))
 }
 
 #[cfg(feature = "performant")]
 pub(super) fn par_sorted_merge_left(
     s_left: &Series,
     s_right: &Series,
 ) -> (Vec<IdxSize>, Vec<Option<IdxSize>>) {
@@ -102,15 +102,15 @@
             let slice_left = &slice_left[offset..offset + len];
             sorted_join::inner::join(slice_left, slice_right, offset as IdxSize)
         })
         .collect::<Vec<_>>();
     let lefts = indexes.iter().map(|t| &t.0).collect::<Vec<_>>();
     let rights = indexes.iter().map(|t| &t.1).collect::<Vec<_>>();
 
-    (flatten(&lefts, None), flatten(&rights, None))
+    (flatten_par(&lefts), flatten_par(&rights))
 }
 
 #[cfg(feature = "performant")]
 pub(super) fn par_sorted_merge_inner_no_nulls(
     s_left: &Series,
     s_right: &Series,
 ) -> (Vec<IdxSize>, Vec<IdxSize>) {
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 use smartstring::alias::String as SmartString;
 
 use crate::frame::groupby::GroupsIndicator;
 #[cfg(feature = "row_hash")]
 use crate::hashing::df_rows_to_hashes_threaded_vertical;
+use crate::prelude::min_max_binary::min_max_binary_series;
 use crate::prelude::sort::{argsort_multiple_row_fmt, prepare_arg_sort};
 use crate::series::IsSorted;
 use crate::POOL;
 
 #[derive(Copy, Clone, Debug)]
 pub enum NullStrategy {
     Ignore,
@@ -2780,18 +2781,15 @@
 
         Ok(DataFrame::new_no_checks(columns))
     }
 
     /// Aggregate the column horizontally to their min values.
     #[cfg(feature = "zip_with")]
     pub fn hmin(&self) -> PolarsResult<Option<Series>> {
-        let min_fn = |acc: &Series, s: &Series| {
-            let mask = acc.lt(s)? & acc.is_not_null() | s.is_null();
-            acc.zip_with(&mask, s)
-        };
+        let min_fn = |acc: &Series, s: &Series| min_max_binary_series(acc, s, true);
 
         match self.columns.len() {
             0 => Ok(None),
             1 => Ok(Some(self.columns[0].clone())),
             2 => min_fn(&self.columns[0], &self.columns[1]).map(Some),
             _ => {
                 // the try_reduce_with is a bit slower in parallelism,
@@ -2809,18 +2807,15 @@
             }
         }
     }
 
     /// Aggregate the column horizontally to their max values.
     #[cfg(feature = "zip_with")]
     pub fn hmax(&self) -> PolarsResult<Option<Series>> {
-        let max_fn = |acc: &Series, s: &Series| {
-            let mask = acc.gt(s)? & acc.is_not_null() | s.is_null();
-            acc.zip_with(&mask, s)
-        };
+        let max_fn = |acc: &Series, s: &Series| min_max_binary_series(acc, s, false);
 
         match self.columns.len() {
             0 => Ok(None),
             1 => Ok(Some(self.columns[0].clone())),
             2 => max_fn(&self.columns[0], &self.columns[1]).map(Some),
             _ => {
                 // the try_reduce_with is a bit slower in parallelism,
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/functions.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/lib.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/named_from.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/named_from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/prelude.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/schema.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/schema.rs`

 * *Files 5% similar despite different names*

```diff
@@ -238,14 +238,18 @@
     ///
     /// If `index` is inbounds, returns `Some((&name, &dtype))`, else `None`. See
     /// [`get_at_index_mut`][Self::get_at_index_mut] for a mutable version.
     pub fn get_at_index(&self, index: usize) -> Option<(&SmartString, &DataType)> {
         self.inner.get_index(index)
     }
 
+    pub fn try_get_at_index(&self, index: usize) -> PolarsResult<(&SmartString, &DataType)> {
+        self.inner.get_index(index).ok_or_else(|| polars_err!(ComputeError: "index {index} out of bounds with 'schema' of len: {}", self.len()))
+    }
+
     /// Get mutable references to the name and dtype of the field at `index`
     ///
     /// If `index` is inbounds, returns `Some((&mut name, &mut dtype))`, else `None`. See
     /// [`get_at_index`][Self::get_at_index] for an immutable version.
     pub fn get_at_index_mut(&mut self, index: usize) -> Option<(&mut SmartString, &mut DataType)> {
         self.inner.get_index_mut(index)
     }
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/serde/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/serde/series.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/any_value.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/comparison.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/from.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/into.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/iterator.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/series/unstable.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/testing.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/utils/flatten.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/utils/flatten.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+use polars_utils::sync::SyncPtr;
+
 use super::*;
 
 pub(super) fn flatten_df(df: &DataFrame) -> impl Iterator<Item = DataFrame> + '_ {
     df.iter_chunks_physical().flat_map(|chunk| {
         let df = DataFrame::new_no_checks(
             df.iter()
                 .zip(chunk.into_arrays())
@@ -43,7 +45,47 @@
             let out = *acc;
             *acc += v.len();
             Some(out)
         })
         .collect::<Vec<_>>();
     (cap, offsets)
 }
+
+pub fn flatten_par<T: Send + Sync + Copy, S: AsRef<[T]>>(bufs: &[S]) -> Vec<T> {
+    let mut len = 0;
+    let mut offsets = Vec::with_capacity(bufs.len());
+    let bufs = bufs
+        .iter()
+        .map(|s| {
+            offsets.push(len);
+            let slice = s.as_ref();
+            len += slice.len();
+            slice
+        })
+        .collect::<Vec<_>>();
+    flatten_par_impl(&bufs, len, offsets)
+}
+
+fn flatten_par_impl<T: Send + Sync + Copy>(
+    bufs: &[&[T]],
+    len: usize,
+    offsets: Vec<usize>,
+) -> Vec<T> {
+    let mut out = Vec::with_capacity(len);
+    let out_ptr = unsafe { SyncPtr::new(out.as_mut_ptr()) };
+
+    POOL.install(|| {
+        offsets.into_par_iter().enumerate().for_each(|(i, offset)| {
+            let buf = bufs[i];
+            let ptr: *mut T = out_ptr.get();
+            unsafe {
+                let dst = ptr.add(offset);
+                let src = buf.as_ptr();
+                std::ptr::copy_nonoverlapping(src, dst, buf.len())
+            }
+        })
+    });
+    unsafe {
+        out.set_len(len);
+    }
+    out
+}
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/utils/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/utils/series.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/utils/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/get.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/null.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/conversion.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/data_types.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/index.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/slice.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/time_zone.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/time_zone.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-arrow/src/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-arrow/src/utils.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::ops::BitAnd;
+use std::ops::{BitAnd, BitOr};
 
 use arrow::array::PrimitiveArray;
 use arrow::bitmap::Bitmap;
 use arrow::types::NativeType;
 
 use crate::trusted_len::{FromIteratorReversed, PushUnchecked, TrustedLen};
 
@@ -46,22 +46,28 @@
 {
     #[inline]
     fn next_back(&mut self) -> Option<Self::Item> {
         self.iter.next_back()
     }
 }
 
-pub fn combine_validities(opt_l: Option<&Bitmap>, opt_r: Option<&Bitmap>) -> Option<Bitmap> {
+pub fn combine_validities_and(opt_l: Option<&Bitmap>, opt_r: Option<&Bitmap>) -> Option<Bitmap> {
     match (opt_l, opt_r) {
         (Some(l), Some(r)) => Some(l.bitand(r)),
         (None, Some(r)) => Some(r.clone()),
         (Some(l), None) => Some(l.clone()),
         (None, None) => None,
     }
 }
+pub fn combine_validities_or(opt_l: Option<&Bitmap>, opt_r: Option<&Bitmap>) -> Option<Bitmap> {
+    match (opt_l, opt_r) {
+        (Some(l), Some(r)) => Some(l.bitor(r)),
+        _ => None,
+    }
+}
 unsafe impl<I, J> arrow::trusted_len::TrustedLen for TrustMyLength<I, J> where I: Iterator<Item = J> {}
 
 pub trait CustomIterTools: Iterator {
     fn fold_first_<F>(mut self, f: F) -> Option<Self::Item>
     where
         Self: Sized,
         F: FnMut(Self::Item, Self::Item) -> Self::Item,
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -52,18 +52,18 @@
 
 [dependencies]
 ahash= "0.8"
 async-trait = { version = "0.1.59", optional = true }
 bytes = "1.3.0"
 chrono = { version = "0.4", default-features = false, features = ["std"], optional = true }
 chrono-tz = { version = "0.8.1", optional = true }
-dirs = "5.0"
 fast-float = { version = "0.2.0", optional = true }
 flate2 = { version = "1", optional = true, default-features = false }
 futures = { version = "0.3.25", optional = true }
+home = "0.5.4"
 lexical = { version = "6", optional = true, default-features = false, features = ["std", "parse-integers"] }
 lexical-core = { version = "0.8", optional = true }
 memchr= "2"
 memmap = { package = "memmap2", version = "0.5.2", optional = true }
 num-traits= "0.2"
 object_store = { version = "0.5.3", default-features = false, optional = true }
 once_cell = "1"
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/avro/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/avro/read.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/avro/write.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/parser.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/read.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/write.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/write.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/json.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/lib.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/mmap.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ndjson_core/buffer.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ndjson_core/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/ndjson_core/ndjson.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/ndjson_core/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/read.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/parquet/write.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/partition.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/predicates.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/prelude.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-io/src/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-io/src/utils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use std::path::{Path, PathBuf};
 
-use dirs::home_dir;
+use home::home_dir;
 use polars_core::frame::DataFrame;
 use polars_core::prelude::*;
 
 #[cfg(any(
     feature = "ipc",
     feature = "ipc_streaming",
     feature = "parquet",
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/approx_unique.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use arrow::array::{Array, PrimitiveArray};
 use num::NumCast;
 use polars_arrow::prelude::ArrayRef;
-use polars_arrow::utils::combine_validities;
+use polars_arrow::utils::combine_validities_and;
 use polars_core::datatypes::PolarsNumericType;
 use polars_core::export::num;
 use polars_core::prelude::*;
 #[cfg(feature = "dtype-struct")]
 use polars_core::series::arithmetic::_struct_arithmetic;
 use polars_core::utils::align_chunks_binary;
 use polars_core::with_match_physical_numeric_polars_type;
@@ -35,15 +35,15 @@
             .as_slice()
             .iter()
             .copied()
             .zip(b.values().as_slice().iter().copied())
             .map(|(a, b)| floor_div_element(a, b))
             .collect::<Vec<_>>();
 
-        let validity = combine_validities(a.validity(), b.validity());
+        let validity = combine_validities_and(a.validity(), b.validity());
 
         PrimitiveArray::new(a.data_type().clone(), values.into(), validity)
     } else {
         let iter = a
             .into_iter()
             .zip(b.into_iter())
             .map(|(opt_a, opt_b)| match (opt_a, opt_b) {
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/Cargo.toml` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/LICENSE` & `polars_lts_cpu-0.17.8/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
             &[T::Native],
             Duration,
             Duration,
             &[i64],
             ClosedWindow,
             TimeUnit,
             Option<&TimeZone>,
-        ) -> ArrayRef,
+        ) -> PolarsResult<ArrayRef>,
     >,
 ) -> PolarsResult<Series>
 where
     T: PolarsNumericType,
 {
     if ca.is_empty() {
         return Ok(Series::new_empty(ca.name(), ca.dtype()));
@@ -249,30 +249,30 @@
 
     let arr = ca.downcast_iter().next().unwrap();
     // "5i" is a window size of 5, e.g. fixed
     let arr = if options.window_size.parsed_int {
         let options: RollingOptionsFixedWindow = options.into();
         check_input(options.window_size, options.min_periods)?;
 
-        match ca.null_count() {
+        Ok(match ca.null_count() {
             0 => rolling_agg_fn(
                 arr.values().as_slice(),
                 options.window_size,
                 options.min_periods,
                 options.center,
                 options.weights.as_deref(),
             ),
             _ => rolling_agg_fn_nulls(
                 arr,
                 options.window_size,
                 options.min_periods,
                 options.center,
                 options.weights.as_deref(),
             ),
-        }
+        })
     } else {
         if arr.null_count() > 0 {
             panic!("'rolling by' not yet supported for series with null values, consider using 'groupby_rolling'")
         }
         let values = arr.values().as_slice();
         let duration = options.window_size;
         let tu = options.tu.unwrap();
@@ -281,10 +281,10 @@
         let mut offset = duration;
         offset.negative = true;
         let func = rolling_agg_fn_dynamic.expect(
             "'rolling by' not yet supported for this expression, consider using 'groupby_rolling'",
         );
 
         func(values, duration, offset, by, closed_window, tu, options.tz)
-    };
+    }?;
     Series::try_from((ca.name(), arr))
 }
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files 4% similar despite different names*

```diff
@@ -4,54 +4,63 @@
 use chrono_tz::Tz;
 use polars_arrow::kernels::rolling::no_nulls::{self, RollingAggWindowNoNulls};
 use polars_core::export::num;
 
 use super::*;
 
 // Use an aggregation window that maintains the state
-pub(crate) fn rolling_apply_agg_window<'a, Agg, T, O>(values: &'a [T], offsets: O) -> ArrayRef
+pub(crate) fn rolling_apply_agg_window<'a, Agg, T, O>(
+    values: &'a [T],
+    offsets: O,
+) -> PolarsResult<ArrayRef>
 where
     // items (offset, len) -> so offsets are offset, offset + len
     Agg: RollingAggWindowNoNulls<'a, T>,
-    O: Iterator<Item = (IdxSize, IdxSize)> + TrustedLen,
+    O: Iterator<Item = PolarsResult<(IdxSize, IdxSize)>> + TrustedLen,
     T: Debug + IsFloat + NativeType,
 {
     if values.is_empty() {
         let out: Vec<T> = vec![];
-        return Box::new(PrimitiveArray::new(T::PRIMITIVE.into(), out.into(), None));
+        return Ok(Box::new(PrimitiveArray::new(
+            T::PRIMITIVE.into(),
+            out.into(),
+            None,
+        )));
     }
     // start with a dummy index, will be overwritten on first iteration.
     let mut agg_window = Agg::new(values, 0, 0);
 
     let out = offsets
-        .map(|(start, len)| {
-            let end = start + len;
-
-            if start == end {
-                None
-            } else {
-                // safety:
-                // we are in bounds
-                Some(unsafe { agg_window.update(start as usize, end as usize) })
-            }
+        .map(|result| {
+            result.map(|(start, len)| {
+                let end = start + len;
+
+                if start == end {
+                    None
+                } else {
+                    // safety:
+                    // we are in bounds
+                    Some(unsafe { agg_window.update(start as usize, end as usize) })
+                }
+            })
         })
-        .collect::<PrimitiveArray<T>>();
+        .collect::<PolarsResult<PrimitiveArray<T>>>()?;
 
-    Box::new(out)
+    Ok(Box::new(out))
 }
 
 pub(crate) fn rolling_min<T>(
     values: &[T],
     period: Duration,
     offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType + PartialOrd + IsFloat + Bounded + NumCast + Mul<Output = T>,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
         Some(tz) => match tz.parse::<Tz>() {
             Ok(tz) => groupby_values_iter(period, offset, time, closed_window, tu, Some(tz)),
@@ -76,15 +85,15 @@
     values: &[T],
     period: Duration,
     offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType + PartialOrd + IsFloat + Bounded + NumCast + Mul<Output = T>,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
         Some(tz) => match tz.parse::<Tz>() {
             Ok(tz) => groupby_values_iter(period, offset, time, closed_window, tu, Some(tz)),
@@ -109,15 +118,15 @@
     values: &[T],
     period: Duration,
     offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType + std::iter::Sum + NumCast + Mul<Output = T> + AddAssign + SubAssign + IsFloat,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
         Some(tz) => match tz.parse::<Tz>() {
             Ok(tz) => groupby_values_iter(period, offset, time, closed_window, tu, Some(tz)),
@@ -142,15 +151,15 @@
     values: &[T],
     period: Duration,
     offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType + Float + std::iter::Sum<T> + SubAssign + AddAssign + IsFloat,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
         Some(tz) => match tz.parse::<Tz>() {
             Ok(tz) => groupby_values_iter(period, offset, time, closed_window, tu, Some(tz)),
@@ -175,15 +184,15 @@
     values: &[T],
     period: Duration,
     offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType + Float + std::iter::Sum<T> + SubAssign + AddAssign + IsFloat,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
         Some(tz) => match tz.parse::<Tz>() {
             Ok(tz) => groupby_values_iter(period, offset, time, closed_window, tu, Some(tz)),
@@ -208,15 +217,15 @@
     values: &[T],
     period: Duration,
     offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType
         + Float
         + IsFloat
         + std::iter::Sum
         + AddAssign
         + SubAssign
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/date_range.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 use polars_arrow::time_zone::PolarsTimeZone;
 use polars_arrow::utils::CustomIterTools;
 use polars_core::export::rayon::prelude::*;
 use polars_core::frame::groupby::GroupsProxy;
 use polars_core::prelude::*;
 use polars_core::series::IsSorted;
 use polars_core::utils::ensure_sorted_arg;
+use polars_core::utils::flatten::flatten_par;
 use polars_core::POOL;
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 use smartstring::alias::String as SmartString;
 
 use crate::prelude::*;
 
@@ -102,14 +103,15 @@
 impl Wrap<&DataFrame> {
     fn groupby_rolling(
         &self,
         by: Vec<Series>,
         options: &RollingGroupOptions,
     ) -> PolarsResult<(Series, Vec<Series>, GroupsProxy)> {
         let time = self.0.column(&options.index_column)?.clone();
+        ensure_sorted_arg(&time);
         let time_type = time.dtype();
 
         polars_ensure!(time.null_count() == 0, ComputeError: "null values in dynamic groupby not supported, fill nulls.");
 
         use DataType::*;
         let (dt, tu, tz): (Series, TimeUnit, Option<TimeZone>) = match time_type {
             Datetime(tu, tz) => (time.clone(), *tu, tz.clone()),
@@ -177,14 +179,15 @@
                     && (options.every.parsed_int || options.every.is_zero())
                     && (options.period.parsed_int || options.period.is_zero())),
                 ComputeError: "you cannot combine time durations like '2h' with integer durations like '3i'"
             )
         }
 
         let time = self.0.column(&options.index_column)?.rechunk();
+        ensure_sorted_arg(&time);
         let time_type = time.dtype();
 
         polars_ensure!(time.null_count() == 0, ComputeError: "null values in dynamic groupby not supported, fill nulls.");
 
         use DataType::*;
         let (dt, tu) = match time_type {
             Datetime(tu, _) => (time.clone(), *tu),
@@ -235,17 +238,15 @@
         tu: TimeUnit,
         time_type: &DataType,
     ) -> PolarsResult<(Series, Vec<Series>, GroupsProxy)> {
         polars_ensure!(!options.every.negative, ComputeError: "'every' argument must be positive");
         if dt.is_empty() {
             return dt.cast(time_type).map(|s| (s, by, GroupsProxy::default()));
         }
-        ensure_sorted_arg(&dt);
 
-        let sorted_set = matches!(dt.is_sorted_flag(), IsSorted::Ascending);
         // a requirement for the index
         // so we can set this such that downstream code has this info
         dt.set_sorted_flag(IsSorted::Ascending);
 
         let w = Window::new(options.every, options.period, options.offset);
         let dt = dt.datetime().unwrap();
         let tz = dt.time_zone();
@@ -276,17 +277,14 @@
                 }
                 _ => unreachable!(),
             };
 
         let groups = if by.is_empty() {
             let vals = dt.downcast_iter().next().unwrap();
             let ts = vals.values().as_slice();
-            if !sorted_set {
-                partially_check_sorted(ts);
-            }
             let (groups, lower, upper) = groupby_windows(
                 w,
                 ts,
                 options.closed_window,
                 tu,
                 tz,
                 include_lower_bound,
@@ -459,35 +457,34 @@
         dt: Series,
         by: Vec<Series>,
         options: &RollingGroupOptions,
         tu: TimeUnit,
         tz: Option<impl PolarsTimeZone>,
         time_type: &DataType,
     ) -> PolarsResult<(Series, Vec<Series>, GroupsProxy)> {
-        ensure_sorted_arg(&dt);
         let mut dt = dt.rechunk();
         // a requirement for the index
         // so we can set this such that downstream code has this info
         dt.set_sorted_flag(IsSorted::Ascending);
 
         let groups = if by.is_empty() {
             let dt = dt.datetime().unwrap();
             let vals = dt.downcast_iter().next().unwrap();
             let ts = vals.values().as_slice();
-            GroupsProxy::Slice {
+            PolarsResult::Ok(GroupsProxy::Slice {
                 groups: groupby_values(
                     options.period,
                     options.offset,
                     ts,
                     options.closed_window,
                     tu,
                     tz,
-                ),
+                )?,
                 rolling: true,
-            }
+            })
         } else {
             let groups = self
                 .0
                 .groupby_with_series(by.clone(), true, true)?
                 .take_groups();
 
             // we keep a local copy, as we are reordering on next operation.
@@ -498,58 +495,59 @@
 
             // continue determining the rolling indexes.
 
             POOL.install(|| match groups {
                 GroupsProxy::Idx(groups) => {
                     let idx = groups
                         .par_iter()
-                        .flat_map(|base_g| {
+                        .map(|base_g| {
                             let dt = unsafe { dt_local.take_unchecked(base_g.1.into()) };
                             let vals = dt.downcast_iter().next().unwrap();
                             let ts = vals.values().as_slice();
                             let sub_groups = groupby_values(
                                 options.period,
                                 options.offset,
                                 ts,
                                 options.closed_window,
                                 tu,
                                 tz.clone(),
-                            );
-                            update_subgroups_idx(&sub_groups, base_g)
+                            )?;
+                            Ok(update_subgroups_idx(&sub_groups, base_g))
                         })
-                        .collect();
+                        .collect::<PolarsResult<Vec<_>>>()?;
 
-                    GroupsProxy::Idx(idx)
+                    Ok(GroupsProxy::Idx(GroupsIdx::from(idx)))
                 }
                 GroupsProxy::Slice { groups, .. } => {
                     let slice_groups = groups
                         .par_iter()
-                        .flat_map(|base_g| {
+                        .map(|base_g| {
                             let dt = dt_local.slice(base_g[0] as i64, base_g[1] as usize);
                             let vals = dt.downcast_iter().next().unwrap();
                             let ts = vals.values().as_slice();
                             let sub_groups = groupby_values(
                                 options.period,
                                 options.offset,
                                 ts,
                                 options.closed_window,
                                 tu,
                                 tz.clone(),
-                            );
-                            update_subgroups_slice(&sub_groups, *base_g)
+                            )?;
+                            Ok(update_subgroups_slice(&sub_groups, *base_g))
                         })
-                        .collect();
+                        .collect::<PolarsResult<Vec<_>>>()?;
 
-                    GroupsProxy::Slice {
+                    let slice_groups = flatten_par(&slice_groups);
+                    Ok(GroupsProxy::Slice {
                         groups: slice_groups,
                         rolling: false,
-                    }
+                    })
                 }
             })
-        };
+        }?;
 
         let dt = dt.cast(time_type).unwrap();
 
         Ok((dt, by, groups))
     }
 }
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/lib.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 #![cfg_attr(docsrs, feature(doc_auto_cfg))]
 pub mod chunkedarray;
 mod date_range;
 mod groupby;
+mod month_end;
+mod month_start;
 pub mod prelude;
 mod round;
 pub mod series;
 mod truncate;
 mod upsample;
 mod utils;
 mod windows;
 
 pub use date_range::*;
 #[cfg(any(feature = "dtype-date", feature = "dtype-datetime"))]
 pub use groupby::dynamic::*;
+pub use month_end::*;
+pub use month_start::*;
 pub use round::*;
 pub use truncate::*;
 pub use upsample::*;
 pub use windows::calendar::date_range as date_range_vec;
 pub use windows::duration::Duration;
 pub use windows::groupby::ClosedWindow;
 pub use windows::window::Window;
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/round.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/_trait.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/series/mod.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/truncate.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/upsample.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/upsample.rs`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     /// - 1ms   (1 millisecond)
     /// - 1s    (1 second)
     /// - 1m    (1 minute)
     /// - 1h    (1 hour)
     /// - 1d    (1 day)
     /// - 1w    (1 week)
     /// - 1mo   (1 calendar month)
+    /// - 1mo_saturating (calendar month, but "saturates" to the last day of the month
+    ///   instead of erroring. For example, 2022-01-29 plus `'1mo_saturating'` goes to
+    ///   2022-02-28)
     /// - 1y    (1 calendar year)
     /// - 1i    (1 index count)
     /// Or combine them:
     /// "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
     fn upsample<I: IntoVec<String>>(
         &self,
         by: I,
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/utils.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/duration.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 use serde::{Deserialize, Serialize};
 
 use super::calendar::{
     NS_DAY, NS_HOUR, NS_MICROSECOND, NS_MILLISECOND, NS_MINUTE, NS_SECOND, NS_WEEK,
 };
 #[cfg(feature = "timezones")]
 use crate::utils::{localize_datetime, unlocalize_datetime};
+use crate::windows::calendar::{is_leap_year, last_day_of_month};
 
 #[derive(Copy, Clone, Debug, Eq, PartialEq, Hash)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 pub struct Duration {
     // the number of months for the duration
     months: i64,
     // the number of weeks for the duration
@@ -33,14 +34,17 @@
     days: i64,
     // the number of nanoseconds for the duration
     nsecs: i64,
     // indicates if the duration is negative
     pub(crate) negative: bool,
     // indicates if an integer string was passed. e.g. "2i"
     pub parsed_int: bool,
+    // indicates if a '1mo' offset to a non-existent date (e.g. 2022-02-29)
+    // should saturate to 2022-02-28 (as opposed to erroring)
+    pub(crate) saturating_months: Option<bool>,
 }
 
 impl PartialOrd<Self> for Duration {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
         self.duration_ns().partial_cmp(&other.duration_ns())
     }
 }
@@ -57,14 +61,15 @@
         Duration {
             months: 0,
             weeks: 0,
             days: 0,
             nsecs: fixed_slots.abs(),
             negative: fixed_slots < 0,
             parsed_int: true,
+            saturating_months: None,
         }
     }
 
     /// Parse a string into a `Duration`
     ///
     /// Strings are composed of a sequence of number-unit pairs, such as `5d` (5 days). A string may begin with a minus
     /// sign, in which case it is interpreted as a negative duration. Some examples:
@@ -83,14 +88,17 @@
     /// * `ms`: millisecond
     /// * `s`:  second
     /// * `m`:  minute
     /// * `h`:  hour
     /// * `d`:  day
     /// * `w`:  week
     /// * `mo`: calendar month
+    /// * `mo_saturating`: calendar month, but "saturates" to the last day of the month
+    ///    instead of erroring. For example, 2022-01-29 plus `'1mo_saturating'` goes to
+    ///    2022-02-28.
     /// * `y`:  calendar year
     /// * `i`:  index value (only for {Int32, Int64} dtypes)
     ///
     /// # Panics
     /// If the given str is invalid for any reason.
     pub fn parse(duration: &str) -> Self {
         let num_minus_signs = duration.matches('-').count();
@@ -104,14 +112,15 @@
         let mut nsecs = 0;
         let mut weeks = 0;
         let mut days = 0;
         let mut months = 0;
         let mut iter = duration.char_indices();
         let negative = duration.starts_with('-');
         let mut start = 0;
+        let mut saturating_months: Option<bool> = None;
 
         // skip the '-' char
         if negative {
             start += 1;
             iter.next().unwrap();
         }
 
@@ -121,15 +130,15 @@
         while let Some((i, mut ch)) = iter.next() {
             if !ch.is_ascii_digit() {
                 let n = duration[start..i]
                     .parse::<i64>()
                     .expect("expected an integer in the duration string");
 
                 loop {
-                    if ch.is_ascii_alphabetic() {
+                    if ch.is_ascii_alphabetic() || ch == '_' {
                         unit.push(ch)
                     } else {
                         break;
                     }
                     match iter.next() {
                         Some((i, ch_)) => {
                             ch = ch_;
@@ -149,15 +158,28 @@
                     "us" => nsecs += n * NS_MICROSECOND,
                     "ms" => nsecs += n * NS_MILLISECOND,
                     "s" => nsecs += n * NS_SECOND,
                     "m" => nsecs += n * NS_MINUTE,
                     "h" => nsecs += n * NS_HOUR,
                     "d" => days += n,
                     "w" => weeks += n,
-                    "mo" => months += n,
+                    "mo" => {
+                        if let Some(true) = saturating_months {
+                            panic!("cannot use both saturating and non-saturating months")
+                        }
+                        saturating_months = Some(false);
+                        months += n
+                    }
+                    "mo_saturating" => {
+                        if let Some(false) = saturating_months {
+                            panic!("cannot use both saturating and non-saturating months")
+                        }
+                        saturating_months = Some(true);
+                        months += n
+                    }
                     "y" => months += n * 12,
                     // we will read indexes as nanoseconds
                     "i" => {
                         nsecs += n;
                         parsed_int = true;
                     }
                     unit => panic!("unit: '{unit}' not supported. Available units are: 'ns', 'us', 'ms', 's', 'm', 'h', 'd', 'w', 'mo', 'y', 'i'"),
@@ -168,14 +190,15 @@
         Duration {
             nsecs: nsecs.abs(),
             days: days.abs(),
             weeks: weeks.abs(),
             months: months.abs(),
             negative,
             parsed_int,
+            saturating_months,
         }
     }
 
     fn to_positive(v: i64) -> (bool, i64) {
         if v < 0 {
             (true, -v)
         } else {
@@ -234,53 +257,57 @@
         Self {
             months: 0,
             weeks: 0,
             days: 0,
             nsecs,
             negative,
             parsed_int: false,
+            saturating_months: None,
         }
     }
 
     /// Creates a [`Duration`] that represents a fixed number of months.
     pub(crate) fn from_months(v: i64) -> Self {
         let (negative, months) = Self::to_positive(v);
         Self {
             months,
             weeks: 0,
             days: 0,
             nsecs: 0,
             negative,
             parsed_int: false,
+            saturating_months: None,
         }
     }
 
     /// Creates a [`Duration`] that represents a fixed number of weeks.
     pub(crate) fn from_weeks(v: i64) -> Self {
         let (negative, weeks) = Self::to_positive(v);
         Self {
             months: 0,
             weeks,
             days: 0,
             nsecs: 0,
             negative,
             parsed_int: false,
+            saturating_months: None,
         }
     }
 
     /// Creates a [`Duration`] that represents a fixed number of days.
     pub(crate) fn from_days(v: i64) -> Self {
         let (negative, days) = Self::to_positive(v);
         Self {
             months: 0,
             weeks: 0,
             days,
             nsecs: 0,
             negative,
             parsed_int: false,
+            saturating_months: None,
         }
     }
 
     /// `true` if zero duration.
     pub fn is_zero(&self) -> bool {
         self.months == 0 && self.weeks == 0 && self.days == 0 && self.nsecs == 0
     }
@@ -517,38 +544,54 @@
             let ts = match tz {
                 #[cfg(feature = "timezones")]
                 Some(tz) => unlocalize_datetime(timestamp_to_datetime(t), tz),
                 _ => timestamp_to_datetime(t),
             };
             let mut year = ts.year();
             let mut month = ts.month() as i32;
-            let day = ts.day();
+            let mut day = ts.day();
             year += (months / 12) as i32;
             month += (months % 12) as i32;
 
             // if the month overflowed or underflowed, adjust the year
             // accordingly. Because we add the modulo for the months
             // the year will only adjust by one
             if month > 12 {
                 year += 1;
                 month -= 12;
             } else if month <= 0 {
                 year -= 1;
                 month += 12;
             }
 
+            if let Some(true) = d.saturating_months {
+                // Normalize the day if we are past the end of the month.
+                let mut last_day_of_month = last_day_of_month(month);
+                if month == (chrono::Month::February.number_from_month() as i32)
+                    && is_leap_year(year)
+                {
+                    last_day_of_month += 1;
+                }
+
+                if day > last_day_of_month {
+                    day = last_day_of_month
+                }
+            }
+
             // Retrieve the original time and construct a data
             // with the new year, month and day
             let hour = ts.hour();
             let minute = ts.minute();
             let sec = ts.second();
             let nsec = ts.nanosecond();
             let dt = new_datetime(year, month as u32, day, hour, minute, sec, nsec).ok_or(
                 polars_err!(
-                    ComputeError: format!("cannot advance '{}' by {} month(s)", ts, d.months)
+                    ComputeError: format!(
+                        "cannot advance '{}' by {} month(s). \
+                         If you were trying to get the last day of each month, you may want to try `.dt.month_end`", ts, if d.negative {-d.months} else {d.months})
                 ),
             )?;
             new_t = match tz {
                 #[cfg(feature = "timezones")]
                 Some(tz) => datetime_to_timestamp(localize_datetime(dt, tz)?),
                 _ => datetime_to_timestamp(dt),
             };
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files 4% similar despite different names*

```diff
@@ -229,38 +229,36 @@
     period: Duration,
     offset: Duration,
     time: &'a [i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<impl PolarsTimeZone + 'a>,
     start_offset: usize,
-) -> impl Iterator<Item = (IdxSize, IdxSize)> + TrustedLen + 'a {
+) -> impl Iterator<Item = PolarsResult<(IdxSize, IdxSize)>> + TrustedLen + 'a {
     debug_assert!(offset.duration_ns() >= period.duration_ns());
     debug_assert!(offset.negative);
-    fn add<T: PolarsTimeZone>(tu: TimeUnit) -> fn(&Duration, i64, Option<&T>) -> PolarsResult<i64> {
-        match tu {
-            TimeUnit::Nanoseconds => Duration::add_ns,
-            TimeUnit::Microseconds => Duration::add_us,
-            TimeUnit::Milliseconds => Duration::add_ms,
-        }
-    }
+    let add = match tu {
+        TimeUnit::Nanoseconds => Duration::add_ns,
+        TimeUnit::Microseconds => Duration::add_us,
+        TimeUnit::Milliseconds => Duration::add_ms,
+    };
 
     let mut last_lookbehind_i = 0;
     let mut last = i64::MIN;
     time[start_offset..]
         .iter()
         .enumerate()
         .map(move |(mut i, lower)| {
             if *lower < last {
                 panic!("index column of 'groupby_rolling' must be sorted in ascending order!")
             }
             last = *lower;
             i += start_offset;
-            let lower = add(tu)(&offset, *lower, tz.as_ref()).unwrap();
-            let upper = add(tu)(&period, lower, tz.as_ref()).unwrap();
+            let lower = add(&offset, *lower, tz.as_ref())?;
+            let upper = add(&period, lower, tz.as_ref())?;
 
             let b = Bounds::new(lower, upper);
 
             // we have a complete lookbehind so we know that `i` is the upper bound.
             // Safety
             // we are in bounds
             let slice = {
@@ -280,48 +278,41 @@
             last_lookbehind_i = lookbehind_i.saturating_sub(1);
 
             let mut len = i - lookbehind_i;
             if matches!(closed_window, ClosedWindow::Right | ClosedWindow::Both) {
                 len += 1;
             }
 
-            (lookbehind_i as IdxSize, len as IdxSize)
+            Ok((lookbehind_i as IdxSize, len as IdxSize))
         })
 }
 
 // this one is correct for all lookbehind/lookaheads, but is slower
 pub(crate) fn groupby_values_iter_window_behind_t<'a>(
     period: Duration,
     offset: Duration,
     time: &'a [i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<impl PolarsTimeZone + 'a>,
-) -> impl Iterator<Item = (IdxSize, IdxSize)> + TrustedLen + 'a {
-    fn add<T: PolarsTimeZone>(tu: TimeUnit) -> fn(&Duration, i64, Option<&T>) -> PolarsResult<i64> {
-        match tu {
-            TimeUnit::Nanoseconds => Duration::add_ns,
-            TimeUnit::Microseconds => Duration::add_us,
-            TimeUnit::Milliseconds => Duration::add_ms,
-        }
-    }
+) -> impl Iterator<Item = PolarsResult<(IdxSize, IdxSize)>> + TrustedLen + 'a {
+    let add = match tu {
+        TimeUnit::Nanoseconds => Duration::add_ns,
+        TimeUnit::Microseconds => Duration::add_us,
+        TimeUnit::Milliseconds => Duration::add_ms,
+    };
 
     let mut lagging_offset = 0;
-    let mut last = i64::MIN;
     time.iter().enumerate().map(move |(i, lower)| {
-        if *lower < last {
-            panic!("index column of 'groupby_rolling' must be sorted!")
-        }
-        last = *lower;
-        let lower = add(tu)(&offset, *lower, tz.as_ref()).unwrap();
-        let upper = add(tu)(&period, lower, tz.as_ref()).unwrap();
+        let lower = add(&offset, *lower, tz.as_ref())?;
+        let upper = add(&period, lower, tz.as_ref())?;
 
         let b = Bounds::new(lower, upper);
         if b.is_future(time[0], closed_window) {
-            (0, 0)
+            Ok((0, 0))
         } else {
             // find starting point of window
             // we can start searching from lagging offset as that is the minimum boundary because data is sorted
             // and every iteration this boundary shifts right
             // we cannot use binary search as a window is not binary,
             // it is false left from the window, true inside, and false right of the window
             let mut count = 0;
@@ -336,45 +327,38 @@
             }
 
             // Safety
             // we just iterated over value i.
             let slice = unsafe { time.get_unchecked(lagging_offset..) };
             let len = slice.partition_point(|v| b.is_member(*v, closed_window));
 
-            (lagging_offset as IdxSize, len as IdxSize)
+            Ok((lagging_offset as IdxSize, len as IdxSize))
         }
     })
 }
 
 // this one is correct for all lookbehind/lookaheads, but is slower
 pub(crate) fn groupby_values_iter_partial_lookbehind<'a>(
     period: Duration,
     offset: Duration,
     time: &'a [i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<impl PolarsTimeZone + 'a>,
-) -> impl Iterator<Item = (IdxSize, IdxSize)> + TrustedLen + 'a {
-    fn add<T: PolarsTimeZone>(tu: TimeUnit) -> fn(&Duration, i64, Option<&T>) -> PolarsResult<i64> {
-        match tu {
-            TimeUnit::Nanoseconds => Duration::add_ns,
-            TimeUnit::Microseconds => Duration::add_us,
-            TimeUnit::Milliseconds => Duration::add_ms,
-        }
-    }
+) -> impl Iterator<Item = PolarsResult<(IdxSize, IdxSize)>> + TrustedLen + 'a {
+    let add = match tu {
+        TimeUnit::Nanoseconds => Duration::add_ns,
+        TimeUnit::Microseconds => Duration::add_us,
+        TimeUnit::Milliseconds => Duration::add_ms,
+    };
 
     let mut lagging_offset = 0;
-    let mut last = i64::MIN;
     time.iter().enumerate().map(move |(i, lower)| {
-        if *lower < last {
-            panic!("index column of 'groupby_rolling' must be sorted!")
-        }
-        last = *lower;
-        let lower = add(tu)(&offset, *lower, tz.as_ref()).unwrap();
-        let upper = add(tu)(&period, lower, tz.as_ref()).unwrap();
+        let lower = add(&offset, *lower, tz.as_ref())?;
+        let upper = add(&period, lower, tz.as_ref())?;
 
         let b = Bounds::new(lower, upper);
 
         for &t in &time[lagging_offset..] {
             if b.is_member(t, closed_window) || lagging_offset == i {
                 break;
             }
@@ -382,60 +366,53 @@
         }
 
         // Safety
         // we just iterated over value i.
         let slice = unsafe { time.get_unchecked(lagging_offset..) };
         let len = slice.partition_point(|v| b.is_member(*v, closed_window));
 
-        (lagging_offset as IdxSize, len as IdxSize)
+        Ok((lagging_offset as IdxSize, len as IdxSize))
     })
 }
 
 #[allow(clippy::too_many_arguments)]
 pub(crate) fn groupby_values_iter_full_lookahead<'a>(
     period: Duration,
     offset: Duration,
     time: &'a [i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<impl PolarsTimeZone + 'a>,
     start_offset: usize,
     upper_bound: Option<usize>,
-) -> impl Iterator<Item = (IdxSize, IdxSize)> + TrustedLen + 'a {
+) -> impl Iterator<Item = PolarsResult<(IdxSize, IdxSize)>> + TrustedLen + 'a {
     let upper_bound = upper_bound.unwrap_or(time.len());
     debug_assert!(!offset.negative);
 
-    fn add<T: PolarsTimeZone>(tu: TimeUnit) -> fn(&Duration, i64, Option<&T>) -> PolarsResult<i64> {
-        match tu {
-            TimeUnit::Nanoseconds => Duration::add_ns,
-            TimeUnit::Microseconds => Duration::add_us,
-            TimeUnit::Milliseconds => Duration::add_ms,
-        }
-    }
+    let add = match tu {
+        TimeUnit::Nanoseconds => Duration::add_ns,
+        TimeUnit::Microseconds => Duration::add_us,
+        TimeUnit::Milliseconds => Duration::add_ms,
+    };
 
-    let mut last = i64::MIN;
     time[start_offset..upper_bound]
         .iter()
         .enumerate()
         .map(move |(mut i, lower)| {
-            if *lower < last {
-                panic!("index column of 'groupby_rolling' must be sorted!")
-            }
-            last = *lower;
             i += start_offset;
-            let lower = add(tu)(&offset, *lower, tz.as_ref()).unwrap();
-            let upper = add(tu)(&period, lower, tz.as_ref()).unwrap();
+            let lower = add(&offset, *lower, tz.as_ref())?;
+            let upper = add(&period, lower, tz.as_ref())?;
 
             let b = Bounds::new(lower, upper);
 
             debug_assert!(i < time.len());
             let slice = unsafe { time.get_unchecked(i..) };
             let len = slice.partition_point(|v| b.is_member(*v, closed_window));
 
-            (i as IdxSize, len as IdxSize)
+            Ok((i as IdxSize, len as IdxSize))
         })
 }
 
 pub(crate) fn partially_check_sorted(time: &[i64]) {
     // check sortedness of a small subslice.
     if time.len() > 1 {
         assert!(time[..std::cmp::min(time.len(), 10)].windows(2).filter_map(|w| match w[0].cmp(&w[1]) {
@@ -449,15 +426,15 @@
 pub(crate) fn groupby_values_iter<'a>(
     period: Duration,
     offset: Duration,
     time: &'a [i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<impl PolarsTimeZone + 'a>,
-) -> Box<dyn TrustedLen<Item = (IdxSize, IdxSize)> + 'a> {
+) -> Box<dyn TrustedLen<Item = PolarsResult<(IdxSize, IdxSize)>> + 'a> {
     partially_check_sorted(time);
     // we have a (partial) lookbehind window
     if offset.negative {
         // only lookbehind
         if offset.nanoseconds() == period.nanoseconds() {
             let iter =
                 groupby_values_iter_full_lookbehind(period, offset, time, closed_window, tu, tz, 0);
@@ -492,15 +469,15 @@
 pub fn groupby_values<'a>(
     period: Duration,
     offset: Duration,
     time: &'a [i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<impl PolarsTimeZone + 'a>,
-) -> GroupsSlice {
+) -> PolarsResult<GroupsSlice> {
     partially_check_sorted(time);
     let thread_offsets = _split_offsets(time.len(), POOL.current_num_threads());
 
     // we have a (partial) lookbehind window
     if offset.negative {
         if offset.duration_ns() >= period.duration_ns() {
             // lookbehind
@@ -519,46 +496,48 @@
                                 offset,
                                 &time[..upper_bound],
                                 closed_window,
                                 tu,
                                 tz.clone(),
                                 base_offset,
                             );
-                            iter.map(|(offset, len)| [offset as IdxSize, len])
-                                .collect_trusted::<Vec<_>>()
+                            iter.map(|result| result.map(|(offset, len)| [offset, len]))
+                                .collect::<PolarsResult<Vec<_>>>()
                         })
-                        .collect::<Vec<_>>()
-                });
-                flatten(&vals, Some(time.len()))
+                        .collect::<PolarsResult<Vec<_>>>()
+                })?;
+                Ok(flatten(&vals, Some(time.len())))
             }
             // window is completely behind t and t itself is not a member
             // ---------------t---
             //  [---]
             else {
                 let iter = groupby_values_iter_window_behind_t(
                     period,
                     offset,
                     time,
                     closed_window,
                     tu,
                     tz,
                 );
-                iter.map(|(offset, len)| [offset, len]).collect_trusted()
+                iter.map(|result| result.map(|(offset, len)| [offset, len]))
+                    .collect::<PolarsResult<_>>()
             }
         }
         // partial lookbehind
         // this one is still single threaded
         // can make it parallel later, its a bit more complicated because the boundaries are unknown
         // window is with -1 periods of t
         // ----t---
         //  [---]
         else {
             let iter =
                 groupby_values_iter_partial_lookbehind(period, offset, time, closed_window, tu, tz);
-            iter.map(|(offset, len)| [offset, len]).collect_trusted()
+            iter.map(|result| result.map(|(offset, len)| [offset, len]))
+                .collect::<PolarsResult<_>>()
         }
     } else {
         let vals = POOL.install(|| {
             thread_offsets
                 .par_iter()
                 .copied()
                 .map(|(base_offset, len)| {
@@ -570,15 +549,15 @@
                         time,
                         closed_window,
                         tu,
                         tz.clone(),
                         lower_bound,
                         Some(upper_bound),
                     );
-                    iter.map(|(offset, len)| [offset as IdxSize, len])
-                        .collect_trusted::<Vec<_>>()
+                    iter.map(|result| result.map(|(offset, len)| [offset as IdxSize, len]))
+                        .collect::<PolarsResult<Vec<_>>>()
                 })
-                .collect::<Vec<_>>()
-        });
-        flatten(&vals, Some(time.len()))
+                .collect::<PolarsResult<Vec<_>>>()
+        })?;
+        Ok(flatten(&vals, Some(time.len())))
     }
 }
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/test.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/test.rs`

 * *Files 1% similar despite different names*

```diff
@@ -641,15 +641,16 @@
     let groups = groupby_values(
         Duration::parse("2h"),
         Duration::parse("-2h"),
         &dates,
         ClosedWindow::Right,
         TimeUnit::Milliseconds,
         NO_TIMEZONE.copied(),
-    );
+    )
+    .unwrap();
     assert_eq!(dates.len(), groups.len());
     assert_eq!(groups[0], [0, 1]); // bound: 22:00 -> 24:00     time: 24:00
     assert_eq!(groups[1], [0, 2]); // bound: 22:30 -> 00:30     time: 00:30
     assert_eq!(groups[2], [0, 3]); // bound: 23:00 -> 01:00     time: 01:00
     assert_eq!(groups[3], [0, 4]); // bound: 23:30 -> 01:30     time: 01:30
     assert_eq!(groups[4], [1, 4]); // bound: 24:00 -> 02:00     time: 02:00
     assert_eq!(groups[5], [2, 4]); // bound: 00:30 -> 02:30     time: 02:30
@@ -661,15 +662,16 @@
     let groups = groupby_values(
         Duration::parse("2h"),
         Duration::parse("-1h"),
         &dates,
         ClosedWindow::Right,
         TimeUnit::Milliseconds,
         NO_TIMEZONE.copied(),
-    );
+    )
+    .unwrap();
     assert_eq!(dates.len(), groups.len());
     assert_eq!(groups[0], [0, 3]);
     assert_eq!(groups[1], [0, 4]);
     assert_eq!(groups[2], [1, 4]);
     assert_eq!(groups[3], [2, 4]);
     assert_eq!(groups[4], [3, 4]);
     assert_eq!(groups[5], [4, 4]);
@@ -681,15 +683,16 @@
     let groups = groupby_values(
         Duration::parse("2h"),
         Duration::parse("0h"),
         &dates,
         ClosedWindow::Right,
         TimeUnit::Milliseconds,
         NO_TIMEZONE.copied(),
-    );
+    )
+    .unwrap();
     assert_eq!(dates.len(), groups.len());
     assert_eq!(groups[0], [0, 5]);
     assert_eq!(groups[1], [1, 5]);
     assert_eq!(groups[2], [2, 5]);
     assert_eq!(groups[3], [3, 5]);
     assert_eq!(groups[4], [4, 5]);
     assert_eq!(groups[5], [5, 4]);
@@ -712,46 +715,50 @@
             &dates,
             closed_window,
             tu,
             NO_TIMEZONE.copied(),
             0,
             None,
         )
-        .collect::<Vec<_>>();
+        .collect::<PolarsResult<Vec<_>>>()
+        .unwrap();
         let g1 = groupby_values_iter_partial_lookbehind(
             period,
             offset,
             &dates,
             closed_window,
             tu,
             NO_TIMEZONE.copied(),
         )
-        .collect::<Vec<_>>();
+        .collect::<PolarsResult<Vec<_>>>()
+        .unwrap();
         assert_eq!(g0, g1);
 
         let offset = Duration::parse("-2h");
         let g0 = groupby_values_iter_full_lookbehind(
             period,
             offset,
             &dates,
             closed_window,
             tu,
             NO_TIMEZONE.copied(),
             0,
         )
-        .collect::<Vec<_>>();
+        .collect::<PolarsResult<Vec<_>>>()
+        .unwrap();
         let g1 = groupby_values_iter_partial_lookbehind(
             period,
             offset,
             &dates,
             closed_window,
             tu,
             NO_TIMEZONE.copied(),
         )
-        .collect::<Vec<_>>();
+        .collect::<PolarsResult<Vec<_>>>()
+        .unwrap();
         assert_eq!(g0, g1);
     }
 }
 
 #[test]
 fn test_end_membership() {
     let time = [
```

### Comparing `polars_lts_cpu-0.17.7/local_dependencies/polars-time/src/windows/window.rs` & `polars_lts_cpu-0.17.8/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/Cargo.toml` & `polars_lts_cpu-0.17.8/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.17.7"
+version = "0.17.8"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_lts_cpu-0.17.7/LICENSE` & `polars_lts_cpu-0.17.8/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/Makefile` & `polars_lts_cpu-0.17.8/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/README.md` & `polars_lts_cpu-0.17.8/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/build.rs` & `polars_lts_cpu-0.17.8/build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/Makefile` & `polars_lts_cpu-0.17.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/_templates/autosummary/class.rst` & `polars_lts_cpu-0.17.8/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/_static/css/custom.css` & `polars_lts_cpu-0.17.8/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/conf.py` & `polars_lts_cpu-0.17.8/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates", sphinx_autosummary_accessors.templates_path]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = []
+exclude_patterns = ["Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
```

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/api.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/config.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/config.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/dataframe/modify_select.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/datatypes.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/expressions/computation.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/expressions/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/expressions/functions.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/expressions/list.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/expressions/modify_select.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/expressions/operators.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/expressions/string.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/expressions/temporal.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/expressions/temporal.rst`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     Expr.dt.microsecond
     Expr.dt.microseconds
     Expr.dt.millisecond
     Expr.dt.milliseconds
     Expr.dt.minute
     Expr.dt.minutes
     Expr.dt.month
+    Expr.dt.month_start
+    Expr.dt.month_end
     Expr.dt.nanosecond
     Expr.dt.nanoseconds
     Expr.dt.offset_by
     Expr.dt.ordinal_day
     Expr.dt.quarter
     Expr.dt.round
     Expr.dt.second
```

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/functions.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/io.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/lazyframe/modify_select.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/series/computation.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/series/descriptive.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/series/list.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/series/modify_select.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/series/string.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/docs/source/reference/series/temporal.rst` & `polars_lts_cpu-0.17.8/docs/source/reference/series/temporal.rst`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     Series.dt.microseconds
     Series.dt.millisecond
     Series.dt.milliseconds
     Series.dt.min
     Series.dt.minute
     Series.dt.minutes
     Series.dt.month
+    Series.dt.month_start
+    Series.dt.month_end
     Series.dt.nanosecond
     Series.dt.nanoseconds
     Series.dt.offset_by
     Series.dt.ordinal_day
     Series.dt.quarter
     Series.dt.round
     Series.dt.second
```

### Comparing `polars_lts_cpu-0.17.7/polars/__init__.py` & `polars_lts_cpu-0.17.8/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/api.py` & `polars_lts_cpu-0.17.8/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/config.py` & `polars_lts_cpu-0.17.8/polars/config.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/convert.py` & `polars_lts_cpu-0.17.8/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/dataframe/_html.py` & `polars_lts_cpu-0.17.8/polars/dataframe/_html.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,20 +111,22 @@
                             else:
                                 series = self.df[:, c]
                                 self.elements.append(
                                     html.escape(series._s.get_fmt(r, str_lengths))
                                 )
 
     def write(self, inner: str) -> None:
+        """Append a raw string to the inner HTML."""
         self.elements.append(inner)
 
     def render(self) -> list[str]:
-        shape: tuple[int, ...] = self.df.shape
-        if self.series:
-            shape = shape[:1]
+        """Return the lines needed to render a HTML table."""
+        # format frame/series shape with '_' thousand-separators
+        s = self.df.shape
+        shape = f"({s[0]:_},)" if self.series else f"({s[0]:_}, {s[1]:_})"
 
         self.elements.append(f"<small>shape: {shape}</small>")
         with Tag(
             # be careful changing the CSS class ref here...
             # ref: https://github.com/pola-rs/polars/issues/7443
             self.elements,
             "table",
```

### Comparing `polars_lts_cpu-0.17.7/polars/dataframe/frame.py` & `polars_lts_cpu-0.17.8/polars/dataframe/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from polars import internals as pli
 from polars.dataframe._html import NotebookFormatter
 from polars.dataframe.groupby import DynamicGroupBy, GroupBy, RollingGroupBy
 from polars.datatypes import (
     FLOAT_DTYPES,
     INTEGER_DTYPES,
     N_INFER_DEFAULT,
+    NUMERIC_DTYPES,
     SIGNED_INTEGER_DTYPES,
     Boolean,
     Categorical,
     DataTypeClass,
     Float64,
     Int8,
     Int16,
@@ -3653,46 +3654,52 @@
 
         """
         if isinstance(percentiles, float):
             percentiles = [percentiles]
         if percentiles and not all((0 <= p <= 1) for p in percentiles):
             raise ValueError("Percentiles must all be in the range [0, 1].")
 
-        def describe_cast(stat: Self) -> Self:
-            columns = []
-            for i, s in enumerate(self.columns):
-                if self[s].is_numeric() or self[s].is_boolean():
-                    columns.append(stat[:, i].cast(float))
-                else:
-                    # for dates, strings, etc, we cast to string so that all
-                    # statistics can be shown
-                    columns.append(stat[:, i].cast(str, strict=False))
-            return self.__class__(columns)
-
-        # Build output rows
-        output_rows = [
-            describe_cast(self.__class__({c: [len(self)] for c in self.columns})),
-            describe_cast(self.null_count()),
-            describe_cast(self.mean()),
-            describe_cast(self.std()),
-            describe_cast(self.min()),
-            describe_cast(self.max()),
-            describe_cast(self.median()),
-        ]
-        row_identifiers = ["count", "null_count", "mean", "std", "min", "max", "median"]
-
-        # Dynamically add rows for quantiles
+        # determine metrics (optional/additional percentiles)
+        metrics = ["count", "null_count", "mean", "std", "min", "max", "median"]
+        percentile_exprs = []
         for p in percentiles or ():
-            output_rows.append(describe_cast(self.quantile(p)))
-            row_identifiers.append(f"{p:.0%}")
+            percentile_exprs.append(F.all().quantile(p).prefix(f"{p}:"))
+            metrics.append(f"{p:.0%}")
+
+        # execute metrics in parallel
+        res = self.select(
+            F.all().count().prefix("count:"),
+            F.all().null_count().prefix("null_count:"),
+            F.all().mean().prefix("mean:"),
+            F.all().std().prefix("std:"),
+            F.all().min().prefix("min:"),
+            F.all().max().prefix("max:"),
+            F.all().median().prefix("median:"),
+            *percentile_exprs,
+        ).row(0)
+
+        # reshape/cast wide result
+        n_cols = len(self.columns)
+        described = [
+            res[(n * n_cols) : (n + 1) * n_cols] for n in range(0, len(metrics))
+        ]
+        summary = dict(zip(self.columns, list(zip(*described))))
+        num_or_bool = NUMERIC_DTYPES | {Boolean}
+        for c, tp in self.schema.items():
+            summary[c] = [
+                None
+                if (v is None or isinstance(v, dict))
+                else (float(v) if tp in num_or_bool else str(v))
+                for v in summary[c]
+            ]
 
-        # Build summary dataframe
-        summary = self._from_pydf(F.concat(output_rows)._df)
-        summary.insert_at_idx(0, pli.Series("describe", row_identifiers))
-        return summary
+        # return as frame
+        df_summary = self.__class__(summary)
+        df_summary.insert_at_idx(0, pli.Series("describe", metrics))
+        return df_summary
 
     def find_idx_by_name(self, name: str) -> int:
         """
         Find the index of a column by name.
 
         Parameters
         ----------
@@ -4588,14 +4595,16 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
+        - 1mo_saturating (same as above, but saturates to the last day of the month
+          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         In case of a groupby_rolling on an integer column, the windows are defined by:
@@ -4703,14 +4712,16 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
+        - 1mo_saturating (same as above, but saturates to the last day of the month
+          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         In case of a groupby_dynamic on an integer column, the windows are defined by:
@@ -4987,14 +4998,16 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
+        - 1mo_saturating (same as above, but saturates to the last day of the month
+          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         Examples
@@ -5113,14 +5126,16 @@
                 - 1ms   (1 millisecond)
                 - 1s    (1 second)
                 - 1m    (1 minute)
                 - 1h    (1 hour)
                 - 1d    (1 day)
                 - 1w    (1 week)
                 - 1mo   (1 calendar month)
+                - 1mo_saturating (same as above, but saturates to the last day of the
+                  month if the target date does not exist)
                 - 1y    (1 calendar year)
                 - 1i    (1 index count)
 
                 Or combine them:
                 "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         allow_parallel
```

### Comparing `polars_lts_cpu-0.17.7/polars/dataframe/groupby.py` & `polars_lts_cpu-0.17.8/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/datatypes/__init__.py` & `polars_lts_cpu-0.17.8/polars/datatypes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from polars.datatypes.classes import (
     Binary,
     Boolean,
     Categorical,
     DataType,
     DataTypeClass,
+    DataTypeGroup,
     Date,
     Datetime,
     Decimal,
     Duration,
     Field,
     Float32,
     Float64,
@@ -73,14 +74,15 @@
 __all__ = [
     # classes
     "Binary",
     "Boolean",
     "Categorical",
     "DataType",
     "DataTypeClass",
+    "DataTypeGroup",
     "Date",
     "Datetime",
     "Decimal",
     "Duration",
     "Field",
     "Float32",
     "Float64",
```

### Comparing `polars_lts_cpu-0.17.7/polars/datatypes/classes.py` & `polars_lts_cpu-0.17.8/polars/datatypes/classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import TYPE_CHECKING, Any, Iterator, Mapping, Sequence
 
 import polars.datatypes
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import dtype_str_repr as _dtype_str_repr
 
-
 if TYPE_CHECKING:
     from polars.type_aliases import PolarsDataType, PythonDataType, SchemaDict, TimeUnit
 
 
 class DataTypeClass(type):
     """Metaclass for nicely printing DataType classes."""
 
@@ -70,14 +69,33 @@
         if base.__init__ != object.__init__:
             base.__init__(obj, state)
     else:
         obj = object.__new__(cls)
     return obj
 
 
+class DataTypeGroup(frozenset):  # type: ignore[type-arg]
+    _match_base_type: bool
+
+    def __new__(cls, items: Any, *, match_base_type: bool = True) -> DataTypeGroup:
+        for it in items:
+            if not isinstance(it, (DataType, DataTypeClass)):
+                raise TypeError(
+                    f"DataTypeGroup items must be dtypes; found {type(it).__name__!r}"
+                )
+        dtype_group = super().__new__(cls, items)
+        dtype_group._match_base_type = match_base_type
+        return dtype_group
+
+    def __contains__(self, item: Any) -> bool:
+        if self._match_base_type and isinstance(item, (DataType, DataTypeClass)):
+            item = item.base_type()
+        return super().__contains__(item)
+
+
 class NumericType(DataType):
     """Base class for numeric data types."""
 
 
 class IntegralType(NumericType):
     """Base class for integral data types."""
```

### Comparing `polars_lts_cpu-0.17.7/polars/datatypes/constants.py` & `polars_lts_cpu-0.17.8/polars/datatypes/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from polars.datatypes import (
+    DataTypeGroup,
     Date,
     Datetime,
     Decimal,
     Duration,
     Float32,
     Float64,
     Int8,
@@ -17,56 +18,57 @@
     UInt8,
     UInt16,
     UInt32,
     UInt64,
 )
 
 if TYPE_CHECKING:
-    from polars.type_aliases import PolarsDataType, TimeUnit
+    from polars.datatypes import PolarsDataType
+    from polars.type_aliases import TimeUnit
+
 
 DTYPE_TEMPORAL_UNITS: frozenset[TimeUnit] = frozenset(["ns", "us", "ms"])
-DATETIME_DTYPES: frozenset[PolarsDataType] = frozenset(
+DATETIME_DTYPES: frozenset[PolarsDataType] = DataTypeGroup(
     [
-        # TODO: ideally need a mechanism to wildcard timezones here too
         Datetime,
         Datetime("ms"),
         Datetime("us"),
         Datetime("ns"),
     ]
 )
-DURATION_DTYPES: frozenset[PolarsDataType] = frozenset(
+DURATION_DTYPES: frozenset[PolarsDataType] = DataTypeGroup(
     [
         Duration,
         Duration("ms"),
         Duration("us"),
         Duration("ns"),
     ]
 )
-TEMPORAL_DTYPES: frozenset[PolarsDataType] = (
+TEMPORAL_DTYPES: frozenset[PolarsDataType] = DataTypeGroup(
     frozenset([Date, Time]) | DATETIME_DTYPES | DURATION_DTYPES
 )
-SIGNED_INTEGER_DTYPES: frozenset[PolarsDataType] = frozenset(
+SIGNED_INTEGER_DTYPES: frozenset[PolarsDataType] = DataTypeGroup(
     [
         Int8,
         Int16,
         Int32,
         Int64,
     ]
 )
-UNSIGNED_INTEGER_DTYPES: frozenset[PolarsDataType] = frozenset(
+UNSIGNED_INTEGER_DTYPES: frozenset[PolarsDataType] = DataTypeGroup(
     [
         UInt8,
         UInt16,
         UInt32,
         UInt64,
     ]
 )
 INTEGER_DTYPES: frozenset[PolarsDataType] = (
     SIGNED_INTEGER_DTYPES | UNSIGNED_INTEGER_DTYPES
 )
-FLOAT_DTYPES: frozenset[PolarsDataType] = frozenset([Float32, Float64])
-NUMERIC_DTYPES: frozenset[PolarsDataType] = (
+FLOAT_DTYPES: frozenset[PolarsDataType] = DataTypeGroup([Float32, Float64])
+NUMERIC_DTYPES: frozenset[PolarsDataType] = DataTypeGroup(
     FLOAT_DTYPES | INTEGER_DTYPES | frozenset([Decimal])
 )
 
 # number of rows to scan by default when inferring datatypes
 N_INFER_DEFAULT = 100
```

### Comparing `polars_lts_cpu-0.17.7/polars/datatypes/constructor.py` & `polars_lts_cpu-0.17.8/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/datatypes/convert.py` & `polars_lts_cpu-0.17.8/polars/datatypes/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/dependencies.py` & `polars_lts_cpu-0.17.8/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/exceptions.py` & `polars_lts_cpu-0.17.8/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/expr/binary.py` & `polars_lts_cpu-0.17.8/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/expr/categorical.py` & `polars_lts_cpu-0.17.8/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/expr/datetime.py` & `polars_lts_cpu-0.17.8/polars/expr/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         - 1ms # 1 millisecond
         - 1s  # 1 second
         - 1m  # 1 minute
         - 1h  # 1 hour
         - 1d  # 1 day
         - 1w  # 1 calendar week
         - 1mo # 1 calendar month
+        - 1mo_saturating # same as above, but saturates to the last day of the month
+          if the target date does not exist
         - 1y  # 1 calendar year
 
         These strings can be combined:
 
         - 3d12h4m25s # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         Returns
@@ -170,14 +172,16 @@
         1ms  # 1 millisecond
         1s   # 1 second
         1m   # 1 minute
         1h   # 1 hour
         1d   # 1 day
         1w   # 1 calendar week
         1mo  # 1 calendar month
+        1mo_saturating  # same as above, but saturates to the last day of the month
+        # if the target date does not exist
         1y   # 1 calendar year
 
         eg: 3d12h4m25s  # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         Returns
         -------
         Date/Datetime series
@@ -1666,14 +1670,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
         Returns
         -------
         Date/Datetime expression
 
@@ -1726,7 +1732,93 @@
         │ 2002-01-31 00:00:00 │
         │ 2003-01-31 00:00:00 │
         │ 2004-01-31 00:00:00 │
         │ 2005-01-31 00:00:00 │
         └─────────────────────┘
         """
         return wrap_expr(self._pyexpr.dt_offset_by(by))
+
+    def month_start(self) -> Expr:
+        """
+        Roll backward to the first day of the month.
+
+        Returns
+        -------
+        Date/Datetime expression
+
+        Notes
+        -----
+        If you're coming from pandas, you can think of this as a vectorised version
+        of ``pandas.tseries.offsets.MonthBegin().rollback(datetime)``.
+
+        Examples
+        --------
+        >>> from datetime import datetime
+        >>> df = pl.DataFrame(
+        ...     {
+        ...         "dates": pl.date_range(
+        ...             datetime(2000, 1, 15, 2), datetime(2000, 12, 15, 2), "1mo"
+        ...         )
+        ...     }
+        ... )
+        >>> df.select(pl.col("dates").dt.month_start())
+        shape: (12, 1)
+        ┌─────────────────────┐
+        │ dates               │
+        │ ---                 │
+        │ datetime[μs]        │
+        ╞═════════════════════╡
+        │ 2000-01-01 02:00:00 │
+        │ 2000-02-01 02:00:00 │
+        │ 2000-03-01 02:00:00 │
+        │ 2000-04-01 02:00:00 │
+        │ …                   │
+        │ 2000-09-01 02:00:00 │
+        │ 2000-10-01 02:00:00 │
+        │ 2000-11-01 02:00:00 │
+        │ 2000-12-01 02:00:00 │
+        └─────────────────────┘
+        """
+        return wrap_expr(self._pyexpr.dt_month_start())
+
+    def month_end(self) -> Expr:
+        """
+        Roll forward to the last day of the month.
+
+        Returns
+        -------
+        Date/Datetime expression
+
+        Notes
+        -----
+        If you're coming from pandas, you can think of this as a vectorised version
+        of ``pandas.tseries.offsets.MonthEnd().rollforward(datetime)``.
+
+        Examples
+        --------
+        >>> from datetime import datetime
+        >>> df = pl.DataFrame(
+        ...     {
+        ...         "dates": pl.date_range(
+        ...             datetime(2000, 1, 1, 2), datetime(2000, 12, 1, 2), "1mo"
+        ...         )
+        ...     }
+        ... )
+        >>> df.select(pl.col("dates").dt.month_end())
+        shape: (12, 1)
+        ┌─────────────────────┐
+        │ dates               │
+        │ ---                 │
+        │ datetime[μs]        │
+        ╞═════════════════════╡
+        │ 2000-01-31 02:00:00 │
+        │ 2000-02-29 02:00:00 │
+        │ 2000-03-31 02:00:00 │
+        │ 2000-04-30 02:00:00 │
+        │ …                   │
+        │ 2000-09-30 02:00:00 │
+        │ 2000-10-31 02:00:00 │
+        │ 2000-11-30 02:00:00 │
+        │ 2000-12-31 02:00:00 │
+        └─────────────────────┘
+        """
+        return wrap_expr(self._pyexpr.dt_month_end())
```

### Comparing `polars_lts_cpu-0.17.7/polars/expr/expr.py` & `polars_lts_cpu-0.17.8/polars/expr/expr.py`

 * *Files 1% similar despite different names*

```diff
@@ -4577,14 +4577,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
@@ -4672,14 +4674,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
@@ -4767,14 +4771,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
@@ -4862,14 +4868,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length of the window that will be multiplied
@@ -4957,14 +4965,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
@@ -5052,14 +5062,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
@@ -5143,14 +5155,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
@@ -5240,14 +5254,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
```

### Comparing `polars_lts_cpu-0.17.7/polars/expr/list.py` & `polars_lts_cpu-0.17.8/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/expr/meta.py` & `polars_lts_cpu-0.17.8/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/expr/string.py` & `polars_lts_cpu-0.17.8/polars/expr/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/expr/struct.py` & `polars_lts_cpu-0.17.8/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/functions/__init__.py` & `polars_lts_cpu-0.17.8/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/functions/eager.py` & `polars_lts_cpu-0.17.8/polars/functions/eager.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,24 +462,22 @@
     Series: '' [datetime[μs, America/New_York]]
     [
         2022-01-01 00:00:00 EST
         2022-02-01 00:00:00 EST
         2022-03-01 00:00:00 EST
     ]
 
-    Combine with ``offset_by`` to get the last day of the month:
+    Combine with ``month_end`` to get the last day of the month:
 
     >>> (
     ...     pl.date_range(
     ...         datetime(2022, 1, 1),
     ...         datetime(2022, 3, 1),
     ...         "1mo",
-    ...     )
-    ...     .dt.offset_by("1mo")
-    ...     .dt.offset_by("-1d")
+    ...     ).dt.month_end()
     ... )
     shape: (3,)
     Series: '' [datetime[μs]]
     [
         2022-01-31 00:00:00
         2022-02-28 00:00:00
         2022-03-31 00:00:00
```

### Comparing `polars_lts_cpu-0.17.7/polars/functions/lazy.py` & `polars_lts_cpu-0.17.8/polars/functions/lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/functions/whenthen.py` & `polars_lts_cpu-0.17.8/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/__init__.py` & `polars_lts_cpu-0.17.8/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/_utils.py` & `polars_lts_cpu-0.17.8/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/avro.py` & `polars_lts_cpu-0.17.8/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/csv/_utils.py` & `polars_lts_cpu-0.17.8/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/csv/batched_reader.py` & `polars_lts_cpu-0.17.8/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/csv/functions.py` & `polars_lts_cpu-0.17.8/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/database.py` & `polars_lts_cpu-0.17.8/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/delta.py` & `polars_lts_cpu-0.17.8/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/excel/_write_utils.py` & `polars_lts_cpu-0.17.8/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/excel/functions.py` & `polars_lts_cpu-0.17.8/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/ipc/anonymous_scan.py` & `polars_lts_cpu-0.17.8/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/ipc/functions.py` & `polars_lts_cpu-0.17.8/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/json.py` & `polars_lts_cpu-0.17.8/polars/io/json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/ndjson.py` & `polars_lts_cpu-0.17.8/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/parquet/anonymous_scan.py` & `polars_lts_cpu-0.17.8/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/parquet/functions.py` & `polars_lts_cpu-0.17.8/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_lts_cpu-0.17.8/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/io/pyarrow_dataset/functions.py` & `polars_lts_cpu-0.17.8/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/lazyframe/frame.py` & `polars_lts_cpu-0.17.8/polars/lazyframe/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1962,15 +1962,15 @@
         <polars.LazyFrame object at ...>
 
         """
         return self._from_pyldf(self._ldf.clone())
 
     def filter(self, predicate: Expr | str | Series | list[bool]) -> Self:
         """
-        Filter the rows in the DataFrame based on a predicate expression.
+        Filter the rows in the LazyFrame based on a predicate expression.
 
         Parameters
         ----------
         predicate
             Expression that evaluates to a boolean Series.
 
         Examples
@@ -2032,15 +2032,15 @@
     def select(
         self,
         exprs: IntoExpr | Iterable[IntoExpr] | None = None,
         *more_exprs: IntoExpr,
         **named_exprs: IntoExpr,
     ) -> Self:
         """
-        Select columns from this DataFrame.
+        Select columns from this LazyFrame.
 
         Parameters
         ----------
         exprs
             Column(s) to select. Accepts expression input. Strings are parsed as column
             names, other non-expression inputs are parsed as literals.
         *more_exprs
@@ -2281,14 +2281,16 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
+        - 1mo_saturating (same as above, but saturates to the last day of the month
+          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         In case of a groupby_rolling on an integer column, the windows are defined by:
@@ -2326,23 +2328,27 @@
         ...     "2020-01-01 13:45:48",
         ...     "2020-01-01 16:42:13",
         ...     "2020-01-01 16:45:09",
         ...     "2020-01-02 18:12:48",
         ...     "2020-01-03 19:45:32",
         ...     "2020-01-08 23:16:43",
         ... ]
-        >>> df = pl.DataFrame({"dt": dates, "a": [3, 7, 5, 9, 2, 1]}).with_columns(
+        >>> df = pl.LazyFrame({"dt": dates, "a": [3, 7, 5, 9, 2, 1]}).with_columns(
         ...     pl.col("dt").str.strptime(pl.Datetime)
         ... )
-        >>> out = df.groupby_rolling(index_column="dt", period="2d").agg(
-        ...     [
-        ...         pl.sum("a").alias("sum_a"),
-        ...         pl.min("a").alias("min_a"),
-        ...         pl.max("a").alias("max_a"),
-        ...     ]
+        >>> out = (
+        ...     df.groupby_rolling(index_column="dt", period="2d")
+        ...     .agg(
+        ...         [
+        ...             pl.sum("a").alias("sum_a"),
+        ...             pl.min("a").alias("min_a"),
+        ...             pl.max("a").alias("max_a"),
+        ...         ]
+        ...     )
+        ...     .collect()
         ... )
         >>> assert out["sum_a"].to_list() == [3, 10, 15, 24, 11, 1]
         >>> assert out["max_a"].to_list() == [3, 7, 7, 9, 9, 1]
         >>> assert out["min_a"].to_list() == [3, 3, 3, 3, 2, 1]
         >>> out
         shape: (6, 4)
         ┌─────────────────────┬───────┬───────┬───────┐
@@ -2406,14 +2412,16 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
+        - 1mo_saturating (same as above, but saturates to the last day of the month
+          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         In case of a groupby_dynamic on an integer column, the windows are defined by:
@@ -2737,14 +2745,16 @@
                 - 1ms   (1 millisecond)
                 - 1s    (1 second)
                 - 1m    (1 minute)
                 - 1h    (1 hour)
                 - 1d    (1 day)
                 - 1w    (1 week)
                 - 1mo   (1 calendar month)
+                - 1mo_saturating (same as above, but saturates to the last day of the
+                  month if the target date does not exist)
                 - 1y    (1 calendar year)
                 - 1i    (1 index count)
 
                 Or combine them:
                 "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         allow_parallel
```

### Comparing `polars_lts_cpu-0.17.7/polars/lazyframe/groupby.py` & `polars_lts_cpu-0.17.8/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/series/_numpy.py` & `polars_lts_cpu-0.17.8/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/series/binary.py` & `polars_lts_cpu-0.17.8/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/series/categorical.py` & `polars_lts_cpu-0.17.8/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/series/datetime.py` & `polars_lts_cpu-0.17.8/polars/series/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1438,14 +1438,16 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
+            - 1mo_saturating (same as above, but saturates to the last day of the month
+              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
         Returns
         -------
         Date/Datetime expression
 
@@ -1529,14 +1531,16 @@
         - 1ms # 1 millisecond
         - 1s  # 1 second
         - 1m  # 1 minute
         - 1h  # 1 hour
         - 1d  # 1 day
         - 1w  # 1 calendar week
         - 1mo # 1 calendar month
+        - 1mo_saturating  # same as above, but saturates to the last day of the month
+          if the target date does not exist
         - 1y  # 1 calendar year
 
         These strings can be combined:
 
         - 3d12h4m25s # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         Returns
@@ -1631,14 +1635,16 @@
         1ms # 1 millisecond
         1s  # 1 second
         1m  # 1 minute
         1h  # 1 hour
         1d  # 1 day
         1w  # 1 calendar week
         1mo # 1 calendar month
+        1mo_saturating  # same as above, but saturates to the last day of the month
+        # if the target date does not exist
         1y  # 1 calendar year
 
         3d12h4m25s # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         Parameters
         ----------
         every
@@ -1736,7 +1742,63 @@
         Series: 'dtm' [datetime[μs]]
         [
             2022-12-31 01:02:03.456
             2023-07-05 01:02:03.456
         ]
 
         """
+
+    def month_start(self) -> Series:
+        """
+        Roll backward to the first day of the month.
+
+        Returns
+        -------
+        Date/Datetime expression
+
+        Notes
+        -----
+        If you're coming from pandas, you can think of this as a vectorised version
+        of ``pandas.tseries.offsets.MonthBegin().rollback(datetime)``.
+
+        Examples
+        --------
+        >>> from datetime import datetime
+        >>> s = pl.date_range(datetime(2000, 1, 2, 2), datetime(2000, 4, 2, 2), "1mo")
+        >>> s.dt.month_start()
+        shape: (4,)
+        Series: '' [datetime[μs]]
+        [
+                2000-01-01 02:00:00
+                2000-02-01 02:00:00
+                2000-03-01 02:00:00
+                2000-04-01 02:00:00
+        ]
+        """
+
+    def month_end(self) -> Series:
+        """
+        Roll forward to the last day of the month.
+
+        Returns
+        -------
+        Date/Datetime expression
+
+        Notes
+        -----
+        If you're coming from pandas, you can think of this as a vectorised version
+        of ``pandas.tseries.offsets.MonthEnd().rollforward(datetime)``.
+
+        Examples
+        --------
+        >>> from datetime import datetime
+        >>> s = pl.date_range(datetime(2000, 1, 2, 2), datetime(2000, 4, 2, 2), "1mo")
+        >>> s.dt.month_end()
+        shape: (4,)
+        Series: '' [datetime[μs]]
+        [
+                2000-01-31 02:00:00
+                2000-02-29 02:00:00
+                2000-03-31 02:00:00
+                2000-04-30 02:00:00
+        ]
+        """
```

### Comparing `polars_lts_cpu-0.17.7/polars/series/list.py` & `polars_lts_cpu-0.17.8/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/series/series.py` & `polars_lts_cpu-0.17.8/polars/series/series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/series/string.py` & `polars_lts_cpu-0.17.8/polars/series/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/series/struct.py` & `polars_lts_cpu-0.17.8/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/series/utils.py` & `polars_lts_cpu-0.17.8/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/slice.py` & `polars_lts_cpu-0.17.8/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/sql/context.py` & `polars_lts_cpu-0.17.8/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/string_cache.py` & `polars_lts_cpu-0.17.8/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/testing/_private.py` & `polars_lts_cpu-0.17.8/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/testing/_tempdir.py` & `polars_lts_cpu-0.17.8/polars/testing/_tempdir.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/testing/asserts.py` & `polars_lts_cpu-0.17.8/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/testing/parametric/__init__.py` & `polars_lts_cpu-0.17.8/polars/testing/parametric/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 if _HYPOTHESIS_AVAILABLE:
     from polars.testing.parametric.primitives import (
         column,
         columns,
         dataframes,
         series,
     )
+    from polars.testing.parametric.profiles import load_profile, set_profile
     from polars.testing.parametric.strategies import (
         create_list_strategy,
         scalar_strategies,
     )
 else:
 
     def __getattr__(*args: Any, **kwargs: Any) -> Any:
@@ -20,12 +21,14 @@
             f"polars.testing.parametric.{args[0]} requires the 'hypothesis' module"
         ) from None
 
 
 __all__ = [
     "column",
     "columns",
-    "dataframes",
-    "series",
     "create_list_strategy",
+    "dataframes",
+    "load_profile",
     "scalar_strategies",
+    "series",
+    "set_profile",
 ]
```

### Comparing `polars_lts_cpu-0.17.7/polars/testing/parametric/primitives.py` & `polars_lts_cpu-0.17.8/polars/testing/parametric/primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     is_polars_dtype,
     py_type_to_dtype,
 )
 from polars.series import Series
 from polars.string_cache import StringCache
 from polars.testing.asserts import is_categorical_dtype
 from polars.testing.parametric.strategies import (
+    _hash,
     between,
     create_list_strategy,
     scalar_strategies,
 )
 
 if TYPE_CHECKING:
     from hypothesis.strategies import DrawFn, SearchStrategy
@@ -258,15 +259,15 @@
     allow_infinities: bool = True,
     unique: bool = False,
     chunked: bool | None = None,
     allowed_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
     excluded_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
 ) -> SearchStrategy[Series]:
     """
-    Strategy for producing a polars Series.
+    Hypothesis strategy for producing a polars Series.
 
     Parameters
     ----------
     name : {str, strategy}, optional
         literal string or a strategy for strings (or None), passed to the Series
         constructor name-param.
     dtype : PolarsDataType, optional
@@ -387,15 +388,15 @@
                 series_values = [None] * series_size
             else:
                 series_values = draw(
                     lists(
                         dtype_strategy,
                         min_size=series_size,
                         max_size=series_size,
-                        unique=unique,
+                        unique_by=(_hash if unique else None),
                     )
                 )
 
             # apply null values (custom frequency)
             if null_probability and null_probability != 1:
                 for idx in range(series_size):
                     if random.random() < null_probability:
@@ -434,15 +435,15 @@
     include_cols: Sequence[column] | None = None,
     null_probability: float | dict[str, float] = 0.0,
     allow_infinities: bool = True,
     allowed_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
     excluded_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
 ) -> SearchStrategy[DataFrame | LazyFrame]:
     """
-    Provides a strategy for producing a DataFrame or LazyFrame.
+    Hypothesis strategy for producing a polars DataFrame or LazyFrame.
 
     Parameters
     ----------
     cols : {int, columns}, optional
         integer number of columns to create, or a sequence of `column` objects
         that describe the desired DataFrame column data.
     lazy : bool, optional
@@ -538,15 +539,15 @@
         allowed_dtypes = [allowed_dtypes]
     if isinstance(excluded_dtypes, (DataType, DataTypeClass)):
         excluded_dtypes = [excluded_dtypes]
 
     selectable_dtypes = [
         dtype
         for dtype in (allowed_dtypes or strategy_dtypes)
-        if dtype not in (excluded_dtypes or ())
+        if dtype in strategy_dtypes and dtype not in (excluded_dtypes or ())
     ]
 
     @composite
     def draw_frames(draw: DrawFn) -> DataFrame | LazyFrame:
         """Reproducibly generate random DataFrames according to the given spec."""
         with StringCache():
             # if not given, create 'n' cols with random dtypes
```

### Comparing `polars_lts_cpu-0.17.7/polars/testing/parametric/strategies.py` & `polars_lts_cpu-0.17.8/polars/testing/parametric/strategies.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from random import choice
 from string import ascii_letters, ascii_uppercase, digits, punctuation
 from typing import TYPE_CHECKING, Any, Sequence
 
 from hypothesis.strategies import (
     booleans,
     characters,
+    composite,
     dates,
     datetimes,
     decimals,
     floats,
     from_type,
     integers,
     lists,
@@ -41,15 +42,17 @@
     UInt16,
     UInt32,
     UInt64,
     Utf8,
 )
 
 if TYPE_CHECKING:
-    from hypothesis.strategies import DrawFn
+    from decimal import Decimal as PyDecimal
+
+    from hypothesis.strategies import DrawFn, SearchStrategy
 
     from polars.type_aliases import PolarsDataType
 
 
 def between(draw: DrawFn, type_: type, min_: Any, max_: Any) -> Any:
     """Draw a value in a given range from a type-inferred strategy."""
     strategy_init = from_type(type_).function  # type: ignore[attr-defined]
@@ -66,24 +69,14 @@
 strategy_i32 = integers(min_value=-(2**31), max_value=(2**31) - 1)
 strategy_i64 = integers(min_value=-(2**63), max_value=(2**63) - 1)
 strategy_u8 = integers(min_value=0, max_value=(2**8) - 1)
 strategy_u16 = integers(min_value=0, max_value=(2**16) - 1)
 strategy_u32 = integers(min_value=0, max_value=(2**32) - 1)
 strategy_u64 = integers(min_value=0, max_value=(2**64) - 1)
 
-# TODO: once fixed, re-enable decimal nan/inf values.
-# TODO: vary the number of decimal places.
-strategy_decimal = decimals(
-    allow_nan=False,
-    allow_infinity=False,
-    min_value=-(2**66),
-    max_value=(2**66) - 1,
-    places=18,
-)
-
 strategy_ascii = text(max_size=8, alphabet=ascii_letters + digits + punctuation)
 strategy_categorical = text(max_size=2, alphabet=ascii_uppercase)
 strategy_utf8 = text(
     alphabet=characters(max_codepoint=1000, blacklist_categories=("Cs", "Cc")),
     max_size=8,
 )
 strategy_datetime_ns = datetimes(
@@ -97,15 +90,31 @@
 strategy_time = times()
 strategy_date = dates()
 strategy_duration = timedeltas(
     min_value=timedelta(microseconds=-(2**46)),
     max_value=timedelta(microseconds=(2**46) - 1),
 )
 
-scalar_strategies: dict[PolarsDataType, Any] = {
+
+@composite
+def strategy_decimal(draw: DrawFn) -> PyDecimal:
+    places = draw(integers(min_value=0, max_value=18))
+    return draw(
+        # TODO: once fixed, re-enable decimal nan/inf values.
+        decimals(
+            allow_nan=False,
+            allow_infinity=False,
+            min_value=-(2**66),
+            max_value=(2**66) - 1,
+            places=places,
+        )
+    )
+
+
+scalar_strategies: dict[PolarsDataType, SearchStrategy[Any]] = {
     Boolean: strategy_bool,
     Float32: strategy_f32,
     Float64: strategy_f64,
     Int8: strategy_i8,
     Int16: strategy_i16,
     Int32: strategy_i32,
     Int64: strategy_i64,
@@ -125,41 +134,43 @@
     Duration: strategy_duration,
     Categorical: strategy_categorical,
     Utf8: strategy_utf8,
 }
 
 # note: decimal support is in early development and requires opt-in
 if os.environ.get("POLARS_ACTIVATE_DECIMAL") == "1":
-    scalar_strategies[Decimal] = strategy_decimal
+    scalar_strategies[Decimal] = strategy_decimal()
 
 _strategy_dtypes = list(scalar_strategies) + [List]
 
 
 def _hash(elem: Any) -> int:
-    """Hashing that can also handle lists (for 'unique' check)."""
+    """Hashing that also handles lists/dicts (for 'unique' check)."""
     if isinstance(elem, list):
         return hash(tuple(_hash(e) for e in elem))
+    elif isinstance(elem, dict):
+        return hash((_hash(k), _hash(v)) for k, v in elem.items())
     return hash(elem)
 
 
 def create_list_strategy(
     inner_dtype: PolarsDataType | None,
     select_from: Sequence[Any] | None = None,
     size: int | None = None,
     min_size: int | None = None,
     max_size: int | None = None,
     unique: bool = False,
 ) -> Any:
     """
-    Create a List strategy for a given inner dtype.
+    Hypothesis strategy for producing polars List data.
 
     Parameters
     ----------
     inner_dtype : PolarsDataType
-        type of the inner list elements (can be another List).
+        type of the inner list elements (can also be another List).
     select_from : list, optional
         randomly select the innermost values from this list (otherwise
         the default strategy associated with the innermost dtype is used).
     size : int, optional
         if set, generated lists will be of exactly this size (and
         ignore the min_size/max_size params).
     min_size : int, optional
@@ -184,15 +195,15 @@
     ...     inner_dtype=pl.List(pl.Utf8),
     ...     select_from=["xx", "yy", "zz"],
     ... )
     >>> lst.example()  # doctest: +SKIP
     [['yy', 'xx'], [], ['zz']]
 
     Create a UInt8 dtype strategy as a hypothesis composite that generates
-     pairs of small int values where the first is always <= the second:
+    pairs of small int values where the first is always <= the second:
 
     >>> from hypothesis.strategies import composite
     >>>
     >>> @composite
     ... def uint8_pairs(draw, uints=create_list_strategy(pl.UInt8, size=2)):
     ...     pairs = list(zip(draw(uints), draw(uints)))
     ...     return [sorted(ints) for ints in pairs]
```

### Comparing `polars_lts_cpu-0.17.7/polars/type_aliases.py` & `polars_lts_cpu-0.17.8/polars/type_aliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,7 +159,10 @@
 ]
 RowTotalsDefinition: TypeAlias = Union[
     # dict of colname to str(s), a collection of str, or a boolean
     Mapping[str, Union[str, Collection[str]]],
     Collection[str],
     bool,
 ]
+
+# standard/named hypothesis profiles used for parametric testing
+ParametricProfileNames: TypeAlias = Literal["fast", "balanced", "expensive"]
```

### Comparing `polars_lts_cpu-0.17.7/polars/utils/__init__.py` & `polars_lts_cpu-0.17.8/polars/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/_construction.py` & `polars_lts_cpu-0.17.8/polars/utils/_construction.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/_parse_expr_input.py` & `polars_lts_cpu-0.17.8/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/_scan.py` & `polars_lts_cpu-0.17.8/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/_wrap.py` & `polars_lts_cpu-0.17.8/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/build_info.py` & `polars_lts_cpu-0.17.8/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/convert.py` & `polars_lts_cpu-0.17.8/polars/utils/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/decorators.py` & `polars_lts_cpu-0.17.8/polars/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/meta.py` & `polars_lts_cpu-0.17.8/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/polars_version.py` & `polars_lts_cpu-0.17.8/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/show_versions.py` & `polars_lts_cpu-0.17.8/polars/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/polars/utils/various.py` & `polars_lts_cpu-0.17.8/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/pyproject.toml` & `polars_lts_cpu-0.17.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/requirements-dev.txt` & `polars_lts_cpu-0.17.8/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 tzdata; platform_system == 'Windows'
 xlsx2csv
 XlsxWriter
 adbc_driver_sqlite; python_version >= '3.9' and platform_system != 'Windows'
 connectorx==0.3.2a2; python_version >= '3.8'  # Latest full release is broken - unpin when 0.3.2 released
 
 # Tooling
-hypothesis==6.72.0
+hypothesis==6.72.1
 maturin==0.14.10
 pytest==7.3.0
 pytest-cov==4.0.0
 pytest-xdist==3.2.0
 
 # Stub files
 pandas-stubs==1.2.0.62
```

### Comparing `polars_lts_cpu-0.17.7/scripts/check_stacklevels.py` & `polars_lts_cpu-0.17.8/scripts/check_stacklevels.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/apply/dataframe.rs` & `polars_lts_cpu-0.17.8/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/apply/mod.rs` & `polars_lts_cpu-0.17.8/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/apply/series.rs` & `polars_lts_cpu-0.17.8/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/arrow_interop/to_py.rs` & `polars_lts_cpu-0.17.8/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/arrow_interop/to_rust.rs` & `polars_lts_cpu-0.17.8/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/batched_csv.rs` & `polars_lts_cpu-0.17.8/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/conversion.rs` & `polars_lts_cpu-0.17.8/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/dataframe.rs` & `polars_lts_cpu-0.17.8/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/datatypes.rs` & `polars_lts_cpu-0.17.8/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/error.rs` & `polars_lts_cpu-0.17.8/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/file.rs` & `polars_lts_cpu-0.17.8/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/lazy/apply.rs` & `polars_lts_cpu-0.17.8/src/lazy/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/lazy/dataframe.rs` & `polars_lts_cpu-0.17.8/src/lazy/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/lazy/dsl.rs` & `polars_lts_cpu-0.17.8/src/lazy/dsl.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1113,14 +1113,22 @@
         self.inner.clone().dt().tz_localize(time_zone).into()
     }
 
     pub fn dt_truncate(&self, every: &str, offset: &str) -> PyExpr {
         self.inner.clone().dt().truncate(every, offset).into()
     }
 
+    pub fn dt_month_start(&self) -> PyExpr {
+        self.inner.clone().dt().month_start().into()
+    }
+
+    pub fn dt_month_end(&self) -> PyExpr {
+        self.inner.clone().dt().month_end().into()
+    }
+
     pub fn dt_round(&self, every: &str, offset: &str) -> PyExpr {
         self.inner.clone().dt().round(every, offset).into()
     }
 
     pub fn dt_combine(&self, time: PyExpr, time_unit: Wrap<TimeUnit>) -> PyExpr {
         self.inner
             .clone()
@@ -1356,15 +1364,14 @@
         window_size: &str,
         weights: Option<Vec<f64>>,
         min_periods: usize,
         center: bool,
         by: Option<String>,
         closed: Option<Wrap<ClosedWindow>>,
     ) -> Self {
-        dbg!(window_size);
         let options = RollingOptions {
             window_size: Duration::parse(window_size),
             weights,
             min_periods,
             center,
             by,
             closed_window: closed.map(|c| c.0),
```

### Comparing `polars_lts_cpu-0.17.7/src/lazy/meta.rs` & `polars_lts_cpu-0.17.8/src/lazy/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/lazy/mod.rs` & `polars_lts_cpu-0.17.8/src/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/lib.rs` & `polars_lts_cpu-0.17.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/npy.rs` & `polars_lts_cpu-0.17.8/src/npy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/object.rs` & `polars_lts_cpu-0.17.8/src/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/series.rs` & `polars_lts_cpu-0.17.8/src/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/set.rs` & `polars_lts_cpu-0.17.8/src/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/sql.rs` & `polars_lts_cpu-0.17.8/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/src/utils.rs` & `polars_lts_cpu-0.17.8/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/README.md` & `polars_lts_cpu-0.17.8/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/benchmark/groupby-datagen.R` & `polars_lts_cpu-0.17.8/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/benchmark/run_h2oai_benchmark.py` & `polars_lts_cpu-0.17.8/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/benchmark/test_release.py` & `polars_lts_cpu-0.17.8/tests/benchmark/test_release.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/docs/run_doctest.py` & `polars_lts_cpu-0.17.8/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/parametric/test_dataframe.py` & `polars_lts_cpu-0.17.8/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/parametric/test_lazyframe.py` & `polars_lts_cpu-0.17.8/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/parametric/test_series.py` & `polars_lts_cpu-0.17.8/tests/parametric/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/parametric/test_testing.py` & `polars_lts_cpu-0.17.8/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/conftest.py` & `polars_lts_cpu-0.17.8/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/datatypes/test_bool.py` & `polars_lts_cpu-0.17.8/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/datatypes/test_categorical.py` & `polars_lts_cpu-0.17.8/tests/unit/datatypes/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/datatypes/test_decimal.py` & `polars_lts_cpu-0.17.8/tests/unit/datatypes/test_decimal.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,18 +70,21 @@
         .strip()[1:-1]
         .split()
     )
     assert formatted == dec_strs
 
 
 def test_init_decimal_dtype() -> None:
-    _ = pl.Series("a", [D("-0.01"), D("1.2345678"), D("500")], dtype=pl.Decimal)
-    _ = pl.DataFrame(
+    s = pl.Series("a", [D("-0.01"), D("1.2345678"), D("500")], dtype=pl.Decimal)
+    assert s.is_numeric()
+
+    df = pl.DataFrame(
         {"a": [D("-0.01"), D("1.2345678"), D("500")]}, schema={"a": pl.Decimal}
     )
+    assert df["a"].is_numeric()
 
 
 def test_decimal_cast() -> None:
     df = pl.DataFrame(
         {
             "decimals": [
                 D("2"),
```

### Comparing `polars_lts_cpu-0.17.7/tests/unit/datatypes/test_list.py` & `polars_lts_cpu-0.17.8/tests/unit/datatypes/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/datatypes/test_object.py` & `polars_lts_cpu-0.17.8/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/datatypes/test_struct.py` & `polars_lts_cpu-0.17.8/tests/unit/datatypes/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/datatypes/test_temporal.py` & `polars_lts_cpu-0.17.8/tests/unit/datatypes/test_temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -2754,15 +2754,18 @@
     parsed = pl.Series([time_string]).str.strptime(pl.Date)
     assert parsed.dt.year().item() == 2134
     assert parsed.dt.month().item() == 12
     assert parsed.dt.day().item() == 13
 
 
 def test_series_is_temporal() -> None:
-    for tp in TEMPORAL_DTYPES:
+    for tp in TEMPORAL_DTYPES | {
+        pl.Datetime("ms", "UTC"),
+        pl.Datetime("ns", "Europe/Amsterdam"),
+    }:
         s = pl.Series([None], dtype=tp)
         assert s.is_temporal() is True
 
     s = pl.Series([datetime(2023, 2, 14, 11, 12, 13)], dtype=pl.Datetime)
     for tp in (pl.Datetime, [pl.Datetime], [pl.Time, pl.Datetime]):  # type: ignore[assignment]
         assert s.is_temporal(excluding=tp) is False
```

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_lts_cpu-0.17.8/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/example.xlsx` & `polars_lts_cpu-0.17.8/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/foods1.ipc` & `polars_lts_cpu-0.17.8/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/foods1.ndjson` & `polars_lts_cpu-0.17.8/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/foods1.parquet` & `polars_lts_cpu-0.17.8/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/foods2.ipc` & `polars_lts_cpu-0.17.8/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/foods2.ndjson` & `polars_lts_cpu-0.17.8/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/foods2.parquet` & `polars_lts_cpu-0.17.8/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/files/small.parquet` & `polars_lts_cpu-0.17.8/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_avro.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_csv.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_database.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_delta.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_excel.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_ipc.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_json.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_lazy_csv.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_lazy_ipc.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_lazy_json.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_lazy_parquet.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_other.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_parquet.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_pickle.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/io/test_pyarrow_dataset.py` & `polars_lts_cpu-0.17.8/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/namespaces/test_binary.py` & `polars_lts_cpu-0.17.8/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/namespaces/test_categorical.py` & `polars_lts_cpu-0.17.8/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/namespaces/test_datetime.py` & `polars_lts_cpu-0.17.8/tests/unit/namespaces/test_datetime.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
-from datetime import date, datetime, time, timedelta
+from datetime import date, datetime, time, timedelta, timezone
 from typing import TYPE_CHECKING
 
 import pytest
 
 import polars as pl
 from polars.datatypes import DTYPE_TEMPORAL_UNITS
-from polars.exceptions import ComputeError
+from polars.exceptions import ComputeError, InvalidOperationError
 from polars.testing import assert_series_equal
 
 if TYPE_CHECKING:
     from polars.type_aliases import TimeUnit
 import sys
 
 from polars.dependencies import _ZONEINFO_AVAILABLE
@@ -123,14 +123,105 @@
     with pytest.raises(ComputeError, match="expected Datetime"):
         pl.Series([timedelta(1)]).dt.datetime()
     with pytest.raises(ComputeError, match="expected Datetime, Date, or Time"):
         pl.Series([timedelta(1)]).dt.time()
 
 
 @pytest.mark.parametrize(
+    ("dt", "expected"),
+    [
+        (datetime(2022, 3, 15, 3), datetime(2022, 3, 1, 3)),
+        (datetime(2022, 3, 15, 3, 2, 1, 123000), datetime(2022, 3, 1, 3, 2, 1, 123000)),
+        (datetime(2022, 3, 15), datetime(2022, 3, 1)),
+        (datetime(2022, 3, 1), datetime(2022, 3, 1)),
+    ],
+)
+@pytest.mark.parametrize(
+    "tzinfo", [None, ZoneInfo("Asia/Kathmandu"), timezone(timedelta(hours=1))]
+)
+@pytest.mark.parametrize("time_unit", ["ms", "us", "ns"])
+def test_month_start_datetime(
+    dt: datetime,
+    expected: datetime,
+    time_unit: TimeUnit,
+    tzinfo: ZoneInfo | timezone | None,
+) -> None:
+    ser = pl.Series([dt.replace(tzinfo=tzinfo)]).dt.cast_time_unit(time_unit)
+    result = ser.dt.month_start().item()
+    assert result == expected.replace(tzinfo=tzinfo)
+
+
+@pytest.mark.parametrize(
+    ("dt", "expected"),
+    [
+        (date(2022, 3, 15), date(2022, 3, 1)),
+        (date(2022, 3, 31), date(2022, 3, 1)),
+    ],
+)
+def test_month_start_date(dt: date, expected: date) -> None:
+    ser = pl.Series([dt])
+    result = ser.dt.month_start().item()
+    assert result == expected
+
+
+@pytest.mark.parametrize(
+    ("dt", "expected"),
+    [
+        (datetime(2022, 3, 15, 3), datetime(2022, 3, 31, 3)),
+        (
+            datetime(2022, 3, 15, 3, 2, 1, 123000),
+            datetime(2022, 3, 31, 3, 2, 1, 123000),
+        ),
+        (datetime(2022, 3, 15), datetime(2022, 3, 31)),
+        (datetime(2022, 3, 31), datetime(2022, 3, 31)),
+    ],
+)
+@pytest.mark.parametrize(
+    "tzinfo", [None, ZoneInfo("Asia/Kathmandu"), timezone(timedelta(hours=1))]
+)
+@pytest.mark.parametrize("time_unit", ["ms", "us", "ns"])
+def test_month_end_datetime(
+    dt: datetime,
+    expected: datetime,
+    time_unit: TimeUnit,
+    tzinfo: ZoneInfo | timezone | None,
+) -> None:
+    ser = pl.Series([dt.replace(tzinfo=tzinfo)]).dt.cast_time_unit(time_unit)
+    result = ser.dt.month_end().item()
+    assert result == expected.replace(tzinfo=tzinfo)
+
+
+@pytest.mark.parametrize(
+    ("dt", "expected"),
+    [
+        (date(2022, 3, 15), date(2022, 3, 31)),
+        (date(2022, 3, 31), date(2022, 3, 31)),
+    ],
+)
+def test_month_end_date(dt: date, expected: date) -> None:
+    ser = pl.Series([dt])
+    result = ser.dt.month_end().item()
+    assert result == expected
+
+
+def test_month_start_end_invalid() -> None:
+    ser = pl.Series([time(1, 2, 3)])
+    with pytest.raises(
+        InvalidOperationError,
+        match=r"`month_start` operation not supported for dtype `time` \(expected: date/datetime\)",
+    ):
+        ser.dt.month_start()
+    with pytest.raises(
+        InvalidOperationError,
+        match=r"`month_end` operation not supported for dtype `time` \(expected: date/datetime\)",
+    ):
+        ser.dt.month_end()
+
+
+@pytest.mark.parametrize(
     ("time_unit", "expected"),
     [
         ("d", pl.Series(values=[18262, 18294], dtype=pl.Int32)),
         ("s", pl.Series(values=[1_577_836_800, 1_580_613_610], dtype=pl.Int64)),
         (
             "ms",
             pl.Series(values=[1_577_836_800_000, 1_580_613_610_000], dtype=pl.Int64),
@@ -429,14 +520,27 @@
 def test_offset_by_crossing_dst(time_zone: str | None) -> None:
     ser = pl.Series([datetime(2021, 11, 7)]).dt.replace_time_zone(time_zone)
     result = ser.dt.offset_by("1d")
     expected = pl.Series([datetime(2021, 11, 8)]).dt.replace_time_zone(time_zone)
     assert_series_equal(result, expected)
 
 
+def test_negative_offset_by_err_msg_8464() -> None:
+    with pytest.raises(
+        ComputeError, match=r"cannot advance '2022-03-30 00:00:00' by -1 month\(s\)"
+    ):
+        pl.Series([datetime(2022, 3, 30)]).dt.offset_by("-1mo")
+
+
+def test_offset_by_saturating_8217() -> None:
+    result = pl.Series([date(2018, 1, 31)]).dt.offset_by("1mo_saturating").item()
+    expected = date(2018, 2, 28)
+    assert result == expected
+
+
 def test_year_empty_df() -> None:
     df = pl.DataFrame(pl.Series(name="date", dtype=pl.Date))
     assert df.select(pl.col("date").dt.year()).dtypes == [pl.Int32]
 
 
 @pytest.mark.parametrize(
     "time_unit",
```

### Comparing `polars_lts_cpu-0.17.7/tests/unit/namespaces/test_list.py` & `polars_lts_cpu-0.17.8/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/namespaces/test_meta.py` & `polars_lts_cpu-0.17.8/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/namespaces/test_string.py` & `polars_lts_cpu-0.17.8/tests/unit/namespaces/test_string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/namespaces/test_strptime.py` & `polars_lts_cpu-0.17.8/tests/unit/namespaces/test_strptime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/namespaces/test_struct.py` & `polars_lts_cpu-0.17.8/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_aggregations.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_apply.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_arithmetic.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_comparison.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_drop.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_explode.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_filter.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_folds.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_groupby.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_is_in.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_is_in.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_join.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_join_asof.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_join_asof.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_melt.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_pivot.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_rolling.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_sort.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_sort.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_statistics.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_statistics.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_transpose.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_unique.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/operations/test_window.py` & `polars_lts_cpu-0.17.8/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_api.py` & `polars_lts_cpu-0.17.8/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_arity.py` & `polars_lts_cpu-0.17.8/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_cfg.py` & `polars_lts_cpu-0.17.8/tests/unit/test_cfg.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_constructors.py` & `polars_lts_cpu-0.17.8/tests/unit/test_constructors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_cse.py` & `polars_lts_cpu-0.17.8/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_datatypes.py` & `polars_lts_cpu-0.17.8/tests/unit/test_datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,43 +3,49 @@
 import pickle
 from datetime import datetime, timedelta
 
 import pytest
 
 import polars as pl
 from polars import datatypes
+from polars.datatypes import (
+    DTYPE_TEMPORAL_UNITS,
+    DataTypeClass,
+    DataTypeGroup,
+    py_type_to_dtype,
+)
 
 
 def test_dtype_init_equivalence() -> None:
     # check "DataType.__new__" behaviour for all datatypes
     all_datatypes = {
         dtype
         for dtype in (getattr(datatypes, attr) for attr in dir(datatypes))
-        if isinstance(dtype, datatypes.DataTypeClass)
+        if isinstance(dtype, DataTypeClass)
     }
     for dtype in all_datatypes:
         assert dtype == dtype()
 
 
 def test_dtype_temporal_units() -> None:
     # check (in)equality behaviour of temporal types that take units
-    for time_unit in datatypes.DTYPE_TEMPORAL_UNITS:
+    for time_unit in DTYPE_TEMPORAL_UNITS:
         assert pl.Datetime == pl.Datetime(time_unit)
         assert pl.Duration == pl.Duration(time_unit)
 
         assert pl.Datetime(time_unit) == pl.Datetime()
         assert pl.Duration(time_unit) == pl.Duration()
 
     assert pl.Datetime("ms") != pl.Datetime("ns")
     assert pl.Duration("ns") != pl.Duration("us")
 
     # check timeunit from pytype
     for inferred_dtype, expected_dtype in (
-        (datatypes.py_type_to_dtype(datetime), pl.Datetime),
-        (datatypes.py_type_to_dtype(timedelta), pl.Duration),
+        (py_type_to_dtype(datetime), pl.Datetime),
+        (py_type_to_dtype(timedelta), pl.Duration),
     ):
         assert inferred_dtype == expected_dtype
         assert inferred_dtype.time_unit == "us"  # type: ignore[union-attr]
 
     with pytest.raises(ValueError, match="Invalid time_unit"):
         pl.Datetime("?")  # type: ignore[arg-type]
 
@@ -54,14 +60,22 @@
         pl.Struct([pl.Field("a", pl.Int64), pl.Field("b", pl.Boolean)]).base_type()
         is pl.Struct
     )
     for dtype in pl.DATETIME_DTYPES:
         assert dtype.base_type() is pl.Datetime
 
 
+def test_dtype_groups() -> None:
+    grp = DataTypeGroup([pl.Datetime], match_base_type=False)
+    assert pl.Datetime("ms", "Asia/Tokyo") not in grp
+
+    grp = DataTypeGroup([pl.Datetime])
+    assert pl.Datetime("ms", "Asia/Tokyo") in grp
+
+
 def test_get_index_type() -> None:
     assert pl.get_index_type() == pl.UInt32
 
 
 def test_dtypes_picklable() -> None:
     parametric_type = pl.Datetime("ns")
     singleton_type = pl.Float64
```

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_df.py` & `polars_lts_cpu-0.17.8/tests/unit/test_df.py`

 * *Files 1% similar despite different names*

```diff
@@ -1295,15 +1295,22 @@
             ("mean", 1.3333333333333333, None, None),
             ("std", 0.5773502691896257, None, None),
             ("min", 1.0, None, None),
             ("max", 2.0, None, None),
             ("median", 1.0, None, None),
         ]
 
-    assert df.describe(percentiles=(0.2, 0.4, 0.6, 0.8)).rows() == [
+    described = df.describe(percentiles=(0.2, 0.4, 0.6, 0.8))
+    assert described.schema == {
+        "describe": pl.Utf8,
+        "numerical": pl.Float64,
+        "struct": pl.Utf8,
+        "list": pl.Utf8,
+    }
+    assert described.rows() == [
         ("count", 4.0, "4", "4"),
         ("null_count", 1.0, "1", "1"),
         ("mean", 1.3333333333333333, None, None),
         ("std", 0.5773502691896257, None, None),
         ("min", 1.0, None, None),
         ("max", 2.0, None, None),
         ("median", 1.0, None, None),
```

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_empty.py` & `polars_lts_cpu-0.17.8/tests/unit/test_empty.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_errors.py` & `polars_lts_cpu-0.17.8/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_expr_multi_cols.py` & `polars_lts_cpu-0.17.8/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_exprs.py` & `polars_lts_cpu-0.17.8/tests/unit/test_exprs.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_fmt.py` & `polars_lts_cpu-0.17.8/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_functions.py` & `polars_lts_cpu-0.17.8/tests/unit/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_interchange.py` & `polars_lts_cpu-0.17.8/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_interop.py` & `polars_lts_cpu-0.17.8/tests/unit/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_lazy.py` & `polars_lts_cpu-0.17.8/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_polars_import.py` & `polars_lts_cpu-0.17.8/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_predicates.py` & `polars_lts_cpu-0.17.8/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_projections.py` & `polars_lts_cpu-0.17.8/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_queries.py` & `polars_lts_cpu-0.17.8/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_rows.py` & `polars_lts_cpu-0.17.8/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_schema.py` & `polars_lts_cpu-0.17.8/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_serde.py` & `polars_lts_cpu-0.17.8/tests/unit/test_serde.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_series.py` & `polars_lts_cpu-0.17.8/tests/unit/test_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,18 +466,44 @@
     a = pl.Series("a", [2, 1, 4])
     a.sort(in_place=True)
     assert_series_equal(a, pl.Series("a", [1, 2, 4]))
     a = pl.Series("a", [2, 1, 1, 4, 4, 4])
     assert_series_equal(a.arg_unique(), pl.Series("a", [0, 1, 3], dtype=UInt32))
 
     assert_series_equal(a.take([2, 3]), pl.Series("a", [1, 4]))
-    assert a.is_numeric()
 
-    a = pl.Series("bool", [True, False])
-    assert not a.is_numeric()
+
+def test_series_dtype_is() -> None:
+    s = pl.Series("s", [1, 2, 3])
+
+    assert s.is_numeric()
+    assert s.is_integer()
+    assert s.is_integer(signed=True)
+    assert not s.is_integer(signed=False)
+    assert (s * 0.99).is_float()
+
+    s = pl.Series("s", [1, 2, 3], dtype=pl.UInt8)
+    assert s.is_numeric()
+    assert s.is_integer()
+    assert not s.is_integer(signed=True)
+    assert s.is_integer(signed=False)
+
+    s = pl.Series("bool", [True, None, False])
+    assert not s.is_numeric()
+
+    s = pl.Series("s", ["testing..."])
+    assert s.is_utf8()
+
+    s = pl.Series("s", [], dtype=pl.Decimal(20, 15))
+    assert not s.is_float()
+    assert s.is_numeric()
+    assert s.is_empty()
+
+    s = pl.Series("s", [], dtype=pl.Datetime("ms", time_zone="UTC"))
+    assert s.is_temporal()
 
 
 def test_series_head_tail_limit() -> None:
     s = pl.Series(range(10))
 
     assert_series_equal(s.head(5), pl.Series(range(5)))
     assert_series_equal(s.limit(5), s.head(5))
```

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_sql.py` & `polars_lts_cpu-0.17.8/tests/unit/test_sql.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_streaming.py` & `polars_lts_cpu-0.17.8/tests/unit/test_streaming.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/test_testing.py` & `polars_lts_cpu-0.17.8/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/tests/unit/utils/test_utils.py` & `polars_lts_cpu-0.17.8/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.7/Cargo.lock` & `polars_lts_cpu-0.17.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -527,34 +527,14 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
-name = "dirs"
-version = "5.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dece029acd3353e3a58ac2e3eb3c8d6c35827a892edc6cc4138ef9c33df46ecd"
-dependencies = [
- "dirs-sys",
-]
-
-[[package]]
-name = "dirs-sys"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04414300db88f70d74c5ff54e50f9e1d1737d9a5b90f53fcf2e95ca2a9ab554b"
-dependencies = [
- "libc",
- "redox_users",
- "windows-sys",
-]
-
-[[package]]
 name = "dyn-clone"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
 
 [[package]]
 name = "either"
@@ -824,14 +804,23 @@
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
+name = "home"
+version = "0.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "747309b4b440c06d57b0b25f2aee03ee9b5e5397d288c60e21fc709bb98a7408"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "iana-time-zone"
 version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
@@ -1571,18 +1560,18 @@
 dependencies = [
  "ahash",
  "arrow2",
  "async-trait",
  "bytes",
  "chrono",
  "chrono-tz",
- "dirs",
  "fast-float",
  "flate2",
  "futures",
+ "home",
  "lexical",
  "lexical-core",
  "memchr",
  "memmap2",
  "num-traits",
  "once_cell",
  "polars-arrow",
@@ -1744,15 +1733,15 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.17.7"
+version = "0.17.8"
 dependencies = [
  "ahash",
  "built",
  "ciborium",
  "jemallocator",
  "lexical-core",
  "libc",
@@ -1921,25 +1910,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "redox_users"
-version = "0.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
-dependencies = [
- "getrandom",
- "redox_syscall",
- "thiserror",
-]
-
-[[package]]
 name = "regex"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac6cf59af1067a3fb53fbe5c88c053764e930f932be1d71d3ffe032cbe147f59"
 dependencies = [
  "aho-corasick",
  "memchr",
```

### Comparing `polars_lts_cpu-0.17.7/PKG-INFO` & `polars_lts_cpu-0.17.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-lts-cpu
-Version: 0.17.7
+Version: 0.17.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -14,50 +14,50 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: typing_extensions >= 4.0.1; python_version < '3.11'
 Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
+Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
 Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
-Requires-Dist: connectorx; extra == 'connectorx'
 Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
-Requires-Dist: matplotlib; extra == 'matplotlib'
-Requires-Dist: fsspec; extra == 'fsspec'
-Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
-Requires-Dist: pandas; extra == 'sqlalchemy'
-Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
+Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
 Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
 Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra == 'timezone'
 Requires-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone'
-Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
-Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
+Requires-Dist: matplotlib; extra == 'matplotlib'
+Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
+Requires-Dist: pandas; extra == 'sqlalchemy'
+Requires-Dist: connectorx; extra == 'connectorx'
+Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
+Requires-Dist: fsspec; extra == 'fsspec'
 Provides-Extra: numpy
+Provides-Extra: xlsx2csv
 Provides-Extra: pyarrow
-Provides-Extra: connectorx
 Provides-Extra: deltalake
+Provides-Extra: xlsxwriter
+Provides-Extra: pandas
+Provides-Extra: timezone
 Provides-Extra: matplotlib
-Provides-Extra: fsspec
 Provides-Extra: sqlalchemy
+Provides-Extra: connectorx
 Provides-Extra: all
-Provides-Extra: pandas
-Provides-Extra: timezone
-Provides-Extra: xlsxwriter
-Provides-Extra: xlsx2csv
+Provides-Extra: fsspec
 License-File: LICENSE
 Summary: Blazingly fast DataFrame library
 Keywords: dataframe,arrow,out-of-core
 Author-email: Ritchie Vink <ritchie46@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Changelog, https://github.com/pola-rs/polars/releases
 Project-URL: Homepage, https://www.pola.rs/
 Project-URL: Repository, https://github.com/pola-rs/polars
 Project-URL: Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/index.html
+Project-URL: Changelog, https://github.com/pola-rs/polars/releases
 
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/polars_github_logo_rect_dark_name.svg">
   <br>
 </h1>
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.7 Classifier:
+Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.8 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Rust Classifier: Topic ::
 Scientific/Engineering Requires-Dist: typing_extensions >= 4.0.1;
 python_version < '3.11' Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
-Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist: connectorx;
-extra == 'connectorx' Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
-Requires-Dist: matplotlib; extra == 'matplotlib' Requires-Dist: fsspec; extra
-== 'fsspec' Requires-Dist: sqlalchemy; extra == 'sqlalchemy' Requires-Dist:
-pandas; extra == 'sqlalchemy' Requires-Dist: polars
+Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv' Requires-Dist:
+pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist: deltalake >= 0.8.0; extra ==
+'deltalake' Requires-Dist: xlsxwriter; extra == 'xlsxwriter' Requires-Dist:
+pyarrow>=7.0.0; extra == 'pandas' Requires-Dist: pandas; extra == 'pandas'
+Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra ==
+'timezone' Requires-Dist: tzdata; (platform_system == 'Windows') and extra ==
+'timezone' Requires-Dist: matplotlib; extra == 'matplotlib' Requires-Dist:
+sqlalchemy; extra == 'sqlalchemy' Requires-Dist: pandas; extra == 'sqlalchemy'
+Requires-Dist: connectorx; extra == 'connectorx' Requires-Dist: polars
 [pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter];
-extra == 'all' Requires-Dist: pyarrow>=7.0.0; extra == 'pandas' Requires-Dist:
-pandas; extra == 'pandas' Requires-Dist: backports.zoneinfo; (python_version <
-'3.9') and extra == 'timezone' Requires-Dist: tzdata; (platform_system ==
-'Windows') and extra == 'timezone' Requires-Dist: xlsxwriter; extra ==
-'xlsxwriter' Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv' Provides-
-Extra: numpy Provides-Extra: pyarrow Provides-Extra: connectorx Provides-Extra:
-deltalake Provides-Extra: matplotlib Provides-Extra: fsspec Provides-Extra:
-sqlalchemy Provides-Extra: all Provides-Extra: pandas Provides-Extra: timezone
-Provides-Extra: xlsxwriter Provides-Extra: xlsx2csv License-File: LICENSE
+extra == 'all' Requires-Dist: fsspec; extra == 'fsspec' Provides-Extra: numpy
+Provides-Extra: xlsx2csv Provides-Extra: pyarrow Provides-Extra: deltalake
+Provides-Extra: xlsxwriter Provides-Extra: pandas Provides-Extra: timezone
+Provides-Extra: matplotlib Provides-Extra: sqlalchemy Provides-Extra:
+connectorx Provides-Extra: all Provides-Extra: fsspec License-File: LICENSE
 Summary: Blazingly fast DataFrame library Keywords: dataframe,arrow,out-of-core
 Author-email: Ritchie Vink
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Changelog, https://github.com/pola-rs/
-polars/releases Project-URL: Homepage, https://www.pola.rs/ Project-URL:
-Repository, https://github.com/pola-rs/polars Project-URL: Documentation,
-https://pola-rs.github.io/polars/py-polars/html/reference/index.html
+charset=UTF-8; variant=GFM Project-URL: Homepage, https://www.pola.rs/ Project-
+URL: Repository, https://github.com/pola-rs/polars Project-URL: Documentation,
+https://pola-rs.github.io/polars/py-polars/html/reference/index.html Project-
+URL: Changelog, https://github.com/pola-rs/polars/releases
  ****** [https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/
                     polars_github_logo_rect_dark_name.svg]
                                      ******
 [rust_docs] [Build_and_test] [https://img.shields.io/crates/v/polars.svg] [PyPi
  Latest_Release] [NPM_Latest_Release] [R-universe_Latest_Release] [DOI_Latest
                                    Release]
   Documentation: Python - Rust - Node.js - R | StackOverflow: Python - Rust -
```

