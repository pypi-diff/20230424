# Comparing `tmp/polyglot_piranha-0.3.2.tar.gz` & `tmp/polyglot_piranha-0.3.3.tar.gz`

## Comparing `polyglot_piranha-0.3.2.tar` & `polyglot_piranha-0.3.3.tar`

### file list

```diff
@@ -1,127 +1,128 @@
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.2/Cargo.toml
--rw-r--r--   0     1001      123    35211 2023-04-11 23:15:27.000000 polyglot_piranha-0.3.2/Cargo.lock
--rw-r--r--   0     1001      123    11359 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/LICENSE
--rw-r--r--   0     1001      123     3091 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/README.md
--rw-r--r--   0     1001      123     1373 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
--rw-r--r--   0     1001      123      994 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
--rw-r--r--   0     1001      123     5517 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
--rw-r--r--   0     1001      123     5621 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
--rw-r--r--   0     1001      123    66915 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
--rw-r--r--   0     1001      123    21518 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
--rw-r--r--   0     1001      123     5106 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
--rw-r--r--   0     1001      123      377 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
--rw-r--r--   0     1001      123     3615 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
--rw-r--r--   0     1001      123     5039 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
--rw-r--r--   0     1001      123     2584 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
--rw-r--r--   0     1001      123     2605 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
--rw-r--r--   0     1001      123      550 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
--rw-r--r--   0     1001      123     2456 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
--rw-r--r--   0     1001      123    13106 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
--rw-r--r--   0     1001      123     5875 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
--rw-r--r--   0     1001      123    85120 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
--rw-r--r--   0     1001      123    55188 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
--rw-r--r--   0     1001      123    48474 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
--rw-r--r--   0     1001      123     2304 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
--rw-r--r--   0     1001      123    33367 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
--rw-r--r--   0     1001      123     6780 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
--rw-r--r--   0     1001      123     3480 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
--rw-r--r--   0     1001      123     8540 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
--rw-r--r--   0     1001      123     4153 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
--rw-r--r--   0     1001      123     4326 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
--rw-r--r--   0     1001      123     2555 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
--rw-r--r--   0     1001      123     1490 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
--rw-r--r--   0     1001      123     2091 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
--rw-r--r--   0     1001      123     2194 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
--rw-r--r--   0     1001      123     1550 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
--rw-r--r--   0     1001      123     1618 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
--rw-r--r--   0     1001      123     1573 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
--rw-r--r--   0     1001      123       75 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
--rw-r--r--   0     1001      123      109 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
--rw-r--r--   0     1001      123      175 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
--rw-r--r--   0     1001      123      103 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
--rw-r--r--   0     1001      123      154 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
--rw-r--r--   0     1001      123      155 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
--rw-r--r--   0     1001      123      160 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
--rw-r--r--   0     1001      123      122 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
--rw-r--r--   0     1001      123      229 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
--rw-r--r--   0     1001      123       97 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
--rw-r--r--   0     1001      123      202 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
--rw-r--r--   0     1001      123      213 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
--rw-r--r--   0     1001      123      216 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
--rw-r--r--   0     1001      123      361 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
--rw-r--r--   0     1001      123      525 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
--rw-r--r--   0     1001      123      526 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
--rw-r--r--   0     1001      123      488 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
--rw-r--r--   0     1001      123      489 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
--rw-r--r--   0     1001      123      526 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
--rw-r--r--   0     1001      123      704 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
--rw-r--r--   0     1001      123     1332 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
--rw-r--r--   0     1001      123      192 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
--rw-r--r--   0     1001      123      739 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
--rw-r--r--   0     1001      123      652 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
--rw-r--r--   0     1001      123     1896 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
--rw-r--r--   0     1001      123      844 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return.json
--rw-r--r--   0     1001      123     1776 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
--rw-r--r--   0     1001      123     1932 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
--rw-r--r--   0     1001      123     4525 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
--rw-r--r--   0     1001      123      251 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
--rw-r--r--   0     1001      123      246 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
--rw-r--r--   0     1001      123      142 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
--rw-r--r--   0     1001      123     1637 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
--rw-r--r--   0     1001      123     1304 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
--rw-r--r--   0     1001      123     1304 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
--rw-r--r--   0     1001      123     1107 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
--rw-r--r--   0     1001      123     2565 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/javascript/src/config_checker.js
--rw-r--r--   0     1001      123     4304 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/javascript/src/piranha.js
--rw-r--r--   0     1001      123    27988 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/javascript/src/refactor.js
--rw-r--r--   0     1001      123     1445 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/javascript/src/source_checker.js
--rw-r--r--   0     1001      123      646 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
--rw-r--r--   0     1001      123     1064 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/README.txt
--rw-r--r--   0     1001      123    26229 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
--rw-r--r--   0     1001      123        0 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
--rw-r--r--   0     1001      123      793 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/pyproject.toml
--rw-r--r--   0     1001      123     2043 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/go/edges.toml
--rw-r--r--   0     1001      123    11027 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/go/rules.toml
--rw-r--r--   0     1001      123     1460 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/go/scope_config.toml
--rwxr-xr-x   0     1001      123     2241 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/java/edges.toml
--rwxr-xr-x   0     1001      123    15939 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/java/rules.toml
--rwxr-xr-x   0     1001      123     3582 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/java/scope_config.toml
--rwxr-xr-x   0     1001      123     2251 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/kt/edges.toml
--rwxr-xr-x   0     1001      123    19122 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/kt/rules.toml
--rwxr-xr-x   0     1001      123     2139 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/kt/scope_config.toml
--rw-r--r--   0     1001      123     1133 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/swift/edges.toml
--rw-r--r--   0     1001      123     9296 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/swift/rules.toml
--rw-r--r--   0     1001      123     1369 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/cleanup_rules/swift/scope_config.toml
--rw-r--r--   0     1001      123     7317 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/lib.rs
--rw-r--r--   0     1001      123     1679 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/main.rs
--rw-r--r--   0     1001      123     5799 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/constraint.rs
--rw-r--r--   0     1001      123     3143 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/default_configs.rs
--rw-r--r--   0     1001      123     4915 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/edit.rs
--rw-r--r--   0     1001      123     6744 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/language.rs
--rw-r--r--   0     1001      123    11140 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/matches.rs
--rw-r--r--   0     1001      123      928 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/mod.rs
--rw-r--r--   0     1001      123     1987 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/outgoing_edges.rs
--rw-r--r--   0     1001      123    14202 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/piranha_arguments.rs
--rw-r--r--   0     1001      123     2091 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/piranha_output.rs
--rw-r--r--   0     1001      123     7916 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/rule.rs
--rw-r--r--   0     1001      123     6286 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/rule_graph.rs
--rw-r--r--   0     1001      123     5931 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/rule_store.rs
--rw-r--r--   0     1001      123     3329 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/scopes.rs
--rw-r--r--   0     1001      123    14473 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/source_code_unit.rs
--rw-r--r--   0     1001      123     1586 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/unit_tests/piranha_arguments_test.rs
--rw-r--r--   0     1001      123     8340 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/unit_tests/rule_test.rs
--rw-r--r--   0     1001      123     6061 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/unit_tests/scopes_test.rs
--rw-r--r--   0     1001      123     6996 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/models/unit_tests/source_code_unit_test.rs
--rw-r--r--   0     1001      123     8196 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/mod.rs
--rw-r--r--   0     1001      123     1647 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_go.rs
--rw-r--r--   0     1001      123    12255 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_java.rs
--rw-r--r--   0     1001      123     1862 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_kt.rs
--rw-r--r--   0     1001      123     2423 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_python.rs
--rw-r--r--   0     1001      123     1833 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_swift.rs
--rw-r--r--   0     1001      123     1138 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_ts.rs
--rw-r--r--   0     1001      123     1281 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/tests/test_piranha_tsx.rs
--rw-r--r--   0     1001      123     5476 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/utilities/mod.rs
--rw-r--r--   0     1001      123    12743 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/utilities/tree_sitter_utilities.rs
--rw-r--r--   0     1001      123     3681 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/utilities/unit_tests/tree_sitter_utilities_test.rs
--rw-r--r--   0     1001      123     2237 2023-04-11 23:13:48.000000 polyglot_piranha-0.3.2/src/utilities/unit_tests/utilities_test.rs
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.3/Cargo.toml
+-rw-r--r--   0     1001      123    35472 2023-04-24 21:40:36.000000 polyglot_piranha-0.3.3/Cargo.lock
+-rw-r--r--   0     1001      123    11359 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/LICENSE
+-rw-r--r--   0     1001      123     3091 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/README.md
+-rw-r--r--   0     1001      123     1373 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
+-rw-r--r--   0     1001      123      994 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
+-rw-r--r--   0     1001      123     5517 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
+-rw-r--r--   0     1001      123     5621 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
+-rw-r--r--   0     1001      123    66915 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
+-rw-r--r--   0     1001      123    21518 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
+-rw-r--r--   0     1001      123     5106 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
+-rw-r--r--   0     1001      123      377 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
+-rw-r--r--   0     1001      123     3615 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
+-rw-r--r--   0     1001      123     5039 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
+-rw-r--r--   0     1001      123     2584 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
+-rw-r--r--   0     1001      123     2605 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
+-rw-r--r--   0     1001      123      550 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
+-rw-r--r--   0     1001      123     2456 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
+-rw-r--r--   0     1001      123    13106 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
+-rw-r--r--   0     1001      123     5875 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
+-rw-r--r--   0     1001      123    85120 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
+-rw-r--r--   0     1001      123    55188 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
+-rw-r--r--   0     1001      123    48474 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
+-rw-r--r--   0     1001      123     2304 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
+-rw-r--r--   0     1001      123    33367 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
+-rw-r--r--   0     1001      123     6780 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
+-rw-r--r--   0     1001      123     3480 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
+-rw-r--r--   0     1001      123     8540 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
+-rw-r--r--   0     1001      123     4153 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
+-rw-r--r--   0     1001      123     4326 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
+-rw-r--r--   0     1001      123     2555 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
+-rw-r--r--   0     1001      123     1490 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
+-rw-r--r--   0     1001      123     2091 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
+-rw-r--r--   0     1001      123     2194 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
+-rw-r--r--   0     1001      123     1550 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
+-rw-r--r--   0     1001      123     1618 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
+-rw-r--r--   0     1001      123     1573 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
+-rw-r--r--   0     1001      123       75 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
+-rw-r--r--   0     1001      123      109 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
+-rw-r--r--   0     1001      123      175 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
+-rw-r--r--   0     1001      123      103 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
+-rw-r--r--   0     1001      123      154 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
+-rw-r--r--   0     1001      123      155 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
+-rw-r--r--   0     1001      123      160 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
+-rw-r--r--   0     1001      123      122 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
+-rw-r--r--   0     1001      123      229 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
+-rw-r--r--   0     1001      123       97 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
+-rw-r--r--   0     1001      123      202 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
+-rw-r--r--   0     1001      123      213 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
+-rw-r--r--   0     1001      123      216 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
+-rw-r--r--   0     1001      123      361 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
+-rw-r--r--   0     1001      123      525 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
+-rw-r--r--   0     1001      123      526 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
+-rw-r--r--   0     1001      123      488 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
+-rw-r--r--   0     1001      123      489 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
+-rw-r--r--   0     1001      123      526 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
+-rw-r--r--   0     1001      123      704 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
+-rw-r--r--   0     1001      123     1332 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
+-rw-r--r--   0     1001      123      192 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
+-rw-r--r--   0     1001      123      739 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
+-rw-r--r--   0     1001      123      652 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
+-rw-r--r--   0     1001      123     1896 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
+-rw-r--r--   0     1001      123      844 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return.json
+-rw-r--r--   0     1001      123     1776 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
+-rw-r--r--   0     1001      123     1932 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
+-rw-r--r--   0     1001      123     4525 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
+-rw-r--r--   0     1001      123      251 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
+-rw-r--r--   0     1001      123      246 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
+-rw-r--r--   0     1001      123      142 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
+-rw-r--r--   0     1001      123     1637 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
+-rw-r--r--   0     1001      123     1304 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
+-rw-r--r--   0     1001      123     1304 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
+-rw-r--r--   0     1001      123     1107 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
+-rw-r--r--   0     1001      123     2565 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/javascript/src/config_checker.js
+-rw-r--r--   0     1001      123     4304 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/javascript/src/piranha.js
+-rw-r--r--   0     1001      123    27988 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/javascript/src/refactor.js
+-rw-r--r--   0     1001      123     1445 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/javascript/src/source_checker.js
+-rw-r--r--   0     1001      123      646 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
+-rw-r--r--   0     1001      123     1064 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/README.txt
+-rw-r--r--   0     1001      123    26229 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
+-rw-r--r--   0     1001      123        0 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
+-rw-r--r--   0     1001      123      793 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/pyproject.toml
+-rw-r--r--   0     1001      123     2043 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/go/edges.toml
+-rw-r--r--   0     1001      123    11027 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/go/rules.toml
+-rw-r--r--   0     1001      123     1460 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/go/scope_config.toml
+-rwxr-xr-x   0     1001      123     2241 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/java/edges.toml
+-rwxr-xr-x   0     1001      123    17618 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/java/rules.toml
+-rwxr-xr-x   0     1001      123     3582 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/java/scope_config.toml
+-rwxr-xr-x   0     1001      123     2251 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/kt/edges.toml
+-rwxr-xr-x   0     1001      123    19122 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/kt/rules.toml
+-rwxr-xr-x   0     1001      123     2139 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/kt/scope_config.toml
+-rw-r--r--   0     1001      123     1133 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/swift/edges.toml
+-rw-r--r--   0     1001      123    10134 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/swift/rules.toml
+-rw-r--r--   0     1001      123     1369 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/swift/scope_config.toml
+-rw-r--r--   0     1001      123     7317 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/lib.rs
+-rw-r--r--   0     1001      123     1679 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/main.rs
+-rw-r--r--   0     1001      123     5799 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/constraint.rs
+-rw-r--r--   0     1001      123     3178 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/default_configs.rs
+-rw-r--r--   0     1001      123     4915 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/edit.rs
+-rw-r--r--   0     1001      123     7047 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/language.rs
+-rw-r--r--   0     1001      123    11140 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/matches.rs
+-rw-r--r--   0     1001      123      928 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/mod.rs
+-rw-r--r--   0     1001      123     1987 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/outgoing_edges.rs
+-rw-r--r--   0     1001      123    14202 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/piranha_arguments.rs
+-rw-r--r--   0     1001      123     2091 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/piranha_output.rs
+-rw-r--r--   0     1001      123     7916 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/rule.rs
+-rw-r--r--   0     1001      123     6286 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/rule_graph.rs
+-rw-r--r--   0     1001      123     5931 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/rule_store.rs
+-rw-r--r--   0     1001      123     3329 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/scopes.rs
+-rw-r--r--   0     1001      123    14473 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/source_code_unit.rs
+-rw-r--r--   0     1001      123     1586 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/unit_tests/piranha_arguments_test.rs
+-rw-r--r--   0     1001      123     8340 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/unit_tests/rule_test.rs
+-rw-r--r--   0     1001      123     6061 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/unit_tests/scopes_test.rs
+-rw-r--r--   0     1001      123     6996 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/unit_tests/source_code_unit_test.rs
+-rw-r--r--   0     1001      123     8222 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/mod.rs
+-rw-r--r--   0     1001      123     1647 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_go.rs
+-rw-r--r--   0     1001      123    12255 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_java.rs
+-rw-r--r--   0     1001      123     1862 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_kt.rs
+-rw-r--r--   0     1001      123     2423 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_python.rs
+-rw-r--r--   0     1001      123     1833 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_swift.rs
+-rw-r--r--   0     1001      123      770 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_thrift.rs
+-rw-r--r--   0     1001      123     1138 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_ts.rs
+-rw-r--r--   0     1001      123     1281 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_tsx.rs
+-rw-r--r--   0     1001      123     5476 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/utilities/mod.rs
+-rw-r--r--   0     1001      123    12743 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/utilities/tree_sitter_utilities.rs
+-rw-r--r--   0     1001      123     3681 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/utilities/unit_tests/tree_sitter_utilities_test.rs
+-rw-r--r--   0     1001      123     2237 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/utilities/unit_tests/utilities_test.rs
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.3/PKG-INFO
```

### Comparing `polyglot_piranha-0.3.2/Cargo.toml` & `polyglot_piranha-0.3.3/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "Ameya Ketkar <ketkara@uber.com>",
   "Lazaro Clapp <lazaro@uber.com>",
   "Murali Krishna Ramanathan",
   "Uber Technologies Inc.",
 ]
 name = "piranha"
 description = "Polyglot Piranha is a library for performing structural find and replace with deep cleanup."
-version = "0.3.2"
+version = "0.3.3"
 edition = "2021"
 include = ["pyproject.toml", "src/"]
 exclude = ["legacy"]
 license-file = "LICENSE"
 categories = [
   "structural find-replace",
   "find-replace",
@@ -46,21 +46,23 @@
 clap = { version = "4.0.3", features = ["derive"] }
 log = "0.4.16"
 env_logger = "0.10.0"
 tempdir = "0.3"
 serde_json = "1.0.82"
 # TODO: Update after https://github.com/fwcd/tree-sitter-kotlin/pull/71 lands
 tree-sitter-kotlin = { git = "https://github.com/ketkarameya/tree-sitter-kotlin.git", rev = "a87ddd003368e068563f1cc478a1b2a3f9d73b60" }
-tree-sitter-java = "0.20.0"
+# TODO: Update after next version is released (https://github.com/tree-sitter/tree-sitter-java/issues/146)
+tree-sitter-java = { git = "https://github.com/tree-sitter/tree-sitter-java.git", rev = "c194ee5e6ede5f26cf4799feead4a8f165dcf14d" }
 # TODO: Update after: https://github.com/alex-pinkus/tree-sitter-swift/issues/278 resolves
 tree-sitter-swift = { git = "https://github.com/satyam1749/tree-sitter-swift.git", rev = "c92496b5273e4d3b094148fee51de371c94729bf" }
 tree-sitter-python = "0.20.2"
 tree-sitter-typescript = "0.20.1"
 # TODO: Update after https://github.com/tree-sitter/tree-sitter-go/pull/103 lands
 tree-sitter-go = { git = "https://github.com/uber/tree-sitter-go.git", rev = "8f807196afab4a1a1256dbf62a011020c6fe7745" }
+tree-sitter-thrift = "0.5.0"
 derive_builder = "0.12.0"
 getset = "0.1.2"
 pyo3 = "0.18.2"
 pyo3-log = "0.8.1"
 
 [features]
 extension-module = ["pyo3/extension-module"]
```

### Comparing `polyglot_piranha-0.3.2/Cargo.lock` & `polyglot_piranha-0.3.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,71 +1,80 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.2.6"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "342258dd14006105c2b75ab1bd7543a03bdf0cfc94383303ac212a04939dff6f"
+checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
 dependencies = [
  "anstyle",
  "anstyle-parse",
+ "anstyle-query",
  "anstyle-wincon",
- "concolor-override",
- "concolor-query",
+ "colorchoice",
  "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "0.3.5"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23ea9e81bd02e310c216d080f6223c179012256e5151c41db88d12c88a1684d2"
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7d1bb534e9efed14f3e5f44e7dd1a4f709384023a4165199a4241e18dff0116"
+checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "anstyle-wincon"
-version = "0.2.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3127af6145b149f3287bb9a0d10ad9c5692dba8c53ad48285e5bec4063834fa"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
 name = "assert_cmd"
-version = "2.0.10"
+version = "2.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec0b2340f55d9661d76793b2bfc2eb0e62689bd79d067a95707ea762afd5e9dd"
+checksum = "86d6b683edf8d1119fe420a94f8a7e389239666aa72e65495d91c00462510151"
 dependencies = [
  "anstyle",
  "bstr",
  "doc-comment",
  "predicates",
  "predicates-core",
  "predicates-tree",
@@ -117,28 +126,28 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.2.1"
+version = "4.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "046ae530c528f252094e4a77886ee1374437744b2bff1497aa898bbddbbb29b3"
+checksum = "956ac1f6381d8d82ab4684768f89c0ea3afe66925ceadb4eeb3fc452ffc55d62"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.1"
+version = "4.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "223163f58c9a40c3b0a43e1c4b50a9ce09f007ea2cb1ec258a687945b4b7929f"
+checksum = "84080e799e54cff944f4b4a4b0e71630b0e0443b25b985175c7dddc1a859b749"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
@@ -148,50 +157,41 @@
 version = "4.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.14",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
 
 [[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "colored"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3616f750b84d8f0de8a58bda93e08e2a81ad3f523089b05f1dffecab48c6cbd"
 dependencies = [
  "atty",
  "lazy_static",
  "winapi",
 ]
 
 [[package]]
-name = "concolor-override"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a855d4a1978dc52fb0536a04d384c2c0c1aa273597f08b77c8c4d3b2eec6037f"
-
-[[package]]
-name = "concolor-query"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88d11d52c3d7ca2e6d0040212be9e4dbbcd78b6447f535b6b561f449427944cf"
-dependencies = [
- "windows-sys 0.45.0",
-]
-
-[[package]]
 name = "crossbeam"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2801af0d36612ae591caa9568261fddce32ce6e08a7275ea334a06a4ad021a2c"
 dependencies = [
  "cfg-if",
  "crossbeam-channel",
@@ -527,23 +527,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.1"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d59d8c75012853d2e872fb56bc8a2e53718e2cafe1a4c823143141c6d90c322f"
+checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -627,15 +627,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "piranha"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "assert_cmd",
  "cc",
  "clap",
  "colored",
  "derive_builder",
  "env_logger",
@@ -655,23 +655,24 @@
  "toml",
  "tree-sitter",
  "tree-sitter-go",
  "tree-sitter-java",
  "tree-sitter-kotlin",
  "tree-sitter-python",
  "tree-sitter-swift",
+ "tree-sitter-thrift",
  "tree-sitter-traversal",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "predicates"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c575290b64d24745b6c57a12a31465f0a66f3a4799686a6921526a33b0797965"
+checksum = "09963355b9f467184c04017ced4a2ba2d75cbcb4e7462690d388233253d4b1a9"
 dependencies = [
  "anstyle",
  "difflib",
  "float-cmp",
  "itertools",
  "normalize-line-endings",
  "predicates-core",
@@ -725,44 +726,44 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
@@ -773,29 +774,29 @@
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -873,49 +874,49 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "remove_dir_all"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.11"
+version = "0.37.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85597d61f83914ddeba6a47b3b8ffe7365107221c2e557ed94426489fefb5f77"
+checksum = "d9b864d3c18a5785a05953adeed93e2dca37ed30f18e69bba9f30079d51f363f"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -943,22 +944,22 @@
 name = "serde_derive"
 version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.14",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -991,17 +992,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.14"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcf316d5356ed6847742d036f8a39c3b8435cac10bd528a4bd461928a6ab34d5"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1087,16 +1088,15 @@
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-java"
 version = "0.20.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0bf5d3f508cbffcbfe1805834101c0d24297a8b6c2184ad9c595556c46d2420"
+source = "git+https://github.com/tree-sitter/tree-sitter-java.git?rev=c194ee5e6ede5f26cf4799feead4a8f165dcf14d#c194ee5e6ede5f26cf4799feead4a8f165dcf14d"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-kotlin"
@@ -1123,14 +1123,24 @@
 source = "git+https://github.com/satyam1749/tree-sitter-swift.git?rev=c92496b5273e4d3b094148fee51de371c94729bf#c92496b5273e4d3b094148fee51de371c94729bf"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
+name = "tree-sitter-thrift"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "10546b134d045fa8d8787d58faf5851d2b8c2d5eaad9699203c4e7197cd8bea5"
+dependencies = [
+ "cc",
+ "tree-sitter",
+]
+
+[[package]]
 name = "tree-sitter-traversal"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df8a158225e4a4d8505f071340bba9edd109b23f01b70540dccb7c799868f307"
 dependencies = [
  "tree-sitter",
 ]
```

### Comparing `polyglot_piranha-0.3.2/LICENSE` & `polyglot_piranha-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/README.md` & `polyglot_piranha-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_argument.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_receive.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json` & `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java` & `polyglot_piranha-0.3.3/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak` & `polyglot_piranha-0.3.3/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect` & `polyglot_piranha-0.3.3/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/javascript/src/config_checker.js` & `polyglot_piranha-0.3.3/legacy/javascript/src/config_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/javascript/src/piranha.js` & `polyglot_piranha-0.3.3/legacy/javascript/src/piranha.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/javascript/src/refactor.js` & `polyglot_piranha-0.3.3/legacy/javascript/src/refactor.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/javascript/src/source_checker.js` & `polyglot_piranha-0.3.3/legacy/javascript/src/source_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt` & `polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/README.txt` & `polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/README.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp` & `polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/pyproject.toml` & `polyglot_piranha-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/go/edges.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/go/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/go/rules.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/go/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/go/scope_config.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/go/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/java/edges.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/java/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/java/rules.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/java/rules.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 # <p>Unless required by applicable law or agreed to in writing, software distributed under the
 # License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
 # The language specific rules in this file are applied after the API specific change has been performed.
 
+# Before: 
+# (true)
+# After 
+# true
+
+[[rules]]
+name = "simplify_parenthesized_expression"
+query = "(parenthesized_expression ([(true) (false) (identifier)] @expression)) @p_expr"
+replace = "@expression"
+replace_node = "p_expr"
+is_seed_rule = false
+groups = ["boolean_expression_simplify"]
+
 # Before : 
 #  if (true) { doSomething(); }
 # After :
 #  { doSomething(); } 
 # 
 # Before : 
 #  if (true) { doSomething(); } else { doSomethingElse();}
@@ -23,15 +36,15 @@
 #
 [[rules]]
 groups = ["if_cleanup"]
 name = "simplify_if_statement_true"
 query = """
 (
     (if_statement
-        condition : ((parenthesized_expression [(true) (parenthesized_expression (true))]))
+        condition : (condition (true))
         consequence : ((statement) @consequence))
 @if_statement)
 """
 replace = "@consequence"
 replace_node = "if_statement"
 is_seed_rule = false
 
@@ -46,15 +59,15 @@
 #  
 [[rules]]
 groups = ["if_cleanup"]
 name = "simplify_if_statement_false"
 query = """
 (
     (if_statement
-        condition : (parenthesized_expression [(false) @i (parenthesized_expression (false))])
+        condition : (condition (false))
         consequence : ((statement) @consequence)
         alternative : ((_) @alternative) ?)
 @if_statement)"""
 replace = "@alternative"
 replace_node = "if_statement"
 is_seed_rule = false
 
@@ -66,15 +79,15 @@
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_not_false"
 query = """
 (
     (unary_expression
         operator: "!"
-        operand: [(false) (parenthesized_expression (false))])
+        operand: (false))
 @unary_expression)
 """
 replace = "true"
 replace_node = "unary_expression"
 is_seed_rule = false
 
 # Before : 
@@ -85,15 +98,15 @@
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_not_true"
 query = """
 (
     (unary_expression
         operator: \"!\"
-        operand: [(true) (parenthesized_expression (true))])
+        operand: (true))
 @unary_expression)
 """
 replace = "false"
 replace_node = "unary_expression"
 is_seed_rule = false
 
 # Before : 
@@ -142,15 +155,15 @@
 
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_true_and_something"
 query = """
 (
     (binary_expression
-        left: [(true) (parenthesized_expression (true))]
+        left: (true)
         operator:"&&"
         right : (_) @rhs) 
 ) @binary_expression
 """
 replace = "@rhs"
 replace_node = "binary_expression"
 is_seed_rule = false
@@ -164,15 +177,15 @@
 groups = ["boolean_expression_simplify"]
 name = "simplify_something_and_true"
 query = """
 (
     (binary_expression
         left : (_) @lhs
         operator:"&&"
-        right: [(true) (parenthesized_expression (true))]
+        right: (true)
     )
 @binary_expression)"""
 replace = "@lhs"
 replace_node = "binary_expression"
 is_seed_rule = false
 
 # Before :
@@ -182,15 +195,15 @@
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_false_and_something"
 query = """
 (
     (binary_expression
-        left: [(false) (parenthesized_expression (false))]
+        left: (false)
         operator : "&&"
         right : (_) @rhs
     )
 @binary_expression)"""
 replace = "false"
 replace_node = "binary_expression"
 is_seed_rule = false
@@ -204,22 +217,19 @@
 name = "simplify_something_and_false"
 groups = ["boolean_expression_simplify"]
 query = """
 (
     (binary_expression
         left : [
             (identifier)
-            (parenthesized_expression (identifier))
             (true)
-            (parenthesized_expression (true))
             (false)
-            (parenthesized_expression (false))
         ] @lhs
         operator : "&&"
-        right: [(false) (parenthesized_expression (false))]
+        right: (false)
     )
 @binary_expression)
 """
 replace = "false"
 replace_node = "binary_expression"
 is_seed_rule = false
 
@@ -232,22 +242,19 @@
 groups = ["boolean_expression_simplify"]
 name = "simplify_something_or_true"
 query = """
 (
     (binary_expression
         left : [
             (identifier)
-            (parenthesized_expression (identifier))
             (true)
-            (parenthesized_expression (true))
             (false)
-            (parenthesized_expression (false))
         ] @lhs
         operator:"||"
-        right: [(true) (parenthesized_expression (true))]
+        right: (true)
     )
 @binary_expression)"""
 replace = "true"
 replace_node = "binary_expression"
 is_seed_rule = false
 
 # Before :
@@ -257,15 +264,15 @@
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_true_or_something"
 query = """
 (
     (binary_expression
-        left : [(true) (parenthesized_expression (true))]
+        left : (true)
         operator:"||"
         right: (_) @rhs
     )
 @binary_expression)
 """
 replace = "true"
 replace_node = "binary_expression"
@@ -280,15 +287,15 @@
 groups = ["boolean_expression_simplify"]
 name = "simplify_something_or_false"
 query = """(
 (
     binary_expression
         left : (_) @lhs
         operator:"||"
-        right: [(false) (parenthesized_expression (false))]
+        right: (false)
     )
 @binary_expression)"""
 replace = "@lhs"
 replace_node = "binary_expression"
 is_seed_rule = false
 
 # Before: 
@@ -298,28 +305,130 @@
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_false_or_something"
 query = """
 (
     (binary_expression
-        left : [(false) (parenthesized_expression (false))]
+        left : (false)
         operator:"||"
         right: (_) @rhs
     )
 @binary_expression)"""
 replace = "@rhs"
 replace_node = "binary_expression"
 is_seed_rule = false
 
+
+# Before: 
+#  (x) == x
+#  x == (x)
+#  x == x
+# After :
+#  true
+#  true
+#  true
+#
+[[rules]]
+groups = ["boolean_expression_simplify"]
+name = "simplify_equals_equals_true"
+query = """
+(
+    (binary_expression
+        left : [(parenthesized_expression (_) @lhs) (_) @lhs]
+        operator:"=="
+        right: [(parenthesized_expression (_) @rhs) (_) @rhs]
+    )
+@binary_expression
+(#eq? @lhs @rhs)
+)"""
+replace = "true"
+replace_node = "binary_expression"
+is_seed_rule = false
+
+
+# Before: 
+#  false == true 
+#  true == false
+# After :
+#  false
+#  false
+#
+[[rules]]
+groups = ["boolean_expression_simplify"]
+name = "simplify_equals_equals_false"
+query = """
+(
+    (binary_expression
+        left : [(false) @lhs (true) @lhs (string_literal) (decimal_integer_literal) @lhs (decimal_floating_point_literal) @lhs]
+        operator:"=="
+        right: [(false) @rhs (true) @rhs (string_literal) @rhs (decimal_integer_literal) @rhs (decimal_floating_point_literal) @rhs]
+    )
+@binary_expression
+(#not-eq? @lhs @rhs)
+)"""
+replace = "false"
+replace_node = "binary_expression"
+is_seed_rule = false
+
+
+# Before: 
+#  false != false 
+#  true != true
+# After :
+#  false
+#  false
+#
+[[rules]]
+groups = ["boolean_expression_simplify"]
+name = "simplify_not_equals_false"
+query = """
+(
+    (binary_expression
+        left : [(false) @lhs (true) @lhs (string_literal) (decimal_integer_literal) @lhs (decimal_floating_point_literal) @lhs]
+        operator:"!="
+        right: [(false) @rhs (true) @rhs (string_literal) @rhs (decimal_integer_literal) @rhs (decimal_floating_point_literal) @rhs]
+    )
+@binary_expression
+(#eq? @lhs @rhs)
+)"""
+replace = "false"
+replace_node = "binary_expression"
+is_seed_rule = false
+
+
+# Before: 
+#  false != true 
+#  true != false
+# After :
+#  true
+#  true
+#
+[[rules]]
+groups = ["boolean_expression_simplify"]
+name = "simplify_not_equals_true"
+query = """
+(
+    (binary_expression
+        left : [(false) @lhs (true) @lhs (string_literal) (decimal_integer_literal) @lhs (decimal_floating_point_literal) @lhs]
+        operator:"!="
+        right: [(false) @rhs (true) @rhs (string_literal) @rhs (decimal_integer_literal) @rhs (decimal_floating_point_literal) @rhs]
+    )
+@binary_expression
+(#not-eq? @lhs @rhs)
+)"""
+replace = "true"
+replace_node = "binary_expression"
+is_seed_rule = false
+
 # Before :
 #  {
 #    something();
 #    return 10;
-#    somethingMore();  
+#    somethingMore();
 #    return 100;
 #  } 
 # After :
 #  {
 #    something();
 #    return 10;
 #  } 
@@ -340,15 +449,15 @@
 #  abc()
 #
 [[rules]]
 groups = ["if_cleanup"]
 name = "simplify_ternary_operator_true"
 query = """
 (
-    (ternary_expression condition: [(true) (parenthesized_expression (true))]
+    (ternary_expression condition: (true)
         consequence: (_)* @consequence
         alternative: (_)* @alternative)
 @ternary_expression)"""
 replace = "@consequence"
 replace_node = "ternary_expression"
 is_seed_rule = false
 
@@ -358,15 +467,15 @@
 #  def()
 #
 [[rules]]
 groups = ["if_cleanup"]
 name = "simplify_ternary_operator_false"
 query = """
 (
-    (ternary_expression condition: [(false) (parenthesized_expression (false))]
+    (ternary_expression condition: (false)
         consequence: (_)* @consequence
         alternative: (_)* @alternative)
 @ternary_expression)"""
 replace = "@alternative"
 replace_node = "ternary_expression"
 is_seed_rule = false
 
@@ -464,15 +573,15 @@
 [[rules]]
 name = "delete_field_declaration"
 query = """
 (
 ((field_declaration 
                 declarator: (variable_declarator 
                                     name: (_) @variable_name
-                                    value: [(true) (false) (parenthesized_expression (true)) (parenthesized_expression (false))] @init)) @field_declaration)
+                                    value: [(true) (false)] @init)) @field_declaration)
 )
 """
 replace = ""
 replace_node = "field_declaration"
 is_seed_rule = false
 
 # Check if there is no assignment where the variable @variable_name is
```

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/java/scope_config.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/java/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/kt/edges.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/kt/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/kt/rules.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/kt/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/kt/scope_config.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/kt/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/swift/edges.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/swift/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/swift/rules.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/swift/rules.toml`

 * *Files 6% similar despite different names*

```diff
@@ -405,14 +405,37 @@
 groups = ["guard_cleanup"]
 replace_node = "guard_block"
 replace = ""
 is_seed_rule = false
 
 #
 # Before
+# var v = true ? x : y
+#
+# After
+# var v = x
+#
+[[rules]]
+name = "ternary_true"
+query = """(
+(ternary_expression
+    condition:[(boolean_literal) @true  
+            (tuple_expression 
+                value: (boolean_literal) @true)]
+    if_true:(_) @block_true
+    ) @ternary_block
+(#eq? @true "true")
+)"""
+groups = ["if_cleanup"]
+replace_node = "ternary_block"
+replace = "@block_true"
+is_seed_rule = false
+
+#
+# Before
 #   guard false else {
 #       return f1()
 #   }
 #   f2()
 # After 
 #   return f1()
 #   f2()
@@ -429,14 +452,36 @@
 (#eq? @false "false")
 )"""
 groups = ["guard_cleanup"]
 replace_node = "guard_block"
 replace = "@else_block"
 is_seed_rule = false
 
+#
+# var v = false ? x : y
+#
+# After
+# var v = y
+#
+[[rules]]
+name = "ternary_false"
+query = """(
+(ternary_expression
+    condition:[(boolean_literal) @false  
+            (tuple_expression 
+                value: (boolean_literal) @false)]
+    if_false:(_) @block_false
+    ) @ternary_block
+(#eq? @false "false")
+)"""
+groups = ["if_cleanup"]
+replace_node = "ternary_block"
+replace = "@block_false"
+is_seed_rule = false
+
 # Dummy rule that acts as a junction for all boolean based cleanups
 # Let's say you want to define rules from A -> B, A -> C, D -> B, D -> C, ... 
 # A pattern here is - if there is an outgoing edge to B there is another to C.
 # In these cases, you can use a dummy rule X as shown below:
 # X -> B, X - C, A -> X, D -> X, ...
 [[rules]]
 name = "boolean_literal_cleanup"
```

### Comparing `polyglot_piranha-0.3.2/src/cleanup_rules/swift/scope_config.toml` & `polyglot_piranha-0.3.3/src/cleanup_rules/swift/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/lib.rs` & `polyglot_piranha-0.3.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/main.rs` & `polyglot_piranha-0.3.3/src/main.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/constraint.rs` & `polyglot_piranha-0.3.3/src/models/constraint.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/default_configs.rs` & `polyglot_piranha-0.3.3/src/models/default_configs.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 pub const JAVA: &str = "java";
 pub const KOTLIN: &str = "kt";
 pub const GO: &str = "go";
 pub const PYTHON: &str = "py";
 pub const SWIFT: &str = "swift";
 pub const TYPESCRIPT: &str = "ts";
 pub const TSX: &str = "tsx";
+pub const THRIFT: &str = "thrift";
 
 #[cfg(test)]
 //FIXME: Remove this  hack by not passing PiranhaArguments to SourceCodeUnit
 pub(crate) const UNUSED_CODE_PATH: &str = "/dev/null";
 
 pub fn default_number_of_ancestors_in_parent_scope() -> u8 {
   4
```

### Comparing `polyglot_piranha-0.3.2/src/models/edit.rs` & `polyglot_piranha-0.3.3/src/models/edit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/language.rs` & `polyglot_piranha-0.3.3/src/models/language.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 use getset::Getters;
 use serde_derive::Deserialize;
 use tree_sitter::{Parser, Query};
 
 use crate::utilities::parse_toml;
 
 use super::{
-  default_configs::{default_language, GO, JAVA, KOTLIN, PYTHON, SWIFT, TSX, TYPESCRIPT},
+  default_configs::{default_language, GO, JAVA, KOTLIN, PYTHON, SWIFT, THRIFT, TSX, TYPESCRIPT},
   outgoing_edges::Edges,
   rule::Rules,
   scopes::{ScopeConfig, ScopeGenerator},
 };
 
 #[derive(Debug, Clone, Getters, PartialEq)]
 pub struct PiranhaLanguage {
@@ -57,14 +57,15 @@
   Java,
   Kotlin,
   Go,
   Swift,
   Ts,
   Tsx,
   Python,
+  Thrift,
 }
 
 impl PiranhaLanguage {
   pub fn create_query(&self, query_str: String) -> Query {
     let query = Query::new(self.language, query_str.as_str());
     if let Ok(q) = query {
       return q;
@@ -202,11 +203,20 @@
         supported_language: SupportedLanguage::Tsx,
         language: tree_sitter_typescript::language_tsx(),
         rules: None,
         edges: None,
         scopes: vec![],
         comment_nodes: vec![],
       }),
+      THRIFT => Ok(PiranhaLanguage {
+        name: language.to_string(),
+        supported_language: SupportedLanguage::Thrift,
+        language: tree_sitter_thrift::language(),
+        rules: None,
+        edges: None,
+        scopes: vec![],
+        comment_nodes: vec![],
+      }),
       _ => Err("Language not supported"),
     }
   }
 }
```

### Comparing `polyglot_piranha-0.3.2/src/models/matches.rs` & `polyglot_piranha-0.3.3/src/models/matches.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/mod.rs` & `polyglot_piranha-0.3.3/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/outgoing_edges.rs` & `polyglot_piranha-0.3.3/src/models/outgoing_edges.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/piranha_arguments.rs` & `polyglot_piranha-0.3.3/src/models/piranha_arguments.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/piranha_output.rs` & `polyglot_piranha-0.3.3/src/models/piranha_output.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/rule.rs` & `polyglot_piranha-0.3.3/src/models/rule.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/rule_graph.rs` & `polyglot_piranha-0.3.3/src/models/rule_graph.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/rule_store.rs` & `polyglot_piranha-0.3.3/src/models/rule_store.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/scopes.rs` & `polyglot_piranha-0.3.3/src/models/scopes.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/source_code_unit.rs` & `polyglot_piranha-0.3.3/src/models/source_code_unit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/unit_tests/piranha_arguments_test.rs` & `polyglot_piranha-0.3.3/src/models/unit_tests/piranha_arguments_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/unit_tests/rule_test.rs` & `polyglot_piranha-0.3.3/src/models/unit_tests/rule_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/unit_tests/scopes_test.rs` & `polyglot_piranha-0.3.3/src/models/unit_tests/scopes_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/models/unit_tests/source_code_unit_test.rs` & `polyglot_piranha-0.3.3/src/models/unit_tests/source_code_unit_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/tests/mod.rs` & `polyglot_piranha-0.3.3/src/tests/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 mod test_piranha_python;
 
 mod test_piranha_go;
 mod test_piranha_ts;
 mod test_piranha_tsx;
 
+mod test_piranha_thrift;
+
 use std::sync::Once;
 
 static INIT: Once = Once::new();
 
 fn initialize() {
   INIT.call_once(|| {
     env_logger::init();
```

### Comparing `polyglot_piranha-0.3.2/src/tests/test_piranha_go.rs` & `polyglot_piranha-0.3.3/src/tests/test_piranha_go.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/tests/test_piranha_java.rs` & `polyglot_piranha-0.3.3/src/tests/test_piranha_java.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/tests/test_piranha_kt.rs` & `polyglot_piranha-0.3.3/src/tests/test_piranha_kt.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/tests/test_piranha_python.rs` & `polyglot_piranha-0.3.3/src/tests/test_piranha_python.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/tests/test_piranha_swift.rs` & `polyglot_piranha-0.3.3/src/tests/test_piranha_swift.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/tests/test_piranha_ts.rs` & `polyglot_piranha-0.3.3/src/tests/test_piranha_ts.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/tests/test_piranha_tsx.rs` & `polyglot_piranha-0.3.3/src/tests/test_piranha_tsx.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/utilities/mod.rs` & `polyglot_piranha-0.3.3/src/utilities/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/utilities/tree_sitter_utilities.rs` & `polyglot_piranha-0.3.3/src/utilities/tree_sitter_utilities.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/utilities/unit_tests/tree_sitter_utilities_test.rs` & `polyglot_piranha-0.3.3/src/utilities/unit_tests/tree_sitter_utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/src/utilities/unit_tests/utilities_test.rs` & `polyglot_piranha-0.3.3/src/utilities/unit_tests/utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.2/PKG-INFO` & `polyglot_piranha-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyglot_piranha
-Version: 0.3.2
+Version: 0.3.3
 License-File: LICENSE
 License-File: LICENSE
 License-File: NOTICE
 Summary: Polyglot Piranha is a library for performing structural find and replace with deep cleanup.
 Keywords: refactoring,code update,structural find-replace,structural search and replace,structural search
 Author: Uber Technologies Inc.
 Author-email: Ameya Ketkar <ketkara@uber.com>, Lazaro Clapp <lazaro@uber.com>
```

