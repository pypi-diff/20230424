# Comparing `tmp/cosmosis-2.3.2.tar.gz` & `tmp/cosmosis-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmosis-2.3.2.tar", last modified: Mon Mar 27 11:19:07 2023, max compression
+gzip compressed data, was "cosmosis-2.4.1.tar", last modified: Mon Apr 24 13:28:36 2023, max compression
```

## Comparing `cosmosis-2.3.2.tar` & `cosmosis-2.4.1.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.482648 cosmosis-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-27 11:19:05.000000 cosmosis-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-03-27 11:19:05.000000 cosmosis-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-27 11:19:07.482648 cosmosis-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-27 11:19:05.000000 cosmosis-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.454648 cosmosis-2.3.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-03-27 11:19:05.000000 cosmosis-2.3.2/bin/cosmosis
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-03-27 11:19:05.000000 cosmosis-2.3.2/bin/cosmosis-configure
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-03-27 11:19:05.000000 cosmosis-2.3.2/bin/cosmosis-extract
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-03-27 11:19:05.000000 cosmosis-2.3.2/bin/cosmosis-postprocess
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-03-27 11:19:05.000000 cosmosis-2.3.2/bin/cosmosis-sample-fisher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.458648 cosmosis-2.3.2/cosmosis/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.458648 cosmosis-2.3.2/cosmosis/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/config/compilers.mk
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/config/subdirs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.458648 cosmosis-2.3.2/cosmosis/datablock/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/c_datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/c_datablock.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/clamp.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_constants.fh
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_modules.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.458648 cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/dbt_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/section_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_section_names.F90
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_types.F90
--rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/cosmosis_wrappers.F90
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/datablock.hh
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/datablock_logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/datablock_logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/datablock_status.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/datablock_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/entry.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/entry.hh
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/generate_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/handler.c
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/ndarray.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/section.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/section.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/section_names.h
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/datablock/section_names.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/gaussian_likelihood.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17782 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.462648 cosmosis-2.3.2/cosmosis/output/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/output/cosmomc_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/output/fits_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/output/in_memory_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/output/null_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/output/output_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/output/text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.462648 cosmosis-2.3.2/cosmosis/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/plotting/chain_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/plotting/grid_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/plotting/kde.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/plotting/plot_demo_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/plotting/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/plotting/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6941 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.462648 cosmosis-2.3.2/cosmosis/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16163 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/cosmology_theory_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/latex.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/lazy_pylab.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41832 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/postprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)    33731 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/postprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.466648 cosmosis-2.3.2/cosmosis/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/declare.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.466648 cosmosis-2.3.2/cosmosis/runtime/julia_modules/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/julia_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/julia_modules/julia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/memmon.py
--rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    56629 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.466648 cosmosis-2.3.2/cosmosis/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.466648 cosmosis-2.3.2/cosmosis/samplers/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/abc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/abc/abc_sampler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/abc/abc_sampler_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/apriori/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/apriori/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2262 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/apriori/apriori_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/dynesty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/dynesty/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3600 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/dynesty/dynesty_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/emcee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/emcee/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7265 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/emcee/emcee_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/fisher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/fisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/fisher/fisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6726 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/fisher/fisher_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/grid/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4715 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/grid/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/gridmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/gridmax/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/gridmax/gridmax_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/importance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/importance/importance_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/kombine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/kombine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5406 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/kombine/kombine_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/list/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/list/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/list/list_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/maxlike/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/maxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4790 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/maxlike/maxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.470648 cosmosis-2.3.2/cosmosis/samplers/metropolis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/metropolis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/metropolis/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/metropolis/metropolis_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.474648 cosmosis-2.3.2/cosmosis/samplers/metropolis/proposal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/metropolis/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/metropolis/proposal/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.474648 cosmosis-2.3.2/cosmosis/samplers/minuit/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/minuit/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/minuit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7592 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/minuit/minuit_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/minuit/minuit_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.474648 cosmosis-2.3.2/cosmosis/samplers/multinest/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.474648 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/README
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
--rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
--rw-r--r--   0 runner    (1001) docker     (123)   106166 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/nested.f90
--rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/posterior.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/utils1.f90
--rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.474648 cosmosis-2.3.2/cosmosis/samplers/nautilus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/nautilus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/nautilus/nautilus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.474648 cosmosis-2.3.2/cosmosis/samplers/pmaxlike/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/pmaxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4537 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.474648 cosmosis-2.3.2/cosmosis/samplers/pmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/pmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/pmc/pmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/pmc/pmc_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.474648 cosmosis-2.3.2/cosmosis/samplers/poco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/poco/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/poco/poco_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.474648 cosmosis-2.3.2/cosmosis/samplers/polychord/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.478648 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/README
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/abort.F90
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/array_utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/calculate.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/clustering.f90
--rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/feedback.f90
--rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/generate.F90
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/ini.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/interfaces.F90
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/interfaces.h
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/params.f90
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/random_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/read_write.f90
--rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/settings.f90
--rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/utils.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.478648 cosmosis-2.3.2/cosmosis/samplers/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/pymc/pymc_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.478648 cosmosis-2.3.2/cosmosis/samplers/snake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/snake/snake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/snake/snake_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.478648 cosmosis-2.3.2/cosmosis/samplers/star/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/star/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/star/star_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.478648 cosmosis-2.3.2/cosmosis/samplers/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/test/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.478648 cosmosis-2.3.2/cosmosis/samplers/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/zeus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11516 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/samplers/zeus/zeus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.478648 cosmosis-2.3.2/cosmosis/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.482648 cosmosis-2.3.2/cosmosis/test/libtest/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/cosmosis_test.F90
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/cosmosis_tests.supp
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/datablock_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/entry_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/ndarray_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/section_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/test_c_datablock_scalars.h
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/libtest/test_c_datablock_scalars.template
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_module2.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_module3.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_module4.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_polychord.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 11:19:05.000000 cosmosis-2.3.2/cosmosis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:19:07.458648 cosmosis-2.3.2/cosmosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-27 11:19:07.000000 cosmosis-2.3.2/cosmosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-03-27 11:19:07.000000 cosmosis-2.3.2/cosmosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 11:19:07.000000 cosmosis-2.3.2/cosmosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-27 11:19:07.000000 cosmosis-2.3.2/cosmosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 11:19:07.000000 cosmosis-2.3.2/cosmosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-27 11:19:05.000000 cosmosis-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 11:19:07.482648 cosmosis-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-03-27 11:19:05.000000 cosmosis-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-24 13:28:34.000000 cosmosis-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-24 13:28:34.000000 cosmosis-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 13:28:36.600744 cosmosis-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 13:28:34.000000 cosmosis-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.580744 cosmosis-2.4.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis-configure
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis-extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis-postprocess
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis-sample-fisher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.580744 cosmosis-2.4.1/cosmosis/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.580744 cosmosis-2.4.1/cosmosis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/config/compilers.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/config/subdirs.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.584744 cosmosis-2.4.1/cosmosis/datablock/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/c_datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/c_datablock.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/clamp.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_constants.fh
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_modules.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.584744 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/dbt_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/section_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_section_names.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_types.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_wrappers.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock_logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock_logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/entry.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/entry.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/generate_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/ndarray.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/section.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/section.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/section_names.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/section_names.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/gaussian_likelihood.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17782 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.584744 cosmosis-2.4.1/cosmosis/output/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/cosmomc_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/fits_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/in_memory_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/null_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/output_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.584744 cosmosis-2.4.1/cosmosis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/chain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/grid_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/kde.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/plot_demo_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6941 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16163 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/cosmology_theory_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/latex.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/lazy_pylab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41832 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/postprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33731 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/runtime/julia_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/julia_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/julia_modules/julia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/memmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56629 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/abc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/abc/abc_sampler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/abc/abc_sampler_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/apriori/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/apriori/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2262 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/apriori/apriori_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/dynesty/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3600 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/dynesty/dynesty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/emcee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/emcee/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7265 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/emcee/emcee_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/fisher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/fisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/fisher/fisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6726 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/fisher/fisher_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/grid/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4715 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/grid/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/gridmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/gridmax/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/gridmax/gridmax_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/importance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/importance/importance_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/kombine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/kombine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5406 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/kombine/kombine_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/list/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/list/list_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/maxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/maxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4790 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/maxlike/maxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/metropolis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/metropolis_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/minuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/minuit/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/minuit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7592 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/minuit/minuit_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/minuit/minuit_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/multinest/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   106166 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/nested.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/posterior.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/utils1.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/nautilus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/nautilus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/nautilus/nautilus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/pmaxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmaxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4537 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/pmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmc/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmc/pmc_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/poco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/poco/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/poco/poco_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/polychord/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/abort.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/calculate.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/clustering.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/feedback.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/generate.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/ini.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/params.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/read_write.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/settings.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/utils.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pymc/pymc_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/snake/snake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/snake/snake_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/samplers/star/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/star/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/star/star_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/samplers/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/test/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/samplers/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/zeus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11516 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/zeus/zeus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/test/libtest/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/cosmosis_test.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/cosmosis_tests.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/datablock_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/entry_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/ndarray_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/section_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/test_c_datablock_scalars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/test_c_datablock_scalars.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_module2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_module3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_module4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_polychord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.580744 cosmosis-2.4.1/cosmosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 13:28:34.000000 cosmosis-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:28:36.600744 cosmosis-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-24 13:28:34.000000 cosmosis-2.4.1/setup.py
```

### Comparing `cosmosis-2.3.2/LICENSE` & `cosmosis-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/MANIFEST.in` & `cosmosis-2.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/bin/cosmosis-configure` & `cosmosis-2.4.1/bin/cosmosis-configure`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/bin/cosmosis-extract` & `cosmosis-2.4.1/bin/cosmosis-extract`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/bin/cosmosis-sample-fisher` & `cosmosis-2.4.1/bin/cosmosis-sample-fisher`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/__init__.py` & `cosmosis-2.4.1/cosmosis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/config/compilers.mk` & `cosmosis-2.4.1/cosmosis/config/compilers.mk`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/configure.py` & `cosmosis-2.4.1/cosmosis/configure.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/constants.py` & `cosmosis-2.4.1/cosmosis/constants.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/Makefile` & `cosmosis-2.4.1/cosmosis/datablock/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/c_datablock.cc` & `cosmosis-2.4.1/cosmosis/datablock/c_datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/c_datablock.h` & `cosmosis-2.4.1/cosmosis/datablock/c_datablock.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/clamp.hh` & `cosmosis-2.4.1/cosmosis/datablock/clamp.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/cosmosis_constants.fh` & `cosmosis-2.4.1/cosmosis/datablock/cosmosis_constants.fh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/cosmosis_constants.h` & `cosmosis-2.4.1/cosmosis/datablock/cosmosis_constants.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/cosmosis_modules.F90` & `cosmosis-2.4.1/cosmosis/datablock/cosmosis_modules.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/block.py` & `cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/errors.py` & `cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/errors.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/lib.py` & `cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/cosmosis_py/section_names.py` & `cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/section_names.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/cosmosis_section_names.F90` & `cosmosis-2.4.1/cosmosis/datablock/cosmosis_section_names.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/cosmosis_wrappers.F90` & `cosmosis-2.4.1/cosmosis/datablock/cosmosis_wrappers.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/datablock.cc` & `cosmosis-2.4.1/cosmosis/datablock/datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/datablock.hh` & `cosmosis-2.4.1/cosmosis/datablock/datablock.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/datablock_logging.cc` & `cosmosis-2.4.1/cosmosis/datablock/datablock_logging.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/datablock_logging.h` & `cosmosis-2.4.1/cosmosis/datablock/datablock_logging.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/datablock_status.h` & `cosmosis-2.4.1/cosmosis/datablock/datablock_status.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/entry.cc` & `cosmosis-2.4.1/cosmosis/datablock/entry.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/entry.hh` & `cosmosis-2.4.1/cosmosis/datablock/entry.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/generate_sections.py` & `cosmosis-2.4.1/cosmosis/datablock/generate_sections.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/handler.c` & `cosmosis-2.4.1/cosmosis/datablock/handler.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/ndarray.hh` & `cosmosis-2.4.1/cosmosis/datablock/ndarray.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/section.cc` & `cosmosis-2.4.1/cosmosis/datablock/section.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/section.hh` & `cosmosis-2.4.1/cosmosis/datablock/section.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/section_names.h` & `cosmosis-2.4.1/cosmosis/datablock/section_names.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/datablock/section_names.txt` & `cosmosis-2.4.1/cosmosis/datablock/section_names.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/gaussian_likelihood.py` & `cosmosis-2.4.1/cosmosis/gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/main.py` & `cosmosis-2.4.1/cosmosis/main.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/output/__init__.py` & `cosmosis-2.4.1/cosmosis/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/output/cosmomc_output.py` & `cosmosis-2.4.1/cosmosis/output/cosmomc_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/output/fits_output.py` & `cosmosis-2.4.1/cosmosis/output/fits_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/output/in_memory_output.py` & `cosmosis-2.4.1/cosmosis/output/in_memory_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/output/null_output.py` & `cosmosis-2.4.1/cosmosis/output/null_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/output/output_base.py` & `cosmosis-2.4.1/cosmosis/output/output_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/output/text_output.py` & `cosmosis-2.4.1/cosmosis/output/text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/output/utils.py` & `cosmosis-2.4.1/cosmosis/output/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/plotting/chain_plots.py` & `cosmosis-2.4.1/cosmosis/plotting/chain_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/plotting/grid_plots.py` & `cosmosis-2.4.1/cosmosis/plotting/grid_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/plotting/kde.py` & `cosmosis-2.4.1/cosmosis/plotting/kde.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/plotting/plotter.py` & `cosmosis-2.4.1/cosmosis/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocess.py` & `cosmosis-2.4.1/cosmosis/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/__init__.py` & `cosmosis-2.4.1/cosmosis/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/cosmology_theory_plots.py` & `cosmosis-2.4.1/cosmosis/postprocessing/cosmology_theory_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/density.py` & `cosmosis-2.4.1/cosmosis/postprocessing/density.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/elements.py` & `cosmosis-2.4.1/cosmosis/postprocessing/elements.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/inputs.py` & `cosmosis-2.4.1/cosmosis/postprocessing/inputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/latex.ini` & `cosmosis-2.4.1/cosmosis/postprocessing/latex.ini`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/lazy_pylab.py` & `cosmosis-2.4.1/cosmosis/postprocessing/lazy_pylab.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/outputs.py` & `cosmosis-2.4.1/cosmosis/postprocessing/outputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/plots.py` & `cosmosis-2.4.1/cosmosis/postprocessing/plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/postprocess.py` & `cosmosis-2.4.1/cosmosis/postprocessing/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/postprocess_base.py` & `cosmosis-2.4.1/cosmosis/postprocessing/postprocess_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/reruns.py` & `cosmosis-2.4.1/cosmosis/postprocessing/reruns.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/statistics.py` & `cosmosis-2.4.1/cosmosis/postprocessing/statistics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/postprocessing/utils.py` & `cosmosis-2.4.1/cosmosis/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/analytics.py` & `cosmosis-2.4.1/cosmosis/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/attribution.py` & `cosmosis-2.4.1/cosmosis/runtime/attribution.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/config.py` & `cosmosis-2.4.1/cosmosis/runtime/config.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/declare.py` & `cosmosis-2.4.1/cosmosis/runtime/declare.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/julia_modules/julia.py` & `cosmosis-2.4.1/cosmosis/runtime/julia_modules/julia.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/memmon.py` & `cosmosis-2.4.1/cosmosis/runtime/memmon.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/module.py` & `cosmosis-2.4.1/cosmosis/runtime/module.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/mpi_pool.py` & `cosmosis-2.4.1/cosmosis/runtime/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/parameter.py` & `cosmosis-2.4.1/cosmosis/runtime/parameter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/pipeline.py` & `cosmosis-2.4.1/cosmosis/runtime/pipeline.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/prior.py` & `cosmosis-2.4.1/cosmosis/runtime/prior.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/runtime/process_pool.py` & `cosmosis-2.4.1/cosmosis/runtime/process_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/__init__.py` & `cosmosis-2.4.1/cosmosis/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/abc/abc_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/abc/abc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/abc/abc_sampler_mpi.py` & `cosmosis-2.4.1/cosmosis/samplers/abc/abc_sampler_mpi.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/apriori/apriori_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/apriori/apriori_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/dynesty/dynesty_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/dynesty/dynesty_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/emcee/emcee_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/emcee/emcee_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/fisher/fisher.py` & `cosmosis-2.4.1/cosmosis/samplers/fisher/fisher.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/fisher/fisher_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/fisher/fisher_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/grid/grid_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/grid/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/gridmax/gridmax_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/gridmax/gridmax_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/hints.py` & `cosmosis-2.4.1/cosmosis/samplers/hints.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/importance/importance_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/importance/importance_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/kombine/kombine_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/kombine/kombine_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/list/list_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/list/list_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/maxlike/maxlike_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/maxlike/maxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/metropolis/metropolis.py` & `cosmosis-2.4.1/cosmosis/samplers/metropolis/metropolis.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/metropolis/metropolis_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/metropolis/metropolis_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py` & `cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/metropolis/proposal/standard.py` & `cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/standard.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/minuit/Makefile` & `cosmosis-2.4.1/cosmosis/samplers/minuit/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/minuit/minuit_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/minuit/minuit_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/minuit/minuit_wrapper.cpp` & `cosmosis-2.4.1/cosmosis/samplers/minuit/minuit_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/LICENCE` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/Makefile` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/README` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/cwrapper.f90` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/nested.f90` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/nested.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/posterior.f90` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/posterior.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/priors.f90` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/utils.f90` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/utils1.f90` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/utils1.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90` & `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/nautilus/nautilus_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/nautilus/nautilus_sampler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .. import ParallelSampler
 import numpy as np
-import sys
 import os
 
+
 def log_probability_function(p):
     r = pipeline.run_results(p)
     out = [r.like, r.prior]
 
     # Flatten any vector outputs here
     for e in r.extra:
         if np.isscalar(e):
@@ -20,29 +20,35 @@
 def prior_transform(p):
     return pipeline.denormalize_vector_from_prior(p)
 
 
 class NautilusSampler(ParallelSampler):
     parallel_output = False
     internal_resume = True
-    sampler_outputs = [ ('log_weight', float), ('prior', float), ("post", float)]
+    sampler_outputs = [('log_weight', float), ('prior', float),
+                       ("post", float)]
 
     def config(self):
         global pipeline
         pipeline = self.pipeline
 
         if self.is_master():
             self.n_live = self.read_ini("n_live", int, 1500)
             self.n_update = self.read_ini("n_update", int, self.n_live)
-            self.enlarge = self.read_ini(
-                "enlarge", float, 1.1**self.pipeline.nvaried)
+            self.enlarge_per_dim = self.read_ini("enlarge_per_dim", float, 1.1)
+            self.n_points_min = self.read_ini("n_points_min", int,
+                                              self.pipeline.nvaried + 50)
+            self.split_threshold = self.read_ini("split_threshold", float,
+                                                 100.0)
+            self.n_networks = self.read_ini("n_networks", int, 4)
+            self.n_jobs = self.read_ini("n_jobs", int, 1)
             self.n_batch = self.read_ini("n_batch", int, 100)
-            self.random_state = self.read_ini("random_state", int, -1)
-            if self.random_state < 0:
-                self.random_state = None
+            self.seed = self.read_ini("seed", int, -1)
+            if self.seed < 0:
+                self.seed = None
             self.resume_ = self.read_ini("resume", bool, False)
             self.f_live = self.read_ini("f_live", float, 0.01)
             self.n_shell = self.read_ini("n_shell", int, self.n_batch)
             self.n_eff = self.read_ini("n_eff", float, 10000.0)
             self.discard_exploration = self.read_ini(
                 "discard_exploration", bool, False)
             self.verbose = self.read_ini("verbose", bool, False)
@@ -66,17 +72,21 @@
 
         sampler = Sampler(
             prior_transform,
             log_probability_function,
             n_dim,
             n_live=self.n_live,
             n_update=self.n_update,
-            enlarge=self.enlarge,
+            enlarge_per_dim=self.enlarge_per_dim,
+            n_points_min=self.n_points_min,
+            split_threshold=self.split_threshold,
+            n_networks=self.n_networks,
+            n_jobs=self.n_jobs,
             n_batch=self.n_batch,
-            random_state=self.random_state,
+            seed=self.seed,
             filepath=resume_filepath,
             resume=self.resume_,
             pool=self.pool,
             blobs_dtype=float
         )
 
         sampler.run(f_live=self.f_live,
```

### Comparing `cosmosis-2.3.2/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/pmc/pmc.py` & `cosmosis-2.4.1/cosmosis/samplers/pmc/pmc.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/pmc/pmc_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/pmc/pmc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/poco/poco_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/poco/poco_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/LICENCE` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/Makefile` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/README` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/abort.F90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/abort.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/array_utils.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/c_interface.cpp` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/calculate.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/calculate.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/clustering.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/clustering.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/feedback.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/feedback.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/generate.F90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/generate.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/ini.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/ini.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/interfaces.F90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/interfaces.h` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/interfaces.hpp` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/params.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/params.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/priors.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/random_utils.F90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/read_write.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/read_write.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/run_time_info.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/settings.f90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/settings.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/polychord/polychord_src/utils.F90` & `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/pymc/pymc_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/pymc/pymc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/snake/snake.py` & `cosmosis-2.4.1/cosmosis/samplers/snake/snake.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/snake/snake_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/snake/snake_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/star/star_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/star/star_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/test/test_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/samplers/zeus/zeus_sampler.py` & `cosmosis-2.4.1/cosmosis/samplers/zeus/zeus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/Makefile` & `cosmosis-2.4.1/cosmosis/test/libtest/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_complex_array_test.c` & `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_double_array_test.c` & `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_int_array_test.c` & `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c` & `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c` & `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c` & `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/c_datablock_test.c` & `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/cosmosis_test.F90` & `cosmosis-2.4.1/cosmosis/test/libtest/cosmosis_test.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/datablock_test.cc` & `cosmosis-2.4.1/cosmosis/test/libtest/datablock_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/entry_test.cc` & `cosmosis-2.4.1/cosmosis/test/libtest/entry_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/ndarray_test.cc` & `cosmosis-2.4.1/cosmosis/test/libtest/ndarray_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/section_test.cc` & `cosmosis-2.4.1/cosmosis/test/libtest/section_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/test_c_datablock_scalars.h` & `cosmosis-2.4.1/cosmosis/test/libtest/test_c_datablock_scalars.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/libtest/test_c_datablock_scalars.template` & `cosmosis-2.4.1/cosmosis/test/libtest/test_c_datablock_scalars.template`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_block.py` & `cosmosis-2.4.1/cosmosis/test/test_block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_chaining.py` & `cosmosis-2.4.1/cosmosis/test/test_chaining.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_gaussian.py` & `cosmosis-2.4.1/cosmosis/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_lib.py` & `cosmosis-2.4.1/cosmosis/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_module2.py` & `cosmosis-2.4.1/cosmosis/test/test_module2.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_modules.py` & `cosmosis-2.4.1/cosmosis/test/test_modules.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_parameters.py` & `cosmosis-2.4.1/cosmosis/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_pipeline.py` & `cosmosis-2.4.1/cosmosis/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_polychord.py` & `cosmosis-2.4.1/cosmosis/test/test_polychord.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_samplers.py` & `cosmosis-2.4.1/cosmosis/test/test_samplers.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,17 @@
 
 def test_snake():
         run('snake', True)
 
 def test_nautilus():
     run('nautilus', True)
     run('nautilus', True, no_extra=True)
+    run('nautilus', True, no_extra=True, n_live=500, enlarge_per_dim=1.05,
+        split_threshold=95., n_networks=3, n_batch=50, verbose=True, f_live=0.02, n_shell=100)
+
 
 def test_star():
         run('star', False)
 
 def test_test():
     run('test', False, can_postprocess=False)
```

### Comparing `cosmosis-2.3.2/cosmosis/test/test_text_output.py` & `cosmosis-2.4.1/cosmosis/test/test_text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/test/test_utils.py` & `cosmosis-2.4.1/cosmosis/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis/utils.py` & `cosmosis-2.4.1/cosmosis/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/cosmosis.egg-info/SOURCES.txt` & `cosmosis-2.4.1/cosmosis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-2.3.2/setup.py` & `cosmosis-2.4.1/setup.py`

 * *Files identical despite different names*

