# Comparing `tmp/semantic_kernel-0.2.3.dev0.tar.gz` & `tmp/semantic_kernel-0.2.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.2.3.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.2.4.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.2.3.dev0.tar` & `semantic_kernel-0.2.4.dev0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0      663 2023-04-17 21:24:30.416680 semantic_kernel-0.2.3.dev0/pyproject.toml
--rw-r--r--   0        0        0     4569 2023-04-17 21:24:30.414681 semantic_kernel-0.2.3.dev0/README.md
--rw-r--r--   0        0        0     1302 2023-04-17 21:24:30.417680 semantic_kernel-0.2.3.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-17 21:24:30.418680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/ai_exception.py
--rw-r--r--   0        0        0      495 2023-04-17 21:24:30.418680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-17 21:24:30.418680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-17 21:24:30.419680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-17 21:24:30.419680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      479 2023-04-17 21:24:30.420680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/embeddings/embedding_index_base.py
--rw-r--r--   0        0        0      817 2023-04-17 21:24:30.420680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2771 2023-04-17 21:24:30.421681 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2763 2023-04-17 21:24:30.422187 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2758 2023-04-17 21:24:30.422187 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     4007 2023-04-17 21:24:30.423196 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     4441 2023-04-17 21:24:30.424202 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2427 2023-04-17 21:24:30.424202 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      476 2023-04-17 21:24:30.425203 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      383 2023-04-17 21:24:30.425203 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-17 21:24:30.426203 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     4641 2023-04-17 21:24:30.427205 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-17 21:24:30.428205 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     5613 2023-04-17 21:24:30.428205 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    11351 2023-04-17 21:24:30.429204 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     2342 2023-04-17 21:24:30.429204 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_base.py
--rw-r--r--   0        0        0     9134 2023-04-17 21:24:30.430322 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_config.py
--rw-r--r--   0        0        0     1626 2023-04-17 21:24:30.430322 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      710 2023-04-17 21:24:30.431831 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-17 21:24:30.432872 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
--rw-r--r--   0        0        0     2374 2023-04-17 21:24:30.432872 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/import_skills.py
--rw-r--r--   0        0        0     2323 2023-04-17 21:24:30.433873 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/inline_definition.py
--rw-r--r--   0        0        0     1531 2023-04-17 21:24:30.433873 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
--rw-r--r--   0        0        0      160 2023-04-17 21:24:30.434874 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-17 21:24:30.435885 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     1598 2023-04-17 21:24:30.435885 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0      299 2023-04-17 21:24:30.437008 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-17 21:24:30.437008 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     2499 2023-04-17 21:24:30.437008 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1237 2023-04-17 21:24:30.438370 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0      836 2023-04-17 21:24:30.438370 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/data_entry.py
--rw-r--r--   0        0        0      953 2023-04-17 21:24:30.438370 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/data_store_base.py
--rw-r--r--   0        0        0     1989 2023-04-17 21:24:30.438370 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/volatile_data_store.py
--rw-r--r--   0        0        0     4050 2023-04-17 21:24:30.439653 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2328 2023-04-17 21:24:30.439653 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-17 21:24:30.439653 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     8966 2023-04-17 21:24:30.440988 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-17 21:24:30.440988 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-17 21:24:30.440988 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    16307 2023-04-17 21:24:30.441995 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6960 2023-04-17 21:24:30.441995 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      919 2023-04-17 21:24:30.443431 semantic_kernel-0.2.3.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      673 2023-04-17 21:24:30.443431 semantic_kernel-0.2.3.dev0/semantic_kernel/reliability/retry_mechanism.py
--rw-r--r--   0        0        0     2101 2023-04-17 21:24:30.444515 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-17 21:24:30.445527 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-17 21:24:30.445527 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4269 2023-04-17 21:24:30.446537 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-17 21:24:30.446537 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-17 21:24:30.447927 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-17 21:24:30.447927 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-17 21:24:30.448939 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-17 21:24:30.448939 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-17 21:24:30.449936 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-17 21:24:30.449936 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-17 21:24:30.451019 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-17 21:24:30.451526 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-17 21:24:30.451526 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-17 21:24:30.452719 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0      830 2023-04-17 21:24:30.453727 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-17 21:24:30.453727 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4566 2023-04-17 21:24:30.454753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-17 21:24:30.455752 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-17 21:24:30.455752 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-17 21:24:30.456753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-17 21:24:30.456753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-17 21:24:30.457753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-17 21:24:30.457753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-17 21:24:30.458753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-17 21:24:30.458753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-17 21:24:30.459752 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-17 21:24:30.459752 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     1115 2023-04-17 21:24:30.452719 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0     7637 2023-04-17 21:24:30.460755 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      403 2023-04-17 21:24:30.460755 semantic_kernel-0.2.3.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-17 21:24:30.461753 semantic_kernel-0.2.3.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-17 21:24:30.461753 semantic_kernel-0.2.3.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-17 21:24:30.462995 semantic_kernel-0.2.3.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 semantic_kernel-0.2.3.dev0/PKG-INFO
+-rw-r--r--   0        0        0     4562 2023-04-19 21:51:48.404232 semantic_kernel-0.2.4.dev0/README.md
+-rw-r--r--   0        0        0      644 2023-04-24 18:00:09.400940 semantic_kernel-0.2.4.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1302 2023-04-19 06:06:19.926015 semantic_kernel-0.2.4.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-14 03:36:09.230039 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/ai_exception.py
+-rw-r--r--   0        0        0      495 2023-04-14 03:36:09.230576 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-14 03:36:09.231022 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-14 03:36:09.231429 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-14 03:36:09.232144 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      479 2023-04-14 03:36:09.232562 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/embeddings/embedding_index_base.py
+-rw-r--r--   0        0        0      817 2023-04-14 03:36:09.232970 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2771 2023-04-14 03:36:09.233875 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2763 2023-04-14 03:36:09.234689 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2758 2023-04-14 03:36:09.235471 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     4007 2023-04-14 03:36:09.236270 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     4441 2023-04-14 03:36:09.236952 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2427 2023-04-14 03:36:09.237661 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      476 2023-04-14 03:36:09.238119 semantic_kernel-0.2.4.dev0/semantic_kernel/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      457 2023-04-21 23:16:53.100030 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-14 03:36:09.239029 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-21 23:16:53.100412 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 03:36:09.239829 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-14 03:36:09.240512 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     5613 2023-04-14 03:36:09.240911 semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    12421 2023-04-21 23:16:53.101120 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     2240 2023-04-20 17:10:26.993745 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_base.py
+-rw-r--r--   0        0        0     9134 2023-04-14 03:36:09.243870 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_config.py
+-rw-r--r--   0        0        0     1626 2023-04-14 03:36:09.244661 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      710 2023-04-14 03:36:09.245082 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-14 03:36:09.245483 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
+-rw-r--r--   0        0        0     3826 2023-04-21 23:16:53.101795 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/import_skills.py
+-rw-r--r--   0        0        0     2323 2023-04-14 03:36:09.246857 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/inline_definition.py
+-rw-r--r--   0        0        0     1531 2023-04-14 03:36:09.247527 semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
+-rw-r--r--   0        0        0      160 2023-04-14 03:36:09.247903 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     1174 2023-04-14 03:36:09.248433 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     1598 2023-04-14 03:36:09.248824 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0      299 2023-04-14 03:36:09.249224 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-14 03:36:09.249612 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     2499 2023-04-14 03:36:09.250068 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1237 2023-04-14 03:36:09.250457 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0      836 2023-04-14 03:36:09.250950 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/storage/data_entry.py
+-rw-r--r--   0        0        0      953 2023-04-14 03:36:09.251369 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/storage/data_store_base.py
+-rw-r--r--   0        0        0     1989 2023-04-14 03:36:09.251740 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/storage/volatile_data_store.py
+-rw-r--r--   0        0        0     4050 2023-04-14 03:36:09.252125 semantic_kernel-0.2.4.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-20 17:10:26.995186 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 03:36:09.253302 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     8966 2023-04-14 03:36:09.253662 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-14 03:36:09.254004 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 03:36:09.254344 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    15963 2023-04-24 01:56:59.028969 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6164 2023-04-24 01:56:59.029417 semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      919 2023-04-14 03:36:09.255908 semantic_kernel-0.2.4.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      673 2023-04-14 03:36:09.256522 semantic_kernel-0.2.4.dev0/semantic_kernel/reliability/retry_mechanism.py
+-rw-r--r--   0        0        0     2101 2023-04-14 03:36:09.256949 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 03:36:09.257319 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-14 03:36:09.257703 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4269 2023-04-14 03:36:09.258212 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 03:36:09.258593 semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 03:36:09.259027 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 03:36:09.259911 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-14 03:36:09.260336 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 03:36:09.261065 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 03:36:09.261495 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 03:36:09.261836 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-14 03:36:09.262309 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 03:36:09.262723 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 03:36:09.263484 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-14 03:36:09.263900 semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-14 03:36:09.264367 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 03:36:09.264992 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 03:36:09.265522 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-24 01:56:59.029930 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-14 03:36:09.267164 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-14 03:36:09.267627 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 03:36:09.268042 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-14 03:36:09.268607 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 03:36:09.269045 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-14 03:36:09.269480 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 03:36:09.269880 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-14 03:36:09.270280 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-14 03:36:09.270855 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-14 03:36:09.271313 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-14 03:36:09.271775 semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      403 2023-04-14 03:36:09.272351 semantic_kernel-0.2.4.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-14 03:36:09.272775 semantic_kernel-0.2.4.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-14 03:36:09.273176 semantic_kernel-0.2.4.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-14 03:36:09.274119 semantic_kernel-0.2.4.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5136 1970-01-01 00:00:00.000000 semantic_kernel-0.2.4.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.2.3.dev0/README.md` & `semantic_kernel-0.2.4.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 Give me the TLDR in exactly 5 words.""")
 
 # Run your prompt
 print(prompt()) # => Robots must not harm humans.
 ```
 
-# Prompts are **semantic functions** with input parameters
+# **Semantic functions** are Prompts with input parameters
 
 ```python
 # Create a reusable function with one input parameter
 summarize = kernel.create_semantic_function("{{$input}}\n\nOne line TLDR with the fewest words.")
 
 # Summarize the laws of thermodynamics
 print(summarize("""
@@ -95,18 +95,18 @@
 * [Getting started with Semantic Kernel](../samples/notebooks/python/00-getting-started.ipynb)
 * [Loading and configuring Semantic Kernel](../samples/notebooks/python/01-basic-loading-the-kernel.ipynb)
 * [Running AI prompts from file](../samples/notebooks/python/02-running-prompts-from-file.ipynb)
 * [Creating Semantic Functions at runtime (i.e. inline functions)](../samples/notebooks/python/03-semantic-function-inline.ipynb)
 * [Using Context Variables to Build a Chat Experience](../samples/notebooks/python/04-context-variables-chat.ipynb)
 * [Building Memory with Embeddings](../samples/notebooks/python/06-memory-and-embeddings.ipynb)
 
-# Frequently asked questions
+# SK Frequently Asked Questions
 
-* How does Python SK compare to the C# version of Semantic Kernel?
+## How does Python SK compare to the C# version of Semantic Kernel?
 
-  The two SDKs are compatible and at the core they follow the same design principles.
-  Some features are still available only in the C# version, and being ported
-  Refer to the [FEATURE PARITY](FEATURE_PARITY.md) doc to see where
-  things stand in matching the features and functionality of the main SK branch.
-  Over time there will be some features available only in the Python version, and
-  others only in the C# version, for example adapters to external services,
-  scientific libraries, etc.
+The two SDKs are compatible and at the core they follow the same design principles.
+Some features are still available only in the C# version, and being ported
+Refer to the [FEATURE MATRIX](../FEATURE_MATRIX.md) doc to see where
+things stand in matching the features and functionality of the main SK branch.
+Over time there will be some features available only in the Python version, and
+others only in the C# version, for example adapters to external services,
+scientific libraries, etc.
```

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/ai_exception.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/chat_request_settings.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/complete_request_settings.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/__init__.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,29 +102,53 @@
         function = self._create_semantic_function(
             skill_name, function_name, function_config
         )
         self._skill_collection.add_semantic_function(function)
 
         return function
 
-    async def run_async(self, *functions: Any) -> SKContext:
-        return await self.run_on_vars_async(ContextVariables(), *functions)
+    async def run_async(
+        self,
+        *functions: Any,
+        input_context: Optional[SKContext] = None,
+        input_vars: Optional[ContextVariables] = None,
+        input_str: Optional[str] = None,
+    ) -> SKContext:
+        # if the user passed in a context, prioritize it, but merge with any other inputs
+        if input_context is not None:
+            context = input_context
+            if input_vars is not None:
+                context._variables = input_vars.merge_or_overwrite(
+                    new_vars=context._variables, overwrite=False
+                )
 
-    async def run_on_str_async(self, input_str: str, *functions: Any) -> SKContext:
-        return await self.run_on_vars_async(ContextVariables(input_str), *functions)
+            if input_str is not None:
+                context._variables = ContextVariables(input_str).merge_or_overwrite(
+                    new_vars=context._variables, overwrite=False
+                )
 
-    async def run_on_vars_async(
-        self, input_vars: ContextVariables, *functions: Any
-    ) -> SKContext:
-        context = SKContext(
-            input_vars,
-            self._memory,
-            self._skill_collection.read_only_skill_collection,
-            self._log,
-        )
+        # if the user did not pass in a context, prioritize an input string, and merge that with input context variables
+        else:
+            if input_str is not None and input_vars is None:
+                variables = ContextVariables(input_str)
+            elif input_str is None and input_vars is not None:
+                variables = input_vars
+            elif input_str is not None and input_vars is not None:
+                variables = ContextVariables(input_str)
+                variables = variables.merge_or_overwrite(
+                    new_vars=input_vars, overwrite=False
+                )
+            else:
+                variables = ContextVariables()
+            context = SKContext(
+                variables,
+                self._memory,
+                self._skill_collection.read_only_skill_collection,
+                self._log,
+            )
 
         pipeline_step = 0
         for func in functions:
             assert isinstance(func, SKFunctionBase), (
                 "All func arguments to Kernel.run*(inputs, func1, func2, ...) "
                 "must be SKFunctionBase instances"
             )
```

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_base.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,27 +62,23 @@
         pass
 
     @abstractmethod
     def register_memory(self, memory: SemanticTextMemoryBase) -> None:
         pass
 
     @abstractmethod
-    async def run_on_str_async(self, input_str: str, *args: Any) -> SKContext:
-        pass
-
-    @abstractmethod
-    async def run_on_vars_async(
-        self, input_vars: ContextVariables, *args: Any
+    async def run_async(
+        self,
+        *functions: Any,
+        input_context: Optional[SKContext],
+        input_vars: Optional[ContextVariables],
+        input_str: Optional[str]
     ) -> SKContext:
         pass
 
     @abstractmethod
-    async def run_async(self, *args: Any) -> SKContext:
-        pass
-
-    @abstractmethod
     def func(self, skill_name: str, function_name: str) -> SKFunctionBase:
         pass
 
     @abstractmethod
     def create_new_context(self) -> SKContext:
         pass
```

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_config.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/__init__.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/inline_definition.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/inline_definition.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/memory_configuration.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/kernel_extensions/memory_configuration.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/data_entry.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/storage/data_entry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/data_store_base.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/storage/data_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/volatile_data_store.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/storage/volatile_data_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,20 +21,20 @@
         return self._variables[self._main_key]
 
     def update(self, content: str) -> "ContextVariables":
         self._variables[self._main_key] = content
         return self
 
     def merge_or_overwrite(
-        self, new_context: "ContextVariables", merge: bool = True
+        self, new_vars: "ContextVariables", overwrite: bool = False
     ) -> "ContextVariables":
-        if not merge:
-            self._variables = {}
-
-        self._variables.update(new_context._variables)
+        if overwrite:
+            self._variables = new_vars._variables
+        else:
+            self._variables.update(new_vars._variables)
         return self
 
     def set(self, name: str, value: str) -> "ContextVariables":
         if not name:
             raise ValueError("The variable name cannot be `None` or empty")
         name = name.lower()
```

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,28 +32,14 @@
 
 
 class SKFunction(SKFunctionBase):
     """
     Semantic Kernel function.
     """
 
-    class RunThread(threading.Thread):
-        """
-        Async code wrapper to allow running async code inside external
-        event loops such as Jupyter notebooks.
-        """
-
-        def __init__(self, code):
-            self.code = code
-            self.result = None
-            super().__init__()
-
-        def run(self):
-            self.result = asyncio.run(self.code)
-
     _parameters: List[ParameterView]
     _delegate_type: DelegateTypes
     _function: Callable[..., Any]
     _skill_collection: Optional[ReadOnlySkillCollectionBase]
     _log: Logger
     _ai_backend: Optional[TextCompletionClientBase]
     _ai_request_settings: CompleteRequestSettings
@@ -259,132 +245,113 @@
             is_semantic=self.is_semantic,
             parameters=self._parameters,
         )
 
     def __call__(
         self,
         input: Optional[str] = None,
+        variables: ContextVariables = None,
         context: Optional[SKContext] = None,
+        memory: Optional[SemanticTextMemoryBase] = None,
         settings: Optional[CompleteRequestSettings] = None,
         log: Optional[Logger] = None,
     ) -> SKContext:
-        return self.invoke(input=input, context=context, settings=settings, log=log)
+        return self.invoke(
+            input=input,
+            variables=variables,
+            context=context,
+            memory=memory,
+            settings=settings,
+            log=log,
+        )
 
     def invoke(
         self,
         input: Optional[str] = None,
+        variables: ContextVariables = None,
         context: Optional[SKContext] = None,
+        memory: Optional[SemanticTextMemoryBase] = None,
         settings: Optional[CompleteRequestSettings] = None,
         log: Optional[Logger] = None,
     ) -> SKContext:
         if context is None:
-            if self._skill_collection is None:
-                raise ValueError("Skill collection cannot be `None`")
-            assert self._skill_collection is not None
-
             context = SKContext(
-                ContextVariables(""),
-                NullMemory.instance,  # type: ignore
-                self._skill_collection,
-                log if log is not None else self._log,
+                variables=ContextVariables("") if variables is None else variables,
+                skill_collection=self._skill_collection,
+                memory=memory if memory is not None else NullMemory.instance,
+                logger=log if log is not None else self._log,
                 # TODO: ctoken?
             )
+        else:
+            # If context is passed, we need to merge the variables
+            if variables is not None:
+                context._variables = variables.merge_or_overwrite(
+                    new_vars=context._variables, overwrite=False
+                )
+            if memory is not None:
+                context._memory = memory
 
         if input is not None:
             context.variables.update(input)
 
         # Check if there is an event loop
         try:
             loop = asyncio.get_running_loop()
         except RuntimeError:
             loop = None
 
         # Handle "asyncio.run() cannot be called from a running event loop"
         if loop and loop.is_running():
             if self.is_semantic:
-                thread = self.RunThread(self._invoke_semantic_async(context, settings))
-                thread.start()
-                thread.join()
-                return thread.result
+                return self._runThread(self._invoke_semantic_async(context, settings))
             else:
-                thread = self.RunThread(self._invoke_native_async(context))
-                thread.start()
-                thread.join()
-                return thread.result
+                return self._runThread(self._invoke_semantic_async(context))
         else:
             if self.is_semantic:
                 return asyncio.run(self._invoke_semantic_async(context, settings))
             else:
                 return asyncio.run(self._invoke_native_async(context))
 
     async def invoke_async(
         self,
         input: Optional[str] = None,
+        variables: ContextVariables = None,
         context: Optional[SKContext] = None,
+        memory: Optional[SemanticTextMemoryBase] = None,
         settings: Optional[CompleteRequestSettings] = None,
         log: Optional[Logger] = None,
     ) -> SKContext:
         if context is None:
-            if self._skill_collection is None:
-                raise ValueError("Skill collection cannot be `None`")
-            assert self._skill_collection is not None
-
             context = SKContext(
-                ContextVariables(""),
-                NullMemory.instance,  # type: ignore
-                self._skill_collection,
-                log if log is not None else self._log,
+                variables=ContextVariables("") if variables is None else variables,
+                skill_collection=self._skill_collection,
+                memory=memory if memory is not None else NullMemory.instance,
+                logger=log if log is not None else self._log,
                 # TODO: ctoken?
             )
+        else:
+            # If context is passed, we need to merge the variables
+            if variables is not None:
+                context._variables = variables.merge_or_overwrite(
+                    new_vars=context._variables, overwrite=False
+                )
+            if memory is not None:
+                context._memory = memory
 
         if input is not None:
             context.variables.update(input)
 
-        if self.is_semantic:
-            return await self._invoke_semantic_async(context, settings)
-        else:
-            return await self._invoke_native_async(context)
-
-    def invoke_with_vars(
-        self,
-        input: ContextVariables,
-        memory: Optional[SemanticTextMemoryBase] = None,
-        log: Optional[Logger] = None,
-    ) -> SKContext:
-        tmp_context = SKContext(
-            variables=input,
-            skill_collection=self._skill_collection,
-            memory=memory if memory is not None else NullMemory.instance,
-            logger=log if log is not None else self._log,
-        )
-
         try:
-            return self.invoke(input=None, context=tmp_context, log=log)
-        except Exception as e:
-            tmp_context.fail(str(e), e)
-            return tmp_context
-
-    async def invoke_with_vars_async(
-        self,
-        input: ContextVariables,
-        memory: Optional[SemanticTextMemoryBase] = None,
-        log: Optional[Logger] = None,
-    ) -> SKContext:
-        tmp_context = SKContext(
-            variables=input,
-            skill_collection=self._skill_collection,
-            memory=memory if memory is not None else NullMemory.instance,
-            logger=log if log is not None else self._log,
-        )
-
-        try:
-            return await self.invoke_async(input=None, context=tmp_context, log=log)
+            if self.is_semantic:
+                return await self._invoke_semantic_async(context, settings)
+            else:
+                return await self._invoke_native_async(context)
         except Exception as e:
-            tmp_context.fail(str(e), e)
-            return tmp_context
+            context.fail(str(e), e)
+            return context
 
     async def _invoke_semantic_async(self, context, settings):
         self._verify_is_semantic()
 
         self._ensure_context_has_skills(context)
 
         if settings is None:
@@ -442,7 +409,22 @@
         if context.skills is not None:
             return
 
         context.skills = self._skill_collection
 
     def _trace_function_type_Call(self, type: Enum, log: Logger) -> None:
         log.debug(f"Executing function type {type}: {type.name}")
+
+    """
+    Async code wrapper to allow running async code inside external
+    event loops such as Jupyter notebooks.
+    """
+
+    def _runThread(self, code: Callable):
+        result = []
+        thread = threading.Thread(target=self._runCode, args=(code, result))
+        thread.start()
+        thread.join()
+        return result[0]
+
+    def _runCode(self, code: Callable, result: List[Any]) -> None:
+        result.append(asyncio.run(code))
```

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,94 +94,56 @@
         """
         pass
 
     @abstractmethod
     def invoke(
         self,
         input: Optional[str] = None,
+        variables: ContextVariables = None,
         context: Optional[SKContext] = None,
+        memory: Optional[SemanticTextMemoryBase] = None,
         settings: Optional[CompleteRequestSettings] = None,
-        log: Optional[Logger] = None
+        log: Optional[Logger] = None,
         # TODO: ctoken
     ) -> SKContext:
         """
         Invokes the function with an explicit string input
-
         Keyword Arguments:
             input {str} -- The explicit string input (default: {None})
+            variables {ContextVariables} -- The custom input
             context {SKContext} -- The context to use
+            memory: {SemanticTextMemoryBase} -- The memory to use
             settings {CompleteRequestSettings} -- LLM completion settings
             log {Logger} -- Application logger
-
         Returns:
             SKContext -- The updated context, potentially a new one if
             context switching is implemented.
         """
         pass
 
     @abstractmethod
     async def invoke_async(
         self,
         input: Optional[str] = None,
+        variables: ContextVariables = None,
         context: Optional[SKContext] = None,
+        memory: Optional[SemanticTextMemoryBase] = None,
         settings: Optional[CompleteRequestSettings] = None,
-        log: Optional[Logger] = None
+        log: Optional[Logger] = None,
         # TODO: ctoken
     ) -> SKContext:
         """
         Invokes the function with an explicit string input
-
         Keyword Arguments:
             input {str} -- The explicit string input (default: {None})
+            variables {ContextVariables} -- The custom input
             context {SKContext} -- The context to use
+            memory: {SemanticTextMemoryBase} -- The memory to use
             settings {CompleteRequestSettings} -- LLM completion settings
             log {Logger} -- Application logger
-
-        Returns:
-            SKContext -- The updated context, potentially a new one if
-            context switching is implemented.
-        """
-        pass
-
-    @abstractmethod
-    def invoke_with_vars(
-        self,
-        input: ContextVariables,
-        memory: Optional[SemanticTextMemoryBase] = None,
-        log: Optional[Logger] = None,
-    ) -> SKContext:
-        """
-        Invokes the function with a custom input
-
-        Arguments:
-            input {ContextVariables} -- The custom input
-            memory {SemanticTextMemoryBase} -- The memory to use
-            log {Logger} -- Application logger
-
-        Returns:
-            SKContext -- The updated context, potentially a new one if
-            context switching is implemented.
-        """
-        pass
-
-    @abstractmethod
-    async def invoke_with_vars_async(
-        self,
-        input: ContextVariables,
-        memory: Optional[SemanticTextMemoryBase] = None,
-        log: Optional[Logger] = None,
-    ) -> SKContext:
-        """
-        Invokes the function with a custom input
-
-        Arguments:
-            input {ContextVariables} -- The custom input
-            memory {SemanticTextMemoryBase} -- The memory to use
-            log {Logger} -- Application logger
-
         Returns:
             SKContext -- The updated context, potentially a new one if
             context switching is implemented.
         """
         pass
 
     @abstractmethod
```

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/reliability/retry_mechanism.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/reliability/retry_mechanism.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         variables_clone = context.variables.clone()
 
         if len(self._tokens) > 1:
             self.log.debug(f"Passing variable/value: `{self._tokens[1].content}`")
             input_value = self._tokens[1].render(variables_clone)
             variables_clone.update(input_value)
 
-        result = await function.invoke_with_vars_async(
-            variables_clone, context.memory, self.log
+        result = await function.invoke_async(
+            variables=variables_clone, memory=context.memory, log=self.log
         )
 
         if result.error_occurred:
             error_msg = (
                 f"Function `{f_block.content}` execution failed. "
                 f"{result.last_exception.__class__.__name__}: "
                 f"{result.last_error_description}"
```

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.2.4.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.3.dev0/PKG-INFO` & `semantic_kernel-0.2.4.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.2.3.dev0
+Version: 0.2.4.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
-Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Description-Content-Type: text/markdown
 
 # Get Started with Semantic Kernel ⚡
 
 Install the latest package:
@@ -70,15 +69,15 @@
 
 Give me the TLDR in exactly 5 words.""")
 
 # Run your prompt
 print(prompt()) # => Robots must not harm humans.
 ```
 
-# Prompts are **semantic functions** with input parameters
+# **Semantic functions** are Prompts with input parameters
 
 ```python
 # Create a reusable function with one input parameter
 summarize = kernel.create_semantic_function("{{$input}}\n\nOne line TLDR with the fewest words.")
 
 # Summarize the laws of thermodynamics
 print(summarize("""
@@ -113,19 +112,19 @@
 * [Getting started with Semantic Kernel](../samples/notebooks/python/00-getting-started.ipynb)
 * [Loading and configuring Semantic Kernel](../samples/notebooks/python/01-basic-loading-the-kernel.ipynb)
 * [Running AI prompts from file](../samples/notebooks/python/02-running-prompts-from-file.ipynb)
 * [Creating Semantic Functions at runtime (i.e. inline functions)](../samples/notebooks/python/03-semantic-function-inline.ipynb)
 * [Using Context Variables to Build a Chat Experience](../samples/notebooks/python/04-context-variables-chat.ipynb)
 * [Building Memory with Embeddings](../samples/notebooks/python/06-memory-and-embeddings.ipynb)
 
-# Frequently asked questions
+# SK Frequently Asked Questions
 
-* How does Python SK compare to the C# version of Semantic Kernel?
+## How does Python SK compare to the C# version of Semantic Kernel?
 
-  The two SDKs are compatible and at the core they follow the same design principles.
-  Some features are still available only in the C# version, and being ported
-  Refer to the [FEATURE PARITY](FEATURE_PARITY.md) doc to see where
-  things stand in matching the features and functionality of the main SK branch.
-  Over time there will be some features available only in the Python version, and
-  others only in the C# version, for example adapters to external services,
-  scientific libraries, etc.
+The two SDKs are compatible and at the core they follow the same design principles.
+Some features are still available only in the C# version, and being ported
+Refer to the [FEATURE MATRIX](../FEATURE_MATRIX.md) doc to see where
+things stand in matching the features and functionality of the main SK branch.
+Over time there will be some features available only in the Python version, and
+others only in the C# version, for example adapters to external services,
+scientific libraries, etc.
```

