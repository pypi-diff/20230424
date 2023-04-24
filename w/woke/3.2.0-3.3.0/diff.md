# Comparing `tmp/woke-3.2.0.tar.gz` & `tmp/woke-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woke-3.2.0.tar", max compression
+gzip compressed data, was "woke-3.3.0.tar", max compression
```

## Comparing `woke-3.2.0.tar` & `woke-3.3.0.tar`

### file list

```diff
@@ -1,238 +1,238 @@
--rw-r--r--   0        0        0      751 2023-04-03 13:13:18.467843 woke-3.2.0/LICENSE
--rw-r--r--   0        0        0     3423 2023-04-03 13:13:18.474510 woke-3.2.0/README.md
--rw-r--r--   0        0        0     2655 2023-04-12 19:11:29.746527 woke-3.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/__init__.py
--rw-r--r--   0        0        0    20349 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/cfg.py
--rw-r--r--   0        0        0     1013 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/__init__.py
--rw-r--r--   0        0        0    21690 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/api.py
--rw-r--r--   0        0        0       61 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/axelar/__init__.py
--rw-r--r--   0        0        0    14739 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/axelar/proxy_contract_id.py
--rw-r--r--   0        0        0     6292 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/balance_state_var.py
--rw-r--r--   0        0        0     4759 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/bug_empty_byte_array_copy.py
--rw-r--r--   0        0        0     1777 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/call_options_not_called.py
--rw-r--r--   0        0        0     4162 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/missing_return.py
--rw-r--r--   0        0        0     3013 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/msg_value_nonpayable_function.py
--rw-r--r--   0        0        0     8578 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
--rw-r--r--   0        0        0    17003 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/ownable.py
--rw-r--r--   0        0        0    23312 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/proxy_contract_selector_clashes.py
--rw-r--r--   0        0        0    13896 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/reentrancy.py
--rw-r--r--   0        0        0     2766 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unchecked_return_value.py
--rw-r--r--   0        0        0     6242 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unsafe_delegatecall.py
--rw-r--r--   0        0        0     1344 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unsafe_selfdestruct.py
--rw-r--r--   0        0        0     5982 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unsafe_tx_origin.py
--rw-r--r--   0        0        0     1397 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/unused_contract.py
--rw-r--r--   0        0        0    12233 2023-04-03 13:13:18.504510 woke-3.2.0/woke/analysis/detectors/utils.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/__init__.py
--rw-r--r--   0        0        0    10921 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/enums.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/__init__.py
--rw-r--r--   0        0        0     5939 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/abc.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/__init__.py
--rw-r--r--   0        0        0     5854 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/abc.py
--rw-r--r--   0        0        0    16242 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/contract_definition.py
--rw-r--r--   0        0        0     2460 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/enum_definition.py
--rw-r--r--   0        0        0     1360 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/enum_value.py
--rw-r--r--   0        0        0     4391 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/error_definition.py
--rw-r--r--   0        0        0     5162 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/event_definition.py
--rw-r--r--   0        0        0    18673 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/function_definition.py
--rw-r--r--   0        0        0    12886 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/modifier_definition.py
--rw-r--r--   0        0        0     2769 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/struct_definition.py
--rw-r--r--   0        0        0     2654 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/user_defined_value_type_definition.py
--rw-r--r--   0        0        0    17582 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/declaration/variable_declaration.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/__init__.py
--rw-r--r--   0        0        0     6583 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/abc.py
--rw-r--r--   0        0        0     3975 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/assignment.py
--rw-r--r--   0        0        0     2959 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/binary_operation.py
--rw-r--r--   0        0        0     2087 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/conditional.py
--rw-r--r--   0        0        0     1361 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/elementary_type_name_expression.py
--rw-r--r--   0        0        0     8923 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/function_call.py
--rw-r--r--   0        0        0     2132 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/function_call_options.py
--rw-r--r--   0        0        0     4446 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/identifier.py
--rw-r--r--   0        0        0     1996 2023-04-03 13:13:18.504510 woke-3.2.0/woke/ast/ir/expression/index_access.py
--rw-r--r--   0        0        0     2661 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/index_range_access.py
--rw-r--r--   0        0        0     1437 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/literal.py
--rw-r--r--   0        0        0    18452 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/member_access.py
--rw-r--r--   0        0        0     1376 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/new_expression.py
--rw-r--r--   0        0        0     2186 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/tuple_expression.py
--rw-r--r--   0        0        0     3071 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/expression/unary_operation.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/__init__.py
--rw-r--r--   0        0        0     8531 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/identifier_path.py
--rw-r--r--   0        0        0     8845 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/import_directive.py
--rw-r--r--   0        0        0     3751 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/inheritance_specifier.py
--rw-r--r--   0        0        0     5699 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/modifier_invocation.py
--rw-r--r--   0        0        0     3456 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/override_specifier.py
--rw-r--r--   0        0        0     4305 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/parameter_list.py
--rw-r--r--   0        0        0     1529 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/pragma_directive.py
--rw-r--r--   0        0        0     9257 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/source_unit.py
--rw-r--r--   0        0        0     2314 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/structured_documentation.py
--rw-r--r--   0        0        0     4541 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/try_catch_clause.py
--rw-r--r--   0        0        0     5698 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/meta/using_for_directive.py
--rw-r--r--   0        0        0     4849 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/reference_resolver.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/__init__.py
--rw-r--r--   0        0        0     5607 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/abc.py
--rw-r--r--   0        0        0     3130 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/block.py
--rw-r--r--   0        0        0     1610 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/break_statement.py
--rw-r--r--   0        0        0     1634 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/continue_statement.py
--rw-r--r--   0        0        0     2563 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/do_while_statement.py
--rw-r--r--   0        0        0     2452 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/emit_statement.py
--rw-r--r--   0        0        0     6016 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/expression_statement.py
--rw-r--r--   0        0        0     5735 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/for_statement.py
--rw-r--r--   0        0        0     3423 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/if_statement.py
--rw-r--r--   0        0        0    10271 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/inline_assembly.py
--rw-r--r--   0        0        0     1582 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/placeholder_statement.py
--rw-r--r--   0        0        0     3336 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/return_statement.py
--rw-r--r--   0        0        0     2608 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/revert_statement.py
--rw-r--r--   0        0        0     3129 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/try_statement.py
--rw-r--r--   0        0        0     2449 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/unchecked_block.py
--rw-r--r--   0        0        0     4325 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/variable_declaration_statement.py
--rw-r--r--   0        0        0     2596 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/statement/while_statement.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/__init__.py
--rw-r--r--   0        0        0     4932 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/abc.py
--rw-r--r--   0        0        0     4036 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/array_type_name.py
--rw-r--r--   0        0        0     5647 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/elementary_type_name.py
--rw-r--r--   0        0        0     3971 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/function_type_name.py
--rw-r--r--   0        0        0     3922 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/mapping.py
--rw-r--r--   0        0        0     8333 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/type_name/user_defined_type_name.py
--rw-r--r--   0        0        0       36 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/utils/__init__.py
--rw-r--r--   0        0        0      589 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/utils/init_tuple.py
--rw-r--r--   0        0        0      578 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/__init__.py
--rw-r--r--   0        0        0      703 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/abc.py
--rw-r--r--   0        0        0     1811 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/assignment.py
--rw-r--r--   0        0        0     4302 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/block.py
--rw-r--r--   0        0        0      300 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/break_statement.py
--rw-r--r--   0        0        0     1199 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/case_statement.py
--rw-r--r--   0        0        0      303 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/continue_statement.py
--rw-r--r--   0        0        0     1658 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/expression_statement.py
--rw-r--r--   0        0        0     1893 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/for_loop.py
--rw-r--r--   0        0        0     2317 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/function_call.py
--rw-r--r--   0        0        0     2288 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/function_definition.py
--rw-r--r--   0        0        0     1492 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/identifier.py
--rw-r--r--   0        0        0     1582 2023-04-03 13:13:18.507843 woke-3.2.0/woke/ast/ir/yul/if_statement.py
--rw-r--r--   0        0        0      300 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/leave.py
--rw-r--r--   0        0        0     1780 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/literal.py
--rw-r--r--   0        0        0     1796 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/switch.py
--rw-r--r--   0        0        0      920 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/typed_name.py
--rw-r--r--   0        0        0     2091 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/ir/yul/variable_declaration.py
--rw-r--r--   0        0        0    37545 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/nodes.py
--rw-r--r--   0        0        0    47040 2023-04-03 13:13:18.511176 woke-3.2.0/woke/ast/types.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/__init__.py
--rw-r--r--   0        0        0     3500 2023-04-12 19:11:06.759862 woke-3.2.0/woke/cli/__main__.py
--rw-r--r--   0        0        0     7942 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/accounts.py
--rw-r--r--   0        0        0     4650 2023-04-06 18:42:41.395142 woke-3.2.0/woke/cli/compile.py
--rw-r--r--   0        0        0       54 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/console.py
--rw-r--r--   0        0        0     3838 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/detect.py
--rw-r--r--   0        0        0     3791 2023-04-12 19:11:06.759862 woke-3.2.0/woke/cli/fuzz.py
--rw-r--r--   0        0        0    11813 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/init.py
--rw-r--r--   0        0        0     1081 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/lsp.py
--rw-r--r--   0        0        0     3154 2023-04-12 19:11:06.759862 woke-3.2.0/woke/cli/run.py
--rw-r--r--   0        0        0     4922 2023-04-03 13:13:18.511176 woke-3.2.0/woke/cli/svm.py
--rw-r--r--   0        0        0     2258 2023-04-11 08:46:32.102660 woke-3.2.0/woke/cli/test.py
--rw-r--r--   0        0        0      187 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/__init__.py
--rw-r--r--   0        0        0     1814 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/build_data_model.py
--rw-r--r--   0        0        0     3078 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/compilation_unit.py
--rw-r--r--   0        0        0    40866 2023-04-10 08:07:29.589366 woke-3.2.0/woke/compiler/compiler.py
--rw-r--r--   0        0        0       97 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/exceptions.py
--rw-r--r--   0        0        0      103 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/__init__.py
--rw-r--r--   0        0        0       48 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/exceptions.py
--rw-r--r--   0        0        0     8554 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/input_data_model.py
--rw-r--r--   0        0        0     8728 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/output_data_model.py
--rw-r--r--   0        0        0     3571 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/solc_frontend/solc_runner.py
--rw-r--r--   0        0        0     2455 2023-04-03 13:13:18.511176 woke-3.2.0/woke/compiler/source_path_resolver.py
--rw-r--r--   0        0        0     4819 2023-04-10 08:45:44.228249 woke-3.2.0/woke/compiler/source_unit_name_resolver.py
--rw-r--r--   0        0        0     1118 2023-04-03 13:13:18.511176 woke-3.2.0/woke/config/__init__.py
--rw-r--r--   0        0        0     6866 2023-04-06 13:04:44.339069 woke-3.2.0/woke/config/data_model.py
--rw-r--r--   0        0        0    12617 2023-04-05 07:53:42.584834 woke-3.2.0/woke/config/woke_config.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/contracts/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/contracts/woke/__init__.py
--rw-r--r--   0        0        0    64087 2023-04-03 13:13:18.511176 woke-3.2.0/woke/contracts/woke/console.sol
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/core/__init__.py
--rw-r--r--   0        0        0      360 2023-04-03 13:13:18.511176 woke-3.2.0/woke/core/enums.py
--rw-r--r--   0        0        0    24824 2023-04-03 13:13:18.511176 woke-3.2.0/woke/core/solidity_version.py
--rw-r--r--   0        0        0      663 2023-04-03 13:13:18.511176 woke-3.2.0/woke/deployment/__init__.py
--rw-r--r--   0        0        0    14322 2023-04-12 19:11:06.759862 woke-3.2.0/woke/deployment/core.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.511176 woke-3.2.0/woke/development/__init__.py
--rw-r--r--   0        0        0     4552 2023-04-03 13:13:18.511176 woke-3.2.0/woke/development/blocks.py
--rw-r--r--   0        0        0    28998 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/call_trace.py
--rw-r--r--   0        0        0    26323 2023-04-11 09:25:36.391768 woke-3.2.0/woke/development/chain_interfaces.py
--rw-r--r--   0        0        0     1132 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/constants.py
--rw-r--r--   0        0        0    94704 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/core.py
--rw-r--r--   0        0        0     7222 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/globals.py
--rw-r--r--   0        0        0   161115 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/hardhat_console.py
--rw-r--r--   0        0        0     1093 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/internal.py
--rw-r--r--   0        0        0       39 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/__init__.py
--rw-r--r--   0        0        0      302 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/abc.py
--rw-r--r--   0        0        0     2070 2023-04-05 07:27:39.545655 woke-3.2.0/woke/development/json_rpc/communicator.py
--rw-r--r--   0        0        0      821 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/http.py
--rw-r--r--   0        0        0     2733 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/ipc.py
--rw-r--r--   0        0        0      625 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/json_rpc/websocket.py
--rw-r--r--   0        0        0     6572 2023-04-03 13:13:18.514510 woke-3.2.0/woke/development/primitive_types.py
--rw-r--r--   0        0        0    88054 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/pytypes_generator.py
--rw-r--r--   0        0        0    26578 2023-04-12 19:11:06.763195 woke-3.2.0/woke/development/transactions.py
--rw-r--r--   0        0        0     7389 2023-04-05 07:53:42.588167 woke-3.2.0/woke/development/utils.py
--rw-r--r--   0        0        0       47 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/__init__.py
--rw-r--r--   0        0        0      310 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/__init__.py
--rw-r--r--   0        0        0     3648 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/generate_control_flow_graph.py
--rw-r--r--   0        0        0      938 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/generate_imports_graph.py
--rw-r--r--   0        0        0     4247 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/generate_inheritance_graph.py
--rw-r--r--   0        0        0     2163 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/commands/generate_linearized_inheritance_graph.py
--rw-r--r--   0        0        0    31330 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/common_structures.py
--rw-r--r--   0        0        0     1721 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/context.py
--rw-r--r--   0        0        0     2574 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/document_sync.py
--rw-r--r--   0        0        0      130 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/enums.py
--rw-r--r--   0        0        0      471 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/__init__.py
--rw-r--r--   0        0        0     9946 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/code_lens.py
--rw-r--r--   0        0        0    14531 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/features/completion.py
--rw-r--r--   0        0        0     9664 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/definition.py
--rw-r--r--   0        0        0     1446 2023-04-06 18:43:28.740922 woke-3.2.0/woke/lsp/features/diagnostic.py
--rw-r--r--   0        0        0     3908 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/document_link.py
--rw-r--r--   0        0        0     8407 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/document_symbol.py
--rw-r--r--   0        0        0    11205 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/features/hover.py
--rw-r--r--   0        0        0     3850 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/implementation.py
--rw-r--r--   0        0        0     5092 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/references.py
--rw-r--r--   0        0        0     8935 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/rename.py
--rw-r--r--   0        0        0     9505 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/type_definition.py
--rw-r--r--   0        0        0    11043 2023-04-03 13:13:18.514510 woke-3.2.0/woke/lsp/features/type_hierarchy.py
--rw-r--r--   0        0        0    37460 2023-04-09 08:21:30.944679 woke-3.2.0/woke/lsp/lsp_compiler.py
--rw-r--r--   0        0        0      328 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/lsp_data_model.py
--rw-r--r--   0        0        0     5551 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/methods.py
--rw-r--r--   0        0        0     1897 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/protocol_structures.py
--rw-r--r--   0        0        0     2229 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/rpc_protocol.py
--rw-r--r--   0        0        0    36478 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/server.py
--rw-r--r--   0        0        0     6541 2023-04-10 08:45:44.228249 woke-3.2.0/woke/lsp/server_capabilities.py
--rw-r--r--   0        0        0       86 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/utils/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/utils/position.py
--rw-r--r--   0        0        0      459 2023-04-03 13:13:18.517843 woke-3.2.0/woke/lsp/utils/uri.py
--rw-r--r--   0        0        0       50 2023-04-03 13:13:18.517843 woke-3.2.0/woke/regex_parser/__init__.py
--rw-r--r--   0        0        0     1690 2023-04-03 13:13:18.517843 woke-3.2.0/woke/regex_parser/solidity_import.py
--rw-r--r--   0        0        0     6653 2023-04-03 13:13:18.517843 woke-3.2.0/woke/regex_parser/solidity_parser.py
--rw-r--r--   0        0        0       36 2023-04-03 13:13:18.517843 woke-3.2.0/woke/svm/__init__.py
--rw-r--r--   0        0        0     1810 2023-04-03 13:13:18.517843 woke-3.2.0/woke/svm/abc.py
--rw-r--r--   0        0        0      270 2023-04-03 13:13:18.517843 woke-3.2.0/woke/svm/exceptions.py
--rw-r--r--   0        0        0    11716 2023-04-03 13:13:18.517843 woke-3.2.0/woke/svm/svm.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.517843 woke-3.2.0/woke/templates/scripts/__init__.py
--rw-r--r--   0        0        0      184 2023-04-03 13:13:18.517843 woke-3.2.0/woke/templates/scripts/deploy.py
--rw-r--r--   0        0        0        0 2023-04-03 13:13:18.517843 woke-3.2.0/woke/templates/tests/__init__.py
--rw-r--r--   0        0        0      140 2023-04-03 13:13:18.517843 woke-3.2.0/woke/templates/tests/test_default.py
--rw-r--r--   0        0        0      663 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/__init__.py
--rw-r--r--   0        0        0    11329 2023-04-12 19:11:06.763195 woke-3.2.0/woke/testing/core.py
--rw-r--r--   0        0        0    24360 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/coverage.py
--rw-r--r--   0        0        0      187 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/fuzzing/__init__.py
--rw-r--r--   0        0        0     4999 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/fuzzing/fuzz_test.py
--rw-r--r--   0        0        0    10795 2023-04-12 19:11:06.763195 woke-3.2.0/woke/testing/fuzzing/fuzzer.py
--rw-r--r--   0        0        0     5780 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/fuzzing/generators.py
--rw-r--r--   0        0        0      298 2023-04-03 13:13:18.517843 woke-3.2.0/woke/testing/pytest_plugin.py
--rw-r--r--   0        0        0      170 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/__init__.py
--rw-r--r--   0        0        0      560 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/context_managers.py
--rw-r--r--   0        0        0      513 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/decorators.py
--rw-r--r--   0        0        0      158 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/enums.py
--rw-r--r--   0        0        0     1699 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/file_utils.py
--rw-r--r--   0        0        0      383 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/keyed_default_dict.py
--rw-r--r--   0        0        0      194 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/networking.py
--rw-r--r--   0        0        0     1017 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/openzeppelin.py
--rw-r--r--   0        0        0      630 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/string.py
--rw-r--r--   0        0        0     1742 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/tee.py
--rw-r--r--   0        0        0     3765 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/threaded_child_watcher.py
--rw-r--r--   0        0        0      423 2023-04-03 13:13:18.517843 woke-3.2.0/woke/utils/version.py
--rw-r--r--   0        0        0     6058 1970-01-01 00:00:00.000000 woke-3.2.0/setup.py
--rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 woke-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0      751 2023-04-24 12:08:38.351342 woke-3.3.0/LICENSE
+-rw-r--r--   0        0        0     3423 2023-04-24 12:08:38.358009 woke-3.3.0/README.md
+-rw-r--r--   0        0        0     2655 2023-04-24 12:09:29.024419 woke-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.388009 woke-3.3.0/woke/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/__init__.py
+-rw-r--r--   0        0        0    20349 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/cfg.py
+-rw-r--r--   0        0        0     1013 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/__init__.py
+-rw-r--r--   0        0        0    21690 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/api.py
+-rw-r--r--   0        0        0       61 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/axelar/__init__.py
+-rw-r--r--   0        0        0    14739 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/axelar/proxy_contract_id.py
+-rw-r--r--   0        0        0     6292 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/balance_state_var.py
+-rw-r--r--   0        0        0     4759 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/bug_empty_byte_array_copy.py
+-rw-r--r--   0        0        0     1777 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/call_options_not_called.py
+-rw-r--r--   0        0        0     4162 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/missing_return.py
+-rw-r--r--   0        0        0     3013 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/msg_value_nonpayable_function.py
+-rw-r--r--   0        0        0     8578 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
+-rw-r--r--   0        0        0    17003 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/ownable.py
+-rw-r--r--   0        0        0    23312 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/proxy_contract_selector_clashes.py
+-rw-r--r--   0        0        0    13896 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/reentrancy.py
+-rw-r--r--   0        0        0     2766 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/unchecked_return_value.py
+-rw-r--r--   0        0        0     6242 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/unsafe_delegatecall.py
+-rw-r--r--   0        0        0     1344 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/unsafe_selfdestruct.py
+-rw-r--r--   0        0        0     5982 2023-04-24 12:08:38.391342 woke-3.3.0/woke/analysis/detectors/unsafe_tx_origin.py
+-rw-r--r--   0        0        0     1397 2023-04-24 12:08:38.391342 woke-3.3.0/woke/analysis/detectors/unused_contract.py
+-rw-r--r--   0        0        0    12233 2023-04-24 12:08:38.391342 woke-3.3.0/woke/analysis/detectors/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/__init__.py
+-rw-r--r--   0        0        0    10921 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/enums.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/__init__.py
+-rw-r--r--   0        0        0     5939 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/abc.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/__init__.py
+-rw-r--r--   0        0        0     5854 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/abc.py
+-rw-r--r--   0        0        0    16242 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/contract_definition.py
+-rw-r--r--   0        0        0     2460 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/enum_definition.py
+-rw-r--r--   0        0        0     1360 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/enum_value.py
+-rw-r--r--   0        0        0     4391 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/error_definition.py
+-rw-r--r--   0        0        0     5162 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/event_definition.py
+-rw-r--r--   0        0        0    18673 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/function_definition.py
+-rw-r--r--   0        0        0    12886 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/modifier_definition.py
+-rw-r--r--   0        0        0     2769 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/struct_definition.py
+-rw-r--r--   0        0        0     2654 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/user_defined_value_type_definition.py
+-rw-r--r--   0        0        0    17582 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/variable_declaration.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/__init__.py
+-rw-r--r--   0        0        0     6583 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/abc.py
+-rw-r--r--   0        0        0     3975 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/assignment.py
+-rw-r--r--   0        0        0     2959 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/binary_operation.py
+-rw-r--r--   0        0        0     2087 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/conditional.py
+-rw-r--r--   0        0        0     1361 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/elementary_type_name_expression.py
+-rw-r--r--   0        0        0     8923 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/function_call.py
+-rw-r--r--   0        0        0     2132 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/function_call_options.py
+-rw-r--r--   0        0        0     4446 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/identifier.py
+-rw-r--r--   0        0        0     1996 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/index_access.py
+-rw-r--r--   0        0        0     2661 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/index_range_access.py
+-rw-r--r--   0        0        0     1437 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/literal.py
+-rw-r--r--   0        0        0    18452 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/member_access.py
+-rw-r--r--   0        0        0     1376 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/new_expression.py
+-rw-r--r--   0        0        0     2186 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/tuple_expression.py
+-rw-r--r--   0        0        0     3071 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/unary_operation.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/__init__.py
+-rw-r--r--   0        0        0     9095 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/identifier_path.py
+-rw-r--r--   0        0        0     8845 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/import_directive.py
+-rw-r--r--   0        0        0     3751 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/inheritance_specifier.py
+-rw-r--r--   0        0        0     5699 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/modifier_invocation.py
+-rw-r--r--   0        0        0     3456 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/override_specifier.py
+-rw-r--r--   0        0        0     4305 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/parameter_list.py
+-rw-r--r--   0        0        0     1529 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/pragma_directive.py
+-rw-r--r--   0        0        0     9257 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/source_unit.py
+-rw-r--r--   0        0        0     2314 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/structured_documentation.py
+-rw-r--r--   0        0        0     4541 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/try_catch_clause.py
+-rw-r--r--   0        0        0     5698 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/using_for_directive.py
+-rw-r--r--   0        0        0     4812 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/reference_resolver.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/__init__.py
+-rw-r--r--   0        0        0     5607 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/abc.py
+-rw-r--r--   0        0        0     3130 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/block.py
+-rw-r--r--   0        0        0     1610 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/break_statement.py
+-rw-r--r--   0        0        0     1634 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/continue_statement.py
+-rw-r--r--   0        0        0     2563 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/do_while_statement.py
+-rw-r--r--   0        0        0     2452 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/emit_statement.py
+-rw-r--r--   0        0        0     6016 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/expression_statement.py
+-rw-r--r--   0        0        0     5735 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/for_statement.py
+-rw-r--r--   0        0        0     3423 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/if_statement.py
+-rw-r--r--   0        0        0    10271 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/inline_assembly.py
+-rw-r--r--   0        0        0     1582 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/placeholder_statement.py
+-rw-r--r--   0        0        0     3336 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/return_statement.py
+-rw-r--r--   0        0        0     2608 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/revert_statement.py
+-rw-r--r--   0        0        0     3129 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/try_statement.py
+-rw-r--r--   0        0        0     2449 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/unchecked_block.py
+-rw-r--r--   0        0        0     4325 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/variable_declaration_statement.py
+-rw-r--r--   0        0        0     2596 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/while_statement.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/__init__.py
+-rw-r--r--   0        0        0     4932 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/abc.py
+-rw-r--r--   0        0        0     4036 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/array_type_name.py
+-rw-r--r--   0        0        0     5647 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/elementary_type_name.py
+-rw-r--r--   0        0        0     3971 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/function_type_name.py
+-rw-r--r--   0        0        0     3922 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/mapping.py
+-rw-r--r--   0        0        0     8333 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/user_defined_type_name.py
+-rw-r--r--   0        0        0       36 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/utils/__init__.py
+-rw-r--r--   0        0        0      589 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/utils/init_tuple.py
+-rw-r--r--   0        0        0      578 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/yul/__init__.py
+-rw-r--r--   0        0        0      703 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/abc.py
+-rw-r--r--   0        0        0     1811 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/assignment.py
+-rw-r--r--   0        0        0     4302 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/block.py
+-rw-r--r--   0        0        0      300 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/break_statement.py
+-rw-r--r--   0        0        0     1199 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/case_statement.py
+-rw-r--r--   0        0        0      303 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/continue_statement.py
+-rw-r--r--   0        0        0     1658 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/expression_statement.py
+-rw-r--r--   0        0        0     1893 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/for_loop.py
+-rw-r--r--   0        0        0     2317 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/function_call.py
+-rw-r--r--   0        0        0     2288 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/function_definition.py
+-rw-r--r--   0        0        0     1492 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/identifier.py
+-rw-r--r--   0        0        0     1582 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/if_statement.py
+-rw-r--r--   0        0        0      300 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/leave.py
+-rw-r--r--   0        0        0     1780 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/literal.py
+-rw-r--r--   0        0        0     1796 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/switch.py
+-rw-r--r--   0        0        0      920 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/typed_name.py
+-rw-r--r--   0        0        0     2091 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/variable_declaration.py
+-rw-r--r--   0        0        0    37545 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/nodes.py
+-rw-r--r--   0        0        0    47040 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/types.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/__init__.py
+-rw-r--r--   0        0        0     3500 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/__main__.py
+-rw-r--r--   0        0        0     7942 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/accounts.py
+-rw-r--r--   0        0        0     4650 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/compile.py
+-rw-r--r--   0        0        0       54 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/console.py
+-rw-r--r--   0        0        0     3838 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/detect.py
+-rw-r--r--   0        0        0     3791 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/fuzz.py
+-rw-r--r--   0        0        0    11813 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/init.py
+-rw-r--r--   0        0        0     1081 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/lsp.py
+-rw-r--r--   0        0        0     3154 2023-04-24 12:08:38.398009 woke-3.3.0/woke/cli/run.py
+-rw-r--r--   0        0        0     4922 2023-04-24 12:08:38.398009 woke-3.3.0/woke/cli/svm.py
+-rw-r--r--   0        0        0     2258 2023-04-24 12:08:38.398009 woke-3.3.0/woke/cli/test.py
+-rw-r--r--   0        0        0      187 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/__init__.py
+-rw-r--r--   0        0        0     1814 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/build_data_model.py
+-rw-r--r--   0        0        0     3078 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/compilation_unit.py
+-rw-r--r--   0        0        0    41519 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/compiler.py
+-rw-r--r--   0        0        0       97 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/exceptions.py
+-rw-r--r--   0        0        0      103 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/exceptions.py
+-rw-r--r--   0        0        0     8554 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/input_data_model.py
+-rw-r--r--   0        0        0     8728 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/output_data_model.py
+-rw-r--r--   0        0        0     3571 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/solc_runner.py
+-rw-r--r--   0        0        0     2455 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/source_path_resolver.py
+-rw-r--r--   0        0        0     4819 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/source_unit_name_resolver.py
+-rw-r--r--   0        0        0     1118 2023-04-24 12:08:38.398009 woke-3.3.0/woke/config/__init__.py
+-rw-r--r--   0        0        0     6866 2023-04-24 12:08:38.398009 woke-3.3.0/woke/config/data_model.py
+-rw-r--r--   0        0        0    12617 2023-04-24 12:08:38.398009 woke-3.3.0/woke/config/woke_config.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.3.0/woke/contracts/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.3.0/woke/contracts/woke/__init__.py
+-rw-r--r--   0        0        0    64087 2023-04-24 12:08:38.398009 woke-3.3.0/woke/contracts/woke/console.sol
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.3.0/woke/core/__init__.py
+-rw-r--r--   0        0        0      360 2023-04-24 12:08:38.398009 woke-3.3.0/woke/core/enums.py
+-rw-r--r--   0        0        0    24824 2023-04-24 12:08:38.398009 woke-3.3.0/woke/core/solidity_version.py
+-rw-r--r--   0        0        0      663 2023-04-24 12:08:38.398009 woke-3.3.0/woke/deployment/__init__.py
+-rw-r--r--   0        0        0    14901 2023-04-24 12:08:38.398009 woke-3.3.0/woke/deployment/core.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/__init__.py
+-rw-r--r--   0        0        0     4552 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/blocks.py
+-rw-r--r--   0        0        0    28998 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/call_trace.py
+-rw-r--r--   0        0        0    25863 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/chain_interfaces.py
+-rw-r--r--   0        0        0     1132 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/constants.py
+-rw-r--r--   0        0        0    95503 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/core.py
+-rw-r--r--   0        0        0     7270 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/globals.py
+-rw-r--r--   0        0        0   161115 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/hardhat_console.py
+-rw-r--r--   0        0        0     1093 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/internal.py
+-rw-r--r--   0        0        0       39 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/abc.py
+-rw-r--r--   0        0        0     2070 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/communicator.py
+-rw-r--r--   0        0        0      821 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/http.py
+-rw-r--r--   0        0        0     2733 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/ipc.py
+-rw-r--r--   0        0        0      625 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/websocket.py
+-rw-r--r--   0        0        0     6572 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/primitive_types.py
+-rw-r--r--   0        0        0    88054 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/pytypes_generator.py
+-rw-r--r--   0        0        0    26697 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/transactions.py
+-rw-r--r--   0        0        0     7389 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/utils.py
+-rw-r--r--   0        0        0       47 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/__init__.py
+-rw-r--r--   0        0        0     3648 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/generate_control_flow_graph.py
+-rw-r--r--   0        0        0      938 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/generate_imports_graph.py
+-rw-r--r--   0        0        0     4247 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/generate_inheritance_graph.py
+-rw-r--r--   0        0        0     2163 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/generate_linearized_inheritance_graph.py
+-rw-r--r--   0        0        0    31330 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/common_structures.py
+-rw-r--r--   0        0        0     1721 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/context.py
+-rw-r--r--   0        0        0     2574 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/document_sync.py
+-rw-r--r--   0        0        0      130 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/enums.py
+-rw-r--r--   0        0        0      471 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/__init__.py
+-rw-r--r--   0        0        0     9946 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/code_lens.py
+-rw-r--r--   0        0        0    14531 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/completion.py
+-rw-r--r--   0        0        0     9948 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/definition.py
+-rw-r--r--   0        0        0     1446 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/diagnostic.py
+-rw-r--r--   0        0        0     3908 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/document_link.py
+-rw-r--r--   0        0        0     8407 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/document_symbol.py
+-rw-r--r--   0        0        0    11205 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/hover.py
+-rw-r--r--   0        0        0     3850 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/implementation.py
+-rw-r--r--   0        0        0     5092 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/references.py
+-rw-r--r--   0        0        0     8935 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/rename.py
+-rw-r--r--   0        0        0     9505 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/type_definition.py
+-rw-r--r--   0        0        0    11043 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/type_hierarchy.py
+-rw-r--r--   0        0        0    37512 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/lsp_compiler.py
+-rw-r--r--   0        0        0      328 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/lsp_data_model.py
+-rw-r--r--   0        0        0     5551 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/methods.py
+-rw-r--r--   0        0        0     1897 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/protocol_structures.py
+-rw-r--r--   0        0        0     2229 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/rpc_protocol.py
+-rw-r--r--   0        0        0    36478 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/server.py
+-rw-r--r--   0        0        0     6541 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/server_capabilities.py
+-rw-r--r--   0        0        0       86 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/utils/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/utils/position.py
+-rw-r--r--   0        0        0      459 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/utils/uri.py
+-rw-r--r--   0        0        0       50 2023-04-24 12:08:38.401342 woke-3.3.0/woke/regex_parser/__init__.py
+-rw-r--r--   0        0        0     1690 2023-04-24 12:08:38.401342 woke-3.3.0/woke/regex_parser/solidity_import.py
+-rw-r--r--   0        0        0     6653 2023-04-24 12:08:38.401342 woke-3.3.0/woke/regex_parser/solidity_parser.py
+-rw-r--r--   0        0        0       36 2023-04-24 12:08:38.401342 woke-3.3.0/woke/svm/__init__.py
+-rw-r--r--   0        0        0     1810 2023-04-24 12:08:38.404675 woke-3.3.0/woke/svm/abc.py
+-rw-r--r--   0        0        0      270 2023-04-24 12:08:38.404675 woke-3.3.0/woke/svm/exceptions.py
+-rw-r--r--   0        0        0    11716 2023-04-24 12:08:38.404675 woke-3.3.0/woke/svm/svm.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.404675 woke-3.3.0/woke/templates/scripts/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-24 12:08:38.404675 woke-3.3.0/woke/templates/scripts/deploy.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.404675 woke-3.3.0/woke/templates/tests/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-24 12:08:38.404675 woke-3.3.0/woke/templates/tests/test_default.py
+-rw-r--r--   0        0        0      663 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/__init__.py
+-rw-r--r--   0        0        0    10878 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/core.py
+-rw-r--r--   0        0        0    24360 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/coverage.py
+-rw-r--r--   0        0        0      187 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/fuzzing/__init__.py
+-rw-r--r--   0        0        0     4999 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/fuzzing/fuzz_test.py
+-rw-r--r--   0        0        0    10795 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/fuzzing/fuzzer.py
+-rw-r--r--   0        0        0     5780 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/fuzzing/generators.py
+-rw-r--r--   0        0        0      298 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/pytest_plugin.py
+-rw-r--r--   0        0        0      170 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/__init__.py
+-rw-r--r--   0        0        0      560 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/context_managers.py
+-rw-r--r--   0        0        0      513 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/decorators.py
+-rw-r--r--   0        0        0      158 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/enums.py
+-rw-r--r--   0        0        0     1699 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/file_utils.py
+-rw-r--r--   0        0        0      383 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/keyed_default_dict.py
+-rw-r--r--   0        0        0      194 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/networking.py
+-rw-r--r--   0        0        0     1017 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/openzeppelin.py
+-rw-r--r--   0        0        0      630 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/string.py
+-rw-r--r--   0        0        0     1742 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/tee.py
+-rw-r--r--   0        0        0     3765 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/threaded_child_watcher.py
+-rw-r--r--   0        0        0      423 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/version.py
+-rw-r--r--   0        0        0     6058 1970-01-01 00:00:00.000000 woke-3.3.0/setup.py
+-rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 woke-3.3.0/PKG-INFO
```

### Comparing `woke-3.2.0/LICENSE` & `woke-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/README.md` & `woke-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/pyproject.toml` & `woke-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "woke"
-version = "3.2.0"
+version = "3.3.0"
 description = "Woke is a Python-based development and testing framework for Solidity."
 license = "ISC"
 authors = ["Ackee Blockchain"]
 readme = "README.md"
 homepage = "https://ackeeblockchain.com"
 repository = "https://github.com/Ackee-Blockchain/woke"
 documentation = "https://ackeeblockchain.com/woke/docs/latest"
```

### Comparing `woke-3.2.0/woke/analysis/cfg.py` & `woke-3.3.0/woke/analysis/cfg.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/__init__.py` & `woke-3.3.0/woke/analysis/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/api.py` & `woke-3.3.0/woke/analysis/detectors/api.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/axelar/proxy_contract_id.py` & `woke-3.3.0/woke/analysis/detectors/axelar/proxy_contract_id.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/balance_state_var.py` & `woke-3.3.0/woke/analysis/detectors/balance_state_var.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/bug_empty_byte_array_copy.py` & `woke-3.3.0/woke/analysis/detectors/bug_empty_byte_array_copy.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/call_options_not_called.py` & `woke-3.3.0/woke/analysis/detectors/call_options_not_called.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/missing_return.py` & `woke-3.3.0/woke/analysis/detectors/missing_return.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/msg_value_nonpayable_function.py` & `woke-3.3.0/woke/analysis/detectors/msg_value_nonpayable_function.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py` & `woke-3.3.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/ownable.py` & `woke-3.3.0/woke/analysis/detectors/ownable.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/proxy_contract_selector_clashes.py` & `woke-3.3.0/woke/analysis/detectors/proxy_contract_selector_clashes.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/reentrancy.py` & `woke-3.3.0/woke/analysis/detectors/reentrancy.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/unchecked_return_value.py` & `woke-3.3.0/woke/analysis/detectors/unchecked_return_value.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/unsafe_delegatecall.py` & `woke-3.3.0/woke/analysis/detectors/unsafe_delegatecall.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/unsafe_selfdestruct.py` & `woke-3.3.0/woke/analysis/detectors/unsafe_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/unsafe_tx_origin.py` & `woke-3.3.0/woke/analysis/detectors/unsafe_tx_origin.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/unused_contract.py` & `woke-3.3.0/woke/analysis/detectors/unused_contract.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/analysis/detectors/utils.py` & `woke-3.3.0/woke/analysis/detectors/utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/enums.py` & `woke-3.3.0/woke/ast/enums.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/abc.py` & `woke-3.3.0/woke/ast/ir/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/abc.py` & `woke-3.3.0/woke/ast/ir/declaration/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/contract_definition.py` & `woke-3.3.0/woke/ast/ir/declaration/contract_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/enum_definition.py` & `woke-3.3.0/woke/ast/ir/declaration/enum_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/enum_value.py` & `woke-3.3.0/woke/ast/ir/declaration/enum_value.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/error_definition.py` & `woke-3.3.0/woke/ast/ir/declaration/error_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/event_definition.py` & `woke-3.3.0/woke/ast/ir/declaration/event_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/function_definition.py` & `woke-3.3.0/woke/ast/ir/declaration/function_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/modifier_definition.py` & `woke-3.3.0/woke/ast/ir/declaration/modifier_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/struct_definition.py` & `woke-3.3.0/woke/ast/ir/declaration/struct_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/user_defined_value_type_definition.py` & `woke-3.3.0/woke/ast/ir/declaration/user_defined_value_type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/declaration/variable_declaration.py` & `woke-3.3.0/woke/ast/ir/declaration/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/abc.py` & `woke-3.3.0/woke/ast/ir/expression/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/assignment.py` & `woke-3.3.0/woke/ast/ir/expression/assignment.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/binary_operation.py` & `woke-3.3.0/woke/ast/ir/expression/binary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/conditional.py` & `woke-3.3.0/woke/ast/ir/expression/conditional.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/elementary_type_name_expression.py` & `woke-3.3.0/woke/ast/ir/expression/elementary_type_name_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/function_call.py` & `woke-3.3.0/woke/ast/ir/expression/function_call.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/function_call_options.py` & `woke-3.3.0/woke/ast/ir/expression/function_call_options.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/identifier.py` & `woke-3.3.0/woke/ast/ir/expression/identifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/index_access.py` & `woke-3.3.0/woke/ast/ir/expression/index_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/index_range_access.py` & `woke-3.3.0/woke/ast/ir/expression/index_range_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/literal.py` & `woke-3.3.0/woke/ast/ir/expression/literal.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/member_access.py` & `woke-3.3.0/woke/ast/ir/expression/member_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/new_expression.py` & `woke-3.3.0/woke/ast/ir/expression/new_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/tuple_expression.py` & `woke-3.3.0/woke/ast/ir/expression/tuple_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/expression/unary_operation.py` & `woke-3.3.0/woke/ast/ir/expression/unary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/identifier_path.py` & `woke-3.3.0/woke/ast/ir/meta/identifier_path.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Tuple, Union
 
 if TYPE_CHECKING:
     from .inheritance_specifier import InheritanceSpecifier
     from .modifier_invocation import ModifierInvocation
     from .override_specifier import OverrideSpecifier
+    from .source_unit import SourceUnit
     from .using_for_directive import UsingForDirective
     from ..type_name.user_defined_type_name import UserDefinedTypeName
 
 from intervaltree import IntervalTree
 
 from woke.ast.ir.abc import SolidityAbc
 from woke.ast.ir.declaration.abc import DeclarationAbc
@@ -57,38 +58,44 @@
         self._file = init.file
         self._byte_location = byte_location
         self._name = name
 
         self._reference_resolver.register_post_process_callback(self._post_process)
 
     def _post_process(self, callback_params: CallbackParams):
+        from .source_unit import SourceUnit
+
         referenced_declaration = self._reference_resolver.resolve_node(
             self._path_referenced_declaration_id, self._cu_hash
         )
         for i in range(self._path_index):
             assert referenced_declaration.parent is not None
             referenced_declaration = referenced_declaration.parent
-        assert isinstance(referenced_declaration, DeclarationAbc)
+        assert isinstance(referenced_declaration, (DeclarationAbc, SourceUnit))
 
         node_path_order = self._reference_resolver.get_node_path_order(
             AstNodeId(referenced_declaration.ast_node_id),
             referenced_declaration.cu_hash,
         )
         this_cu_id = self._reference_resolver.get_ast_id_from_cu_node_path_order(
             node_path_order, self._cu_hash
         )
-
         self._referenced_declaration_id = this_cu_id
-        referenced_declaration.register_reference(self)
-        self._reference_resolver.register_destroy_callback(
-            self.file, partial(self._destroy, referenced_declaration)
-        )
 
-    def _destroy(self, referenced_declaration: DeclarationAbc) -> None:
-        referenced_declaration.unregister_reference(self)
+        if isinstance(referenced_declaration, DeclarationAbc):
+            referenced_declaration.register_reference(self)
+            self._reference_resolver.register_destroy_callback(
+                self.file, partial(self._destroy, referenced_declaration)
+            )
+
+    def _destroy(
+        self, referenced_declaration: Union[DeclarationAbc, SourceUnit]
+    ) -> None:
+        if isinstance(referenced_declaration, DeclarationAbc):
+            referenced_declaration.unregister_reference(self)
 
     @property
     def underlying_node(self) -> Union[IdentifierPath, UserDefinedTypeName]:
         """
         Returns:
             Underlying IR node (parent) of this identifier path part.
         """
@@ -121,26 +128,33 @@
             `Contract` or `Event` in `Contract.Event`.
         Returns:
             Name of the identifier path part as it appears in the source code.
         """
         return self._name
 
     @property
-    def referenced_declaration(self) -> DeclarationAbc:
+    def referenced_declaration(self) -> Union[DeclarationAbc, SourceUnit]:
         """
         !!! example
             In the case of `Contract.Struct` [IdentifierPath][woke.ast.ir.meta.identifier_path.IdentifierPath], the referenced declaration of `Struct` is the declaration of the struct `Struct` in the contract `Contract`.
+        !!! example
+            Can be a [SourceUnit][woke.ast.ir.meta.source_unit.SourceUnit] in the following case:
+            ```solidity
+            import * as Utils from "./Utils.sol";
+            ```
         Returns:
             Declaration referenced by this identifier path part.
         """
+        from .source_unit import SourceUnit
+
         assert self._referenced_declaration_id is not None
         node = self._reference_resolver.resolve_node(
             self._referenced_declaration_id, self._cu_hash
         )
-        assert isinstance(node, DeclarationAbc)
+        assert isinstance(node, (DeclarationAbc, SourceUnit))
         return node
 
 
 class IdentifierPath(SolidityAbc):
     """
     Identifier path represents a path name of identifiers separated by dots. It was introduced in Solidity 0.8.0 to replace
     [UserDefinedTypeName][woke.ast.ir.type_name.user_defined_type_name.UserDefinedTypeName] in some cases.
```

### Comparing `woke-3.2.0/woke/ast/ir/meta/import_directive.py` & `woke-3.3.0/woke/ast/ir/meta/import_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/inheritance_specifier.py` & `woke-3.3.0/woke/ast/ir/meta/inheritance_specifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/modifier_invocation.py` & `woke-3.3.0/woke/ast/ir/meta/modifier_invocation.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/override_specifier.py` & `woke-3.3.0/woke/ast/ir/meta/override_specifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/parameter_list.py` & `woke-3.3.0/woke/ast/ir/meta/parameter_list.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/pragma_directive.py` & `woke-3.3.0/woke/ast/ir/meta/pragma_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/source_unit.py` & `woke-3.3.0/woke/ast/ir/meta/source_unit.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/structured_documentation.py` & `woke-3.3.0/woke/ast/ir/meta/structured_documentation.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/try_catch_clause.py` & `woke-3.3.0/woke/ast/ir/meta/try_catch_clause.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/meta/using_for_directive.py` & `woke-3.3.0/woke/ast/ir/meta/using_for_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/reference_resolver.py` & `woke-3.3.0/woke/ast/ir/reference_resolver.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,93 +31,93 @@
 @dataclass(order=True)
 class PostProcessQueueItem:
     priority: int
     callback: Callable[[CallbackParams], None] = field(compare=False)
 
 
 class ReferenceResolver:
-    __ordered_nodes: DefaultDict[bytes, Dict[AstNodeId, Tuple[Path, int]]]
-    __ordered_nodes_inverted: DefaultDict[bytes, Dict[Tuple[Path, int], AstNodeId]]
-    __registered_source_files: DefaultDict[bytes, Dict[int, Path]]
-    __registered_nodes: Dict[Tuple[Path, int], SolidityAbc]
-    __post_process_callbacks: List[PostProcessQueueItem]
-    __destroy_callbacks: DefaultDict[Path, List[Callable[[], None]]]
-    __global_symbol_references: DefaultDict[
+    _ordered_nodes: DefaultDict[bytes, Dict[AstNodeId, Tuple[Path, int]]]
+    _ordered_nodes_inverted: DefaultDict[bytes, Dict[Tuple[Path, int], AstNodeId]]
+    _registered_source_files: DefaultDict[bytes, Dict[int, Path]]
+    _registered_nodes: Dict[Tuple[Path, int], SolidityAbc]
+    _post_process_callbacks: List[PostProcessQueueItem]
+    _destroy_callbacks: DefaultDict[Path, List[Callable[[], None]]]
+    _global_symbol_references: DefaultDict[
         GlobalSymbolsEnum, List[Union[Identifier, MemberAccess]]
     ]
 
     def __init__(self):
-        self.__ordered_nodes = defaultdict(dict)
-        self.__ordered_nodes_inverted = defaultdict(dict)
-        self.__registered_source_files = defaultdict(dict)
-        self.__registered_nodes = {}
-        self.__post_process_callbacks = []
-        self.__destroy_callbacks = defaultdict(list)
-        self.__global_symbol_references = defaultdict(list)
+        self._ordered_nodes = defaultdict(dict)
+        self._ordered_nodes_inverted = defaultdict(dict)
+        self._registered_source_files = defaultdict(dict)
+        self._registered_nodes = {}
+        self._post_process_callbacks = []
+        self._destroy_callbacks = defaultdict(list)
+        self._global_symbol_references = defaultdict(list)
 
     def index_nodes(self, root_node: AstSolc, path: Path, cu_hash: bytes) -> None:
-        self.__ordered_nodes[cu_hash][root_node.id] = (path, 0)
-        self.__ordered_nodes_inverted[cu_hash][(path, 0)] = root_node.id
+        self._ordered_nodes[cu_hash][root_node.id] = (path, 0)
+        self._ordered_nodes_inverted[cu_hash][(path, 0)] = root_node.id
         for index, node in enumerate(root_node):
-            self.__ordered_nodes[cu_hash][node.id] = (path, index + 1)
-            self.__ordered_nodes_inverted[cu_hash][(path, index + 1)] = node.id
+            self._ordered_nodes[cu_hash][node.id] = (path, index + 1)
+            self._ordered_nodes_inverted[cu_hash][(path, index + 1)] = node.id
 
     def register_source_file_id(self, source_file_id: int, path: Path, cu_hash: bytes):
-        self.__registered_source_files[cu_hash][source_file_id] = path
+        self._registered_source_files[cu_hash][source_file_id] = path
 
     def get_node_path_order(
         self, node_id: AstNodeId, cu_hash: bytes
     ) -> Tuple[Path, int]:
-        return self.__ordered_nodes[cu_hash][node_id]
+        return self._ordered_nodes[cu_hash][node_id]
 
     def get_ast_id_from_cu_node_path_order(
         self, node_path_order: Tuple[Path, int], cu_hash: bytes
     ) -> AstNodeId:
-        return self.__ordered_nodes_inverted[cu_hash][node_path_order]
+        return self._ordered_nodes_inverted[cu_hash][node_path_order]
 
     def register_node(self, node: SolidityAbc, node_id: AstNodeId, cu_hash: bytes):
-        assert cu_hash in self.__ordered_nodes
-        assert node_id in self.__ordered_nodes[cu_hash]
-        node_path_order = self.__ordered_nodes[cu_hash][node_id]
-        self.__registered_nodes[node_path_order] = node
+        assert cu_hash in self._ordered_nodes
+        assert node_id in self._ordered_nodes[cu_hash]
+        node_path_order = self._ordered_nodes[cu_hash][node_id]
+        self._registered_nodes[node_path_order] = node
 
     def resolve_node(self, node_id: AstNodeId, cu_hash: bytes) -> SolidityAbc:
-        node_path_order = self.__ordered_nodes[cu_hash][node_id]
-        return self.__registered_nodes[node_path_order]
+        node_path_order = self._ordered_nodes[cu_hash][node_id]
+        return self._registered_nodes[node_path_order]
 
     def resolve_source_file_id(self, source_file_id: int, cu_hash: bytes) -> Path:
-        return self.__registered_source_files[cu_hash][source_file_id]
+        return self._registered_source_files[cu_hash][source_file_id]
 
     def register_post_process_callback(
         self, callback: Callable[[CallbackParams], None], priority: int = 0
     ):
         heapq.heappush(
-            self.__post_process_callbacks, PostProcessQueueItem(priority, callback)
+            self._post_process_callbacks, PostProcessQueueItem(priority, callback)
         )
 
     def register_destroy_callback(self, file: Path, callback: Callable[[], None]):
-        self.__destroy_callbacks[file].append(callback)
+        self._destroy_callbacks[file].append(callback)
 
     def run_post_process_callbacks(self, callback_params: CallbackParams):
-        while len(self.__post_process_callbacks):
-            callback = heapq.heappop(self.__post_process_callbacks).callback
+        while len(self._post_process_callbacks):
+            callback = heapq.heappop(self._post_process_callbacks).callback
             callback(callback_params)
 
     def run_destroy_callbacks(self, file: Path):
-        for callback in self.__destroy_callbacks[file]:
+        for callback in self._destroy_callbacks[file]:
             callback()
-        del self.__destroy_callbacks[file]
+        del self._destroy_callbacks[file]
 
     def register_global_symbol_reference(
         self, node_id: GlobalSymbolsEnum, node: Union[Identifier, MemberAccess]
     ):
-        self.__global_symbol_references[node_id].append(node)
+        self._global_symbol_references[node_id].append(node)
 
     def unregister_global_symbol_reference(
         self, node_id: GlobalSymbolsEnum, node: Union[Identifier, MemberAccess]
     ):
-        self.__global_symbol_references[node_id].remove(node)
+        self._global_symbol_references[node_id].remove(node)
 
     def get_global_symbol_references(
         self, node_id: GlobalSymbolsEnum
     ) -> Tuple[Union[Identifier, MemberAccess], ...]:
-        return tuple(self.__global_symbol_references[node_id])
+        return tuple(self._global_symbol_references[node_id])
```

### Comparing `woke-3.2.0/woke/ast/ir/statement/abc.py` & `woke-3.3.0/woke/ast/ir/statement/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/block.py` & `woke-3.3.0/woke/ast/ir/statement/block.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/break_statement.py` & `woke-3.3.0/woke/ast/ir/statement/break_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/continue_statement.py` & `woke-3.3.0/woke/ast/ir/statement/continue_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/do_while_statement.py` & `woke-3.3.0/woke/ast/ir/statement/do_while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/emit_statement.py` & `woke-3.3.0/woke/ast/ir/statement/emit_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/expression_statement.py` & `woke-3.3.0/woke/ast/ir/statement/expression_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/for_statement.py` & `woke-3.3.0/woke/ast/ir/statement/for_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/if_statement.py` & `woke-3.3.0/woke/ast/ir/statement/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/inline_assembly.py` & `woke-3.3.0/woke/ast/ir/statement/inline_assembly.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/placeholder_statement.py` & `woke-3.3.0/woke/ast/ir/statement/placeholder_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/return_statement.py` & `woke-3.3.0/woke/ast/ir/statement/return_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/revert_statement.py` & `woke-3.3.0/woke/ast/ir/statement/revert_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/try_statement.py` & `woke-3.3.0/woke/ast/ir/statement/try_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/unchecked_block.py` & `woke-3.3.0/woke/ast/ir/statement/unchecked_block.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/variable_declaration_statement.py` & `woke-3.3.0/woke/ast/ir/statement/variable_declaration_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/statement/while_statement.py` & `woke-3.3.0/woke/ast/ir/statement/while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/type_name/abc.py` & `woke-3.3.0/woke/ast/ir/type_name/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/type_name/array_type_name.py` & `woke-3.3.0/woke/ast/ir/type_name/array_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/type_name/elementary_type_name.py` & `woke-3.3.0/woke/ast/ir/type_name/elementary_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/type_name/function_type_name.py` & `woke-3.3.0/woke/ast/ir/type_name/function_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/type_name/mapping.py` & `woke-3.3.0/woke/ast/ir/type_name/mapping.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/type_name/user_defined_type_name.py` & `woke-3.3.0/woke/ast/ir/type_name/user_defined_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/utils/init_tuple.py` & `woke-3.3.0/woke/ast/ir/utils/init_tuple.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/__init__.py` & `woke-3.3.0/woke/ast/ir/yul/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/abc.py` & `woke-3.3.0/woke/ast/ir/yul/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/assignment.py` & `woke-3.3.0/woke/ast/ir/yul/assignment.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/block.py` & `woke-3.3.0/woke/ast/ir/yul/block.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/case_statement.py` & `woke-3.3.0/woke/ast/ir/yul/case_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/expression_statement.py` & `woke-3.3.0/woke/ast/ir/yul/expression_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/for_loop.py` & `woke-3.3.0/woke/ast/ir/yul/for_loop.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/function_call.py` & `woke-3.3.0/woke/ast/ir/yul/function_call.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/function_definition.py` & `woke-3.3.0/woke/ast/ir/yul/function_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/identifier.py` & `woke-3.3.0/woke/ast/ir/yul/identifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/if_statement.py` & `woke-3.3.0/woke/ast/ir/yul/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/literal.py` & `woke-3.3.0/woke/ast/ir/yul/literal.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/switch.py` & `woke-3.3.0/woke/ast/ir/yul/switch.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/typed_name.py` & `woke-3.3.0/woke/ast/ir/yul/typed_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/ir/yul/variable_declaration.py` & `woke-3.3.0/woke/ast/ir/yul/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/nodes.py` & `woke-3.3.0/woke/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/ast/types.py` & `woke-3.3.0/woke/ast/types.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/__main__.py` & `woke-3.3.0/woke/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/accounts.py` & `woke-3.3.0/woke/cli/accounts.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/compile.py` & `woke-3.3.0/woke/cli/compile.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/detect.py` & `woke-3.3.0/woke/cli/detect.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/fuzz.py` & `woke-3.3.0/woke/cli/fuzz.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/init.py` & `woke-3.3.0/woke/cli/init.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/lsp.py` & `woke-3.3.0/woke/cli/lsp.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/run.py` & `woke-3.3.0/woke/cli/run.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/svm.py` & `woke-3.3.0/woke/cli/svm.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/cli/test.py` & `woke-3.3.0/woke/cli/test.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/compiler/build_data_model.py` & `woke-3.3.0/woke/compiler/build_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/compiler/compilation_unit.py` & `woke-3.3.0/woke/compiler/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/compiler/compiler.py` & `woke-3.3.0/woke/compiler/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             dest_file = Path(event.dest_path)
             if (
                 src_file == self._config_path
                 or src_file.suffix == ".sol"
                 or dest_file == self._config_path
                 or dest_file.suffix == ".sol"
             ):
-                self._loop.call_soon_threadsafe(self._queue.put, event)
+                self._loop.call_soon_threadsafe(self._queue.put_nowait, event)
         else:
             file = Path(event.src_path)
             if file == self._config_path or file.suffix == ".sol":
                 self._loop.call_soon_threadsafe(self._queue.put_nowait, event)
 
     async def _compile(self):
         assert self._compiler.latest_build_info is not None
@@ -214,25 +214,25 @@
 
             deleted_files = self._deleted_files
         else:
             files = {
                 unit_info.fs_path
                 for unit_info in self._compiler.latest_build_info.source_units_info.values()
             }
+            files.update(self._created_files)
+            files.update(self._modified_files)
             ignored_files = {
                 f
                 for f in files
                 if any(
                     is_relative_to(f, p)
                     for p in self._config.compiler.solc.ignore_paths
                 )
                 or not is_relative_to(f, self._config.project_root_path)
             }
-            files.update(self._created_files)
-            files.update(self._modified_files)
             files.difference_update(ignored_files)
             files.difference_update(self._deleted_files)
             deleted_files = self._deleted_files
 
         await self._compiler.compile(
             files,
             self._output_types,
@@ -378,14 +378,16 @@
                 import_unit_name = self.__source_unit_name_resolver.resolve_import(
                     source_unit_name, _import
                 )
                 try:
                     import_path = self.__source_path_resolver.resolve(
                         import_unit_name, source_unit_name, modified_files.keys()
                     ).resolve()
+                    if import_path not in modified_files:
+                        import_path = import_path.resolve(strict=True)
                 except (FileNotFoundError, CompilationResolveError):
                     if ignore_errors:
                         graph.nodes[source_unit_name]["unresolved_imports"].add(
                             import_unit_name
                         )
                         continue
                     raise
@@ -876,28 +878,39 @@
         )
         start = time.perf_counter()
         processed_files: Set[Path] = set()
 
         with ctx_manager:
             successful_compilation_units = []
             for cu, solc_output in zip(compilation_units, ret):
-                errored: bool = False
+                errored_files: Set[Path] = set()
                 errors_per_cu[cu.hash] = set()
 
                 for error in solc_output.errors:
                     errors_per_cu[cu.hash].add(error)
                     if error.severity == SolcOutputErrorSeverityEnum.ERROR:
-                        errored = True
+                        if error.source_location is not None:
+                            path = cu.source_unit_name_to_path(
+                                error.source_location.file
+                            )
+                            errored_files.add(path)
+                        else:
+                            # whole compilation unit errored
+                            errored_files |= cu.files
+
+                self._out_edge_bfs(cu, errored_files, errored_files)
+
+                for file in errored_files:
+                    if file in build.source_units:
+                        build.reference_resolver.run_destroy_callbacks(file)
+                        build.source_units.pop(file)
+                    if file in build.interval_trees:
+                        build.interval_trees.pop(file)
 
-                if errored:
-                    for file in cu.files:
-                        if file in build.source_units and file in files_to_compile:
-                            build.reference_resolver.run_destroy_callbacks(file)
-                            build.source_units.pop(file)
-                else:
+                if len(errored_files) == 0:
                     successful_compilation_units.append((cu, solc_output))
 
             for cu, solc_output in successful_compilation_units:
                 # files requested to be compiled and files that import these files (even indirectly)
                 recompiled_files: Set[Path] = set()
                 self._out_edge_bfs(cu, files_to_compile & cu.files, recompiled_files)
```

### Comparing `woke-3.2.0/woke/compiler/solc_frontend/input_data_model.py` & `woke-3.3.0/woke/compiler/solc_frontend/input_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/compiler/solc_frontend/output_data_model.py` & `woke-3.3.0/woke/compiler/solc_frontend/output_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/compiler/solc_frontend/solc_runner.py` & `woke-3.3.0/woke/compiler/solc_frontend/solc_runner.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/compiler/source_path_resolver.py` & `woke-3.3.0/woke/compiler/source_path_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/compiler/source_unit_name_resolver.py` & `woke-3.3.0/woke/compiler/source_unit_name_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/config/__init__.py` & `woke-3.3.0/woke/config/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/config/data_model.py` & `woke-3.3.0/woke/config/data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/config/woke_config.py` & `woke-3.3.0/woke/config/woke_config.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/contracts/woke/console.sol` & `woke-3.3.0/woke/contracts/woke/console.sol`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/core/solidity_version.py` & `woke-3.3.0/woke/core/solidity_version.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/deployment/__init__.py` & `woke-3.3.0/woke/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/deployment/core.py` & `woke-3.3.0/woke/deployment/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import time
 from contextlib import contextmanager, nullcontext
 from typing import Any, Dict, Iterable, Optional, Union, cast
+from urllib.error import HTTPError
 
 import eth_utils
 from rich.console import Group
 from rich.pretty import pprint
 from rich.progress import BarColumn, Progress, TextColumn, TimeElapsedColumn
 from rich.prompt import Confirm
 from rich.table import Table
 
 import woke.development.core
 from woke.cli.console import console
 from woke.development.chain_interfaces import AnvilChainInterface, TxParams
 from woke.development.core import (
     Abi,
-    Account,
     Address,
     RequestType,
     RevertToSnapshotFailedError,
     TransactionConfirmationFailedError,
     Wei,
     check_connected,
     fix_library_abi,
@@ -62,29 +62,26 @@
         self, min_gas_price: Optional[int], block_base_fee_per_gas: Optional[int]
     ) -> None:
         self._require_signed_txs = True
 
         if min_gas_price is not None:
             try:
                 self._chain_interface.set_min_gas_price(min_gas_price)
-            except JsonRpcError:
+            except (JsonRpcError, HTTPError):
                 pass
 
     def _connect_finalize(self) -> None:
         chain_interfaces_manager.close(self._chain_interface)
 
-    def _update_nonce(self, address: Address, nonce: int) -> None:
-        # nothing to do
-        pass
-
     @check_connected
     def snapshot(self) -> str:
         snapshot_id = self._chain_interface.snapshot()
 
         self._snapshots[snapshot_id] = {
+            "nonces": self._nonces.copy(),
             "accounts": self._accounts.copy(),
             "default_call_account": self._default_call_account,
             "default_tx_account": self._default_tx_account,
             "txs": dict(self._txs._transactions),
             "blocks": dict(self._blocks._blocks),
         }
         return snapshot_id
@@ -92,14 +89,15 @@
     @check_connected
     def revert(self, snapshot_id: str) -> None:
         reverted = self._chain_interface.revert(snapshot_id)
         if not reverted:
             raise RevertToSnapshotFailedError()
 
         snapshot = self._snapshots[snapshot_id]
+        self._nonces = snapshot["nonces"]
         self._accounts = snapshot["accounts"]
         self._default_call_account = snapshot["default_call_account"]
         self._default_tx_account = snapshot["default_tx_account"]
         self._txs._transactions = snapshot["txs"]
         self._blocks._blocks = snapshot["blocks"]
         del self._snapshots[snapshot_id]
 
@@ -197,16 +195,17 @@
             arguments = [self._convert_to_web3_type(arg) for arg in arguments]
             types = [
                 eth_utils.abi.collapse_if_tuple(cast(Dict[str, Any], arg))
                 for arg in fix_library_abi(abi["inputs"])
             ]
             params["data"] += Abi.encode(types, arguments)
 
+        n = self._nonces[Address(sender)]
         tx: TxParams = {
-            "nonce": Account(sender, self).nonce,
+            "nonce": n,
             "from": sender,
             "value": params["value"] if "value" in params else 0,
             "data": params["data"],
         }
         if tx_type != 0:
             tx["type"] = tx_type
 
@@ -237,21 +236,25 @@
                     or self.require_signed_txs
                 ):
                     tx["maxFeePerGas"] = tx["maxPriorityFeePerGas"] + int(
                         int(
                             self.chain_interface.get_block("pending")["baseFeePerGas"],
                             16,
                         )
-                        * 1.125
+                        * 2
                     )
 
         if "gas" not in params or params["gas"] == "auto":
             # use "auto when unset
             try:
-                tx["gas"] = int(self._chain_interface.estimate_gas(tx) * 1.1)
+                tx_copy = tx.copy()
+                tx_copy.pop("gasPrice", None)
+                tx_copy.pop("maxPriorityFeePerGas", None)
+                tx_copy.pop("maxFeePerGas", None)
+                tx["gas"] = int(self._chain_interface.estimate_gas(tx_copy) * 1.1)
             except JsonRpcError as e:
                 self._process_call_revert(e)
                 raise
         elif isinstance(params["gas"], int):
             tx["gas"] = params["gas"]
         else:
             raise ValueError(f"Invalid gas value: {params['gas']}")
@@ -259,28 +262,35 @@
         if (
             tx_type in {1, 2}
             and ("accessList" not in params or params["accessList"] == "auto")
             and request_type != "access_list"
         ):
             try:
                 response = self._chain_interface.create_access_list(tx)
-                gas_used = int(response["gasUsed"], 16)
+                gas_used = int(int(response["gasUsed"], 16) * 1.1)
 
                 if params.get("accessList", None) == "auto" or (
                     "accessList" not in params and gas_used <= tx["gas"]
                 ):
                     tx["accessList"] = response["accessList"]
 
                     if "gas" not in params or params["gas"] == "auto":
                         tx["gas"] = gas_used
-            except JsonRpcError as e:
+            except (JsonRpcError, HTTPError) as e:
                 try:
-                    # will re-raise if not a revert error
-                    self._process_call_revert(e)
-                    raise
+                    if isinstance(e, JsonRpcError):
+                        # will re-raise if not a revert error
+                        self._process_call_revert(e)
+                        raise
+                    else:
+                        # HTTPError -> eth_createAccessList not supported
+                        if "accessList" not in params:
+                            tx["accessList"] = []
+                        else:
+                            raise
                 except JsonRpcError:
                     # eth_createAccessList probably not supported
                     if "accessList" not in params:
                         tx["accessList"] = []
                     else:
                         raise
 
@@ -343,19 +353,19 @@
                 time.sleep(0.5)
                 if status is not None:
                     status.update(get_pending_text())
 
         if not config.deployment.silent:
             if tx.chain.chain_id in chain_explorer_urls:
                 console.print(
-                    f"Transaction [link={chain_explorer_urls[tx.chain.chain_id].url}/tx/{tx.tx_hash}]{tx.tx_hash}[/link] mined in block {tx.block.number}"
+                    f"Transaction [link={chain_explorer_urls[tx.chain.chain_id].url}/tx/{tx.tx_hash}]{tx.tx_hash}[/link] mined in block {tx.block_number}"
                 )
             else:
                 console.print(
-                    f"Transaction {tx.tx_hash} mined in block {tx.block.number}"
+                    f"Transaction {tx.tx_hash} mined in block {tx.block_number}"
                 )
 
         latest_block_number = self.chain_interface.get_block_number()
 
         ctx_manager = (
             Progress(
                 TextColumn("[progress.description]{task.description}"),
@@ -369,24 +379,24 @@
         )
 
         with ctx_manager as progress:
             if progress is not None:
                 task_id = progress.add_task(
                     "Confirmations",
                     total=confirmations,
-                    completed=(latest_block_number - tx.block.number + 1),
+                    completed=(latest_block_number - tx.block_number + 1),
                 )
-            while latest_block_number - tx.block.number < confirmations - 1:
+            while latest_block_number - tx.block_number < confirmations - 1:
                 time.sleep(1)
                 latest_block_number = self.chain_interface.get_block_number()
                 if progress is not None:
                     progress.update(
                         task_id,
                         completed=(
-                            latest_block_number - tx.block.number + 1
+                            latest_block_number - tx.block_number + 1
                         ),  # pyright: reportUnboundVariable=false
                     )
 
     def _confirm_transaction(self, tx: TxParams) -> None:
         config = get_config()
         if config.deployment.silent:
             return
```

### Comparing `woke-3.2.0/woke/development/blocks.py` & `woke-3.3.0/woke/development/blocks.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/call_trace.py` & `woke-3.3.0/woke/development/call_trace.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/chain_interfaces.py` & `woke-3.3.0/woke/development/chain_interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,23 +219,30 @@
     def connect(cls, config: WokeConfig, uri: str) -> ChainInterfaceAbc:
         communicator = JsonRpcCommunicator(config, uri)
         communicator.__enter__()
         try:
             client_version: str = communicator.send_request(
                 "web3_clientVersion"
             ).lower()
+            chain_id = int(communicator.send_request("eth_chainId"), 16)
             if "anvil" in client_version:
                 return AnvilChainInterface(config, communicator)
             elif "hardhat" in client_version:
                 return HardhatChainInterface(config, communicator)
             elif "ethereumjs" in client_version:
                 return GanacheChainInterface(config, communicator)
-            elif client_version.startswith(("geth", "bor", "nitro")):
+            elif client_version.startswith(("geth", "bor")):
                 return GethChainInterface(config, communicator)
-            elif "hermez" in client_version:
+            elif "nitro" in client_version:
+                return NitroChainInterface(config, communicator)
+            elif chain_id in {43113, 43114}:
+                # Avax client reports just a version number without the name of the client
+                # => hard to distinguish from other clients
+                return AvalancheChainInterface(config, communicator)
+            elif chain_id in {1101, 1442}:
                 return HermezChainInterface(config, communicator)
             else:
                 raise NotImplementedError(
                     f"Client version {client_version} not supported"
                 )
         except Exception:
             communicator.__exit__(None, None, None)
@@ -246,14 +253,17 @@
         if self._process is not None:
             self._process.terminate()
             try:
                 self._process.communicate(timeout=self._config.testing.timeout)
             except subprocess.TimeoutExpired:
                 self._process.kill()
 
+    def get_client_version(self) -> str:
+        return self._communicator.send_request("web3_clientVersion")
+
     def get_balance(
         self, address: str, block_identifier: Union[int, str] = "latest"
     ) -> int:
         return int(
             self._communicator.send_request(
                 "eth_getBalance",
                 [address, self._encode_block_identifier(block_identifier)],
@@ -629,95 +639,88 @@
             "Ganache does not support setting next block base fee per gas"
         )
 
     def set_min_gas_price(self, value: int) -> None:
         self._communicator.send_request("miner_setGasPrice", [hex(value)])
 
 
-class GethChainInterface(ChainInterfaceAbc):
-    def get_accounts(self) -> List[str]:
-        return self._communicator.send_request("eth_accounts")
-
-    def get_automine(self) -> bool:
-        raise NotImplementedError("Geth does not support automine")
-
-    def set_automine(self, value: bool) -> None:
-        raise NotImplementedError("Geth does not support automine")
-
-    def reset(self, options: Optional[Dict] = None) -> None:
-        raise NotImplementedError("Geth does not support resetting the chain")
-
-    def set_coinbase(self, address: str) -> None:
-        raise NotImplementedError("Geth does not support setting coinbase")
-
-    def set_balance(self, address: str, value: int) -> None:
-        raise NotImplementedError("Geth does not support setting balance")
-
-    def set_block_gas_limit(self, gas_limit: int) -> None:
-        raise NotImplementedError("Geth does not support setting block gas limit")
-
-    def set_code(self, address: str, value: bytes) -> None:
-        raise NotImplementedError("Geth does not support setting code")
-
-    def set_nonce(self, address: str, value: int) -> None:
-        raise NotImplementedError("Geth does not support setting nonce")
-
-    def set_next_block_timestamp(self, timestamp: int) -> None:
-        raise NotImplementedError("Geth does not support setting next block timestamp")
-
-    def send_unsigned_transaction(self, params: TxParams) -> str:
-        raise NotImplementedError("Geth does not support sending unsigned transactions")
-
-    def set_next_block_base_fee_per_gas(self, value: int) -> None:
-        raise NotImplementedError(
-            "Geth does not support setting next block base fee per gas"
-        )
-
-    def set_min_gas_price(self, value: int) -> None:
-        raise NotImplementedError("Geth does not support setting min gas price")
-
+class GethLikeChainInterfaceAbc(ChainInterfaceAbc, ABC):
+    @property
+    @abstractmethod
+    def _name(self) -> str:
+        ...
 
-class HermezChainInterface(ChainInterfaceAbc):
     def get_accounts(self) -> List[str]:
         return []
 
     def get_automine(self) -> bool:
-        raise NotImplementedError("Hermez does not support automine")
+        raise NotImplementedError(f"{self._name} does not support automine")
 
     def set_automine(self, value: bool) -> None:
-        raise NotImplementedError("Hermez does not support automine")
+        raise NotImplementedError(f"{self._name} does not support automine")
 
     def reset(self, options: Optional[Dict] = None) -> None:
-        raise NotImplementedError("Hermez does not support resetting the chain")
+        raise NotImplementedError(f"{self._name} does not support resetting the chain")
 
     def set_coinbase(self, address: str) -> None:
-        raise NotImplementedError("Hermez does not support setting coinbase")
+        raise NotImplementedError(f"{self._name} does not support setting coinbase")
 
     def set_balance(self, address: str, value: int) -> None:
-        raise NotImplementedError("Hermez does not support setting balance")
+        raise NotImplementedError(f"{self._name} does not support setting balance")
 
     def set_block_gas_limit(self, gas_limit: int) -> None:
-        raise NotImplementedError("Hermez does not support setting block gas limit")
+        raise NotImplementedError(
+            f"{self._name} does not support setting block gas limit"
+        )
 
     def set_code(self, address: str, value: bytes) -> None:
-        raise NotImplementedError("Hermez does not support setting code")
+        raise NotImplementedError(f"{self._name} does not support setting code")
 
     def set_nonce(self, address: str, value: int) -> None:
-        raise NotImplementedError("Hermez does not support setting nonce")
+        raise NotImplementedError(f"{self._name} does not support setting nonce")
 
     def set_next_block_timestamp(self, timestamp: int) -> None:
         raise NotImplementedError(
-            "Hermez does not support setting next block timestamp"
+            f"{self._name} does not support setting next block timestamp"
         )
 
     def send_unsigned_transaction(self, params: TxParams) -> str:
         raise NotImplementedError(
-            "Hermez does not support sending unsigned transactions"
+            f"{self._name} does not support sending unsigned transactions"
         )
 
     def set_next_block_base_fee_per_gas(self, value: int) -> None:
         raise NotImplementedError(
-            "Hermez does not support setting next block base fee per gas"
+            f"{self._name} does not support setting next block base fee per gas"
         )
 
     def set_min_gas_price(self, value: int) -> None:
-        raise NotImplementedError("Hermez does not support setting min gas price")
+        raise NotImplementedError(
+            f"{self._name} does not support setting min gas price"
+        )
+
+
+class GethChainInterface(GethLikeChainInterfaceAbc):
+    @property
+    def _name(self) -> str:
+        return "Geth"
+
+    def get_accounts(self) -> List[str]:
+        return self._communicator.send_request("eth_accounts")
+
+
+class HermezChainInterface(GethLikeChainInterfaceAbc):
+    @property
+    def _name(self) -> str:
+        return "Hermez"
+
+
+class NitroChainInterface(GethLikeChainInterfaceAbc):
+    @property
+    def _name(self) -> str:
+        return "Nitro"
+
+
+class AvalancheChainInterface(GethLikeChainInterfaceAbc):
+    @property
+    def _name(self) -> str:
+        return "Avalanche"
```

### Comparing `woke-3.2.0/woke/development/constants.py` & `woke-3.3.0/woke/development/constants.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/core.py` & `woke-3.3.0/woke/development/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Set,
     Tuple,
     Type,
     Union,
     cast,
     overload,
 )
+from urllib.error import HTTPError
 
 import eth_abi
 import eth_abi.packed
 import eth_account
 import eth_account.messages
 import eth_utils
 from Crypto.Hash import BLAKE2b, keccak
@@ -46,23 +47,23 @@
     get_args,
     get_origin,
     get_type_hints,
 )
 
 from woke.utils import StrEnum
 
+from ..utils.keyed_default_dict import KeyedDefaultDict
 from . import hardhat_console
 from .blocks import ChainBlocks
 from .chain_interfaces import (
     AnvilChainInterface,
     ChainInterfaceAbc,
     GanacheChainInterface,
-    GethChainInterface,
+    GethLikeChainInterfaceAbc,
     HardhatChainInterface,
-    HermezChainInterface,
     TxParams,
 )
 from .globals import (
     chain_interfaces_manager,
     get_config,
     get_coverage_handler,
     get_exception_handler,
@@ -1030,14 +1031,15 @@
 
 
 class Chain(ABC):
     _connected: bool
     _chain_interface: ChainInterfaceAbc
     _accounts: List[Account]
     _accounts_set: Set[Account]  # for faster lookup
+    _nonces: KeyedDefaultDict[Address, int]  # pyright: reportGeneralTypeIssues=false
     _default_call_account: Optional[Account]
     _default_tx_account: Optional[Account]
     _default_estimate_account: Optional[Account]
     _default_access_list_account: Optional[Account]
     _default_tx_type: int
     _default_tx_confirmations: int
     _deployed_libraries: DefaultDict[bytes, List[Library]]
@@ -1047,32 +1049,29 @@
     _txs: ChainTransactions
     _chain_id: int
     _labels: Dict[Address, str]
     _private_keys: Dict[Address, bytes]
     _require_signed_txs: bool
     _fork: Optional[str]
     _debug_trace_call_supported: bool
+    _client_version: str
 
     tx_callback: Optional[Callable[[TransactionAbc], None]]
 
     @abstractmethod
     def _connect_setup(
         self, min_gas_price: Optional[int], block_base_fee_per_gas: Optional[int]
     ) -> None:
         ...
 
     @abstractmethod
     def _connect_finalize(self) -> None:
         ...
 
     @abstractmethod
-    def _update_nonce(self, address: Address, nonce: int) -> None:
-        ...
-
-    @abstractmethod
     def snapshot(self) -> str:
         ...
 
     @abstractmethod
     def revert(self, snapshot_id: str) -> None:
         ...
 
@@ -1165,23 +1164,24 @@
 
         self._chain_interface = chain_interfaces_manager.get_or_create(
             uri, accounts=accounts, chain_id=chain_id, fork=fork, hardfork=hardfork
         )
 
         try:
             self._connected = True
+            self._client_version = self._chain_interface.get_client_version()
 
             try:
                 self._chain_interface.debug_trace_call(
                     {
                         "type": 0,
                     }
                 )
                 self._debug_trace_call_supported = True
-            except JsonRpcError:
+            except (JsonRpcError, HTTPError):
                 self._debug_trace_call_supported = False
 
             self._chain_id = self._chain_interface.get_chain_id()
 
             # determine the chain hardfork to set the default tx type
             if isinstance(self._chain_interface, AnvilChainInterface):
                 hardfork = self._chain_interface.node_info()["hardFork"]
@@ -1199,15 +1199,15 @@
                     self._default_tx_type = 0
                 elif hardfork == "BERLIN":
                     self._default_tx_type = 1
                 else:
                     self._default_tx_type = 2
             elif isinstance(
                 self._chain_interface,
-                (GethChainInterface, HardhatChainInterface, HermezChainInterface),
+                (GethLikeChainInterfaceAbc, HardhatChainInterface),
             ):
                 if self._chain_id in {56, 97}:
                     # BSC clients do not fail on the calls below
                     self._default_tx_type = 1
                 else:
                     # TODO this is not the correct flow for Hermez:
                     # EIP-1559 txs should be supported
@@ -1254,14 +1254,19 @@
 
             self._txs = ChainTransactions(self)
 
             self._accounts = [
                 Account(acc, self) for acc in self._chain_interface.get_accounts()
             ]
             self._accounts_set = set(self._accounts)
+            self._nonces = KeyedDefaultDict(
+                lambda addr: self._chain_interface.get_transaction_count(
+                    str(addr)
+                )  # pyright: reportGeneralTypeIssues=false
+            )
             self._snapshots = {}
             self._deployed_libraries = defaultdict(list)
             self._default_call_account = (
                 self._accounts[0] if len(self._accounts) > 0 else None
             )
             self._default_tx_account = None
             self._default_estimate_account = None
@@ -1294,14 +1299,18 @@
             self._connected = False
 
     @property
     def connected(self) -> bool:
         return self._connected
 
     @property
+    def client_version(self) -> str:
+        return self._client_version
+
+    @property
     @check_connected
     def chain_interface(self) -> ChainInterfaceAbc:
         return self._chain_interface
 
     @property
     @check_connected
     def chain_id(self) -> int:
@@ -1519,14 +1528,17 @@
                 exception_handler = get_exception_handler()
                 if exception_handler is not None:
                     exception_handler(e)
                 raise
         finally:
             self.revert(snapshot_id)
 
+    def _update_nonce(self, address: Address, nonce: int) -> None:
+        self._nonces[address] = nonce
+
     def _convert_to_web3_type(self, value: Any) -> Any:
         if dataclasses.is_dataclass(value):
             return tuple(
                 self._convert_to_web3_type(getattr(value, f.name))
                 for f in dataclasses.fields(value)
             )
         elif isinstance(value, list):
@@ -1853,31 +1865,37 @@
                         read_from_memory(args_offset, args_size, trace["memory"])
                     )
                     console_logs.append(self._parse_console_log_data(data))
 
         return console_logs
 
     def _process_call_revert(self, e: JsonRpcError):
-        if (
-            isinstance(self._chain_interface, (AnvilChainInterface, GethChainInterface))
-            and e.data["code"] == 3
-        ):
-            revert_data = e.data["data"]
-        elif (
-            isinstance(self._chain_interface, GanacheChainInterface)
-            and e.data["code"] == -32000
-        ):
-            revert_data = e.data["data"]
-        elif (
-            isinstance(self._chain_interface, HardhatChainInterface)
-            and e.data["code"] == -32603
-        ):
-            revert_data = e.data["data"]["data"]
-        else:
+        try:
             # Hermez does not provide revert data for estimate
+            if (
+                isinstance(
+                    self._chain_interface,
+                    (AnvilChainInterface, GethLikeChainInterfaceAbc),
+                )
+                and e.data["code"] == 3
+            ):
+                revert_data = e.data["data"]
+            elif (
+                isinstance(self._chain_interface, GanacheChainInterface)
+                and e.data["code"] == -32000
+            ):
+                revert_data = e.data["data"]
+            elif (
+                isinstance(self._chain_interface, HardhatChainInterface)
+                and e.data["code"] == -32603
+            ):
+                revert_data = e.data["data"]["data"]
+            else:
+                raise e from None
+        except Exception:
             raise e from None
 
         if revert_data.startswith("0x"):
             revert_data = revert_data[2:]
 
         self._process_revert_data(None, bytes.fromhex(revert_data))
 
@@ -1902,26 +1920,26 @@
             if Account(tx_params["from"], self) in self._accounts_set:
                 try:
                     tx_hash = self._chain_interface.send_transaction(tx_params)
                 except (ValueError, JsonRpcError) as e:
                     try:
                         tx_hash = e.args[0]["data"]["txHash"]
                     except Exception:
-                        raise e
+                        raise e from None
             elif key is not None:
                 signed_tx = bytes(
                     eth_account.Account.sign_transaction(tx_params, key).rawTransaction
                 )
                 try:
                     tx_hash = self._chain_interface.send_raw_transaction(signed_tx)
                 except (ValueError, JsonRpcError) as e:
                     try:
                         tx_hash = e.args[0]["data"]["txHash"]
                     except Exception:
-                        raise e
+                        raise e from None
             else:
                 raise ValueError(
                     f"Private key for account {tx_params['from']} not known and is not owned by the connected client either."
                 )
             self._update_nonce(Address(tx_params["from"]), tx_params["nonce"] + 1)
         else:
             if isinstance(self.chain_interface, AnvilChainInterface):
```

### Comparing `woke-3.2.0/woke/development/globals.py` & `woke-3.3.0/woke/development/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 from collections import defaultdict
 from pathlib import Path
 from types import TracebackType
 from typing import TYPE_CHECKING, Callable, DefaultDict, List, Optional, Set, Tuple
+from urllib.error import HTTPError
 
 from ipdb.__main__ import _init_pdb
 
 from woke.config import WokeConfig
 from woke.development.chain_interfaces import ChainInterfaceAbc
 from woke.development.json_rpc import JsonRpcError
 from woke.utils.file_utils import is_relative_to
@@ -158,15 +159,15 @@
                 fork,
                 hardfork,
             )
             chain_interface = self._free_chain_interfaces[params].pop()
 
         try:
             snapshot = chain_interface.snapshot()
-        except JsonRpcError:
+        except (JsonRpcError, HTTPError):
             snapshot = None
 
         self._chain_interfaces[params].append((chain_interface, snapshot))
         return chain_interface
 
     def free(self, chain_interface: ChainInterfaceAbc) -> None:
         snapshot_reverted = False
```

### Comparing `woke-3.2.0/woke/development/hardhat_console.py` & `woke-3.3.0/woke/development/hardhat_console.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/internal.py` & `woke-3.3.0/woke/development/internal.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/json_rpc/communicator.py` & `woke-3.3.0/woke/development/json_rpc/communicator.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/json_rpc/http.py` & `woke-3.3.0/woke/development/json_rpc/http.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/json_rpc/ipc.py` & `woke-3.3.0/woke/development/json_rpc/ipc.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/json_rpc/websocket.py` & `woke-3.3.0/woke/development/json_rpc/websocket.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/primitive_types.py` & `woke-3.3.0/woke/development/primitive_types.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/pytypes_generator.py` & `woke-3.3.0/woke/development/pytypes_generator.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/development/transactions.py` & `woke-3.3.0/woke/development/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,25 @@
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
+from urllib.error import HTTPError
 
 if TYPE_CHECKING:
     from .blocks import Block
 
 from .call_trace import CallTrace
 from .chain_interfaces import (
     AnvilChainInterface,
     GanacheChainInterface,
-    GethChainInterface,
+    GethLikeChainInterfaceAbc,
     HardhatChainInterface,
-    HermezChainInterface,
     TxParams,
 )
 from .core import (
     Account,
     Address,
     Chain,
     Wei,
@@ -212,15 +212,20 @@
     @property
     def chain(self) -> Chain:
         return self._chain
 
     @property
     @_fetch_tx_receipt
     def block(self) -> Block:
-        return self._chain.blocks[int(self._tx_receipt["blockNumber"], 16)]
+        return self._chain.blocks[self.block_number]
+
+    @property
+    @_fetch_tx_receipt
+    def block_number(self) -> int:
+        return int(self._tx_receipt["blockNumber"], 16)
 
     @property
     def data(self) -> bytes:
         return self._tx_params["data"] if "data" in self._tx_params else b""
 
     @property
     def from_(self) -> Account:
@@ -332,28 +337,28 @@
             chain_interface, (GanacheChainInterface, HardhatChainInterface)
         ):
             self._fetch_debug_trace_transaction()
             assert self._debug_trace_transaction is not None
             return self._chain._process_console_logs_from_debug_trace(
                 self._debug_trace_transaction
             )
-        elif isinstance(chain_interface, (GethChainInterface, HermezChainInterface)):
+        elif isinstance(chain_interface, GethLikeChainInterfaceAbc):
             try:
                 self._fetch_trace_transaction()
                 assert self._trace_transaction is not None
                 return self._chain._process_console_logs(self._trace_transaction)
-            except JsonRpcError as e:
+            except (JsonRpcError, HTTPError):
                 # TODO make assertions about error.code?
                 try:
                     self._fetch_debug_trace_transaction()
                     assert self._debug_trace_transaction is not None
                     return self._chain._process_console_logs_from_debug_trace(
                         self._debug_trace_transaction
                     )
-                except JsonRpcError as e:
+                except (JsonRpcError, HTTPError):
                     # TODO make assertions about error.code?
                     raise RuntimeError(
                         f"Could not get console logs for transaction {self.tx_hash} as trace_transaction and debug_trace_transaction are both unavailable"
                     )
         else:
             raise NotImplementedError
 
@@ -437,28 +442,28 @@
                 length = int(trace["stack"][-2], 16)
 
                 revert_data = bytes(read_from_memory(offset, length, trace["memory"]))
         elif isinstance(chain_interface, HardhatChainInterface):
             self._fetch_debug_trace_transaction()
             assert self._debug_trace_transaction is not None
             revert_data = bytes.fromhex(self._debug_trace_transaction["returnValue"])  # type: ignore
-        elif isinstance(chain_interface, (GethChainInterface, HermezChainInterface)):
+        elif isinstance(chain_interface, GethLikeChainInterfaceAbc):
             try:
                 self._fetch_trace_transaction()
                 assert self._trace_transaction is not None
                 revert_data = bytes.fromhex(
                     self._trace_transaction[0]["result"]["output"][2:]
                 )
-            except JsonRpcError as e:
+            except (JsonRpcError, HTTPError):
                 # TODO make assertions about error.code?
                 try:
                     self._fetch_debug_trace_transaction()
                     assert self._debug_trace_transaction is not None
                     revert_data = bytes.fromhex(self._debug_trace_transaction["returnValue"])  # type: ignore
-                except JsonRpcError as e:
+                except (JsonRpcError, HTTPError):
                     # TODO make assertions about error.code?
                     raise RuntimeError(
                         f"Could not get revert reason data for transaction {self.tx_hash} as trace_transaction and debug_trace_transaction are both unavailable"
                     )
         else:
             raise NotImplementedError
 
@@ -520,28 +525,28 @@
                 length = int(trace["stack"][-2], 16)
 
                 output = read_from_memory(offset, length, trace["memory"])
         elif isinstance(chain_interface, HardhatChainInterface):
             self._fetch_debug_trace_transaction()
             assert self._debug_trace_transaction is not None
             output = bytes.fromhex(self._debug_trace_transaction["returnValue"])  # type: ignore
-        elif isinstance(chain_interface, (GethChainInterface, HermezChainInterface)):
+        elif isinstance(chain_interface, GethLikeChainInterfaceAbc):
             try:
                 self._fetch_trace_transaction()
                 assert self._trace_transaction is not None
                 output = bytes.fromhex(
                     self._trace_transaction[0]["result"]["output"][2:]
                 )
-            except JsonRpcError as e:
+            except (JsonRpcError, HTTPError):
                 # TODO make assertions about error.code?
                 try:
                     self._fetch_debug_trace_transaction()
                     assert self._debug_trace_transaction is not None
                     output = bytes.fromhex(self._debug_trace_transaction["returnValue"])  # type: ignore
-                except JsonRpcError as e:
+                except (JsonRpcError, HTTPError):
                     # TODO make assertions about error.code?
                     raise RuntimeError(
                         f"Could not get return value for transaction {self.tx_hash} as trace_transaction and debug_trace_transaction are both unavailable"
                     )
         else:
             raise NotImplementedError
```

### Comparing `woke-3.2.0/woke/development/utils.py` & `woke-3.3.0/woke/development/utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/commands/generate_control_flow_graph.py` & `woke-3.3.0/woke/lsp/commands/generate_control_flow_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/commands/generate_imports_graph.py` & `woke-3.3.0/woke/lsp/commands/generate_imports_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/commands/generate_inheritance_graph.py` & `woke-3.3.0/woke/lsp/commands/generate_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/commands/generate_linearized_inheritance_graph.py` & `woke-3.3.0/woke/lsp/commands/generate_linearized_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/common_structures.py` & `woke-3.3.0/woke/lsp/common_structures.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/context.py` & `woke-3.3.0/woke/lsp/context.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/document_sync.py` & `woke-3.3.0/woke/lsp/document_sync.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/code_lens.py` & `woke-3.3.0/woke/lsp/features/code_lens.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/completion.py` & `woke-3.3.0/woke/lsp/features/completion.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/definition.py` & `woke-3.3.0/woke/lsp/features/definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from woke.ast.ir.declaration.modifier_definition import ModifierDefinition
 from woke.ast.ir.declaration.variable_declaration import VariableDeclaration
 from woke.ast.ir.expression.binary_operation import BinaryOperation
 from woke.ast.ir.expression.identifier import Identifier
 from woke.ast.ir.expression.member_access import MemberAccess
 from woke.ast.ir.expression.unary_operation import UnaryOperation
 from woke.ast.ir.meta.identifier_path import IdentifierPath
+from woke.ast.ir.meta.source_unit import SourceUnit
 from woke.ast.ir.type_name.user_defined_type_name import UserDefinedTypeName
 from woke.lsp.common_structures import (
     DocumentUri,
     Location,
     LocationLink,
     PartialResultParams,
     Position,
@@ -91,15 +92,15 @@
         isinstance(original_node, (UnaryOperation, BinaryOperation))
         and original_node.function is not None
     ):
         node = original_node.function
     else:
         node = original_node
 
-    if not isinstance(node, DeclarationAbc):
+    if not isinstance(node, (DeclarationAbc, SourceUnit)):
         return None
 
     definitions = []
 
     if isinstance(node, (FunctionDefinition, VariableDeclaration)):
         if isinstance(node, VariableDeclaration) or node.implemented:
             definitions.append((node.file, node.name_location))
@@ -125,14 +126,16 @@
             definitions.append((node.file, node.name_location))
         for base_modifier in node.base_modifiers:
             if base_modifier.implemented:
                 definitions.append((base_modifier.file, base_modifier.name_location))
         for child_modifier in node.child_modifiers:
             if child_modifier.implemented:
                 definitions.append((child_modifier.file, child_modifier.name_location))
+    elif isinstance(node, SourceUnit):
+        definitions.append((node.file, node.byte_location))
     else:
         definitions.append((node.file, node.name_location))
 
     return definitions
 
 
 async def _get_definition_from_cache(
@@ -154,16 +157,19 @@
     intervals = tree.at(old_byte_offset)
     nodes: List[IrAbc] = [interval.data for interval in intervals]
     if len(nodes) == 0:
         raise ValueError(f"Could not find node at {old_byte_offset}")
 
     node = max(nodes, key=lambda n: n.ast_tree_depth)
 
-    if isinstance(node, DeclarationAbc):
-        location = node.name_location
+    if isinstance(node, (DeclarationAbc, SourceUnit)):
+        if isinstance(node, DeclarationAbc):
+            location = node.name_location
+        else:
+            location = node.byte_location
         forward_changes = context.compiler.get_last_compilation_forward_changes(path)
         if forward_changes is None:
             raise Exception("No forward changes found")
         new_start = (
             changes_to_byte_offset(forward_changes[0 : location[0]]) + location[0]
         )
         new_end = changes_to_byte_offset(forward_changes[0 : location[1]]) + location[1]
```

### Comparing `woke-3.2.0/woke/lsp/features/diagnostic.py` & `woke-3.3.0/woke/lsp/features/diagnostic.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/document_link.py` & `woke-3.3.0/woke/lsp/features/document_link.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/document_symbol.py` & `woke-3.3.0/woke/lsp/features/document_symbol.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/hover.py` & `woke-3.3.0/woke/lsp/features/hover.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/implementation.py` & `woke-3.3.0/woke/lsp/features/implementation.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/references.py` & `woke-3.3.0/woke/lsp/features/references.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/rename.py` & `woke-3.3.0/woke/lsp/features/rename.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/type_definition.py` & `woke-3.3.0/woke/lsp/features/type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/features/type_hierarchy.py` & `woke-3.3.0/woke/lsp/features/type_hierarchy.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/lsp_compiler.py` & `woke-3.3.0/woke/lsp/lsp_compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,14 +362,15 @@
                     self.__discovered_files.add(new_path)
                     self.__force_compile_files.add(new_path)
         elif isinstance(change, DeleteFilesParams):
             for delete in change.files:
                 path = uri_to_path(delete.uri)
                 self.__deleted_files.add(path)
                 self.__discovered_files.discard(path)
+                self.__opened_files.pop(path, None)
         elif isinstance(change, DidOpenTextDocumentParams):
             path = uri_to_path(change.text_document.uri).resolve()
             self.__opened_files[path] = VersionedFile(
                 change.text_document.text, change.text_document.version
             )
             if (
                 path not in self.__discovered_files
```

### Comparing `woke-3.2.0/woke/lsp/methods.py` & `woke-3.3.0/woke/lsp/methods.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/protocol_structures.py` & `woke-3.3.0/woke/lsp/protocol_structures.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/rpc_protocol.py` & `woke-3.3.0/woke/lsp/rpc_protocol.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/server.py` & `woke-3.3.0/woke/lsp/server.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/server_capabilities.py` & `woke-3.3.0/woke/lsp/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/lsp/utils/position.py` & `woke-3.3.0/woke/lsp/utils/position.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/regex_parser/solidity_import.py` & `woke-3.3.0/woke/regex_parser/solidity_import.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/regex_parser/solidity_parser.py` & `woke-3.3.0/woke/regex_parser/solidity_parser.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/svm/abc.py` & `woke-3.3.0/woke/svm/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/svm/svm.py` & `woke-3.3.0/woke/svm/svm.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/testing/__init__.py` & `woke-3.3.0/woke/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/testing/core.py` & `woke-3.3.0/woke/testing/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,20 @@
     fix_library_abi,
 )
 from woke.development.globals import chain_interfaces_manager
 from woke.development.json_rpc import JsonRpcError
 
 from ..development.chain_interfaces import AnvilChainInterface
 from ..development.transactions import TransactionAbc, TransactionStatusEnum
-from ..utils.keyed_default_dict import KeyedDefaultDict
 
 
 class Chain(woke.development.core.Chain):
     _block_gas_limit: int
     _gas_price: Wei
     _max_priority_fee_per_gas: Wei
-    _nonces: KeyedDefaultDict[Address, int]  # pyright: reportGeneralTypeIssues=false
     _initial_base_fee_per_gas: Wei
 
     @contextmanager
     def connect(
         self,
         uri: Optional[str] = None,
         *,
@@ -58,19 +56,14 @@
         self, min_gas_price: Optional[int], block_base_fee_per_gas: Optional[int]
     ) -> None:
         connected_chains.append(self)
 
         self._require_signed_txs = False
         self._gas_price = Wei(0)
         self._max_priority_fee_per_gas = Wei(0)
-        self._nonces = KeyedDefaultDict(
-            lambda addr: self._chain_interface.get_transaction_count(
-                str(addr)
-            )  # pyright: reportGeneralTypeIssues=false
-        )
         block_info = self._chain_interface.get_block("pending")
         assert "gasLimit" in block_info
         self._block_gas_limit = int(block_info["gasLimit"], 16)
 
         if block_base_fee_per_gas is not None:
             self._initial_base_fee_per_gas = Wei(block_base_fee_per_gas)
         else:
@@ -85,17 +78,14 @@
         else:
             self.gas_price = self._chain_interface.get_gas_price()
 
     def _connect_finalize(self) -> None:
         connected_chains.remove(self)
         chain_interfaces_manager.free(self._chain_interface)
 
-    def _update_nonce(self, address: Address, nonce: int) -> None:
-        self._nonces[address] = nonce
-
     @check_connected
     def snapshot(self) -> str:
         snapshot_id = self._chain_interface.snapshot()
 
         self._snapshots[snapshot_id] = {
             "nonces": self._nonces.copy(),
             "accounts": self._accounts.copy(),
@@ -307,15 +297,15 @@
 
         while tx.status == TransactionStatusEnum.PENDING:
             pass
 
         if confirmations == 1:
             return
 
-        while self.blocks["latest"].number - tx.block.number < confirmations - 1:
+        while self.blocks["latest"].number - tx.block_number < confirmations - 1:
             pass
 
     def _confirm_transaction(self, tx: TxParams) -> None:
         pass
 
 
 default_chain = Chain()
```

### Comparing `woke-3.2.0/woke/testing/coverage.py` & `woke-3.3.0/woke/testing/coverage.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/testing/fuzzing/fuzz_test.py` & `woke-3.3.0/woke/testing/fuzzing/fuzz_test.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/testing/fuzzing/fuzzer.py` & `woke-3.3.0/woke/testing/fuzzing/fuzzer.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/testing/fuzzing/generators.py` & `woke-3.3.0/woke/testing/fuzzing/generators.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/utils/context_managers.py` & `woke-3.3.0/woke/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/utils/decorators.py` & `woke-3.3.0/woke/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/utils/file_utils.py` & `woke-3.3.0/woke/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/utils/openzeppelin.py` & `woke-3.3.0/woke/utils/openzeppelin.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/utils/string.py` & `woke-3.3.0/woke/utils/string.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/utils/tee.py` & `woke-3.3.0/woke/utils/tee.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/woke/utils/threaded_child_watcher.py` & `woke-3.3.0/woke/utils/threaded_child_watcher.py`

 * *Files identical despite different names*

### Comparing `woke-3.2.0/setup.py` & `woke-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 entry_points = \
 {'console_scripts': ['woke = woke.cli.__main__:main',
                      'woke-solc = woke.cli.__main__:woke_solc']}
 
 setup_kwargs = {
     'name': 'woke',
-    'version': '3.2.0',
+    'version': '3.3.0',
     'description': 'Woke is a Python-based development and testing framework for Solidity.',
     'long_description': '# Woke\n\nWoke is a Python-based development and testing framework for Solidity.\n\nFeatures:\n\n- **Testing framework** - a testing framework for Solidity smart contracts with Python-native equivalents of Solidity types and blazing fast execution.\n\n- **Fuzzer** - a property-based fuzzer for Solidity smart contracts that allows testers to write their fuzz tests in Python.\n\n- **Vulnerability detectors**\n\n- **LSP server**\n\n## Dependencies\n\n- [Python](https://www.python.org/downloads/release/python-3910/) (version 3.7 or higher)\n\n> :warning: Python 3.11 is experimentally supported.\n\n## Installation\n\nvia `pip`\n\n```shell\npip3 install woke\n```\n\n## Documentation & Contribution\n\nWoke documentation can be found [here](https://ackeeblockchain.com/woke/docs/latest).\n\nThere you can also find a section on [contributing](https://ackeeblockchain.com/woke/docs/latest/contributing/).\n\n## Features\n\n### Testing framework\n\nSee [examples](examples/testing) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.\n\nWriting tests is as simple as:\n\n```python\nfrom woke.testing import *\nfrom pytypes.contracts.Counter import Counter\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n\n    counter = Counter.deploy()\n    assert counter.count() == 0\n\n    counter.increment()\n    assert counter.count() == 1\n```\n\n### Fuzzer\n\nFuzzer builds on top of the testing framework and allows efficient fuzz testing of Solidity smart contracts.\n\n```python\nfrom woke.testing import *\nfrom woke.testing.fuzzing import *\nfrom pytypes.contracts.Counter import Counter\n\nclass CounterTest(FuzzTest):\n    def pre_sequence(self) -> None:\n        self.counter = Counter.deploy()\n        self.count = 0\n\n    @flow()\n    def increment(self) -> None:\n        self.counter.increment()\n        self.count += 1\n\n    @flow()\n    def decrement(self) -> None:\n        with may_revert(Panic(PanicCodeEnum.UNDERFLOW_OVERFLOW)) as e:\n            self.counter.decrement()\n\n        if e.value is not None:\n            assert self.count == 0\n        else:\n            self.count -= 1\n\n    @invariant(period=10)\n    def count(self) -> None:\n        assert self.counter.count() == self.count\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n    CounterTest().run(sequences_count=30, flows_count=100)\n```\n\n### Vulnerability detectors\n\nVulnerability detectors can be run using:\n```shell\nwoke detect\n```\n\n### LSP server\n\nWoke implements an [LSP](https://microsoft.github.io/language-server-protocol/) server for Solidity. The only currently supported communication channel is TCP.\n\nWoke LSP server can be run using:\n\n```shell\nwoke lsp\n```\n\nOr with an optional --port argument:\n\n```shell\nwoke lsp --port 1234\n```\n\nAll LSP server features can be found in the [documentation](https://ackeeblockchain.com/woke/docs/latest/language-server/).\n\n## License\n\nThis project is licensed under the [ISC license](https://github.com/Ackee-Blockchain/woke/blob/main/LICENSE).\n\n## Partners\n\nRockawayX             |  Coinbase\n:-------------------------:|:-------------------------:\n[![](https://github.com/Ackee-Blockchain/woke/blob/main/images/rockawayx.jpg?raw=true)](https://rockawayx.com/)  |  [![](https://github.com/Ackee-Blockchain/woke/blob/main/images/coinbase.png?raw=true)](https://www.coinbase.com/)\n\n\n\n\n\n\n',
     'author': 'Ackee Blockchain',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ackeeblockchain.com',
```

### Comparing `woke-3.2.0/PKG-INFO` & `woke-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woke
-Version: 3.2.0
+Version: 3.3.0
 Summary: Woke is a Python-based development and testing framework for Solidity.
 Home-page: https://ackeeblockchain.com
 License: ISC
 Keywords: ethereum,solidity,security,testing,development,framework,audit
 Author: Ackee Blockchain
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved
```

