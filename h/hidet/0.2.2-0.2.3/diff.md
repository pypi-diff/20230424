# Comparing `tmp/hidet-0.2.2-py3-none-any.whl.zip` & `tmp/hidet-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,308 +1,320 @@
-Zip file size: 530703 bytes, number of entries: 306
--rwxr-xr-x  2.0 unx     7123 b- defN 23-Mar-24 01:21 libhidet.so
--rwxr-xr-x  2.0 unx    55385 b- defN 23-Mar-24 01:21 libhidet_runtime.so
--rw-r--r--  2.0 unx     1673 b- defN 23-Mar-24 01:21 hidet/__init__.py
--rw-r--r--  2.0 unx     2797 b- defN 23-Mar-24 01:21 hidet/array_api.py
--rw-r--r--  2.0 unx    10611 b- defN 23-Mar-24 01:21 hidet/driver.py
--rw-r--r--  2.0 unx     2178 b- defN 23-Mar-24 01:21 hidet/libinfo.py
--rw-r--r--  2.0 unx     2039 b- defN 23-Mar-24 01:21 hidet/logging.py
--rw-r--r--  2.0 unx    13706 b- defN 23-Mar-24 01:21 hidet/option.py
--rw-r--r--  2.0 unx      566 b- defN 23-Mar-24 01:21 hidet/version.py
--rw-r--r--  2.0 unx      745 b- defN 23-Mar-24 01:21 hidet/backend/__init__.py
--rw-r--r--  2.0 unx     8609 b- defN 23-Mar-24 01:21 hidet/backend/build.py
--rw-r--r--  2.0 unx    27422 b- defN 23-Mar-24 01:21 hidet/backend/codegen.py
--rw-r--r--  2.0 unx      564 b- defN 23-Mar-24 01:21 hidet/cli/__init__.py
--rw-r--r--  2.0 unx      875 b- defN 23-Mar-24 01:21 hidet/cli/main.py
--rw-r--r--  2.0 unx      887 b- defN 23-Mar-24 01:21 hidet/cli/bench/__init__.py
--rw-r--r--  2.0 unx     1667 b- defN 23-Mar-24 01:21 hidet/cli/bench/bench.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Mar-24 01:21 hidet/cli/bench/bench_all.py
--rw-r--r--  2.0 unx     1020 b- defN 23-Mar-24 01:21 hidet/cli/bench/bench_common.py
--rw-r--r--  2.0 unx     4859 b- defN 23-Mar-24 01:21 hidet/cli/bench/model.py
--rw-r--r--  2.0 unx      574 b- defN 23-Mar-24 01:21 hidet/cli/bench/nlp/__init__.py
--rw-r--r--  2.0 unx     2547 b- defN 23-Mar-24 01:21 hidet/cli/bench/nlp/models.py
--rw-r--r--  2.0 unx     1487 b- defN 23-Mar-24 01:21 hidet/cli/bench/nlp/nlp_model.py
--rw-r--r--  2.0 unx      702 b- defN 23-Mar-24 01:21 hidet/cli/bench/vision/__init__.py
--rw-r--r--  2.0 unx     1781 b- defN 23-Mar-24 01:21 hidet/cli/bench/vision/inception_v3.py
--rw-r--r--  2.0 unx     1781 b- defN 23-Mar-24 01:21 hidet/cli/bench/vision/mobilenet_v2.py
--rw-r--r--  2.0 unx     2464 b- defN 23-Mar-24 01:21 hidet/cli/bench/vision/resnet.py
--rw-r--r--  2.0 unx     2342 b- defN 23-Mar-24 01:21 hidet/cli/bench/vision/resnext.py
--rw-r--r--  2.0 unx     1269 b- defN 23-Mar-24 01:21 hidet/cli/bench/vision/vision_model.py
--rw-r--r--  2.0 unx     1034 b- defN 23-Mar-24 01:21 hidet/cuda/__init__.py
--rw-r--r--  2.0 unx     4572 b- defN 23-Mar-24 01:21 hidet/cuda/device.py
--rw-r--r--  2.0 unx     4171 b- defN 23-Mar-24 01:21 hidet/cuda/event.py
--rw-r--r--  2.0 unx     8203 b- defN 23-Mar-24 01:21 hidet/cuda/graph.py
--rw-r--r--  2.0 unx     7460 b- defN 23-Mar-24 01:21 hidet/cuda/memory.py
--rw-r--r--  2.0 unx     7709 b- defN 23-Mar-24 01:21 hidet/cuda/stream.py
--rw-r--r--  2.0 unx      695 b- defN 23-Mar-24 01:21 hidet/ffi/__init__.py
--rw-r--r--  2.0 unx     2496 b- defN 23-Mar-24 01:21 hidet/ffi/callbacks.py
--rw-r--r--  2.0 unx     3079 b- defN 23-Mar-24 01:21 hidet/ffi/ffi.py
--rw-r--r--  2.0 unx     6540 b- defN 23-Mar-24 01:21 hidet/ffi/packedfunc.py
--rw-r--r--  2.0 unx     1766 b- defN 23-Mar-24 01:21 hidet/ffi/runtime_api.py
--rw-r--r--  2.0 unx     3427 b- defN 23-Mar-24 01:21 hidet/ffi/shared_lib.py
--rw-r--r--  2.0 unx     1240 b- defN 23-Mar-24 01:21 hidet/graph/__init__.py
--rw-r--r--  2.0 unx      672 b- defN 23-Mar-24 01:21 hidet/graph/common.py
--rw-r--r--  2.0 unx     5356 b- defN 23-Mar-24 01:21 hidet/graph/jit.py
--rw-r--r--  2.0 unx     3735 b- defN 23-Mar-24 01:21 hidet/graph/module.py
--rw-r--r--  2.0 unx     7073 b- defN 23-Mar-24 01:21 hidet/graph/operator.py
--rw-r--r--  2.0 unx    41965 b- defN 23-Mar-24 01:21 hidet/graph/tensor.py
--rw-r--r--  2.0 unx      694 b- defN 23-Mar-24 01:21 hidet/graph/frontend/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 23-Mar-24 01:21 hidet/graph/frontend/onnx/__init__.py
--rw-r--r--  2.0 unx      848 b- defN 23-Mar-24 01:21 hidet/graph/frontend/onnx/availability.py
--rw-r--r--  2.0 unx    46729 b- defN 23-Mar-24 01:21 hidet/graph/frontend/onnx/onnx.py
--rw-r--r--  2.0 unx     2076 b- defN 23-Mar-24 01:21 hidet/graph/frontend/onnx/utils.py
--rw-r--r--  2.0 unx     2109 b- defN 23-Mar-24 01:21 hidet/graph/frontend/torch/__init__.py
--rw-r--r--  2.0 unx     1325 b- defN 23-Mar-24 01:21 hidet/graph/frontend/torch/availability.py
--rw-r--r--  2.0 unx     6425 b- defN 23-Mar-24 01:21 hidet/graph/frontend/torch/dynamo_backends.py
--rw-r--r--  2.0 unx     3855 b- defN 23-Mar-24 01:21 hidet/graph/frontend/torch/dynamo_config.py
--rw-r--r--  2.0 unx    17516 b- defN 23-Mar-24 01:21 hidet/graph/frontend/torch/interpreter.py
--rw-r--r--  2.0 unx    15277 b- defN 23-Mar-24 01:21 hidet/graph/frontend/torch/register_functions.py
--rw-r--r--  2.0 unx     6312 b- defN 23-Mar-24 01:21 hidet/graph/frontend/torch/register_methods.py
--rw-r--r--  2.0 unx     7629 b- defN 23-Mar-24 01:21 hidet/graph/frontend/torch/register_modules.py
--rw-r--r--  2.0 unx     7289 b- defN 23-Mar-24 01:21 hidet/graph/frontend/torch/utils.py
--rw-r--r--  2.0 unx      544 b- defN 23-Mar-24 01:21 hidet/graph/impl/__init__.py
--rw-r--r--  2.0 unx    10004 b- defN 23-Mar-24 01:21 hidet/graph/impl/dlpack.py
--rw-r--r--  2.0 unx      748 b- defN 23-Mar-24 01:21 hidet/graph/ir/__init__.py
--rw-r--r--  2.0 unx    19637 b- defN 23-Mar-24 01:21 hidet/graph/ir/flow_graph.py
--rw-r--r--  2.0 unx    10110 b- defN 23-Mar-24 01:21 hidet/graph/ir/flow_graph_impl.py
--rw-r--r--  2.0 unx     5681 b- defN 23-Mar-24 01:21 hidet/graph/ir/functors.py
--rw-r--r--  2.0 unx      585 b- defN 23-Mar-24 01:21 hidet/graph/modules/__init__.py
--rw-r--r--  2.0 unx     1655 b- defN 23-Mar-24 01:21 hidet/graph/modules/container.py
--rw-r--r--  2.0 unx     5755 b- defN 23-Mar-24 01:21 hidet/graph/modules/nn.py
--rw-r--r--  2.0 unx     2791 b- defN 23-Mar-24 01:21 hidet/graph/ops/__init__.py
--rw-r--r--  2.0 unx     2082 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/__init__.py
--rw-r--r--  2.0 unx     3863 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/activation.py
--rw-r--r--  2.0 unx    21758 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/arithmetic.py
--rw-r--r--  2.0 unx     1310 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/arithmetic_resolve.py
--rw-r--r--  2.0 unx     3341 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/compare.py
--rw-r--r--  2.0 unx     5592 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/create.py
--rw-r--r--  2.0 unx     2970 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/cumulative.py
--rw-r--r--  2.0 unx     9939 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/image.py
--rw-r--r--  2.0 unx     2459 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/norm.py
--rw-r--r--  2.0 unx    11594 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/pool.py
--rw-r--r--  2.0 unx     2609 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/softmax.py
--rw-r--r--  2.0 unx     1587 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/special.py
--rw-r--r--  2.0 unx    28652 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/transform.py
--rw-r--r--  2.0 unx     7149 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/utils.py
--rw-r--r--  2.0 unx     1157 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d/__init__.py
--rw-r--r--  2.0 unx     3165 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d/conv2d.py
--rw-r--r--  2.0 unx     3961 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d/conv2d_gemm.py
--rw-r--r--  2.0 unx     7505 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d/conv2d_winograd.py
--rw-r--r--  2.0 unx     1720 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d/resolve.py
--rw-r--r--  2.0 unx     1325 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d/utils.py
--rw-r--r--  2.0 unx      690 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d_transpose/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose.py
--rw-r--r--  2.0 unx     4894 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose_gemm.py
--rw-r--r--  2.0 unx     1246 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv2d_transpose/resolve.py
--rw-r--r--  2.0 unx      827 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv3d/__init__.py
--rw-r--r--  2.0 unx     3466 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv3d/conv3d.py
--rw-r--r--  2.0 unx     4319 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv3d/conv3d_gemm.py
--rw-r--r--  2.0 unx     1376 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv3d/resolve.py
--rw-r--r--  2.0 unx     1425 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/conv3d/utils.py
--rw-r--r--  2.0 unx      686 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/matmul/__init__.py
--rw-r--r--  2.0 unx     3699 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/matmul/batch_matmul.py
--rw-r--r--  2.0 unx     3256 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/matmul/matmul.py
--rw-r--r--  2.0 unx    16662 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/matmul/matmul_f16.py
--rw-r--r--  2.0 unx    10405 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/matmul/resolve.py
--rw-r--r--  2.0 unx      782 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/reduce/__init__.py
--rw-r--r--  2.0 unx     9811 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/reduce/reduce.py
--rw-r--r--  2.0 unx    13095 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/reduce/reduce_f16.py
--rw-r--r--  2.0 unx     2724 b- defN 23-Mar-24 01:21 hidet/graph/ops/definitions/reduce/resolve.py
--rw-r--r--  2.0 unx      754 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/__init__.py
--rw-r--r--  2.0 unx    14074 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/auto_scheduler.py
--rw-r--r--  2.0 unx     6384 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/common.py
--rw-r--r--  2.0 unx     7529 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/resolve.py
--rw-r--r--  2.0 unx      574 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/scheduler.py
--rw-r--r--  2.0 unx     7123 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/tune.py
--rw-r--r--  2.0 unx      544 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cpu/__init__.py
--rw-r--r--  2.0 unx     2611 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cpu/auto_scheduler.py
--rw-r--r--  2.0 unx      661 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/__init__.py
--rw-r--r--  2.0 unx     3097 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/auto_scheduler.py
--rw-r--r--  2.0 unx     4935 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/common.py
--rw-r--r--  2.0 unx    11077 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/depthwise_conv.py
--rw-r--r--  2.0 unx     6670 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/reduce.py
--rw-r--r--  2.0 unx     3639 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/softmax.py
--rw-r--r--  2.0 unx      698 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/matmul/__init__.py
--rw-r--r--  2.0 unx    21106 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/matmul/mma.py
--rw-r--r--  2.0 unx    22755 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/matmul/simt.py
--rw-r--r--  2.0 unx    21271 b- defN 23-Mar-24 01:21 hidet/graph/ops/schedules/cuda/matmul/wmma.py
--rw-r--r--  2.0 unx     2405 b- defN 23-Mar-24 01:21 hidet/graph/transforms/__init__.py
--rw-r--r--  2.0 unx     3648 b- defN 23-Mar-24 01:21 hidet/graph/transforms/automatic_mix_precision.py
--rw-r--r--  2.0 unx     8882 b- defN 23-Mar-24 01:21 hidet/graph/transforms/base.py
--rw-r--r--  2.0 unx      781 b- defN 23-Mar-24 01:21 hidet/graph/transforms/common.py
--rw-r--r--  2.0 unx     1327 b- defN 23-Mar-24 01:21 hidet/graph/transforms/eliminate_barrier.py
--rw-r--r--  2.0 unx     1616 b- defN 23-Mar-24 01:21 hidet/graph/transforms/fold_const.py
--rw-r--r--  2.0 unx    14965 b- defN 23-Mar-24 01:21 hidet/graph/transforms/fuse_operator.py
--rw-r--r--  2.0 unx     7011 b- defN 23-Mar-24 01:21 hidet/graph/transforms/resolve_variant.py
--rw-r--r--  2.0 unx     6274 b- defN 23-Mar-24 01:21 hidet/graph/transforms/subgraph_rewrite.py
--rw-r--r--  2.0 unx      712 b- defN 23-Mar-24 01:21 hidet/graph/transforms/utils.py
--rw-r--r--  2.0 unx      925 b- defN 23-Mar-24 01:21 hidet/graph/transforms/graph_patterns/__init__.py
--rw-r--r--  2.0 unx     2525 b- defN 23-Mar-24 01:21 hidet/graph/transforms/graph_patterns/arithmetic_patterns.py
--rw-r--r--  2.0 unx    12000 b- defN 23-Mar-24 01:21 hidet/graph/transforms/graph_patterns/base.py
--rw-r--r--  2.0 unx     4867 b- defN 23-Mar-24 01:21 hidet/graph/transforms/graph_patterns/conv2d_patterns.py
--rw-r--r--  2.0 unx     5378 b- defN 23-Mar-24 01:21 hidet/graph/transforms/graph_patterns/matmul_patterns.py
--rw-r--r--  2.0 unx     6850 b- defN 23-Mar-24 01:21 hidet/graph/transforms/graph_patterns/transform_patterns.py
--rw-r--r--  2.0 unx      687 b- defN 23-Mar-24 01:21 hidet/graph/transforms/instruments/__init__.py
--rw-r--r--  2.0 unx     3405 b- defN 23-Mar-24 01:21 hidet/graph/transforms/instruments/base.py
--rw-r--r--  2.0 unx     1865 b- defN 23-Mar-24 01:21 hidet/graph/transforms/instruments/profile_instrument.py
--rw-r--r--  2.0 unx     1608 b- defN 23-Mar-24 01:21 hidet/graph/transforms/instruments/save_graph_instrument.py
--rw-r--r--  2.0 unx      950 b- defN 23-Mar-24 01:21 hidet/include/hidet/packedfunc.h
--rw-r--r--  2.0 unx      754 b- defN 23-Mar-24 01:21 hidet/include/hidet/runtime.h
--rw-r--r--  2.0 unx      927 b- defN 23-Mar-24 01:21 hidet/include/hidet/runtime/callbacks.h
--rw-r--r--  2.0 unx      690 b- defN 23-Mar-24 01:21 hidet/include/hidet/runtime/common.h
--rw-r--r--  2.0 unx     1011 b- defN 23-Mar-24 01:21 hidet/include/hidet/runtime/context.h
--rw-r--r--  2.0 unx      777 b- defN 23-Mar-24 01:21 hidet/include/hidet/runtime/cpu_context.h
--rw-r--r--  2.0 unx     1190 b- defN 23-Mar-24 01:21 hidet/include/hidet/runtime/cuda_context.h
--rw-r--r--  2.0 unx     1249 b- defN 23-Mar-24 01:21 hidet/include/hidet/runtime/logging.h
--rw-r--r--  2.0 unx     2061 b- defN 23-Mar-24 01:21 hidet/ir/__init__.py
--rw-r--r--  2.0 unx    17680 b- defN 23-Mar-24 01:21 hidet/ir/expr.py
--rw-r--r--  2.0 unx     6359 b- defN 23-Mar-24 01:21 hidet/ir/func.py
--rw-r--r--  2.0 unx    16184 b- defN 23-Mar-24 01:21 hidet/ir/layout.py
--rw-r--r--  2.0 unx    12429 b- defN 23-Mar-24 01:21 hidet/ir/mapping.py
--rw-r--r--  2.0 unx      797 b- defN 23-Mar-24 01:21 hidet/ir/node.py
--rw-r--r--  2.0 unx     8049 b- defN 23-Mar-24 01:21 hidet/ir/stmt.py
--rw-r--r--  2.0 unx    12678 b- defN 23-Mar-24 01:21 hidet/ir/task.py
--rw-r--r--  2.0 unx     9225 b- defN 23-Mar-24 01:21 hidet/ir/type.py
--rw-r--r--  2.0 unx      640 b- defN 23-Mar-24 01:21 hidet/ir/analyzers/__init__.py
--rw-r--r--  2.0 unx    11678 b- defN 23-Mar-24 01:21 hidet/ir/analyzers/bound_analyzer.py
--rw-r--r--  2.0 unx      679 b- defN 23-Mar-24 01:21 hidet/ir/builders/__init__.py
--rw-r--r--  2.0 unx     3502 b- defN 23-Mar-24 01:21 hidet/ir/builders/func_builder.py
--rw-r--r--  2.0 unx     5210 b- defN 23-Mar-24 01:21 hidet/ir/builders/stmt_builder.py
--rw-r--r--  2.0 unx      884 b- defN 23-Mar-24 01:21 hidet/ir/compute/__init__.py
--rw-r--r--  2.0 unx    14773 b- defN 23-Mar-24 01:21 hidet/ir/compute/primitives.py
--rw-r--r--  2.0 unx     6861 b- defN 23-Mar-24 01:21 hidet/ir/compute/reduce_operations.py
--rw-r--r--  2.0 unx      544 b- defN 23-Mar-24 01:21 hidet/ir/dialects/__init__.py
--rw-r--r--  2.0 unx    17047 b- defN 23-Mar-24 01:21 hidet/ir/dialects/pattern.py
--rw-r--r--  2.0 unx     1877 b- defN 23-Mar-24 01:21 hidet/ir/dtypes/__init__.py
--rw-r--r--  2.0 unx     1543 b- defN 23-Mar-24 01:21 hidet/ir/dtypes/boolean.py
--rw-r--r--  2.0 unx     3610 b- defN 23-Mar-24 01:21 hidet/ir/dtypes/floats.py
--rw-r--r--  2.0 unx     2643 b- defN 23-Mar-24 01:21 hidet/ir/dtypes/integer.py
--rw-r--r--  2.0 unx     3379 b- defN 23-Mar-24 01:21 hidet/ir/dtypes/promotion.py
--rw-r--r--  2.0 unx     3146 b- defN 23-Mar-24 01:21 hidet/ir/dtypes/utils.py
--rw-r--r--  2.0 unx     2372 b- defN 23-Mar-24 01:21 hidet/ir/dtypes/vector.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Mar-24 01:21 hidet/ir/functors/__init__.py
--rw-r--r--  2.0 unx     4031 b- defN 23-Mar-24 01:21 hidet/ir/functors/base_functor.py
--rw-r--r--  2.0 unx     6786 b- defN 23-Mar-24 01:21 hidet/ir/functors/compute_functor.py
--rw-r--r--  2.0 unx    14474 b- defN 23-Mar-24 01:21 hidet/ir/functors/expr_functor.py
--rw-r--r--  2.0 unx     1448 b- defN 23-Mar-24 01:21 hidet/ir/functors/ir_functor.py
--rw-r--r--  2.0 unx      544 b- defN 23-Mar-24 01:21 hidet/ir/functors/layout_functor.py
--rw-r--r--  2.0 unx     2358 b- defN 23-Mar-24 01:21 hidet/ir/functors/mapping_functor.py
--rw-r--r--  2.0 unx     2439 b- defN 23-Mar-24 01:21 hidet/ir/functors/module_functor.py
--rw-r--r--  2.0 unx    12152 b- defN 23-Mar-24 01:21 hidet/ir/functors/stmt_functor.py
--rw-r--r--  2.0 unx     3707 b- defN 23-Mar-24 01:21 hidet/ir/functors/type_functor.py
--rw-r--r--  2.0 unx     1323 b- defN 23-Mar-24 01:21 hidet/ir/primitives/__init__.py
--rw-r--r--  2.0 unx     1116 b- defN 23-Mar-24 01:21 hidet/ir/primitives/debug.py
--rw-r--r--  2.0 unx     5739 b- defN 23-Mar-24 01:21 hidet/ir/primitives/func.py
--rw-r--r--  2.0 unx    11314 b- defN 23-Mar-24 01:21 hidet/ir/primitives/math.py
--rw-r--r--  2.0 unx     1800 b- defN 23-Mar-24 01:21 hidet/ir/primitives/runtime.py
--rw-r--r--  2.0 unx      563 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cpu/__init__.py
--rw-r--r--  2.0 unx      628 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cpu/math/__init__.py
--rw-r--r--  2.0 unx     5376 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cpu/math/float32.py
--rw-r--r--  2.0 unx     5344 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cpu/math/float64.py
--rw-r--r--  2.0 unx     3034 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cpu/math/int32.py
--rw-r--r--  2.0 unx     3034 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cpu/math/int64.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/__init__.py
--rw-r--r--  2.0 unx     1840 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/atomic.py
--rw-r--r--  2.0 unx     7479 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/cp_async.py
--rw-r--r--  2.0 unx     2898 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/cvt.py
--rw-r--r--  2.0 unx     2856 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/cvta.py
--rw-r--r--  2.0 unx     2246 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/funcs.py
--rw-r--r--  2.0 unx     8543 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/ldst.py
--rw-r--r--  2.0 unx    14458 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/mma.py
--rw-r--r--  2.0 unx     4736 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/mutex.py
--rw-r--r--  2.0 unx     1983 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/shfl.py
--rw-r--r--  2.0 unx     2273 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/smem.py
--rw-r--r--  2.0 unx     1934 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/sync.py
--rw-r--r--  2.0 unx     1750 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/time.py
--rw-r--r--  2.0 unx     2683 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/vars.py
--rw-r--r--  2.0 unx    12898 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/wmma.py
--rw-r--r--  2.0 unx      673 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/math/__init__.py
--rw-r--r--  2.0 unx     3787 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/math/bfloat16.py
--rw-r--r--  2.0 unx     7382 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/math/float16.py
--rw-r--r--  2.0 unx     5384 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/math/float32.py
--rw-r--r--  2.0 unx     5352 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/math/float64.py
--rw-r--r--  2.0 unx     3043 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/math/int32.py
--rw-r--r--  2.0 unx     3350 b- defN 23-Mar-24 01:21 hidet/ir/primitives/cuda/math/int64.py
--rw-r--r--  2.0 unx      767 b- defN 23-Mar-24 01:21 hidet/ir/tools/__init__.py
--rw-r--r--  2.0 unx     5649 b- defN 23-Mar-24 01:21 hidet/ir/tools/hasher.py
--rw-r--r--  2.0 unx    22686 b- defN 23-Mar-24 01:21 hidet/ir/tools/printer.py
--rw-r--r--  2.0 unx     5792 b- defN 23-Mar-24 01:21 hidet/ir/tools/simplifier.py
--rw-r--r--  2.0 unx     7252 b- defN 23-Mar-24 01:21 hidet/ir/tools/type_infer.py
--rw-r--r--  2.0 unx     4580 b- defN 23-Mar-24 01:21 hidet/ir/tools/util_functors.py
--rw-r--r--  2.0 unx      811 b- defN 23-Mar-24 01:21 hidet/ir/utils/__init__.py
--rw-r--r--  2.0 unx     3417 b- defN 23-Mar-24 01:21 hidet/ir/utils/call_graph.py
--rw-r--r--  2.0 unx     1038 b- defN 23-Mar-24 01:21 hidet/ir/utils/expr_utils.py
--rw-r--r--  2.0 unx     1414 b- defN 23-Mar-24 01:21 hidet/ir/utils/hash_sum.py
--rw-r--r--  2.0 unx     1325 b- defN 23-Mar-24 01:21 hidet/ir/utils/index_transform.py
--rw-r--r--  2.0 unx     4385 b- defN 23-Mar-24 01:21 hidet/ir/utils/task_utils.py
--rw-r--r--  2.0 unx     1811 b- defN 23-Mar-24 01:21 hidet/ir/utils/type_utils.py
--rw-r--r--  2.0 unx     3031 b- defN 23-Mar-24 01:21 hidet/lang/__init__.py
--rw-r--r--  2.0 unx     1826 b- defN 23-Mar-24 01:21 hidet/lang/attr.py
--rw-r--r--  2.0 unx     2219 b- defN 23-Mar-24 01:21 hidet/lang/cuda.py
--rw-r--r--  2.0 unx      653 b- defN 23-Mar-24 01:21 hidet/lang/layout.py
--rw-r--r--  2.0 unx      963 b- defN 23-Mar-24 01:21 hidet/lang/mapping.py
--rw-r--r--  2.0 unx      679 b- defN 23-Mar-24 01:21 hidet/lang/runtime.py
--rw-r--r--  2.0 unx     4695 b- defN 23-Mar-24 01:21 hidet/lang/script.py
--rw-r--r--  2.0 unx    40907 b- defN 23-Mar-24 01:21 hidet/lang/transpiler.py
--rw-r--r--  2.0 unx     1880 b- defN 23-Mar-24 01:21 hidet/lang/type_utils.py
--rwxr-xr-x  2.0 unx     7123 b- defN 23-Mar-24 01:21 hidet/lib/libhidet.so
--rwxr-xr-x  2.0 unx    55385 b- defN 23-Mar-24 01:21 hidet/lib/libhidet_runtime.so
--rw-r--r--  2.0 unx      670 b- defN 23-Mar-24 01:21 hidet/runtime/__init__.py
--rw-r--r--  2.0 unx     4118 b- defN 23-Mar-24 01:21 hidet/runtime/device.py
--rw-r--r--  2.0 unx     3191 b- defN 23-Mar-24 01:21 hidet/runtime/module.py
--rw-r--r--  2.0 unx    12683 b- defN 23-Mar-24 01:21 hidet/runtime/storage.py
--rw-r--r--  2.0 unx      751 b- defN 23-Mar-24 01:21 hidet/testing/__init__.py
--rw-r--r--  2.0 unx     4542 b- defN 23-Mar-24 01:21 hidet/testing/onnx_models.py
--rw-r--r--  2.0 unx     2091 b- defN 23-Mar-24 01:21 hidet/testing/onnx_utils.py
--rw-r--r--  2.0 unx     1494 b- defN 23-Mar-24 01:21 hidet/testing/torch_utils.py
--rw-r--r--  2.0 unx     5293 b- defN 23-Mar-24 01:21 hidet/testing/utils.py
--rw-r--r--  2.0 unx      615 b- defN 23-Mar-24 01:21 hidet/testing/models/__init__.py
--rw-r--r--  2.0 unx     5544 b- defN 23-Mar-24 01:21 hidet/testing/models/resnet.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Mar-24 01:21 hidet/transforms/__init__.py
--rw-r--r--  2.0 unx     6379 b- defN 23-Mar-24 01:21 hidet/transforms/add_explicit_cast.py
--rw-r--r--  2.0 unx     3822 b- defN 23-Mar-24 01:21 hidet/transforms/base.py
--rw-r--r--  2.0 unx     3587 b- defN 23-Mar-24 01:21 hidet/transforms/declare_to_let.py
--rw-r--r--  2.0 unx     3204 b- defN 23-Mar-24 01:21 hidet/transforms/expand_let_expr.py
--rw-r--r--  2.0 unx     4185 b- defN 23-Mar-24 01:21 hidet/transforms/flatten_tensor_index.py
--rw-r--r--  2.0 unx     4338 b- defN 23-Mar-24 01:21 hidet/transforms/flatten_tensor_slice.py
--rw-r--r--  2.0 unx     4900 b- defN 23-Mar-24 01:21 hidet/transforms/generate_packed_func.py
--rw-r--r--  2.0 unx     2025 b- defN 23-Mar-24 01:21 hidet/transforms/import_primitive_functions.py
--rw-r--r--  2.0 unx     4342 b- defN 23-Mar-24 01:21 hidet/transforms/inline_let_stmt.py
--rw-r--r--  2.0 unx     2811 b- defN 23-Mar-24 01:21 hidet/transforms/lower_protect_access.py
--rw-r--r--  2.0 unx     3596 b- defN 23-Mar-24 01:21 hidet/transforms/lower_special_cast.py
--rw-r--r--  2.0 unx     5252 b- defN 23-Mar-24 01:21 hidet/transforms/lower_task_mapping.py
--rw-r--r--  2.0 unx     1845 b- defN 23-Mar-24 01:21 hidet/transforms/normalize_const_tensor.py
--rw-r--r--  2.0 unx     2403 b- defN 23-Mar-24 01:21 hidet/transforms/propogate_launch_bound.py
--rw-r--r--  2.0 unx     4786 b- defN 23-Mar-24 01:21 hidet/transforms/resolve_generic_primitive_function.py
--rw-r--r--  2.0 unx    10048 b- defN 23-Mar-24 01:21 hidet/transforms/rule_based_simplifier.py
--rw-r--r--  2.0 unx     1693 b- defN 23-Mar-24 01:21 hidet/transforms/simplify_stmt.py
--rw-r--r--  2.0 unx      623 b- defN 23-Mar-24 01:21 hidet/transforms/common/__init__.py
--rw-r--r--  2.0 unx     5654 b- defN 23-Mar-24 01:21 hidet/transforms/common/scope.py
--rw-r--r--  2.0 unx      676 b- defN 23-Mar-24 01:21 hidet/transforms/instruments/__init__.py
--rw-r--r--  2.0 unx      892 b- defN 23-Mar-24 01:21 hidet/transforms/instruments/base.py
--rw-r--r--  2.0 unx     1851 b- defN 23-Mar-24 01:21 hidet/transforms/instruments/profile_instrument.py
--rw-r--r--  2.0 unx     1552 b- defN 23-Mar-24 01:21 hidet/transforms/instruments/save_ir_instrument.py
--rw-r--r--  2.0 unx     1281 b- defN 23-Mar-24 01:21 hidet/transforms/tools/__init__.py
--rw-r--r--  2.0 unx    10966 b- defN 23-Mar-24 01:21 hidet/transforms/tools/apply_prologue_epilogue.py
--rw-r--r--  2.0 unx     5376 b- defN 23-Mar-24 01:21 hidet/transforms/tools/generate_packed_func.py
--rw-r--r--  2.0 unx     1150 b- defN 23-Mar-24 01:21 hidet/utils/__init__.py
--rw-r--r--  2.0 unx     2184 b- defN 23-Mar-24 01:21 hidet/utils/bench.py
--rw-r--r--  2.0 unx     1176 b- defN 23-Mar-24 01:21 hidet/utils/cache_utils.py
--rw-r--r--  2.0 unx     3283 b- defN 23-Mar-24 01:21 hidet/utils/doc.py
--rw-r--r--  2.0 unx     1666 b- defN 23-Mar-24 01:21 hidet/utils/exiting.py
--rw-r--r--  2.0 unx     2664 b- defN 23-Mar-24 01:21 hidet/utils/git_utils.py
--rw-r--r--  2.0 unx     2401 b- defN 23-Mar-24 01:21 hidet/utils/namer.py
--rw-r--r--  2.0 unx     2471 b- defN 23-Mar-24 01:21 hidet/utils/net_utils.py
--rw-r--r--  2.0 unx     8524 b- defN 23-Mar-24 01:21 hidet/utils/netron.py
--rw-r--r--  2.0 unx     2275 b- defN 23-Mar-24 01:21 hidet/utils/ort_utils.py
--rw-r--r--  2.0 unx      785 b- defN 23-Mar-24 01:21 hidet/utils/overrides.py
--rw-r--r--  2.0 unx    11319 b- defN 23-Mar-24 01:21 hidet/utils/py.py
--rw-r--r--  2.0 unx      822 b- defN 23-Mar-24 01:21 hidet/utils/stack_limit.py
--rw-r--r--  2.0 unx     4794 b- defN 23-Mar-24 01:21 hidet/utils/structure.py
--rw-r--r--  2.0 unx     2272 b- defN 23-Mar-24 01:21 hidet/utils/torch_utils.py
--rw-r--r--  2.0 unx     1891 b- defN 23-Mar-24 01:21 hidet/utils/transformers_utils.py
--rw-r--r--  2.0 unx     4096 b- defN 23-Mar-24 01:21 hidet-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-24 01:21 hidet-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      136 b- defN 23-Mar-24 01:21 hidet-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-24 01:21 hidet-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    27533 b- defN 23-Mar-24 01:21 hidet-0.2.2.dist-info/RECORD
-306 files, 1640439 bytes uncompressed, 487099 bytes compressed:  70.3%
+Zip file size: 569215 bytes, number of entries: 318
+-rwxr-xr-x  2.0 unx     7123 b- defN 23-Apr-24 21:28 libhidet.so
+-rwxr-xr-x  2.0 unx    55385 b- defN 23-Apr-24 21:28 libhidet_runtime.so
+-rw-r--r--  2.0 unx     1673 b- defN 23-Apr-24 21:28 hidet/__init__.py
+-rw-r--r--  2.0 unx     2797 b- defN 23-Apr-24 21:28 hidet/array_api.py
+-rw-r--r--  2.0 unx    11538 b- defN 23-Apr-24 21:28 hidet/driver.py
+-rw-r--r--  2.0 unx     2178 b- defN 23-Apr-24 21:28 hidet/libinfo.py
+-rw-r--r--  2.0 unx     2039 b- defN 23-Apr-24 21:28 hidet/logging.py
+-rw-r--r--  2.0 unx    13706 b- defN 23-Apr-24 21:28 hidet/option.py
+-rw-r--r--  2.0 unx      566 b- defN 23-Apr-24 21:28 hidet/version.py
+-rw-r--r--  2.0 unx      745 b- defN 23-Apr-24 21:28 hidet/backend/__init__.py
+-rw-r--r--  2.0 unx     8591 b- defN 23-Apr-24 21:28 hidet/backend/build.py
+-rw-r--r--  2.0 unx    31602 b- defN 23-Apr-24 21:28 hidet/backend/codegen.py
+-rw-r--r--  2.0 unx      564 b- defN 23-Apr-24 21:28 hidet/cli/__init__.py
+-rw-r--r--  2.0 unx      875 b- defN 23-Apr-24 21:28 hidet/cli/main.py
+-rw-r--r--  2.0 unx      887 b- defN 23-Apr-24 21:28 hidet/cli/bench/__init__.py
+-rw-r--r--  2.0 unx     2907 b- defN 23-Apr-24 21:28 hidet/cli/bench/bench.py
+-rw-r--r--  2.0 unx      935 b- defN 23-Apr-24 21:28 hidet/cli/bench/bench_all.py
+-rw-r--r--  2.0 unx      939 b- defN 23-Apr-24 21:28 hidet/cli/bench/bench_common.py
+-rw-r--r--  2.0 unx     6111 b- defN 23-Apr-24 21:28 hidet/cli/bench/model.py
+-rw-r--r--  2.0 unx      574 b- defN 23-Apr-24 21:28 hidet/cli/bench/nlp/__init__.py
+-rw-r--r--  2.0 unx     2493 b- defN 23-Apr-24 21:28 hidet/cli/bench/nlp/models.py
+-rw-r--r--  2.0 unx     1851 b- defN 23-Apr-24 21:28 hidet/cli/bench/nlp/nlp_model.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Apr-24 21:28 hidet/cli/bench/vision/__init__.py
+-rw-r--r--  2.0 unx     1727 b- defN 23-Apr-24 21:28 hidet/cli/bench/vision/inception_v3.py
+-rw-r--r--  2.0 unx     1727 b- defN 23-Apr-24 21:28 hidet/cli/bench/vision/mobilenet_v2.py
+-rw-r--r--  2.0 unx     2410 b- defN 23-Apr-24 21:28 hidet/cli/bench/vision/resnet.py
+-rw-r--r--  2.0 unx     2288 b- defN 23-Apr-24 21:28 hidet/cli/bench/vision/resnext.py
+-rw-r--r--  2.0 unx     1269 b- defN 23-Apr-24 21:28 hidet/cli/bench/vision/vision_model.py
+-rw-r--r--  2.0 unx     1034 b- defN 23-Apr-24 21:28 hidet/cuda/__init__.py
+-rw-r--r--  2.0 unx     3876 b- defN 23-Apr-24 21:28 hidet/cuda/device.py
+-rw-r--r--  2.0 unx     4171 b- defN 23-Apr-24 21:28 hidet/cuda/event.py
+-rw-r--r--  2.0 unx     8203 b- defN 23-Apr-24 21:28 hidet/cuda/graph.py
+-rw-r--r--  2.0 unx     7460 b- defN 23-Apr-24 21:28 hidet/cuda/memory.py
+-rw-r--r--  2.0 unx     7759 b- defN 23-Apr-24 21:28 hidet/cuda/stream.py
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-24 21:28 hidet/ffi/__init__.py
+-rw-r--r--  2.0 unx     2496 b- defN 23-Apr-24 21:28 hidet/ffi/callbacks.py
+-rw-r--r--  2.0 unx     3079 b- defN 23-Apr-24 21:28 hidet/ffi/ffi.py
+-rw-r--r--  2.0 unx     6858 b- defN 23-Apr-24 21:28 hidet/ffi/packedfunc.py
+-rw-r--r--  2.0 unx     1766 b- defN 23-Apr-24 21:28 hidet/ffi/runtime_api.py
+-rw-r--r--  2.0 unx     3427 b- defN 23-Apr-24 21:28 hidet/ffi/shared_lib.py
+-rw-r--r--  2.0 unx     1240 b- defN 23-Apr-24 21:28 hidet/graph/__init__.py
+-rw-r--r--  2.0 unx      672 b- defN 23-Apr-24 21:28 hidet/graph/common.py
+-rw-r--r--  2.0 unx     5356 b- defN 23-Apr-24 21:28 hidet/graph/jit.py
+-rw-r--r--  2.0 unx     3735 b- defN 23-Apr-24 21:28 hidet/graph/module.py
+-rw-r--r--  2.0 unx     7701 b- defN 23-Apr-24 21:28 hidet/graph/operator.py
+-rw-r--r--  2.0 unx    43043 b- defN 23-Apr-24 21:28 hidet/graph/tensor.py
+-rw-r--r--  2.0 unx      694 b- defN 23-Apr-24 21:28 hidet/graph/frontend/__init__.py
+-rw-r--r--  2.0 unx      649 b- defN 23-Apr-24 21:28 hidet/graph/frontend/onnx/__init__.py
+-rw-r--r--  2.0 unx      848 b- defN 23-Apr-24 21:28 hidet/graph/frontend/onnx/availability.py
+-rw-r--r--  2.0 unx    46729 b- defN 23-Apr-24 21:28 hidet/graph/frontend/onnx/onnx.py
+-rw-r--r--  2.0 unx     2076 b- defN 23-Apr-24 21:28 hidet/graph/frontend/onnx/utils.py
+-rw-r--r--  2.0 unx     2109 b- defN 23-Apr-24 21:28 hidet/graph/frontend/torch/__init__.py
+-rw-r--r--  2.0 unx     1325 b- defN 23-Apr-24 21:28 hidet/graph/frontend/torch/availability.py
+-rw-r--r--  2.0 unx     6866 b- defN 23-Apr-24 21:28 hidet/graph/frontend/torch/dynamo_backends.py
+-rw-r--r--  2.0 unx     4600 b- defN 23-Apr-24 21:28 hidet/graph/frontend/torch/dynamo_config.py
+-rw-r--r--  2.0 unx    17516 b- defN 23-Apr-24 21:28 hidet/graph/frontend/torch/interpreter.py
+-rw-r--r--  2.0 unx    22755 b- defN 23-Apr-24 21:28 hidet/graph/frontend/torch/register_functions.py
+-rw-r--r--  2.0 unx     7061 b- defN 23-Apr-24 21:28 hidet/graph/frontend/torch/register_methods.py
+-rw-r--r--  2.0 unx    10033 b- defN 23-Apr-24 21:28 hidet/graph/frontend/torch/register_modules.py
+-rw-r--r--  2.0 unx     7611 b- defN 23-Apr-24 21:28 hidet/graph/frontend/torch/utils.py
+-rw-r--r--  2.0 unx      544 b- defN 23-Apr-24 21:28 hidet/graph/impl/__init__.py
+-rw-r--r--  2.0 unx    10004 b- defN 23-Apr-24 21:28 hidet/graph/impl/dlpack.py
+-rw-r--r--  2.0 unx      748 b- defN 23-Apr-24 21:28 hidet/graph/ir/__init__.py
+-rw-r--r--  2.0 unx    20377 b- defN 23-Apr-24 21:28 hidet/graph/ir/flow_graph.py
+-rw-r--r--  2.0 unx    10017 b- defN 23-Apr-24 21:28 hidet/graph/ir/flow_graph_impl.py
+-rw-r--r--  2.0 unx     5681 b- defN 23-Apr-24 21:28 hidet/graph/ir/functors.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Apr-24 21:28 hidet/graph/modules/__init__.py
+-rw-r--r--  2.0 unx     1655 b- defN 23-Apr-24 21:28 hidet/graph/modules/container.py
+-rw-r--r--  2.0 unx     5755 b- defN 23-Apr-24 21:28 hidet/graph/modules/nn.py
+-rw-r--r--  2.0 unx     2989 b- defN 23-Apr-24 21:28 hidet/graph/ops/__init__.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/__init__.py
+-rw-r--r--  2.0 unx     8723 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/activation.py
+-rw-r--r--  2.0 unx    21886 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/arithmetic.py
+-rw-r--r--  2.0 unx     1310 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/arithmetic_resolve.py
+-rw-r--r--  2.0 unx     3341 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/compare.py
+-rw-r--r--  2.0 unx     5507 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/create.py
+-rw-r--r--  2.0 unx     2970 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/cumulative.py
+-rw-r--r--  2.0 unx     9939 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/image.py
+-rw-r--r--  2.0 unx     3284 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/norm.py
+-rw-r--r--  2.0 unx    11594 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/pool.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/softmax.py
+-rw-r--r--  2.0 unx     1602 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/special.py
+-rw-r--r--  2.0 unx    29926 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/transform.py
+-rw-r--r--  2.0 unx       33 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/attention/__init__.py
+-rw-r--r--  2.0 unx    35378 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/attention/attention.py
+-rw-r--r--  2.0 unx    36447 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/attention/attention_mask.py
+-rw-r--r--  2.0 unx     1157 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d/__init__.py
+-rw-r--r--  2.0 unx     3165 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d/conv2d.py
+-rw-r--r--  2.0 unx     3961 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d/conv2d_gemm.py
+-rw-r--r--  2.0 unx     7505 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d/conv2d_winograd.py
+-rw-r--r--  2.0 unx     1720 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d/resolve.py
+-rw-r--r--  2.0 unx     1325 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d/utils.py
+-rw-r--r--  2.0 unx      690 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d_transpose/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose.py
+-rw-r--r--  2.0 unx     4894 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose_gemm.py
+-rw-r--r--  2.0 unx     1246 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv2d_transpose/resolve.py
+-rw-r--r--  2.0 unx      827 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv3d/__init__.py
+-rw-r--r--  2.0 unx     3466 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv3d/conv3d.py
+-rw-r--r--  2.0 unx     4319 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv3d/conv3d_gemm.py
+-rw-r--r--  2.0 unx     1376 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv3d/resolve.py
+-rw-r--r--  2.0 unx     1425 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/conv3d/utils.py
+-rw-r--r--  2.0 unx       43 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/fusion/__init__.py
+-rw-r--r--  2.0 unx    11864 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/fusion/apply_prologue_epilogue.py
+-rw-r--r--  2.0 unx     7428 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/fusion/fused_operator.py
+-rw-r--r--  2.0 unx      686 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/matmul/__init__.py
+-rw-r--r--  2.0 unx     3725 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/matmul/batch_matmul.py
+-rw-r--r--  2.0 unx     3271 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/matmul/matmul.py
+-rw-r--r--  2.0 unx    17991 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/matmul/matmul_f16.py
+-rw-r--r--  2.0 unx    10483 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/matmul/resolve.py
+-rw-r--r--  2.0 unx      782 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/reduce/__init__.py
+-rw-r--r--  2.0 unx     9923 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/reduce/reduce.py
+-rw-r--r--  2.0 unx    12868 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/reduce/reduce_f16.py
+-rw-r--r--  2.0 unx     2719 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/reduce/resolve.py
+-rw-r--r--  2.0 unx       47 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/utils/__init__.py
+-rw-r--r--  2.0 unx     7149 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/utils/tensor_utils.py
+-rw-r--r--  2.0 unx     7341 b- defN 23-Apr-24 21:28 hidet/graph/ops/definitions/utils/tune.py
+-rw-r--r--  2.0 unx      754 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/__init__.py
+-rw-r--r--  2.0 unx    16490 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/auto_scheduler.py
+-rw-r--r--  2.0 unx     6384 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/common.py
+-rw-r--r--  2.0 unx     7029 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/resolve.py
+-rw-r--r--  2.0 unx      574 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/scheduler.py
+-rw-r--r--  2.0 unx      544 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cpu/__init__.py
+-rw-r--r--  2.0 unx     2362 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cpu/auto_scheduler.py
+-rw-r--r--  2.0 unx      661 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/__init__.py
+-rw-r--r--  2.0 unx     2986 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/auto_scheduler.py
+-rw-r--r--  2.0 unx     4935 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/common.py
+-rw-r--r--  2.0 unx    10965 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/depthwise_conv.py
+-rw-r--r--  2.0 unx     6557 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/reduce.py
+-rw-r--r--  2.0 unx     3563 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/softmax.py
+-rw-r--r--  2.0 unx      698 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/matmul/__init__.py
+-rw-r--r--  2.0 unx    21042 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/matmul/mma.py
+-rw-r--r--  2.0 unx    22703 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/matmul/simt.py
+-rw-r--r--  2.0 unx    21213 b- defN 23-Apr-24 21:28 hidet/graph/ops/schedules/cuda/matmul/wmma.py
+-rw-r--r--  2.0 unx     2405 b- defN 23-Apr-24 21:28 hidet/graph/transforms/__init__.py
+-rw-r--r--  2.0 unx     3648 b- defN 23-Apr-24 21:28 hidet/graph/transforms/automatic_mix_precision.py
+-rw-r--r--  2.0 unx     9490 b- defN 23-Apr-24 21:28 hidet/graph/transforms/base.py
+-rw-r--r--  2.0 unx      781 b- defN 23-Apr-24 21:28 hidet/graph/transforms/common.py
+-rw-r--r--  2.0 unx     1327 b- defN 23-Apr-24 21:28 hidet/graph/transforms/eliminate_barrier.py
+-rw-r--r--  2.0 unx     1616 b- defN 23-Apr-24 21:28 hidet/graph/transforms/fold_const.py
+-rw-r--r--  2.0 unx    16457 b- defN 23-Apr-24 21:28 hidet/graph/transforms/fuse_operator.py
+-rw-r--r--  2.0 unx     7011 b- defN 23-Apr-24 21:28 hidet/graph/transforms/resolve_variant.py
+-rw-r--r--  2.0 unx     6274 b- defN 23-Apr-24 21:28 hidet/graph/transforms/subgraph_rewrite.py
+-rw-r--r--  2.0 unx      712 b- defN 23-Apr-24 21:28 hidet/graph/transforms/utils.py
+-rw-r--r--  2.0 unx     1041 b- defN 23-Apr-24 21:28 hidet/graph/transforms/graph_patterns/__init__.py
+-rw-r--r--  2.0 unx     2525 b- defN 23-Apr-24 21:28 hidet/graph/transforms/graph_patterns/arithmetic_patterns.py
+-rw-r--r--  2.0 unx     4818 b- defN 23-Apr-24 21:28 hidet/graph/transforms/graph_patterns/attn_patterns.py
+-rw-r--r--  2.0 unx    12434 b- defN 23-Apr-24 21:28 hidet/graph/transforms/graph_patterns/base.py
+-rw-r--r--  2.0 unx     4867 b- defN 23-Apr-24 21:28 hidet/graph/transforms/graph_patterns/conv2d_patterns.py
+-rw-r--r--  2.0 unx     5378 b- defN 23-Apr-24 21:28 hidet/graph/transforms/graph_patterns/matmul_patterns.py
+-rw-r--r--  2.0 unx     6850 b- defN 23-Apr-24 21:28 hidet/graph/transforms/graph_patterns/transform_patterns.py
+-rw-r--r--  2.0 unx      687 b- defN 23-Apr-24 21:28 hidet/graph/transforms/instruments/__init__.py
+-rw-r--r--  2.0 unx     3405 b- defN 23-Apr-24 21:28 hidet/graph/transforms/instruments/base.py
+-rw-r--r--  2.0 unx     1865 b- defN 23-Apr-24 21:28 hidet/graph/transforms/instruments/profile_instrument.py
+-rw-r--r--  2.0 unx     1608 b- defN 23-Apr-24 21:28 hidet/graph/transforms/instruments/save_graph_instrument.py
+-rw-r--r--  2.0 unx      950 b- defN 23-Apr-24 21:28 hidet/include/hidet/packedfunc.h
+-rw-r--r--  2.0 unx      754 b- defN 23-Apr-24 21:28 hidet/include/hidet/runtime.h
+-rw-r--r--  2.0 unx    16107 b- defN 23-Apr-24 21:28 hidet/include/hidet/cpu/bfloat16.h
+-rw-r--r--  2.0 unx    25684 b- defN 23-Apr-24 21:28 hidet/include/hidet/cpu/float16.h
+-rw-r--r--  2.0 unx      927 b- defN 23-Apr-24 21:28 hidet/include/hidet/runtime/callbacks.h
+-rw-r--r--  2.0 unx      690 b- defN 23-Apr-24 21:28 hidet/include/hidet/runtime/common.h
+-rw-r--r--  2.0 unx     1011 b- defN 23-Apr-24 21:28 hidet/include/hidet/runtime/context.h
+-rw-r--r--  2.0 unx      777 b- defN 23-Apr-24 21:28 hidet/include/hidet/runtime/cpu_context.h
+-rw-r--r--  2.0 unx     1190 b- defN 23-Apr-24 21:28 hidet/include/hidet/runtime/cuda_context.h
+-rw-r--r--  2.0 unx     1249 b- defN 23-Apr-24 21:28 hidet/include/hidet/runtime/logging.h
+-rw-r--r--  2.0 unx     2094 b- defN 23-Apr-24 21:28 hidet/ir/__init__.py
+-rw-r--r--  2.0 unx    17680 b- defN 23-Apr-24 21:28 hidet/ir/expr.py
+-rw-r--r--  2.0 unx     6359 b- defN 23-Apr-24 21:28 hidet/ir/func.py
+-rw-r--r--  2.0 unx    16178 b- defN 23-Apr-24 21:28 hidet/ir/layout.py
+-rw-r--r--  2.0 unx    13727 b- defN 23-Apr-24 21:28 hidet/ir/mapping.py
+-rw-r--r--  2.0 unx      797 b- defN 23-Apr-24 21:28 hidet/ir/node.py
+-rw-r--r--  2.0 unx    11391 b- defN 23-Apr-24 21:28 hidet/ir/stmt.py
+-rw-r--r--  2.0 unx    12861 b- defN 23-Apr-24 21:28 hidet/ir/task.py
+-rw-r--r--  2.0 unx     9584 b- defN 23-Apr-24 21:28 hidet/ir/type.py
+-rw-r--r--  2.0 unx      640 b- defN 23-Apr-24 21:28 hidet/ir/analyzers/__init__.py
+-rw-r--r--  2.0 unx    11678 b- defN 23-Apr-24 21:28 hidet/ir/analyzers/bound_analyzer.py
+-rw-r--r--  2.0 unx      679 b- defN 23-Apr-24 21:28 hidet/ir/builders/__init__.py
+-rw-r--r--  2.0 unx     3343 b- defN 23-Apr-24 21:28 hidet/ir/builders/func_builder.py
+-rw-r--r--  2.0 unx     5245 b- defN 23-Apr-24 21:28 hidet/ir/builders/stmt_builder.py
+-rw-r--r--  2.0 unx      884 b- defN 23-Apr-24 21:28 hidet/ir/compute/__init__.py
+-rw-r--r--  2.0 unx    14773 b- defN 23-Apr-24 21:28 hidet/ir/compute/primitives.py
+-rw-r--r--  2.0 unx     6917 b- defN 23-Apr-24 21:28 hidet/ir/compute/reduce_operations.py
+-rw-r--r--  2.0 unx      544 b- defN 23-Apr-24 21:28 hidet/ir/dialects/__init__.py
+-rw-r--r--  2.0 unx    17322 b- defN 23-Apr-24 21:28 hidet/ir/dialects/pattern.py
+-rw-r--r--  2.0 unx     1877 b- defN 23-Apr-24 21:28 hidet/ir/dtypes/__init__.py
+-rw-r--r--  2.0 unx     1543 b- defN 23-Apr-24 21:28 hidet/ir/dtypes/boolean.py
+-rw-r--r--  2.0 unx     3610 b- defN 23-Apr-24 21:28 hidet/ir/dtypes/floats.py
+-rw-r--r--  2.0 unx     2643 b- defN 23-Apr-24 21:28 hidet/ir/dtypes/integer.py
+-rw-r--r--  2.0 unx     3379 b- defN 23-Apr-24 21:28 hidet/ir/dtypes/promotion.py
+-rw-r--r--  2.0 unx     3146 b- defN 23-Apr-24 21:28 hidet/ir/dtypes/utils.py
+-rw-r--r--  2.0 unx     2372 b- defN 23-Apr-24 21:28 hidet/ir/dtypes/vector.py
+-rw-r--r--  2.0 unx     1161 b- defN 23-Apr-24 21:28 hidet/ir/functors/__init__.py
+-rw-r--r--  2.0 unx     4601 b- defN 23-Apr-24 21:28 hidet/ir/functors/base_functor.py
+-rw-r--r--  2.0 unx     6307 b- defN 23-Apr-24 21:28 hidet/ir/functors/compute_functor.py
+-rw-r--r--  2.0 unx    14474 b- defN 23-Apr-24 21:28 hidet/ir/functors/expr_functor.py
+-rw-r--r--  2.0 unx     1573 b- defN 23-Apr-24 21:28 hidet/ir/functors/ir_functor.py
+-rw-r--r--  2.0 unx     4170 b- defN 23-Apr-24 21:28 hidet/ir/functors/layout_functor.py
+-rw-r--r--  2.0 unx     2358 b- defN 23-Apr-24 21:28 hidet/ir/functors/mapping_functor.py
+-rw-r--r--  2.0 unx     2439 b- defN 23-Apr-24 21:28 hidet/ir/functors/module_functor.py
+-rw-r--r--  2.0 unx    12215 b- defN 23-Apr-24 21:28 hidet/ir/functors/stmt_functor.py
+-rw-r--r--  2.0 unx     3707 b- defN 23-Apr-24 21:28 hidet/ir/functors/type_functor.py
+-rw-r--r--  2.0 unx     1328 b- defN 23-Apr-24 21:28 hidet/ir/primitives/__init__.py
+-rw-r--r--  2.0 unx     1116 b- defN 23-Apr-24 21:28 hidet/ir/primitives/debug.py
+-rw-r--r--  2.0 unx     5739 b- defN 23-Apr-24 21:28 hidet/ir/primitives/func.py
+-rw-r--r--  2.0 unx    11610 b- defN 23-Apr-24 21:28 hidet/ir/primitives/math.py
+-rw-r--r--  2.0 unx     1800 b- defN 23-Apr-24 21:28 hidet/ir/primitives/runtime.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cpu/__init__.py
+-rw-r--r--  2.0 unx      673 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cpu/math/__init__.py
+-rw-r--r--  2.0 unx     3212 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cpu/math/bfloat16.py
+-rw-r--r--  2.0 unx     5404 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cpu/math/float16.py
+-rw-r--r--  2.0 unx     5476 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cpu/math/float32.py
+-rw-r--r--  2.0 unx     5442 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cpu/math/float64.py
+-rw-r--r--  2.0 unx     3034 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cpu/math/int32.py
+-rw-r--r--  2.0 unx     3034 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cpu/math/int64.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/__init__.py
+-rw-r--r--  2.0 unx     1840 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/atomic.py
+-rw-r--r--  2.0 unx     7479 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/cp_async.py
+-rw-r--r--  2.0 unx     2898 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/cvt.py
+-rw-r--r--  2.0 unx     2856 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/cvta.py
+-rw-r--r--  2.0 unx     2246 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/funcs.py
+-rw-r--r--  2.0 unx     8543 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/ldst.py
+-rw-r--r--  2.0 unx    14458 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/mma.py
+-rw-r--r--  2.0 unx     4736 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/mutex.py
+-rw-r--r--  2.0 unx     1983 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/shfl.py
+-rw-r--r--  2.0 unx     2273 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/smem.py
+-rw-r--r--  2.0 unx     1934 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/sync.py
+-rw-r--r--  2.0 unx     1750 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/time.py
+-rw-r--r--  2.0 unx     2683 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/vars.py
+-rw-r--r--  2.0 unx    12898 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/wmma.py
+-rw-r--r--  2.0 unx      673 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/math/__init__.py
+-rw-r--r--  2.0 unx     3787 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/math/bfloat16.py
+-rw-r--r--  2.0 unx     7382 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/math/float16.py
+-rw-r--r--  2.0 unx     5484 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/math/float32.py
+-rw-r--r--  2.0 unx     5451 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/math/float64.py
+-rw-r--r--  2.0 unx     3043 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/math/int32.py
+-rw-r--r--  2.0 unx     3350 b- defN 23-Apr-24 21:28 hidet/ir/primitives/cuda/math/int64.py
+-rw-r--r--  2.0 unx      819 b- defN 23-Apr-24 21:28 hidet/ir/tools/__init__.py
+-rw-r--r--  2.0 unx     2769 b- defN 23-Apr-24 21:28 hidet/ir/tools/free_var_collector.py
+-rw-r--r--  2.0 unx     5649 b- defN 23-Apr-24 21:28 hidet/ir/tools/hasher.py
+-rw-r--r--  2.0 unx    19438 b- defN 23-Apr-24 21:28 hidet/ir/tools/printer.py
+-rw-r--r--  2.0 unx     2968 b- defN 23-Apr-24 21:28 hidet/ir/tools/rewriter.py
+-rw-r--r--  2.0 unx     5804 b- defN 23-Apr-24 21:28 hidet/ir/tools/simplifier.py
+-rw-r--r--  2.0 unx     7252 b- defN 23-Apr-24 21:28 hidet/ir/tools/type_infer.py
+-rw-r--r--  2.0 unx     3276 b- defN 23-Apr-24 21:28 hidet/ir/tools/util_functors.py
+-rw-r--r--  2.0 unx      744 b- defN 23-Apr-24 21:28 hidet/ir/utils/__init__.py
+-rw-r--r--  2.0 unx     3561 b- defN 23-Apr-24 21:28 hidet/ir/utils/call_graph.py
+-rw-r--r--  2.0 unx     1038 b- defN 23-Apr-24 21:28 hidet/ir/utils/expr_utils.py
+-rw-r--r--  2.0 unx     1414 b- defN 23-Apr-24 21:28 hidet/ir/utils/hash_sum.py
+-rw-r--r--  2.0 unx     1325 b- defN 23-Apr-24 21:28 hidet/ir/utils/index_transform.py
+-rw-r--r--  2.0 unx     1811 b- defN 23-Apr-24 21:28 hidet/ir/utils/type_utils.py
+-rw-r--r--  2.0 unx     3446 b- defN 23-Apr-24 21:28 hidet/lang/__init__.py
+-rw-r--r--  2.0 unx     1826 b- defN 23-Apr-24 21:28 hidet/lang/attr.py
+-rw-r--r--  2.0 unx     2219 b- defN 23-Apr-24 21:28 hidet/lang/cuda.py
+-rw-r--r--  2.0 unx      653 b- defN 23-Apr-24 21:28 hidet/lang/layout.py
+-rw-r--r--  2.0 unx      963 b- defN 23-Apr-24 21:28 hidet/lang/mapping.py
+-rw-r--r--  2.0 unx      679 b- defN 23-Apr-24 21:28 hidet/lang/runtime.py
+-rw-r--r--  2.0 unx     4695 b- defN 23-Apr-24 21:28 hidet/lang/script.py
+-rw-r--r--  2.0 unx    41589 b- defN 23-Apr-24 21:28 hidet/lang/transpiler.py
+-rw-r--r--  2.0 unx     1880 b- defN 23-Apr-24 21:28 hidet/lang/type_utils.py
+-rwxr-xr-x  2.0 unx     7123 b- defN 23-Apr-24 21:28 hidet/lib/libhidet.so
+-rwxr-xr-x  2.0 unx    55385 b- defN 23-Apr-24 21:28 hidet/lib/libhidet_runtime.so
+-rw-r--r--  2.0 unx      670 b- defN 23-Apr-24 21:28 hidet/runtime/__init__.py
+-rw-r--r--  2.0 unx     4118 b- defN 23-Apr-24 21:28 hidet/runtime/device.py
+-rw-r--r--  2.0 unx     3191 b- defN 23-Apr-24 21:28 hidet/runtime/module.py
+-rw-r--r--  2.0 unx    13426 b- defN 23-Apr-24 21:28 hidet/runtime/storage.py
+-rw-r--r--  2.0 unx      751 b- defN 23-Apr-24 21:28 hidet/testing/__init__.py
+-rw-r--r--  2.0 unx     4542 b- defN 23-Apr-24 21:28 hidet/testing/onnx_models.py
+-rw-r--r--  2.0 unx     2091 b- defN 23-Apr-24 21:28 hidet/testing/onnx_utils.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-Apr-24 21:28 hidet/testing/torch_utils.py
+-rw-r--r--  2.0 unx     5263 b- defN 23-Apr-24 21:28 hidet/testing/utils.py
+-rw-r--r--  2.0 unx      615 b- defN 23-Apr-24 21:28 hidet/testing/models/__init__.py
+-rw-r--r--  2.0 unx     5544 b- defN 23-Apr-24 21:28 hidet/testing/models/resnet.py
+-rw-r--r--  2.0 unx     3096 b- defN 23-Apr-24 21:28 hidet/transforms/__init__.py
+-rw-r--r--  2.0 unx     6379 b- defN 23-Apr-24 21:28 hidet/transforms/add_explicit_cast.py
+-rw-r--r--  2.0 unx     3822 b- defN 23-Apr-24 21:28 hidet/transforms/base.py
+-rw-r--r--  2.0 unx     3587 b- defN 23-Apr-24 21:28 hidet/transforms/declare_to_let.py
+-rw-r--r--  2.0 unx     3204 b- defN 23-Apr-24 21:28 hidet/transforms/expand_let_expr.py
+-rw-r--r--  2.0 unx     2068 b- defN 23-Apr-24 21:28 hidet/transforms/explicit_unroll.py
+-rw-r--r--  2.0 unx     4296 b- defN 23-Apr-24 21:28 hidet/transforms/flatten_tensor_index.py
+-rw-r--r--  2.0 unx     4338 b- defN 23-Apr-24 21:28 hidet/transforms/flatten_tensor_slice.py
+-rw-r--r--  2.0 unx     6551 b- defN 23-Apr-24 21:28 hidet/transforms/generate_packed_func.py
+-rw-r--r--  2.0 unx     2025 b- defN 23-Apr-24 21:28 hidet/transforms/import_primitive_functions.py
+-rw-r--r--  2.0 unx     5684 b- defN 23-Apr-24 21:28 hidet/transforms/inline_function.py
+-rw-r--r--  2.0 unx     4342 b- defN 23-Apr-24 21:28 hidet/transforms/inline_let_stmt.py
+-rw-r--r--  2.0 unx     2811 b- defN 23-Apr-24 21:28 hidet/transforms/lower_protect_access.py
+-rw-r--r--  2.0 unx     3596 b- defN 23-Apr-24 21:28 hidet/transforms/lower_special_cast.py
+-rw-r--r--  2.0 unx     4694 b- defN 23-Apr-24 21:28 hidet/transforms/lower_task_mapping.py
+-rw-r--r--  2.0 unx     1845 b- defN 23-Apr-24 21:28 hidet/transforms/normalize_const_tensor.py
+-rw-r--r--  2.0 unx     2403 b- defN 23-Apr-24 21:28 hidet/transforms/propogate_launch_bound.py
+-rw-r--r--  2.0 unx     4786 b- defN 23-Apr-24 21:28 hidet/transforms/resolve_generic_primitive_function.py
+-rw-r--r--  2.0 unx    10235 b- defN 23-Apr-24 21:28 hidet/transforms/rule_based_simplifier.py
+-rw-r--r--  2.0 unx     1693 b- defN 23-Apr-24 21:28 hidet/transforms/simplify_stmt.py
+-rw-r--r--  2.0 unx      623 b- defN 23-Apr-24 21:28 hidet/transforms/common/__init__.py
+-rw-r--r--  2.0 unx     5662 b- defN 23-Apr-24 21:28 hidet/transforms/common/scope.py
+-rw-r--r--  2.0 unx      676 b- defN 23-Apr-24 21:28 hidet/transforms/instruments/__init__.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Apr-24 21:28 hidet/transforms/instruments/base.py
+-rw-r--r--  2.0 unx     1851 b- defN 23-Apr-24 21:28 hidet/transforms/instruments/profile_instrument.py
+-rw-r--r--  2.0 unx     1552 b- defN 23-Apr-24 21:28 hidet/transforms/instruments/save_ir_instrument.py
+-rw-r--r--  2.0 unx     1160 b- defN 23-Apr-24 21:28 hidet/utils/__init__.py
+-rw-r--r--  2.0 unx     2184 b- defN 23-Apr-24 21:28 hidet/utils/bench.py
+-rw-r--r--  2.0 unx     1176 b- defN 23-Apr-24 21:28 hidet/utils/cache_utils.py
+-rw-r--r--  2.0 unx     3283 b- defN 23-Apr-24 21:28 hidet/utils/doc.py
+-rw-r--r--  2.0 unx     1666 b- defN 23-Apr-24 21:28 hidet/utils/exiting.py
+-rw-r--r--  2.0 unx     2664 b- defN 23-Apr-24 21:28 hidet/utils/git_utils.py
+-rw-r--r--  2.0 unx     2401 b- defN 23-Apr-24 21:28 hidet/utils/namer.py
+-rw-r--r--  2.0 unx     2471 b- defN 23-Apr-24 21:28 hidet/utils/net_utils.py
+-rw-r--r--  2.0 unx     8524 b- defN 23-Apr-24 21:28 hidet/utils/netron.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-Apr-24 21:28 hidet/utils/ort_utils.py
+-rw-r--r--  2.0 unx      785 b- defN 23-Apr-24 21:28 hidet/utils/overrides.py
+-rw-r--r--  2.0 unx    11570 b- defN 23-Apr-24 21:28 hidet/utils/py.py
+-rw-r--r--  2.0 unx      822 b- defN 23-Apr-24 21:28 hidet/utils/stack_limit.py
+-rw-r--r--  2.0 unx     4794 b- defN 23-Apr-24 21:28 hidet/utils/structure.py
+-rw-r--r--  2.0 unx     2272 b- defN 23-Apr-24 21:28 hidet/utils/torch_utils.py
+-rw-r--r--  2.0 unx     1891 b- defN 23-Apr-24 21:28 hidet/utils/transformers_utils.py
+-rw-r--r--  2.0 unx     3878 b- defN 23-Apr-24 21:28 hidet-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 21:28 hidet-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      136 b- defN 23-Apr-24 21:28 hidet-0.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-24 21:28 hidet-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    28771 b- defN 23-Apr-24 21:28 hidet-0.2.3.dist-info/RECORD
+318 files, 1822821 bytes uncompressed, 523591 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -243,15 +243,21 @@
 
 Filename: hidet/graph/ops/definitions/special.py
 Comment: 
 
 Filename: hidet/graph/ops/definitions/transform.py
 Comment: 
 
-Filename: hidet/graph/ops/definitions/utils.py
+Filename: hidet/graph/ops/definitions/attention/__init__.py
+Comment: 
+
+Filename: hidet/graph/ops/definitions/attention/attention.py
+Comment: 
+
+Filename: hidet/graph/ops/definitions/attention/attention_mask.py
 Comment: 
 
 Filename: hidet/graph/ops/definitions/conv2d/__init__.py
 Comment: 
 
 Filename: hidet/graph/ops/definitions/conv2d/conv2d.py
 Comment: 
@@ -291,14 +297,23 @@
 
 Filename: hidet/graph/ops/definitions/conv3d/resolve.py
 Comment: 
 
 Filename: hidet/graph/ops/definitions/conv3d/utils.py
 Comment: 
 
+Filename: hidet/graph/ops/definitions/fusion/__init__.py
+Comment: 
+
+Filename: hidet/graph/ops/definitions/fusion/apply_prologue_epilogue.py
+Comment: 
+
+Filename: hidet/graph/ops/definitions/fusion/fused_operator.py
+Comment: 
+
 Filename: hidet/graph/ops/definitions/matmul/__init__.py
 Comment: 
 
 Filename: hidet/graph/ops/definitions/matmul/batch_matmul.py
 Comment: 
 
 Filename: hidet/graph/ops/definitions/matmul/matmul.py
@@ -318,14 +333,23 @@
 
 Filename: hidet/graph/ops/definitions/reduce/reduce_f16.py
 Comment: 
 
 Filename: hidet/graph/ops/definitions/reduce/resolve.py
 Comment: 
 
+Filename: hidet/graph/ops/definitions/utils/__init__.py
+Comment: 
+
+Filename: hidet/graph/ops/definitions/utils/tensor_utils.py
+Comment: 
+
+Filename: hidet/graph/ops/definitions/utils/tune.py
+Comment: 
+
 Filename: hidet/graph/ops/schedules/__init__.py
 Comment: 
 
 Filename: hidet/graph/ops/schedules/auto_scheduler.py
 Comment: 
 
 Filename: hidet/graph/ops/schedules/common.py
@@ -333,17 +357,14 @@
 
 Filename: hidet/graph/ops/schedules/resolve.py
 Comment: 
 
 Filename: hidet/graph/ops/schedules/scheduler.py
 Comment: 
 
-Filename: hidet/graph/ops/schedules/tune.py
-Comment: 
-
 Filename: hidet/graph/ops/schedules/cpu/__init__.py
 Comment: 
 
 Filename: hidet/graph/ops/schedules/cpu/auto_scheduler.py
 Comment: 
 
 Filename: hidet/graph/ops/schedules/cuda/__init__.py
@@ -408,14 +429,17 @@
 
 Filename: hidet/graph/transforms/graph_patterns/__init__.py
 Comment: 
 
 Filename: hidet/graph/transforms/graph_patterns/arithmetic_patterns.py
 Comment: 
 
+Filename: hidet/graph/transforms/graph_patterns/attn_patterns.py
+Comment: 
+
 Filename: hidet/graph/transforms/graph_patterns/base.py
 Comment: 
 
 Filename: hidet/graph/transforms/graph_patterns/conv2d_patterns.py
 Comment: 
 
 Filename: hidet/graph/transforms/graph_patterns/matmul_patterns.py
@@ -438,14 +462,20 @@
 
 Filename: hidet/include/hidet/packedfunc.h
 Comment: 
 
 Filename: hidet/include/hidet/runtime.h
 Comment: 
 
+Filename: hidet/include/hidet/cpu/bfloat16.h
+Comment: 
+
+Filename: hidet/include/hidet/cpu/float16.h
+Comment: 
+
 Filename: hidet/include/hidet/runtime/callbacks.h
 Comment: 
 
 Filename: hidet/include/hidet/runtime/common.h
 Comment: 
 
 Filename: hidet/include/hidet/runtime/context.h
@@ -585,14 +615,20 @@
 
 Filename: hidet/ir/primitives/cpu/__init__.py
 Comment: 
 
 Filename: hidet/ir/primitives/cpu/math/__init__.py
 Comment: 
 
+Filename: hidet/ir/primitives/cpu/math/bfloat16.py
+Comment: 
+
+Filename: hidet/ir/primitives/cpu/math/float16.py
+Comment: 
+
 Filename: hidet/ir/primitives/cpu/math/float32.py
 Comment: 
 
 Filename: hidet/ir/primitives/cpu/math/float64.py
 Comment: 
 
 Filename: hidet/ir/primitives/cpu/math/int32.py
@@ -666,20 +702,26 @@
 
 Filename: hidet/ir/primitives/cuda/math/int64.py
 Comment: 
 
 Filename: hidet/ir/tools/__init__.py
 Comment: 
 
+Filename: hidet/ir/tools/free_var_collector.py
+Comment: 
+
 Filename: hidet/ir/tools/hasher.py
 Comment: 
 
 Filename: hidet/ir/tools/printer.py
 Comment: 
 
+Filename: hidet/ir/tools/rewriter.py
+Comment: 
+
 Filename: hidet/ir/tools/simplifier.py
 Comment: 
 
 Filename: hidet/ir/tools/type_infer.py
 Comment: 
 
 Filename: hidet/ir/tools/util_functors.py
@@ -696,17 +738,14 @@
 
 Filename: hidet/ir/utils/hash_sum.py
 Comment: 
 
 Filename: hidet/ir/utils/index_transform.py
 Comment: 
 
-Filename: hidet/ir/utils/task_utils.py
-Comment: 
-
 Filename: hidet/ir/utils/type_utils.py
 Comment: 
 
 Filename: hidet/lang/__init__.py
 Comment: 
 
 Filename: hidet/lang/attr.py
@@ -783,26 +822,32 @@
 
 Filename: hidet/transforms/declare_to_let.py
 Comment: 
 
 Filename: hidet/transforms/expand_let_expr.py
 Comment: 
 
+Filename: hidet/transforms/explicit_unroll.py
+Comment: 
+
 Filename: hidet/transforms/flatten_tensor_index.py
 Comment: 
 
 Filename: hidet/transforms/flatten_tensor_slice.py
 Comment: 
 
 Filename: hidet/transforms/generate_packed_func.py
 Comment: 
 
 Filename: hidet/transforms/import_primitive_functions.py
 Comment: 
 
+Filename: hidet/transforms/inline_function.py
+Comment: 
+
 Filename: hidet/transforms/inline_let_stmt.py
 Comment: 
 
 Filename: hidet/transforms/lower_protect_access.py
 Comment: 
 
 Filename: hidet/transforms/lower_special_cast.py
@@ -840,23 +885,14 @@
 
 Filename: hidet/transforms/instruments/profile_instrument.py
 Comment: 
 
 Filename: hidet/transforms/instruments/save_ir_instrument.py
 Comment: 
 
-Filename: hidet/transforms/tools/__init__.py
-Comment: 
-
-Filename: hidet/transforms/tools/apply_prologue_epilogue.py
-Comment: 
-
-Filename: hidet/transforms/tools/generate_packed_func.py
-Comment: 
-
 Filename: hidet/utils/__init__.py
 Comment: 
 
 Filename: hidet/utils/bench.py
 Comment: 
 
 Filename: hidet/utils/cache_utils.py
@@ -897,23 +933,23 @@
 
 Filename: hidet/utils/torch_utils.py
 Comment: 
 
 Filename: hidet/utils/transformers_utils.py
 Comment: 
 
-Filename: hidet-0.2.2.dist-info/METADATA
+Filename: hidet-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: hidet-0.2.2.dist-info/WHEEL
+Filename: hidet-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: hidet-0.2.2.dist-info/entry_points.txt
+Filename: hidet-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: hidet-0.2.2.dist-info/top_level.txt
+Filename: hidet-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: hidet-0.2.2.dist-info/RECORD
+Filename: hidet-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hidet/driver.py

```diff
@@ -14,14 +14,15 @@
 import os
 import multiprocessing
 import logging
 from hashlib import sha256
 import psutil
 from tqdm import tqdm
 
+import hidet.cuda
 from hidet import option
 from hidet.transforms import lower, PassContext, SaveIRInstrument, ProfileInstrument
 from hidet.backend import codegen, compile_source, load_task_func, load_lib_func
 from hidet.backend.build import CompilationFailed
 from hidet.utils.py import cyan, green, Timer
 from hidet.ir.task import Task
 from hidet.ir.func import IRModule, Function
@@ -80,15 +81,15 @@
             logger.info(f"Compiling {target_device} task {green(task.signature())}...")
             # build from scratch
             os.makedirs(task_dir, exist_ok=True)
             # write task
             with open(os.path.join(task_dir, 'task.txt'), 'w') as f:
                 f.write(task_string)
             # implement task
-            ir_module = task.implement(target=target_device, workding_dir=task_dir)
+            ir_module = task.implement(target=target_device, working_dir=task_dir)
             # lower ir module
             if option.get_option('save_lower_ir'):
                 instruments = [
                     SaveIRInstrument(out_dir=os.path.join(task_dir, './ir')),
                     ProfileInstrument(log_file=os.path.join(task_dir, './lower_time.txt')),
                 ]
             else:
@@ -115,18 +116,37 @@
     except CompilationFailed as e:
         if option.get_option('parallel_build'):
             return False
         else:
             raise e
 
 
+def _lazy_initialize_cuda():
+    # We intentionally query the cuda device information to put the properties of all devices to the lru_cache.
+    #
+    # Reasons:
+    #   Hidet relies on the multiprocessing to parallelize the compilation. During the process, the forked process will
+    #   query the properties of the device. If we do not cache the properties, the forked process will query the device
+    #   via the cuda runtime API. However, the cuda runtime API does not work when the multiprocessing package is
+    #   working in the fork mode. With the properties of all the GPUs cached, the forked process will not run any cuda
+    #   runtime API and will not cause any problem.
+    if getattr(_lazy_initialize_cuda, '_initialized', False):
+        return
+    _lazy_initialize_cuda._initialized = True  # pylint: disable=protected-access
+    if hidet.cuda.available():
+        for i in range(hidet.cuda.device_count()):
+            hidet.cuda.properties(i)
+            hidet.cuda.compute_capability(i)
+
+
 def build_task_batch(tasks: List[Task], target_device: str = 'cuda', raise_on_error: bool = True):
     dumped_options = option.dump_options()
     jobs = [(task, target_device, dumped_options) for task in tasks]
     if option.get_option('parallel_build') and len(jobs) > 1:
+        _lazy_initialize_cuda()
         with multiprocessing.Pool() as pool:
             status_list = list(pool.map(_build_task_job, jobs))
     else:
         status_list = list(map(_build_task_job, jobs))
     if not all(status_list) and raise_on_error:
         msg = ['Failed to build {} tasks:'.format(sum(1 for s in status_list if not s))]
         for task, status in zip(tasks, status_list):
@@ -135,87 +155,78 @@
         msg.append('Please turn off parallel build to see the error message:')
         msg.append('  hidet.option.parallel_build(False)')
         raise RuntimeError('\n'.join(msg))
 
 
 def build_ir_module(
     ir_module: IRModule,
-    func_name: str,
     output_dir='./outs/ir_module',
     save_ir: bool = True,
     profile_pass: bool = True,
     load: bool = True,
     use_hash_dir: bool = True,
 ):
     if use_hash_dir:
         hash_dir = sha256(str(ir_module).encode()).hexdigest()[:16]
         output_dir = os.path.join(output_dir, hash_dir)
 
     src_path = os.path.join(output_dir, 'source.cu')
     lib_path = os.path.join(output_dir, 'lib.so')
 
-    # get function type
-    func: Function = ir_module.lookup(func_name)
-    if func.kind == 'packed_func':
-        packed_func = ir_module.lookup(func.attrs['packed_func'])
-        func_type = FuncType.from_func(packed_func)
-    else:
-        func_type = FuncType.from_func(func)
-
     # lower ir module
     instruments = []
     if save_ir:
         instruments.append(SaveIRInstrument(out_dir=os.path.join(output_dir, './ir')))
     if profile_pass:
         instruments.append(ProfileInstrument(log_file=os.path.join(output_dir, './lower_time.txt')))
     with PassContext(instruments=instruments):
         ir_module = lower(ir_module)
 
+    # get function type
+    func: Function = ir_module.lookup('launch')
+    kernel_func = ir_module.lookup(func.attrs['packed_func'])
+    func_type = FuncType.from_func(kernel_func)
+
     # code generation
     codegen(ir_module, src_out_path=src_path)
 
     # compile source code
     compile_source(src_path, out_lib_path=lib_path, keep_ptx=False)
 
     if load:
         # load function
-        return load_lib_func(lib_path, 'hidet_' + func_name, func_type=func_type, src_path=src_path)
+        return load_lib_func(lib_path, 'hidet_launch', func_type=func_type, src_path=src_path)
     else:
-        return lib_path, func_name, func_type
+        return lib_path, func_type
 
 
-def _build_ir_module_job(args) -> Optional[Tuple[str, str, FuncType]]:
-    ir_module, func_name, output_dir, dumped_options = args
+def _build_ir_module_job(args) -> Optional[Tuple[str, FuncType]]:
+    ir_module, output_dir, dumped_options = args
     option.restore_options(dumped_options)
     try:
-        return build_ir_module(
-            ir_module, func_name, output_dir, save_ir=False, profile_pass=False, load=False, use_hash_dir=False
-        )
+        return build_ir_module(ir_module, output_dir, save_ir=False, profile_pass=False, load=False, use_hash_dir=False)
     except subprocess.CalledProcessError:
         print('Failed launch subprocess to compile the lowered source code via nvcc.')
         return None
     except CompilationFailed:
         print('Failed to compile the lowered source code via nvcc.')
         return None
 
 
 def build_ir_module_batch(
-    ir_modules: Sequence[IRModule], func_name: str, output_dir: str, parallel=True, verbose=False
+    ir_modules: Sequence[IRModule], output_dir: str, parallel=True, verbose=False
 ) -> List[Optional[CompiledFunction]]:
     """
     Build a batch of ir modules.
 
     Parameters
     ----------
     ir_modules: Sequence[IRModule]
         A sequence of ir modules to build.
 
-    func_name: str
-        The name of the function to load after building.
-
     output_dir: str
         The output directory to save the compiled library and source code (lib.so and source.cu).
 
     parallel: bool
         Whether build in parallel. Default True.
 
     verbose: bool
@@ -226,46 +237,48 @@
     funcs:
         The compiled functions, in the same order as build_instances.
         When the build for a build instance failed, None for that instance is returned.
     """
     with Timer() as timer:
         dumped_options = option.dump_options()
         jobs = [
-            (ir_module, func_name, os.path.join(output_dir, str(idx)), dumped_options)
-            for idx, ir_module in enumerate(ir_modules)
+            (ir_module, os.path.join(output_dir, str(idx)), dumped_options) for idx, ir_module in enumerate(ir_modules)
         ]
         build_results = []
         if parallel:
             # Set the affinity of current process. Some package such as numpy will change affinity of current process,
             # which might limit the parallelism of compilation.
             os.sched_setaffinity(0, range(os.cpu_count()))
 
             # the maximum number of processes is limited by the number of cores and memory
             mem_for_worker = 1.5 * 1024 * 1024 * 1024  # 1.5 GiB
             num_workers = min(max(int(psutil.virtual_memory().available // mem_for_worker), 1), psutil.cpu_count())
 
+            _lazy_initialize_cuda()
             with multiprocessing.Pool(processes=num_workers) as pool:
                 for build_result in tqdm(
                     pool.imap(_build_ir_module_job, jobs),
                     desc='Compiling',
                     total=len(jobs),
                     disable=not verbose,
                     ncols=80,
                 ):
                     build_results.append(build_result)
         else:
             # sequential build
+            for job in tqdm(jobs, desc='Compiling', disable=not verbose, ncols=80):
+                build_results.append(_build_ir_module_job(job))
             build_results = list(map(_build_ir_module_job, jobs))
 
         # load compiled functions
         funcs: List[Optional[CompiledFunction]] = []
         for build_result in build_results:
             if build_result is not None:
-                lib_path, func_name, func_type = build_result
-                funcs.append(load_lib_func(lib_path, 'hidet_' + func_name, func_type))
+                lib_path, func_type = build_result
+                funcs.append(load_lib_func(lib_path, 'hidet_launch', func_type))
             else:
                 funcs.append(None)
     if verbose:
         print(
             'Batch build {} modules within {:.3f} seconds, on average {:.1f} seconds per module.'.format(
                 len(jobs), timer.elapsed_seconds(), timer.elapsed_seconds() / len(jobs)
             )
```

## hidet/version.py

```diff
@@ -5,8 +5,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.2.2"
+__version__ = "0.2.3"
```

## hidet/backend/build.py

```diff
@@ -183,16 +183,16 @@
     """
     try:
         lib = SharedLibrary(lib_path)
     except OSError as e:
         print("Removed the file '{}'".format(lib_path))
         os.remove(lib_path)
         raise e
-    func_name = 'hidet_{}'.format(task.name)
-    param_types = [param.type for param in task.parameters]
+    func_name = 'hidet_launch'
+    param_types = [param.type for param in task.params]
     packed_func = PackedFunc(param_types=param_types, c_func_pointer=lib[func_name])
 
     potential_src_path = os.path.join(os.path.dirname(lib_path), 'source.cu')
     if os.path.isfile(potential_src_path):
         src_path = potential_src_path
     else:
         src_path = None
```

## hidet/backend/codegen.py

```diff
@@ -12,21 +12,21 @@
 from typing import Optional, List, Tuple, Dict, Union
 import os
 import numpy as np
 from hidet.ir.dialects.pattern import AnyExpr
 from hidet.ir import dtypes
 from hidet.ir.type import DataType, PointerType, TensorPointerType, ReferenceType, TensorType, FuncType
 from hidet.ir.type import VoidType
-from hidet.ir.expr import Var, Expr, Add, Sub, Multiply, Div, Mod, FloorDiv, LessThan, Neg, NotEqual, Equal, LogicalAnd
+from hidet.ir.expr import Var, Add, Sub, Multiply, Div, Mod, FloorDiv, LessThan, Neg, NotEqual, Equal, LogicalAnd
 from hidet.ir.expr import LogicalOr, LogicalNot, BitwiseAnd, BitwiseOr, BitwiseXor, BitwiseNot, LeftShift, RightShift
 from hidet.ir.expr import IfThenElse, Cast, Address, Reference, Dereference, Call, Let, Constant, TensorSlice, convert
 from hidet.ir.expr import TensorElement
 from hidet.ir.stmt import DeclareScope, DeclareStmt, EvaluateStmt, BufferStoreStmt, AssignStmt, LetStmt, ForStmt
 from hidet.ir.stmt import LaunchKernelStmt
-from hidet.ir.stmt import ForTaskStmt, WhileStmt, BreakStmt, ContinueStmt, IfStmt, ReturnStmt, AssertStmt, AsmStmt
+from hidet.ir.stmt import ForMappingStmt, WhileStmt, BreakStmt, ContinueStmt, IfStmt, ReturnStmt, AssertStmt, AsmStmt
 from hidet.ir.stmt import BlackBoxStmt, SeqStmt
 from hidet.ir.func import IRModule, Function
 from hidet.ir.compute import TensorNode, ScalarNode
 from hidet.ir.functors import ModuleFunctor, StmtFunctor, ExprFunctor, TypeFunctor
 from hidet.ir.tools import TypeInfer
 from hidet.utils.doc import Doc, NewLine, Text, doc_join
 from hidet.ir.utils.call_graph import CallGraph
@@ -43,14 +43,17 @@
         self.namer = Namer()
         self.type_infer = TypeInfer()
 
     @staticmethod
     def canonize_funcname(name: str):
         return 'hidet_' + name.replace('.', '_')
 
+    def scalar_literal(self, value, dtype: DataType):
+        raise NotImplementedError()
+
     def param_declare(self, v: Var):
         v_type = v.type
         name_doc = self(v)
         if isinstance(v_type, DataType):
             dtype_doc = self(v_type)
             return dtype_doc + ' ' + name_doc
         elif isinstance(v_type, PointerType):
@@ -159,97 +162,18 @@
 
     def visit_PyConstant(self, c: Union[str, int, float, None]):
         if c is None:
             raise RuntimeError('None encountered during code generation')
         return Text(str(c))
 
     def visit_IRModule(self, module: IRModule) -> Doc:
-        self.ir_module = module
-        doc = Doc()
-        # todo: only add necessary headers
-        doc += Text('#include <stdint.h>') + NewLine()
-        doc += Text('#include <cuda_fp16.h>') + NewLine()
-        doc += Text('#include <cuda_bf16.h>') + NewLine()
-        doc += Text('#include <hidet/runtime/cuda_context.h>') + NewLine()
-        doc += Text('#include <hidet/runtime/cpu_context.h>') + NewLine()
-
-        # nvcc use float to 'store' tfloat32 data
-        doc += Text('typedef float tfloat32_t;') + NewLine()
-
-        # According to here: https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#wmma-altfp
-        # there should be a function called '__float_to_tf32' in cuda c to convert float to tfloat32,
-        # but I did not find such a function. By looking at cutlass's implementation of converting
-        # float to tfloat32, it seems that we do not need to do anything to convert. Put a definition
-        # here in case nvidia add the definition in the future.
-        doc += Text('#define __float_to_tf32(x) (x)') + NewLine()
-
-        if module.task is not None:
-            doc += '/*' + NewLine()
-            doc += str(module.task) + NewLine()
-            doc += '*/' + NewLine()
-        doc += Text('extern "C" {') + NewLine()
-
-        call_graph = CallGraph(module)
-        for node in call_graph.reversed_order:
-            doc += self(node.func) + NewLine()
-
-        doc += NewLine() + '}'
-        return doc
+        raise NotImplementedError()
 
     def visit_Function(self, func: Function) -> Doc:
-        self.namer.clear()
-
-        doc = NewLine()
-
-        # ret
-        if func.kind == 'cuda_kernel':
-            doc += '__global__'
-        elif func.kind == 'cuda_device':
-            doc += '__device__ __forceinline__'
-        elif func.kind in ['packed_func', 'host_kernel']:
-            doc += '__host__'
-
-        doc += ' ' + self(func.ret_type)
-        # doc += ' void'
-
-        # launch bound for grid worker
-        if func.kind == 'cuda_kernel':
-            block_dim = func.attrs['cuda_block_dim']
-            if isinstance(block_dim, list):
-                block_dim = prod(block_dim)
-            if 'cuda_min_blocks' in func.attrs:
-                min_blocks = func.attrs['cuda_min_blocks']
-                doc += f' __launch_bounds__({block_dim}, {min_blocks})'
-            else:
-                doc += f' __launch_bounds__({block_dim})'
-
-        # func name
-        canonized_func_name = self.canonize_funcname(func.name)
-        doc += ' ' + canonized_func_name
-        self.func_name_map[func.name] = canonized_func_name
-
-        # parameters
-        doc += '('
-        param_docs = []
-        for param in func.params:
-            param_docs.append(self.param_declare(param))
-        doc += doc_join(param_docs, Text(', '))
-        doc += ') {'
-
-        # comments
-        label = func.get_attr('label', default=None, allow_missing=True)
-        if label:
-            doc += (NewLine() + '// label: {}'.format(label)).indent()
-
-        # body
-        doc += self(func.body).indent()
-
-        doc += NewLine() + '}'
-
-        return doc
+        raise NotImplementedError()
 
     def visit_Add(self, e: Add):
         return Text('(') + self(e.a) + ' + ' + self(e.b) + ')'
 
     def visit_Sub(self, e: Sub):
         return Text('(') + self(e.a) + ' - ' + self(e.b) + ')'
 
@@ -324,29 +248,29 @@
         src_dtype = self.type_infer(e.expr)
         dst_dtype = e.target_type
         if isinstance(src_dtype, DataType) and isinstance(dst_dtype, DataType) and src_dtype == dtypes.float16:
             # in cuda, cuda_fp16.h only defines the half struct with conversion operators for the types like float,
             # short, int, unsigned int, long long, unsigned long long, but not for the types like int8_t, uint8_t,
             # int16_t, uint16_t, int32_t, uint32_t, int64_t, uint64_t, so we need to cast them here.
             if dst_dtype == dtypes.int64:
-                return '(int64_t)(' + self(e.expr) + ')'
+                return '(int64_t)((long long)(' + self(e.expr) + '))'
             elif dst_dtype == dtypes.uint64:
-                return '(uint64_t)(' + self(e.expr) + ')'
+                return '(uint64_t)((unsigned long long)(' + self(e.expr) + '))'
             elif dst_dtype == dtypes.int32:
                 return '(int32_t)(' + self(e.expr) + ')'
             elif dst_dtype == dtypes.uint32:
                 return '(uint32_t)(' + self(e.expr) + ')'
             elif dst_dtype == dtypes.int16:
                 return '(int16_t)(' + self(e.expr) + ')'
             elif dst_dtype == dtypes.uint16:
                 return '(uint16_t)(' + self(e.expr) + ')'
             elif dst_dtype == dtypes.int8:
-                return '(int8_t)(' + self(e.expr) + ')'
+                return '(int8_t)(short)(' + self(e.expr) + ')'
             elif dst_dtype == dtypes.uint8:
-                return '(uint8_t)(' + self(e.expr) + ')'
+                return '(uint8_t)(unsigned short)(' + self(e.expr) + ')'
             elif dst_dtype == dtypes.boolean:
                 return '(bool)(' + self(e.expr) + ')'
             elif dst_dtype == dtypes.float32:
                 return '(float)(' + self(e.expr) + ')'
             elif dst_dtype == dtypes.float64:
                 return '(double)(' + self(e.expr) + ')'
             else:
@@ -365,36 +289,17 @@
 
     def visit_Call(self, e: Call):
         func_name = e.func_var.hint
         if func_name in self.ir_module.functions:
             func = self.ir_module.lookup(func_name)
             func_name = Text(self.canonize_funcname(func_name))
             if func.kind == 'cuda_kernel':
-
-                if isinstance(func.attrs['cuda_block_dim'], int) and func.attrs['cuda_block_dim'] > 1024:
-                    raise ValueError('CUDA block dimension cannot be larger than 1024.')
-
-                def dim3_str(dims):
-                    if isinstance(dims, (int, Expr)):
-                        return self(dims)
-                    else:
-                        return Text('dim3(') + self(dims) + ')'
-
-                configs = [
-                    dim3_str(func.attrs['cuda_grid_dim']),  # grid dimension
-                    dim3_str(func.attrs['cuda_block_dim']),  # block dimension
-                    func.attrs.get('cuda_dynamic_smem_bytes', 0),  # dynamic shared memory size
-                    # cuda stream (get_cuda_stream() function is defined in hidet/runtime.h)
-                    '(cudaStream_t)get_cuda_stream()',
-                ]
-                launch_config = Text('<<<') + doc_join([self(v) for v in configs], sep=', ') + Text('>>>')
-            else:
-                launch_config = []
+                raise RuntimeError('Call to cuda kernel should be lowered to LaunchKernelStmt.')
             param_doc = Text('(') + doc_join([self(arg) for arg in e.args], Text(', ')) + ')'
-            return func_name + launch_config + param_doc
+            return func_name + param_doc
         elif is_primitive_function(func_name):
             entry = lookup_primitive_function(func_name)
             if entry.function is not None:
                 msg = (
                     f"Please use import_primitive_functions pass to import primitive function first: {entry.name}, "
                     f"functions in current module:\n{list(self.ir_module.functions.keys())}."
                 )
@@ -420,48 +325,14 @@
         if name in cast2int:
             return Text(f'(int){name}')
         else:
             if isinstance(e.type, FuncType):
                 name = self.canonize_funcname(name)
             return Text(name)
 
-    @staticmethod
-    def scalar_literal(value, dtype: DataType):
-        if dtype == dtypes.boolean:
-            ret = 'true' if value else 'false'
-        elif dtype == dtypes.float64:
-            ret = '{}'.format(float(value))
-        elif dtype == dtypes.float32:
-            ret = '{}f'.format(float(value))
-        elif dtype == dtypes.float16:
-            ret = 'half({}f)'.format(float(value))
-        elif dtype == dtypes.tfloat32:
-            ret = '__float_to_tf32({}f)'.format(float(value))
-        elif dtype == dtypes.bfloat16:
-            ret = '__float2bfloat16({}f)'.format(float(value))
-        elif dtype == dtypes.int64:
-            ret = 'int64_t({}ll)'.format(int(value))
-        elif dtype == dtypes.int32:
-            ret = '{}'.format(int(value))
-        elif dtype == dtypes.int16:
-            ret = 'int16_t({})'.format(int(value))
-        elif dtype == dtypes.int8:
-            ret = 'int8_t({})'.format(int(value))
-        elif dtype == dtypes.uint64:
-            ret = 'uint64_t({}ull)'.format(int(value))
-        elif dtype == dtypes.uint32:
-            ret = 'uint32_t({}u)'.format(int(value))
-        elif dtype == dtypes.uint16:
-            ret = 'uint16_t({})'.format(int(value))
-        elif dtype == dtypes.uint8:
-            ret = 'uint8_t({})'.format(int(value))
-        else:
-            raise NotImplementedError('Cannot recognize scalar literal {} with dtype {}'.format(value, dtype))
-        return Text(ret)
-
     def visit_Constant(self, e: Constant):
         if e.is_scalar():
             return self.scalar_literal(e.value, e.type)
         else:
             assert isinstance(e.type, TensorType)
             dtype = e.type.dtype
             items = [self.scalar_literal(v, dtype) for v in np.array(e.value).flatten()]
@@ -509,29 +380,30 @@
 
     def visit_ForStmt(self, stmt: ForStmt):
         v = stmt.loop_var
         init_doc = self(v.type) + ' ' + self(v) + ' = ' + self(convert(0))
         cond_doc = self(v < stmt.extent)
         update_doc = self(v) + ' = ' + self(v + 1)
         doc = Text('')
-        if stmt.unroll is not None:
-            if isinstance(stmt.unroll, bool):
-                if stmt.unroll:
+        if stmt.attr.unroll is not None:
+            assert not stmt.attr.explicit_unroll, 'explicit_unroll should be lowered before codegen'
+            if isinstance(stmt.attr.unroll, bool):
+                if stmt.attr.unroll:
                     doc += NewLine() + '#pragma unroll'  # complete unroll
                 else:
                     doc += NewLine() + '#pragma unroll 1'  # prevent from unrolling
             else:
-                assert isinstance(stmt.unroll, int)
-                doc += NewLine() + '#pragma unroll {}'.format(stmt.unroll)
+                assert isinstance(stmt.attr.unroll, int)
+                doc += NewLine() + '#pragma unroll {}'.format(stmt.attr.unroll)
         doc += NewLine() + Text('for (') + init_doc + '; ' + cond_doc + '; ' + update_doc + ') '
         body_doc = self(stmt.body)
         doc += Text('{') + body_doc.indent() + NewLine() + Text('} ')
         return doc
 
-    def visit_ForTaskStmt(self, stmt: ForTaskStmt):
+    def visit_ForTaskStmt(self, stmt: ForMappingStmt):
         raise ValueError('ForTaskStmt should be lowered to ForStmt in lower_task_mapping pass before code generation.')
 
     def visit_WhileStmt(self, stmt: WhileStmt):
         doc = NewLine() + Text('while (') + self(stmt.cond) + ')'
         body_doc = self(stmt.body)
         doc += Text(' {') + body_doc.indent() + NewLine() + Text('} ')
         return doc
@@ -612,31 +484,15 @@
     def visit_SeqStmt(self, stmt: SeqStmt):
         doc = Doc()
         for s in stmt.seq:
             doc += self(s)
         return doc
 
     def visit_ScalarType(self, t: DataType):
-        scalar_type_map = {
-            'bool': 'bool',
-            'uint8': 'uint8_t',
-            'uint16': 'uint16_t',
-            'uint32': 'uint32_t',
-            'uint64': 'uint64_t',
-            'int8': 'int8_t',
-            'int16': 'int16_t',
-            'int32': 'int32_t',
-            'int64': 'int64_t',
-            'float16': 'half',
-            'float32': 'float',
-            'float64': 'double',
-            'bfloat16': 'nv_bfloat16',
-            'tfloat32': 'tfloat32_t',
-        }
-        return Text(scalar_type_map[t.name])
+        raise NotImplementedError()
 
     def visit_TensorType(self, t: TensorType):
         return Text('TensorType(') + self(t.dtype) + ', [' + doc_join([self(s) for s in t.shape], ", ") + '])'
 
     def visit_PointerType(self, t: PointerType):
         return self(t.base_type) + Text('*')
 
@@ -659,16 +515,282 @@
     def visit_TensorNode(self, e: TensorNode):
         raise ValueError()
 
     def visit_AnyExpr(self, e: AnyExpr):
         raise ValueError()
 
 
-def codegen(ir_module: IRModule, src_out_path: Optional[str] = None) -> str:
-    gen = Codegen()
+class CUDACodegen(Codegen):
+    # pylint: disable=abstract-method
+
+    def scalar_literal(self, value, dtype: DataType):
+        if dtype == dtypes.boolean:
+            ret = 'true' if value else 'false'
+        elif dtype == dtypes.float64:
+            ret = '{}'.format(float(value))
+        elif dtype == dtypes.float32:
+            ret = '{}f'.format(float(value))
+        elif dtype == dtypes.float16:
+            ret = 'half({}f)'.format(float(value))
+        elif dtype == dtypes.tfloat32:
+            ret = '__float_to_tf32({}f)'.format(float(value))
+        elif dtype == dtypes.bfloat16:
+            ret = '__float2bfloat16({}f)'.format(float(value))
+        elif dtype == dtypes.int64:
+            ret = 'int64_t({}ll)'.format(int(value))
+        elif dtype == dtypes.int32:
+            ret = '{}'.format(int(value))
+        elif dtype == dtypes.int16:
+            ret = 'int16_t({})'.format(int(value))
+        elif dtype == dtypes.int8:
+            ret = 'int8_t({})'.format(int(value))
+        elif dtype == dtypes.uint64:
+            ret = 'uint64_t({}ull)'.format(int(value))
+        elif dtype == dtypes.uint32:
+            ret = 'uint32_t({}u)'.format(int(value))
+        elif dtype == dtypes.uint16:
+            ret = 'uint16_t({})'.format(int(value))
+        elif dtype == dtypes.uint8:
+            ret = 'uint8_t({})'.format(int(value))
+        else:
+            raise NotImplementedError('Cannot recognize scalar literal {} with dtype {}'.format(value, dtype))
+        return Text(ret)
+
+    def visit_ScalarType(self, t: DataType):
+        scalar_type_map = {
+            'bool': 'bool',
+            'uint8': 'uint8_t',
+            'uint16': 'uint16_t',
+            'uint32': 'uint32_t',
+            'uint64': 'uint64_t',
+            'int8': 'int8_t',
+            'int16': 'int16_t',
+            'int32': 'int32_t',
+            'int64': 'int64_t',
+            'float16': 'half',
+            'float32': 'float',
+            'float64': 'double',
+            'bfloat16': 'nv_bfloat16',
+            'tfloat32': 'tfloat32_t',
+        }
+        return Text(scalar_type_map[t.name])
+
+    def visit_Function(self, func: Function) -> Doc:
+        self.namer.clear()
+
+        doc = NewLine()
+
+        # ret
+        if func.kind == 'cuda_kernel':
+            doc += '__global__'
+        elif func.kind == 'cuda_device':
+            doc += '__device__ __forceinline__'
+        elif func.kind in ['packed_func', 'host_kernel']:
+            doc += '__host__'
+
+        doc += ' ' + self(func.ret_type)
+        # doc += ' void'
+
+        # launch bound for grid worker
+        if func.kind == 'cuda_kernel':
+            block_dim = func.attrs['cuda_block_dim']
+            if isinstance(block_dim, list):
+                block_dim = prod(block_dim)
+            if 'cuda_min_blocks' in func.attrs:
+                min_blocks = func.attrs['cuda_min_blocks']
+                doc += f' __launch_bounds__({block_dim}, {min_blocks})'
+            else:
+                doc += f' __launch_bounds__({block_dim})'
+
+        # func name
+        canonized_func_name = self.canonize_funcname(func.name)
+        doc += ' ' + canonized_func_name
+        self.func_name_map[func.name] = canonized_func_name
+
+        # parameters
+        doc += '('
+        param_docs = []
+        for param in func.params:
+            param_docs.append(self.param_declare(param))
+        doc += doc_join(param_docs, Text(', '))
+        doc += ') {'
+
+        # comments
+        label = func.get_attr('label', default=None, allow_missing=True)
+        if label:
+            doc += (NewLine() + '// label: {}'.format(label)).indent()
+
+        # body
+        doc += self(func.body).indent()
+
+        doc += NewLine() + '}'
+
+        return doc
+
+    def visit_IRModule(self, module: IRModule) -> Doc:
+        self.ir_module = module
+        doc = Doc()
+        # todo: only add necessary headers
+        doc += Text('#include <stdint.h>') + NewLine()
+        doc += Text('#include <cuda_fp16.h>') + NewLine()
+        doc += Text('#include <cuda_bf16.h>') + NewLine()
+        doc += Text('#include <hidet/runtime/cuda_context.h>') + NewLine()
+        doc += Text('#include <hidet/runtime/cpu_context.h>') + NewLine()
+
+        # nvcc use float to 'store' tfloat32 data
+        doc += Text('typedef float tfloat32_t;') + NewLine()
+
+        # According to here: https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#wmma-altfp
+        # there should be a function called '__float_to_tf32' in cuda c to convert float to tfloat32,
+        # but I did not find such a function. By looking at cutlass's implementation of converting
+        # float to tfloat32, it seems that we do not need to do anything to convert. Put a definition
+        # here in case nvidia add the definition in the future.
+        doc += Text('#define __float_to_tf32(x) (x)') + NewLine()
+
+        if module.task is not None:
+            doc += '/*' + NewLine()
+            doc += str(module.task) + NewLine()
+            doc += '*/' + NewLine()
+        doc += Text('extern "C" {') + NewLine()
+
+        call_graph = CallGraph(module)
+        for node in call_graph.reversed_order:
+            doc += self(node.func) + NewLine()
+
+        doc += NewLine() + '}'
+        return doc
+
+
+class CPUCodegen(Codegen):
+    # pylint: disable=abstract-method
+
+    def scalar_literal(self, value, dtype: DataType):
+        if dtype == dtypes.boolean:
+            ret = 'true' if value else 'false'
+        elif dtype == dtypes.float64:
+            ret = '{}'.format(float(value))
+        elif dtype == dtypes.float32:
+            ret = '{}f'.format(float(value))
+        # current cpu has very poor support of float16, bfloat16
+        # like cuda did, we emulate them in include/cpu/float16.h and include/cpu/bfloat16.h
+        elif dtype == dtypes.float16:
+            ret = '(half){}f'.format(float(value))
+        elif dtype == dtypes.tfloat32:
+            ret = '(float){}f'.format(float(value))
+        elif dtype == dtypes.bfloat16:
+            ret = '(bfloat16_t){}f'.format(float(value))
+        elif dtype == dtypes.int64:
+            ret = 'int64_t({}ll)'.format(int(value))
+        elif dtype == dtypes.int32:
+            ret = '{}'.format(int(value))
+        elif dtype == dtypes.int16:
+            ret = 'int16_t({})'.format(int(value))
+        elif dtype == dtypes.int8:
+            ret = 'int8_t({})'.format(int(value))
+        elif dtype == dtypes.uint64:
+            ret = 'uint64_t({}ull)'.format(int(value))
+        elif dtype == dtypes.uint32:
+            ret = 'uint32_t({}u)'.format(int(value))
+        elif dtype == dtypes.uint16:
+            ret = 'uint16_t({})'.format(int(value))
+        elif dtype == dtypes.uint8:
+            ret = 'uint8_t({})'.format(int(value))
+        else:
+            raise NotImplementedError('Cannot recognize scalar literal {} with dtype {}'.format(value, dtype))
+        return Text(ret)
+
+    def visit_ScalarType(self, t: DataType):
+        # float16, bfloat16 and tfloat32 are not supported on CPU yet
+        # https://moocaholic.medium.com/fp64-fp32-fp16-bfloat16-tf32-and-other-members-of-the-zoo-a1ca7897d407
+        scalar_type_map = {
+            'bool': 'bool',
+            'uint8': 'uint8_t',
+            'uint16': 'uint16_t',
+            'uint32': 'uint32_t',
+            'uint64': 'uint64_t',
+            'int8': 'int8_t',
+            'int16': 'int16_t',
+            'int32': 'int32_t',
+            'int64': 'int64_t',
+            'float16': 'half',
+            'float32': 'float',
+            'float64': 'double',
+            'bfloat16': 'bfloat16_t',
+            'tfloat32': 'float',
+        }
+        return Text(scalar_type_map[t.name])
+
+    def visit_IRModule(self, module: IRModule) -> Doc:
+        self.ir_module = module
+        doc = Doc()
+        # todo: only add necessary headers
+        doc += Text('#include <stdint.h>') + NewLine()
+        doc += Text('#include <hidet/runtime/cpu_context.h>') + NewLine()
+        doc += Text('#include <math.h>') + NewLine()
+        # float16 and bfloat16 emulation
+        doc += Text('#include <hidet/cpu/float16.h>') + NewLine()
+        doc += Text('#include <hidet/cpu/bfloat16.h>') + NewLine()
+
+        if module.task is not None:
+            doc += '/*' + NewLine()
+            doc += str(module.task) + NewLine()
+            doc += '*/' + NewLine()
+
+        doc += Text('extern "C" {') + NewLine()
+
+        # add namespace to activate data type and function
+        doc += Text('using float16::Half;') + NewLine()
+        doc += Text('using bfloat16::BFloat16;') + NewLine()
+
+        # use typedef to map half and bfloat16 type
+        doc += Text('typedef Half half;') + NewLine()
+        doc += Text('typedef BFloat16 bfloat16_t;') + NewLine()
+
+        call_graph = CallGraph(module)
+        for node in call_graph.reversed_order:
+            doc += self(node.func) + NewLine()
+
+        doc += NewLine() + '}'
+        return doc
+
+    def visit_Function(self, func: Function) -> Doc:
+        self.namer.clear()
+
+        doc = NewLine()
+
+        doc += ' ' + self(func.ret_type)
+
+        # func name
+        canonized_func_name = self.canonize_funcname(func.name)
+        doc += ' ' + canonized_func_name
+        self.func_name_map[func.name] = canonized_func_name
+
+        # parameters
+        doc += '('
+        param_docs = []
+        for param in func.params:
+            param_docs.append(self.param_declare(param))
+        doc += doc_join(param_docs, Text(', '))
+        doc += ') {'
+
+        # comments
+        label = func.get_attr('label', default=None, allow_missing=True)
+        if label:
+            doc += (NewLine() + '// label: {}'.format(label)).indent()
+
+        # body
+        doc += self(func.body).indent()
+
+        doc += NewLine() + '}'
+
+        return doc
+
+
+def codegen(ir_module: IRModule, src_out_path: Optional[str] = None, target='cuda') -> str:
+    gen = CUDACodegen()
     doc = gen(ir_module)
     code = str(doc)
     if src_out_path is not None:
         dir_path = os.path.dirname(src_out_path)
         if not os.path.exists(dir_path):
             os.makedirs(dir_path)
         with open(src_out_path, 'w') as f:
```

## hidet/cli/bench/bench.py

```diff
@@ -5,15 +5,18 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Optional
 import click
+import torch
+import hidet
 from hidet.utils import initialize
 from . import vision
 from . import nlp
 from .model import BenchModel
 from .bench_common import bench_common
 from .bench_all import bench_all
 
@@ -23,23 +26,62 @@
     '--space',
     default='0',
     show_default=True,
     type=click.Choice(['0', '1', '2']),
     help='Schedule space. 0: default schedule. 1: small schedule space. 2: large schedule space.',
 )
 @click.option(
-    '--torch-tf32',
+    '--dtype', default='float32', show_default=True, type=click.Choice(['float32', 'float16']), help='Data type to use.'
+)
+@click.option(
+    '--tensor-core',
     default=False,
     show_default=True,
+    is_flag=True,
+    type=bool,
+    help='Whether to use tensor core in hidet.',
+)
+@click.option('--report', type=click.Path(exists=False, dir_okay=False, writable=True), help='Report file path.')
+@click.option(
+    '--disable-torch-cudnn-tf32',
+    default=False,
+    is_flag=True,
     type=bool,
-    help='Enable torch.backends.cuda.matmul.allow_tf32 and torch.backends.cudnn.allow_tf32.',
+    help='Set torch.backends.cudnn.allow_tf32=False.',
+)
+@click.option(
+    '--enable-torch-cublas-tf32',
+    default=False,
+    is_flag=True,
+    type=bool,
+    help='Set torch.backends.cuda.matmul.allow_tf32=True.',
+)
+@click.option(
+    '--cache-dir',
+    default=None,
+    type=click.Path(dir_okay=True, file_okay=False, writable=True),
+    help='The cache directory to store the generated kernels.',
 )
-def bench_group(space: str, torch_tf32: bool):
+def bench_group(
+    space: str,
+    dtype: str,
+    tensor_core: bool,
+    report: Optional[click.Path],
+    disable_torch_cudnn_tf32: bool,
+    enable_torch_cublas_tf32: bool,
+    cache_dir: Optional[click.Path],
+):
     BenchModel.search_space = int(space)
-    BenchModel.allow_tf32 = torch_tf32
+    BenchModel.dtype = getattr(torch, dtype)
+    BenchModel.tensor_core = tensor_core
+    BenchModel.disable_torch_cudnn_tf32 = disable_torch_cudnn_tf32
+    BenchModel.enable_torch_cublas_tf32 = enable_torch_cublas_tf32
+    BenchModel.report_path = report
+    if cache_dir:
+        hidet.option.cache_dir(str(cache_dir))
 
 
 @initialize()
 def register_commands():
     for command in [
         bench_common,
         bench_all,
```

## hidet/cli/bench/bench_all.py

```diff
@@ -16,8 +16,7 @@
 
 @click.command(name='all')
 def bench_all():
     header = BenchModel.headers()
     result = [bench_model.benchmark() for bench_model in all_registered_models]
 
     click.echo(tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left'))
-    click.echo('(PyTorch backend: allow_tf32={})'.format(BenchModel.allow_tf32))
```

## hidet/cli/bench/bench_common.py

```diff
@@ -16,8 +16,7 @@
 
 @click.command(name='common')
 def bench_common():
     header = BenchModel.headers()
     result = [bench_model.benchmark() for bench_model in commonly_used_models]
 
     click.echo(tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left'))
-    click.echo('(PyTorch backend: allow_tf32={})'.format(BenchModel.allow_tf32))
```

## hidet/cli/bench/model.py

```diff
@@ -6,22 +6,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # pylint: disable=ungrouped-imports, no-name-in-module
-from typing import List, Any
+from typing import List, Any, Optional
+import click
+import torch
 from hidet.testing import benchmark_func
 import hidet
 
 
 class BenchModel:
     search_space = 0
-    allow_tf32 = False
+    dtype: torch.dtype = torch.float32
+    tensor_core: bool = False
+    disable_torch_cudnn_tf32 = False
+    enable_torch_cublas_tf32 = False
+    report_path: Optional[str] = None
 
     def __str__(self):
         raise NotImplementedError()
 
     def model(self):
         """
         Returns a pytorch model to benchmark.
@@ -40,14 +46,32 @@
         Returns
         -------
         ret: Tuple[Sequence[torch.Tensor], Dict[str, torch.Tensor]]
             The inputs to pass to the model.
         """
         raise NotImplementedError()
 
+    def converted_model(self):
+        model = self.model().eval()
+        model = model.to(dtype=BenchModel.dtype)
+        model = model.cuda()
+        return model
+
+    def converted_inputs(self):
+        args, kwargs = self.example_inputs()
+
+        def convert_f32(arg):
+            if arg.dtype == torch.float32:
+                return arg.to(dtype=BenchModel.dtype)
+            return arg
+
+        args = [convert_f32(arg.cuda()) for arg in args]
+        kwargs = {k: convert_f32(v.cuda()) for k, v in kwargs.items()}
+        return args, kwargs
+
     @staticmethod
     def tensor_str(tensor) -> str:
         """
         Returns a string representation of a tensor.
 
         Parameters
         ----------
@@ -67,79 +91,90 @@
         Returns a string representation of the inputs to the model.
 
         Returns
         -------
         ret: str
             The string representation of the inputs to the model.
         """
-        args, kwargs = self.example_inputs()
+        args, kwargs = self.converted_inputs()
         items = []
         for arg in args:
             items.append(self.tensor_str(arg))
         for k, v in kwargs.items():
             items.append('{}={}'.format(k, self.tensor_str(v)))
         return ', '.join(items)
 
+    @classmethod
+    def report_table(cls, table_str):
+        if cls.report_path is not None:
+            with open(cls.report_path, 'w') as f:
+                click.echo(table_str, file=f)
+        click.echo(table_str)
+
     def bench_with_backend(self, backend: str, mode=None, warmup=3, number=10, repeat=10):
-        import torch.backends.cudnn
-        import torch.backends.cuda
+        try:
+            import torch.backends.cudnn  # pylint: disable=redefined-outer-name
+            import torch.backends.cuda
+
+            if not hidet.torch.dynamo_available():
+                raise RuntimeError('Torch Dynamo is not available, please install pytorch 2.0 or higher.')
+            import torch._dynamo as dynamo
+
+            torch.backends.cudnn.allow_tf32 = not self.disable_torch_cudnn_tf32
+            torch.backends.cuda.matmul.allow_tf32 = self.enable_torch_cublas_tf32
+
+            model, (args, kwargs) = self.converted_model(), self.converted_inputs()
+            dynamo.reset()
+            with torch.no_grad():
+                model_opt = torch.compile(model, backend=backend, mode=mode)
+                latency = benchmark_func(
+                    run_func=lambda: model_opt(*args, **kwargs), warmup=warmup, number=number, repeat=repeat
+                )
+            return latency
+        except Exception as e:  # pylint: disable=broad-except
+            from traceback import format_exc
 
-        if not hidet.torch.dynamo_available():
-            raise RuntimeError('Torch Dynamo is not available, please install pytorch 2.0 or higher.')
-        import torch._dynamo as dynamo
-
-        torch.backends.cudnn.allow_tf32 = self.allow_tf32
-        torch.backends.cuda.matmul.allow_tf32 = self.allow_tf32
-
-        model, (args, kwargs) = self.model(), self.example_inputs()
-        model = model.cuda().eval()
-        args = [arg.cuda() for arg in args]
-        kwargs = {k: v.cuda() for k, v in kwargs.items()}
-        dynamo.reset()
-        with torch.no_grad():
-            model_opt = torch.compile(model, backend=backend, mode=mode)
-            latency = benchmark_func(
-                run_func=lambda: model_opt(*args, **kwargs), warmup=warmup, number=number, repeat=repeat
-            )
-        return latency
+            print('Failed to benchmark {} with {}: {}\nTraceback:\n{}'.format(self, backend, e, format_exc()))
+            return float('NaN')
 
     def bench_eager(self) -> float:
         print('Benchmarking {} with backend {}...'.format(self, 'eager'))
         return self.bench_with_backend('eager')
 
     def bench_inductor(self, mode: str) -> float:
         print('Benchmarking {} with backend {}...'.format(self, 'inductor(mode={})'.format(mode)))
         return self.bench_with_backend('inductor', mode=mode)
 
     def bench_hidet(self, use_cuda_graph=True, use_fp16=False, use_fp16_reduction=False) -> float:
         print('Benchmarking {} with backend {}...'.format(self, 'hidet(space={})'.format(self.search_space)))
         config = hidet.torch.dynamo_config
         config.search_space(self.search_space)
         config.use_cuda_graph(use_cuda_graph)
+        config.use_tensor_core(self.tensor_core)
         config.use_fp16(use_fp16)
         config.use_fp16_reduction(use_fp16_reduction)
         return self.bench_with_backend('hidet')
 
     @staticmethod
     def headers() -> List[str]:
         return [
             'model',
             'inputs',
             'eager',
-            'inductor(mode=reduce-overhead)',
-            # 'inductor(mode=max-autotune)'
-            'hidet(space={})'.format(BenchModel.search_space),
+            'reduce-overhead',
+            'max-autotune',
+            'hidet({})'.format(BenchModel.search_space),
         ]
 
     def benchmark(self) -> List[Any]:
         return [
             str(self),
             self.inputs_str(),
             self.bench_eager(),
             self.bench_inductor('reduce-overhead'),
-            # self.bench_inductor('max-autotune'),
+            self.bench_inductor('max-autotune'),
             self.bench_hidet(),
         ]
 
 
 all_registered_models: List[BenchModel] = []
 commonly_used_models: List[BenchModel] = []
```

## hidet/cli/bench/nlp/models.py

```diff
@@ -54,9 +54,10 @@
 
     bench_models = [
         NLPModel('huggingface/pytorch-transformers', 'model', model, batch_size, seq_length) for model in models
     ]
     header = BenchModel.headers()
     result = [bench_model.benchmark() for bench_model in bench_models]
 
-    click.echo(tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left'))
-    click.echo('(PyTorch backend: allow_tf32={})'.format(BenchModel.allow_tf32))
+    BenchModel.report_table(
+        tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left')
+    )
```

## hidet/cli/bench/nlp/nlp_model.py

```diff
@@ -5,14 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import torch
 from hidet.cli.bench.model import BenchModel
 
 
 class NLPModel(BenchModel):
     def __init__(self, repo_name, model_name, label, batch_size: int, sequence_length: int):
         self.repo_name = repo_name
         self.model_name = model_name
@@ -20,19 +21,26 @@
         self.batch_size = batch_size
         self.sequence_length = sequence_length
 
     def __str__(self):
         return '{}/{}'.format(self.model_name, self.label)
 
     def model(self):
-        import torch
-
         return torch.hub.load(self.repo_name, self.model_name, self.label)
 
     def example_inputs(self):
-        import torch
-
         tokens_tensor = torch.zeros((self.batch_size, self.sequence_length), dtype=torch.long, device='cuda')
         segments_tensors = torch.zeros((self.batch_size, self.sequence_length), dtype=torch.long, device='cuda')
         args = (tokens_tensor,)
         kwargs = {'token_type_ids': segments_tensors}
         return args, kwargs
+
+    def inputs_str(self) -> str:
+        if self.dtype == torch.float16:
+            dtype = 'f16'
+        elif self.dtype == torch.float32:
+            dtype = 'f32'
+        elif self.dtype == torch.float64:
+            dtype = 'f64'
+        else:
+            raise ValueError('Unknown dtype: {}'.format(self.dtype))
+        return f'{dtype}, bs={self.batch_size}, seq={self.sequence_length}'
```

## hidet/cli/bench/vision/inception_v3.py

```diff
@@ -28,9 +28,10 @@
 @click.option('-h', '--height', default=224, show_default=True, help='Input image height')
 @click.option('-w', '--width', default=224, show_default=True, help='Input image width')
 def bench_inception_v3(batch_size: int, channels: int, height: int, width: int):
     bench_models = [VisionModel('inception_v3', batch_size, channels, height, width)]
     header = BenchModel.headers()
     result = [bench_model.benchmark() for bench_model in bench_models]
 
-    click.echo(tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left'))
-    click.echo('(PyTorch backend: allow_tf32={})'.format(BenchModel.allow_tf32))
+    BenchModel.report_table(
+        tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left')
+    )
```

## hidet/cli/bench/vision/mobilenet_v2.py

```diff
@@ -28,9 +28,10 @@
 @click.option('-h', '--height', default=224, show_default=True, help='Input image height')
 @click.option('-w', '--width', default=224, show_default=True, help='Input image width')
 def bench_mobilenet_v2(batch_size: int, channels: int, height: int, width: int):
     bench_models = [VisionModel('mobilenet_v2', batch_size, channels, height, width)]
     header = BenchModel.headers()
     result = [bench_model.benchmark() for bench_model in bench_models]
 
-    click.echo(tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left'))
-    click.echo('(PyTorch backend: allow_tf32={})'.format(BenchModel.allow_tf32))
+    BenchModel.report_table(
+        tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left')
+    )
```

## hidet/cli/bench/vision/resnet.py

```diff
@@ -46,9 +46,10 @@
         if model not in resnet_models:
             raise ValueError('Unknown model: {}, candidates: {}'.format(model, list(resnet_models.keys())))
 
     bench_models = [VisionModel(model_name, batch_size, channels, height, width) for model_name in models]
     header = BenchModel.headers()
     result = [bench_model.benchmark() for bench_model in bench_models]
 
-    click.echo(tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left'))
-    click.echo('(PyTorch backend: allow_tf32={})'.format(BenchModel.allow_tf32))
+    BenchModel.report_table(
+        tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left')
+    )
```

## hidet/cli/bench/vision/resnext.py

```diff
@@ -43,9 +43,10 @@
         if model not in resnext_models:
             raise ValueError('Unknown model: {}, candidates: {}'.format(model, list(resnext_models.keys())))
 
     bench_models = [VisionModel(model_name, batch_size, channels, height, width) for model_name in models]
     header = BenchModel.headers()
     result = [bench_model.benchmark() for bench_model in bench_models]
 
-    click.echo(tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left'))
-    click.echo('(PyTorch backend: allow_tf32={})'.format(BenchModel.allow_tf32))
+    BenchModel.report_table(
+        tabulate(result, headers=header, tablefmt='github', floatfmt='.3f', numalign='right', stralign='left')
+    )
```

## hidet/cuda/device.py

```diff
@@ -162,21 +162,7 @@
 
 def profiler_stop():
     """
     Mark the end of a profiling range.
     """
     (err,) = cudart.cudaProfilerStop()
     assert err == 0, err
-
-
-# We intentionally put the properties of all devices to the cache here.
-#
-# Reasons:
-#   Hidet relies on the multiprocessing to parallelize the compilation. During the process, the forked process will
-#   query the properties of the device. If we do not cache the properties, the forked process will query the device
-#   via the cuda runtime API. However, the cuda runtime API does not work when the multiprocessing package is working
-#   in the fork mode. With the properties of all the GPUs cached, the forked process will not run any cuda runtime API
-#   and will not cause any problem.
-if available():
-    for i in range(device_count()):
-        properties(i)
-        compute_capability(i)
```

## hidet/cuda/stream.py

```diff
@@ -12,15 +12,15 @@
 # pylint: disable=no-name-in-module, c-extension-no-member
 from __future__ import annotations
 from typing import Union, Optional, Dict
 from cuda import cudart
 from cuda.cudart import cudaStream_t
 from hidet.utils import exiting
 from .event import Event
-from .device import CudaDeviceContext, device_count, current_device
+from .device import CudaDeviceContext, current_device
 
 
 def _get_device_id(device) -> int:
     """
     Get the device ID from a device.
 
     Parameters
@@ -164,17 +164,15 @@
         The device ID of the stream. If None, the current device will be used.
     """
 
     def __init__(self, handle: Union[cudaStream_t, int], device_id: Optional[int] = None):
         super().__init__(handle=handle, device=device_id)
 
 
-_current_streams: Dict[int, Stream] = {
-    device_id: ExternalStream(handle=0, device_id=device_id) for device_id in range(device_count())
-}
+_current_streams: Dict[int, Stream] = {}
 
 
 class StreamContext:
     def __init__(self, stream: Stream):  # pylint: disable=redefined-outer-name
         self.device_context = CudaDeviceContext(stream.device_id())
         self.device: int = stream.device_id()
         self.stream: Stream = stream
@@ -208,14 +206,17 @@
         The device on which to get the current stream. If None, the current device will be used.
 
     Returns
     -------
     stream: Stream
         The current stream.
     """
+    device_id = _get_device_id(device)
+    if device_id not in _current_streams:
+        _current_streams[device_id] = ExternalStream(handle=0, device_id=device_id)
     return _current_streams[_get_device_id(device)]
 
 
 def default_stream(device=None) -> Stream:
     """
     Get the default stream.
```

## hidet/ffi/__init__.py

```diff
@@ -7,11 +7,11 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from .ffi import _LIB
 from .packedfunc import PackedFunc
-from .packedfunc import ArgType
+from .packedfunc import ArgTypeCode
 
 from .runtime_api import runtime_api
 from . import callbacks
```

## hidet/ffi/packedfunc.py

```diff
@@ -5,56 +5,61 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 from typing import Sequence, List
 import time
 import ctypes
 from enum import Enum
 
 from ctypes import c_int32, c_void_p, pointer, c_float, cast
 from ctypes import POINTER, Structure
+
+import hidet.graph.frontend.torch
 from hidet.ir.type import TypeNode, DataType, TensorType, PointerType, TensorPointerType
-from hidet.utils.py import same_list
+from hidet.ir.expr import Constant
 from .ffi import _LIB
 
 c_int32_p = POINTER(c_int32)
 c_float_p = POINTER(c_float)
 
 
-class ArgType(Enum):
+class ArgTypeCode(Enum):
     INT32 = 1
     FLOAT32 = 2
     POINTER = 3
     FLOAT16 = 4
 
+    @staticmethod
+    def from_type(type_node: TypeNode) -> ArgTypeCode:
+        if isinstance(type_node, DataType):
+            if type_node.name == 'int32':
+                return ArgTypeCode.INT32
+            elif type_node.name == 'float32':
+                return ArgTypeCode.FLOAT32
+            elif type_node.name == 'float16':
+                return ArgTypeCode.FLOAT16
+            else:
+                raise NotImplementedError('Unsupported scalar type: {}'.format(type_node.name))
+        elif isinstance(type_node, (TensorType, PointerType, TensorPointerType)):
+            return ArgTypeCode.POINTER
+        else:
+            raise NotImplementedError('Unsupported type: {}'.format(type_node))
+
 
 class CPackedFunc(Structure):
     _fields_ = [("num_args", c_int32), ("arg_types", c_int32_p), ("func_pointer", c_void_p)]
 
 
 def make_c_packed_func(param_types: Sequence[TypeNode], c_func_pointer) -> CPackedFunc:
-    type_codes = []
-    for param_type in param_types:
-        if isinstance(param_type, DataType):
-            if param_type.name == 'int32':
-                type_codes.append(ArgType.INT32.value)
-            elif param_type.name == 'float32':
-                type_codes.append(ArgType.FLOAT32.value)
-            elif param_type.name == 'float16':
-                type_codes.append(ArgType.FLOAT16.value)
-            else:
-                raise NotImplementedError('Unsupported scalar type: {}'.format(param_type.name))
-        elif isinstance(param_type, (TensorType, PointerType, TensorPointerType)):
-            type_codes.append(ArgType.POINTER.value)
-        else:
-            raise NotImplementedError('Unsupported type: {}'.format(param_type))
+    type_codes = [ArgTypeCode.from_type(param_type).value for param_type in param_types]
     n = len(type_codes)
     num_args = c_int32(n)
     arg_types = cast(pointer((c_int32 * n)(*type_codes)), POINTER(c_int32))
     func_pointer = cast(c_func_pointer, c_void_p)
     return CPackedFunc(num_args, arg_types, func_pointer)
 
 
@@ -81,14 +86,24 @@
         from hidet.graph import Tensor
 
         if len(args) != len(self.param_types):
             raise ValueError('The callee expects {} arguments, but got {}.'.format(len(self.param_types), len(args)))
 
         converted_args: List[ctypes.c_void_p] = []
         for i, (param_type, arg) in enumerate(zip(self.param_types, args)):
+            if isinstance(arg, Constant):
+                if arg.is_scalar():
+                    arg = arg.value
+                else:
+                    assert arg.is_tensor()
+                    raise NotImplementedError('Constant tensor is not supported.')
+            if not isinstance(arg, Tensor) and arg.__class__.__name__ == 'Tensor':
+                if hidet.graph.frontend.torch.available() and arg.__class__.__name__ == 'Tensor':
+                    arg = hidet.from_torch(arg)
+
             if isinstance(arg, (float, int)):
                 if not isinstance(param_type, DataType):
                     raise ValueError(
                         'The callee expects the {}-th element to be a {}, but got a {}.'.format(
                             i + 1, param_type, type(arg)
                         )
                     )
@@ -99,32 +114,29 @@
                     assert isinstance(arg, float), 'Expect a float, but got a {}.'.format(type(arg))
                     converted_args.append(cast(pointer(c_float(arg)), c_void_p))
                 else:
                     raise NotImplementedError(f"PackedFunc does not support argument type '{param_type.name}'.")
             elif isinstance(arg, Tensor):
                 if isinstance(param_type, TensorType):
                     expect_dtype = param_type.dtype
-                    expect_shape = param_type.const_shape()
                 elif isinstance(param_type, TensorPointerType):
                     expect_dtype = param_type.tensor_type.dtype
-                    expect_shape = param_type.tensor_type.const_shape()
                 elif isinstance(param_type, PointerType):
                     isinstance(param_type.base_type, DataType)
                     expect_dtype = param_type.base_type
-                    expect_shape = None
                 else:
                     raise ValueError(
                         'The callee expects the {}-th element to be a {}, but got a {}.'.format(
                             i + 1, param_type, type(arg)
                         )
                     )
-                if arg.dtype != expect_dtype or (expect_shape is not None and not same_list(arg.shape, expect_shape)):
+                if arg.dtype != expect_dtype:
                     raise ValueError(
-                        'The callee expects the {}-th element to be a {}{}, but got a {}{}.'.format(
-                            i + 1, expect_dtype, expect_shape if expect_shape else " tensor", arg.dtype, arg.shape
+                        'The callee expects the {}-th element to be a {} tensor, but got a {} tensor.'.format(
+                            i + 1, expect_dtype, arg.dtype
                         )
                     )
                 converted_args.append(cast(arg.storage.addr, c_void_p))
             else:
                 raise ValueError(f"Argument type '{type(arg)}' is not supported.")
         return cast((c_void_p * len(converted_args))(*converted_args), c_void_p)
```

## hidet/graph/operator.py

```diff
@@ -7,15 +7,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Dict, Any, Union
 
-from hidet.ir.dtypes import float16, bfloat16, float32
+from hidet.ir.type import TensorType, DataType
+from hidet.ir.expr import Var, Constant, var
+from hidet.ir.compute import TensorNode
+from hidet.ir.dtypes import float16, bfloat16, float32, int32
 from hidet.ir.task import Task
 from hidet.runtime.module import CompiledFunction
 from hidet.graph.tensor import empty, empty_like, Tensor
 from hidet.ffi.ffi import get_last_error, BackendException
 from hidet.runtime.device import Device, instantiate_device
 
 
@@ -28,32 +31,27 @@
     else:
         return cls_name
 
 
 class Operator:
     """An operator that takes tensor as input and output."""
 
-    def __init__(
-        self,
-        inputs: List[Tensor],
-        task: Optional[Task],
-        outputs: Optional[List[Tensor]] = None,
-        name: Optional[str] = None,
-        attributes: Optional[Dict[str, Any]] = None,
-    ):
-        self.inputs: List[Tensor] = inputs
-        self.task: Optional[Task] = task
-        self.attrs: Dict[str, Any] = attributes if attributes is not None else {}
-        self.outputs: Optional[List[Tensor]] = outputs
-        self.name: str = get_operator_name(self, name)
-
+    def __init__(self, inputs: List[Tensor], attributes: Dict[str, Any], task: Optional[Task]):
         assert all(isinstance(v, Tensor) for v in inputs)
 
+        self.name: str = get_operator_name(self)
+        self.inputs: List[Tensor] = inputs
+        self.attrs: Dict[str, Any] = attributes
+        self.task: Optional[Task] = task.specialize_for(self.inputs)
+        self.outputs: List[Tensor] = []
+
         # cache
-        self.task_func: Optional[CompiledFunction] = None
+        self._task_func: Optional[CompiledFunction] = None
+
+        self.outputs = self._run()
 
     def __str__(self):
         arguments = ['{}: {}{}'.format(i, t.dtype.name, t.shape) for i, t in enumerate(self.inputs)]
         attributes = ['{}={}'.format(name, str(value)) for name, value in self.attrs.items()]
         return '{}({})'.format(self.name, ', '.join(arguments + attributes))
 
     @property
@@ -65,113 +63,119 @@
             return instantiate_device(self.attrs['device'])
         else:
             # when the operator has inputs, get the device from the inputs
             if not all(t.device == self.inputs[0].device for t in self.inputs):
                 raise ValueError('All inputs of an operator must be on the same device')
             return self.inputs[0].device
 
-    def run(self) -> List[Tensor]:
+    @property
+    def task_func(self) -> CompiledFunction:
+        if self._task_func is None:
+            self._task_func = self.task.build(target=self.device.type)
+        return self._task_func
+
+    def _run(self) -> List[Tensor]:
+        from hidet.ir.tools import rewrite, simplify
+
         if all(t.storage is not None for t in self.inputs):
             return self.imperative_run(self.inputs)
         else:
-            self.outputs = self.symbolic_run()
-            return self.outputs
+            output_types: List[TensorType] = [output_node.type for output_node in self.task.outputs]
+            outputs: List[Tensor] = []
+            remap: Dict[Var, Constant] = {}
+            for i, (a, b) in enumerate(zip(self.task.inputs, self.inputs)):
+                for d1, d2 in zip(a.type.shape, b.shape):
+                    if isinstance(d2, int) and isinstance(d1, Var):
+                        if d1 in remap:
+                            assert int(remap[d1]) == d2
+                            continue
+                        remap[d1] = int32(d2)
+            for i, output_type in enumerate(output_types):
+                symbol_shape = [simplify(rewrite(d, remap)) for d in output_type.shape]
+                shape = [int(d) if isinstance(d, Constant) else var(f'd{i}') for i, d in enumerate(symbol_shape)]
+                outputs.append(
+                    Tensor(shape=shape, dtype=output_type.dtype.name, device=self.device, storage=None, trace=(self, i))
+                )
+            return outputs
 
     def get_output(self, idx: int) -> Tensor:
         if self.outputs is None:
-            outputs = self.run()
+            outputs = self._run()
         else:
             outputs = self.outputs
         return outputs[idx]
 
     def imperative_run(self, inputs: List[Tensor]) -> List[Tensor]:
-        self.build_task_func()
-        assert len(inputs) + len(self.task.outputs) == len(self.task.parameters)
-        output_types = [output.type for output in self.task.parameters[-len(self.task.outputs) :]]
-        outputs = [
-            empty(shape=type.const_shape(), dtype=type.dtype.name, device=self.device, layout=type.layout)
-            for type in output_types
+        from hidet.ir.tools import rewrite, simplify_to_int
+
+        remap: Dict[Var, Constant] = {}
+        for ta, tb in zip(self.task.inputs, inputs):
+            for d1, d2 in zip(ta.type.shape, tb.shape):
+                if isinstance(d1, Var):
+                    remap[d1] = int32(d2)
+        output_dtypes: List[DataType] = [output.type.dtype for output in self.task.outputs]
+        output_shapes: List[List[int]] = [
+            [simplify_to_int(rewrite(d, remap)) for d in output.type.shape] for output in self.task.outputs
+        ]
+        outputs: List[Tensor] = [
+            empty(shape=shape, dtype=dtype, device=self.device) for shape, dtype in zip(output_shapes, output_dtypes)
         ]
 
-        args = self.task.generate_arguments(inputs, outputs)
+        arg_remap: Dict[Union[Var, TensorNode], Union[Constant, Tensor]] = remap
+        for a, b in zip(self.task.inputs, inputs):
+            arg_remap[a] = b
+        for a, b in zip(self.task.outputs, outputs):
+            arg_remap[a] = b
+
+        args = [arg_remap[param] for param in self.task.params]
         self.task_func(*args)
 
         status = get_last_error()
         if status is not None:
             msg = 'Kernel for operator {} failed. Error:\n{}'.format(self.name, status)
             raise BackendException(msg)
 
         return outputs
 
-    def symbolic_run(self) -> List[Tensor]:
-        output_nodes = self.task.parameters[-len(self.task.outputs) :]
-        output_types = [output_node.type for output_node in output_nodes]
-        outputs = []
-        for i, output_type in enumerate(output_types):
-            outputs.append(
-                Tensor(
-                    shape=output_type.const_shape(),
-                    dtype=output_type.dtype.name,
-                    device=self.device,
-                    storage=None,
-                    layout=output_type.layout,
-                    trace=(self, i),
-                )
-            )
-        return outputs
-
     def reforward(self, inputs: List[Tensor], update_attributes: Optional[Dict[str, Any]] = None) -> List[Tensor]:
         cls = self.__class__
-        if not isinstance(self, Operator) or cls is Operator:
-            raise ValueError('Can only reforward operator whose class is a proper class of Operator. Please use .clone')
         attributes = self.attrs.copy()
         if update_attributes is not None:
             attributes.update(update_attributes)
-        return cls(*inputs, **attributes).run()
+        return cls(*inputs, **attributes).outputs
 
     def clone(self, inputs: List[Tensor], update_attributes: Optional[Dict[str, Any]] = None) -> List[Tensor]:
-        cls = self.__class__
-        attributes = self.attrs.copy()
-        if update_attributes is not None:
-            attributes.update(update_attributes)
-
-        new_op = cls.__new__(cls)
-        new_op.name = self.name
-        new_op.inputs = inputs
-        new_op.task = self.task
-        new_op.attrs = attributes
-        new_op.outputs = new_op.run()
-        new_op.task_func = None
-        return new_op.outputs
+        return self.reforward(inputs, update_attributes)
+        # # todo: remove this method, use rerun instead
+        # cls = self.__class__
+        # attributes = self.attrs.copy()
+        # if update_attributes is not None:
+        #     attributes.update(update_attributes)
+        #
+        # new_op = cls.__new__(cls)
+        # new_op.name = self.name
+        # new_op.inputs = inputs
+        # new_op.task = self.task
+        # new_op.attrs = attributes
+        # new_op.outputs = new_op._run()
+        # new_op._task_func = None    # pylint: disable=protected-access
+        # return new_op.outputs
 
     def dummy_inputs(self) -> List[Tensor]:
         dummy_inputs = []
         for x in self.inputs:
             if x.storage is not None:
                 dummy_inputs.append(x)
             else:
                 if x.dtype in [float16, bfloat16, float32]:
                     dummy_inputs.append(empty_like(x))
                 else:
                     raise ValueError('Can not generate dummy input for dtype {}'.format(x.dtype))
         return dummy_inputs
 
-    def dummy_outputs(self) -> List[Tensor]:
-        output_types = [output.type for output in self.task.parameters[-len(self.task.outputs) :]]
-        dummy_outputs = [
-            empty(shape=type.const_shape(), dtype=type.dtype.name, device=self.device, layout=type.layout)
-            for type in output_types
-        ]
-        return dummy_outputs
-
     def latency(self, warmup=3, number=20, repeat=5, median=True) -> Union[List[float], float]:
         from hidet.testing import benchmark_func
 
         dummy_inputs = self.dummy_inputs()
-        outputs = self.dummy_outputs()
-        self.imperative_run(dummy_inputs)
+        outputs = self.imperative_run(dummy_inputs)
         args = self.task.generate_arguments(dummy_inputs, outputs)
         return benchmark_func(lambda: self.task_func(*args), warmup=warmup, number=number, repeat=repeat, median=median)
-
-    def build_task_func(self):
-        if self.task_func is None:
-            self.task_func = self.task.build(target=self.device.type)
```

## hidet/graph/tensor.py

```diff
@@ -16,21 +16,37 @@
 
 import numpy as np
 
 import hidet.runtime.storage
 import hidet.cuda
 from hidet.ir import dtypes
 from hidet.ir.type import DataType, data_type
+from hidet.ir.expr import Var, Expr, Constant
 from hidet.ir.layout import DataLayout, RowMajorLayout
 from hidet.runtime.storage import Storage
 from hidet.utils import prod
 from hidet.utils.overrides import set_module
 from hidet.runtime.device import Device, instantiate_device
 
 
+def _simplify_dim(dim: Union[int, Expr]) -> Union[int, Var]:
+    from hidet.ir.tools import simplify
+
+    if isinstance(dim, (int, Var)):
+        return dim
+    elif isinstance(dim, Constant):
+        return int(dim)
+    else:
+        dim = simplify(dim)
+        if isinstance(dim, (int, Var, Constant)):
+            return _simplify_dim(dim)
+        else:
+            raise ValueError(f"Cannot simplify {dim} to a constant integer or variable.")
+
+
 @set_module('hidet')
 class Tensor:
     """An n-dimension array, could be symbolic or concrete.
 
     This class defines an n-dimension array.
 
     Parameters
@@ -54,23 +70,23 @@
         Where this tensor is derived from. A trace = (op, i) indicates that this tensor is the i-th output of the op
         operator.
     """
 
     def __init__(self, shape, dtype, device, storage, layout=None, trace=None):
         from hidet.graph.operator import Operator
 
-        self._shape: List[int] = [int(v) for v in shape]
+        self._shape: List[Union[Var, int]] = [_simplify_dim(dim) for dim in shape]
         self._dtype: DataType = data_type(dtype)
         self._device: Device = instantiate_device(device)
         self._storage: Optional[Storage] = storage
         self._layout: DataLayout = layout if layout else DataLayout.row_major(shape)
         self._trace: Optional[Tuple[Operator, int]] = trace
 
     @property
-    def shape(self) -> Tuple[int, ...]:
+    def shape(self) -> Tuple[Union[int, Var], ...]:
         """
         The shape of the tensor.
 
         The shape is a tuple of integers indicating the size of the tensor along each dimension.
 
         Returns
         -------
@@ -265,18 +281,18 @@
         return less_equal(self, utils.convert_to_tensor(other, self))
 
     def __gt__(self, other):
         from .ops import greater, utils
 
         return greater(self, utils.convert_to_tensor(other, self))
 
-    def __eq__(self, other):
-        from .ops import equal, utils
-
-        return equal(self, utils.convert_to_tensor(other, self))
+    # def __eq__(self, other):
+    #     from .ops import equal, utils
+    #
+    #     return equal(self, utils.convert_to_tensor(other, self))
 
     def __ne__(self, other):
         from .ops import not_equal, utils
 
         return not_equal(self, utils.convert_to_tensor(other, self))
 
     def __radd__(self, other):
@@ -931,14 +947,18 @@
         Returns
         -------
         ret: torch.Tensor
             The torch tensor that shares the memory with the hidet tensor.
         """
         import torch
 
+        if self.dtype == dtypes.boolean:
+            # workaround for torch not supporting exporting boolean to dlpack
+            return torch.from_dlpack(self.to(dtype='uint8')).bool()
+
         return torch.from_dlpack(self)
 
 
 def empty(shape, dtype='float32', device='cpu', layout=None):
     """Create an uninitialized tensor.
 
     Parameters
@@ -988,23 +1008,23 @@
     ret: Tensor
         The created tensor.
 
     """
     return Tensor(shape=shape, dtype=dtype, device=device, storage=None, layout=layout)
 
 
-def zeros(shape: Sequence[int], dtype='float32', device='cpu') -> Tensor:
+def zeros(shape: Sequence[int], dtype: Union[DataType, str] = 'float32', device='cpu') -> Tensor:
     """Create a tensor initialized with zero.
 
     Parameters
     ----------
     shape: Sequence[int]
         The shape of new tensor.
 
-    dtype: str
+    dtype: str or DataType
         The data type of element of the tensor.
 
     device: Device or str, default 'cpu'
         The device of the new tensor is created on.
 
     Returns
     -------
@@ -1094,17 +1114,19 @@
     Examples
     --------
     >>> randn([2, 3])
     Tensor(shape=[2, 3], dtype='float32', device='cuda')
     [[ 0.10720467 -1.6906018   0.06347568]
      [-0.37061226  0.562728    1.857547  ]]
     """
+    np_tensor = np.random.randn(*shape) * stddev + mean
+
+    if isinstance(np_tensor, float):  # shape = []
+        np_tensor = np.array(np_tensor)
 
-    np_tensor = np.random.randn(*shape).astype(np.float32)
-    np_tensor = np_tensor * stddev + mean
     hidet_tensor = from_numpy(np_tensor)
     return hidet_tensor.to(device=device, dtype=dtype)
 
 
 def randint(low: int, high=None, shape: Sequence[int] = (), dtype: str = 'int32') -> Tensor:
     dtype_map = {'int32': np.int32, 'int64': np.int64}
     if dtype not in dtype_map:
@@ -1276,24 +1298,35 @@
         fill_value=fill_value,
         dtype=data.dtype if dtype is None else dtype,
         device=data.device if device is None else device,
     )
 
 
 def randn_like(
-    data: Tensor, shape: Optional[Sequence[int]] = None, dtype: Optional[str] = None, device: Optional[str] = None
+    data: Tensor,
+    mean: float = 0.0,
+    stddev: float = 1.0,
+    shape: Optional[Sequence[int]] = None,
+    dtype: Optional[str] = None,
+    device: Optional[str] = None,
 ) -> Tensor:
     """
     Create a randomly initialized tensor with the same shape, dtype, and device as the given tensor.
 
     Parameters
     ----------
     data: Tensor
         The tensor to copy shape, dtype, and device from.
 
+    mean: float, optional
+        The mean of the normal distribution.
+
+    stddev: float, optional
+        The standard deviation of the normal distribution.
+
     shape: Sequence[int], optional
         The shape of new tensor. If None, the shape of data is used.
 
     dtype: DataType or str, optional
         The data type of element of the tensor. If None, the dtype of data is used.
 
     device: Device or str, optional
@@ -1304,14 +1337,16 @@
     ret: Tensor
         The created tensor with random values sampled from a normal distribution.
     """
     return randn(
         shape=data.shape if shape is None else shape,
         dtype=data.dtype if dtype is None else dtype,
         device=data.device if device is None else device,
+        mean=mean,
+        stddev=stddev,
     )
 
 
 def from_numpy(nparray: np.ndarray) -> Tensor:
     """
     Create a tensor from a numpy array, sharing the memory with the numpy array when possible.
```

## hidet/graph/frontend/torch/dynamo_backends.py

```diff
@@ -13,47 +13,55 @@
 from typing import List, Callable, Sequence, Union
 import logging
 import torch
 import hidet.option
 from hidet.ir.type import data_type
 from hidet.graph.ir.flow_graph import FlowGraph
 from hidet.graph.transforms import PassContext, optimize
-from .utils import serialize_output, deserialize_output
+from .utils import serialize_output, deserialize_output, resolve_save_dir_multigraph
 from .dynamo_config import dynamo_config
 
 
 logger = logging.getLogger(__name__)
 
 
 def generate_executor(flow_graph: FlowGraph) -> Callable:
     from hidet.cuda.graph import CudaGraph
 
     use_fp16 = dynamo_config['use_fp16']
     use_fp16_reduction = dynamo_config['use_fp16_reduction']
     use_cuda_graph = dynamo_config['use_cuda_graph']
+    use_attention = dynamo_config['use_attention']
     search_space = dynamo_config['search_space']
     parallel_k = dynamo_config['parallel_k']
+    tensor_core = dynamo_config['use_tensor_core']
+    save_dir = dynamo_config['dump_graph_ir']
 
     with PassContext() as ctx:
         if use_fp16:
             ctx.set_precision('float16')
         if use_fp16 and use_fp16_reduction:
             ctx.set_reduce_precision('float16')
+        ctx.set_use_attention(use_attention)
+        if save_dir:
+            graph_dir = resolve_save_dir_multigraph(save_dir)
+            ctx.save_graph_instrument(graph_dir)
+        if tensor_core:
+            ctx.set_mma('mma' if tensor_core else 'simt')
         ctx.set_parallel_k(disabled=(parallel_k == 'disabled'), search=(parallel_k == 'search'))
         logger.info('start to optimize the flow graph')
         graph_opt: FlowGraph = optimize(flow_graph)
         logger.info('finish optimizing the flow graph')
 
     logger.info('schedule search space: %d', search_space)
 
     has_cpu_tensor = any(tensor.device.type == 'cpu' for tensor in graph_opt.inputs + graph_opt.outputs)
-    has_cuda_tensor = any(tensor.device.type == 'cuda' for tensor in graph_opt.inputs + graph_opt.outputs)
-
-    if has_cpu_tensor and has_cuda_tensor:
-        raise RuntimeError('the flow graph contains both CPU and CUDA tensors, currently not supported by hidet')
+    # has_cuda_tensor = any(tensor.device.type == 'cuda' for tensor in graph_opt.inputs + graph_opt.outputs)
+    # if has_cpu_tensor and has_cuda_tensor:
+    #     raise RuntimeError('the flow graph contains both CPU and CUDA tensors, currently not supported by hidet')
 
     def preprocess_inputs(inputs: Sequence[torch.Tensor]) -> List[hidet.Tensor]:
         torch_inputs: List[torch.Tensor] = []
         for x in inputs:
             if not x.is_contiguous():
                 logger.warning('Hidet received a non-contiguous torch input tensor, converting it to contiguous')
                 x = x.contiguous()
```

## hidet/graph/frontend/torch/dynamo_config.py

```diff
@@ -14,24 +14,40 @@
 
 class DynamoConfig:
     def __init__(self):
         self._search_space: int = 0
         self._parallel_k: str = 'default'
         self._use_fp16: bool = False
         self._use_fp16_reduction: bool = False
+        self._use_attention: bool = False
         self._use_cuda_graph: bool = True
-        self._use_tensor_core: bool = True
+        self._use_tensor_core: bool = False
         self._print_input_graph: bool = False
         self._dump_graph_ir: Optional[str] = None
         self._correctness_report: bool = False
 
     def __getitem__(self, item: str):
         assert isinstance(item, str)
         return getattr(self, f"_{item}")
 
+    def reset(self):
+        """
+        Reset the configuration to the default values
+        """
+        self._search_space: int = 0
+        self._parallel_k: str = 'default'
+        self._use_fp16: bool = False
+        self._use_fp16_reduction: bool = False
+        self._use_attention: bool = False
+        self._use_cuda_graph: bool = True
+        self._use_tensor_core: bool = False
+        self._print_input_graph: bool = False
+        self._dump_graph_ir: Optional[str] = None
+        self._correctness_report: bool = False
+
     def search_space(self, level: int = 2):
         """
         The schedule search space for the operator kernel tuning
         Candidates are: ``0``, ``1``, ``2``
 
         - ``0``:
             Use the default schedule, without tuning.
@@ -85,14 +101,21 @@
     def use_fp16_reduction(self, flag=True):
         """
         Whether to use float16 data type for reduction
         """
         self._use_fp16_reduction = flag
         return self
 
+    def use_attention(self, flag=False):
+        """
+        Whether to use fused attention schedule
+        """
+        self._use_attention = flag
+        return self
+
     def use_cuda_graph(self, flag=True):
         """
         Whether to use cuda graph
         """
         self._use_cuda_graph = flag
         return self
```

## hidet/graph/frontend/torch/register_functions.py

```diff
@@ -84,24 +84,37 @@
 def linear(x: Tensor, weight: Tensor, bias: Optional[Tensor]):
     y = ops.matmul(x, weight)
     if bias is not None:
         y = y + bias
     return y
 
 
+@register_function(torch.nn.functional.bilinear)
+def bilinear(x_1: Tensor, x_2: Tensor, weight: Tensor, bias: Optional[Tensor]):
+    y = ops.matmul(x_1, ops.matmul(weight, x_2))
+    if bias is not None:
+        y = y + bias
+    return y
+
+
 @register_function(operator.add)
 def add(x: Tensor, y: Tensor):
     return ops.add(x, y)
 
 
 @register_function(operator.iadd)
 def iadd(x: Tensor, y: Tensor):
     return ops.add(x, y)
 
 
+@register_function(operator.neg)
+def neg(x: Tensor):
+    return -x
+
+
 @register_function(torch.sin)
 def sin(x: Tensor):
     return ops.sin(x)
 
 
 @register_function(torch.cos)
 def cos(x: Tensor):
@@ -179,14 +192,75 @@
         raise NotImplementedError("count_include_pad=False")
     if divisor_override is not None:
         raise NotImplementedError("divisor_override is not None")
     y = ops.avg_pool3d(x, kernel_size, stride, padding)
     return y
 
 
+@register_function(torch.nn.functional.interpolate)
+def interpolate(
+    input: Tensor,
+    size=None,
+    scale_factor=None,
+    mode='nearest',
+    align_corners=None,
+    recompute_scale_factor=None,
+    antialias=False,
+):
+    if len(input.shape) != 4:
+        raise NotImplementedError("Currently only supports 4D inputs (NCHW)")
+
+    if antialias:
+        raise NotImplementedError("Currently does not support antialias=True")
+
+    if recompute_scale_factor:
+        raise NotImplementedError("Currently does not support recompute_scale_factor=True")
+
+    if size is None == scale_factor is None:
+        raise ValueError("Exactly one of size or scale_factor can be None")
+
+    target_size = None
+    if size is not None:
+        if isinstance(size, int):
+            target_size = [size, size]
+        else:
+            if len(size) != 2:
+                raise ValueError("Length of \"size\" must be of type int or tuple([int, int])")
+            target_size = list(size)
+    else:
+        if isinstance(scale_factor, (int, float)):
+            target_size = [int(i * scale_factor) for i in input.shape[2:]]
+        else:
+            if len(scale_factor) != 2:
+                raise ValueError("Length of \"scale_factor\" must be of type int or tuple([int, int])")
+            target_size = [a * b for a, b in zip(input.shape[2:], scale_factor)]
+
+    supported_methods = {'nearest': 'nearest', 'bilinear': 'linear', 'bicubic': 'cubic'}
+    if mode not in supported_methods:
+        raise NotImplementedError("Mode not supported")
+
+    mode_hidet = supported_methods[mode]
+    if align_corners:
+        coordinate_transformation_mode = 'align_corners'
+    else:
+        coordinate_transformation_mode = 'pytorch_half_pixel'
+
+    return ops.resize2d(
+        input,
+        target_size,
+        mode_hidet,
+        coordinate_transformation_mode,
+        rounding_method='round_prefer_floor',
+        roi=None,
+        cubic_alpha=-0.75,
+        cubic_exclude=0,
+        extrapolation_value=0.0,
+    )
+
+
 @register_function(operator.truediv)
 def truediv(x: Union[Tensor, int, float], y: Union[Tensor, int, float]):
     import hidet
 
     def is_integer(v: Union[Tensor, int, float]) -> bool:
         return isinstance(v, int) or (isinstance(v, Tensor) and v.dtype.is_integer())
 
@@ -200,25 +274,47 @@
 
 @register_function(operator.sub)
 def sub(x: Tensor, y: Tensor):
     return x - y
 
 
 @register_function(torch.nn.functional.softmax)
-def softmax(x: Tensor, dim: int, dtype=None):
+@register_method(torch.Tensor.softmax)
+def softmax(x: Tensor, dim: int, _stacklevel: int = 3, dtype=None):
     if dtype is not None:
         raise NotImplementedError("dtype is not None")
     return ops.softmax(x, dim)
 
 
 @register_function(torch.matmul)
 def matmul(x: Tensor, y: Tensor):
     return ops.matmul(x, y)
 
 
+@register_function(torch.zeros)
+def zeros(*size, out=None, dtype=None, layout=None, device=None, pin_memory=False, requires_grad=False):
+    import hidet
+
+    if out is not None:
+        raise NotImplementedError("out is not None")
+    if layout is not None:
+        raise NotImplementedError("layout is not None")
+    if len(size) == 1:
+        if isinstance(size[0], (list, tuple)):
+            size = size[0]
+    shape = [int(v) for v in size]
+    if dtype is None:
+        dtype = torch.get_default_dtype()
+
+    _ = pin_memory
+    _ = requires_grad
+
+    return hidet.zeros(shape, dtype=dtype_from_torch(dtype), device=device_from_torch(device))
+
+
 @register_function(torch.ones)
 def ones(
     *size: Union[int, Sequence[int]],
     out: Optional[Tensor] = None,
     dtype: Optional[torch.dtype] = None,
     layout: Optional[torch.layout] = None,
     device: Optional[Union[torch.device, str, None]] = None,
@@ -269,14 +365,38 @@
     if weight is not None:
         y = y * weight
     if bias is not None:
         y = y + bias
     return y
 
 
+@register_function(torch.nn.functional.group_norm)
+def group_norm(
+    x: Tensor,
+    num_groups: int,
+    num_channels: int,
+    weight: Optional[Tensor] = None,
+    bias: Optional[Tensor] = None,
+    eps: float = 1e-5,
+):
+    if x.shape[1] != num_channels:
+        raise ValueError(
+            "num_channels does not match tensor shape at index 2, expect {} but got {}".format(num_channels, x.shape[2])
+        )
+    if num_channels % num_groups != 0:
+        raise ValueError("num_channels {} must be divisible by num_groups {}".format(num_channels, num_groups))
+
+    y = ops.group_norm(x, num_groups, epsilon=eps)
+    if weight is not None:
+        y = y * weight.reshape([num_channels, 1, 1])
+    if bias is not None:
+        y = y + bias.reshape([num_channels, 1, 1])
+    return y
+
+
 @register_function(torch.tanh)
 def tanh(x: Tensor):
     return ops.tanh(x)
 
 
 @register_function(torch.nn.functional.embedding)
 def embedding(
@@ -405,21 +525,77 @@
     if requires_grad and torch.is_grad_enabled():
         warnings.warn_once("hidet: requires_grad=True when torch.is_grad_enabled(), treating as requires_grad=False")
     hidet_device: Device = device_from_torch(torch_device=device)
     hidet_dtype: DataType = dtype_from_torch(torch_dtype=dtype)
     return ops.full(size, fill_value, dtype=hidet_dtype, device=hidet_device)
 
 
+@register_function(torch.empty)
+def empty(
+    *size,
+    out=None,
+    dtype=None,
+    layout=torch.strided,
+    device=None,
+    requires_grad=False,
+    pin_memory=False,
+    memory_format=torch.contiguous_format,
+):
+    import hidet
+
+    if out is not None:
+        raise NotImplementedError("hidet: does not support torch.empty(..., out=..., ...)")
+    if layout not in [None, torch.strided]:
+        raise NotImplementedError("hidet: does not support torch.empty(..., layout=..., ...)")
+    if requires_grad and torch.is_grad_enabled():
+        warnings.warn_once("hidet: requires_grad=True when torch.is_grad_enabled(), treating as requires_grad=False")
+    if pin_memory:
+        raise NotImplementedError("hidet: does not support torch.empty(..., pin_memory=True, ...)")
+    if memory_format != torch.contiguous_format:
+        raise NotImplementedError("hidet: does not support torch.empty(..., memory_format=..., ...)")
+
+    hidet_device: Device = device_from_torch(torch_device=device)
+    hidet_dtype: DataType = dtype_from_torch(torch_dtype=dtype)
+    if len(size) == 1 and isinstance(size[0], (tuple, list)):
+        size = size[0]
+    return hidet.empty(size, dtype=hidet_dtype, device=hidet_device)
+
+
 @register_function(torch.bmm)
 def bmm(input: Tensor, mat2: Tensor, *, out: Optional[Tensor] = None) -> Tensor:
     if out is not None:
         raise NotImplementedError("hidet: does not support torch.bmm(..., out=...)")
     return ops.matmul(input, mat2)
 
 
+@register_function(torch.baddbmm)
+def baddbmm(input, batch1, batch2, *, beta=1, alpha=1, out: Optional[Tensor] = None) -> Tensor:
+    import hidet
+
+    if out is not None:
+        raise NotImplementedError("hidet: does not support torch.baddbmm(..., out=...)")
+
+    if alpha == 0 and beta == 0:
+        size = batch1.shape[0:2] + [batch2.shape[-1]]
+        return hidet.zeros(shape=size, dtype=input.dtype, device=input.device)
+    elif alpha == 0:
+        return beta * input
+    elif beta == 0:
+        return alpha * ops.matmul(batch1, batch2)
+
+    if alpha == 1 and beta == 1:
+        return input + ops.matmul(batch1, batch2)
+    elif alpha == 1:
+        return beta * input + ops.matmul(batch1, batch2)
+    elif beta == 1:
+        return input + alpha * ops.matmul(batch1, batch2)
+
+    return beta * input + alpha * ops.matmul(batch1, batch2)
+
+
 @register_function(torch.tensor)
 def torch_tensor(
     data: Any, dtype: Optional[torch.dtype] = None, device: Optional[torch.device] = None, requires_grad: bool = False
 ) -> Tensor:
     if requires_grad and torch.is_grad_enabled():
         warnings.warn_once("hidet: requires_grad=True when torch.is_grad_enabled(), treating as requires_grad=False")
     if isinstance(data, Tensor):
@@ -433,14 +609,21 @@
 @register_function(torch.sigmoid)
 def sigmoid(x: Tensor, *, out: Optional[Tensor] = None) -> Tensor:
     if out is not None:
         warnings.warn_once("hidet: does not support torch.sigmoid(..., out=...)")
     return ops.sigmoid(x)
 
 
+@register_function(torch.exp)
+def exp(x: Tensor, *, out: Optional[Tensor] = None) -> Tensor:
+    if out is not None:
+        warnings.warn_once("hidet: does not support torch.exp(..., out=...)")
+    return ops.exp(x)
+
+
 @register_function(torch.nn.functional.hardsigmoid)
 def hardsigmoid(x: Tensor, inplace: bool):
     if inplace:
         warnings.warn_once('hidet: hardsigmoid with inplace=True is not supported. Treat as inplace=False.')
     return ops.hardsigmoid(x)
 
 
@@ -452,7 +635,56 @@
 
 
 @register_function(torch.nn.functional.hardswish)
 def hardswish(x: Tensor, inplace: bool):
     if inplace:
         warnings.warn_once('hidet: hardswish with inplace=True is not supported. Treat as inplace=False.')
     return ops.hardswish(x)
+
+
+@register_function(torch.nn.functional.softmin)
+def softmin(x: Tensor, axis: int):
+    return ops.softmin(x, axis)
+
+
+@register_function(torch.nn.functional.softplus)
+def softplus(x: Tensor, beta: int, threshold: int):
+    return ops.softplus(x, beta, threshold)
+
+
+@register_function(torch.nn.functional.softshrink)
+def softshrink(x: Tensor, lambda_val: float):
+    return ops.softshrink(x, lambda_val)
+
+
+@register_function(torch.nn.functional.tanhshrink)
+def tanhshrink(x: Tensor):
+    return ops.tanhshrink(x)
+
+
+@register_function(torch.nn.functional.hardshrink)
+def hardshrink(x: Tensor, lambda_val: float):
+    return ops.hardshrink(x, lambda_val)
+
+
+@register_function(torch.nn.functional.softsign)
+def softsign(x: Tensor):
+    return ops.softsign(x)
+
+
+@register_function(torch.nn.functional.celu)
+def celu(x: Tensor, alpha: float):
+    return ops.celu(x, alpha)
+
+
+@register_function(torch.nn.functional.logsigmoid)
+def logsigmoid(x: Tensor):
+    return ops.logsigmoid(x)
+
+
+@register_function(torch.gather)
+def gather(x: Tensor, dim: int, index: Tensor, *, sparse_grad=False, out=None):
+    if sparse_grad:
+        warnings.warn_once('hidet: gather with sparse_grad=True is not supported. Treat as sparse_grad=False.')
+    if out is not None:
+        raise NotImplementedError('hidet: gather with out=... is not supported')
+    return ops.gather(x, index, axis=dim)
```

## hidet/graph/frontend/torch/register_methods.py

```diff
@@ -6,14 +6,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
+import math
 from typing import List, Union
 import torch
 from hidet.ir.type import DataType
 from hidet.graph.tensor import Tensor
 from hidet.graph import ops
 from .interpreter import register_method
 from .utils import dtype_from_torch, device_from_torch, dtype_to_torch
@@ -29,14 +30,29 @@
 @register_method(torch.Tensor.cpu)
 def tensor_cpu(self: Tensor) -> Tensor:
     if self.is_symbolic():
         raise NotImplementedError('hidet: torch.Tensor.cpu() is not supported for symbolic tensors.')
     return self.cpu()
 
 
+@register_method(torch.Tensor.float)
+def tensor_float(self: Tensor) -> Tensor:
+    return ops.cast(self, "float32")
+
+
+@register_method(torch.Tensor.half)
+def tensor_half(self: Tensor) -> Tensor:
+    return ops.cast(self, "float16")
+
+
+@register_method(torch.Tensor.bool)
+def tensor_bool(self: Tensor) -> Tensor:
+    return ops.cast(self, "bool")
+
+
 @register_method(torch.Tensor.to)
 def tensor_to(self: Tensor, *args, **kwargs) -> Tensor:
     """
     There are three argument format for torch.Tensor.to:
 
     1. to(self, dtype, non_blocking=False, copy=False, memory_format=torch.preserve_format)
     2. to(self, device=None, dtype=None, non_blocking=False, copy=False, memory_format=torch.preserve_format)
@@ -128,14 +144,25 @@
     else:
         assert isinstance(split_size, (list, tuple))
         parts = [int(v) for v in split_size]
         assert sum(parts) == self.shape[dim]
     return ops.split(self, axis=dim, parts=parts)
 
 
+@register_method(torch.Tensor.chunk)
+def tensor_chunk(self: Tensor, chunks, dim=0) -> List[Tensor]:
+    dim_size = self.shape[dim]
+    chunk_size = math.ceil(dim_size / chunks)
+    parts = []
+    for start in range(0, dim_size, chunk_size):
+        parts.append(min(chunk_size, dim_size - start))
+    assert sum(parts) == self.shape[dim]
+    return ops.split(self, axis=dim, parts=parts)
+
+
 @register_method(torch.Tensor.squeeze)
 def tensor_squeeze(self: Tensor, dim=None) -> Tensor:
     if dim is None:
         dims = [i for i, s in enumerate(self.shape) if s == 1]
         return ops.squeeze(self, dims)
     else:
         dim = int(dim)
```

## hidet/graph/frontend/torch/register_modules.py

```diff
@@ -96,15 +96,15 @@
         super().__init__(torch_module)
         from hidet import ops
 
         self.transposed_weight = ops.transpose(self.param('weight'), [1, 0])
 
     def __call__(self, x: Tensor) -> Tensor:
         assert isinstance(self.mod, torch.nn.Linear)
-        return regs.linear(x=x, weight=self.transposed_weight, bias=self.param('bias'))
+        return regs.linear(x=x, weight=self.transposed_weight, bias=self.param('bias', optional=True))
 
 
 @register_module(torch.nn.BatchNorm2d)
 class HidetBatchNorm2d(HidetModule):
     def __call__(self, x: Tensor) -> Tensor:
         assert isinstance(self.mod, torch.nn.BatchNorm2d)
         return regs.batch_norm(
@@ -138,14 +138,28 @@
             normalized_shape=self.mod.normalized_shape,
             weight=self.param('weight'),
             bias=self.param('bias'),
             eps=self.mod.eps,
         )
 
 
+@register_module(torch.nn.GroupNorm)
+class HidetGroupNorm(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.GroupNorm)
+        return regs.group_norm(
+            x=x,
+            num_groups=self.mod.num_groups,
+            num_channels=self.mod.num_channels,
+            weight=self.param('weight'),
+            bias=self.param('bias'),
+            eps=self.mod.eps,
+        )
+
+
 @register_module(torch.nn.Tanh)
 class HidetTanh(HidetModule):
     def __call__(self, x: Tensor) -> Tensor:
         assert isinstance(self.mod, torch.nn.Tanh)
         return regs.tanh(x)
 
 
@@ -222,7 +236,70 @@
 
 
 @register_module(torch.nn.SiLU)
 class HidetSiLU(HidetModule):
     def __call__(self, x: Tensor) -> Tensor:
         assert isinstance(self.mod, torch.nn.SiLU)
         return regs.silu(x, self.mod.inplace)
+
+
+@register_module(torch.nn.Softmax)
+class HidetSoftmax(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.Softmax)
+        return regs.softmax(x, self.mod.dim)
+
+
+@register_module(torch.nn.Softmin)
+class HidetSoftmin(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.Softmin)
+        return regs.softmin(x, self.mod.dim)
+
+
+@register_module(torch.nn.Softplus)
+class HidetSoftplus(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.Softplus)
+        return regs.softplus(x, self.mod.beta, self.mod.threshold)
+
+
+@register_module(torch.nn.Softsign)
+class HidetSoftsign(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.Softsign)
+        return regs.softsign(x)
+
+
+@register_module(torch.nn.Softshrink)
+class HidetSoftshrink(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.Softshrink)
+        return regs.softshrink(x, self.mod.lambd)
+
+
+@register_module(torch.nn.Tanhshrink)
+class HidetTanhshrink(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.Tanhshrink)
+        return regs.tanhshrink(x)
+
+
+@register_module(torch.nn.Hardshrink)
+class HidetHardshrink(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.Hardshrink)
+        return regs.hardshrink(x, self.mod.lambd)
+
+
+@register_module(torch.nn.CELU)
+class HidetCELU(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.CELU)
+        return regs.celu(x, self.mod.alpha)
+
+
+@register_module(torch.nn.LogSigmoid)
+class HidetLogSigmoid(HidetModule):
+    def __call__(self, x: Tensor) -> Tensor:
+        assert isinstance(self.mod, torch.nn.LogSigmoid)
+        return regs.logsigmoid(x)
```

## hidet/graph/frontend/torch/utils.py

```diff
@@ -6,14 +6,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Tuple, Any, List, Union, Dict, Optional
+from pathlib import Path
 from hidet.graph.tensor import Tensor
 from hidet.ir.type import DataType
 from hidet.ir import dtypes
 from hidet.runtime.device import Device
 from .availability import available
 
 
@@ -241,7 +242,15 @@
         The relative error
     """
     import torch
 
     actual: torch.Tensor = actual.detach()
     expected: torch.Tensor = expected.detach()
     return float(torch.max(torch.abs(actual - expected) / (torch.abs(expected) + 1.0)))
+
+
+def resolve_save_dir_multigraph(save_dir: str) -> str:
+    func = resolve_save_dir_multigraph
+    if not hasattr(func, 'counter'):
+        func.counter = {}
+    func.counter[save_dir] = func.counter.get(save_dir, 0) + 1
+    return str(Path(save_dir) / "graph_{}".format(func.counter[save_dir]))
```

## hidet/graph/ir/flow_graph.py

```diff
@@ -94,43 +94,44 @@
 def forward_context() -> GraphForwardContext:
     return GraphForwardContext()
 
 
 class FlowGraph:
     """The computation graph representation."""
 
-    def __init__(self, outputs: List[Tensor], inputs=None, nodes=None):
-        self.outputs: List[Tensor] = outputs
-        self.inputs: Optional[List[Tensor]] = inputs
-        self.nodes: Optional[List[Operator]] = nodes
-        self.usage_count: Optional[Dict[Tensor, int]] = None
+    def __init__(self, outputs: Sequence[Tensor], inputs: Optional[Sequence[Tensor]] = None, nodes=None):
+        self.outputs: List[Tensor] = list(outputs)
+        self.inputs: Optional[List[Tensor]] = list(inputs) if inputs is not None else None
+        self._nodes: Optional[List[Operator]] = nodes
+        self._usage_count: Optional[Dict[Tensor, int]] = None
+        self.update_nodes()
 
     def __call__(self, *inputs: Tensor) -> Union[List[Tensor], Tensor]:
         """Run the computation graph.
         See Also :func:`FlowGraph.forward`.
         """
         return self.forward(*inputs)
 
     def __str__(self):
-        if any(v is None for v in [self.inputs, self.nodes, self.usage_count]):
-            self.update_nodes()
         namer = Namer()
 
         def get_tensor_sig(x: Tensor) -> Doc:
             return Text(x.dtype.name) + '[' + doc_join([str(v) for v in x.shape], ', ') + ']'
 
-        def get_attr_repr(value: Union[float, int, bool, str, list, tuple]) -> Doc:
+        def get_attr_repr(value: Union[float, int, bool, str, list, tuple, FlowGraph]) -> Doc:
             if isinstance(value, (float, int, bool)):
                 return Text(str(value))
             elif isinstance(value, str):
                 return Text('"{}"'.format(value))
             elif isinstance(value, list):
                 return '[' + doc_join([get_attr_repr(v) for v in value], ', ') + ']'
             elif isinstance(value, tuple):
                 return '(' + doc_join([get_attr_repr(v) for v in value], ', ') + ')'
+            elif isinstance(value, FlowGraph):
+                return Text('FlowGraph({})'.format(', '.join(u.name for u in value.nodes)))
             else:
                 return Text(str(value))
 
         param_docs = []
         for x in self.inputs:
             name = namer(x)
             param_docs.append(Text(name) + ': ' + get_tensor_sig(x))
@@ -149,41 +150,62 @@
                     const_doc += NewLine() + namer.get_name(x, hint='c') + ' = Constant(' + get_tensor_sig(x) + ')'
             outputs = op.outputs
             if len(outputs) > 1:
                 raise NotImplementedError()
             output: Tensor = outputs[0]
             line_doc = Doc()
             line_doc += namer(output) + ': ' + get_tensor_sig(output) + ' = '
-            line_doc += op.name + ('*' if len(op.task.task_graph.nodes) > 1 else '') + '('
+            line_doc += op.name + '('
             line_doc += doc_join([namer(x) for x in op.inputs], sep=', ')
             if op.attrs:
                 line_doc += ', ' + doc_join(
                     [Text(name) + '=' + get_attr_repr(value) for name, value in op.attrs.items()], ', '
                 )
             line_doc += ')  '
             body_doc += NewLine() + line_doc
 
         # return statement
         body_doc += NewLine() + Text('return ') + doc_join([namer(x) for x in self.outputs], ', ')
 
         graph_doc = head_doc + '{' + const_doc.indent() + body_doc.indent() + NewLine() + '}'
         return str(graph_doc)
 
+    @property
+    def nodes(self) -> List[Operator]:
+        """The list of operators in the computation graph."""
+        if self._nodes is None:
+            self.update_nodes()
+        return self._nodes
+
+    @property
+    def usage_count(self) -> Dict[Tensor, int]:
+        """The usage count of each tensor in the computation graph."""
+        if self._usage_count is None:
+            self.update_nodes()
+        return self._usage_count.copy()
+
+    def invalid_cache(self):
+        self._nodes = None
+        self._usage_count = None
+
     def build(self):
         tasks = []
         tunable_tasks = []
         task_keys = set()
         search_space = hidet.option.get_option('search_space')
         for node in self.nodes:
             if node.task_func is None:
                 task_key = hash(str(node.task))
                 if task_key in task_keys:
                     continue
                 task_keys.add(task_key)
-                if search_space == 0 or 'implement_cuda' not in node.task.__class__.__dict__:
+                if search_space == 0 or all(
+                    method not in node.task.__class__.__dict__
+                    for method in ['implement_cuda', 'implement_cpu', 'implement']
+                ):
                     tasks.append(node.task)
                 else:
                     tunable_tasks.append(node.task)
 
         hidet.driver.build_task_batch(tasks)
 
         with option.context():
@@ -207,16 +229,14 @@
         """
         inputs: List[Tensor] = list(inputs)
 
         for idx, tensor in enumerate(inputs):
             if tensor.storage is None:
                 msg = 'Expect non-symbolic input tensors, got symbolic input {} ({}).'.format(idx, tensor.signature())
                 raise ValueError(msg)
-        if any(v is None for v in [self.inputs, self.nodes, self.usage_count]):
-            self.update_nodes()
         self.build()
 
         GraphForwardContext.current()._trigger_before_graph(self, inputs)
 
         usage_count = self.usage_count.copy()
         tensor_map: Dict[Tensor, Tensor] = {}
         for st, at in zip(self.inputs, inputs):
@@ -280,15 +300,15 @@
         ----------
         model_file: str
             The model file to store the flow graph.
         """
         # before save, clear the packed func cache because ctypes object can not be pickled
         for node in self.nodes:
             node.task_func = None
-        self.usage_count, self.nodes = None, None
+        self._usage_count, self._nodes = None, None
 
         dirname = os.path.dirname(model_file)
         os.makedirs(dirname, exist_ok=True)
         # save to a temporary file first, in case pickle fails.
         with open(model_file + '.temp', 'wb') as f:
             pickle.dump(self, f)
         os.rename(model_file + '.temp', model_file)
@@ -307,19 +327,18 @@
         ret: FlowGraph
             The loaded flow graph.
         """
         with open(model_file, 'rb') as f:
             ret = pickle.load(f)
         if not isinstance(ret, FlowGraph):
             raise TypeError('Expect to load FlowGraph, got {}'.format(type(ret)))
-        ret.update_nodes()
         return ret
 
     def update_nodes(self):
-        free_vars, self.nodes, self.usage_count = self._analyze(self.outputs)
+        free_vars, self._nodes, self._usage_count = self._analyze(self.outputs)
         if self.inputs:
             non_bound_free_vars: Set[Tensor] = set(free_vars) - set(self.inputs)
             if len(non_bound_free_vars) > 0:
                 msg = ['There is free variable(s) not given in inputs:']
                 for v in non_bound_free_vars:
                     msg.append('  {}'.format(v.signature()))
                 raise ValueError('\n'.join(msg))
@@ -457,14 +476,16 @@
             nodes.append(op)
             for it in op.inputs:
                 if it.op is None:
                     if it.storage is None and all(it is not v for v in free_vars):
                         # input
                         free_vars.append(it)
                 else:
+                    if it is not it.op.outputs[it.trace[1]]:
+                        raise ValueError('The trace is broken')
                     out_degree[it.op] -= 1
                     if out_degree[it.op] == 0:
                         stack.append(it.op)
         nodes = list(reversed(nodes))
         assert len(nodes) == len(all_nodes), 'all_nodes {} topo_order {}'.format(len(all_nodes), len(nodes))
 
         # tensor usage count
```

## hidet/graph/ir/flow_graph_impl.py

```diff
@@ -13,15 +13,15 @@
 import os
 import numpy as np
 from hidet.runtime import CompiledFunction
 from .flow_graph import FlowGraph, Operator, Tensor, GraphForwardInstrument
 
 
 class GraphForwardDebugInstrument(GraphForwardInstrument):
-    _template = '{:>5} {:>25} {:>3}   {:<25} {:>8} {:>8} {:>8} {:>10} {:>10} {:>10} {:>10}'
+    _template = '{:>5} {:>30} {:>3}   {:<25} {:>8} {:>8} {:>8} {:>10} {:>10} {:>10} {:>10}'
 
     def __init__(self, output_dir='./outs/debug', print_summary=False):
         self.output_dir: str = output_dir
         self.print_summary: bool = print_summary
 
         self.debugging: bool = False
         self.run_dir: Optional[str] = None
@@ -58,15 +58,15 @@
             netron.dump(graph, f)
 
         with open(self.summary_file, 'w') as f:
             head = self._template.format(
                 'Index', 'Operator', 'Arg', 'Shape', 'NaN', 'Inf', 'Zero', 'Min', 'Max', 'Mean', 'Std'
             )
             top_sep = '-' * len(head)
-            bot_sep = self._template.format(*['-' * extent for extent in [5, 25, 3, 25, 8, 8, 8, 10, 10, 10, 10]])
+            bot_sep = self._template.format(*['-' * extent for extent in [5, 30, 3, 25, 8, 8, 8, 10, 10, 10, 10]])
             f.write(''.join([top_sep, '\n', head, '\n', bot_sep, '\n']))
 
     @staticmethod
     def tensor_stats(array: np.ndarray) -> Dict[str, str]:
         double_array = array.astype(np.float64)
         return {
             'nan': '{:8d}'.format(np.count_nonzero(np.isnan(array))),
@@ -80,15 +80,15 @@
 
     def before_operator(self, op: Operator, inputs: List[Tensor]) -> None:
         if not self.debugging:
             return
 
         lines = []
         for idx, tensor in enumerate(inputs):
-            array: np.ndarray = tensor.numpy(share_mem=False)
+            array: np.ndarray = tensor.cpu().numpy()
             stats = self.tensor_stats(array)
             if idx == 0:
                 op_idx = str(self.operator_idx)
                 op_name = op.name
             else:
                 op_idx = op_name = ''
             line = self._template.format(
@@ -111,15 +111,15 @@
     def after_operator(self, op: Operator, inputs: List[Tensor], outputs: List[Tensor]) -> None:
         if not self.debugging:
             return
 
         lines = []
         found_abnormal = False
         for idx, tensor in enumerate(outputs):
-            array: np.ndarray = tensor.numpy(share_mem=False)
+            array: np.ndarray = tensor.cpu().numpy()
             stats = self.tensor_stats(array)
             op_idx = op_name = ''
             line = self._template.format(
                 op_idx,
                 op_name,
                 'y{}'.format(idx),
                 '{}{}'.format(tensor.dtype.short_name, list(tensor.shape)),
@@ -134,15 +134,15 @@
             lines.append(line)
             found_abnormal = found_abnormal or int(stats['nan']) > 0 or int(stats['inf']) > 0
 
         with open(self.summary_file, 'a') as f:
             f.write('\n'.join(lines) + '\n')
 
         if found_abnormal:
-            arrays = [tensor.numpy(share_mem=False) for tensor in inputs + outputs]
+            arrays = [tensor.cpu().numpy() for tensor in inputs + outputs]
             names = ['x{}'.format(idx) for idx in range(len(inputs))] + [
                 'y{}'.format(idx) for idx in range(len(outputs))
             ]
             np.savez(os.path.join(self.run_dir, 'abnormal_in_outs.npz'), **dict(zip(names, arrays)))
             with open(os.path.join(self.run_dir, '{}.txt'.format(op.name)), 'w') as f:
                 f.write('Operator:\n{}\n'.format(op))
                 f.write('Task:\n{}\n'.format(op.task))
@@ -198,16 +198,14 @@
         self.latency_list = []
         os.makedirs(self.run_dir, exist_ok=True)
 
     def after_operator(self, op: Operator, inputs: List[Tensor], outputs: List[Tensor]) -> None:
         if not self.benchmarking:
             return
 
-        if op.task_func is None:
-            op.build_task_func()
         task_func: CompiledFunction = op.task_func
         latency: List[float] = task_func.profile(
             *inputs, *outputs, warmup=self.warmup, number=self.number, repeat=self.repeat
         )
         self.latency_list.append((op, float(np.median(latency)), float(np.std(latency))))
 
     def after_graph(self, graph: FlowGraph, inputs: List[Tensor], outputs: List[Tensor]) -> None:
```

## hidet/graph/ops/__init__.py

```diff
@@ -14,31 +14,33 @@
 
 from .definitions.conv2d import conv2d, conv2d_winograd, conv2d_gemm, conv2d_gemm_image_transform
 from .definitions.conv2d_transpose import conv2d_transpose, conv2d_transpose_gemm
 from .definitions.conv3d import conv3d, conv3d_gemm
 from .definitions.matmul import batch_matmul, matmul
 from .definitions.pool import avg_pool2d, avg_pool3d, adaptive_avg_pool1d, adaptive_avg_pool2d, adaptive_avg_pool3d
 from .definitions.pool import max_pool2d, max_pool3d, adaptive_max_pool1d, adaptive_max_pool2d, adaptive_max_pool3d
-from .definitions.softmax import softmax
 from .definitions.activation import relu, leaky_relu, sigmoid, hardsigmoid, clip, relu6, prelu, gelu, silu, hardswish
-from .definitions.norm import batch_norm_infer, instance_norm, layer_norm
+from .definitions.activation import logsigmoid, celu, hardshrink, softplus, softsign, tanhshrink
+from .definitions.activation import softshrink, softmax, softmin, hardtanh
+from .definitions.norm import batch_norm_infer, instance_norm, layer_norm, group_norm
 from .definitions.image import resize2d
 from .definitions.create import full, arange, linspace
 from .definitions.arithmetic import add, subtract, multiply, divide, mod, remainder, negative, positive, square
 from .definitions.arithmetic import floor, ceil, round, trunc, sqrt, rsqrt, pow, abs
 from .definitions.arithmetic import reciprocal, exp, expm1, log, log2, log10, log1p, logaddexp, erf
 from .definitions.arithmetic import bitwise_right_shift, bitwise_left_shift, bitwise_and, bitwise_invert, bitwise_or
 from .definitions.arithmetic import bitwise_xor, maximum, minimum
 from .definitions.arithmetic import isfinite, isinf, isnan, sign, where
 from .definitions.arithmetic import sin, cos, tan, sinh, cosh, tanh, asin, acos, atan, asinh, acosh, atanh, atan2
 from .definitions.compare import equal, not_equal, less, greater, less_equal, greater_equal
 from .definitions.compare import logical_not, logical_and, logical_or, logical_xor
 from .definitions.reduce import mean, sum, var, min, max, std, prod, argmin, argmax, all, any
 from .definitions.cumulative import cumsum
 from .definitions.transform import squeeze, unsqueeze, flatten, concat, cast, take, rearrange, strided_slice, reshape
-from .definitions.transform import transpose, broadcast, pad, tile, split, conv_pad, expand_dims
+from .definitions.transform import transpose, broadcast, pad, tile, split, conv_pad, expand_dims, gather
 from .definitions.transform import permute_dims
+from .definitions.fusion import fused_operator
 from .definitions.special import barrier
 
 from .definitions import utils
 
 from . import schedules
```

## hidet/graph/ops/definitions/__init__.py

```diff
@@ -7,49 +7,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # pylint: disable=redefined-builtin
 from .create import full
-from .arithmetic import (
-    add,
-    subtract,
-    multiply,
-    divide,
-    negative,
-    sqrt,
-    rsqrt,
-    where,
-    maximum,
-    minimum,
-    reciprocal,
-    exp,
-    log,
-    abs,
-)
-from .arithmetic import (
-    bitwise_and,
-    bitwise_invert,
-    bitwise_or,
-    bitwise_xor,
-    ceil,
-    bitwise_right_shift,
-    bitwise_left_shift,
-)
+from .arithmetic import add, subtract, multiply, divide, negative, sqrt, rsqrt, where, maximum, minimum, reciprocal
+from .arithmetic import bitwise_and, bitwise_invert, bitwise_or, bitwise_xor, bitwise_right_shift, bitwise_left_shift
+from .arithmetic import ceil, exp, log, abs
 from .compare import equal, less, greater, less_equal, greater_equal, logical_not, logical_and
 from .transform import squeeze, unsqueeze, flatten, concat, cast, take, rearrange, strided_slice, split, pad, conv_pad
 from .pool import avg_pool2d, adaptive_avg_pool1d, adaptive_avg_pool2d, adaptive_avg_pool3d
 from .pool import max_pool2d, adaptive_max_pool1d, adaptive_max_pool2d, adaptive_max_pool3d
-from .softmax import softmax
-from .activation import relu, sigmoid, relu6, clip, prelu
+from .activation import relu, leaky_relu, sigmoid, hardsigmoid, clip, relu6, prelu, gelu, silu, hardswish
+from .activation import logsigmoid, celu, hardshrink, softplus, softsign, tanhshrink, softshrink
+from .activation import softmax, softmin, hardtanh
 from .norm import batch_norm_infer, instance_norm
 from .image import resize2d
 from .cumulative import cumsum
 from .special import barrier
+from .attention import attention
 from .conv2d import conv2d
 from .conv2d_transpose import conv2d_transpose
 from .matmul import batch_matmul, matmul
 
 from .matmul import BatchMatmulOp, MatmulOp
 from .conv2d import Conv2dOp
 from .arithmetic import ErfOp, PowOp, AddOp, SubtractOp, MultiplyOp, DivideOp, WhereOp
```

## hidet/graph/ops/definitions/activation.py

```diff
@@ -8,17 +8,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 import math
 from hidet.ir import primitives as prim
-from hidet.ir.expr import if_then_else
-from .utils import Tensor
+from hidet.ir.expr import if_then_else, BitwiseAnd
+from .utils import Tensor, Operator, normalize_dim, input_like
 from .arithmetic import UnaryElementwiseOp, BinaryElementwiseOp
+from .softmax import SoftmaxTask
 
 
 class ReluOp(UnaryElementwiseOp):
     def __init__(self, x: Tensor):
         super().__init__(x, op=lambda v: prim.max(v, x.dtype.zero), name='relu')
 
 
@@ -83,14 +84,114 @@
             op=lambda v: if_then_else(
                 v <= x.dtype(-3), x.dtype.zero, if_then_else(v >= x.dtype(3), v, (v * (v + x.dtype(3))) / x.dtype(6))
             ),
             name='hardswish',
         )
 
 
+class ThresholdOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor, threshold_val: float, value: float) -> Tensor:
+        super().__init__(x, op=lambda v: if_then_else(v > x.dtype(threshold_val), v, x.dtype(value)), name='threshold')
+
+
+class HardTanhOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor, min_val: float = -1.0, max_val: float = 1.0) -> Tensor:
+        super().__init__(x, op=lambda v: prim.min(x.dtype(max_val), prim.max(x.dtype(min_val), v)), name='hardtanh')
+
+
+class EluOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor, alpha: float = 1.0) -> Tensor:
+        super().__init__(
+            x, op=lambda v: if_then_else(v > 0, v, x.dtype(alpha) * (prim.exp(v) - x.dtype(1.0))), name='elu'
+        )
+
+
+class SeluOp(UnaryElementwiseOp):
+    def __init__(
+        self,
+        x: Tensor,
+        alpha: float = 1.6732632423543772848170429916717,
+        scale: float = 1.0507009873554804934193349852946,
+    ) -> Tensor:
+        super().__init__(
+            x,
+            op=lambda v: x.dtype(scale)
+            * (prim.max(x.dtype(0.0), v) + prim.min(x.dtype(0.0), x.dtype(alpha) * (prim.exp(v) - x.dtype(-1.0)))),
+            name='selu',
+        )
+
+
+class CeluOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor, alpha: float = 1.0) -> Tensor:
+        super().__init__(
+            x,
+            op=lambda v: prim.max(x.dtype(0.0), v)
+            + prim.min(x.dtype(0.0), x.dtype(alpha) * (prim.exp(v / x.dtype(alpha)) - x.dtype(1.0))),
+            name='celu',
+        )
+
+
+class LogSigmoidOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor):
+        super().__init__(x, op=lambda v: -(prim.log(x.dtype(1.0) + prim.exp(-v))), name='logsigmoid')
+
+
+class HardShrinkOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor, lambda_val: float = 0.5):
+        super().__init__(
+            x,
+            op=lambda v: if_then_else(BitwiseAnd(v >= x.dtype(-lambda_val), v <= x.dtype(lambda_val)), x.dtype(0), v),
+            name='hardshrink',
+        )
+
+
+class TanhShrinkOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor):
+        super().__init__(
+            x, op=lambda v: v - (prim.exp(v) - prim.exp(-v)) / (prim.exp(v) + prim.exp(-v)), name='tanhshrink'
+        )
+
+
+class SoftSignOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor):
+        super().__init__(x, op=lambda v: v / (x.dtype(1.0) + prim.abs(v)), name='softsign')
+
+
+class SoftPlusOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor, beta: int = 1, threshold_val: int = 20):
+        super().__init__(
+            x,
+            op=lambda v: if_then_else(
+                v * x.dtype(beta) <= x.dtype(threshold_val),
+                (x.dtype(1.0 / beta)) * prim.log(x.dtype(1.0) + prim.exp(x.dtype(beta) * v)),
+                v,
+            ),
+            name='softplus',
+        )
+
+
+class SoftShrinkOp(UnaryElementwiseOp):
+    def __init__(self, x: Tensor, lambda_val: float = 0.5):
+        super().__init__(
+            x,
+            op=lambda v: if_then_else(
+                v > x.dtype(lambda_val),
+                v - x.dtype(lambda_val),
+                if_then_else(v < x.dtype(-lambda_val), v + x.dtype(lambda_val), x.dtype(0.0)),
+            ),
+            name='softshrink',
+        )
+
+
+class SoftmaxOp(Operator):
+    def __init__(self, x: Tensor, axis: int = 1):
+        axis = normalize_dim(axis, len(x.shape))
+        super().__init__(inputs=[x], attributes={'axis': axis}, task=SoftmaxTask(input_like(x, 'x'), axis))
+
+
 def relu(x) -> Tensor:
     return ReluOp(x).get_output(0)
 
 
 def leaky_relu(x: Tensor, alpha: float) -> Tensor:
     return LeakyReluOp(x, alpha).get_output(0)
 
@@ -121,7 +222,59 @@
 
 def prelu(x: Tensor, slope: Tensor) -> Tensor:
     return PReluOp(x, slope).get_output(0)
 
 
 def hardswish(x: Tensor) -> Tensor:
     return HardSwishOp(x).get_output(0)
+
+
+def threshold(x: Tensor, threshold_val: float, value: float) -> Tensor:
+    return ThresholdOp(x, threshold_val, value).get_output(0)
+
+
+def hardtanh(x: Tensor, min_val: float, max_val: float) -> Tensor:
+    return HardTanhOp(x, min_val, max_val).get_output(0)
+
+
+def elu(x: Tensor, alpha: float) -> Tensor:
+    return EluOp(x, alpha).get_output(0)
+
+
+def selu(x: Tensor, alpha: float, scale: float) -> Tensor:
+    return SeluOp(x, alpha, scale).get_output(0)
+
+
+def celu(x: Tensor, alpha: float) -> Tensor:
+    return CeluOp(x, alpha).get_output(0)
+
+
+def logsigmoid(x: Tensor) -> Tensor:
+    return LogSigmoidOp(x).get_output(0)
+
+
+def hardshrink(x: Tensor, lambda_val: float) -> Tensor:
+    return HardShrinkOp(x, lambda_val).get_output(0)
+
+
+def tanhshrink(x: Tensor) -> Tensor:
+    return TanhShrinkOp(x).get_output(0)
+
+
+def softsign(x: Tensor) -> Tensor:
+    return SoftSignOp(x).get_output(0)
+
+
+def softplus(x: Tensor, beta: int, threshold_val: int) -> Tensor:
+    return SoftPlusOp(x, beta, threshold_val).get_output(0)
+
+
+def softshrink(x: Tensor, lambda_val: float) -> Tensor:
+    return SoftShrinkOp(x, lambda_val).get_output(0)
+
+
+def softmax(x: Tensor, axis=1) -> Tensor:
+    return SoftmaxOp(x, axis).get_output(0)
+
+
+def softmin(x: Tensor, axis: int) -> Tensor:
+    return SoftmaxOp(-x, axis).get_output(0)
```

## hidet/graph/ops/definitions/arithmetic.py

```diff
@@ -108,20 +108,26 @@
                 if prod(v_shape) == prod(z_shape)
             },
         )
 
 
 class UnaryElementwiseOp(Operator):
     def __init__(self, x: Tensor, op, name: str, attributes: Optional[Dict[str, Any]] = None):
-        super().__init__(inputs=[x], task=UnaryElementwiseTask(name, input_like(x, 'x'), op=op), attributes=attributes)
+        if attributes is None:
+            attributes = {}
+        super().__init__(inputs=[x], attributes=attributes, task=UnaryElementwiseTask(name, input_like(x, 'x'), op=op))
 
 
 class BinaryElementwiseOp(Operator):
     def __init__(self, x: Tensor, y: Tensor, op, name: str):
-        super().__init__(inputs=[x, y], task=BinaryElementwiseTask(name, input_like(x, 'x'), input_like(y, 'y'), op=op))
+        super().__init__(
+            inputs=[x, y],
+            attributes={},
+            task=BinaryElementwiseTask(name, input_like(x, 'x'), input_like(y, 'y'), op=op),
+        )
 
 
 def resolve_dtype(tensor_dtype: DataType, scalar_dtype: DataType) -> DataType:
     if tensor_dtype.is_integer() and scalar_dtype.is_float():
         return scalar_dtype
     else:
         return tensor_dtype
@@ -404,54 +410,54 @@
         super().__init__(x, y, op=lambda a, b: primitives.mod(a, b), name='mod')
 
 
 class WhereOp(Operator):
     def __init__(self, cond: Tensor, x: Tensor, y: Tensor):
         super().__init__(
             inputs=[cond, x, y],
+            attributes={},
             task=WhereTask(input_like(cond, 'cond'), input_like(x, 'x'), input_like(y, 'y')),
-            name='where',
         )
 
 
 class MaxOp(Operator):
     def __init__(self, *tensors: Tensor):
         def scalar_max(args: List[expr.Expr]):
             if len(args) == 1:
                 return args[0]
             else:
                 return primitives.max(args[0], scalar_max(args[1:]))
 
         super().__init__(
             inputs=list(tensors),
+            attributes={},
             task=VariadicElementwiseTask(
                 name='max',
                 args=[input_like(x, f'x{idx}') for idx, x in enumerate(tensors)],
                 op=lambda *args: scalar_max(args),
             ),
-            name='max',
         )
 
 
 class MinOp(Operator):
     def __init__(self, *tensors: Tensor):
         def scalar_min(args: List[expr.Expr]):
             if len(args) == 1:
                 return args[0]
             else:
                 return primitives.min(args[0], scalar_min(args[1:]))
 
         super().__init__(
             inputs=list(tensors),
+            attributes={},
             task=VariadicElementwiseTask(
                 name='min',
                 args=[input_like(x, f'x{idx}') for idx, x in enumerate(tensors)],
                 op=lambda *args: scalar_min(args),
             ),
-            name='min',
         )
 
 
 def binary_arithmetic(
     x: Union[Tensor, Constant, float, int],
     y: Union[Tensor, Constant, float, int],
     tensor_scalar_op: Callable[[Tensor, Constant], Tensor],
```

## hidet/graph/ops/definitions/create.py

```diff
@@ -73,18 +73,17 @@
         )
 
 
 class LinSpaceOp(Operator):
     def __init__(self, start, stop, num, *, dtype: DataType, device, endpoint=True):
         device = instantiate_device(device)
         super().__init__(
-            name='linspace',
             inputs=[],
-            task=LinSpaceTask(start, stop, num, endpoint, dtype),
             attributes={'dtype': dtype, 'device': device},
+            task=LinSpaceTask(start, stop, num, endpoint, dtype),
         )
 
 
 class ArangeOp(Operator):
     def __init__(self, start, stop, step, dtype, device):
         if stop is None:
             stop = start
@@ -92,18 +91,17 @@
         if dtype is None:
             if all(isinstance(v, int) for v in [start, stop, step]):
                 dtype = dtypes.int32
             else:
                 dtype = dtypes.float32
         device = instantiate_device(device)
         super().__init__(
-            name='arange',
             inputs=[],
-            task=ArangeTask(start, stop, step, dtype),
             attributes={'start': start, 'stop': stop, 'step': step, 'dtype': dtype, 'device': device},
+            task=ArangeTask(start, stop, step, dtype),
         )
 
 
 class FullOp(Operator):
     def __init__(
         self,
         shape: Sequence[int],
@@ -123,18 +121,17 @@
             elif isinstance(value, Constant):
                 assert isinstance(value.type, DataType)
                 dtype = value.type
             else:
                 raise ValueError(f'Unknown type for value {value}')
 
         super().__init__(
-            name='constant',
             inputs=[],
-            task=FullTask(shape=shape, value=value, dtype=dtype),
             attributes={'shape': shape, 'value': value, 'dtype': dtype, 'device': device},
+            task=FullTask(shape=shape, value=value, dtype=dtype),
         )
 
 
 def full(
     shape: Sequence[int],
     value: Union[float, int, bool, Constant],
     dtype: Optional[Union[DataType, str]] = None,
```

## hidet/graph/ops/definitions/cumulative.py

 * *Ordering differences only*

```diff
@@ -53,16 +53,16 @@
 class CumulativeBaseOp(Operator):
     def __init__(self, x: Tensor, dim: int, exclusive: bool, reverse: bool, reduce_type: str):
         if reduce_type not in ['sum']:
             raise NotImplementedError(f'Current do not support cumulative operator for {reduce_type} reduction.')
         dim = normalize_dim(dim, rank=len(x.shape))
         super().__init__(
             inputs=[x],
-            task=CumulativeTask(input_like(x, 'x'), dim, reduce_type, exclusive, reverse),
             attributes={'dim': dim, 'exclusive': exclusive, 'reverse': reverse},
+            task=CumulativeTask(input_like(x, 'x'), dim, reduce_type, exclusive, reverse),
         )
 
 
 class CumulativeSumOp(CumulativeBaseOp):
     def __init__(self, x: Tensor, dim: int, exclusive: bool, reverse: bool):
         super().__init__(x, dim, exclusive, reverse, 'sum')
```

## hidet/graph/ops/definitions/image.py

 * *Ordering differences only*

```diff
@@ -216,35 +216,35 @@
                 )
             )
         if len(size) != 2:
             raise ValueError('Resize2d expect size has 2 elements (height, width), got {}'.format(size))
 
         super().__init__(
             inputs=[data],
+            attributes={
+                'size': size,
+                'method': method,
+                'coordinate_transformation_mode': coordinate_transformation_mode,
+                'rounding_method': rounding_method,
+                'roi': roi,
+                'cubic_alpha': cubic_alpha,
+                'cubic_exclude': cubic_exclude,
+                'extrapolation_value': extrapolation_value,
+            },
             task=Resize2dTask(
                 input_like(data, 'data'),
                 size,
                 method,
                 coordinate_transformation_mode,
                 rounding_method,
                 roi,
                 cubic_alpha,
                 cubic_exclude,
                 extrapolation_value,
             ),
-            attributes={
-                'size': size,
-                'method': method,
-                'coordinate_transformation_mode': coordinate_transformation_mode,
-                'rounding_method': rounding_method,
-                'roi': roi,
-                'cubic_alpha': cubic_alpha,
-                'cubic_exclude': cubic_exclude,
-                'extrapolation_value': extrapolation_value,
-            },
         )
 
 
 def resize2d(
     data: Tensor,
     size: List[int],
     method: str,
```

## hidet/graph/ops/definitions/norm.py

```diff
@@ -69,7 +69,42 @@
     Returns
     -------
     ret: Tensor
         The normalized tensor.
     """
     dims = list(range(len(x.shape) - num_last_dims, len(x.shape)))
     return normalize(x, dims=dims, epsilon=epsilon)
+
+
+def group_norm(x: Tensor, num_groups, epsilon: float = 1e-5):
+    """
+    Group norm.
+
+    Parameters
+    ----------
+    x: Tensor
+        The data to be normalized.
+    num_groups: int
+        The number of groups
+    epsilon: float
+        The epsilon added to variance.
+
+    Returns
+    -------
+    ret: Tensor
+        The normalized tensor.
+    """
+    # first split out the group dimension
+    x_shape = list(x.shape)
+    new_shape = x_shape[:]
+    grouped_rank = 1
+    grouped_dim = new_shape[grouped_rank]
+    assert grouped_dim % num_groups == 0
+
+    new_shape[grouped_rank] = int(grouped_dim // num_groups)
+    new_shape.insert(grouped_rank, num_groups)
+
+    x = x.reshape(new_shape)
+    dims = list(range(2, len(x.shape)))
+    normed = normalize(x, dims=dims, epsilon=epsilon)
+
+    return normed.reshape(x_shape)
```

## hidet/graph/ops/definitions/pool.py

 * *Ordering differences only*

```diff
@@ -143,77 +143,77 @@
         x: Tensor,
         kernel: Union[int, Sequence[int]],
         stride: Union[int, Sequence[int]],
         padding: Union[int, Sequence[int]],
     ):
         super().__init__(
             inputs=[x],
-            task=Pool2dTask(input_like(x, 'x'), kernel, stride, padding, reduce_type='max'),
             attributes={'kernel': kernel, 'stride': stride, 'padding': padding},
+            task=Pool2dTask(input_like(x, 'x'), kernel, stride, padding, reduce_type='max'),
         )
 
 
 class MaxPool3dOp(Operator):
     def __init__(
         self,
         x: Tensor,
         kernel: Union[int, Sequence[int]],
         stride: Union[int, Sequence[int]],
         padding: Union[int, Sequence[int]],
     ):
         super().__init__(
             inputs=[x],
-            task=Pool3dTask(input_like(x, 'x'), kernel, stride, padding, reduce_type='max'),
             attributes={'kernel': kernel, 'stride': stride, 'padding': padding},
+            task=Pool3dTask(input_like(x, 'x'), kernel, stride, padding, reduce_type='max'),
         )
 
 
 class AvgPool2dOp(Operator):
     def __init__(
         self,
         x: Tensor,
         kernel: Union[int, Sequence[int]],
         stride: Union[int, Sequence[int]],
         padding: Union[int, Sequence[int]],
     ):
         super().__init__(
             inputs=[x],
-            task=Pool2dTask(input_like(x, 'x'), kernel, stride, padding, reduce_type='avg'),
             attributes={'kernel': kernel, 'stride': stride, 'padding': padding},
+            task=Pool2dTask(input_like(x, 'x'), kernel, stride, padding, reduce_type='avg'),
         )
 
 
 class AvgPool3dOp(Operator):
     def __init__(
         self,
         x: Tensor,
         kernel: Union[int, Sequence[int]],
         stride: Union[int, Sequence[int]],
         padding: Union[int, Sequence[int]],
     ):
         super().__init__(
             inputs=[x],
-            task=Pool3dTask(input_like(x, 'x'), kernel, stride, padding, reduce_type='avg'),
             attributes={'kernel': kernel, 'stride': stride, 'padding': padding},
+            task=Pool3dTask(input_like(x, 'x'), kernel, stride, padding, reduce_type='avg'),
         )
 
 
 class AdaptivePoolOp(Operator):
     def __init__(self, x: Tensor, output_size, reduce_type: str, attrs: Dict[str, Any], spatial_ndim: int):
         if len(x.shape) != spatial_ndim + 2:
             raise ValueError(
                 'Adaptive{}Pool{}d expects {}D input, got {}D one.'.format(
                     reduce_type.capitalize(), spatial_ndim, spatial_ndim + 2, len(x.shape)
                 )
             )
         output_size = normalize_output(output_size, spatial_ndim)
         super().__init__(
             inputs=[x],
-            task=AdaptivePoolTask(input_like(x, 'x'), output_size, reduce_type=reduce_type),
             attributes=attrs,
+            task=AdaptivePoolTask(input_like(x, 'x'), output_size, reduce_type=reduce_type),
         )
 
 
 class AdaptiveAvgPool1dOp(AdaptivePoolOp):
     def __init__(self, x: Tensor, output_size: Union[int, Sequence[int]]):
         super().__init__(x, output_size, reduce_type='avg', attrs={'output_size': output_size}, spatial_ndim=1)
```

## hidet/graph/ops/definitions/softmax.py

```diff
@@ -7,15 +7,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from hidet.ir.func import IRModule
 from hidet.ir import primitives as prim
-from .utils import Task, Operator, Tensor, TensorNode, compute, input_like, normalize_dim, reduce
+from .utils import Task, TensorNode, compute, reduce
 
 
 class SoftmaxTask(Task):
     def __init__(self, x: TensorNode, axis: int):
         self.x_shape = x.const_shape()
         self.axis = axis
 
@@ -54,21 +54,11 @@
         out = compute(
             name='out',
             shape=shape,
             fcompute=lambda *indices: exp_value[indices] / sum_value[indices[:axis] + indices[axis + 1 :]],
         )
         super().__init__(name='softmax', inputs=[x], outputs=[out])
 
-    def implement_cuda(self, workding_dir: str) -> IRModule:
+    def implement_cuda(self, working_dir: str) -> IRModule:
         from hidet.graph.ops.schedules import softmax_cuda_schedule
 
         return softmax_cuda_schedule(self)
-
-
-class SoftmaxOp(Operator):
-    def __init__(self, x: Tensor, axis: int = 1):
-        axis = normalize_dim(axis, len(x.shape))
-        super().__init__(inputs=[x], task=SoftmaxTask(input_like(x, 'x'), axis), attributes={'axis': axis})
-
-
-def softmax(x: Tensor, axis=1) -> Tensor:
-    return SoftmaxOp(x, axis).get_output(0)
```

## hidet/graph/ops/definitions/special.py

```diff
@@ -19,15 +19,15 @@
     def __init__(self, x: TensorNode):
         y = compute(name='y', shape=x.const_shape(), fcompute=lambda *indices: x[indices])
         super().__init__(name='barrier', inputs=[x], outputs=[y])
 
 
 class BarrierOp(Operator):
     def __init__(self, x: Tensor):
-        super().__init__(inputs=[x], task=BarrierTask(input_like(x, 'x')))
+        super().__init__(inputs=[x], attributes={}, task=BarrierTask(input_like(x, 'x')))
 
 
 def barrier(x: Tensor) -> Tensor:
     """
     Barrier operator is an identity operator and return the same tensor as input. During
     graph-level optimizations, this operator prevents the fusion of producer and consumer
     of the input tensor and output tensor, respectively. This operator will be eliminated
```

## hidet/graph/ops/definitions/transform.py

```diff
@@ -12,29 +12,30 @@
 from typing import List, Optional, Union, Sequence
 from hidet.ir.type import DataType, data_type
 from hidet.ir.expr import LogicalAnd, if_then_else, convert
 from hidet.ir.layout import RowMajorLayout, ColumnMajorLayout
 from hidet.ir.utils import index_deserialize, index_serialize
 from hidet.utils import prod
 from .utils import Task, InverseMap, Operator, Tensor, TensorNode, compute, input_like, normalize_dim, can_broadcast
+from .utils import TensorInput
 
 
 def same_shape(shape_a: Sequence[int], shape_b: Sequence[int]) -> bool:
     return len(shape_a) == len(shape_b) and all(a == b for a, b in zip(shape_a, shape_b))
 
 
 class ReshapeTask(Task):
     def __init__(self, x: TensorNode, y_shape: List[int]):
         x_shape = x.const_shape()
         if prod(x_shape) != prod(y_shape):
             raise ValueError(
                 'Can not reshape {} to {} because they have different number '
                 'of elements: {} vs {}'.format(x_shape, y_shape, prod(x_shape), prod(y_shape))
             )
-        if not isinstance(x.ttype.layout, RowMajorLayout):
+        if not isinstance(x.type.layout, RowMajorLayout):
             raise NotImplementedError(
                 'currently, only support row major layout. Please use '
                 '.contiguous() to transfer the given tensor into row major layout first.'
             )
 
         def index_map(dst_indices, src_shape, dst_shape):
             src_groups = []
@@ -183,14 +184,30 @@
             data_indices = output_indices[:axis] + (index_value,) + output_indices[axis + len(indices_shape) :]
             return data[data_indices]
 
         output = compute(name='output', shape=output_shape, fcompute=lambda *output_indices: fmap(*output_indices))
         super().__init__(name='take', inputs=[data, indices], outputs=[output])
 
 
+class GatherTask(Task):
+    def __init__(self, data: TensorInput, indices: TensorInput, axis=0):
+        data_shape = data.const_shape()
+        indices_shape = indices.const_shape()
+        output_shape = data_shape[:axis] + [indices_shape[axis]] + data_shape[axis + 1 :]
+
+        def fmap(*output_indices):
+            index_value = indices[output_indices]
+            index_value = if_then_else(index_value < 0, index_value + data_shape[axis], index_value)
+            data_indices = output_indices[:axis] + (index_value,) + output_indices[axis + 1 :]
+            return data[data_indices]
+
+        output = compute(name='output', shape=output_shape, fcompute=lambda *output_indices: fmap(*output_indices))
+        super().__init__(name='gather', inputs=[data, indices], outputs=[output])
+
+
 class StridedSliceTask(Task):
     def __init__(
         self,
         data: TensorNode,
         starts: List[Optional[int]],
         ends: List[Optional[int]],
         axes: List[int],
@@ -281,15 +298,15 @@
         super().__init__(name='tile', inputs=[data], outputs=[out])
 
 
 class ReshapeOp(Operator):
     def __init__(self, x: Tensor, shape):
         shape = self.normalize_shape(x.shape, shape)
         task = ReshapeTask(input_like(x, 'x'), shape)
-        super().__init__(inputs=[x], task=task, attributes={'shape': shape})
+        super().__init__(inputs=[x], attributes={'shape': shape}, task=task)
 
     @staticmethod
     def normalize_shape(origin_shape: Sequence[int], shape: Sequence[int]):
         # [1, 3, 224, 224], [1, -1, 224, 0] => [1, 3, 224, 224]
         shape = list(shape)
         for i in range(len(shape)):
             if shape[i] == 0:
@@ -325,23 +342,23 @@
             return [Tensor(shape=shape, dtype=x.dtype, device=x.device, storage=x.storage, layout=layout, trace=None)]
         else:
             return Operator.imperative_run(self, inputs)
 
 
 class RearrangeOp(Operator):
     def __init__(self, x: Tensor, plan: List[List[int]]):
-        super().__init__(inputs=[x], task=RearrangeTask(input_like(x, 'x'), plan=plan), attributes={'plan': plan})
+        super().__init__(inputs=[x], attributes={'plan': plan}, task=RearrangeTask(input_like(x, 'x'), plan=plan))
 
 
 class SqueezeOp(Operator):
     def __init__(self, x: Tensor, dims: List[int]):
         super().__init__(
             inputs=[x],
-            task=RearrangeTask(input_like(x, 'x'), plan=[[i] for i in range(len(x.shape)) if i not in dims]),
             attributes={'dims': dims},
+            task=RearrangeTask(input_like(x, 'x'), plan=[[i] for i in range(len(x.shape)) if i not in dims]),
         )
 
     def imperative_run(self, inputs: Optional[List[Tensor]] = None) -> List[Tensor]:
         x = inputs[0] if inputs else self.inputs[0]
         if isinstance(x.layout, (RowMajorLayout, ColumnMajorLayout)):
             shape = self.task.outputs[0].const_shape()
             layout = x.layout.__class__(shape)
@@ -358,15 +375,15 @@
         for i in range(len(x.shape) + len(dims)):
             if i in dims:
                 plan.append([])
             else:
                 plan.append([c])
                 c += 1
         assert c == len(x.shape)
-        super().__init__(inputs=[x], task=RearrangeTask(input_like(x, 'x'), plan=plan), attributes={'dims': dims})
+        super().__init__(inputs=[x], attributes={'dims': dims}, task=RearrangeTask(input_like(x, 'x'), plan=plan))
 
     def imperative_run(self, inputs: Optional[List[Tensor]] = None) -> List[Tensor]:
         x = inputs[0] if inputs else self.inputs[0]
         if isinstance(x.layout, (RowMajorLayout, ColumnMajorLayout)):
             shape = self.task.outputs[0].const_shape()
             layout = x.layout.__class__(shape)
             return [Tensor(shape=shape, dtype=x.dtype, device=x.device, storage=x.storage, layout=layout, trace=None)]
@@ -380,16 +397,16 @@
         start_dim = normalize_dim(start_dim, rank)
         end_dim = normalize_dim(end_dim, rank)
         assert 0 <= start_dim <= end_dim < rank
         dims = list(range(len(x.shape)))
         plan = [[v] for v in dims[:start_dim]] + [dims[start_dim : end_dim + 1]] + [[v] for v in dims[end_dim + 1 :]]
         super().__init__(
             inputs=[x],
-            task=RearrangeTask(input_like(x, 'x'), plan=plan),
             attributes={'start_dim': start_dim, 'end_dim': end_dim},
+            task=RearrangeTask(input_like(x, 'x'), plan=plan),
         )
 
     def imperative_run(self, inputs: List[Tensor]) -> List[Tensor]:
         x = inputs[0] if inputs else self.inputs[0]
         if isinstance(x.layout, (RowMajorLayout, ColumnMajorLayout)):
             shape = self.task.outputs[0].const_shape()
             layout = x.layout.__class__(shape)
@@ -404,48 +421,57 @@
             msg = 'Transpose tensor with shape {} expect a permutation of axes with length {}, got {}'.format(
                 x.shape, len(x.shape), axes
             )
             raise ValueError(msg)
         if axes is None:
             axes = list(reversed(range(len(x.shape))))
         plan = [[v] for v in axes]
-        super().__init__(inputs=[x], task=RearrangeTask(input_like(x, 'x'), plan), attributes={'axes': axes})
+        super().__init__(inputs=[x], attributes={'axes': axes}, task=RearrangeTask(input_like(x, 'x'), plan))
 
 
 class CastOp(Operator):
     def __init__(self, x: Tensor, dtype: DataType):
         from hidet.ir.expr import Cast
         from .arithmetic import UnaryElementwiseTask
 
         super().__init__(
             inputs=[x],
-            task=UnaryElementwiseTask('cast', input_like(x, 'x'), op=lambda v: Cast(v, dtype)),
             attributes={'dtype': dtype},
+            task=UnaryElementwiseTask('cast', input_like(x, 'x'), op=lambda v: Cast(v, dtype)),
         )
 
 
 class ConcatOp(Operator):
     def __init__(self, *tensors: Tensor, axis: int):
         tensors = list(tensors)
         if len(tensors) == 0:
             raise ValueError('Concat requires at least one tensor, 0 given.')
         axis = normalize_dim(axis, len(tensors[0].shape))
         super().__init__(
             inputs=tensors,
-            task=ConcatTask([input_like(tensor, 'x{}'.format(idx)) for idx, tensor in enumerate(tensors)], axis=axis),
             attributes={'axis': axis},
+            task=ConcatTask([input_like(tensor, 'x{}'.format(idx)) for idx, tensor in enumerate(tensors)], axis=axis),
         )
 
 
 class TakeOp(Operator):
     def __init__(self, data: Tensor, indices: Tensor, axis: int):
         super().__init__(
             inputs=[data, indices],
+            attributes={'axis': axis},
             task=TakeTask(input_like(data, 'data'), input_like(indices, 'indices'), axis=axis),
+        )
+
+
+class GatherOp(Operator):
+    def __init__(self, data: Tensor, indices: Tensor, axis: int):
+        super().__init__(
+            inputs=[data, indices],
             attributes={'axis': axis},
+            task=GatherTask(input_like(data, 'data'), input_like(indices, 'indices'), axis=axis),
         )
 
 
 class StridedSliceOp(Operator):
     def __init__(
         self,
         data: Tensor,
@@ -453,15 +479,15 @@
         ends: Sequence[Optional[int]],
         axes: Optional[Sequence[Optional[int]]] = None,
         strides: Optional[Sequence[Optional[int]]] = None,
     ):
         starts, ends, axes, strides = self.normalize(data.shape, starts, ends, axes, strides)
         task = StridedSliceTask(input_like(data, 'data'), starts, ends, axes, strides)
         super().__init__(
-            inputs=[data], task=task, attributes={'starts': starts, 'ends': ends, 'axes': axes, 'strides': strides}
+            inputs=[data], attributes={'starts': starts, 'ends': ends, 'axes': axes, 'strides': strides}, task=task
         )
 
     @staticmethod
     def normalize(data_shape, starts, ends, axes: Optional[List[int]], strides: Optional[List[Optional[int]]]):
         # follow: https://data-apis.org/array-api/latest/API_specification/indexing.html
         if axes is None:
             axes = [i for i in range(len(starts))]
@@ -474,16 +500,17 @@
         ii, jj, kk = [], [], []
         for i, j, k, n in zip(starts, ends, strides, shape):
             if k is None:
                 k = 1
             if k > 0:
                 i = i if i is not None else 0
                 j = j if j is not None else n
-                if not (-n <= i <= n and -n <= j <= n):
+                if not (-n <= i <= n and -n <= j):
                     raise IndexError('Invalid slice')
+                j = min(j, n)
                 if i < 0:
                     i += n
                 if j < 0:
                     j += n
             elif k < 0:
                 i = i if i is not None else n - 1
                 j = j if j is not None else -n - 1
@@ -511,43 +538,43 @@
         #         ends[i] = max(-1, min(shape[i] - 1, ends[i]))
         # return starts, ends, axes, strides
 
 
 class BroadcastOp(Operator):
     def __init__(self, data: Tensor, shape: List[int]):
         super().__init__(
-            inputs=[data], task=BroadcastTask(input_like(data, 'data'), shape), attributes={'shape': shape}
+            inputs=[data], attributes={'shape': shape}, task=BroadcastTask(input_like(data, 'data'), shape)
         )
 
 
 class PadOp(Operator):
     def __init__(self, data: Tensor, pads: List[int], mode: str = 'constant', value: float = 0.0):
         if len(pads) < len(data.shape) * 2:
             assert len(pads) % 2 == 0, 'The pads must have even number of elements.'
             half = len(pads) // 2
             extra = [0 for _ in range(len(data.shape) - half)]
             pads = extra + pads[:half] + extra + pads[half:]
         if mode != 'constant':
             raise NotImplementedError("Padding mode '{}' has not been implemented yet.".format(mode))
         super().__init__(
             inputs=[data],
-            task=PadTask(input_like(data, 'data'), pads, value),
             attributes={'pads': pads, 'mode': mode, 'value': value},
+            task=PadTask(input_like(data, 'data'), pads, value),
         )
 
 
 class TileOp(Operator):
     def __init__(self, data: Tensor, repeats: List[int]):
         if len(repeats) != len(data.shape):
             raise ValueError(
                 "The length of 'repeats' parameter of Tile operator expects to have the "
                 "same length as data shape. shape: {}, repeats: {}".format(data.shape, repeats)
             )
         super().__init__(
-            inputs=[data], task=TileTask(input_like(data, 'data'), repeats), attributes={'repeats': repeats}
+            inputs=[data], attributes={'repeats': repeats}, task=TileTask(input_like(data, 'data'), repeats)
         )
 
 
 def reshape(x: Tensor, shape) -> Tensor:
     if same_shape(x.shape, shape):
         return x
     return ReshapeOp(x, shape).get_output(0)
@@ -644,14 +671,18 @@
     return CastOp(x, dtype).get_output(0)
 
 
 def take(data: Tensor, indices: Tensor, axis: int = 0) -> Tensor:
     return TakeOp(data, indices, axis).get_output(0)
 
 
+def gather(data: Tensor, indices: Tensor, axis: int = 0) -> Tensor:
+    return GatherOp(data, indices, axis).outputs[0]
+
+
 def strided_slice(
     data: Tensor,
     starts: Sequence[Optional[int]],
     ends: Sequence[Optional[int]],
     axes: Optional[Sequence[int]] = None,
     strides: Optional[Sequence[Optional[int]]] = None,
 ) -> Tensor:
```

## hidet/graph/ops/definitions/conv2d/conv2d.py

 * *Ordering differences only*

```diff
@@ -54,16 +54,16 @@
 class Conv2dOp(Operator):
     def __init__(self, x: Tensor, w: Tensor, stride: Sequence[int], dilations: Union[int, Sequence[int]], groups: int):
         stride = normalize_stride(stride)
         if isinstance(dilations, int):
             dilations = [dilations, dilations]
         super().__init__(
             inputs=[x, w],
-            task=Conv2dTask(input_like(x, 'x'), input_like(w, 'w'), stride, dilations, groups),
             attributes={'stride': stride, 'groups': groups, 'dilations': dilations},
+            task=Conv2dTask(input_like(x, 'x'), input_like(w, 'w'), stride, dilations, groups),
         )
 
 
 def conv2d(
     data: Tensor,
     weight: Tensor,
     stride: Union[int, Sequence[int]],
```

## hidet/graph/ops/definitions/conv2d/conv2d_gemm.py

 * *Ordering differences only*

```diff
@@ -40,16 +40,16 @@
 
 class Conv2dGemmImageTransformOp(Operator):
     def __init__(self, x: Tensor, kernel, stride, dilations, groups):
         kernel = normalize_kernel(kernel)
         stride = normalize_stride(stride)
         super().__init__(
             inputs=[x],
-            task=Conv2dGemmImageTransformTask(input_like(x, 'x'), kernel, stride, dilations, groups),
             attributes={'kernel': kernel, 'stride': stride, 'groups': groups, 'dilations': dilations},
+            task=Conv2dGemmImageTransformTask(input_like(x, 'x'), kernel, stride, dilations, groups),
         )
 
 
 def conv2d_gemm_image_transform(
     x: Tensor, kernel: List[int], stride: List[int], dilations: List[int], groups: int = 1
 ) -> Tensor:
     return Conv2dGemmImageTransformOp(x, kernel, stride, dilations, groups).get_output(0)
```

## hidet/graph/ops/definitions/conv2d/conv2d_winograd.py

```diff
@@ -120,34 +120,34 @@
     def __init__(self, x: Tensor, kernel, ms):
         if len(x.shape) != 4:
             raise NotImplementedError('Current only support winograd conv2d')
         kernel = normalize_kernel(kernel, dim=2)
         assert len(ms) == 2
         super().__init__(
             inputs=[x],
-            task=Conv2dWinogradImageTransformTask(input_like(x, 'x'), kernel, ms),
             attributes={'kernel': kernel, 'ms': ms},
+            task=Conv2dWinogradImageTransformTask(input_like(x, 'x'), kernel, ms),
         )
 
 
 class Conv2dWinogradFilterTransformOp(Operator):
     def __init__(self, w: Tensor, ms):
         assert len(ms) == 2
         super().__init__(
-            inputs=[w], task=Conv2dWinogradFilterTransformTask(input_like(w, 'w'), ms), attributes={'ms': ms}
+            inputs=[w], attributes={'ms': ms}, task=Conv2dWinogradFilterTransformTask(input_like(w, 'w'), ms)
         )
 
 
 class Conv2dWinogradInverseTransformOp(Operator):
     def __init__(self, y: Tensor, input_shape, kernel, ms):
         kernel = normalize_kernel(kernel, dim=2)
         super().__init__(
             inputs=[y],
-            task=Conv2dWinogradInverseTransformTask(input_like(y, 'y'), input_shape, kernel, ms),
             attributes={'input_shape': input_shape, 'kernel': kernel, 'ms': ms},
+            task=Conv2dWinogradInverseTransformTask(input_like(y, 'y'), input_shape, kernel, ms),
         )
 
 
 def conv2d_winograd_image_transform(x: Tensor, kernel, ms) -> Tensor:
     return Conv2dWinogradImageTransformOp(x, kernel, ms).get_output(0)
```

## hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose.py

 * *Ordering differences only*

```diff
@@ -77,16 +77,16 @@
         stride: Tuple[int, int],
         padding: Tuple[int, int, int, int],
         groups: int,
         output_padding: Tuple[int, int],
     ):
         super().__init__(
             inputs=[x, w],
-            task=Conv2dTransposeTask(input_like(x, 'x'), input_like(w, 'w'), stride, padding, groups, output_padding),
             attributes={'stride': stride, 'padding': padding, 'groups': groups, 'output_padding': output_padding},
+            task=Conv2dTransposeTask(input_like(x, 'x'), input_like(w, 'w'), stride, padding, groups, output_padding),
         )
 
 
 def conv2d_transpose(
     data: Tensor,
     weight: Tensor,
     stride: Union[int, Sequence[int]],
```

## hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose_gemm.py

 * *Ordering differences only*

```diff
@@ -59,24 +59,24 @@
         stride: Tuple[int, int],
         padding: Tuple[int, int, int, int],
         groups: int,
         output_padding: Tuple[int, int],
     ):
         super().__init__(
             inputs=[data],
-            task=Conv2dTransposeGemmImageTask(
-                input_like(data, 'data'), kernel, stride, padding, groups, output_padding
-            ),
             attributes={
                 'kernel': kernel,
                 'stride': stride,
                 'padding': padding,
                 'groups': groups,
                 'output_padding': output_padding,
             },
+            task=Conv2dTransposeGemmImageTask(
+                input_like(data, 'data'), kernel, stride, padding, groups, output_padding
+            ),
         )
 
 
 def conv2d_transpose_gemm_image(
     data: Tensor,
     kernel: Tuple[int, int],
     stride: Tuple[int, int],
```

## hidet/graph/ops/definitions/conv3d/conv3d.py

 * *Ordering differences only*

```diff
@@ -64,16 +64,16 @@
 class Conv3dOp(Operator):
     def __init__(self, x: Tensor, w: Tensor, stride: Sequence[int], dilations: Union[int, Sequence[int]], groups: int):
         stride = normalize_stride(stride, dim=3)
         if isinstance(dilations, int):
             dilations = [dilations, dilations, dilations]
         super().__init__(
             inputs=[x, w],
-            task=Conv3dTask(input_like(x, 'x'), input_like(w, 'w'), stride, dilations, groups),
             attributes={'stride': stride, 'groups': groups, 'dilations': dilations},
+            task=Conv3dTask(input_like(x, 'x'), input_like(w, 'w'), stride, dilations, groups),
         )
 
 
 def conv3d(
     data: Tensor,
     weight: Tensor,
     stride: Union[int, Sequence[int]],
```

## hidet/graph/ops/definitions/conv3d/conv3d_gemm.py

 * *Ordering differences only*

```diff
@@ -48,16 +48,16 @@
 
 class Conv3dGemmImageTransformOp(Operator):
     def __init__(self, x: Tensor, kernel, stride, dilations, groups):
         kernel = normalize_kernel(kernel, dim=3)
         stride = normalize_stride(stride, dim=3)
         super().__init__(
             inputs=[x],
-            task=Conv3dGemmImageTransformTask(input_like(x, 'x'), kernel, stride, dilations, groups),
             attributes={'kernel': kernel, 'stride': stride, 'groups': groups, 'dilations': dilations},
+            task=Conv3dGemmImageTransformTask(input_like(x, 'x'), kernel, stride, dilations, groups),
         )
 
 
 def conv3d_gemm_image_transform(
     x: Tensor, kernel: List[int], stride: List[int], dilations: List[int], groups: int = 1
 ) -> Tensor:
     return Conv3dGemmImageTransformOp(x, kernel, stride, dilations, groups).get_output(0)
```

## hidet/graph/ops/definitions/matmul/batch_matmul.py

```diff
@@ -5,14 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import List
 from hidet.ir.func import IRModule
 from hidet.graph.ops.definitions.utils import Task, Operator, Tensor, TensorNode, compute, reduce, input_like
 
 
 class BatchMatmulTask(Task):
     def __init__(self, a: TensorNode, b: TensorNode, mma: str = 'simt'):
         batch_size, m_size, k_size = a.const_shape()
@@ -32,36 +33,36 @@
         super().__init__(
             name='batch_matmul',
             inputs=[a, b],
             outputs=[c],
             attributes={'batch_size': batch_size, 'm_size': m_size, 'n_size': n_size, 'k_size': k_size, 'mma': mma},
         )
 
-    def implement_cuda(self, workding_dir: str) -> IRModule:
+    def implement_cuda(self, working_dir: str) -> List[IRModule]:
         from hidet.graph.ops.schedules.cuda import matmul as matmul_schedule  # pylint: disable=import-outside-toplevel
 
         if self.mma == 'simt':
-            return matmul_schedule.batched_matmul_cuda_schedule_simt(self, workding_dir)
+            return matmul_schedule.batched_matmul_cuda_schedule_simt(self, working_dir)
         elif self.mma.startswith('wmma'):
-            return matmul_schedule.batched_matmul_cuda_schedule_wmma(self, workding_dir)
+            return matmul_schedule.batched_matmul_cuda_schedule_wmma(self, working_dir)
         elif self.mma.startswith('mma'):
-            return matmul_schedule.batched_matmul_cuda_schedule_mma(self, workding_dir)
+            return matmul_schedule.batched_matmul_cuda_schedule_mma(self, working_dir)
         else:
             raise ValueError('Can not recognize mma type {}, candidates: {}'.format(self.mma, ['simt', 'wmma', 'mma']))
 
 
 class BatchMatmulOp(Operator):
     def __init__(self, a: Tensor, b: Tensor, mma: str = 'simt'):
         if not (len(a.shape) == len(b.shape) == 3 and a.shape[0] == b.shape[0] and a.shape[2] == b.shape[1]):
             raise ValueError(
                 'Matrix multiplication expect tensor A and B with shape [B, M, K] and [B, K, N]'
                 + ', got {} and {}'.format(a.shape, b.shape)
             )
         task = BatchMatmulTask(input_like(a, 'a'), input_like(b, 'b'), mma)
-        super().__init__(inputs=[a, b], task=task, attributes={'mma': mma})
+        super().__init__(inputs=[a, b], attributes={'mma': mma}, task=task)
 
 
 def batch_matmul(a: Tensor, b: Tensor, mma: str = 'simt') -> Tensor:
     """Batched matrix multiplication.
 
     Parameters
     ----------
```

## hidet/graph/ops/definitions/matmul/matmul.py

```diff
@@ -62,12 +62,12 @@
         )
         super().__init__(name='matmul', inputs=[a, b], outputs=[c])
 
 
 class MatmulOp(Operator):
     def __init__(self, a: Tensor, b: Tensor):
         task = MatmulTask(input_like(a, 'a'), input_like(b, 'b'))
-        super().__init__(inputs=[a, b], task=task)
+        super().__init__(inputs=[a, b], attributes={}, task=task)
 
 
 def matmul(a: Tensor, b: Tensor) -> Tensor:
     return MatmulOp(a, b).get_output(0)
```

## hidet/graph/ops/definitions/matmul/matmul_f16.py

```diff
@@ -14,26 +14,26 @@
 from hidet.ir.dtypes import float16
 from hidet.ir.expr import if_then_else
 from hidet.ir.func import IRModule, Function
 from hidet.ir.compute import TensorNode
 from hidet.ir.task import Task
 from hidet.ir.compute import compute, reduce
 from hidet.graph.ops.definitions.utils import input_like, broadcast_shape, can_mutually_broadcast
-from hidet.graph.ops.schedules import tune
+from hidet.graph.ops.definitions.utils import tune
 from hidet.graph.operator import Operator, Tensor
 from hidet.utils.py import is_power_of_two, cdiv, prod
 from hidet.graph.ops.definitions.utils import broadcast_indices
 
 
 class MatmulF16Task(Task):
     def __init__(self, a: TensorNode, b: TensorNode, parallel_k_parts: int = 1):
         a_shape = a.const_shape()
         b_shape = b.const_shape()
 
-        if not a.ttype.dtype == float16 or not b.ttype.dtype == float16:
+        if not a.type.dtype == float16 or not b.type.dtype == float16:
             raise ValueError('Both inputs must be float16 tensors')
 
         if len(a_shape) < 2 or len(b_shape) < 2:
             raise ValueError('Matrix multiplication expect at least 2D tensor, got {} and {}'.format(a_shape, b_shape))
 
         if a_shape[-1] != b_shape[-2]:
             raise ValueError(
@@ -70,18 +70,18 @@
             name='matmul_f16_pk', inputs=[a, b], outputs=[c], attributes={'parallel_k_parts': parallel_k_parts}
         )
 
     def allow_prologue(self) -> bool:
         return False
 
     def allow_epilogue(self) -> bool:
-        return False
+        return True
 
-    def implement_cuda(self, working_dir: str) -> IRModule:
-        return tune.tune(self.schedule, task=self, target_device='cuda', working_dir=working_dir)
+    def implement_cuda(self, working_dir: str) -> List[IRModule]:
+        return tune.extract_ir_modules(self.schedule)
 
     @tune.space(2, 'block_m', [32, 64, 128, 256])
     @tune.space(2, 'block_n', [32, 64, 128, 256])
     @tune.space(2, 'block_k', [8, 16, 32, 64, 128])
     @tune.space(2, 'warp_m', [16, 32, 48, 64])
     @tune.space(2, 'warp_n', [16, 32, 48, 64])
     @tune.space(2, 'warp_k', [8, 16, 32, 64])
@@ -97,68 +97,72 @@
         self, block_m=64, block_n=128, block_k=16, warp_m=32, warp_n=64, warp_k=16, mma: str = 'm16n8k16'
     ) -> IRModule:
         # pylint: disable=unused-variable
         import hidet
         from hidet.ir.type import tensor_type
         from hidet.lang import attr, col_spatial, view, u32, tensor_pointer, grid
         from hidet.lang.layout import row_layout
-        from hidet.lang.mapping import repeat, spatial
+        from hidet.lang.mapping import spatial, auto_map
         from hidet.lang.cuda import blockIdx, threadIdx, syncthreads, dynamic_shared_memory
         from hidet.lang.cuda import MmaConfig, mma_sync, cp_async, cp_async_wait_all, ldmatrix
         from hidet.lang.cuda import register_tensor
-        from hidet.transforms.tools import fuse_and_pack
 
         # input shapes
         node_a, node_b, node_c = self.inputs[0], self.inputs[1], self.outputs[0]
         a_shape: List[int] = node_a.const_shape()
         b_shape: List[int] = node_b.const_shape()
         c_shape: List[int] = node_c.const_shape()
         m_size, n_size, k_size = a_shape[-2], b_shape[-1], a_shape[-1]
         a_head, b_head, c_head = a_shape[:-2], b_shape[:-2], c_shape[:-2]
-        k_parts = self.attributes['parallel_k_parts']
+        k_parts = self.attrs['parallel_k_parts']
         k_part_extent = cdiv(cdiv(k_size, k_parts), 8) * 8
 
         # schedule parameters
         mma_configs = {'m16n8k8': MmaConfig.m16n8k8_f16_f16(), 'm16n8k16': MmaConfig.m16n8k16_f16_f16()}
         tune.check(mma in mma_configs)
         mma_config = mma_configs[mma]
 
         mma_m, mma_n, mma_k = mma_config.m, mma_config.n, mma_config.k  # 16, 8, 16
         warp_count_m, warp_count_n, warp_count_k = block_m // warp_m, block_n // warp_n, block_k // warp_k
         mma_count_m, mma_count_n, mma_count_k = warp_m // mma_m, warp_n // mma_n, warp_k // mma_k
         threads = warp_count_m * warp_count_n * warp_count_k * 32
         grid_dim: Tuple[int, int, int] = cdiv(m_size, block_m), cdiv(n_size, block_n), prod(c_head)
-        dynamic_smem_bytes = 2 * (block_m + block_n) * block_k * 2
+        dynamic_smem_bytes = max(2 * (block_m + block_n) * block_k * 2, block_m * block_n * 2)
 
         tune.check(block_m % warp_m == block_n % warp_n == block_k % warp_k == 0, 'warp dims divide block dims')
         tune.check(warp_m % mma_m == warp_n % mma_n == warp_k % mma_k == 0, 'mma dims divide warp dims')
         tune.check(threads <= 1024, 'threads in a block <= 1024')
-        tune.check(dynamic_smem_bytes <= 49152, 'dynamic shared memory <= 49152')
+        # maximum_smem_bytes = hidet.cuda.properties().sharedMemPerBlock
+        maximum_smem_bytes = 49152
+        tune.check(dynamic_smem_bytes <= maximum_smem_bytes, 'dynamic shared memory <= 49152')
 
         tune.check(block_n % 64 == 0, 'block_n must be multiple of 64, required by async gmem -> smem loading')
         tune.check(block_k % 8 == 0)
         tune.check(is_power_of_two(block_k // 8))
-        tune.check(threads % (block_k // 8) == 0)
-        tune.check(threads % (block_n // 8) == 0)
-        tune.check(block_m % (threads // (block_k // 8)) == 0)
-        tune.check(block_k % (threads // (block_n // 8)) == 0)
+        # tune.check(threads % (block_k // 8) == 0)
+        # tune.check(threads % (block_n // 8) == 0)
+        # tune.check(block_m % (threads // (block_k // 8)) == 0)
+        # tune.check(block_k % (threads // (block_n // 8)) == 0)
         smem_a_type = tensor_type(
             'float16', shape=[block_m, block_k], layout=row_layout(block_m, block_k // 8).swizzle(1) * row_layout(1, 8)
         )
         smem_b_type = tensor_type(
             'float16',
             shape=[block_k, block_n],
             layout=row_layout(block_k // 8, block_n // 64) * row_layout(8, 8).swizzle(1) * row_layout(1, 8),
         )
-        load_smem_a_map = repeat(block_m // (threads // (block_k // 8)), 1).spatial(
-            threads // (block_k // 8), block_k // 8
-        )
-        load_smem_b_map = repeat(block_k // (threads // (block_n // 8)), 1).spatial(
-            threads // (block_n // 8), block_n // 8
-        )
+        load_smem_a_map = auto_map(block_m, block_k // 8, workers=threads, on_fail=lambda msg: tune.check(False, msg))
+        load_smem_b_map = auto_map(block_k, block_n // 8, workers=threads, on_fail=lambda msg: tune.check(False, msg))
+        # load_smem_a_map = repeat(block_m // (threads // (block_k // 8)), 1).spatial(
+        #     threads // (block_k // 8), block_k // 8
+        # )
+        # load_smem_b_map = repeat(block_k // (threads // (block_n // 8)), 1).spatial(
+        #     threads // (block_n // 8), block_n // 8
+        # )
+        store_smem_c_map = auto_map(block_m, block_n, workers=threads, on_fail=lambda msg: tune.check(False, msg))
 
         with hidet.script_module() as module:
 
             @hidet.script
             def load_regs_a(mi: int, k1: int, smem_a: smem_a_type, regs_a: float16[mma_config.a_elements]):
                 warp_id, lane_id = threadIdx.x / 32, threadIdx.x % 32
                 for wi, wj, wk in spatial(warp_count_m, warp_count_n, warp_count_k).on(warp_id):
@@ -217,20 +221,14 @@
                 for k, j_seg in load_smem_b_map.on(threadIdx.x):
                     j = j_seg * 8
                     src_size = (
                         0 if (offset_k + k >= maximum_k or offset_n + j >= n_size) else min(n_size - (offset_n + j), 8)
                     )
                     cp_async(~smem_b[k, j], ~gmem_b[k, j], cp_size=16, src_size=src_size * 2, cache_level='global')
 
-            # @hidet.script
-            # def store_c(
-            #         regs_c: float16[mma_count_m, mma_count_n, mma_config.c_elements],
-            #         c: float16[c_head + [m_size, n_size]]
-            # ):
-
             @hidet.script
             def matmul_f16_kernel(
                 a: float16[a_head + [m_size, k_size]],
                 b: float16[b_head + [k_size, n_size]],
                 c: float16[c_head + [m_size, n_size]],
             ):
                 # matrix multiplication, using mma instruction
@@ -279,45 +277,62 @@
 
                 # store back
                 warp_id, lane_id = threadIdx.x / 32, threadIdx.x % 32
                 offset_m, offset_n = blockIdx.x * block_m, blockIdx.y * block_n
                 c_head_index = spatial(*c_head).map(blockIdx.z)
                 gmem_c = c[c_head_index][offset_m:, offset_n:]
 
-                for k_round in range(warp_count_k):
+                if warp_count_k == 1:
                     for wi, wj, wk in spatial(warp_count_m, warp_count_n, warp_count_k).on(warp_id):
-                        if wk == k_round:
-                            for mi, mj in grid(mma_count_m, mma_count_n):
-                                p = 0
-                                for i, j in mma_config.c_store_map.on(lane_id):
-                                    delta_m = wi * warp_m + mi * mma_m + i
-                                    delta_n = wj * warp_n + mj * mma_n + j
-                                    in_bound = (offset_m + delta_m < m_size) and (offset_n + delta_n < n_size)
-                                    if in_bound:
-                                        if k_round == 0:
-                                            gmem_c[delta_m, delta_n] = regs_c[mi, mj, p]
-                                        else:
-                                            gmem_c[delta_m, delta_n] += regs_c[mi, mj, p]
-                                    p += 1
-                    if warp_count_k > 1:
-                        syncthreads()
+                        for mi, mj in grid(mma_count_m, mma_count_n):
+                            p = 0
+                            for i, j in mma_config.c_store_map.on(lane_id):
+                                delta_m = wi * warp_m + mi * mma_m + i
+                                delta_n = wj * warp_n + mj * mma_n + j
+                                in_bound = (offset_m + delta_m < m_size) and (offset_n + delta_n < n_size)
+                                if in_bound:
+                                    gmem_c[delta_m, delta_n] = regs_c[mi, mj, p]
+                                p += 1
+                else:
+                    smem_c = tensor_pointer('float16', shape=[block_m, block_n])
+                    smem_c = dynamic_shared_memory(byte_offset=0, dtype=float16)
+
+                    for k_round in range(warp_count_k):
+                        for wi, wj, wk in spatial(warp_count_m, warp_count_n, warp_count_k).on(warp_id):
+                            if wk == k_round:
+                                for mi, mj in grid(mma_count_m, mma_count_n):
+                                    p = 0
+                                    for i, j in mma_config.c_store_map.on(lane_id):
+                                        delta_m = wi * warp_m + mi * mma_m + i
+                                        delta_n = wj * warp_n + mj * mma_n + j
+                                        in_bound = (offset_m + delta_m < m_size) and (offset_n + delta_n < n_size)
+                                        if in_bound:
+                                            if k_round == 0:
+                                                smem_c[delta_m, delta_n] = regs_c[mi, mj, p]
+                                            else:
+                                                smem_c[delta_m, delta_n] += regs_c[mi, mj, p]
+                                        p += 1
+                        if warp_count_k > 1:
+                            syncthreads()
+                    for i, j in store_smem_c_map.on(threadIdx.x):
+                        if offset_m + i < m_size and offset_n + j < n_size:
+                            gmem_c[i, j] = smem_c[i, j]
 
         ir_module = module.ir_module()
         assert isinstance(matmul_f16_kernel, Function)
-        fuse_and_pack(ir_module, matmul_f16_kernel, task=self)
 
         return ir_module
 
 
 class MatmulF16Op(Operator):
     def __init__(self, a: Tensor, b: Tensor, parallel_k_parts=1):
         super().__init__(
             inputs=[a, b],
-            task=MatmulF16Task(input_like(a, 'a'), input_like(b, 'b'), parallel_k_parts),
             attributes={'parallel_k_parts': parallel_k_parts},
+            task=MatmulF16Task(input_like(a, 'a'), input_like(b, 'b'), parallel_k_parts),
         )
 
 
 def matmul_f16(a: Tensor, b: Tensor, parallel_k_parts=1) -> Tensor:
     if len(a.shape) < 2 or len(b.shape) < 2:
         raise ValueError('a and b must have at least 2 dimensions, got shape {} and {}'.format(a.shape, b.shape))
     if a.shape[-1] % 8 != 0 or b.shape[-1] % 8 != 0:
```

## hidet/graph/ops/definitions/matmul/resolve.py

```diff
@@ -169,14 +169,17 @@
         a: Tensor = op.inputs[0]
         b: Tensor = op.inputs[1]
         c: Tensor = op.outputs[0]
 
         if not (a.dtype == dtypes.float16 and b.dtype == dtypes.float16 and a.shape[-1] % 8 == b.shape[-1] % 8 == 0):
             return None
 
+        if hidet.cuda.compute_capability() < (8, 0):
+            return None
+
         parallel_k = self.get_config('parallel_k', default='default')  # 'default', 'search', 2, 4, ...
         if isinstance(parallel_k, str):
             if parallel_k == 'default':
                 batch_size, m_size, n_size, k_size = prod(c.shape[:-2]), c.shape[-2], c.shape[-1], a.shape[-1]
                 estimate_blocks = batch_size * cdiv(m_size, 64) * cdiv(n_size, 64)
                 estimate_concurrent_blocks = 80 * 5
                 max_k_parts = cdiv(k_size, 64)
```

## hidet/graph/ops/definitions/reduce/reduce.py

```diff
@@ -65,18 +65,21 @@
                 'dims': dims,
                 'keep_dim': keep_dim,
                 'reduce_type': reduce_type,
                 'accumulate_dtype': accumulate_dtype,
             },
         )
 
-    def implement_cuda(self, workding_dir: str) -> IRModule:
+    def implement_cuda(self, working_dir: str) -> IRModule:
         # pylint: disable=import-outside-toplevel
         from ...schedules import cuda_schedule_reduce_by_default, cuda_schedule_reduce_by_warp_reduce
 
+        if self.inputs[0].type.dtype.name == 'float64':
+            return NotImplemented  # use auto-scheduler
+
         rank = len(self.inputs[0].const_shape())
         if rank - 1 in self.dims:
             # reduce over last dimension
             return cuda_schedule_reduce_by_warp_reduce(self)
         else:
             # last dimension has not been reduced
             return cuda_schedule_reduce_by_default(self)
@@ -115,27 +118,27 @@
     def __init__(self, x: Tensor, dims: Optional[Sequence[int]], keep_dim: bool, reduce_type: ReduceType):
         rank = len(x.shape)
         if dims is None:
             dims = list(range(rank))
         dims = normalize_dim(dims, rank=rank)
         super().__init__(
             inputs=[x],
-            task=ReduceTask(input_like(x, 'x'), dims, keep_dim, reduce_type),
             attributes={'dims': dims, 'keepdims': keep_dim},
+            task=ReduceTask(input_like(x, 'x'), dims, keep_dim, reduce_type),
         )
 
 
 class ArgReduceBaseOp(Operator):
     def __init__(self, x: Tensor, dim: int, keep_dim: bool, reduce_type: ReduceType):
         if reduce_type not in [ReduceType.Min, ReduceType.Max]:
             raise NotImplementedError('Do not support arg reduce type: {}'.format(reduce_type))
         super().__init__(
             inputs=[x],
-            task=ArgReduceTask(input_like(x, 'x'), dim, keep_dim, reduce_type),
             attributes={'dim': dim, 'keepdims': keep_dim},
+            task=ArgReduceTask(input_like(x, 'x'), dim, keep_dim, reduce_type),
         )
 
 
 class ReduceMeanOp(ReduceBaseOp):
     def __init__(self, x: Tensor, dims: Optional[Sequence[int]], keepdims: bool = False):
         super().__init__(x, dims, keepdims, ReduceType.Average)
```

## hidet/graph/ops/definitions/reduce/reduce_f16.py

```diff
@@ -13,15 +13,14 @@
 from hidet.ir import IRModule, dtypes
 from hidet.ir.primitives import active_mask, shfl_down_sync, shfl_sync
 from hidet.ir.compute import ReduceOperation, reduce
 from hidet.ir.type import data_type
 from hidet.ir.layout import DataLayout
 from hidet.lang import f16, f32, spatial, repeat, attr, tensor_pointer
 from hidet.lang.cuda import blockIdx, threadIdx, register_tensor
-from hidet.transforms.tools import add_packed_func, fuse_and_pack
 from hidet.graph.ops.definitions.utils import Task, Operator, Tensor, TensorNode, ReduceType
 from hidet.graph.ops.definitions.utils import compute, input_like, normalize_dim
 from hidet.utils import prod
 
 
 class ReduceF16Task(Task):
     def __init__(
@@ -86,15 +85,15 @@
         if rank - 1 in self.dims:  # pylint: disable=simplifiable-if-statement
             # use self.cuda_schedule_reduce_by_warp
             return True
         else:
             # use self.cuda_schedule_reduce_by_default
             return False
 
-    def implement_cuda(self, workding_dir: str) -> IRModule:
+    def implement_cuda(self, working_dir: str) -> IRModule:
         rank = len(self.inputs[0].const_shape())
         if rank - 1 in self.dims:
             return self.cuda_schedule_reduce_by_warp()
         else:
             return self.cuda_schedule_reduce_by_default()
 
     def cuda_schedule_reduce_by_warp(self) -> IRModule:
@@ -127,16 +126,16 @@
                 spatial_shape.append(1)
                 repeat_shape.append(shape_32bit[i])
             else:
                 spatial_shape.append(shape_32bit[i])
                 repeat_shape.append(1)
         task_layout = repeat(*repeat_shape) * spatial(*spatial_shape)
         grid_size = remain_layout.num_workers
-        accumulate_dtype = self.attributes['accumulate_dtype']
-        reduce_type = self.attributes['reduce_type']
+        accumulate_dtype = self.attrs['accumulate_dtype']
+        reduce_type = self.attrs['reduce_type']
         ro = ReduceOperation.from_name(reduce_type)
 
         with hidet.script_module() as module:
 
             @hidet.script
             def reduce_kernel(x: f16[x.const_shape()], y: f16[y.const_shape()]):
                 attr.cuda_grid_dim = grid_size
@@ -166,15 +165,14 @@
                 rv[0] = shfl_sync(mask, rv[0], 0, 32)
                 rv[0] = ro.finalize(acc=rv[0], size=reduce_extent)
                 if threadIdx.x == 0:
                     for indices in remain_layout.on(blockIdx.x):
                         y.write(indices, rv[0], protected=False)
 
         ir_module = module.ir_module()
-        fuse_and_pack(ir_module, reduce_kernel, task=self)
         return ir_module
 
     def cuda_schedule_reduce_by_default(self) -> IRModule:
         import hidet
 
         x, y = self.inputs[0], self.outputs[0]
         dims = self.dims
@@ -202,16 +200,16 @@
                 repeat_shape.append(shape_32bit[i])
             else:
                 spatial_shape.append(shape_32bit[i])
                 repeat_shape.append(1)
         task_layout = repeat(*repeat_shape) * spatial(*spatial_shape)
 
         grid_size = (remain_layout.num_workers + block_size - 1) // block_size
-        accumulate_dtype = self.attributes['accumulate_dtype']
-        reduce_type = self.attributes['reduce_type']
+        accumulate_dtype = self.attrs['accumulate_dtype']
+        reduce_type = self.attrs['reduce_type']
         ro = ReduceOperation.from_name(reduce_type)
 
         with hidet.script_module() as module:
 
             @hidet.script
             def reduce_kernel(x: f16[x.const_shape()], y: f16[y.const_shape()]):
                 # Each 256-thread ThreadBlock handles 512 columns
@@ -238,28 +236,27 @@
                         rv[1] = ro.combine(rv[1], regs16[1])
                     regs16[0] = ro.finalize(acc=rv[0], size=reduce_extent)
                     regs16[1] = ro.finalize(acc=rv[1], size=reduce_extent)
                     for indices in remain_layout.on(threadIdx.x + blockIdx.x * block_size):
                         y_f32.write(indices, reg32[0], protected=False)
 
         ir_module = module.ir_module()
-        add_packed_func(ir_module, func=reduce_kernel, pack_func_name=self.name)
         return ir_module
 
 
 class ReduceBaseF16Op(Operator):
     def __init__(self, x: Tensor, dims: Optional[Sequence[int]], keep_dim: bool, reduce_type: ReduceType):
         rank = len(x.shape)
         if dims is None:
             dims = list(range(rank))
         dims = normalize_dim(dims, rank=rank)
         super().__init__(
             inputs=[x],
-            task=ReduceF16Task(input_like(x, 'x'), dims, keep_dim, reduce_type),
             attributes={'dims': dims, 'keepdims': keep_dim},
+            task=ReduceF16Task(input_like(x, 'x'), dims, keep_dim, reduce_type),
         )
 
 
 class ReduceMeanF16Op(ReduceBaseF16Op):
     def __init__(self, x: Tensor, dims: Optional[Sequence[int]], keepdims: bool = False):
         super().__init__(x, dims, keepdims, ReduceType.Average)
```

## hidet/graph/ops/definitions/reduce/resolve.py

```diff
@@ -40,15 +40,15 @@
         if keepdims:
             return [x]
         return [x.squeeze(dims)]
 
     def resolve_f16(self, op: Operator) -> Optional[List[Tensor]]:
         dims = op.attrs['dims']
         keepdims = op.attrs['keepdims']
-        reduce_type = op.task.attributes['reduce_type']
+        reduce_type = op.task.attrs['reduce_type']
         x: Tensor = op.inputs[0]
         last_dim = x.shape[-1]
         if x.dtype != dtypes.float16 or last_dim % 2 != 0:
             return None
         return [reduce_f16(x, dims, keepdims, reduce_type)]
 
     def resolve_generic(self, op: Operator) -> Optional[List[Tensor]]:
```

## hidet/graph/ops/schedules/auto_scheduler.py

```diff
@@ -8,25 +8,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Union, List, Dict, Sequence, Tuple, Set
 
 from hidet.ir.type import tensor_pointer_type, void_pointer
-from hidet.ir.expr import TensorElement, Expr, Var, scalar_var, convert, cast
-from hidet.ir.stmt import Stmt, AssignStmt, ForStmt, DeclareStmt, BufferStoreStmt
+from hidet.ir.expr import TensorElement, Expr, Var, Constant, scalar_var, convert, cast, deref
+from hidet.ir.stmt import Stmt, AssignStmt, ForStmt, DeclareStmt, BufferStoreStmt, AssertStmt
 from hidet.ir.task import Task
 from hidet.ir.func import IRModule, Function
 from hidet.ir.builders import FunctionBuilder, StmtBuilder
-from hidet.ir.functors import ExprRewriter, ExprVisitor, ComputeVisitor, ComputeRewriter
-from hidet.ir.tools import collect, rewrite, infer_type, simplify_to_int
+from hidet.ir.functors import ExprRewriter, ExprVisitor, ComputeVisitor, ComputeRewriter, TypeRewriter
+from hidet.ir.tools import collect, rewrite, infer_type, simplify
 from hidet.ir.compute import ScalarInput, TensorInput, GridCompute, ReduceCompute, ArgReduceCompute
 from hidet.ir.compute import TensorNode, ScalarNode
 from hidet.ir.primitives.runtime import request_cuda_workspace, request_cpu_workspace
-from hidet.ir.dtypes import uint8, int32
+from hidet.ir.dtypes import uint8, int32, int64
 from hidet.utils import prod, DirectedGraph
 from hidet.utils.namer import Namer
 
 
 class ScalarComputeFound(Exception):
     pass
 
@@ -152,36 +152,36 @@
         return dag
 
     @staticmethod
     def plan_memory(
         dag: DirectedGraph,  # pylint: disable=unused-argument
         order: Sequence[TensorNode],
         require_allocate: Set[TensorNode],
-    ) -> Tuple[int, Dict[TensorNode, int]]:
+    ) -> Tuple[Expr, Dict[TensorNode, Expr]]:
         # dag has not been used in this simple plan.
         alignment_bytes: int = 128  # make sure each buffer aligns with 128 bytes
-        allocated_bytes: int = 0
-        buffer_offset: Dict[TensorNode, int] = {}
+        allocated_bytes: Expr = int64(0)
+        buffer_offset: Dict[TensorNode, Expr] = {}
         for tensor in order:
             if tensor not in require_allocate:
                 continue
             buffer_offset[tensor] = allocated_bytes
-            allocated_bytes += simplify_to_int(tensor.type.storage_bytes())
-            allocated_bytes = (allocated_bytes + alignment_bytes - 1) // alignment_bytes * alignment_bytes
+            allocated_bytes = allocated_bytes + simplify(tensor.type.storage_bytes())
+            allocated_bytes = (allocated_bytes + (alignment_bytes - 1)) // alignment_bytes * alignment_bytes
         return allocated_bytes, buffer_offset
 
     @staticmethod
     def allocate_tensors(
         fb: FunctionBuilder,
         device: str,
-        buffer_bytes: int,
-        buffer_offset: Dict[TensorNode, int],
+        buffer_bytes: Expr,
+        buffer_offset: Dict[TensorNode, Expr],
         node_map: Dict[TensorNode, Var],
     ):
-        if buffer_bytes > 0:
+        if not (isinstance(buffer_bytes, Constant) and int(buffer_bytes) == 0):
             buffer = Var('buffer', tensor_pointer_type(dtype='uint8', shape=[buffer_bytes]))
             if device == 'cuda':
                 space_ptr: Expr = request_cuda_workspace(nbytes=buffer_bytes, require_clean=False)
             elif device == 'cpu':
                 space_ptr: Expr = request_cpu_workspace(nbytes=buffer_bytes, require_clean=False)
             else:
                 raise ValueError()
@@ -195,58 +195,74 @@
             assert buffer is not None
             v = Var(node.name, ~node.type)
             node_map[node] = v
             fb += DeclareStmt(v, init=cast(~buffer[buffer_offset[node]], ~v.type.tensor_type.dtype))
 
     def schedule_task(self, task: Task, device: str) -> IRModule:
         # pylint: disable=too-many-locals, unnecessary-comprehension
-        # absorb the prologue and epilogue into a single task
-        task = task.task_graph.absorb()
+        from hidet.ffi.packedfunc import ArgTypeCode
 
         self.ir_module.task = task
 
         # Inline the grid compute that does not contain reduce
         outputs: List[TensorNode] = inline_grid_compute(task.outputs)
+        output_remap: Dict[TensorNode, TensorNode] = {a: b for a, b in zip(task.outputs, outputs)}
+        updated_params = [output_remap[p] if p in output_remap else p for p in task.params]
 
         # Taking the TensorNode as node to construct the computation directed-acyclic-graph (DAG)
         # In the DAG, each node is a TensorNode and each edge (src, dst) indicates src is accessed by dst.
         dag = self.build_dag(outputs)
 
         # Get a topological order of the tensor nodes in the DAG
         order: List[TensorNode] = dag.topological_order()
 
         # Plan the memory for intermediate tensors
+        # only allocate the memory for intermediate tensors
         require_allocate = set(node for node in order if node not in task.inputs and node not in outputs)
+        # plan the memory for intermediate tensors
         buffer_bytes, buffer_offset = self.plan_memory(dag, order, require_allocate)
 
-        # Allocate the memory for intermediate tensors, get the mapping from node to tensor var or tensor pointer var
-        with FunctionBuilder(name=task.name, kind='packed_func') as fb:
+        # Construct the function body
+        with FunctionBuilder(name='launch', kind='packed_func') as fb:
             # packed function arguments, packed_func(num_args: int32, arg_types: *int32, args: **void)
             num_args = scalar_var('num_args', 'int32')
             arg_types = Var('arg_types', ~int32)
             args = Var('args', ~void_pointer())
             fb.extend_params([num_args, arg_types, args])
 
-            # extract the actual arguments from packed arguments
-            params: List[Var] = []
-            for idx, task_param in enumerate(task.inputs + task.outputs):
-                param = Var(task_param.name, ~task_param.type.dtype)
-                params.append(param)
-                fb += DeclareStmt(param, init=cast(args[idx], param.type))
+            # extract the packed arguments
+            node_map: Dict[TensorNode, Var] = {}  # tensor arguments
+            scalar_map: Dict[Var, Var] = {}  # scalar arguments
+            for idx, task_param in enumerate(updated_params):
+                if isinstance(task_param, Var):
+                    param = Var(task_param.name, task_param.type)
+                    expect_type_code = ArgTypeCode.from_type(task_param.type).value
+                    scalar_map[task_param] = param
+                    init = deref(cast(args[idx], ~task_param.type))
+                else:
+                    assert isinstance(task_param, TensorNode)
+                    param = Var(task_param.name, ~task_param.type.dtype)
+                    expect_type_code = ArgTypeCode.POINTER.value
+                    node_map[task_param] = param
+                    init = cast(args[idx], param.type)
+                fb += AssertStmt(
+                    cond=(arg_types[idx] == expect_type_code),
+                    msg='Argument {} expects a {}'.format(idx, ArgTypeCode(expect_type_code).name.lower()),
+                )
+                fb += DeclareStmt(param, init=init)
 
             # allocate memory space for intermediate tensors
-            node_map: Dict[TensorNode, Var] = {a: b for a, b in zip(task.inputs + outputs, params)}
             self.allocate_tensors(fb, device, buffer_bytes, buffer_offset, node_map)
 
             # schedule each tensor computation
             for node in order:
                 if isinstance(node, TensorInput):
                     pass  # input tensor does not need scheduling, skip
                 elif isinstance(node, GridCompute):
-                    fb += self.schedule_grid_compute(node, node_map)
+                    fb += self.schedule_grid_compute(node, node_map, scalar_map)
                 else:
                     raise NotImplementedError()
         func = fb.get()
         self.ir_module.add(func.name, func)
 
         return self.ir_module
 
@@ -267,52 +283,73 @@
             The variable points to the added function.
         """
         name = Namer.unique_name_among(func.name, self.ir_module.functions.keys())
         func.name = name
         self.ir_module.add(func.name, func)
         return self.ir_module.lookup_var(func.name)
 
-    def schedule_grid_compute(self, node: GridCompute, node_map: Dict[TensorNode, Expr]) -> Stmt:
+    def grid_compute_params_and_args(
+        self, node: GridCompute, node_map: Dict[TensorNode, Var], scalar_map: Dict[Var, Var]
+    ) -> Tuple[List[Var], Dict[Union[TensorNode, Var], Var], List[Expr]]:
+        # collect used tensors and scalars
+        used_scalars: List[Var] = collect(node.value, Var)
+        used_tensors: List[TensorNode] = collect(node.value, TensorNode, stop_when_found=True)
+
+        # get the scalar and tensor parameters
+        param_scalars: List[Var] = [v for v in used_scalars if v in scalar_map]
+        param_tensors: List[TensorNode] = used_tensors + [node]
+
+        # declare the parameter variables
+        params: List[Var] = []
+        # first declare the scalar parameters
+        params.extend([Var(scalar.name, scalar.type) for scalar in param_scalars])
+        param_map: Dict[Union[TensorNode, Var], Var] = {scalar: param for scalar, param in zip(param_scalars, params)}
+        params.extend([Var(tensor.name, rewrite(tensor.type, param_map)) for tensor in param_tensors])
+        # the tensor shape and layout may use the scalar parameters, so we need to rewrite them to use the param vars
+        param_map.update({tensor: param for tensor, param in zip(param_tensors, params[len(param_scalars) :])})
+
+        # construct the call arguments
+        call_args: List[Expr] = []
+        call_args.extend([scalar_map[param_scalar] for param_scalar in param_scalars])
+        call_args.extend([node_map[param_tensor] for param_tensor in param_tensors])
+
+        return params, param_map, call_args
+
+    def schedule_grid_compute(
+        self, node: GridCompute, node_map: Dict[TensorNode, Var], scalar_map: Dict[Var, Var]
+    ) -> Stmt:
         raise NotImplementedError()
 
 
-class ComputeExprLower(ExprRewriter, ComputeRewriter):
-    def __init__(self, expr: Expr, param_map: Dict[Union[TensorNode, ScalarNode], Expr]):
+class ComputeExprLower(ExprRewriter, ComputeRewriter, TypeRewriter):
+    def __init__(self, expr: Expr, param_map: Dict[Union[TensorNode, ScalarNode, Var], Expr]):
         super().__init__()
         self.sb: StmtBuilder = StmtBuilder()
         self.compute_expr: Expr = expr
         self.param_map: Dict[Union[TensorNode, ScalarNode], Expr] = param_map
+        self.memo.update(param_map)
 
     def lower(self) -> Tuple[List[Stmt], Expr]:
         result = self.visit(self.compute_expr)
         assert len(self.sb.scope_stack) == 1, "some scope has not been exited?"
         return self.sb.scope_stack[0], result
 
     def visit_TensorInput(self, node: TensorInput):
-        if node in self.param_map:
-            return self.param_map[node]
-        else:
-            raise ValueError('Expect tensor input "{}" in param_map.'.format(node))
+        raise ValueError('Expect tensor input "{}" in param_map.'.format(node))
 
     def visit_ScalarInput(self, node: ScalarInput):
-        if node in self.param_map:
-            return self.param_map[node]
-        else:
-            raise ValueError('Expect scalar input "{}" in param_map.'.format(node))
+        raise ValueError('Expect scalar input "{}" in param_map.'.format(node))
 
     def visit_GridCompute(self, node: GridCompute):
-        if node in self.param_map:
-            return self.param_map[node]
-
         # declare intermediate tensor buffer
         buf = Var(node.name, node.type)
 
         # tensor compute loops
         for i in range(len(node.shape)):
-            self.sb.enter_body(ForStmt(node.axes[i], node.shape[i]))
+            self.sb.enter_body(ForStmt(node.axes[i], self.visit(node.shape[i])))
 
         # at the innermost loop body
         expr = self.visit(node.value)
         self.sb.append(BufferStoreStmt(buf, node.axes, expr))
 
         # exit loop scope
         for i in range(len(node.shape)):
@@ -323,15 +360,15 @@
         shape, axes, value = node.shape, node.axes, node.value
         # declare accumulator
         acc = scalar_var(node.name, infer_type(value))
         self.sb += DeclareStmt(acc, init=node.reduce_operation.initial_value(node.type))
 
         # reduction loops
         for i in range(len(shape)):
-            self.sb.enter_body(ForStmt(axes[i], shape[i]))
+            self.sb.enter_body(ForStmt(axes[i], self.visit(shape[i])))
 
         # at the innermost loop body
         expr = self.visit(value)
         self.sb += AssignStmt(acc, node.reduce_operation.combine(acc, expr))
 
         # exit loop scope
         for i in range(len(shape)):
@@ -339,15 +376,15 @@
 
         # finalize
         acc = node.reduce_operation.finalize(acc, prod(shape))
 
         return acc
 
     def visit_ArgReduceCompute(self, node: ArgReduceCompute):
-        extent, axis, value = node.extent, node.axis, node.value
+        extent, axis, value = self.visit(node.extent), node.axis, node.value
         value_dtype = infer_type(value)
         # declare index accumulator
         acc_index = scalar_var(node.name + '_idx', node.index_dtype)
         acc_value = scalar_var(node.name + '_val', value_dtype)
 
         # init accumulator
         self.sb += DeclareStmt(acc_index, init=convert(0))
```

## hidet/graph/ops/schedules/resolve.py

```diff
@@ -13,64 +13,60 @@
 import time
 from typing import List, Optional
 import shutil
 import numpy as np
 from tqdm import tqdm
 
 from hidet import option
-from hidet.ir.type import TensorType
-from hidet.ir.expr import Constant
 from hidet.ir.func import IRModule
-from hidet.ir.task import Task
 from hidet.utils import TableBuilder, strict_zip, error_tolerance
-from hidet.graph.tensor import randn, zeros, ones, Tensor
+from hidet.graph.tensor import Tensor
 from hidet.option import get_option
 from .common import Schedule
 
 
-def dummy_inputs_from_task(task: Task, target_device: str) -> List[Tensor]:
-    """
-    Create dummy inputs values for given task.
-
-    Parameters
-    ----------
-    task: Task
-        The task to generate dummy inputs for.
-
-    Returns
-    -------
-    ret: List[Tensor]
-        The dummy input tensors.
-    """
-    inputs = []
-    for param in task.parameters:
-        param_type = param.type
-
-        if not isinstance(param_type, TensorType):
-            raise ValueError('Currently, only support create dummy scalar inputs.')
-        if any(not isinstance(s, Constant) for s in param_type.shape):
-            raise ValueError('Currently, only support create dummy values for static tensor inputs.')
-        dtype = param_type.dtype.name
-        shape = [int(s) for s in param_type.shape]
-        if dtype in ['float32', 'float16', 'bfloat16']:
-            x = randn(shape, dtype, device=target_device)
-        elif dtype in ['int64', 'int32', 'int8', 'uint64', 'uint32', 'uint8']:
-            x = zeros(shape, dtype, device=target_device)
-        elif dtype == 'bool':
-            x = ones(shape, dtype, device=target_device)
-        else:
-            raise ValueError('Currently do not support generate random array for data type {}'.format(dtype))
-        inputs.append(x)
-    return inputs
+# def dummy_inputs_from_task(task: Task, target_device: str) -> List[Tensor]:
+#     """
+#     Create dummy inputs values for given task.
+#
+#     Parameters
+#     ----------
+#     task: Task
+#         The task to generate dummy inputs for.
+#
+#     Returns
+#     -------
+#     ret: List[Tensor]
+#         The dummy input tensors.
+#     """
+#     inputs = []
+#     for param in task.parameters:
+#         param_type = param.type
+#
+#         if not isinstance(param_type, TensorType):
+#             raise ValueError('Currently, only support create dummy scalar inputs.')
+#         if any(not isinstance(s, Constant) for s in param_type.shape):
+#             raise ValueError('Currently, only support create dummy values for static tensor inputs.')
+#         dtype = param_type.dtype.name
+#         shape = [int(s) for s in param_type.shape]
+#         if dtype in ['float32', 'float16', 'bfloat16']:
+#             x = randn(shape, dtype, device=target_device)
+#         elif dtype in ['int64', 'int32', 'int8', 'uint64', 'uint32', 'uint8']:
+#             x = zeros(shape, dtype, device=target_device)
+#         elif dtype == 'bool':
+#             x = ones(shape, dtype, device=target_device)
+#         else:
+#             raise ValueError('Currently do not support generate random array for data type {}'.format(dtype))
+#         inputs.append(x)
+#     return inputs
 
 
 def resolve_ir_modules(
     ir_modules: List[IRModule],
     schedules: List[Schedule],
-    func_name: str,
     target_device: str,
     output_dir: str,
     parallel=True,
     verbose=True,
     validate=False,
 ) -> IRModule:
     """
@@ -109,32 +105,20 @@
         return ir_modules[0]
     if len(schedules) != len(ir_modules):
         raise ValueError('The number of ir modules and schedules does not match.')
     if any(ir_module.task != ir_modules[0].task for ir_module in ir_modules):
         raise ValueError('Require all ir modules are from the same task.')
 
     # build ir modules
-    # build_instances = [
-    #     BuildInstance(
-    #         ir_module=ir_module,
-    #         output_dir=os.path.join(output_dir, 'resolve', str(idx)),
-    #         keep_ir=False,
-    #         nvcc_keep=False,
-    #         verbose=False,
-    #     )
-    #     for idx, ir_module in enumerate(ir_modules)
-    # ]
-    # compiled_funcs: List[Optional[CompiledFunction]] = batch_build_ir_modules(
-    #     build_instances, parallel=parallel, verbose=verbose
-    # )
     resolve_dir = os.path.join(output_dir, 'resolve')
     compiled_funcs: List[Optional[CompiledFunction]] = build_ir_module_batch(
-        ir_modules, func_name=func_name, output_dir=resolve_dir, parallel=parallel, verbose=verbose
+        ir_modules, output_dir=resolve_dir, parallel=parallel, verbose=verbose
     )
-    dummy_inputs = dummy_inputs_from_task(ir_modules[0].task, target_device)
+    # dummy_inputs = dummy_inputs_from_task(ir_modules[0].task, target_device)
+    dummy_inputs = ir_modules[0].task.dummy_arguments(target_device)
     best_latency = 1e30
     best_ir_module = None
     latencies = []
     time.sleep(1.0)
 
     if all(f is None for f in compiled_funcs):
         raise ValueError('All ir modules are failed in building.')
```

## hidet/graph/ops/schedules/cpu/auto_scheduler.py

```diff
@@ -5,46 +5,45 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List, Dict
+from typing import Dict
 
 from hidet.ir.builders import FunctionBuilder
 from hidet.ir.compute import TensorNode, GridCompute
-from hidet.ir.expr import Call, Expr, Var, convert
-from hidet.ir.tools import collect, rewrite
+from hidet.ir.expr import Call, Var, convert
+from hidet.ir.tools import rewrite
 from hidet.ir.stmt import Stmt, BufferStoreStmt, EvaluateStmt
 from ..auto_scheduler import AutoScheduler, ComputeExprLower
 
 
 class CpuAutoScheduler(AutoScheduler):
-    def schedule_grid_compute(self, node: GridCompute, node_map: Dict[TensorNode, Expr]) -> Stmt:
+    def schedule_grid_compute(
+        self, node: GridCompute, node_map: Dict[TensorNode, Var], scalar_map: Dict[Var, Var]
+    ) -> Stmt:
         # pylint: disable=too-many-locals, import-outside-toplevel, unnecessary-comprehension
         from hidet.ir.mapping import row_repeat, TaskMapping
 
-        used_tensors: List[TensorNode] = collect(node.value, TensorNode, stop_when_found=True)
-        param_tensors: List[TensorNode] = used_tensors + [node]
-        params: List[Var] = [Var(tensor.name, tensor.type) for tensor in param_tensors]
+        params, param_map, call_args = self.grid_compute_params_and_args(node, node_map, scalar_map)
 
         with FunctionBuilder(name=f'compute_{node.name}', kind='host_kernel') as fb:
             # set function parameters
             fb.extend_params(params)
 
-            mapping: TaskMapping = row_repeat(*node.shape)
+            mapping: TaskMapping = row_repeat(*[rewrite(d, param_map) for d in node.shape])
             iter_names = [f'i{i}' for i in range(len(node.shape))]
             with fb.for_mapping(iter_names, mapping, convert(0)) as task_index:
-                out_param: Var = params[-1]
-                param_map: Dict[TensorNode, Expr] = {
-                    tensor_node: param_var for tensor_node, param_var in zip(param_tensors, params)
-                }
+                out_param: Var = param_map[node]
                 compute_lower = ComputeExprLower(node.value, param_map=param_map)
                 stmts, value = compute_lower.lower()
                 rmap = {axis: axis_value for axis, axis_value in zip(node.axes, task_index)}
                 stmts, value = [rewrite(stmt, rmap) for stmt in stmts], rewrite(value, rmap)
                 fb += stmts
                 fb += BufferStoreStmt(out_param, task_index, value)
         func = fb.get()
         func_var = self.add_function(func)
-        return EvaluateStmt(Call(func_var, args=[node_map[param_tensor] for param_tensor in param_tensors]))
+
+        # call the created function in the launch function
+        return EvaluateStmt(Call(func_var, args=call_args))
```

## hidet/graph/ops/schedules/cuda/auto_scheduler.py

```diff
@@ -5,57 +5,59 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List, Dict
+from typing import List, Dict, Union
 
 from hidet.ir.builders import FunctionBuilder
 from hidet.ir.compute import TensorNode, GridCompute
-from hidet.ir.expr import Call, Expr, Var
-from hidet.ir.tools import collect, rewrite, simplify_to_int
-from hidet.ir.stmt import Stmt, BufferStoreStmt, EvaluateStmt
+from hidet.ir.expr import Expr, Var
+from hidet.ir.tools import rewrite, simplify
+from hidet.ir.stmt import Stmt, BufferStoreStmt, launch_kernel
 from hidet.utils import prod
 from ..auto_scheduler import AutoScheduler, ComputeExprLower
 
 
 class CudaAutoScheduler(AutoScheduler):
-    def schedule_grid_compute(self, node: GridCompute, node_map: Dict[TensorNode, Expr]) -> Stmt:
+    def schedule_grid_compute(
+        self, node: GridCompute, node_map: Dict[TensorNode, Var], scalar_map: Dict[Var, Var]
+    ) -> Stmt:
         # pylint: disable=unnecessary-comprehension, import-outside-toplevel
         from hidet.ir.primitives.cuda import threadIdx, blockIdx
         from hidet.ir.mapping import row_spatial, TaskMapping
 
-        used_tensors: List[TensorNode] = collect(node.value, TensorNode, stop_when_found=True)
-        param_tensors: List[TensorNode] = used_tensors + [node]
-        params: List[Var] = [Var(tensor.name, tensor.type) for tensor in param_tensors]
+        params: List[Var]
+        param_map: Dict[Union[TensorNode, Var], Var]
+        call_args: List[Expr]
+        params, param_map, call_args = self.grid_compute_params_and_args(node, node_map, scalar_map)
 
-        block_dim = 500
-        grid_dim: int = simplify_to_int((prod(node.shape) + block_dim - 1) // block_dim)
+        node_shape: List[Expr] = [simplify(rewrite(dim, param_map)) for dim in node.shape]
+
+        block_dim = 512
+        grid_dim: Expr = (prod(rewrite(node.shape, scalar_map)) + block_dim - 1) // block_dim
 
         with FunctionBuilder(
             name=f'compute_{node.name}', kind='cuda_kernel', grid_dim=grid_dim, block_dim=block_dim
         ) as fb:
             # set function parameters
             fb.extend_params(params)
 
             # calculate task indices assigned to current worker
             worker = blockIdx.x * block_dim + threadIdx.x
 
-            mapping: TaskMapping = row_spatial(*node.shape)
-            iter_names = [f'i{i}' for i in range(len(node.shape))]
+            mapping: TaskMapping = row_spatial(*node_shape)
+            iter_names = [f'i{i}' for i in range(len(node_shape))]
             with fb.if_then(worker < mapping.num_workers):
                 with fb.for_mapping(iter_names, mapping, worker) as task_index:
                     out_param: Var = params[-1]
-                    param_map: Dict[TensorNode, Expr] = {
-                        tensor_node: param_var for tensor_node, param_var in zip(param_tensors, params)
-                    }
                     compute_lower = ComputeExprLower(node.value, param_map=param_map)
                     stmts, value = compute_lower.lower()
                     rmap = {axis: axis_value for axis, axis_value in zip(node.axes, task_index)}
                     stmts, value = [rewrite(stmt, rmap) for stmt in stmts], rewrite(value, rmap)
                     fb += stmts
                     fb += BufferStoreStmt(out_param, task_index, value)
         func = fb.get()
         func_var = self.add_function(func)
-        return EvaluateStmt(Call(func_var, args=[node_map[param_tensor] for param_tensor in param_tensors]))
+        return launch_kernel(func_var, args=call_args, grid_dim=grid_dim, block_dim=block_dim)
```

## hidet/graph/ops/schedules/cuda/depthwise_conv.py

```diff
@@ -15,15 +15,14 @@
 import hidet.cuda
 from hidet import option
 from hidet.ir.func import IRModule
 from hidet.graph.ops.definitions.conv2d.conv2d import Conv2dTask
 from hidet.graph.ops.schedules.common import Schedule, NotSupportedError
 from hidet.graph.ops.schedules.resolve import resolve_ir_modules
 from hidet.utils import prod
-from hidet.transforms.tools import fuse_and_pack
 
 
 T = TypeVar('T', bound=Tuple)
 
 
 def tuple_divide(lhs: T, rhs: T, ceil=False) -> T:
     assert len(lhs) == len(rhs)
@@ -137,15 +136,14 @@
             stride_height,
         )
         for sch in schedules
     ]
     return resolve_ir_modules(
         ir_modules=ir_modules,
         schedules=schedules,
-        func_name=task.name,
         target_device='cuda',
         output_dir=os.path.join(workding_dir, './resolve'),
         parallel=True,
         verbose=True,
     )
 
 
@@ -256,8 +254,8 @@
                         regs_y[rn, rc, rh, rw] = (
                             regs_y[rn, rc, rh, rw]
                             + smem_x[nn, cc, hh * stride_height + r, ww * stride_width + s] * smem_w[cc, r, s]
                         )
                     if gn < batch_size and gc < channels and gh < height and gw < width:
                         gmem_y[gn, gc, gh, gw] = regs_y[rn, rc, rh, rw]
 
-    return fuse_and_pack(script_module.ir_module(), conv2d_grid, task)
+    return script_module.ir_module()
```

## hidet/graph/ops/schedules/cuda/reduce.py

```diff
@@ -19,15 +19,14 @@
 from hidet.ir.compute import ReduceOperation
 from hidet.ir.stmt import AssignStmt, BufferStoreStmt, DeclareStmt
 from hidet.ir.type import data_type
 from hidet.ir.utils import index_deserialize
 from hidet.graph.ops.definitions.reduce import ReduceTask
 from hidet.graph.ops.schedules.common import params_from_task
 from hidet.utils import prod
-from hidet.transforms.tools import fuse_and_pack
 from .common import warp_reduce
 
 
 def merge_indices(grid_indices: List[Expr], reduce_indices: List[Expr], reduce_dims: List[int]) -> List[Expr]:
     indices = []
     grid_indices = list(reversed(grid_indices))
     reduce_indices = list(reversed(reduce_indices))
@@ -52,15 +51,15 @@
 
     warp_size = 32
     reduce_extent = prod(reduce_shape)
     warp_extent = (reduce_extent + warp_size - 1) // warp_size
     block_layout = TaskMapping.full_layout([warp_extent]) * TaskMapping.row_major([warp_size])
 
     x_dtype = task.inputs[0].ttype.dtype
-    accumulate_dtype = task.attributes['accumulate_dtype']
+    accumulate_dtype = task.attrs['accumulate_dtype']
 
     with FunctionBuilder(
         name=task.name + '_grid',
         kind='cuda_kernel',
         grid_dim=grid_layout.num_workers,
         block_dim=block_layout.num_workers,
         label='reduce schedule',
@@ -99,15 +98,15 @@
                     else:
                         output_indices = grid_indices
                     fb += BufferStoreStmt(y, output_indices, cast(rv, x_dtype))
 
         fb.set_body(fb.finish())
     func = fb.get()
     ir_module = IRModule(funcs={func.name: func}, task=task)
-    return fuse_and_pack(ir_module, func, task)
+    return ir_module
 
 
 def cuda_schedule_reduce_by_default(task: ReduceTask) -> IRModule:
     x, y = task.inputs[0], task.outputs[0]
 
     shape: List[int] = x.const_shape()
     dims = task.dims
@@ -119,15 +118,15 @@
     block_size = 256
     remain_layout = TaskMapping.row_major(remain_shape)
     reduce_layout = TaskMapping.full_layout(reduce_shape)
 
     grid_size = (remain_layout.num_workers + block_size - 1) // block_size
 
     x_dtype = task.inputs[0].ttype.dtype
-    accumulate_dtype = task.attributes['accumulate_dtype']
+    accumulate_dtype = task.attrs['accumulate_dtype']
 
     with FunctionBuilder(
         name=task.name + '_grid', kind='cuda_kernel', grid_dim=grid_size, block_dim=block_size, label='reduce schedule'
     ) as fb:
         # params
         params = params_from_task(task)
         x, y = params
@@ -155,8 +154,8 @@
                 output_indices = merge_indices(remain_indices, reduce_indices, reduce_dims=task.dims)
             else:
                 output_indices = remain_indices
             fb += BufferStoreStmt(y, output_indices, cast(rv, x_dtype))
 
     func = fb.get()
     ir_module = IRModule(funcs={func.name: func}, task=task)
-    return fuse_and_pack(ir_module, func, task)
+    return ir_module
```

## hidet/graph/ops/schedules/cuda/softmax.py

```diff
@@ -17,15 +17,14 @@
 from hidet.ir.mapping import TaskMapping
 from hidet.ir.primitives import block_idx, thread_idx
 from hidet.ir import primitives as prim
 from hidet.ir.stmt import AssignStmt, BufferStoreStmt, DeclareStmt
 from hidet.ir.layout import row_layout, local_layout
 from hidet.graph.ops.definitions.softmax import SoftmaxTask
 from hidet.graph.ops.schedules.common import params_from_task
-from hidet.transforms.tools import fuse_and_pack
 from .common import warp_reduce
 
 
 def softmax_cuda_schedule(task: SoftmaxTask) -> IRModule:
     shape: List[int] = task.x_shape
     axis = task.axis
 
@@ -84,8 +83,8 @@
         for (r,) in block_layout.worker2task(thread_idx()):
             with sb.if_then(r < reduce_extent):
                 sb += BufferStoreStmt(y, other_indices[:axis] + (r,) + other_indices[axis:], buf[r] / rv)
 
         fb.set_body(sb.finish())
     func = fb.get()
     ir_module = IRModule(funcs={func.name: func}, task=task)
-    return fuse_and_pack(ir_module, func, task)
+    return ir_module
```

## hidet/graph/ops/schedules/cuda/matmul/mma.py

```diff
@@ -8,34 +8,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import contextlib
 from typing import List, Tuple, Union, Optional, Sequence, TypeVar
 
-import os
-
 import hidet.cuda
 from hidet import option
 from hidet.ir.builders import FunctionBuilder, StmtBuilder
 from hidet.ir.expr import Var, LogicalAnd, Equal, if_then_else, convert, Expr, tensor_var, cast, TensorSlice
 from hidet.ir.expr import tensor_pointer_var
 from hidet.ir.func import IRModule
 from hidet.ir.primitives import syncthreads, thread_idx, block_idx
 from hidet.ir.primitives.cuda.mma import MmaConfig, mma_sync
 from hidet.ir.mapping import row_spatial, row_repeat
 from hidet.ir.layout import row_layout, data_layout
 from hidet.ir.stmt import BufferStoreStmt, IfStmt, Stmt, DeclareStmt, DeclareScope
 from hidet.ir.type import DataType, data_type
 from hidet.utils import prod
 from hidet.graph.ops.definitions.matmul import BatchMatmulTask
-from hidet.graph.ops.schedules.resolve import resolve_ir_modules
 from hidet.graph.ops.schedules.common import params_from_task, Schedule, NotSupportedError
 from hidet.graph.ops.schedules.cuda.common import get_transfer_task_map
-from hidet.transforms.tools import fuse_and_pack
 
 T = TypeVar('T', bound=Tuple)
 
 
 def tuple_divide(lhs: T, rhs: T) -> T:
     assert len(lhs) == len(rhs) and all(a % b == 0 for a, b in zip(lhs, rhs))
     return tuple(a // b for a, b in zip(lhs, rhs))
@@ -109,15 +105,15 @@
     @staticmethod
     def schedules(task: BatchMatmulTask, space_level: int):
         # ta, tb = task.attributes['ta'], task.attributes['tb']
         ta, tb = False, False
         if ta or tb:
             raise NotImplementedError()
 
-        mma_type = task.attributes['mma']  # like 'wmma_f16_f32' or 'wmma'
+        mma_type = task.attrs['mma']  # like 'wmma_f16_f32' or 'wmma'
         if mma_type == 'mma':
             a, b, c = task.inputs[0], task.inputs[1], task.outputs[0]
             a_dtype, b_dtype, c_dtype = [t.type.dtype for t in [a, b, c]]
             mma_type = MatmulMmaSchedule.resolve_mma_type(a_dtype, b_dtype, c_dtype)
 
         assert mma_type.startswith('mma')
         if space_level == 0:
@@ -174,29 +170,29 @@
             ('mma_count', '{}x{}x{}'.format(self.mma_count_m, self.mma_count_n, self.mma_count_k)),
             ('threads', self.threads),
             ('smem_bytes', self.smem_storage_nbytes),
             ('registers', self.used_registers),
         ]
 
 
-def batched_matmul_cuda_schedule_mma(task: BatchMatmulTask, working_dir: str) -> IRModule:
+def batched_matmul_cuda_schedule_mma(task: BatchMatmulTask, working_dir: str) -> List[IRModule]:
     all_schedules = MatmulMmaSchedule.schedules(task, space_level=option.get_option('search_space'))
-    ir_modules = []
-    for sch in all_schedules:
-        ir_modules.append(batched_matmul_cuda_with_given_schedule(task, sch))
-
-    return resolve_ir_modules(
-        ir_modules=ir_modules,
-        schedules=all_schedules,
-        func_name=task.name,
-        target_device='cuda',
-        output_dir=os.path.join(working_dir, './resolve'),
-        parallel=True,
-        verbose=True,
-    )
+    return [batched_matmul_cuda_with_given_schedule(task, sch) for sch in all_schedules]
+    # ir_modules = []
+    # for sch in all_schedules:
+    #     ir_modules.append(batched_matmul_cuda_with_given_schedule(task, sch))
+    #
+    # return resolve_ir_modules(
+    #     ir_modules=ir_modules,
+    #     schedules=all_schedules,
+    #     target_device='cuda',
+    #     output_dir=os.path.join(working_dir, './resolve'),
+    #     parallel=True,
+    #     verbose=True,
+    # )
 
 
 def batched_matmul_cuda_with_given_schedule(task: BatchMatmulTask, sch: MatmulMmaSchedule) -> IRModule:
     m_size, n_size, k_size = task.m_size, task.n_size, task.k_size
     m_tile_size, n_tile_size, k_tile_size = sch.block_shape  # pylint: disable=unused-variable
     m_tiles = (m_size + m_tile_size - 1) // m_tile_size
     n_tiles = (n_size + n_tile_size - 1) // n_tile_size
@@ -325,15 +321,15 @@
                 m_size - block_offset_m,
                 n_size - block_offset_n,
                 sch,
             )
 
     func = fb.func
     ir_module = IRModule(funcs={func.name: func}, task=task)
-    return fuse_and_pack(ir_module, func, task)
+    return ir_module
 
 
 def load_regs_a(smem_a: Union[Var, TensorSlice], regs_a: Var, sch: MatmulMmaSchedule) -> Stmt:
     # smem_a: Tensor[block_m, block_k]
     # regs_a: Tensor[mma_count_m, mma_a_elements]
     # will copy the [0, warp_k] in block_k range
     sb = StmtBuilder()
```

## hidet/graph/ops/schedules/cuda/matmul/simt.py

```diff
@@ -41,31 +41,27 @@
     else k1 == block_k / warp_k - 1:
         regs[k1 % 2] -> acc regs
 sync
 write back
 """
 from typing import List, Tuple, Union, Optional
 
-import os
-
 import hidet.cuda
 from hidet import option
 from hidet.ir.builders import FunctionBuilder, StmtBuilder
 from hidet.ir.expr import Var, LogicalAnd, Equal, Cast, if_then_else, convert, Expr
 from hidet.ir.func import IRModule
 from hidet.ir.tools import simplify_to_int
 from hidet.ir.mapping import TaskMapping
 from hidet.ir.layout import DataLayout, StridesLayout
 from hidet.ir.primitives import syncthreads, thread_idx, block_idx
 from hidet.ir.stmt import BufferStoreStmt, IfStmt, DeclareStmt, DeclareScope
 from hidet.ir.type import data_type, tensor_type, PointerType, tensor_pointer_type
 from hidet.graph.ops.definitions.matmul import BatchMatmulTask
-from hidet.graph.ops.schedules.resolve import resolve_ir_modules
 from hidet.graph.ops.schedules.common import params_from_task, Schedule, NotSupportedError
-from hidet.transforms.tools import fuse_and_pack
 
 
 class MatmulSchedule(Schedule):
     def __init__(
         self,
         block_warps_k=8,
         warp_k=1,
@@ -302,29 +298,29 @@
                                 except NotSupportedError:
                                     pass
         else:
             raise NotImplementedError()
         return settings
 
 
-def batched_matmul_cuda_schedule_simt(task: BatchMatmulTask, working_dir: str) -> IRModule:
+def batched_matmul_cuda_schedule_simt(task: BatchMatmulTask, working_dir: str) -> List[IRModule]:
     all_schedules = MatmulSchedule.schedules(space_level=option.get_option('search_space'))
-    resolve_out_dir = os.path.join(working_dir, './resolve')
-    ir_modules = []
-    for schedule in all_schedules:
-        ir_modules.append(batched_matmul_cuda_with_given_schedule(task, schedule))
-    return resolve_ir_modules(
-        ir_modules=ir_modules,
-        schedules=all_schedules,
-        func_name=task.name,
-        target_device='cuda',
-        output_dir=resolve_out_dir,
-        parallel=True,
-        verbose=True,
-    )
+    # resolve_out_dir = os.path.join(working_dir, './resolve')
+    return [batched_matmul_cuda_with_given_schedule(task, schedule) for schedule in all_schedules]
+    # ir_modules = []
+    # for schedule in all_schedules:
+    #     ir_modules.append(batched_matmul_cuda_with_given_schedule(task, schedule))
+    # return resolve_ir_modules(
+    #     ir_modules=ir_modules,
+    #     schedules=all_schedules,
+    #     target_device='cuda',
+    #     output_dir=resolve_out_dir,
+    #     parallel=True,
+    #     verbose=True,
+    # )
 
 
 def batched_matmul_cuda_with_given_schedule(task: BatchMatmulTask, schedule: MatmulSchedule) -> IRModule:
     sch = schedule
 
     a_dtype = task.inputs[0].type.dtype
     b_dtype = task.inputs[1].type.dtype
@@ -468,15 +464,15 @@
                 dst_predicate=lambda i, j: LogicalAnd(block_offset[0] + i < m_size, block_offset[1] + j < n_size),
             )
         # set body
         fb.set_body(sb.finish())
 
     func = fb.get()
     ir_module = IRModule(funcs={func.name: func}, task=task)
-    return fuse_and_pack(ir_module, func, task)
+    return ir_module
 
 
 def init(dst, init_value, layout):
     sb = StmtBuilder()
     for indices in layout(thread_idx()):
         sb += BufferStoreStmt(dst, indices, init_value)
     return sb.finish()
```

## hidet/graph/ops/schedules/cuda/matmul/wmma.py

```diff
@@ -5,15 +5,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
 from typing import List, Tuple, Union, Optional
 
 import hidet.cuda
 from hidet import option
 from hidet.ir.builders import FunctionBuilder, StmtBuilder
 from hidet.ir.expr import Var, LogicalAnd, Cast, if_then_else, convert, Expr, cast
 from hidet.ir.func import IRModule
@@ -24,17 +23,15 @@
 from hidet.ir.primitives.cuda.wmma import WmmaConfig, wmma_load_a, wmma_load_b, wmma_mma, wmma_store, wmma_configs
 from hidet.ir.stmt import BufferStoreStmt, IfStmt, DeclareStmt, DeclareScope
 from hidet.ir.task import Task
 from hidet.ir.type import data_type, tensor_type, PointerType, tensor_pointer_type
 from hidet.graph.ops.definitions.matmul import BatchMatmulTask
 from hidet.graph.ops.schedules.common import params_from_task, Schedule, NotSupportedError
 from hidet.graph.ops.schedules.cuda.common import get_task_map, get_transfer_task_map
-from hidet.graph.ops.schedules.resolve import resolve_ir_modules
 from hidet.utils import prod
-from hidet.transforms.tools import fuse_and_pack
 
 
 def shape_prod(a_shape: List[int], b_shape: List[int]) -> List[int]:
     assert len(a_shape) == len(b_shape)
     return [a * b for a, b in zip(a_shape, b_shape)]
 
 
@@ -159,15 +156,15 @@
 
     def check(self, cond, msg: str = ""):
         if not cond:
             raise NotSupportedError(self, msg)
 
     @staticmethod
     def schedules(task: Task, space_level: int = 0):
-        wmma_type = task.attributes['mma']  # like 'wmma_f16_f32' or 'wmma'
+        wmma_type = task.attrs['mma']  # like 'wmma_f16_f32' or 'wmma'
 
         # choose a specific wmma type when needed
         if wmma_type == 'wmma':
             dtype_rank = {'float16': 0, 'bfloat16': 1, 'tfloat32': 2, 'float32': 4}
             a_dtype = task.inputs[0].type.dtype.name
             b_dtype = task.inputs[1].type.dtype.name
             c_dtype = task.outputs[0].type.dtype.name
@@ -228,28 +225,28 @@
             if len(ret) == 0:
                 raise ValueError('Can not find schedule for task: \n{}'.format(task))
             return ret
         else:
             raise ValueError('Space level {} must in [0, 1, 2].'.format(space_level))
 
 
-def batched_matmul_cuda_schedule_wmma(task: BatchMatmulTask, working_dir: str) -> IRModule:
+def batched_matmul_cuda_schedule_wmma(task: BatchMatmulTask, working_dir: str) -> List[IRModule]:
     all_schedules = MatmulSchedule.schedules(task, space_level=option.get_option('search_space'))
-    ir_modules = []
-    for schedule in all_schedules:
-        ir_modules.append(batched_matmul_cuda_with_given_schedule(task, schedule))
-    return resolve_ir_modules(
-        ir_modules=ir_modules,
-        schedules=all_schedules,
-        func_name=task.name,
-        target_device='cuda',
-        output_dir=os.path.join(working_dir, './resolve'),
-        parallel=True,
-        verbose=True,
-    )
+    return [batched_matmul_cuda_with_given_schedule(task, schedule) for schedule in all_schedules]
+    # ir_modules = []
+    # for schedule in all_schedules:
+    #     ir_modules.append(batched_matmul_cuda_with_given_schedule(task, schedule))
+    # return resolve_ir_modules(
+    #     ir_modules=ir_modules,
+    #     schedules=all_schedules,
+    #     target_device='cuda',
+    #     output_dir=os.path.join(working_dir, './resolve'),
+    #     parallel=True,
+    #     verbose=True,
+    # )
 
 
 def batched_matmul_cuda_with_given_schedule(task: BatchMatmulTask, schedule: MatmulSchedule) -> IRModule:
     ir_module = IRModule(task=task)
     sch = schedule
 
     dtype_short2long = {'f16': 'float16', 'bf16': 'bfloat16', 'tf32': 'tfloat32', 'f32': 'float32'}
@@ -422,15 +419,15 @@
                         block_offset[0] + offset_x + i < m_size, block_offset[1] + offset_y + j < n_size
                     ),
                     worker_idx=thread_idx() % warp_size,
                 )
 
     func = fb.get()
     ir_module = IRModule(funcs={func.name: func}, task=task)
-    return fuse_and_pack(ir_module, func, task)
+    return ir_module
 
 
 def init(dst, init_value, sch):
     sb = StmtBuilder()
     warp_idx = thread_idx() / 32
     for indices in sch.warp_map(warp_idx):
         for i in range(sch.wmma_config.c_regs):
```

## hidet/graph/transforms/base.py

```diff
@@ -69,14 +69,17 @@
         self.configs: Dict[str, Any] = {
             # target precision:
             # [None, 'float16', 'bfloat16', 'float32']
             'precision': None,
             # target reduce precision:
             # [None, 'float16', 'float32']
             'reduce_precision': None,
+            # use attention or not
+            # [True, False]
+            'use_attention': False,
             # mma primitive:
             # ['simt', 'wmma', 'mma']
             'mma': 'simt',
             # parallel k
             # ['default', 'disabled', 'search', 2, 4, ...]
             'parallel_k': 'default',
             # print lower details
@@ -84,14 +87,17 @@
         }
 
     def __enter__(self) -> PassContext:
         self._stack.append(self)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        from ..transforms.graph_patterns import deregister_attn_patterns
+
+        deregister_attn_patterns()
         popped = self._stack.pop()
         assert popped == self
 
     @classmethod
     def current(cls):
         """
         Get the current pass context.
@@ -144,14 +150,28 @@
               Use 'float16' to accumulate. Only valid when set_precision('float16') has been used.
             - 'float32'
               Use 'float32' to accumulate.
         """
         self.configs['reduce_precision'] = dtype
         return self
 
+    def set_use_attention(self, flag=False) -> PassContext:
+        """
+        Set to use fused attention schedule
+
+        """
+        from ..transforms.graph_patterns import register_attn_patterns, deregister_attn_patterns
+
+        self.configs['use_attention'] = flag
+        if flag:
+            register_attn_patterns()
+        else:
+            deregister_attn_patterns()
+        return self
+
     def set_verbose(self) -> PassContext:
         """
         Allow each graph level passes to print detailed information related to its lowering and optimization.
         """
         self.configs['verbose'] = True
         return self
```

## hidet/graph/transforms/fuse_operator.py

```diff
@@ -5,18 +5,17 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List, Sequence, Dict, Tuple, Optional, Set
-import copy
-from hidet.ir.task import Task, TaskGraph, TensorNode
-from hidet.graph.ops.definitions.utils import input_like
+from typing import List, Sequence, Dict, Tuple, Optional, Set, Union
+
+import hidet
 from hidet.graph.ir import FlowGraph, Operator, Tensor
 from hidet.graph.ops.definitions.special import BarrierOp
 from hidet.graph.ir.functors import analyze_usage
 from hidet.graph.transforms.base import GraphPass
 from hidet.utils.structure import DirectedGraph
 from hidet.utils.doc import Doc, Text, NewLine, doc_join
 from hidet.utils.namer import Namer
@@ -39,14 +38,34 @@
             output_doc = doc_join([namer(t) for t in op.outputs], ', ')
             input_doc = doc_join([namer(t) for t in op.inputs], ', ')
             body += NewLine() + output_doc + ' = ' + op.name + '(' + input_doc + ')'
         body += NewLine() + 'return ' + doc_join([namer(t) for t in self.output_tensors], ', ')
         tail = NewLine() + '}'
         return str(head + body.indent() + tail)
 
+    def flow_graph_and_anchor(self) -> Tuple[FlowGraph, int]:
+        from hidet.graph import symbol_like
+
+        graph_inputs: List[Tensor] = [symbol_like(x) for x in self.input_tensors]
+        remap: Dict[Tensor, Tensor] = {x: y for x, y in zip(self.input_tensors, graph_inputs)}
+        updated_anchor: Optional[Operator] = None
+        for op in self.operators:
+            inputs = [remap[x] for x in op.inputs]
+            outputs = op.reforward(inputs)
+            if op is self.anchor:
+                updated_anchor = outputs[0].op
+            for x, y in zip(op.outputs, outputs):
+                remap[x] = y
+        graph_outputs = [remap[x] for x in self.output_tensors]
+        flow_graph = hidet.trace_from(graph_outputs, graph_inputs)
+
+        assert updated_anchor is not None
+        anchor_idx = flow_graph.nodes.index(updated_anchor)
+        return flow_graph, anchor_idx
+
 
 Usage = Dict[Tensor, List[Tuple[Operator, int]]]
 
 
 def fuse_epilogue_operators(anchors: Sequence[Operator], usage: Usage, belong: Dict[Operator, FusibleGraph]):
     for anchor in anchors:
         if not anchor.task.allow_epilogue():
@@ -218,15 +237,15 @@
         # some pass will invalidate the cache, so we need to re-trace the graph.
         graph.update_nodes()
 
     belong: Dict[Operator, FusibleGraph] = {}
 
     # first, we find all non-injective operators as the anchor operators,
     # and create a sub-graph for each such operator.
-    anchors: List[Operator] = [op for op in graph.nodes if not op.task.is_injective_task()]
+    anchors: List[Operator] = [op for op in graph.nodes if not op.task.is_injective()]
     for anchor in anchors:
         belong[anchor] = FusibleGraph(anchor)
 
     # fuse epilogue operators.
     fuse_epilogue_operators(anchors, usage, belong)
 
     # fuse prologue operators.
@@ -247,86 +266,96 @@
 
     # sanity check that it is a partition
     sanity_check_partition(graph, partition, belong)
 
     return partition
 
 
-def task_from_sub_graph(sub_graph: FusibleGraph, usage: Usage) -> Task:
-    mapping: Dict[Tensor, TensorNode] = {}
-    task_graph_inputs: List[TensorNode] = []
-    for tensor in sub_graph.input_tensors:
-        user, idx = usage[tensor][0]
-        # Because the name is just a hint, we can choose one we like.
-        if user is None:
-            # this tensor is also a graph output.
-            name = 'out'
-        else:
-            # we use the name from one of its user task.
-            name = user.task.inputs[idx].name
-        task_graph_inputs.append(input_like(tensor, name))
-        mapping[tensor] = task_graph_inputs[-1]
-
-    nodes: List[Task] = []
-    consume: Dict[TensorNode, TensorNode] = {}
-    for op in sub_graph.operators:
-        task = op.task
-        nodes.append(task)
-        num_inputs, num_outputs = len(op.inputs), len(op.outputs)
-        for i in range(num_inputs):
-            consume[task.inputs[i]] = mapping[op.inputs[i]]
-        for i in range(num_outputs):
-            mapping[op.outputs[i]] = task.outputs[i]
-    task_graph_outputs: List[TensorNode] = [mapping[tensor] for tensor in sub_graph.output_tensors]
-
-    anchor_task = copy.copy(sub_graph.anchor.task)
-    nodes[nodes.index(sub_graph.anchor.task)] = anchor_task
-    task_graph = TaskGraph(
-        anchor=anchor_task,
-        nodes=nodes,
-        consume=consume,
-        input_tensors=task_graph_inputs,
-        output_tensors=task_graph_outputs,
-    )
-
-    anchor_task.task_graph = task_graph
-
-    return anchor_task
-
-
+# def task_from_sub_graph(sub_graph: FusibleGraph, usage: Usage) -> Task:
+#     mapping: Dict[Tensor, TensorNode] = {}
+#     task_graph_inputs: List[TensorNode] = []
+#     for tensor in sub_graph.input_tensors:
+#         user, idx = usage[tensor][0]
+#         # Because the name is just a hint, we can choose one we like.
+#         if user is None:
+#             # this tensor is also a graph output.
+#             name = 'out'
+#         else:
+#             # we use the name from one of its user task.
+#             name = user.task.inputs[idx].name
+#         task_graph_inputs.append(input_like(tensor, name))
+#         mapping[tensor] = task_graph_inputs[-1]
+#
+#     nodes: List[Task] = []
+#     consume: Dict[TensorNode, TensorNode] = {}
+#     for op in sub_graph.operators:
+#         task = op.task
+#         nodes.append(task)
+#         num_inputs, num_outputs = len(op.inputs), len(op.outputs)
+#         for i in range(num_inputs):
+#             consume[task.inputs[i]] = mapping[op.inputs[i]]
+#         for i in range(num_outputs):
+#             mapping[op.outputs[i]] = task.outputs[i]
+#     task_graph_outputs: List[TensorNode] = [mapping[tensor] for tensor in sub_graph.output_tensors]
+#
+#     anchor_task = copy.copy(sub_graph.anchor.task)
+#     nodes[nodes.index(sub_graph.anchor.task)] = anchor_task
+#     task_graph = TaskGraph(
+#         anchor=anchor_task,
+#         nodes=nodes,
+#         consume=consume,
+#         input_tensors=task_graph_inputs,
+#         output_tensors=task_graph_outputs,
+#     )
+#
+#     anchor_task.task_graph = task_graph
+#
+#     return anchor_task
+#
+#
 def operator_from_sub_graph(sub_graph: FusibleGraph, input_remap: Dict[Tensor, Tensor], usage: Usage) -> Operator:
     if len(sub_graph.operators) == 1:
         # if there is only one operator in the sub-graph, we just update its inputs.
         origin_op = sub_graph.operators[0]
         updated_inputs: List[Tensor] = [
             input_remap[tensor] if tensor in input_remap else tensor for tensor in origin_op.inputs
         ]
         if origin_op.__class__ is Operator:
             raise ValueError(
                 'Found an fused operator in the fusion pass.\n'
                 'For now, this pass expects to accept a graph without fused operators.\n'
                 'Have you run this pass twice?'
             )
-        outs = origin_op.reforward(updated_inputs)
+        outs: List[Tensor] = origin_op.reforward(updated_inputs)
         updated_op = outs[0].trace[0]
         return updated_op
     else:
         # otherwise, create a new operator from the sub-graph.
+        # updated_inputs: List[Tensor] = [
+        #     input_remap[tensor] if tensor in input_remap else tensor for tensor in sub_graph.input_tensors
+        # ]
+        # task: Task = task_from_sub_graph(sub_graph, usage)
+        # op = Operator(
+        #     inputs=updated_inputs,
+        #     task=task,
+        #     name='Fused' + sub_graph.anchor.name,
+        #     attributes={**sub_graph.anchor.attrs, 'fusion': ' '.join([op.name for op in sub_graph.operators])},
+        # )
+        # op.outputs = op.run()
+        # return op
+        from hidet.graph.ops.definitions.fusion.fused_operator import fused_operator
+
+        fused_graph, anchor = sub_graph.flow_graph_and_anchor()
         updated_inputs: List[Tensor] = [
             input_remap[tensor] if tensor in input_remap else tensor for tensor in sub_graph.input_tensors
         ]
-        task: Task = task_from_sub_graph(sub_graph, usage)
-        op = Operator(
-            inputs=updated_inputs,
-            task=task,
-            name='Fused' + sub_graph.anchor.name,
-            attributes={**sub_graph.anchor.attrs, 'fusion': ' '.join([op.name for op in sub_graph.operators])},
-        )
-        op.outputs = op.run()
-        return op
+        outs: Union[List[Tensor], Tensor] = fused_operator(*updated_inputs, fused_graph=fused_graph, anchor=anchor)
+        if isinstance(outs, Tensor):
+            outs = [outs]
+        return outs[0].trace[0]
 
 
 def construct_fused_graph(graph: FlowGraph, sub_graphs: Sequence[FusibleGraph], usage: Usage) -> FlowGraph:
     graph_input_tensors: List[Tensor] = graph.inputs
     graph_nodes: List[Operator] = []
     input_remap: Dict[Tensor, Tensor] = {}
 
@@ -340,12 +369,14 @@
     return FlowGraph(graph_output_tensors, inputs=graph_input_tensors, nodes=graph_nodes)
 
 
 class FuseOperatorPass(GraphPass):
     def process_graph(self, graph: FlowGraph) -> FlowGraph:
         usage: Usage = analyze_usage(graph)
         partition: List[FusibleGraph] = partition_graph(graph, usage)
-        return construct_fused_graph(graph, partition, usage)
+        fused_graph = construct_fused_graph(graph, partition, usage)
+        fused_graph.update_nodes()
+        return fused_graph
 
 
 def fuse_operator_pass() -> GraphPass:
     return FuseOperatorPass()
```

## hidet/graph/transforms/graph_patterns/__init__.py

```diff
@@ -6,12 +6,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from .base import TensorPattern, OperatorPattern, SubgraphRewriteRule, MatchDict, Usage, graph_pattern_match
-from .base import register_rewrite_rule, op_pattern, registered_rewrite_rules
+from .base import register_rewrite_rule, op_pattern, registered_rewrite_rules, deregister_rewrite_rule
 from .arithmetic_patterns import arithmetic_patterns
 from .transform_patterns import transform_patterns
+from .attn_patterns import attn_patterns, register_attn_patterns, deregister_attn_patterns
 from .conv2d_patterns import conv2d_patterns
 from .matmul_patterns import matmul_patterns
```

## hidet/graph/transforms/graph_patterns/base.py

```diff
@@ -303,7 +303,23 @@
         registered_rewrite_rules.append(rule)
         return None
     elif issubclass(rule, SubgraphRewriteRule):
         registered_rewrite_rules.append(rule())
         return rule
     else:
         raise TypeError('rule should be a SubgraphRewriteRule or a subclass of SubgraphRewriteRule')
+
+
+def deregister_rewrite_rule(rule: SubgraphRewriteRule):
+    """
+    Remove a sub-graph rewrite rule from list of currently registered rules
+
+    Parameters
+    ----------
+    rule: SubgraphRewriteRule
+        The rule to be deregistered.
+    """
+    if isinstance(rule, SubgraphRewriteRule):
+        registered_rewrite_rules.remove(rule)
+        return None
+    else:
+        raise TypeError('rule should be a SubgraphRewriteRule')
```

## hidet/ir/__init__.py

```diff
@@ -31,15 +31,16 @@
 from .expr import var, scalar_var, tensor_var, is_one, is_zero, convert
 
 from .layout import DataLayout
 
 from .mapping import TaskMapping
 
 from .stmt import Stmt, DeclareStmt, EvaluateStmt, BufferStoreStmt, AssignStmt, ForStmt, IfStmt, AssertStmt, SeqStmt
-from .stmt import LetStmt, ForTaskStmt, ReturnStmt, WhileStmt, BreakStmt, ContinueStmt
+from .stmt import LetStmt, ForMappingStmt, ReturnStmt, WhileStmt, BreakStmt, ContinueStmt
+from .stmt import ForStmtAttr
 
 from .compute import TensorNode, ScalarNode
 
 from .builders import FunctionBuilder, StmtBuilder
 
 from .task import Task, save_task, load_task
```

## hidet/ir/layout.py

```diff
@@ -129,38 +129,38 @@
         assert len(args) == len(self.shape)
         var2value = OrderedDict()
         arg_vars = variablize(args, var2value)
         cond = self.global2cond(*arg_vars)
         cond = concat_let_expr(var2value=var2value, body=cond)
         return cond
 
-    def tile(self, inner_shape: Sequence[Int]):
-        return TiledDataLayout(base=self, inner_shape=inner_shape)
+    # def tile(self, inner_shape: Sequence[Int]):
+    #     return TiledDataLayout(base=self, inner_shape=inner_shape)
 
-    def split(self, dim2factor: Mapping[int, Int]):
-        return SplitDataLayout(base=self, dim2factor=dim2factor)
+    # def split(self, dim2factor: Mapping[int, Int]):
+    #     return SplitDataLayout(base=self, dim2factor=dim2factor)
 
-    def reorder(self, order: Sequence[int]):
-        return self.fuse(order)
+    # def reorder(self, order: Sequence[int]):
+    #     return self.fuse(order)
 
     def swizzle(self, dim: int, regards_dim: Optional[int] = None, log_step: int = 0):
-        return SwizzleDataLayout(base=self, dim=dim, regards_dim=regards_dim, log_step=log_step)
+        return SwizzleLayout(base=self, dim=dim, regards_dim=regards_dim, log_step=log_step)
 
-    def fuse(self, dim2fuse: Sequence[Union[Sequence[int], int]]):
-        return FusedDataLayout(base=self, dim2fuse=dim2fuse)
+    # def fuse(self, dim2fuse: Sequence[Union[Sequence[int], int]]):
+    #     return FusedDataLayout(base=self, dim2fuse=dim2fuse)
 
     @staticmethod
     def product(outer, inner):
-        return ProductDataLayout(outer, inner)
+        return ComposedLayout(outer, inner)
 
     @staticmethod
     def concat(lhs, rhs):
         lhs = to_data_layout(lhs)
         rhs = to_data_layout(rhs)
-        return ConcatDataLayout(lhs, rhs)
+        return ConcatLayout(lhs, rhs)
 
     @staticmethod
     def local(shape: Sequence[Int]):
         return LocalLayout(shape=shape)
 
     @staticmethod
     def row_major(shape: Sequence[Int]):
@@ -229,15 +229,15 @@
 
     def global2cond(self, *args: Int) -> Bool:
         from hidet.ir.expr import LogicalAnd
 
         return LogicalAnd.join_list([v < s for s, v in zip(self.shape, args)])
 
 
-class SwizzleDataLayout(DataLayout):
+class SwizzleLayout(DataLayout):
     """
     Swizzle a layout (called base layout) to get a swizzled data layout. The shape of swizzled layout is the same as
     the base layout.
 
     Example:
         A 2-dimension tensor with shape [a, b] where a = 2^m for some m and b <= a,
         After swizzle(plan={0: [1]}), we get a data layout with shape [a, b], and
@@ -392,15 +392,15 @@
     def global2local(self, *args: Int) -> Int:
         return self.base(*self.base_args(*args))
 
     def global2cond(self, *args: Int) -> Bool:
         return self.base.within_bound(*self.base_args(*args))
 
 
-class ProductDataLayout(DataLayout):
+class ComposedLayout(DataLayout):
     def __init__(self, outer: DataLayout, inner: DataLayout):
         assert len(outer.shape) == len(inner.shape)
         super().__init__(shape=[a * b for a, b in zip(outer.shape, inner.shape)], size=outer.size * inner.size)
         self.outer = outer
         self.inner = inner
 
     def global2local(self, *args: Int) -> Int:
@@ -412,15 +412,15 @@
         from hidet.ir.expr import LogicalAnd
 
         outer_args = [v // b for v, b in zip(args, self.inner.shape)]
         inner_args = [v % b for v, b in zip(args, self.inner.shape)]
         return LogicalAnd(self.outer.within_bound(*outer_args), self.inner.within_bound(*inner_args))
 
 
-class ConcatDataLayout(DataLayout):
+class ConcatLayout(DataLayout):
     def __init__(self, lhs: DataLayout, rhs: DataLayout):
         super().__init__(shape=list(lhs.shape) + list(rhs.shape), size=lhs.size * rhs.size)
         self.lhs = lhs
         self.rhs = rhs
 
     def global2local(self, *args: Int) -> Int:
         lhs_args = args[: len(self.lhs.shape)]
```

## hidet/ir/mapping.py

```diff
@@ -7,92 +7,77 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # pylint: disable=import-outside-toplevel
 from __future__ import annotations
-from typing import Union, Tuple, List, Optional, Sequence, Callable, Mapping
+from typing import Union, Tuple, List, Optional, Sequence, Callable, Dict
 import itertools
-import numpy as np
 from hidet.ir.node import Node
+from hidet.ir.expr import Expr, convert
 from hidet.utils import prod, gcd
 
-Int = Union['Expr', int]
+Int = Union[Expr, int]
 
 
 def is_atom(expr):
     from hidet.ir import Constant, Var
 
     return isinstance(expr, (Constant, Var))
 
 
 def var(hint):
     from hidet import ir
 
     return ir.var(hint)
 
 
-def strides_from_ranks(shape: Sequence[int], ranks: Sequence[int]) -> List[int]:
-    if any(v < 0 for v in shape):
+def strides_from_ranks(shape: Sequence[Int], ranks: Sequence[int]) -> List[Int]:
+    if any(isinstance(v, int) and v < 0 for v in shape):
         raise ValueError('Shape must be non-negative, got {}'.format(shape))
     if len(set(ranks)) != len(ranks):
         raise ValueError('Duplicated ranks: {}'.format(ranks))
-    if any(v < 0 or v >= len(shape) for v in ranks):
+    if any(isinstance(v, int) and v < 0 or v >= len(shape) for v in ranks):
         raise ValueError('Ranks {} out of bound for shape {}'.format(ranks, shape))
     if len(ranks) != len(shape):
         raise ValueError('Ranks must have the same length as shape, got shape {} and ranks {}'.format(shape, ranks))
-    strides: List[Optional[int]] = [None] * len(shape)
+    strides: List[Optional[Int]] = [None] * len(shape)
     acc = 1
     for i in reversed(range(len(shape))):
         dim = ranks.index(i)
         strides[dim] = acc
-        acc *= shape[dim]
+        acc = acc * shape[dim]
     return strides
 
 
 class TaskMapping(Node):
     registered = []
 
     def __init__(
         self,
-        num_workers: int = None,
-        task_shape: Tuple[int, ...] = None,
+        num_workers: Int = None,
+        task_shape: Tuple[Int, ...] = None,
         worker2task: Optional[Callable[[Int], List[Tuple[Int, ...]]]] = None,
     ):
-        from hidet.ir import Expr
-        from hidet.ir.tools import simplify_to_int
+        from hidet.ir.tools import simplify
 
-        if isinstance(num_workers, Expr):
-            num_workers = simplify_to_int(num_workers)
-        task_shape = tuple(simplify_to_int(v) for v in task_shape)
-        self.num_workers: int = num_workers
-        self.task_shape: Tuple[int, ...] = task_shape
+        self.num_workers: Int = simplify(num_workers)
+        self.task_shape: Tuple[Int, ...] = tuple(simplify(v) for v in task_shape)
         self.worker2task: Callable[[Int], List[Tuple[Int]]] = worker2task
-        if num_workers is not None:
-            assert isinstance(num_workers, int)
-        if task_shape is not None:
-            assert all(isinstance(s, int) for s in task_shape)
 
     def __call__(self, w: Int) -> List[Tuple[Int, ...]]:
         return self.worker2task(w)
 
-    def __mul__(self, other) -> 'TaskMapping':
+    def __mul__(self, other) -> TaskMapping:
         return ComposedTaskMapping(outer=self, inner=other)
 
     def __getitem__(self, w: Int) -> List[Tuple[Int, ...]]:
         return self.worker2task(w)
 
-    def __str__(self):
-        worker_id = np.empty(shape=self.task_shape, dtype=np.int32)
-        for w in range(self.num_workers):
-            for task_indices in self.worker2task(w):
-                worker_id[task_indices] = w
-        return np.array2string(worker_id)
-
     def on(self, w: Int) -> List[Tuple[Int, ...]]:
         return self.worker2task(w)
 
     def map(self, w: Int) -> Tuple[Int, ...]:
         return self.single_task_of(w)
 
     def single_task_of(self, w: Int) -> Tuple[Int, ...]:
@@ -107,226 +92,262 @@
 
     @staticmethod
     def column_major(task_shape: Sequence[int]):
         return SpatialTaskMapping(task_shape, ranks=list(reversed(range(len(task_shape)))))
 
     @staticmethod
     def full_layout(task_shape: Sequence[int]):
-        return RepeatTaskMapping(task_shape, ranks=list(range(len(task_shape))))
+        return row_repeat(*task_shape)
 
-    def projection(self, dim2value: Mapping[int, Int]) -> 'TaskMapping':
+    def projection(self, dim2value: Dict[int, Int]) -> TaskMapping:
         return ProjectedTaskMapping(base=self, dim2value=dim2value)
 
     # chain api
     def spatial(self, *task_shape, ranks: List[int] = None) -> TaskMapping:
         return self * spatial_map(task_shape, ranks)
 
     def repeat(self, *task_shape, ranks: List[int] = None) -> TaskMapping:
         return self * repeat_map(task_shape, ranks)
 
 
 class RepeatTaskMapping(TaskMapping):
-    def __init__(self, task_shape: Sequence[int], ranks: Optional[Sequence[int]]):
-        if ranks is None:
-            ranks = list(range(len(task_shape)))
-        self.ranks: List[int] = list(ranks)
-        self.strides: List[int] = strides_from_ranks(task_shape, ranks)
+    def __init__(self, task_shape: Sequence[Int], ranks: Sequence[int], attrs):
+        from hidet.ir.stmt import ForStmtAttr
+        from hidet.ir.tools import simplify
+
         super().__init__(num_workers=1, task_shape=tuple(task_shape), worker2task=self._worker2task)
+        self.ranks: List[int] = list(ranks)
+        self.strides: List[Int] = [simplify(v) for v in strides_from_ranks(task_shape, ranks)]
+        self.attrs: List[ForStmtAttr] = list(attrs)
 
     # noinspection PyUnusedLocal
     def _worker2task(self, w: Int) -> List[Tuple[Int]]:  # pylint: disable=unused-argument
-        def key_func(task: Tuple[int]) -> int:
+        def key_func(task: Tuple[Int, ...]) -> Int:
             global_index = sum(a * b for a, b in zip(task, self.strides))
             return global_index
 
         ranges = [range(s) for s in self.task_shape]
         tasks = list(tuple(task) for task in itertools.product(*ranges))
         return list(sorted(tasks, key=key_func))
 
 
 class SpatialTaskMapping(TaskMapping):
     def __init__(self, task_shape: Sequence[int], ranks: Sequence[int]):
-        assert len(task_shape) == len(ranks)
+        from hidet.ir.tools import simplify
+
         super().__init__(num_workers=prod(task_shape), task_shape=tuple(task_shape), worker2task=self._worker2task)
-        self.ranks = list(ranks)
-        self.strides = strides_from_ranks(task_shape, ranks)
+        self.ranks: List[int] = list(ranks)
+        self.strides: List[Int] = [simplify(v) for v in strides_from_ranks(task_shape, ranks)]
 
-    def _worker2task(self, w: Int) -> List[Tuple[Int]]:
+        assert len(task_shape) == len(ranks)
+
+    def _worker2task(self, w: Int) -> List[Tuple[Int, ...]]:
         task = []
         for mod, b in zip(self.task_shape, self.strides):
             task.append((w // b) % mod)
         return [tuple(task)]
 
 
 class ProjectedTaskMapping(TaskMapping):
-    def __init__(self, base: TaskMapping, dim2value: Mapping[int, Int]):
+    def __init__(self, base: TaskMapping, dim2value: Dict[int, Int]):
         assert all(int(v) == 0 for v in dim2value.values())
         task_shape = tuple(base.task_shape[i] if i not in dim2value else 1 for i in range(len(base.task_shape)))
         super().__init__(num_workers=base.num_workers, task_shape=task_shape, worker2task=self._worker2task)
         self.base = base
-        self.dim2value = dim2value
+        self.dim2value: Dict[int, Int] = dim2value
 
-    def _worker2task(self, w: Int) -> List[Tuple[Int]]:
+    def _worker2task(self, w: Int) -> List[Tuple[Int, ...]]:
         rank = len(self.task_shape)
         projected_tasks = []
         for task in self.base(w):
             projected_tasks.append(tuple(self.dim2value[i] if i in self.dim2value else task[i] for i in range(rank)))
         return projected_tasks
 
 
 class ComposedTaskMapping(TaskMapping):
     def __init__(self, outer: TaskMapping, inner: TaskMapping):
-        assert len(outer.task_shape) == len(inner.task_shape)
         super().__init__(
             num_workers=outer.num_workers * inner.num_workers,
             task_shape=tuple(a * b for a, b in zip(outer.task_shape, inner.task_shape)),
             worker2task=self._worker2task,
         )
-        self.outer = outer
-        self.inner = inner
+        self.outer: TaskMapping = outer
+        self.inner: TaskMapping = inner
+
+        assert len(outer.task_shape) == len(inner.task_shape)
 
     def _worker2task(self, worker_index: Int) -> List[Tuple[Int, ...]]:
         outer_worker_index = worker_index // self.inner.num_workers
         inner_worker_index = worker_index % self.inner.num_workers
         outer_tasks = self.outer.worker2task(outer_worker_index)
         inner_tasks = self.inner.worker2task(inner_worker_index)
         tasks = []
         for outer_task in outer_tasks:
             for inner_task in inner_tasks:
                 task = tuple(a * self.inner.task_shape[i] + b for i, (a, b) in enumerate(zip(outer_task, inner_task)))
                 tasks.append(task)
         return tasks
 
 
-class TaskMappingExpander:
-    def __init__(self):
-        from hidet.ir.stmt import ForStmt, LetStmt
-
-        self.stmts: List[Union[LetStmt, ForStmt]] = []
+def spatial_map(task_shape: Sequence[Int], ranks: Optional[Sequence[int]] = None):
+    from hidet.ir.tools import simplify
 
-    def variablize(self, e):
-        from hidet.ir import LetStmt
-
-        if is_atom(e):
-            return e
-        else:
-            v = var('p')
-            self.stmts.append(LetStmt(v, e))
-            return v
-
-    def expand(self, w: Int, task_layout: TaskMapping) -> List[Sequence[Int]]:
-        vtable = {
-            RepeatTaskMapping: self.expand_full,
-            SpatialTaskMapping: self.expand_grid,
-            ComposedTaskMapping: self.expand_composed,
-            ProjectedTaskMapping: self.expand_projected,
-            TaskMapping: self.expand_atom,
-        }
-        w = self.variablize(w)
-        # noinspection PyArgumentList
-        return vtable[task_layout.__class__](w, task_layout)
-
-    def expand_composed(self, w: Int, layout: ComposedTaskMapping):
-        outer_w = self.variablize(w // layout.inner.num_workers)
-        inner_w = self.variablize(w % layout.inner.num_workers)
-        outer_fields = self.expand(outer_w, layout.outer)
-        inner_fields = self.expand(inner_w, layout.inner)
-        fields = []
-        for outer_field in outer_fields:
-            scaled_outer_field = [self.variablize(a * b) for a, b in zip(outer_field, layout.inner.task_shape)]
-            for inner_field in inner_fields:
-                fields.append(tuple(a + b for a, b in zip(scaled_outer_field, inner_field)))
-        return fields
-
-    def expand_projected(self, w: Int, layout: ProjectedTaskMapping):
-        rank = len(layout.task_shape)
-        base_fields = self.expand(w, layout.base)
-        projected_fields = []
-        for field in base_fields:
-            projected_fields.append(
-                tuple(layout.dim2value[i] if i in layout.dim2value else field[i] for i in range(rank))
-            )
-        return projected_fields
-
-    def expand_grid(self, w: Int, layout: SpatialTaskMapping):
-        return [[self.variablize(v) for v in layout(w)[0]]]
-
-    def expand_full(self, w: Int, layout: RepeatTaskMapping):
-        unroll_limit = 1024
-        if prod(layout.task_shape) < unroll_limit:
-            # unroll automatically
-            return layout(w)
-        else:
-            # do not expand, use for loop
-            from hidet.ir import ForStmt
-
-            shape = layout.task_shape
-            axes = []
-            for i, s in enumerate(shape):
-                axis = var(chr(ord('i') + i))
-                self.stmts.append(ForStmt(loop_var=axis, extent=s))
-                axes.append(axis)
-            return [axes]
-
-    @staticmethod
-    def expand_atom(w: Int, layout: TaskMapping):
-        return layout(w)
-
-
-def spatial_map(task_shape: Sequence[int], ranks: Optional[Sequence[int]] = None):
-    from hidet.ir.tools import simplify_to_int
-
-    task_shape = [simplify_to_int(v) for v in task_shape]
+    task_shape = [simplify(v) for v in task_shape]
     if ranks is None:
         ranks = list(range(len(task_shape)))
     return SpatialTaskMapping(task_shape, ranks)
 
 
-def row_spatial(*task_shape: int):
+def row_spatial(*task_shape: Int):
     return spatial_map(task_shape)
 
 
-def col_spatial(*task_shape: int):
+def col_spatial(*task_shape: Int):
     return spatial_map(task_shape, ranks=list(reversed(range(len(task_shape)))))
 
 
-def repeat_map(task_shape: Sequence[int], ranks: Optional[Sequence[int]] = None):
-    from hidet.ir.tools import simplify_to_int
+def repeat_map(task_shape: Sequence[Int], ranks: Optional[Sequence[int]] = None, attrs: Optional[str] = None):
+    from hidet.ir.stmt import ForStmtAttr
+    from hidet.ir.tools import simplify
 
-    task_shape = [simplify_to_int(v) for v in task_shape]
+    task_shape = [simplify(v) for v in task_shape]
     if ranks is None:
         ranks = list(range(len(task_shape)))
-    return RepeatTaskMapping(task_shape, ranks)
-
-
-def row_repeat(*task_shape: int):
-    return repeat_map(task_shape)
-
-
-def col_repeat(*task_shape: int):
-    return repeat_map(task_shape, ranks=list(reversed(range(len(task_shape)))))
+    if attrs is None:
+        attrs = [ForStmtAttr() for _ in range(len(task_shape))]
+    else:
+        assert isinstance(attrs, str)
+        attrs: List[ForStmtAttr] = ForStmtAttr.parse(attrs)
+        if len(attrs) != len(task_shape):
+            raise ValueError(f"Invalid number of attributes: {len(attrs)} vs {len(task_shape)}")
+    return RepeatTaskMapping(task_shape, ranks, attrs)
+
+
+def row_repeat(*task_shape: Int, attrs: Optional[str] = None):
+    return repeat_map(task_shape, attrs=attrs)
+
+
+def col_repeat(*task_shape: Int, attrs: Optional[str] = None):
+    return repeat_map(task_shape, ranks=list(reversed(range(len(task_shape)))), attrs=attrs)
+
+
+def auto_map(
+    *task_shape: Int,
+    workers: Int,
+    on_fail: Optional[Callable[[str], None]] = None,
+    ranks: Optional[Sequence[int]] = None,
+) -> Optional[TaskMapping]:
+    """
+    Automatically generate a task mapping composed by spatial and repeat mappings.
+
+    Given the task shape [d1, d2, ..., dn] and the number of workers m, this function tries to find a task mapping
+    composed by spatial and repeat mappings that distribute the tasks to different workers. The goal is to make the
+    contiguous workers to process contiguous tasks. The number of tasks must be a multiple of the number of workers.
+
+    Some examples:
+        - the default ranks will be used if not specified:
+        auto_map(8, 32, workers=64) = repeat(4, 1).spatial(2, 32)
+        auto_map(8, 64, workers=64) = repeat(8, 1).spatial(1, 64)
+        auto_map(8, 96, workers=64) = repeat(4, 3).spatial(2, 32)
+        auto_map(8, 128, workers=64) = repeat(8, 2).spatial(1, 64)
+
+        - the ranks specify the order of dimensions to be mapped for contiguous workers:
+        auto_map(8, 96, workers=64, ranks=[1, 0]) = repeat(1, 12).spatial(8, 8)
+        auto_map(64, 8, workers=64, ranks=[1, 0]) = repeat(1, 8).spatial(64, 1)
+
+        - on_fail will be called if the task shape cannot be mapped to the number of workers:
+        auto_map(8, 41, workers=64) = None (on_fail will be called with an error message)
+
+        - task shape can have arbitrary dimensions:
+        auto_map(8, 16, 24, workers=32) = repeat(8, 4, 3).spatial(1, 4, 8)
+
+    Parameters
+    ----------
+    task_shape: Sequence[Expr or int]
+        The task shape.
+    workers: Expr or int
+        The number of workers.
+    on_fail: Callable[[str], None], optional
+        The callback function to be called when the task shape cannot be mapped to the number of workers.
+        This function it not necessarily to return (e.g., it can raise an exception).
+        The default is None, which means no callback function will be called, but a RuntimeError will be raised.
+    ranks:
+        The ranks of the task shape to be mapped to the workers. If not specified, the ranks will be
+        [0, 1, ..., n-1], where n is the number of dimensions.
+
+    Returns
+    -------
+    ret: Optional[TaskMapping]
+        The task mapping. If the task shape cannot be mapped to the number of workers and on_fail returns, None will be
+        returned.
+    """
+    from hidet.ir.tools import simplify_to_int
 
+    # automatic mapping requires both task shape and number of workers to be constant
+    task_shape: List[int] = [simplify_to_int(v) for v in task_shape]
+    workers: int = simplify_to_int(workers)
 
-def auto_map(*task_shape: int, workers: int, ranks: Optional[Sequence[int]] = None) -> TaskMapping:
-    task_shape: List[int] = list(task_shape)
     num_tasks = prod(task_shape)
     if num_tasks % workers != 0:
-        raise ValueError(
-            'Expect the number of tasks {} in task shape {} be a multiple of number of workers {}.'.format(
-                num_tasks, task_shape, workers
-            )
+        msg = 'Expect the number of tasks {} in task shape {} be a multiple of number of workers {}.'.format(
+            num_tasks, task_shape, workers
         )
+        if on_fail is None:
+            raise RuntimeError(msg)
+        else:
+            on_fail(msg)
+        return None
+
     num_dims = len(task_shape)
     if ranks is None:
         ranks = list(range(num_dims))
     else:
         ranks = list(ranks)
     spatial_shape = [0] * num_dims
     repeat_shape = [0] * num_dims
 
-    remain = workers
+    remain: int = workers
     for rank in reversed(range(num_dims)):
         dim = ranks.index(rank)
         spatial_shape[dim] = gcd(remain, task_shape[dim])
         repeat_shape[dim] = task_shape[dim] // spatial_shape[dim]
         remain //= spatial_shape[dim]
     return repeat_map(repeat_shape, ranks) * spatial_map(spatial_shape, ranks)
+
+
+def predicated_auto_map(
+    *task_shape: Int, workers: Int, ranks: Optional[Sequence[int]] = None
+) -> Tuple[TaskMapping, Callable[[Expr], Expr]]:
+    from hidet.ir.tools import simplify_to_int
+
+    # automatic mapping requires both task shape and number of workers to be constant
+    task_shape: List[int] = [simplify_to_int(v) for v in task_shape]
+    workers: int = simplify_to_int(workers)
+
+    num_dims: int = len(task_shape)
+    ranks: List[int]
+    if ranks is None:
+        ranks = list(range(num_dims))
+    else:
+        ranks = list(ranks)
+    spatial_shape: List[int] = [0] * num_dims
+    repeat_shape: List[int] = [0] * num_dims
+
+    remain: int = workers
+    for rank in reversed(range(num_dims)):
+        dim = ranks.index(rank)
+
+        if remain >= task_shape[dim]:
+            spatial_shape[dim] = task_shape[dim]
+            repeat_shape[dim] = 1
+            remain //= task_shape[dim]
+        else:
+            spatial_shape[dim] = gcd(remain, task_shape[dim])
+            repeat_shape[dim] = task_shape[dim] // spatial_shape[dim]
+            remain = 1
+
+    used_workers: int = prod(spatial_shape)
+
+    def predicate(worker_idx: Union[Expr, int]) -> Expr:
+        return convert(worker_idx < used_workers, dtype='bool')
+
+    return repeat_map(repeat_shape, ranks) * spatial_map(spatial_shape, ranks), predicate
```

## hidet/ir/stmt.py

```diff
@@ -5,14 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 from typing import Sequence, Tuple, Any, List, Union, Optional
 import enum
 from hidet.ir.node import Node
 from hidet.ir.type import DataType, PointerType, TensorPointerType, ReferenceType
 from hidet.ir.expr import Var, Expr, convert, Constant
 from hidet.ir.compute import TensorNode
 from hidet.ir.mapping import TaskMapping
@@ -93,28 +94,108 @@
         assert len(bind_vars) > 0
         bind_values = [convert(bind_value) for bind_value in bind_values]
         self.bind_vars: List[Var] = bind_vars
         self.bind_values: List[Expr] = bind_values
         self.body: Optional[Stmt] = body
 
 
+class ForStmtAttr:
+    def __init__(self, unroll=None, explicit_unroll=False):
+        self.unroll: Union[int, bool, None] = unroll
+        self.explicit_unroll: bool = explicit_unroll
+
+    def __str__(self):
+        if self.unroll is None:
+            return '.'
+        elif isinstance(self.unroll, bool):
+            if self.explicit_unroll:
+                return 'u+'
+            else:
+                return 'u'
+        else:
+            if self.explicit_unroll:
+                return f'u{self.unroll}+'
+            else:
+                return f'u{self.unroll}'
+
+    @staticmethod
+    def parse(attr: str) -> List[ForStmtAttr]:
+        """
+        Parse the attribute string and return a list of ForStmtAttr.
+
+        attr-string: attr+
+        attr:
+             | unroll
+             | default
+        unroll:
+             | 'u'          # unroll
+             | 'u' INT+     # unroll with factor, e.g., u1 u2 u3. u1 indicates unroll with factor 1 (i.e., no unroll)
+             | 'u' '+'      # explicit unroll, will be unrolled by hidet instead of underlying compiler
+        default: '.'
+
+
+        Parameters
+        ----------
+        attr: str
+            The attribute string.
+
+        Returns
+        -------
+        attrs: List[ForStmtAttr]
+            The list of ForStmtAttr.
+        """
+        s = attr.replace(' ', '')
+        idx = 0
+
+        def cur() -> Optional[str]:
+            if idx >= len(s):
+                return None
+            return s[idx]
+
+        attrs: List[ForStmtAttr] = []
+        while idx < len(s):
+            if s[idx] == '.':
+                idx += 1
+                attrs.append(ForStmtAttr(unroll=None, explicit_unroll=False))
+            elif s[idx] == 'u':
+                idx += 1
+                c = cur()
+                if c == '+':
+                    attrs.append(ForStmtAttr(unroll=True, explicit_unroll=True))
+                    idx += 1
+                elif c and c.isdigit():
+                    unroll = 0
+                    while c and c.isdigit():
+                        unroll = unroll * 10 + int(c)
+                        idx += 1
+                        c = cur()
+                    if unroll == 0:
+                        raise ValueError(f"Invalid attribute string: {attr}")
+                    attrs.append(ForStmtAttr(unroll=unroll, explicit_unroll=False))
+                else:
+                    attrs.append(ForStmtAttr(unroll=True, explicit_unroll=False))
+            else:
+                raise ValueError(f"Invalid attribute string: {attr}")
+        return attrs
+
+
 class ForStmt(Stmt):
     DEFAULT_UNROLL_LIMIT = 32
 
-    def __init__(self, loop_var, extent, unroll: Optional[Union[int, bool]] = None, body=None):
+    def __init__(self, loop_var, extent, body=None, *, attr: Optional[ForStmtAttr] = None):
         from hidet.ir.tools import simplify  # pylint: disable=import-outside-toplevel
 
         super().__init__()
         self.loop_var: Var = loop_var
         self.extent: Expr = simplify(convert(extent))
-        self.unroll: Optional[Union[int, bool]] = unroll
         self.body: Optional[Stmt] = body
+        self.attr: ForStmtAttr = attr if attr else ForStmtAttr()
 
 
-class ForTaskStmt(Stmt):
+class ForMappingStmt(Stmt):
     def __init__(self, loop_vars: Sequence[Var], mapping: TaskMapping, worker: Expr, body: Stmt):
         self.loop_vars: List[Var] = list(loop_vars)
         self.mapping: TaskMapping = mapping
         self.worker: Expr = worker
         self.body: Stmt = body
 
 
@@ -198,15 +279,15 @@
 
 def asm(
     template: str,
     *,
     outputs: Sequence[Any] = (),
     output_inputs: Sequence[Any] = (),
     inputs: Sequence[Any] = (),
-    is_volatile=False
+    is_volatile=False,
 ):
     from hidet.ir.tools import infer_type  # pylint: disable=import-outside-toplevel
 
     updated_outputs = []
     updated_inputs = []
 
     def get_register_type(expr: Expr) -> str:
@@ -248,7 +329,31 @@
     for output_input in output_inputs:
         constraint = '+' + get_register_type(output_input)
         updated_outputs.append((constraint, convert(output_input)))
     for x in inputs:
         constraint = get_register_type(x)
         updated_inputs.append((constraint, convert(x)))
     return AsmStmt(template, updated_outputs, updated_inputs, is_volatile)
+
+
+Int = Union[Expr, int]
+
+
+def launch_kernel(
+    func_var: Var,
+    args: Sequence[Expr],
+    grid_dim: Union[Sequence[Int], Int],
+    block_dim: Union[Sequence[Int], Int],
+    shared_mem: Optional[Int] = 0,
+) -> LaunchKernelStmt:
+    launch_config: List[Tuple[Expr, Expr, Expr]] = []
+    for dims in [grid_dim, block_dim]:
+        if not isinstance(dims, (list, tuple)):
+            dims = [dims]
+        dims = list(dims)
+        if len(dims) > 3:
+            raise ValueError('Grid/Block dimension must be 3 or less.')
+        while len(dims) < 3:
+            dims.append(1)
+        launch_config.append(convert(dims))
+    grid_dim, block_dim = launch_config
+    return LaunchKernelStmt(func_var, args, grid_dim, block_dim, convert(shared_mem))
```

## hidet/ir/task.py

```diff
@@ -7,22 +7,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # pylint: disable=import-outside-toplevel
 from __future__ import annotations
-from typing import Any, Dict, List, Union, Optional, Sequence, Callable
+from typing import Any, Dict, List, Union, Callable
 import os
 import pickle
 from hidet.ir.node import Node
 from hidet.ir.type import FuncType, VoidType
 from hidet.ir.expr import Expr, Var, var
 from hidet.ir.func import IRModule
-from hidet.ir.compute import ComputeNode, TensorNode, TensorInput, ScalarNode, ScalarInput, GridCompute
+from hidet.ir.compute import ComputeNode, TensorNode, TensorInput, ScalarInput, GridCompute
 
 
 class Target:
     _supported_targets = ['cuda', 'cpu']
 
     def __init__(self, name: str, attrs: List[str]):
         if name not in self._supported_targets:
@@ -76,72 +76,30 @@
                 'where a has {} indices and b has {} axes'.format(len(lhs.indices), len(rhs.axes))
             )
         rmap = dict(zip(rhs.axes, lhs.indices))
         indices = [rewrite(index_expr, rmap) for index_expr in rhs.indices]
         return InverseMap(lhs.axes, indices)
 
 
-class TaskGraph(Node):
-    def __init__(
-        self,
-        anchor: Task,
-        nodes: Sequence[Task],
-        consume: Dict[TensorInput, TensorNode],
-        input_tensors: Sequence[TensorNode],
-        output_tensors: Sequence[TensorNode],
-    ):
-        self.anchor: Task = anchor
-        self.nodes: List[Task] = list(nodes)
-        self.input_tensors: List[TensorNode] = list(input_tensors)
-        self.output_tensors: List[TensorNode] = list(output_tensors)
-        self.consume: Dict[TensorInput, TensorNode] = consume
-
-    @staticmethod
-    def from_task(task: Task) -> TaskGraph:
-        return TaskGraph(anchor=task, nodes=[task], consume={}, input_tensors=task.inputs, output_tensors=task.outputs)
-
-    def absorb(self) -> Task:
-        from hidet.ir.tools import rewrite
-
-        graph_input_tensors: List[TensorNode] = self.input_tensors
-        update_map: Dict[TensorNode, TensorNode] = {a: a for a in graph_input_tensors}
-        for task in self.nodes:
-            remap: Dict[TensorNode, TensorNode] = {}
-            for task_input_tensor in task.inputs:
-                if task_input_tensor not in self.consume:
-                    assert task_input_tensor in graph_input_tensors, 'must be graph input tensor'
-                    # do not need to rewrite, skip
-                else:
-                    remap[task_input_tensor] = update_map[self.consume[task_input_tensor]]
-            for task_output_tensor in task.outputs:
-                update_map[task_output_tensor] = rewrite(task_output_tensor, remap)
-                # original_output_tensor = task_output_tensor
-                # updated_output = rewrite(task_output_tensor, remap)
-                # update_map[original_output_tensor] = updated_output
-        graph_output_tensors: List[TensorNode] = [update_map[tensor] for tensor in self.output_tensors]
-        return Task(name=self.anchor.name, inputs=graph_input_tensors, outputs=graph_output_tensors)
-
-
 class Task(Node):
     """
     A task defines the operator computation.
     """
 
-    def __init__(self, name, inputs, outputs, inverse_map=None, arguments=None, attributes=None):
-        if inverse_map is None:
-            inverse_map = {}
-        if attributes is None:
-            attributes = {}
+    def __init__(self, name, inputs, outputs, *, params=None, inverse_map=None, attributes=None):
+        params = params if params else list(inputs) + list(outputs)
+        inverse_map = inverse_map if inverse_map else {}
+        attributes = attributes if attributes else {}
         self.name: str = name
-        self.inputs: List[TensorInput] = inputs
-        self.outputs: List[TensorNode] = outputs
-        self.attributes: Dict[str, Union[str, float, int, bool]] = attributes
-        self.arguments: Optional[List[Expr]] = arguments
+        self.inputs: List[TensorInput] = list(inputs)
+        self.outputs: List[TensorNode] = list(outputs)
+        self.params: List[Union[Var, TensorNode]] = params
         self.inverse_map: Dict[TensorInput, InverseMap] = {a: InverseMap.from_obj(b) for a, b in inverse_map.items()}
-        self.task_graph: Optional[TaskGraph] = TaskGraph.from_task(self)
+        self.attrs: Dict[str, Union[str, float, int, bool]] = attributes
+        self.specialization: Dict[Var, int] = {}
 
         # sanity check
         for tn, im in self.inverse_map.items():
             if len(im.axes) != tn.ndim:
                 raise ValueError(
                     'InverseMap for tensor {} has {} input axes, but input tensor has {} axes'.format(
                         tn.name, len(im.axes), tn.ndim
@@ -150,39 +108,56 @@
             if len(im.indices) != self.outputs[0].ndim:
                 raise ValueError(
                     'InverseMap for tensor {} has {} output indices, but output tensor has {} axes'.format(
                         tn.name, len(im.indices), self.outputs[0].ndim
                     )
                 )
 
+        from hidet.ir.tools import collect_free_vars
+
+        free_vars: List[Var] = collect_free_vars(self.outputs)
+        if any(v not in self.params and not isinstance(v.type, FuncType) for v in free_vars):
+            raise ValueError('Some free variables are not in params: {}'.format(free_vars))
+
     def signature(self) -> str:
         params = []
-        for tensor in self.inputs:
+        for tensor in self.tensor_params:
             name = tensor.name
-            dtype = tensor.ttype.dtype.name
-            shape = tensor.const_shape()
-            params.append('{}={}{}'.format(name, dtype, shape))
-        for name, value in self.attributes.items():
-            params.append('{}={}'.format(name, value))
+            dtype = tensor.type.dtype.name
+            params.append('{}={}{}'.format(name, dtype, tensor.type.shape))
+        for name, value in self.attrs.items():
+            params.append('{}={}'.format(name, repr(value)))
         param_doc = ', '.join(params)
         fuse_doc = ''
-        if len(self.task_graph.nodes) > 1:
-            fuse_doc = ' ({} fused)'.format(len(self.task_graph.nodes) - 1)
         return ''.join([self.name, '(', param_doc, ')', fuse_doc])
 
-    @property
-    def parameters(self) -> List[TensorNode]:
-        return self.task_graph.input_tensors + self.task_graph.output_tensors
+    def specialize_for(self, inputs):
+        """
+        Specialize this task for the given inputs.
 
-    @property
-    def self_params(self) -> List[TensorNode]:
-        params: List[TensorNode] = []
-        params += self.inputs
-        params += self.outputs
-        return params
+        Parameters
+        ----------
+        inputs: Sequence[hidet.graph.Tensor]
+            The input tensors.
+
+        Returns
+        -------
+        task: hidet.ir.Task
+            Self task specialized for the given inputs.
+        """
+        remap: Dict[Var, int] = {}
+        for a, b in zip(self.inputs, inputs):
+            for d1, d2 in zip(a.shape, b.shape):
+                if isinstance(d1, Var) and isinstance(d2, int):
+                    remap[d1] = d2
+        self.specialization.clear()
+        for param in self.params:
+            if isinstance(param, Var) and param in remap:
+                self.specialization[param] = remap[param]
+        return self
 
     def generate_arguments(self, inputs, outputs):
         """
         Generate arguments for the compiled function of this task given the tensor parameters.
 
         Parameters
         ----------
@@ -193,28 +168,56 @@
             The output tensors.
 
         Returns
         -------
         args: Sequence[Tensor or int]
             The arguments for the compiled function.
         """
-        if self.arguments is None:
-            return list(inputs) + list(outputs)
-        else:
-            from hidet.ir.tools import rewrite
+        remap = {a: b for a, b in zip(self.inputs, inputs)}
+        remap.update({a: b for a, b in zip(self.outputs, outputs)})
+        return [remap[arg] for arg in self.params]
 
-            remap = {}
-            for param, arg in zip(self.parameters, list(inputs) + list(outputs)):
-                remap[param] = arg
-                if param.ndim != len(arg.shape):
-                    raise ValueError(
-                        'Expect a tensor with {} dimensions, but got {} dimensions'.format(param.ndim, len(arg.shape))
-                    )
-                remap.update({param.type.shape[i]: arg.shape[i] for i in range(param.ndim)})
-            return [rewrite(arg, remap) for arg in self.arguments]
+    @property
+    def tensor_params(self) -> List[TensorNode]:
+        ret: List[TensorNode] = []
+        ret.extend(self.inputs)
+        ret.extend(self.outputs)
+        return ret
+
+    def dummy_arguments(self, device: str):
+        """
+        Generate dummy arguments for the compiled function of this task.
+
+        Parameters
+        ----------
+        device: str
+            The target device.
+
+        Returns
+        -------
+        args: Sequence[Tensor or int]
+            The arguments for the compiled function.
+        """
+        import hidet
+        from hidet.graph.tensor import Tensor
+
+        arguments: List[Union[Tensor, int]] = []
+        for param in self.params:
+            if isinstance(param, Var):
+                arguments.append(10)
+            elif isinstance(param, TensorNode):
+                if param.type.dtype.is_integer():
+                    arguments.append(hidet.zeros(param.const_shape(), dtype=param.type.dtype, device=device))
+                elif param.type.dtype.is_float():
+                    arguments.append(hidet.randn(param.const_shape(), dtype=param.type.dtype, device=device))
+                else:
+                    raise ValueError('Unknown dtype: {}'.format(param.type.dtype))
+            else:
+                raise ValueError('Unknown parameter type: {}'.format(type(param)))
+        return arguments
 
     def build(self, target: Union[str, Target]):
         """
         Build the task for the given target to a callable function.
 
         Parameters
         ----------
@@ -228,121 +231,133 @@
         """
         from hidet.driver import build_task
 
         if isinstance(target, Target):
             target = target.name
         return build_task(self, target_device=target, load=True)
 
-    def implement(self, target: Union[Target, str], workding_dir: str) -> IRModule:
+    def implement(self, target: Union[Target, str], working_dir: str) -> IRModule:
         from hidet.graph.ops.schedules.cuda.auto_scheduler import CudaAutoScheduler
         from hidet.graph.ops.schedules.cpu.auto_scheduler import CpuAutoScheduler
+        from hidet.graph.ops.definitions.utils.tune import tune
 
         if isinstance(target, str):
             target = Target.from_string(target)
         if target.name == 'cuda':
-            ret = self.implement_cuda(workding_dir)
+            ret = self.implement_cuda(working_dir)
             if ret is NotImplemented:
                 auto_scheduler = CudaAutoScheduler()
                 ret = auto_scheduler.schedule_task(self, 'cuda')
         elif target.name == 'cpu':
-            ret = self.implement_cpu(workding_dir)
+            ret = self.implement_cpu(working_dir)
             if ret is NotImplemented:
                 auto_scheduler = CpuAutoScheduler()
                 ret = auto_scheduler.schedule_task(self, 'cpu')
         else:
             raise ValueError()
-        if not isinstance(ret, IRModule):
-            raise AssertionError(f'The task implement function should return an IRModule, but got a {type(ret)}.')
-        return ret
+        if isinstance(ret, IRModule):
+            return ret
+
+        ir_modules: List[IRModule] = ret
+
+        if len(ir_modules) == 1:
+            return ir_modules[0]
+
+        if not all(isinstance(m, IRModule) for m in ir_modules):
+            raise AssertionError(
+                f'The task implement function should return an IRModule or a sequence of IRModule, '
+                f'but got a {type(ir_modules)}.'
+            )
+        dummy_args = self.dummy_arguments(target.name)
+        best_ir_module = tune(ir_modules, dummy_inputs=dummy_args, working_dir=working_dir)
+        return best_ir_module
 
-    def implement_cuda(self, workding_dir: str) -> IRModule:
+    def implement_cuda(self, working_dir: str) -> Union[IRModule, List[IRModule]]:
         return NotImplemented
 
-    def implement_cpu(self, workding_dir: str) -> IRModule:
+    def implement_cpu(self, working_dir: str) -> Union[IRModule, List[IRModule]]:
         return NotImplemented
 
     def allow_prologue(self) -> bool:
         return True
 
     def allow_epilogue(self) -> bool:
         return True
 
-    def is_injective_task(self) -> bool:
+    def is_injective(self) -> bool:
         from hidet.ir.tools import collect
 
         allowed_nodes = (ScalarInput, TensorInput, GridCompute)
         # if found other node like ReduceCompute and ArgReduceCompute, return False
         found_nodes = collect(self.outputs, ComputeNode, stop_when_found=False)
         return all(isinstance(node, allowed_nodes) for node in found_nodes)
 
+    def is_bijective(self) -> bool:
+        return self.is_injective() and len(self.inverse_map) > 0
+
     def save(self, fname: str):
         dirname = os.path.dirname(fname)
         os.makedirs(dirname, exist_ok=True)
         with open(fname, 'wb') as f:
             pickle.dump(self, f)
 
     @staticmethod
     def load(fname: str) -> Task:
         with open(fname, 'rb') as f:
             return pickle.load(f)
 
 
-def is_injective_task(task: Task) -> bool:
-    """
-    Check whether a task is an injective task. A task is injective if and only if there is no reduce compute in
-    the task.
-
-    Parameters
-    ----------
-    task: Task
-        The task to check.
-
-    Returns
-    -------
-    ret: bool
-        Whether the task is injective.
-    """
-    from hidet.ir.tools import collect
-
-    scalar_nodes: List[ScalarNode] = collect(task.outputs, ScalarNode, stop_when_found=False)
-    return all(sn.scalar_compute is None for sn in scalar_nodes)
-
-
-def is_unary_injective_task(task: Task) -> bool:
-    return len(task.inputs) == 1 and len(task.outputs) == 1 and is_injective_task(task)
-
-
-def is_elementwise_task(task: Task) -> bool:
-    """
-    Check whether a task is an elementwise task. A task is elementwise if and only if it is a unary injective and
-    invertible.
-
-    Parameters
-    ----------
-    task: Task
-        The task to check.
-
-    Returns
-    -------
-    ret: bool
-        Whether the task is elementwise.
-    """
-    return is_unary_injective_task(task) and len(task.inverse_map) > 0
+# def is_injective_task(task: Task) -> bool:
+#     """
+#     Check whether a task is an injective task. A task is injective if and only if there is no reduce compute in
+#     the task.
+#
+#     Parameters
+#     ----------
+#     task: Task
+#         The task to check.
+#
+#     Returns
+#     -------
+#     ret: bool
+#         Whether the task is injective.
+#     """
+#     from hidet.ir.tools import collect
+#
+#     scalar_nodes: List[ScalarNode] = collect(task.outputs, ScalarNode, stop_when_found=False)
+#     return all(sn.scalar_compute is None for sn in scalar_nodes)
+#
+#
+# def is_unary_injective_task(task: Task) -> bool:
+#     return len(task.inputs) == 1 and len(task.outputs) == 1 and is_injective_task(task)
+#
+#
+# def is_elementwise_task(task: Task) -> bool:
+#     """
+#     Check whether a task is an elementwise task. A task is elementwise if and only if it is a unary injective and
+#     invertible.
+#
+#     Parameters
+#     ----------
+#     task: Task
+#         The task to check.
+#
+#     Returns
+#     -------
+#     ret: bool
+#         Whether the task is elementwise.
+#     """
+#     return is_unary_injective_task(task) and len(task.inverse_map) > 0
 
 
 def save_task(task: Task, fname: str):
     task.save(fname)
 
 
 def load_task(fname: str) -> Task:
     return Task.load(fname)
 
 
 def task_compiled_func_type(task: Task) -> FuncType:
     from hidet.ir.tools import infer_type
 
-    if task.arguments:
-        args = task.arguments
-    else:
-        args = task.parameters
-
-    return FuncType(param_types=[infer_type(t) for t in args], ret_type=VoidType())
+    return FuncType(param_types=[infer_type(t) for t in task.params], ret_type=VoidType())
```

## hidet/ir/type.py

```diff
@@ -28,14 +28,26 @@
         elif isinstance(self, DataType):
             return PointerType(base_type=self)
         elif isinstance(self, (PointerType, TensorPointerType)):
             return PointerType(base_type=self)
         else:
             raise ValueError('Can not recognize type {}'.format(self))
 
+    def is_void(self):
+        return isinstance(self, VoidType)
+
+    def is_tensor(self):
+        return isinstance(self, TensorType)
+
+    def is_pointer(self):
+        return isinstance(self, (PointerType, TensorPointerType))
+
+    def is_data_type(self):
+        return isinstance(self, DataType)
+
 
 class DataType(TypeNode):
     """
     The data type that defines how to interpret the data in memory.
     """
 
     def __init__(self, name: str, short_name: str, nbytes: int):
@@ -258,20 +270,21 @@
         assert isinstance(layout, DataLayout)
         shape = layout.shape
     elif layout is None:
         layout = DataLayout.row_major(list(shape))
     else:
         assert isinstance(layout, DataLayout)
         assert isinstance(shape, (list, tuple))
-        for a, b in zip(shape, layout.shape):
-            if int(a) != int(b):
-                raise ValueError(
-                    'The shape of tensor and the shape of layout are not compatible, '
-                    '{} vs {}'.format(list(shape), list(layout.shape))
-                )
+        assert len(shape) == len(layout.shape)
+        # for a, b in zip(shape, layout.shape):
+        #     if int(a) != int(b):
+        #         raise ValueError(
+        #             'The shape of tensor and the shape of layout are not compatible, '
+        #             '{} vs {}'.format(list(shape), list(layout.shape))
+        #         )
     shape = convert(shape)
     return TensorType(dtype, shape, layout)
 
 
 def pointer_type(base_type):
     return PointerType(base_type)
```

## hidet/ir/builders/func_builder.py

```diff
@@ -61,18 +61,14 @@
 
     def extend_params(self, params: List[Var]):
         self.params.extend(params)
 
     def extend_extern_vars(self, extern_vars: List[Var]):
         self.extern_vars.extend(extern_vars)
 
-    # def extend_local_vars(self, local_vars: List[Var]):
-    #     assert isinstance(local_vars, (tuple, list))
-    #     self.local_vars.extend(local_vars)
-
     def extend_attrs(self, new_attrs: Dict[str, object]):
         self.attrs.update(new_attrs)
 
     def set_body(self, body: Stmt):
         self.body = body
 
     def finish_func(self):
```

## hidet/ir/builders/stmt_builder.py

```diff
@@ -7,24 +7,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Union, Optional, Sequence
 
-from hidet.ir.stmt import Stmt, ForStmt, IfStmt, EvaluateStmt, SeqStmt, LetStmt, ForTaskStmt
+from hidet.ir.stmt import Stmt, ForStmt, IfStmt, EvaluateStmt, SeqStmt, LetStmt, ForMappingStmt, ForStmtAttr
 from hidet.ir.expr import Expr, Var, var, convert
-from hidet.ir.mapping import TaskMapping, TaskMappingExpander
+from hidet.ir.mapping import TaskMapping
 
-ScopedStmt = Union[IfStmt, ForStmt, LetStmt, ForTaskStmt]
+ScopedStmt = Union[IfStmt, ForStmt, LetStmt, ForMappingStmt]
 
 
 class StmtScope:
     def __init__(self, sb: 'StmtBuilder', stmts: Union[Sequence[ScopedStmt], ScopedStmt], ret=None):
-        if isinstance(stmts, (IfStmt, ForStmt, LetStmt, ForTaskStmt)):
+        if isinstance(stmts, (IfStmt, ForStmt, LetStmt, ForMappingStmt)):
             stmts = [stmts]
         self.sb = sb
         self.stmts = stmts
         self.ret = ret
 
     def __enter__(self):
         for stmt in self.stmts:
@@ -64,36 +64,36 @@
         bind_values = [convert(value) for value in values]
         seq_let_stmt = LetStmt(bind_vars, bind_values, body=1)
         return StmtScope(self, stmts=seq_let_stmt, ret=bind_vars)
 
     def for_loop(self, v: Union[str, Var], extent: Union[int, Expr], unroll: Optional[bool] = None) -> StmtScope:
         if isinstance(v, str):
             v = var(v)
-        return StmtScope(self, stmts=ForStmt(v, extent, unroll), ret=v)
+        return StmtScope(self, stmts=ForStmt(v, extent, attr=ForStmtAttr(unroll)), ret=v)
 
     def if_then(self, cond: Union[bool, Expr]) -> StmtScope:
         return StmtScope(self, stmts=[IfStmt(cond)], ret=None)
 
     def otherwise(self) -> StmtScope:
         assert len(self.scope_stack[-1]) > 0
         if_stmt = self.scope_stack[-1].pop()
         assert isinstance(if_stmt, IfStmt)
         assert if_stmt.then_body is not None
         assert if_stmt.else_body is None
         return StmtScope(self, stmts=if_stmt, ret=None)
 
     def for_mapping(self, iter_names: Sequence[str], mapping: TaskMapping, worker: Expr) -> StmtScope:
         iter_names = [var(name) for name in iter_names]
-        return StmtScope(self, stmts=ForTaskStmt(iter_names, mapping, worker, None), ret=iter_names)
+        return StmtScope(self, stmts=ForMappingStmt(iter_names, mapping, worker, None), ret=iter_names)
 
-    def for_task(self, worker_index: Expr, task_layout: TaskMapping):
-        # replaced by for_mapping, todo: remove this function and rewrite all its usage
-        expander = TaskMappingExpander()
-        fields = expander.expand(worker_index, task_layout)
-        return StmtScope(self, stmts=expander.stmts, ret=fields)
+    # def for_task(self, worker_index: Expr, task_layout: TaskMapping):
+    #     # replaced by for_mapping, todo: remove this function and rewrite all its usage
+    #     expander = TaskMappingExpander()
+    #     fields = expander.expand(worker_index, task_layout)
+    #     return StmtScope(self, stmts=expander.stmts, ret=fields)
 
     def append(self, stmt: Union[Stmt, Expr, Sequence[Stmt]]):
         if stmt is None:
             return
         if isinstance(stmt, (Stmt, Expr)):
             if isinstance(stmt, Expr):
                 stmt = EvaluateStmt(stmt)
@@ -116,15 +116,15 @@
             last_stmt.body = body
         elif isinstance(last_stmt, IfStmt):
             if last_stmt.then_body is None:
                 last_stmt.then_body = body
             else:
                 assert last_stmt.else_body is None
                 last_stmt.else_body = body
-        elif isinstance(last_stmt, ForTaskStmt):
+        elif isinstance(last_stmt, ForMappingStmt):
             last_stmt.body = body
         else:
             assert False
 
     def finish(self):
         assert len(self.scope_stack) == 1
         return SeqStmt(self.scope_stack[0])
```

## hidet/ir/compute/reduce_operations.py

```diff
@@ -24,14 +24,17 @@
     Average = 'avg'
     And = 'and'
     Or = 'or'
 
     def __str__(self):
         return self.value
 
+    def __repr__(self):
+        return self.value
+
 
 class ReduceOperation:
     @staticmethod
     def from_name(name: Union[ReduceType, str]) -> ReduceOperation:
         name = ReduceType(name)
         name2operation = {
             ReduceType.Sum: SumReduce,
@@ -43,15 +46,15 @@
             ReduceType.Or: OrReduce,
         }
         if name not in name2operation:
             raise ValueError('Can not recognize reduce type {}'.format(name))
         return name2operation[name]()
 
     def __str__(self):
-        return self.__class__.__name__.lower()
+        return self.__class__.__name__.lower()[:-6]
 
     def initial_value(self, dtype: Union[DataType, str]) -> Constant:
         """
         The initial value of the reduction.
 
         Parameters
         ----------
```

## hidet/ir/dialects/pattern.py

```diff
@@ -10,14 +10,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Sequence, Tuple, Type, Optional, List, Union, Dict, Callable, ContextManager
 from contextlib import ExitStack
 from hidet.ir.node import Node
 from hidet.ir.type import TypeNode, DataType, TensorType, FuncType, data_type
 from hidet.ir.expr import Expr, Constant, Add, Sub, Multiply, Div, Mod, FloorDiv, LessThan, Equal, LessEqual
+from hidet.ir.expr import BitwiseXor
 from hidet.ir.expr import TensorElement, IfThenElse, Call, Var, LogicalAnd, LogicalOr, BinaryOp, convert, var
 from hidet.ir.compute import TensorNode, ScalarNode, ReduceOperation, ReduceCompute
 from hidet.ir.stmt import DeclareScope
 from hidet.ir.layout import StridesLayout, DataLayout
 
 
 class PatternNode(Node):
@@ -118,15 +119,18 @@
             PatternMatcher.check_type(self.pattern, self.target)
         try:
             self.matched[self.pattern] = self.target
             if isinstance(self.pattern, DataType):
                 self.dispatch[DataType](self.matcher, self.pattern, self.target)
             else:
                 # noinspection PyArgumentList
-                self.dispatch[self.pattern.__class__](self.matcher, self.pattern, self.target)
+                dispatched = self.dispatch.get(self.pattern.__class__, None)
+                if dispatched is None:
+                    raise NotImplementedError(f'Pattern {self.pattern} is not implemented')
+                dispatched(self.matcher, self.pattern, self.target)
         except NotMatchedError as e:
             # error from current <pattern, target>
             del self.matched[self.pattern]
             raise e
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type == NotMatchedError:
@@ -159,14 +163,15 @@
                 StringPattern: PatternMatcher.match_StringPattern,
                 # expr
                 Add: PatternMatcher.match_CommutativeBinary,
                 Sub: PatternMatcher.match_Binary,
                 Multiply: PatternMatcher.match_CommutativeBinary,
                 Div: PatternMatcher.match_Binary,
                 Mod: PatternMatcher.match_Binary,
+                BitwiseXor: PatternMatcher.match_Binary,
                 FloorDiv: PatternMatcher.match_Binary,
                 LessThan: PatternMatcher.match_Binary,
                 Equal: PatternMatcher.match_Binary,
                 LessEqual: PatternMatcher.match_Binary,
                 TensorElement: PatternMatcher.match_TensorElement,
                 IfThenElse: PatternMatcher.match_IfThenElse,
                 Call: PatternMatcher.match_Call,
```

## hidet/ir/functors/__init__.py

```diff
@@ -8,12 +8,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from .base_functor import BaseFunctor, BaseVisitor, BaseRewriter
 from .type_functor import TypeFunctor, TypeVisitor, TypeRewriter
 from .mapping_functor import MappingFunctor, MappingVisitor, MappingRewriter
+from .layout_functor import LayoutFunctor, LayoutVisitor, LayoutRewriter
 from .expr_functor import ExprFunctor, ExprVisitor, ExprRewriter
 from .stmt_functor import StmtFunctor, StmtVisitor, StmtRewriter
 from .compute_functor import ComputeFunctor, ComputeVisitor, ComputeRewriter
 from .module_functor import ModuleFunctor, ModuleVisitor, ModuleRewriter
 from .ir_functor import IRFunctor, IRVisitor, IRRewriter
```

## hidet/ir/functors/base_functor.py

```diff
@@ -5,15 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, Union, List, Dict, Tuple
+from typing import Any, Union, List, Dict, Tuple, Type
 from hidet.ir.node import Node
 from hidet.utils import same_list
 
 
 class BaseFunctor:
     def __init__(self, use_memo=True):
         self.memo = {} if use_memo else None
@@ -22,26 +22,37 @@
         return self.visit(node)
 
     def visit(self, node: Union[Node, Tuple, List, Dict[str, Any], str, int, float]):
         key = id(node) if isinstance(node, (list, dict)) else node
         if self.memo is not None and key in self.memo:
             return self.memo[key]
 
-        # iterate through the mro of the class to find a visit_dispatch method
-        for cls in type(self).__mro__:
-            if cls is object:
-                # we have reached the end of the mro but still not found a visit_dispatch method to dispatch the node
-                raise NotImplementedError("Can not dispatch object with type {}".format(type(node)))
-            if 'visit_dispatch' not in cls.__dict__:
-                continue
-            ret = cls.__dict__['visit_dispatch'](self, node)
-            if ret is not NotImplemented:
-                break
+        functor_cls: Type[BaseFunctor] = type(self)
+        node_cls = type(node)
+        dispatch_table = getattr(functor_cls, '__dispatch_table', None)
+        if dispatch_table and node_cls in dispatch_table:
+            # fast path
+            ret = dispatch_table[node_cls](self, node)
         else:
-            assert False  # should never reach here as object is always in the mro
+            # slow path
+            # iterate through the mro of the class to find a visit_dispatch method that can handle the node
+            for cls in type(self).__mro__:
+                dispatch_func = cls.__dict__.get('visit_dispatch', None)  # do not use getattr here
+                if dispatch_func is None:
+                    continue
+                ret = dispatch_func(self, node)
+                if ret is not NotImplemented:
+                    # record the dispatch function to the dispatch table of the functor class for fast path
+                    if dispatch_table is None:
+                        dispatch_table = {}
+                        setattr(functor_cls, '__dispatch_table', dispatch_table)
+                    dispatch_table[node_cls] = dispatch_func
+                    break
+            else:
+                raise NotImplementedError("Can not dispatch object with type {}".format(type(node)))
 
         if self.memo is not None:
             self.memo[key] = ret
 
         return ret
 
     def visit_dispatch(self, node: Union[Node, Tuple, List, Dict[str, Any], str, int, float]):
```

## hidet/ir/functors/compute_functor.py

```diff
@@ -8,27 +8,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # pylint: disable=bad-staticmethod-argument, too-many-boolean-expressions
 from typing import Any, Union, List, Dict, Tuple
 
-from hidet.ir.task import Task, TaskGraph
+from hidet.ir.task import Task
 from hidet.ir.compute import TensorInput, ScalarInput, ReduceCompute, ArgReduceCompute, GridCompute
 from hidet.ir.node import Node
 from hidet.utils import same_list
 from .base_functor import BaseFunctor, BaseVisitor, BaseRewriter
 
 
 class ComputeFunctor(BaseFunctor):
     def visit_dispatch(self, node: Union[Node, Tuple, List, Dict[str, Any], str]):
         if isinstance(node, Task):
             return self.visit_Task(node)
-        elif isinstance(node, TaskGraph):
-            return self.visit_TaskGraph(node)
         elif isinstance(node, ScalarInput):
             return self.visit_ScalarInput(node)
         elif isinstance(node, TensorInput):
             return self.visit_TensorInput(node)
         elif isinstance(node, GridCompute):
             return self.visit_GridCompute(node)
         elif isinstance(node, ReduceCompute):
@@ -37,17 +35,14 @@
             return self.visit_ArgReduceCompute(node)
         else:
             return NotImplemented
 
     def visit_Task(self, task: Task):
         raise NotImplementedError()
 
-    def visit_TaskGraph(self, task_graph: TaskGraph):
-        raise NotImplementedError()
-
     def visit_ScalarInput(self, node: ScalarInput):
         raise NotImplementedError()
 
     def visit_TensorInput(self, node: TensorInput):
         raise NotImplementedError()
 
     def visit_GridCompute(self, node: GridCompute):
@@ -60,20 +55,14 @@
         raise NotImplementedError()
 
 
 class ComputeVisitor(BaseVisitor, ComputeFunctor):
     def visit_Task(self, task: Task):
         self.visit(task.inputs)
         self.visit(task.outputs)
-        self.visit(task.task_graph)
-
-    def visit_TaskGraph(self, task_graph: TaskGraph):
-        for node in task_graph.nodes:
-            if node is not task_graph.anchor:
-                self.visit(node)
 
     def visit_ScalarInput(self, node: ScalarInput):
         self.visit(node.dtype)
 
     def visit_TensorInput(self, node: TensorInput):
         self.visit(node.ttype)
 
@@ -102,17 +91,14 @@
         self.visit(node.input_tensors)
 
 
 class ComputeRewriter(BaseRewriter, ComputeFunctor):
     def visit_Task(self, task: Task):
         return task
 
-    def visit_TaskGraph(self, task_graph: TaskGraph):
-        return task_graph
-
     def visit_ScalarInput(self, node: ScalarInput):
         dtype = self.visit(node.dtype)
         if dtype is node.dtype:
             return node
         else:
             return ScalarInput(node.name, dtype)
```

## hidet/ir/functors/ir_functor.py

```diff
@@ -11,21 +11,24 @@
 # limitations under the License.
 # pylint: disable=bad-staticmethod-argument, abstract-method, too-many-ancestors
 from .expr_functor import ExprFunctor, ExprRewriter, ExprVisitor
 from .compute_functor import ComputeFunctor, ComputeRewriter, ComputeVisitor
 from .stmt_functor import StmtFunctor, StmtRewriter, StmtVisitor
 from .type_functor import TypeFunctor, TypeRewriter, TypeVisitor
 from .mapping_functor import MappingFunctor, MappingRewriter, MappingVisitor
+from .layout_functor import LayoutFunctor, LayoutRewriter, LayoutVisitor
 from .module_functor import ModuleFunctor, ModuleRewriter, ModuleVisitor
 
 
-class IRFunctor(ModuleFunctor, StmtFunctor, ComputeFunctor, ExprFunctor, MappingFunctor, TypeFunctor):
+class IRFunctor(ModuleFunctor, StmtFunctor, ComputeFunctor, ExprFunctor, MappingFunctor, LayoutFunctor, TypeFunctor):
     pass
 
 
-class IRVisitor(ModuleVisitor, StmtVisitor, ComputeVisitor, ExprVisitor, MappingVisitor, TypeVisitor):
+class IRVisitor(ModuleVisitor, StmtVisitor, ComputeVisitor, ExprVisitor, MappingVisitor, LayoutVisitor, TypeVisitor):
     pass
 
 
-class IRRewriter(ModuleRewriter, StmtRewriter, ComputeRewriter, ExprRewriter, MappingRewriter, TypeRewriter):
+class IRRewriter(
+    ModuleRewriter, StmtRewriter, ComputeRewriter, ExprRewriter, MappingRewriter, LayoutRewriter, TypeRewriter
+):
     def rewrite(self, node):
         return self.visit(node)
```

## hidet/ir/functors/layout_functor.py

```diff
@@ -5,7 +5,108 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from hidet.ir.layout import DataLayout, StridesLayout, LocalLayout, ComposedLayout, SwizzleLayout, ConcatLayout
+from hidet.utils import same_list
+from .base_functor import BaseFunctor, BaseVisitor, BaseRewriter
+
+
+class LayoutFunctor(BaseFunctor):
+    def visit_dispatch(self, node):
+        if isinstance(node, DataLayout):
+            if isinstance(node, StridesLayout):
+                return self.visit_StridesLayout(node)
+            elif isinstance(node, LocalLayout):
+                return self.visit_LocalLayout(node)
+            elif isinstance(node, ComposedLayout):
+                return self.visit_ComposedLayout(node)
+            elif isinstance(node, SwizzleLayout):
+                return self.visit_SwizzleLayout(node)
+            elif isinstance(node, ConcatLayout):
+                return self.visit_ConcatLayout(node)
+            else:
+                raise ValueError('Can not recognize layout {}'.format(node))
+        else:
+            return NotImplemented
+
+    def visit_StridesLayout(self, layout: StridesLayout):
+        raise NotImplementedError()
+
+    def visit_LocalLayout(self, layout: LocalLayout):
+        raise NotImplementedError()
+
+    def visit_ComposedLayout(self, layout: ComposedLayout):
+        raise NotImplementedError()
+
+    def visit_SwizzleLayout(self, layout: SwizzleLayout):
+        raise NotImplementedError()
+
+    def visit_ConcatLayout(self, layout: ConcatLayout):
+        raise NotImplementedError()
+
+
+class LayoutVisitor(BaseVisitor, LayoutFunctor):
+    def visit_StridesLayout(self, layout: StridesLayout):
+        self.visit(layout.size)
+        self.visit(layout.shape)
+        self.visit(layout.strides)
+
+    def visit_LocalLayout(self, layout: LocalLayout):
+        self.visit(layout.shape)
+
+    def visit_ComposedLayout(self, layout: ComposedLayout):
+        self.visit(layout.outer)
+        self.visit(layout.inner)
+
+    def visit_SwizzleLayout(self, layout: SwizzleLayout):
+        self.visit(layout.base)
+        self.visit(layout.shape)
+        self.visit(layout.size)
+
+    def visit_ConcatLayout(self, layout: ConcatLayout):
+        self.visit(layout.lhs)
+        self.visit(layout.rhs)
+
+
+class LayoutRewriter(BaseRewriter, LayoutFunctor):
+    def visit_StridesLayout(self, layout: StridesLayout):
+        size = self.visit(layout.size)
+        shape = self.visit(layout.shape)
+        strides = self.visit(layout.strides)
+        if same_list([size], [layout.size]) and same_list(shape, layout.shape) and same_list(strides, layout.strides):
+            return layout
+        else:
+            return StridesLayout(shape, strides)
+
+    def visit_LocalLayout(self, layout: LocalLayout):
+        shape = self.visit(layout.shape)
+        if same_list(shape, layout.shape):
+            return layout
+        else:
+            return LocalLayout(shape)
+
+    def visit_ComposedLayout(self, layout: ComposedLayout):
+        outer = self.visit(layout.outer)
+        inner = self.visit(layout.inner)
+        if outer is layout.outer and inner is layout.inner:
+            return layout
+        else:
+            return ComposedLayout(outer, inner)
+
+    def visit_SwizzleLayout(self, layout: SwizzleLayout):
+        base = self.visit(layout.base)
+        if base is layout.base:
+            return layout
+        else:
+            return SwizzleLayout(base, layout.dim, layout.regards_dim, layout.log_step)
+
+    def visit_ConcatLayout(self, layout: ConcatLayout):
+        lhs = self.visit(layout.lhs)
+        rhs = self.visit(layout.rhs)
+        if lhs is layout.lhs and rhs is layout.rhs:
+            return layout
+        else:
+            return ConcatLayout(lhs, rhs)
```

## hidet/ir/functors/module_functor.py

```diff
@@ -48,15 +48,15 @@
 class ModuleRewriter(ModuleFunctor, BaseRewriter):
     def visit_IRModule(self, module: IRModule):
         global_vars = self.visit(module.global_vars)
         functions = self.visit(module.functions)
         if same_list(global_vars, module.global_vars) and functions is module.functions:
             return module
         else:
-            return IRModule(global_vars, module.task, functions)
+            return IRModule(functions, module.task, global_vars)
 
     def visit_Function(self, func: Function):
         params = self.visit(func.params)
         ret_type = self.visit(func.ret_type)
         body = self.visit(func.body)
         attrs = self.visit(func.attrs)
         if same_list(params, func.params) and ret_type is func.ret_type and body is func.body and attrs is func.attrs:
```

## hidet/ir/functors/stmt_functor.py

```diff
@@ -10,15 +10,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # pylint: disable=bad-staticmethod-argument
 from typing import List
 
 from hidet.ir.node import Node
 from hidet.ir.expr import Expr, Var
-from hidet.ir.stmt import EvaluateStmt, DeclareStmt, BufferStoreStmt, AssignStmt, LetStmt, ForStmt, ForTaskStmt, SeqStmt
+from hidet.ir.stmt import (
+    EvaluateStmt,
+    DeclareStmt,
+    BufferStoreStmt,
+    AssignStmt,
+    LetStmt,
+    ForStmt,
+    ForMappingStmt,
+    SeqStmt,
+)
 from hidet.ir.stmt import WhileStmt, BreakStmt, ContinueStmt, IfStmt, ReturnStmt, AsmStmt, AssertStmt, BlackBoxStmt
 from hidet.ir.stmt import LaunchKernelStmt
 from hidet.utils import same_list
 
 from .base_functor import BaseFunctor, BaseVisitor, BaseRewriter
 
 
@@ -32,15 +41,15 @@
             return self.visit_BufferStoreStmt(node)
         elif isinstance(node, AssignStmt):
             return self.visit_AssignStmt(node)
         elif isinstance(node, LetStmt):
             return self.visit_LetStmt(node)
         elif isinstance(node, ForStmt):
             return self.visit_ForStmt(node)
-        elif isinstance(node, ForTaskStmt):
+        elif isinstance(node, ForMappingStmt):
             return self.visit_ForTaskStmt(node)
         elif isinstance(node, WhileStmt):
             return self.visit_WhileStmt(node)
         elif isinstance(node, BreakStmt):
             return self.visit_BreakStmt(node)
         elif isinstance(node, ContinueStmt):
             return self.visit_ContinueStmt(node)
@@ -75,15 +84,15 @@
 
     def visit_LetStmt(self, stmt: LetStmt):
         raise NotImplementedError()
 
     def visit_ForStmt(self, stmt: ForStmt):
         raise NotImplementedError()
 
-    def visit_ForTaskStmt(self, stmt: ForTaskStmt):
+    def visit_ForTaskStmt(self, stmt: ForMappingStmt):
         raise NotImplementedError()
 
     def visit_WhileStmt(self, stmt: WhileStmt):
         raise NotImplementedError()
 
     def visit_BreakStmt(self, stmt: BreakStmt):
         raise NotImplementedError()
@@ -137,15 +146,15 @@
             self.visit(bind_value)
         self.visit(stmt.body)
 
     def visit_ForStmt(self, stmt: ForStmt):
         self.visit(stmt.extent)
         self.visit(stmt.body)
 
-    def visit_ForTaskStmt(self, stmt: ForTaskStmt):
+    def visit_ForTaskStmt(self, stmt: ForMappingStmt):
         for loop_var in stmt.loop_vars:
             self.visit(loop_var)
         self.visit(stmt.worker)
         self.visit(stmt.body)
 
     def visit_WhileStmt(self, stmt: WhileStmt):
         self.visit(stmt.cond)
@@ -238,27 +247,27 @@
     def visit_ForStmt(self, stmt: ForStmt):
         loop_var = stmt.loop_var
         extent = self.visit(stmt.extent)
         body = self.visit(stmt.body)
         if loop_var is stmt.loop_var and extent is stmt.extent and body is stmt.body:
             return stmt
         else:
-            return ForStmt(loop_var, extent, stmt.unroll, body)
+            return ForStmt(loop_var, extent, body=body, attr=stmt.attr)
 
-    def visit_ForTaskStmt(self, stmt: ForTaskStmt):
+    def visit_ForTaskStmt(self, stmt: ForMappingStmt):
         loop_vars: List[Expr] = [self.visit(v) for v in stmt.loop_vars]
         # todo: visit expressions in task mapping
         worker = self.visit(stmt.worker)
         body = self.visit(stmt.body)
         if same_list(loop_vars, stmt.loop_vars) and worker is stmt.worker and body is stmt.body:
             return stmt
         else:
             assert all(isinstance(v, Var) for v in loop_vars)
             asserted_loop_vars: List[Var] = [v for v in loop_vars if isinstance(v, Var)]  # avoid IDE warning
-            return ForTaskStmt(loop_vars=asserted_loop_vars, mapping=stmt.mapping, worker=worker, body=body)
+            return ForMappingStmt(loop_vars=asserted_loop_vars, mapping=stmt.mapping, worker=worker, body=body)
 
     def visit_WhileStmt(self, stmt: WhileStmt):
         cond = self.visit(stmt.cond)
         body = self.visit(stmt.body)
         if cond is stmt.cond and body is stmt.body:
             return stmt
         else:
```

## hidet/ir/primitives/__init__.py

```diff
@@ -9,15 +9,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from .func import register_primitive_function, is_primitive_function, lookup_primitive_function
 
 # base primitive functions
 # pylint: disable=redefined-builtin
-from .math import sin, cos, tan, sinh, cosh, tanh, asin, acos, atan, asinh, acosh, atanh, expm1
+from .math import sin, cos, tan, sinh, cosh, tanh, asin, acos, atan, asinh, acosh, atanh, expm1, abs
 from .math import max, min, exp, pow, sqrt, rsqrt, erf, ceil, log, log2, log10, log1p, round, floor, trunc
 from .math import isfinite, isinf, isnan
 
 # function used to debug
 from .debug import printf
 
 # cpu primitive functions
```

## hidet/ir/primitives/math.py

```diff
@@ -104,14 +104,17 @@
 
     def log1p(self, a: Expr) -> Expr:
         raise NotImplementedError()
 
     def round(self, a: Expr) -> Expr:
         raise NotImplementedError()
 
+    def abs(self, a: Expr) -> Expr:
+        raise NotImplementedError()
+
     def trunc(self, a: Expr) -> Expr:
         raise NotImplementedError()
 
     def ceil(self, a: Expr) -> Expr:
         raise NotImplementedError()
 
     def floor(self, a: Expr) -> Expr:
@@ -170,18 +173,19 @@
     def register():
         unary_names = [
             'sin',
             'cos',
             'tanh',
             'exp',
             'round',
+            'abs',
             'floor',
             'ceil',
-            'rsqrt',
             'sqrt',
+            'rsqrt',
             'erf',
             'log',
             'log2',
             'log10',
             'log1p',
             'trunc',
             'isfinite',
@@ -198,14 +202,16 @@
             register_primitive_function(name=f'generic_{name}', codegen_name=None, func_or_type=func_type, generic=True)
 
     @staticmethod
     def call(name, *args) -> Expr:
         entry = lookup_primitive_function(f'generic_{name}')
         return Call(entry.var, args)
 
+    # unary names
+
     def sin(self, a: Expr) -> Expr:
         return self.call('sin', a)
 
     def cos(self, a: Expr) -> Expr:
         return self.call('cos', a)
 
     def tan(self, a: Expr) -> Expr:
@@ -234,17 +240,14 @@
 
     def acosh(self, a: Expr) -> Expr:
         return self.call('acosh', a)
 
     def atanh(self, a: Expr) -> Expr:
         return self.call('atanh', a)
 
-    def atan2(self, a: Expr, b: Expr) -> Expr:
-        return self.call('atan2', a, b)
-
     def exp(self, a: Expr) -> Expr:
         return self.call('exp', a)
 
     def expm1(self, a: Expr) -> Expr:
         return self.call('expm1', a)
 
     def erf(self, a: Expr) -> Expr:
@@ -267,14 +270,17 @@
 
     def log1p(self, a: Expr) -> Expr:
         return self.call('log1p', a)
 
     def round(self, a: Expr) -> Expr:
         return self.call('round', a)
 
+    def abs(self, a: Expr) -> Expr:
+        return self.call('abs', a)
+
     def ceil(self, a: Expr) -> Expr:
         return self.call('ceil', a)
 
     def floor(self, a: Expr) -> Expr:
         return self.call('floor', a)
 
     def trunc(self, a: Expr) -> Expr:
@@ -285,26 +291,33 @@
 
     def isinf(self, a: Expr) -> Expr:
         return self.call('isinf', a)
 
     def isnan(self, a: Expr) -> Expr:
         return self.call('isnan', a)
 
+    # binary names
+
+    def atan2(self, a: Expr, b: Expr) -> Expr:
+        return self.call('atan2', a, b)
+
     def min(self, a: Expr, b: Expr) -> Expr:
         return self.call('min', a, b)
 
     def max(self, a: Expr, b: Expr) -> Expr:
         return self.call('max', a, b)
 
     def mod(self, a: Expr, b: Expr) -> Expr:
         return self.call('mod', a, b)
 
     def pow(self, a: Expr, b: Expr) -> Expr:
         return self.call('pow', a, b)
 
+    # ternary names
+
     def fma(self, a: Expr, b: Expr, c: Expr) -> Expr:
         return self.call('fma', a, b, c)
 
 
 generic_math_function_set = MathFunctionSetGeneric()
 generic_math_function_set.register()
 
@@ -397,14 +410,18 @@
     return generic_math_function_set.log1p(a)
 
 
 def round(a: Expr) -> Expr:
     return generic_math_function_set.round(a)
 
 
+def abs(a: Expr) -> Expr:
+    return generic_math_function_set.abs(a)
+
+
 def ceil(a: Expr) -> Expr:
     return generic_math_function_set.ceil(a)
 
 
 def floor(a: Expr) -> Expr:
     return generic_math_function_set.floor(a)
```

## hidet/ir/primitives/cpu/math/__init__.py

```diff
@@ -9,7 +9,9 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from . import float32
 from . import float64
 from . import int32
 from . import int64
+from . import bfloat16
+from . import float16
```

## hidet/ir/primitives/cpu/math/float32.py

```diff
@@ -33,14 +33,15 @@
             'atanh': 'atanhf',
             'exp': 'expf',
             'erf': 'erff',
             'sqrt': 'sqrtf',
             'rsqrt': 'rsqrtf',
             'log': 'logf',
             'round': 'roundf',
+            'abs': 'fabsf',
             'ceil': 'ceilf',
             'floor': 'floorf',
             'expm1': 'expm1f',
             'log2': 'log2f',
             'log10': 'log10f',
             'log1p': 'log1pf',
             'trunc': 'truncf',
@@ -90,14 +91,17 @@
 
     def log(self, a: Expr) -> Expr:
         return self.call('log', a)
 
     def round(self, a: Expr) -> Expr:
         return self.call('round', a)
 
+    def abs(self, a: Expr) -> Expr:
+        return self.call('abs', a)
+
     def ceil(self, a: Expr) -> Expr:
         return self.call('ceil', a)
 
     def floor(self, a: Expr) -> Expr:
         return self.call('floor', a)
 
     def tan(self, a: Expr) -> Expr:
```

## hidet/ir/primitives/cpu/math/float64.py

```diff
@@ -33,14 +33,15 @@
             'atanh': 'atanh',
             'exp': 'exp',
             'erf': 'erf',
             'sqrt': 'sqrt',
             'rsqrt': 'rsqrt',
             'log': 'log',
             'round': 'round',
+            'abs': 'abs',
             'ceil': 'ceil',
             'floor': 'floor',
             'expm1': 'expm1',
             'log2': 'log2',
             'log10': 'log10',
             'log1p': 'log1p',
             'trunc': 'trunc',
@@ -90,14 +91,17 @@
 
     def log(self, a: Expr) -> Expr:
         return self.call('log', a)
 
     def round(self, a: Expr) -> Expr:
         return self.call('round', a)
 
+    def abs(self, a: Expr) -> Expr:
+        return self.call('abs', a)
+
     def ceil(self, a: Expr) -> Expr:
         return self.call('ceil', a)
 
     def floor(self, a: Expr) -> Expr:
         return self.call('floor', a)
 
     def tan(self, a: Expr) -> Expr:
```

## hidet/ir/primitives/cuda/math/float32.py

```diff
@@ -33,14 +33,15 @@
             'atanh': 'atanhf',
             'exp': 'expf',
             'erf': 'erff',
             'sqrt': 'sqrtf',
             'rsqrt': 'rsqrtf',
             'log': 'logf',
             'round': 'roundf',
+            'abs': 'fabsf',
             'ceil': 'ceilf',
             'floor': 'floorf',
             'expm1': 'expm1f',
             'log2': 'log2f',
             'log10': 'log10f',
             'log1p': 'log1pf',
             'trunc': 'truncf',
@@ -90,14 +91,17 @@
 
     def log(self, a: Expr) -> Expr:
         return self.call('log', a)
 
     def round(self, a: Expr) -> Expr:
         return self.call('round', a)
 
+    def abs(self, a: Expr) -> Expr:
+        return self.call('abs', a)
+
     def ceil(self, a: Expr) -> Expr:
         return self.call('ceil', a)
 
     def floor(self, a: Expr) -> Expr:
         return self.call('floor', a)
 
     def tan(self, a: Expr) -> Expr:
```

## hidet/ir/primitives/cuda/math/float64.py

```diff
@@ -33,14 +33,15 @@
             'atanh': 'atanh',
             'exp': 'exp',
             'erf': 'erf',
             'sqrt': 'sqrt',
             'rsqrt': 'rsqrt',
             'log': 'log',
             'round': 'round',
+            'abs': 'fabs',
             'ceil': 'ceil',
             'floor': 'floor',
             'expm1': 'expm1',
             'log2': 'log2',
             'log10': 'log10',
             'log1p': 'log1p',
             'trunc': 'trunc',
@@ -90,14 +91,17 @@
 
     def log(self, a: Expr) -> Expr:
         return self.call('log', a)
 
     def round(self, a: Expr) -> Expr:
         return self.call('round', a)
 
+    def abs(self, a: Expr) -> Expr:
+        return self.call('abs', a)
+
     def ceil(self, a: Expr) -> Expr:
         return self.call('ceil', a)
 
     def floor(self, a: Expr) -> Expr:
         return self.call('floor', a)
 
     def tan(self, a: Expr) -> Expr:
```

## hidet/ir/tools/__init__.py

```diff
@@ -6,11 +6,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from .type_infer import infer_type, TypeInfer
-from .util_functors import rewrite, collect, collect_free_vars, clone
+from .util_functors import collect, clone
+from .rewriter import rewrite
+from .free_var_collector import collect_free_vars
 from .printer import astext
 from .simplifier import simplify, simplify_to_int
 from .hasher import ExprHash
```

## hidet/ir/tools/printer.py

```diff
@@ -14,62 +14,49 @@
 from hidet.ir.func import IRModule, Function
 from hidet.ir.type import DataType, TensorType, VoidType, PointerType, ReferenceType, TensorPointerType
 from hidet.ir.expr import Constant, Var, Call, TensorElement, Add, Multiply, LessThan, FloorDiv, Mod, Equal, Div
 from hidet.ir.expr import Sub, LogicalNot, LogicalOr, LogicalAnd, Let, IfThenElse, TensorSlice
 from hidet.ir.expr import RightShift, LeftShift, BitwiseNot, BitwiseOr
 from hidet.ir.expr import BitwiseAnd, Neg, Cast, NotEqual, BitwiseXor, Reference, Dereference, Address
 from hidet.ir.stmt import SeqStmt, IfStmt, ForStmt, AssignStmt, BufferStoreStmt, EvaluateStmt, AssertStmt
-from hidet.ir.stmt import BlackBoxStmt, AsmStmt, ReturnStmt, LetStmt, DeclareStmt, ForTaskStmt, WhileStmt, ContinueStmt
+from hidet.ir.stmt import (
+    BlackBoxStmt,
+    AsmStmt,
+    ReturnStmt,
+    LetStmt,
+    DeclareStmt,
+    ForMappingStmt,
+    WhileStmt,
+    ContinueStmt,
+)
 from hidet.ir.stmt import BreakStmt, DeclareScope, LaunchKernelStmt
+from hidet.ir.layout import StridesLayout, ConcatLayout, LocalLayout, SwizzleLayout, ComposedLayout, RowMajorLayout
+from hidet.ir.layout import ColumnMajorLayout
 from hidet.ir.mapping import RepeatTaskMapping, SpatialTaskMapping, ComposedTaskMapping
 from hidet.ir.compute import TensorNode, GridCompute, ArgReduceCompute, ReduceCompute, TensorInput, ScalarInput
 from hidet.ir.dialects.pattern import AnyExpr
-from hidet.ir.layout import RowMajorLayout, ColumnMajorLayout
-from hidet.ir.task import Task, TaskGraph
+from hidet.ir.task import Task
 from hidet.utils import same_list
 from hidet.utils.doc import Doc, NewLine, Text, doc_join
 from hidet.utils.namer import Namer
 
 from hidet.ir.functors import IRFunctor
 
+_show_var_id = False
+
 
 class IRPrinter(IRFunctor):
     def __init__(self):
-        super().__init__()
+        super().__init__(use_memo=False)
         self.namer = Namer()
         self.ir_module: Optional[IRModule] = None
 
     def __call__(self, node):
         return self.visit(node)
 
-    # def visit_dispatch(self, obj):  # pylint: disable=arguments-renamed, too-many-branches
-    #     # type node
-    #     if isinstance(obj, TypeNode):
-    #         return TypeFunctor.visit(self, obj)
-    #     # function and ir module
-    #     elif isinstance(obj, Function):
-    #         return self.visit_Function(obj)
-    #     elif isinstance(obj, IRModule):
-    #         return self.visit_IRModule(obj)
-    #     # expression and statement
-    #     elif isinstance(obj, (Expr, Stmt)):
-    #         return BaseFunctor.visit(self, obj)
-    #     # task related
-    #     elif isinstance(obj, Task):
-    #         return self.visit_Task(obj)
-    #     elif isinstance(obj, TaskGraph):
-    #         return self.visit_TaskGraph(obj)
-    #     elif isinstance(obj, InverseMap):
-    #         return self.visit_InverseMap(obj)
-    #     # task mapping
-    #     elif isinstance(obj, TaskMapping):
-    #         return self.visit_TaskMapping(obj)
-    #     else:
-    #         raise ValueError('Do not support print object {}'.format(object.__repr__(obj)))
-
     def visit_Tuple(self, tp: Tuple):
         return doc_join([self(v) for v in tp], ', ')
 
     def visit_List(self, lst: List):
         return doc_join([self(v) for v in lst], ', ')
 
     def visit_Dict(self, d: Dict):
@@ -79,46 +66,42 @@
         raise NotImplementedError('Do not support print node {}'.format(type(n)))
 
     def visit_PyConstant(self, c: Union[str, int, float, None]):
         return Text(str(c))
 
     def visit_Function(self, func: Function):
         self.namer.clear()
-        doc = Doc()
 
         # parameters
-        doc += 'fn('
-        param_docs = []
+        head_doc = Doc()
+        head_doc += Text('def ') + func.name + '('
         for i, param in enumerate(func.params):
-            line = []
-            if i != 0:
-                line.append(NewLine())
-            line.extend([self(param), ': ', self(param.type)])
-            param_docs.append(line)
-        doc += doc_join(param_docs, Text(', '))
-        doc += ')'
-        doc = doc.indent(3)
+            head_doc += (NewLine() + self(param) + ': ' + self(param.type)).indent(4)
+            if i < len(func.params) - 1:
+                head_doc += ','
+        head_doc += NewLine() + ')'
 
         # attributes
+        attr_doc = Doc()
         for attr_name, attr_value in func.attrs.items():
-            doc += (NewLine() + '# {}: {}'.format(attr_name, attr_value)).indent(4)
+            attr_doc += (NewLine() + '# {}: {}'.format(attr_name, attr_value)).indent(4)
 
         # body
-        doc += self(func.body).indent(4)
+        body_doc = self(func.body).indent(4)
 
-        return doc
+        return head_doc + attr_doc + body_doc + NewLine()
 
     def visit_IRModule(self, ir_module: IRModule):
         doc = Doc()
         self.ir_module = ir_module
         if ir_module.task is not None:
-            doc += str(ir_module.task)
+            doc += self(ir_module.task)
         doc += NewLine()
-        for name, func in ir_module.functions.items():
-            doc += ['def ', name, ' ', self(func), NewLine(), NewLine()]
+        for func in ir_module.functions.values():
+            doc += self(func) + NewLine()
         return doc
 
     def visit_Add(self, e: Add):
         return Text('(') + self(e.a) + ' + ' + self(e.b) + ')'
 
     def visit_Sub(self, e: Sub):
         return Text('(') + self(e.a) + ' - ' + self(e.b) + ')'
@@ -228,14 +211,16 @@
     def visit_Dereference(self, e: Dereference):
         return Text('*') + self(e.expr)
 
     def visit_Address(self, e: Address):
         return Text('&') + self(e.expr)
 
     def visit_Var(self, e: Var):
+        if _show_var_id:
+            return Text('{}@{}'.format(self.namer.get_name(e), e.id))
         return Text(self.namer.get_name(e))
 
     def visit_Constant(self, e: Constant):
         if e.value is None:
             return self('Constant(None, type=') + self(e.type) + ')'
         if e.is_tensor():
             return 'ConstTensor({}, {})'.format(e.value.shape, e.type)
@@ -283,23 +268,20 @@
         doc += self(stmt.body)
         # doc += self(stmt.body).indent()
         return doc
 
     def visit_ForStmt(self, stmt: ForStmt):
         rng = Text('range(') + self(stmt.extent) + ')'
         doc = NewLine() + Text('for ') + self(stmt.loop_var) + ' in ' + rng
-        if stmt.unroll is not None:
-            if stmt.unroll:
-                doc += '[unroll]'
-            else:
-                doc += '[no-unroll]'
+        if stmt.attr.unroll is not None:
+            doc += '  # ' + str(stmt.attr)
         doc += self(stmt.body).indent(4)
         return doc
 
-    def visit_ForTaskStmt(self, stmt: ForTaskStmt):
+    def visit_ForTaskStmt(self, stmt: ForMappingStmt):
         doc = NewLine() + Text('for ') + self(stmt.loop_vars) + ' in ' + self(stmt.mapping) + ' on ' + self(stmt.worker)
         doc += self(stmt.body).indent(4)
         return doc
 
     def visit_WhileStmt(self, stmt: WhileStmt):
         doc = NewLine() + 'while ' + self(stmt.cond)
         doc += self(stmt.body).indent(4)
@@ -350,15 +332,15 @@
             + doc_join(output_docs, ', ')
             + ' : '
             + doc_join(input_docs, ', ')
             + ');'
         )
 
     def visit_LaunchKernelStmt(self, stmt: LaunchKernelStmt):
-        return Text("{}<<<dim3({}, {}, {}), dim3({}, {}, {}), {}>>>({});").format(
+        return NewLine() + Text("{}<<<dim3({}, {}, {}), dim3({}, {}, {}), {}>>>({});").format(
             self(stmt.func_var),
             self(stmt.grid_dim[0]),
             self(stmt.grid_dim[1]),
             self(stmt.grid_dim[2]),
             self(stmt.block_dim[0]),
             self(stmt.block_dim[1]),
             self(stmt.block_dim[2]),
@@ -380,33 +362,31 @@
         for s in stmt.seq:
             doc += self(s)
         return doc
 
     def visit_ScalarType(self, t: DataType):
         return Text('{}'.format(t.name))
 
-    def visit_TensorType(self, t: TensorType):
+    def _tensor_type(self, t: TensorType):
         items = [self(t.dtype), '[' + self(t.shape) + ']']
-        if isinstance(t.layout, RowMajorLayout):
+        if isinstance(t.layout, RowMajorLayout) or t.layout is None:
             # default layout, do not print
             pass
-        elif isinstance(t.layout, ColumnMajorLayout):
-            items.append(Text('col_major'))
-        elif t.layout is None:
-            # skip None
-            pass
         else:
-            items.append(Text(type(t.layout).__name__))
-        return Text('tensor(') + doc_join(items, ', ') + ')'
+            items.append(self(t.layout))
+        return doc_join(items, ', ')
+
+    def visit_TensorType(self, t: TensorType):
+        return Text('tensor(') + self._tensor_type(t) + ')'
 
     def visit_PointerType(self, t: PointerType):
         return Text('PointerType(') + self(t.base_type) + ')'
 
     def visit_TensorPointerType(self, t: TensorPointerType):
-        return Text('TensorPointerType(') + self(t.tensor_type) + ')'
+        return Text('tensor_pointer(') + self._tensor_type(t.tensor_type) + ')'
 
     def visit_ReferenceType(self, t: ReferenceType):
         return Text('ReferenceType(') + self(t.base_type) + ')'
 
     def visit_VoidType(self, t: VoidType):
         return Text('VoidType')
 
@@ -437,88 +417,30 @@
 
     def visit_Task(self, e: Task):
         lines = [
             Text('name: ') + e.name,
             Text('parameters: ')
             + (
                 NewLine()
-                + doc_join(['{}: {}'.format(self.namer.get_name(v), self(v.type)) for v in e.parameters], NewLine())
+                + doc_join(['{}: {}'.format(self.namer.get_name(v), self(v.type)) for v in e.params], NewLine())
             ).indent(),
             Text('inputs: ') + '[' + doc_join([self.namer.get_name(v) for v in e.inputs], ', ') + ']',
             Text('outputs: ') + '[' + doc_join([self.namer.get_name(v) for v in e.outputs], ', ') + ']',
             Text('computations: ') + self.print_tensor_nodes(e.outputs).indent(),
-            Text('attributes: {') + self({k: str(v) for k, v in e.attributes.items()}) + '}',
+            Text('attributes: {') + self({k: str(v) for k, v in e.attrs.items()}) + '}',
         ]
-        if len(e.task_graph.nodes) > 1:
-            lines.append(Text('task_graph: ') + self(e.task_graph))
         front_part = doc_join(lines, NewLine())
         inverse_map_doc = Doc()
         if e.inverse_map:
             inverse_map_doc += NewLine() + Text('inverse_map:')
             for tensor, inverse_map in e.inverse_map.items():
                 inverse_map_body = 'InverseMap([' + self(inverse_map.axes) + '] => [' + self(inverse_map.indices) + '])'
                 inverse_map_doc += (NewLine() + self.namer.get_name(tensor) + ': ' + inverse_map_body).indent()
         return Text('Task(') + (NewLine() + front_part + inverse_map_doc).indent() + NewLine() + ')'
 
-    def visit_TaskGraph(self, task_graph: TaskGraph):
-        head = Text('TaskGraph(') + self(task_graph.input_tensors) + ') {'
-        body = []
-        for task in task_graph.nodes:
-            arg_items = []
-            for task_input in task.inputs:
-                if task_input in task_graph.consume:
-                    arg_items.append(self(task_input) + '=' + self(task_graph.consume[task_input]))
-                else:
-                    arg_items.append(self(task_input))
-            for name, value in task.attributes.items():
-                arg_items.append(self(name) + '=' + self(str(value)))
-            args = doc_join(arg_items, ', ')
-            assign_line = self(task.outputs) + ' = ' + task.name + '(' + args + ')'
-            if task is task_graph.anchor:
-                assign_line = assign_line + ' [anchor]'
-            if task is task_graph.anchor:
-                compute_body = Doc()
-            else:
-                compute_body = self.print_tensor_nodes(task.outputs, exclude_nodes=task.inputs).indent()
-            body.append(assign_line + compute_body)
-
-        body.append(
-            'return '
-            + self([task_graph.consume[v] if v in task_graph.consume else v for v in task_graph.output_tensors])
-        )
-
-        body = (NewLine() + doc_join(body, NewLine())).indent()
-        tail = NewLine() + '}'
-        return head + body + tail
-
-    # def visit_InverseMap(self, e: InverseMap):
-    #     return 'InverseMap([' + self(e.axes) + '] => [' + self(e.indices) + '])'
-    #
-    # def visit_ScalarNode(self, e: ScalarNode):
-    #     if e.scalar_compute is None:
-    #         return self.namer.get_name(e, e.name)
-    #     else:
-    #         sc = e.scalar_compute
-    #         if isinstance(sc, ReduceCompute):
-    #             items = [
-    #                 '[' + self(sc.shape) + ']',
-    #                 '(' + self(sc.axes) + ') => ' + self(sc.value),
-    #                 str(sc.reduce_operation),
-    #             ]
-    #             return 'reduce(' + doc_join(items, ', ') + ')'
-    #         elif isinstance(sc, ArgReduceCompute):
-    #             items = [
-    #                 '[' + self(sc.extent) + ']',
-    #                 '' + self(sc.axis) + ' => ' + self(sc.value),
-    #                 str(sc.reduce_operation),
-    #             ]
-    #             return 'arg_reduce(' + doc_join(items, ', ') + ')'
-    #         else:
-    #             raise NotImplementedError()
-
     def visit_TensorNode(self, e: TensorNode):
         return self.namer.get_name(e)
 
     def visit_ScalarInput(self, node: ScalarInput):
         return self.namer.get_name(node)
 
     def visit_TensorInput(self, node: TensorInput):
@@ -531,29 +453,14 @@
         items = ['[' + self(c.shape) + ']', '(' + self(c.axes) + ') => ' + self(c.value), str(c.reduce_operation)]
         return 'reduce(' + doc_join(items, ', ') + ')'
 
     def visit_ArgReduceCompute(self, c: ArgReduceCompute):
         items = ['[' + self(c.extent) + ']', self(c.axis) + ' => ' + self(c.value), str(c.reduce_operation)]
         return 'arg_reduce(' + doc_join(items, ', ') + ')'
 
-    #
-    # def visit_TaskMapping(self, mapping: TaskMapping):
-    #     if isinstance(mapping, (RepeatTaskMapping, SpatialTaskMapping)):
-    #         name = 'repeat' if isinstance(mapping, RepeatTaskMapping) else 'spatial'
-    #         args = [self(mapping.task_shape)]
-    #         if not same_list(mapping.ranks, list(range(len(mapping.task_shape)))):
-    #             args.append('ranks=[' + self(mapping.ranks) + ']')
-    #         arg_doc = doc_join(args, ', ')
-    #         # something like: spatial(1, 3, ranks=[1, 0])
-    #         return doc_join([name, '(', arg_doc, ')'], '')
-    #     elif isinstance(mapping, ComposedTaskMapping):
-    #         return self(mapping.outer) + '.' + self(mapping.inner)
-    #     else:
-    #         raise NotImplementedError()
-
     def visit_SpatialTaskMapping(self, mapping: SpatialTaskMapping):
         items = [self(mapping.task_shape)]
         if not same_list(mapping.ranks, list(range(len(mapping.task_shape)))):
             items.append('ranks=[' + self(mapping.ranks) + ']')
         return 'spatial(' + doc_join(items, ', ') + ')'
 
     def visit_RepeatTaskMapping(self, mapping: RepeatTaskMapping):
@@ -561,14 +468,37 @@
         if not same_list(mapping.ranks, list(range(len(mapping.task_shape)))):
             items.append('ranks=[' + self(mapping.ranks) + ']')
         return 'repeat(' + doc_join(items, ', ') + ')'
 
     def visit_ComposedTaskMapping(self, mapping: ComposedTaskMapping):
         return self(mapping.outer) + '.' + self(mapping.inner)
 
+    def visit_StridesLayout(self, layout: StridesLayout):
+        if isinstance(layout, RowMajorLayout):
+            return Text('row(') + self(layout.shape) + ')'
+        elif isinstance(layout, ColumnMajorLayout):
+            return Text('column(') + self(layout.shape) + ')'
+        else:
+            return Text('strides(') + self(layout.strides) + ')'
+
+    def visit_SwizzleLayout(self, layout: SwizzleLayout):
+        items = [self(layout.base), Text('dim=') + self(layout.dim), Text('regards=') + self(layout.regards_dim)]
+        if layout.log_step != 0:
+            items.append(Text('log_step=') + self(layout.log_step))
+        return Text('swizzle(') + doc_join(items, ', ') + ')'
+
+    def visit_LocalLayout(self, layout: LocalLayout):
+        return Text('local(') + self(layout.shape) + ')'
+
+    def visit_ComposedLayout(self, layout: ComposedLayout):
+        return self(layout.outer) + ' * ' + self(layout.inner)
+
+    def visit_ConcatLayout(self, layout: ConcatLayout):
+        return Text('concat(') + self(layout.lhs) + ', ' + self(layout.rhs) + ')'
+
 
 def astext(obj: Node) -> str:
     if isinstance(obj, Node):
         printer = IRPrinter()
         return str(printer(obj))
     else:
         raise ValueError()
```

## hidet/ir/tools/simplifier.py

```diff
@@ -135,18 +135,18 @@
         body = self(stmt.body)
         if is_one(extent):
             return rewrite(stmt.body, {loop_var: convert(0)})
         else:
             if loop_var is stmt.loop_var and body is stmt.body:
                 return stmt
             else:
-                return ForStmt(loop_var, extent, stmt.unroll, body)
+                return ForStmt(loop_var, extent, body=body, attr=stmt.attr)
 
 
-def simplify(node: Union[Stmt, Expr], repeat_limit=10):
+def simplify(node: Union[Stmt, Expr, int, float], repeat_limit=10):
     if isinstance(node, (int, float)):
         return node
     simplifier = Simplifier()
     for _ in range(repeat_limit):
         old_node = node
         node = simplifier(node)
         if old_node is node:
@@ -154,12 +154,10 @@
     return node
 
 
 def simplify_to_int(node: Union[Expr, int], repeat_limit=10) -> int:
     if isinstance(node, int):
         return node
     node = simplify(node, repeat_limit)
-    assert isinstance(node, Constant) and node.type.name in [
-        'int32',
-        'uint8',
-    ], 'Invalid input. Input type must be one of [int32, uint8].'
+    if not (isinstance(node, Constant) and node.type.is_integer()):
+        raise ValueError('Can not simplify expression {} to an integer'.format(node))
     return node.value
```

## hidet/ir/tools/util_functors.py

```diff
@@ -5,25 +5,20 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Union, Mapping
+from typing import Union
+
 from hidet.ir.expr import Let, Var, Expr
 from hidet.ir.func import Function
-from hidet.ir.stmt import Stmt, ForStmt, LetStmt
-from hidet.ir.functors import StmtVisitor, ExprVisitor, IRVisitor, IRRewriter
-
-
-class MapBasedRewriter(IRRewriter):
-    def __init__(self, rmap):
-        super().__init__()
-        self.memo.update(rmap)
+from hidet.ir.functors import IRVisitor, IRRewriter
+from hidet.ir.stmt import Stmt, LetStmt
 
 
 class IRCollector(IRVisitor):
     def __init__(self, expr_types, stop_when_found=False):
         super().__init__()
         self.expr_types = expr_types
         self.stop_when_found = stop_when_found
@@ -31,54 +26,26 @@
 
     def collect(self, e):
         self.exprs.clear()
         self.visit(e)
         return self.exprs
 
     def visit(self, node):
-        if node in self.memo:
-            return self.memo[node]
+        key = id(node) if isinstance(node, (list, dict)) else node
+        if key in self.memo:
+            return self.memo[key]
 
         if isinstance(node, self.expr_types):
             self.exprs.append(node)
             if self.stop_when_found:
                 self.memo[node] = None
                 return None
         return super().visit(node)
 
 
-class FreeVarCollector(StmtVisitor, ExprVisitor):
-    def __init__(self):
-        super().__init__()
-        self.defined = set()
-        self.free_vars = set()
-
-    def collect(self, e):
-        self.defined.clear()
-        self.visit(e)
-        return self.free_vars
-
-    def visit_LetStmt(self, stmt: LetStmt):
-        for bind_var, bind_value in zip(stmt.bind_vars, stmt.bind_values):
-            self.visit(bind_value)
-            self.defined.add(bind_var)
-        self.visit(stmt.body)
-        for bind_var in stmt.bind_vars:
-            self.defined.remove(bind_var)
-
-    def visit_ForStmt(self, stmt: ForStmt):
-        self.defined.add(stmt.loop_var)
-        super().visit_ForStmt(stmt)
-        self.defined.remove(stmt.loop_var)
-
-    def visit_Var(self, e: Var):
-        if e not in self.defined:
-            self.free_vars.add(e)
-
-
 class CloneRewriter(IRRewriter):
     def clone(self, obj: Union[Stmt, Expr]):
         return self(obj)
 
     def visit_LetStmt(self, stmt: LetStmt):
         bind_vars = []
         bind_values = []
@@ -90,20 +57,14 @@
 
     def visit_Let(self, e: Let):
         v = Var(e.var.hint, e.var.type)
         self.memo[e.var] = v
         return Let(v, self(e.value), self(e.body))
 
 
-def rewrite(node: Union[Function, Expr, Stmt, tuple], rewrite_map: Mapping[Union[Stmt, Expr], Union[Stmt, Expr]]):
-    assert isinstance(rewrite_map, dict)
-    rewriter = MapBasedRewriter(rewrite_map)
-    return rewriter.rewrite(node)
-
-
 def collect(node: Union[Function, Expr, Stmt, list, tuple], node_types, stop_when_found=False) -> list:
     """
     Collect sub-nodes in given node with specific types.
 
     Parameters
     ----------
     node: Union[Function, Expr, Stmt, list, tuple]
@@ -132,12 +93,7 @@
     collector = IRCollector(node_types, stop_when_found)
     collected = collector.collect(node)
     return collected
 
 
 def clone(node: Union[Stmt, Expr]) -> Union[Stmt, Expr]:
     return CloneRewriter()(node)
-
-
-def collect_free_vars(node: Union[Expr, Stmt]):
-    collector = FreeVarCollector()
-    return collector.collect(node)
```

## hidet/ir/utils/__init__.py

```diff
@@ -8,13 +8,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from . import call_graph
 from . import hash_sum
 from . import index_transform
-from . import task_utils
 from . import expr_utils
 
 from .index_transform import index_serialize, index_deserialize
-from .task_utils import validate_schedule
 from .expr_utils import as_expr
```

## hidet/ir/utils/call_graph.py

```diff
@@ -28,15 +28,15 @@
 
     def add_callee(self, callee):
         if callee not in self.callees:
             self.callees.append(callee)
 
 
 class CallGraph:
-    def __init__(self, ir_module: IRModule):
+    def __init__(self, ir_module: IRModule, allow_missing: bool = False):
         # pylint: disable=import-outside-toplevel
         from hidet.ir.primitives import is_primitive_function, lookup_primitive_function
 
         self.nodes: List[CallGraphNode] = []
         self.func2node = {}
 
         self.order: List[CallGraphNode] = []  # topological order, from caller to callee
@@ -50,14 +50,16 @@
         for func in ir_module.functions.values():
             caller = func
             for call in collect(func.body, Call):
                 if is_primitive_function(call.func_var.hint):
                     entry = lookup_primitive_function(call.func_var.hint)
                     if entry.function is not None:
                         name = call.func_var.hint
+                        if name not in ir_module.functions and allow_missing:
+                            continue
                         callee = ir_module.lookup(name)
                     else:
                         continue
                 else:
                     callee = ir_module.lookup(call.func_var.hint)
                 self._add_edge(caller, callee)
```

## hidet/lang/__init__.py

```diff
@@ -7,15 +7,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Union, Sequence, Optional, List
 from hidet.ir.type import TypeNode, DataType, TensorType, PointerType, VoidType, ReferenceType, void_p, data_type
-from hidet.ir.expr import Expr, Var, cast, view, Dereference
+from hidet.ir.expr import Expr, Var, cast, view, address, Dereference
 from hidet.ir.mapping import row_spatial, row_repeat, col_repeat, col_spatial, TaskMapping, auto_map
 from hidet.ir.layout import DataLayout
 from hidet.ir.primitives import printf
 from hidet.lang.script import script, script_module
 from hidet.ir.stmt import asm, DeclareScope
 from hidet.ir.func import Function
 from hidet.lang.type_utils import static, with_scope
@@ -61,15 +61,31 @@
     dtype: Union[DataType, str],
     shape: Optional[Sequence[ConstExpr]] = None,
     layout: Optional[DataLayout] = None,
 ) -> Expr:
     return cast(expr, tensor_pointer(dtype, shape, layout))
 
 
-def grid(*dim_extents):
+def grid(*dim_extents, attrs: Optional[str] = None):
+    """
+    Iterate over the grid.
+
+    Parameters
+    ----------
+    dim_extents: Sequence[Expr or int]
+        The length of each dimension.
+
+    attrs: Optional[str]
+        The attributes of each loop. See ForStmtAttr for more information.
+
+    Returns
+    -------
+    indices: Sequence[Tuple[Expr, ...]]
+        The sequence of indices in the grid to be iterated.
+    """
     raise ValueError('Please call this function within the @hidet.script decorated function.')
 
 
 def deref(addr: Expr):
     return Dereference(addr)
```

## hidet/lang/transpiler.py

```diff
@@ -38,27 +38,27 @@
 from ast import Not, And, Or, Eq, NotEq, Lt, LtE, Gt, GtE
 
 from ast import Index
 
 import astunparse
 from hidet import ir
 from hidet.ir.expr import Var
-from hidet.ir.stmt import DeclareScope
+from hidet.ir.stmt import DeclareScope, ForStmtAttr
 from hidet.ir.tools import simplify
 from hidet.ir.builders import FunctionBuilder
 from hidet.utils import red, bold, blue, str_indent
 import hidet.lang.attr
 from hidet.lang.type_utils import TypeDecorator
 
 
 class HidetProgramError(Exception):
     def __init__(
         self,
         translator: PythonAstFunctor,
-        obj: Union[ast.AST, ast.expr, ast.arg, ast.stmt, ast.Attribute, ast.Name],
+        obj: Union[ast.AST, ast.expr, ast.arg, ast.stmt, ast.Attribute, ast.Name, ast.Call],
         msg: str,
     ):
         super().__init__()
         self.file = translator.file
         self.lineno = translator.start_lineno + obj.lineno
         self.column = translator.start_column + obj.col_offset
         self.msg = msg
@@ -683,14 +683,16 @@
         return self.visit(expr.value)
 
     def visit_Constant(self, expr: Constant):
         if isinstance(expr.value, (float, int)):
             return expr.value
         elif isinstance(expr.value, str):
             return expr.value
+        elif expr.value is None:
+            return expr.value
         else:
             raise HidetProgramError(self, expr, 'Can not recognize Constant {}'.format(repr(expr.value)))
 
     def visit_For(self, stmt: For):
         # create loop vars
         iter_targets: list[Name] = []
         if isinstance(stmt.target, (List, Tuple)):
@@ -763,34 +765,45 @@
             and self.visit(stmt.iter.func) is hidet.lang.grid
         ):
             # case 2:
             #  for i, j in grid(3, 4):
             #    ...
             # Will be translated to nested for loops (i.e., ForStmt).
             call = stmt.iter
+            attr_string: Optional[str] = None
+            for keyword in call.keywords:
+                if keyword.arg == 'attrs':
+                    assert attr_string is None
+                    attr_string = self.visit(keyword.value)
+                else:
+                    raise HidetProgramError(self, call, 'Can not recognize keyword argument: {}.'.format(keyword.arg))
+            if attr_string is None:
+                attrs = [ForStmtAttr() for _ in range(len(call.args))]
+            else:
+                attrs = ForStmtAttr.parse(attr_string)
             extents = [self.visit(arg) for arg in call.args]
             declare_loop_vars(num=len(extents))
             body = visit_body()
-            for loop_var, extent in zip(reversed(loop_vars), reversed(extents)):
-                body = ir.ForStmt(loop_var=loop_var, extent=extent, body=body)
+            for loop_var, extent, attr in zip(reversed(loop_vars), reversed(extents), reversed(attrs)):
+                body = ir.ForStmt(loop_var=loop_var, extent=extent, body=body, attr=attr)
             self.current_scope.append(body)
         elif isinstance(stmt.iter, Call) and isinstance(stmt.iter.func, Attribute) and stmt.iter.func.attr == 'on':
             # case 3:
             #  for a, b in row_spatial(3, 4).on(thread_x):
             #    ...
             # Will be translated to ForTaskStmt
             if len(stmt.iter.args) != 1:
                 raise HidetProgramError(self, stmt.iter, 'Expect a single expression representing worker index.')
             worker = ir.convert(self.visit(stmt.iter.args[0]))
             mapping = self.visit(stmt.iter.func.value)
             if not isinstance(mapping, ir.TaskMapping):
                 raise HidetProgramError(self, stmt.iter.func.value, 'Expect task mapping here.')
             declare_loop_vars(num=len(mapping.task_shape))
             self.current_scope.append(
-                ir.ForTaskStmt(loop_vars=loop_vars, mapping=mapping, worker=worker, body=visit_body())
+                ir.ForMappingStmt(loop_vars=loop_vars, mapping=mapping, worker=worker, body=visit_body())
             )
         else:
             msg = (
                 'Cannot recognize the for loop statement. Currently, we support two types of for loop statements:\n'
                 '  for i in range(extent):\n'
                 '    body(i)\n'
                 'and\n'
```

## hidet/runtime/storage.py

```diff
@@ -10,15 +10,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 from typing import Callable, Dict, List, Optional, Union
 from collections import defaultdict
 import hidet.cuda
 from hidet.cuda.stream import Stream
-from hidet.utils import green, initialize, exiting
+from hidet.utils import green, exiting
 from hidet.runtime.device import Device, instantiate_device
 
 
 def nbytes2str(nbytes: int) -> str:
     if nbytes > 1024 * 1024:
         size = nbytes // 1024 // 1024
         unit = 'MiB'
@@ -328,26 +328,48 @@
         self.prev_memory_pool = _device2pool[self.device]
         _device2pool[self.device] = self.memory_pool
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         _device2pool[self.device] = self.prev_memory_pool
 
 
-_device2pool: Dict[Device, MemoryPool] = {}
+class DeviceMemoryPools:
+    def __init__(self):
+        self.device2pool: Dict[Device, MemoryPool] = {}
+
+    def __getitem__(self, device: Device) -> MemoryPool:
+        if device not in self.device2pool:
+            if device.is_cuda():
+                self.device2pool[device] = MemoryPool(
+                    CudaMemoryAPI(device), block_size=4096, max_reserve_size=4 * 1024**3
+                )
+            elif device.is_cpu():
+                self.device2pool[device] = MemoryPool(
+                    CpuMemoryAPI(device), block_size=4096, max_reserve_size=512 * 1024**2
+                )
+            else:
+                raise ValueError('Unsupported device: {}'.format(device))
+        return self.device2pool[device]
+
+    def __setitem__(self, device: Device, pool: MemoryPool):
+        self.device2pool[device] = pool
+
+
+_device2pool: DeviceMemoryPools = DeviceMemoryPools()
 
 
-@initialize()
-def initialize_memory_pools():
-    global _device2pool
-    _device2pool = {
-        Device('cpu'): MemoryPool(CpuMemoryAPI(Device('cpu')), block_size=4096, max_reserve_size=512 * 1024**2)
-    }
-    for device_id in range(hidet.cuda.device_count()):
-        device = Device('cuda', device_id)
-        _device2pool[device] = MemoryPool(CudaMemoryAPI(device), block_size=4096, max_reserve_size=4 * 1024**3)
+# @initialize()
+# def initialize_memory_pools():
+#     global _device2pool
+#     _device2pool = {
+#         Device('cpu'): MemoryPool(CpuMemoryAPI(Device('cpu')), block_size=4096, max_reserve_size=512 * 1024**2)
+#     }
+#     for device_id in range(hidet.cuda.device_count()):
+#         device = Device('cuda', device_id)
+#         _device2pool[device] = MemoryPool(CudaMemoryAPI(device), block_size=4096, max_reserve_size=4 * 1024**3)
 
 
 def current_memory_pool(device: Union[Device, str]) -> MemoryPool:
     """
     Get current memory pool for the given device.
 
     All memory allocations on given device will be performed from the returned memory pool. You can change the current
@@ -360,14 +382,12 @@
 
     Returns
     -------
     ret: MemoryPool
         Current memory pool for the given device.
     """
     device = instantiate_device(device)
-    if device not in _device2pool:
-        raise ValueError('No memory pool for device {}'.format(device))
     return _device2pool[device]
 
 
 def memory_pool(pool: MemoryPool):
     return MemoryPoolContext(pool)
```

## hidet/testing/torch_utils.py

```diff
@@ -11,14 +11,15 @@
 # limitations under the License.
 from typing import Sequence
 import numpy.testing
 import torch
 
 
 def check_module(model: torch.nn.Module, args: Sequence[torch.Tensor], atol=1e-4, rtol=1e-4):
+    model = torch.nn.Sequential(model)
     model = model.cuda()
     model.eval()
     args = [x.cuda() for x in args]
     model_opt = torch.compile(model, backend='hidet')
     torch_outputs = model(*args)
     hidet_outputs = model_opt(*args)
     if isinstance(torch_outputs, torch.Tensor):
```

## hidet/testing/utils.py

```diff
@@ -10,17 +10,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Union, Sequence
 import numpy as np
 from hidet.graph.tensor import asarray
 
 
-def check_unary(
-    shape, numpy_op, hidet_op, device: str = 'all', dtype: Union[str, np.dtype] = np.float32, atol=0, rtol=0
-):
+def check_unary(shape, numpy_op, hidet_op, device: str = 'all', dtype=np.float32, atol=0, rtol=0):
     if device == 'all':
         for dev in ['cuda', 'cpu']:
             check_unary(shape, numpy_op, hidet_op, dev, dtype, atol, rtol)
         return
     # wrap np.array(...) in case shape = []
     data = np.array(np.random.randn(*shape)).astype(dtype)
     numpy_result = numpy_op(data)
```

## hidet/transforms/__init__.py

```diff
@@ -13,51 +13,57 @@
 
 from .base import Pass, FunctionPass, FunctionBodyPass, SequencePass, RepeatFunctionPass, PassContext
 from .instruments import PassInstrument, SaveIRInstrument, ProfileInstrument
 
 from .flatten_tensor_slice import flatten_tensor_slice_pass
 from .flatten_tensor_index import flatten_tensor_index_pass
 from .generate_packed_func import generate_packed_func_pass
+from .explicit_unroll import explicit_unroll_pass
 from .import_primitive_functions import import_primitive_functions_pass
 from .simplify_stmt import simplify_stmt_pass
 from .expand_let_expr import expand_let_expr_pass
 from .resolve_generic_primitive_function import resolve_primitive_func_pass
+from .inline_function import inline_function_pass
 from .add_explicit_cast import add_explicit_cast_pass
 from .inline_let_stmt import inline_let_stmt_pass
 from .rule_based_simplifier import rule_based_simplify_pass
 from .normalize_const_tensor import normalize_const_tensor_pass
 from .lower_task_mapping import lower_task_mapping_pass
 from .lower_protect_access import lower_protect_access_pass
 from .declare_to_let import declare_to_let_pass
 from .propogate_launch_bound import propagate_launch_bound_pass
 from .lower_special_cast import lower_special_cast_pass
 
 
 def lower(ir_module: IRModule) -> IRModule:
     transforms = [
         # necessary passes
+        generate_packed_func_pass(),
         flatten_tensor_slice_pass(),
         lower_protect_access_pass(),
         lower_task_mapping_pass(),
         normalize_const_tensor_pass(),
         declare_to_let_pass(),
         rule_based_simplify_pass(),  # make ir more readable
+        explicit_unroll_pass(),
         flatten_tensor_index_pass(),
         lower_special_cast_pass(),
+        inline_function_pass(),
         resolve_primitive_func_pass(),
         import_primitive_functions_pass(),
         resolve_primitive_func_pass(),
         import_primitive_functions_pass(),
         propagate_launch_bound_pass(),
         add_explicit_cast_pass(),
         declare_to_let_pass(),
         # simplification
         expand_let_expr_pass(),
         inline_let_stmt_pass(inline_all=False),
         rule_based_simplify_pass(),
+        inline_let_stmt_pass(inline_all=False),
         simplify_stmt_pass(),
     ]
 
     ctx = PassContext.current()
     for instrument in ctx.instruments:
         instrument.before_all_passes(ir_module)
     for transform in transforms:
```

## hidet/transforms/flatten_tensor_index.py

```diff
@@ -5,36 +5,37 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from hidet.ir.type import TensorType, tensor_type, PointerType, TensorPointerType
+from hidet.ir.type import TensorType, tensor_type, tensor_pointer_type, PointerType, TensorPointerType
 from hidet.ir.expr import Var, TensorElement, TensorSlice, Constant
 from hidet.ir.stmt import BufferStoreStmt, DeclareStmt
 from hidet.ir.func import Function
 from hidet.ir.functors import IRRewriter
-from hidet.ir.tools import simplify_to_int
+from hidet.ir.tools import simplify
 from hidet.transforms import Pass
 from hidet.ir.layout import StridesLayout, DataLayout
 
 
 class FlattenTensorAccessRewriter(IRRewriter):
     # flatten all high-dimension tensor access
     # A = int[3, 4]
     #   TensorElement:  A[2, 1]     ==> A[2 * 4 + 1]
     # BufferStoreStmt:  A[2, 1] = 3 ==> A[2 * 4 + 1] = 3
     def visit_Function(self, func: Function):
         for var in func.params:
             if isinstance(var.type, TensorType):
-                size = simplify_to_int(var.type.layout.size)
-                self.memo[var] = Var(var.hint, tensor_type(var.type.dtype, [size], DataLayout.row_major([size])))
+                size = simplify(var.type.layout.size)
+                self.memo[var] = Var(var.hint, tensor_pointer_type(var.type.dtype, [size]))
             elif isinstance(var.type, TensorPointerType):
-                self.memo[var] = var
+                size = simplify(var.type.tensor_type.layout.size)
+                self.memo[var] = Var(var.hint, tensor_pointer_type(var.type.tensor_type.dtype, [size]))
         body = self(func.body)
         params = [self(p) for p in func.params]
         return Function(
             func.name, params, body, func.ret_type, kind=func.kind, extern_vars=func.extern_vars, attrs=func.attrs
         )
 
     @staticmethod
@@ -48,15 +49,15 @@
                 return StridesLayout(shape=[0], strides=[1])
         elif isinstance(e, Constant) and isinstance(e.type, TensorType):
             return e.type.layout
         raise ValueError("Can not infer layout from '{}' (expression {})".format(type(e), e))
 
     def visit_DeclareStmt(self, stmt: DeclareStmt):
         if isinstance(stmt.var.type, TensorType):
-            size = simplify_to_int(stmt.var.type.layout.size)
+            size = simplify(stmt.var.type.layout.size)
             var = Var(stmt.var.hint, tensor_type(stmt.var.type.dtype, [size], DataLayout.row_major([size])))
             self.memo[stmt.var] = var
             init = self(stmt.init) if stmt.init is not None else None
             return DeclareStmt(var, init, scope=stmt.scope)
         else:
             return IRRewriter.visit_DeclareStmt(self, stmt)
```

## hidet/transforms/generate_packed_func.py

```diff
@@ -5,91 +5,133 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from hidet.ffi import ArgType
-from hidet.ir.type import DataType, TensorType, VoidType, PointerType, TensorPointerType, data_type
-from hidet.ir.expr import Var, Call, Equal, Cast, Dereference
-from hidet.ir.stmt import AssertStmt
-from hidet.ir.func import IRModule, Function
-from hidet.ir.tools import astext, simplify_to_int
-from hidet.ir.builders import FunctionBuilder, StmtBuilder
+from typing import Dict, Tuple, Sequence, Union
+from hidet.ffi.packedfunc import ArgTypeCode
+from hidet.ir.func import Function, IRModule
+from hidet.ir.type import DataType, TensorType, TensorPointerType, PointerType
+from hidet.ir.dtypes import int32
+from hidet.ir.expr import Expr, Var, Call, Constant
+from hidet.ir.stmt import Stmt, AssertStmt, LaunchKernelStmt, DeclareStmt
+from hidet.ir.tools import rewrite, simplify
+from hidet.ir.builders import StmtBuilder
 from hidet.transforms import Pass
-from hidet.ir.primitives import set_kernel_max_dynamic_smem_bytes
+
+
+def _normalize_dim3(dim3: Union[int, Expr, Sequence[Union[int, Expr]]]) -> Tuple[Expr, Expr, Expr]:
+    if isinstance(dim3, int):
+        return int32(dim3), int32(1), int32(1)
+    elif isinstance(dim3, Expr):
+        return simplify(dim3), int32(1), int32(1)
+    elif isinstance(dim3, Sequence):
+        dim3 = [simplify(int32(v)) for v in dim3]
+        assert len(dim3) <= 3
+        while len(dim3) < 3:
+            dim3.append(int32(1))
+        return dim3[0], dim3[1], dim3[2]
+    else:
+        raise TypeError('Unsupported type: {}'.format(type(dim3)))
+
+
+def _rewrite_dim3(dim3: Tuple[Expr, Expr, Expr], param2arg: Dict[Expr, Expr]) -> Tuple[Expr, Expr, Expr]:
+    return rewrite(dim3[0], param2arg), rewrite(dim3[1], param2arg), rewrite(dim3[2], param2arg)
+
+
+def add_packed_func(ir_module: IRModule, func: Function, pack_func_name: str):
+    from hidet import lang
+    from hidet.lang import attr, i32, void_p, deref, cast
+    from hidet.lang.cuda import set_kernel_max_dynamic_smem_bytes
+
+    func_var = ir_module.lookup_var(func.name)
+
+    def extract_params_and_call(num_args: Expr, arg_types: Expr, args: Expr) -> Stmt:
+        sb = StmtBuilder()
+        sb += AssertStmt(num_args == len(func.params), 'Expect {} arguments'.format(len(func.params)))
+        param2arg: Dict[Var, Var] = {}
+        for idx, param in enumerate(func.params):
+            assert isinstance(param, Var)
+            if isinstance(param.type, DataType):
+                name2code = {'int32': ArgTypeCode.INT32, 'float32': ArgTypeCode.FLOAT32, 'float16': ArgTypeCode.FLOAT16}
+                if param.type.name not in name2code:
+                    raise NotImplementedError('Unsupported scalar type: {}'.format(param.type.name))
+                code: ArgTypeCode = name2code[param.type.name]
+                arg: Expr = deref(cast(args[idx], ~param.type))
+                arg_var: Var = Var(param.hint, param.type)
+            elif isinstance(param.type, TensorType):
+                code: ArgTypeCode = ArgTypeCode.POINTER
+                arg: Expr = cast(args[idx], ~param.type.dtype)
+                arg_var: Var = Var(param.hint, ~param.type.dtype)
+            elif isinstance(param.type, TensorPointerType):
+                code: ArgTypeCode = ArgTypeCode.POINTER
+                arg: Expr = cast(args[idx], ~param.type.tensor_type.dtype)
+                arg_var: Var = Var(param.hint, ~param.type.tensor_type.dtype)
+            elif isinstance(param.type, PointerType):
+                code: ArgTypeCode = ArgTypeCode.POINTER
+                arg: Expr = cast(args[idx], param.type)
+                arg_var: Var = Var(param.hint, param.type)
+            else:
+                raise NotImplementedError('Unsupported type: {}'.format(param.type))
+            param2arg[param] = arg_var
+            sb += AssertStmt(arg_types[idx] == code.value, 'The {}-th argument should be {}'.format(idx, param.type))
+            sb += DeclareStmt(arg_var, init=arg)
+
+        if func.kind == 'cuda_kernel':
+            smem_bytes: Union[Expr, int] = simplify(func.get_attr('cuda_dynamic_smem_bytes', 0))
+            if isinstance(smem_bytes, (int, Constant)):
+                # compiled-time known size of shared memory
+                if int(smem_bytes) > 48 * 1024:
+                    sb += set_kernel_max_dynamic_smem_bytes(func_var, smem_bytes)
+            else:
+                # run-time known size of shared memory
+                smem_bytes = rewrite(smem_bytes, param2arg)
+                with sb.if_then(smem_bytes > 48 * 1024):
+                    sb += set_kernel_max_dynamic_smem_bytes(func_var, smem_bytes)
+            sb += LaunchKernelStmt(
+                func_var,
+                [param2arg[param] for param in func.params],
+                grid_dim=_rewrite_dim3(_normalize_dim3(func.get_attr('cuda_grid_dim')), param2arg),
+                block_dim=_rewrite_dim3(_normalize_dim3(func.get_attr('cuda_block_dim')), param2arg),
+                shared_mem=smem_bytes,
+            )
+        elif func.kind == 'host_kernel':
+            sb += Call(func_var, [param2arg[param] for param in func.params])
+        else:
+            raise NotImplementedError('Unsupported function kind: {}'.format(func.kind))
+        return sb.finish()
+
+    with lang.script_module():
+
+        @lang.script
+        def packed_func(num_args: i32, arg_types: ~i32, args: ~void_p):
+            attr.func_name = pack_func_name
+            attr.func_kind = 'packed_func'
+            attr.packed_func = func_var
+            extract_params_and_call(num_args, arg_types, args)
+
+    assert isinstance(packed_func, Function)
+    ir_module.add(packed_func.name, packed_func)
 
 
 class GeneratePackedFuncPass(Pass):
     def process_module(self, ir_module: IRModule) -> IRModule:
-        new_ir_module = IRModule(task=ir_module.task)
-        for func in ir_module.functions.values():
-            new_ir_module.add(func.name, func)
-            if func.kind not in ['cuda_kernel', 'host_kernel']:
-                # only generate packed func for entry function
-                continue
-            if func.get_attr('packed_func', allow_missing=True) is not None:
-                # this function itself is a packed function
-                continue
-            if any(
-                f.get_attr('packed_func', allow_missing=True) is ir_module.lookup_var(func.name)
-                for f in ir_module.functions.values()
-            ):
-                # the packed function for current function has existed, skip
-                continue
-            if not func.name.endswith('_grid') and not func.name.endswith('_host'):
-                continue
-            packed_func = self.generate_packed_func(func, ir_module.lookup_var(func.name))
-            new_ir_module.add(packed_func.name, packed_func)
-        return new_ir_module
-
-    def generate_packed_func(self, func: Function, func_global_var: Var) -> Function:
-        assert isinstance(func.ret_type, VoidType)
-        assert isinstance(func.name, str) and (func.name.endswith('_grid') or func.name.endswith('_host'))
-        packed_name = func.name[:-5]
-        with FunctionBuilder(name=packed_name, kind='packed_func', attrs={'packed_func': func_global_var}) as fb:
-            # params
-            p_num_args = Var('num_args', data_type('int32'))
-            p_arg_types = Var('arg_types', PointerType(data_type('int32')))
-            p_args = Var('args', PointerType(PointerType(VoidType())))
-            fb.extend_params([p_num_args, p_arg_types, p_args])
-
-            # body
-            sb = StmtBuilder()
-            sb += AssertStmt(Equal(p_num_args, len(func.params)), "expect {} args".format(len(func.params)))
-            func_args = []
-            for idx, param in enumerate(func.params):
-                assert isinstance(param, Var)
-                if isinstance(param.type, DataType):
-                    if param.type.name == 'int32':
-                        code: ArgType = ArgType.INT32
-                    elif param.type.name == 'float32':
-                        code: ArgType = ArgType.FLOAT32
-                    else:
-                        raise NotImplementedError()
-                    func_args.append(Dereference(Cast(p_args[idx], PointerType(param.type))))
-                elif isinstance(param.type, (TensorPointerType, TensorType)):
-                    code: ArgType = ArgType.POINTER
-                    if isinstance(param.type, TensorType):
-                        dtype = param.type.dtype
-                    else:
-                        dtype = param.type.tensor_type.dtype
-                    func_args.append(Cast(p_args[idx], PointerType(dtype)))
-                elif isinstance(param.type, PointerType):
-                    code: ArgType = ArgType.POINTER
-                    func_args.append(Cast(p_args[idx], param.type))
-                else:
-                    raise NotImplementedError()
-                sb += AssertStmt(
-                    Equal(p_arg_types[idx], code), "The {} th arg should be {}".format(idx + 1, astext(param.type))
-                )
-            if func.kind == 'cuda_kernel' and simplify_to_int(func.get_attr('cuda_dynamic_smem_bytes', 0)) > 48 * 1024:
-                dynamic_smem_bytes = simplify_to_int(func.get_attr('cuda_dynamic_smem_bytes', 0))
-                sb += set_kernel_max_dynamic_smem_bytes(func_global_var, dynamic_smem_bytes)
-            sb += Call(func_global_var, func_args)
-            fb.set_body(sb.finish())
-        return fb.get()
+        if 'launch' in ir_module.functions:
+            # the launch function has already existed
+            return ir_module
+        kernel_functions: Dict[str, Function] = {
+            name: func for name, func in ir_module.functions.items() if func.kind in ['cuda_kernel', 'host_kernel']
+        }
+        if len(kernel_functions) == 0:
+            # no kernel function found in the module, do nothing
+            return ir_module
+        if len(kernel_functions) > 1:
+            raise NotImplementedError('Can only handle one kernel function in a module')
+        func = next(iter(kernel_functions.values()))
+        add_packed_func(ir_module, func, 'launch')
+        return ir_module
 
 
-def generate_packed_func_pass():
+def generate_packed_func_pass() -> Pass:
     return GeneratePackedFuncPass()
```

## hidet/transforms/inline_let_stmt.py

```diff
@@ -21,18 +21,18 @@
 
 class LetVarRefAnalyzer(IRVisitor):
     def __init__(self):
         super().__init__(use_memo=False)
         self.usage_count = None
         self.var2value = None
 
-    def analyze(self, expr):
+    def analyze(self, stmt):
         self.usage_count = defaultdict(int)
         self.var2value = {}
-        self.visit(expr)
+        self.visit(stmt)
 
     def visit(self, node):
         if isinstance(node, Var):
             self.usage_count[node] += 1
         return IRVisitor.visit(self, node)
 
     def visit_LetStmt(self, stmt: LetStmt):
```

## hidet/transforms/lower_task_mapping.py

```diff
@@ -6,16 +6,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Dict, Sequence, Union, Optional
-import itertools
-from hidet.ir import Var, ForTaskStmt, Stmt, ForStmt, Expr, SeqStmt
+from hidet.ir import Var, ForMappingStmt, Stmt, ForStmt, Expr, SeqStmt
 from hidet.ir.expr import var
 from hidet.ir.mapping import TaskMapping, SpatialTaskMapping, RepeatTaskMapping, ComposedTaskMapping
 from hidet.transforms.base import Pass, FunctionBodyPass
 from hidet.ir.functors import IRRewriter
 from hidet.ir.tools import rewrite, simplify
 from hidet.utils import prod
 
@@ -65,35 +64,24 @@
         for extent, stride in zip(mapping.task_shape, strides):
             task.append(worker // stride % extent)
         return [task]
 
     def visit_Repeat(self, mapping: RepeatTaskMapping, worker: Expr) -> List[TaskIndex]:
         # pylint: disable=unused-argument
         # worker is unused because there is only a single worker with index 0
-        unroll = False
-        if unroll:
-
-            def global_index(task: Sequence[int], strides: Sequence[int]) -> int:
-                return sum(a * b for a, b in zip(task, strides))
-
-            strides = strides_from_ranks(shape=mapping.task_shape, ranks=mapping.ranks)
-            ranges = [range(s) for s in mapping.task_shape]
-            tasks = list(tuple(task) for task in itertools.product(*ranges))
-            tasks = sorted(tasks, key=lambda task: global_index(task, strides))
-            return [list(task) for task in tasks]
-        else:
-            num_loops = len(mapping.task_shape)
-            task: List[Optional[Var]] = [None for _ in range(num_loops)]
-            for i in range(num_loops):
-                dim = mapping.ranks.index(i)
-                extent = simplify(mapping.task_shape[dim])
-                loop_var = var('i')
-                self.loop_nests.append(ForStmt(loop_var=loop_var, extent=extent))
-                task[dim] = loop_var
-            return [task]
+        num_loops = len(mapping.task_shape)
+        task: List[Optional[Var]] = [None for _ in range(num_loops)]
+        for i in range(num_loops):
+            dim = mapping.ranks.index(i)
+            extent = simplify(mapping.task_shape[dim])
+            attr = mapping.attrs[dim]
+            loop_var = var('i')
+            self.loop_nests.append(ForStmt(loop_var=loop_var, extent=extent, attr=attr))
+            task[dim] = loop_var
+        return [task]
 
     def visit_Composed(self, mapping: ComposedTaskMapping, worker: Expr) -> List[TaskIndex]:
         outer, inner = mapping.outer, mapping.inner
         outer_worker, inner_worker = worker // inner.num_workers, worker % inner.num_workers
         outer_tasks = self.visit(outer, outer_worker)
         inner_tasks = self.visit(inner, inner_worker)
         tasks = []
@@ -101,15 +89,15 @@
             for inner_task in inner_tasks:
                 task = [a * inner.task_shape[i] + b for i, (a, b) in enumerate(zip(outer_task, inner_task))]
                 tasks.append(task)
         return tasks
 
 
 class LowerTaskMappingRewriter(IRRewriter):
-    def visit_ForTaskStmt(self, stmt: ForTaskStmt):
+    def visit_ForTaskStmt(self, stmt: ForMappingStmt):
         body = self.visit(stmt.body)
         expander = TaskMappingExpander()
         return expander.expand(mapping=stmt.mapping, worker=stmt.worker, loop_vars=stmt.loop_vars, body=body)
 
 
 class LowerTaskMappingPass(FunctionBodyPass):
     def process_body(self, stmt: Stmt) -> Stmt:
```

## hidet/transforms/rule_based_simplifier.py

```diff
@@ -10,28 +10,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import operator
 from typing import Dict
 from itertools import product
 
 from hidet.ir.dialects.pattern import AnyExpr, match
-from hidet.ir.expr import (
-    Add,
-    convert,
-    Sub,
-    Multiply,
-    Mod,
-    LessThan,
-    LessEqual,
-    Equal,
-    BinaryOp,
-    LogicalAnd,
-    IfThenElse,
-    LogicalOr,
-)
+from hidet.ir.expr import Add, convert, Sub, Multiply, Mod, LessThan, LessEqual, Equal, BinaryOp, LogicalAnd, IfThenElse
+from hidet.ir.expr import LogicalOr, BitwiseXor, BitwiseAnd, BitwiseOr, BitwiseNot
 from hidet.ir.expr import Div, Constant, Expr
 from hidet.ir.functors import IRRewriter
 from hidet.ir.tools import rewrite
 from hidet.transforms.base import FunctionPass
 from hidet.utils import prod, repeat_until_converge
 from hidet.ir.func import Function
 from hidet.ir.analyzers import BoundAnalyzer, BoundInfo
@@ -57,14 +45,18 @@
 
 class ConstExprSimplifier(IRRewriter):
     op_dict = {
         Add: operator.add,
         Sub: operator.sub,
         Multiply: operator.mul,
         Div: c_div,
+        BitwiseOr: operator.or_,
+        BitwiseAnd: operator.and_,
+        BitwiseXor: operator.xor,
+        BitwiseNot: operator.invert,
         Mod: operator.mod,
         LessThan: operator.lt,
         LessEqual: operator.le,
         Equal: operator.eq,
     }
 
     def visit_Binary(self, e: BinaryOp):
@@ -113,14 +105,15 @@
         self.args = {e1, e2, c1, c2, ec1, ec2}
         self.patterns = [
             (e1 + zero, e1),
             (e1 - zero, e1),
             (e1 * one, e1),
             (e1 * zero, zero),
             (e1 // one, e1),
+            (e1 ^ zero, e1),
             # add
             ((c1 + e1) + e2, (e1 + e2) + c1),
             ((e1 + c1) + c2, e1 + (c1 + c2)),
             ((c1 - e1) + e2, (e2 - e1) + c1),
             ((e1 - c1) + e2, (e1 + e2) - c1),
             # sub
             ((c1 + e1) - e2, (e1 - e2) + c1),
```

## hidet/transforms/common/scope.py

```diff
@@ -135,14 +135,14 @@
             )
 
     def visit_ForStmt(self, stmt: ForStmt):
         with self.new_scope(stmt) as scope:
             self.visit(stmt.extent)
             scope.declare(stmt.loop_var)
             body = scope.wrap(self.visit(stmt.body))
-            return ForStmt(stmt.loop_var, stmt.extent, stmt.unroll, body)
+            return ForStmt(stmt.loop_var, stmt.extent, body=body, attr=stmt.attr)
 
     def visit_LetStmt(self, stmt: LetStmt):
         with self.new_scope(stmt) as scope:
             for var, value in zip(stmt.bind_vars, stmt.bind_values):
                 scope.define(var, self.visit(value))
             return scope.wrap(self.visit(stmt.body))
```

## hidet/utils/__init__.py

```diff
@@ -14,13 +14,13 @@
 from . import py
 from . import netron
 from . import transformers_utils
 from . import structure
 from . import stack_limit
 
 from .py import prod, Timer, repeat_until_converge, COLORS, get_next_file_index, factorize, HidetProfiler, TableBuilder
-from .py import same_list, strict_zip, initialize, gcd, lcm, error_tolerance, green, red, cyan, bold, blue
+from .py import same_list, strict_zip, index_of, initialize, gcd, lcm, error_tolerance, green, red, cyan, bold, blue
 from .py import str_indent, unique
 from .bench import benchmark_func
 from .structure import DirectedGraph
 from .cache_utils import hidet_cache_dir, hidet_cache_file, hidet_clear_op_cache
 from .net_utils import download
```

## hidet/utils/py.py

```diff
@@ -244,14 +244,24 @@
                 return False
         else:
             if l is not r:
                 return False
     return True
 
 
+def index_of(value: object, lst: Sequence, allow_missing=True) -> int:
+    for i, v in enumerate(lst):
+        if v is value:
+            return i
+    if allow_missing:
+        return -1
+    else:
+        raise ValueError('value not found in list')
+
+
 class HidetProfiler:
     def __init__(self, display_on_exit=True):
         self.pr = cProfile.Profile()
         self.display_on_exit = display_on_exit
 
     def __enter__(self):
         self.pr.enable()
```

## Comparing `hidet/graph/ops/definitions/utils.py` & `hidet/graph/ops/definitions/utils/tensor_utils.py`

 * *Files identical despite different names*

## Comparing `hidet/graph/ops/schedules/tune.py` & `hidet/graph/ops/definitions/utils/tune.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 from typing import Union, Sequence, TypeVar, Any, Dict, List, Optional
 import os
 import itertools
 import shutil
 from tqdm import tqdm
 import numpy as np
 from hidet.ir.func import IRModule
-from hidet.ir.task import Task
 import hidet.option
 from hidet.utils import prod
-from .resolve import dummy_inputs_from_task
 
 Choice = TypeVar('Choice')
 
 
 class ScheduleError(Exception):
     pass
 
@@ -86,15 +84,15 @@
         tuning_space: TuningSpace = getattr(func, '_tuning_space')
         tuning_space.add_sub_space(level, names, choices)
         return func
 
     return wrapper
 
 
-def _generate_summary(kwargs_list: List[Dict[str, Any]], latencies: List[float]) -> str:
+def _generate_summary(kwargs_list: Sequence[Dict[str, Any]], latencies: Sequence[float]) -> str:
     # sort by latency
     indices, kwargs_list, latencies = zip(
         *sorted(zip(range(len(latencies)), kwargs_list, latencies), key=lambda x: x[-1])
     )
 
     # generate summary column by column
     columns = []
@@ -108,56 +106,60 @@
     for column, width in zip(columns, column_widths):
         justified_columns.append([v.ljust(width) for v in column])
     summary = '\n'.join(''.join(row_items) for row_items in zip(*justified_columns))
 
     return summary
 
 
-def tune(template_func, task: Task, target_device: str, working_dir: str) -> IRModule:
-    from hidet.driver import build_ir_module_batch
-    from hidet.runtime import CompiledFunction
-
+def extract_ir_modules(template_func) -> List[IRModule]:
     # get ir modules to tune
     if hasattr(template_func, '_tuning_space'):
         tuning_space: TuningSpace = getattr(template_func, '_tuning_space')
         # iterate space and instantiate schedules into tensor programs
         kwargs_list = list(tuning_space.iterate_space(hidet.option.get_search_space()))
     else:
         raise ValueError(
             'No tuning space is attached to the template function.\n'
             'Please use @tune.space to decorate the template function to define the search space.'
         )
 
     ir_modules = []
-    ir_modules_kwargs = []
     for kwargs in kwargs_list:
         try:
-            ir_modules.append(template_func(**kwargs))
-            ir_modules_kwargs.append(kwargs)
+            ir_module = template_func(**kwargs)
+            ir_modules.append(ir_module)
+            setattr(ir_module, '_tuning_kwargs', kwargs)  # workaround to pass kwargs to the tune function
         except ScheduleError:
             # the schedule is invalid, skip it
             continue
+    return ir_modules
+
+
+def tune(ir_modules: Sequence[IRModule], dummy_inputs: Sequence[Any], working_dir: str) -> IRModule:
+    from hidet.driver import build_ir_module_batch
+    from hidet.runtime import CompiledFunction
+
+    ir_modules = list(ir_modules)
 
     if len(ir_modules) == 0:
         raise ValueError('No valid schedule is found.')
     elif len(ir_modules) == 1:
         # do not need to tune
         return ir_modules[0]
 
     # build ir modules into compiled functions
     tuning_dir = os.path.join(working_dir, 'tuning')
     compiled_funcs: List[Optional[CompiledFunction]] = build_ir_module_batch(
-        ir_modules, func_name=task.name, output_dir=tuning_dir, parallel=True, verbose=True
+        ir_modules, output_dir=tuning_dir, parallel=True, verbose=True
     )
     assert len(compiled_funcs) == len(ir_modules)
     if any(f is None for f in compiled_funcs):
         raise ValueError('All ir modules failed to build.')
 
     # benchmark
-    dummy_inputs = dummy_inputs_from_task(task, target_device=target_device)
     latencies = []
     warmup, number, repeat = hidet.option.get_option('bench_config')
     for compiled_func in tqdm(compiled_funcs, desc='Benchmarking', total=len(ir_modules), ncols=80):
         if compiled_func:
             repeat_latency = compiled_func.profile(*dummy_inputs, warmup=warmup, number=number, repeat=repeat)
             latency = float(np.median(repeat_latency))
         else:
@@ -166,17 +168,19 @@
         latencies.append(latency)
 
     # remove tuning directory
     if not hidet.option.get_option('debug_cache_tuning'):
         shutil.rmtree(tuning_dir)
 
     # generate summary
-    summary = _generate_summary(ir_modules_kwargs, latencies)
-    with open(os.path.join(working_dir, 'tuning_summary.txt'), 'w') as f:
-        f.write(summary)
+    if all(hasattr(ir_module, '_tuning_kwargs') for ir_module in ir_modules):
+        ir_modules_kwargs = [getattr(ir_module, '_tuning_kwargs') for ir_module in ir_modules]
+        summary = _generate_summary(ir_modules_kwargs, latencies)
+        with open(os.path.join(working_dir, 'tuning_summary.txt'), 'w') as f:
+            f.write(summary)
 
     # select the best schedule and return
     return ir_modules[np.argmin(latencies)]
 
 
 def check(condition: bool, message: str = ""):
     if not condition:
```

## Comparing `hidet/transforms/tools/apply_prologue_epilogue.py` & `hidet/graph/ops/definitions/fusion/apply_prologue_epilogue.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,125 +5,135 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 from hidet.ir.compute import TensorNode, GridCompute, TensorInput
-from hidet.ir.expr import Expr, Var, TensorElement
+from hidet.ir.expr import Expr, Var, TensorElement, tensor_var
 from hidet.ir.stmt import BufferStoreStmt
 from hidet.ir.func import Function, IRModule
-from hidet.ir.task import Task, TaskGraph, InverseMap
+from hidet.ir.task import Task, InverseMap
 from hidet.ir.functors import IRRewriter
 from hidet.ir.tools import rewrite, collect
+from hidet.graph.ir import FlowGraph, Operator, Tensor
 from hidet.utils import strict_zip
+from hidet.transforms.flatten_tensor_slice import FlattenTensorSliceRewriter
+from .fused_operator import FusedTask
 
 
 class PrologueEpilogueRewriter(IRRewriter):
-    def __init__(self, task: Task):
+    def __init__(self, fused_task: FusedTask):
         super().__init__()
-        self.task: Task = task
-        self.task_graph: TaskGraph = task.task_graph
+        self.fused_task: FusedTask = fused_task
+        self.fused_graph: FlowGraph = fused_task.fused_graph
+        self.anchor_operator: Operator = fused_task.fused_graph.nodes[fused_task.anchor]
+        self.anchor_task: Task = self.anchor_operator.task
+        self.anchor_inputs: List[Var] = []
+        self.anchor_outputs: List[Var] = []
+
+        # declare inputs and outputs of the fused function
+        self.graph_params: List[Var] = []
+        self.tensor2var: Dict[Tensor, Var] = {}
+        for tn, tensor in zip(fused_task.tensor_params, self.fused_graph.inputs + self.fused_graph.outputs):
+            var = tensor_var(tn.name, shape=tensor.shape, dtype=tensor.dtype)
+            self.graph_params.append(var)
+            self.tensor2var[tensor] = var
+
+        # computation relation
+        self.graph_input_to_var: Dict[TensorNode, Var] = {}
+        self.graph_output_to_var: Dict[TensorNode, Var] = {}
+        self.consume: Dict[TensorInput, TensorNode] = {}
         self.reverse_consume: Dict[TensorNode, List[TensorInput]] = {}
-        for a, b in self.task_graph.consume.items():
+        self.input2task: Dict[TensorInput, Task] = {}
+        for node in self.fused_graph.nodes:
+            for tensor, tensor_node in zip(node.inputs, node.task.inputs):
+                if tensor.op is None:
+                    self.graph_input_to_var[tensor_node] = self.tensor2var[tensor]
+                else:
+                    producer: Operator = tensor.op
+                    self.consume[tensor_node] = producer.task.outputs[tensor.trace[1]]
+                self.input2task[tensor_node] = node.task
+        for a, b in self.consume.items():
             if b not in self.reverse_consume:
                 self.reverse_consume[b] = []
             self.reverse_consume[b].append(a)
-        self.input2task: Dict[TensorNode, Task] = {}
-        for internal_task in self.task_graph.nodes:
-            for input_tensor in internal_task.inputs:
-                self.input2task[input_tensor] = internal_task
-
-        self.binding: Dict[TensorNode, Var] = {}
-        self.new_params: List[Var] = []
-        self.anchor_inputs: List[Var] = []
-        self.anchor_outputs: List[Var] = []
-        self.anchor_input_new_index: Dict[int, int] = {}
-        self.anchor_output_new_index: Dict[int, int] = {}
+        for output_tensor in self.fused_graph.outputs:
+            node, op_output_idx = output_tensor.trace
+            output_compute: TensorNode = node.task.outputs[op_output_idx]
+            self.graph_output_to_var[output_compute] = self.tensor2var[output_tensor]
 
     def visit_Function(self, func: Function):
-        anchor_num_inputs = len(self.task.inputs)
-        anchor_num_outputs = len(self.task.outputs)
-        assert len(func.params) == anchor_num_inputs + anchor_num_outputs
-        self.anchor_inputs: List[Var] = func.params[:anchor_num_inputs]
-        self.anchor_outputs: List[Var] = func.params[anchor_num_inputs:]
-
-        for input_index in range(anchor_num_inputs):
-            tn = self.task.inputs[input_index]
-            while tn in self.task_graph.consume:
-                tn = self.task_graph.consume[tn]
-            if tn in self.task_graph.input_tensors:
-                self.anchor_input_new_index[input_index] = self.task_graph.input_tensors.index(tn)
-
-        for output_index in range(anchor_num_outputs):
-            tn = self.task.outputs[output_index]
-            if tn in self.task_graph.output_tensors:
-                self.anchor_output_new_index[output_index] = self.task_graph.output_tensors.index(tn)
-
-        # create parameters for fused function, and bind task graph parameters to function parameters
-        # todo: do not create new parameters for the inputs/outputs that have not been fused
-        self.new_params: List[Var] = []
-        for tensor_node in self.task_graph.input_tensors + self.task_graph.output_tensors:
-            self.new_params.append(Var(tensor_node.name, tensor_node.type))
-            self.binding[tensor_node] = self.new_params[-1]
-
-        return Function(
-            name=func.name,
-            params=self.new_params,
-            body=self.visit(func.body),
-            ret_type=func.ret_type,
-            kind=func.kind,
-            extern_vars=func.extern_vars,
-            attrs=func.attrs,
-        )
+        if func.kind not in ['cuda_kernel', 'host_kernel']:
+            return func
+        else:
+            # extract tensor inputs and outputs of the anchor function
+            param_dict: Dict[TensorNode, Var] = {
+                task_param: func_param
+                for task_param, func_param in zip(self.anchor_task.params, func.params)
+                if isinstance(task_param, TensorNode)
+            }
+            self.anchor_inputs: List[Var] = [param_dict[task_input] for task_input in self.anchor_task.inputs]
+            self.anchor_outputs: List[Var] = [param_dict[task_output] for task_output in self.anchor_task.outputs]
+
+            return Function(
+                name=func.name,
+                params=self.graph_params,
+                body=self.visit(func.body),
+                ret_type=func.ret_type,
+                kind=func.kind,
+                extern_vars=func.extern_vars,
+                attrs=func.attrs,
+            )
 
     def visit_Var(self, e: Var):
         if e in self.anchor_inputs:
             input_index = self.anchor_inputs.index(e)
-            if input_index in self.anchor_input_new_index:
-                return self.new_params[self.anchor_input_new_index[input_index]]
+
+            if self.anchor_operator.inputs[input_index].op is None:
+                return self.tensor2var[self.anchor_operator.inputs[input_index]]
             else:
                 # we encounter a usage of an input tensor of the task other than TensorElement and BufferStoreStmt
                 raise ValueError(
-                    'Did you used a tensor in expression other than tensor[...] and tensor[...] = ...'
+                    'Did you used a tensor in expression other than pure tensor indexing (e.g., tensor[...])'
                     ' while marking the task as allowing prologue?'
                 )
         elif e in self.anchor_outputs:
             output_index = self.anchor_outputs.index(e)
-            if output_index in self.anchor_output_new_index:
-                return self.new_params[len(self.task_graph.input_tensors) + self.anchor_output_new_index[output_index]]
+            if self.anchor_operator.outputs[output_index] in self.fused_graph.outputs:
+                return self.tensor2var[self.anchor_operator.outputs[output_index]]
             else:
                 # we encounter a usage of an output tensor of the task other than TensorElement and BufferStoreStmt
                 raise ValueError(
-                    'Did you used a tensor in expression other than tensor[...] and tensor[...] = ...'
+                    'Did you used a tensor in expression other than tensor storing (e.g., tensor[...] = ...)'
                     ' while marking the task as allowing epilogue?'
                 )
         else:
             return e
 
     def visit_TensorElement(self, e: TensorElement):
         if e.base in self.anchor_inputs:
             # access an input tensor in the anchor operator, replace it with the task input (i.e., InputTensor)
             input_index = self.anchor_inputs.index(e.base)
-            return self.visit(TensorElement(self.task.inputs[input_index], e.indices))
+            return self.visit(TensorElement(self.anchor_task.inputs[input_index], e.indices))
         elif isinstance(e.base, TensorNode):
             # apply prologue
             buf: TensorNode = e.base
             indices = [self.visit(v) for v in e.indices]
             if isinstance(buf, TensorInput):
-                if buf in self.binding:
-                    # buf is an input tensor of the task graph
-                    return TensorElement(self.binding[buf], indices)
-                elif buf in self.task_graph.consume:
-                    # buf is an input tensor of an inner task of the task graph,
-                    # but not an input tensor of task graph.
-                    buf = self.task_graph.consume[buf]
+                if buf in self.graph_input_to_var:
+                    # buf is an input tensor of the fused graph
+                    return TensorElement(self.graph_input_to_var[buf], indices)
+                elif buf in self.consume:
+                    # buf is an input tensor of an inner task of the fused graph,
+                    # but not an input tensor of fused graph.
+                    buf = self.consume[buf]
                     return self.visit(buf[indices])
                 else:
                     raise ValueError('Input tensor {} has not been bound.'.format(buf))
             elif isinstance(buf, GridCompute):
                 remap = {a: b for a, b in strict_zip(buf.axes, indices)}
                 return self.visit(rewrite(buf.value, remap))
             else:
@@ -132,23 +142,23 @@
             return IRRewriter.visit_TensorElement(self, e)
 
     def visit_BufferStoreStmt(self, stmt: BufferStoreStmt):
         if stmt.buf in self.anchor_outputs:
             # store a value to an output tensor with epilogue, replace it with the task output (i.e., TensorNode)
             output_index = self.anchor_outputs.index(stmt.buf)
             return self.visit(
-                BufferStoreStmt(self.task.outputs[output_index], stmt.indices, stmt.value, stmt.protected)
+                BufferStoreStmt(self.anchor_task.outputs[output_index], stmt.indices, stmt.value, stmt.protected)
             )
         elif isinstance(stmt.buf, TensorNode):
             # apply epilogue
             buf: TensorNode = stmt.buf
             indices = [self.visit(v) for v in stmt.indices]
-            if buf in self.task_graph.output_tensors:
+            if buf in self.graph_output_to_var:
                 # buf is an output tensor of the task graph
-                return BufferStoreStmt(self.binding[buf], indices, self.visit(stmt.value), stmt.protected)
+                return BufferStoreStmt(self.graph_output_to_var[buf], indices, self.visit(stmt.value), stmt.protected)
             elif buf in self.reverse_consume:
                 # buf is an output tensor of an inner task of the task graph,
                 # but not an output tensor of task graph.
                 consumed_by: List[TensorInput] = self.reverse_consume[buf]
                 if len(consumed_by) != 1:
                     raise ValueError(
                         'Expect tensor {} to be consumed exactly once, got {}.'.format(buf, len(consumed_by))
@@ -201,15 +211,20 @@
                 return self.visit(BufferStoreStmt(consumer_output, out_indices, value, stmt.protected))
             else:
                 raise ValueError('Output tensor {} has not been bound.'.format(buf))
         else:
             return IRRewriter.visit_BufferStoreStmt(self, stmt)
 
 
-def apply_prologue_epilogue(ir_module: IRModule, func: Function, task: Task) -> Function:
-    from hidet.transforms.flatten_tensor_slice import FlattenTensorSliceRewriter
+def apply_prologue_epilogue(ir_module: IRModule, fused_task: FusedTask) -> IRModule:
+    anchor_function: Optional[Function] = None
+    for func in ir_module.functions.values():
+        if func.kind in ['cuda_kernel', 'host_kernel']:
+            if anchor_function is not None:
+                raise RuntimeError('More than one function found.')
+            anchor_function = func
+    if anchor_function is None:
+        raise RuntimeError('No kernel function found.')
 
     rewriter1 = FlattenTensorSliceRewriter()
-    rewriter2 = PrologueEpilogueRewriter(task)
-    fused_func = rewriter2(rewriter1(func))
-    ir_module.update_function(fused_func)
-    return fused_func
+    rewriter2 = PrologueEpilogueRewriter(fused_task)
+    return rewriter2(rewriter1(ir_module))
```

## Comparing `hidet-0.2.2.dist-info/METADATA` & `hidet-0.2.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidet
-Version: 0.2.2
+Version: 0.2.3
 Summary: Hidet: a compilation-based DNN inference framework.
 Home-page: https://docs.hidet.org
 License: Apache-2.0
 Keywords: deep learning,machine learning,neural network,inference,compiler
 Platform: linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -41,18 +41,14 @@
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/hidet-org/hidet/tests.yaml)
 
 
 Hidet is an open-source deep learning inference framework based on compilation. 
 It supports end-to-end compilation of DNN models from PyTorch and ONNX to efficient cuda kernels.
 A series of graph-level and operator-level optimizations are applied to optimize the performance.
 
-## News
-- We will host a [tutorial](https://centml.github.io/asplos23-tutorial/) about Hidet at 
-  [ASPLOS 2023](https://asplos-conference.org/workshops-tutorials/) on March 25th. Welcome to attend and ask questions!
-
 ## Getting Started
 
 ### Installation
 ```bash
 pip install hidet
 ```
 See [here](http://docs.hidet.org/) for building from source.
```

## Comparing `hidet-0.2.2.dist-info/RECORD` & `hidet-0.2.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,206 +1,218 @@
 libhidet.so,sha256=jnnNW97jt8ioIytjqKSL2B6RRGOyLy80kB6GPymC46k,7123
 libhidet_runtime.so,sha256=7u4j4lt0XWPPzsjndSMdxtTj9c4WRM5A1OncSFXrm40,55385
 hidet/__init__.py,sha256=KwIhc8_lUWN6EhQyXFR41SdS3uokAiGKR5kcEj7K4Mw,1673
 hidet/array_api.py,sha256=HuK4YPnjW0qZzfdzAawX-ATzQOyjoHNL_EUuIIjajlA,2797
-hidet/driver.py,sha256=nQEDhURYJioL9Mg9TqRFvdaybPLE9ElXPeLJZgLkrS8,10611
+hidet/driver.py,sha256=itfeNlnotjQcIw57zQUIgrxFIeF9F4DdD4yfotp-Cfo,11538
 hidet/libinfo.py,sha256=r4wgD_v4qQbUtjzB4C5zjAOH1Dl-5YxYNkm0aC-CFIE,2178
 hidet/logging.py,sha256=8eCFyq8CQxubbeUOxj6GJxNbPoxvnoxHYpcBLUzzHi8,2039
 hidet/option.py,sha256=mgB4A-xbzNsJRr6Ez5xIxRrwcl4-5uy9zK0DUdYD38M,13706
-hidet/version.py,sha256=mcwf5dN3aqIukcgjT5AaeaSoqUEH6A77ukEphFMg9ao,566
+hidet/version.py,sha256=E0HegdfHQgsZLjsarFGb3yBZqt0SVY3wYVaaKXvZygc,566
 hidet/backend/__init__.py,sha256=Vrr3qboi1hmAx_flF9WEUOvZ9UWuPY3docPuzGlLyl8,745
-hidet/backend/build.py,sha256=oRQC6sMiEBidnr0iblsysNb5QsJJxhX9h5mjr1SbM0E,8609
-hidet/backend/codegen.py,sha256=z3tZ6dfW8MRGPyln_OjR-tQYNaV5SoVFBmLL8roJLGI,27422
+hidet/backend/build.py,sha256=vUlI5ZhhJnNlmjAhXmhMNhVVY1IVfyLLOehyBdnEj9w,8591
+hidet/backend/codegen.py,sha256=kLWBXzAZFmQGkXtRxDYZ_ouAYuqN1-xRMMR6vvFokaA,31602
 hidet/cli/__init__.py,sha256=64MvxrLvD-cvb02E5ydU8MRBcUFZ1p61sA3qaf7rd5I,564
 hidet/cli/main.py,sha256=oNo44ope2qCyj7WK_c4lHaeuGbt_G6ql81RvbBYLE5s,875
 hidet/cli/bench/__init__.py,sha256=gscZTk0geTQ72fQZ8N8YWo-AWLjmQpkIpC9q3xS6Mfk,887
-hidet/cli/bench/bench.py,sha256=21YDOTVW90lnE6g3QIk5zBL8O9RL4-Ss0k648cqyjo8,1667
-hidet/cli/bench/bench_all.py,sha256=of0kn3KD-W5hT-bZJTNnAjFY48oV8UMWJJ5LM_B8tYA,1016
-hidet/cli/bench/bench_common.py,sha256=ApDkFRafCxJ7qJe5rOkiQOFnwsGZBK36WzrSbMGsrZg,1020
-hidet/cli/bench/model.py,sha256=fCx_VXN5lpF5UAsgQXLVWgwpjBuy-rk-KpKp3pybYjc,4859
+hidet/cli/bench/bench.py,sha256=jItYSRfSFNzGW8moO7m3yOH9COi2_VDeAwiRAkJ10VU,2907
+hidet/cli/bench/bench_all.py,sha256=oIlUtUjwsQfIk0Yv42IAPA83nHEoXd8DXu80_8ImSfE,935
+hidet/cli/bench/bench_common.py,sha256=NvjeOsmWQRT-DZ4v6G2kKowNNIR4RYxmZLBvliuES0o,939
+hidet/cli/bench/model.py,sha256=-mgW6RA3eY1ijE813ihBdLrOxFp-zNZRDhLiYsorllI,6111
 hidet/cli/bench/nlp/__init__.py,sha256=wK_OG0ERGwTtuF3ZC0qo7T4qpPOCQIDsS_cSpe07rwo,574
-hidet/cli/bench/nlp/models.py,sha256=wrgeUNkWnv4s0b4YkQlpNyoa6AE_H2WzaNkXV24TfuU,2547
-hidet/cli/bench/nlp/nlp_model.py,sha256=tBunZrkztqHz766SejfJ6PsvWFGcTDSP7fMxK7LY_78,1487
+hidet/cli/bench/nlp/models.py,sha256=Qbwq2dyJeyMLUbNPLWZNpYuWeSNwJcvoeoAHpbnxqh8,2493
+hidet/cli/bench/nlp/nlp_model.py,sha256=Pu3PwxujjPkKKHA4yuvuwXJj6BixF5PWplq5RLmg5rY,1851
 hidet/cli/bench/vision/__init__.py,sha256=XClDsRq-KKFLD_qjI24Fs0UpKyHv1gcqidoFnTYyPCY,702
-hidet/cli/bench/vision/inception_v3.py,sha256=vURR9UB4W_ZArk6ms23l_Tr7LR87ERiWMS8b2nrfxQY,1781
-hidet/cli/bench/vision/mobilenet_v2.py,sha256=WAlo8kE6WhxIUGfyVxqP38McC69scTa97DaRYZMmco0,1781
-hidet/cli/bench/vision/resnet.py,sha256=fEakYqGODZuptk6NhBOIEEOYh4iAVyK5WTLb00xCmns,2464
-hidet/cli/bench/vision/resnext.py,sha256=EcrV4U0wj3FdoNiTfqOqct1sN0WApMUCu-r-VYIiUyk,2342
+hidet/cli/bench/vision/inception_v3.py,sha256=1BPx98UEzSmd7oXAgwecKmil2_DTYSDbCJadSukPBsk,1727
+hidet/cli/bench/vision/mobilenet_v2.py,sha256=80MP8mpV8_V3A70RpMTEaLWVmJZtSE41cQJYSgxCZIQ,1727
+hidet/cli/bench/vision/resnet.py,sha256=ioKBbomIb8rjNUGgZVdMKSGPe7bvKhUOiwwxJL6DG90,2410
+hidet/cli/bench/vision/resnext.py,sha256=enP71avHfrIy3Ws86e3bsg2yij3SDiDEYZxzCbK-whM,2288
 hidet/cli/bench/vision/vision_model.py,sha256=sf5o8oX8_pz85f2USnuCxNMFx87hN_PpSt26I9Wx1RQ,1269
 hidet/cuda/__init__.py,sha256=edjcRO5nVwG6OdZIZfOpRPJUowkyL0qG20RcTiPgEps,1034
-hidet/cuda/device.py,sha256=4OWvypBhvD9Cib4RQv8FFCkrHjCGhPmkiroIZSLVfzU,4572
+hidet/cuda/device.py,sha256=tmCfX4u5jJX4m1XtvswZXBSkeKl6Yjrc_5IqbvDkBLU,3876
 hidet/cuda/event.py,sha256=AUR5gNJA4BGfeCi7bSpyxXsaYmkKYki_lk8SN8Y1urw,4171
 hidet/cuda/graph.py,sha256=aIQkWLeSDXrP_RIvSxRu_9H8UulWSSKZtmTPeXIPNsA,8203
 hidet/cuda/memory.py,sha256=OubMnF8bZ0PWSrfzQ_-cHP9ev1kpIcsN-Hk2E-_SPq0,7460
-hidet/cuda/stream.py,sha256=tEmlJIt1xvp89Vqd7BNUJhJsUG24juQQ2XffuHw25Os,7709
-hidet/ffi/__init__.py,sha256=WDttb266NjSqGEBTWmIVYaTdgusDycmYiczlCldVmP8,695
+hidet/cuda/stream.py,sha256=rt7IhgxAiqbc5_C3kuIeew5Bk7NuhaQxec4deJfw5aY,7759
+hidet/ffi/__init__.py,sha256=_58srxVUcM7FW4HPyoxu70YDf6SLjosvjACiesEykqU,699
 hidet/ffi/callbacks.py,sha256=ReK_ZK-1CbKSQtggt8ZL6T4lAqhUIiuBHSUzXrGzwVk,2496
 hidet/ffi/ffi.py,sha256=aV82RP_a2NhZvqKOCDK1ZJji7OEN3Da_H3Tzifn2CDc,3079
-hidet/ffi/packedfunc.py,sha256=rB7vHNBvoHypwSNsqudLOFrA_mQvR87YjPfCKX4NLoc,6540
+hidet/ffi/packedfunc.py,sha256=CqC9xGBqd0heLBsA__2EzFarQ9UMaPAalmBF6Guxuj0,6858
 hidet/ffi/runtime_api.py,sha256=CeTIbG8V9wRXk8Lz6wpi_UT2_YAsDZdp6d15SeJgnWk,1766
 hidet/ffi/shared_lib.py,sha256=qlTz1R7xpwjeQ6gXV7MRTSZIzisf6afgpUrbgfN4_9o,3427
 hidet/graph/__init__.py,sha256=gnN30gxfGSrAtQUGCgFGddqOfxpFM0kHATcX7k24Kdo,1240
 hidet/graph/common.py,sha256=PCk-WjvrgrI-DZ7shTiBpkv4B53EbmOtzASNzA4Vf8Y,672
 hidet/graph/jit.py,sha256=HJWlc2Fgu0HYZBTtPRRrUEDu16PcD7uUkNW6q9qa7uM,5356
 hidet/graph/module.py,sha256=zdKNcKGkQxroc_lVYlJrzhj3Qp1ttMxfUPX3l0pDkfg,3735
-hidet/graph/operator.py,sha256=EfZi_emuYq8JTZhY-hlPrCjeCzEfwr7ZDe_F7d_fYS4,7073
-hidet/graph/tensor.py,sha256=Z_WCrRQHZa1GdSPee7aKXwB2g3ySVvZzURCBdMDkYnE,41965
+hidet/graph/operator.py,sha256=k5RKurQRbRj2EOHKvcVdScrY5RufxPsvsv8mT2HZmvc,7701
+hidet/graph/tensor.py,sha256=RygLk-OoglfWfyX8lQzrAGBJC4OwtSeMi2wlV0BxaH0,43043
 hidet/graph/frontend/__init__.py,sha256=OwIub7ls06TsnuWHKUJy9Ti-_lwsESwC8IHPXQV8z-c,694
 hidet/graph/frontend/onnx/__init__.py,sha256=O1X6sRvk_rUAIilRk5GNMYjJk4pkwGD8O8mIgwlkq6U,649
 hidet/graph/frontend/onnx/availability.py,sha256=Rx5klf9j9hjDg6X2-rrhHz0sqzlKzapeU5ab-nyvXYE,848
 hidet/graph/frontend/onnx/onnx.py,sha256=eknBvVK8JzwGTpHFch926YrAHSzCm_5zDx8jNYJDhHE,46729
 hidet/graph/frontend/onnx/utils.py,sha256=7nDz3UlTS2_Slu9eIYmtfxT1IXB34Uuf2MIM4cVzKow,2076
 hidet/graph/frontend/torch/__init__.py,sha256=4w2Ud2FSgTi7nleksUDdIJEQdL0kmrj7uEjnDoDbyDw,2109
 hidet/graph/frontend/torch/availability.py,sha256=hQx81BJPnYkUFCcPZHaj6SgmXv1VFwTZPdfu2B48PEc,1325
-hidet/graph/frontend/torch/dynamo_backends.py,sha256=_jX5OWZdsHPKxL9W8F9Oz7DNt7IJcD_-HiaxbcXe_GI,6425
-hidet/graph/frontend/torch/dynamo_config.py,sha256=_vh4Bm7Rlwsnk-QJn5ZIa76eeyp-RRH5wglNB0blkIs,3855
+hidet/graph/frontend/torch/dynamo_backends.py,sha256=iQ9--84cTZPHWtYlDpag0A5f7ITXYenKygnxhXsi5vI,6866
+hidet/graph/frontend/torch/dynamo_config.py,sha256=xyt-9Wl7h3SSRjNKwvkboBS7SgVK_lT9xeiOqVsVw-k,4600
 hidet/graph/frontend/torch/interpreter.py,sha256=yS3tSPFM5fppbdoT-zCBciWPbQxz4TtvoBLsRVEtEy0,17516
-hidet/graph/frontend/torch/register_functions.py,sha256=mSACzcRMZxtnj384HYrHP-gRCjHLuWm8QwJqgCjy0OM,15277
-hidet/graph/frontend/torch/register_methods.py,sha256=E1KspBy9ksjpmeKLbTrML3dykXGrjDvhKLoMOCDXCIw,6312
-hidet/graph/frontend/torch/register_modules.py,sha256=880DaasufTkGEv65L_RHhM3q6opLHKi0nP28oGKgPNw,7629
-hidet/graph/frontend/torch/utils.py,sha256=v89FU9u81Jfq2xxaQSUnz8emlbp68agGDZg4RfgKbdY,7289
+hidet/graph/frontend/torch/register_functions.py,sha256=vJKl1KRf_HOmro317N38MnWIsMZKwboa6PqT6R6AftM,22755
+hidet/graph/frontend/torch/register_methods.py,sha256=PxIIt0KPrVCanh8YBLXTTIIObvHwDSpdK2RIt8OBqhM,7061
+hidet/graph/frontend/torch/register_modules.py,sha256=on3_fcxsq68Am4wummrdccucnv8A3755VTkmIX60chY,10033
+hidet/graph/frontend/torch/utils.py,sha256=D5KOvrFLNncg-inL4AGd5XmvQ2xAHkNKRNiuJLOJ0xo,7611
 hidet/graph/impl/__init__.py,sha256=K3tEEv3Pt67q900U_xkDrNYi89Gl70sjV3ueoon0Fjo,544
 hidet/graph/impl/dlpack.py,sha256=RcRY7g1UshaiSIF6gEbQAKvXQakBtz6ln90gXCb1ZLI,10004
 hidet/graph/ir/__init__.py,sha256=FYzYuNZltE_koyFKGNrVc_eRq__KTrhO21fxipqKbuQ,748
-hidet/graph/ir/flow_graph.py,sha256=pOV79T199ZJxvluUsYJhPUEw8l70zSlgQQFuW1usAy8,19637
-hidet/graph/ir/flow_graph_impl.py,sha256=QqnPKOZ2kGmCx9uRy9ZVe1eT1Ea61r0cqtHmwkysx8A,10110
+hidet/graph/ir/flow_graph.py,sha256=NwC8nXkzn0WYtnDedfL9vCfvP3j3HuY_tebUTEa1vnw,20377
+hidet/graph/ir/flow_graph_impl.py,sha256=hIKh3pYkAM184R4PkUbSv4g3CY4vEtiLghF5LNsBDrc,10017
 hidet/graph/ir/functors.py,sha256=R1xc0wHw7I654uvqfg42OgBUU7S3Yw_7wPkhInGisoQ,5681
 hidet/graph/modules/__init__.py,sha256=mMQqc33NoRExdBkLvGnxe1alruMVOHP661DmMMDuh0A,585
 hidet/graph/modules/container.py,sha256=VYqBUDg9lKPpa169sA-l27FsaRctWU1yAZOiwiFTo7o,1655
 hidet/graph/modules/nn.py,sha256=cuxVcHEYfKy2Dx-M0KGcBiuZXOsWJmXQ2yLIvfB7TAU,5755
-hidet/graph/ops/__init__.py,sha256=8bQ9rkXOw1M7Lq6zqqILlK0Li9t8MaveMQ8zJv1HstI,2791
-hidet/graph/ops/definitions/__init__.py,sha256=jVHGCo0dVqPUprVaI4v9l6JHN2HnqKG5dtlLu-4LIaI,2082
-hidet/graph/ops/definitions/activation.py,sha256=1da5bQeVpoXVuHaa6rLiM1_3If5qwXIDZSzUseaA_PM,3863
-hidet/graph/ops/definitions/arithmetic.py,sha256=RNN8jca63njOg2ROeSpDINx6h35E9c3IpxIc4KcArQI,21758
+hidet/graph/ops/__init__.py,sha256=2EASaYLBzkSzib8uEUXium2XBupv4lIgSTUup7G2W8Q,2989
+hidet/graph/ops/definitions/__init__.py,sha256=xvfoUn0vL2mLBklQjsLqNCI_ewfp4bVFYnb35ngtleQ,2211
+hidet/graph/ops/definitions/activation.py,sha256=w8UdxzHTiGfS3RdeWae30Lz8AuZUDamzjKZdAqGNElc,8723
+hidet/graph/ops/definitions/arithmetic.py,sha256=VLtN5KxmPO9mIX9XUUfeFnml5C1yqlumdgXy78geN5s,21886
 hidet/graph/ops/definitions/arithmetic_resolve.py,sha256=ZFqfUV0xKPw4RhR-2EE8u7h_SPlB49FNqgrdwKyaqjc,1310
 hidet/graph/ops/definitions/compare.py,sha256=CFz7tXDQIgzCZONV_ztkP9F9VKCpXIO5aSHG4cZlF6U,3341
-hidet/graph/ops/definitions/create.py,sha256=UaxUevMogC4TcLC9h9nRUrIMH8OaYVfpSU0nqRWq9yo,5592
-hidet/graph/ops/definitions/cumulative.py,sha256=zNpxgb3gOHvVyJ7aYGGAfVtZChyTLaiB1A2SAiH6QW4,2970
-hidet/graph/ops/definitions/image.py,sha256=FPvD5oBVebdJTrMZ4wfmzCX7aHdz3WUK_HOIAOU2SyU,9939
-hidet/graph/ops/definitions/norm.py,sha256=rOtFugzh6W9Te1JBBGurpDEbm6fNHQUQPP3emjOqmCc,2459
-hidet/graph/ops/definitions/pool.py,sha256=Huo5-3EBbmacmku0XisR7RPzF2Y-5wTFVMZ5JbGQoYo,11594
-hidet/graph/ops/definitions/softmax.py,sha256=fPNfurS02LFOeH8Ka3a_YlSL-NUm8gPmMj8ifcP-F0U,2609
-hidet/graph/ops/definitions/special.py,sha256=gglkRvE9FihVqfss6YcR_8yl-IowVf4vagrfnc7_3uc,1587
-hidet/graph/ops/definitions/transform.py,sha256=c0O8kZTK5wz1d31PE_5CM0Lsb8rXbP27tRyJ5DeoqRI,28652
-hidet/graph/ops/definitions/utils.py,sha256=vEjhK48oxoZzycBKf64iVrQTnIsgdwtjmvDShZdcKjI,7149
+hidet/graph/ops/definitions/create.py,sha256=gdWHDSa_ox2itO1TipC-8Ff81kKqQqkuIJ0IauPQzEQ,5507
+hidet/graph/ops/definitions/cumulative.py,sha256=-4CGaNMilRvCRCh_TZ7KUXIDQHJVMhVxSt0Tku8TUIU,2970
+hidet/graph/ops/definitions/image.py,sha256=7H0xJaGi8CtC2hP1gDo7UrwZdTrVpebjsh7Zt8ZrpSo,9939
+hidet/graph/ops/definitions/norm.py,sha256=W0INaetKAhGh0CHIYOS09McPxNmhX0QSa7mfb9_EqJk,3284
+hidet/graph/ops/definitions/pool.py,sha256=3x-34ZBcyLUdw7BcOO9hiWYL2sGAW9webwvtNhZRaYw,11594
+hidet/graph/ops/definitions/softmax.py,sha256=XdXn78GGxFAQJ1FI6X2asO0fDtN_VJBAIMHvqW_wE18,2239
+hidet/graph/ops/definitions/special.py,sha256=-M-0rrGVqnpyo6VU98Ar8QIbRCnOhvX_yGspGVSnn7c,1602
+hidet/graph/ops/definitions/transform.py,sha256=hxqNJ0BdpaOScTU1V3mARV1fBJ4Pwj2kXq03NGFslN8,29926
+hidet/graph/ops/definitions/attention/__init__.py,sha256=wVTyHXuljUAI6FvoCOktnCm2tfC-ewNzIKxYhauHGHc,33
+hidet/graph/ops/definitions/attention/attention.py,sha256=ET4LNPP8lbk700LhvWNGN6-qCg61OQglDSrCFa4GNX0,35378
+hidet/graph/ops/definitions/attention/attention_mask.py,sha256=XczwkQ9AYVgL6dc4iTE_gjCHXHbXAaAbgLtmX2Yikfs,36447
 hidet/graph/ops/definitions/conv2d/__init__.py,sha256=L48x5_bMfB0iaTvvByla__M_K2GTXDE0qeEPuKWTolk,1157
-hidet/graph/ops/definitions/conv2d/conv2d.py,sha256=-T0t_Bh-eoOjr332Fgxj66QxvdzZ5CBPv4DPenGnCFc,3165
-hidet/graph/ops/definitions/conv2d/conv2d_gemm.py,sha256=Q5zsnJlf5fF5NTuJiQOJRutynF1EUQnmUZyBAuDaBXs,3961
-hidet/graph/ops/definitions/conv2d/conv2d_winograd.py,sha256=DcvPwdspwpnOcDQVvlKv4JtZfUUcy4v2sTWF9At29hc,7505
+hidet/graph/ops/definitions/conv2d/conv2d.py,sha256=1kB4FWDpVW263WPjY8G5jS2GJw3QbeuiwT3cpXajzus,3165
+hidet/graph/ops/definitions/conv2d/conv2d_gemm.py,sha256=fcX_7hLHzpghr2Mr8ipunWOkVJEZpx1P-2iBjPKnDHY,3961
+hidet/graph/ops/definitions/conv2d/conv2d_winograd.py,sha256=SYyfuylfwACDLGGBe-dxVPyThRcJTLsWj-YQdrXG_GQ,7505
 hidet/graph/ops/definitions/conv2d/resolve.py,sha256=0SjlTNRHrpXMXDIeb_G-NUCu1lEx2MQwIYgaBMMKzuM,1720
 hidet/graph/ops/definitions/conv2d/utils.py,sha256=iSOuiFHvWYAX_oK4oGWEWxI5qirTiimqoOASYUrrkg8,1325
 hidet/graph/ops/definitions/conv2d_transpose/__init__.py,sha256=ROudWMK7eCZdk_17G7ikne6PNME00XwA77XJE2nwu7w,690
-hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose.py,sha256=U59gm6jzr1wHy3dhlDQ8eyiz0-En_XgWJ-0GILClCVw,3957
-hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose_gemm.py,sha256=FjqmJrEqe2jMiyyp9f-6CpjXJoUqtUb8DhGmqBu8IH4,4894
+hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose.py,sha256=pK259oY1Saaj0J6Jip-rN6zCHDFdpdqRJTs-RCN8Akw,3957
+hidet/graph/ops/definitions/conv2d_transpose/conv2d_transpose_gemm.py,sha256=PE12gaZrV3pi8pnGDdGNZo64w1Qi6u_aNReJcl3rl_I,4894
 hidet/graph/ops/definitions/conv2d_transpose/resolve.py,sha256=C5NHy3xqEyCjYdp8Ebh-1Hv4pF-HgFkjGqRfNQC5lCo,1246
 hidet/graph/ops/definitions/conv3d/__init__.py,sha256=xQd6KACuyAFiKf5ugBsR2jkfnnjumYqygMnVh8WraUs,827
-hidet/graph/ops/definitions/conv3d/conv3d.py,sha256=PMcTJ0K6NsT86byMStdw2FOBIkLQLTbMkAYDUIaLKLk,3466
-hidet/graph/ops/definitions/conv3d/conv3d_gemm.py,sha256=xd9VyAl8sFLL3hveRC9B7t4-vwTzQQuiEax1GtCn9wE,4319
+hidet/graph/ops/definitions/conv3d/conv3d.py,sha256=nVZeHNNwWWPu1Z2b0DcQFj7yjrGrxM0wN0obIdbSMho,3466
+hidet/graph/ops/definitions/conv3d/conv3d_gemm.py,sha256=g10kAbEFGeK-vR8vQlwT-I_0F-SyAh4nszgwAbm_8w4,4319
 hidet/graph/ops/definitions/conv3d/resolve.py,sha256=3vag2ua6H0IeKvx4D59i4jqz_rlWHDSi4gwPq361maQ,1376
 hidet/graph/ops/definitions/conv3d/utils.py,sha256=gIrsDArRTsuui-bgEpt3Rg8ASxhrg2IuPlTeove72BI,1425
+hidet/graph/ops/definitions/fusion/__init__.py,sha256=I4B0etDtqK0Jhi40PwzVO0BZrjMtIKQmY3gD_-RJraA,43
+hidet/graph/ops/definitions/fusion/apply_prologue_epilogue.py,sha256=1gWNxX49FTPL61FpOiu15C_R-HovV_vCYHv0F3l4Vzc,11864
+hidet/graph/ops/definitions/fusion/fused_operator.py,sha256=HBEmDcMi758rRqGbCuHn4VIc7EWEDELQPcduC0z1HDs,7428
 hidet/graph/ops/definitions/matmul/__init__.py,sha256=faip20w22mxWlO4UMWLeDzAgiWZ4N49Omyw51k5HOCY,686
-hidet/graph/ops/definitions/matmul/batch_matmul.py,sha256=QW0E-S5ESzkmxoeCoYjApPWkg7XH072qNqW6z7Uyvoc,3699
-hidet/graph/ops/definitions/matmul/matmul.py,sha256=gLvijb5q2TP4rBduJQnZC6-tQjcHqXXQ-zcq4oIk_I4,3256
-hidet/graph/ops/definitions/matmul/matmul_f16.py,sha256=prN-JQr-EPDbsVr2pVA-i2dz-tQ2PIiAiZvoKL1CUIE,16662
-hidet/graph/ops/definitions/matmul/resolve.py,sha256=QeLO5xKNRUgsKd5UiHv_EuESsm6kWQ9TAnk5du3Ocm0,10405
+hidet/graph/ops/definitions/matmul/batch_matmul.py,sha256=lP2e8sFXCqbuWi2kobtwt4SbkKSQHTEhJfpWrmpOVaM,3725
+hidet/graph/ops/definitions/matmul/matmul.py,sha256=_xeeckYXB2xffWPmlF7631h_ERtaplSJrZW7qEurbL8,3271
+hidet/graph/ops/definitions/matmul/matmul_f16.py,sha256=0a48uht3sg-Il0L4wDFkTC2-c317ltJKxKP8nxjrYR4,17991
+hidet/graph/ops/definitions/matmul/resolve.py,sha256=e5I1AFYhGTxahDR7XnsRMeEbjTnZkwDgx1XdPO9vWi4,10483
 hidet/graph/ops/definitions/reduce/__init__.py,sha256=aFW2NklSwGTdmqsv6cEmu-eTZEJK-M9NeorZTh4ejew,782
-hidet/graph/ops/definitions/reduce/reduce.py,sha256=WpAm_tutqrEv9z7z_Hy23zFw6V9sqnVKjU3BHfyUE4Q,9811
-hidet/graph/ops/definitions/reduce/reduce_f16.py,sha256=yBaNJG1Mvsxmsun4n-cBBBEcj91bM6bphPZT_CJ2OfA,13095
-hidet/graph/ops/definitions/reduce/resolve.py,sha256=BFx2KzB6LqhXof13jYpfMKgSOJVEF7l_Y4L975bwZLk,2724
+hidet/graph/ops/definitions/reduce/reduce.py,sha256=hTysaRKpehbKI_cDOJULoeRZYToSPOXWPWcTjkwDBtg,9923
+hidet/graph/ops/definitions/reduce/reduce_f16.py,sha256=fNlNQ5EJX-RauezC4QEBhImCnu9mEQwjZH06aY3w16k,12868
+hidet/graph/ops/definitions/reduce/resolve.py,sha256=VLxpWX5UowUCVzSSsNpD4I1P7OLwGOYjTAhyrgbwSFU,2719
+hidet/graph/ops/definitions/utils/__init__.py,sha256=sV3hgbSwYTw7hexnu6l7yIVz1v3KN_1qE_ru2E5a0ws,47
+hidet/graph/ops/definitions/utils/tensor_utils.py,sha256=vEjhK48oxoZzycBKf64iVrQTnIsgdwtjmvDShZdcKjI,7149
+hidet/graph/ops/definitions/utils/tune.py,sha256=VrjfiXB3CHVD3UGjgbpJ53AHG88wmiCuR7qdpMJ0DJw,7341
 hidet/graph/ops/schedules/__init__.py,sha256=mBjv_ppXW_AIVeIIWJT_mH8u8vzdbTCAZrnvgGVHUiw,754
-hidet/graph/ops/schedules/auto_scheduler.py,sha256=mhLIVDDVOT80iVkcdcJKPxH4TWiOTN5Ok8KNlFoyU_0,14074
+hidet/graph/ops/schedules/auto_scheduler.py,sha256=eZPEyZphNB2Oy3b1sCiS_2LAxN3YcQQ_eYWInRLPhrI,16490
 hidet/graph/ops/schedules/common.py,sha256=Vqk6eK7nxKbzVAJZIYO4wEocJLTWWISpxesSJurV9w0,6384
-hidet/graph/ops/schedules/resolve.py,sha256=4888QGfEuOq0s7b0oQR2bPq4cVWDqHMeAThbzc3FgHM,7529
+hidet/graph/ops/schedules/resolve.py,sha256=2VVGnI5YDSkM_7ED49kg0A9ftZfalYCU3MH4XjGGf5Q,7029
 hidet/graph/ops/schedules/scheduler.py,sha256=mUkZbu8rqD58M4PdrBlqkzLs3RMTiCf74Y79MIIYYOA,574
-hidet/graph/ops/schedules/tune.py,sha256=4XR4OqX4tKcZ0EFEs5piRpc92m1z8lSEMXhjhAFH2vQ,7123
 hidet/graph/ops/schedules/cpu/__init__.py,sha256=K3tEEv3Pt67q900U_xkDrNYi89Gl70sjV3ueoon0Fjo,544
-hidet/graph/ops/schedules/cpu/auto_scheduler.py,sha256=ZylvzwpFsAN1MQrys59fxSD0KFSQtTco90Rwc0KJW10,2611
+hidet/graph/ops/schedules/cpu/auto_scheduler.py,sha256=-vBCtyOwXqFjH-tt6_qu120Vk1C14N2Z409Z1fEBAuo,2362
 hidet/graph/ops/schedules/cuda/__init__.py,sha256=TteVkEEV7LarkbIaZHJhCkAXyhUf036zOECE9YoWlTg,661
-hidet/graph/ops/schedules/cuda/auto_scheduler.py,sha256=jEFOu-_spnYtkdwbKHPf8NW9AV7TJHBSNtDqrOF5a_M,3097
+hidet/graph/ops/schedules/cuda/auto_scheduler.py,sha256=ywFcGZ_eVY-vFV3vetOaf2bomW1agbIj0qVoUPcBMg8,2986
 hidet/graph/ops/schedules/cuda/common.py,sha256=UZM5lbRHwJL_tys7UMg6x3I-keSGNK2GGw8ZfRB42Vk,4935
-hidet/graph/ops/schedules/cuda/depthwise_conv.py,sha256=iByNhtAy5Uh0Ud2bNZukXBdSGDNlX1VP7a369-cGYfs,11077
-hidet/graph/ops/schedules/cuda/reduce.py,sha256=GFv1t2Ewpf90SqEHQfSRwccr9aVSAfuygZInFMG3QhI,6670
-hidet/graph/ops/schedules/cuda/softmax.py,sha256=HAOpJXW1Y7_RDCLN05O8jbRx65ecoYgL3e0v1ztNPkc,3639
+hidet/graph/ops/schedules/cuda/depthwise_conv.py,sha256=21qBHR6VB_bItmOF8Q5_p0g_NxFxDvOSFiGggx63hQo,10965
+hidet/graph/ops/schedules/cuda/reduce.py,sha256=vHrDpyWNDxcCObEb67gHrJkNys0-iSgib8vSnCxZlZE,6557
+hidet/graph/ops/schedules/cuda/softmax.py,sha256=GSy9ooN7FBFO7KRW8TsB7iL2KpF8D8drpGNiBCt0mwo,3563
 hidet/graph/ops/schedules/cuda/matmul/__init__.py,sha256=5ssgY6ZlmB3oQo54mNwHyM07Yc0eR3IxpIDtfG8SZCo,698
-hidet/graph/ops/schedules/cuda/matmul/mma.py,sha256=S4jAQuDqD72ytBQ4mhR5BXCne9pieArwhQeUYJZpd2E,21106
-hidet/graph/ops/schedules/cuda/matmul/simt.py,sha256=UPEOXTsCi5RSytlMKR6ntyV_euK8ia6AeEWhBSFqBFk,22755
-hidet/graph/ops/schedules/cuda/matmul/wmma.py,sha256=mBU-hcmBkgbU_MN0m13sD1mDKufSWHlUHo0UXcsOSa8,21271
+hidet/graph/ops/schedules/cuda/matmul/mma.py,sha256=xi0D3Z-0BQZ42ap4n5tGnnh21EZIXzizA3ZjAZF9Ts4,21042
+hidet/graph/ops/schedules/cuda/matmul/simt.py,sha256=bDPhwNNjlF5vsFujOKnRrGnFqvXBw_qExpzfVEFKb1Q,22703
+hidet/graph/ops/schedules/cuda/matmul/wmma.py,sha256=NVsVtWOJorzvUpJ-7sTFR_QPr8ptrHA-kbEVvrU6Lyk,21213
 hidet/graph/transforms/__init__.py,sha256=OKbDG0BeOmfdiTpYc3T-seNYEEY_I156AW2svuRUTp4,2405
 hidet/graph/transforms/automatic_mix_precision.py,sha256=BeblhywKrt11fmx4BWdIL1mmEpL7UBBHQ5Ig0kn5Bec,3648
-hidet/graph/transforms/base.py,sha256=yWiR6XBFnoMpsCq1QEvZIaIyYxKIGxR-GPJDuSBYNao,8882
+hidet/graph/transforms/base.py,sha256=gSBx-Wqazl1SW5aItMFTWWjObNiv09QNJIGPr5FZIKQ,9490
 hidet/graph/transforms/common.py,sha256=26a1-ODwNTM92lGxalFF0G0Nm51Cfz7kOVzhAHMCdGk,781
 hidet/graph/transforms/eliminate_barrier.py,sha256=fLeWtBVBUlVUwrq6mafHNzTrZl1jlksFUDPewAaxWeQ,1327
 hidet/graph/transforms/fold_const.py,sha256=QlsEFUHtSYMdL63a6LYHC-HPwLPgCFAUi1av_3M0VTY,1616
-hidet/graph/transforms/fuse_operator.py,sha256=7iYh7rCQAUaqs_FyNNSSxu89zHqGegp09b-tdRNM2xs,14965
+hidet/graph/transforms/fuse_operator.py,sha256=eZMseF2JiZzeExqB7C7bZY2MsOjI-Tiy-UhOJtChHbs,16457
 hidet/graph/transforms/resolve_variant.py,sha256=KLIGfx64cOAc3lpOn-pwv9IBf-OAgE2mosw-5khBh08,7011
 hidet/graph/transforms/subgraph_rewrite.py,sha256=eSZXIPR9Hq4Rt6CY5_UU_1nlW01UwCrEgyroEj_IfdI,6274
 hidet/graph/transforms/utils.py,sha256=-fN0NMGPX2bUwjRewur_80EESeNtFAGy6TUAgP9X6lE,712
-hidet/graph/transforms/graph_patterns/__init__.py,sha256=RPJhkd6yDf-JjKkgSPEv8BHcrtVdUVklRGJ7M8RPOPs,925
+hidet/graph/transforms/graph_patterns/__init__.py,sha256=5ITQ2mONr3jO2cppc16Xi71Iqb-EkQTgMDiHZYFMS40,1041
 hidet/graph/transforms/graph_patterns/arithmetic_patterns.py,sha256=yeOTCJBCHNeuxSe3EPkpvkfonGqihMB_FJM-jgL5dJ4,2525
-hidet/graph/transforms/graph_patterns/base.py,sha256=ENMn8I2RMfB3NCNND_8GVR74nv_4W1FF2c_h0_SH2zo,12000
+hidet/graph/transforms/graph_patterns/attn_patterns.py,sha256=OoYX0wTtaVo7LR1BFNh6SKQ5r10wX5IkoYhpOx-hSIA,4818
+hidet/graph/transforms/graph_patterns/base.py,sha256=4tw3y5_sSuF9EGp5_3464KMHVyu4-83JyyzURl5IixE,12434
 hidet/graph/transforms/graph_patterns/conv2d_patterns.py,sha256=j_vksoxui1GfWEkj1JPMo5gWLYepjEWYCSfAjDdOqRU,4867
 hidet/graph/transforms/graph_patterns/matmul_patterns.py,sha256=35DybP3XEUfJkk6gssPlJCPYH3UgafNBFd89o1O38jo,5378
 hidet/graph/transforms/graph_patterns/transform_patterns.py,sha256=IOOC28PUGWUzTZOr_W8o-Pb9oQukcPXN_MIjq93a_2c,6850
 hidet/graph/transforms/instruments/__init__.py,sha256=rJNzJCYzIlI2ZU8PNCEQyUQNll5_SDASVqsiyVOnO0w,687
 hidet/graph/transforms/instruments/base.py,sha256=I8rgvST-ikk_cZY_tZg8cTuqCNzblV0P9Re3MNX-FHo,3405
 hidet/graph/transforms/instruments/profile_instrument.py,sha256=2JGhFdJI0XtlCnSo-Vlrc6J-7V3TJxAy4LEXgb_0-jo,1865
 hidet/graph/transforms/instruments/save_graph_instrument.py,sha256=u4mv99-DRHzbbMrHH-TWRDLeQ265ukQAXaPw1c40ZXQ,1608
 hidet/include/hidet/packedfunc.h,sha256=jZWbvEc5sg9GstQPusqrGMADQGeapowxAg2gbnOlFBI,950
 hidet/include/hidet/runtime.h,sha256=OmNVl8FZrjE3DaX1TcVPbxiMltOz2V4IxmTxFAI-MtU,754
+hidet/include/hidet/cpu/bfloat16.h,sha256=QJdS0TiuLr8UvDKJ-ofQ-pgzPGfA6AQbdYmZNuVox_E,16107
+hidet/include/hidet/cpu/float16.h,sha256=4fxBNIehTrfLATGvoDcgGOYfAs8-52z7X9eYLxjqkrg,25684
 hidet/include/hidet/runtime/callbacks.h,sha256=LLJ2QbCzo4pC3SiNT4f1Ak46dZohskiPUexBPrS3vXM,927
 hidet/include/hidet/runtime/common.h,sha256=xMMSdBXeow8YVe6_BZAA4VNgDGGH3IKL9KdjwRTSxX4,690
 hidet/include/hidet/runtime/context.h,sha256=7LD_pjX4YDTWfp1DczhJAfz8Lj9LbTim4kYQWiWY6E0,1011
 hidet/include/hidet/runtime/cpu_context.h,sha256=rq0gdy5woLTeX0HUbHJhuQ2xnf1oo0knduvJnk0uEbY,777
 hidet/include/hidet/runtime/cuda_context.h,sha256=nI9fFqsKoiN8dwR2RfMLu2WWaoJdb9FbWTc3MXsEQnc,1190
 hidet/include/hidet/runtime/logging.h,sha256=tCA31u1IOYKlMauYKrq9jr4y2rHXVt4LIFtpr4pWdHs,1249
-hidet/ir/__init__.py,sha256=DPCZ-FmNA36XVe3vgWFvvKPiKsFq85Uj-iJzJxQ8zio,2061
+hidet/ir/__init__.py,sha256=I0fePQhSx06RjAHqxtu4KGmKAAs13dmbLnuNZBZWb_o,2094
 hidet/ir/expr.py,sha256=oDLT_NJo0lsUJlVy1xPBmp6vOzOAPm5Ac-TbeA9nQrw,17680
 hidet/ir/func.py,sha256=59Hm1XNBcVs6Dzq5hVEJQf-DAs1TnagCLfLFN9kNBW8,6359
-hidet/ir/layout.py,sha256=lMissptMDoLAdyNZarEGwHLVQd4KXKKUBWcu4CMua9c,16184
-hidet/ir/mapping.py,sha256=-iHgB_VlQ3G7pilx9KnvRyp33CA-UJSJZXgmdTRAiII,12429
+hidet/ir/layout.py,sha256=Y57g1jINiwkm8naBSxV0sDR8wTFf6zWp3tDDWq8LOaY,16178
+hidet/ir/mapping.py,sha256=GtGBIL2Ezvv2yaDXAwyQz7eFhnIHGdMX14VVFINYwHw,13727
 hidet/ir/node.py,sha256=Lhbh0iNpO0z4QznWXNd8h3yHwWbNy5A_C7FGVyURmxw,797
-hidet/ir/stmt.py,sha256=RSpX13NDAaXWWGkGF-5RQEdoE7ZjlNX5g6Mnq7AoEo8,8049
-hidet/ir/task.py,sha256=AB-rsKQ-ni5X2RnCRqCoSEc4W94sp5K-7ELsr-7W8KA,12678
-hidet/ir/type.py,sha256=KG1ccazl0xrxuAl1fP-oX6woCUHWK5lXvrh8EvAKHxQ,9225
+hidet/ir/stmt.py,sha256=7KJtvcIsX_NHKrcLWP2RCDkwP9I3pEs8LzSbu_izODc,11391
+hidet/ir/task.py,sha256=5CQGl5r9QTVgPB_TdE9h37_7c3IXmYObLZB6GhDNbuI,12861
+hidet/ir/type.py,sha256=W6WyLTpgIsiSVEzs00oIU14e3l1cicYJPg2EWsibgWI,9584
 hidet/ir/analyzers/__init__.py,sha256=BlSsHTyfkT2Kx8m9dTR6C6YvsnmlOIhPi5QJ9E0NhJc,640
 hidet/ir/analyzers/bound_analyzer.py,sha256=RDYjRpAenarkkF6fI4GMytOUQxlTCAAXtNbW7efIubc,11678
 hidet/ir/builders/__init__.py,sha256=Iy33x_gvHm8gHA7O51PWfnPBFwcywvhjcfGuDELxHm8,679
-hidet/ir/builders/func_builder.py,sha256=HGUOE0D2FUM7o9O6jmB1oxNCz1WA4qYZyBAkw4L1n78,3502
-hidet/ir/builders/stmt_builder.py,sha256=A2H_Lj2jHSmsI4kv34H12F9yqOW1f69AqCQ2NJd9YWs,5210
+hidet/ir/builders/func_builder.py,sha256=IyFEno4UGDWjRH1FHDcforIQWLoFFLeNV0mZUXi9buo,3343
+hidet/ir/builders/stmt_builder.py,sha256=LEUGjDY3ORFtujspmraQqhKXbSiUJw3UzUgoBC9_Ybs,5245
 hidet/ir/compute/__init__.py,sha256=dG5F5PN3XfR6phvsxW_oKRbDHxivqxo3a8_aoKJpm9M,884
 hidet/ir/compute/primitives.py,sha256=ePI32nHG-MP0VwFv4uGHh8bcCn7UO7ZRYpeT_GqAx4E,14773
-hidet/ir/compute/reduce_operations.py,sha256=VpuMjsKBmhqJ63UVLvMS5WjRQT_UzBeshQjYnCb77Sk,6861
+hidet/ir/compute/reduce_operations.py,sha256=9GdJwU5c4BUU2C985aKiIb30HW4pz6UiKO-xBpIz_yI,6917
 hidet/ir/dialects/__init__.py,sha256=K3tEEv3Pt67q900U_xkDrNYi89Gl70sjV3ueoon0Fjo,544
-hidet/ir/dialects/pattern.py,sha256=5ix4DLqwumSTWI6uWWUN_XrxhWD-zxYUtTgSX_WPIa4,17047
+hidet/ir/dialects/pattern.py,sha256=oXGPi_8QRnKR5JWqUjxyuyISVNMIclwXWzYavhCPn-8,17322
 hidet/ir/dtypes/__init__.py,sha256=9Oxz0MoMknS7BnQiEVP4T-1icECjgJBE7yN2Za2caMA,1877
 hidet/ir/dtypes/boolean.py,sha256=gchM0qD1JX9xigguBhgbYtTK_Qxy0GRVMrs46DVuwng,1543
 hidet/ir/dtypes/floats.py,sha256=FvtyYsRotfIDbpbZtuS2zkAQExL6VgNVU1mLZj1jrpc,3610
 hidet/ir/dtypes/integer.py,sha256=cDb9v7pjNpTfObTFMPsErcI1hu-IYFXzhqPOlN6x9-I,2643
 hidet/ir/dtypes/promotion.py,sha256=b8-QzKwW1d-hDKRrpmp2uwXpa1M3NqLdvMWwZoptjN0,3379
 hidet/ir/dtypes/utils.py,sha256=o166dJU37ruhiDXE34Zb5eV3Y6Z5s7UcSHoxSgVrX7k,3146
 hidet/ir/dtypes/vector.py,sha256=agQBI3WiQuWzhfOJWrZv0ERBCDYNtNiJMzVAjDLOCe0,2372
-hidet/ir/functors/__init__.py,sha256=iAJYABumINqji4ENKe0JUKjBKPMK1exQ35CK1b1u33w,1088
-hidet/ir/functors/base_functor.py,sha256=0lzEYmjRmC4AK2cbhVBNy3N3ZfRMItWr8MFULg8fWbw,4031
-hidet/ir/functors/compute_functor.py,sha256=AISPXzQNKMJqNyyfvKjXV2ndWQJxo99FBpDlG85aBjs,6786
+hidet/ir/functors/__init__.py,sha256=o7jvc3LnFixlMLq7O4eDTioEst1dWHA5UOWutOuYKhE,1161
+hidet/ir/functors/base_functor.py,sha256=Zs1uPxruetnlheLhzH45HtQOH8Ke1VGYUucHqrpz23M,4601
+hidet/ir/functors/compute_functor.py,sha256=XZyljGRKrg2xSvrQ9L8w54olQusbDuSpbQ4ExDuMd2Y,6307
 hidet/ir/functors/expr_functor.py,sha256=_7rgcTCCQvznBpK1-SXybT4qjHXXlI4r2qHbdg7QOAc,14474
-hidet/ir/functors/ir_functor.py,sha256=3rhGy-AIVly2SZ8JOMbGY1A97tFC1dj1nYvUy43OezE,1448
-hidet/ir/functors/layout_functor.py,sha256=K3tEEv3Pt67q900U_xkDrNYi89Gl70sjV3ueoon0Fjo,544
+hidet/ir/functors/ir_functor.py,sha256=lASAP1-vf7TmIN7LVw-VwuRMC--tCv_k2neGTWFU6HQ,1573
+hidet/ir/functors/layout_functor.py,sha256=ECRZY3Pgp9zJjFcrs_h5RTkVde7NXkbXAIOyDi3HJIc,4170
 hidet/ir/functors/mapping_functor.py,sha256=_0uy4cKg92T3aKLNpiOgIRNMqQfdZQgGlsmzpovaKMs,2358
-hidet/ir/functors/module_functor.py,sha256=9OV0vPTetiORgUydyCRJz285MHARVCNrc9MTK1qu9YM,2439
-hidet/ir/functors/stmt_functor.py,sha256=cviWsvEunpTsDCv_jRKqd0_TE-Ng65w4taqOFAu5Ax8,12152
+hidet/ir/functors/module_functor.py,sha256=K4L1kVLhbTfU344sPbVy22VqV7YZJtgd9uKU8P0QFE4,2439
+hidet/ir/functors/stmt_functor.py,sha256=hvEx6NwQApV3dAYPguLkOrN8bdvJhplsJLtcfBjrvho,12215
 hidet/ir/functors/type_functor.py,sha256=Gi-jfEkPFPWLuSJmmLeqw0kXXTd5xbGl6sdUwJxxjvA,3707
-hidet/ir/primitives/__init__.py,sha256=njpXzWC3wFbOYoIX4LMMOpVWWLJ0HPxVoqiQ9E5QSms,1323
+hidet/ir/primitives/__init__.py,sha256=Er57k5h6vz2wW_1wfEAgMyjdBl3LqVNs91yL2rptyY4,1328
 hidet/ir/primitives/debug.py,sha256=XEOlL-be8lLSdu8mYz2ZpNbjvdDL1XHgRspkf0ENgqg,1116
 hidet/ir/primitives/func.py,sha256=2VlkjmrOwWUZt4PYSqIW_p9OwOpu3cBtbEonb5id0nE,5739
-hidet/ir/primitives/math.py,sha256=De2CVHHWfPhDd6_xa1YqS3X7xsA_sGlQug1hVFMJCgM,11314
+hidet/ir/primitives/math.py,sha256=7EV054tulFTtrsEdWm7s9qlur4nLr5O_a7iLVgO-P9Y,11610
 hidet/ir/primitives/runtime.py,sha256=5Ll-CHPiau689CbTNjqleVIhopya5r9q7LfB9xkEVEA,1800
 hidet/ir/primitives/cpu/__init__.py,sha256=Ps-haCsJtXcBMi92QI1P12EOgR59jf_JLy9mmbprkOI,563
-hidet/ir/primitives/cpu/math/__init__.py,sha256=Q1UWFQiIcTr6BC2UZG0_INIpYWoo0Rp4uxdlcyiueHQ,628
-hidet/ir/primitives/cpu/math/float32.py,sha256=Yto3NmBGU4gOromXLRg5bvged9_bcXIW3V3jwrPiRFA,5376
-hidet/ir/primitives/cpu/math/float64.py,sha256=NQ8zyqI-PN5KVEcsw48VcxJRsJkzysB7ylA72YXvnjk,5344
+hidet/ir/primitives/cpu/math/__init__.py,sha256=T_Wl8H1R-VsUS4mx7ufJ5WJ0p3z3-eyIQmNW_74kG0w,673
+hidet/ir/primitives/cpu/math/bfloat16.py,sha256=bin-ZVPbl7i0TWrqKu8UViuniXZezRbRgcGpCjxhDgI,3212
+hidet/ir/primitives/cpu/math/float16.py,sha256=_3Dx2IY0PRvimS5zlpezrIR0gEeymQBwHdCPZhV3CUM,5404
+hidet/ir/primitives/cpu/math/float32.py,sha256=B5F9cetmQiAhm30_nb46iBEo7OxaNrDf7iT8JjOCnKY,5476
+hidet/ir/primitives/cpu/math/float64.py,sha256=BtCaJCToMLhaTMJkbU-QBQD6vYeeXVt-TJ1HeVZcH9A,5442
 hidet/ir/primitives/cpu/math/int32.py,sha256=gIdG_I4BpfImmX72l2MTrep8vte4Mwk4ah5x9MQrO2M,3034
 hidet/ir/primitives/cpu/math/int64.py,sha256=VW_IwbyurBHnpYRBXhKzpn4qbk8B51jEaSHyn7Rc3ro,3034
 hidet/ir/primitives/cuda/__init__.py,sha256=VLl5-2ozyAXZjoERo5cFdpj8_GTFquAvkWGqBu_8sN4,1025
 hidet/ir/primitives/cuda/atomic.py,sha256=Epy7feaSqxxIT_zcApZvvshxUBMye_Af_-SnQkg-Fy0,1840
 hidet/ir/primitives/cuda/cp_async.py,sha256=nkKsHEcV6yn0iz5o5N9GT3Lj_rp0acK-34DT6hZ12cI,7479
 hidet/ir/primitives/cuda/cvt.py,sha256=ab1nkSTWLCTV8ymf18rnx-gEF-CbOVpyRZTf-XkOygE,2898
 hidet/ir/primitives/cuda/cvta.py,sha256=fS4QrIInMt1-0LIRYKb8QqknkDN7uzf4E4mzYj_L1oY,2856
@@ -213,94 +225,94 @@
 hidet/ir/primitives/cuda/sync.py,sha256=EeaGvOK7GFshrEeHQuY5WgYio1WlgKoiAs0EZEbQsyE,1934
 hidet/ir/primitives/cuda/time.py,sha256=0KULS3BlCA8ZuDIeyGh5kWGiUM04pU16FQfz5DjiCrk,1750
 hidet/ir/primitives/cuda/vars.py,sha256=_iMAVdvia8EP4U3m_AM8C5bnFPaFjbQO7Dt3Sc1ocKQ,2683
 hidet/ir/primitives/cuda/wmma.py,sha256=4m_Tlg0GzqZc8OmXul5hQvEyGZUIyI2RI8A66pGg7Vo,12898
 hidet/ir/primitives/cuda/math/__init__.py,sha256=1-4oM510X9Ac2PLCwjUbBvhgDfBHid1BFnTa4ntqq6w,673
 hidet/ir/primitives/cuda/math/bfloat16.py,sha256=lHs1RZqXqlbweK2QBybS_xwhORzZHKS-Q42hb4GFVik,3787
 hidet/ir/primitives/cuda/math/float16.py,sha256=Ls7MNqswS2tl-_okmYqxn6q3BuBr-OHyXd6x5COzkOk,7382
-hidet/ir/primitives/cuda/math/float32.py,sha256=ZRYHT1gpF083GQ-jI6nhcEm2gGd63o-LmbEnQJ80mDQ,5384
-hidet/ir/primitives/cuda/math/float64.py,sha256=4pHWABsAaDljD2OsTsmIzazmonY7MFTyPih3R2FFw_4,5352
+hidet/ir/primitives/cuda/math/float32.py,sha256=9oeNXgCcQHbtHiz0IK27FMLb2gYFCh47hv-5xmK0cBE,5484
+hidet/ir/primitives/cuda/math/float64.py,sha256=WSMAwJ6UUDY370yeeG8mg9VBR_sDX6knrz7AKuCDxbM,5451
 hidet/ir/primitives/cuda/math/int32.py,sha256=Q2Sh5llIoS709lgojYmh48J0Nd7kI_eRTZFPYmlvYd8,3043
 hidet/ir/primitives/cuda/math/int64.py,sha256=1xpnpXOH4dChD5dw6Ar0U1mQfXx7CzcOv0lclgOT0vs,3350
-hidet/ir/tools/__init__.py,sha256=ElAgCoJAkCeluxcqP_KiNiJgmzFEmf4O3Wd_EyHnzRE,767
+hidet/ir/tools/__init__.py,sha256=OsaqdbBNM1wd__lI5y0jm0XlbHnQ5xEuFNhR0eZ6BPE,819
+hidet/ir/tools/free_var_collector.py,sha256=-zANnghxr2N8uMlupXeRIDdEF3aktMwJ2BJqua56EDs,2769
 hidet/ir/tools/hasher.py,sha256=NwYYT4eG6cDiIWsqHC9H4As0IOSBaUYMbDSKdW33NRI,5649
-hidet/ir/tools/printer.py,sha256=mvfwtV0bkDdjUXD3XOn_XMAUW-22PInr1QPip7smW24,22686
-hidet/ir/tools/simplifier.py,sha256=xHFnLQuyBEgArGnuydEAzEIkHTDUhIkAfxAAFUDGBI4,5792
+hidet/ir/tools/printer.py,sha256=E_s7Q4kyIzAqd_ivdnSVmbjaWfh6VIJBmhnkcAO44UI,19438
+hidet/ir/tools/rewriter.py,sha256=3OASZsamWFcquX5qt3uLb99hdcrPY7ZbEprCcO95RvQ,2968
+hidet/ir/tools/simplifier.py,sha256=BS3AIx3FyfgIgRtQCJlz5_JbDN5bn3ZJ_nH6qEFTtV8,5804
 hidet/ir/tools/type_infer.py,sha256=EFl19AinVGorJL4rmWrylPdiK6eOLpRaXLDA_GlwAro,7252
-hidet/ir/tools/util_functors.py,sha256=Ht89LDUAJHXGUIPROo5SDUO2WP4cr8JV6T3sQu4Ggf0,4580
-hidet/ir/utils/__init__.py,sha256=iitKbDcz9MxloHMduAW2O6yLOsABxKdw4zlET_OvKTM,811
-hidet/ir/utils/call_graph.py,sha256=RP-eLUzCvusyiNDNeb50ksvYVFMaNZjRv7tHqHvBD7o,3417
+hidet/ir/tools/util_functors.py,sha256=8UorldEhtsb7i1IAfmqcik40gCxPgV0xf1pXqrTaluI,3276
+hidet/ir/utils/__init__.py,sha256=TailelaliC5l2LrUyu9ztotvoAdmizZ6cLERcWiMjuU,744
+hidet/ir/utils/call_graph.py,sha256=auLdcNlerlc4GCMGmG0mOutrWzI0qWKS2CqsuB80EXQ,3561
 hidet/ir/utils/expr_utils.py,sha256=tIwDYzHlVGrBddLfba_l6IxTNCvkJRtp7RHUKUNcg48,1038
 hidet/ir/utils/hash_sum.py,sha256=fdrxyNrkysWWqZu0beZUZm60pjtedYVRDqO6rTbeZXI,1414
 hidet/ir/utils/index_transform.py,sha256=WcLU_bn8BztMN3vtvfydh3XRUci_zNO5f7kP_1xXDXc,1325
-hidet/ir/utils/task_utils.py,sha256=MkmHZXYBLAmcSHK6Eib5SlXfGcTzu0xo1rySB07aj6w,4385
 hidet/ir/utils/type_utils.py,sha256=7QeAJqnLDuKXEtPPxFM9Y22_541aQ3nc4rr4KYh7K4I,1811
-hidet/lang/__init__.py,sha256=lXB2aEuRA9Qx-97yCru3dsyEarD6d87vh0-pm63JsrQ,3031
+hidet/lang/__init__.py,sha256=Ov7GiAEoMg1gfh126QVxM_ceqDBzJ6Nbw3imE3on9NA,3446
 hidet/lang/attr.py,sha256=FrYK2rseniEltHXPC1X-JfB4BvejfoL3nill8cag00Q,1826
 hidet/lang/cuda.py,sha256=7tfgwBUKGe3mkToYSC1GYmhzp-nPSDwMFTxL7MPX0CQ,2219
 hidet/lang/layout.py,sha256=2eqxeHmjrpEMz690ioWyyOFQ42RcjX9JeklP6kAKDY0,653
 hidet/lang/mapping.py,sha256=5LV5HZUbzkM0JnUcN3ma4VyLSdGTzFooiJYDeVd7ITc,963
 hidet/lang/runtime.py,sha256=zASGK-ZLWDVkC9cdl0I1xdoFOLtjBrxpqzw5CrqH6sA,679
 hidet/lang/script.py,sha256=_2fOlSwHilSP3rFi-8NvdogX1yAc-RHo0lnKoUuI4B4,4695
-hidet/lang/transpiler.py,sha256=MNYWnHlN_sdzABsiI6VUavtpXXi7hVHt2ln2Ia2K1F4,40907
+hidet/lang/transpiler.py,sha256=sa7gzOxGxNaiiuFWashSXARbWd9uCuOkMWI54f53Dro,41589
 hidet/lang/type_utils.py,sha256=Os4ktHjtlqUXvGwXRD4EXEagIuzkioxTRhYQithLhqw,1880
 hidet/lib/libhidet.so,sha256=jnnNW97jt8ioIytjqKSL2B6RRGOyLy80kB6GPymC46k,7123
 hidet/lib/libhidet_runtime.so,sha256=7u4j4lt0XWPPzsjndSMdxtTj9c4WRM5A1OncSFXrm40,55385
 hidet/runtime/__init__.py,sha256=wgrjM_WuLwtFtM1XpgSxWzGqhrX8MjPiuYjJyrczPDU,670
 hidet/runtime/device.py,sha256=rLjppk80na4mrBRnw1BwMBF91-SWTD7fno7WUzMZwkE,4118
 hidet/runtime/module.py,sha256=DEKLhAZasHr0tjmb8FbB5wLkXyoTmxPfywunWvGkYlk,3191
-hidet/runtime/storage.py,sha256=Y6ubzpjN232gyz3FAc8JBoTtNW59QhBY4hii_9NxLuc,12683
+hidet/runtime/storage.py,sha256=VO3EYycv7yn-aGmwUa038EcqBOTV5IOWhQO_P74nOiQ,13426
 hidet/testing/__init__.py,sha256=U56JCi4M0U-iJqyGTGzEC2i419TUi54hTHUcpfjTwsk,751
 hidet/testing/onnx_models.py,sha256=Q3LhnqDK9ZqpsL_7s0vxQkl_jAuKRTRK4iMNf3H2ZBc,4542
 hidet/testing/onnx_utils.py,sha256=9ACgUC8S6dfcsADlUYZfgd6EtWRXW6QK7VEL78rF3Xc,2091
-hidet/testing/torch_utils.py,sha256=qLjCRKuDlYry85kE4SnYp_CHVDmkAhIpI947MDtx1wI,1494
-hidet/testing/utils.py,sha256=1XbSU7e065MPYw50yDQLjWjqYpYBxlko683idliqeus,5293
+hidet/testing/torch_utils.py,sha256=I38DfpcDlGmPhxLF4h1_ow31Ogkx3EybQ6hCs3xF3T8,1533
+hidet/testing/utils.py,sha256=nyHZufnLGufL0ekHCR76OEh-9QouQx3UOksEoBGmVmI,5263
 hidet/testing/models/__init__.py,sha256=BoTk9ypEukmuQj5lQHCKJLALU71fQJgPQTyNrADUeh0,615
 hidet/testing/models/resnet.py,sha256=EFflyygsx0IEt1kBsf8LEC5G1hhKHNpCVdyi4Hlp60U,5544
-hidet/transforms/__init__.py,sha256=dDZRTIaZzPUU6BDFyPcQmjAM_AXkyFFlql8mW_T0wTM,2847
+hidet/transforms/__init__.py,sha256=DVMIvbcl9wWjTe-xyk7mVuHSiZD9IMNHW9pwkAznAB0,3096
 hidet/transforms/add_explicit_cast.py,sha256=pnPrX2AOZE5LPxtcTXjaARcVYHe8PyQbQHFBZnuxDCY,6379
 hidet/transforms/base.py,sha256=Zl3zLrxQpktgCIrKRHpyyx2VIoIEP5ReBtY9skj22ZI,3822
 hidet/transforms/declare_to_let.py,sha256=hdd-OM7qyUcxr02HzKQ8oY687LtqaFppMvrQEf3JAy8,3587
 hidet/transforms/expand_let_expr.py,sha256=TKgCStcwwwqYHZ10A3nifpfey8QDoqjpy5ADh42ZbX0,3204
-hidet/transforms/flatten_tensor_index.py,sha256=JdrIugGGkkG-P7GwqA4S-Tn-zmw7Ee0gXWZ7uxS_nbU,4185
+hidet/transforms/explicit_unroll.py,sha256=ez9TfcVmoLRQgmgGntps1WUPMcOvhp4MISXLtssF2D8,2068
+hidet/transforms/flatten_tensor_index.py,sha256=27sTWr2ViUGOD2k1x_ZJjrk0l5ETN6e2mWCSShYiXlw,4296
 hidet/transforms/flatten_tensor_slice.py,sha256=T0C8G8tJEXFLKIGIq3pFMYz3yvgqrJBacoN4TBHYTlc,4338
-hidet/transforms/generate_packed_func.py,sha256=LDM6bmS5mUleRCCTiSpCrWTJB7LkQdJE3X0NzVDJuk4,4900
+hidet/transforms/generate_packed_func.py,sha256=5kaVIpxauOolFDXZ4at3exxeSXW_Xuo3EHi1tU0_ciA,6551
 hidet/transforms/import_primitive_functions.py,sha256=v05_FRRroIM8dJh772G45iJao4F-vH45OaqNr-YkSzY,2025
-hidet/transforms/inline_let_stmt.py,sha256=Px26CAfZUUBwpQF3OJO9XkRD6GcCIqca9Fy6vScbQek,4342
+hidet/transforms/inline_function.py,sha256=U8YSWwFFdjPUwW8d2-McthsO0MZjpI5lEFFmHgrFb1Y,5684
+hidet/transforms/inline_let_stmt.py,sha256=3Rc6mHLJjU-XD7UKkT6ZvvKVXGrKnws2vBHtJ4iB1zE,4342
 hidet/transforms/lower_protect_access.py,sha256=s9u48vPbeqIT12ufZZbhVUnFwioTjCDWdGBM80Hc1dw,2811
 hidet/transforms/lower_special_cast.py,sha256=0m_jXKk4Tw65uYEixfb9z5yKngryuOeXD6p86urD4_g,3596
-hidet/transforms/lower_task_mapping.py,sha256=9gEGXbL1vgaKy51pSWZ2x_nFehpfjKPYeLk9-MipqYU,5252
+hidet/transforms/lower_task_mapping.py,sha256=6y0HgfkJ1y6FBmQjDT94Qoahk5HZld99CV2uDpLRkPI,4694
 hidet/transforms/normalize_const_tensor.py,sha256=-PWM1tIZiBqDeCSaPykKeDvPYwBXUv6EvKVcJa9ZVhs,1845
 hidet/transforms/propogate_launch_bound.py,sha256=eQeSkc9Ingc-W5tBagn9caNB_kkV7BK-unMorp7OieU,2403
 hidet/transforms/resolve_generic_primitive_function.py,sha256=5idNoKdN_sZEicLyTTJU5PfAPyS2J_AVVTwi63UPufw,4786
-hidet/transforms/rule_based_simplifier.py,sha256=NSMQ_RKE83mNbNVGFwz0LO_Unxwm0fcDhKX117mthT8,10048
+hidet/transforms/rule_based_simplifier.py,sha256=hkW90nG5UpTQVDmSqeg6XvJLyB6_g-r3yi-zpZyoLwg,10235
 hidet/transforms/simplify_stmt.py,sha256=5-dFvpf30VfKtv4mKWAm1t6ganyVgPk7jwhYOKd52q8,1693
 hidet/transforms/common/__init__.py,sha256=JkcEQP8F10JE_EunYt-yMncLlhlxUj8ZoIvwqp1UHjU,623
-hidet/transforms/common/scope.py,sha256=7UQkmFCyT7qT3-5DUxsJms2wKpDSjp2tADBtGfGxpwY,5654
+hidet/transforms/common/scope.py,sha256=4gHPn9JyKMPcVhJZnJ9RqMlo3Lz7PszRbStZX8yMsYY,5662
 hidet/transforms/instruments/__init__.py,sha256=QOIDqnNL9iSfcuC3VCX031PHeDidTHmn39Gylimc2Ao,676
 hidet/transforms/instruments/base.py,sha256=CuOPSsRf6lb7SZ0FaVshWPFFHwDk8BQcy0h4clndwoE,892
 hidet/transforms/instruments/profile_instrument.py,sha256=B3eQ8T2KKuNZHdmF89hKXl05GeWSTWzAhxKNR62S3k4,1851
 hidet/transforms/instruments/save_ir_instrument.py,sha256=YqRMnn7o-hZz59i3w5juPZjW09j48SEX-GFh_ErzvtM,1552
-hidet/transforms/tools/__init__.py,sha256=gtQdwcAOXFi3YSr0ZC7CBNaPtkLEwXaa5b3DF_007mc,1281
-hidet/transforms/tools/apply_prologue_epilogue.py,sha256=kg72EY5Ov0spZ_yJs2X-N1vD1Y4a4_y3QDZhlooOC3A,10966
-hidet/transforms/tools/generate_packed_func.py,sha256=9CezcESa6e1L5EXgL9nNNJjE2PaJWELNwHtinwH98mA,5376
-hidet/utils/__init__.py,sha256=bYXgKmkYVHrRv4Zxlvb4hRrzmeZwtyfPBWojHtoW1aw,1150
+hidet/utils/__init__.py,sha256=mh8gCvgOb-wx2a2itQJ9BmIri4wZ7tVt9rLvxISRc80,1160
 hidet/utils/bench.py,sha256=sMTGUowPLQ54Jg4VCDYlyPeeiU5gyBEg0h1dKenMP9U,2184
 hidet/utils/cache_utils.py,sha256=IRYQyXG4HTHcX-Ov2Sa7kGmpBGi6u2thsQF8KsJtLFk,1176
 hidet/utils/doc.py,sha256=ECGAa5zX9Kj8915Fk5rkve9BynafxRwxt6HPTCW65UM,3283
 hidet/utils/exiting.py,sha256=aeXtzaFz_Lhw2z_5lSOJ21fDnQj5zi56pLhC2tkxYSM,1666
 hidet/utils/git_utils.py,sha256=2nif-3UdTY06vW3Ig_B7hpapnIzei7fedXTj9M8bEWE,2664
 hidet/utils/namer.py,sha256=4vC2AmYCEFYE8MnshvEkC4yCN4OCeRkT2YKkK4RdX1s,2401
 hidet/utils/net_utils.py,sha256=P_d1RzkFVYX5gRrx9eQTvnU34EIhrg_X3W86J8mgZco,2471
 hidet/utils/netron.py,sha256=WosRlCq0_Rqj0PRA2V5Dob1zBfxgE1YCuub2OGM1wIE,8524
 hidet/utils/ort_utils.py,sha256=eWtfBsNtZS4-iczBmnIT5fEdch6UVgAEiHYBL-8Dp80,2275
 hidet/utils/overrides.py,sha256=fPHAewYVgdeC-y2asRjMyuAEyLuGcQWe5NLvqFKPsls,785
-hidet/utils/py.py,sha256=HDUJ3jsT4HfheWX7yev3som6K4yMESngCtZ6mk1LFXs,11319
+hidet/utils/py.py,sha256=Ekz8L1y8Wa0kGXrmhDgqmnYAJ5yAOlQJClOpJLN87is,11570
 hidet/utils/stack_limit.py,sha256=AyP-JDTeMCJB6UJVpFwjb2sDakSwLXFiMf406F3yWCc,822
 hidet/utils/structure.py,sha256=ydP6NWWSMRT6Ctt0gr2Dd7TAhJYVwZvTL3V7SY24wnM,4794
 hidet/utils/torch_utils.py,sha256=4Rrx1f4L2EAhnxfsHjewxfPTV5cQ5OIolp54E-oIIWs,2272
 hidet/utils/transformers_utils.py,sha256=Md0EixR_HsPxjb1koPakY3Kf4Raca6wan0yIYI-93DA,1891
-hidet-0.2.2.dist-info/METADATA,sha256=na-rTwjQKs0V1uZhD7_WBoK38t5i_UxTA8ws2rrkOBE,4096
-hidet-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hidet-0.2.2.dist-info/entry_points.txt,sha256=wYQSqJRmAO73kWszS87YSet63vBfLTwZ9Bn3cQpqnzs,136
-hidet-0.2.2.dist-info/top_level.txt,sha256=7orBmjHo1P1KeDWR9XJPNqWOpl-UeoImAAv10voCab4,6
-hidet-0.2.2.dist-info/RECORD,,
+hidet-0.2.3.dist-info/METADATA,sha256=wrnyRVe8bLu4jRjxwj7-MmWms_5JZJkNupaFwcO7jf8,3878
+hidet-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hidet-0.2.3.dist-info/entry_points.txt,sha256=wYQSqJRmAO73kWszS87YSet63vBfLTwZ9Bn3cQpqnzs,136
+hidet-0.2.3.dist-info/top_level.txt,sha256=7orBmjHo1P1KeDWR9XJPNqWOpl-UeoImAAv10voCab4,6
+hidet-0.2.3.dist-info/RECORD,,
```

